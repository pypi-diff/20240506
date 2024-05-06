# Comparing `tmp/blint-2.1.3.tar.gz` & `tmp/blint-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.1.3.tar", max compression
+gzip compressed data, was "blint-2.1.4.tar", max compression
```

## Comparing `blint-2.1.3.tar` & `blint-2.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-04-21 15:41:54.867738 blint-2.1.3/LICENSE
--rw-r--r--   0        0        0     6240 2024-04-21 15:41:54.867738 blint-2.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-21 15:41:54.867738 blint-2.1.3/blint/__init__.py
--rw-r--r--   0        0        0    24122 2024-04-21 15:41:54.867738 blint-2.1.3/blint/analysis.py
--rw-r--r--   0        0        0    13915 2024-04-21 15:41:54.867738 blint-2.1.3/blint/android.py
--rw-r--r--   0        0        0    56702 2024-04-21 15:41:54.871738 blint-2.1.3/blint/binary.py
--rw-r--r--   0        0        0     2794 2024-04-21 15:41:54.871738 blint-2.1.3/blint/checks.py
--rw-r--r--   0        0        0     6198 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cli.py
--rw-r--r--   0        0        0    20365 2024-04-21 15:41:54.871738 blint-2.1.3/blint/config.py
--rw-r--r--   0        0        0      324 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-04-21 15:41:54.871738 blint-2.1.3/blint/logger.py
--rw-r--r--   0        0        0    24904 2024-04-21 15:41:54.875738 blint-2.1.3/blint/sbom.py
--rw-r--r--   0        0        0    14323 2024-04-21 15:41:54.875738 blint-2.1.3/blint/utils.py
--rw-r--r--   0        0        0     1812 2024-04-21 15:41:54.875738 blint-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 blint-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-05 17:51:02.425936 blint-2.1.4/LICENSE
+-rw-r--r--   0        0        0     6233 2024-05-05 17:51:02.425936 blint-2.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 17:51:02.425936 blint-2.1.4/blint/__init__.py
+-rw-r--r--   0        0        0    24653 2024-05-05 17:51:02.425936 blint-2.1.4/blint/analysis.py
+-rw-r--r--   0        0        0    13915 2024-05-05 17:51:02.425936 blint-2.1.4/blint/android.py
+-rw-r--r--   0        0        0    57666 2024-05-05 17:51:02.425936 blint-2.1.4/blint/binary.py
+-rw-r--r--   0        0        0     2794 2024-05-05 17:51:02.425936 blint-2.1.4/blint/checks.py
+-rw-r--r--   0        0        0     6198 2024-05-05 17:51:02.425936 blint-2.1.4/blint/cli.py
+-rw-r--r--   0        0        0    20192 2024-05-05 17:51:02.425936 blint-2.1.4/blint/config.py
+-rw-r--r--   0        0        0      324 2024-05-05 17:51:02.425936 blint-2.1.4/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 17:51:02.425936 blint-2.1.4/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-05-05 17:51:02.425936 blint-2.1.4/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-05-05 17:51:02.425936 blint-2.1.4/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:51:02.425936 blint-2.1.4/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 17:51:02.425936 blint-2.1.4/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-05 17:51:02.425936 blint-2.1.4/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-05-05 17:51:02.425936 blint-2.1.4/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-05-05 17:51:02.429937 blint-2.1.4/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-05-05 17:51:02.429937 blint-2.1.4/blint/logger.py
+-rw-r--r--   0        0        0    24904 2024-05-05 17:51:02.429937 blint-2.1.4/blint/sbom.py
+-rw-r--r--   0        0        0    14365 2024-05-05 17:51:02.429937 blint-2.1.4/blint/utils.py
+-rw-r--r--   0        0        0     1872 2024-05-05 17:51:02.433936 blint-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7494 1970-01-01 00:00:00.000000 blint-2.1.4/PKG-INFO
```

### Comparing `blint-2.1.3/LICENSE` & `blint-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/README.md` & `blint-2.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 - reviews.json - Contains information from the capability reviews. Useful for further analysis
 - fuzzables.json - Contains a suggested list of methods for fuzzing
 
 sbom command generates CycloneDX json.
 
 ## References
 
