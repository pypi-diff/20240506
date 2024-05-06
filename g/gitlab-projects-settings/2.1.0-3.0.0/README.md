# Comparing `tmp/gitlab_projects_settings-2.1.0.tar.gz` & `tmp/gitlab_projects_settings-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-2.1.0.tar", last modified: Sun Apr 28 18:42:00 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-3.0.0.tar", last modified: Mon May  6 01:25:25 2024, max compression
```

## Comparing `gitlab_projects_settings-2.1.0.tar` & `gitlab_projects_settings-3.0.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.832775 gitlab_projects_settings-2.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.825775 gitlab_projects_settings-2.1.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     7153 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.825775 gitlab_projects_settings-2.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     2480 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-28 18:42:00.832775 gitlab_projects_settings-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3483 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.832775 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-28 18:42:00.000000 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-28 18:42:00.000000 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 18:42:00.000000 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-28 18:42:00.000000 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-28 18:42:00.000000 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-28 18:42:00.000000 gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.828776 gitlab_projects_settings-2.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 18:42:00.832775 gitlab_projects_settings-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.828776 gitlab_projects_settings-2.1.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.829776 gitlab_projects_settings-2.1.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10018 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     5497 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.829776 gitlab_projects_settings-2.1.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11891 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.830776 gitlab_projects_settings-2.1.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.831776 gitlab_projects_settings-2.1.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 18:42:00.831776 gitlab_projects_settings-2.1.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-28 18:41:53.000000 gitlab_projects_settings-2.1.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.484876 gitlab_projects_settings-3.0.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     7147 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.484876 gitlab_projects_settings-3.0.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     3518 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5642 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5642 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      946 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 01:25:25.000000 gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.487877 gitlab_projects_settings-3.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 01:25:25.491876 gitlab_projects_settings-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.487877 gitlab_projects_settings-3.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.488876 gitlab_projects_settings-3.0.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14204 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     6683 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.488876 gitlab_projects_settings-3.0.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14867 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.489876 gitlab_projects_settings-3.0.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.489876 gitlab_projects_settings-3.0.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.490877 gitlab_projects_settings-3.0.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:25:25.490877 gitlab_projects_settings-3.0.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-06 01:25:18.000000 gitlab_projects_settings-3.0.0/src/types/namespaces.py
```

### Comparing `gitlab_projects_settings-2.1.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-3.0.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/.chglog/changelog.sh` & `gitlab_projects_settings-3.0.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/.chglog/config.yml` & `gitlab_projects_settings-3.0.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/.gitlab-ci.yml` & `gitlab_projects_settings-3.0.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -49,51 +49,14 @@
     - sh ./.chglog/changelog.sh --clean
     - git add -v ./CHANGELOG.md
     - git commit --amend --no-edit
     - git tag -f -m '' "${tag}"
   rules:
     - if: $CI_LOCAL
 
-readme:
-  stage: development
-  image: local:silent
-  script:
-    - |
-      export COLUMNS=120
-      mkdir -p ./.tmp/
-      PACKAGE_NAME=$(grep '^PROJECT_NAME =' ./setup.py | cut -d"'" -f2)
-      {
-        echo ''
-        echo '```yaml'
-        alignments='[ ]\{2,\}'
-        argument='[[:alnum:]][[:alnum:]_-]\{0,\}'
-        letter='[[:alnum:]_]\{1\}'
-        parameter='[-]\{1,2\}[[:alnum:]][[:alnum:]_-]\{0,\}'
-        word='[[:alnum:]_-]\{1,\}'
-        "${PACKAGE_NAME}" --help \
-          | sed '1d; $d' \
-          | sed "s/^\(  ${parameter} ${word}${alignments}\)/\1# /g" \
-          | sed "s/^\(  ${parameter}${alignments}\)/\1# /g" \
-          | sed "s/^\(  ${parameter}, ${parameter}${alignments}\)/\1# /g" \
-          | sed "s/^\(  ${argument}${alignments}\)/\1# /g"
-        echo '```'
-        echo ''
-      } >./.tmp/README.help.tmp
-    - |
-      lead='^<!-- readme-help-start -->$'
-      tail='^<!-- readme-help-stop -->$'
-      sed -i "/${lead}/,/${tail}/{ /${lead}/{ p; r ./.tmp/README.help.tmp
-        }; /${tail}/p; d }"  ./README.md | head -n 100
-    - rm -f ./.tmp/README.help.tmp
-    - |
-      git -c color.diff=always --no-pager diff ./README.md | grep --color=never '.' && echo ''
-      echo  ' > README: Updated successfully'
-  rules:
-    - if: $CI_LOCAL
-
 # =============================================================================
 # Stage: prepare
 
 codestyle:
   stage: prepare
   image: registry.gitlab.com/adriandc/gitlabci-local/gitlabci-local:codestyle
   script:
@@ -188,14 +151,51 @@
   image: local:quiet
   script:
     - pipx uninstall $(ls -1 ./dist/*.whl | cut -d'/' -f3 | cut -d'-' -f1) || true
     - pipx install --force ./dist/*.whl
   rules:
     - if: $CI_LOCAL
 
+readme:
+  stage: build
+  image: local:silent
+  script:
+    - |
+      export COLUMNS=120
+      mkdir -p ./.tmp/
+      PACKAGE_NAME=$(grep '^PROJECT_NAME =' ./setup.py | cut -d"'" -f2)
+      {
+        echo ''
+        echo '```yaml'
+        alignments='[ ]\{2,\}'
+        argument='[[:alnum:]][[:alnum:]_-]\{0,\}'
+        letter='[[:alnum:]_]\{1\}'
+        parameter='[-]\{1,2\}[[:alnum:]][[:alnum:]_-]\{0,\}'
+        word='[[:alnum:]_-]\{1,\}'
+        "${PACKAGE_NAME}" --help \
+          | sed '1d; $d' \
+          | sed "s/^\(  ${parameter} ${word}${alignments}\)/\1# /g" \
+          | sed "s/^\(  ${parameter}${alignments}\)/\1# /g" \
+          | sed "s/^\(  ${parameter}, ${parameter}${alignments}\)/\1# /g" \
+          | sed "s/^\(  ${argument}${alignments}\)/\1# /g"
+        echo '```'
+        echo ''
+      } >./.tmp/README.help.tmp
+    - |
+      lead='^<!-- readme-help-start -->$'
+      tail='^<!-- readme-help-stop -->$'
+      sed -i "/${lead}/,/${tail}/{ /${lead}/{ p; r ./.tmp/README.help.tmp
+        }; /${tail}/p; d }"  ./README.md | head -n 100
+    - rm -f ./.tmp/README.help.tmp
+    - |
+      git -c color.diff=always --no-pager diff ./README.md | grep --color=never '.' && echo ''
+      echo  ' > README: Updated successfully'
+  rules:
+    - if: $CI_LOCAL
+
 # =============================================================================
 # Stage: deploy
 
 deploy:release:
   stage: deploy
   image: registry.gitlab.com/adriandc/gitlabci-local/gitlabci-local:deploy
   needs:
```

### Comparing `gitlab_projects_settings-2.1.0/.style.yapf` & `gitlab_projects_settings-3.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/.vscode/extensions.json` & `gitlab_projects_settings-3.0.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/.vscode/settings.json` & `gitlab_projects_settings-3.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/CHANGELOG.md` & `gitlab_projects_settings-3.0.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,38 @@
 
+<a name="3.0.0"></a>
+## [3.0.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/2.1.0...3.0.0) (2024-05-06)
+
+### Bug Fixes
+
+* **entrypoint:** resolve support for private user namespaces
+* **entrypoint:** detect if GitLab actions can continue
+* **entrypoint:** enforce against missing '.description' values
+* **gitlab:** enforce 'group_delete' usage in '--dry-run' mode
+* **gitlab:** delay groups deletion by 10s and projects by 5s
+* **gitlab:** get all branches and tags upon 'list()' calls
+* **gitlab:** get all members in 'project_reset_members'
+
+### Ci
+
+* **gitlab-ci:** move 'readme' job after 'build' and local 'install'
+
+### Cleanups
+
+* **gitlab:** minor comments changes in 'project_reset_features'
+
+### Features
+
+* **entrypoint:** preserve main group description if exists
+* **entrypoint:** always flush progress output logs
+* **gitlab:** detect multiple branches to keep 'Merge requests'
+* **gitlab:** detect 'Token Access' usage for 'CI/CD' features
+* **namespaces:** migrate 'Helper' class to 'Namespaces' class
+
+
 <a name="2.1.0"></a>
 ## [2.1.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/2.0.2...2.1.0) (2024-04-28)
 
 ### Bug Fixes
 
 * **entrypoint:** fix project '--update-description' logs output
```

### Comparing `gitlab_projects_settings-2.1.0/LICENSE` & `gitlab_projects_settings-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/PKG-INFO` & `gitlab_projects_settings-3.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 2.1.0
+Version: 3.0.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -60,16 +60,17 @@
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
                                 [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
-                                [--set-description TEXT] [--update-description] [--protect-branches]
-                                [--protect-tags LEVEL]
+                                [--set-description TEXT] [--update-description] [--run-housekeeping]
+                                [--archive-project | --unarchive-project] [--delete-group] [--delete-project]
+                                [--protect-branches] [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
   -h, --help              # Show this help message
   --version               # Show the current version
@@ -86,21 +87,28 @@
 general settings arguments:
   --reset-features        # Reset features of GitLab projects based on usage
   --reset-members         # Reset members of GitLab projects and groups
   --set-avatar FILE       # Set avatar of GitLab projects and groups
   --set-description TEXT  # Set description of GitLab projects and groups
   --update-description    # Update description of GitLab projects and groups automatically
 
+advanced settings arguments:
+  --run-housekeeping      # Run housekeeping of project or projects GitLab in groups
+  --archive-project       # Archive project or projects in GitLab groups
+  --unarchive-project     # Unarchive project or projects in GitLab groups
+  --delete-group          # Delete group or groups in GitLab groups
+  --delete-project        # Delete project or projects in GitLab groups
+
 repository settings arguments:
   --protect-branches      # Protect branches with default master/main, develop and staging
   --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
   gitlab                  # GitLab URL (default: https://gitlab.com)
-  path                    # GitLab group or project path
+  path                    # GitLab group, user namespace or project path
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
```

### Comparing `gitlab_projects_settings-2.1.0/README.md` & `gitlab_projects_settings-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
                                 [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
-                                [--set-description TEXT] [--update-description] [--protect-branches]
-                                [--protect-tags LEVEL]
+                                [--set-description TEXT] [--update-description] [--run-housekeeping]
+                                [--archive-project | --unarchive-project] [--delete-group] [--delete-project]
+                                [--protect-branches] [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
   -h, --help              # Show this help message
   --version               # Show the current version
@@ -52,21 +53,28 @@
 general settings arguments:
   --reset-features        # Reset features of GitLab projects based on usage
   --reset-members         # Reset members of GitLab projects and groups
   --set-avatar FILE       # Set avatar of GitLab projects and groups
   --set-description TEXT  # Set description of GitLab projects and groups
   --update-description    # Update description of GitLab projects and groups automatically
 
+advanced settings arguments:
+  --run-housekeeping      # Run housekeeping of project or projects GitLab in groups
+  --archive-project       # Archive project or projects in GitLab groups
+  --unarchive-project     # Unarchive project or projects in GitLab groups
+  --delete-group          # Delete group or groups in GitLab groups
+  --delete-project        # Delete project or projects in GitLab groups
+
 repository settings arguments:
   --protect-branches      # Protect branches with default master/main, develop and staging
   --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
   gitlab                  # GitLab URL (default: https://gitlab.com)
-  path                    # GitLab group or project path
+  path                    # GitLab group, user namespace or project path
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
```

### Comparing `gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 2.1.0
+Version: 3.0.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -60,16 +60,17 @@
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [-t TOKEN] [--dry-run] [--exclude-group] [--exclude-subgroups]
                                 [--exclude-projects] [--reset-features] [--reset-members] [--set-avatar FILE]
-                                [--set-description TEXT] [--update-description] [--protect-branches]
-                                [--protect-tags LEVEL]
+                                [--set-description TEXT] [--update-description] [--run-housekeeping]
+                                [--archive-project | --unarchive-project] [--delete-group] [--delete-project]
+                                [--protect-branches] [--protect-tags LEVEL]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
   -h, --help              # Show this help message
   --version               # Show the current version
@@ -86,21 +87,28 @@
 general settings arguments:
   --reset-features        # Reset features of GitLab projects based on usage
   --reset-members         # Reset members of GitLab projects and groups
   --set-avatar FILE       # Set avatar of GitLab projects and groups
   --set-description TEXT  # Set description of GitLab projects and groups
   --update-description    # Update description of GitLab projects and groups automatically
 
+advanced settings arguments:
+  --run-housekeeping      # Run housekeeping of project or projects GitLab in groups
+  --archive-project       # Archive project or projects in GitLab groups
+  --unarchive-project     # Unarchive project or projects in GitLab groups
+  --delete-group          # Delete group or groups in GitLab groups
+  --delete-project        # Delete project or projects in GitLab groups
+
 repository settings arguments:
   --protect-branches      # Protect branches with default master/main, develop and staging
   --protect-tags LEVEL    # Protect tags at level [no-one,admins,maintainers,developers]
 
 positional arguments:
   gitlab                  # GitLab URL (default: https://gitlab.com)
-  path                    # GitLab group or project path
+  path                    # GitLab group, user namespace or project path
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
```

### Comparing `gitlab_projects_settings-2.1.0/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-3.0.0/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 src/features/gitlab.py
 src/package/__init__.py
 src/package/bundle.py
 src/package/version.py
 src/prints/__init__.py
 src/prints/colors.py
 src/system/__init__.py
-src/system/platform.py
+src/system/platform.py
+src/types/__init__.py
+src/types/namespaces.py
```

### Comparing `gitlab_projects_settings-2.1.0/setup.py` & `gitlab_projects_settings-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/src/cli/entrypoint.py` & `gitlab_projects_settings-3.0.0/src/cli/entrypoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from argparse import Namespace
 
 # Modules libraries
 from gitlab.exceptions import GitlabGetError
-from gitlab.v4.objects import Group, Project
+from gitlab.v4.objects import Group as GitLabGroup, Project as GitLabProject, User as GitLabUser
 
 # Components
 from ..features.gitlab import GitLabFeature
 from ..prints.colors import Colors
 from ..system.platform import Platform
+from ..types.namespaces import Namespaces
 
 # Entrypoint class, pylint: disable=too-few-public-methods
 class Entrypoint:
 
-    # CLI
+    # CLI, pylint: disable=too-many-branches
     @staticmethod
     def cli(options: Namespace) -> bool:
 
         # Variables
-        group: Group = None
-        project: Project = None
+        group: GitLabGroup = None
+        project: GitLabProject = None
+        user: GitLabUser = None
 
         # Header
         print(' ')
 
         # GitLab client
         gitlab = GitLabFeature(
             options.gitlab,
@@ -42,94 +44,129 @@
             group = gitlab.group(options.path)
             print(f'{Colors.BOLD} - GitLab group: '
                   f'{Colors.GREEN}{group.full_path}'
                   f'{Colors.CYAN} ({group.description})'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
-        except GitlabGetError:
-            project = gitlab.project(options.path)
-            print(f'{Colors.BOLD} - GitLab project: '
-                  f'{Colors.GREEN}{project.path_with_namespace}'
-                  f'{Colors.CYAN} ({project.description})'
-                  f'{Colors.RESET}')
-            print(' ')
-            Platform.flush()
+        except GitlabGetError as exception:
+            try:
+                if '/' in options.path:
+                    raise TypeError from exception
+                user = gitlab.user(options.path)
+                namespace = gitlab.namespace(user.namespace_id)
+                print(f'{Colors.BOLD} - GitLab user namespace: '
+                      f'{Colors.GREEN}{namespace.full_path}'
+                      f'{Colors.CYAN} ({namespace.name})'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
+            except (GitlabGetError, TypeError):
+                project = gitlab.project(options.path)
+                print(f'{Colors.BOLD} - GitLab project: '
+                      f'{Colors.GREEN}{project.path_with_namespace}'
+                      f'{Colors.CYAN} ({project.description})'
+                      f'{Colors.RESET}')
+                print(' ')
+                Platform.flush()
 
         # Handle single project
         if project:
             Entrypoint.project(
                 options,
                 gitlab,
                 project.id,
             )
 
         # Handle group recursively
         elif group:
 
             # Handle group
             if not options.exclude_group:
-                Entrypoint.group(
-                    options,
-                    gitlab,
-                    group.id,
-                )
+                if not Entrypoint.group(
+                        options,
+                        gitlab,
+                        group.id,
+                ):
+                    return False
 
             # Iterate through subgroups
             if not options.exclude_subgroups:
                 for group_subgroup in sorted(
                         group.descendant_groups.list(
                             get_all=True,
                             include_subgroups=True,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.full_path,
                 ):
-                    Entrypoint.group(
-                        options,
-                        gitlab,
-                        group_subgroup.id,
-                        True,
-                    )
+                    if not Entrypoint.group(
+                            options,
+                            gitlab,
+                            group_subgroup.id,
+                            True,
+                    ):
+                        return False
 
             # Iterate through projects
             if not options.exclude_projects:
                 for group_project in sorted(
                         group.projects.list(
                             get_all=True,
                             include_subgroups=not options.exclude_subgroups,
                             order_by='path',
                             sort='asc',
                         ),
                         key=lambda item: item.path_with_namespace,
                 ):
-                    Entrypoint.project(
-                        options,
-                        gitlab,
-                        group_project.id,
-                    )
+                    if not Entrypoint.project(
+                            options,
+                            gitlab,
+                            group_project.id,
+                    ):
+                        return False
+
+        # Handle user recursively
+        elif user:
+
+            # Iterate through projects
+            if not options.exclude_projects:
+                for user_project in sorted(
+                        user.projects.list(
+                            get_all=True,
+                            order_by='path',
+                            sort='asc',
+                        ),
+                        key=lambda item: item.path_with_namespace,
+                ):
+                    if not Entrypoint.project(
+                            options,
+                            gitlab,
+                            user_project.id,
+                    ):
+                        return False
 
         # Result
         return True
 
     # Group
     @staticmethod
     def group(
         options: Namespace,
         gitlab: GitLabFeature,
         criteria: str,
         subgroup: bool = False,
-    ) -> None:
+    ) -> bool:
 
         # Acquire group
         group = gitlab.group(criteria)
 
         # Acquire parent group
-        parent_group: Group = None
+        parent_group: GitLabGroup = None
         if group.parent_id:
             parent_group = gitlab.group(group.parent_id)
 
         # Get parent description
         parent_description: str = ''
         parent_name: str = ''
         if parent_group:
@@ -138,153 +175,227 @@
 
         # Show group details
         group_type = 'subgroup' if subgroup else 'group'
         print(f'{Colors.BOLD} - GitLab {group_type}: '
               f'{Colors.YELLOW_LIGHT}{group.full_path} '
               f'{Colors.CYAN}({group.description})'
               f'{Colors.RESET}')
+        Platform.flush()
+
+        # Delete group
+        if options.delete_group:
+            gitlab.group_delete(criteria)
+            print(f'{Colors.BOLD}   - Delete {group_type}: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+            print(' ')
+            Platform.flush()
+            return subgroup
 
         # Set group description
         if options.set_description:
             gitlab.group_set_description(criteria, options.set_description)
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Update group description
         elif options.update_description:
             parent_description_text: str = ''
             if parent_name:
-                parent_description_text = ' - ' + GitLabFeature.Helper.describe(
-                    parent_description,
-                    parent_name,
+                parent_description_text = ' - ' + Namespaces.describe(
+                    name=parent_name,
+                    description=parent_description,
                 )
-            if not parent_description_text or not group.description.endswith(
-                    f'{parent_description_text}'):
-                description = f'{GitLabFeature.Helper.capitalize(group.name)}' \
-                            f'{parent_description_text}'
+            if not group.description or subgroup and ( \
+                        not parent_description_text or \
+                        not group.description.endswith(f'{parent_description_text}') \
+                    ):
+                description = f'{Namespaces.describe(name=group.name)}' \
+                              f'{parent_description_text}'
                 gitlab.group_set_description(criteria, description)
                 print(f'{Colors.BOLD}   - Updated description: '
                       f'{Colors.CYAN}{description}'
                       f'{Colors.RESET}')
+                Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Kept description: '
                       f'{Colors.GREEN}{group.description}'
                       f'{Colors.RESET}')
+                Platform.flush()
 
         # Reset group members
         if options.reset_members:
             gitlab.group_reset_members(criteria)
             print(f'{Colors.BOLD}   - Reset members: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Set group avatar
         if options.set_avatar:
             gitlab.group_set_avatar(criteria, options.set_avatar)
             print(f'{Colors.BOLD}   - Set avatar: '
                   f'{Colors.CYAN}{options.set_avatar}'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Footer
         print(' ')
         Platform.flush()
 
-    # Project, pylint: disable=too-many-branches
+        # Result
+        return True
+
+    # Project, pylint: disable=too-many-branches,too-many-statements
     @staticmethod
     def project(
         options: Namespace,
         gitlab: GitLabFeature,
         criteria: str,
-    ) -> None:
+    ) -> bool:
 
         # Acquire project
         project = gitlab.project(criteria)
 
-        # Acquire group
-        group = gitlab.group(project.namespace['id'])
-
         # Show project details
         print(f'{Colors.BOLD} - GitLab project: '
               f'{Colors.YELLOW_LIGHT}{project.path_with_namespace} '
               f'{Colors.CYAN}({project.description})'
               f'{Colors.RESET}')
+        Platform.flush()
+
+        # Delete project
+        if options.delete_project:
+            gitlab.project_delete(criteria)
+            print(f'{Colors.BOLD}   - Delete project: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+            print(' ')
+            Platform.flush()
+            return True
 
         # Set project description
         if options.set_description:
             gitlab.project_set_description(criteria, options.set_description)
             print(f'{Colors.BOLD}   - Set description: '
                   f'{Colors.CYAN}{options.set_description}'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Update project description
         elif options.update_description:
-            group_description = GitLabFeature.Helper.describe(
-                group.description,
-                group.name,
-            )
-            if not project.description.endswith(f' - {group_description}'):
-                description = f'{GitLabFeature.Helper.capitalize(project.name)}' \
-                              f' - {group_description}'
+            namespace_description: str
+            if project.namespace['kind'] == 'user':
+                namespace = gitlab.namespace(project.namespace['id'])
+                namespace_description = namespace.name
+            else:
+                group = gitlab.group(project.namespace['id'])
+                namespace_description = Namespaces.describe(
+                    name=group.name,
+                    description=group.description,
+                )
+            if not project.description or \
+                    not project.description.endswith(f' - {namespace_description}'):
+                description = f'{Namespaces.describe(name=project.name)}' \
+                              f' - {namespace_description}'
                 gitlab.project_set_description(criteria, description)
                 print(f'{Colors.BOLD}   - Updated description: '
                       f'{Colors.CYAN}{description}'
                       f'{Colors.RESET}')
+                Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Kept description: '
                       f'{Colors.GREEN}{project.description}'
                       f'{Colors.RESET}')
+                Platform.flush()
 
         # Reset project features
         if options.reset_features:
             features = ', '.join(gitlab.project_reset_features(criteria))
             if features:
                 print(f'{Colors.BOLD}   - Reset features: '
                       f'{Colors.CYAN}{features}'
                       f'{Colors.RESET}')
+                Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Reset features: '
                       f'{Colors.GREEN}Already done'
                       f'{Colors.RESET}')
+                Platform.flush()
 
         # Reset project members
         if options.reset_members:
             gitlab.project_reset_members(criteria)
             print(f'{Colors.BOLD}   - Reset members: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
+            Platform.flush()
 
         # Set project avatar
         if options.set_avatar:
             gitlab.project_set_avatar(criteria, options.set_avatar)
             print(f'{Colors.BOLD}   - Set avatar: '
                   f'{Colors.CYAN}{options.set_avatar}'
                   f'{Colors.RESET}')
+            Platform.flush()
+
+        # Run project housekeeping
+        if options.run_housekeeping:
+            gitlab.project_run_housekeeping(criteria)
+            print(f'{Colors.BOLD}   - Ran housekeeping: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+            Platform.flush()
+
+        # Archive project
+        if options.archive_project:
+            gitlab.project_set_archive(criteria, True)
+            print(f'{Colors.BOLD}   - Archive project: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+            Platform.flush()
+
+        # Unarchive project
+        elif options.unarchive_project:
+            gitlab.project_set_archive(criteria, False)
+            print(f'{Colors.BOLD}   - Unarchive project: '
+                  f'{Colors.GREEN}Success'
+                  f'{Colors.RESET}')
+            Platform.flush()
 
         # Protect project branches
         if options.protect_branches:
             branches = ', '.join(gitlab.project_protect_branches(criteria))
             if branches:
                 print(f'{Colors.BOLD}   - Protecting branches: '
                       f'{Colors.CYAN}{branches}'
                       f'{Colors.RESET}')
+                Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Protecting branches: '
                       f'{Colors.GREEN}Already done'
                       f'{Colors.RESET}')
+                Platform.flush()
 
         # Protect project tags
         if options.protect_tags:
             tags = ', '.join(gitlab.project_protect_tags(criteria, options.protect_tags))
             if tags:
                 print(f'{Colors.BOLD}   - Protecting tags: '
                       f'{Colors.CYAN}{tags}'
                       f'{Colors.GREEN} (level: {options.protect_tags})'
                       f'{Colors.RESET}')
+                Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Protecting tags: '
                       f'{Colors.GREEN}Already done'
                       f'{Colors.RESET}')
+                Platform.flush()
 
         # Footer
         print(' ')
         Platform.flush()
+
+        # Result
+        return True
```

### Comparing `gitlab_projects_settings-2.1.0/src/cli/main.py` & `gitlab_projects_settings-3.0.0/src/cli/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 # Standard libraries
-from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter)
+from argparse import (_ArgumentGroup, _MutuallyExclusiveGroup, ArgumentParser, Namespace,
+                      RawTextHelpFormatter)
 from os import environ
 from shutil import get_terminal_size
 from sys import exit as sys_exit
 
 # Components
 from ..package.bundle import Bundle
 from ..package.version import Version
@@ -15,14 +16,15 @@
 
 # Main, pylint: disable=too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
     result: bool = False
+    subgroup: _MutuallyExclusiveGroup
 
     # Arguments creation
     parser: ArgumentParser = ArgumentParser(
         prog=Bundle.NAME,
         description=f'{Bundle.NAME}: {Bundle.DESCRIPTION}',
         add_help=False,
         formatter_class=lambda prog: RawTextHelpFormatter(
@@ -118,14 +120,48 @@
     group.add_argument(
         '--update-description',
         dest='update_description',
         action='store_true',
         help='Update description of GitLab projects and groups automatically',
     )
 
+    # Arguments advanced settings definitions
+    group = parser.add_argument_group('advanced settings arguments')
+    group.add_argument(
+        '--run-housekeeping',
+        dest='run_housekeeping',
+        action='store_true',
+        help='Run housekeeping of project or projects GitLab in groups',
+    )
+    subgroup = group.add_mutually_exclusive_group()
+    subgroup.add_argument(
+        '--archive-project',
+        dest='archive_project',
+        action='store_true',
+        help='Archive project or projects in GitLab groups',
+    )
+    subgroup.add_argument(
+        '--unarchive-project',
+        dest='unarchive_project',
+        action='store_true',
+        help='Unarchive project or projects in GitLab groups',
+    )
+    group.add_argument(
+        '--delete-group',
+        dest='delete_group',
+        action='store_true',
+        help='Delete group or groups in GitLab groups',
+    )
+    group.add_argument(
+        '--delete-project',
+        dest='delete_project',
+        action='store_true',
+        help='Delete project or projects in GitLab groups',
+    )
+
     # Arguments repository settings definitions
     group = parser.add_argument_group('repository settings arguments')
     group.add_argument(
         '--protect-branches',
         dest='protect_branches',
         action='store_true',
         help='Protect branches with default master/main, develop and staging',
@@ -147,15 +183,15 @@
         default='https://gitlab.com',
         help='GitLab URL (default: https://gitlab.com)',
     )
     group.add_argument(
         dest='path',
         action='store',
         nargs='?',
-        help='GitLab group or project path',
+        help='GitLab group, user namespace or project path',
     )
 
     # Arguments parser
     options: Namespace = parser.parse_args()
 
     # Help informations
     if options.help:
```

### Comparing `gitlab_projects_settings-2.1.0/src/features/gitlab.py` & `gitlab_projects_settings-3.0.0/src/features/gitlab.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 # Standard libraries
+from time import sleep
 from typing import List
 
 # Modules libraries
 from gitlab import Gitlab
-from gitlab.exceptions import GitlabListError
-from gitlab.v4.objects import Group, Project
+from gitlab.exceptions import GitlabGetError, GitlabListError
+from gitlab.v4.objects import Group, Namespace, Project, User
 
 # GitLabFeature class
 class GitLabFeature:
 
     # Members
     __dry_run: bool = False
     __gitlab: Gitlab
@@ -21,20 +22,29 @@
         self.__gitlab = Gitlab(url, private_token=token)
         self.__gitlab.auth()
 
     # Group
     def group(self, criteria: str) -> Group:
         return self.__gitlab.groups.get(criteria)
 
+    # Group delete
+    def group_delete(self, criteria: str) -> None:
+
+        # Delete group
+        if not self.__dry_run:
+            group = self.group(criteria)
+            group.delete()
+            sleep(10)
+
     # Group reset members
     def group_reset_members(self, criteria: str) -> None:
 
         # Remove group members
         group = self.group(criteria)
-        for member in group.members.list():
+        for member in group.members.list(get_all=True):
             if not self.__dry_run:
                 group.members.delete(member.id)
 
         # Save group
         if not self.__dry_run:
             group.save()
 
@@ -57,33 +67,47 @@
         if not self.__dry_run:
             group = self.group(criteria)
             group.description = description
 
             # Save group
             group.save()
 
+    # Namespace
+    def namespace(self, criteria: str) -> Namespace:
+        return self.__gitlab.namespaces.get(criteria)
+
     # Project
     def project(self, criteria: str) -> Project:
         return self.__gitlab.projects.get(criteria)
 
+    # Project delete
+    def project_delete(self, criteria: str) -> None:
+
+        # Delete project
+        project = self.project(criteria)
+        if not self.__dry_run:
+            project.delete()
+            sleep(5)
+
     # Project protect branches
     def project_protect_branches(self, criteria: str) -> List[str]:
 
         # Validate project feature
         result: List[str] = []
         project = self.project(criteria)
         try:
-            assert project.branches.list()
+            assert project.branches.list(get_all=True)
         except (AssertionError, GitlabListError):
             return result
 
         # Acquire project, branches and protected branches
-        branches = [branch.name for branch in project.branches.list()]
+        branches = [branch.name for branch in project.branches.list(get_all=True)]
         protectedbranches = [
-            protectedbranch.name for protectedbranch in project.protectedbranches.list()
+            protectedbranch.name
+            for protectedbranch in project.protectedbranches.list(get_all=True)
         ]
 
         # Protect main/master
         for branch in ['main', 'master']:
             if branch in branches and branch not in protectedbranches:
                 if not self.__dry_run:
                     project.protectedbranches.create({
@@ -128,15 +152,15 @@
     # Project protect tags, pylint: disable=too-many-branches
     def project_protect_tags(self, criteria: str, protect_level: str) -> List[str]:
 
         # Validate project feature
         result: List[str] = []
         project = self.project(criteria)
         try:
-            assert project.tags.list()
+            assert project.tags.list(get_all=True)
         except (AssertionError, GitlabListError):
             return result
 
         # Prepare access level
         access_level: int
         if protect_level == 'no-one':
             access_level = 0
@@ -147,33 +171,33 @@
         elif protect_level == 'developers':
             access_level = 30
         else:
             raise SyntaxError(f'Unknown protection level: {access_level}')
 
         # Acquire protected tags
         protectedtags = [
-            protectedtag.name for protectedtag in project.protectedtags.list()
+            protectedtag.name for protectedtag in project.protectedtags.list(get_all=True)
         ]
 
         # Update protected tags
-        for protectedtag in project.protectedtags.list():
+        for protectedtag in project.protectedtags.list(get_all=True):
             protectedtag_level = protectedtag.create_access_levels[0]['access_level']
             if protectedtag_level != 0 and (access_level == 0
                                             or protectedtag_level < access_level):
                 name = protectedtag.name
                 if not self.__dry_run:
                     protectedtag.delete()
                     project.protectedtags.create({
                         'name': name,
                         'create_access_level': access_level
                     })
                 result += [name]
 
         # Protect unprotected tags
-        for tag in project.tags.list():
+        for tag in project.tags.list(get_all=True):
             if tag.name not in protectedtags:
                 if not self.__dry_run:
                     project.protectedtags.create({
                         'name': tag.name,
                         'create_access_level': access_level
                     })
                 result += [tag.name]
@@ -189,88 +213,153 @@
     # Project reset features, pylint: disable=too-many-branches,too-many-statements
     def project_reset_features(self, criteria: str) -> List[str]:
 
         # Variables
         result: List[str] = []
         project = self.__gitlab.projects.get(criteria, statistics=True)
 
-        # Disable unused features
+        # Disable unused feature (Issues)
         if project.issues_enabled and not project.issues.list(get_all=False):
             project.issues_enabled = False
             result += ['Issues']
+
+        # Disable unused feature (Repository)
         try:
             assert project.commits.list(get_all=False)
         except (AssertionError, GitlabListError):
             if project.repository_access_level != 'disabled':
                 project.repository_access_level = 'disabled'
                 result += ['Repository']
-        if project.merge_requests_enabled and not project.mergerequests.list(
-                get_all=False):
-            project.merge_requests_enabled = False
-            result += ['Merge requests']
+
+        # Disable unused feature (Merge requests)
+        try:
+            if not project.mergerequests.list(get_all=False):
+                pass
+            elif len(project.branches.list(get_all=False)) > 1:
+                pass
+            else:
+                assert False
+        except (AssertionError, GitlabListError):
+            if project.merge_requests_enabled:
+                project.merge_requests_enabled = False
+                result += ['Merge requests']
+
+        # Disable unused feature (Forks)
         if project.forking_access_level != 'disabled' and not project.forks.list(
                 get_all=False):
             project.forking_access_level = 'disabled'
             result += ['Forks']
+
+        # Disable unused feature (Git LFS)
         if project.lfs_enabled and project.statistics['lfs_objects_size'] == 0:
             project.lfs_enabled = False
             result += ['Git LFS']
-        if project.jobs_enabled and not project.jobs.list(get_all=False):
-            project.jobs_enabled = False
-            result += ['CI/CD']
+
+        # Disable unused feature (CI/CD)
+        try:
+            if project.jobs.list(get_all=False):
+                pass
+            elif any('name' in item and item['name'] == '.gitlab-ci.yml'
+                     for item in project.repository_tree(get_all=True)):
+                pass
+            elif any('path_with_namespace' in item
+                     and item['path_with_namespace'] != project.path_with_namespace
+                     for item in self.__gitlab.http_get(
+                         f'/projects/{project.id}/job_token_scope/allowlist',
+                         get_all=True,
+                     )):
+                pass
+            else:
+                assert False
+        except (AssertionError, GitlabGetError, GitlabListError):
+            if project.jobs_enabled:
+                project.jobs_enabled = False
+                result += ['CI/CD']
+
+        # Disable unused feature (Container registry)
         if project.container_registry_enabled and not project.repositories.list(
                 get_all=False):
             project.container_registry_enabled = False
             result += ['Container registry']
+
+        # Disable unused feature (Analytics)
         if project.analytics_access_level != 'disabled':
             project.analytics_access_level = 'disabled'
             result += ['Analytics']
+
+        # Disable unused feature (Security and Compliance)
         if project.security_and_compliance_access_level != 'disabled':
             project.security_and_compliance_access_level = 'disabled'
             result += ['Security and Compliance']
+
+        # Disable unused feature (Wiki)
         if project.wiki_enabled and not project.wikis.list(get_all=False):
             project.wiki_enabled = False
             result += ['Wiki']
+
+        # Disable unused feature (Snippets)
         if project.snippets_enabled and not project.snippets.list(get_all=False):
             project.snippets_enabled = False
             result += ['Snippets']
+
+        # Disable unused feature (Package registry)
         if project.packages_enabled and not project.packages.list(get_all=False):
             project.packages_enabled = False
             result += ['Package registry']
+
+        # Disable unused feature (Model experiments)
         if project.model_experiments_access_level != 'disabled':
             project.model_experiments_access_level = 'disabled'
             result += ['Model experiments']
+
+        # Disable unused feature (Model registry)
         if project.model_registry_access_level != 'disabled':
             project.model_registry_access_level = 'disabled'
             result += ['Model registry']
+
+        # Disable unused feature (Pages)
         if project.pages_access_level != 'disabled':
             project.pages_access_level = 'disabled'
             result += ['Pages']
+
+        # Disable unused feature (Monitor)
         if project.monitor_access_level != 'disabled':
             project.monitor_access_level = 'disabled'
             result += ['Monitor']
+
+        # Disable unused feature (Environments)
         try:
             assert project.environments.list(get_all=False)
         except (AssertionError, GitlabListError):
             if project.environments_access_level != 'disabled':
                 project.environments_access_level = 'disabled'
                 result += ['Environments']
+
+        # Disable unused feature (Feature flags)
         if project.feature_flags_access_level != 'disabled':
             project.feature_flags_access_level = 'disabled'
             result += ['Feature flags']
+
+        # Disable unused feature (Infrastructure)
         if project.infrastructure_access_level != 'disabled':
             project.infrastructure_access_level = 'disabled'
             result += ['Infrastructure']
+
+        # Disable unused feature (Releases)
         if project.releases_access_level != 'disabled' and not project.releases.list(
                 get_all=False):
             project.releases_access_level = 'disabled'
             result += ['Releases']
+
+        # Disable unused feature (Service Desk)
         if project.service_desk_enabled:
             project.service_desk_enabled = False
             result += ['Service Desk']
+
+        # Disable unused feature (Auto DevOps)
         if project.auto_devops_enabled:
             project.auto_devops_enabled = False
             result += ['Auto DevOps']
 
         # Save project
         if not self.__dry_run:
             project.save()
@@ -280,20 +369,41 @@
 
     # Project reset members
     def project_reset_members(self, criteria: str) -> None:
 
         # Remove project members
         if not self.__dry_run:
             project = self.project(criteria)
-            for member in project.members.list():
+            for member in project.members.list(get_all=True):
                 project.members.delete(member.id)
 
             # Save project
             project.save()
 
+    # Project run housekeeping
+    def project_run_housekeeping(self, criteria: str) -> None:
+
+        # Run project housekeeping
+        if not self.__dry_run:
+            project = self.project(criteria)
+            project.housekeeping()
+
+    # Project set archive
+    def project_set_archive(self, criteria: str, enabled: bool) -> None:
+
+        # Archive project
+        if not self.__dry_run and enabled:
+            project = self.project(criteria)
+            project.archive()
+
+        # Unarchive project
+        elif not self.__dry_run:
+            project = self.project(criteria)
+            project.unarchive()
+
     # Project set avatar
     def project_set_avatar(self, criteria: str, file: str) -> None:
 
         # Set project avatar
         if not self.__dry_run:
             project = self.project(criteria)
             with open(file, 'rb') as avatar:
@@ -309,29 +419,15 @@
         if not self.__dry_run:
             project = self.project(criteria)
             project.description = description
 
             # Save project
             project.save()
 
+    # User
+    def user(self, criteria: str) -> User:
+        return self.__gitlab.users.list(username=criteria)[0]
+
     # URL
     @property
     def url(self) -> str:
         return str(self.__gitlab.api_url)
-
-    # Helper class
-    class Helper:
-
-        # Capitalize
-        @staticmethod
-        def capitalize(text: str) -> str:
-            return f'{text[:1].capitalize()}{text[1:]}'
-
-        # Describe
-        @staticmethod
-        def describe(
-            description: str,
-            name: str,
-        ) -> str:
-            if description:
-                return description
-            return GitLabFeature.Helper.capitalize(name)
```

### Comparing `gitlab_projects_settings-2.1.0/src/package/version.py` & `gitlab_projects_settings-3.0.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/src/prints/colors.py` & `gitlab_projects_settings-3.0.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-2.1.0/src/system/platform.py` & `gitlab_projects_settings-3.0.0/src/system/platform.py`

 * *Files identical despite different names*

