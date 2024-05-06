# Comparing `tmp/furo-2024.4.27.tar.gz` & `tmp/furo-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furo-2024.4.27.tar", last modified: Sat Apr 27 10:31:33 2024, max compression
+gzip compressed data, was "furo-2024.5.6.tar", last modified: Mon May  6 18:27:21 2024, max compression
```

## Comparing `furo-2024.4.27.tar` & `furo-2024.5.6.tar`

### file list

```diff
@@ -1,159 +1,161 @@
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:31:33.841484 furo-2024.4.27/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2024.4.27/CODE_OF_CONDUCT.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2024.4.27/LICENSE
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2024.4.27/README.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:38.977274 furo-2024.4.27/docs/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2024.4.27/docs/_static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2024.4.27/docs/_static/demo-dark.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2024.4.27/docs/_static/demo-light.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2024.4.27/docs/_static/demo.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2024.4.27/docs/_static/pied-piper-admonition.css
--rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2024.4.27/docs/_static/readthedocs-dummy.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    20299 2024-04-27 10:27:15.767102 furo-2024.4.27/docs/changelog.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2024-01-30 01:39:25.360621 furo-2024.4.27/docs/conf.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2024.4.27/docs/contributing/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2024.4.27/docs/contributing/design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2024.4.27/docs/contributing/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2024.4.27/docs/contributing/internals.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2024.4.27/docs/contributing/workflow.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.071941 furo-2024.4.27/docs/customisation/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2024.4.27/docs/customisation/announcement.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2024.4.27/docs/customisation/colors.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2024.4.27/docs/customisation/edit-button.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2024.4.27/docs/customisation/fonts.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5208 2023-12-10 17:13:56.071813 furo-2024.4.27/docs/customisation/footer.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3577 2023-05-20 06:29:53.184453 furo-2024.4.27/docs/customisation/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2024.4.27/docs/customisation/injecting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      965 2023-12-10 17:13:56.072135 furo-2024.4.27/docs/customisation/landing-page.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1799 2023-05-20 06:29:53.184857 furo-2024.4.27/docs/customisation/logo.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2024.4.27/docs/customisation/sidebar-title.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2024.4.27/docs/customisation/sidebar.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2024.4.27/docs/customisation/toc.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2024.4.27/docs/index.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.072300 furo-2024.4.27/docs/kitchen-sink/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2023-07-15 10:12:04.480639 furo-2024.4.27/docs/kitchen-sink/admonitions.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2024.4.27/docs/kitchen-sink/api.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8423 2023-12-10 17:13:56.072569 furo-2024.4.27/docs/kitchen-sink/blocks.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2024.4.27/docs/kitchen-sink/generic.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2024.4.27/docs/kitchen-sink/images.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2024.4.27/docs/kitchen-sink/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2024.4.27/docs/kitchen-sink/lists.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12941 2023-07-02 07:54:47.884930 furo-2024.4.27/docs/kitchen-sink/really-long.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2024.4.27/docs/kitchen-sink/sphinx-design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2024.4.27/docs/kitchen-sink/structure.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5200 2023-07-15 08:51:23.625580 furo-2024.4.27/docs/kitchen-sink/tables.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2024.4.27/docs/kitchen-sink/typography.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2023-11-06 23:31:33.042578 furo-2024.4.27/docs/license.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2024.4.27/docs/quickstart.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2024.4.27/docs/recommendations.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-09 14:47:21.361291 furo-2024.4.27/docs/reference/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2024.4.27/docs/reference/admonitions.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-04-09 14:47:21.362077 furo-2024.4.27/docs/reference/api.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2024.4.27/docs/reference/code-blocks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2024.4.27/docs/reference/hyperlinks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2350 2023-07-15 09:18:08.114960 furo-2024.4.27/docs/reference/images.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2024.4.27/docs/reference/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2024.4.27/docs/reference/lists.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2024.4.27/docs/reference/tables.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2024.4.27/docs/reference/tabs.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2024.4.27/docs/reference/text-formatting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2024.4.27/docs/requirements.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2024.4.27/docs/stability.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4973 2024-01-30 01:36:38.605170 furo-2024.4.27/noxfile.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)   123797 2024-04-27 10:23:07.241777 furo-2024.4.27/package-lock.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)      422 2024-04-27 10:23:07.242305 furo-2024.4.27/package.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2024.4.27/postcss.config.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1394 2024-02-16 11:01:24.612304 furo-2024.4.27/pyproject.toml
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2024.4.27/src/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:31:29.593578 furo-2024.4.27/src/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12715 2024-04-27 10:31:27.583826 furo-2024.4.27/src/furo/__init__.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1764 2024-02-14 21:57:37.106174 furo-2024.4.27/src/furo/_demo_module.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2024.4.27/src/furo/assets/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-01-30 01:36:38.279679 furo-2024.4.27/src/furo/assets/scripts/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2024-01-30 01:36:38.279984 furo-2024.4.27/src/furo/assets/scripts/furo.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12995 2023-12-10 17:13:56.072855 furo-2024.4.27/src/furo/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-10-11 08:48:22.837263 furo-2024.4.27/src/furo/assets/styles/
--rw-r--r--   0 pradyunsg   (501) staff       (20)    10020 2024-01-30 01:32:10.312810 furo-2024.4.27/src/furo/assets/styles/_scaffold.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2024.4.27/src/furo/assets/styles/_shame.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2024.4.27/src/furo/assets/styles/base/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2024.4.27/src/furo/assets/styles/base/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2024.4.27/src/furo/assets/styles/base/_print.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      387 2024-01-30 01:45:45.842282 furo-2024.4.27/src/furo/assets/styles/base/_screen-readers.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2024.4.27/src/furo/assets/styles/base/_theme.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1986 2024-01-30 00:59:20.983828 furo-2024.4.27/src/furo/assets/styles/base/_typography.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:07.243569 furo-2024.4.27/src/furo/assets/styles/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2024.4.27/src/furo/assets/styles/components/_footer.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2024.4.27/src/furo/assets/styles/components/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2024.4.27/src/furo/assets/styles/components/_search.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6138 2024-01-30 01:36:38.418271 furo-2024.4.27/src/furo/assets/styles/components/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1835 2024-04-27 10:23:07.243741 furo-2024.4.27/src/furo/assets/styles/components/_table_of_contents.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:07.243894 furo-2024.4.27/src/furo/assets/styles/content/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1945 2023-07-15 08:52:07.005777 furo-2024.4.27/src/furo/assets/styles/content/_admonitions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2282 2024-01-29 23:46:50.094207 furo-2024.4.27/src/furo/assets/styles/content/_api.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2024.4.27/src/furo/assets/styles/content/_blocks.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2024.4.27/src/furo/assets/styles/content/_captions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3231 2023-07-15 10:15:52.575334 furo-2024.4.27/src/furo/assets/styles/content/_code.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      856 2024-04-27 10:23:07.244044 furo-2024.4.27/src/furo/assets/styles/content/_footnotes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2024.4.27/src/furo/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2024.4.27/src/furo/assets/styles/content/_images.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2024.4.27/src/furo/assets/styles/content/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2024.4.27/src/furo/assets/styles/content/_indexes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2024.4.27/src/furo/assets/styles/content/_lists.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2024.4.27/src/furo/assets/styles/content/_math.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2024.4.27/src/furo/assets/styles/content/_misc.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2024.4.27/src/furo/assets/styles/content/_rubrics.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2024.4.27/src/furo/assets/styles/content/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2024.4.27/src/furo/assets/styles/content/_tables.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2024-01-30 01:32:03.792174 furo-2024.4.27/src/furo/assets/styles/content/_target.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2024.4.27/src/furo/assets/styles/extensions/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2024.4.27/src/furo/assets/styles/extensions/_copybutton.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2024.4.27/src/furo/assets/styles/extensions/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2024.4.27/src/furo/assets/styles/extensions/_readthedocs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-design.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-panels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2024.4.27/src/furo/assets/styles/furo-extensions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2024.4.27/src/furo/assets/styles/furo.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-02-14 21:56:45.361121 furo-2024.4.27/src/furo/assets/styles/variables/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2024.4.27/src/furo/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6676 2024-02-14 21:56:45.343355 furo-2024.4.27/src/furo/assets/styles/variables/_colors.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1411 2024-01-30 00:53:16.184455 furo-2024.4.27/src/furo/assets/styles/variables/_fonts.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2024.4.27/src/furo/assets/styles/variables/_icons.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2024.4.27/src/furo/assets/styles/variables/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2024.4.27/src/furo/assets/styles/variables/_layout.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2024.4.27/src/furo/assets/styles/variables/_spacing.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2023-04-13 21:46:27.392172 furo-2024.4.27/src/furo/navigation.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2425 2023-09-09 22:19:15.862233 furo-2024.4.27/src/furo/sphinxext.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2024.4.27/src/furo/theme/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:07.244176 furo-2024.4.27/src/furo/theme/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3245 2023-08-18 23:16:51.465972 furo-2024.4.27/src/furo/theme/furo/base.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2024.4.27/src/furo/theme/furo/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2024.4.27/src/furo/theme/furo/components/edit-this-page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2024.4.27/src/furo/theme/furo/domainindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2024.4.27/src/furo/theme/furo/genindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2024.4.27/src/furo/theme/furo/globaltoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2024.4.27/src/furo/theme/furo/layout.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2024.4.27/src/furo/theme/furo/localtoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)    11172 2024-01-30 00:59:20.037638 furo-2024.4.27/src/furo/theme/furo/page.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2024.4.27/src/furo/theme/furo/partials/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2024.4.27/src/furo/theme/furo/partials/_head_css_variables.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2024.4.27/src/furo/theme/furo/partials/icons.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      861 2024-04-27 10:23:07.244436 furo-2024.4.27/src/furo/theme/furo/search.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2024.4.27/src/furo/theme/furo/sidebar/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2024.4.27/src/furo/theme/furo/sidebar/brand.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2024.4.27/src/furo/theme/furo/sidebar/ethical-ads.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2024.4.27/src/furo/theme/furo/sidebar/navigation.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2024.4.27/src/furo/theme/furo/sidebar/rtd-versions.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2024.4.27/src/furo/theme/furo/sidebar/scroll-end.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2024.4.27/src/furo/theme/furo/sidebar/scroll-start.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2024.4.27/src/furo/theme/furo/sidebar/search.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2024.4.27/src/furo/theme/furo/sidebar/variant-selector.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2024.4.27/src/furo/theme/furo/static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2024.4.27/src/furo/theme/furo/static/.gitignore
--rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2024.4.27/src/furo/theme/furo/theme.conf
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-11-07 21:23:47.887523 furo-2024.4.27/tests/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       54 2023-09-01 22:33:56.796743 furo-2024.4.27/tests/requirements.txt
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-02-14 21:57:44.566705 furo-2024.4.27/tests/workflow/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3023 2023-09-01 22:31:55.015509 furo-2024.4.27/tests/workflow/test_sphinx_versions.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2024.4.27/webpack.config.js
--rw-r--r--   0        0        0     5917 1970-01-01 00:00:00.000000 furo-2024.4.27/PKG-INFO
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 18:27:21.370201 furo-2024.5.6/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2024.5.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2024.5.6/LICENSE
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2024.5.6/README.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 14:08:05.487807 furo-2024.5.6/docs/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2024.5.6/docs/_static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2024.5.6/docs/_static/demo-dark.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2024.5.6/docs/_static/demo-light.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2024.5.6/docs/_static/demo.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2024.5.6/docs/_static/pied-piper-admonition.css
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2024.5.6/docs/_static/readthedocs-dummy.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    20644 2024-05-06 18:25:37.923655 furo-2024.5.6/docs/changelog.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5245 2024-05-06 17:23:21.406119 furo-2024.5.6/docs/conf.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2024.5.6/docs/contributing/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2024.5.6/docs/contributing/design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2024.5.6/docs/contributing/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2024.5.6/docs/contributing/internals.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2024.5.6/docs/contributing/workflow.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 18:15:54.880411 furo-2024.5.6/docs/customisation/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      758 2024-05-06 17:40:50.305929 furo-2024.5.6/docs/customisation/announcement.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2241 2024-05-06 17:44:52.448893 furo-2024.5.6/docs/customisation/colors.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      277 2024-05-06 17:43:06.395135 furo-2024.5.6/docs/customisation/edit-button.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1135 2024-05-06 17:49:20.767890 furo-2024.5.6/docs/customisation/fonts.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5243 2024-05-06 17:50:51.575194 furo-2024.5.6/docs/customisation/footer.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4428 2024-05-06 18:17:34.689709 furo-2024.5.6/docs/customisation/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2024-05-06 17:51:56.629001 furo-2024.5.6/docs/customisation/injecting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      965 2024-05-06 17:52:08.742598 furo-2024.5.6/docs/customisation/landing-page.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1936 2024-05-06 17:54:22.210212 furo-2024.5.6/docs/customisation/logo.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2024.5.6/docs/customisation/sidebar-title.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4031 2024-05-06 17:55:59.910375 furo-2024.5.6/docs/customisation/sidebar.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2024-05-06 17:56:28.992991 furo-2024.5.6/docs/customisation/toc.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3687 2024-05-06 18:02:42.598569 furo-2024.5.6/docs/customisation/top-of-page-buttons.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2024-05-05 17:03:05.891498 furo-2024.5.6/docs/index.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 11:31:40.169585 furo-2024.5.6/docs/kitchen-sink/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2023-07-15 10:12:04.480639 furo-2024.5.6/docs/kitchen-sink/admonitions.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2024-05-06 14:05:30.522386 furo-2024.5.6/docs/kitchen-sink/api.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8423 2024-04-27 11:31:40.168895 furo-2024.5.6/docs/kitchen-sink/blocks.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2024.5.6/docs/kitchen-sink/generic.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2024.5.6/docs/kitchen-sink/images.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2024.5.6/docs/kitchen-sink/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2024.5.6/docs/kitchen-sink/lists.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12941 2024-04-27 11:31:40.169502 furo-2024.5.6/docs/kitchen-sink/really-long.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2024.5.6/docs/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2024.5.6/docs/kitchen-sink/structure.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5200 2024-04-27 11:31:40.169678 furo-2024.5.6/docs/kitchen-sink/tables.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2024.5.6/docs/kitchen-sink/typography.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2023-11-06 23:31:33.042578 furo-2024.5.6/docs/license.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2024.5.6/docs/quickstart.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2024.5.6/docs/recommendations.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 13:21:17.145344 furo-2024.5.6/docs/reference/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2024.5.6/docs/reference/admonitions.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2024-05-06 13:21:17.146823 furo-2024.5.6/docs/reference/api.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2024.5.6/docs/reference/code-blocks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2024.5.6/docs/reference/hyperlinks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2350 2024-04-27 11:31:40.170095 furo-2024.5.6/docs/reference/images.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2024.5.6/docs/reference/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2024.5.6/docs/reference/lists.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2024.5.6/docs/reference/tables.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2024.5.6/docs/reference/tabs.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2024.5.6/docs/reference/text-formatting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2024.5.6/docs/requirements.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2024.5.6/docs/stability.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4973 2024-04-27 11:31:40.170393 furo-2024.5.6/noxfile.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   123796 2024-05-06 16:45:44.923981 furo-2024.5.6/package-lock.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      421 2024-05-06 15:30:13.337672 furo-2024.5.6/package.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2024.5.6/postcss.config.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1409 2024-05-06 12:03:42.061000 furo-2024.5.6/pyproject.toml
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2024.5.6/src/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 18:27:15.308860 furo-2024.5.6/src/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12712 2024-05-06 18:27:12.625066 furo-2024.5.6/src/furo/__init__.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2040 2024-05-06 14:07:08.119028 furo-2024.5.6/src/furo/_demo_module.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2024.5.6/src/furo/assets/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 15:30:10.243462 furo-2024.5.6/src/furo/assets/scripts/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2024-05-06 15:30:10.243628 furo-2024.5.6/src/furo/assets/scripts/furo.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12995 2024-04-27 11:31:40.173080 furo-2024.5.6/src/furo/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 13:18:08.865127 furo-2024.5.6/src/furo/assets/styles/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    10110 2024-05-06 13:19:40.305162 furo-2024.5.6/src/furo/assets/styles/_scaffold.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2024.5.6/src/furo/assets/styles/_shame.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-05 21:17:57.456664 furo-2024.5.6/src/furo/assets/styles/base/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2024.5.6/src/furo/assets/styles/base/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2024.5.6/src/furo/assets/styles/base/_print.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      387 2024-04-27 11:31:40.173757 furo-2024.5.6/src/furo/assets/styles/base/_screen-readers.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1490 2024-05-05 21:17:57.456759 furo-2024.5.6/src/furo/assets/styles/base/_theme.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1986 2024-04-27 11:31:40.174109 furo-2024.5.6/src/furo/assets/styles/base/_typography.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 11:31:40.174544 furo-2024.5.6/src/furo/assets/styles/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2024.5.6/src/furo/assets/styles/components/_footer.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2024.5.6/src/furo/assets/styles/components/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2024.5.6/src/furo/assets/styles/components/_search.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6138 2024-04-27 11:31:40.174450 furo-2024.5.6/src/furo/assets/styles/components/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1835 2024-04-27 11:31:40.174760 furo-2024.5.6/src/furo/assets/styles/components/_table_of_contents.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 14:08:29.704234 furo-2024.5.6/src/furo/assets/styles/content/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1945 2024-05-06 14:01:15.498326 furo-2024.5.6/src/furo/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2835 2024-05-06 14:08:29.704675 furo-2024.5.6/src/furo/assets/styles/content/_api.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2024.5.6/src/furo/assets/styles/content/_blocks.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2024.5.6/src/furo/assets/styles/content/_captions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3231 2024-04-27 11:31:40.175674 furo-2024.5.6/src/furo/assets/styles/content/_code.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      856 2024-04-27 11:31:40.175987 furo-2024.5.6/src/furo/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2024.5.6/src/furo/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2024.5.6/src/furo/assets/styles/content/_images.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2024.5.6/src/furo/assets/styles/content/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2024.5.6/src/furo/assets/styles/content/_indexes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2024.5.6/src/furo/assets/styles/content/_lists.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2024.5.6/src/furo/assets/styles/content/_math.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2024.5.6/src/furo/assets/styles/content/_misc.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2024.5.6/src/furo/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2024.5.6/src/furo/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2024.5.6/src/furo/assets/styles/content/_tables.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2024-04-27 11:36:40.509388 furo-2024.5.6/src/furo/assets/styles/content/_target.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2024.5.6/src/furo/assets/styles/extensions/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2024.5.6/src/furo/assets/styles/extensions/_copybutton.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2024.5.6/src/furo/assets/styles/extensions/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2024.5.6/src/furo/assets/styles/extensions/_readthedocs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2024.5.6/src/furo/assets/styles/extensions/_sphinx-design.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2024.5.6/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2024.5.6/src/furo/assets/styles/extensions/_sphinx-panels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2024.5.6/src/furo/assets/styles/furo-extensions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2024.5.6/src/furo/assets/styles/furo.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 14:09:34.418590 furo-2024.5.6/src/furo/assets/styles/variables/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2024.5.6/src/furo/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     7251 2024-05-06 18:14:09.563404 furo-2024.5.6/src/furo/assets/styles/variables/_colors.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1411 2024-04-27 11:31:40.177036 furo-2024.5.6/src/furo/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2024.5.6/src/furo/assets/styles/variables/_icons.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2024.5.6/src/furo/assets/styles/variables/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2024.5.6/src/furo/assets/styles/variables/_layout.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2024.5.6/src/furo/assets/styles/variables/_spacing.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2024-04-27 11:37:36.254445 furo-2024.5.6/src/furo/navigation.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2425 2024-04-27 11:31:40.177473 furo-2024.5.6/src/furo/sphinxext.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2024.5.6/src/furo/theme/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 15:30:10.243760 furo-2024.5.6/src/furo/theme/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3245 2024-05-06 15:30:10.243843 furo-2024.5.6/src/furo/theme/furo/base.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 12:01:00.124051 furo-2024.5.6/src/furo/theme/furo/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      993 2024-05-06 16:45:38.667493 furo-2024.5.6/src/furo/theme/furo/components/edit-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1006 2024-05-06 16:48:02.660781 furo-2024.5.6/src/furo/theme/furo/components/view-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2024.5.6/src/furo/theme/furo/domainindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2024.5.6/src/furo/theme/furo/genindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2024.5.6/src/furo/theme/furo/globaltoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2024.5.6/src/furo/theme/furo/layout.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2024.5.6/src/furo/theme/furo/localtoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12444 2024-05-06 12:23:12.430817 furo-2024.5.6/src/furo/theme/furo/page.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-05 21:17:57.457004 furo-2024.5.6/src/furo/theme/furo/partials/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2024.5.6/src/furo/theme/furo/partials/_head_css_variables.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6872 2024-05-06 12:03:05.899110 furo-2024.5.6/src/furo/theme/furo/partials/icons.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      861 2024-04-27 11:31:40.179158 furo-2024.5.6/src/furo/theme/furo/search.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-05-06 15:30:10.244063 furo-2024.5.6/src/furo/theme/furo/sidebar/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2024.5.6/src/furo/theme/furo/sidebar/brand.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2024.5.6/src/furo/theme/furo/sidebar/ethical-ads.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2024.5.6/src/furo/theme/furo/sidebar/navigation.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2024-05-06 15:30:10.244108 furo-2024.5.6/src/furo/theme/furo/sidebar/rtd-versions.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2024.5.6/src/furo/theme/furo/sidebar/scroll-end.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2024.5.6/src/furo/theme/furo/sidebar/scroll-start.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2024.5.6/src/furo/theme/furo/sidebar/search.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2024.5.6/src/furo/theme/furo/sidebar/variant-selector.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2024.5.6/src/furo/theme/furo/static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2024.5.6/src/furo/theme/furo/static/.gitignore
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      596 2024-05-06 11:52:20.000864 furo-2024.5.6/src/furo/theme/furo/theme.conf
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 11:31:40.179380 furo-2024.5.6/tests/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       54 2024-04-27 11:31:40.179703 furo-2024.5.6/tests/requirements.txt
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 11:31:40.179761 furo-2024.5.6/tests/workflow/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3023 2024-04-27 11:31:40.180214 furo-2024.5.6/tests/workflow/test_sphinx_versions.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2024.5.6/webpack.config.js
+-rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 furo-2024.5.6/PKG-INFO
```

### Comparing `furo-2024.4.27/CODE_OF_CONDUCT.md` & `furo-2024.5.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/LICENSE` & `furo-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/README.md` & `furo-2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/_static/demo-dark.png` & `furo-2024.5.6/docs/_static/demo-dark.png`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/_static/demo-light.png` & `furo-2024.5.6/docs/_static/demo-light.png`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/_static/demo.png` & `furo-2024.5.6/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/_static/pied-piper-admonition.css` & `furo-2024.5.6/docs/_static/pied-piper-admonition.css`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/changelog.md` & `furo-2024.5.6/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 date "+## %Y.%m.%d -- {adjective} {colorname}" | pbcopy
 
 https://patternbasedwriting.com/elementary_writing_success/list-4800-adjectives/
 https://en.wikipedia.org/wiki/Lists_of_colors
 
 -->
 
+## 2024.05.06 -- Cheerful Cerulean
+
+- ✨ Add new custom icons for auto mode, reflecting the currently active theme.
+- ✨ Add a view this page button.
+- ✨ Add colours and highlighting to "version modified" API helpers.
+- ✨ Add release information to various customisation knobs.
+- Make all icons bigger and use a thinner stroke with them.
+
 ## 2024.04.27 -- Bold Burgundy
 
 - Add a skip to content link.
 - Add `--font-stack--headings`.
 - Add `:visited` colour and enforce uniform contrast between light/dark.
 - Add an offset of `:target` to reduce back-to-top overlap.
 - Improve dark mode colours.
```