-- [lief examples](https://github.com/lief-project/LIEF/tree/master/examples/python)
+- [lief examples](https://github.com/lief-project/LIEF/tree/master/examples)
 - [checksec](https://github.com/Wenzel/checksec.py)
 
 ## Discord support
 
 The developers can be reached via the [Discord](https://discord.gg/DCNxzaeUpd) channel.
 
 ## Sponsorship wishlist
```

### Comparing `blint-2.1.3/blint/analysis.py` & `blint-2.1.4/blint/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import contextlib
 import importlib  # noqa
-import json
 import os
 import re
 import sys
 import uuid
 from collections import defaultdict
 from datetime import datetime
 from itertools import islice
 from pathlib import Path
 
+import orjson
 import yaml
 from rich.progress import Progress
 from rich.terminal_theme import MONOKAI
 
 from blint.binary import parse
-from blint.checks import (check_nx, check_pie,  # noqa, pylint: disable=unused-import
+# pylint: disable-next=unused-import
+from blint.checks import (check_nx, check_pie,
                           check_relro, check_canary, check_rpath,
                           check_virtual_size, check_authenticode,
                           check_dll_characteristics, check_codesign,
                           check_trust_info)
 from blint.logger import LOG, console
 from blint.utils import (create_findings_table, is_fuzzable_name, print_findings_table)
 
@@ -296,14 +297,15 @@
                 r.get("summary"),
                 "\n".join(evidences),
             )
     console.print(table)
 
 
 def json_serializer(obj):
+    """JSON serializer to help serialize problematic types such as bytes"""
     if isinstance(obj, bytes):
         return obj.decode('utf-8')
 
     return obj
 
 
 def report(src_dir, reports_dir, findings, reviews, files, fuzzables):
@@ -323,31 +325,33 @@
         "scan_id": run_uuid,
         "created": f"{datetime.now():%Y-%m-%d %H:%M:%S%z}",
     }
     if findings:
         print_findings_table(findings, files)
         findings_file = Path(reports_dir) / "findings.json"
         LOG.info(f"Findings written to {findings_file}")
+        output = orjson.dumps({**common_metadata, "findings": findings}, default=json_serializer).decode("utf-8",
+                                                                                                         "ignore")
         with open(findings_file, mode="w", encoding="utf-8") as ffp:
-            json.dump(
-                {**common_metadata, "findings": findings}, ffp, default=json_serializer
-            )
+            ffp.write(output)
     if reviews:
         print_reviews_table(reviews, files)
         reviews_file = Path(reports_dir) / "reviews.json"
         LOG.info(f"Review written to {reviews_file}")
+        output = orjson.dumps({**common_metadata, "reviews": reviews}, default=json_serializer).decode("utf-8",
+                                                                                                       "ignore")
         with open(reviews_file, mode="w", encoding="utf-8") as rfp:
-            json.dump({**common_metadata, "reviews": reviews}, rfp, default=json_serializer)
+            rfp.write(output)
     if fuzzables:
         fuzzables_file = Path(reports_dir) / "fuzzables.json"
         LOG.info(f"Fuzzables data written to {fuzzables_file}")
+        output = orjson.dumps({**common_metadata, "fuzzables": fuzzables}, default=json_serializer).decode("utf-8",
+                                                                                                           "ignore")
         with open(fuzzables_file, mode="w", encoding="utf-8") as rfp:
-            json.dump(
-                {**common_metadata, "fuzzables": fuzzables}, rfp, default=json_serializer
-            )
+            rfp.write(output)
     else:
         LOG.debug("No suggestion available for fuzzing")
 
     if not findings and not reviews:
         LOG.info(f":white_heavy_check_mark: No issues found in {src_dir}!")
     # Try console output as html
     else:
@@ -408,16 +412,17 @@
             self.task, description=f"Processing [bold]{f}[/bold]")
         metadata = parse(f)
         exe_name = metadata.get("name", "")
         # Store raw metadata
         metadata_file = (Path(reports_dir) / f"{os.path.basename(exe_name)}"
                                              f"-metadata.json")
         LOG.debug(f"Metadata written to {metadata_file}")
+        output = orjson.dumps(metadata, default=json_serializer).decode("utf-8", "ignore")
         with open(metadata_file, mode="w", encoding="utf-8") as ffp:
-            json.dump(metadata, ffp, default=json_serializer)
+            ffp.write(output)
         self.progress.update(
             self.task,
             description=f"Checking [bold]{f}[/bold] against rules")
         if finding := run_checks(f, metadata):
             self.findings += finding
         # Perform symbol reviews
         if no_reviews:
@@ -635,15 +640,14 @@
                 if found_cid[cid] > EVIDENCE_LIMIT:
                     continue
                 patterns = rule_obj.get("patterns")
                 for apattern in patterns:
                     if found_pattern[apattern] > EVIDENCE_LIMIT or found_cid[cid] > EVIDENCE_LIMIT:
                         continue
                     for afun in functions_list:
-                        if ((apattern.lower() in afun.lower()) and not
-                                found_function.get(afun.lower())):
+                        if apattern.lower() in afun.lower() and not found_function.get(afun.lower()):
                             result = {"pattern": apattern, "function": afun, }
                             results[cid].append(result)
                             found_cid[cid] += 1
                             found_pattern[apattern] += 1
                             found_function[afun.lower()] = True
         self.results |= results
```

### Comparing `blint-2.1.3/blint/android.py` & `blint-2.1.4/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/binary.py` & `blint-2.1.4/blint/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,52 @@
 # pylint: disable=too-many-lines,consider-using-f-string
 import codecs
 import contextlib
-import json
 import sys
 from typing import Tuple
 import zlib
+import orjson
 
 import lief
 
 from blint.logger import DEBUG, LOG
 from blint.utils import calculate_entropy, check_secret, cleanup_dict_lief_errors, decode_base64
 
+SYMBOLIC_FOUND = True
+try:
+    from symbolic._lowlevel import ffi, lib
+    from symbolic.utils import encode_str, decode_str, rustcall
+except OSError:
+    SYMBOLIC_FOUND = False
+
 MIN_ENTROPY = 0.39
 MIN_LENGTH = 80
 
 # Enable lief logging in debug mode
 if LOG.level != DEBUG:
     lief.logging.disable()
 
 ADDRESS_FMT = "0x{:<10x}"
 
 
+def demangle_symbolic_name(symbol, lang=None, no_args=False):
+    """Demangles a symbol."""
+    if not SYMBOLIC_FOUND:
+        return symbol
+    try:
+        func = lib.symbolic_demangle_no_args if no_args else lib.symbolic_demangle
+        lang_str = encode_str(lang) if lang else ffi.NULL
+
+        demangled = rustcall(func, encode_str(symbol), lang_str)
+        demangled_symbol = decode_str(demangled, free=True)
+        return demangled_symbol.strip()
+    except AttributeError:
+        return symbol
+
+
 def is_shared_library(parsed_obj):
     """
     Checks if the given parsed binary object represents a shared library.
 
     Args:
         parsed_obj: The parsed binary object to be checked.
 
@@ -239,15 +261,17 @@
             is_exported = False
             if symbol.imported and not isinstance(symbol.imported, lief.lief_errors):
                 is_imported = True
             if symbol.exported and not isinstance(symbol.exported, lief.lief_errors):
                 is_exported = True
             symbol_name = symbol.demangled_name
             if isinstance(symbol_name, lief.lief_errors):
-                symbol_name = symbol.name
+                symbol_name = demangle_symbolic_name(symbol.name)
+            else:
+                symbol_name = demangle_symbolic_name(symbol_name)
             exe_type = guess_exe_type(symbol_name)
             symbols_list.append(
                 {
                     "name": symbol_name,
                     "type": str(symbol.type).rsplit(".", maxsplit=1)[-1],
                     "value": symbol.value,
                     "visibility": str(symbol.visibility).rsplit(".", maxsplit=1)[-1],
@@ -493,20 +517,22 @@
             - symbols_list (list): A list of symbol dictionaries
             - exe_type (str): The determined executable type.
     """
     LOG.debug("Parsing symbols")
     symbols_list = []
     exe_type = ""
     for symbol in symbols:
+        if not symbol:
+            continue
         try:
             if symbol.section_number <= 0:
                 section_nb_str = str(lief.PE.SYMBOL_SECTION_NUMBER(symbol.section_number)).rsplit(
                     ".", maxsplit=1
                 )[-1]
-            elif symbol.section.name:
+            elif symbol.section and symbol.section.name:
                 section_nb_str = symbol.section.name
             else:
                 section_nb_str = "section<{:d}>".format(symbol.section_number)
         except (AttributeError, TypeError) as e:
             LOG.debug(f"Caught {type(e)}: {e} while parsing {symbol} PE symbol.")
             section_nb_str = ""
         try:
@@ -521,14 +547,16 @@
                         "base_type": str(symbol.base_type).rsplit(".", maxsplit=1)[-1],
                         "complex_type": str(symbol.complex_type).rsplit(".", maxsplit=1)[-1],
                         "storage_class": str(symbol.storage_class).rsplit(".", maxsplit=1)[-1],
                     }
                 )
         except (IndexError, AttributeError, ValueError) as e:
             LOG.debug(f"Caught {type(e)}: {e} while parsing {symbol}.")
