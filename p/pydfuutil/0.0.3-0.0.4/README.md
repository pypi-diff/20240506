# Comparing `tmp/pydfuutil-0.0.3.tar.gz` & `tmp/pydfuutil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydfuutil-0.0.3.tar", last modified: Mon May  6 09:58:21 2024, max compression
+gzip compressed data, was "pydfuutil-0.0.4.tar", last modified: Mon May  6 14:46:55 2024, max compression
```

## Comparing `pydfuutil-0.0.3.tar` & `pydfuutil-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.226199 pydfuutil-0.0.3/pydfuutil/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35908 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19557 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/portable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/usb_dfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/pydfuutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_quirks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:46:55.818327 pydfuutil-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 14:46:55.818327 pydfuutil-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:46:55.814327 pydfuutil-0.0.4/pydfuutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35935 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19557 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pydfuutil/usb_dfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:46:55.818327 pydfuutil-0.0.4/pydfuutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 14:46:55.000000 pydfuutil-0.0.4/pydfuutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 14:46:55.000000 pydfuutil-0.0.4/pydfuutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:46:55.000000 pydfuutil-0.0.4/pydfuutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 14:46:55.000000 pydfuutil-0.0.4/pydfuutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 14:46:55.000000 pydfuutil-0.0.4/pydfuutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 14:46:55.000000 pydfuutil-0.0.4/pydfuutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:46:55.818327 pydfuutil-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:46:55.818327 pydfuutil-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 14:46:45.000000 pydfuutil-0.0.4/tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.3/LICENSE` & `pydfuutil-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/PKG-INFO` & `pydfuutil-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pydfuutil-0.0.3/README.md` & `pydfuutil-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/__main__.py` & `pydfuutil-0.0.4/pydfuutil/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     #                 force           You really know what you are doing!
     #                 <length>        Length of firmware to upload from device
     #
     parser.add_argument("-y", "--yes-to-all", action="store_true",
                         help="Say yes to all prompts")
 
 
-def main() -> None:
+def _main() -> None:
     """Cli entry point"""
 
     # Create argument parser
     parser = argparse.ArgumentParser(
         prog="pydfuutil",
         description="Python implementation of DFU-Util tools"
     )
@@ -1010,18 +1010,22 @@
             logger.error("error resetting after download")
             logger.debug(e)
 
     usb.util.release_interface(dif.dev, dif.interface)
     usb.util.dispose_resources(dif.dev)
 
 
-if __name__ == '__main__':
+def main():
     try:
-        main()
+        _main()
     except GeneralError as err:
         if err.__str__():
             logger.error(err)
         sys.exit(err.exit_code)
     except Exception as err:
         logger.error(err)
         sys.exit(1)
     sys.exit(0)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `pydfuutil-0.0.3/pydfuutil/dfu.py` & `pydfuutil-0.0.4/pydfuutil/dfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/dfu_file.py` & `pydfuutil-0.0.4/pydfuutil/dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/dfu_load.py` & `pydfuutil-0.0.4/pydfuutil/dfu_load.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/dfuse.py` & `pydfuutil-0.0.4/pydfuutil/dfuse.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/dfuse_mem.py` & `pydfuutil-0.0.4/pydfuutil/dfuse_mem.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/exceptions.py` & `pydfuutil-0.0.4/pydfuutil/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/lmdfu.py` & `pydfuutil-0.0.4/pydfuutil/lmdfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/progress.py` & `pydfuutil-0.0.4/pydfuutil/progress.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/quirks.py` & `pydfuutil-0.0.4/pydfuutil/quirks.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil/suffix.py` & `pydfuutil-0.0.4/pydfuutil/suffix.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                         type=lambda x: int(x, 16), help='Add device ID into DFU suffix in <file>')
     parser.add_argument('-s', '--stellaris-address', dest='lmdfu_flash_address',
                         metavar="<address>", type=int, help='Specify lmdfu address for LMDFU_ADD')
     parser.add_argument('-T', '--stellaris', dest='lmdfu_mode', action='store_const',
                         const=LmdfuMode.CHECK, help='Set lmdfu mode to LMDFU_CHECK')
 
 
-def main() -> None:
+def _main() -> None:
     """cli entry point for suffix"""
 
     parser = argparse.ArgumentParser(
         prog='pydfuutil-suffix',
         exit_on_error=False,
     )
     add_cli_options(parser)
@@ -210,21 +210,25 @@
             if lmdfu_mode == LmdfuMode.DEL and lmdfu.check_prefix(file):
                 lmdfu.remove_prefix(file)
 
         except Exception as error:
             raise GeneralError(error)
 
 
-if __name__ == '__main__':
+def main():
     try:
         main()
     except GeneralWarning as warn:
         if warn.__str__():
             _logger.warning(warn)
     except GeneralError as err:
         if err.__str__():
             _logger.error(err)
         sys.exit(err.exit_code)
     except Exception as err:
         logger.error(err)
         sys.exit(1)
     sys.exit(0)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `pydfuutil-0.0.3/pydfuutil/usb_dfu.py` & `pydfuutil-0.0.4/pydfuutil/usb_dfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pydfuutil.egg-info/PKG-INFO` & `pydfuutil-0.0.4/pydfuutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pydfuutil-0.0.3/pydfuutil.egg-info/SOURCES.txt` & `pydfuutil-0.0.4/pydfuutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/pyproject.toml` & `pydfuutil-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydfuutil"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
 ]
 description = "PyDfuUtil - Pure python fork of dfu-util wrappers to libusb"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["dfu_util", "dfu-util", "pydfu", "libusb", "python", "python3"]
```

### Comparing `pydfuutil-0.0.3/tests/test_dfu.py` & `pydfuutil-0.0.4/tests/test_dfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_dfu_file.py` & `pydfuutil-0.0.4/tests/test_dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_dfu_load.py` & `pydfuutil-0.0.4/tests/test_dfu_load.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_dfuse.py` & `pydfuutil-0.0.4/tests/test_dfuse.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_dfuse_mem.py` & `pydfuutil-0.0.4/tests/test_dfuse_mem.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_lmdfu.py` & `pydfuutil-0.0.4/tests/test_lmdfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_main.py` & `pydfuutil-0.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_progress.py` & `pydfuutil-0.0.4/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.3/tests/test_quirks.py` & `pydfuutil-0.0.4/tests/test_quirks.py`

 * *Files identical despite different names*

