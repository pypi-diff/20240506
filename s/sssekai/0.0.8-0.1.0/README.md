# Comparing `tmp/sssekai-0.0.8.tar.gz` & `tmp/sssekai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssekai-0.0.8.tar", last modified: Sat Apr 27 08:13:05 2024, max compression
+gzip compressed data, was "sssekai-0.1.0.tar", last modified: Mon May  6 15:53:39 2024, max compression
```

## Comparing `sssekai-0.0.8.tar` & `sssekai-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-27 08:13:05.016878 sssekai-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-27 08:13:00.000000 sssekai-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:13:05.016878 sssekai-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 08:13:00.000000 sssekai-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/abcache/
--rw-r--r--   0 runner    (1001) docker     (127)    14490 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/abcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/crypto/APIManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/crypto/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/abcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/abdecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/apidecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/live2dextract.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/mitm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/mvdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/spineextract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/entrypoint/usmdemux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.012878 sssekai-0.0.8/sssekai/fmt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/fmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/fmt/moc3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/sssekai/unity/
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/AnimationClip.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/sssekai/unity/constant/
--rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/constant/SekaiLive2DPathNames.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:00.000000 sssekai-0.0.8/sssekai/unity/constant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:13:05.016878 sssekai-0.0.8/sssekai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 08:13:05.000000 sssekai-0.0.8/sssekai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-06 15:53:39.116844 sssekai-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-06 15:53:34.000000 sssekai-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:53:39.116844 sssekai-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-06 15:53:34.000000 sssekai-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.112844 sssekai-0.1.0/sssekai/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.112844 sssekai-0.1.0/sssekai/abcache/
+-rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/abcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/crypto/APIManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/crypto/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/abcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/abdecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/apidecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/live2dextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/mitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/mvdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/spineextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/usmdemux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/fmt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/fmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/fmt/moc3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/unity/
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/AnimationClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/unity/constant/
+-rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/constant/SekaiLive2DPathNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/constant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/top_level.txt
```

### Comparing `sssekai-0.0.8/setup.py` & `sssekai-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="sssekai",
     version=sssekai.__version__,
     author="greats3an",
     author_email="greats3an@gmail.com",
-    description="",
+    description="Project SEKAI Asset Utility / PJSK 资源下载 + Live2D, Spine, USM 提取",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mos9527/sssekai",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sssekai-0.0.8/sssekai/__main__.py` & `sssekai-0.1.0/sssekai/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sssekai.entrypoint.mitm import main_mitm
 from sssekai.entrypoint.mvdata import main_mvdata
 from sssekai.entrypoint.usmdemux import main_usmdemux
 from sssekai.entrypoint.abcache import main_abcache
 from sssekai.entrypoint.live2dextract import main_live2dextract
 from sssekai.entrypoint.spineextract import main_spineextract
 from sssekai.unity import SEKAI_UNITY_VERSION
-from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_LATEST_VERSION, DEFAULT_SEKAI_PLATFORM
+from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_APP_PLATFORM, DEFAULT_SEKAI_APP_VERSION, DEFAULT_SEKAI_APP_HASH, DEFAULT_SEKAI_AB_HASH, DEFAULT_SEKAI_AB_HOST_HASH
 def __main__():
     from tqdm.std import tqdm as tqdm_c
     class SemaphoreStdout:
         @staticmethod
         def write(__s):
             # Blocks tqdm's output until write on this stream is done
             # Solves cases where progress bars gets re-rendered when logs
@@ -51,16 +51,19 @@
     abcache_parser = subparsers.add_parser('abcache', help='''Sekai AssetBundle local cache
 Downloads/Updates *ALL* PJSK JP assets to local devices.
 NOTE: The assets can take quite a lot of space (est. 42.5GB for app version 3.3.1) so be prepared
 NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
       that supports stripped Unity version (should be %s. the version is ripped).''' % SEKAI_UNITY_VERSION)
     abcache_parser.add_argument('--cache-dir', type=str, help='cache directory (default: %(default)s)',default=DEFAULT_CACHE_DIR)
     abcache_parser.add_argument('--skip-update',action='store_true',help='skip all updates and use cached assets as is.')
