# Comparing `tmp/plone.app.robotframework-2.1.2.tar.gz` & `tmp/plone_app_robotframework-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.robotframework-2.1.2.tar", last modified: Mon Feb 12 15:11:14 2024, max compression
+gzip compressed data, was "plone_app_robotframework-2.1.3.tar", last modified: Mon May  6 12:44:45 2024, max compression
```

## Comparing `plone.app.robotframework-2.1.2.tar` & `plone_app_robotframework-2.1.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.808848 plone.app.robotframework-2.1.2/
--rw-r--r--   0 maurits    (501) staff       (20)    21554 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      493 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      116 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    25052 2024-02-12 15:11:14.808008 plone.app.robotframework-2.1.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      574 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.767863 plone.app.robotframework-2.1.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      733 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/LICENSE.txt
--rwxr-xr-x   0 maurits    (501) staff       (20)     1844 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/libdoc.sh
--rw-r--r--   0 maurits    (501) staff       (20)      142 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/requirements.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.774289 plone.app.robotframework-2.1.2/docs/source/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.774716 plone.app.robotframework-2.1.2/docs/source/_static/
--rw-r--r--   0 maurits    (501) staff       (20)       23 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/_static/README
--rw-r--r--   0 maurits    (501) staff       (20)      640 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/bdd.txt
--rw-r--r--   0 maurits    (501) staff       (20)     8052 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3191 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/debugging.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/examples.rst
--rw-r--r--   0 maurits    (501) staff       (20)    12860 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/happy.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5220 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3219 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/keywords.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.784208 plone.app.robotframework-2.1.2/docs/source/libdoc/
--rw-r--r--   0 maurits    (501) staff       (20)   128738 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/python_debugging.html
--rw-r--r--   0 maurits    (501) staff       (20)   128732 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/python_layoutmath.html
--rw-r--r--   0 maurits    (501) staff       (20)   128720 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/python_saucelabs.html
--rw-r--r--   0 maurits    (501) staff       (20)   130037 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/python_zope2server.html
--rw-r--r--   0 maurits    (501) staff       (20)   130314 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_autologin.html
--rw-r--r--   0 maurits    (501) staff       (20)   130621 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_content.html
--rw-r--r--   0 maurits    (501) staff       (20)   129104 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_genericsetup.html
--rw-r--r--   0 maurits    (501) staff       (20)   129386 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_i18n.html
--rw-r--r--   0 maurits    (501) staff       (20)   129622 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_mockmailhost.html
--rw-r--r--   0 maurits    (501) staff       (20)   129647 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_quickinstaller.html
--rw-r--r--   0 maurits    (501) staff       (20)   129153 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_users.html
--rw-r--r--   0 maurits    (501) staff       (20)   129063 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/remote_zope2server.html
--rw-r--r--   0 maurits    (501) staff       (20)   109966 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/selenium.html
--rw-r--r--   0 maurits    (501) staff       (20)   137194 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/user_keywords.html
--rw-r--r--   0 maurits    (501) staff       (20)   129209 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/user_saucelabs.html
--rw-r--r--   0 maurits    (501) staff       (20)   131206 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/user_selenium.html
--rw-r--r--   0 maurits    (501) staff       (20)   128933 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/libdoc/user_server.html
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.786491 plone.app.robotframework-2.1.2/docs/source/plone-keywords/
--rw-r--r--   0 maurits    (501) staff       (20)      864 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/browser.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2032 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/content.rst
--rw-r--r--   0 maurits    (501) staff       (20)      291 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/edit-wizard-tabs.rst
--rw-r--r--   0 maurits    (501) staff       (20)      303 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/generic.rst
--rw-r--r--   0 maurits    (501) staff       (20)      241 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/history.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2896 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      351 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/plone-keywords/login.rst
--rw-r--r--   0 maurits    (501) staff       (20)      902 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/reload.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1453 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/remote.rst
--rw-r--r--   0 maurits    (501) staff       (20)      917 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/ride.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6099 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/robot.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3981 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/saucelabs.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1086 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/server.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13988 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/templer.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1655 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/travis-ci.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10381 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/docs/source/tutorial.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4497 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-02-12 15:11:14.809029 plone.app.robotframework-2.1.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     4023 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.763320 plone.app.robotframework-2.1.2/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.786759 plone.app.robotframework-2.1.2/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.789538 plone.app.robotframework-2.1.2/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.799831 plone.app.robotframework-2.1.2/src/plone/app/robotframework/
--rw-r--r--   0 maurits    (501) staff       (20)     1223 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      430 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/_variables.robot
--rw-r--r--   0 maurits    (501) staff       (20)      493 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/annotate.py
--rw-r--r--   0 maurits    (501) staff       (20)    12936 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/annotate.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2172 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/autologin.py
--rw-r--r--   0 maurits    (501) staff       (20)     3187 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/browser.robot
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/config.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.800527 plone.app.robotframework-2.1.2/src/plone/app/robotframework/content/
--rw-r--r--   0 maurits    (501) staff       (20)    74429 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/content/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)     5131 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/content/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    10683 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/content.py
--rw-r--r--   0 maurits    (501) staff       (20)      449 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/genericsetup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2069 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/i18n.py
--rw-r--r--   0 maurits    (501) staff       (20)      607 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/keywords.py
--rw-r--r--   0 maurits    (501) staff       (20)     9712 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/keywords.robot
--rw-r--r--   0 maurits    (501) staff       (20)      138 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/keywords.txt
--rw-r--r--   0 maurits    (501) staff       (20)      505 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/mailhost.py
--rw-r--r--   0 maurits    (501) staff       (20)      715 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/patches.py
--rw-r--r--   0 maurits    (501) staff       (20)      945 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/pybabel.py
--rw-r--r--   0 maurits    (501) staff       (20)      830 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/quickinstaller.py
--rw-r--r--   0 maurits    (501) staff       (20)     8885 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/reload.py
--rw-r--r--   0 maurits    (501) staff       (20)     2384 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/remote.py
--rw-r--r--   0 maurits    (501) staff       (20)     2904 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/robotentrypoints.py
--rw-r--r--   0 maurits    (501) staff       (20)     1333 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/saucelabs.py
--rw-r--r--   0 maurits    (501) staff       (20)     1528 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/saucelabs.robot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.801443 plone.app.robotframework-2.1.2/src/plone/app/robotframework/selectors/
--rw-r--r--   0 maurits    (501) staff       (20)      154 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/selectors/cmfplone43.robot
--rw-r--r--   0 maurits    (501) staff       (20)      154 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/selectors/cmfplone50.robot
--rw-r--r--   0 maurits    (501) staff       (20)      142 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/selectors/cmfplone60.robot
--rw-r--r--   0 maurits    (501) staff       (20)     6331 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/selenium.robot
--rw-r--r--   0 maurits    (501) staff       (20)    14137 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/server.py
--rw-r--r--   0 maurits    (501) staff       (20)      853 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/server.robot
--rw-r--r--   0 maurits    (501) staff       (20)      134 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/server.txt
--rw-r--r--   0 maurits    (501) staff       (20)      584 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/speak.robot
--rw-r--r--   0 maurits    (501) staff       (20)    11115 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.805123 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.805839 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      347 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/docs/test_hello.robot
--rw-r--r--   0 maurits    (501) staff       (20)      934 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/docs/test_keywords.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3248 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_autologin_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)      535 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_browser_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2601 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)     2407 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_content_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)      439 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_i18n_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)      434 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_quickinstaller_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2164 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     1271 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_robotfixture.py
--rw-r--r--   0 maurits    (501) staff       (20)      410 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_robotfixture.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3650 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_speakjs_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1205 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_users_library.robot
--rw-r--r--   0 maurits    (501) staff       (20)      955 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/user.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1822 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/users.py
--rw-r--r--   0 maurits    (501) staff       (20)      228 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      510 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)      163 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone/app/robotframework/variables.robot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:11:14.806255 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    25052 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4450 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      424 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      723 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-12 15:11:14.000000 plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.729990 plone_app_robotframework-2.1.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    21686 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      493 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    25184 2024-05-06 12:44:45.729458 plone_app_robotframework-2.1.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      574 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.688282 plone_app_robotframework-2.1.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      733 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/LICENSE.txt
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1844 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/libdoc.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/requirements.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.695672 plone_app_robotframework-2.1.3/docs/source/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.696135 plone_app_robotframework-2.1.3/docs/source/_static/
+-rw-r--r--   0 maurits    (501) staff       (20)       23 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/_static/README
+-rw-r--r--   0 maurits    (501) staff       (20)      640 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/bdd.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     8052 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3191 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/debugging.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/examples.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    12860 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/happy.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5220 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3219 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/keywords.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.704384 plone_app_robotframework-2.1.3/docs/source/libdoc/
+-rw-r--r--   0 maurits    (501) staff       (20)   128738 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/python_debugging.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128732 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/python_layoutmath.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128720 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/python_saucelabs.html
+-rw-r--r--   0 maurits    (501) staff       (20)   130037 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/python_zope2server.html
+-rw-r--r--   0 maurits    (501) staff       (20)   130314 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_autologin.html
+-rw-r--r--   0 maurits    (501) staff       (20)   130621 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_content.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129104 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_genericsetup.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129386 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_i18n.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129622 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_mockmailhost.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129647 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_quickinstaller.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129153 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_users.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129063 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/remote_zope2server.html
+-rw-r--r--   0 maurits    (501) staff       (20)   109966 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/selenium.html
+-rw-r--r--   0 maurits    (501) staff       (20)   137194 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/user_keywords.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129209 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/user_saucelabs.html
+-rw-r--r--   0 maurits    (501) staff       (20)   131206 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/user_selenium.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128933 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/libdoc/user_server.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.706714 plone_app_robotframework-2.1.3/docs/source/plone-keywords/
+-rw-r--r--   0 maurits    (501) staff       (20)      864 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/browser.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2032 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/content.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/edit-wizard-tabs.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/generic.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/history.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2896 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      351 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/plone-keywords/login.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      902 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/reload.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1453 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/remote.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      917 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/ride.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6099 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/robot.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3981 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/saucelabs.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1086 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/server.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13988 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/templer.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1655 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/travis-ci.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10381 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/docs/source/tutorial.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4497 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:44:45.730077 plone_app_robotframework-2.1.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     4023 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.683129 plone_app_robotframework-2.1.3/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.706996 plone_app_robotframework-2.1.3/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.710052 plone_app_robotframework-2.1.3/src/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.720669 plone_app_robotframework-2.1.3/src/plone/app/robotframework/
+-rw-r--r--   0 maurits    (501) staff       (20)     1223 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      430 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/_variables.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      493 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/annotate.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12936 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/annotate.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2172 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/autologin.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3187 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/browser.robot
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/config.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.721502 plone_app_robotframework-2.1.3/src/plone/app/robotframework/content/
+-rw-r--r--   0 maurits    (501) staff       (20)    74429 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/content/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)     5131 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/content/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)    10683 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      449 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/genericsetup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2069 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/i18n.py
+-rw-r--r--   0 maurits    (501) staff       (20)      607 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/keywords.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9712 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      138 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/keywords.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      505 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/mailhost.py
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/patches.py
+-rw-r--r--   0 maurits    (501) staff       (20)      945 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/pybabel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      830 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/quickinstaller.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8885 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/reload.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2384 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/remote.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2904 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/robotentrypoints.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1333 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/saucelabs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1528 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/saucelabs.robot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.722375 plone_app_robotframework-2.1.3/src/plone/app/robotframework/selectors/
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/selectors/cmfplone43.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/selectors/cmfplone50.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/selectors/cmfplone60.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6423 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/selenium.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    14137 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/server.py
+-rw-r--r--   0 maurits    (501) staff       (20)      853 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/server.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/server.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/speak.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    11115 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.726568 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.727186 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      347 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/docs/test_hello.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      934 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/docs/test_keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3248 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_autologin_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_browser_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2601 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2407 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_content_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      439 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_i18n_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      434 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_quickinstaller_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2164 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1271 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_robotfixture.py
+-rw-r--r--   0 maurits    (501) staff       (20)      410 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_robotfixture.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3650 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_speakjs_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1205 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_users_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      955 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/user.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1822 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/users.py
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2024-05-06 12:44:44.000000 plone_app_robotframework-2.1.3/src/plone/app/robotframework/variables.robot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:44:45.727731 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    25184 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4450 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      424 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      723 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:44:45.000000 plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/top_level.txt
```

### Comparing `plone.app.robotframework-2.1.2/CHANGES.rst` & `plone_app_robotframework-2.1.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.1.3 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Makes ``Wait For Then Click Element`` keyword more robust. @wesleybl (#157)
+
+
 2.1.2 (2024-02-12)
 ------------------
 
 Bug fixes:
 
 
 - Fix duplicate installation of plone.app.contenttypes:default profile. @davisagli (#154)
```

### Comparing `plone.app.robotframework-2.1.2/PKG-INFO` & `plone_app_robotframework-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.robotframework
-Version: 2.1.2
+Version: 2.1.3
 Summary: Robot Framework testing resources for Plone
 Home-page: https://github.com/plone/plone.app.robotframework/
 Author: Asko Soukka
 Author-email: asko.soukka@iki.fi
 License: GPL
 Keywords: robot automatic browser testing Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -119,14 +119,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.1.3 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Makes ``Wait For Then Click Element`` keyword more robust. @wesleybl (#157)
+
+
 2.1.2 (2024-02-12)
 ------------------
 
 Bug fixes:
 
 
 - Fix duplicate installation of plone.app.contenttypes:default profile. @davisagli (#154)
```

### Comparing `plone.app.robotframework-2.1.2/README.rst` & `plone_app_robotframework-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/LICENSE.GPL` & `plone_app_robotframework-2.1.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/LICENSE.txt` & `plone_app_robotframework-2.1.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/libdoc.sh` & `plone_app_robotframework-2.1.3/docs/libdoc.sh`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/bdd.txt` & `plone_app_robotframework-2.1.3/docs/source/bdd.txt`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/conf.py` & `plone_app_robotframework-2.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/debugging.rst` & `plone_app_robotframework-2.1.3/docs/source/debugging.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/examples.rst` & `plone_app_robotframework-2.1.3/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/happy.rst` & `plone_app_robotframework-2.1.3/docs/source/happy.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/index.rst` & `plone_app_robotframework-2.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/keywords.rst` & `plone_app_robotframework-2.1.3/docs/source/keywords.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/python_debugging.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/python_debugging.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/python_layoutmath.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/python_layoutmath.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/python_saucelabs.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/python_saucelabs.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/python_zope2server.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/python_zope2server.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_autologin.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_autologin.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_content.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_content.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_genericsetup.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_genericsetup.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_i18n.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_i18n.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_mockmailhost.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_mockmailhost.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_quickinstaller.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_quickinstaller.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_users.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_users.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/remote_zope2server.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/remote_zope2server.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/selenium.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/selenium.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/user_keywords.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/user_keywords.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/user_saucelabs.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/user_saucelabs.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/user_selenium.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/user_selenium.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/libdoc/user_server.html` & `plone_app_robotframework-2.1.3/docs/source/libdoc/user_server.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/plone-keywords/browser.rst` & `plone_app_robotframework-2.1.3/docs/source/plone-keywords/browser.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/plone-keywords/content.rst` & `plone_app_robotframework-2.1.3/docs/source/plone-keywords/content.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/plone-keywords/index.rst` & `plone_app_robotframework-2.1.3/docs/source/plone-keywords/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/reload.rst` & `plone_app_robotframework-2.1.3/docs/source/reload.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/remote.rst` & `plone_app_robotframework-2.1.3/docs/source/remote.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/ride.rst` & `plone_app_robotframework-2.1.3/docs/source/ride.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/robot.rst` & `plone_app_robotframework-2.1.3/docs/source/robot.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/saucelabs.rst` & `plone_app_robotframework-2.1.3/docs/source/saucelabs.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/server.rst` & `plone_app_robotframework-2.1.3/docs/source/server.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/templer.rst` & `plone_app_robotframework-2.1.3/docs/source/templer.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/travis-ci.rst` & `plone_app_robotframework-2.1.3/docs/source/travis-ci.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/docs/source/tutorial.rst` & `plone_app_robotframework-2.1.3/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/pyproject.toml` & `plone_app_robotframework-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/setup.py` & `plone_app_robotframework-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.1.2"
+version = "2.1.3"
 
 
 def indented(filename):
     return "".join([indent(line) for line in open(filename)])
 
 
 def indent(line):
```

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/__init__.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/annotate.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/annotate.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/autologin.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/autologin.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/browser.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/browser.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/content/file.pdf` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/content/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/content/image.jpg` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/content/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/content.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/content.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/i18n.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/i18n.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/keywords.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/keywords.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/keywords.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/keywords.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/patches.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/patches.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/pybabel.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/pybabel.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/quickinstaller.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/quickinstaller.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/reload.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/reload.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/remote.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/remote.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/robotentrypoints.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/robotentrypoints.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/saucelabs.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/saucelabs.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/saucelabs.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/saucelabs.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/selenium.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/selenium.robot`

 * *Files 4% similar despite different names*

```diff
@@ -97,27 +97,29 @@
     ...                          ${locator}
 
 Wait For Element
     [Documentation]  Can contain css=, jquery=, or any other element selector.
     ...              Element must match exactly one time.
     [Arguments]  ${element}
     Wait Until Page Contains Element  ${element}
-    Set Focus To Element  ${element}
     Wait Until Element Is Visible  ${element}
+    Wait Until Element Is Enabled  ${element}
+    Set Focus To Element  ${element}
     Sleep  0.1
     ${count} =  Get Element Count  ${element}
     Should Be Equal as Numbers  ${count}  1
 
 Wait For Elements
     [Documentation]  Can contain css=, jquery=, or any other element selector.
     ...              Element may match more than once.
     [Arguments]  ${element}
     Wait Until Page Contains Element  ${element}
-    Set Focus To Element  ${element}
     Wait Until Element Is Visible  ${element}
+    Wait Until Element Is Enabled  ${element}
+    Set Focus To Element  ${element}
 
 Wait For Then Click Element
     [Documentation]  Can contain css=, jquery=, or any other element selector.
     ...              Element must match exactly one time.
     [Arguments]  ${element}
     Wait For Element  ${element}
     Click Element  ${element}
```

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/server.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/server.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/server.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/speak.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/speak.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/testing.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/docs/test_keywords.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/docs/test_keywords.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_autologin_library.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_autologin_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_browser_library.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_browser_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_content.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_content_library.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_content_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_robot.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_robotfixture.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_robotfixture.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_speakjs_library.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_speakjs_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/tests/test_users_library.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/tests/test_users_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/user.robot` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/user.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone/app/robotframework/users.py` & `plone_app_robotframework-2.1.3/src/plone/app/robotframework/users.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/PKG-INFO` & `plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.robotframework
-Version: 2.1.2
+Version: 2.1.3
 Summary: Robot Framework testing resources for Plone
 Home-page: https://github.com/plone/plone.app.robotframework/
 Author: Asko Soukka
 Author-email: asko.soukka@iki.fi
 License: GPL
 Keywords: robot automatic browser testing Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -119,14 +119,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.1.3 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Makes ``Wait For Then Click Element`` keyword more robust. @wesleybl (#157)
+
+
 2.1.2 (2024-02-12)
 ------------------
 
 Bug fixes:
 
 
 - Fix duplicate installation of plone.app.contenttypes:default profile. @davisagli (#154)
```

### Comparing `plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/SOURCES.txt` & `plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.1.2/src/plone.app.robotframework.egg-info/requires.txt` & `plone_app_robotframework-2.1.3/src/plone.app.robotframework.egg-info/requires.txt`

 * *Files identical despite different names*

