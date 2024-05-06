# Comparing `tmp/gendazpack-0.1.1.tar.gz` & `tmp/gendazpack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gendazpack-0.1.1.tar", max compression
+gzip compressed data, was "gendazpack-0.1.2.tar", max compression
```

## Comparing `gendazpack-0.1.1.tar` & `gendazpack-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1085 2024-02-09 02:26:13.630670 gendazpack-0.1.1/LICENSE
--rw-r--r--   0        0        0      859 2024-04-28 21:13:50.588351 gendazpack-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1767 2024-04-28 20:38:56.268546 gendazpack-0.1.1/README.rst
--rw-r--r--   0        0        0        0 2022-09-05 23:10:13.045452 gendazpack-0.1.1/src/gendazpack/__init__.py
--rw-r--r--   0        0        0     3740 2024-02-13 02:06:27.760553 gendazpack-0.1.1/src/gendazpack/__main__.py
--rw-r--r--   0        0        0      119 2023-12-10 04:29:09.239477 gendazpack-0.1.1/src/gendazpack/generator/__init__.py
--rw-r--r--   0        0        0     2709 2024-02-09 01:07:55.000901 gendazpack-0.1.1/src/gendazpack/generator/loadmetadata.py
--rw-r--r--   0        0        0     1188 2024-04-17 01:26:13.824284 gendazpack-0.1.1/src/gendazpack/generator/packagedata.py
--rw-r--r--   0        0        0    14343 2024-04-28 21:12:36.029210 gendazpack-0.1.1/src/gendazpack/generator/packagegenerator.py
--rw-r--r--   0        0        0      378 2023-11-19 02:25:00.738769 gendazpack-0.1.1/src/gendazpack/scrapers/__init__.py
--rw-r--r--   0        0        0     3465 2024-02-07 20:49:25.371542 gendazpack-0.1.1/src/gendazpack/scrapers/deviantart.py
--rw-r--r--   0        0        0     3732 2024-03-16 04:19:22.216416 gendazpack-0.1.1/src/gendazpack/scrapers/renderhub.py
--rw-r--r--   0        0        0     6021 2024-01-07 02:51:46.968034 gendazpack-0.1.1/src/gendazpack/scrapers/renderosity.py
--rw-r--r--   0        0        0     5108 2024-03-03 21:53:38.586403 gendazpack-0.1.1/src/gendazpack/scrapers/renderotica.py
--rw-r--r--   0        0        0     1208 2024-02-09 01:10:21.735323 gendazpack-0.1.1/src/gendazpack/scrapers/scraper.py
--rw-r--r--   0        0        0     5410 2024-01-22 05:40:17.071320 gendazpack-0.1.1/src/gendazpack/scrapers/sharecg.py
--rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 gendazpack-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-02-09 02:26:13.630670 gendazpack-0.1.2/LICENSE
+-rw-r--r--   0        0        0      859 2024-05-06 05:37:25.841911 gendazpack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1767 2024-04-28 20:38:56.268546 gendazpack-0.1.2/README.rst
+-rw-r--r--   0        0        0        0 2022-09-05 23:10:13.045452 gendazpack-0.1.2/src/gendazpack/__init__.py
+-rw-r--r--   0        0        0     3740 2024-02-13 02:06:27.760553 gendazpack-0.1.2/src/gendazpack/__main__.py
+-rw-r--r--   0        0        0      119 2023-12-10 04:29:09.239477 gendazpack-0.1.2/src/gendazpack/generator/__init__.py
+-rw-r--r--   0        0        0     2709 2024-02-09 01:07:55.000901 gendazpack-0.1.2/src/gendazpack/generator/loadmetadata.py
+-rw-r--r--   0        0        0     1188 2024-04-17 01:26:13.824284 gendazpack-0.1.2/src/gendazpack/generator/packagedata.py
+-rw-r--r--   0        0        0    14482 2024-05-05 23:32:22.145077 gendazpack-0.1.2/src/gendazpack/generator/packagegenerator.py
+-rw-r--r--   0        0        0      378 2023-11-19 02:25:00.738769 gendazpack-0.1.2/src/gendazpack/scrapers/__init__.py
+-rw-r--r--   0        0        0     3465 2024-02-07 20:49:25.371542 gendazpack-0.1.2/src/gendazpack/scrapers/deviantart.py
+-rw-r--r--   0        0        0     3732 2024-03-16 04:19:22.216416 gendazpack-0.1.2/src/gendazpack/scrapers/renderhub.py
+-rw-r--r--   0        0        0     6021 2024-01-07 02:51:46.968034 gendazpack-0.1.2/src/gendazpack/scrapers/renderosity.py
+-rw-r--r--   0        0        0     5108 2024-03-03 21:53:38.586403 gendazpack-0.1.2/src/gendazpack/scrapers/renderotica.py
+-rw-r--r--   0        0        0     1208 2024-02-09 01:10:21.735323 gendazpack-0.1.2/src/gendazpack/scrapers/scraper.py
+-rw-r--r--   0        0        0     5410 2024-01-22 05:40:17.071320 gendazpack-0.1.2/src/gendazpack/scrapers/sharecg.py
+-rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 gendazpack-0.1.2/PKG-INFO
```

### Comparing `gendazpack-0.1.1/LICENSE` & `gendazpack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/pyproject.toml` & `gendazpack-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gendazpack"
-version = "0.1.1"
+version = "0.1.2"
 description = "DAZ Content Package Generator"
 license = "MIT"
 authors = ["Omni Flux <omniflux@omniflux.com>"]
 readme = "README.rst"
 repository = "https://github.com/Omniflux/gendazpack"
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `gendazpack-0.1.1/README.rst` & `gendazpack-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/__main__.py` & `gendazpack-0.1.2/src/gendazpack/__main__.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/generator/loadmetadata.py` & `gendazpack-0.1.2/src/gendazpack/generator/loadmetadata.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/generator/packagedata.py` & `gendazpack-0.1.2/src/gendazpack/generator/packagedata.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/generator/packagegenerator.py` & `gendazpack-0.1.2/src/gendazpack/generator/packagegenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import sys
 import zipfile
 
 from dataclasses import dataclass, fields, KW_ONLY
 from http.client import HTTPResponse
 from mimetypes import guess_extension
 from pathlib import Path
+from struct import pack
 from urllib.parse import ParseResult
 from uuid import uuid4
-from lxml import etree
 
+from lxml import etree
 
 from .loadmetadata import load_metadata
 from .packagedata import PackageData
 from ..scrapers import scrape
 
 _CONTENT_DIR = 'Content'
 _SUPPORT_DIR = 'Runtime/Support'
@@ -24,32 +25,37 @@
 _COMPRESSABLE_DAZ_EXTENSIONS = ('.dsf', '.duf')
 _NON_USER_FACING_DIRECTORIES = ('data', "readme's", 'runtime', 'uninstallers')
 
 _USER_FACING_POSER_EXTENSIONS = ('.pz3', '.pzz', '.cr2', '.crz', '.pz2', '.p2z', '.fc2', '.fcz', '.hr2', '.hrz', '.hd2', '.hdz', '.pp2', '.ppz', '.lt2', '.ltz', '.cm2', '.cmz', '.mc6', '.mcz', '.mt5', '.mz5')
 _OTHER_POSER_EXTENSIONS = ('.pmd',)
 _POSER_USER_FACING_DIRECTORIES = ('camera', 'character', 'collections', 'face', 'hair', 'hand', 'light', 'materials', 'pose', 'props', 'scene')
 
-_EXCLUDE_FILES = (x.lower() for x in ['.DS_Store', '._.DS_Store', 'InstallManagerFileRegister.json', 'Desktop.ini', 'Thumbs.db'])
+_EXCLUDE_FILES = (x.lower() for x in ['.DS_Store', '._.DS_Store', 'InstallManagerFileRegister.json', 'Desktop.ini', 'pspbrwse.jbf', 'Thumbs.db'])
 _EXCLUDE_SUFFIXES = ('.xmp',)
 
 
 # DIM does not support Unicode filenames in ZIP files due to using the minizip 1.01 library.
-# Examining offical DAZ packages reveals Windows-1252 encoding is used. Packages with
+# Examining official DAZ packages reveals Windows-1252 encoding is used. Packages with
 # filenames using non ASCII characters may not extract correctly on OS X.
 Ascii_ZipInfo = zipfile.ZipInfo
 class Windows1252_ZipInfo(zipfile.ZipInfo):
-    def _encodeFilenameFlags(self):
-        try:
-            return self.filename.encode('Windows-1252'), self.flag_bits
-        except UnicodeEncodeError as e:
-            raise SystemExit(f'DIM does not support Unicode filenames: {self.filename}') from e
-
-_ENCODING_WARNING = ('WARNING: Non ASCII characters detected in file paths.\n'
-					 'Windows-1252 encoding used for compatibility with DIM.\n'
-					 'Archive may not extract correctly with normal ZIP tools.')
+	def _encodeFilenameFlags(self):
+		try:
+			return self.filename.encode('Windows-1252'), self.flag_bits
+		except UnicodeEncodeError as e:
+			raise SystemExit(f'DIM does not support Unicode filenames: {self.filename}') from e
+
+	def __init__(self, filename: str = "NoName", date_time: tuple[int, int, int, int, int, int] = (1980,1,1,0,0,0)):
+		super().__init__(filename, date_time)
+
+		if self.filename.encode() != self.filename.encode('Windows-1252', 'replace'):
+			UNICODE_PATH_EXTRA_FIELD_ID = 0x7075
+			encoded_filename = self.filename.encode()
+			crc = zipfile.crc32(self._encodeFilenameFlags()[0])	# pyright: ignore[reportAttributeAccessIssue, reportUnknownMemberType, reportUnknownVariableType]
+			self.extra += pack(f'<HHBL{len(encoded_filename)}s', UNICODE_PATH_EXTRA_FIELD_ID, len(encoded_filename) + 5, 1, crc, encoded_filename)
 
 @dataclass
 class PackageGenerator(PackageData):
 	id: int | None = None
 	url: ParseResult | None = None
 	verbose: bool = False
 	_: KW_ONLY
@@ -303,15 +309,14 @@
 		if self.verbose:
 			print('Generating ZIP file')
 
 		self._assert_required_vars()
 
 		# Use Windows-1252 encoding for filenames
 		zipfile.ZipInfo = Windows1252_ZipInfo
-		encoding_issue = self.metadata_filename_base.encode() != self.metadata_filename_base.encode('Windows-1252')
 
 		with zipfile.ZipFile(self.zip_filename, 'x', zipfile.ZIP_DEFLATED) as zip_file:
 			# DIM Package
 			zip_file.writestr(_MANIFEST_FILE, self.manifest_file)
 			zip_file.writestr(_SUPPLEMENT_FILE, self.supplement_file)
 
 			# ReadMe
@@ -330,35 +335,29 @@
 					zip_file.writestr(f'{_CONTENT_DIR}/{_SUPPORT_DIR}/{self.metadata_filename_base}{image_extension}', self.image.read())
 
 			# Content
 			if self.verbose:
 				print('Adding Content')
 
 			for file_path, relative_file_path, in self._files():
-				if not encoding_issue and file_path.as_posix().encode() != file_path.as_posix().encode('Windows-1252', 'replace'):
-					encoding_issue = True
-
 				# Compress DAZ compressable files before adding to archive
 				if file_path.suffix.lower() in _COMPRESSABLE_DAZ_EXTENSIONS and file_path.stat().st_size:
 					with gzip.open(file_path) as f:
 						try:
 							f.read(1)
 							zip_file.write(file_path, _CONTENT_DIR / relative_file_path)
 						except gzip.BadGzipFile:
 							if self.verbose:
 								print (f'Compressing: {relative_file_path}')
 							with open(file_path, 'rb') as f:
-								zip_file.writestr((_CONTENT_DIR / relative_file_path).as_posix(), gzip.compress(f.read()))
+								zip_file.writestr(zipfile.ZipInfo.from_file(file_path, (_CONTENT_DIR / relative_file_path).as_posix()), gzip.compress(f.read()))
 				else:
 					zip_file.write(file_path, _CONTENT_DIR / relative_file_path)
 
 		# Revert filename encoding
 		zipfile.ZipInfo = Ascii_ZipInfo
 
-		if encoding_issue:
-			print(_ENCODING_WARNING)
-
 	def make_package(self) -> None:
 		try:
 			self._create_zip()
 		except (FileExistsError) as e:
 			sys.exit(e)	# pyright: ignore[reportArgumentType]
```

### Comparing `gendazpack-0.1.1/src/gendazpack/scrapers/deviantart.py` & `gendazpack-0.1.2/src/gendazpack/scrapers/deviantart.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/scrapers/renderhub.py` & `gendazpack-0.1.2/src/gendazpack/scrapers/renderhub.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/scrapers/renderosity.py` & `gendazpack-0.1.2/src/gendazpack/scrapers/renderosity.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/scrapers/renderotica.py` & `gendazpack-0.1.2/src/gendazpack/scrapers/renderotica.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/scrapers/scraper.py` & `gendazpack-0.1.2/src/gendazpack/scrapers/scraper.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/src/gendazpack/scrapers/sharecg.py` & `gendazpack-0.1.2/src/gendazpack/scrapers/sharecg.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.1/PKG-INFO` & `gendazpack-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gendazpack
-Version: 0.1.1
+Version: 0.1.2
 Summary: DAZ Content Package Generator
 Home-page: https://github.com/Omniflux/gendazpack
 License: MIT
 Author: Omni Flux
 Author-email: omniflux@omniflux.com
 Requires-Python: >=3.11
 Classifier: Development Status :: 5 - Production/Stable
```