-    abcache_parser.add_argument('--version', type=str, help='PJSK app version (default: %(default)s)', default=DEFAULT_SEKAI_LATEST_VERSION)
-    abcache_parser.add_argument('--platform', type=str, help='PJSK app platform (default: %(default)s)', default=DEFAULT_SEKAI_PLATFORM)
+    abcache_parser.add_argument('--version', type=str, help='PJSK app version (default: %(default)s)', default=DEFAULT_SEKAI_APP_VERSION)
+    abcache_parser.add_argument('--platform', type=str, help='PJSK app platform (default: %(default)s)', default=DEFAULT_SEKAI_APP_PLATFORM)
+    abcache_parser.add_argument('--appHash', type=str, help='PJSK app hash (default: %(default)s)', default=DEFAULT_SEKAI_APP_HASH)
+    abcache_parser.add_argument('--assetHash', type=str, help='PJSK asset hash (default: %(default)s)', default=DEFAULT_SEKAI_AB_HASH)
+    abcache_parser.add_argument('--assetHostHash', type=str, help='PJSK asset host hash (default: %(default)s)', default=DEFAULT_SEKAI_AB_HOST_HASH)
     abcache_parser.add_argument('--open', action='store_true',help='open cache directory. this will skip all updates.')
     abcache_parser.set_defaults(func=main_abcache)
     # live2dextract
     live2dextract_parser = subparsers.add_parser('live2dextract', help='''Extract Sekai Live2D Models in a AssetBundle''')
     live2dextract_parser.add_argument('infile', type=str, help='input file')
     live2dextract_parser.add_argument('outdir', type=str, help='output directory')
     live2dextract_parser.add_argument('--no-anim',action='store_true',help='don\'t extract animation clips')
```

### Comparing `sssekai-0.0.8/sssekai/abcache/__init__.py` & `sssekai-0.1.0/sssekai/abcache/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 logger = getLogger('sssekai.abcache')
 
 from sssekai.crypto.APIManager import decrypt
 from sssekai.crypto.AssetBundle import decrypt_headaer_inplace, SEKAI_AB_MAGIC
 from msgpack import unpackb, dump, load
 from tqdm import tqdm
 DEFAULT_CACHE_DIR = '~/.sssekai/abcache'
-DEFAULT_SEKAI_LATEST_VERSION = 'latest'
-DEFAULT_SEKAI_PLATFORM = 'android'
 DOWNLOADER_WORKER_COUNT = 8
-# TODO: These seems to be in pairs?
-DEFAULT_SEKAI_FALLBACK_VERSION = '3.4.1'
-DEFAULT_SEKAI_FALLBACK_APP_HASH = 'a3015fe8-785f-27e1-fb8b-546a23c82c1f'
-
 DEFAULT_FILESIZE_MATCH_RATIO = 1.5
-class SekaiAssetBundleThreadpoolDownloader(ThreadPoolExecutor):
-    session : Session
-    progress : tqdm
 
-    def download(self, url, fname, length):
+DEFAULT_SEKAI_APP_VERSION = '3.5.0'
+DEFAULT_SEKAI_APP_HASH = '5e9fea31-2613-bd13-1723-9fe15156bd66'
+DEFAULT_SEKAI_AB_HASH = '9a5e2be1-0502-24c6-389e-b79b6a24ec0b'
+DEFAULT_SEKAI_AB_HOST_HASH = 'cf2d2388'
+DEFAULT_SEKAI_APP_PLATFORM = 'android'
+
+class AbCacheDownloader(ThreadPoolExecutor):
+    session : Session
+    progress : tqdm = None
+    def _ensure_progress(self):
+        if not self.progress:
+            self.progress = tqdm(bar_format="{desc}: {percentage:.1f}%|{bar}| {n_fmt}/{total_fmt} {rate_fmt} {elapsed}<{remaining}", total=0,unit='B', unit_scale=True, unit_divisor=1024,desc="Downloading")
+    def _download(self, url, fname, length):
+        self._ensure_progress()
         RETRIES = 1
         for _ in range(0,RETRIES):
             try:
                 resp = self.session.get(url,stream=True)
                 resp.raise_for_status()
                 makedirs(path.dirname(fname),exist_ok=True)
                 with open(fname, 'wb') as f:
@@ -44,35 +48,31 @@
                         self.progress.update(len(chunk))
                         f.write(chunk)
                     return
             except Exception as e:
                 logger.error('While downloading %s : %s. Retrying' % (url,e))
         if _ == RETRIES - 1:
             logger.critical('Did not download %s' % url)
+        self._ensure_progress()
+    def __init__(self, session) -> None:
+        self.session = session        
+        super().__init__(max_workers=DOWNLOADER_WORKER_COUNT)
     def add_link(self, url, fname, length):
+        self._ensure_progress()
         self.progress.total += length
-        return self.submit(self.download, url, fname, length)
-    def __init__(self, session = None) -> None:
-        self.session = session or Session()
-        self.progress = tqdm(bar_format="{desc}: {percentage:.1f}%|{bar}| {n_fmt}/{total_fmt} {rate_fmt} {elapsed}<{remaining}", total=0,unit='B', unit_scale=True, unit_divisor=1024,desc="Downloading")
-        super().__init__(max_workers=DOWNLOADER_WORKER_COUNT)
+        return self.submit(self._download, url, fname, length)
 
+@dataclass
 class AbCacheConfig:
-    app_version : str
-    app_platform : str
-
     cache_dir : str # absolute path to cache directory
-    downloader : SekaiAssetBundleThreadpoolDownloader
-
-    def __init__(self, downloader : SekaiAssetBundleThreadpoolDownloader, cache_dir: str = DEFAULT_CACHE_DIR, version: str = DEFAULT_SEKAI_LATEST_VERSION, platform : str = DEFAULT_SEKAI_PLATFORM) -> None:
-        self.cache_dir = path.expanduser(cache_dir)
-        self.cache_dir = path.abspath(self.cache_dir)
-        self.downloader = downloader
-        self.app_version = version
-        self.app_platform = platform
+    app_version : str = None
+    app_platform : str = None
+    app_hash : str  = None
+    ab_hash : str = None
+    ab_host_hash : str  = None
 
 @dataclass
 class AbCacheEntry(dict):
     bundleName: str
     cacheFileName: str
     cacheDirectoryName: str
     hash: str
@@ -116,19 +116,20 @@
         relpath = fpath.relative_to(cpath).as_posix()
         return self.bundles.get(relpath,None)    
 @dataclass
 class SekaiAppVersion:
     systemProfile : str
     appVersion : str
     multiPlayVersion : str
-    dataVersion : str
-    assetVersion : str
-    appHash : str
-    assetHash : str
     appVersionStatus : str
+    assetVersion : str
+    # These are sadly removed from 3.5.0
+    _dataVersion : str = None 
+    _appHash : str = None 
+    _assetHash : str = None 
 @dataclass
 class SekaiSystemData:
     serverDate : int
     timezone : str
     profile : str
     maintenanceStatus : str
     appVersions : List[SekaiAppVersion]    
@@ -146,34 +147,31 @@
         return [av.appVersion for av in self.appVersions]
 @dataclass
 class SekaiGameVersionData:
     profile : str
     assetbundleHostHash : str
     domain : str
 class AbCache(Session):    
+    downloader : AbCacheDownloader
+
     config : AbCacheConfig
-    
     local_abcache_index : AbCacheIndex  = None
 
     sekai_abcache_index  : AbCacheIndex = None
     sekai_system_data : SekaiSystemData  = None
     sekai_gameversion_data : SekaiGameVersionData  = None
 
     @property
