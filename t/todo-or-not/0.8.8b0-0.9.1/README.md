# Comparing `tmp/todo_or_not-0.8.8b0.tar.gz` & `tmp/todo_or_not-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todo_or_not-0.8.8b0.tar", max compression
+gzip compressed data, was "todo_or_not-0.9.1.tar", max compression
```

## Comparing `todo_or_not-0.8.8b0.tar` & `todo_or_not-0.9.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-03-20 23:41:59.045418 todo_or_not-0.8.8b0/LICENSE
--rw-r--r--   0        0        0     8362 2024-03-20 23:41:59.045418 todo_or_not-0.8.8b0/README.md
--rw-r--r--   0        0        0      858 2024-03-20 23:41:59.045418 todo_or_not-0.8.8b0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 23:41:59.045418 todo_or_not-0.8.8b0/todo_or_not/__init__.py
--rw-r--r--   0        0        0    11085 2024-03-20 23:41:59.049419 todo_or_not-0.8.8b0/todo_or_not/localize.py
--rw-r--r--   0        0        0    28227 2024-03-20 23:41:59.049419 todo_or_not-0.8.8b0/todo_or_not/todo_check.py
--rw-r--r--   0        0        0     9187 1970-01-01 00:00:00.000000 todo_or_not-0.8.8b0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-24 02:39:13.346592 todo_or_not-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2823 2024-03-24 02:39:13.346592 todo_or_not-0.9.1/README.md
+-rw-r--r--   0        0        0      921 2024-03-24 02:39:13.346592 todo_or_not-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-24 02:39:13.350592 todo_or_not-0.9.1/todo_or_not/__init__.py
+-rw-r--r--   0        0        0    11822 2024-03-24 02:39:13.350592 todo_or_not-0.9.1/todo_or_not/localize.py
+-rw-r--r--   0        0        0    29947 2024-03-24 02:39:13.350592 todo_or_not-0.9.1/todo_or_not/todo_check.py
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 todo_or_not-0.9.1/PKG-INFO
```

### Comparing `todo_or_not-0.8.8b0/LICENSE` & `todo_or_not-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `todo_or_not-0.8.8b0/todo_or_not/localize.py` & `todo_or_not-0.9.1/todo_or_not/localize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,89 @@
 SUPPORTED_ENCODINGS_TODOIGNORE = ["utf-8", "utf-16"]
 SUPPORTED_ENCODINGS_TODO_CHECK = ["utf-8", "utf-16"]
 
 LOCALIZE = {
     "en_us": {
+        "general_done": "Done!",
         "issue_body_reference_link": "Reference",
         "summary_title": "Summary",
         "summary_encoding_unsupported_singular": "File skipped due to unsupported encoding",
         "summary_encoding_unsupported_plural": "Files skipped due to unsupported encodings",
         "summary_files_scanned_singular": "File scanned",
         "summary_files_scanned_plural": "Files scanned",
         "summary_issues_generated_singular": "Issue generated",
         "summary_issues_generated_plural": "Issues generated",
         "summary_issues_generated_none": "No issues generated",
         "summary_duplicate_issues_avoided_singular": "Duplicate issue prevented",
         "summary_duplicate_issues_avoided_plural": "Duplicate issues prevented",
         "info_duplicate_issue_avoided": "INFO: Duplicate issue avoided",
         "error_cannot_specify_ni_xi": "ERROR: Cannot specify both --ni and --xi",
         "error_is_not_file": "ERROR: Specified path is not a file",
+        "error_file_already_exists": "ERROR: Specified file already exists",
         "error_todo_ignore_not_found": "ERROR: .todo-ignore NOT FOUND! use -i to copy another .ignore OR --force to run without a .todo-ignore (NOT RECOMMENDED)",
         "error_todo_ignore_not_supported": f"ERROR: .todo-ignore uses unsupported encoding or doesn't exist! Supported encodings: {SUPPORTED_ENCODINGS_TODOIGNORE}",
         "error_exceeded_maximum_issues": "ERROR: Exceeded maximum number of issues for this run, exiting now",
         "warning_force_overrides_ignore": "WARNING: --force will ignore the contents of the .todo-ignore generated when you specified (.todo-ignore will still be changed, just not used)",
+        "warning_file_does_not_exist": "WARNING: File doesn't exist",
         "warning_run_with_empty_todo_ignore": "WARNING: .todo-ignore was empty (if the file isn't empty, check its encoding), running anyway. To cancel use ",
         "warning_run_without_todo_ignore": "WARNING: Running without a .todo-ignore, to cancel use ",
         "warning_encoding_not_supported": f"WARNING: File uses unsupported encoding, we will skip it but consider adding to .todo-ignore (Supported encodings: {SUPPORTED_ENCODINGS_TODO_CHECK})",
         "warning_using_default_region": f"WARNING: Unsupported region detected, defaulting to en_us. Detected region:",
         "warning_using_default_os": f"WARNING: Unsupported OS detected, using default tips. Detected OS:",
     },
     "ko_kr": {
+        "general_done": "끝났습니다!",
         "issue_body_reference_link": "참조",
         "summary_title": "요약",
         "summary_encoding_unsupported_singular": "지원되지 않는 인코딩(문자)의 이유로 파일이 제외되었습니다",
         "summary_encoding_unsupported_plural": "지원되지 않는 인코딩(문자)의 이유로 여러 파일이 제외되었습니다",
         "summary_files_scanned_singular": "하나의 파일을 스캔하였습니다",
         "summary_files_scanned_plural": "여러 개의 파일을 스캔하였습니다",
         "summary_issues_generated_singular": "깃허브 이슈가 생성되었습니다",
         "summary_issues_generated_plural": "깃허브 이슈들이 생성되었습니다",
         "summary_issues_generated_none": "생성된 깃허브 이슈가 없습니다",
         "summary_duplicate_issues_avoided_singular": "깃허브 이슈의 중복 생성이 방지되었습니다",
         "summary_duplicate_issues_avoided_plural": "깃허브 이슈들의 중복 생성이 방지되었습니다",
         "info_duplicate_issue_avoided": "정보: 중복 이슈 생성이 방지되었습니다",
         "error_cannot_specify_ni_xi": "오류: --ni 와 --xi 키워드는 동시에 사용할 수 없습니다",
         "error_is_not_file": "오류: 해당 경로는 파일이 아닙니다",
+        "error_file_already_exists": "오류: 이미 그 파일이 존재합니다",
         "error_todo_ignore_not_found": "오류: .todo-ignore 를 찾을 수 없습니다! -i 를 사용하여 다른 .ignore를 복사하시거나 --force 를 사용하여 .todo-ignore 없이 실행할 수 있습니다(권장되지 않음)",
         "error_todo_ignore_not_supported": f"오류: .todo-ignore 가 지원되지 않는 인코딩(문자)을 사용하고 있거나 존재하지 않습니다! 지원되는 인코딩: {SUPPORTED_ENCODINGS_TODOIGNORE}",
         "error_exceeded_maximum_issues": "오류: 한 번에 생성할 수 있는 최대 깃허브 이슈 생성 횟수를 초과하였으므로 해당 실행을 중단합니다",
         "warning_force_overrides_ignore": "경고: --force 옵션을 지정한다면 해당 실행에서는 .todo-ignore 가 생성한 내용들을 무시할 것입니다 (.todo-ignore 은 여전히 변경되긴 하지만, 그저 사용되지 않을 뿐입니다)",
+        "warning_file_does_not_exist": "경고: 파일이 존재하지 않습니다",
         "warning_run_with_empty_todo_ignore": "경고: .todo-ignore 이 비어있는 상태로 실행합니다 (만약 파일이 비어있지 않다면, 해당 파일의 인코딩을 확인하십시오), 해당 실행을 취소하고 싶다면 다음을 사용하세요 - ",
         "warning_run_without_todo_ignore": "경고: .todo-ignore 을 제외하고 실행합니다, 해당 실행을 취소하고 싶다면 다음을 사용하세요 -  ",
         "warning_encoding_not_supported": f"경고: 파일이 지원되지 않는 인코딩(문자)을 사용하고 있습니다, .todo-ignore 에 이 파일이 있다고 가정하고 해당 파일을 건너 뛸 것입니다 (지원되는 인코딩: {SUPPORTED_ENCODINGS_TODOIGNORE})",
         "warning_using_default_region": f"경고: 지원되지 않는 지역이 감지되었습니다, en_us(영어)를 기본값으로 둡니다. 감지된 지역:",
         "warning_using_default_os": f"경고: 지원되지 않는 운영체제가 감지되었습니다, 기본 단축키(Ctrl + C)를 사용합니다. 감지된 운영체제:",
     },
     "bu_mm": {
+        "general_done": "ပြီးပါပြီ။",
         "issue_body_reference_link": "အညွှန်း",
         "summary_title": "အနှစ်ချုပ် ခေါင်းစဉ်",
         "summary_encoding_unsupported_singular": "ကုဒ်ပြောင်းခြင်းကို ပံ့ပိုးမထားသောကြောင့် ဖိုင်ကို ကျော်သွားသည်",
         "summary_encoding_unsupported_plural": "ကုဒ်ပြောင်းခြင်းကို ပံ့ပိုးမထားသောကြောင့် ဖိုင်များကို ကျော်သွားခဲ့သည်",
         "summary_files_scanned_singular": "ဖိုင်ကို စကင်(န်)ဖတ်ခဲ့ပသည်",
         "summary_files_scanned_plural": "ဖိုင်များကို စကင်(န်)ဖတ်ခဲ့သည်။",
         "summary_issues_generated_singular": "ထုတ်ပေးသော ကိစ္စ",
         "summary_issues_generated_plural": "ထုတ်ပေးသော ကိစ္စများ",
         "summary_issues_generated_none": "မည်သည့်ပြဿနာမှ မထုတ်ပေးခဲ့ပါ",
         "summary_duplicate_issues_avoided_singular": "ထပ်တူကိစ္စကို တားဆီးခဲ့သည်",
         "summary_duplicate_issues_avoided_plural": "ထပ်တူကိစ္စများကို တားဆီးခဲ့သည်။",
         "info_duplicate_issue_avoided": "အချက်အလက်- မိတ္တူပွားခြင်းပြဿနာကို ရှောင်ကြဉ်ပါ",
         "error_cannot_specify_ni_xi": "အမှား- _ni နှင့် _xi နှစ်မျိုးလုံးကို သတ်မှတ်၍မရပါ",
         "error_is_not_file": "အမှား- သတ်မှတ်ထားသောလမ်းကြောင်းသည် ဖိုင် မဟုတ်ပါ",
+        "error_file_already_exists": "အမှား- သတ်မှတ်ထားသောဖိုင် ရှိနှင့်ပြီးဖြစ်သည်။",
         "error_todo_ignore_not_found": "အမှား- .todo-ignore မတွေ့ပါ။ အခြား .ignore ကိုကူးယူရန် -i ကိုသုံးပါ သို့မဟုတ် .todo-ignore မပါဘဲ run ရန် --force (အကြံပြုမထားပါ)",
         "error_todo_ignore_not_supported": f"အမှား- .todo-ignore သည် ပံ့ပိုးမထားသော ကုဒ်နံပါတ်ကို အသုံးပြုသည် သို့မဟုတ် မရှိပါ။ ပံ့ပိုးထားသော ကုဒ်နံပါတ်များ- {SUPPORTED_ENCODINGS_TODOIGNORE}",
         "error_exceeded_maximum_issues": "အမှား- ဤလုပ်ဆောင်မှုအတွက် ပြဿနာအများဆုံးအရေအတွက်ကို ကျော်သွားသည်၊ ယခုထွက်နေပါသည်",
         "warning_force_overrides_ignore": "သတိပေးချက်- --force သည် သင်သတ်မှတ်လိုက်သောအခါတွင် ထုတ်ပေးသည့် .todo-ignore ၏ အကြောင်းအရာများကို လျစ်လျူရှုလိမ့်မည် (.todo-ignore သည် ပြောင်းလဲနေသေးသည်၊ အသုံးသာမပြုဘဲ)",
+        "warning_file_does_not_exist": "သတိပေးချက်- ဖိုင်မရှိပါ။",
         "warning_run_with_empty_todo_ignore": "သတိပေးချက်- .todo-ignore သည် ဗလာဖြစ်သည် (ဖိုင်ဗလာမဟုတ်ပါက ၎င်း၏ကုဒ်နံပါတ်ကို စစ်ဆေးပါ) မည်သို့ပင်ဖြစ်စေ လုပ်ဆောင်နေပါသည်။ အသုံးပြုမှုကို ပယ်ဖျက်ရန် -",
         "warning_run_without_todo_ignore": "သတိပေးချက်- .todo-ignore မပါဘဲ လုပ်ဆောင်နေသည်။ အသုံးပြုမှုကို ပယ်ဖျက်ရန် -",
         "warning_encoding_not_supported": f"သတိပေးချက်- ဖိုင်သည် ပံ့ပိုးမထားသော ကုဒ်နံပါတ်ကို အသုံးပြုသည်၊ ၎င်းကို ကျော်သွားပါမည်၊ သို့သော် .todo-ignore တွင် ထည့်ရန်စဉ်းစားသည် (ပံ့ပိုးပေးထားသော ကုဒ်နံပါတ်များ- {SUPPORTED_ENCODINGS_TODO_CHECK})",
         "warning_using_default_region": f"သတိပေးချက်- ပံ့ပိုးမထားသော ဒေသကို တွေ့ရှိပြီး en_us သို့ ပုံသေသတ်မှတ်ထားသည်။ တွေ့ရှိထားသော ဒေသ-",
         "warning_using_default_os": f"သတိပေးချက်- ပံ့ပိုးမထားသော OS ကို တွေ့ရှိခဲ့ပြီး မပုံသေဖြတ်လမ်းကို အသုံးပြုပါမည်။ တွေ့ရှိထားသော OS-",
     },
     "default": {"shell_sigint": "CTRL + C"},
```