### Comparing `furo-2024.4.27/docs/conf.py` & `furo-2024.5.6/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,23 @@
     # External stuff
     "myst_parser",
     "sphinx_copybutton",
     "sphinx_design",
     "sphinx_inline_tabs",
 ]
 
+# -- Options for Autodoc --------------------------------------------------------------
+
+autodoc_member_order = "bysource"
+autodoc_preserve_defaults = True
+
+# Keep the type hints outside the function signature, moving them to the
+# descriptions of the relevant function/methods.
+autodoc_typehints = "description"
+
 # -- Options for extlinks ----------------------------------------------------
 #
 
 extlinks = {
     "pypi": ("https://pypi.org/project/%s/", "%s"),
 }
```

#### html2text {}

```diff
@@ -7,45 +7,49 @@
 ---------- # project = "furo" copyright = "2020, Pradyun Gedam" author =
 "Pradyun Gedam" # -- General configuration ------------------------------------
 --------------- # extensions = [ # Sphinx's own extensions
 "sphinx.ext.autodoc", "sphinx.ext.extlinks", "sphinx.ext.intersphinx",
 "sphinx.ext.mathjax", "sphinx.ext.todo", "sphinx.ext.viewcode", # Our custom
 extension, only meant for Furo's own documentation. "furo.sphinxext", #
 External stuff "myst_parser", "sphinx_copybutton", "sphinx_design",