+        except RuntimeError:
+            pass
     return symbols_list, exe_type
 
 
 def parse_pe_imports(imports):
     """
     Parses the imports and returns lists of imported symbols and DLLs.
 
@@ -633,16 +661,17 @@
             symbol_value = (
                 symbol.value
                 if symbol.value > 0 or not symbol.has_binding_info
                 else ADDRESS_FMT.format(symbol.binding_info.address)
             )
             symbol_name = symbol.demangled_name
             if not symbol_name or isinstance(symbol_name, lief.lief_errors):
-                symbol_name = symbol.name
-            symbol_name = symbol_name.replace("..", "::")
+                symbol_name = demangle_symbolic_name(symbol.name)
+            else:
+                symbol_name = demangle_symbolic_name(symbol_name)
             if not exe_type:
                 exe_type = guess_exe_type(symbol_name)
             symbols_list.append(
                 {
                     "name": (f"{libname}::{symbol_name}" if libname else symbol_name),
                     "short_name": symbol_name,
                     "type": symbol.type,
@@ -903,16 +932,16 @@
             start_index = overlay_str.find('{"runtimeTarget')
             end_index = overlay_str.rfind("}}}")
             if end_index > -1:
                 overlay_str = overlay_str[start_index: end_index + 3]
                 try:
                     # deps should have runtimeTarget, compilationOptions, targets, and libraries
                     # Use libraries to construct BOM components and targets for the dependency tree
-                    deps = json.loads(overlay_str)
-                except json.JSONDecodeError:
+                    deps = orjson.loads(overlay_str)
+                except orjson.JSONDecodeError:
                     pass
     return deps
 
 
 def parse_go_buildinfo(parsed_obj: lief.Binary) -> Tuple[dict[str, dict[str, str]], dict[str, str]]:
     """
     Parse the go build info section to extract go dependencies
