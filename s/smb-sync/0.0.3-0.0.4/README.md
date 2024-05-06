# Comparing `tmp/smb_sync-0.0.3.tar.gz` & `tmp/smb_sync-0.0.4.tar.gz`

## Comparing `smb_sync-0.0.3.tar` & `smb_sync-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/__main__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/cli.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/file_base.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/file_factory.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/file_local.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 smb_sync-0.0.3/smb_sync/file_samba.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 smb_sync-0.0.3/.gitignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 smb_sync-0.0.3/README.md
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 smb_sync-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 smb_sync-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/__main__.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/cli.py
+-rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_base.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_factory.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_local.py
+-rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_samba.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 smb_sync-0.0.4/.gitignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 smb_sync-0.0.4/README.md
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 smb_sync-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 smb_sync-0.0.4/PKG-INFO
```

### Comparing `smb_sync-0.0.3/smb_sync/cli.py` & `smb_sync-0.0.4/smb_sync/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+"""
+smb_sync.cli
+"""
+
 import logging
+import sys
 
 from argparse import ArgumentParser, BooleanOptionalAction
 from smb_sync.file_base import FileSyncOptions
-from smb_sync.file_factory import CreateFileContextManager
+from smb_sync.file_factory import create_file_context_manager
 
 
 def setup_logger():
+    """
+    Setup logger.
+    """
     # Create a formatter to specify the log message format
     formatter = logging.Formatter("[%(levelname)s] %(name)s - %(message)s")
 
     # Create a StreamHandler to log messages to stdout
     console_handler = logging.StreamHandler()
 
     # Set the logging level for the console handler (DEBUG, INFO, WARNING, ERROR, CRITICAL)
@@ -17,42 +25,58 @@
 
     # Set the formatter for the console handler
     console_handler.setFormatter(formatter)
 
     # Set the logging level for the root logger (DEBUG, INFO, WARNING, ERROR, CRITICAL)
     logging.basicConfig(level=logging.INFO, handlers=[console_handler])
 
+    # Only show error logs from pysmb.
+    logging.getLogger("SMB.SMBConnection").setLevel(logging.ERROR)
+
 
 def arg_parser():
+    """
+    Build argument parser.
+    """
     parser = ArgumentParser(
         prog="smb-sync",
         description="A tool for copying files between local drive and smb network drive",
     )
 
     parser.add_argument("source", help="source file or directory")
     parser.add_argument("target", help="target file or directory")
 
     parser.add_argument(
         "--auto-delete",
         action=BooleanOptionalAction,
-        help="delete target files if they are removed in the source folder",
+        help="automatically delete extraneous files from target directories",
         default=False,
     )
 
     return parser
 
 
 def main():
+    """
+    Main.
+    """
     setup_logger()
 
     parser = arg_parser()
     args = parser.parse_args()
 
-    if args.source == None and args.target == None:
+    if args.source is None and args.target is None:
         parser.print_usage()
         return
 