-"sphinx_inline_tabs", ] # -- Options for extlinks -----------------------------
------------------------ # extlinks = { "pypi": ("https://pypi.org/project/%s/",
-"%s"), } # -- Options for intersphinx -----------------------------------------
--------- # intersphinx_mapping = { "python": ("https://docs.python.org/3",
-None), "sphinx": ("https://www.sphinx-doc.org/en/master", None), } # -- Options
-for TODOs ------------------------------------------------------- #
-todo_include_todos = True # -- Options for Markdown files ---------------------
-------------------------- # myst_enable_extensions = [ "colon_fence",
-"deflist", ] myst_heading_anchors = 3 # -- Options for HTML output ------------
-------------------------------------- # html_theme = "furo" html_title = "Furo"
-language = "en" html_static_path = ["_static"] html_css_files = ["pied-piper-
-admonition.css"] html_theme_options: Dict[str, Any] = { "footer_icons": [
-{ "name": "GitHub", "url": "https://github.com/pradyunsg/furo", "html": """
-""", "class": "", }, ], "source_repository": "https://github.com/pradyunsg/
-furo/", "source_branch": "main", "source_directory": "docs/", } if
-"READTHEDOCS" in os.environ: html_theme_options["announcement"] = ( "This
-documentation is hosted on Read the Docs only for testing. Please use " "_t_h_e
-_m_a_i_n_ _d_o_c_u_m_e_n_t_a_t_i_o_n instead." ) # -- Options for theme development -------------
------------------------------- # Make sure these are all set to the default
-values. html_js_files = [] html_context: Dict[str, Any] = {} # html_show_sphinx
-= False # html_show_copyright = False # html_last_updated_fmt = "" RTD_TESTING
-= False if RTD_TESTING or "FURO_RTD_TESTING" in os.environ: del
-html_theme_options["footer_icons"] html_css_files += [ "https://
-assets.readthedocs.org/static/css/readthedocs-doc-embed.css", "https://
-assets.readthedocs.org/static/css/badge_only.css", ] html_js_files +=
-[ "readthedocs-dummy.js", "https://assets.readthedocs.org/static/javascript/
-readthedocs-doc-embed.js", ] html_context["READTHEDOCS"] = True html_context
-["current_version"] = "latest" html_context["conf_py_path"] = "/docs/
-" html_context["display_github"] = True html_context["github_user"] =
-"pradyunsg" html_context["github_repo"] = "furo" html_context["github_version"]
-= "main" html_context["slug"] = "furo" FONT_AWESOME_TESTING = False if
-FONT_AWESOME_TESTING: html_css_files += [ "https://cdnjs.cloudflare.com/ajax/
-libs/font-awesome/6.0.0/css/fontawesome.min.css", "https://
-cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/solid.min.css", "https://
-cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/brands.min.css", ]
-html_theme_options["footer_icons"] = [ { "name": "GitHub", "url": "https://
-github.com/pradyunsg/furo", "html": "", "class": "fa-brands fa-solid fa-github
-fa-2x", }, ]
+"sphinx_inline_tabs", ] # -- Options for Autodoc ------------------------------
+-------------------------------- autodoc_member_order = "bysource"
+autodoc_preserve_defaults = True # Keep the type hints outside the function
+signature, moving them to the # descriptions of the relevant function/methods.
+autodoc_typehints = "description" # -- Options for extlinks -------------------
+--------------------------------- # extlinks = { "pypi": ("https://pypi.org/
+project/%s/", "%s"), } # -- Options for intersphinx ---------------------------
+---------------------- # intersphinx_mapping = { "python": ("https://
+docs.python.org/3", None), "sphinx": ("https://www.sphinx-doc.org/en/master",
+None), } # -- Options for TODOs -----------------------------------------------
+-------- # todo_include_todos = True # -- Options for Markdown files ----------
+------------------------------------ # myst_enable_extensions =
+[ "colon_fence", "deflist", ] myst_heading_anchors = 3 # -- Options for HTML
+output ------------------------------------------------- # html_theme = "furo"
+html_title = "Furo" language = "en" html_static_path = ["_static"]
+html_css_files = ["pied-piper-admonition.css"] html_theme_options: Dict[str,
+Any] = { "footer_icons": [ { "name": "GitHub", "url": "https://github.com/
+pradyunsg/furo", "html": """ """, "class": "", }, ], "source_repository":
+"https://github.com/pradyunsg/furo/", "source_branch": "main",
+"source_directory": "docs/", } if "READTHEDOCS" in os.environ:
+html_theme_options["announcement"] = ( "This documentation is hosted on Read
+the Docs only for testing. Please use " "_t_h_e_ _m_a_i_n_ _d_o_c_u_m_e_n_t_a_t_i_o_n instead." ) # -
+- Options for theme development ------------------------------------------- #
+Make sure these are all set to the default values. html_js_files = []
+html_context: Dict[str, Any] = {} # html_show_sphinx = False #
+html_show_copyright = False # html_last_updated_fmt = "" RTD_TESTING = False if
+RTD_TESTING or "FURO_RTD_TESTING" in os.environ: del html_theme_options
+["footer_icons"] html_css_files += [ "https://assets.readthedocs.org/static/
+css/readthedocs-doc-embed.css", "https://assets.readthedocs.org/static/css/
+badge_only.css", ] html_js_files += [ "readthedocs-dummy.js", "https://
+assets.readthedocs.org/static/javascript/readthedocs-doc-embed.js", ]
+html_context["READTHEDOCS"] = True html_context["current_version"] = "latest"
+html_context["conf_py_path"] = "/docs/" html_context["display_github"] = True
+html_context["github_user"] = "pradyunsg" html_context["github_repo"] = "furo"
+html_context["github_version"] = "main" html_context["slug"] = "furo"
+FONT_AWESOME_TESTING = False if FONT_AWESOME_TESTING: html_css_files +=
+[ "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/
+fontawesome.min.css", "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/
+6.0.0/css/solid.min.css", "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/
+6.0.0/css/brands.min.css", ] html_theme_options["footer_icons"] = [ { "name":
+"GitHub", "url": "https://github.com/pradyunsg/furo", "html": "", "class": "fa-
+brands fa-solid fa-github fa-2x", }, ]
```

### Comparing `furo-2024.4.27/docs/contributing/design.md` & `furo-2024.5.6/docs/contributing/design.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/contributing/index.md` & `furo-2024.5.6/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/contributing/internals.md` & `furo-2024.5.6/docs/contributing/internals.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/contributing/workflow.md` & `furo-2024.5.6/docs/contributing/workflow.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/customisation/announcement.md` & `furo-2024.5.6/docs/customisation/announcement.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Adding an announcement banner
 
+```{versionadded} 2020.12.28.beta22
+
+```
+
 Furo makes it fairly straightforward to add a site-wide announcement (AKA top banner). The announcement is added to the top of all pages on the website.
 
 This is done by setting `announcement` key in [`html_theme_options`][sphinx-html_theme_options] in your `conf.py` file. The value of this key is HTML, which is included as-is into the page.
 
 ```python
 html_theme_options = {
     "announcement": "<em>Important</em> announcement!",
```

### Comparing `furo-2024.4.27/docs/customisation/colors.md` & `furo-2024.5.6/docs/customisation/colors.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changing colors
 
+```{versionadded} 2020.11.14.beta16
+
+```
+
 Furo allows customising colors to fit your brand's identity, by using CSS variables. These can be declared directly in [`html_theme_options`][sphinx-html_theme_options], in your `conf.py`.
 
 ## How light and dark mode work
 
 Furo is in light mode by default, switching to the dark mode when requested by the user's browser (through `prefers-color-scheme: dark`).
 
 As a consequence of this design, the dark mode inherits the variable definitions from the light mode, only overriding specific values to adapt the theme. While the mechanism for switching between light/dark mode is not configurable, the exact CSS variable definitions used in this process can be configured.
```

### Comparing `furo-2024.4.27/docs/customisation/footer.md` & `furo-2024.5.6/docs/customisation/footer.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changing footer icons
 
+```{versionadded} 2022.02.14
+
+```
+
 Furo allows customising the icons that are presented in the page footer. These icons can be used to link to relevant resources for your project and documentation.
 
 ```{admonition} Unstable, seeking feedback
 :class: caution
 
 This feature is treated as "unstable" under Furo's {doc}`../stability`.
```

### Comparing `furo-2024.4.27/docs/customisation/index.md` & `furo-2024.5.6/docs/customisation/index.md`

 * *Files 25% similar despite different names*

```diff
@@ -5,36 +5,40 @@
 This section serves to guide the user with customising Furo-based documentation. This page lists all the theme-specific customisations, as provided by this theme. Other pages in this section provide guidance for making specific customisations when using Sphinx with Furo.
 
 ```{toctree}
 :hidden:
 
 logo
 announcement
-edit-button
+top-of-page-buttons
 colors
 fonts
 footer
 landing-page
 sidebar
 sidebar-title
 toc
 injecting
 ```
 
 ## Theme options
 
-[`html_theme_options`][sphinx-html_theme_options] in `conf.py` is used for customisations that affect the entire documentation. This is for stuff like fonts and colors.
-
-```{note}
-Note that only the configuration options listed here are supported (not the ones inherited from the built-in `basic` Sphinx theme).
-```
+[`html_theme_options`][sphinx-html_theme_options] in `conf.py` is used for customisations that affect the entire documentation. This is for stuff like fonts and colors. While this theme inherits some options from the built-in `basic` Sphinx theme, only the ones documented here are supported.
 
 (css-variables)=
 
-### `light_css_variables`/`dark_css_variables`
+### `light_css_variables` / `dark_css_variables`
+
+```{versionadded} 2020.08.14.beta5
+
+```
+
+```{versionchanged} 2020.11.01.beta14
+Support for dark mode involved replacing `css_variables` with `light_css_variables` / `dark_css_variables`.
+```
 
 Furo makes extensive use of [CSS variables][css-variables]. These can be overridden by the user and are used for stylizing nearly all elements of the documentation. {doc}`colors` contains important details of how these variables are used.
 
 Setting `*_css_variables` is the recommended mechanism to override Furo's default values for these variables.
 
 ```python
 html_theme_options = {
@@ -50,59 +54,106 @@
 Typos in the `*_css_variables` dictionary are silently ignored, and do not raise any errors or warnings. Double check that your spellings and values are correct and valid.
 ```
 
 (sidebar_hide_name)=
 
 ### `sidebar_hide_name`
 
+```{versionadded} 2020.08.14.beta5
+
+```
+
 Controls whether you see the project's name in the sidebar of the documentation. This is useful when you only want to show your documentation's logo in the sidebar. The default is `False`.
 
 ```python
 html_theme_options = {
     "sidebar_hide_name": True,
 }
 ```
 
 ### `navigation_with_keys`
 
+```{versionadded} 2020.11.01.beta14
+
+```
+
 Controls whether the user can navigate the documentation using the keyboard’s left and right arrows. The default is `False`.
 
 ```python
 html_theme_options = {
     "navigation_with_keys": True,
 }
 ```
 
 (top_of_page_button)=
 
 ### `top_of_page_button`
 
+```{versionadded} 2022.06.04
+
+```
+
+```{deprecated} 2024.05.06
+This will be removed after 2024-11-01. Use `top_of_page_buttons` instead.
+```
+
 Controls which button is shown on the top of the page. The only supported values are `"edit"` (the default) and `None`.
 
 ```python
 html_theme_options = {
     "top_of_page_button": "edit",
 }
 ```
 
+(top_of_page_buttons)=
+
+### `top_of_page_buttons`
+
+```{versionadded} 2024.05.06
+
+```
+
+Controls which buttons are shown on the top of the page. This is a list which can be empty or contain one-or-more of the following values:
+
+- `"edit"`
+- `"view"`
+
+```python
+html_theme_options = {
+    "top_of_page_buttons": ["view", "edit"],
+}
+```
+
 ### `announcement`
 
+```{versionadded} 2020.12.28.beta22
+
+```
+
 Add a site-wide announcement, to the top of every page when set. See {doc}`./announcement` for the details.
 
 ### `footer_icons`
 
+```{versionadded} 2022.02.14
+
+```
+
 Changes the icons presented in the site footer. See {doc}`./footer` for the details.
 
 ## Page specific tweaks
 
 [File-Wide metadata][sphinx-file-wide-metadata] is used for per-page customisation, primarily for controlling which UI elements are presented.
 
 ### `hide-toc`
 
-The “Contents” sidebar is automatically hidden for any pages that don’t have any inner headings. It is possible to hide it even when a page has inner headings, by setting `hide-toc` at the page level. See {doc}`./toc` for an example.
+```{versionadded} 2020.08.14.beta5
+
+```
+
+The "Contents" sidebar is automatically hidden for any pages that don’t have any inner headings. It is possible to hide it even when a page has inner headings, by setting `hide-toc` at the page level. See {doc}`./toc` for an example.
 
 ## Custom CSS files
 
 If you want more control than what is provided by the above theme options, see {doc}`injecting`.
 
 [css-variables]: https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties
 [sphinx-html_theme_options]: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_theme_options
```

### Comparing `furo-2024.4.27/docs/customisation/injecting.md` & `furo-2024.5.6/docs/customisation/injecting.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/customisation/landing-page.md` & `furo-2024.5.6/docs/customisation/landing-page.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/customisation/logo.md` & `furo-2024.5.6/docs/customisation/logo.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Adding a logo
 
+```{versionadded} 2020.08.14.beta5
+
+```
+
+```{versionchanged} 2020.11.10.beta15
+Support for different logos for light and dark mode.
+```
+
 Logos are a point of recognition and an important part of branding. Furo supports adding your project's logo at the top of the navigational (left) sidebar, like most other Sphinx themes.
 
 ## Same logo for light and dark mode
 
 Furo supports the standard Sphinx mechanism to add your project's logo in the documentation, using the [`html_logo`][sphinx-html_logo] variable in `conf.py`.
 
 ```python
```

### Comparing `furo-2024.4.27/docs/customisation/sidebar.md` & `furo-2024.5.6/docs/customisation/sidebar.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changing sidebar elements
 
+```{versionadded} 2020.11.15.beta17
+
+```
+
 Furo supports customising the elements that show up in the navigational sidebar (left). This is to provide documentation authors who are willing to work with HTML/CSS to change and tweak how the sidebar looks.
 
 ```{admonition} Unstable
 :class: caution
 
 This customisation considered "unstable" under Furo's {doc}`../stability`.
```

### Comparing `furo-2024.4.27/docs/customisation/toc.md` & `furo-2024.5.6/docs/customisation/toc.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Hiding Contents sidebar
 
+```{versionadded} 2020.08.14.beta5
+
+```
+
 Furo supports hiding the "Contents" sidebar (right), and does so automatically for any pages that don't have any inner headings.
 
 To explicitly hide it on a specific page, `hide-toc` can be set in the [File-Wide metadata][sphinx-file-wide-metadata] for that page.
 
 ````{tab} reStructuredText
 ```rst
 :hide-toc:
```

### Comparing `furo-2024.4.27/docs/kitchen-sink/admonitions.rst` & `furo-2024.5.6/docs/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/api.rst` & `furo-2024.5.6/docs/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/blocks.rst` & `furo-2024.5.6/docs/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/generic.rst` & `furo-2024.5.6/docs/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/images.rst` & `furo-2024.5.6/docs/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/index.md` & `furo-2024.5.6/docs/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/lists.rst` & `furo-2024.5.6/docs/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/really-long.md` & `furo-2024.5.6/docs/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/sphinx-design.md` & `furo-2024.5.6/docs/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/structure.rst` & `furo-2024.5.6/docs/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/tables.rst` & `furo-2024.5.6/docs/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/kitchen-sink/typography.rst` & `furo-2024.5.6/docs/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/recommendations.md` & `furo-2024.5.6/docs/recommendations.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/admonitions.md` & `furo-2024.5.6/docs/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/api.md` & `furo-2024.5.6/docs/reference/api.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/code-blocks.md` & `furo-2024.5.6/docs/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/hyperlinks.md` & `furo-2024.5.6/docs/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/images.md` & `furo-2024.5.6/docs/reference/images.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/index.md` & `furo-2024.5.6/docs/reference/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/lists.md` & `furo-2024.5.6/docs/reference/lists.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/tables.md` & `furo-2024.5.6/docs/reference/tables.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/tabs.md` & `furo-2024.5.6/docs/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/reference/text-formatting.md` & `furo-2024.5.6/docs/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/docs/stability.md` & `furo-2024.5.6/docs/stability.md`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/noxfile.py` & `furo-2024.5.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/package-lock.json` & `furo-2024.5.6/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995714327989719%*

 * *Differences: {"'packages'": "{'': {'devDependencies': {'css-loader': '^7.1.1', 'mini-css-extract-plugin': "*

 * *               "'^2.9.0', 'sass': '^1.76.0', 'sass-loader': '^14.2.1', 'style-loader': '^4.0.0'}}, "*

 * *               "'node_modules/css-loader': {'version': '7.1.1', 'resolved': "*

 * *               "'https://registry.npmjs.org/css-loader/-/css-loader-7.1.1.tgz', 'integrity': "*

 * *               "'sha512-OxIR5P2mjO1PSXk44bWuQ8XtMK4dpEqpIyERCx3ewOo3I8EmbcxMPUc5ScLtQfgXtOojoMv57So4V/C02HQLsw==', "*

 * *               "'dependenc […]*

```diff
@@ -1,22 +1,22 @@
 {
     "lockfileVersion": 3,
     "name": "furo",
     "packages": {
         "": {
             "devDependencies": {
                 "autoprefixer": "^10.4.19",
-                "css-loader": "^6.10.0",
+                "css-loader": "^7.1.1",
                 "css-minimizer-webpack-plugin": "^6.0.0",
-                "mini-css-extract-plugin": "^2.8.1",
+                "mini-css-extract-plugin": "^2.9.0",
                 "normalize.css": "^8.0.1",
                 "postcss-loader": "^8.1.1",
-                "sass": "^1.72.0",
-                "sass-loader": "^14.1.1",
-                "style-loader": "^3.3.2",
+                "sass": "^1.76.0",
+                "sass-loader": "^14.2.1",
+                "style-loader": "^4.0.0",
                 "webpack": "^5.91.0",
                 "webpack-cli": "^5.0.1"
             }
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
                 "@babel/highlight": "^7.23.4",
@@ -997,44 +997,44 @@
             "resolved": "https://registry.npmjs.org/css-declaration-sorter/-/css-declaration-sorter-7.1.1.tgz",
             "version": "7.1.1"
         },
         "node_modules/css-loader": {
             "dependencies": {
                 "icss-utils": "^5.1.0",
                 "postcss": "^8.4.33",
-                "postcss-modules-extract-imports": "^3.0.0",
-                "postcss-modules-local-by-default": "^4.0.4",
-                "postcss-modules-scope": "^3.1.1",
+                "postcss-modules-extract-imports": "^3.1.0",
+                "postcss-modules-local-by-default": "^4.0.5",
+                "postcss-modules-scope": "^3.2.0",
                 "postcss-modules-values": "^4.0.0",
                 "postcss-value-parser": "^4.2.0",
                 "semver": "^7.5.4"
             },
             "dev": true,
             "engines": {
-                "node": ">= 12.13.0"
+                "node": ">= 18.12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-LTSA/jWbwdMlk+rhmElbDR2vbtQoTBPr7fkJE+mxrHj+7ru0hUmHafDRzWIjIHTwpitWVaqY2/UWGRca3yUgRw==",
+            "integrity": "sha512-OxIR5P2mjO1PSXk44bWuQ8XtMK4dpEqpIyERCx3ewOo3I8EmbcxMPUc5ScLtQfgXtOojoMv57So4V/C02HQLsw==",
             "peerDependencies": {
                 "@rspack/core": "0.x || 1.x",
-                "webpack": "^5.0.0"
+                "webpack": "^5.27.0"
             },
             "peerDependenciesMeta": {
                 "@rspack/core": {
                     "optional": true
                 },
                 "webpack": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.10.0.tgz",
-            "version": "6.10.0"
+            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-7.1.1.tgz",
+            "version": "7.1.1"
         },
         "node_modules/css-minimizer-webpack-plugin": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "^0.3.21",
                 "cssnano": "^6.0.3",
                 "jest-worker": "^29.7.0",
                 "postcss": "^8.4.33",
@@ -1896,20 +1896,20 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-/1HDlyFRxWIZPI1ZpgqlZ8jMw/1Dp/dl3P0L1jtZ+zVcHqwPhGwaJwKL00WVgfnBy6PWCde9W65or7IIETImuA==",
+            "integrity": "sha512-Zs1YsZVfemekSZG+44vBsYTLQORkPMwnlv+aehcxK/NLKC+EGhDB39/YePYYqx/sTk6NnYpuqikhSn7+JIevTA==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.8.1.tgz",
-            "version": "2.8.1"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.9.0.tgz",
+            "version": "2.9.0"
         },
         "node_modules/nanoid": {
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
             "dev": true,
             "engines": {
@@ -2349,52 +2349,52 @@
             "version": "6.0.2"
         },
         "node_modules/postcss-modules-extract-imports": {
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
-            "integrity": "sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==",
+            "integrity": "sha512-k3kNe0aNFQDAZGbin48pL2VNidTF0w4/eASDsxlyspobzU3wZQLOGj7L9gfRe0Jo9/4uud09DsjFNH7winGv8Q==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.0.0.tgz",
-            "version": "3.0.0"
+            "resolved": "https://registry.npmjs.org/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.1.0.tgz",
+            "version": "3.1.0"
         },
         "node_modules/postcss-modules-local-by-default": {
             "dependencies": {
                 "icss-utils": "^5.0.0",
                 "postcss-selector-parser": "^6.0.2",
                 "postcss-value-parser": "^4.1.0"
             },
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
-            "integrity": "sha512-L4QzMnOdVwRm1Qb8m4x8jsZzKAaPAgrUF1r/hjDR2Xj7R+8Zsf97jAlSQzWtKx5YNiNGN8QxmPFIc/sh+RQl+Q==",
+            "integrity": "sha512-6MieY7sIfTK0hYfafw1OMEG+2bg8Q1ocHCpoWLqOKj3JXlKu4G7btkmM/B7lFubYkYWmRSPLZi5chid63ZaZYw==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.4.tgz",
-            "version": "4.0.4"
+            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.5.tgz",
+            "version": "4.0.5"
         },
         "node_modules/postcss-modules-scope": {
             "dependencies": {
                 "postcss-selector-parser": "^6.0.4"
             },
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
-            "integrity": "sha512-uZgqzdTleelWjzJY+Fhti6F3C9iF1JR/dODLs/JDefozYcKTBCdD8BIl6nNPbTbcLnGrk56hzwZC2DaGNvYjzA==",
+            "integrity": "sha512-oq+g1ssrsZOsx9M96c5w8laRmvEu9C3adDSjI8oTcbfkrTE8hx/zfyobUoWIxaKPO8bt6S62kxpw5GqypEw1QQ==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-modules-scope/-/postcss-modules-scope-3.1.1.tgz",
-            "version": "3.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-modules-scope/-/postcss-modules-scope-3.2.0.tgz",
+            "version": "3.2.0"
         },
         "node_modules/postcss-modules-values": {
             "dependencies": {
                 "icss-utils": "^5.0.0"
             },
             "dev": true,
             "engines": {
@@ -2764,31 +2764,31 @@
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-Gpczt3WA56Ly0Mn8Sl21Vj94s1axi9hDIzDFn9Ph9x3C3p4nNyvsqJoQyVXKou6cBlfFWEgRW4rT8Tb4i3XnVA==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.72.0.tgz",
-            "version": "1.72.0"
+            "integrity": "sha512-nc3LeqvF2FNW5xGF1zxZifdW3ffIz5aBb7I7tSvOoNu7z1RQ6pFt9MBuiPtjgaI62YWrM/txjWlOCFiGtf2xpw==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.76.0.tgz",
+            "version": "1.76.0"
         },
         "node_modules/sass-loader": {
             "dependencies": {
                 "neo-async": "^2.6.2"
             },
             "dev": true,
             "engines": {
                 "node": ">= 18.12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-QX8AasDg75monlybel38BZ49JP5Z+uSKfKwF2rO7S74BywaRmGQMUBw9dtkS+ekyM/QnP+NOrRYq8ABMZ9G8jw==",
+            "integrity": "sha512-G0VcnMYU18a4N7VoNDegg2OuMjYtxnqzQWARVWCIVSZwJeiL9kg8QMsuIZOplsJgTzZLF6jGxI3AClj8I9nRdQ==",
             "peerDependencies": {
                 "@rspack/core": "0.x || 1.x",
                 "node-sass": "^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0 || ^9.0.0",
                 "sass": "^1.3.0",
                 "sass-embedded": "*",
                 "webpack": "^5.0.0"
             },
@@ -2805,16 +2805,16 @@
                 "sass-embedded": {
                     "optional": true
                 },
                 "webpack": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-14.1.1.tgz",
-            "version": "14.1.1"
+            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-14.2.1.tgz",
+            "version": "14.2.1"
         },
         "node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
                 "ajv": "^8.9.0",
                 "ajv-formats": "^2.1.1",
                 "ajv-keywords": "^5.1.0"
@@ -2915,26 +2915,26 @@
             "integrity": "sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==",
             "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
             "version": "0.5.21"
         },
         "node_modules/style-loader": {
             "dev": true,
             "engines": {
-                "node": ">= 12.13.0"
+                "node": ">= 18.12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-0WqXzrsMTyb8yjZJHDqwmnwRJvhALK9LfRtRc6B4UTWe8AijYLZYZ9thuJTZc2VfQWINADW/j+LiJnfy2RoC1w==",
+            "integrity": "sha512-1V4WqhhZZgjVAVJyt7TdDPZoPBPNHbekX4fWnCJL1yQukhCeZhJySUL+gL9y6sNdN95uEOS83Y55SqHcP7MzLA==",
             "peerDependencies": {
-                "webpack": "^5.0.0"
+                "webpack": "^5.27.0"
             },
-            "resolved": "https://registry.npmjs.org/style-loader/-/style-loader-3.3.4.tgz",
-            "version": "3.3.4"
+            "resolved": "https://registry.npmjs.org/style-loader/-/style-loader-4.0.0.tgz",
+            "version": "4.0.0"
         },
         "node_modules/stylehacks": {
             "dependencies": {
                 "browserslist": "^4.22.2",
                 "postcss-selector-parser": "^6.0.15"
             },
             "dev": true,
```

### Comparing `furo-2024.4.27/pyproject.toml` & `furo-2024.5.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 dynamic = ["version"]
 readme = "README.md"
 
 requires-python = ">=3.8"
 dependencies = [
   "beautifulsoup4",
   "sphinx >= 6.0,<8.0",
-  "sphinx-basic-ng",
+  "sphinx-basic-ng >= 1.0.0.beta2",
   "pygments >= 2.7",
 ]
 
 license = { file = "LICENSE" }
 authors = [{ name = "Pradyun Gedam", email = "mail@pradyunsg.me" }]
 classifiers = [
   "Framework :: Sphinx",
```

### Comparing `furo-2024.4.27/src/furo/__init__.py` & `furo-2024.5.6/src/furo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A clean customisable Sphinx documentation theme."""
 
-__version__ = "2024.04.27"
+__version__ = "2024.05.06"
 
 import hashlib
 import logging
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, cast
@@ -72,16 +72,16 @@
 
     toctree = TocTree(builder.env).get_toc_for(docname, builder)
     try:
         self_toctree = toctree[0][1]  # type: ignore[index]
     except IndexError:
         val = True
     else:
-        # There's only the page's own toctree in there.
-        val = len(self_toctree) == 1 and self_toctree[0].tagname == "toctree"
+        # There's only the page's own toctree(s) in there.
+        val = all(entry.tagname == "toctree" for entry in self_toctree)
     return val
 
 
 def get_pygments_style_colors(
     style: Style, *, fallbacks: Dict[str, str]
 ) -> Dict[str, str]:
     """Get background/foreground colors for given pygments style."""
```

### Comparing `furo-2024.4.27/src/furo/_demo_module.py` & `furo-2024.5.6/src/furo/_demo_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,25 @@
         """Initialize."""
         self._seed = 4
 
     @property
     def seed(self) -> int:
         """Get seed for random number generation.
 
+        .. versionadded:: 1.0
+
+        .. versionchanged:: 1.1
+            Use ``random`` to create the seed.
+
+        .. deprecated:: 1.2
+            ``random`` raises security concerns.
+
+        .. versionremoved:: 1.3
+            ``random`` replaced with a random number.
+
         .. seealso:: https://xkcd.com/221/
         """
         return self._seed
 
     def get_random_integer(self) -> int:
         """Return a random integer."""
         return self.seed
```

### Comparing `furo-2024.4.27/src/furo/assets/scripts/furo.js` & `furo-2024.5.6/src/furo/assets/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/scripts/gumshoe-patched.js` & `furo-2024.5.6/src/furo/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/_scaffold.sass` & `furo-2024.5.6/src/furo/assets/styles/_scaffold.sass`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 // scrollbar and allowing the scrollbars to cover the padding.
 // https://www.456bereastreet.com/archive/201301/media_query_width_and_vertical_scrollbars/
 
 // HACK: Always having the scrollbar visible, prevents certain browsers from
 // causing the content to stutter horizontally between taller-than-viewport and
 // not-taller-than-viewport pages.
 
+$icon-size: 1.25rem
+
 html
   overflow-x: hidden
   overflow-y: scroll
   scroll-behavior: smooth
 
 .sidebar-scroll, .toc-scroll, article[role=main] *
   // Override Firefox scrollbar style
@@ -199,16 +201,16 @@
   cursor: pointer
   border: none
   padding: 0
   background: transparent
 
 .theme-toggle svg
   vertical-align: middle
-  height: 1rem
-  width: 1rem
+  height: $icon-size
+  width: $icon-size
   color: var(--color-foreground-primary)
   display: none
 
 .theme-toggle-header
   float: left
   padding: 1rem 0.5rem
 
@@ -217,16 +219,16 @@
 ////////////////////////////////////////////////////////////////////////////////
 .toc-overlay-icon, .nav-overlay-icon
   display: none
   cursor: pointer
 
   .icon
     color: var(--color-foreground-secondary)
-    height: 1rem
-    width: 1rem
+    height: $icon-size
+    width: $icon-size
 
 .toc-header-icon, .nav-overlay-icon
   // for when we set display: flex
   justify-content: center
   align-items: center
 
 .toc-content-icon
@@ -237,18 +239,19 @@
   float: right
   display: flex
   margin-top: 1.5rem
   margin-left: 1rem
   margin-bottom: 1rem
   gap: 0.5rem
 
-  .edit-this-page svg
-    color: inherit
-    height: 1rem
-    width: 1rem
+  .edit-this-page, .view-this-page
+    svg
+      color: inherit
+      height: $icon-size
+      width: $icon-size
 
 .sidebar-toggle
   position: absolute
   display: none
 // <debugging things>
 .sidebar-toggle[name="__toc"]
   left: 20px
@@ -397,16 +400,16 @@
       label
         height: 100%
         width: 100%
         user-select: none
 
   .nav-overlay-icon .icon,
   .theme-toggle svg
-    height: 1.25rem
-    width: 1.25rem
+    height: $icon-size
+    width: $icon-size
 
   // Add a scroll margin for the content
   :target
     scroll-margin-top: calc(var(--header-height) + 2.5rem)
 
   // Show back-to-top below the header
   .back-to-top
```

### Comparing `furo-2024.4.27/src/furo/assets/styles/base/_print.sass` & `furo-2024.5.6/src/furo/assets/styles/base/_print.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/base/_theme.sass` & `furo-2024.5.6/src/furo/assets/styles/base/_theme.sass`

 * *Files 20% similar despite different names*

```diff
@@ -39,17 +39,23 @@
       .only-dark
         display: block !important
 
 //
 // Theme toggle presentation
 //
 body[data-theme="auto"]
-  .theme-toggle svg.theme-icon-when-auto
+  .theme-toggle svg.theme-icon-when-auto-light
     display: block
 
+  @media (prefers-color-scheme: dark)
+    .theme-toggle svg.theme-icon-when-auto-dark
+      display: block
+    .theme-toggle svg.theme-icon-when-auto-light
+      display: none
+
 body[data-theme="dark"]
   .theme-toggle svg.theme-icon-when-dark
     display: block
 
 body[data-theme="light"]
   .theme-toggle svg.theme-icon-when-light
     display: block
```

### Comparing `furo-2024.4.27/src/furo/assets/styles/base/_typography.sass` & `furo-2024.5.6/src/furo/assets/styles/base/_typography.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/components/_footer.sass` & `furo-2024.5.6/src/furo/assets/styles/components/_footer.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/components/_sidebar.sass` & `furo-2024.5.6/src/furo/assets/styles/components/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/components/_table_of_contents.sass` & `furo-2024.5.6/src/furo/assets/styles/components/_table_of_contents.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_admonitions.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_api.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_api.sass`

 * *Files 17% similar despite different names*

```diff
@@ -78,18 +78,44 @@
   font-weight: normal
   color: var(--color-api-pre-name)
 .sig-paren
   color: var(--color-api-paren)
 .sig-param
   font-style: normal
 
-.versionmodified
-  font-style: italic
-div.versionadded, div.versionchanged, div.deprecated
+div.versionadded,
+div.versionchanged,
+div.deprecated,
+div.versionremoved
+  border-left: 0.1875rem solid
+  border-radius: 0.125rem
+
+  padding-left: 0.75rem
+
   p
     margin-top: 0.125rem
     margin-bottom: 0.125rem
 
+div.versionadded
+  border-color: var(--color-api-added-border)
+  .versionmodified
+    color: var(--color-api-added)
+
+div.versionchanged
+  border-color: var(--color-api-changed-border)
+  .versionmodified
+    color: var(--color-api-changed)
+
+div.deprecated
+  border-color: var(--color-api-deprecated-border)
+  .versionmodified
+    color: var(--color-api-deprecated)
+
+div.versionremoved
+  border-color: var(--color-api-removed-border)
+  .versionmodified
+    color: var(--color-api-removed)
+
 // Align the [docs] and [source] to the right.
 .viewcode-link, .viewcode-back
   float: right
   text-align: right
```

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_code.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_footnotes.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_images.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_lists.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_misc.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_sidebar.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_tables.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/content/_target.sass` & `furo-2024.5.6/src/furo/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/extensions/_copybutton.sass` & `furo-2024.5.6/src/furo/assets/styles/extensions/_copybutton.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/extensions/_readthedocs.sass` & `furo-2024.5.6/src/furo/assets/styles/extensions/_readthedocs.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-design.sass` & `furo-2024.5.6/src/furo/assets/styles/extensions/_sphinx-design.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass` & `furo-2024.5.6/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-panels.sass` & `furo-2024.5.6/src/furo/assets/styles/extensions/_sphinx-panels.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/variables/_admonitions.scss` & `furo-2024.5.6/src/furo/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/variables/_colors.scss` & `furo-2024.5.6/src/furo/assets/styles/variables/_colors.scss`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,24 @@
   --color-api-background: var(--color-background-hover--transparent);
   --color-api-background-hover: var(--color-background-hover);
   --color-api-overall: var(--color-foreground-secondary);
   --color-api-name: var(--color-problematic);
   --color-api-pre-name: var(--color-problematic);
   --color-api-paren: var(--color-foreground-secondary);
   --color-api-keyword: var(--color-foreground-primary);
+
+  --color-api-added: #21632c;
+  --color-api-added-border: #38a84d;
+  --color-api-changed: #046172;
+  --color-api-changed-border: #06a1bc;
+  --color-api-deprecated: #605706;
+  --color-api-deprecated-border: #f0d90f;
+  --color-api-removed: #b30000;
+  --color-api-removed-border: #ff5c5c;
+
   --color-highlight-on-target: #ffffcc;
 
   // Inline code background
   --color-inline-code-background: var(--color-background-secondary);
 
   // Highlighted text (search)
   --color-highlighted-background: #ddeeff;
@@ -163,14 +173,23 @@
   --color-guilabel-background: #08356380;
   --color-guilabel-border: #13395f80;
 
   // API documentation
   --color-api-keyword: var(--color-foreground-secondary);
   --color-highlight-on-target: #333300;
 
+  --color-api-added: #3db854;
+  --color-api-added-border: #267334;
+  --color-api-changed: #09b0ce;
+  --color-api-changed-border: #056d80;
+  --color-api-deprecated: #b1a10b;
+  --color-api-deprecated-border: #6e6407;
+  --color-api-removed: #ff7575;
+  --color-api-removed-border: #b03b3b;
+
   // Admonitions
   --color-admonition-background: #18181a;
 
   // Cards
   --color-card-border: var(--color-background-secondary);
   --color-card-background: #18181a;
   --color-card-marginals-background: var(--color-background-hover);
```

### Comparing `furo-2024.4.27/src/furo/assets/styles/variables/_fonts.scss` & `furo-2024.5.6/src/furo/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/variables/_icons.scss` & `furo-2024.5.6/src/furo/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/assets/styles/variables/_spacing.scss` & `furo-2024.5.6/src/furo/assets/styles/variables/_spacing.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/navigation.py` & `furo-2024.5.6/src/furo/navigation.py`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/sphinxext.py` & `furo-2024.5.6/src/furo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/base.html` & `furo-2024.5.6/src/furo/theme/furo/base.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/domainindex.html` & `furo-2024.5.6/src/furo/theme/furo/domainindex.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/genindex.html` & `furo-2024.5.6/src/furo/theme/furo/genindex.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/page.html` & `furo-2024.5.6/src/furo/theme/furo/page.html`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     <div class="header-center">
       <a href="{{ pathto(master_doc) }}"><div class="brand">{{ docstitle if docstitle else project }}</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
-          <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
+          <svg class="theme-icon-when-auto-light"><use href="#svg-sun-with-moon"></use></svg>
+          <svg class="theme-icon-when-auto-dark"><use href="#svg-moon-with-sun"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
           <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
         </button>
       </div>
       <label class="toc-overlay-icon toc-header-icon{% if furo_hide_toc %} no-toc{% endif %}" for="__toc">
         <div class="visually-hidden">Toggle table of contents sidebar</div>
         <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
@@ -70,24 +71,46 @@
         <a href="#" class="back-to-top muted-link">
           <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
             <path d="M13 20h-2V8l-5.5 5.5-1.42-1.42L12 4.16l7.92 7.92-1.42 1.42L13 8v12z"></path>
           </svg>
           <span>{% trans %}Back to top{% endtrans %}</span>
         </a>
         <div class="content-icon-container">
-          {% if theme_top_of_page_button == "edit" -%}
-          {%- include "components/edit-this-page.html" with context -%}
-          {%- elif theme_top_of_page_button != None -%}
-          {{ warning("Got an unsupported value for 'top_of_page_button'") }}
+          {% if theme_top_of_page_button != "edit" -%}
+            {{ warning("Got configuration for 'top_of_page_button': this is deprecated.") }}
           {%- endif -%}
+
+          {%- if theme_top_of_page_buttons == "" -%}
+            {% if theme_top_of_page_button == None -%}
+              {#- We respect the old configuration of disabling all the buttons -#}
+              {%- set theme_top_of_page_buttons = [] -%}
+            {% else %}
+              {%- set theme_top_of_page_buttons = ["view", "edit"] -%}
+            {%- endif -%}
+          {% else -%}
+            {% if theme_top_of_page_button != "edit" -%}
+              {%- set theme_top_of_page_buttons = [] -%}
+              {{ warning("Got configuration for both 'top_of_page_button' and 'top_of_page_buttons', ignoring both and removing all top of page buttons.") }}
+            {%- endif -%}
+          {%- endif -%}
+          {% for button in theme_top_of_page_buttons -%}
+            {% if button == "view" %}
+            {%- include "components/view-this-page.html" with context -%}
+            {% elif button == "edit" %}
+            {%- include "components/edit-this-page.html" with context -%}
+            {% else %}
+            {{ warning("Got an unsupported value in 'top_of_page_buttons' for theme configuration") }}
+            {% endif %}
+          {%- endfor -%}
           {#- Theme toggle -#}
           <div class="theme-toggle-container theme-toggle-content">
             <button class="theme-toggle">
               <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
-              <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
+              <svg class="theme-icon-when-auto-light"><use href="#svg-sun-with-moon"></use></svg>
+              <svg class="theme-icon-when-auto-dark"><use href="#svg-moon-with-sun"></use></svg>
               <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
               <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
             </button>
           </div>
           <label class="toc-overlay-icon toc-content-icon{% if furo_hide_toc %} no-toc{% endif %}" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
```

#### html2text {}

```diff
@@ -10,18 +10,28 @@
 Toggle Light / Dark / Auto color theme
 Toggle table of contents sidebar
 {% block left_sidebar %}
 {%- for sidebar_section in sidebars %} {%- include sidebar_section %} {%-
 endfor %}
 {% endblock left_sidebar %}
 _{_%_ _t_r_a_n_s_ _%_}_B_a_c_k_ _t_o_ _t_o_p_{_%_ _e_n_d_t_r_a_n_s_ _%_}
-{% if theme_top_of_page_button == "edit" -%} {%- include "components/edit-this-
-page.html" with context -%} {%- elif theme_top_of_page_button != None -%} {
-{ warning("Got an unsupported value for 'top_of_page_button'") }} {%- endif -%}
-{#- Theme toggle -#}
+{% if theme_top_of_page_button != "edit" -%} {{ warning("Got configuration for
+'top_of_page_button': this is deprecated.") }} {%- endif -%} {%- if
+theme_top_of_page_buttons == "" -%} {% if theme_top_of_page_button == None -%}
+{#- We respect the old configuration of disabling all the buttons -#} {%- set
+theme_top_of_page_buttons = [] -%} {% else %} {%- set theme_top_of_page_buttons
+= ["view", "edit"] -%} {%- endif -%} {% else -%} {% if theme_top_of_page_button
+!= "edit" -%} {%- set theme_top_of_page_buttons = [] -%} {{ warning("Got
+configuration for both 'top_of_page_button' and 'top_of_page_buttons', ignoring
+both and removing all top of page buttons.") }} {%- endif -%} {%- endif -%} {%
+for button in theme_top_of_page_buttons -%} {% if button == "view" %} {%-
+include "components/view-this-page.html" with context -%} {% elif button ==
+"edit" %} {%- include "components/edit-this-page.html" with context -%} {% else
+%} {{ warning("Got an unsupported value in 'top_of_page_buttons' for theme
+configuration") }} {% endif %} {%- endfor -%} {#- Theme toggle -#}
 Toggle Light / Dark / Auto color theme
 Toggle table of contents sidebar
 {% block content %}{{ body }}{% endblock %}
 {% block footer %}
 {% if next -%}
 _{_{_ ___(_"_N_e_x_t_"_)_ _}_}
 _{_{_ _n_e_x_t_._t_i_t_l_e_ _}_}
```

### Comparing `furo-2024.4.27/src/furo/theme/furo/partials/_head_css_variables.html` & `furo-2024.5.6/src/furo/theme/furo/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/search.html` & `furo-2024.5.6/src/furo/theme/furo/search.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/sidebar/brand.html` & `furo-2024.5.6/src/furo/theme/furo/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/sidebar/rtd-versions.html` & `furo-2024.5.6/src/furo/theme/furo/sidebar/rtd-versions.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/src/furo/theme/furo/sidebar/variant-selector.html` & `furo-2024.5.6/src/furo/theme/furo/sidebar/variant-selector.html`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/tests/workflow/test_sphinx_versions.py` & `furo-2024.5.6/tests/workflow/test_sphinx_versions.py`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/webpack.config.js` & `furo-2024.5.6/webpack.config.js`

 * *Files identical despite different names*

### Comparing `furo-2024.4.27/PKG-INFO` & `furo-2024.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furo
-Version: 2024.4.27
+Version: 2024.5.6
 Summary: A clean customisable Sphinx documentation theme.
 Author-Email: Pradyun Gedam <mail@pradyunsg.me>
 License: Copyright (c) 2020 Pradyun Gedam <mail@pradyunsg.me>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to
         deal in the Software without restriction, including without limitation the
@@ -37,15 +37,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Project-URL: Github, https://github.com/pradyunsg/furo
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
 Requires-Dist: sphinx<8.0,>=6.0
-Requires-Dist: sphinx-basic-ng
+Requires-Dist: sphinx-basic-ng>=1.0.0.beta2
 Requires-Dist: pygments>=2.7
 Description-Content-Type: text/markdown
 
 <h1 align="center">Furo</h1>
 <p align="center">
   A clean customisable <a href="https://www.sphinx-doc.org/">Sphinx</a> documentation theme.
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: furo Version: 2024.4.27 Summary: A clean
+Metadata-Version: 2.1 Name: furo Version: 2024.5.6 Summary: A clean
 customisable Sphinx documentation theme. Author-Email: Pradyun Gedam
 pradyunsg.me> License: Copyright (c) 2020 Pradyun Gedam
 pradyunsg.me> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -22,16 +22,16 @@
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Operating System :: OS Independent Classifier: Topic
 :: Documentation Classifier: Topic :: Software Development :: Documentation
 Project-URL: Github, https://github.com/pradyunsg/furo Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4 Requires-Dist: sphinx<8.0,>=6.0 Requires-Dist:
-sphinx-basic-ng Requires-Dist: pygments>=2.7 Description-Content-Type: text/
-markdown
+sphinx-basic-ng>=1.0.0.beta2 Requires-Dist: pygments>=2.7 Description-Content-
+Type: text/markdown
                               ************ FFuurroo ************
                A clean customisable _S_p_h_i_n_x documentation theme.
 _[_D_e_m_o_ _i_m_a_g_e_]## Elevator pitch - **Intentionally minimal** --- the most
 important thing is the content, not the scaffolding around it. - **Responsive**
 --- adapting perfectly to the available screen space, to work on all sorts of
 devices. - **Customisable** --- change the color palette, font families, logo
 and more! - **Easy to navigate** --- with carefully-designed sidebar navigation
```

