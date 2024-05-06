# Comparing `tmp/versup-1.5.9.tar.gz` & `tmp/versup-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versup-1.5.9.tar", max compression
+gzip compressed data, was "versup-1.6.0.tar", max compression
```

## Comparing `versup-1.5.9.tar` & `versup-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-10-25 18:33:08.486052 versup-1.5.9/LICENSE.txt
--rw-r--r--   0        0        0     6276 2023-10-25 18:33:08.486052 versup-1.5.9/README.md
--rw-r--r--   0        0        0      801 2023-11-29 17:40:34.828712 versup-1.5.9/pyproject.toml
--rw-r--r--   0        0        0      225 2023-11-29 17:40:34.828712 versup-1.5.9/versup/__init__.py
--rw-r--r--   0        0        0      112 2023-10-25 18:33:08.486052 versup-1.5.9/versup/__main__.py
--rw-r--r--   0        0        0     2817 2023-11-29 17:39:26.608720 versup-1.5.9/versup/changelog.py
--rw-r--r--   0        0        0     8122 2023-11-29 17:39:32.238721 versup-1.5.9/versup/command_line.py
--rw-r--r--   0        0        0     1813 2023-11-29 17:39:26.578720 versup-1.5.9/versup/conf_reader.py
--rw-r--r--   0        0        0     1058 2023-10-25 18:33:08.486052 versup-1.5.9/versup/custom_cmd_group.py
--rw-r--r--   0        0        0     2401 2023-10-25 18:33:08.486052 versup-1.5.9/versup/default_conf.py
--rw-r--r--   0        0        0     2911 2023-11-29 17:39:26.568720 versup-1.5.9/versup/file_updater.py
--rw-r--r--   0        0        0     4046 2023-11-29 17:39:26.618720 versup-1.5.9/versup/gitops.py
--rw-r--r--   0        0        0      328 2023-10-25 18:33:08.486052 versup-1.5.9/versup/printer.py
--rw-r--r--   0        0        0     1531 2023-11-29 17:39:26.618720 versup-1.5.9/versup/script_runner.py
--rw-r--r--   0        0        0      677 2023-10-25 18:33:08.486052 versup-1.5.9/versup/template.py
--rw-r--r--   0        0        0     1657 2023-11-29 17:39:26.568720 versup-1.5.9/versup/versioning.py
--rw-r--r--   0        0        0     7109 1970-01-01 00:00:00.000000 versup-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-30 16:05:10.112427 versup-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     6276 2024-04-30 16:05:10.112427 versup-1.6.0/README.md
+-rw-r--r--   0        0        0      945 2024-05-06 13:30:29.451645 versup-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-05-06 13:30:29.451645 versup-1.6.0/versup/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-30 16:05:10.116427 versup-1.6.0/versup/__main__.py
+-rw-r--r--   0        0        0     2817 2024-04-30 16:05:10.116427 versup-1.6.0/versup/changelog.py
+-rw-r--r--   0        0        0     8737 2024-05-06 13:30:17.875544 versup-1.6.0/versup/command_line.py
+-rw-r--r--   0        0        0     1813 2024-04-30 16:05:10.116427 versup-1.6.0/versup/conf_reader.py
+-rw-r--r--   0        0        0     1058 2024-04-30 16:05:10.116427 versup-1.6.0/versup/custom_cmd_group.py
+-rw-r--r--   0        0        0     2465 2024-05-06 13:30:17.875544 versup-1.6.0/versup/default_conf.py
+-rw-r--r--   0        0        0     2939 2024-05-06 13:30:17.875544 versup-1.6.0/versup/file_updater.py
+-rw-r--r--   0        0        0     4046 2024-04-30 16:05:10.116427 versup-1.6.0/versup/gitops.py
+-rw-r--r--   0        0        0      739 2024-05-06 13:30:17.879544 versup-1.6.0/versup/printer.py
+-rw-r--r--   0        0        0     1531 2024-04-30 16:05:10.116427 versup-1.6.0/versup/script_runner.py
+-rw-r--r--   0        0        0      677 2024-04-30 16:05:10.116427 versup-1.6.0/versup/template.py
+-rw-r--r--   0        0        0     1657 2024-04-30 16:05:10.116427 versup-1.6.0/versup/versioning.py
+-rw-r--r--   0        0        0     7207 1970-01-01 00:00:00.000000 versup-1.6.0/PKG-INFO
```

### Comparing `versup-1.5.9/LICENSE.txt` & `versup-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/README.md` & `versup-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/changelog.py` & `versup-1.6.0/versup/changelog.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/command_line.py` & `versup-1.6.0/versup/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import datetime
 import os
 from typing import Any, Dict, List
 
 import click
