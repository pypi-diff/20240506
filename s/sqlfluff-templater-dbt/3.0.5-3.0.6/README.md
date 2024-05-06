# Comparing `tmp/sqlfluff_templater_dbt-3.0.5.tar.gz` & `tmp/sqlfluff_templater_dbt-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff_templater_dbt-3.0.5.tar", last modified: Fri Apr 19 13:48:32 2024, max compression
+gzip compressed data, was "sqlfluff_templater_dbt-3.0.6.tar", last modified: Mon May  6 19:38:39 2024, max compression
```

## Comparing `sqlfluff_templater_dbt-3.0.5.tar` & `sqlfluff_templater_dbt-3.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33153 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:39.922756 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33073 2024-05-06 19:38:31.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:39.926756 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 19:38:39.000000 sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff_templater_dbt-3.0.5/LICENSE.md` & `sqlfluff_templater_dbt-3.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff_templater_dbt-3.0.5/PKG-INFO` & `sqlfluff_templater_dbt-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 3.0.5
+Version: 3.0.6
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: sqlfluff==3.0.5
+Requires-Dist: sqlfluff==3.0.6
 Requires-Dist: dbt-core>=1.0.0
 Requires-Dist: jinja2-simple-tags>=0.3.1
 Requires-Dist: markupsafe
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
```

### Comparing `sqlfluff_templater_dbt-3.0.5/setup.cfg` & `sqlfluff_templater_dbt-3.0.6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 3.0.5
+version = 3.0.6
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -60,15 +60,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	sqlfluff==3.0.5
+	sqlfluff==3.0.6
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/templater.py` & `sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt/templater.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,14 @@
                 pass
 
     @cached_property
     def dbt_config(self):
         """Loads the dbt config."""
         from dbt import flags
         from dbt.adapters.factory import register_adapter
-        from dbt.config import read_user_config
         from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
 
         # Attempt to silence internal logging at this point.
         # https://github.com/sqlfluff/sqlfluff/issues/5054
         self.try_silence_dbt_logs()
 
         if self.dbt_version_tuple >= (1, 5):
@@ -159,14 +158,16 @@
         else:
             # Here, we read flags.PROFILE_DIR directly, prior to calling
             # set_from_args(). Apparently, set_from_args() sets PROFILES_DIR
             # to a lowercase version of the value, and the profile wouldn't be
             # found if the directory name contained uppercase letters. This fix
             # was suggested and described here:
             # https://github.com/sqlfluff/sqlfluff/issues/2253#issuecomment-1018722979
+            from dbt.config import read_user_config
+
             user_config = read_user_config(flags.PROFILES_DIR)
             # Pre 1.5.x this is a string.
             cli_vars = str(self._get_cli_vars())
 
         flags.set_from_args(
             DbtConfigArgs(
                 project_dir=self.project_dir,
@@ -434,15 +435,15 @@
     def process(
         self,
         *,
         fname: str,
         in_str: Optional[str] = None,
         config: Optional["FluffConfig"] = None,
         formatter: Optional["OutputStreamFormatter"] = None,
-    ):
+    ) -> Tuple[TemplatedFile, List[SQLTemplaterError]]:
         """Compile a dbt model and return the compiled SQL.
 
         Args:
             fname: Path to dbt model(s)
             in_str: fname contents using configured encoding
             config: A specific config to use for this
                 templating operation. Only necessary for some templaters.
@@ -469,43 +470,39 @@
         try:
             os.chdir(self.project_dir)
             processed_result = self._unsafe_process(fname_absolute_path, in_str, config)
             # Reset the fail counter
             self._sequential_fails = 0
             return processed_result
         except FailedToConnectError as e:
-            return None, [
-                SQLTemplaterError(
-                    "dbt tried to connect to the database and failed: you could use "
-                    "'execute' to skip the database calls. See "
-                    "https://docs.getdbt.com/reference/dbt-jinja-functions/execute/ "
-                    f"Error: {e.msg}",
-                    fatal=True,
-                )
-            ]
+            raise SQLTemplaterError(
+                "dbt tried to connect to the database and failed: you could use "
+                "'execute' to skip the database calls. See "
+                "https://docs.getdbt.com/reference/dbt-jinja-functions/execute/ "
+                f"Error: {e.msg}",
+                fatal=True,
+            )
         except CompilationError as e:
             # Increment the counter
             self._sequential_fails += 1
             if e.node:
                 _msg = (
                     f"dbt compilation error on file '{e.node.original_file_path}'"
                     f", {e.msg}"
                 )
             else:
                 _msg = f"dbt compilation error: {e.msg}"
-            return None, [
-                SQLTemplaterError(
-                    _msg,
-                    # It's fatal if we're over the limit
-                    fatal=self._sequential_fails > self.sequential_fail_limit,
-                )
-            ]
-        # If a SQLFluff error is raised, just pass it through
-        except SQLTemplaterError as e:  # pragma: no cover
-            return None, [e]
+            raise SQLTemplaterError(
+                _msg,
+                # It's fatal if we're over the limit
+                fatal=self._sequential_fails > self.sequential_fail_limit,
+            )
+        except SQLTemplaterError:
+            # Templater errors are re-raised directly to be caught by the linter.
+            raise
         finally:
             os.chdir(self.working_dir)
 
     def _find_node(self, fname, config=None):
         if not config:  # pragma: no cover
             raise ValueError(
                 "For the dbt templater, the `process()` method "
```

### Comparing `sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff_templater_dbt-3.0.6/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 3.0.5
+Version: 3.0.6
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: sqlfluff==3.0.5
+Requires-Dist: sqlfluff==3.0.6
 Requires-Dist: dbt-core>=1.0.0
 Requires-Dist: jinja2-simple-tags>=0.3.1
 Requires-Dist: markupsafe
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
```