### Comparing `todo_or_not-0.8.8b0/todo_or_not/todo_check.py` & `todo_or_not-0.9.1/todo_or_not/todo_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import os
 import json
 import hashlib
 import subprocess
 import sys
 
 from pathlib import Path
@@ -13,14 +14,16 @@
 from todo_or_not.localize import LOCALIZE  # todoon
 from todo_or_not.localize import SUPPORTED_ENCODINGS_TODOIGNORE  # todoon
 from todo_or_not.localize import SUPPORTED_ENCODINGS_TODO_CHECK  # todoon
 
 MAXIMUM_ISSUES_GENERATED = os.environ.get("MAXIMUM_ISSUES_GENERATED", "8")
 PERTINENT_LINE_LIMIT = os.environ.get("PERTINENT_LINE_LIMIT", "8")
 
+todoon_app = typer.Typer(name="todoon")  # todoon
+
 
 def get_project_dir():
     return os.getcwd()
 
 
 def get_todo_ignore_path():  # todoon
     return os.path.join(get_project_dir(), ".todo-ignore")  # todoon
@@ -36,15 +39,15 @@
 
 def get_region():
     region = os.environ.get("REGION", "en_us")
 
     # Validate that we support the region, otherwise default to something we have
     if region not in LOCALIZE:
         print(
-            LOCALIZE[REGION]["warning_using_default_region"],  # TODO Localization | New target for #localization
+            LOCALIZE["en_us"]["warning_using_default_region"],
             region,
             file=sys.stderr,
         )
         region = "en_us"
 
     return region
 