-    def SEKAI_APP_VERSION(self): 
-        if self.config.app_version == DEFAULT_SEKAI_LATEST_VERSION:
-            version = self.sekai_system_data.get_app_version_latest()
-        else:
-            version = self.sekai_system_data.get_app_version_by_app(self.config.app_version)
-        assert version, "Incorrect app version %s. Please choose from: %s" % (self.config.app_version, ', '.join(self.sekai_system_data.list_app_versions()))
-        return version
+    def SEKAI_APP_VERSION(self): return self.config.app_version
+    @property
+    def SEKAI_ASSET_VERSION(self): return self.sekai_system_data.get_app_version_by_app(self.SEKAI_APP_VERSION).assetVersion
     @property
-    def SEKAI_ASSET_VERSION(self): return self.SEKAI_APP_VERSION.assetVersion
+    def SEKAI_APP_HASH(self): return self.config.app_hash
     @property
-    def SEKAI_AB_HASH(self): return self.SEKAI_APP_VERSION.assetHash
+    def SEKAI_AB_HASH(self): return self.config.ab_hash
     @property
     def SEKAI_AB_HOST_HASH(self): return self.sekai_gameversion_data.assetbundleHostHash
     @property
     def SEKAI_API_ENDPOINT(self): return 'https://production-game-api.sekai.colorfulpalette.org'
     @property
     def SEKAI_API_SYSTEM_DATA(self): return self.SEKAI_API_ENDPOINT + '/api/system'
     @property
@@ -207,15 +205,15 @@
         data = unpackb(data)
         self.sekai_system_data = SekaiSystemData(**data)
         for i, appVersion in enumerate(self.sekai_system_data.appVersions):
             self.sekai_system_data.appVersions[i] = SekaiAppVersion(**appVersion)
 
     def update_gameversion_data(self):
         logger.info('Updating game version data')
-        resp = self.get(self.SEKAI_API_GAMEVERSION_ENDPOINT + '/' + self.SEKAI_APP_VERSION.appVersion + '/' + self.SEKAI_APP_VERSION.appHash)
+        resp = self.get(self.SEKAI_API_GAMEVERSION_ENDPOINT + '/' + self.SEKAI_APP_VERSION + '/' + self.SEKAI_APP_HASH)
         resp.raise_for_status()
         data = decrypt(resp.content)
         data = unpackb(data)
         self.sekai_gameversion_data = SekaiGameVersionData(**data)
     
     def update_abcache_index(self) -> AbCacheIndex:
         logger.info('Updating Assetbundle index')
@@ -234,15 +232,15 @@
 
     def query_entry(self, bundleName : str) -> AbCacheEntry | None:
         return self.local_abcache_index.bundles.get(bundleName, None)
 
     def queue_update_cache_entry(self, entry : AbCacheEntry, new_entry : AbCacheEntry = None):
         if new_entry:
             entry = new_entry