@@ -977,20 +1006,20 @@
     """
     deps = []
 
     try:
         audit_data_section = next(filter(lambda section: section.name == ".dep-v0", parsed_obj.sections), None)
         if audit_data_section is not None and audit_data_section.content:
             json_string = zlib.decompress(audit_data_section.content)
-            audit_data = json.loads(json_string)
+            audit_data = orjson.loads(json_string)
 
             if audit_data and audit_data["packages"]:
                 packages = audit_data["packages"]
                 deps = [x for x in packages if 'root' not in x]
-    except json.JSONDecodeError:
+    except orjson.JSONDecodeError:
         pass
 
     return deps
 
 
 def add_pe_metadata(exe_file: str, metadata: dict, parsed_obj: lief.PE.Binary):
     """Adds PE metadata to the given metadata dictionary.
```

### Comparing `blint-2.1.3/blint/checks.py` & `blint-2.1.4/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/cli.py` & `blint-2.1.4/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/config.py` & `blint-2.1.4/blint/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,28 +33,14 @@
     ".gz",
     ".tar",
     ".tar.gz",
     ".tar.xz",
     ".tar",
     ".log",
     ".tmp",
-    ".gif",
-    ".png",
-    ".jpg",
-    ".webp",
-    ".webm",
-    ".icns",
-    ".pcm",
-    ".wav",
-    ".mp3",
-    ".pdf",
-    ".doc",
-    ".docx",
-    ".xls",
-    ".xlsx",
     ".d.ts",
     ".min.js",
     ".min.css",
     ".eslintrc.js",
     ".babelrc.js",
     ".spec.js",
     ".spec.ts",
