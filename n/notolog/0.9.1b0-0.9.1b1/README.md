# Comparing `tmp/notolog-0.9.1b0.tar.gz` & `tmp/notolog-0.9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.1b0.tar", last modified: Sun May  5 14:52:07 2024, max compression
+gzip compressed data, was "notolog-0.9.1b1.tar", last modified: Mon May  6 20:29:08 2024, max compression
```

## Comparing `notolog-0.9.1b0.tar` & `notolog-0.9.1b1.tar`

### file list

```diff
@@ -1,430 +1,430 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.029801 notolog-0.9.1b0/
--rw-r--r--   0 vadikus    (501) staff       (20)     4751 2024-05-05 14:33:15.000000 notolog-0.9.1b0/CHANGELOG.md
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b0/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      191 2024-05-05 14:33:15.000000 notolog-0.9.1b0/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    18015 2024-05-05 14:52:07.027689 notolog-0.9.1b0/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    15870 2024-05-05 14:33:15.000000 notolog-0.9.1b0/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.603522 notolog-0.9.1b0/app/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.605430 notolog-0.9.1b0/app/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.571156 notolog-0.9.1b0/app/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.620631 notolog-0.9.1b0/app/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2187 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6330 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.635281 notolog-0.9.1b0/app/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.686332 notolog-0.9.1b0/app/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7980 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.697229 notolog-0.9.1b0/app/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6433 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.712332 notolog-0.9.1b0/app/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      771 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7963 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.724840 notolog-0.9.1b0/app/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4337 2024-05-05 14:40:40.000000 notolog-0.9.1b0/app/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.732733 notolog-0.9.1b0/app/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1876 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6158 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1470 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1386 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3236 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.733723 notolog-0.9.1b0/app/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.739524 notolog-0.9.1b0/app/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-04 21:27:31.000000 notolog-0.9.1b0/app/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.744935 notolog-0.9.1b0/app/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9027 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    48888 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9600 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/image_downloader.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.747525 notolog-0.9.1b0/app/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.750002 notolog-0.9.1b0/app/lexemes/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      160 2024-05-04 21:42:24.000000 notolog-0.9.1b0/app/lexemes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3224 2024-05-05 14:44:43.000000 notolog-0.9.1b0/app/lexemes/__pycache__/lexemes.cpython-39.pyc
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.757090 notolog-0.9.1b0/app/lexemes/de/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.764205 notolog-0.9.1b0/app/lexemes/de/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6854 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5899 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2183 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2914 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1272 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6579 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.778370 notolog-0.9.1b0/app/lexemes/en/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.786332 notolog-0.9.1b0/app/lexemes/en/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6663 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5462 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2086 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3470 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1243 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2495 2024-05-04 21:55:13.000000 notolog-0.9.1b0/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6044 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.793193 notolog-0.9.1b0/app/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6549 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.801668 notolog-0.9.1b0/app/lexemes/fi/
--rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6284 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/fi/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.808184 notolog-0.9.1b0/app/lexemes/fr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.815721 notolog-0.9.1b0/app/lexemes/fr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6899 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6212 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2256 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3928 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1274 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2794 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6709 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.829335 notolog-0.9.1b0/app/lexemes/ge/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.837231 notolog-0.9.1b0/app/lexemes/ge/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1355 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)    10384 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9053 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3389 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5710 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1642 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     4138 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9721 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.844850 notolog-0.9.1b0/app/lexemes/gr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.855987 notolog-0.9.1b0/app/lexemes/gr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1172 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8982 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8175 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2804 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5014 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1528 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3735 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8654 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/lexemes/gr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/gr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.861966 notolog-0.9.1b0/app/lexemes/in/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.870851 notolog-0.9.1b0/app/lexemes/in/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9403 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9416 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3029 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5585 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1618 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10062 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/in/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.882984 notolog-0.9.1b0/app/lexemes/it/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.889821 notolog-0.9.1b0/app/lexemes/it/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      930 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6824 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5639 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2188 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2925 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1290 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2700 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6359 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.896330 notolog-0.9.1b0/app/lexemes/ja/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.903427 notolog-0.9.1b0/app/lexemes/ja/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6837 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     4046 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7241 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.909112 notolog-0.9.1b0/app/lexemes/ko/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.915635 notolog-0.9.1b0/app/lexemes/ko/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      954 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     7562 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6404 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2277 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3723 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1285 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:28:24.000000 notolog-0.9.1b0/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6765 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.927248 notolog-0.9.1b0/app/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6236 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.935376 notolog-0.9.1b0/app/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6347 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.941882 notolog-0.9.1b0/app/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7931 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.950917 notolog-0.9.1b0/app/lexemes/se/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.957197 notolog-0.9.1b0/app/lexemes/se/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6826 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5756 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2125 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3568 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1275 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2574 2024-05-05 14:45:05.000000 notolog-0.9.1b0/app/lexemes/se/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6246 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/lexemes/se/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.963809 notolog-0.9.1b0/app/lexemes/tr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.974534 notolog-0.9.1b0/app/lexemes/tr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     7114 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5741 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2272 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3751 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1297 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6147 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:27:29.000000 notolog-0.9.1b0/app/lexemes/tr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:06.983125 notolog-0.9.1b0/app/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5770 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-04 21:27:28.000000 notolog-0.9.1b0/app/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)   175569 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.002594 notolog-0.9.1b0/app/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-04 21:27:27.000000 notolog-0.9.1b0/app/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    37283 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)    12655 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:26.000000 notolog-0.9.1b0/app/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-04 21:27:30.000000 notolog-0.9.1b0/app/view_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b0/app_config.toml
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.004956 notolog-0.9.1b0/docs/
--rw-r--r--   0 vadikus    (501) staff       (20)     8621 2024-05-05 14:47:11.000000 notolog-0.9.1b0/docs/Examples.md
--rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b0/docs/notolog-ui-settings.png
--rw-r--r--   0 vadikus    (501) staff       (20)     2770 2024-05-05 14:33:15.000000 notolog-0.9.1b0/main.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.025968 notolog-0.9.1b0/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    18015 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14261 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-05-05 14:52:06.000000 notolog-0.9.1b0/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-05 14:33:15.000000 notolog-0.9.1b0/requirements.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-05 14:52:07.030211 notolog-0.9.1b0/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     2166 2024-05-05 14:33:15.000000 notolog-0.9.1b0/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-05 14:52:07.024292 notolog-0.9.1b0/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9880 2024-05-05 14:33:15.000000 notolog-0.9.1b0/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5823 2024-05-04 21:27:31.000000 notolog-0.9.1b0/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4464 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6222 2024-05-04 21:27:32.000000 notolog-0.9.1b0/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.382591 notolog-0.9.1b1/
+-rw-r--r--   0 vadikus    (501) staff       (20)     5008 2024-05-06 20:09:20.000000 notolog-0.9.1b1/CHANGELOG.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b1/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      191 2024-05-05 14:33:15.000000 notolog-0.9.1b1/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    17029 2024-05-06 20:29:08.380968 notolog-0.9.1b1/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14998 2024-05-06 20:20:54.000000 notolog-0.9.1b1/README.md
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.809018 notolog-0.9.1b1/app/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.815389 notolog-0.9.1b1/app/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.752985 notolog-0.9.1b1/app/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.832963 notolog-0.9.1b1/app/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2187 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6330 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.876101 notolog-0.9.1b1/app/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.999339 notolog-0.9.1b1/app/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7980 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.021476 notolog-0.9.1b1/app/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6433 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.034576 notolog-0.9.1b1/app/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      771 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7963 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.041930 notolog-0.9.1b1/app/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4337 2024-05-06 20:24:02.000000 notolog-0.9.1b1/app/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.051858 notolog-0.9.1b1/app/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1876 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6158 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1487 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1386 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3236 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.053109 notolog-0.9.1b1/app/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.058743 notolog-0.9.1b1/app/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.063403 notolog-0.9.1b1/app/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9027 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    48888 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9600 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.065333 notolog-0.9.1b1/app/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.067687 notolog-0.9.1b1/app/lexemes/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      160 2024-05-04 21:42:24.000000 notolog-0.9.1b1/app/lexemes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3224 2024-05-06 20:15:44.000000 notolog-0.9.1b1/app/lexemes/__pycache__/lexemes.cpython-39.pyc
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.079033 notolog-0.9.1b1/app/lexemes/de/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.090534 notolog-0.9.1b1/app/lexemes/de/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6854 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5899 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2183 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2914 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1272 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6579 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.099809 notolog-0.9.1b1/app/lexemes/en/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.107424 notolog-0.9.1b1/app/lexemes/en/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6663 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5462 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2086 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3470 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1243 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2495 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6044 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.113391 notolog-0.9.1b1/app/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6549 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.119517 notolog-0.9.1b1/app/lexemes/fi/
+-rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6284 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.130970 notolog-0.9.1b1/app/lexemes/fr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.141109 notolog-0.9.1b1/app/lexemes/fr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6899 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6212 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2256 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3928 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1274 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2794 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6709 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.148603 notolog-0.9.1b1/app/lexemes/ge/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.155476 notolog-0.9.1b1/app/lexemes/ge/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1355 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)    10384 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9053 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3389 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5710 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1642 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     4138 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9721 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.162290 notolog-0.9.1b1/app/lexemes/gr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.170560 notolog-0.9.1b1/app/lexemes/gr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1172 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8982 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8175 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2804 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5014 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1528 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3735 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8654 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.187388 notolog-0.9.1b1/app/lexemes/in/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.195193 notolog-0.9.1b1/app/lexemes/in/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9403 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9416 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3029 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5585 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1618 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10062 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.202894 notolog-0.9.1b1/app/lexemes/it/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.210712 notolog-0.9.1b1/app/lexemes/it/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      930 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6824 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5639 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2188 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2925 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1290 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2700 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6359 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.217774 notolog-0.9.1b1/app/lexemes/ja/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.229700 notolog-0.9.1b1/app/lexemes/ja/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1023 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8455 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2414 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     4049 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1304 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3050 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7241 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.241178 notolog-0.9.1b1/app/lexemes/ko/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.250342 notolog-0.9.1b1/app/lexemes/ko/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      954 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     7562 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6404 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2277 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3723 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1285 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6765 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.257817 notolog-0.9.1b1/app/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6236 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.264114 notolog-0.9.1b1/app/lexemes/nl/
+-rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6468 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.270007 notolog-0.9.1b1/app/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6347 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.278185 notolog-0.9.1b1/app/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7931 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.291170 notolog-0.9.1b1/app/lexemes/se/
+-rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6246 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.308613 notolog-0.9.1b1/app/lexemes/tr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.322106 notolog-0.9.1b1/app/lexemes/tr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     7114 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5741 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2272 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3751 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1297 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6147 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.331958 notolog-0.9.1b1/app/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5770 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   175569 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.355075 notolog-0.9.1b1/app/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37283 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12655 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:26.000000 notolog-0.9.1b1/app/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/view_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app_config.toml
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.356988 notolog-0.9.1b1/docs/
+-rw-r--r--   0 vadikus    (501) staff       (20)     7749 2024-05-06 20:22:54.000000 notolog-0.9.1b1/docs/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b1/docs/notolog-ui-settings.png
+-rw-r--r--   0 vadikus    (501) staff       (20)     2770 2024-05-05 14:33:15.000000 notolog-0.9.1b1/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.378317 notolog-0.9.1b1/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    17029 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14093 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-06 20:09:20.000000 notolog-0.9.1b1/requirements.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-06 20:29:08.383136 notolog-0.9.1b1/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2166 2024-05-06 20:09:20.000000 notolog-0.9.1b1/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.376505 notolog-0.9.1b1/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9880 2024-05-05 14:33:15.000000 notolog-0.9.1b1/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5823 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4464 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6222 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_themes.py
```

### Comparing `notolog-0.9.1b0/CHANGELOG.md` & `notolog-0.9.1b1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 # Changelog
 All notologable changes to this project will be documented in this file.
 
+## [0.9.1b1] - 2024-05-06
+### Added
+- New interface language: Dutch
+
+### Updated
+- Upgraded `cryptography` to version 42.0.7 to align with the latest standards and enhance security.
+
+### Changed
+- Updated requirements.txt to match the actual package list.
+
 ## [0.9.1b0] - 2024-05-05
 ### Added
 - New interface languages: Finnish and Swedish, expanding accessibility for users in these regions.
 - Additional entries to the `.gitignore` and `.gitattributes` files to improve version control practices.
 - A dedicated `app_config.toml` file with initial configuration parameters, simplifying initial setup and customization.
 
 ### Updated
```

### Comparing `notolog-0.9.1b0/LICENSE` & `notolog-0.9.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/PKG-INFO` & `notolog-0.9.1b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b0
+Version: 0.9.1b1
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,ai,markdown,editor
@@ -30,35 +30,32 @@
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi==1.16.0
 Requires-Dist: click==8.1.7
-Requires-Dist: cryptography==42.0.6
+Requires-Dist: cryptography==42.0.7
 Requires-Dist: emoji==2.11.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Markdown==3.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
-Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: qasync==0.27.1
-Requires-Dist: qt6-applications==6.5.0.2.3
-Requires-Dist: qt6-tools==6.5.0.1.3
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-05 15:21:52.653006"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-06 21:20:54.001715"}} -->
 # Notolog
 
 ![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
 Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
@@ -303,12 +300,8 @@
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
 This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
 
 ---
-
-`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
-`╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
+This README.md file has been carefully crafted and edited using the Notolog editor itself.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `notolog-0.9.1b0/README.md` & `notolog-0.9.1b1/notolog.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-05 15:21:52.653006"}} -->
+Metadata-Version: 2.1
+Name: notolog
+Version: 0.9.1b1
+Summary: Notolog Markdown Editor
+Home-page: https://github.com/notolog/notolog-editor
+Author: Vadim Bakhrenkov
+License: MIT
+Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
+Project-URL: Source, https://github.com/notolog/notolog-editor/
+Keywords: notolog,ai,markdown,editor
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Text Editors
+Classifier: Topic :: Text Editors :: Documentation
+Classifier: Topic :: Text Editors :: Emacs
+Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
+Classifier: Topic :: Text Editors :: Text Processing
+Classifier: Topic :: Text Editors :: Word Processors
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Requires-Python: >=3.9, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cffi==1.16.0
+Requires-Dist: click==8.1.7
+Requires-Dist: cryptography==42.0.7
+Requires-Dist: emoji==2.11.1
+Requires-Dist: iniconfig==2.0.0
+Requires-Dist: Markdown==3.6
+Requires-Dist: packaging==24.0
+Requires-Dist: pluggy==1.5.0
+Requires-Dist: pycparser==2.22
+Requires-Dist: Pygments==2.18.0
+Requires-Dist: PySide6==6.7.0
+Requires-Dist: PySide6_Addons==6.7.0
+Requires-Dist: PySide6_Essentials==6.7.0
+Requires-Dist: pytest==8.2.0
+Requires-Dist: pytest-mock==3.14.0
+Requires-Dist: qasync==0.27.1
+Requires-Dist: shiboken6==6.7.0
+Requires-Dist: tomli==2.0.1
+
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-06 21:20:54.001715"}} -->
 # Notolog
 
 ![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
 Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
@@ -247,12 +300,8 @@
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
 This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
 
 ---
-
-`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
-`╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
+This README.md file has been carefully crafted and edited using the Notolog editor itself.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `notolog-0.9.1b0/app/app_config.py` & `notolog-0.9.1b1/app/app_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tomli
 
 toml_base_app_config = """
 [app]
 name = "Notolog"
-version = "0.9.1b0"
+version = "0.9.1b1"
 license = "MIT"
 date = "2024"
 website = "https://notolog.app"
 repository = "https://github.com/notolog/notolog-editor"
 pypi = "https://pypi.org/project/notolog"
 author = "Vadim Bakhrenkov"
```

### Comparing `notolog-0.9.1b0/app/assets/notolog-example-image.png` & `notolog-0.9.1b1/app/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/notolog-logo.png` & `notolog-0.9.1b1/app/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.1b1/app/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/calligraphy/default.ini` & `notolog-0.9.1b1/app/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/calligraphy/md.ini` & `notolog-0.9.1b1/app/assets/themes/calligraphy/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.1b1/app/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/calligraphy/styles.css` & `notolog-0.9.1b1/app/assets/themes/calligraphy/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.1b1/app/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/about_popup.css` & `notolog-0.9.1b1/app/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/default.ini` & `notolog-0.9.1b1/app/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/LICENSE` & `notolog-0.9.1b1/app/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/balloon.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/folder.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/github.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/quote.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/robot.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/star.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/trash3.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.1b1/app/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/md.ini` & `notolog-0.9.1b1/app/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/settings_dialog.css` & `notolog-0.9.1b1/app/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/styles.css` & `notolog-0.9.1b1/app/assets/themes/default/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/default/tree_view.css` & `notolog-0.9.1b1/app/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.1b1/app/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/noir_dark/default.ini` & `notolog-0.9.1b1/app/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/noir_dark/md.ini` & `notolog-0.9.1b1/app/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.1b1/app/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/noir_dark/styles.css` & `notolog-0.9.1b1/app/assets/themes/noir_dark/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.1b1/app/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/strawberry/about_popup.css` & `notolog-0.9.1b1/app/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/strawberry/default.ini` & `notolog-0.9.1b1/app/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/strawberry/md.ini` & `notolog-0.9.1b1/app/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.1b1/app/assets/themes/strawberry/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/strawberry/styles.css` & `notolog-0.9.1b1/app/assets/themes/strawberry/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/assets/themes/strawberry/tree_view.css` & `notolog-0.9.1b1/app/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/edit_widget.py` & `notolog-0.9.1b1/app/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/editor_state.py` & `notolog-0.9.1b1/app/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/encrypt/enc_helper.py` & `notolog-0.9.1b1/app/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/encrypt/enc_new_password_dialog.py` & `notolog-0.9.1b1/app/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/encrypt/enc_password.py` & `notolog-0.9.1b1/app/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/encrypt/enc_password_dialog.py` & `notolog-0.9.1b1/app/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.1b1/app/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/enums/ai_model_names.py` & `notolog-0.9.1b1/app/enums/ai_model_names.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/enums/colors.py` & `notolog-0.9.1b1/app/enums/colors.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/enums/languages.py` & `notolog-0.9.1b1/app/enums/languages.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     GE = "Georgian"
     GR = "Greek"
     IN = "Hindi"
     IT = "Italian"
     JA = "Japanese"
     KO = "Korean"
     LA = "Latin"
+    NL = "Dutch"
     PT = "Portuguese"
     RU = "Russian"
     SE = "Swedish"
     TR = "Turkish"
     ZH = "Chinese"
 
     def __init__(self, value, is_default=False):
```

### Comparing `notolog-0.9.1b0/app/enums/themes.py` & `notolog-0.9.1b1/app/enums/themes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/etree_extension.py` & `notolog-0.9.1b1/app/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/file_header.py` & `notolog-0.9.1b1/app/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/file_system_watcher.py` & `notolog-0.9.1b1/app/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/helpers/file_helper.py` & `notolog-0.9.1b1/app/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/helpers/theme_helper.py` & `notolog-0.9.1b1/app/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/helpers/tooltip_helper.py` & `notolog-0.9.1b1/app/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/helpers/update_helper.py` & `notolog-0.9.1b1/app/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/highlight/main_highlighter.py` & `notolog-0.9.1b1/app/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/highlight/md_highlighter.py` & `notolog-0.9.1b1/app/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/highlight/view_highlighter.py` & `notolog-0.9.1b1/app/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/image_downloader.py` & `notolog-0.9.1b1/app/image_downloader.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/__pycache__/lexemes.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/__pycache__/lexemes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/common.py` & `notolog-0.9.1b1/app/lexemes/de/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/main_menu.py` & `notolog-0.9.1b1/app/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/de/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/statusbar.py` & `notolog-0.9.1b1/app/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/de/toolbar.py` & `notolog-0.9.1b1/app/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/common.py` & `notolog-0.9.1b1/app/lexemes/en/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/main_menu.py` & `notolog-0.9.1b1/app/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/en/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/statusbar.py` & `notolog-0.9.1b1/app/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/en/toolbar.py` & `notolog-0.9.1b1/app/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/common.py` & `notolog-0.9.1b1/app/lexemes/es/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/main_menu.py` & `notolog-0.9.1b1/app/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/es/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/statusbar.py` & `notolog-0.9.1b1/app/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/es/toolbar.py` & `notolog-0.9.1b1/app/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/fi/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/fi/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/common.py` & `notolog-0.9.1b1/app/lexemes/fi/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/main_menu.py` & `notolog-0.9.1b1/app/lexemes/fi/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/fi/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/statusbar.py` & `notolog-0.9.1b1/app/lexemes/fi/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fi/toolbar.py` & `notolog-0.9.1b1/app/lexemes/fi/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/common.py` & `notolog-0.9.1b1/app/lexemes/fr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/main_menu.py` & `notolog-0.9.1b1/app/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/fr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/statusbar.py` & `notolog-0.9.1b1/app/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/fr/toolbar.py` & `notolog-0.9.1b1/app/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/common.py` & `notolog-0.9.1b1/app/lexemes/ge/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/main_menu.py` & `notolog-0.9.1b1/app/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/ge/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/statusbar.py` & `notolog-0.9.1b1/app/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ge/toolbar.py` & `notolog-0.9.1b1/app/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/gr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/gr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/common.py` & `notolog-0.9.1b1/app/lexemes/gr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/main_menu.py` & `notolog-0.9.1b1/app/lexemes/gr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/gr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/statusbar.py` & `notolog-0.9.1b1/app/lexemes/gr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/gr/toolbar.py` & `notolog-0.9.1b1/app/lexemes/gr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/in/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/in/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/common.py` & `notolog-0.9.1b1/app/lexemes/in/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/main_menu.py` & `notolog-0.9.1b1/app/lexemes/in/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/in/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/statusbar.py` & `notolog-0.9.1b1/app/lexemes/in/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/in/toolbar.py` & `notolog-0.9.1b1/app/lexemes/in/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/common.py` & `notolog-0.9.1b1/app/lexemes/it/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/main_menu.py` & `notolog-0.9.1b1/app/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/it/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/statusbar.py` & `notolog-0.9.1b1/app/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/it/toolbar.py` & `notolog-0.9.1b1/app/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 21:20:02 2024 UTC, .py size: 931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 020f 3066 a303 0000  a.........0f....
+00000000: 610d 0d0a 0000 0000 40a8 3666 a303 0000  a.......@.6f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 9c0c 5a00 640d 5300  d.d.d.d...Z.d.S.
 00000050: 290e 7518 0000 0041 4920 e381 b8e3 81ae  ).u....AI ......
 00000060: e383 aae3 82af e382 a8e3 82b9 e383 8875  ...............u
 00000070: 0f00 0000 e383 aae3 82af e382 a8e3 82b9  ................
@@ -50,15 +50,15 @@
 00000310: 6b65 6e73 5f70 726f 6d70 745a 1a64 6961  kens_promptZ.dia
 00000320: 6c6f 675f 7573 6167 655f 746f 6b65 6e73  log_usage_tokens
 00000330: 5f61 6e73 7765 72da 1964 6961 6c6f 675f  _answer..dialog_
 00000340: 7573 6167 655f 746f 6b65 6e73 5f74 6f74  usage_tokens_tot
 00000350: 616c da1a 6469 616c 6f67 5f62 7574 746f  al..dialog_butto
 00000360: 6e5f 7365 6e64 5f72 6571 7565 7374 4e29  n_send_requestN)
 00000370: 01da 076c 6578 656d 6573 a900 720d 0000  ...lexemes..r...
-00000380: 0072 0d00 0000 fa49 2f55 7365 7273 2f76  .r.....I/Users/v
+00000380: 0072 0d00 0000 fa4c 2f55 7365 7273 2f76  .r.....L/Users/v
 00000390: 6164 696b 7573 2f50 7963 6861 726d 5072  adikus/PycharmPr
-000003a0: 6f6a 6563 7473 2f6e 6f74 6f6c 6f67 2d64  ojects/notolog-d
-000003b0: 6576 2f61 7070 2f6c 6578 656d 6573 2f6a  ev/app/lexemes/j
-000003c0: 612f 6169 5f61 7373 6973 7461 6e74 2e70  a/ai_assistant.p
-000003d0: 79da 083c 6d6f 6475 6c65 3e04 0000 0073  y..<module>....s
-000003e0: 1800 0000 0201 0201 0201 0201 0201 0202  ................
-000003f0: 0201 0201 0201 0201 0201 02f2            ............
+000003a0: 6f6a 6563 7473 2f6e 6f74 6f6c 6f67 2d65  ojects/notolog-e
+000003b0: 6469 746f 722f 6170 702f 6c65 7865 6d65  ditor/app/lexeme
+000003c0: 732f 6a61 2f61 695f 6173 7369 7374 616e  s/ja/ai_assistan
+000003d0: 742e 7079 da08 3c6d 6f64 756c 653e 0400  t.py..<module>..
+000003e0: 0000 7318 0000 0002 0102 0102 0102 0102  ..s.............
+000003f0: 0102 0202 0102 0102 0102 0102 0102 f2    ...............
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 21:20:02 2024 UTC, .py size: 8464 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 020f 3066 1021 0000  a.........0f.!..
+00000000: 610d 0d0a 0000 0000 40a8 3666 1021 0000  a.......@.6f.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 008f 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
@@ -498,32 +498,32 @@
 00001f10: 5a18 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
 00001f20: 6f6c 6f72 5f77 6865 6174 5a1d 636f 6c6f  olor_wheatZ.colo
 00001f30: 725f 7069 636b 6572 5f63 6f6c 6f72 5f77  r_picker_color_w
 00001f40: 6869 7465 736d 6f6b 655a 1e63 6f6c 6f72  hitesmokeZ.color
 00001f50: 5f70 6963 6b65 725f 636f 6c6f 725f 7965  _picker_color_ye
 00001f60: 6c6c 6f77 6772 6565 6e4e 2901 da07 6c65  llowgreenN)...le
 00001f70: 7865 6d65 73a9 0072 0300 0000 7203 0000  xemes..r....r...
-00001f80: 00fa 502f 5573 6572 732f 7661 6469 6b75  ..P/Users/vadiku
+00001f80: 00fa 532f 5573 6572 732f 7661 6469 6b75  ..S/Users/vadiku
 00001f90: 732f 5079 6368 6172 6d50 726f 6a65 6374  s/PycharmProject
-00001fa0: 732f 6e6f 746f 6c6f 672d 6465 762f 6170  s/notolog-dev/ap
-00001fb0: 702f 6c65 7865 6d65 732f 6a61 2f63 6f6c  p/lexemes/ja/col
-00001fc0: 6f72 5f70 6963 6b65 725f 6469 616c 6f67  or_picker_dialog
-00001fd0: 2e70 79da 083c 6d6f 6475 6c65 3e03 0000  .py..<module>...
-00001fe0: 0073 1e01 0000 0202 0201 0201 0201 0201  .s..............
-00001ff0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002000: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002010: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002020: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002030: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002040: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002050: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002060: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002070: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002080: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002090: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000020a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000020b0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000020c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000020d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000020e0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000020f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00002100: 0280 00f1                                ....
+00001fa0: 732f 6e6f 746f 6c6f 672d 6564 6974 6f72  s/notolog-editor
+00001fb0: 2f61 7070 2f6c 6578 656d 6573 2f6a 612f  /app/lexemes/ja/
+00001fc0: 636f 6c6f 725f 7069 636b 6572 5f64 6961  color_picker_dia
+00001fd0: 6c6f 672e 7079 da08 3c6d 6f64 756c 653e  log.py..<module>
+00001fe0: 0300 0000 731e 0100 0002 0202 0102 0102  ....s...........
+00001ff0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002000: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002010: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002020: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002030: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002040: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002050: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002060: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002070: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002080: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002090: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000020a0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000020b0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000020c0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000020d0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000020e0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000020f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002100: 0102 0102 8000 f1                        .......
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May  4 03:19:30 2024 UTC, .py size: 7241 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 42a9 3566 491c 0000  a.......B.5fI...
+00000000: 610d 0d0a 0000 0000 40a8 3666 491c 0000  a.......@.6fI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0055 0000 0040 0000 0073 b200 0000 6400  .U...@...s....d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6403 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
 00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
 00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
 00000070: 6420 6421 6422 641e 641f 6423 6424 6425  d d!d"d.d.d#d$d%
@@ -405,24 +405,24 @@
 00001940: 776f 726b 5f63 6f6e 6e65 6374 696f 6e5f  work_connection_
 00001950: 6572 726f 725f 636f 6e6e 6563 7469 6f6e  error_connection
 00001960: 5f34 3034 5f65 7272 6f72 da31 6e65 7477  _404_error.1netw
 00001970: 6f72 6b5f 636f 6e6e 6563 7469 6f6e 5f65  ork_connection_e
 00001980: 7272 6f72 5f67 656e 6572 6963 5f77 6974  rror_generic_wit
 00001990: 685f 7374 6174 7573 5f63 6f64 654e 2901  h_status_codeN).
 000019a0: da07 6c65 7865 6d65 73a9 0072 5500 0000  ..lexemes..rU...
-000019b0: 7255 0000 00fa 432f 5573 6572 732f 7661  rU....C/Users/va
+000019b0: 7255 0000 00fa 462f 5573 6572 732f 7661  rU....F/Users/va
 000019c0: 6469 6b75 732f 5079 6368 6172 6d50 726f  dikus/PycharmPro
-000019d0: 6a65 6374 732f 6e6f 746f 6c6f 672d 6465  jects/notolog-de
-000019e0: 762f 6170 702f 6c65 7865 6d65 732f 6a61  v/app/lexemes/ja
-000019f0: 2f63 6f6d 6d6f 6e2e 7079 da08 3c6d 6f64  /common.py..<mod
-00001a00: 756c 653e 0300 0000 73a8 0000 0002 0102  ule>....s.......
-00001a10: 0202 0202 0102 0102 0102 0202 0102 0102  ................
-00001a20: 0102 0202 0102 0102 0102 0102 0102 0202  ................
-00001a30: 0102 0102 0102 0202 0102 0202 0102 0102  ................
-00001a40: 0202 0102 0202 0102 0102 0102 0102 0202  ................
-00001a50: 0102 0102 0102 0102 0202 0102 0102 0102  ................
-00001a60: 0102 0302 0102 0102 0102 0102 0102 0102  ................
-00001a70: 0202 0102 0102 0102 0102 0102 0202 0102  ................
-00001a80: 0102 0102 0202 0102 0202 0102 0102 0202  ................
-00001a90: 0202 0202 0202 0102 0202 0102 0102 0102  ................
-00001aa0: 0102 0102 0202 0102 0202 0202 0202 0102  ................
-00001ab0: 0202 0102 91                             .....
+000019d0: 6a65 6374 732f 6e6f 746f 6c6f 672d 6564  jects/notolog-ed
+000019e0: 6974 6f72 2f61 7070 2f6c 6578 656d 6573  itor/app/lexemes
+000019f0: 2f6a 612f 636f 6d6d 6f6e 2e70 79da 083c  /ja/common.py..<
+00001a00: 6d6f 6475 6c65 3e03 0000 0073 a800 0000  module>....s....
+00001a10: 0201 0202 0202 0201 0201 0201 0202 0201  ................
+00001a20: 0201 0201 0202 0201 0201 0201 0201 0201  ................
+00001a30: 0202 0201 0201 0201 0202 0201 0202 0201  ................
+00001a40: 0201 0202 0201 0202 0201 0201 0201 0201  ................
+00001a50: 0202 0201 0201 0201 0201 0202 0201 0201  ................
+00001a60: 0201 0201 0203 0201 0201 0201 0201 0201  ................
+00001a70: 0201 0202 0201 0201 0201 0201 0201 0202  ................
+00001a80: 0201 0201 0201 0202 0201 0202 0201 0201  ................
+00001a90: 0202 0202 0202 0202 0201 0202 0201 0201  ................
+00001aa0: 0201 0201 0201 0202 0201 0202 0202 0202  ................
+00001ab0: 0201 0202 0201 0291                      ........
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 21:20:02 2024 UTC, .py size: 2443 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 020f 3066 8b09 0000  a.........0f....
+00000000: 610d 0d0a 0000 0000 40a8 3666 8b09 0000  a.......@.6f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0029 0000 0040 0000 0073 5a00 0000 6400  .)...@...sZ...d.
 00000030: 6401 6402 6403 6404 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
 00000040: 6408 6409 640a 640b 640b 6401 640c 640d  d.d.d.d.d.d.d.d.
 00000050: 640e 640f 6410 6411 6412 6413 6414 6415  d.d.d.d.d.d.d.d.
 00000060: 6416 6417 6418 6419 641a 641b 641c 641d  d.d.d.d.d.d.d.d.
 00000070: 641d 641e 641e 641f 6420 6421 6421 6422  d.d.d.d.d d!d!d"
@@ -134,18 +134,18 @@
 00000850: 6163 6365 7373 6962 6c65 5f6e 616d 655f  accessible_name_
 00000860: 6275 675f 7265 706f 7274 da18 6163 7469  bug_report..acti
 00000870: 6f6e 735f 6865 6c70 5f6c 6162 656c 5f61  ons_help_label_a
 00000880: 626f 7574 da22 6163 7469 6f6e 735f 6865  bout."actions_he
 00000890: 6c70 5f61 6363 6573 7369 626c 655f 6e61  lp_accessible_na
 000008a0: 6d65 5f61 626f 7574 4e29 01da 076c 6578  me_aboutN)...lex
 000008b0: 656d 6573 a900 7228 0000 0072 2800 0000  emes..r(...r(...
-000008c0: fa46 2f55 7365 7273 2f76 6164 696b 7573  .F/Users/vadikus
+000008c0: fa49 2f55 7365 7273 2f76 6164 696b 7573  .I/Users/vadikus
 000008d0: 2f50 7963 6861 726d 5072 6f6a 6563 7473  /PycharmProjects
-000008e0: 2f6e 6f74 6f6c 6f67 2d64 6576 2f61 7070  /notolog-dev/app
-000008f0: 2f6c 6578 656d 6573 2f6a 612f 6d61 696e  /lexemes/ja/main
-00000900: 5f6d 656e 752e 7079 da08 3c6d 6f64 756c  _menu.py..<modul
-00000910: 653e 0300 0000 7350 0000 0002 0102 0102  e>....sP........
-00000920: 0102 0202 0102 0102 0102 0102 0102 0102  ................
-00000930: 0102 0102 0102 0202 0102 0102 0102 0102  ................
-00000940: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000950: 0102 0202 0102 0102 0102 0202 0102 0102  ................
-00000960: 0102 0102 0102 0102 0102 d4              ...........
+000008e0: 2f6e 6f74 6f6c 6f67 2d65 6469 746f 722f  /notolog-editor/
+000008f0: 6170 702f 6c65 7865 6d65 732f 6a61 2f6d  app/lexemes/ja/m
+00000900: 6169 6e5f 6d65 6e75 2e70 79da 083c 6d6f  ain_menu.py..<mo
+00000910: 6475 6c65 3e03 0000 0073 5000 0000 0201  dule>....sP.....
+00000920: 0201 0201 0202 0201 0201 0201 0201 0201  ................
+00000930: 0201 0201 0201 0201 0202 0201 0201 0201  ................
+00000940: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000950: 0201 0201 0202 0201 0201 0201 0202 0201  ................
+00000960: 0201 0201 0201 0201 0201 0201 02d4       ..............
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May  4 03:19:30 2024 UTC, .py size: 4014 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 42a9 3566 ae0f 0000  a.......B.5f....
+00000000: 610d 0d0a 0000 0000 40a8 3666 ae0f 0000  a.......@.6f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0030 0000 0040 0000 0073 6800 0000 6400  .0...@...sh...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
@@ -235,19 +235,20 @@
 00000ea0: 706f 6e73 655f 6d61 785f 746f 6b65 6e73  ponse_max_tokens
 00000eb0: 5f6c 6162 656c da3f 6169 5f63 6f6e 6669  _label.?ai_confi
 00000ec0: 675f 6261 7365 5f72 6573 706f 6e73 655f  g_base_response_
 00000ed0: 6d61 785f 746f 6b65 6e73 5f69 6e70 7574  max_tokens_input
 00000ee0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
 00000ef0: 7269 7074 696f 6e4e 2901 da07 6c65 7865  riptionN)...lexe
 00000f00: 6d65 73a9 0072 3000 0000 7230 0000 00fa  mes..r0...r0....
-00000f10: 4c2f 5573 6572 732f 7661 6469 6b75 732f  L/Users/vadikus/
+00000f10: 4f2f 5573 6572 732f 7661 6469 6b75 732f  O/Users/vadikus/
 00000f20: 5079 6368 6172 6d50 726f 6a65 6374 732f  PycharmProjects/
-00000f30: 6e6f 746f 6c6f 672d 6465 762f 6170 702f  notolog-dev/app/
-00000f40: 6c65 7865 6d65 732f 6a61 2f73 6574 7469  lexemes/ja/setti
-00000f50: 6e67 735f 6469 616c 6f67 2e70 79da 083c  ngs_dialog.py..<
-00000f60: 6d6f 6475 6c65 3e04 0000 0073 5e00 0000  module>....s^...
-00000f70: 0202 0202 0201 0201 0201 0202 0201 0201  ................
-00000f80: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000f90: 0201 0202 0201 0202 0202 0201 0201 0202  ................
-00000fa0: 0201 0201 0201 0201 0201 0201 0201 0202  ................
-00000fb0: 0202 0201 0201 0201 0201 0201 0201 0201  ................
-00000fc0: 0202 0201 0201 0202 0201 0201 02c5       ..............
+00000f30: 6e6f 746f 6c6f 672d 6564 6974 6f72 2f61  notolog-editor/a
+00000f40: 7070 2f6c 6578 656d 6573 2f6a 612f 7365  pp/lexemes/ja/se
+00000f50: 7474 696e 6773 5f64 6961 6c6f 672e 7079  ttings_dialog.py
+00000f60: da08 3c6d 6f64 756c 653e 0400 0000 735e  ..<module>....s^
+00000f70: 0000 0002 0202 0202 0102 0102 0102 0202  ................
+00000f80: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000f90: 0102 0102 0102 0202 0102 0202 0202 0102  ................
+00000fa0: 0102 0202 0102 0102 0102 0102 0102 0102  ................
+00000fb0: 0102 0202 0202 0102 0102 0102 0102 0102  ................
+00000fc0: 0102 0102 0202 0102 0102 0202 0102 0102  ................
+00000fd0: c5                                       .
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 21:20:02 2024 UTC, .py size: 1242 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 020f 3066 da04 0000  a.........0f....
+00000000: 610d 0d0a 0000 0000 40a8 3666 da04 0000  a.......@.6f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 9c11 5a00 6412 5300 2913 7509 0000  d...Z.d.S.).u...
 00000060: 00e3 8194 e381 bfe7 aeb1 751b 0000 00e3  ..........u.....
 00000070: 8194 e381 bfe7 aeb1 e381 aee5 8685 e5ae  ................
@@ -67,16 +67,16 @@
 00000420: 5f6c 6162 656c 5f73 656c 6563 7465 64da  _label_selected.
 00000430: 2273 7461 7475 7362 6172 5f63 7572 736f  "statusbar_curso
 00000440: 725f 6c61 6265 6c5f 7769 7468 5f67 6c6f  r_label_with_glo
 00000450: 6261 6cda 2b73 7461 7475 7362 6172 5f63  bal.+statusbar_c
 00000460: 7572 736f 725f 6c61 6265 6c5f 7365 6c65  ursor_label_sele
 00000470: 6374 6564 5f77 6974 685f 676c 6f62 616c  cted_with_global
 00000480: 4e29 01da 076c 6578 656d 6573 a900 720e  N)...lexemes..r.
-00000490: 0000 0072 0e00 0000 fa46 2f55 7365 7273  ...r.....F/Users
+00000490: 0000 0072 0e00 0000 fa49 2f55 7365 7273  ...r.....I/Users
 000004a0: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
 000004b0: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
-000004c0: 2d64 6576 2f61 7070 2f6c 6578 656d 6573  -dev/app/lexemes
-000004d0: 2f6a 612f 7374 6174 7573 6261 722e 7079  /ja/statusbar.py
-000004e0: da08 3c6d 6f64 756c 653e 0300 0000 7322  ..<module>....s"
-000004f0: 0000 0002 0102 0202 0102 0102 0202 0102  ................
-00000500: 0102 0202 0102 0202 0102 0102 0202 0102  ................
-00000510: 0102 0102 ea                             .....
+000004c0: 2d65 6469 746f 722f 6170 702f 6c65 7865  -editor/app/lexe
+000004d0: 6d65 732f 6a61 2f73 7461 7475 7362 6172  mes/ja/statusbar
+000004e0: 2e70 79da 083c 6d6f 6475 6c65 3e03 0000  .py..<module>...
+000004f0: 0073 2200 0000 0201 0202 0201 0201 0202  .s".............
+00000500: 0201 0201 0202 0201 0202 0201 0201 0202  ................
+00000510: 0201 0201 0201 02ea                      ........
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 21:20:02 2024 UTC, .py size: 3000 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 020f 3066 b80b 0000  a.........0f....
+00000000: 610d 0d0a 0000 0000 40a8 3666 b80b 0000  a.......@.6f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0032 0000 0040 0000 0073 6c00 0000 6400  .2...@...sl...d.
 00000030: 6400 6401 6402 6403 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
 00000040: 6408 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
 00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
 00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
 00000070: 6420 6421 6422 6423 6424 6425 6426 6427  d d!d"d#d$d%d&d'
@@ -172,20 +172,20 @@
 00000ab0: 6e73 5f6c 6162 656c 5f6e 6578 74da 2373  ns_label_next.#s
 00000ac0: 6561 7263 685f 6275 7474 6f6e 735f 6163  earch_buttons_ac
 00000ad0: 6365 7373 6962 6c65 5f6e 616d 655f 6e65  cessible_name_ne
 00000ae0: 7874 da15 7365 6172 6368 5f63 6173 655f  xt..search_case_
 00000af0: 7365 6e73 6974 6976 65da 1973 6561 7263  sensitive..searc
 00000b00: 685f 6d61 7463 685f 6361 7365 5f74 6f6f  h_match_case_too
 00000b10: 6c74 6970 4e29 01da 076c 6578 656d 6573  ltipN)...lexemes
-00000b20: a900 722f 0000 0072 2f00 0000 fa44 2f55  ..r/...r/....D/U
+00000b20: a900 722f 0000 0072 2f00 0000 fa47 2f55  ..r/...r/....G/U
 00000b30: 7365 7273 2f76 6164 696b 7573 2f50 7963  sers/vadikus/Pyc
 00000b40: 6861 726d 5072 6f6a 6563 7473 2f6e 6f74  harmProjects/not
-00000b50: 6f6c 6f67 2d64 6576 2f61 7070 2f6c 6578  olog-dev/app/lex
-00000b60: 656d 6573 2f6a 612f 746f 6f6c 6261 722e  emes/ja/toolbar.
-00000b70: 7079 da08 3c6d 6f64 756c 653e 0300 0000  py..<module>....
-00000b80: 7362 0000 0002 0102 0102 0102 0102 0102  sb..............
-00000b90: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000ba0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000bb0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000bc0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000bd0: 0202 0102 0102 0102 0102 0102 0102 0102  ................
-00000be0: 0102 0102 0102 ce                        .......
+00000b50: 6f6c 6f67 2d65 6469 746f 722f 6170 702f  olog-editor/app/
+00000b60: 6c65 7865 6d65 732f 6a61 2f74 6f6f 6c62  lexemes/ja/toolb
+00000b70: 6172 2e70 79da 083c 6d6f 6475 6c65 3e03  ar.py..<module>.
+00000b80: 0000 0073 6200 0000 0201 0201 0201 0201  ...sb...........
+00000b90: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000ba0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000bb0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000bc0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000bd0: 0201 0202 0201 0201 0201 0201 0201 0201  ................
+00000be0: 0201 0201 0201 0201 02ce                 ..........
```

### Comparing `notolog-0.9.1b0/app/lexemes/ja/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/common.py` & `notolog-0.9.1b1/app/lexemes/ja/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/main_menu.py` & `notolog-0.9.1b1/app/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/ja/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/statusbar.py` & `notolog-0.9.1b1/app/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ja/toolbar.py` & `notolog-0.9.1b1/app/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/common.py` & `notolog-0.9.1b1/app/lexemes/ko/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/main_menu.py` & `notolog-0.9.1b1/app/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/ko/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/statusbar.py` & `notolog-0.9.1b1/app/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ko/toolbar.py` & `notolog-0.9.1b1/app/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/common.py` & `notolog-0.9.1b1/app/lexemes/la/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/main_menu.py` & `notolog-0.9.1b1/app/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/la/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/statusbar.py` & `notolog-0.9.1b1/app/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/la/toolbar.py` & `notolog-0.9.1b1/app/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/lexemes.py` & `notolog-0.9.1b1/app/lexemes/lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/common.py` & `notolog-0.9.1b1/app/lexemes/pt/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/main_menu.py` & `notolog-0.9.1b1/app/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/pt/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/statusbar.py` & `notolog-0.9.1b1/app/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/pt/toolbar.py` & `notolog-0.9.1b1/app/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/common.py` & `notolog-0.9.1b1/app/lexemes/ru/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/main_menu.py` & `notolog-0.9.1b1/app/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/ru/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/statusbar.py` & `notolog-0.9.1b1/app/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/ru/toolbar.py` & `notolog-0.9.1b1/app/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May  5 14:33:15 2024 UTC, .py size: 835 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-00000000: 610d 0d0a 0000 0000 ab98 3766 4303 0000  a.........7fC...
+00000000: 610d 0d0a 0000 0000 42a9 3566 2903 0000  a.......B.5f)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 9c0c 5a00 640d 5300  d.d.d.d...Z.d.S.
-00000050: 290e 7513 0000 0046 c3b6 7266 72c3 a567  ).u....F..rfr..g
-00000060: 616e 2074 696c 6c20 4149 750b 0000 0046  an till AIu....F
-00000070: c3b6 7266 72c3 a567 616e 753b 0000 0041  ..rfr..ganu;...A
-00000080: 6e67 6520 656e 2066 c3b6 7266 72c3 a567  nge en f..rfr..g
-00000090: 616e 2066 c3b6 7220 6174 7420 6765 206b  an f..r att ge k
-000000a0: 6f6e 7465 7874 2074 696c 6c20 4149 2d61  ontext till AI-a
-000000b0: 7373 6973 7465 6e74 656e 5a09 5376 6172  ssistentenZ.Svar
-000000c0: 7364 6174 6175 2800 0000 5376 6172 7364  sdatau(...Svarsd
-000000d0: 6174 6120 6b6f 6d6d 6572 2061 7474 2076  ata kommer att v
-000000e0: 6973 6173 2069 2064 6574 7461 2066 c3a4  isas i detta f..
-000000f0: 6c74 7525 0000 0041 6e67 6520 7465 7874  ltu%...Ange text
-00000100: 2066 c3b6 7220 6174 7420 66c3 a520 6574   f..r att f.. et
-00000110: 7420 7376 6172 206f 6d2e 2e2e 5a06 4d4f  t svar om...Z.MO
-00000120: 4445 4c4c 5a06 544f 4b45 4e53 7a10 7072  DELLZ.TOKENSz.pr
-00000130: 6f6d 7074 3a20 7b74 6f6b 656e 737d 7a0e  ompt: {tokens}z.
-00000140: 7376 6172 3a20 7b74 6f6b 656e 737d 7a10  svar: {tokens}z.
-00000150: 746f 7461 6c74 3a20 7b74 6f6b 656e 737d  totalt: {tokens}
-00000160: 7512 0000 0053 6b69 636b 6120 66c3 b672  u....Skicka f..r
-00000170: 6672 c3a5 6761 6e29 0cda 0c64 6961 6c6f  fr..gan)...dialo
-00000180: 675f 7469 746c 65da 2464 6961 6c6f 675f  g_title.$dialog_
-00000190: 7072 6f6d 7074 5f69 6e70 7574 5f70 6c61  prompt_input_pla
-000001a0: 6365 686f 6c64 6572 5f74 6578 74da 2a64  ceholder_text.*d
-000001b0: 6961 6c6f 675f 7072 6f6d 7074 5f69 6e70  ialog_prompt_inp
-000001c0: 7574 5f61 6363 6573 7369 626c 655f 6465  ut_accessible_de
-000001d0: 7363 7269 7074 696f 6eda 2764 6961 6c6f  scription.'dialo
-000001e0: 675f 7265 7370 6f6e 7365 5f6f 7574 7075  g_response_outpu
-000001f0: 745f 706c 6163 6568 6f6c 6465 725f 7465  t_placeholder_te
-00000200: 7874 da2d 6469 616c 6f67 5f72 6573 706f  xt.-dialog_respo
-00000210: 6e73 655f 6f75 7470 7574 5f61 6363 6573  nse_output_acces
-00000220: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000230: 6eda 2864 6961 6c6f 675f 7265 7370 6f6e  n.(dialog_respon
-00000240: 7365 5f6f 7574 7075 745f 6e6f 7469 6365  se_output_notice
-00000250: 5f65 6d70 7479 5f74 6578 74da 1864 6961  _empty_text..dia
-00000260: 6c6f 675f 7573 6167 655f 6d6f 6465 6c5f  log_usage_model_
-00000270: 6c61 6265 6cda 1964 6961 6c6f 675f 7573  label..dialog_us
-00000280: 6167 655f 746f 6b65 6e73 5f6c 6162 656c  age_tokens_label
-00000290: da1a 6469 616c 6f67 5f75 7361 6765 5f74  ..dialog_usage_t
-000002a0: 6f6b 656e 735f 7072 6f6d 7074 da1a 6469  okens_prompt..di
-000002b0: 616c 6f67 5f75 7361 6765 5f74 6f6b 656e  alog_usage_token
-000002c0: 735f 616e 7377 6572 da19 6469 616c 6f67  s_answer..dialog
-000002d0: 5f75 7361 6765 5f74 6f6b 656e 735f 746f  _usage_tokens_to
-000002e0: 7461 6cda 1a64 6961 6c6f 675f 6275 7474  tal..dialog_butt
-000002f0: 6f6e 5f73 656e 645f 7265 7175 6573 744e  on_send_requestN
-00000300: 2901 da07 6c65 7865 6d65 73a9 0072 0e00  )...lexemes..r..
-00000310: 0000 720e 0000 00fa 4c2f 5573 6572 732f  ..r.....L/Users/
-00000320: 7661 6469 6b75 732f 5079 6368 6172 6d50  vadikus/PycharmP
-00000330: 726f 6a65 6374 732f 6e6f 746f 6c6f 672d  rojects/notolog-
-00000340: 6564 6974 6f72 2f61 7070 2f6c 6578 656d  editor/app/lexem
-00000350: 6573 2f73 652f 6169 5f61 7373 6973 7461  es/se/ai_assista
-00000360: 6e74 2e70 79da 083c 6d6f 6475 6c65 3e04  nt.py..<module>.
+00000050: 290e 750c 0000 0041 4927 7961 20c4 b073  ).u....AI'ya ..s
+00000060: 7465 6b75 0600 0000 c4b0 7374 656b 7536  teku......steku6
+00000070: 0000 0041 4920 7961 7264 c4b1 6d63 c4b1  ...AI yard..mc..
+00000080: 73c4 b16e 6120 6261 c49f 6c61 6d20 7361  s..na ba..lam sa
+00000090: c49f 6c61 6d61 6b20 69c3 a769 6e20 6973  ..lamak i..in is
+000000a0: 7465 6b20 6769 7269 6e75 0d00 0000 5961  tek girinu....Ya
+000000b0: 6ec4 b174 2076 6572 6973 6975 2300 0000  n..t verisiu#...
+000000c0: 5961 6ec4 b174 2076 6572 6973 6920 6275  Yan..t verisi bu
+000000d0: 2061 6c61 6e64 6120 67c3 b672 c3bc 6e65   alanda g..r..ne
+000000e0: 6365 6b75 3a00 0000 5961 6b6c 61c5 9fc4  ceku:...Yakla...
+000000f0: b16b 2062 6972 2079 616e c4b1 7420 616c  .k bir yan..t al
+00000100: 6d61 6b20 69c3 a769 6e20 6d65 7469 6e20  mak i..in metin 
+00000110: 6769 7269 c59f 6920 7361 c49f 6c61 79c4  giri..i sa..lay.
+00000120: b16e da05 4d4f 4445 4c5a 0854 4f4b 454e  .n..MODELZ.TOKEN
+00000130: 4c41 527a 0f69 7374 656b 3a20 7b74 6f6b  LARz.istek: {tok
+00000140: 656e 737d 7a0f 6365 7661 703a 207b 746f  ens}z.cevap: {to
+00000150: 6b65 6e73 7d7a 1074 6f70 6c61 6d3a 207b  kens}z.toplam: {
+00000160: 746f 6b65 6e73 7d75 0e00 0000 c4b0 7374  tokens}u......st
+00000170: 656b 2047 c3b6 6e64 6572 290c da0c 6469  ek G..nder)...di
+00000180: 616c 6f67 5f74 6974 6c65 da24 6469 616c  alog_title.$dial
+00000190: 6f67 5f70 726f 6d70 745f 696e 7075 745f  og_prompt_input_
+000001a0: 706c 6163 6568 6f6c 6465 725f 7465 7874  placeholder_text
+000001b0: da2a 6469 616c 6f67 5f70 726f 6d70 745f  .*dialog_prompt_
+000001c0: 696e 7075 745f 6163 6365 7373 6962 6c65  input_accessible
+000001d0: 5f64 6573 6372 6970 7469 6f6e da27 6469  _description.'di
+000001e0: 616c 6f67 5f72 6573 706f 6e73 655f 6f75  alog_response_ou
+000001f0: 7470 7574 5f70 6c61 6365 686f 6c64 6572  tput_placeholder
+00000200: 5f74 6578 74da 2d64 6961 6c6f 675f 7265  _text.-dialog_re
+00000210: 7370 6f6e 7365 5f6f 7574 7075 745f 6163  sponse_output_ac
+00000220: 6365 7373 6962 6c65 5f64 6573 6372 6970  cessible_descrip
+00000230: 7469 6f6e da28 6469 616c 6f67 5f72 6573  tion.(dialog_res
+00000240: 706f 6e73 655f 6f75 7470 7574 5f6e 6f74  ponse_output_not
+00000250: 6963 655f 656d 7074 795f 7465 7874 da18  ice_empty_text..
+00000260: 6469 616c 6f67 5f75 7361 6765 5f6d 6f64  dialog_usage_mod
+00000270: 656c 5f6c 6162 656c da19 6469 616c 6f67  el_label..dialog
+00000280: 5f75 7361 6765 5f74 6f6b 656e 735f 6c61  _usage_tokens_la
+00000290: 6265 6cda 1a64 6961 6c6f 675f 7573 6167  bel..dialog_usag
+000002a0: 655f 746f 6b65 6e73 5f70 726f 6d70 74da  e_tokens_prompt.
+000002b0: 1a64 6961 6c6f 675f 7573 6167 655f 746f  .dialog_usage_to
+000002c0: 6b65 6e73 5f61 6e73 7765 72da 1964 6961  kens_answer..dia
+000002d0: 6c6f 675f 7573 6167 655f 746f 6b65 6e73  log_usage_tokens
+000002e0: 5f74 6f74 616c da1a 6469 616c 6f67 5f62  _total..dialog_b
+000002f0: 7574 746f 6e5f 7365 6e64 5f72 6571 7565  utton_send_reque
+00000300: 7374 4e29 01da 076c 6578 656d 6573 a900  stN)...lexemes..
+00000310: 720f 0000 0072 0f00 0000 fa49 2f55 7365  r....r.....I/Use
+00000320: 7273 2f76 6164 696b 7573 2f50 7963 6861  rs/vadikus/Pycha
+00000330: 726d 5072 6f6a 6563 7473 2f6e 6f74 6f6c  rmProjects/notol
+00000340: 6f67 2d64 6576 2f61 7070 2f6c 6578 656d  og-dev/app/lexem
+00000350: 6573 2f74 722f 6169 5f61 7373 6973 7461  es/tr/ai_assista
+00000360: 6e74 2e70 79da 083c 6d6f 6475 6c65 3e03  nt.py..<module>.
 00000370: 0000 0073 1800 0000 0201 0201 0201 0201  ...s............
-00000380: 0201 0202 0201 0201 0201 0201 0201 02f2  ................
+00000380: 0201 0202 0201 0201 0201 0201 0201 02f3  ................
```

### Comparing `notolog-0.9.1b0/app/lexemes/se/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May  5 14:33:15 2024 UTC, .py size: 7048 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,427 +1,445 @@
-00000000: 610d 0d0a 0000 0000 ab98 3766 881b 0000  a.........7f....
+00000000: 610d 0d0a 0000 0000 42a9 3566 e91c 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 008f 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
-00000080: 6429 642a 642b 642c 642d 642e 642f 6430  d)d*d+d,d-d.d/d0
-00000090: 6431 6432 6433 6434 6435 6436 6437 6438  d1d2d3d4d5d6d7d8
-000000a0: 6439 643a 643b 643c 643d 643e 643f 6440  d9d:d;d<d=d>d?d@
-000000b0: 6441 6442 6443 6444 6445 6446 6447 6448  dAdBdCdDdEdFdGdH
-000000c0: 6449 644a 644b 644c 644d 644e 644f 6450  dIdJdKdLdMdNdOdP
-000000d0: 6451 6452 6453 6454 6455 6456 640a 6457  dQdRdSdTdUdVd.dW
-000000e0: 6458 6459 645a 645b 645c 645d 645e 645f  dXdYdZd[d\d]d^d_
-000000f0: 6460 6461 6462 6463 6464 6465 6466 6467  d`dadbdcdddedfdg
-00000100: 6468 6469 646a 646b 646c 646d 646e 646f  dhdidjdkdldmdndo
-00000110: 6470 6471 6472 6473 6474 6475 6476 6477  dpdqdrdsdtdudvdw
-00000120: 6478 6479 647a 647b 647c 647d 647e 647f  dxdydzd{d|d}d~d.
-00000130: 6480 6481 6482 6483 6484 6485 6486 6487  d.d.d.d.d.d.d.d.
-00000140: 6488 6489 648a 648b 648c 648d 9c8e 5a00  d.d.d.d.d.d...Z.
-00000150: 648e 5300 298f 750e 0000 0056 c3a4 6c6a  d.S.).u....V..lj
-00000160: 2065 6e20 66c3 a472 675a 0553 7661 7274   en f..rgZ.Svart
-00000170: da06 5369 6c76 6572 7504 0000 0047 72c3  ..Silveru....Gr.
-00000180: a55a 0356 6974 7508 0000 0052 c3b6 6462  .Z.Vitu....R..db
-00000190: 7275 6e75 0400 0000 52c3 b664 5a04 4c69  runu....R..dZ.Li
-000001a0: 6c61 5a07 4675 6368 7369 6175 0500 0000  laZ.Fuchsiau....
-000001b0: 4772 c3b6 6e75 0900 0000 4c69 6d65 6772  Gr..nu....Limegr
-000001c0: c3b6 6e5a 044f 6c69 765a 0347 756c 7509  ..nZ.OlivZ.Gulu.
-000001d0: 0000 004d 6172 696e 626c c3a5 7504 0000  ...Marinbl..u...
-000001e0: 0042 6cc3 a5da 0454 6561 6c5a 0941 6b76  .Bl....TealZ.Akv
-000001f0: 616d 6172 696e 7509 0000 0041 6c69 6365  amarinu....Alice
-00000200: 626c c3a5 5a08 416e 7469 6b76 6974 da0a  bl..Z.Antikvit..
-00000210: 4171 7561 6d61 7269 6e65 7508 0000 0041  Aquamarineu....A
-00000220: 7a75 7262 6cc3 a5da 0542 6569 6765 da06  zurbl....Beige..
-00000230: 4269 7371 7565 750f 0000 0053 6bc3 a56c  Bisqueu....Sk..l
-00000240: 6c61 6420 6d61 6e64 656c 750b 0000 0042  lad mandelu....B
-00000250: 6cc3 a576 696f 6c65 7474 5a04 4272 756e  l..violettZ.Brun
-00000260: 5a09 4275 726c 7977 6f6f 6475 0a00 0000  Z.Burlywoodu....
-00000270: 4b61 6465 7474 626c c3a5 da0a 4368 6172  Kadettbl....Char
-00000280: 7472 6575 7365 5a07 4368 6f6b 6c61 645a  treuseZ.ChokladZ
-00000290: 064b 6f72 616c 6c75 0800 0000 4b6f 726e  .Korallu....Korn
-000002a0: 626c c3a5 5a09 4d61 6a73 7369 6c6b 655a  bl..Z.MajssilkeZ
-000002b0: 084b 6172 6d6f 7369 6eda 0443 7961 6e75  .Karmosin..Cyanu
-000002c0: 0900 0000 4dc3 b672 6b62 6cc3 a575 0a00  ....M..rkbl..u..
-000002d0: 0000 4dc3 b672 6b20 6379 616e 7512 0000  ..M..rk cyanu...
-000002e0: 004d c3b6 726b 2067 796c 6c65 6e73 74c3  .M..rk gyllenst.
-000002f0: a56e 6775 0900 0000 4dc3 b672 6b67 72c3  .ngu....M..rkgr.
-00000300: a575 0a00 0000 4dc3 b672 6b67 72c3 b66e  .u....M..rkgr..n
-00000310: 750b 0000 004d c3b6 726b 206b 6861 6b69  u....M..rk khaki
-00000320: 750d 0000 004d c3b6 726b 206d 6167 656e  u....M..rk magen
-00000330: 7461 750e 0000 004d c3b6 726b 6f6c 6976  tau....M..rkoliv
-00000340: 6772 c3b6 6e75 0b00 0000 4dc3 b672 6b6f  gr..nu....M..rko
-00000350: 7261 6e67 6575 0d00 0000 4dc3 b672 6b20  rangeu....M..rk 
-00000360: 6f72 6b69 64c3 a975 0900 0000 4dc3 b672  orkid..u....M..r
-00000370: 6b72 c3b6 6475 0800 0000 4dc3 b672 6b6c  kr..du....M..rkl
-00000380: 6178 7510 0000 004d c3b6 726b 7420 6861  axu....M..rkt ha
-00000390: 7673 6772 c3b6 6e75 1100 0000 4dc3 b672  vsgr..nu....M..r
-000003a0: 6b20 736b 6966 6665 7262 6cc3 a575 1100  k skifferbl..u..
-000003b0: 0000 4dc3 b672 6b20 736b 6966 6665 7267  ..M..rk skifferg
-000003c0: 72c3 a575 0b00 0000 4dc3 b672 6b74 7572  r..u....M..rktur
-000003d0: 6b6f 7375 0c00 0000 4dc3 b672 6b76 696f  kosu....M..rkvio
-000003e0: 6c65 7474 5a08 446a 7570 726f 7361 750f  lettZ.Djuprosau.
-000003f0: 0000 0044 6a75 7068 696d 6d65 6c73 626c  ...Djuphimmelsbl
-00000400: c3a5 7507 0000 0044 696d 6772 c3a5 750a  ..u....Dimgr..u.
-00000410: 0000 0044 6f64 6765 7262 6cc3 a55a 074d  ...Dodgerbl..Z.M
-00000420: 7572 7374 656e 5a0b 426c 6f6d 7374 6572  urstenZ.Blomster
-00000430: 7669 7475 0a00 0000 536b 6f67 7367 72c3  vitu....Skogsgr.
-00000440: b66e da09 4761 696e 7362 6f72 6f75 0800  .n..Gainsborou..
-00000450: 0000 5370 c3b6 6b76 6974 5a04 4775 6c64  ..Sp..kvitZ.Guld
-00000460: 750c 0000 0047 796c 6c65 6e73 74c3 a56e  u....Gyllenst..n
-00000470: 6775 0800 0000 4772 c3b6 6e67 756c 5a0b  gu....Gr..ngulZ.
-00000480: 486f 6e75 6e67 7364 6167 677a 0948 6574  Honungsdaggz.Het
-00000490: 7420 726f 7361 750b 0000 0049 6e64 6973  t rosau....Indis
-000004a0: 6b20 72c3 b664 da06 496e 6469 676f 5a08  k r..d..IndigoZ.
-000004b0: 456c 6665 6e62 656e da05 4b68 616b 695a  Elfenben..KhakiZ
-000004c0: 084c 6176 656e 6465 6c5a 0c4c 6176 656e  .LavendelZ.Laven
-000004d0: 6465 6c72 6f73 6175 0f00 0000 4772 c3a4  delrosau....Gr..
-000004e0: 736d 6174 7461 6772 c3b6 6e5a 0e43 6974  smattagr..nZ.Cit
-000004f0: 726f 6e63 6869 6666 6f6e 6775 0800 0000  ronchiffongu....
-00000500: 4c6a 7573 626c c3a5 5a0a 4c6a 7573 6b6f  Ljusbl..Z.Ljusko
-00000510: 7261 6c6c 7a09 4c6a 7573 2063 7961 6e75  rallz.Ljus cyanu
-00000520: 1500 0000 4c6a 7573 2067 796c 6c65 6e73  ....Ljus gyllens
-00000530: 74c3 a56e 6773 6775 6c75 0800 0000 4c6a  t..ngsgulu....Lj
-00000540: 7573 6772 c3a5 7509 0000 004c 6a75 7367  usgr..u....Ljusg
-00000550: 72c3 b66e 5a08 4c6a 7573 726f 7361 5a07  r..nZ.LjusrosaZ.
-00000560: 4c6a 7573 6c61 7875 0f00 0000 4c6a 7573  Ljuslaxu....Ljus
-00000570: 7420 6861 7673 6772 c3b6 6e75 1000 0000  t havsgr..nu....
-00000580: 4c6a 7573 2068 696d 6d65 6c73 626c c3a5  Ljus himmelsbl..
-00000590: 7510 0000 004c 6a75 7320 736b 6966 6665  u....Ljus skiffe
-000005a0: 7267 72c3 a575 0f00 0000 4c6a 7573 7420  rgr..u....Ljust 
-000005b0: 7374 c3a5 6c62 6cc3 a55a 074c 6a75 7367  st..lbl..Z.Ljusg
-000005c0: 756c 5a08 4c69 6e6e 6574 7967 da07 4d61  ulZ.Linnetyg..Ma
-000005d0: 6765 6e74 617a 114d 656c 6c61 6e20 6171  gentaz.Mellan aq
-000005e0: 7561 6d61 7269 6e65 750a 0000 004d 656c  uamarineu....Mel
-000005f0: 6c61 6e62 6cc3 a575 0e00 0000 4d65 6c6c  lanbl..u....Mell
-00000600: 616e 206f 726b 6964 c3a9 5a0a 4d65 6c6c  an orkid..Z.Mell
-00000610: 616e 6c69 6c61 7511 0000 004d 656c 6c61  anlilau....Mella
-00000620: 6e74 2068 6176 7367 72c3 b66e 7512 0000  nt havsgr..nu...
-00000630: 004d 656c 6c61 6e20 736b 6966 6665 7262  .Mellan skifferb
-00000640: 6cc3 a575 1100 0000 4d65 6c6c 616e 7420  l..u....Mellant 
-00000650: 76c3 a572 6772 c3b6 6e5a 0c4d 656c 6c61  v..rgr..nZ.Mella
-00000660: 6e74 7572 6b6f 7375 1100 0000 4d65 6c6c  nturkosu....Mell
-00000670: 616e 2076 696f 6c65 7472 c3b6 6475 0c00  an violetr..du..
-00000680: 0000 4d69 646e 6174 7473 626c c3a5 7509  ..Midnattsbl..u.
-00000690: 0000 004d 696e 746b 72c3 a46d 5a07 4469  ...Mintkr..mZ.Di
-000006a0: 6d72 6f73 615a 084d 6f63 6b61 7369 6e5a  mrosaZ.MockasinZ
-000006b0: 094e 6176 616a 6f76 6974 7a0c 4761 6d6d  .Navajovitz.Gamm
-000006c0: 616c 2073 7065 7473 5a09 4f6c 6976 7472  al spetsZ.Olivtr
-000006d0: 6973 74da 064f 7261 6e67 6575 0a00 0000  ist..Orangeu....
-000006e0: 4f72 616e 6765 72c3 b664 7507 0000 004f  Oranger..du....O
-000006f0: 726b 6964 c3a9 7511 0000 0042 6c65 6b20  rkid..u....Blek 
-00000700: 6779 6c6c 656e 7374 c3a5 6e67 7509 0000  gyllenst..ngu...
-00000710: 0042 6c65 6b67 72c3 b66e 5a0a 426c 656b  .Blekgr..nZ.Blek
-00000720: 7475 726b 6f73 750f 0000 0042 6c65 6b20  turkosu....Blek 
-00000730: 7669 6f6c 6574 72c3 b664 750d 0000 0050  violetr..du....P
-00000740: 6170 6179 6167 72c3 a464 6465 5a0b 5065  apayagr..ddeZ.Pe
-00000750: 7273 696b 6f70 7566 66da 0450 6572 755a  rsikopuff..PeruZ
-00000760: 0452 6f73 615a 0750 6c6f 6d6d 6f6e 750a  .RosaZ.Plommonu.
-00000770: 0000 0050 756c 7665 7262 6cc3 a55a 0b52  ...Pulverbl..Z.R
-00000780: 6562 6563 6361 6c69 6c61 5a09 526f 7365  ebeccalilaZ.Rose
-00000790: 6e62 7275 6e75 0900 0000 4b75 6e67 7362  nbrunu....Kungsb
-000007a0: 6cc3 a55a 0953 6164 656c 6272 756e 5a03  l..Z.SadelbrunZ.
-000007b0: 4c61 785a 0853 616e 6462 7275 6e75 0900  LaxZ.Sandbrunu..
-000007c0: 0000 4861 7673 6772 c3b6 6e75 0a00 0000  ..Havsgr..nu....
-000007d0: 536e c3a4 636b 736b 616c 5a06 5369 656e  Sn..ckskalZ.Sien
-000007e0: 6e61 750b 0000 0048 696d 6d65 6c73 626c  nau....Himmelsbl
-000007f0: c3a5 750b 0000 0053 6b69 6666 6572 626c  ..u....Skifferbl
-00000800: c3a5 750b 0000 0053 6b69 6666 6572 6772  ..u....Skiffergr
-00000810: c3a5 7504 0000 0053 6ec3 b675 0900 0000  ..u....Sn..u....
-00000820: 56c3 a572 6772 c3b6 6e75 0900 0000 5374  V..rgr..nu....St
-00000830: c3a5 6c62 6cc3 a55a 0354 616e 5a06 5469  ..lbl..Z.TanZ.Ti
-00000840: 7374 656c 5a05 546f 6d61 745a 0654 7572  stelZ.TomatZ.Tur
-00000850: 6b6f 735a 0756 696f 6c65 7474 5a04 5665  kosZ.ViolettZ.Ve
-00000860: 7465 7507 0000 0056 6974 72c3 b66b 7508  teu....Vitr..ku.
-00000870: 0000 0047 756c 6772 c3b6 6e29 8eda 1263  ...Gulgr..n)...c
-00000880: 6f6c 6f72 5f70 6963 6b65 725f 7469 746c  olor_picker_titl
-00000890: 65da 1863 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
-000008a0: 636f 6c6f 725f 626c 6163 6bda 1963 6f6c  color_black..col
-000008b0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-000008c0: 7369 6c76 6572 da17 636f 6c6f 725f 7069  silver..color_pi
-000008d0: 636b 6572 5f63 6f6c 6f72 5f67 7261 79da  cker_color_gray.
-000008e0: 1863 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-000008f0: 6c6f 725f 7768 6974 65da 1963 6f6c 6f72  lor_white..color
-00000900: 5f70 6963 6b65 725f 636f 6c6f 725f 6d61  _picker_color_ma
-00000910: 726f 6f6e da16 636f 6c6f 725f 7069 636b  roon..color_pick
-00000920: 6572 5f63 6f6c 6f72 5f72 6564 da19 636f  er_color_red..co
-00000930: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00000940: 5f70 7572 706c 65da 1a63 6f6c 6f72 5f70  _purple..color_p
-00000950: 6963 6b65 725f 636f 6c6f 725f 6675 6368  icker_color_fuch
-00000960: 7369 61da 1863 6f6c 6f72 5f70 6963 6b65  sia..color_picke
-00000970: 725f 636f 6c6f 725f 6772 6565 6eda 1763  r_color_green..c
-00000980: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000990: 725f 6c69 6d65 da18 636f 6c6f 725f 7069  r_lime..color_pi
-000009a0: 636b 6572 5f63 6f6c 6f72 5f6f 6c69 7665  cker_color_olive
-000009b0: da19 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
-000009c0: 6f6c 6f72 5f79 656c 6c6f 77da 1763 6f6c  olor_yellow..col
-000009d0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-000009e0: 6e61 7679 da17 636f 6c6f 725f 7069 636b  navy..color_pick
-000009f0: 6572 5f63 6f6c 6f72 5f62 6c75 65da 1763  er_color_blue..c
-00000a00: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000a10: 725f 7465 616c da17 636f 6c6f 725f 7069  r_teal..color_pi
-00000a20: 636b 6572 5f63 6f6c 6f72 5f61 7175 61da  cker_color_aqua.
-00000a30: 1c63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00000a40: 6c6f 725f 616c 6963 6562 6c75 65da 1f63  lor_aliceblue..c
-00000a50: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000a60: 725f 616e 7469 7175 6577 6869 7465 da1d  r_antiquewhite..
-00000a70: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000a80: 6f72 5f61 7175 616d 6172 696e 65da 1863  or_aquamarine..c
-00000a90: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000aa0: 725f 617a 7572 65da 1863 6f6c 6f72 5f70  r_azure..color_p
-00000ab0: 6963 6b65 725f 636f 6c6f 725f 6265 6967  icker_color_beig
-00000ac0: 65da 1963 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
-00000ad0: 636f 6c6f 725f 6269 7371 7565 da21 636f  color_bisque.!co
-00000ae0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00000af0: 5f62 6c61 6e63 6865 6461 6c6d 6f6e 64da  _blanchedalmond.
-00000b00: 1d63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00000b10: 6c6f 725f 626c 7565 7669 6f6c 6574 da18  lor_blueviolet..
-00000b20: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000b30: 6f72 5f62 726f 776e da1c 636f 6c6f 725f  or_brown..color_
-00000b40: 7069 636b 6572 5f63 6f6c 6f72 5f62 7572  picker_color_bur
-00000b50: 6c79 776f 6f64 da1c 636f 6c6f 725f 7069  lywood..color_pi
-00000b60: 636b 6572 5f63 6f6c 6f72 5f63 6164 6574  cker_color_cadet
-00000b70: 626c 7565 da1d 636f 6c6f 725f 7069 636b  blue..color_pick
-00000b80: 6572 5f63 6f6c 6f72 5f63 6861 7274 7265  er_color_chartre
-00000b90: 7573 65da 1c63 6f6c 6f72 5f70 6963 6b65  use..color_picke
-00000ba0: 725f 636f 6c6f 725f 6368 6f63 6f6c 6174  r_color_chocolat
-00000bb0: 65da 1863 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
-00000bc0: 636f 6c6f 725f 636f 7261 6cda 2163 6f6c  color_coral.!col
-00000bd0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00000be0: 636f 726e 666c 6f77 6572 626c 7565 da1b  cornflowerblue..
-00000bf0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000c00: 6f72 5f63 6f72 6e73 696c 6bda 1a63 6f6c  or_cornsilk..col
-00000c10: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00000c20: 6372 696d 736f 6eda 1763 6f6c 6f72 5f70  crimson..color_p
-00000c30: 6963 6b65 725f 636f 6c6f 725f 6379 616e  icker_color_cyan
-00000c40: da1b 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
-00000c50: 6f6c 6f72 5f64 6172 6b62 6c75 65da 1b63  olor_darkblue..c
-00000c60: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000c70: 725f 6461 726b 6379 616e da20 636f 6c6f  r_darkcyan. colo
-00000c80: 725f 7069 636b 6572 5f63 6f6c 6f72 5f64  r_picker_color_d
-00000c90: 6172 6b67 6f6c 6465 6e72 6f64 da1b 636f  arkgoldenrod..co
-00000ca0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00000cb0: 5f64 6172 6b67 7261 79da 1c63 6f6c 6f72  _darkgray..color
-00000cc0: 5f70 6963 6b65 725f 636f 6c6f 725f 6461  _picker_color_da
-00000cd0: 726b 6772 6565 6eda 1c63 6f6c 6f72 5f70  rkgreen..color_p
-00000ce0: 6963 6b65 725f 636f 6c6f 725f 6461 726b  icker_color_dark
-00000cf0: 6b68 616b 69da 1e63 6f6c 6f72 5f70 6963  khaki..color_pic
-00000d00: 6b65 725f 636f 6c6f 725f 6461 726b 6d61  ker_color_darkma
-00000d10: 6765 6e74 61da 2163 6f6c 6f72 5f70 6963  genta.!color_pic
-00000d20: 6b65 725f 636f 6c6f 725f 6461 726b 6f6c  ker_color_darkol
-00000d30: 6976 6567 7265 656e da1d 636f 6c6f 725f  ivegreen..color_
-00000d40: 7069 636b 6572 5f63 6f6c 6f72 5f64 6172  picker_color_dar
-00000d50: 6b6f 7261 6e67 65da 1d63 6f6c 6f72 5f70  korange..color_p
-00000d60: 6963 6b65 725f 636f 6c6f 725f 6461 726b  icker_color_dark
-00000d70: 6f72 6368 6964 da1a 636f 6c6f 725f 7069  orchid..color_pi
-00000d80: 636b 6572 5f63 6f6c 6f72 5f64 6172 6b72  cker_color_darkr
-00000d90: 6564 da1d 636f 6c6f 725f 7069 636b 6572  ed..color_picker
-00000da0: 5f63 6f6c 6f72 5f64 6172 6b73 616c 6d6f  _color_darksalmo
-00000db0: 6eda 1f63 6f6c 6f72 5f70 6963 6b65 725f  n..color_picker_
-00000dc0: 636f 6c6f 725f 6461 726b 7365 6167 7265  color_darkseagre
-00000dd0: 656e da20 636f 6c6f 725f 7069 636b 6572  en. color_picker
-00000de0: 5f63 6f6c 6f72 5f64 6172 6b73 6c61 7465  _color_darkslate
-00000df0: 626c 7565 da20 636f 6c6f 725f 7069 636b  blue. color_pick
-00000e00: 6572 5f63 6f6c 6f72 5f64 6172 6b73 6c61  er_color_darksla
-00000e10: 7465 6772 6179 da20 636f 6c6f 725f 7069  tegray. color_pi
-00000e20: 636b 6572 5f63 6f6c 6f72 5f64 6172 6b74  cker_color_darkt
-00000e30: 7572 7175 6f69 7365 da1d 636f 6c6f 725f  urquoise..color_
+00000080: 6429 642a 642b 642c 6421 642d 642e 642f  d)d*d+d,d!d-d.d/
+00000090: 6430 6431 6432 6433 6434 6435 6436 6437  d0d1d2d3d4d5d6d7
+000000a0: 6438 6439 643a 643b 643c 643d 643e 643f  d8d9d:d;d<d=d>d?
+000000b0: 6440 6441 6442 6443 6444 6445 6446 6447  d@dAdBdCdDdEdFdG
+000000c0: 6448 6449 644a 644b 644c 644d 640a 644e  dHdIdJdKdLdMd.dN
+000000d0: 644f 6450 6451 6452 6453 6454 6455 6456  dOdPdQdRdSdTdUdV
+000000e0: 6457 6458 6459 645a 645b 645c 645d 645e  dWdXdYdZd[d\d]d^
+000000f0: 645f 6460 6461 6462 6463 6464 6465 6466  d_d`dadbdcdddedf
+00000100: 640b 6467 6468 6469 646a 646b 646c 646d  d.dgdhdidjdkdldm
+00000110: 646e 646f 6470 6471 6472 6473 6474 6475  dndodpdqdrdsdtdu
+00000120: 6476 6477 6478 6479 647a 647b 647c 6414  dvdwdxdydzd{d|d.
+00000130: 647d 647e 647f 6480 6481 6482 6483 6484  d}d~d.d.d.d.d.d.
+00000140: 6485 6486 6487 6488 6489 648a 9c8e 5a00  d.d.d.d.d.d...Z.
+00000150: 648b 5300 298c 7509 0000 0052 656e 6b20  d.S.).u....Renk 
+00000160: 5365 c3a7 5a05 5369 7961 6875 0800 0000  Se..Z.Siyahu....
+00000170: 47c3 bc6d c3bc c59f 5a03 4772 695a 0542  G..m....Z.GriZ.B
+00000180: 6579 617a 5a05 426f 7264 6f75 0a00 0000  eyazZ.Bordou....
+00000190: 4bc4 b172 6dc4 b17a c4b1 5a03 4d6f 7275  K..rm..z..Z.Moru
+000001a0: 0600 0000 4675 c59f 7961 7506 0000 0059  ....Fu..yau....Y
+000001b0: 65c5 9f69 6c75 0d00 0000 41c3 a7c4 b16b  e..ilu....A....k
+000001c0: 2059 65c5 9f69 6c75 0e00 0000 5a65 7974   Ye..ilu....Zeyt
+000001d0: 696e 2059 65c5 9f69 6c69 7505 0000 0053  in Ye..iliu....S
+000001e0: 6172 c4b1 5a08 4c61 6369 7665 7274 5a04  ar..Z.LacivertZ.
+000001f0: 4d61 7669 da04 5465 616c 7a09 5375 204d  Mavi..Tealz.Su M
+00000200: 6176 6973 697a 0c41 6c69 6365 204d 6176  avisiz.Alice Mav
+00000210: 6973 697a 0b41 6e74 696b 2042 6579 617a  isiz.Antik Beyaz
+00000220: 5a09 416b 7561 6d61 7269 6e75 1100 0000  Z.Akuamarinu....
+00000230: 47c3 b66b 79c3 bc7a c3bc 204d 6176 6973  G..ky..z.. Mavis
+00000240: 695a 0342 656a 7508 0000 0042 6973 6bc3  iZ.Beju....Bisk.
+00000250: bc76 6975 1b00 0000 4265 7961 7a6c 61c5  .viu....Beyazla.
+00000260: 9f74 c4b1 72c4 b16c 6dc4 b1c5 9f20 4261  .t..r..lm.... Ba
+00000270: 6465 6d75 0d00 0000 4d61 7669 204d 656e  demu....Mavi Men
+00000280: 656b c59f 655a 0a4b 6168 7665 7265 6e67  ek..eZ.Kahvereng
+00000290: 6975 0e00 0000 4b6f 7975 204b 6176 756e  iu....Koyu Kavun
+000002a0: 69c3 a769 7a0b 4173 6b65 7269 204d 6176  i..iz.Askeri Mav
+000002b0: 6975 1300 0000 5061 726c 616b 2053 6172  iu....Parlak Sar
+000002c0: c4b1 2059 65c5 9f69 6c75 0900 0000 c387  .. Ye..ilu......
+000002d0: 696b 6f6c 6174 615a 064d 6572 6361 6e75  ikolataZ.Mercanu
+000002e0: 1800 0000 4dc4 b173 c4b1 7220 c387 69c3  ....M..s..r ..i.
+000002f0: a765 c49f 6920 4d61 7669 7369 750f 0000  .e..i Mavisiu...
+00000300: 004d c4b1 73c4 b172 20c4 b070 65c4 9f69  .M..s..r ..pe..i
+00000310: 750f 0000 004b 6f79 7520 4bc4 b172 6dc4  u....Koyu K..rm.
+00000320: b17a c4b1 750c 0000 0043 616d 2047 c3b6  .z..u....Cam G..
+00000330: 6265 c49f 697a 094b 6f79 7520 4d61 7669  be..iz.Koyu Mavi
+00000340: 7510 0000 004b 6f79 7520 4361 6d67 c3b6  u....Koyu Camg..
+00000350: 6265 c49f 6975 1100 0000 4b6f 7975 2041  be..iu....Koyu A
+00000360: 6c74 c4b1 6e20 5265 6e67 697a 084b 6f79  lt..n Rengiz.Koy
+00000370: 7520 4772 6975 0b00 0000 4b6f 7975 2059  u Griu....Koyu Y
+00000380: 65c5 9f69 6c7a 094b 6f79 7520 4861 6b69  e..ilz.Koyu Haki
+00000390: 7a0c 4b6f 7975 204d 6167 656e 7461 7513  z.Koyu Magentau.
+000003a0: 0000 004b 6f79 7520 5a65 7974 696e 2059  ...Koyu Zeytin Y
+000003b0: 65c5 9f69 6c69 7a0c 4b6f 7975 2054 7572  e..iliz.Koyu Tur
+000003c0: 756e 6375 7a0b 4b6f 7975 204f 726b 6964  uncuz.Koyu Orkid
+000003d0: 657a 0a4b 6f79 7520 536f 6d6f 6e75 1200  ez.Koyu Somonu..
+000003e0: 0000 4b6f 7975 2044 656e 697a 2059 65c5  ..Koyu Deniz Ye.
+000003f0: 9f69 6c69 7a13 4b6f 7975 2041 7264 7576  .iliz.Koyu Arduv
+00000400: 617a 204d 6176 6973 697a 104b 6f79 7520  az Mavisiz.Koyu 
+00000410: 4172 6475 7661 7a20 4772 697a 0c4b 6f79  Arduvaz Griz.Koy
+00000420: 7520 5475 726b 7561 7a75 0d00 0000 4b6f  u Turkuazu....Ko
+00000430: 7975 204d 656e 656b c59f 657a 0b44 6572  yu Menek..ez.Der
+00000440: 696e 2050 656d 6265 7517 0000 0044 6572  in Pembeu....Der
+00000450: 696e 2047 c3b6 6b79 c3bc 7ac3 bc20 4d61  in G..ky..z.. Ma
+00000460: 7669 7369 7a09 5369 736c 6920 4772 697a  visiz.Sisli Griz
+00000470: 0d44 6f64 6765 7220 4d61 7669 7369 750f  .Dodger Mavisiu.
+00000480: 0000 0041 7465 c59f 2054 75c4 9f6c 6173  ...Ate.. Tu..las
+00000490: c4b1 750f 0000 00c3 8769 c3a7 656b 2042  ..u......i..ek B
+000004a0: 6579 617a c4b1 750d 0000 004f 726d 616e  eyaz..u....Orman
+000004b0: 2059 65c5 9f69 6c69 da09 4761 696e 7362   Ye..ili..Gainsb
+000004c0: 6f72 6f75 0f00 0000 4861 7961 6c65 7420  orou....Hayalet 
+000004d0: 4265 7961 7ac4 b175 0600 0000 416c 74c4  Beyaz..u....Alt.
+000004e0: b16e 750c 0000 0041 6c74 c4b1 6e20 5265  .nu....Alt..n Re
+000004f0: 6e67 6975 0c00 0000 5965 c59f 696c 2053  ngiu....Ye..il S
+00000500: 6172 c4b1 7a09 4261 6c20 5265 6e67 6975  ar..z.Bal Rengiu
+00000510: 0c00 0000 4361 6e6c c4b1 2050 656d 6265  ....Canl.. Pembe
+00000520: 7517 0000 0048 696e 6469 7374 616e 204b  u....Hindistan K
+00000530: c4b1 726d c4b1 7ac4 b173 c4b1 7506 0000  ..rm..z..s..u...
+00000540: 00c3 8769 7669 7475 0800 0000 4669 6c64  ...ivitu....Fild
+00000550: 69c5 9f69 5a04 4861 6b69 5a07 4c61 7661  i..iZ.HakiZ.Lava
+00000560: 6e74 617a 0f4c 6176 616e 7461 2050 656d  ntaz.Lavanta Pem
+00000570: 6265 7369 750c 0000 00c3 8769 6d20 5965  besiu......im Ye
+00000580: c59f 696c 6975 0c00 0000 4c69 6d6f 6e20  ..iliu....Limon 
+00000590: c59e 6966 6f6e 750b 0000 0041 c3a7 c4b1  ..ifonu....A....
+000005a0: 6b20 4d61 7669 750d 0000 0041 c3a7 c4b1  k Maviu....A....
+000005b0: 6b20 4d65 7263 616e 7512 0000 0041 c3a7  k Mercanu....A..
+000005c0: c4b1 6b20 4361 6d67 c3b6 6265 c49f 6975  ..k Camg..be..iu
+000005d0: 1600 0000 41c3 a7c4 b16b 2041 6c74 c4b1  ....A....k Alt..
+000005e0: 6e20 5361 72c4 b173 c4b1 750a 0000 0041  n Sar..s..u....A
+000005f0: c3a7 c4b1 6b20 4772 6975 0c00 0000 41c3  ....k Griu....A.
+00000600: a7c4 b16b 2050 656d 6265 750c 0000 0041  ...k Pembeu....A
+00000610: c3a7 c4b1 6b20 536f 6d6f 6e75 1400 0000  ....k Somonu....
+00000620: 41c3 a7c4 b16b 2044 656e 697a 2059 65c5  A....k Deniz Ye.
+00000630: 9f69 6c69 7518 0000 0041 c3a7 c4b1 6b20  .iliu....A....k 
+00000640: 47c3 b66b 79c3 bc7a c3bc 204d 6176 6973  G..ky..z.. Mavis
+00000650: 6975 1200 0000 41c3 a7c4 b16b 2041 7264  iu....A....k Ard
+00000660: 7576 617a 2047 7269 7514 0000 0041 c3a7  uvaz Griu....A..
+00000670: c4b1 6b20 c387 656c 696b 204d 6176 6973  ..k ..elik Mavis
+00000680: 6975 0c00 0000 41c3 a7c4 b16b 2053 6172  iu....A....k Sar
+00000690: c4b1 750d 0000 004c 696d 6f6e 2059 65c5  ..u....Limon Ye.
+000006a0: 9f69 6c69 5a05 4b65 7465 6e5a 074d 6163  .iliZ.KetenZ.Mac
+000006b0: 656e 7461 7a0e 4f72 7461 2041 6b75 616d  entaz.Orta Akuam
+000006c0: 6172 696e 7a09 4f72 7461 204d 6176 697a  arinz.Orta Maviz
+000006d0: 0b4f 7274 6120 4f72 6b69 6465 7a08 4f72  .Orta Orkidez.Or
+000006e0: 7461 204d 6f72 7512 0000 004f 7274 6120  ta Moru....Orta 
+000006f0: 4465 6e69 7a20 5965 c59f 696c 697a 134f  Deniz Ye..iliz.O
+00000700: 7274 6120 4172 6475 7661 7a20 4d61 7669  rta Arduvaz Mavi
+00000710: 7369 7516 0000 004f 7274 6120 c4b0 6c6b  siu....Orta ..lk
+00000720: 6261 6861 7220 5965 c59f 696c 697a 0c4f  bahar Ye..iliz.O
+00000730: 7274 6120 5475 726b 7561 7a75 1b00 0000  rta Turkuazu....
+00000740: 4f72 7461 204d 656e 656b c59f 6520 4bc4  Orta Menek..e K.
+00000750: b172 6dc4 b17a c4b1 73c4 b17a 0b47 6563  .rm..z..s..z.Gec
+00000760: 6520 4d61 7669 7369 750d 0000 004e 616e  e Mavisiu....Nan
+00000770: 6520 4b72 656d 6173 c4b1 750a 0000 0053  e Kremas..u....S
+00000780: 6973 6c69 2047 c3bc 6c5a 074d 6f6b 6173  isli G..lZ.Mokas
+00000790: 656e 750e 0000 004e 6176 616a 6f20 4265  enu....Navajo Be
+000007a0: 7961 7ac4 b17a 0b45 736b 6920 4461 6e74  yaz..z.Eski Dant
+000007b0: 656c 5a07 5475 7275 6e63 7575 1200 0000  elZ.Turuncuu....
+000007c0: 5475 7275 6e63 7520 4bc4 b172 6dc4 b17a  Turuncu K..rm..z
+000007d0: c4b1 5a06 4f72 6b69 6465 7512 0000 0053  ..Z.Orkideu....S
+000007e0: 6f6c 756b 2041 6c74 c4b1 6e20 5265 6e67  oluk Alt..n Reng
+000007f0: 6975 0c00 0000 536f 6c75 6b20 5965 c59f  iu....Soluk Ye..
+00000800: 696c 7a0d 536f 6c75 6b20 5475 726b 7561  ilz.Soluk Turkua
+00000810: 7a75 1c00 0000 536f 6c75 6b20 4d65 6e65  zu....Soluk Mene
+00000820: 6bc5 9f65 204b c4b1 726d c4b1 7ac4 b173  k..e K..rm..z..s
+00000830: c4b1 750f 0000 0050 6170 6179 6120 4b72  ..u....Papaya Kr
+00000840: 656d 6173 c4b1 750c 0000 00c5 9e65 6674  emas..u......eft
+00000850: 616c 6920 5075 66da 0450 6572 755a 0550  ali Puf..PeruZ.P
+00000860: 656d 6265 5a04 4572 696b 7a08 546f 7a20  embeZ.Erikz.Toz 
+00000870: 4d61 7669 7a0c 5265 6265 6363 6120 4d6f  Maviz.Rebecca Mo
+00000880: 7275 750f 0000 0047 c3bc 6c20 4b61 6876  ruu....G..l Kahv
+00000890: 6572 656e 6769 7a0f 4b72 616c 6979 6574  erengiz.Kraliyet
+000008a0: 204d 6176 6973 697a 0f45 7965 7220 4b61   Mavisiz.Eyer Ka
+000008b0: 6876 6572 656e 6769 5a05 536f 6d6f 6e7a  hverengiZ.Somonz
+000008c0: 0e4b 756d 204b 6168 7665 7265 6e67 6975  .Kum Kahverengiu
+000008d0: 0d00 0000 4465 6e69 7a20 5965 c59f 696c  ....Deniz Ye..il
+000008e0: 6975 0d00 0000 4465 6e69 7a20 4b61 6275  iu....Deniz Kabu
+000008f0: c49f 755a 0753 6979 656e 6e61 7a0e 4172  ..uZ.Siyennaz.Ar
+00000900: 6475 7661 7a20 4d61 7669 7369 7a0b 4172  duvaz Mavisiz.Ar
+00000910: 6475 7661 7a20 4772 695a 034b 6172 750d  duvaz GriZ.Karu.
+00000920: 0000 0042 6168 6172 2059 65c5 9f69 6c69  ...Bahar Ye..ili
+00000930: 750d 0000 00c3 8765 6c69 6b20 4d61 7669  u......elik Mavi
+00000940: 7369 5a05 4272 6f6e 7a5a 0a44 6576 6564  siZ.BronzZ.Deved
+00000950: 696b 656e 695a 0744 6f6d 6174 6573 5a07  ikeniZ.DomatesZ.
+00000960: 5475 726b 7561 7a75 0800 0000 4d65 6e65  Turkuazu....Mene
+00000970: 6bc5 9f65 7507 0000 0042 75c4 9f64 6179  k..eu....Bu..day
+00000980: 7a0b 4265 7961 7a20 4475 6d61 6e75 0c00  z.Beyaz Dumanu..
+00000990: 0000 5361 72c4 b120 5965 c59f 696c 298e  ..Sar.. Ye..il).
+000009a0: da12 636f 6c6f 725f 7069 636b 6572 5f74  ..color_picker_t
+000009b0: 6974 6c65 da18 636f 6c6f 725f 7069 636b  itle..color_pick
+000009c0: 6572 5f63 6f6c 6f72 5f62 6c61 636b da19  er_color_black..
+000009d0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+000009e0: 6f72 5f73 696c 7665 72da 1763 6f6c 6f72  or_silver..color
+000009f0: 5f70 6963 6b65 725f 636f 6c6f 725f 6772  _picker_color_gr
+00000a00: 6179 da18 636f 6c6f 725f 7069 636b 6572  ay..color_picker
+00000a10: 5f63 6f6c 6f72 5f77 6869 7465 da19 636f  _color_white..co
+00000a20: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
+00000a30: 5f6d 6172 6f6f 6eda 1663 6f6c 6f72 5f70  _maroon..color_p
+00000a40: 6963 6b65 725f 636f 6c6f 725f 7265 64da  icker_color_red.
+00000a50: 1963 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
+00000a60: 6c6f 725f 7075 7270 6c65 da1a 636f 6c6f  lor_purple..colo
+00000a70: 725f 7069 636b 6572 5f63 6f6c 6f72 5f66  r_picker_color_f
+00000a80: 7563 6873 6961 da18 636f 6c6f 725f 7069  uchsia..color_pi
+00000a90: 636b 6572 5f63 6f6c 6f72 5f67 7265 656e  cker_color_green
+00000aa0: da17 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000ab0: 6f6c 6f72 5f6c 696d 65da 1863 6f6c 6f72  olor_lime..color
+00000ac0: 5f70 6963 6b65 725f 636f 6c6f 725f 6f6c  _picker_color_ol
+00000ad0: 6976 65da 1963 6f6c 6f72 5f70 6963 6b65  ive..color_picke
+00000ae0: 725f 636f 6c6f 725f 7965 6c6c 6f77 da17  r_color_yellow..
+00000af0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00000b00: 6f72 5f6e 6176 79da 1763 6f6c 6f72 5f70  or_navy..color_p
+00000b10: 6963 6b65 725f 636f 6c6f 725f 626c 7565  icker_color_blue
+00000b20: da17 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000b30: 6f6c 6f72 5f74 6561 6cda 1763 6f6c 6f72  olor_teal..color
+00000b40: 5f70 6963 6b65 725f 636f 6c6f 725f 6171  _picker_color_aq
+00000b50: 7561 da1c 636f 6c6f 725f 7069 636b 6572  ua..color_picker
+00000b60: 5f63 6f6c 6f72 5f61 6c69 6365 626c 7565  _color_aliceblue
+00000b70: da1f 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000b80: 6f6c 6f72 5f61 6e74 6971 7565 7768 6974  olor_antiquewhit
+00000b90: 65da 1d63 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
+00000ba0: 636f 6c6f 725f 6171 7561 6d61 7269 6e65  color_aquamarine
+00000bb0: da18 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000bc0: 6f6c 6f72 5f61 7a75 7265 da18 636f 6c6f  olor_azure..colo
+00000bd0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f62  r_picker_color_b
+00000be0: 6569 6765 da19 636f 6c6f 725f 7069 636b  eige..color_pick
+00000bf0: 6572 5f63 6f6c 6f72 5f62 6973 7175 65da  er_color_bisque.
+00000c00: 2163 6f6c 6f72 5f70 6963 6b65 725f 636f  !color_picker_co
+00000c10: 6c6f 725f 626c 616e 6368 6564 616c 6d6f  lor_blanchedalmo
+00000c20: 6e64 da1d 636f 6c6f 725f 7069 636b 6572  nd..color_picker
+00000c30: 5f63 6f6c 6f72 5f62 6c75 6576 696f 6c65  _color_blueviole
+00000c40: 74da 1863 6f6c 6f72 5f70 6963 6b65 725f  t..color_picker_
+00000c50: 636f 6c6f 725f 6272 6f77 6eda 1c63 6f6c  color_brown..col
+00000c60: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+00000c70: 6275 726c 7977 6f6f 64da 1c63 6f6c 6f72  burlywood..color
+00000c80: 5f70 6963 6b65 725f 636f 6c6f 725f 6361  _picker_color_ca
+00000c90: 6465 7462 6c75 65da 1d63 6f6c 6f72 5f70  detblue..color_p
+00000ca0: 6963 6b65 725f 636f 6c6f 725f 6368 6172  icker_color_char
+00000cb0: 7472 6575 7365 da1c 636f 6c6f 725f 7069  treuse..color_pi
+00000cc0: 636b 6572 5f63 6f6c 6f72 5f63 686f 636f  cker_color_choco
+00000cd0: 6c61 7465 da18 636f 6c6f 725f 7069 636b  late..color_pick
+00000ce0: 6572 5f63 6f6c 6f72 5f63 6f72 616c da21  er_color_coral.!
+00000cf0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00000d00: 6f72 5f63 6f72 6e66 6c6f 7765 7262 6c75  or_cornflowerblu
+00000d10: 65da 1b63 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
+00000d20: 636f 6c6f 725f 636f 726e 7369 6c6b da1a  color_cornsilk..
+00000d30: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00000d40: 6f72 5f63 7269 6d73 6f6e da17 636f 6c6f  or_crimson..colo
+00000d50: 725f 7069 636b 6572 5f63 6f6c 6f72 5f63  r_picker_color_c
+00000d60: 7961 6eda 1b63 6f6c 6f72 5f70 6963 6b65  yan..color_picke
+00000d70: 725f 636f 6c6f 725f 6461 726b 626c 7565  r_color_darkblue
+00000d80: da1b 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000d90: 6f6c 6f72 5f64 6172 6b63 7961 6eda 2063  olor_darkcyan. c
+00000da0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
+00000db0: 725f 6461 726b 676f 6c64 656e 726f 64da  r_darkgoldenrod.
+00000dc0: 1b63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
+00000dd0: 6c6f 725f 6461 726b 6772 6179 da1c 636f  lor_darkgray..co
+00000de0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
+00000df0: 5f64 6172 6b67 7265 656e da1c 636f 6c6f  _darkgreen..colo
+00000e00: 725f 7069 636b 6572 5f63 6f6c 6f72 5f64  r_picker_color_d
+00000e10: 6172 6b6b 6861 6b69 da1e 636f 6c6f 725f  arkkhaki..color_
+00000e20: 7069 636b 6572 5f63 6f6c 6f72 5f64 6172  picker_color_dar
+00000e30: 6b6d 6167 656e 7461 da21 636f 6c6f 725f  kmagenta.!color_
 00000e40: 7069 636b 6572 5f63 6f6c 6f72 5f64 6172  picker_color_dar
-00000e50: 6b76 696f 6c65 74da 1b63 6f6c 6f72 5f70  kviolet..color_p
-00000e60: 6963 6b65 725f 636f 6c6f 725f 6465 6570  icker_color_deep
-00000e70: 7069 6e6b da1e 636f 6c6f 725f 7069 636b  pink..color_pick
-00000e80: 6572 5f63 6f6c 6f72 5f64 6565 7073 6b79  er_color_deepsky
-00000e90: 626c 7565 da1a 636f 6c6f 725f 7069 636b  blue..color_pick
-00000ea0: 6572 5f63 6f6c 6f72 5f64 696d 6772 6179  er_color_dimgray
-00000eb0: da1d 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
-00000ec0: 6f6c 6f72 5f64 6f64 6765 7262 6c75 65da  olor_dodgerblue.
-00000ed0: 1c63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00000ee0: 6c6f 725f 6669 7265 6272 6963 6bda 1e63  lor_firebrick..c
-00000ef0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000f00: 725f 666c 6f72 616c 7768 6974 65da 1e63  r_floralwhite..c
-00000f10: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000f20: 725f 666f 7265 7374 6772 6565 6eda 1c63  r_forestgreen..c
-00000f30: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000f40: 725f 6761 696e 7362 6f72 6fda 1d63 6f6c  r_gainsboro..col
-00000f50: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00000f60: 6768 6f73 7477 6869 7465 da17 636f 6c6f  ghostwhite..colo
-00000f70: 725f 7069 636b 6572 5f63 6f6c 6f72 5f67  r_picker_color_g
-00000f80: 6f6c 64da 1c63 6f6c 6f72 5f70 6963 6b65  old..color_picke
-00000f90: 725f 636f 6c6f 725f 676f 6c64 656e 726f  r_color_goldenro
-00000fa0: 64da 1e63 6f6c 6f72 5f70 6963 6b65 725f  d..color_picker_
-00000fb0: 636f 6c6f 725f 6772 6565 6e79 656c 6c6f  color_greenyello
-00000fc0: 77da 1b63 6f6c 6f72 5f70 6963 6b65 725f  w..color_picker_
-00000fd0: 636f 6c6f 725f 686f 6e65 7964 6577 da1a  color_honeydew..
-00000fe0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000ff0: 6f72 5f68 6f74 7069 6e6b da1c 636f 6c6f  or_hotpink..colo
-00001000: 725f 7069 636b 6572 5f63 6f6c 6f72 5f69  r_picker_color_i
-00001010: 6e64 6961 6e72 6564 da19 636f 6c6f 725f  ndianred..color_
-00001020: 7069 636b 6572 5f63 6f6c 6f72 5f69 6e64  picker_color_ind
-00001030: 6967 6fda 1863 6f6c 6f72 5f70 6963 6b65  igo..color_picke
-00001040: 725f 636f 6c6f 725f 6976 6f72 79da 1863  r_color_ivory..c
-00001050: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001060: 725f 6b68 616b 69da 1b63 6f6c 6f72 5f70  r_khaki..color_p
-00001070: 6963 6b65 725f 636f 6c6f 725f 6c61 7665  icker_color_lave
-00001080: 6e64 6572 da20 636f 6c6f 725f 7069 636b  nder. color_pick
-00001090: 6572 5f63 6f6c 6f72 5f6c 6176 656e 6465  er_color_lavende
-000010a0: 7262 6c75 7368 da1c 636f 6c6f 725f 7069  rblush..color_pi
-000010b0: 636b 6572 5f63 6f6c 6f72 5f6c 6177 6e67  cker_color_lawng
-000010c0: 7265 656e da1f 636f 6c6f 725f 7069 636b  reen..color_pick
-000010d0: 6572 5f63 6f6c 6f72 5f6c 656d 6f6e 6368  er_color_lemonch
-000010e0: 6966 666f 6eda 1c63 6f6c 6f72 5f70 6963  iffon..color_pic
-000010f0: 6b65 725f 636f 6c6f 725f 6c69 6768 7462  ker_color_lightb
-00001100: 6c75 65da 1d63 6f6c 6f72 5f70 6963 6b65  lue..color_picke
-00001110: 725f 636f 6c6f 725f 6c69 6768 7463 6f72  r_color_lightcor
-00001120: 616c da1c 636f 6c6f 725f 7069 636b 6572  al..color_picker
-00001130: 5f63 6f6c 6f72 5f6c 6967 6874 6379 616e  _color_lightcyan
-00001140: da27 636f 6c6f 725f 7069 636b 6572 5f63  .'color_picker_c
-00001150: 6f6c 6f72 5f6c 6967 6874 676f 6c64 656e  olor_lightgolden
-00001160: 726f 6479 656c 6c6f 77da 1c63 6f6c 6f72  rodyellow..color
-00001170: 5f70 6963 6b65 725f 636f 6c6f 725f 6c69  _picker_color_li
-00001180: 6768 7467 7261 79da 1d63 6f6c 6f72 5f70  ghtgray..color_p
-00001190: 6963 6b65 725f 636f 6c6f 725f 6c69 6768  icker_color_ligh
-000011a0: 7467 7265 656e da1c 636f 6c6f 725f 7069  tgreen..color_pi
-000011b0: 636b 6572 5f63 6f6c 6f72 5f6c 6967 6874  cker_color_light
-000011c0: 7069 6e6b da1e 636f 6c6f 725f 7069 636b  pink..color_pick
-000011d0: 6572 5f63 6f6c 6f72 5f6c 6967 6874 7361  er_color_lightsa
-000011e0: 6c6d 6f6e da20 636f 6c6f 725f 7069 636b  lmon. color_pick
-000011f0: 6572 5f63 6f6c 6f72 5f6c 6967 6874 7365  er_color_lightse
-00001200: 6167 7265 656e da1f 636f 6c6f 725f 7069  agreen..color_pi
-00001210: 636b 6572 5f63 6f6c 6f72 5f6c 6967 6874  cker_color_light
-00001220: 736b 7962 6c75 65da 2163 6f6c 6f72 5f70  skyblue.!color_p
-00001230: 6963 6b65 725f 636f 6c6f 725f 6c69 6768  icker_color_ligh
-00001240: 7473 6c61 7465 6772 6179 da21 636f 6c6f  tslategray.!colo
-00001250: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
-00001260: 6967 6874 7374 6565 6c62 6c75 65da 1e63  ightsteelblue..c
-00001270: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001280: 725f 6c69 6768 7479 656c 6c6f 77da 1c63  r_lightyellow..c
-00001290: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-000012a0: 725f 6c69 6d65 6772 6565 6eda 1863 6f6c  r_limegreen..col
-000012b0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-000012c0: 6c69 6e65 6eda 1a63 6f6c 6f72 5f70 6963  linen..color_pic
-000012d0: 6b65 725f 636f 6c6f 725f 6d61 6765 6e74  ker_color_magent
-000012e0: 61da 2363 6f6c 6f72 5f70 6963 6b65 725f  a.#color_picker_
-000012f0: 636f 6c6f 725f 6d65 6469 756d 6171 7561  color_mediumaqua
-00001300: 6d61 7269 6e65 da1d 636f 6c6f 725f 7069  marine..color_pi
-00001310: 636b 6572 5f63 6f6c 6f72 5f6d 6564 6975  cker_color_mediu
-00001320: 6d62 6c75 65da 1f63 6f6c 6f72 5f70 6963  mblue..color_pic
-00001330: 6b65 725f 636f 6c6f 725f 6d65 6469 756d  ker_color_medium
-00001340: 6f72 6368 6964 da1f 636f 6c6f 725f 7069  orchid..color_pi
-00001350: 636b 6572 5f63 6f6c 6f72 5f6d 6564 6975  cker_color_mediu
-00001360: 6d70 7572 706c 65da 2163 6f6c 6f72 5f70  mpurple.!color_p
-00001370: 6963 6b65 725f 636f 6c6f 725f 6d65 6469  icker_color_medi
-00001380: 756d 7365 6167 7265 656e da22 636f 6c6f  umseagreen."colo
-00001390: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6d  r_picker_color_m
-000013a0: 6564 6975 6d73 6c61 7465 626c 7565 da24  ediumslateblue.$
-000013b0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-000013c0: 6f72 5f6d 6564 6975 6d73 7072 696e 6767  or_mediumspringg
-000013d0: 7265 656e da22 636f 6c6f 725f 7069 636b  reen."color_pick
-000013e0: 6572 5f63 6f6c 6f72 5f6d 6564 6975 6d74  er_color_mediumt
-000013f0: 7572 7175 6f69 7365 da22 636f 6c6f 725f  urquoise."color_
-00001400: 7069 636b 6572 5f63 6f6c 6f72 5f6d 6564  picker_color_med
-00001410: 6975 6d76 696f 6c65 7472 6564 da1f 636f  iumvioletred..co
-00001420: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00001430: 5f6d 6964 6e69 6768 7462 6c75 65da 1c63  _midnightblue..c
-00001440: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001450: 725f 6d69 6e74 6372 6561 6dda 1c63 6f6c  r_mintcream..col
-00001460: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00001470: 6d69 7374 7972 6f73 65da 1b63 6f6c 6f72  mistyrose..color
-00001480: 5f70 6963 6b65 725f 636f 6c6f 725f 6d6f  _picker_color_mo
-00001490: 6363 6173 696e da1e 636f 6c6f 725f 7069  ccasin..color_pi
-000014a0: 636b 6572 5f63 6f6c 6f72 5f6e 6176 616a  cker_color_navaj
-000014b0: 6f77 6869 7465 da1a 636f 6c6f 725f 7069  owhite..color_pi
-000014c0: 636b 6572 5f63 6f6c 6f72 5f6f 6c64 6c61  cker_color_oldla
-000014d0: 6365 da1c 636f 6c6f 725f 7069 636b 6572  ce..color_picker
-000014e0: 5f63 6f6c 6f72 5f6f 6c69 7665 6472 6162  _color_olivedrab
-000014f0: da19 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
-00001500: 6f6c 6f72 5f6f 7261 6e67 65da 1c63 6f6c  olor_orange..col
-00001510: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00001520: 6f72 616e 6765 7265 64da 1963 6f6c 6f72  orangered..color
-00001530: 5f70 6963 6b65 725f 636f 6c6f 725f 6f72  _picker_color_or
-00001540: 6368 6964 da20 636f 6c6f 725f 7069 636b  chid. color_pick
-00001550: 6572 5f63 6f6c 6f72 5f70 616c 6567 6f6c  er_color_palegol
-00001560: 6465 6e72 6f64 da1c 636f 6c6f 725f 7069  denrod..color_pi
-00001570: 636b 6572 5f63 6f6c 6f72 5f70 616c 6567  cker_color_paleg
-00001580: 7265 656e da20 636f 6c6f 725f 7069 636b  reen. color_pick
-00001590: 6572 5f63 6f6c 6f72 5f70 616c 6574 7572  er_color_paletur
-000015a0: 7175 6f69 7365 da20 636f 6c6f 725f 7069  quoise. color_pi
-000015b0: 636b 6572 5f63 6f6c 6f72 5f70 616c 6576  cker_color_palev
-000015c0: 696f 6c65 7472 6564 da1d 636f 6c6f 725f  ioletred..color_
-000015d0: 7069 636b 6572 5f63 6f6c 6f72 5f70 6170  picker_color_pap
-000015e0: 6179 6177 6869 70da 1c63 6f6c 6f72 5f70  ayawhip..color_p
-000015f0: 6963 6b65 725f 636f 6c6f 725f 7065 6163  icker_color_peac
-00001600: 6870 7566 66da 1763 6f6c 6f72 5f70 6963  hpuff..color_pic
-00001610: 6b65 725f 636f 6c6f 725f 7065 7275 da17  ker_color_peru..
-00001620: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00001630: 6f72 5f70 696e 6bda 1763 6f6c 6f72 5f70  or_pink..color_p
-00001640: 6963 6b65 725f 636f 6c6f 725f 706c 756d  icker_color_plum
-00001650: da1d 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
-00001660: 6f6c 6f72 5f70 6f77 6465 7262 6c75 65da  olor_powderblue.
-00001670: 2063 6f6c 6f72 5f70 6963 6b65 725f 636f   color_picker_co
-00001680: 6c6f 725f 7265 6265 6363 6170 7572 706c  lor_rebeccapurpl
-00001690: 65da 1c63 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
-000016a0: 636f 6c6f 725f 726f 7379 6272 6f77 6eda  color_rosybrown.
-000016b0: 1c63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-000016c0: 6c6f 725f 726f 7961 6c62 6c75 65da 1e63  lor_royalblue..c
-000016d0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-000016e0: 725f 7361 6464 6c65 6272 6f77 6eda 1963  r_saddlebrown..c
-000016f0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001700: 725f 7361 6c6d 6f6e da1d 636f 6c6f 725f  r_salmon..color_
-00001710: 7069 636b 6572 5f63 6f6c 6f72 5f73 616e  picker_color_san
-00001720: 6479 6272 6f77 6eda 1b63 6f6c 6f72 5f70  dybrown..color_p
-00001730: 6963 6b65 725f 636f 6c6f 725f 7365 6167  icker_color_seag
-00001740: 7265 656e da1b 636f 6c6f 725f 7069 636b  reen..color_pick
-00001750: 6572 5f63 6f6c 6f72 5f73 6561 7368 656c  er_color_seashel
-00001760: 6cda 1963 6f6c 6f72 5f70 6963 6b65 725f  l..color_picker_
-00001770: 636f 6c6f 725f 7369 656e 6e61 da1a 636f  color_sienna..co
-00001780: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00001790: 5f73 6b79 626c 7565 da1c 636f 6c6f 725f  _skyblue..color_
-000017a0: 7069 636b 6572 5f63 6f6c 6f72 5f73 6c61  picker_color_sla
-000017b0: 7465 626c 7565 da1c 636f 6c6f 725f 7069  teblue..color_pi
-000017c0: 636b 6572 5f63 6f6c 6f72 5f73 6c61 7465  cker_color_slate
-000017d0: 6772 6179 da17 636f 6c6f 725f 7069 636b  gray..color_pick
-000017e0: 6572 5f63 6f6c 6f72 5f73 6e6f 77da 1e63  er_color_snow..c
-000017f0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001800: 725f 7370 7269 6e67 6772 6565 6eda 1c63  r_springgreen..c
-00001810: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001820: 725f 7374 6565 6c62 6c75 65da 1663 6f6c  r_steelblue..col
+00000e50: 6b6f 6c69 7665 6772 6565 6eda 1d63 6f6c  kolivegreen..col
+00000e60: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+00000e70: 6461 726b 6f72 616e 6765 da1d 636f 6c6f  darkorange..colo
+00000e80: 725f 7069 636b 6572 5f63 6f6c 6f72 5f64  r_picker_color_d
+00000e90: 6172 6b6f 7263 6869 64da 1a63 6f6c 6f72  arkorchid..color
+00000ea0: 5f70 6963 6b65 725f 636f 6c6f 725f 6461  _picker_color_da
+00000eb0: 726b 7265 64da 1d63 6f6c 6f72 5f70 6963  rkred..color_pic
+00000ec0: 6b65 725f 636f 6c6f 725f 6461 726b 7361  ker_color_darksa
+00000ed0: 6c6d 6f6e da1f 636f 6c6f 725f 7069 636b  lmon..color_pick
+00000ee0: 6572 5f63 6f6c 6f72 5f64 6172 6b73 6561  er_color_darksea
+00000ef0: 6772 6565 6eda 2063 6f6c 6f72 5f70 6963  green. color_pic
+00000f00: 6b65 725f 636f 6c6f 725f 6461 726b 736c  ker_color_darksl
+00000f10: 6174 6562 6c75 65da 2063 6f6c 6f72 5f70  ateblue. color_p
+00000f20: 6963 6b65 725f 636f 6c6f 725f 6461 726b  icker_color_dark
+00000f30: 736c 6174 6567 7261 79da 2063 6f6c 6f72  slategray. color
+00000f40: 5f70 6963 6b65 725f 636f 6c6f 725f 6461  _picker_color_da
+00000f50: 726b 7475 7271 756f 6973 65da 1d63 6f6c  rkturquoise..col
+00000f60: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+00000f70: 6461 726b 7669 6f6c 6574 da1b 636f 6c6f  darkviolet..colo
+00000f80: 725f 7069 636b 6572 5f63 6f6c 6f72 5f64  r_picker_color_d
+00000f90: 6565 7070 696e 6bda 1e63 6f6c 6f72 5f70  eeppink..color_p
+00000fa0: 6963 6b65 725f 636f 6c6f 725f 6465 6570  icker_color_deep
+00000fb0: 736b 7962 6c75 65da 1a63 6f6c 6f72 5f70  skyblue..color_p
+00000fc0: 6963 6b65 725f 636f 6c6f 725f 6469 6d67  icker_color_dimg
+00000fd0: 7261 79da 1d63 6f6c 6f72 5f70 6963 6b65  ray..color_picke
+00000fe0: 725f 636f 6c6f 725f 646f 6467 6572 626c  r_color_dodgerbl
+00000ff0: 7565 da1c 636f 6c6f 725f 7069 636b 6572  ue..color_picker
+00001000: 5f63 6f6c 6f72 5f66 6972 6562 7269 636b  _color_firebrick
+00001010: da1e 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001020: 6f6c 6f72 5f66 6c6f 7261 6c77 6869 7465  olor_floralwhite
+00001030: da1e 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001040: 6f6c 6f72 5f66 6f72 6573 7467 7265 656e  olor_forestgreen
+00001050: da1c 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001060: 6f6c 6f72 5f67 6169 6e73 626f 726f da1d  olor_gainsboro..
+00001070: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00001080: 6f72 5f67 686f 7374 7768 6974 65da 1763  or_ghostwhite..c
+00001090: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
+000010a0: 725f 676f 6c64 da1c 636f 6c6f 725f 7069  r_gold..color_pi
+000010b0: 636b 6572 5f63 6f6c 6f72 5f67 6f6c 6465  cker_color_golde
+000010c0: 6e72 6f64 da1e 636f 6c6f 725f 7069 636b  nrod..color_pick
+000010d0: 6572 5f63 6f6c 6f72 5f67 7265 656e 7965  er_color_greenye
+000010e0: 6c6c 6f77 da1b 636f 6c6f 725f 7069 636b  llow..color_pick
+000010f0: 6572 5f63 6f6c 6f72 5f68 6f6e 6579 6465  er_color_honeyde
+00001100: 77da 1a63 6f6c 6f72 5f70 6963 6b65 725f  w..color_picker_
+00001110: 636f 6c6f 725f 686f 7470 696e 6bda 1c63  color_hotpink..c
+00001120: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
+00001130: 725f 696e 6469 616e 7265 64da 1963 6f6c  r_indianred..col
+00001140: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+00001150: 696e 6469 676f da18 636f 6c6f 725f 7069  indigo..color_pi
+00001160: 636b 6572 5f63 6f6c 6f72 5f69 766f 7279  cker_color_ivory
+00001170: da18 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001180: 6f6c 6f72 5f6b 6861 6b69 da1b 636f 6c6f  olor_khaki..colo
+00001190: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
+000011a0: 6176 656e 6465 72da 2063 6f6c 6f72 5f70  avender. color_p
+000011b0: 6963 6b65 725f 636f 6c6f 725f 6c61 7665  icker_color_lave
+000011c0: 6e64 6572 626c 7573 68da 1c63 6f6c 6f72  nderblush..color
+000011d0: 5f70 6963 6b65 725f 636f 6c6f 725f 6c61  _picker_color_la
+000011e0: 776e 6772 6565 6eda 1f63 6f6c 6f72 5f70  wngreen..color_p
+000011f0: 6963 6b65 725f 636f 6c6f 725f 6c65 6d6f  icker_color_lemo
+00001200: 6e63 6869 6666 6f6e da1c 636f 6c6f 725f  nchiffon..color_
+00001210: 7069 636b 6572 5f63 6f6c 6f72 5f6c 6967  picker_color_lig
+00001220: 6874 626c 7565 da1d 636f 6c6f 725f 7069  htblue..color_pi
+00001230: 636b 6572 5f63 6f6c 6f72 5f6c 6967 6874  cker_color_light
+00001240: 636f 7261 6cda 1c63 6f6c 6f72 5f70 6963  coral..color_pic
+00001250: 6b65 725f 636f 6c6f 725f 6c69 6768 7463  ker_color_lightc
+00001260: 7961 6eda 2763 6f6c 6f72 5f70 6963 6b65  yan.'color_picke
+00001270: 725f 636f 6c6f 725f 6c69 6768 7467 6f6c  r_color_lightgol
+00001280: 6465 6e72 6f64 7965 6c6c 6f77 da1c 636f  denrodyellow..co
+00001290: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
+000012a0: 5f6c 6967 6874 6772 6179 da1d 636f 6c6f  _lightgray..colo
+000012b0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
+000012c0: 6967 6874 6772 6565 6eda 1c63 6f6c 6f72  ightgreen..color
+000012d0: 5f70 6963 6b65 725f 636f 6c6f 725f 6c69  _picker_color_li
+000012e0: 6768 7470 696e 6bda 1e63 6f6c 6f72 5f70  ghtpink..color_p
+000012f0: 6963 6b65 725f 636f 6c6f 725f 6c69 6768  icker_color_ligh
+00001300: 7473 616c 6d6f 6eda 2063 6f6c 6f72 5f70  tsalmon. color_p
+00001310: 6963 6b65 725f 636f 6c6f 725f 6c69 6768  icker_color_ligh
+00001320: 7473 6561 6772 6565 6eda 1f63 6f6c 6f72  tseagreen..color
+00001330: 5f70 6963 6b65 725f 636f 6c6f 725f 6c69  _picker_color_li
+00001340: 6768 7473 6b79 626c 7565 da21 636f 6c6f  ghtskyblue.!colo
+00001350: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
+00001360: 6967 6874 736c 6174 6567 7261 79da 2163  ightslategray.!c
+00001370: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
+00001380: 725f 6c69 6768 7473 7465 656c 626c 7565  r_lightsteelblue
+00001390: da1e 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+000013a0: 6f6c 6f72 5f6c 6967 6874 7965 6c6c 6f77  olor_lightyellow
+000013b0: da1c 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+000013c0: 6f6c 6f72 5f6c 696d 6567 7265 656e da18  olor_limegreen..
+000013d0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+000013e0: 6f72 5f6c 696e 656e da1a 636f 6c6f 725f  or_linen..color_
+000013f0: 7069 636b 6572 5f63 6f6c 6f72 5f6d 6167  picker_color_mag
+00001400: 656e 7461 da23 636f 6c6f 725f 7069 636b  enta.#color_pick
+00001410: 6572 5f63 6f6c 6f72 5f6d 6564 6975 6d61  er_color_mediuma
+00001420: 7175 616d 6172 696e 65da 1d63 6f6c 6f72  quamarine..color
+00001430: 5f70 6963 6b65 725f 636f 6c6f 725f 6d65  _picker_color_me
+00001440: 6469 756d 626c 7565 da1f 636f 6c6f 725f  diumblue..color_
+00001450: 7069 636b 6572 5f63 6f6c 6f72 5f6d 6564  picker_color_med
+00001460: 6975 6d6f 7263 6869 64da 1f63 6f6c 6f72  iumorchid..color
+00001470: 5f70 6963 6b65 725f 636f 6c6f 725f 6d65  _picker_color_me
+00001480: 6469 756d 7075 7270 6c65 da21 636f 6c6f  diumpurple.!colo
+00001490: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6d  r_picker_color_m
+000014a0: 6564 6975 6d73 6561 6772 6565 6eda 2263  ediumseagreen."c
+000014b0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
+000014c0: 725f 6d65 6469 756d 736c 6174 6562 6c75  r_mediumslateblu
+000014d0: 65da 2463 6f6c 6f72 5f70 6963 6b65 725f  e.$color_picker_
+000014e0: 636f 6c6f 725f 6d65 6469 756d 7370 7269  color_mediumspri
+000014f0: 6e67 6772 6565 6eda 2263 6f6c 6f72 5f70  nggreen."color_p
+00001500: 6963 6b65 725f 636f 6c6f 725f 6d65 6469  icker_color_medi
+00001510: 756d 7475 7271 756f 6973 65da 2263 6f6c  umturquoise."col
+00001520: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+00001530: 6d65 6469 756d 7669 6f6c 6574 7265 64da  mediumvioletred.
+00001540: 1f63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
+00001550: 6c6f 725f 6d69 646e 6967 6874 626c 7565  lor_midnightblue
+00001560: da1c 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001570: 6f6c 6f72 5f6d 696e 7463 7265 616d da1c  olor_mintcream..
+00001580: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00001590: 6f72 5f6d 6973 7479 726f 7365 da1b 636f  or_mistyrose..co
+000015a0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
+000015b0: 5f6d 6f63 6361 7369 6eda 1e63 6f6c 6f72  _moccasin..color
+000015c0: 5f70 6963 6b65 725f 636f 6c6f 725f 6e61  _picker_color_na
+000015d0: 7661 6a6f 7768 6974 65da 1a63 6f6c 6f72  vajowhite..color
+000015e0: 5f70 6963 6b65 725f 636f 6c6f 725f 6f6c  _picker_color_ol
+000015f0: 646c 6163 65da 1c63 6f6c 6f72 5f70 6963  dlace..color_pic
+00001600: 6b65 725f 636f 6c6f 725f 6f6c 6976 6564  ker_color_olived
+00001610: 7261 62da 1963 6f6c 6f72 5f70 6963 6b65  rab..color_picke
+00001620: 725f 636f 6c6f 725f 6f72 616e 6765 da1c  r_color_orange..
+00001630: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00001640: 6f72 5f6f 7261 6e67 6572 6564 da19 636f  or_orangered..co
+00001650: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
+00001660: 5f6f 7263 6869 64da 2063 6f6c 6f72 5f70  _orchid. color_p
+00001670: 6963 6b65 725f 636f 6c6f 725f 7061 6c65  icker_color_pale
+00001680: 676f 6c64 656e 726f 64da 1c63 6f6c 6f72  goldenrod..color
+00001690: 5f70 6963 6b65 725f 636f 6c6f 725f 7061  _picker_color_pa
+000016a0: 6c65 6772 6565 6eda 2063 6f6c 6f72 5f70  legreen. color_p
+000016b0: 6963 6b65 725f 636f 6c6f 725f 7061 6c65  icker_color_pale
+000016c0: 7475 7271 756f 6973 65da 2063 6f6c 6f72  turquoise. color
+000016d0: 5f70 6963 6b65 725f 636f 6c6f 725f 7061  _picker_color_pa
+000016e0: 6c65 7669 6f6c 6574 7265 64da 1d63 6f6c  levioletred..col
+000016f0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+00001700: 7061 7061 7961 7768 6970 da1c 636f 6c6f  papayawhip..colo
+00001710: 725f 7069 636b 6572 5f63 6f6c 6f72 5f70  r_picker_color_p
+00001720: 6561 6368 7075 6666 da17 636f 6c6f 725f  eachpuff..color_
+00001730: 7069 636b 6572 5f63 6f6c 6f72 5f70 6572  picker_color_per
+00001740: 75da 1763 6f6c 6f72 5f70 6963 6b65 725f  u..color_picker_
+00001750: 636f 6c6f 725f 7069 6e6b da17 636f 6c6f  color_pink..colo
+00001760: 725f 7069 636b 6572 5f63 6f6c 6f72 5f70  r_picker_color_p
+00001770: 6c75 6dda 1d63 6f6c 6f72 5f70 6963 6b65  lum..color_picke
+00001780: 725f 636f 6c6f 725f 706f 7764 6572 626c  r_color_powderbl
+00001790: 7565 da20 636f 6c6f 725f 7069 636b 6572  ue. color_picker
+000017a0: 5f63 6f6c 6f72 5f72 6562 6563 6361 7075  _color_rebeccapu
+000017b0: 7270 6c65 da1c 636f 6c6f 725f 7069 636b  rple..color_pick
+000017c0: 6572 5f63 6f6c 6f72 5f72 6f73 7962 726f  er_color_rosybro
+000017d0: 776e da1c 636f 6c6f 725f 7069 636b 6572  wn..color_picker
+000017e0: 5f63 6f6c 6f72 5f72 6f79 616c 626c 7565  _color_royalblue
+000017f0: da1e 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001800: 6f6c 6f72 5f73 6164 646c 6562 726f 776e  olor_saddlebrown
+00001810: da19 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001820: 6f6c 6f72 5f73 616c 6d6f 6eda 1d63 6f6c  olor_salmon..col
 00001830: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00001840: 7461 6eda 1a63 6f6c 6f72 5f70 6963 6b65  tan..color_picke
-00001850: 725f 636f 6c6f 725f 7468 6973 746c 65da  r_color_thistle.
-00001860: 1963 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00001870: 6c6f 725f 746f 6d61 746f da1c 636f 6c6f  lor_tomato..colo
-00001880: 725f 7069 636b 6572 5f63 6f6c 6f72 5f74  r_picker_color_t
-00001890: 7572 7175 6f69 7365 da19 636f 6c6f 725f  urquoise..color_
-000018a0: 7069 636b 6572 5f63 6f6c 6f72 5f76 696f  picker_color_vio
-000018b0: 6c65 74da 1863 6f6c 6f72 5f70 6963 6b65  let..color_picke
-000018c0: 725f 636f 6c6f 725f 7768 6561 74da 1d63  r_color_wheat..c
-000018d0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-000018e0: 725f 7768 6974 6573 6d6f 6b65 da1e 636f  r_whitesmoke..co
-000018f0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00001900: 5f79 656c 6c6f 7767 7265 656e 4e29 01da  _yellowgreenN)..
-00001910: 076c 6578 656d 6573 a900 729d 0000 0072  .lexemes..r....r
-00001920: 9d00 0000 fa53 2f55 7365 7273 2f76 6164  .....S/Users/vad
-00001930: 696b 7573 2f50 7963 6861 726d 5072 6f6a  ikus/PycharmProj
-00001940: 6563 7473 2f6e 6f74 6f6c 6f67 2d65 6469  ects/notolog-edi
-00001950: 746f 722f 6170 702f 6c65 7865 6d65 732f  tor/app/lexemes/
-00001960: 7365 2f63 6f6c 6f72 5f70 6963 6b65 725f  se/color_picker_
-00001970: 6469 616c 6f67 2e70 79da 083c 6d6f 6475  dialog.py..<modu
-00001980: 6c65 3e03 0000 0073 1e01 0000 0202 0201  le>....s........
-00001990: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000019a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000019b0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000019c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000019d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000019e0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000019f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a00: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a10: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a20: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a30: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a40: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a50: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a60: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a70: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a80: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001a90: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001aa0: 0201 0201 0201 0280 00f1                 ..........
+00001840: 7361 6e64 7962 726f 776e da1b 636f 6c6f  sandybrown..colo
+00001850: 725f 7069 636b 6572 5f63 6f6c 6f72 5f73  r_picker_color_s
+00001860: 6561 6772 6565 6eda 1b63 6f6c 6f72 5f70  eagreen..color_p
+00001870: 6963 6b65 725f 636f 6c6f 725f 7365 6173  icker_color_seas
+00001880: 6865 6c6c da19 636f 6c6f 725f 7069 636b  hell..color_pick
+00001890: 6572 5f63 6f6c 6f72 5f73 6965 6e6e 61da  er_color_sienna.
+000018a0: 1a63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
+000018b0: 6c6f 725f 736b 7962 6c75 65da 1c63 6f6c  lor_skyblue..col
+000018c0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+000018d0: 736c 6174 6562 6c75 65da 1c63 6f6c 6f72  slateblue..color
+000018e0: 5f70 6963 6b65 725f 636f 6c6f 725f 736c  _picker_color_sl
+000018f0: 6174 6567 7261 79da 1763 6f6c 6f72 5f70  ategray..color_p
+00001900: 6963 6b65 725f 636f 6c6f 725f 736e 6f77  icker_color_snow
+00001910: da1e 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001920: 6f6c 6f72 5f73 7072 696e 6767 7265 656e  olor_springgreen
+00001930: da1c 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001940: 6f6c 6f72 5f73 7465 656c 626c 7565 da16  olor_steelblue..
+00001950: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00001960: 6f72 5f74 616e da1a 636f 6c6f 725f 7069  or_tan..color_pi
+00001970: 636b 6572 5f63 6f6c 6f72 5f74 6869 7374  cker_color_thist
+00001980: 6c65 da19 636f 6c6f 725f 7069 636b 6572  le..color_picker
+00001990: 5f63 6f6c 6f72 5f74 6f6d 6174 6fda 1c63  _color_tomato..c
+000019a0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
+000019b0: 725f 7475 7271 756f 6973 65da 1963 6f6c  r_turquoise..col
+000019c0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
+000019d0: 7669 6f6c 6574 da18 636f 6c6f 725f 7069  violet..color_pi
+000019e0: 636b 6572 5f63 6f6c 6f72 5f77 6865 6174  cker_color_wheat
+000019f0: da1d 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001a00: 6f6c 6f72 5f77 6869 7465 736d 6f6b 65da  olor_whitesmoke.
+00001a10: 1e63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
+00001a20: 6c6f 725f 7965 6c6c 6f77 6772 6565 6e4e  lor_yellowgreenN
+00001a30: 2901 da07 6c65 7865 6d65 73a9 0072 9300  )...lexemes..r..
+00001a40: 0000 7293 0000 00fa 502f 5573 6572 732f  ..r.....P/Users/
+00001a50: 7661 6469 6b75 732f 5079 6368 6172 6d50  vadikus/PycharmP
+00001a60: 726f 6a65 6374 732f 6e6f 746f 6c6f 672d  rojects/notolog-
+00001a70: 6465 762f 6170 702f 6c65 7865 6d65 732f  dev/app/lexemes/
+00001a80: 7472 2f63 6f6c 6f72 5f70 6963 6b65 725f  tr/color_picker_
+00001a90: 6469 616c 6f67 2e70 79da 083c 6d6f 6475  dialog.py..<modu
+00001aa0: 6c65 3e03 0000 0073 1e01 0000 0202 0201  le>....s........
+00001ab0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001ac0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001ad0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001ae0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001af0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b00: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b10: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b20: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b30: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b40: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b50: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b60: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b70: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b80: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001b90: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001ba0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001bb0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001bc0: 0201 0201 0201 0280 00f1                 ..........
```

### Comparing `notolog-0.9.1b0/app/lexemes/se/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May  5 14:33:15 2024 UTC, .py size: 6246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,360 +1,359 @@
-00000000: 610d 0d0a 0000 0000 ab98 3766 6618 0000  a.........7ff...
+00000000: 610d 0d0a 0000 0000 42a9 3566 0318 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0055 0000 0040 0000 0073 b200 0000 6400  .U...@...s....d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6403 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
-00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
-00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
-00000070: 6420 6421 6422 641e 641f 6423 6424 6425  d d!d"d.d.d#d$d%
-00000080: 6426 6427 6428 6429 642a 642b 642c 642b  d&d'd(d)d*d+d,d+
-00000090: 642d 642e 6424 642e 6426 6429 642a 642f  d-d.d$d.d&d)d*d/
-000000a0: 6430 642a 6431 6432 6433 6434 6435 6436  d0d*d1d2d3d4d5d6
-000000b0: 6437 6438 6439 643a 643b 643c 643d 643e  d7d8d9d:d;d<d=d>
-000000c0: 643f 6440 6441 6442 6443 6444 6445 6446  d?d@dAdBdCdDdEdF
-000000d0: 6447 6448 6449 644a 9c54 5a00 644b 5300  dGdHdIdJ.TZ.dKS.
-000000e0: 294c 7a12 4e6f 746f 6c6f 6720 5265 6469  )Lz.Notolog Redi
-000000f0: 6765 7261 7265 7a19 7b61 7070 5f74 6974  gerarez.{app_tit
-00000100: 6c65 7d20 2d20 7b73 7562 5f74 6974 6c65  le} - {sub_title
-00000110: 7d75 1600 0000 4669 6c74 6572 66c3 a46c  }u....Filterf..l
-00000120: 7420 66c3 b672 2066 696c 6572 7a08 4279  t f..r filerz.By
-00000130: 7420 6e61 6d6e 5a06 5261 6465 7261 7a0b  t namnZ.Raderaz.
-00000140: 5261 6465 7261 2068 656c 7475 0b00 0000  Radera heltu....
-00000150: c385 7465 7273 74c3 a46c 6c75 1000 0000  ..terst..llu....
-00000160: 4279 7420 6e61 6d6e 2070 c3a5 2066 696c  Byt namn p.. fil
-00000170: 7a11 416e 6765 206e 7974 7420 6669 6c6e  z.Ange nytt filn
-00000180: 616d 6e7a 2145 6e20 6669 6c20 6d65 6420  amnz!En fil med 
-00000190: 7361 6d6d 6120 6e61 6d6e 2066 696e 6e73  samma namn finns
-000001a0: 2072 6564 616e 7a0a 5261 6465 7261 2066   redanz.Radera f
-000001b0: 696c 7a23 5669 6c6c 2064 7520 7261 6465  ilz#Vill du rade
-000001c0: 7261 2066 696c 656e 2022 7b66 696c 655f  ra filen "{file_
-000001d0: 6e61 6d65 7d22 3f7a 1152 6164 6572 6120  name}"?z.Radera 
-000001e0: 6669 6c65 6e20 6865 6c74 7a28 5669 6c6c  filen heltz(Vill
-000001f0: 2064 7520 7261 6465 7261 2066 696c 656e   du radera filen
-00000200: 2022 7b66 696c 655f 6e61 6d65 7d22 2068   "{file_name}" h
-00000210: 656c 743f 752a 0000 004b 616e 2069 6e74  elt?u*...Kan int
-00000220: 6520 7261 6465 7261 2066 696c 656e 2c20  e radera filen, 
-00000230: 6574 7420 6665 6c20 696e 7472 c3a4 6666  ett fel intr..ff
-00000240: 6164 657a 1346 696c 656e 2068 6974 7461  adez.Filen hitta
-00000250: 6465 7320 696e 7465 750f 0000 00c3 8574  des inteu......t
-00000260: 6572 7374 c3a4 6c6c 2066 696c 7520 0000  erst..ll filu ..
-00000270: 00c3 8574 6572 7374 c3a4 6c6c 2066 696c  ...terst..ll fil
-00000280: 656e 2022 7b66 696c 655f 6e61 6d65 7d22  en "{file_name}"
-00000290: 3f75 3000 0000 4b61 6e20 696e 7465 20c3  ?u0...Kan inte .
-000002a0: a574 6572 7374 c3a4 6c6c 6120 6669 6c65  .terst..lla file
-000002b0: 6e2c 2065 7474 2066 656c 2069 6e74 72c3  n, ett fel intr.
-000002c0: a466 6661 6465 7a29 456e 2066 696c 206d  .ffadez)En fil m
-000002d0: 6564 206e 616d 6e65 7420 7b66 696c 655f  ed namnet {file_
-000002e0: 6e61 6d65 7d20 6669 6e6e 7320 7265 6461  name} finns reda
-000002f0: 6e5a 0a4d 6564 6465 6c61 6e64 6575 0600  nZ.Meddelandeu..
-00000300: 0000 5374 c3a4 6e67 7a0d 4e79 7474 2064  ..St..ngz.Nytt d
-00000310: 6f6b 756d 656e 7475 0a00 0000 c396 7070  okumentu......pp
-00000320: 6e61 2066 696c 7a09 5370 6172 6120 6669  na filz.Spara fi
-00000330: 6c7a 0d53 7061 7261 2074 6f6d 2066 696c  lz.Spara tom fil
-00000340: 752b 0000 0054 696c 6cc3 a574 2061 7474  u+...Till..t att
-00000350: 2073 7061 7261 2066 696c 656e 206d 6564   spara filen med
-00000360: 2074 6f6d 7420 696e 6e65 68c3 a56c 6c3f   tomt inneh..ll?
-00000370: 7a0c 4b72 7970 7465 7261 2066 696c 7a1d  z.Kryptera filz.
-00000380: 4b72 7970 7465 7261 2066 696c 656e 2022  Kryptera filen "
-00000390: 7b66 696c 655f 6e61 6d65 7d22 3f75 1a00  {file_name}"?u..
-000003a0: 0000 4669 6c65 6e20 c3a4 7220 7265 6461  ..Filen ..r reda
-000003b0: 6e20 6b72 7970 7465 7261 6421 7519 0000  n krypterad!u...
-000003c0: 0053 6b72 6976 20c3 b676 6572 2062 6566  .Skriv ..ver bef
-000003d0: 696e 746c 6967 2066 696c 752f 0000 0053  intlig filu/...S
-000003e0: 6b72 6976 20c3 b676 6572 2064 656e 2062  kriv ..ver den b
-000003f0: 6566 696e 746c 6967 6120 6669 6c65 6e20  efintliga filen 
-00000400: 227b 6669 6c65 5f70 6174 687d 223f 7a0e  "{file_path}"?z.
-00000410: 4465 6b72 7970 7465 7261 2066 696c 7a1f  Dekryptera filz.
-00000420: 4465 6b72 7970 7465 7261 2066 696c 656e  Dekryptera filen
-00000430: 2022 7b66 696c 655f 6e61 6d65 7d22 3f75   "{file_name}"?u
-00000440: 1900 0000 4669 6c65 6e20 c3a4 7220 696e  ....Filen ..r in
-00000450: 7465 206b 7279 7074 6572 6164 2175 0e00  te krypterad!u..
-00000460: 0000 4e79 7474 206c c3b6 7365 6e6f 7264  ..Nytt l..senord
-00000470: 750a 0000 004c c3b6 7365 6e6f 7264 3a75  u....L..senord:u
-00000480: 1300 0000 416e 6765 206e 7974 7420 6cc3  ....Ange nytt l.
-00000490: b673 656e 6f72 6475 0900 0000 4c65 6474  .senordu....Ledt
-000004a0: 72c3 a564 3a75 c400 0000 4c65 6474 72c3  r..d:u....Ledtr.
-000004b0: a564 656e 20c3 a472 2069 6e74 6520 6b72  .den ..r inte kr
-000004c0: 7970 7465 7261 6420 6f63 6820 6b61 6e20  ypterad och kan 
-000004d0: 6cc3 a473 6173 2066 72c3 a56e 2066 696c  l..sas fr..n fil
-000004e0: 656e 210a 556e 6476 696b 2075 7070 656e  en!.Undvik uppen
-000004f0: 6261 7261 206c 6564 7472 c3a5 6461 7220  bara ledtr..dar 
-00000500: 736f 6d20 6b61 6e20 6769 7373 6173 206c  som kan gissas l
-00000510: c3a4 7474 2c20 73c3 a573 6f6d 2066 c3b6  ..tt, s..som f..
-00000520: 6465 6c73 6564 6174 756d 2e0a 46c3 b672  delsedatum..F..r
-00000530: 73c3 b66b 2061 6e76 c3a4 6e64 6120 656e  s..k anv..nda en
-00000540: 2072 6566 6572 656e 7320 736f 6d20 696e   referens som in
-00000550: 7465 206c c3a4 7474 206b 616e 206b 6f70  te l..tt kan kop
-00000560: 706c 6173 2074 696c 6c20 6469 672e 7518  plas till dig.u.
-00000570: 0000 0041 6e67 6520 6c65 6474 72c3 a564  ...Ange ledtr..d
-00000580: 2028 7661 6c66 7269 7474 295a 024f 4b5a   (valfritt)Z.OKZ
-00000590: 0641 7662 7279 745a 0756 6172 6e69 6e67  .AvbrytZ.Varning
-000005a0: 7526 0000 004c c3b6 7365 6e6f 7264 7366  u&...L..senordsf
-000005b0: c3a4 6c74 6574 2066 c3a5 7220 696e 7465  ..ltet f..r inte
-000005c0: 2076 6172 6120 746f 6d74 2175 3700 0000   vara tomt!u7...
-000005d0: 4c65 6474 72c3 a564 7366 c3a4 6c74 6574  Ledtr..dsf..ltet
-000005e0: 20c3 a472 2066 c3b6 7220 6cc3 a56e 6774   ..r f..r l..ngt
-000005f0: 2c20 6d61 7820 7b73 796d 626f 6c73 7d20  , max {symbols} 
-00000600: 7465 636b 656e 2175 0e00 0000 416e 6765  tecken!u....Ange
-00000610: 206c c3b6 7365 6e6f 7264 7520 0000 00c3   l..senordu ....
-00000620: 8574 6572 7374 c3a4 6c6c 206b 7279 7074  .terst..ll krypt
-00000630: 6572 696e 6773 6cc3 b673 656e 6f72 6475  eringsl..senordu
-00000640: 5000 0000 c384 7220 6475 2073 c3a4 6b65  P.....r du s..ke
-00000650: 7220 70c3 a520 6174 7420 6475 2076 696c  r p.. att du vil
-00000660: 6c20 c3a5 7465 7273 74c3 a46c 6c61 2064  l ..terst..lla d
-00000670: 6574 206e 7576 6172 616e 6465 206b 7279  et nuvarande kry
-00000680: 7074 6572 696e 6773 6cc3 b673 656e 6f72  pteringsl..senor
-00000690: 6465 743f 5a02 4a61 7505 0000 004c c3a4  det?Z.Jau....L..
-000006a0: 6e6b 7528 0000 00c3 9670 706e 6120 6cc3  nku(.....ppna l.
-000006b0: a46e 6b65 6e20 227b 7572 6c7d 2220 6920  .nken "{url}" i 
-000006c0: 656e 2077 6562 626c c3a4 7361 7265 3f75  en webbl..sare?u
-000006d0: 2500 0000 4b72 7970 7465 7269 6e67 736c  %...Krypteringsl
-000006e0: c3b6 7365 6e6f 7264 6574 2073 74c3 a46d  ..senordet st..m
-000006f0: 6d65 7220 696e 7465 2175 1900 0000 4665  mer inte!u....Fe
-00000700: 6c20 6b72 7970 7465 7269 6e67 736c c3b6  l krypteringsl..
-00000710: 7365 6e6f 7264 217a 1646 696c 656e 206b  senord!z.Filen k
-00000720: 616e 2069 6e74 6520 6c61 6464 6173 2e75  an inte laddas.u
-00000730: 2900 0000 4b61 6e20 696e 7465 2073 7061  )...Kan inte spa
-00000740: 7261 2066 696c 656e 2c20 6574 7420 6665  ra filen, ett fe
-00000750: 6c20 696e 7472 c3a4 6666 6164 657a 124d  l intr..ffadez.M
-00000760: 6572 2069 6e66 6f72 6d61 7469 6f6e 2e2e  er information..
-00000770: 2e7a 2a46 6f72 6d61 7465 7261 6420 7465  .z*Formaterad te
-00000780: 7874 2068 6172 206b 6f70 6965 7261 7473  xt har kopierats
-00000790: 2074 696c 6c20 7572 6b6c 6970 707a 0d4f   till urklippz.O
-000007a0: 6d20 7072 6f67 7261 6d6d 6574 7a13 4d61  m programmetz.Ma
-000007b0: 726b 646f 776e 2d72 6564 6967 6572 6172  rkdown-redigerar
-000007c0: 65da 0756 6572 7369 6f6e 5a06 4c69 6365  e..VersionZ.Lice
-000007d0: 6e73 5a09 5765 6262 706c 6174 73da 0647  nsZ.Webbplats..G
-000007e0: 6974 4875 62da 0450 7950 695a 0544 6174  itHub..PyPiZ.Dat
-000007f0: 756d 753a 0000 0045 6e20 6e79 2076 6572  umu:...En ny ver
-00000800: 7369 6f6e 2027 7b6c 6174 6573 745f 7665  sion '{latest_ve
-00000810: 7273 696f 6e7d 2720 6176 2061 7070 656e  rsion}' av appen
-00000820: 20c3 a472 2074 696c 6c67 c3a4 6e67 6c69   ..r tillg..ngli
-00000830: 6775 2e00 0000 4465 6e20 7365 6e61 7374  gu....Den senast
-00000840: 6520 7665 7273 696f 6e65 6e20 6176 2061  e versionen av a
-00000850: 7070 656e 20c3 a472 2069 6e73 7461 6c6c  ppen ..r install
-00000860: 6572 6164 7520 0000 004b 616e 2069 6e74  eradu ...Kan int
-00000870: 6520 68c3 a46d 7461 2073 7661 7273 696e  e h..mta svarsin
-00000880: 666f 726d 6174 696f 6e75 5300 0000 56c3  formationuS...V.
-00000890: a472 6465 6e20 6869 7474 6164 6573 2069  .rden hittades i
-000008a0: 6e74 652e 2044 6574 206b 616e 2076 6172  nte. Det kan var
-000008b0: 6120 6574 7420 7072 6f62 6c65 6d20 6d65  a ett problem me
-000008c0: 6420 696e 7465 726e 6574 616e 736c 7574  d internetanslut
-000008d0: 6e69 6e67 656e 2065 6c6c 6572 2044 4e53  ningen eller DNS
-000008e0: 2e75 5700 0000 416e 736c 7574 6e69 6e67  .uW...Anslutning
-000008f0: 656e 206e 656b 6164 6573 2e20 5365 7276  en nekades. Serv
-00000900: 6572 6e20 6b61 6e20 7661 7261 206e 6572  ern kan vara ner
-00000910: 652c 2065 6c6c 6572 2073 c3a5 206b 616e  e, eller s.. kan
-00000920: 2064 6574 2066 696e 6e61 7320 6ec3 a474   det finnas n..t
-00000930: 7665 726b 7370 726f 626c 656d 2e75 3e00  verksproblem.u>.
-00000940: 0000 416e 736c 7574 6e69 6e67 656e 206c  ..Anslutningen l
-00000950: c3b6 7074 6520 7574 2069 2074 6964 2e20  ..pte ut i tid. 
-00000960: 4465 7420 6b61 6e20 6669 6e6e 6173 206e  Det kan finnas n
-00000970: c3a4 7476 6572 6b73 7072 6f62 6c65 6d2e  ..tverksproblem.
-00000980: 7548 0000 0034 3034 2d66 656c 2076 6964  uH...404-fel vid
-00000990: 2061 6e73 6c75 746e 696e 672e 2044 656e   anslutning. Den
-000009a0: 2062 6567 c3a4 7264 6120 7369 6461 6e20   beg..rda sidan 
-000009b0: 656c 6c65 7220 7265 7375 7273 656e 2068  eller resursen h
-000009c0: 6974 7461 6465 7320 696e 7465 2e75 3500  ittades inte.u5.
-000009d0: 0000 46c3 b672 6672 c3a5 6761 6e20 6d69  ..F..rfr..gan mi
-000009e0: 7373 6c79 636b 6164 6573 206d 6564 2073  sslyckades med s
-000009f0: 7461 7475 736b 6f64 3a20 7b73 7461 7475  tatuskod: {statu
-00000a00: 735f 636f 6465 7d29 54da 0961 7070 5f74  s_code})T..app_t
-00000a10: 6974 6c65 da12 6170 705f 7469 746c 655f  itle..app_title_
-00000a20: 7769 7468 5f73 7562 da1b 7472 6565 5f66  with_sub..tree_f
-00000a30: 696c 7465 725f 6163 6365 7373 6962 6c65  ilter_accessible
-00000a40: 5f64 6573 63da 126d 656e 755f 6163 7469  _desc..menu_acti
-00000a50: 6f6e 5f72 656e 616d 65da 126d 656e 755f  on_rename..menu_
-00000a60: 6163 7469 6f6e 5f64 656c 6574 65da 1d6d  action_delete..m
-00000a70: 656e 755f 6163 7469 6f6e 5f64 656c 6574  enu_action_delet
-00000a80: 655f 636f 6d70 6c65 7465 6c79 da13 6d65  e_completely..me
-00000a90: 6e75 5f61 6374 696f 6e5f 7265 7374 6f72  nu_action_restor
-00000aa0: 65da 1864 6961 6c6f 675f 6669 6c65 5f72  e..dialog_file_r
-00000ab0: 656e 616d 655f 7469 746c 65da 1e64 6961  ename_title..dia
-00000ac0: 6c6f 675f 6669 6c65 5f72 656e 616d 655f  log_file_rename_
-00000ad0: 6669 656c 645f 6c61 6265 6cda 1c64 6961  field_label..dia
-00000ae0: 6c6f 675f 6669 6c65 5f72 656e 616d 655f  log_file_rename_
-00000af0: 6275 7474 6f6e 5f6f 6bda 2164 6961 6c6f  button_ok.!dialo
-00000b00: 675f 6669 6c65 5f72 656e 616d 655f 7761  g_file_rename_wa
-00000b10: 726e 696e 675f 6578 6973 7473 da18 6469  rning_exists..di
-00000b20: 616c 6f67 5f66 696c 655f 6465 6c65 7465  alog_file_delete
-00000b30: 5f74 6974 6c65 da17 6469 616c 6f67 5f66  _title..dialog_f
-00000b40: 696c 655f 6465 6c65 7465 5f74 6578 74da  ile_delete_text.
-00000b50: 2364 6961 6c6f 675f 6669 6c65 5f64 656c  #dialog_file_del
-00000b60: 6574 655f 636f 6d70 6c65 7465 6c79 5f74  ete_completely_t
-00000b70: 6974 6c65 da22 6469 616c 6f67 5f66 696c  itle."dialog_fil
-00000b80: 655f 6465 6c65 7465 5f63 6f6d 706c 6574  e_delete_complet
-00000b90: 656c 795f 7465 7874 da18 6469 616c 6f67  ely_text..dialog
-00000ba0: 5f66 696c 655f 6465 6c65 7465 5f65 7272  _file_delete_err
-00000bb0: 6f72 da22 6469 616c 6f67 5f66 696c 655f  or."dialog_file_
-00000bc0: 6465 6c65 7465 5f65 7272 6f72 5f6e 6f74  delete_error_not
-00000bd0: 5f66 6f75 6e64 da19 6469 616c 6f67 5f66  _found..dialog_f
-00000be0: 696c 655f 7265 7374 6f72 655f 7469 746c  ile_restore_titl
-00000bf0: 65da 1864 6961 6c6f 675f 6669 6c65 5f72  e..dialog_file_r
-00000c00: 6573 746f 7265 5f74 6578 74da 1964 6961  estore_text..dia
-00000c10: 6c6f 675f 6669 6c65 5f72 6573 746f 7265  log_file_restore
-00000c20: 5f65 7272 6f72 da22 6469 616c 6f67 5f66  _error."dialog_f
-00000c30: 696c 655f 7265 7374 6f72 655f 7761 726e  ile_restore_warn
-00000c40: 696e 675f 6578 6973 7473 da18 6469 616c  ing_exists..dial
-00000c50: 6f67 5f6d 6573 7361 6765 5f62 6f78 5f74  og_message_box_t
-00000c60: 6974 6c65 da1c 6469 616c 6f67 5f6d 6573  itle..dialog_mes
-00000c70: 7361 6765 5f62 6f78 5f62 7574 746f 6e5f  sage_box_button_
-00000c80: 6f6b da28 6163 7469 6f6e 5f6e 6577 5f66  ok.(action_new_f
-00000c90: 696c 655f 6669 7273 745f 6c69 6e65 5f74  ile_first_line_t
-00000ca0: 656d 706c 6174 655f 7465 7874 da1f 6163  emplate_text..ac
-00000cb0: 7469 6f6e 5f6f 7065 6e5f 6669 6c65 5f64  tion_open_file_d
-00000cc0: 6961 6c6f 675f 6361 7074 696f 6eda 2261  ialog_caption."a
-00000cd0: 6374 696f 6e5f 7361 7665 5f61 735f 6669  ction_save_as_fi
-00000ce0: 6c65 5f64 6961 6c6f 675f 6361 7074 696f  le_dialog_captio
-00000cf0: 6eda 1c64 6961 6c6f 675f 7361 7665 5f65  n..dialog_save_e
-00000d00: 6d70 7479 5f66 696c 655f 7469 746c 65da  mpty_file_title.
-00000d10: 1b64 6961 6c6f 675f 7361 7665 5f65 6d70  .dialog_save_emp
-00000d20: 7479 5f66 696c 655f 7465 7874 da19 6469  ty_file_text..di
-00000d30: 616c 6f67 5f65 6e63 7279 7074 5f66 696c  alog_encrypt_fil
-00000d40: 655f 7469 746c 65da 1864 6961 6c6f 675f  e_title..dialog_
-00000d50: 656e 6372 7970 745f 6669 6c65 5f74 6578  encrypt_file_tex
-00000d60: 74da 2e65 6e63 7279 7074 5f66 696c 655f  t..encrypt_file_
-00000d70: 7761 726e 696e 675f 6669 6c65 5f69 735f  warning_file_is_
-00000d80: 616c 7265 6164 795f 656e 6372 7970 7465  already_encrypte
-00000d90: 64da 2a64 6961 6c6f 675f 656e 6372 7970  d.*dialog_encryp
-00000da0: 745f 6669 6c65 5f72 6577 7269 7465 5f65  t_file_rewrite_e
-00000db0: 7869 7374 696e 675f 7469 746c 65da 2964  xisting_title.)d
-00000dc0: 6961 6c6f 675f 656e 6372 7970 745f 6669  ialog_encrypt_fi
-00000dd0: 6c65 5f72 6577 7269 7465 5f65 7869 7374  le_rewrite_exist
-00000de0: 696e 675f 7465 7874 da19 6469 616c 6f67  ing_text..dialog
-00000df0: 5f64 6563 7279 7074 5f66 696c 655f 7469  _decrypt_file_ti
-00000e00: 746c 65da 1864 6961 6c6f 675f 6465 6372  tle..dialog_decr
-00000e10: 7970 745f 6669 6c65 5f74 6578 74da 2a64  ypt_file_text.*d
-00000e20: 6563 7279 7074 5f66 696c 655f 7761 726e  ecrypt_file_warn
-00000e30: 696e 675f 6669 6c65 5f69 735f 6e6f 745f  ing_file_is_not_
-00000e40: 656e 6372 7970 7465 64da 2a64 6961 6c6f  encrypted.*dialo
-00000e50: 675f 6465 6372 7970 745f 6669 6c65 5f72  g_decrypt_file_r
-00000e60: 6577 7269 7465 5f65 7869 7374 696e 675f  ewrite_existing_
-00000e70: 7469 746c 65da 2964 6961 6c6f 675f 6465  title.)dialog_de
-00000e80: 6372 7970 745f 6669 6c65 5f72 6577 7269  crypt_file_rewri
-00000e90: 7465 5f65 7869 7374 696e 675f 7465 7874  te_existing_text
-00000ea0: da21 6469 616c 6f67 5f65 6e63 7279 7074  .!dialog_encrypt
-00000eb0: 5f6e 6577 5f70 6173 7377 6f72 645f 7469  _new_password_ti
-00000ec0: 746c 65da 2164 6961 6c6f 675f 656e 6372  tle.!dialog_encr
-00000ed0: 7970 745f 6e65 775f 7061 7373 776f 7264  ypt_new_password
-00000ee0: 5f6c 6162 656c da32 6469 616c 6f67 5f65  _label.2dialog_e
-00000ef0: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-00000f00: 6f72 645f 696e 7075 745f 706c 6163 6568  ord_input_placeh
-00000f10: 6f6c 6465 725f 7465 7874 da26 6469 616c  older_text.&dial
-00000f20: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
-00000f30: 6173 7377 6f72 645f 6869 6e74 5f6c 6162  assword_hint_lab
-00000f40: 656c da32 6469 616c 6f67 5f65 6e63 7279  el.2dialog_encry
-00000f50: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
-00000f60: 6869 6e74 5f6c 6162 656c 5f64 6573 6372  hint_label_descr
-00000f70: 6970 7469 6f6e da37 6469 616c 6f67 5f65  iption.7dialog_e
-00000f80: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-00000f90: 6f72 645f 6869 6e74 5f69 6e70 7574 5f70  ord_hint_input_p
-00000fa0: 6c61 6365 686f 6c64 6572 5f74 6578 74da  laceholder_text.
-00000fb0: 2564 6961 6c6f 675f 656e 6372 7970 745f  %dialog_encrypt_
-00000fc0: 6e65 775f 7061 7373 776f 7264 5f62 7574  new_password_but
-00000fd0: 746f 6e5f 6f6b da29 6469 616c 6f67 5f65  ton_ok.)dialog_e
-00000fe0: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-00000ff0: 6f72 645f 6275 7474 6f6e 5f63 616e 6365  ord_button_cance
-00001000: 6cda 2f64 6961 6c6f 675f 656e 6372 7970  l./dialog_encryp
-00001010: 745f 6e65 775f 7061 7373 776f 7264 5f77  t_new_password_w
-00001020: 6172 6e69 6e67 5f65 6d70 7479 5f74 6974  arning_empty_tit
-00001030: 6c65 da2e 6469 616c 6f67 5f65 6e63 7279  le..dialog_encry
-00001040: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
-00001050: 7761 726e 696e 675f 656d 7074 795f 7465  warning_empty_te
-00001060: 7874 da32 6469 616c 6f67 5f65 6e63 7279  xt.2dialog_encry
-00001070: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
-00001080: 7761 726e 696e 675f 746f 6f5f 6c6f 6e67  warning_too_long
-00001090: 5f74 6974 6c65 da31 6469 616c 6f67 5f65  _title.1dialog_e
-000010a0: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-000010b0: 6f72 645f 7761 726e 696e 675f 746f 6f5f  ord_warning_too_
-000010c0: 6c6f 6e67 5f74 6578 74da 1d64 6961 6c6f  long_text..dialo
-000010d0: 675f 656e 6372 7970 745f 7061 7373 776f  g_encrypt_passwo
-000010e0: 7264 5f74 6974 6c65 da1d 6469 616c 6f67  rd_title..dialog
-000010f0: 5f65 6e63 7279 7074 5f70 6173 7377 6f72  _encrypt_passwor
-00001100: 645f 6c61 6265 6cda 2e64 6961 6c6f 675f  d_label..dialog_
-00001110: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
-00001120: 5f69 6e70 7574 5f70 6c61 6365 686f 6c64  _input_placehold
-00001130: 6572 5f74 6578 74da 2264 6961 6c6f 675f  er_text."dialog_
-00001140: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
-00001150: 5f68 696e 745f 6c61 6265 6cda 2164 6961  _hint_label.!dia
-00001160: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
-00001170: 776f 7264 5f62 7574 746f 6e5f 6f6b da25  word_button_ok.%
-00001180: 6469 616c 6f67 5f65 6e63 7279 7074 5f70  dialog_encrypt_p
-00001190: 6173 7377 6f72 645f 6275 7474 6f6e 5f63  assword_button_c
-000011a0: 616e 6365 6cda 2364 6961 6c6f 675f 656e  ancel.#dialog_en
-000011b0: 6372 7970 745f 7061 7373 776f 7264 5f72  crypt_password_r
-000011c0: 6573 6574 5f74 6974 6c65 da22 6469 616c  eset_title."dial
-000011d0: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
-000011e0: 6f72 645f 7265 7365 745f 7465 7874 da2b  ord_reset_text.+
-000011f0: 6469 616c 6f67 5f65 6e63 7279 7074 5f70  dialog_encrypt_p
-00001200: 6173 7377 6f72 645f 7265 7365 745f 6275  assword_reset_bu
-00001210: 7474 6f6e 5f63 616e 6365 6cda 2864 6961  tton_cancel.(dia
-00001220: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
-00001230: 776f 7264 5f72 6573 6574 5f62 7574 746f  word_reset_butto
-00001240: 6e5f 7965 73da 1664 6961 6c6f 675f 6f70  n_yes..dialog_op
-00001250: 656e 5f6c 696e 6b5f 7469 746c 65da 1564  en_link_title..d
-00001260: 6961 6c6f 675f 6f70 656e 5f6c 696e 6b5f  ialog_open_link_
-00001270: 7465 7874 da26 6c6f 6164 5f66 696c 655f  text.&load_file_
-00001280: 656e 6372 7970 7469 6f6e 5f70 6173 7377  encryption_passw
-00001290: 6f72 645f 6d69 736d 6174 6368 da27 6c6f  ord_mismatch.'lo
-000012a0: 6164 5f66 696c 655f 656e 6372 7970 7469  ad_file_encrypti
-000012b0: 6f6e 5f70 6173 7377 6f72 645f 696e 636f  on_password_inco
-000012c0: 7272 6563 74da 1c6c 6f61 645f 6669 6c65  rrect..load_file
-000012d0: 5f6e 6f6e 655f 636f 6e74 656e 745f 6572  _none_content_er
-000012e0: 726f 72da 1f73 6176 655f 6163 7469 7665  ror..save_active
-000012f0: 5f66 696c 655f 6572 726f 725f 6f63 6375  _file_error_occu
-00001300: 7272 6564 da1e 6578 7061 6e64 6162 6c65  rred..expandable
-00001310: 5f62 6c6f 636b 5f64 6566 6175 6c74 5f74  _block_default_t
-00001320: 6974 6c65 da31 6469 616c 6f67 5f63 6f6c  itle.1dialog_col
-00001330: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00001340: 636f 7069 6564 5f74 6f5f 7468 655f 636c  copied_to_the_cl
-00001350: 6970 626f 6172 64da 1170 6f70 7570 5f61  ipboard..popup_a
-00001360: 626f 7574 5f74 6974 6c65 da20 706f 7075  bout_title. popu
-00001370: 705f 6162 6f75 745f 6170 705f 6e61 6d65  p_about_app_name
-00001380: 5f64 6573 6372 6970 7469 6f6e da13 706f  _description..po
-00001390: 7075 705f 6162 6f75 745f 7665 7273 696f  pup_about_versio
-000013a0: 6eda 1370 6f70 7570 5f61 626f 7574 5f6c  n..popup_about_l
-000013b0: 6963 656e 7365 da13 706f 7075 705f 6162  icense..popup_ab
-000013c0: 6f75 745f 7765 6273 6974 65da 1670 6f70  out_website..pop
-000013d0: 7570 5f61 626f 7574 5f72 6570 6f73 6974  up_about_reposit
-000013e0: 6f72 79da 1070 6f70 7570 5f61 626f 7574  ory..popup_about
-000013f0: 5f70 7970 69da 1070 6f70 7570 5f61 626f  _pypi..popup_abo
-00001400: 7574 5f64 6174 65da 2675 7064 6174 655f  ut_date.&update_
-00001410: 6865 6c70 6572 5f6e 6577 5f76 6572 7369  helper_new_versi
-00001420: 6f6e 5f69 735f 6176 6169 6c61 626c 65da  on_is_available.
-00001430: 2675 7064 6174 655f 6865 6c70 6572 5f6c  &update_helper_l
-00001440: 6174 6573 745f 7665 7273 696f 6e5f 696e  atest_version_in
-00001450: 7374 616c 6c65 64da 1e6e 6574 776f 726b  stalled..network
-00001460: 5f63 6f6e 6e65 6374 696f 6e5f 6572 726f  _connection_erro
-00001470: 725f 656d 7074 79da 2a6e 6574 776f 726b  r_empty.*network
-00001480: 5f63 6f6e 6e65 6374 696f 6e5f 6572 726f  _connection_erro
-00001490: 725f 636f 6e6e 6563 7469 6f6e 5f6f 725f  r_connection_or_
-000014a0: 646e 73da 2b6e 6574 776f 726b 5f63 6f6e  dns.+network_con
-000014b0: 6e65 6374 696f 6e5f 6572 726f 725f 636f  nection_error_co
-000014c0: 6e6e 6563 7469 6f6e 5f72 6566 7573 6564  nnection_refused
-000014d0: da2d 6e65 7477 6f72 6b5f 636f 6e6e 6563  .-network_connec
-000014e0: 7469 6f6e 5f65 7272 6f72 5f63 6f6e 6e65  tion_error_conne
-000014f0: 6374 696f 6e5f 7469 6d65 645f 6f75 74da  ction_timed_out.
-00001500: 2d6e 6574 776f 726b 5f63 6f6e 6e65 6374  -network_connect
-00001510: 696f 6e5f 6572 726f 725f 636f 6e6e 6563  ion_error_connec
-00001520: 7469 6f6e 5f34 3034 5f65 7272 6f72 da31  tion_404_error.1
-00001530: 6e65 7477 6f72 6b5f 636f 6e6e 6563 7469  network_connecti
-00001540: 6f6e 5f65 7272 6f72 5f67 656e 6572 6963  on_error_generic
-00001550: 5f77 6974 685f 7374 6174 7573 5f63 6f64  _with_status_cod
-00001560: 654e 2901 da07 6c65 7865 6d65 73a9 0072  eN)...lexemes..r
-00001570: 5900 0000 7259 0000 00fa 462f 5573 6572  Y...rY....F/User
-00001580: 732f 7661 6469 6b75 732f 5079 6368 6172  s/vadikus/Pychar
-00001590: 6d50 726f 6a65 6374 732f 6e6f 746f 6c6f  mProjects/notolo
-000015a0: 672d 6564 6974 6f72 2f61 7070 2f6c 6578  g-editor/app/lex
-000015b0: 656d 6573 2f73 652f 636f 6d6d 6f6e 2e70  emes/se/common.p
-000015c0: 79da 083c 6d6f 6475 6c65 3e03 0000 0073  y..<module>....s
-000015d0: a800 0000 0201 0202 0202 0201 0201 0201  ................
-000015e0: 0202 0201 0201 0201 0202 0201 0201 0201  ................
-000015f0: 0201 0201 0202 0201 0201 0201 0202 0201  ................
-00001600: 0202 0201 0201 0202 0201 0202 0201 0201  ................
-00001610: 0201 0201 0202 0201 0201 0201 0201 0202  ................
-00001620: 0201 0201 0201 0201 0204 0201 0201 0201  ................
-00001630: 0201 0201 0201 0202 0201 0201 0201 0201  ................
-00001640: 0201 0202 0201 0201 0201 0202 0201 0202  ................
-00001650: 0201 0201 0202 0202 0202 0202 0201 0202  ................
-00001660: 0201 0201 0201 0201 0201 0202 0201 0202  ................
-00001670: 0202 0202 0201 0202 0201 0290            ............
+00000050: 6410 6411 6412 6409 6413 6414 6415 6416  d.d.d.d.d.d.d.d.
+00000060: 6417 6418 6419 641a 641b 641c 641d 641e  d.d.d.d.d.d.d.d.
+00000070: 641f 6420 6421 641d 641e 6422 6423 6424  d.d d!d.d.d"d#d$
+00000080: 6425 6426 6427 6428 6429 642a 642b 642a  d%d&d'd(d)d*d+d*
+00000090: 642c 642d 6423 642d 6425 6428 6429 642e  d,d-d#d-d%d(d)d.
+000000a0: 642f 6429 6430 6431 6432 6433 6434 6435  d/d)d0d1d2d3d4d5
+000000b0: 6436 6437 6438 6439 643a 643b 643c 643d  d6d7d8d9d:d;d<d=
+000000c0: 643e 643f 6440 6441 6442 6443 6444 6445  d>d?d@dAdBdCdDdE
+000000d0: 6446 6447 6448 6449 9c54 5a00 644a 5300  dFdGdHdI.TZ.dJS.
+000000e0: 294b 7511 0000 004e 6f74 6f6c 6f67 2045  )Ku....Notolog E
+000000f0: 6469 74c3 b672 c3bc 7a19 7b61 7070 5f74  dit..r..z.{app_t
+00000100: 6974 6c65 7d20 2d20 7b73 7562 5f74 6974  itle} - {sub_tit
+00000110: 6c65 7d75 1300 0000 446f 7379 6120 6669  le}u....Dosya fi
+00000120: 6c74 7265 2061 6c61 6ec4 b175 1100 0000  ltre alan..u....
+00000130: 5965 6e69 6465 6e20 4164 6c61 6e64 c4b1  Yeniden Adland..
+00000140: 725a 0353 696c 7a0b 5461 6d61 6d65 6e20  rZ.Silz.Tamamen 
+00000150: 5369 6c75 0b00 0000 4765 7269 2059 c3bc  Silu....Geri Y..
+00000160: 6b6c 6575 1a00 0000 446f 7379 6179 c4b1  kleu....Dosyay..
+00000170: 2059 656e 6964 656e 2041 646c 616e 64c4   Yeniden Adland.
+00000180: b172 7518 0000 0059 656e 6920 646f 7379  .ru....Yeni dosy
+00000190: 6120 6164 c4b1 6ec4 b120 6769 7269 6e75  a ad..n.. girinu
+000001a0: 1c00 0000 4179 6ec4 b120 6973 696d 6465  ....Ayn.. isimde
+000001b0: 2064 6f73 7961 207a 6174 656e 2076 6172   dosya zaten var
+000001c0: 750c 0000 0044 6f73 7961 79c4 b120 5369  u....Dosyay.. Si
+000001d0: 6c75 1e00 0000 227b 6669 6c65 5f6e 616d  lu...."{file_nam
+000001e0: 657d 2220 646f 7379 6173 c4b1 6ec4 b120  e}" dosyas..n.. 
+000001f0: 7369 6c3f 7514 0000 0044 6f73 7961 79c4  sil?u....Dosyay.
+00000200: b120 5461 6d61 6d65 6e20 5369 6c75 2600  . Tamamen Silu&.
+00000210: 0000 227b 6669 6c65 5f6e 616d 657d 2220  .."{file_name}" 
+00000220: 646f 7379 6173 c4b1 6ec4 b120 7461 6d61  dosyas..n.. tama
+00000230: 6d65 6e20 7369 6c3f 751e 0000 0044 6f73  men sil?u....Dos
+00000240: 7961 2073 696c 696e 656d 6564 692c 2068  ya silinemedi, h
+00000250: 6174 6120 6f6c 75c5 9f74 7575 1100 0000  ata olu..tuu....
+00000260: 446f 7379 6120 6275 6c75 6e61 6d61 64c4  Dosya bulunamad.
+00000270: b175 1400 0000 446f 7379 6179 c4b1 2047  .u....Dosyay.. G
+00000280: 6572 6920 59c3 bc6b 6c65 7526 0000 0022  eri Y..kleu&..."
+00000290: 7b66 696c 655f 6e61 6d65 7d22 2064 6f73  {file_name}" dos
+000002a0: 7961 73c4 b16e c4b1 2067 6572 6920 79c3  yas..n.. geri y.
+000002b0: bc6b 6c65 3f75 2500 0000 446f 7379 6120  .kle?u%...Dosya 
+000002c0: 6765 7269 2079 c3bc 6b6c 656e 656d 6564  geri y..klenemed
+000002d0: 692c 2068 6174 6120 6f6c 75c5 9f74 755a  i, hata olu..tuZ
+000002e0: 054d 6573 616a 5a05 4b61 7061 747a 0a59  .MesajZ.Kapatz.Y
+000002f0: 656e 6920 6265 6c67 6575 0900 0000 446f  eni belgeu....Do
+00000300: 7379 6120 41c3 a775 1700 0000 446f 7379  sya A..u....Dosy
+00000310: 6179 c4b1 2046 6172 6b6c c4b1 204b 6179  ay.. Farkl.. Kay
+00000320: 6465 7475 1400 0000 426f c59f 2044 6f73  detu....Bo.. Dos
+00000330: 7961 79c4 b120 4b61 7964 6574 752c 0000  yay.. Kaydetu,..
+00000340: 0042 6fc5 9f20 69c3 a765 7269 6b6c 6920  .Bo.. i..erikli 
+00000350: 646f 7379 6179 c4b1 206b 6179 6465 746d  dosyay.. kaydetm
+00000360: 6579 6520 697a 696e 2076 6572 3f75 1100  eye izin ver?u..
+00000370: 0000 446f 7379 6179 c4b1 20c5 9e69 6672  ..Dosyay.. ..ifr
+00000380: 656c 6575 2300 0000 227b 6669 6c65 5f6e  eleu#..."{file_n
+00000390: 616d 657d 2220 646f 7379 6173 c4b1 6ec4  ame}" dosyas..n.
+000003a0: b120 c59f 6966 7265 6c65 3f75 1a00 0000  . ..ifrele?u....
+000003b0: 446f 7379 6120 7a61 7465 6e20 c59f 6966  Dosya zaten ..if
+000003c0: 7265 6c65 6e6d 69c5 9f21 751b 0000 004d  relenmi..!u....M
+000003d0: 6576 6375 7420 646f 7379 6179 c4b1 2079  evcut dosyay.. y
+000003e0: 656e 6964 656e 2079 617a 752a 0000 0022  eniden yazu*..."
+000003f0: 7b66 696c 655f 7061 7468 7d22 206d 6576  {file_path}" mev
+00000400: 6375 7420 646f 7379 6179 c4b1 2079 656e  cut dosyay.. yen
+00000410: 6964 656e 2079 617a 3f75 1a00 0000 446f  iden yaz?u....Do
+00000420: 7379 616e c4b1 6e20 c59e 6966 7265 7369  syan..n ..ifresi
+00000430: 6e69 20c3 87c3 b67a 752c 0000 0022 7b66  ni ....zu,..."{f
+00000440: 696c 655f 6e61 6d65 7d22 2064 6f73 7961  ile_name}" dosya
+00000450: 73c4 b16e c4b1 6e20 c59f 6966 7265 7369  s..n..n ..ifresi
+00000460: 6e69 20c3 a7c3 b67a 3f75 1600 0000 446f  ni ....z?u....Do
+00000470: 7379 6120 c59f 6966 7265 6c69 2064 65c4  sya ..ifreli de.
+00000480: 9f69 6c21 750b 0000 0059 656e 6920 c59e  .il!u....Yeni ..
+00000490: 6966 7265 7507 0000 00c5 9e69 6672 653a  ifreu......ifre:
+000004a0: 7511 0000 0059 656e 6920 c59e 6966 7265  u....Yeni ..ifre
+000004b0: 2047 6972 696e 7507 0000 00c4 b070 7563   Girinu......puc
+000004c0: 753a 75be 0000 00c4 b070 7563 7520 c59f  u:u......pucu ..
+000004d0: 6966 7265 6c65 6e6d 657a 2076 6520 646f  ifrelenmez ve do
+000004e0: 7379 6164 616e 206f 6b75 6e61 6269 6c69  syadan okunabili
+000004f0: 7221 0a4b 6f6c 6179 2074 6168 6d69 6e20  r!.Kolay tahmin 
+00000500: 6564 696c 6562 696c 6563 656b 2061 c3a7  edilebilecek a..
+00000510: c4b1 6b20 6970 75c3 a76c 6172 c4b1 206b  ..k ipu..lar.. k
+00000520: 756c 6c61 6e6d 6179 c4b1 6e2c 20c3 b672  ullanmay..n, ..r
+00000530: 6e65 c49f 696e 2064 6fc4 9f75 6d20 7461  ne..in do..um ta
+00000540: 7269 686c 6572 6920 6769 6269 2e0a 4b6f  rihleri gibi..Ko
+00000550: 6c61 7963 6120 696c 69c5 9f6b 696c 656e  layca ili..kilen
+00000560: 6469 7269 6c65 6d65 7965 6365 6b20 6269  dirilemeyecek bi
+00000570: 7220 7265 6665 7261 6e73 206b 756c 6c61  r referans kulla
+00000580: 6ec4 b16e 2e75 1f00 0000 c4b0 7075 6375  n..n.u......pucu
+00000590: 2047 6972 696e 2028 c4b0 7374 65c4 9f65   Girin (..ste..e
+000005a0: 2042 61c4 9f6c c4b1 295a 0554 616d 616d   Ba..l..)Z.Tamam
+000005b0: 7506 0000 00c4 b070 7461 6c75 0600 0000  u......ptalu....
+000005c0: 5579 6172 c4b1 751a 0000 00c5 9e69 6672  Uyar..u......ifr
+000005d0: 6520 616c 616e c4b1 2062 6fc5 9f20 6f6c  e alan.. bo.. ol
+000005e0: 616d 617a 2175 3500 0000 c4b0 7075 6375  amaz!u5.....pucu
+000005f0: 2061 6c61 6ec4 b120 c3a7 6f6b 2075 7a75   alan.. ..ok uzu
+00000600: 6e2c 206d 616b 7369 6d75 6d20 7b73 796d  n, maksimum {sym
+00000610: 626f 6c73 7d20 6b61 7261 6b74 6572 2175  bols} karakter!u
+00000620: 0c00 0000 c59e 6966 7265 2047 6972 696e  ......ifre Girin
+00000630: 751f 0000 00c5 9e69 6672 656c 656d 6520  u......ifreleme 
+00000640: c59e 6966 7265 7369 6e69 2053 c4b1 66c4  ..ifresini S..f.
+00000650: b172 6c61 7547 0000 004d 6576 6375 7420  .rlauG...Mevcut 
+00000660: c59f 6966 7265 6c65 6d65 20c5 9f69 6672  ..ifreleme ..ifr
+00000670: 6573 696e 6920 73c4 b166 c4b1 726c 616d  esini s..f..rlam
+00000680: 616b 2069 7374 6564 69c4 9f69 6e69 7a64  ak istedi..inizd
+00000690: 656e 2065 6d69 6e20 6d69 7369 6e69 7a3f  en emin misiniz?
+000006a0: 5a04 4576 6574 750a 0000 0042 61c4 9f6c  Z.Evetu....Ba..l
+000006b0: 616e 74c4 b175 2a00 0000 227b 7572 6c7d  ant..u*..."{url}
+000006c0: 2220 6261 c49f 6c61 6e74 c4b1 73c4 b16e  " ba..lant..s..n
+000006d0: c4b1 2074 6172 6179 c4b1 63c4 b164 6120  .. taray..c..da 
+000006e0: 61c3 a73f 751f 0000 00c5 9e69 6672 656c  a..?u......ifrel
+000006f0: 656d 6520 c59f 6966 7265 7369 2075 7975  eme ..ifresi uyu
+00000700: c59f 6d75 796f 7221 751d 0000 00c5 9e69  ..muyor!u......i
+00000710: 6672 656c 656d 6520 c59f 6966 7265 7369  freleme ..ifresi
+00000720: 2079 616e 6cc4 b1c5 9f21 7513 0000 0044   yanl....!u....D
+00000730: 6f73 7961 2079 c3bc 6b6c 656e 656d 6564  osya y..klenemed
+00000740: 692e 7521 0000 0044 6f73 7961 206b 6179  i.u!...Dosya kay
+00000750: 6465 6469 6c65 6d65 6469 2c20 6861 7461  dedilemedi, hata
+00000760: 206f 6c75 c59f 7475 7a13 4461 6861 2066   olu..tuz.Daha f
+00000770: 617a 6c61 2062 696c 6769 2e2e 2e75 2b00  azla bilgi...u+.
+00000780: 0000 4269 c3a7 696d 6c65 6e64 6972 696c  ..Bi..imlendiril
+00000790: 6d69 c59f 206d 6574 696e 2070 616e 6f79  mi.. metin panoy
+000007a0: 6120 6b6f 7079 616c 616e 64c4 b17a 1055  a kopyaland..z.U
+000007b0: 7967 756c 616d 6120 4269 6c67 6973 6975  ygulama Bilgisiu
+000007c0: 1200 0000 4d61 726b 646f 776e 2045 6469  ....Markdown Edi
+000007d0: 74c3 b672 c3bc 5a08 5665 7273 6979 6f6e  t..r..Z.Versiyon
+000007e0: 5a06 4c69 7361 6e73 7a0a 5765 6220 5369  Z.Lisansz.Web Si
+000007f0: 7465 7369 da06 4769 7448 7562 da04 5079  tesi..GitHub..Py
+00000800: 5069 5a05 5461 7269 6875 3500 0000 5579  PiZ.Tarihu5...Uy
+00000810: 6775 6c61 6d61 6ec4 b16e 2079 656e 6920  gulaman..n yeni 
+00000820: 7665 7273 6979 6f6e 7520 277b 6c61 7465  versiyonu '{late
+00000830: 7374 5f76 6572 7369 6f6e 7d27 206d 6576  st_version}' mev
+00000840: 6375 7475 2900 0000 5579 6775 6c61 6d61  cutu)...Uygulama
+00000850: 6ec4 b16e 2065 6e20 67c3 bc6e 6365 6c20  n..n en g..ncel 
+00000860: 7665 7273 6979 6f6e 7520 79c3 bc6b 6cc3  versiyonu y..kl.
+00000870: bc75 1b00 0000 5961 6ec4 b174 2062 696c  .u....Yan..t bil
+00000880: 6769 7369 2061 6cc4 b16e 616d c4b1 796f  gisi al..nam..yo
+00000890: 7275 4e00 0000 5375 6e75 6375 2062 756c  ruN...Sunucu bul
+000008a0: 756e 616d 6164 c4b1 2e20 c4b0 6e74 6572  unamad... ..nter
+000008b0: 6e65 7420 6261 c49f 6c61 6e74 c4b1 73c4  net ba..lant..s.
+000008c0: b16e 6461 2076 6579 6120 444e 5327 6465  .nda veya DNS'de
+000008d0: 2062 6972 2073 6f72 756e 206f 6c61 6269   bir sorun olabi
+000008e0: 6c69 722e 754f 0000 0042 61c4 9f6c 616e  lir.uO...Ba..lan
+000008f0: 74c4 b120 7265 6464 6564 696c 6469 2e20  t.. reddedildi. 
+00000900: 5375 6e75 6375 20c3 a7c3 b66b 6dc3 bcc5  Sunucu ....km...
+00000910: 9f20 6f6c 6162 696c 6972 2076 6579 6120  . olabilir veya 
+00000920: 61c4 9f20 736f 7275 6e6c 6172 c4b1 206f  a.. sorunlar.. o
+00000930: 6c61 6269 6c69 722e 753e 0000 0042 61c4  labilir.u>...Ba.
+00000940: 9f6c 616e 74c4 b120 7a61 6d61 6e20 61c5  .lant.. zaman a.
+00000950: 9fc4 b16d c4b1 6e61 2075 c49f 7261 64c4  ...m..na u..rad.
+00000960: b12e 2041 c49f 2073 6f72 756e 6c61 72c4  .. A.. sorunlar.
+00000970: b120 6f6c 6162 696c 6972 2e75 3f00 0000  . olabilir.u?...
+00000980: 3430 3420 6261 c49f 6c61 6e74 c4b1 2068  404 ba..lant.. h
+00000990: 6174 6173 c4b1 2e20 c4b0 7374 656e 656e  atas... ..stenen
+000009a0: 2073 6179 6661 2076 6579 6120 6b61 796e   sayfa veya kayn
+000009b0: 616b 2062 756c 756e 616d 6164 c4b1 2e75  ak bulunamad...u
+000009c0: 3700 0000 c4b0 7374 656b 2c20 7b73 7461  7.....stek, {sta
+000009d0: 7475 735f 636f 6465 7d20 6475 7275 6d20  tus_code} durum 
+000009e0: 6b6f 6475 2069 6c65 2062 61c5 9f61 72c4  kodu ile ba..ar.
+000009f0: b173 c4b1 7a20 6f6c 6475 2e29 54da 0961  .s..z oldu.)T..a
+00000a00: 7070 5f74 6974 6c65 da12 6170 705f 7469  pp_title..app_ti
+00000a10: 746c 655f 7769 7468 5f73 7562 da1b 7472  tle_with_sub..tr
+00000a20: 6565 5f66 696c 7465 725f 6163 6365 7373  ee_filter_access
+00000a30: 6962 6c65 5f64 6573 63da 126d 656e 755f  ible_desc..menu_
+00000a40: 6163 7469 6f6e 5f72 656e 616d 65da 126d  action_rename..m
+00000a50: 656e 755f 6163 7469 6f6e 5f64 656c 6574  enu_action_delet
+00000a60: 65da 1d6d 656e 755f 6163 7469 6f6e 5f64  e..menu_action_d
+00000a70: 656c 6574 655f 636f 6d70 6c65 7465 6c79  elete_completely
+00000a80: da13 6d65 6e75 5f61 6374 696f 6e5f 7265  ..menu_action_re
+00000a90: 7374 6f72 65da 1864 6961 6c6f 675f 6669  store..dialog_fi
+00000aa0: 6c65 5f72 656e 616d 655f 7469 746c 65da  le_rename_title.
+00000ab0: 1e64 6961 6c6f 675f 6669 6c65 5f72 656e  .dialog_file_ren
+00000ac0: 616d 655f 6669 656c 645f 6c61 6265 6cda  ame_field_label.
+00000ad0: 1c64 6961 6c6f 675f 6669 6c65 5f72 656e  .dialog_file_ren
+00000ae0: 616d 655f 6275 7474 6f6e 5f6f 6bda 2164  ame_button_ok.!d
+00000af0: 6961 6c6f 675f 6669 6c65 5f72 656e 616d  ialog_file_renam
+00000b00: 655f 7761 726e 696e 675f 6578 6973 7473  e_warning_exists
+00000b10: da18 6469 616c 6f67 5f66 696c 655f 6465  ..dialog_file_de
+00000b20: 6c65 7465 5f74 6974 6c65 da17 6469 616c  lete_title..dial
+00000b30: 6f67 5f66 696c 655f 6465 6c65 7465 5f74  og_file_delete_t
+00000b40: 6578 74da 2364 6961 6c6f 675f 6669 6c65  ext.#dialog_file
+00000b50: 5f64 656c 6574 655f 636f 6d70 6c65 7465  _delete_complete
+00000b60: 6c79 5f74 6974 6c65 da22 6469 616c 6f67  ly_title."dialog
+00000b70: 5f66 696c 655f 6465 6c65 7465 5f63 6f6d  _file_delete_com
+00000b80: 706c 6574 656c 795f 7465 7874 da18 6469  pletely_text..di
+00000b90: 616c 6f67 5f66 696c 655f 6465 6c65 7465  alog_file_delete
+00000ba0: 5f65 7272 6f72 da22 6469 616c 6f67 5f66  _error."dialog_f
+00000bb0: 696c 655f 6465 6c65 7465 5f65 7272 6f72  ile_delete_error
+00000bc0: 5f6e 6f74 5f66 6f75 6e64 da19 6469 616c  _not_found..dial
+00000bd0: 6f67 5f66 696c 655f 7265 7374 6f72 655f  og_file_restore_
+00000be0: 7469 746c 65da 1864 6961 6c6f 675f 6669  title..dialog_fi
+00000bf0: 6c65 5f72 6573 746f 7265 5f74 6578 74da  le_restore_text.
+00000c00: 1964 6961 6c6f 675f 6669 6c65 5f72 6573  .dialog_file_res
+00000c10: 746f 7265 5f65 7272 6f72 da22 6469 616c  tore_error."dial
+00000c20: 6f67 5f66 696c 655f 7265 7374 6f72 655f  og_file_restore_
+00000c30: 7761 726e 696e 675f 6578 6973 7473 da18  warning_exists..
+00000c40: 6469 616c 6f67 5f6d 6573 7361 6765 5f62  dialog_message_b
+00000c50: 6f78 5f74 6974 6c65 da1c 6469 616c 6f67  ox_title..dialog
+00000c60: 5f6d 6573 7361 6765 5f62 6f78 5f62 7574  _message_box_but
+00000c70: 746f 6e5f 6f6b da28 6163 7469 6f6e 5f6e  ton_ok.(action_n
+00000c80: 6577 5f66 696c 655f 6669 7273 745f 6c69  ew_file_first_li
+00000c90: 6e65 5f74 656d 706c 6174 655f 7465 7874  ne_template_text
+00000ca0: da1f 6163 7469 6f6e 5f6f 7065 6e5f 6669  ..action_open_fi
+00000cb0: 6c65 5f64 6961 6c6f 675f 6361 7074 696f  le_dialog_captio
+00000cc0: 6eda 2261 6374 696f 6e5f 7361 7665 5f61  n."action_save_a
+00000cd0: 735f 6669 6c65 5f64 6961 6c6f 675f 6361  s_file_dialog_ca
+00000ce0: 7074 696f 6eda 1c64 6961 6c6f 675f 7361  ption..dialog_sa
+00000cf0: 7665 5f65 6d70 7479 5f66 696c 655f 7469  ve_empty_file_ti
+00000d00: 746c 65da 1b64 6961 6c6f 675f 7361 7665  tle..dialog_save
+00000d10: 5f65 6d70 7479 5f66 696c 655f 7465 7874  _empty_file_text
+00000d20: da19 6469 616c 6f67 5f65 6e63 7279 7074  ..dialog_encrypt
+00000d30: 5f66 696c 655f 7469 746c 65da 1864 6961  _file_title..dia
+00000d40: 6c6f 675f 656e 6372 7970 745f 6669 6c65  log_encrypt_file
+00000d50: 5f74 6578 74da 2e65 6e63 7279 7074 5f66  _text..encrypt_f
+00000d60: 696c 655f 7761 726e 696e 675f 6669 6c65  ile_warning_file
+00000d70: 5f69 735f 616c 7265 6164 795f 656e 6372  _is_already_encr
+00000d80: 7970 7465 64da 2a64 6961 6c6f 675f 656e  ypted.*dialog_en
+00000d90: 6372 7970 745f 6669 6c65 5f72 6577 7269  crypt_file_rewri
+00000da0: 7465 5f65 7869 7374 696e 675f 7469 746c  te_existing_titl
+00000db0: 65da 2964 6961 6c6f 675f 656e 6372 7970  e.)dialog_encryp
+00000dc0: 745f 6669 6c65 5f72 6577 7269 7465 5f65  t_file_rewrite_e
+00000dd0: 7869 7374 696e 675f 7465 7874 da19 6469  xisting_text..di
+00000de0: 616c 6f67 5f64 6563 7279 7074 5f66 696c  alog_decrypt_fil
+00000df0: 655f 7469 746c 65da 1864 6961 6c6f 675f  e_title..dialog_
+00000e00: 6465 6372 7970 745f 6669 6c65 5f74 6578  decrypt_file_tex
+00000e10: 74da 2a64 6563 7279 7074 5f66 696c 655f  t.*decrypt_file_
+00000e20: 7761 726e 696e 675f 6669 6c65 5f69 735f  warning_file_is_
+00000e30: 6e6f 745f 656e 6372 7970 7465 64da 2a64  not_encrypted.*d
+00000e40: 6961 6c6f 675f 6465 6372 7970 745f 6669  ialog_decrypt_fi
+00000e50: 6c65 5f72 6577 7269 7465 5f65 7869 7374  le_rewrite_exist
+00000e60: 696e 675f 7469 746c 65da 2964 6961 6c6f  ing_title.)dialo
+00000e70: 675f 6465 6372 7970 745f 6669 6c65 5f72  g_decrypt_file_r
+00000e80: 6577 7269 7465 5f65 7869 7374 696e 675f  ewrite_existing_
+00000e90: 7465 7874 da21 6469 616c 6f67 5f65 6e63  text.!dialog_enc
+00000ea0: 7279 7074 5f6e 6577 5f70 6173 7377 6f72  rypt_new_passwor
+00000eb0: 645f 7469 746c 65da 2164 6961 6c6f 675f  d_title.!dialog_
+00000ec0: 656e 6372 7970 745f 6e65 775f 7061 7373  encrypt_new_pass
+00000ed0: 776f 7264 5f6c 6162 656c da32 6469 616c  word_label.2dial
+00000ee0: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
+00000ef0: 6173 7377 6f72 645f 696e 7075 745f 706c  assword_input_pl
+00000f00: 6163 6568 6f6c 6465 725f 7465 7874 da26  aceholder_text.&
+00000f10: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
+00000f20: 6577 5f70 6173 7377 6f72 645f 6869 6e74  ew_password_hint
+00000f30: 5f6c 6162 656c da32 6469 616c 6f67 5f65  _label.2dialog_e
+00000f40: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
+00000f50: 6f72 645f 6869 6e74 5f6c 6162 656c 5f64  ord_hint_label_d
+00000f60: 6573 6372 6970 7469 6f6e da37 6469 616c  escription.7dial
+00000f70: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
+00000f80: 6173 7377 6f72 645f 6869 6e74 5f69 6e70  assword_hint_inp
+00000f90: 7574 5f70 6c61 6365 686f 6c64 6572 5f74  ut_placeholder_t
+00000fa0: 6578 74da 2564 6961 6c6f 675f 656e 6372  ext.%dialog_encr
+00000fb0: 7970 745f 6e65 775f 7061 7373 776f 7264  ypt_new_password
+00000fc0: 5f62 7574 746f 6e5f 6f6b da29 6469 616c  _button_ok.)dial
+00000fd0: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
+00000fe0: 6173 7377 6f72 645f 6275 7474 6f6e 5f63  assword_button_c
+00000ff0: 616e 6365 6cda 2f64 6961 6c6f 675f 656e  ancel./dialog_en
+00001000: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
+00001010: 7264 5f77 6172 6e69 6e67 5f65 6d70 7479  rd_warning_empty
+00001020: 5f74 6974 6c65 da2e 6469 616c 6f67 5f65  _title..dialog_e
+00001030: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
+00001040: 6f72 645f 7761 726e 696e 675f 656d 7074  ord_warning_empt
+00001050: 795f 7465 7874 da32 6469 616c 6f67 5f65  y_text.2dialog_e
+00001060: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
+00001070: 6f72 645f 7761 726e 696e 675f 746f 6f5f  ord_warning_too_
+00001080: 6c6f 6e67 5f74 6974 6c65 da31 6469 616c  long_title.1dial
+00001090: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
+000010a0: 6173 7377 6f72 645f 7761 726e 696e 675f  assword_warning_
+000010b0: 746f 6f5f 6c6f 6e67 5f74 6578 74da 1d64  too_long_text..d
+000010c0: 6961 6c6f 675f 656e 6372 7970 745f 7061  ialog_encrypt_pa
+000010d0: 7373 776f 7264 5f74 6974 6c65 da1d 6469  ssword_title..di
+000010e0: 616c 6f67 5f65 6e63 7279 7074 5f70 6173  alog_encrypt_pas
+000010f0: 7377 6f72 645f 6c61 6265 6cda 2e64 6961  sword_label..dia
+00001100: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
+00001110: 776f 7264 5f69 6e70 7574 5f70 6c61 6365  word_input_place
+00001120: 686f 6c64 6572 5f74 6578 74da 2264 6961  holder_text."dia
+00001130: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
+00001140: 776f 7264 5f68 696e 745f 6c61 6265 6cda  word_hint_label.
+00001150: 2164 6961 6c6f 675f 656e 6372 7970 745f  !dialog_encrypt_
+00001160: 7061 7373 776f 7264 5f62 7574 746f 6e5f  password_button_
+00001170: 6f6b da25 6469 616c 6f67 5f65 6e63 7279  ok.%dialog_encry
+00001180: 7074 5f70 6173 7377 6f72 645f 6275 7474  pt_password_butt
+00001190: 6f6e 5f63 616e 6365 6cda 2364 6961 6c6f  on_cancel.#dialo
+000011a0: 675f 656e 6372 7970 745f 7061 7373 776f  g_encrypt_passwo
+000011b0: 7264 5f72 6573 6574 5f74 6974 6c65 da22  rd_reset_title."
+000011c0: 6469 616c 6f67 5f65 6e63 7279 7074 5f70  dialog_encrypt_p
+000011d0: 6173 7377 6f72 645f 7265 7365 745f 7465  assword_reset_te
+000011e0: 7874 da2b 6469 616c 6f67 5f65 6e63 7279  xt.+dialog_encry
+000011f0: 7074 5f70 6173 7377 6f72 645f 7265 7365  pt_password_rese
+00001200: 745f 6275 7474 6f6e 5f63 616e 6365 6cda  t_button_cancel.
+00001210: 2864 6961 6c6f 675f 656e 6372 7970 745f  (dialog_encrypt_
+00001220: 7061 7373 776f 7264 5f72 6573 6574 5f62  password_reset_b
+00001230: 7574 746f 6e5f 7965 73da 1664 6961 6c6f  utton_yes..dialo
+00001240: 675f 6f70 656e 5f6c 696e 6b5f 7469 746c  g_open_link_titl
+00001250: 65da 1564 6961 6c6f 675f 6f70 656e 5f6c  e..dialog_open_l
+00001260: 696e 6b5f 7465 7874 da26 6c6f 6164 5f66  ink_text.&load_f
+00001270: 696c 655f 656e 6372 7970 7469 6f6e 5f70  ile_encryption_p
+00001280: 6173 7377 6f72 645f 6d69 736d 6174 6368  assword_mismatch
+00001290: da27 6c6f 6164 5f66 696c 655f 656e 6372  .'load_file_encr
+000012a0: 7970 7469 6f6e 5f70 6173 7377 6f72 645f  yption_password_
+000012b0: 696e 636f 7272 6563 74da 1c6c 6f61 645f  incorrect..load_
+000012c0: 6669 6c65 5f6e 6f6e 655f 636f 6e74 656e  file_none_conten
+000012d0: 745f 6572 726f 72da 1f73 6176 655f 6163  t_error..save_ac
+000012e0: 7469 7665 5f66 696c 655f 6572 726f 725f  tive_file_error_
+000012f0: 6f63 6375 7272 6564 da1e 6578 7061 6e64  occurred..expand
+00001300: 6162 6c65 5f62 6c6f 636b 5f64 6566 6175  able_block_defau
+00001310: 6c74 5f74 6974 6c65 da31 6469 616c 6f67  lt_title.1dialog
+00001320: 5f63 6f6c 6f72 5f70 6963 6b65 725f 636f  _color_picker_co
+00001330: 6c6f 725f 636f 7069 6564 5f74 6f5f 7468  lor_copied_to_th
+00001340: 655f 636c 6970 626f 6172 64da 1170 6f70  e_clipboard..pop
+00001350: 7570 5f61 626f 7574 5f74 6974 6c65 da20  up_about_title. 
+00001360: 706f 7075 705f 6162 6f75 745f 6170 705f  popup_about_app_
+00001370: 6e61 6d65 5f64 6573 6372 6970 7469 6f6e  name_description
+00001380: da13 706f 7075 705f 6162 6f75 745f 7665  ..popup_about_ve
+00001390: 7273 696f 6eda 1370 6f70 7570 5f61 626f  rsion..popup_abo
+000013a0: 7574 5f6c 6963 656e 7365 da13 706f 7075  ut_license..popu
+000013b0: 705f 6162 6f75 745f 7765 6273 6974 65da  p_about_website.
+000013c0: 1670 6f70 7570 5f61 626f 7574 5f72 6570  .popup_about_rep
+000013d0: 6f73 6974 6f72 79da 1070 6f70 7570 5f61  ository..popup_a
+000013e0: 626f 7574 5f70 7970 69da 1070 6f70 7570  bout_pypi..popup
+000013f0: 5f61 626f 7574 5f64 6174 65da 2675 7064  _about_date.&upd
+00001400: 6174 655f 6865 6c70 6572 5f6e 6577 5f76  ate_helper_new_v
+00001410: 6572 7369 6f6e 5f69 735f 6176 6169 6c61  ersion_is_availa
+00001420: 626c 65da 2675 7064 6174 655f 6865 6c70  ble.&update_help
+00001430: 6572 5f6c 6174 6573 745f 7665 7273 696f  er_latest_versio
+00001440: 6e5f 696e 7374 616c 6c65 64da 1e6e 6574  n_installed..net
+00001450: 776f 726b 5f63 6f6e 6e65 6374 696f 6e5f  work_connection_
+00001460: 6572 726f 725f 656d 7074 79da 2a6e 6574  error_empty.*net
+00001470: 776f 726b 5f63 6f6e 6e65 6374 696f 6e5f  work_connection_
+00001480: 6572 726f 725f 636f 6e6e 6563 7469 6f6e  error_connection
+00001490: 5f6f 725f 646e 73da 2b6e 6574 776f 726b  _or_dns.+network
+000014a0: 5f63 6f6e 6e65 6374 696f 6e5f 6572 726f  _connection_erro
+000014b0: 725f 636f 6e6e 6563 7469 6f6e 5f72 6566  r_connection_ref
+000014c0: 7573 6564 da2d 6e65 7477 6f72 6b5f 636f  used.-network_co
+000014d0: 6e6e 6563 7469 6f6e 5f65 7272 6f72 5f63  nnection_error_c
+000014e0: 6f6e 6e65 6374 696f 6e5f 7469 6d65 645f  onnection_timed_
+000014f0: 6f75 74da 2d6e 6574 776f 726b 5f63 6f6e  out.-network_con
+00001500: 6e65 6374 696f 6e5f 6572 726f 725f 636f  nection_error_co
+00001510: 6e6e 6563 7469 6f6e 5f34 3034 5f65 7272  nnection_404_err
+00001520: 6f72 da31 6e65 7477 6f72 6b5f 636f 6e6e  or.1network_conn
+00001530: 6563 7469 6f6e 5f65 7272 6f72 5f67 656e  ection_error_gen
+00001540: 6572 6963 5f77 6974 685f 7374 6174 7573  eric_with_status
+00001550: 5f63 6f64 654e 2901 da07 6c65 7865 6d65  _codeN)...lexeme
+00001560: 73a9 0072 5800 0000 7258 0000 00fa 432f  s..rX...rX....C/
+00001570: 5573 6572 732f 7661 6469 6b75 732f 5079  Users/vadikus/Py
+00001580: 6368 6172 6d50 726f 6a65 6374 732f 6e6f  charmProjects/no
+00001590: 746f 6c6f 672d 6465 762f 6170 702f 6c65  tolog-dev/app/le
+000015a0: 7865 6d65 732f 7472 2f63 6f6d 6d6f 6e2e  xemes/tr/common.
+000015b0: 7079 da08 3c6d 6f64 756c 653e 0300 0000  py..<module>....
+000015c0: 73a8 0000 0002 0102 0202 0202 0102 0102  s...............
+000015d0: 0102 0202 0102 0102 0102 0202 0102 0102  ................
+000015e0: 0102 0102 0102 0202 0102 0102 0102 0202  ................
+000015f0: 0102 0202 0102 0102 0202 0102 0202 0102  ................
+00001600: 0102 0102 0102 0202 0102 0102 0102 0102  ................
+00001610: 0202 0102 0102 0102 0102 0302 0102 0102  ................
+00001620: 0102 0102 0102 0102 0202 0102 0102 0102  ................
+00001630: 0102 0102 0202 0102 0102 0102 0202 0102  ................
+00001640: 0202 0102 0102 0202 0202 0202 0202 0102  ................
+00001650: 0202 0102 0102 0102 0102 0102 0202 0102  ................
+00001660: 0202 0202 0202 0102 0202 0102 91         .............
```

### Comparing `notolog-0.9.1b0/app/lexemes/se/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May  5 14:33:15 2024 UTC, .py size: 3627 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,223 +1,235 @@
-00000000: 610d 0d0a 0000 0000 ab98 3766 2b0e 0000  a.........7f+...
+00000000: 610d 0d0a 0000 0000 42a9 3566 950e 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0030 0000 0040 0000 0073 6800 0000 6400  .0...@...sh...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
 00000080: 6429 642a 642b 642c 642d 642e 642f 9c2f  d)d*d+d,d-d.d/./
-00000090: 5a00 6430 5300 2931 750e 0000 0049 6e73  Z.d0S.)1u....Ins
-000000a0: 74c3 a46c 6c6e 696e 6761 7275 0600 0000  t..llningaru....
-000000b0: 5374 c3a4 6e67 7508 0000 0041 6c6c 6dc3  St..ngu....Allm.
-000000c0: a46e 745a 0a52 6564 6967 6572 6172 655a  .ntZ.RedigerareZ
-000000d0: 0656 6973 6172 657a 1041 492d 6b6f 6e66  .Visarez.AI-konf
-000000e0: 6967 7572 6174 696f 6e5a 1041 7070 6b6f  igurationZ.Appko
-000000f0: 6e66 6967 7572 6174 696f 6e75 0600 0000  nfigurationu....
-00000100: 5370 72c3 a56b 7510 0000 0056 c3a4 6c6a  Spr..ku....V..lj
-00000110: 2065 7474 2073 7072 c3a5 6b75 1900 0000   ett spr..ku....
-00000120: 4170 7065 6e73 2067 72c3 a46e 7373 6e69  Appens gr..nssni
-00000130: 7474 7373 7072 c3a5 6b5a 0454 656d 6175  ttsspr..kZ.Temau
-00000140: 0e00 0000 56c3 a46c 6a20 6574 7420 7465  ....V..lj ett te
-00000150: 6d61 7517 0000 0041 7070 656e 7320 6772  mau....Appens gr
-00000160: c3a4 6e73 736e 6974 7473 7465 6d61 5a09  ..nssnittstemaZ.
-00000170: 4875 7675 646d 656e 797a 0e56 6973 6120  Huvudmenyz.Visa 
-00000180: 6875 7675 646d 656e 797a 1d56 6973 6120  huvudmenyz.Visa 
-00000190: 6170 7065 6e73 2068 7576 7564 6472 6f70  appens huvuddrop
-000001a0: 646f 776e 6d65 6e79 7a17 5465 636b 656e  downmenyz.Tecken
-000001b0: 7374 6f72 6c65 6b3a 207b 7369 7a65 7d70  storlek: {size}p
-000001c0: 747a 244a 7573 7465 7261 2061 7070 656e  tz$Justera appen
-000001d0: 7320 676c 6f62 616c 6120 7465 636b 656e  s globala tecken
-000001e0: 7374 6f72 6c65 6b75 0b00 0000 5374 6174  storleku....Stat
-000001f0: 7573 66c3 a46c 747a 1d56 6973 6120 676c  usf..ltz.Visa gl
-00000200: 6f62 616c 206d 7573 7065 6b61 7265 706f  obal muspekarepo
-00000210: 7369 7469 6f6e 7534 0000 0056 6973 6120  sitionu4...Visa 
-00000220: 6465 6e20 676c 6f62 616c 6120 6d75 7370  den globala musp
-00000230: 656b 6172 6570 6f73 6974 696f 6e65 6e20  ekarepositionen 
-00000240: 6920 7374 6174 7573 66c3 a46c 7465 745a  i statusf..ltetZ
-00000250: 1652 6564 6967 6572 6172 6b6f 6e66 6967  .Redigerarkonfig
-00000260: 7572 6174 696f 6e7a 0e56 6973 6120 7261  urationz.Visa ra
-00000270: 646e 756d 6d65 727a 1c56 6973 6120 7261  dnummerz.Visa ra
-00000280: 646e 756d 6d65 7220 6920 7265 6469 6765  dnummer i redige
-00000290: 7261 7265 6e5a 1256 6973 6172 6b6f 6e66  rarenZ.Visarkonf
-000002a0: 6967 7572 6174 696f 6e7a 214b 6f6e 7665  igurationz!Konve
-000002b0: 7274 6572 6120 7465 7874 656d 6f6a 6973  rtera textemojis
-000002c0: 2074 696c 6c20 6772 6166 696b 7a34 4b6f   till grafikz4Ko
-000002d0: 6e76 6572 7465 7261 2074 6578 7465 6d6f  nvertera textemo
-000002e0: 6a69 7320 7469 6c6c 2067 7261 6669 736b  jis till grafisk
-000002f0: 6120 7265 7072 6573 656e 7461 7469 6f6e  a representation
-00000300: 6572 7a0d 4d61 726b 6572 6120 544f 444f  erz.Markera TODO
-00000310: 737a 1c4d 6172 6b65 7261 2054 4f44 4f2d  sz.Markera TODO-
-00000320: 7461 6767 6172 2069 2074 6578 7465 6e75  taggar i textenu
-00000330: 2a00 0000 4b72 c3a4 7620 6265 6b72 c3a4  *...Kr..v bekr..
-00000340: 6674 656c 7365 2066 c3b6 7220 6174 7420  ftelse f..r att 
-00000350: c3b6 7070 6e61 206c c3a4 6e6b 6172 7529  ..ppna l..nkaru)
-00000360: 0000 0042 6567 c3a4 7220 6265 6b72 c3a4  ...Beg..r bekr..
-00000370: 6674 656c 7365 2069 6e6e 616e 206c c3a4  ftelse innan l..
-00000380: 6e6b 6172 20c3 b670 706e 6173 7529 0000  nkar ..ppnasu)..
-00000390: 0053 7061 7261 2061 7574 6f6d 6174 6973  .Spara automatis
-000003a0: 6b74 2065 7874 6572 6e61 2062 696c 6465  kt externa bilde
-000003b0: 7220 70c3 a520 6469 736b 754c 0000 0053  r p.. diskuL...S
-000003c0: 7061 7261 7220 6175 746f 6d61 7469 736b  parar automatisk
-000003d0: 7420 6b6f 7069 6f72 2061 7620 6578 7465  t kopior av exte
-000003e0: 726e 6120 6269 6c64 6572 2070 c3a5 2064  rna bilder p.. d
-000003f0: 6973 6b65 6e20 66c3 b672 206f 6666 6c69  isken f..r offli
-00000400: 6e65 2dc3 a574 6b6f 6d73 747a 0a4f 7065  ne-..tkomstz.Ope
-00000410: 6e41 4920 4150 497a 0741 5049 2055 524c  nAI APIz.API URL
-00000420: 7a0e 4f70 656e 4149 2041 5049 2055 524c  z.OpenAI API URL
-00000430: 7a0a 4150 492d 6e79 636b 656c 7a11 4f70  z.API-nyckelz.Op
-00000440: 656e 4149 2041 5049 2d6e 7963 6b65 6c75  enAI API-nyckelu
-00000450: 1000 0000 5374 c3b6 6464 6120 6d6f 6465  ....St..dda mode
-00000460: 6c6c 6572 750c 0000 0056 c3a4 6c6a 206d  lleru....V..lj m
-00000470: 6f64 656c 6c75 1c00 0000 56c3 a46c 6a20  odellu....V..lj 
-00000480: 626c 616e 6420 7374 c3b6 6464 6120 6d6f  bland st..dda mo
-00000490: 6465 6c6c 6572 5a0d 4261 7370 6172 616d  dellerZ.Basparam
-000004a0: 6574 7261 725a 0c53 7973 7465 6d70 726f  etrarZ.Systempro
-000004b0: 6d70 7475 3000 0000 4261 7320 7379 7374  mptu0...Bas syst
-000004c0: 656d 7072 6f6d 7074 2073 6f6d 2066 c3b6  emprompt som f..
-000004d0: 7265 67c3 a572 2076 6172 6a65 2066 c3b6  reg..r varje f..
-000004e0: 7266 72c3 a567 616e 7545 0000 0042 6173  rfr..ganuE...Bas
-000004f0: 2073 7973 7465 6d70 726f 6d70 7420 736f   systemprompt so
-00000500: 6d20 66c3 b672 6567 c3a5 7220 7661 726a  m f..reg..r varj
-00000510: 6520 66c3 b672 6672 c3a5 6761 6e2e 2044  e f..rfr..gan. D
-00000520: 6574 7461 20c3 a472 2072 656e 2074 6578  etta ..r ren tex
-00000530: 742e 7a19 4d61 7869 6d61 6c74 2061 6e74  t.z.Maximalt ant
-00000540: 616c 2073 7661 7273 746f 6b65 6e7a 294d  al svarstokenz)M
-00000550: 6178 696d 616c 7420 616e 7461 6c20 746f  aximalt antal to
-00000560: 6b65 6e20 6174 7420 7461 2065 6d6f 7420  ken att ta emot 
-00000570: 736f 6d20 7376 6172 292f da0c 7769 6e64  som svar)/..wind
-00000580: 6f77 5f74 6974 6c65 da0c 6275 7474 6f6e  ow_title..button
-00000590: 5f63 6c6f 7365 da0b 7461 625f 6765 6e65  _close..tab_gene
-000005a0: 7261 6cda 1174 6162 5f65 6469 746f 725f  ral..tab_editor_
-000005b0: 636f 6e66 6967 da11 7461 625f 7669 6577  config..tab_view
-000005c0: 6572 5f63 6f6e 6669 67da 0d74 6162 5f61  er_config..tab_a
-000005d0: 695f 636f 6e66 6967 da18 6765 6e65 7261  i_config..genera
-000005e0: 6c5f 6170 705f 636f 6e66 6967 5f6c 6162  l_app_config_lab
-000005f0: 656c da1a 6765 6e65 7261 6c5f 6170 705f  el..general_app_
-00000600: 6c61 6e67 7561 6765 5f6c 6162 656c da2b  language_label.+
-00000610: 6765 6e65 7261 6c5f 6170 705f 6c61 6e67  general_app_lang
-00000620: 7561 6765 5f63 6f6d 626f 5f70 6c61 6365  uage_combo_place
-00000630: 686f 6c64 6572 5f74 6578 74da 3167 656e  holder_text.1gen
-00000640: 6572 616c 5f61 7070 5f6c 616e 6775 6167  eral_app_languag
-00000650: 655f 636f 6d62 6f5f 6163 6365 7373 6962  e_combo_accessib
-00000660: 6c65 5f64 6573 6372 6970 7469 6f6e da17  le_description..
-00000670: 6765 6e65 7261 6c5f 6170 705f 7468 656d  general_app_them
-00000680: 655f 6c61 6265 6cda 2867 656e 6572 616c  e_label.(general
-00000690: 5f61 7070 5f74 6865 6d65 5f63 6f6d 626f  _app_theme_combo
-000006a0: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
-000006b0: 74da 2e67 656e 6572 616c 5f61 7070 5f74  t..general_app_t
-000006c0: 6865 6d65 5f63 6f6d 626f 5f61 6363 6573  heme_combo_acces
-000006d0: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-000006e0: 6eda 1b67 656e 6572 616c 5f61 7070 5f6d  n..general_app_m
-000006f0: 6169 6e5f 6d65 6e75 5f6c 6162 656c da1e  ain_menu_label..
-00000700: 6765 6e65 7261 6c5f 6170 705f 6d61 696e  general_app_main
-00000710: 5f6d 656e 755f 6368 6563 6b62 6f78 da35  _menu_checkbox.5
-00000720: 6765 6e65 7261 6c5f 6170 705f 6d61 696e  general_app_main
-00000730: 5f6d 656e 755f 6368 6563 6b62 6f78 5f61  _menu_checkbox_a
-00000740: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
-00000750: 7074 696f 6eda 1b67 656e 6572 616c 5f61  ption..general_a
-00000760: 7070 5f66 6f6e 745f 7369 7a65 5f6c 6162  pp_font_size_lab
-00000770: 656c da33 6765 6e65 7261 6c5f 6170 705f  el.3general_app_
-00000780: 666f 6e74 5f73 697a 655f 736c 6964 6572  font_size_slider
-00000790: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-000007a0: 7269 7074 696f 6eda 1767 656e 6572 616c  ription..general
-000007b0: 5f73 7461 7475 7362 6172 5f6c 6162 656c  _statusbar_label
-000007c0: da36 6765 6e65 7261 6c5f 7374 6174 7573  .6general_status
-000007d0: 6261 725f 7368 6f77 5f67 6c6f 6261 6c5f  bar_show_global_
-000007e0: 6375 7273 6f72 5f70 6f73 6974 696f 6e5f  cursor_position_
-000007f0: 6368 6563 6b62 6f78 da4d 6765 6e65 7261  checkbox.Mgenera
-00000800: 6c5f 7374 6174 7573 6261 725f 7368 6f77  l_statusbar_show
-00000810: 5f67 6c6f 6261 6c5f 6375 7273 6f72 5f70  _global_cursor_p
-00000820: 6f73 6974 696f 6e5f 6368 6563 6b62 6f78  osition_checkbox
-00000830: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-00000840: 7269 7074 696f 6eda 1365 6469 746f 725f  ription..editor_
-00000850: 636f 6e66 6967 5f6c 6162 656c da28 6564  config_label.(ed
-00000860: 6974 6f72 5f63 6f6e 6669 675f 7368 6f77  itor_config_show
-00000870: 5f6c 696e 655f 6e75 6d62 6572 735f 6368  _line_numbers_ch
-00000880: 6563 6b62 6f78 da3f 6564 6974 6f72 5f63  eckbox.?editor_c
-00000890: 6f6e 6669 675f 7368 6f77 5f6c 696e 655f  onfig_show_line_
-000008a0: 6e75 6d62 6572 735f 6368 6563 6b62 6f78  numbers_checkbox
-000008b0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-000008c0: 7269 7074 696f 6eda 1376 6965 7765 725f  ription..viewer_
-000008d0: 636f 6e66 6967 5f6c 6162 656c da25 7669  config_label.%vi
-000008e0: 6577 6572 5f63 6f6e 6669 675f 7072 6f63  ewer_config_proc
-000008f0: 6573 735f 656d 6f6a 6973 5f63 6865 636b  ess_emojis_check
-00000900: 626f 78da 3c76 6965 7765 725f 636f 6e66  box.<viewer_conf
-00000910: 6967 5f70 726f 6365 7373 5f65 6d6f 6a69  ig_process_emoji
-00000920: 735f 6368 6563 6b62 6f78 5f61 6363 6573  s_checkbox_acces
-00000930: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000940: 6eda 2676 6965 7765 725f 636f 6e66 6967  n.&viewer_config
-00000950: 5f68 6967 686c 6967 6874 5f74 6f64 6f73  _highlight_todos
-00000960: 5f63 6865 636b 626f 78da 3d76 6965 7765  _checkbox.=viewe
-00000970: 725f 636f 6e66 6967 5f68 6967 686c 6967  r_config_highlig
-00000980: 6874 5f74 6f64 6f73 5f63 6865 636b 626f  ht_todos_checkbo
-00000990: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
-000009a0: 6372 6970 7469 6f6e da2d 7669 6577 6572  cription.-viewer
-000009b0: 5f63 6f6e 6669 675f 6f70 656e 5f6c 696e  _config_open_lin
-000009c0: 6b5f 636f 6e66 6972 6d61 7469 6f6e 5f63  k_confirmation_c
-000009d0: 6865 636b 626f 78da 4476 6965 7765 725f  heckbox.Dviewer_
-000009e0: 636f 6e66 6967 5f6f 7065 6e5f 6c69 6e6b  config_open_link
-000009f0: 5f63 6f6e 6669 726d 6174 696f 6e5f 6368  _confirmation_ch
-00000a00: 6563 6b62 6f78 5f61 6363 6573 7369 626c  eckbox_accessibl
-00000a10: 655f 6465 7363 7269 7074 696f 6eda 2576  e_description.%v
-00000a20: 6965 7765 725f 636f 6e66 6967 5f73 6176  iewer_config_sav
-00000a30: 655f 7265 736f 7572 6365 735f 6368 6563  e_resources_chec
-00000a40: 6b62 6f78 da3c 7669 6577 6572 5f63 6f6e  kbox.<viewer_con
-00000a50: 6669 675f 7361 7665 5f72 6573 6f75 7263  fig_save_resourc
-00000a60: 6573 5f63 6865 636b 626f 785f 6163 6365  es_checkbox_acce
-00000a70: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
-00000a80: 6f6e da1a 6169 5f63 6f6e 6669 675f 6f70  on..ai_config_op
-00000a90: 656e 6169 5f61 7069 5f6c 6162 656c da2f  enai_api_label./
-00000aa0: 6169 5f63 6f6e 6669 675f 6f70 656e 6169  ai_config_openai
-00000ab0: 5f61 7069 5f75 726c 5f69 6e70 7574 5f70  _api_url_input_p
-00000ac0: 6c61 6365 686f 6c64 6572 5f74 6578 74da  laceholder_text.
-00000ad0: 3561 695f 636f 6e66 6967 5f6f 7065 6e61  5ai_config_opena
-00000ae0: 695f 6170 695f 7572 6c5f 696e 7075 745f  i_api_url_input_
-00000af0: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
-00000b00: 6970 7469 6f6e da2f 6169 5f63 6f6e 6669  iption./ai_confi
-00000b10: 675f 6f70 656e 6169 5f61 7069 5f6b 6579  g_openai_api_key
-00000b20: 5f69 6e70 7574 5f70 6c61 6365 686f 6c64  _input_placehold
-00000b30: 6572 5f74 6578 74da 3561 695f 636f 6e66  er_text.5ai_conf
-00000b40: 6967 5f6f 7065 6e61 695f 6170 695f 6b65  ig_openai_api_ke
-00000b50: 795f 696e 7075 745f 6163 6365 7373 6962  y_input_accessib
-00000b60: 6c65 5f64 6573 6372 6970 7469 6f6e da2b  le_description.+
-00000b70: 6169 5f63 6f6e 6669 675f 6f70 656e 6169  ai_config_openai
-00000b80: 5f61 7069 5f73 7570 706f 7274 6564 5f6d  _api_supported_m
-00000b90: 6f64 656c 735f 6c61 6265 6cda 2f61 695f  odels_label./ai_
-00000ba0: 636f 6e66 6967 5f61 695f 6d6f 6465 6c5f  config_ai_model_
-00000bb0: 6e61 6d65 735f 636f 6d62 6f5f 706c 6163  names_combo_plac
-00000bc0: 6568 6f6c 6465 725f 7465 7874 da35 6169  eholder_text.5ai
-00000bd0: 5f63 6f6e 6669 675f 6169 5f6d 6f64 656c  _config_ai_model
-00000be0: 5f6e 616d 6573 5f63 6f6d 626f 5f61 6363  _names_combo_acc
-00000bf0: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
-00000c00: 696f 6eda 1461 695f 636f 6e66 6967 5f62  ion..ai_config_b
-00000c10: 6173 655f 6c61 6265 6cda 2261 695f 636f  ase_label."ai_co
-00000c20: 6e66 6967 5f62 6173 655f 7379 7374 656d  nfig_base_system
-00000c30: 5f70 726f 6d70 745f 6c61 6265 6cda 3261  _prompt_label.2a
-00000c40: 695f 636f 6e66 6967 5f62 6173 655f 7379  i_config_base_sy
-00000c50: 7374 656d 5f70 726f 6d70 745f 6564 6974  stem_prompt_edit
-00000c60: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
-00000c70: 74da 3861 695f 636f 6e66 6967 5f62 6173  t.8ai_config_bas
-00000c80: 655f 7379 7374 656d 5f70 726f 6d70 745f  e_system_prompt_
-00000c90: 6564 6974 5f61 6363 6573 7369 626c 655f  edit_accessible_
-00000ca0: 6465 7363 7269 7074 696f 6eda 2861 695f  description.(ai_
-00000cb0: 636f 6e66 6967 5f62 6173 655f 7265 7370  config_base_resp
-00000cc0: 6f6e 7365 5f6d 6178 5f74 6f6b 656e 735f  onse_max_tokens_
-00000cd0: 6c61 6265 6cda 3f61 695f 636f 6e66 6967  label.?ai_config
-00000ce0: 5f62 6173 655f 7265 7370 6f6e 7365 5f6d  _base_response_m
-00000cf0: 6178 5f74 6f6b 656e 735f 696e 7075 745f  ax_tokens_input_
-00000d00: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
-00000d10: 6970 7469 6f6e 4e29 01da 076c 6578 656d  iptionN)...lexem
-00000d20: 6573 a900 7231 0000 0072 3100 0000 fa4f  es..r1...r1....O
-00000d30: 2f55 7365 7273 2f76 6164 696b 7573 2f50  /Users/vadikus/P
-00000d40: 7963 6861 726d 5072 6f6a 6563 7473 2f6e  ycharmProjects/n
-00000d50: 6f74 6f6c 6f67 2d65 6469 746f 722f 6170  otolog-editor/ap
-00000d60: 702f 6c65 7865 6d65 732f 7365 2f73 6574  p/lexemes/se/set
-00000d70: 7469 6e67 735f 6469 616c 6f67 2e70 79da  tings_dialog.py.
-00000d80: 083c 6d6f 6475 6c65 3e04 0000 0073 5e00  .<module>....s^.
-00000d90: 0000 0202 0202 0201 0201 0201 0202 0201  ................
-00000da0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000db0: 0201 0201 0202 0201 0202 0202 0201 0201  ................
-00000dc0: 0202 0201 0201 0201 0201 0201 0202 0201  ................
-00000dd0: 0202 0202 0201 0201 0201 0201 0201 0201  ................
-00000de0: 0201 0202 0201 0201 0202 0201 0201 02c4  ................
+00000090: 5a00 6430 5300 2931 da07 4179 6172 6c61  Z.d0S.)1..Ayarla
+000000a0: 72da 054b 6170 6174 5a05 4765 6e65 6c75  r..KapatZ.Genelu
+000000b0: 0700 0000 4564 6974 c3b6 7275 1000 0000  ....Edit..ru....
+000000c0: 47c3 b672 c3bc 6e74 c3bc 6c65 7969 6369  G..r..nt..leyici
+000000d0: 750c 0000 0041 4920 4179 6172 6c61 72c4  u....AI Ayarlar.
+000000e0: b175 1200 0000 5579 6775 6c61 6d61 2061  .u....Uygulama a
+000000f0: 7961 726c 6172 c4b1 5a03 4469 6c75 0e00  yarlar..Z.Dilu..
+00000100: 0000 4269 7220 6469 6c20 7365 c3a7 696e  ..Bir dil se..in
+00000110: 7519 0000 0055 7967 756c 616d 616e c4b1  u....Uygulaman..
+00000120: 6e20 6172 6179 c3bc 7a20 6469 6c69 5a04  n aray..z diliZ.
+00000130: 5465 6d61 750f 0000 0042 6972 2074 656d  Temau....Bir tem
+00000140: 6120 7365 c3a7 696e 751c 0000 0055 7967  a se..inu....Uyg
+00000150: 756c 616d 616e c4b1 6e20 6172 6179 c3bc  ulaman..n aray..
+00000160: 7a20 7465 6d61 73c4 b175 0900 0000 416e  z temas..u....An
+00000170: 6120 4d65 6ec3 bc75 1400 0000 416e 6120  a Men..u....Ana 
+00000180: 4d65 6ec3 bc79 c3bc 2047 c3b6 7374 6572  Men..y.. G..ster
+00000190: 752e 0000 0055 7967 756c 616d 616e c4b1  u....Uygulaman..
+000001a0: 6e20 616e 6120 61c3 a7c4 b16c c4b1 7220  n ana a....l..r 
+000001b0: 6d65 6ec3 bc73 c3bc 6ec3 bc20 67c3 b673  men..s..n.. g..s
+000001c0: 7465 7275 1600 0000 5961 7ac4 b120 426f  teru....Yaz.. Bo
+000001d0: 7975 7475 3a20 7b73 697a 657d 7074 752c  yutu: {size}ptu,
+000001e0: 0000 0055 7967 756c 616d 616e c4b1 6e20  ...Uygulaman..n 
+000001f0: 6765 6e65 6c20 7961 7ac4 b120 626f 7975  genel yaz.. boyu
+00000200: 7475 6e75 2061 7961 726c 6179 c4b1 6e75  tunu ayarlay..nu
+00000210: 0e00 0000 4475 7275 6d20 c387 7562 75c4  ....Durum ..ubu.
+00000220: 9f75 7521 0000 0047 656e 656c 20c4 b06d  .uu!...Genel ..m
+00000230: 6c65 c3a7 2050 6f7a 6973 796f 6e75 6e75  le.. Pozisyonunu
+00000240: 2047 c3b6 7374 6572 7532 0000 0044 7572   G..steru2...Dur
+00000250: 756d 20c3 a775 6275 c49f 756e 6461 2067  um ..ubu..unda g
+00000260: 656e 656c 2069 6d6c 65c3 a720 706f 7a69  enel imle.. pozi
+00000270: 7379 6f6e 756e 7520 67c3 b673 7465 7275  syonunu g..steru
+00000280: 1900 0000 4564 6974 c3b6 7220 5961 70c4  ....Edit..r Yap.
+00000290: b16c 616e 64c4 b172 6d61 73c4 b175 1d00  .land..rmas..u..
+000002a0: 0000 5361 74c4 b172 204e 756d 6172 616c  ..Sat..r Numaral
+000002b0: 6172 c4b1 6ec4 b120 47c3 b673 7465 7275  ar..n.. G..steru
+000002c0: 2700 0000 4564 6974 c3b6 7264 6520 7361  '...Edit..rde sa
+000002d0: 74c4 b172 206e 756d 6172 616c 6172 c4b1  t..r numaralar..
+000002e0: 6ec4 b120 67c3 b673 7465 7275 2200 0000  n.. g..steru"...
+000002f0: 47c3 b672 c3bc 6e74 c3bc 6c65 7969 6369  G..r..nt..leyici
+00000300: 2059 6170 c4b1 6c61 6e64 c4b1 726d 6173   Yap..land..rmas
+00000310: c4b1 7529 0000 004d 6574 696e 2045 6d6f  ..u)...Metin Emo
+00000320: 6a69 6c65 7269 6e69 2047 7261 6669 6b6c  jilerini Grafikl
+00000330: 6572 6520 44c3 b66e c3bc c59f 74c3 bc72  ere D..n....t..r
+00000340: 7533 0000 004d 6574 696e 2065 6d6f 6a69  u3...Metin emoji
+00000350: 6c65 7269 6e69 2067 7261 6669 6b73 656c  lerini grafiksel
+00000360: 2074 656d 7369 6c6c 6572 6520 64c3 b66e   temsillere d..n
+00000370: c3bc c59f 74c3 bc72 7512 0000 0054 4f44  ....t..ru....TOD
+00000380: 4f27 6c61 72c4 b120 5675 7267 756c 617a  O'lar.. Vurgulaz
+00000390: 234d 6574 696e 6465 6b69 2054 4f44 4f20  #Metindeki TODO 
+000003a0: 6574 696b 6574 6c65 7269 6e69 2076 7572  etiketlerini vur
+000003b0: 6775 6c61 7529 0000 0042 61c4 9f6c 616e  gulau)...Ba..lan
+000003c0: 74c4 b16c 6172 c4b1 2041 c3a7 6d61 6461  t..lar.. A..mada
+000003d0: 6e20 c396 6e63 6520 4f6e 6179 20c4 b073  n ..nce Onay ..s
+000003e0: 7465 752b 0000 0042 61c4 9f6c 616e 74c4  teu+...Ba..lant.
+000003f0: b16c 6172 c4b1 2061 c3a7 6d61 6461 6e20  .lar.. a..madan 
+00000400: c3b6 6e63 6520 6f6e 6179 2069 7374 6579  ..nce onay istey
+00000410: 696e 7526 0000 0044 c4b1 c59f 2052 6573  inu&...D.... Res
+00000420: 696d 6c65 7269 2044 6973 6b74 6520 4f74  imleri Diskte Ot
+00000430: 6f6d 6174 696b 204b 6179 6465 7475 5800  omatik KaydetuX.
+00000440: 0000 44c4 b1c5 9f20 7265 7369 6d6c 6572  ..D.... resimler
+00000450: 696e 206b 6f70 7961 6c61 72c4 b16e c4b1  in kopyalar..n..
+00000460: 20c3 a765 7672 696d 64c4 b1c5 9fc4 b120   ..evrimd...... 
+00000470: 6572 69c5 9f69 6d20 69c3 a769 6e20 6469  eri..im i..in di
+00000480: 736b 6520 6f74 6f6d 6174 696b 206f 6c61  ske otomatik ola
+00000490: 7261 6b20 6b61 7964 6574 7a0a 4f70 656e  rak kaydetz.Open
+000004a0: 4149 2041 5049 7a07 4150 4920 5552 4c7a  AI APIz.API URLz
+000004b0: 114f 7065 6e41 4920 4150 4920 5552 4c27  .OpenAI API URL'
+000004c0: 7369 750d 0000 0041 5049 2061 6e61 6874  siu....API anaht
+000004d0: 6172 c4b1 7514 0000 004f 7065 6e41 4920  ar..u....OpenAI 
+000004e0: 4150 4920 616e 6168 7461 72c4 b17a 1444  API anahtar..z.D
+000004f0: 6573 7465 6b6c 656e 656e 206d 6f64 656c  esteklenen model
+00000500: 6c65 7275 0a00 0000 4d6f 6465 6c20 7365  leru....Model se
+00000510: c3a7 7523 0000 0053 65c3 a769 6c65 6269  ..u#...Se..ilebi
+00000520: 6c65 6365 6b20 6465 7374 656b 6c65 6e65  lecek desteklene
+00000530: 6e20 6d6f 6465 6c6c 6572 7a12 5465 6d65  n modellerz.Teme
+00000540: 6c20 5061 7261 6d65 7472 656c 6572 7511  l Parametreleru.
+00000550: 0000 0053 6973 7465 6d20 c4b0 7374 656d  ...Sistem ..stem
+00000560: 6369 7369 752f 0000 0048 6572 2069 7374  cisiu/...Her ist
+00000570: 656b 7465 6e20 c3b6 6e63 6520 6765 6c65  ekten ..nce gele
+00000580: 6e20 7465 6d65 6c20 7369 7374 656d 2069  n temel sistem i
+00000590: 7374 656d 6369 7369 7542 0000 0048 6572  stemcisiuB...Her
+000005a0: 2069 7374 656b 7465 6e20 c3b6 6e63 6520   istekten ..nce 
+000005b0: 6765 6c65 6e20 7465 6d65 6c20 7369 7374  gelen temel sist
+000005c0: 656d 2069 7374 656d 6369 7369 2e20 4275  em istemcisi. Bu
+000005d0: 2064 c3bc 7a20 6d65 7469 6e64 6972 2e75   d..z metindir.u
+000005e0: 1b00 0000 4d61 6b73 696d 756d 2059 616e  ....Maksimum Yan
+000005f0: c4b1 7420 546f 6b65 6e27 6c61 72c4 b175  ..t Token'lar..u
+00000600: 2e00 0000 5961 6ec4 b174 7461 2061 6cc4  ....Yan..tta al.
+00000610: b16e 6162 696c 6563 656b 206d 616b 7369  .nabilecek maksi
+00000620: 6d75 6d20 746f 6b65 6e20 7361 79c4 b173  mum token say..s
+00000630: c4b1 292f da0c 7769 6e64 6f77 5f74 6974  ..)/..window_tit
+00000640: 6c65 da0c 6275 7474 6f6e 5f63 6c6f 7365  le..button_close
+00000650: da0b 7461 625f 6765 6e65 7261 6cda 1174  ..tab_general..t
+00000660: 6162 5f65 6469 746f 725f 636f 6e66 6967  ab_editor_config
+00000670: da11 7461 625f 7669 6577 6572 5f63 6f6e  ..tab_viewer_con
+00000680: 6669 67da 0d74 6162 5f61 695f 636f 6e66  fig..tab_ai_conf
+00000690: 6967 da18 6765 6e65 7261 6c5f 6170 705f  ig..general_app_
+000006a0: 636f 6e66 6967 5f6c 6162 656c da1a 6765  config_label..ge
+000006b0: 6e65 7261 6c5f 6170 705f 6c61 6e67 7561  neral_app_langua
+000006c0: 6765 5f6c 6162 656c da2b 6765 6e65 7261  ge_label.+genera
+000006d0: 6c5f 6170 705f 6c61 6e67 7561 6765 5f63  l_app_language_c
+000006e0: 6f6d 626f 5f70 6c61 6365 686f 6c64 6572  ombo_placeholder
+000006f0: 5f74 6578 74da 3167 656e 6572 616c 5f61  _text.1general_a
+00000700: 7070 5f6c 616e 6775 6167 655f 636f 6d62  pp_language_comb
+00000710: 6f5f 6163 6365 7373 6962 6c65 5f64 6573  o_accessible_des
+00000720: 6372 6970 7469 6f6e da17 6765 6e65 7261  cription..genera
+00000730: 6c5f 6170 705f 7468 656d 655f 6c61 6265  l_app_theme_labe
+00000740: 6cda 2867 656e 6572 616c 5f61 7070 5f74  l.(general_app_t
+00000750: 6865 6d65 5f63 6f6d 626f 5f70 6c61 6365  heme_combo_place
+00000760: 686f 6c64 6572 5f74 6578 74da 2e67 656e  holder_text..gen
+00000770: 6572 616c 5f61 7070 5f74 6865 6d65 5f63  eral_app_theme_c
+00000780: 6f6d 626f 5f61 6363 6573 7369 626c 655f  ombo_accessible_
+00000790: 6465 7363 7269 7074 696f 6eda 1b67 656e  description..gen
+000007a0: 6572 616c 5f61 7070 5f6d 6169 6e5f 6d65  eral_app_main_me
+000007b0: 6e75 5f6c 6162 656c da1e 6765 6e65 7261  nu_label..genera
+000007c0: 6c5f 6170 705f 6d61 696e 5f6d 656e 755f  l_app_main_menu_
+000007d0: 6368 6563 6b62 6f78 da35 6765 6e65 7261  checkbox.5genera
+000007e0: 6c5f 6170 705f 6d61 696e 5f6d 656e 755f  l_app_main_menu_
+000007f0: 6368 6563 6b62 6f78 5f61 6363 6573 7369  checkbox_accessi
+00000800: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
+00000810: 1b67 656e 6572 616c 5f61 7070 5f66 6f6e  .general_app_fon
+00000820: 745f 7369 7a65 5f6c 6162 656c da33 6765  t_size_label.3ge
+00000830: 6e65 7261 6c5f 6170 705f 666f 6e74 5f73  neral_app_font_s
+00000840: 697a 655f 736c 6964 6572 5f61 6363 6573  ize_slider_acces
+00000850: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
+00000860: 6eda 1767 656e 6572 616c 5f73 7461 7475  n..general_statu
+00000870: 7362 6172 5f6c 6162 656c da36 6765 6e65  sbar_label.6gene
+00000880: 7261 6c5f 7374 6174 7573 6261 725f 7368  ral_statusbar_sh
+00000890: 6f77 5f67 6c6f 6261 6c5f 6375 7273 6f72  ow_global_cursor
+000008a0: 5f70 6f73 6974 696f 6e5f 6368 6563 6b62  _position_checkb
+000008b0: 6f78 da4d 6765 6e65 7261 6c5f 7374 6174  ox.Mgeneral_stat
+000008c0: 7573 6261 725f 7368 6f77 5f67 6c6f 6261  usbar_show_globa
+000008d0: 6c5f 6375 7273 6f72 5f70 6f73 6974 696f  l_cursor_positio
+000008e0: 6e5f 6368 6563 6b62 6f78 5f61 6363 6573  n_checkbox_acces
+000008f0: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
+00000900: 6eda 1365 6469 746f 725f 636f 6e66 6967  n..editor_config
+00000910: 5f6c 6162 656c da28 6564 6974 6f72 5f63  _label.(editor_c
+00000920: 6f6e 6669 675f 7368 6f77 5f6c 696e 655f  onfig_show_line_
+00000930: 6e75 6d62 6572 735f 6368 6563 6b62 6f78  numbers_checkbox
+00000940: da3f 6564 6974 6f72 5f63 6f6e 6669 675f  .?editor_config_
+00000950: 7368 6f77 5f6c 696e 655f 6e75 6d62 6572  show_line_number
+00000960: 735f 6368 6563 6b62 6f78 5f61 6363 6573  s_checkbox_acces
+00000970: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
+00000980: 6eda 1376 6965 7765 725f 636f 6e66 6967  n..viewer_config
+00000990: 5f6c 6162 656c da25 7669 6577 6572 5f63  _label.%viewer_c
+000009a0: 6f6e 6669 675f 7072 6f63 6573 735f 656d  onfig_process_em
+000009b0: 6f6a 6973 5f63 6865 636b 626f 78da 3c76  ojis_checkbox.<v
+000009c0: 6965 7765 725f 636f 6e66 6967 5f70 726f  iewer_config_pro
+000009d0: 6365 7373 5f65 6d6f 6a69 735f 6368 6563  cess_emojis_chec
+000009e0: 6b62 6f78 5f61 6363 6573 7369 626c 655f  kbox_accessible_
+000009f0: 6465 7363 7269 7074 696f 6eda 2676 6965  description.&vie
+00000a00: 7765 725f 636f 6e66 6967 5f68 6967 686c  wer_config_highl
+00000a10: 6967 6874 5f74 6f64 6f73 5f63 6865 636b  ight_todos_check
+00000a20: 626f 78da 3d76 6965 7765 725f 636f 6e66  box.=viewer_conf
+00000a30: 6967 5f68 6967 686c 6967 6874 5f74 6f64  ig_highlight_tod
+00000a40: 6f73 5f63 6865 636b 626f 785f 6163 6365  os_checkbox_acce
+00000a50: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+00000a60: 6f6e da2d 7669 6577 6572 5f63 6f6e 6669  on.-viewer_confi
+00000a70: 675f 6f70 656e 5f6c 696e 6b5f 636f 6e66  g_open_link_conf
+00000a80: 6972 6d61 7469 6f6e 5f63 6865 636b 626f  irmation_checkbo
+00000a90: 78da 4476 6965 7765 725f 636f 6e66 6967  x.Dviewer_config
+00000aa0: 5f6f 7065 6e5f 6c69 6e6b 5f63 6f6e 6669  _open_link_confi
+00000ab0: 726d 6174 696f 6e5f 6368 6563 6b62 6f78  rmation_checkbox
+00000ac0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
+00000ad0: 7269 7074 696f 6eda 2576 6965 7765 725f  ription.%viewer_
+00000ae0: 636f 6e66 6967 5f73 6176 655f 7265 736f  config_save_reso
+00000af0: 7572 6365 735f 6368 6563 6b62 6f78 da3c  urces_checkbox.<
+00000b00: 7669 6577 6572 5f63 6f6e 6669 675f 7361  viewer_config_sa
+00000b10: 7665 5f72 6573 6f75 7263 6573 5f63 6865  ve_resources_che
+00000b20: 636b 626f 785f 6163 6365 7373 6962 6c65  ckbox_accessible
+00000b30: 5f64 6573 6372 6970 7469 6f6e da1a 6169  _description..ai
+00000b40: 5f63 6f6e 6669 675f 6f70 656e 6169 5f61  _config_openai_a
+00000b50: 7069 5f6c 6162 656c da2f 6169 5f63 6f6e  pi_label./ai_con
+00000b60: 6669 675f 6f70 656e 6169 5f61 7069 5f75  fig_openai_api_u
+00000b70: 726c 5f69 6e70 7574 5f70 6c61 6365 686f  rl_input_placeho
+00000b80: 6c64 6572 5f74 6578 74da 3561 695f 636f  lder_text.5ai_co
+00000b90: 6e66 6967 5f6f 7065 6e61 695f 6170 695f  nfig_openai_api_
+00000ba0: 7572 6c5f 696e 7075 745f 6163 6365 7373  url_input_access
+00000bb0: 6962 6c65 5f64 6573 6372 6970 7469 6f6e  ible_description
+00000bc0: da2f 6169 5f63 6f6e 6669 675f 6f70 656e  ./ai_config_open
+00000bd0: 6169 5f61 7069 5f6b 6579 5f69 6e70 7574  ai_api_key_input
+00000be0: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
+00000bf0: 74da 3561 695f 636f 6e66 6967 5f6f 7065  t.5ai_config_ope
+00000c00: 6e61 695f 6170 695f 6b65 795f 696e 7075  nai_api_key_inpu
+00000c10: 745f 6163 6365 7373 6962 6c65 5f64 6573  t_accessible_des
+00000c20: 6372 6970 7469 6f6e da2b 6169 5f63 6f6e  cription.+ai_con
+00000c30: 6669 675f 6f70 656e 6169 5f61 7069 5f73  fig_openai_api_s
+00000c40: 7570 706f 7274 6564 5f6d 6f64 656c 735f  upported_models_
+00000c50: 6c61 6265 6cda 2f61 695f 636f 6e66 6967  label./ai_config
+00000c60: 5f61 695f 6d6f 6465 6c5f 6e61 6d65 735f  _ai_model_names_
+00000c70: 636f 6d62 6f5f 706c 6163 6568 6f6c 6465  combo_placeholde
+00000c80: 725f 7465 7874 da35 6169 5f63 6f6e 6669  r_text.5ai_confi
+00000c90: 675f 6169 5f6d 6f64 656c 5f6e 616d 6573  g_ai_model_names
+00000ca0: 5f63 6f6d 626f 5f61 6363 6573 7369 626c  _combo_accessibl
+00000cb0: 655f 6465 7363 7269 7074 696f 6eda 1461  e_description..a
+00000cc0: 695f 636f 6e66 6967 5f62 6173 655f 6c61  i_config_base_la
+00000cd0: 6265 6cda 2261 695f 636f 6e66 6967 5f62  bel."ai_config_b
+00000ce0: 6173 655f 7379 7374 656d 5f70 726f 6d70  ase_system_promp
+00000cf0: 745f 6c61 6265 6cda 3261 695f 636f 6e66  t_label.2ai_conf
+00000d00: 6967 5f62 6173 655f 7379 7374 656d 5f70  ig_base_system_p
+00000d10: 726f 6d70 745f 6564 6974 5f70 6c61 6365  rompt_edit_place
+00000d20: 686f 6c64 6572 5f74 6578 74da 3861 695f  holder_text.8ai_
+00000d30: 636f 6e66 6967 5f62 6173 655f 7379 7374  config_base_syst
+00000d40: 656d 5f70 726f 6d70 745f 6564 6974 5f61  em_prompt_edit_a
+00000d50: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00000d60: 7074 696f 6eda 2861 695f 636f 6e66 6967  ption.(ai_config
+00000d70: 5f62 6173 655f 7265 7370 6f6e 7365 5f6d  _base_response_m
+00000d80: 6178 5f74 6f6b 656e 735f 6c61 6265 6cda  ax_tokens_label.
+00000d90: 3f61 695f 636f 6e66 6967 5f62 6173 655f  ?ai_config_base_
+00000da0: 7265 7370 6f6e 7365 5f6d 6178 5f74 6f6b  response_max_tok
+00000db0: 656e 735f 696e 7075 745f 6163 6365 7373  ens_input_access
+00000dc0: 6962 6c65 5f64 6573 6372 6970 7469 6f6e  ible_description
+00000dd0: 4e29 01da 076c 6578 656d 6573 a900 7233  N)...lexemes..r3
+00000de0: 0000 0072 3300 0000 fa4c 2f55 7365 7273  ...r3....L/Users
+00000df0: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
+00000e00: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
+00000e10: 2d64 6576 2f61 7070 2f6c 6578 656d 6573  -dev/app/lexemes
+00000e20: 2f74 722f 7365 7474 696e 6773 5f64 6961  /tr/settings_dia
+00000e30: 6c6f 672e 7079 da08 3c6d 6f64 756c 653e  log.py..<module>
+00000e40: 0300 0000 735e 0000 0002 0202 0202 0102  ....s^..........
+00000e50: 0102 0102 0202 0102 0102 0102 0102 0102  ................
+00000e60: 0102 0102 0102 0102 0102 0102 0202 0102  ................
+00000e70: 0202 0202 0102 0102 0202 0102 0102 0102  ................
+00000e80: 0102 0102 0102 0102 0202 0202 0102 0102  ................
+00000e90: 0102 0102 0102 0102 0102 0202 0102 0102  ................
+00000ea0: 0202 0102 0102 c6                        .......
```

### Comparing `notolog-0.9.1b0/app/lexemes/se/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May  5 14:33:15 2024 UTC, .py size: 1220 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-00000000: 610d 0d0a 0000 0000 ab98 3766 c404 0000  a.........7f....
+00000000: 610d 0d0a 0000 0000 42a9 3566 d804 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
-00000050: 6411 9c11 5a00 6412 5300 2913 5a0b 5061  d...Z.d.S.).Z.Pa
-00000060: 7070 6572 736b 6f72 6775 1d00 0000 5669  pperskorgu....Vi
-00000070: 7361 2070 6170 7065 7273 6b6f 7267 656e  sa papperskorgen
-00000080: 7320 696e 6e65 68c3 a56c 6c73 0400 0000  s inneh..lls....
-00000090: f09f 92be 7304 0000 00f0 9f94 9273 0400  ....s........s..
-000000a0: 0000 f09f 9493 750d 0000 0056 6973 6e69  ......u....Visni
-000000b0: 6e67 736c c3a4 6765 7510 0000 0052 6564  ngsl..geu....Red
-000000c0: 6967 6572 696e 6773 6cc3 a467 6575 0e00  igeringsl..geu..
-000000d0: 0000 4bc3 a46c 6c6b 6f64 736c c3a4 6765  ..K..llkodsl..ge
-000000e0: da08 4d61 726b 646f 776e da04 4854 4d4c  ..Markdown..HTML
-000000f0: 7a13 7b65 6e63 7279 7074 696f 6e7d 207b  z.{encryption} {
-00000100: 6963 6f6e 7d5a 084f 736b 7964 6461 645a  icon}Z.OskyddadZ
-00000110: 094b 7279 7074 6572 6164 751d 0000 0072  .Krypteradu....r
-00000120: 6164 3a20 7b6c 696e 657d 20e2 8692 206b  ad: {line} ... k
-00000130: 6f6c 3a20 7b63 6f6c 756d 6e7d 7531 0000  ol: {column}u1..
-00000140: 0072 6164 3a20 7b6c 696e 657d 20e2 8692  .rad: {line} ...
-00000150: 206b 6f6c 3a20 7b63 6f6c 756d 6e7d 20e2   kol: {column} .
-00000160: 8692 2076 616c 3a20 7b73 656c 6563 7465  .. val: {selecte
-00000170: 647d 7531 0000 0072 6164 3a20 7b6c 696e  d}u1...rad: {lin
-00000180: 657d 20e2 8692 206b 6f6c 3a20 7b63 6f6c  e} ... kol: {col
-00000190: 756d 6e7d 20e2 8692 2070 6f73 3a20 7b70  umn} ... pos: {p
-000001a0: 6f73 6974 696f 6e7d 7545 0000 0072 6164  osition}uE...rad
-000001b0: 3a20 7b6c 696e 657d 20e2 8692 206b 6f6c  : {line} ... kol
-000001c0: 3a20 7b63 6f6c 756d 6e7d 20e2 8692 2070  : {column} ... p
-000001d0: 6f73 3a20 7b70 6f73 6974 696f 6e7d 20e2  os: {position} .
-000001e0: 8692 2076 616c 3a20 7b73 656c 6563 7465  .. val: {selecte
-000001f0: 647d 2911 da1a 7374 6174 7573 6261 725f  d})...statusbar_
-00000200: 6c69 7474 6572 5f62 696e 5f6c 6162 656c  litter_bin_label
-00000210: da24 7374 6174 7573 6261 725f 6c69 7474  .$statusbar_litt
-00000220: 6572 5f62 696e 5f61 6363 6573 7369 626c  er_bin_accessibl
-00000230: 655f 6e61 6d65 da1d 7374 6174 7573 6261  e_name..statusba
-00000240: 725f 7361 7665 5f70 726f 6772 6573 735f  r_save_progress_
-00000250: 6c61 6265 6cda 2b73 7461 7475 7362 6172  label.+statusbar
-00000260: 5f65 6e63 7279 7074 696f 6e5f 7379 6d62  _encryption_symb
-00000270: 6f6c 5f65 6e63 7279 7074 6564 5f6c 6162  ol_encrypted_lab
-00000280: 656c da2d 7374 6174 7573 6261 725f 656e  el.-statusbar_en
-00000290: 6372 7970 7469 6f6e 5f73 796d 626f 6c5f  cryption_symbol_
-000002a0: 756e 656e 6372 7970 7465 645f 6c61 6265  unencrypted_labe
-000002b0: 6cda 1e73 7461 7475 7362 6172 5f6d 6f64  l..statusbar_mod
-000002c0: 655f 6c61 6265 6c5f 6d6f 6465 5f76 6965  e_label_mode_vie
-000002d0: 77da 1e73 7461 7475 7362 6172 5f6d 6f64  w..statusbar_mod
-000002e0: 655f 6c61 6265 6c5f 6d6f 6465 5f65 6469  e_label_mode_edi
-000002f0: 74da 2073 7461 7475 7362 6172 5f6d 6f64  t. statusbar_mod
-00000300: 655f 6c61 6265 6c5f 6d6f 6465 5f73 6f75  e_label_mode_sou
-00000310: 7263 65da 2673 7461 7475 7362 6172 5f73  rce.&statusbar_s
-00000320: 6f75 7263 655f 6c61 6265 6c5f 736f 7572  ource_label_sour
-00000330: 6365 5f6d 6172 6b64 6f77 6eda 2273 7461  ce_markdown."sta
-00000340: 7475 7362 6172 5f73 6f75 7263 655f 6c61  tusbar_source_la
-00000350: 6265 6c5f 736f 7572 6365 5f68 746d 6cda  bel_source_html.
-00000360: 1a73 7461 7475 7362 6172 5f65 6e63 7279  .statusbar_encry
-00000370: 7074 696f 6e5f 6c61 6265 6cda 2b73 7461  ption_label.+sta
-00000380: 7475 7362 6172 5f65 6e63 7279 7074 696f  tusbar_encryptio
-00000390: 6e5f 6c61 6265 6c5f 656e 6372 7970 7469  n_label_encrypti
-000003a0: 6f6e 5f70 6c61 696e da2f 7374 6174 7573  on_plain./status
-000003b0: 6261 725f 656e 6372 7970 7469 6f6e 5f6c  bar_encryption_l
-000003c0: 6162 656c 5f65 6e63 7279 7074 696f 6e5f  abel_encryption_
-000003d0: 656e 6372 7970 7465 64da 1673 7461 7475  encrypted..statu
-000003e0: 7362 6172 5f63 7572 736f 725f 6c61 6265  sbar_cursor_labe
-000003f0: 6cda 1f73 7461 7475 7362 6172 5f63 7572  l..statusbar_cur
-00000400: 736f 725f 6c61 6265 6c5f 7365 6c65 6374  sor_label_select
-00000410: 6564 da22 7374 6174 7573 6261 725f 6375  ed."statusbar_cu
-00000420: 7273 6f72 5f6c 6162 656c 5f77 6974 685f  rsor_label_with_
-00000430: 676c 6f62 616c da2b 7374 6174 7573 6261  global.+statusba
-00000440: 725f 6375 7273 6f72 5f6c 6162 656c 5f73  r_cursor_label_s
-00000450: 656c 6563 7465 645f 7769 7468 5f67 6c6f  elected_with_glo
-00000460: 6261 6c4e 2901 da07 6c65 7865 6d65 73a9  balN)...lexemes.
-00000470: 0072 1500 0000 7215 0000 00fa 492f 5573  .r....r.....I/Us
-00000480: 6572 732f 7661 6469 6b75 732f 5079 6368  ers/vadikus/Pych
-00000490: 6172 6d50 726f 6a65 6374 732f 6e6f 746f  armProjects/noto
-000004a0: 6c6f 672d 6564 6974 6f72 2f61 7070 2f6c  log-editor/app/l
-000004b0: 6578 656d 6573 2f73 652f 7374 6174 7573  exemes/se/status
-000004c0: 6261 722e 7079 da08 3c6d 6f64 756c 653e  bar.py..<module>
-000004d0: 0300 0000 7322 0000 0002 0102 0202 0102  ....s"..........
-000004e0: 0102 0202 0102 0102 0202 0102 0202 0102  ................
-000004f0: 0102 0202 0102 0102 0102 ea              ...........
+00000050: 6411 9c11 5a00 6412 5300 2913 750c 0000  d...Z.d.S.).u...
+00000060: 00c3 87c3 b670 206b 7574 7573 7575 2000  .....p kutusuu .
+00000070: 0000 c387 c3b6 7020 6b75 7475 7375 2069  ......p kutusu i
+00000080: c3a7 6572 69c4 9f69 6e69 2067 c3b6 7374  ..eri..ini g..st
+00000090: 6572 7304 0000 00f0 9f92 be73 0400 0000  ers........s....
+000000a0: f09f 9492 7304 0000 00f0 9f94 9375 1300  ....s........u..
+000000b0: 0000 47c3 b672 c3bc 6e74 c3bc 6c65 6d65  ..G..r..nt..leme
+000000c0: 206d 6f64 7575 0f00 0000 44c3 bc7a 656e   moduu....D..zen
+000000d0: 6c65 6d65 206d 6f64 757a 0b4b 6179 6e61  leme moduz.Kayna
+000000e0: 6b20 6d6f 6475 da08 4d61 726b 646f 776e  k modu..Markdown
+000000f0: da04 4854 4d4c 7a13 7b65 6e63 7279 7074  ..HTMLz.{encrypt
+00000100: 696f 6e7d 207b 6963 6f6e 7d75 0400 0000  ion} {icon}u....
+00000110: 44c3 bc7a 7508 0000 00c5 9e69 6672 656c  D..zu......ifrel
+00000120: 6975 2100 0000 7361 74c4 b172 3a20 7b6c  iu!...sat..r: {l
+00000130: 696e 657d 20e2 8692 2073 c3bc 743a 207b  ine} ... s..t: {
+00000140: 636f 6c75 6d6e 7d75 3600 0000 7361 74c4  column}u6...sat.
+00000150: b172 3a20 7b6c 696e 657d 20e2 8692 2073  .r: {line} ... s
+00000160: c3bc 743a 207b 636f 6c75 6d6e 7d20 e286  ..t: {column} ..
+00000170: 9220 7365 c3a7 3a20 7b73 656c 6563 7465  . se..: {selecte
+00000180: 647d 7535 0000 0073 6174 c4b1 723a 207b  d}u5...sat..r: {
+00000190: 6c69 6e65 7d20 e286 9220 73c3 bc74 3a20  line} ... s..t: 
+000001a0: 7b63 6f6c 756d 6e7d 20e2 8692 206b 6f6e  {column} ... kon
+000001b0: 3a20 7b70 6f73 6974 696f 6e7d 754a 0000  : {position}uJ..
+000001c0: 0073 6174 c4b1 723a 207b 6c69 6e65 7d20  .sat..r: {line} 
+000001d0: e286 9220 73c3 bc74 3a20 7b63 6f6c 756d  ... s..t: {colum
+000001e0: 6e7d 20e2 8692 206b 6f6e 3a20 7b70 6f73  n} ... kon: {pos
+000001f0: 6974 696f 6e7d 20e2 8692 2073 65c3 a73a  ition} ... se..:
+00000200: 207b 7365 6c65 6374 6564 7d29 11da 1a73   {selected})...s
+00000210: 7461 7475 7362 6172 5f6c 6974 7465 725f  tatusbar_litter_
+00000220: 6269 6e5f 6c61 6265 6cda 2473 7461 7475  bin_label.$statu
+00000230: 7362 6172 5f6c 6974 7465 725f 6269 6e5f  sbar_litter_bin_
+00000240: 6163 6365 7373 6962 6c65 5f6e 616d 65da  accessible_name.
+00000250: 1d73 7461 7475 7362 6172 5f73 6176 655f  .statusbar_save_
+00000260: 7072 6f67 7265 7373 5f6c 6162 656c da2b  progress_label.+
+00000270: 7374 6174 7573 6261 725f 656e 6372 7970  statusbar_encryp
+00000280: 7469 6f6e 5f73 796d 626f 6c5f 656e 6372  tion_symbol_encr
+00000290: 7970 7465 645f 6c61 6265 6cda 2d73 7461  ypted_label.-sta
+000002a0: 7475 7362 6172 5f65 6e63 7279 7074 696f  tusbar_encryptio
+000002b0: 6e5f 7379 6d62 6f6c 5f75 6e65 6e63 7279  n_symbol_unencry
+000002c0: 7074 6564 5f6c 6162 656c da1e 7374 6174  pted_label..stat
+000002d0: 7573 6261 725f 6d6f 6465 5f6c 6162 656c  usbar_mode_label
+000002e0: 5f6d 6f64 655f 7669 6577 da1e 7374 6174  _mode_view..stat
+000002f0: 7573 6261 725f 6d6f 6465 5f6c 6162 656c  usbar_mode_label
+00000300: 5f6d 6f64 655f 6564 6974 da20 7374 6174  _mode_edit. stat
+00000310: 7573 6261 725f 6d6f 6465 5f6c 6162 656c  usbar_mode_label
+00000320: 5f6d 6f64 655f 736f 7572 6365 da26 7374  _mode_source.&st
+00000330: 6174 7573 6261 725f 736f 7572 6365 5f6c  atusbar_source_l
+00000340: 6162 656c 5f73 6f75 7263 655f 6d61 726b  abel_source_mark
+00000350: 646f 776e da22 7374 6174 7573 6261 725f  down."statusbar_
+00000360: 736f 7572 6365 5f6c 6162 656c 5f73 6f75  source_label_sou
+00000370: 7263 655f 6874 6d6c da1a 7374 6174 7573  rce_html..status
+00000380: 6261 725f 656e 6372 7970 7469 6f6e 5f6c  bar_encryption_l
+00000390: 6162 656c da2b 7374 6174 7573 6261 725f  abel.+statusbar_
+000003a0: 656e 6372 7970 7469 6f6e 5f6c 6162 656c  encryption_label
+000003b0: 5f65 6e63 7279 7074 696f 6e5f 706c 6169  _encryption_plai
+000003c0: 6eda 2f73 7461 7475 7362 6172 5f65 6e63  n./statusbar_enc
+000003d0: 7279 7074 696f 6e5f 6c61 6265 6c5f 656e  ryption_label_en
+000003e0: 6372 7970 7469 6f6e 5f65 6e63 7279 7074  cryption_encrypt
+000003f0: 6564 da16 7374 6174 7573 6261 725f 6375  ed..statusbar_cu
+00000400: 7273 6f72 5f6c 6162 656c da1f 7374 6174  rsor_label..stat
+00000410: 7573 6261 725f 6375 7273 6f72 5f6c 6162  usbar_cursor_lab
+00000420: 656c 5f73 656c 6563 7465 64da 2273 7461  el_selected."sta
+00000430: 7475 7362 6172 5f63 7572 736f 725f 6c61  tusbar_cursor_la
+00000440: 6265 6c5f 7769 7468 5f67 6c6f 6261 6cda  bel_with_global.
+00000450: 2b73 7461 7475 7362 6172 5f63 7572 736f  +statusbar_curso
+00000460: 725f 6c61 6265 6c5f 7365 6c65 6374 6564  r_label_selected
+00000470: 5f77 6974 685f 676c 6f62 616c 4e29 01da  _with_globalN)..
+00000480: 076c 6578 656d 6573 a900 7215 0000 0072  .lexemes..r....r
+00000490: 1500 0000 fa46 2f55 7365 7273 2f76 6164  .....F/Users/vad
+000004a0: 696b 7573 2f50 7963 6861 726d 5072 6f6a  ikus/PycharmProj
+000004b0: 6563 7473 2f6e 6f74 6f6c 6f67 2d64 6576  ects/notolog-dev
+000004c0: 2f61 7070 2f6c 6578 656d 6573 2f74 722f  /app/lexemes/tr/
+000004d0: 7374 6174 7573 6261 722e 7079 da08 3c6d  statusbar.py..<m
+000004e0: 6f64 756c 653e 0300 0000 7322 0000 0002  odule>....s"....
+000004f0: 0102 0202 0102 0102 0202 0102 0102 0202  ................
+00000500: 0102 0202 0102 0102 0202 0102 0102 0102  ................
+00000510: ea                                       .
```

### Comparing `notolog-0.9.1b0/app/lexemes/se/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/se/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/se/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/common.py` & `notolog-0.9.1b1/app/lexemes/se/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/main_menu.py` & `notolog-0.9.1b1/app/lexemes/se/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/se/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/statusbar.py` & `notolog-0.9.1b1/app/lexemes/se/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/se/toolbar.py` & `notolog-0.9.1b1/app/lexemes/se/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.1b1/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/tr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/tr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/common.py` & `notolog-0.9.1b1/app/lexemes/tr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/main_menu.py` & `notolog-0.9.1b1/app/lexemes/tr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/tr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/statusbar.py` & `notolog-0.9.1b1/app/lexemes/tr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/tr/toolbar.py` & `notolog-0.9.1b1/app/lexemes/tr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/ai_assistant.py` & `notolog-0.9.1b1/app/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.1b1/app/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/common.py` & `notolog-0.9.1b1/app/lexemes/zh/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/main_menu.py` & `notolog-0.9.1b1/app/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/settings_dialog.py` & `notolog-0.9.1b1/app/lexemes/zh/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/statusbar.py` & `notolog-0.9.1b1/app/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/lexemes/zh/toolbar.py` & `notolog-0.9.1b1/app/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/notolog_editor.py` & `notolog-0.9.1b1/app/notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/settings.py` & `notolog-0.9.1b1/app/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/text_block_data.py` & `notolog-0.9.1b1/app/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/theme.py` & `notolog-0.9.1b1/app/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/about_popup.py` & `notolog-0.9.1b1/app/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/ai_assistant.py` & `notolog-0.9.1b1/app/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/color_picker_dialog.py` & `notolog-0.9.1b1/app/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/common_dialog.py` & `notolog-0.9.1b1/app/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/enum_combo_box.py` & `notolog-0.9.1b1/app/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/file_system_model.py` & `notolog-0.9.1b1/app/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/line_numbers.py` & `notolog-0.9.1b1/app/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/rename_file_dialog.py` & `notolog-0.9.1b1/app/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/rotating_label.py` & `notolog-0.9.1b1/app/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/settings_dialog.py` & `notolog-0.9.1b1/app/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/sort_filter_proxy_model.py` & `notolog-0.9.1b1/app/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/statusbar.py` & `notolog-0.9.1b1/app/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/ui/toolbar.py` & `notolog-0.9.1b1/app/ui/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/view_decorator.py` & `notolog-0.9.1b1/app/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/view_processor.py` & `notolog-0.9.1b1/app/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/app/view_widget.py` & `notolog-0.9.1b1/app/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/docs/notolog-ui-settings.png` & `notolog-0.9.1b1/docs/notolog-ui-settings.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/main.py` & `notolog-0.9.1b1/main.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/notolog.egg-info/SOURCES.txt` & `notolog-0.9.1b1/notolog.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -291,14 +291,21 @@
 app/lexemes/la/ai_assistant.py
 app/lexemes/la/color_picker_dialog.py
 app/lexemes/la/common.py
 app/lexemes/la/main_menu.py
 app/lexemes/la/settings_dialog.py
 app/lexemes/la/statusbar.py
 app/lexemes/la/toolbar.py
+app/lexemes/nl/ai_assistant.py
+app/lexemes/nl/color_picker_dialog.py
+app/lexemes/nl/common.py
+app/lexemes/nl/main_menu.py
+app/lexemes/nl/settings_dialog.py
+app/lexemes/nl/statusbar.py
+app/lexemes/nl/toolbar.py
 app/lexemes/pt/ai_assistant.py
 app/lexemes/pt/color_picker_dialog.py
 app/lexemes/pt/common.py
 app/lexemes/pt/main_menu.py
 app/lexemes/pt/settings_dialog.py
 app/lexemes/pt/statusbar.py
 app/lexemes/pt/toolbar.py
@@ -312,21 +319,14 @@
 app/lexemes/se/ai_assistant.py
 app/lexemes/se/color_picker_dialog.py
 app/lexemes/se/common.py
 app/lexemes/se/main_menu.py
 app/lexemes/se/settings_dialog.py
 app/lexemes/se/statusbar.py
 app/lexemes/se/toolbar.py
-app/lexemes/se/__pycache__/ai_assistant.cpython-39.pyc
-app/lexemes/se/__pycache__/color_picker_dialog.cpython-39.pyc
-app/lexemes/se/__pycache__/common.cpython-39.pyc
-app/lexemes/se/__pycache__/main_menu.cpython-39.pyc
-app/lexemes/se/__pycache__/settings_dialog.cpython-39.pyc
-app/lexemes/se/__pycache__/statusbar.cpython-39.pyc
-app/lexemes/se/__pycache__/toolbar.cpython-39.pyc
 app/lexemes/tr/ai_assistant.py
 app/lexemes/tr/color_picker_dialog.py
 app/lexemes/tr/common.py
 app/lexemes/tr/main_menu.py
 app/lexemes/tr/settings_dialog.py
 app/lexemes/tr/statusbar.py
 app/lexemes/tr/toolbar.py
```

### Comparing `notolog-0.9.1b0/setup.py` & `notolog-0.9.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.1b0',
+    version='0.9.1b1',
     description='Notolog Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     license='MIT',
     py_modules=['main'],
```

### Comparing `notolog-0.9.1b0/tests/test_enc_helper.py` & `notolog-0.9.1b1/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_enc_password.py` & `notolog-0.9.1b1/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_file_header.py` & `notolog-0.9.1b1/tests/test_file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_html_view.py` & `notolog-0.9.1b1/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_lexemes.py` & `notolog-0.9.1b1/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_notolog_editor.py` & `notolog-0.9.1b1/tests/test_notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_settings.py` & `notolog-0.9.1b1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_text_block_data.py` & `notolog-0.9.1b1/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_theme_helper.py` & `notolog-0.9.1b1/tests/test_theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b0/tests/test_themes.py` & `notolog-0.9.1b1/tests/test_themes.py`

 * *Files identical despite different names*