+from rich import print
+from rich.prompt import Confirm
 
 import versup.changelog as changelog
 import versup.file_updater as file_updater
 import versup.gitops as gitops
 import versup.script_runner as script_runner
 import versup.template as template
 from versup import VersupError, __version__
 from versup.conf_reader import (
     get_conf_value,
     merge_configs_with_default,
     parse_config_file,
 )
 from versup.custom_cmd_group import DefaultCommandGroup
-from versup.printer import print_error, print_ok, print_warn
+from versup.printer import make_file_tree, print_error, print_ok, print_warn
 from versup.versioning import get_new_version
 
 CONTEXT_SETTINGS = dict(
     help_option_names=["-h", "--help"],
 )
 
 
@@ -42,24 +44,25 @@
 @click.pass_context
 @click.option("-l", "--local", is_flag=True, help="Show local configuration options")
 @click.option("-g", "--global", is_flag=True, help="Show global configuration options")
 @click.option(
     "-c", "--current", is_flag=True, help="Show current configuration options"
 )
 def show_config(ctx, **kwargs):
-    import pprint
+    from rich.pretty import pprint
 
     config = ctx.obj.conf
     if kwargs["local"]:
         config = parse_config_file("./.versup.json")
     if kwargs["global"]:
         config = parse_config_file("~/.config/versup.json")
     if kwargs["current"]:
         config = merge_configs_with_default()
-    pprint.pprint(config)
+
+    pprint(config)
 
 
 @cli.command(
     default_command=True, name="increment/version", context_settings=CONTEXT_SETTINGS
 )
 @click.pass_context
 @click.argument("increment")
@@ -73,27 +76,39 @@
     is_flag=True,
     help="Show what will be done without applying anything",
 )
 def do_versup(ctx, **kwargs):
     """
     Increment or set project version
     """
+    print()
+    if kwargs["dryrun"]:
+        print(
+            "[bold green]:arrow_forward:[/bold green] Dry run set. No changes will be"
+            " made.\n"
+        )
     current_branch: str = gitops.get_current_branch()
     target_branch: str = get_conf_value(ctx.obj.conf, "commit/mainbranch")
     if not gitops.check_current_branch_matches(target_branch):
         print_warn(
             f"Main branch set to '{target_branch}'. Currently on '{current_branch}'"
         )
-        if not kwargs["dryrun"] and not click.confirm("Continue anyway?"):
+        if not kwargs["dryrun"] and not Confirm.ask("Continue anyway?"):
             return
 
-    unstaged_files = "\n".join(gitops.get_unstaged_changes())
+    unstaged_files = gitops.get_unstaged_changes()
     if unstaged_files:
-        print_warn(f"There are unstaged files\n{unstaged_files}")
-        if not kwargs["dryrun"] and not click.confirm("Continue with versup?"):
+        print_warn("There are unstaged files")
+
+        tree = make_file_tree(unstaged_files)
+
+        print(tree)
+        print()
+
+        if not kwargs["dryrun"] and not Confirm.ask("Continue with versup?"):
             return
 
     ctx.obj.version = kwargs["increment"]
 
     try:
         try:
             latest_version: str = gitops.get_latest_tag()