```

### Comparing `blint-2.1.3/blint/cyclonedx/spdx.py` & `blint-2.1.4/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/cyclonedx/spec.py` & `blint-2.1.4/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.4/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.4/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_exe_go.yml` & `blint-2.1.4/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.4/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.4/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.4/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.4/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_monero_go.yml` & `blint-2.1.4/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_monero_rust` & `blint-2.1.4/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.4/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.4/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.4/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.4/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.4/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.4/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.4/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/data/rules.yml` & `blint-2.1.4/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/logger.py` & `blint-2.1.4/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/sbom.py` & `blint-2.1.4/blint/sbom.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.3/blint/utils.py` & `blint-2.1.4/blint/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,9 +501,10 @@
                 )
             ],
         )
     )
 
 
 def camel_to_snake(name: str) -> str:
+    """Convert camelCase to snake_case"""
     name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
```

### Comparing `blint-2.1.3/pyproject.toml` & `blint-2.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.1.3"
+version = "2.1.4"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
@@ -30,14 +30,16 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 lief = "^0.14.0"
 rich = "^13.7.0"
 PyYAML = "^6.0.1"
 defusedxml = "^0.7.1"
 pydantic = {version = "^2.6.0", extras = ["email"]}
+orjson = "^3.10.1"
+symbolic = "10.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 black = "^24.0.0"
 flake8 = "^7.0.0"
 pylint = "^3.0.0"
 pytest-cov = "^4.0.0"
@@ -50,16 +52,16 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov-append --cov-report term --cov blint"
 
 [tool.pylint]
-generated-members = ["lief"]
-ignore-paths = ["blint/cyclonedx/*"]
+generated-members = ["lief", "orjson"]
+ignore-paths = ["blint/cyclonedx/*", "tests/*"]
 # Let's not fuss about long strings
 ignore-long-lines = "[r|f]\""
 disable = ["missing-module-docstring", "logging-fstring-interpolation"]
 
 [tool.pylint.format]
 max-line-length = 99
```

### Comparing `blint-2.1.3/PKG-INFO` & `blint-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.1.3
+Version: 2.1.4
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
@@ -18,16 +18,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: lief (>=0.14.0,<0.15.0)
+Requires-Dist: orjson (>=3.10.1,<4.0.0)
 Requires-Dist: pydantic[email] (>=2.6.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: symbolic (==10.2.1)
 Project-URL: CI, https://github.com/AppThreat/blint/actions
 Project-URL: Repository, https://github.com/OWASP-dep-scan/blint
 Description-Content-Type: text/markdown
 
 # BLint
 
 <img src="./blint.png" width="400" />
@@ -172,15 +174,15 @@
 - reviews.json - Contains information from the capability reviews. Useful for further analysis
 - fuzzables.json - Contains a suggested list of methods for fuzzing
 
 sbom command generates CycloneDX json.
 
 ## References
 
-- [lief examples](https://github.com/lief-project/LIEF/tree/master/examples/python)
+- [lief examples](https://github.com/lief-project/LIEF/tree/master/examples)
 - [checksec](https://github.com/Wenzel/checksec.py)
 
 ## Discord support
 
 The developers can be reached via the [Discord](https://discord.gg/DCNxzaeUpd) channel.
 
 ## Sponsorship wishlist
```