-        return self.config.downloader.add_link(
+        return self.downloader.add_link(
             self.SEKAI_AB_ENDPOINT + self.SEKAI_AB_BASE_PATH + entry.bundleName,
             entry.get_file_path(self.config),
             entry.fileSize
         )
 
     def queue_update_cache_entry_full(self):        
         all_keys = sorted(list({k for k in self.sekai_abcache_index.bundles.keys()}.union({k for k in self.local_abcache_index.bundles.keys()})))
@@ -267,52 +265,54 @@
                 logger.debug('Removing bundle %s', k)
                 if path.exists(self.local_abcache_index.bundles[k].get_file_path(self.config)):
                     remove(self.local_abcache_index.bundles[k].get_file_path(self.config))
                 del self.local_abcache_index.bundles[k]
         logger.debug('Saving AssetBundle index')
         self.save()
         logger.debug('Queued %d updates' % update_count)
+
+    def wait_for_downloads(self):       
+        self.downloader = AbCacheDownloader(self)
+
+    def cancel_downloads(self):
+        self.downloader.shutdown(wait=False, cancel_futures=True)
+        self.wait_for_downloads()
     
     def update_metadata(self):
         logger.info('Updating metadata')
         logger.debug('Cache directory: %s' % self.config.cache_dir)
-        logger.debug('Set App version: %s (%s)' % (self.config.app_version,self.config.app_platform))
+        logger.debug('Set App version: %s (%s), hash=%s' % (self.config.app_version,self.config.app_platform, self.SEKAI_APP_HASH))
         self.update_signatures()
         self.update_system_data()
         self.update_gameversion_data()               
         self.update_abcache_index()
-        # Update to the actually usable set version
-        self.config.app_version = self.SEKAI_APP_VERSION.appVersion
-        self.headers['X-App-Version'] = self.SEKAI_APP_VERSION.appVersion
-        self.headers['X-App-Hash'] = self.SEKAI_APP_VERSION.appHash
-        logger.debug('Actual App version: %s (%s), hash=%s' % (self.config.app_version,self.config.app_platform, self.SEKAI_APP_VERSION.appHash))
         logger.debug('Sekai AssetBundle version: %s' % self.SEKAI_ASSET_VERSION)
         logger.debug('Sekai AssetBundle host hash: %s' % self.SEKAI_AB_HOST_HASH)
 
     def __init__(self, config : AbCacheConfig) -> None:
         super().__init__()
         self.config = config
         self.headers.update({
             'Accept': 'application/octet-stream',
             'Content-Type': 'application/octet-stream',
             'Accept-Encoding': 'deflate, gzip',
             'User-Agent': 'UnityPlayer/2020.3.32f1 (UnityWebRequest/1.0, libcurl/7.80.0-DEV)',
             'X-Platform': self.config.app_platform,
             'X-Unity-Version': '2020.3.32f1',
-            'X-App-Version': DEFAULT_SEKAI_FALLBACK_VERSION, # These will be updated later
-            'X-App-Hash': DEFAULT_SEKAI_FALLBACK_APP_HASH
+            'X-App-Version': self.SEKAI_APP_VERSION,
+            'X-App-Hash': self.SEKAI_APP_HASH
         })
+        self.downloader = AbCacheDownloader(self)
         makedirs(self.config.cache_dir,exist_ok=True)
         try:
             self.load()
         except Exception as e:
             logger.warning('Failed to load cache index. Creating a new one. (%s)' % e)
             self.local_abcache_index = AbCacheIndex(bundles=dict())
             self.save()
-        
     
     def save(self):
         with open(path.join(self.config.cache_dir, 'abindex'),'wb') as f:
             dump(asdict(self.local_abcache_index), f)
             logger.info("Saved %d entries to cache index" % len(self.local_abcache_index.bundles))
 
     def load(self):
```

### Comparing `sssekai-0.0.8/sssekai/crypto/APIManager.py` & `sssekai-0.1.0/sssekai/crypto/APIManager.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai/crypto/AssetBundle.py` & `sssekai-0.1.0/sssekai/crypto/AssetBundle.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai/entrypoint/live2dextract.py` & `sssekai-0.1.0/sssekai/entrypoint/live2dextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai/entrypoint/mvdata.py` & `sssekai-0.1.0/sssekai/entrypoint/mvdata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from sssekai.unity.AssetBundle import load_assetbundle
-from sssekai.abcache import AbCache, AbCacheConfig,SekaiAssetBundleThreadpoolDownloader, logger, DEFAULT_CACHE_DIR
+from sssekai.abcache import AbCache, AbCacheConfig
+import os
 def main_mvdata(args):
     from UnityPy.enums import ClassIDType
     from pprint import pprint
-    cache_dir = args.cache_dir or DEFAULT_CACHE_DIR
-    config = AbCacheConfig(None, cache_dir)
+    cache_dir = args.cache_dir
+    cache_dir = os.path.expanduser(cache_dir)
+    cache_dir = os.path.abspath(cache_dir)
+    config = AbCacheConfig(cache_dir)
     cache = AbCache(config)
     mvdata_keys = filter(lambda x: x.startswith('live_pv/mv_data/'),cache.list_entry_keys())
     mvdata_items = list()
     mvdata_lut = dict()
     for key in mvdata_keys:
         entry = cache.query_entry(key)
         if entry.get_file_exists(config):
```

### Comparing `sssekai-0.0.8/sssekai/entrypoint/spineextract.py` & `sssekai-0.1.0/sssekai/entrypoint/spineextract.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import os
 from sssekai.unity.AssetBundle import load_assetbundle
+from UnityPy.enums import ClassIDType
 from logging import getLogger
 logger = getLogger(__name__)
 
 def main_spineextract(args):
     outdir = args.outdir
     with open(args.infile, "rb") as f:
         env = load_assetbundle(f)
         objects = [pobj.read() for pobj in env.objects]
-        objects = {obj.name: obj for obj in objects if hasattr(obj,'name')}
+        binaries = {obj.name: obj for obj in objects if getattr(obj,'type',None) in {ClassIDType.TextAsset}}
+        textures = {obj.name: obj for obj in objects if getattr(obj,'type',None) in {ClassIDType.Texture2D}}
         spines = set()
-        for name in objects:
+        for name in binaries:
             if name.endswith(".atlas") or name.endswith(".skel"):
                 spines.add(".".join(name.split(".")[:-1]))
         for spine in spines:
             logger.info('Extracting %s' % spine)
-            atlas = objects.get(spine + ".atlas", None)
-            skel = objects.get(spine + ".skel", None)
-            texture = objects.get(spine, None)
+            atlas = binaries.get(spine + ".atlas", None)
+            skel = binaries.get(spine + ".skel", None)
             os.makedirs(os.path.join(outdir, spine), exist_ok=True)
             if atlas:
+                logger.info('...has Atlas %s' % spine)
                 with open(os.path.join(outdir, spine, spine + ".atlas.txt"), "wb") as f:
                     f.write(atlas.script)
+                texfiles = [line.strip() for line in atlas.text.split("\n")]
+                texfiles = ['.'.join(line.split('.')[:-1]) for line in texfiles if (line.endswith(".png"))]
+                for tex in texfiles:
+                    logger.info('...has Texture %s' % tex)
+                    textureobj = textures.get(tex, None)
+                    if textureobj:
+                        textureobj.image.save(os.path.join(outdir, spine, tex + '.png'))
+                    else:
+                        logger.warning('No texture found for %s' % tex)
             else:
-                logger.warning("No atlas found for %s" % spine)
+                logger.warning("No atlas found for %s. Consequnetially, no textures cannot be exported either." % spine)
 
             if skel:
+                logger.info('...has Skeleton %s' % spine)
                 with open(os.path.join(outdir, spine, spine + ".skel.bytes"), "wb") as f:
                     f.write(skel.script)
             else:
                 logger.warning("No skel found for %s" % spine)
-
-            if texture:            
-                with open(os.path.join(outdir, spine, spine + ".png"), "wb") as f:
-                    texture.image.save(f)
-            else:
-                logger.warning("No texture found for %s" % spine)
```

### Comparing `sssekai-0.0.8/sssekai/entrypoint/usmdemux.py` & `sssekai-0.1.0/sssekai/entrypoint/usmdemux.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai/fmt/moc3.py` & `sssekai-0.1.0/sssekai/fmt/moc3.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai/unity/AnimationClip.py` & `sssekai-0.1.0/sssekai/unity/AnimationClip.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai/unity/constant/SekaiLive2DPathNames.py` & `sssekai-0.1.0/sssekai/unity/constant/SekaiLive2DPathNames.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.0.8/sssekai.egg-info/SOURCES.txt` & `sssekai-0.1.0/sssekai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

