# Comparing `tmp/py2saber-0.13.1.tar.gz` & `tmp/py2saber-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.13.1.tar", last modified: Fri May  3 19:00:28 2024, max compression
+gzip compressed data, was "py2saber-0.14.tar", last modified: Mon May  6 20:03:34 2024, max compression
```

## Comparing `py2saber-0.13.1.tar` & `py2saber-0.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-03 19:00:28.987971 py2saber-0.13.1/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.13.1/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-03 19:00:28.987804 py2saber-0.13.1/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.13.1/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-03 19:00:28.987602 py2saber-0.13.1/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-03 19:00:28.000000 py2saber-0.13.1/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-03 19:00:28.000000 py2saber-0.13.1/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-03 19:00:28.000000 py2saber-0.13.1/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-03 19:00:28.000000 py2saber-0.13.1/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-03 19:00:28.000000 py2saber-0.13.1/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-03 19:00:28.000000 py2saber-0.13.1/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    28619 2024-05-03 19:00:21.000000 py2saber-0.13.1/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-03 19:00:14.000000 py2saber-0.13.1/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-03 19:00:28.988003 py2saber-0.13.1/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-06 20:03:34.487074 py2saber-0.14/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.14/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)    43209 2024-05-06 20:03:34.486898 py2saber-0.14/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.14/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-06 20:03:34.486679 py2saber-0.14/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43209 2024-05-06 20:03:34.000000 py2saber-0.14/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-06 20:03:34.000000 py2saber-0.14/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-06 20:03:34.000000 py2saber-0.14/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-06 20:03:34.000000 py2saber-0.14/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-06 20:03:34.000000 py2saber-0.14/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-06 20:03:34.000000 py2saber-0.14/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)    29950 2024-05-06 20:00:34.000000 py2saber-0.14/py2saber.py
+-rw-r--r--   0 jramboz    (501) staff       (20)      791 2024-05-06 19:22:42.000000 py2saber-0.14/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-06 20:03:34.487106 py2saber-0.14/setup.cfg
```

### Comparing `py2saber-0.13.1/COPYING` & `py2saber-0.14/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.13.1/PKG-INFO` & `py2saber-0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.13.1
+Version: 0.14
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.13.1/README.md` & `py2saber-0.14/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.13.1/py2saber.egg-info/PKG-INFO` & `py2saber-0.14/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.13.1
+Version: 0.14
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.13.1/py2saber.py` & `py2saber-0.14/py2saber.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import sys
 import argparse
 import errno
 from getch import pause_exit
 import glob
 import time
 
-script_version = '0.13.1'
+script_version = '0.14'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
@@ -66,14 +66,16 @@
                         'stopbits': 1, 
                         'xonxoff': False, 
                         'dsrdtr': False, 
                         'rtscts': False, 
                         'timeout': 3, 
                         'write_timeout': None, 
                         'inter_byte_timeout': None}
+    
+    _CHUNK_SIZE = 130   # NXTs run into buffer problems if you try to send more than 130 bytes at a time
 
     def __init__(self, port: str=None, gui: bool = False, loglevel: int = logging.ERROR) -> None:
         self.log = logging.getLogger('Saber_Controller')
         self.log.setLevel(loglevel)
         self.log.info('Initializing saber connection.')
         self.gui = gui # Flag for whether to output signals for PySide GUI
         self.port = port
@@ -204,28 +206,37 @@
 
     def send_command(self, cmd: bytes) -> None:
         '''Send command string to attached saber. It will automatically add b'\n' terminator if not already present.
         
         Note: this method does not check that the saber is write-ready.'''
         if not cmd.endswith(b'\n'):
             cmd += b'\n'
-        self.log.debug(f'Sending command to saber: {cmd}')
-        self._ser.write(cmd)
+        if len(cmd) <= self._CHUNK_SIZE: # Send the whole thing at once
+            self.log.debug(f'Sending command to saber: {cmd}')
+            self._ser.write(cmd)
+        else: # send in chunks
+            self.log.debug(f'Sending command in chunks of {self._CHUNK_SIZE} bytes')
+            pos = 0
+            while pos < len(cmd):
+                self.log.debug(f'Sending command to saber: {cmd[pos:pos+self._CHUNK_SIZE]}')
+                self._ser.write(cmd[pos:pos+self._CHUNK_SIZE])
+                pos += self._CHUNK_SIZE
+                time.sleep(0.5)
     
     def read_line(self) -> bytes:
         '''Reads the next line (terminated by b'\n') from the serial buffer.
         
         Note: this removes the line from the buffer.'''
         response = self._ser.readline()
         self.log.debug(f'Received response: {response}')
         # Sometimes it seems the read request comes too fast, before the anima has had a chance to respond.
         # So now, if I get a blank response, I wait and try again until a response is received or timeout.
         if not response:
             tries = 1
-            max_tries = 5
+            max_tries = 3
             while not response and tries < max_tries:
                 time.sleep(0.5)
                 response = self._ser.readline()
                 self.log.debug(f'Received response: {response}')
                 tries += 1
         return response
 
@@ -518,14 +529,17 @@
 def error_handler(e: DocDefaultException):
     '''Print an exception to the log.'''
     log = logging.getLogger()
     log.debug(e, exc_info=True)
 
 def main_func():
     log = logging.getLogger()
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setFormatter(logging.Formatter('%(levelname)s: %(message)s'))
+    log.addHandler(handler)
 
     exit_code = 0
 
     # configure command line parser and options
     parser = argparse.ArgumentParser(prog='py2saber',
                                      description='A utility for working with OpenCore-based sabers, based on "sendtosaber" by Nuntis')
     parser.add_argument('-v', '--version',
@@ -555,14 +569,17 @@
                         help='Show debugging information')
     parser.add_argument('--erase-all', 
                         action="store_true",
                         help='erase all files on saber')
     parser.add_argument('--config',
                         action="store_true",
                         help='Display config.ini from saber')
+    parser.add_argument('-t', '--command',
+                        action='store', dest='cmd',
+                        help='send literal command CMD to saber (NOTE: only use if you know what you are doing!)')
     
     args = parser.parse_args(args=None if sys.argv[1:] else ['--help'])
 
     if args.debug:
         log.setLevel(logging.DEBUG)
 
     # Find port that Anima is connected to
@@ -584,14 +601,24 @@
         
         if args.config:
             print('\nRetrieving config.ini from saber')
             config = sc.read_config_ini()
             print('Config.ini:\n')
             print(config)
 
+        if args.cmd:
+            print(f'\nSending command to saber: {args.cmd}')
+            sc.send_command(args.cmd.encode('utf-8'))
+            response = sc.read_line().strip().decode('utf-8')
+            print("Received response: ")
+            while response:
+                print(response)
+                response = sc.read_line().strip().decode('utf-8')
+            return
+
         if args.erase_all: # erase all files on saber
             print('\n*** This will erase ALL files on the saber! ***')
             yorn = input('Do you want to continue? (Y/N): ')
             if yorn.lower() == 'y' or yorn.lower() == 'yes':
                 # do the thing
                 print('Erasing all files on saber. This may take several minutes.')
                 sc.erase_all_files()
```

### Comparing `py2saber-0.13.1/pyproject.toml` & `py2saber-0.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.13.1"
+version = "0.14"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