@@ -145,16 +160,21 @@
 def apply_bump(config, version, **kwargs):
     """
     Runs through all the stages of the release as defined by the config file.
     """
     # Update the files specified in config
     if not kwargs["no_fileupdate"]:
         files_to_update: Dict[str, Any] = get_conf_value(config, "files")
-        updated = file_updater.update_files(version, files_to_update, kwargs["dryrun"])
-        print_ok(f"Updated {', '.join(updated)}")
+        updated, updates = file_updater.update_files(
+            version, files_to_update, kwargs["dryrun"]
+        )
+        print_ok("Updated strings in the following files:")
+        tree = make_file_tree(updated, updates)
+        print(tree)
+        print()
 
     # create changelog
     if not kwargs["no_changelog"] and get_conf_value(config, "changelog/enabled"):
         do_changelog(config, version, **kwargs)
 
     # create new commit with version
     if not kwargs["no_commit"] and get_conf_value(config, "commit/enabled"):
@@ -179,15 +199,15 @@
     if not get_conf_value(config, "changelog/enabled"):
         return
     changelog_config: Dict = get_conf_value(config, "changelog")
     changelog_file: str = changelog_config["file"]
     # If no changelog file and create is off, prompt
     if not kwargs["dryrun"] and not os.path.isfile(changelog_file):
         if not changelog_config["create"]:
-            if not click.confirm("No changelog file found. Create it?"):
+            if not Confirm.ask("No changelog file found. Create it?"):
                 return
             # Ok to create/update it now
     changelog.write(
         changelog_file,
         changelog_config["version"],
         changelog_config["commit"],
         changelog_config["separator"],
@@ -231,16 +251,22 @@
     if not get_conf_value(config, "tag/enabled"):
         return
 
     tag_config: Dict = get_conf_value(config, "tag")
     template.token_data["version"] = version
     tag_name: str = template.render(tag_config["name"])
     if kwargs["dryrun"]:
-        print(f"Create tag {version} with msg {tag_name}")
+        print(
+            f"Create tag [bold cyan]{version}[/bold cyan] with message [bold"
+            f" cyan]{tag_name}[/bold cyan]"
+        )
     else:
         gitops.create_new_tag(version, tag_name)
 
-    print_ok(f"Tag {tag_name} created")
+    print_ok(
+        f"Tag for [bold cyan]{version}[/bold cyan] with message [cyan"
+        f" bold]{tag_name}[/cyan bold] created"
+    )
 
 
 def main():
     cli(prog_name="versup")
```

### Comparing `versup-1.5.9/versup/conf_reader.py` & `versup-1.6.0/versup/conf_reader.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/custom_cmd_group.py` & `versup-1.6.0/versup/custom_cmd_group.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/default_conf.py` & `versup-1.6.0/versup/default_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,22 @@
     },
     "tag": {
         "enabled": True,  # Tag the bump commit
         "name": "v[version]",  # Template for the name of the tag in the tag message
     },
     "tokens": {
         "date": {
-            "format": "%Y-%m-%d"  # Python datetime format to use when generating the `[date]` token
+            "format": (  # Python datetime format to use when generating the `[date]` token
+                "%Y-%m-%d"
+            )
         },
         "version_date": {
-            "format": "%Y-%m-%d"  # Python datetime format to use when generating the `[version_date]` token
+            "format": (  # Python datetime format to use when generating the `[version_date]` token
+                "%Y-%m-%d"
+            )
         },
     },
     "scripts": {
         "prebump": "",  # Script to execute before bumping the version
         "postbump": "",  # Script to execute after bumping the version
         "prechangelog": "",  # Script to execute before updating the changelog
         "postchangelog": "",  # Script to execute after updating the changelog
```

### Comparing `versup-1.5.9/versup/file_updater.py` & `versup-1.6.0/versup/file_updater.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import print_function
 
 import re
 from typing import Any, Dict, List
 
-from colorama import Style
+from rich import print
 
 import versup.template as template
 
 
 def update_file_data(data: str, replace_list: list) -> str:
     """
     The replace list is a list of two strings, the first is a regex
@@ -20,71 +20,73 @@
     """
     regex, new_text = replace_list
 
     updated_data: str = re.sub(regex, new_text, data, flags=re.M)
     return updated_data
 
 
-def show_updates(filename: str, data: str, replace_list: List[str]):
+def get_updates(filename: str, data: str, replace_list: List[str]):
     """
     This is the same as :update_file_data: but for dry runs. It will
     search for the matches to replace and print out the changes that will
     occur instead of actually updating the files
     """
     regex, new_text = replace_list
-
+    updates = {}
     lines: List[str] = data.split("\n")
     for line in lines:
         line = line.strip()
         m = re.search(regex, line)
         if m:
             updated_data = re.sub(regex, new_text, line, flags=re.M)
-            print(
-                f"In file {Style.BRIGHT}{filename}{Style.RESET_ALL} replace "
-                f"{Style.BRIGHT}{line}{Style.RESET_ALL} with "
-                f"{Style.BRIGHT}{updated_data}{Style.RESET_ALL}"
+            updates[filename.split("/")[-1]] = (
+                f"[bold red]{line}[/bold red] :arrow_forward: [bold"
+                f" green]{updated_data}[bold green]"
             )
+    return updates
 
 
-def update_files(new_version: str, files: Dict[str, Any], dryrun: bool) -> list:
+def update_files(
+    new_version: str, files: Dict[str, Any], dryrun: bool
+) -> tuple[list, dict]:
     """
     Will update the given files with the defined regex from
     the config files and the text to replace with
 
     :new_version: the new version for the next release
     :files: a list of dictionaries of  filenames with path on which to run the replace
     :dryrun: boolean flag whether to do a dry run or not
     """
     if not files:
         # No files to update
-        return []
+        return [], {}
 
     filenames = list(files.keys())
     template_data = {"version": new_version}
     updated_files: List[str] = []
+    updates: dict[str, str] = {}
     for filename in filenames:
         try:
             with open(filename, "r") as file_h:
                 data = file_h.read()
         except IOError:
             print(f"Unable to find {filename} to update.")
             continue
 
         updated_files.append(filename)
 
         # If it's only one entry make it a list to simplify program flow
         if not any(isinstance(el, list) for el in files[filename]):
             files[filename] = [files[filename]]
 
-        replace: List[str] = []
         for replace in files[filename]:
             replace[1] = template.render(replace[1], template_data)
             if dryrun:
-                show_updates(filename, data, replace)
+                updates = updates | get_updates(filename, data, replace)
             else:
                 data = update_file_data(data, replace)
 
         if not dryrun:
             with open(filename, "w") as file_h:
                 file_h.write(data)
 
-    return updated_files
+    return updated_files, updates
```

### Comparing `versup-1.5.9/versup/gitops.py` & `versup-1.6.0/versup/gitops.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/script_runner.py` & `versup-1.6.0/versup/script_runner.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/template.py` & `versup-1.6.0/versup/template.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/versup/versioning.py` & `versup-1.6.0/versup/versioning.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.9/PKG-INFO` & `versup-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: versup
-Version: 1.5.9
+Version: 1.6.0
 Summary: Version up your project with ease.
 Home-page: https://github.com/Svenito/versup
 License: MIT
 Author: Sven Steinbauer
 Author-email: sven@unlogic.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0,<9.0)
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: flake8-pyproject (>=1.2.3,<2.0.0)
 Requires-Dist: gitpython (>=3.1,<4.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: semver (>=2.13,<3.0)
 Requires-Dist: setuptools (>=65.5.3,<66.0.0)
 Project-URL: Repository, https://github.com/Svenito/versup
 Description-Content-Type: text/markdown
 
 # versup
```