-    with CreateFileContextManager(args.source) as source_fcm:
-        with CreateFileContextManager(args.target) as target_fcm:
-            source_fcm.Entry().SyncTo(
-                target_fcm.Entry(), FileSyncOptions(auto_delete=args.auto_delete)
+    with create_file_context_manager(args.source) as source_fcm:
+        source_entry = source_fcm.entry()
+        # We should quit immediately if source entry does not exist.
+        if not source_entry.exists():
+            logging.getLogger("smb_sync").fatal(
+                "Source `%s` does not exist.", source_entry.url()
+            )
+            sys.exit(1)
+        with create_file_context_manager(args.target) as target_fcm:
+            source_entry.sync_to(
+                target_fcm.entry(), FileSyncOptions(auto_delete=args.auto_delete)
             )
```

### Comparing `smb_sync-0.0.3/smb_sync/file_base.py` & `smb_sync-0.0.4/smb_sync/file_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,246 @@
+"""
+smb_sync.file_base
+"""
+
 from abc import ABC, abstractmethod
-from diskcache import Cache
 from hashlib import sha1
 from logging import getLogger
-from os.path import basename, expanduser, join
+from os.path import basename, expanduser
 from typing import IO, Self
+from diskcache import Cache
 
 
-def _GetCache():
+def _get_cache():
     return Cache(directory=expanduser("~/.cache/smb_sync"))
 
 
 class FileSyncOptions:
+    """
+    File sync options.
+    """
+
     # Delete target files which do not exist in the source folder.
-    auto_delete: bool
+    _auto_delete: bool
 
     def __init__(self, auto_delete=False):
-        self.auto_delete = auto_delete
+        self._auto_delete = auto_delete
+
+    def auto_delete(self) -> bool:
+        """
+        Returns should we auto delete files.
+        """
+        return self._auto_delete
 
 
 class FileBase(ABC):
+    """
+    File base.
+    """
+
     logger = getLogger("smb_sync")
 
     @abstractmethod
-    def Path(self) -> str:
-        pass
+    def path(self) -> str:
+        """
+        Returns the path of current file.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Url(self) -> str:
-        pass
+    def url(self) -> str:
+        """
+        Returns the URL of current file.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Resolve(self, path: str) -> Self:
-        pass
+    def resolve(self, path: str) -> Self:
+        """
+        Returns resolved file by given path.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Exists(self) -> bool:
-        pass
+    def parent(self) -> Self:
+        """
+        Returns parent directory by given path.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def IsDirectory(self) -> bool:
-        pass
+    def exists(self) -> bool:
+        """
+        Returns if the file exists or not.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def MakeDirectory(self) -> Self:
-        pass
+    def is_directory(self) -> bool:
+        """
+        Returns if the file is directory.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def LastWriteTimestamp(self) -> float:
-        pass
+    def make_directory(self) -> Self:
+        """
+        Makes it directory.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def FileSizeInBytes(self) -> int:
-        pass
+    def last_write_timestamp(self) -> float:
+        """
+        Returns last write timestamp.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Children(self) -> set[Self]:
-        pass
+    def file_size_in_bytes(self) -> int:
+        """
+        Returns file size in bytes.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Read(self) -> IO[bytes]:
-        pass
+    def children(self) -> set[Self]:
+        """
+        Returns chilren of current file.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Write(self, content: IO[bytes]) -> Self:
-        pass
+    def read(self) -> IO[bytes]:
+        """
+        Returns bytes of current file.
+        """
+        raise NotImplementedError()
 
     @abstractmethod
-    def Remove(self) -> Self:
-        pass
+    def write(self, content: IO[bytes]) -> Self:
+        """
+        Writes bytes into current file.
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
+    def remove(self) -> Self:
+        """
+        Removes current file.
+        """
+        raise NotImplementedError()
 
-    def Checksum(self) -> str | None:
-        cache_key = f"check_sum:{self.Url()}:{self.LastWriteTimestamp()}"
+    def checksum(self) -> str | None:
+        """
+        Returns checksum of current file.
+        """
+        cache_key = f"check_sum:{self.url()}:{self.last_write_timestamp()}"
 
         # Try to re-use cached check sum if it exists.
-        with _GetCache() as cache:
+        with _get_cache() as cache:
             cached_checksum = cache.get(cache_key)
             if cached_checksum:
                 self.logger.debug(
-                    f"Re-using cached checksum: {cached_checksum} for {self.Url()}"
+                    "Re-using cached checksum: %s for %s",
+                    str(cached_checksum),
+                    self.url(),
                 )
                 return str(cached_checksum)
 
         # Compute checksum (algorithm: SHA1).
-        hash = sha1()
-        with self.Read() as content:
+        hash_val = sha1()
+        with self.read() as content:
             while True:
                 block = content.read(65536)
                 if not block:
                     break
-                hash.update(block)
-        checksum = hash.hexdigest()
+                hash_val.update(block)
+        checksum = hash_val.hexdigest()
 
-        self.logger.debug(f"Computed checksum: {checksum} for {self.Url()}")
+        self.logger.debug("Computed checksum: %s for %s", checksum, self.url())
 
         # Save cached checksum.
-        with _GetCache() as cache:
+        with _get_cache() as cache:
             cache.set(cache_key, checksum)
 
         return checksum
 
-    def SyncTo(self, target: Self, options: FileSyncOptions) -> Self:
-        self.logger.info(f"Checking {target.Path()}")
+    def sync_to(self, target: Self, options: FileSyncOptions) -> Self:
+        """
+        Syncs current file to given target file.
+        """
+        self.logger.info("Checking %s", target.url())
 
-        if not self.Exists():
+        if not self.exists():
             # Remove target if it exists.
-            if target.Exists():
-                self.logger.info(f"Removing {target.Path()}")
-                target.Remove()
+            if target.exists() and options.auto_delete():
+                self.logger.info("Removing %s", target.url())
+                target.remove()
 
-        elif self.IsDirectory():
+        elif self.is_directory():
             # Remove target if target is not directory.
-            if target.Exists() and not target.IsDirectory():
-                target.Remove()
+            if target.exists() and not target.is_directory():
+                self.logger.info("Removing %s", target.url())
+                target.remove()
 
             # Creates directory target if it does not exist.
-            if not target.Exists():
-                self.logger.info(f"Creating directory {target.Path()}")
-                target.MakeDirectory()
+            if not target.exists():
+                self.logger.info("Creating directory %s", target.url())
+                target.make_directory()
 
-            self_children = {basename(c.Path()): c for c in self.Children()}
-            target_children = {basename(c.Path()): c for c in target.Children()}
+            self_children = {basename(c.path()): c for c in self.children()}
+            target_children = {basename(c.path()): c for c in target.children()}
 
             # Recursively sync self children.
             for name, self_child in self_children.items():
-                self_child.SyncTo(target=target.Resolve(name), options=options)
+                self_child.sync_to(target=target.resolve(name), options=options)
 
-            if options.auto_delete:
+            if options.auto_delete():
                 # Remove target child if there is no equivalent child in self.
                 for name, target_child in target_children.items():
                     if name not in self_children:
-                        self.logger.info(f"Removing {target_child.Path()}")
-                        target_child.Remove()
+                        self.logger.info("Removing %s", target_child.url())
+                        target_child.remove()
 
         else:
             # Remove target if target is a directory.
-            if target.Exists() and target.IsDirectory():
-                self.logger.info(f"Removing {target.Path()}")
-                target.Remove()
+            if target.exists() and target.is_directory():
+                self.logger.info("Removing %s", target.url())
+                target.remove()
+
+            # Check if target file's parent directory exists.
+            target_parent = target.parent()
+            if not target_parent.exists():
+                target_parent.make_directory()
 
             # If src and target are at same size, we assume they are same.
             # Otherwise we override the content.
             if (
-                not target.Exists()
-                or target.FileSizeInBytes() != self.FileSizeInBytes()
-                or target.Checksum() != self.Checksum()
+                not target.exists()
+                or target.file_size_in_bytes() != self.file_size_in_bytes()
+                or target.checksum() != self.checksum()
             ):
-                self.logger.info(f"Writing {target.Path()}")
-                with self.Read() as self_content:
-                    target.Write(self_content)
+                self.logger.info("Writing %s", target.url())
+                with self.read() as self_content:
+                    target.write(self_content)
 
         return self
 
 
 class FileContextManager(ABC):
+    """
+    File context manager.
+    """
+
     def __enter__(self):
         return self
 
     def __exit__(self, exec_type, exec_value, traceback):
         pass
 
     @abstractmethod
-    def Entry(self) -> FileBase:
-        pass
+    def entry(self) -> FileBase:
+        """
+        Returns the entry file.
+        """
+        raise NotImplementedError()
```

### Comparing `smb_sync-0.0.3/smb_sync/file_samba.py` & `smb_sync-0.0.4/smb_sync/file_samba.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,130 @@
+"""
+smb_sync.file_samba
+"""
+
 from io import BytesIO
-from os.path import join
+from os.path import dirname, join
+from typing import IO, Self
 from smb.base import OperationFailure, SharedFile
 from smb.SMBConnection import SMBConnection
-from typing import IO, Self
 
 from .file_base import FileBase, FileContextManager
 
 
 class FileSamba(FileBase):
+    """
+    File samba.
+    """
+
     _base_url: str
     _name: str
     _path: str
     _conn: SMBConnection
 
     def __init__(self, base_url: str, name: str, path: str, conn: SMBConnection):
         self._base_url = base_url
         self._name = name
         self._path = path
         self._conn = conn
 
-    def Path(self) -> str:
+    def stat(self) -> SharedFile | None:
+        """
+        Returns samba file state.
+        """
+        try:
+            return self._conn.getAttributes(self._name, self.path())
+        except OperationFailure:
+            return None
+
+    def path(self) -> str:
         return self._path
 
-    def Url(self) -> str:
-        return f"{self._base_url}/{self.Path()}"
+    def url(self) -> str:
+        return f"{self._base_url}/{self.path()}"
 
-    def Resolve(self, path: str) -> Self:
+    def resolve(self, path: str) -> Self:
         return FileSamba(
-            self._base_url, self._name, join(self.Path(), path), self._conn
+            self._base_url, self._name, join(self.path(), path), self._conn
         )
 
-    def _Stat(self) -> SharedFile | None:
-        try:
-            return self._conn.getAttributes(self._name, self.Path())
-        except OperationFailure:
-            return None
+    def parent(self) -> Self:
+        return FileSamba(self._base_url, self._name, dirname(self.path()), self._conn)
 
-    def Exists(self) -> bool:
-        return self._Stat() != None
+    def exists(self) -> bool:
+        return self.stat() is not None
 
-    def IsDirectory(self) -> bool:
-        stat = self._Stat()
-        return stat != None and stat.isDirectory
+    def is_directory(self) -> bool:
+        stat = self.stat()
+        return stat is not None and stat.isDirectory
 
-    def MakeDirectory(self) -> Self:
+    def make_directory(self) -> Self:
         current_path = ""
-        for directory in self.Path().strip("/").split("/"):
+        for directory in self.path().strip("/").split("/"):
             current_path = join(current_path, directory)
             current_file = FileSamba(
                 base_url=self._base_url,
                 name=self._name,
                 path=current_path,
                 conn=self._conn,
             )
 
-            attr: None | SharedFile = current_file._Stat()
+            attr: None | SharedFile = current_file.stat()
 
-            if attr == None:
+            if attr is None:
                 self._conn.createDirectory(self._name, current_path)
             elif not attr.isDirectory:
                 raise Exception(f"Cannot create directory: {current_path}")
 
         return self
 
-    def LastWriteTimestamp(self) -> float:
-        stat = self._Stat()
-        if stat == None:
+    def last_write_timestamp(self) -> float:
+        stat = self.stat()
+        if stat is None:
             raise Exception(f"File / directory {self.Path()} does not exist")
         return stat.last_write_time
 
-    def FileSizeInBytes(self) -> int:
-        stat = self._Stat()
-        if stat == None:
+    def file_size_in_bytes(self) -> int:
+        stat = self.stat()
+        if stat is None:
             raise Exception(f"File / directory {self.Path()} does not exist")
         return stat.file_size
 
-    def Children(self) -> set[Self]:
-        files: list[SharedFile] = self._conn.listPath(self._name, self.Path())
+    def children(self) -> set[Self]:
+        files: list[SharedFile] = self._conn.listPath(self._name, self.path())
         files = [f for f in files if not f.filename in [".", ".."]]
-        return set([self.Resolve(file.filename) for file in files])
+        return set([self.resolve(file.filename) for file in files])
 
-    def Read(self) -> IO[bytes]:
+    def read(self) -> IO[bytes]:
         content = BytesIO()
-        self._conn.retrieveFile(self._name, self.Path(), content)
+        self._conn.retrieveFile(self._name, self.path(), content)
         content.seek(0)
         return content
 
-    def Write(self, content: IO[bytes]) -> Self:
-        self._conn.storeFile(self._name, self.Path(), content)
+    def write(self, content: IO[bytes]) -> Self:
+        self._conn.storeFile(self._name, self.path(), content)
         return self
 
-    def Remove(self) -> Self:
-        stat = self._Stat()
-        if stat != None:
+    def remove(self) -> Self:
+        stat = self.stat()
+        if stat is not None:
             if stat.isDirectory:
-                for c in self.Children():
-                    c.Remove()
-                self._conn.deleteDirectory(self._name, self.Path())
+                for c in self.children():
+                    c.remove()
+                self._conn.deleteDirectory(self._name, self.path())
             else:
-                self._conn.deleteFiles(self._name, self.Path())
+                self._conn.deleteFiles(self._name, self.path())
         return self
 
 
 class FileContextManagerSamba(FileContextManager):
+    """
+    File context manager samba.
+    """
+
     _username: str
     _password: str
     _name: str
     _path: str
     _host: str
     _port: int
     _conn: SMBConnection
@@ -127,33 +145,51 @@
             remote_name=name,
             use_ntlm_v2=True,
             is_direct_tcp=True,
         )
 
     def __enter__(self):
         if not self._conn.connect(ip=self._host, port=self._port):
-            raise Exception(f"Cannot connect to {self.BaseUrl()}")
+            raise Exception(f"Cannot connect to {self.base_url()}")
         return self
 
     def __exit__(self, exec_type, exec_value, traceback):
         self._conn.close()
 
-    def Username(self) -> str:
+    def username(self) -> str:
+        """
+        Returns username.
+        """
         return self._username
 
-    def Password(self) -> str:
+    def password(self) -> str:
+        """
+        Returns password.
+        """
         return self._password
 
-    def Name(self) -> str:
+    def name(self) -> str:
+        """
+        Returns name.
+        """
         return self._name
 
-    def Host(self) -> str:
+    def host(self) -> str:
+        """
+        Returns host.
+        """
         return self._host
 
-    def Port(self) -> int:
+    def port(self) -> int:
+        """
+        Returns port.
+        """
         return self._port
 
-    def BaseUrl(self) -> str:
-        return f"smb://{self.Host()}:{self.Port()}/{self.Name()}"
+    def base_url(self) -> str:
+        """
+        Returns base URL.
+        """
+        return f"smb://{self.host()}:{self.port()}/{self.name()}"
 
-    def Entry(self) -> FileBase:
-        return FileSamba(self.BaseUrl(), self._name, self._path, self._conn)
+    def entry(self) -> FileBase:
+        return FileSamba(self.base_url(), self._name, self._path, self._conn)
```