@@ -52,26 +55,23 @@
 def get_os():
     _os = os.environ.get("OS", "default")
     _os = _os.lower()
 
     # Validate that we support the region, otherwise default to something we have
     if _os not in LOCALIZE:
         print(
-            LOCALIZE[REGION]["warning_using_default_os"],  # TODO Localization | New target for #localization
+            LOCALIZE[get_region()]["warning_using_default_os"],
             _os,
             file=sys.stderr,
         )
         _os = "default"
 
     return _os
 
 
-REGION = get_region()
-
-
 class Hit:
     def __init__(
             self,
             source_file: str,
             source_line: int,
             found_keys: list[str],
             pertinent_lines: list[str],
@@ -199,15 +199,15 @@
         reference_file = self.source_file.split(":")[0]
 
         reference_uri = f"{repo_uri}/blob/{github_ref}/{reference_file}"
 
         body = (
             f"## {self if self.structured_body is None else self.structured_body}\n\n"
             f"{self.get_pertinent_lines()}\n\n"
-            f"{LOCALIZE[REGION]['issue_body_reference_link']}: <a href=\"{reference_uri}\">{self.source_file}</a>"
+            f"{LOCALIZE[get_region()]['issue_body_reference_link']}: <a href=\"{reference_uri}\">{self.source_file}</a>"
         )
 
         # Sanitize @ to prevent abuse
         body.replace("@", "@<!-- -->")
 
         api_call = [
             "gh",
@@ -319,15 +319,15 @@
                         _trigger_line,
                     )
                     output.append(_hit)
 
     else:
         if verbose:
             print(
-                LOCALIZE[REGION]["warning_encoding_not_supported"],
+                LOCALIZE[get_region()]["warning_encoding_not_supported"],
                 "\n * ",
                 filename,
                 file=sys.stderr,
             )
 
     return output, use_encoding
 
@@ -389,15 +389,15 @@
     :param _supported_encodings: A list of supported encodings e.g. `['utf-8', 'iso-8859-1', 'iso']`
     :return: The encoding of the target file if found, None if no supported encoding could be found
     """
     try:
         assert os.path.isfile(_target_path)
     except AssertionError:
         print(
-            f"{LOCALIZE[REGION]['error_is_not_file']}: {_target_path}", file=sys.stderr
+            f"{LOCALIZE[get_region()]['error_is_not_file']}: {_target_path}", file=sys.stderr
         )
         return None
 
     # Try to read the file in a supported encoding
     _use_encoding = None
     for encoding in _supported_encodings:
         try:
@@ -413,31 +413,45 @@
         # If able to open, use this encoding and exit the search for valid encoding
         _use_encoding = encoding
         break
 
     return _use_encoding
 
 
-def main(
-        files: Annotated[Optional[List[str]], typer.Argument()] = None,
-        mode: str = "print",
-        silent: bool = False,
-        force: bool = False,
-        verbose: bool = False,
-        ni: Annotated[
+# fmt: off
+@todoon_app.command(  # todoon
+    help="Checks files for occurrences of TODO or FIXME and reports them for use with automation or other development operations.")  # todoon
+def todoon(  # todoon
+        files: Annotated[
             Optional[List[str]],
-            Option(help="Copy the contents of another file into a new .todo-ignore"),  # todoon
-        ] = None,
-        xi: Annotated[
-            Optional[List[str]],
-            Option(help="Copy the contents of another file into an existing .todo-ignore"),  # todoon
-        ] = None,
+            typer.Argument(
+                help="If specified, only these [FILES] will be scanned for TODOs and FIXMEs. "  # todoon
+                     "Otherwise, all files in the current working directory except for those "
+                     "specified in .todo-ignore will be scanned.")] = None,  # todoon
+        print_mode: Annotated[
+            bool,
+            typer.Option("--print/--issue", "-p/-i",
+                help="Whether to print the discovered TODOs and FIXMEs to stderr or to try"  # todoon
+                     " an generate GitHub issues")] = True,
+        silent: Annotated[
+            bool,
+            typer.Option("--silent/", "-s/",
+                help="If specified, todoon will not exit with an error code even when TODOs and/or "  # todoon
+                     "FIXMEs are detected")] = False,  # todoon
+        force: Annotated[
+            bool,
+            typer.Option("--force/", "-f/",
+                help="If specified, the .todo-ignore file will not be used. NOT RECOMMENDED")] = False,  # todoon
+        verbose: Annotated[
+            bool,
+            typer.Option("--verbose/", "-v/",
+                help="If specified, todoon will not to print lengthy or numerous messages"  # todoon
+                     " (like each encoding failure)")] = False,
 ):
-    mode = mode.lower()
-
+# fmt: on
     targets = []
     ignored_files = []
     ignored_dirs = []
 
     use_specified_files = False
 
     if files is not None and len(files) > 0:
@@ -452,59 +466,14 @@
     os.environ["TODOON_FILES_SCANNED"] = "0"  # todoon
     os.environ["TODOON_TODOS_FOUND"] = "0"  # todoon
     os.environ["TODOON_FIXMES_FOUND"] = "0"  # todoon
     os.environ["TODOON_ENCODING_ERRORS"] = "0"  # todoon
     os.environ["TODOON_ISSUES_GENERATED"] = "0"  # todoon
     os.environ["TODOON_DUPLICATE_ISSUES_AVOIDED"] = "0"  # todoon
 
-    # If using specific files, no todo-ignore utils are necessary # todoon
-    if not use_specified_files:
-        # Don't worry about it if both ni and xi are none
-        if (ni is None) and (xi is None):
-            pass
-        # If using EITHER ni or ci...
-        elif xi is None and len(ni) > 0:
-            # ...check if force is used and warn the user if so
-            if force:
-                print(
-                    LOCALIZE[REGION]["warning_force_overrides_ignore"],
-                    "--ni",
-                    file=sys.stderr,
-                )
-
-            # Create new .todo-ignore # todoon
-            with open(
-                    os.path.join(get_project_dir(), ".todo-ignore"), "x", encoding="UTF-8"  # todoon
-            ) as new_todo_ignore_file:  # todoon
-                paste_contents_into_file(ni, new_todo_ignore_file)  # todoon
-
-        elif ni is None and len(xi) > 0:
-            # ...check if force is used and warn the user if so
-            if force:
-                # Check which mode is being used
-                _option = "--ni" if (len(ni) > len(xi)) else "--xi"
-                print(
-                    LOCALIZE[REGION]["warning_force_overrides_ignore"],
-                    "--xi",
-                    file=sys.stderr,
-                )
-
-            # Update append to the existing .todo-ignore # todoon
-            with open(
-                    os.path.join(get_project_dir(), ".todo-ignore"),  # todoon
-                    "a+",
-                    encoding="UTF-8",
-            ) as new_todo_ignore_file:  # todoon
-                paste_contents_into_file(xi, new_todo_ignore_file)  # todoon
-
-        # Don't allow the use of ni and ci at the same time
-        elif (len(ni) > 0) and (len(xi) > 0):
-            print(LOCALIZE[REGION]["error_cannot_specify_ni_xi"], file=sys.stderr)
-            exit(1)
-
     #############################################
     # Parse .todo-ignore # todoon
     #############################################
 
     # If using specific files, no todo-ignore parsing is necessary # todoon
     if not use_specified_files:
         os.environ["TODOON_STATUS"] = "parsing-todo-ignore"  # todoon
@@ -514,15 +483,15 @@
             use_encoding = get_encoding(
                 get_todo_ignore_path(), SUPPORTED_ENCODINGS_TODOIGNORE  # todoon
             )
 
             # If we weren't able to find a file in a supported encoding, program must exit
             if use_encoding is None:
                 print(
-                    LOCALIZE[REGION]["error_todo_ignore_not_supported"], file=sys.stderr  # todoon
+                    LOCALIZE[get_region()]["error_todo_ignore_not_supported"], file=sys.stderr  # todoon
                 )
                 exit(1)
 
             # ... actually do the reading of the .todo-ignore # todoon
             with open(
                     get_todo_ignore_path(), "r", encoding=use_encoding  # todoon
             ) as _ignore:
@@ -531,33 +500,38 @@
                         if line.endswith("\n"):
                             cur_name = line[:-1]
                         else:
                             cur_name = line
 
                         cur_path = os.path.join(get_project_dir(), cur_name)
 
+                        # Resolve wildcards
+                        if '*' in cur_path:
+                            ignored_files.extend(glob.glob(cur_path, recursive=True))
+
                         if os.path.isfile(cur_path):
                             ignored_files.append(cur_path)
 
                         if os.path.isdir(cur_path):
                             ignored_dirs.append(cur_path)
 
                 if len(ignored_files) == 0 and len(ignored_dirs) == 0:
                     print(
-                        LOCALIZE[REGION][
+                        LOCALIZE[get_region()][
                             "warning_run_with_empty_todo_ignore"  # todoon
                         ],
                         file=sys.stderr,
                     )
 
                 # Ignore the .todo-ignore itself # todoon
                 ignored_files.append(os.path.abspath(_ignore.name))
         else:
             print(
-                f"{LOCALIZE[REGION]['error_todo_ignore_not_found']}[{LOCALIZE[get_os()]['shell_sigint']}]",  # todoon
+                f"{LOCALIZE[get_region()]['error_todo_ignore_not_found']}"  # todoon
+                f"[{LOCALIZE[get_os()]['shell_sigint']}]",
                 file=sys.stderr,
             )
 
     #############################################
     # Collect files to scan
     #############################################
 
@@ -619,15 +593,15 @@
     # Preventing duplicate issues
     #############################################
 
     # When pinging for all queries, their titles are hashed and saved here. This is for checking for duplicate issues
     existing_issues_hashed = []
 
     # Collect all the issues that the bot has so far submitted to check for duplicates
-    if mode == "issue":
+    if not print_mode:
         os.environ["TODOON_STATUS"] = "collecting-issues"  # todoon
         todoon_created_issues = get_bot_submitted_issues()  # todoon
 
         for issue in todoon_created_issues:  # todoon
             existing_issues_hashed.append(_hash(issue["title"]))
 
     #############################################
@@ -671,90 +645,93 @@
                 number_of_hits += 1
                 number_of_todo += 1 if "todo" in hit.found_keys else 0  # todoon
                 number_of_fixme += 1 if "fixme" in hit.found_keys else 0  # todoon
 
                 #############################################
                 # Special handling for the ISSUE mode
 
-                if mode == "issue":
+                if not print_mode:
                     _this_hit_hashed = _hash(hit.get_title())
 
                     # Check if the app already created this hit's title
                     if _this_hit_hashed not in existing_issues_hashed:
 
                         # Limit the number of issues created in one run
                         if number_of_issues < int(MAXIMUM_ISSUES_GENERATED):
                             hit.generate_issue()
                             number_of_issues += 1
                         else:
                             print(
-                                LOCALIZE[REGION][
+                                LOCALIZE[get_region()][
                                     "error_exceeded_maximum_issues"
                                 ],
                                 file=sys.stderr,
                             )
                             exit(1)
                     # If this title already exists, notify but do not halt
                     else:
                         print(
-                            f"{LOCALIZE[REGION]['info_duplicate_issue_avoided']}: {hit}",
+                            f"{LOCALIZE[get_region()]['info_duplicate_issue_avoided']}: {hit}",
                             file=sys.stderr,
                         )
 
                 #############################################
                 # If not in ISSUE mode, print hit to stderr
 
                 else:
                     print(hit, file=sys.stderr)
 
     #############################################
     # Summarize the run of todo-check  # todoon
     #############################################
 
-    summary = f"\n##########################\n# {LOCALIZE[REGION]['summary_title']}\n"
+    summary = f"\n##########################\n# {LOCALIZE[get_region()]['summary_title']}\n"
     # Mode the tool was run in
-    summary += f"# ({mode.upper()} MODE)\n"
+    if print_mode:
+        summary += "# (PRINT MODE)\n"
+    else:
+        summary += "# (ISSUE MODE)\n"
 
     # Number of TODOs and FIXMEs found  # todoon
     summary += f"# {number_of_todo} TODO | {number_of_fixme} FIXME\n"  # todoon
 
     # Number of encoding failures
     if number_of_encoding_failures > 1:
-        summary += f"# {number_of_encoding_failures} {LOCALIZE[REGION]['summary_encoding_unsupported_plural']}\n"
+        summary += f"# {number_of_encoding_failures} {LOCALIZE[get_region()]['summary_encoding_unsupported_plural']}\n"
     elif number_of_encoding_failures == 1:
-        summary += f"# {number_of_encoding_failures} {LOCALIZE[REGION]['summary_encoding_unsupported_singular']}\n"
+        summary += f"# {number_of_encoding_failures} {LOCALIZE[get_region()]['summary_encoding_unsupported_singular']}\n"
 
     # Total number of files scanned
     if number_of_files_scanned > 1:
         summary += (f"# {number_of_files_scanned} "
-                    f"{LOCALIZE[REGION]['summary_files_scanned_plural']}\n")  # TODO Localization | New target for #localization
+                    f"{LOCALIZE[get_region()]['summary_files_scanned_plural']}\n")
     elif number_of_files_scanned == 1:
         summary += (f"# {number_of_files_scanned} "
-                    f"{LOCALIZE[REGION]['summary_files_scanned_singular']}\n")  # TODO Localization | New target for #localization
+                    f"{LOCALIZE[get_region()]['summary_files_scanned_singular']}\n")
 
-    # Number of issues (if any) that were generated
-    if mode == "issue":
+        # Number of issues (if any) that were generated
+    if not print_mode:
         # Total number of issues generated
         if number_of_issues > 1:
             summary += (f"# {number_of_issues} "
-                        f"{LOCALIZE[REGION]['summary_issues_generated_plural']}\n")  # TODO Localization | New target for #localization
+                        f"{LOCALIZE[get_region()]['summary_issues_generated_plural']}\n")
         elif number_of_issues == 1:
             summary += (f"# {number_of_issues} "
-                        f"{LOCALIZE[REGION]['summary_issues_generated_singular']}\n")  # TODO Localization | New target for #localization
+                        f"{LOCALIZE[get_region()]['summary_issues_generated_singular']}\n")
         else:
             summary += (f"# "
-                        f"{LOCALIZE[REGION]['summary_issues_generated_none']}\n")  # TODO Localization | New target for #localization
+                        f"{LOCALIZE[get_region()]['summary_issues_generated_none']}\n")
 
-        # Total number of duplicate issues avoided
+            # Total number of duplicate issues avoided
         if number_of_duplicate_issues_avoided > 1:
             summary += (f"# {number_of_duplicate_issues_avoided} "
-                        f"{LOCALIZE[REGION]['summary_duplicate_issues_avoided_plural']}\n")  # TODO Localization | New target for #localization
+                        f"{LOCALIZE[get_region()]['summary_duplicate_issues_avoided_plural']}\n")
         elif number_of_duplicate_issues_avoided == 1:
             summary += (f"# {number_of_duplicate_issues_avoided} "
-                        f"{LOCALIZE[REGION]['summary_duplicate_issues_avoided_singular']}\n")  # TODO Localization | New target for #localization
+                        f"{LOCALIZE[get_region()]['summary_duplicate_issues_avoided_singular']}\n")
 
     summary += "##########################\n"
 
     os.environ["TODOON_STATUS"] = "finished"  # todoon
     os.environ["TODOON_PROGRESS"] = "100.0"  # todoon
     os.environ["TODOON_FILES_SCANNED"] = str(number_of_files_scanned)  # todoon
     os.environ["TODOON_TODOS_FOUND"] = str(number_of_todo)  # todoon
@@ -768,13 +745,84 @@
     print(summary, file=sys.stderr)
 
     # Fail if any hits were found and we are not in silent mode
     if number_of_hits > 0 and not silent:
         exit(1)
 
 
-def typer_main():
-    run(main)
+# fmt: off
+@todoon_app.command(help="Small utility for generating a .todo-ignore file")  # todoon
+def todo_ignore_util(  # todoon
+        sources: Annotated[
+            Optional[List[str]],
+            typer.Argument(
+                help="(default) [with -p] Files whose contents will be added to the .todo-ignore file.\n\n          "  # todoon
+                     "[with -t] Lines of text to be added to the .todo-ignore file.")] = None,  # todoon
+        create_mode: Annotated[
+            bool,
+            typer.Option("--create/--update", "-c/-u",
+                help="Whether to create a new .todo-ignore file or update an existing one")] = True,  # todoon
+        source_is_text: Annotated[bool, typer.Option("--source-text/--source-paths", "-t/-p",
+                                                     help="Whether to treat SOURCES as text or as file paths.")] = True
+):
+#fmt: on
+    todoignore_path = os.path.join(os.getcwd(), ".todo-ignore")  # todoon
+    output = []
+
+    if create_mode:
+        access_mode = "x"
+    else:
+        access_mode = "a"
+
+    if source_is_text:
+        if sources is not None and len(sources) > 0:
+            output.extend(sources)
+    else:
+        if sources is not None and len(sources) > 0:
+            for file in sources:
+                _path = os.path.join(os.getcwd(), file)
+
+                try:
+                    with (open(_path, "r")) as current:
+                        _current_lines = current.readlines()
+
+                        for line in _current_lines:
+                            line = line.strip()
+
+                            if len(line) > 0:
+                                output.append(line)
+                except FileNotFoundError:
+                    print(LOCALIZE[get_region()]["warning_file_does_not_exist"], _path, file=sys.stderr)
+
+    try:
+        with open(todoignore_path, access_mode) as target:  # todoon
+            previous = None
+            for line in output:
+                if previous != line[0]:
+                    target.write('\n')
+                previous = line[0]
+
+                target.write(f"{line}\n")
+    except FileNotFoundError:
+        print(
+            LOCALIZE[get_region()]["error_is_not_file"], todoignore_path, file=sys.stderr  # todoon
+        )
+        exit(1)
+    except FileExistsError:
+        print(
+            LOCALIZE[get_region()]["error_file_already_exists"], todoignore_path, file=sys.stderr  # todoon
+        )
+        exit(1)
+
+    print(LOCALIZE[get_region()]["general_done"])
+
+
+def typer_todoon():  # todoon
+    run(todoon)  # todoon
+
+
+def typer_todo_ignore_util():  # todoon
+    run(todo_ignore_util)  # todoon
 
 
 if __name__ == "__main__":
-    typer_main()
+    todoon_app()  # todoon
```

