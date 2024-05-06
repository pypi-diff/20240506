# Comparing `tmp/elisa_lib-0.1.0.tar.gz` & `tmp/elisa_lib-0.1.1.tar.gz`

## Comparing `elisa_lib-0.1.0.tar` & `elisa_lib-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,80 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/noxfile.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/docs/modules.rst
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/__about__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/data/__init__.py
--rw-r--r--   0        0        0    21847 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/data/grouping.py
--rw-r--r--   0        0        0    55530 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/data/ogip.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/__init__.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/data.py
--rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/fit.py
--rw-r--r--   0        0        0    33616 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/helper.py
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/likelihood.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/lrt.py
--rw-r--r--   0        0        0    19964 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/nested_sampling.py
--rw-r--r--   0        0        0    67863 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/infer/results.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/__init__.py
--rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/add.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/conv.py
--rw-r--r--   0        0        0    55905 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/model.py
--rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/mul.py
--rw-r--r--   0        0        0    30650 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/parameter.py
--rw-r--r--   0        0        0    14335 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/xspec.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/tables/generate_xsect_table.py
--rw-r--r--   0        0        0  3172880 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/models/tables/xsect.hdf5
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/__init__.py
--rw-r--r--   0        0        0    30171 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/data.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/errorbars.py
--rw-r--r--   0        0        0     9438 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/misc.py
--rw-r--r--   0        0        0    51692 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/plotter.py
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/residuals.py
--rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/scale.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/plot/util.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/__init__.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/bslogu.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/config.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/integrate.py
--rw-r--r--   0        0        0    14312 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/misc.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/scipy_nquad.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/src/elisa/util/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/model/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/model/test_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/parameter/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/tests/parameter/test_name.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/LICENSE
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/README.md
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 elisa_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/noxfile.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/api.md
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/contributing.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/guide.md
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/installation.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/troubleshooting.md
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/tutorials.md
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_static/favicon.svg
+-rw-r--r--   0        0        0   450129 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_static/logo1.png
+-rw-r--r--   0        0        0   435014 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_static/logo2.png
+-rw-r--r--   0        0        0   748938 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_static/logo3.png
+-rw-r--r--   0        0        0  1259327 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_static/logo4.png
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_templates/apidoc/module.rst_t
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/_templates/apidoc/package.rst_t
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/quick-start.ipynb
+-rw-r--r--   0        0        0   134102 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/xspec-models.ipynb
+-rw-r--r--   0        0        0    25920 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_HE.bak
+-rw-r--r--   0        0        0    34560 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_HE.pi
+-rw-r--r--   0        0        0   521280 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_HE.rsp
+-rw-r--r--   0        0        0    57600 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_LE.bak
+-rw-r--r--   0        0        0    46080 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_LE.pi
+-rw-r--r--   0        0        0  7058880 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_LE.rsp
+-rw-r--r--   0        0        0    43200 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_ME.bak
+-rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_ME.pi
+-rw-r--r--   0        0        0  2738880 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/docs/notebooks/data/P011160500104_ME.rsp
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/__about__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/data/__init__.py
+-rw-r--r--   0        0        0    21961 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/data/grouping.py
+-rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/data/ogip.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/__init__.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/data.py
+-rw-r--r--   0        0        0    35078 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/fit.py
+-rw-r--r--   0        0        0    33741 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/helper.py
+-rw-r--r--   0        0        0    15947 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/likelihood.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/lrt.py
+-rw-r--r--   0        0        0    20147 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/nested_sampling.py
+-rw-r--r--   0        0        0    71215 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/infer/results.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/__init__.py
+-rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/add.py
+-rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/conv.py
+-rw-r--r--   0        0        0    55908 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/model.py
+-rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/mul.py
+-rw-r--r--   0        0        0    30650 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/parameter.py
+-rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/xspec.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/tables/generate_xsect_table.py
+-rw-r--r--   0        0        0  3172880 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/models/tables/xsect.hdf5
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/__init__.py
+-rw-r--r--   0        0        0    30817 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/data.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/errorbars.py
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/misc.py
+-rw-r--r--   0        0        0    53226 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/plotter.py
+-rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/residuals.py
+-rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/scale.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/plot/util.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/__init__.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/bslogu.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/config.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/integrate.py
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/misc.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/scipy_nquad.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/src/elisa/util/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/tests/model/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/tests/model/test_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/tests/parameter/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/tests/parameter/test_name.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/README.md
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 elisa_lib-0.1.1/PKG-INFO
```

### Comparing `elisa_lib-0.1.0/.github/workflows/tests.yml` & `elisa_lib-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/docs/Makefile` & `elisa_lib-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/docs/conf.py` & `elisa_lib-0.1.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,45 +51,53 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_book_theme'
 html_theme_options = {
     'github_url': 'https://github.com/wcxve/elisa',
     'repository_url': 'https://github.com/wcxve/elisa',
     'repository_branch': 'main',
-    'home_page_in_toc': True,
     'path_to_docs': 'docs',
     'launch_buttons': {
         'binderhub_url': 'https://mybinder.org',
         'colab_url': 'https://colab.research.google.com/',
         'notebook_interface': 'jupyterlab',
     },
     'navigation_with_keys': False,
     'use_edit_page_button': True,
     'use_repository_button': True,
     'use_download_button': True,
     'use_issues_button': True,
 }
-# html_static_path = ['_static']
+html_title = 'elisa'
+html_static_path = ['_static']
+html_logo = '_static/logo2.png'
+html_favicon = '_static/favicon.svg'
 html_baseurl = 'https://elisa-lib.readthedocs.io/en/latest/'
+html_show_sourcelink = False
+master_doc = 'index'
 
+add_module_names = False
 autodoc_member_order = 'bysource'
 
+copybutton_selector = 'div:not(.output) > div.highlight pre'
+
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3.9', None),
     'arviz': ('https://python.arviz.org/en/stable/', None),
     'jax': ('https://jax.readthedocs.io/en/latest/', None),
     'matplotlib': ('https://matplotlib.org/stable/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'numpyro': ('https://num.pyro.ai/en/stable/', None),
     'tinygp': ('https://tinygp.readthedocs.io/en/latest/', None),
 }
 
 myst_enable_extensions = [
     'amsmath',
     'dollarmath',
+    'colon_fence',
 ]
 
 nb_ipywidgets_js = {
     'https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js': {
         'integrity': 'sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=',
         'crossorigin': 'anonymous',
     },
@@ -108,15 +116,20 @@
 numpydoc_show_inherited_class_members = True
 numpydoc_xref_aliases = {
     'Data': 'elisa.data.ogip.Data',
     'Model': 'elisa.models.model.Model',
     'Parameter': 'elisa.models.parameter.Parameter',
 }
 numpydoc_xref_param_type = True
-numpydoc_xref_ignore = {'optional', 'type_without_description', 'BadException'}
+numpydoc_xref_ignore = {
+    'or',
+    'optional',
+    'type_without_description',
+    'BadException',
+}
 # Run docstring validation as part of build process
 # numpydoc_validation_checks = {"all", "GL01", "SA04", "RT03"}
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 typehints_document_rtype = False
 typehints_use_signature = True
```

### Comparing `elisa_lib-0.1.0/src/elisa/__init__.py` & `elisa_lib-0.1.1/src/elisa/__init__.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/data/grouping.py` & `elisa_lib-0.1.1/src/elisa/data/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,20 +231,23 @@
         success = False
     else:
         success = True
 
     return flag, success
 
 
-def _significance_lima(
+def significance_lima(
     n_on: float | NDArray,
     n_off: float | NDArray,
     a: float | NDArray,
 ) -> NDArray:
     """Significance using the formula of Li & Ma 1983."""
+    n_on = np.asarray(n_on)
+    n_off = np.asarray(n_off)
+
     term1 = np.zeros_like(n_on).astype(float)
     mask = n_on > 0.0
     if mask.any():
         term1[mask] = xlogy(
             n_on[mask], (1.0 + a) / a * n_on[mask] / (n_on[mask] + n_off[mask])
         )
 
@@ -254,21 +257,25 @@
         term2[mask] = xlogy(
             n_off[mask], (1.0 + a) * n_off[mask] / (n_on[mask] + n_off[mask])
         )
 
     return np.sqrt(2.0 * (term1 + term2))
 
 
-def _significance_gv(
+def significance_gv(
     n: float | NDArray,
     b: float | NDArray,
     s: float | NDArray,
     a: float | NDArray,
 ) -> NDArray:
     """Significance using the formula of Vianello 2018."""
+    n = np.asarray(n)
+    b = np.asarray(b)
+    s = np.asarray(s)
+
     b = b * a
     s = s * a
     s2 = s * s
     s4 = s2 * s2
     b0_mle = 0.5 * (b - s2 + np.sqrt(b * b - 2 * b * s2 + 4 * n * s2 + s4))
     b0_mle = np.clip(b0_mle, 0, None)
 
@@ -441,18 +448,18 @@
         if k.size:
             j = np.minimum(j, np.min(k + bint[k] - 1))
 
         # Ensure minimum significance and extend the bin if necessary to abide
         # that constraint
         on = n_on[i : j + 1].sum()
         off = n_off[i : j + 1].sum()
-        if _significance_lima(on, off, a) < sig:
+        if significance_lima(on, off, a) < sig:
             on = n_on[j + 1 :].cumsum()
             off = n_off[j + 1 :].cumsum()
-            mask = _significance_lima(on, off, a) >= sig
+            mask = significance_lima(on, off, a) >= sig
             if np.any(mask):
                 # the smallest j for the significance threshold
                 j += np.flatnonzero(mask)[0] + 1
             else:
                 # if the last group does not have a nominal significance,
                 # then combine the last two groups to ensure all
                 # groups meet the count requirement
@@ -470,15 +477,15 @@
 
     idx = idx[:ng]
     flag = np.full(nchan, -1, dtype=int)
     flag[idx] = 1
 
     on = np.add.reduceat(n_on, idx)
     off = np.add.reduceat(n_off, idx)
-    if np.all(_significance_lima(on, off, a) >= sig):
+    if np.all(significance_lima(on, off, a) >= sig):
         success = True
     else:
         success = False
 
     return flag, success
 
 
@@ -547,20 +554,20 @@
 
         # Ensure minimum significance and extend the bin if necessary to abide
         # that constraint
         n_ = n[i : j + 1].sum()
         b_ = b[i : j + 1].sum()
         s_ = s[i : j + 1]
         s_ = np.sqrt(np.sum(s_ * s_))
-        if _significance_gv(n_, b_, s_, a) < sig:
+        if significance_gv(n_, b_, s_, a) < sig:
             n_ = n[j + 1 :].cumsum()
             b_ = b[j + 1 :].cumsum()
             s_ = s[j + 1 :]
             s_ = np.sqrt(np.sum(s_ * s_))
-            mask = _significance_gv(n_, b_, s_, a) >= sig
+            mask = significance_gv(n_, b_, s_, a) >= sig
             if np.any(mask):
                 # the smallest j for the significance threshold
                 j += np.flatnonzero(mask)[0] + 1
             else:
                 # if the last group does not have a nominal significance,
                 # then combine the last two groups to ensure all
                 # groups meet the count requirement
@@ -579,15 +586,15 @@
     idx = idx[:ng]
     flag = np.full(nchan, -1, dtype=int)
     flag[idx] = 1
 
     n_ = np.add.reduceat(n, idx)
     b_ = np.add.reduceat(b, idx)
     s_ = np.sqrt(np.add.reduceat(s * s, idx))
-    if np.all(_significance_gv(n_, b_, s_, a) >= sig):
+    if np.all(significance_gv(n_, b_, s_, a) >= sig):
         success = True
     else:
         success = False
 
     return flag, success
 
 
@@ -701,15 +708,15 @@
     imax = nd - 1
 
     group_on = 0.0
     group_off = 0.0
     for i, (j, k) in enumerate(zip(n_on, n_off)):
         group_on += j
         group_off += k
-        group_sig = _significance_lima(group_on, group_off, a)
+        group_sig = significance_lima(group_on, group_off, a)
 
         if i == imax:
             if group_sig < sig and ng > 1:
                 # if the last group does not have a nominal significance,
                 # then combine the last two groups to ensure all
                 # groups meet the count requirement
                 ng -= 1
@@ -721,15 +728,15 @@
             ng += 1
             group_on = 0.0
             group_off = 0.0
 
     idx = idx[:ng]
     group_on = np.add.reduceat(n_on, idx)
     group_off = np.add.reduceat(n_off, idx)
-    if np.all(_significance_lima(group_on, group_off, a) >= sig):
+    if np.all(significance_lima(group_on, group_off, a) >= sig):
         success = True
     else:
         success = False
 
     flag = np.full(nd, -1, dtype=int)
     flag[idx] = 1
 
@@ -782,15 +789,15 @@
     group_n = 0.0
     group_b = 0.0
     group_var = 0.0
     for i, (ni, bi, si) in enumerate(zip(n, b, s)):
         group_n += ni
         group_b += bi
         group_var += si * si
-        group_sig = _significance_gv(group_n, group_b, np.sqrt(group_var), a)
+        group_sig = significance_gv(group_n, group_b, np.sqrt(group_var), a)
 
         if i == imax:
             if group_sig < sig and ng > 1:
                 # if the last group does not have a nominal significance,
                 # then combine the last two groups to ensure all
                 # groups meet the count requirement
                 ng -= 1
@@ -804,15 +811,15 @@
             group_b = 0.0
             group_var = 0.0
 
     idx = idx[:ng]
     group_n = np.add.reduceat(n, idx)
     group_b = np.add.reduceat(b, idx)
     group_var = np.sqrt(np.add.reduceat(s * s, idx))
-    group_sig = _significance_gv(group_n, group_b, np.sqrt(group_var), a)
+    group_sig = significance_gv(group_n, group_b, np.sqrt(group_var), a)
     if np.all(group_sig >= sig):
         success = True
     else:
         success = False
 
     flag = np.full(nd, -1, dtype=int)
     flag[idx] = 1
```

### Comparing `elisa_lib-0.1.0/src/elisa/data/ogip.py` & `elisa_lib-0.1.1/src/elisa/data/ogip.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     group_opt,
     group_optsig_gv,
     group_optsig_lima,
     group_optsig_normal,
     group_sig_gv,
     group_sig_lima,
     group_sig_normal,
+    significance_gv,
+    significance_lima,
 )
+from elisa.plot.misc import get_colors
 
 if TYPE_CHECKING:
     from elisa.util.typing import NumPyArray as NDArray
 
 # TODO: support multiple response in a single data object
 # TODO: support creating Data object from array
 
@@ -102,20 +105,14 @@
 
     record_channel : bool, optional
         Whether to record channel information in the label of grouped
         channel. Only takes effect if `group` is not None or spectral data
         has ``GROUPING`` defined. The default is False.
     resp_sparse : bool, optional
         Whether the response matrix is sparse. The default is False.
-    corrfile : str or None, optional
-        Correction file applied to `specfile`. Read from the `specfile`
-        header if None. The default is None.
-    corrnorm : float or None, optional
-        Scaling factor to be applied to `corrfile`. Read from the
-        `specfile` header if None. The default is None.
 
     Notes
     -----
     Reading and applying correction to data is not yet supported.
 
     References
     ----------
@@ -138,16 +135,16 @@
         group: str | None = None,
         scale: float | int | None = None,
         spec_poisson: bool | None = None,
         back_poisson: bool | None = None,
         ignore_bad: bool = True,
         record_channel: bool = False,
         resp_sparse: bool = False,
-        corrfile: bool | None = None,
-        corrnorm: bool | None = None,
+        # corrfile: bool | None = None,
+        # corrnorm: bool | None = None,
     ):
         erange = np.array(erange, dtype=np.float64, order='C', ndmin=2)
 
         # check if erange is increasing
         if np.any(np.diff(erange, axis=1) <= 0.0):
             raise ValueError('erange must be increasing')
 
@@ -225,30 +222,30 @@
                     Warning,
                     stacklevel=2,
                 )
         if not np.any(good_quality):
             raise RuntimeError(f'no good channel is found for {name} data')
 
         # corrfile and corrnorm are not supported yet
-        if corrfile or corrnorm:
-            warnings.warn(
-                'correction to data is not yet supported',
-                Warning,
-                stacklevel=2,
-            )
-
+        # if corrfile or corrnorm:
+        #     warnings.warn(
+        #         'correction to data is not yet supported',
+        #         Warning,
+        #         stacklevel=2,
+        #     )
+        #
         # check correction file
         # use poisson=True to bypass stat_err check, which takes no effect
         # if corrfile:
         #     corr = Spectrum(corrfile, True)
         # elif spec.corrfile:
         #     corr = Spectrum(spec.corrfile, True)
         # else:
         #     corr = None
-
+        #
         # check correction scale
         # if corr:
         #     if corrnorm:
         #         spec._corr_scale = corrnorm
 
         self._spec = spec
         self._resp = resp
@@ -604,23 +601,146 @@
         """Return channel mask given energy grid and erange of interest."""
         emin = np.expand_dims(self._erange[:, 0], axis=1)
         emax = np.expand_dims(self._erange[:, 1], axis=1)
         mask1 = np.less_equal(emin, ch_emin)
         mask2 = np.less_equal(ch_emax, emax)
         return np.bitwise_and(mask1, mask2)
 
+    def plot_spec(self, xlog: bool = True, ylog: bool = False):
+        """Plot the spectrum.
+
+        .. warning::
+            The significance plot is accurate only if the spectrum data has
+            enough count statistics.
+
+        Parameters
+        ----------
+        xlog : bool, optional
+            Whether to use log scale on x-axis. The default is True.
+        ylog : bool, optional
+            Whether to use log scale on y-axis. The default is False.
+        """
+        fig, axs = plt.subplots(
+            nrows=2,
+            ncols=1,
+            sharex=True,
+            height_ratios=[1.618, 1.0],
+            gridspec_kw={'hspace': 0.05},
+        )
+        fig.align_ylabels(axs)
+
+        for ax in axs:
+            ax.tick_params(
+                axis='both',
+                which='both',
+                direction='in',
+                bottom=True,
+                top=True,
+                left=True,
+                right=True,
+            )
+
+        plt.rcParams['axes.formatter.min_exponent'] = 3
+
+        axs[0].set_ylabel(r'$C_E\ \mathrm{[s^{-1}\ keV^{-1}]}$')
+        axs[1].set_ylabel(r'Significance [$\mathrm{\sigma}$]')
+        axs[1].set_xlabel(r'$\mathrm{Energy\ [keV]}$')
+
+        if self.has_back:
+            colors = get_colors(2, 'colorblind')
+        else:
+            colors = get_colors(1, 'colorblind')
+
+        factor = 1.0 / (self.spec_exposure * self.ch_width)
+        x = self.ch_mean if xlog else self.ch_emid
+        xerr = self.ch_error if xlog else 0.5 * self.ch_width
+        axs[0].errorbar(
+            x=x,
+            xerr=xerr,
+            y=self.spec_counts * factor,
+            yerr=self.spec_error * factor,
+            fmt='o',
+            color=colors[0],
+            alpha=0.8,
+            label='Observation',
+            ms=3,
+            mfc='#FFFFFFCC',
+        )
+
+        if self.has_back:
+            factor = self.back_ratio / (self.spec_exposure * self.ch_width)
+            axs[0].errorbar(
+                x=x,
+                xerr=xerr,
+                y=self.back_counts * factor,
+                yerr=self.back_error * factor,
+                fmt='s',
+                color=colors[1],
+                alpha=0.8,
+                label='Background',
+                ms=3,
+                mfc='#FFFFFFCC',
+            )
+
+        if self.spec_poisson and self.has_back:
+            if self.back_poisson:
+                sig = significance_lima(
+                    self.spec_counts, self.back_counts, self.back_ratio
+                )
+            else:
+                sig = significance_gv(
+                    self.spec_counts,
+                    self.back_counts,
+                    self.back_error,
+                    self.back_ratio,
+                )
+            sig *= np.sign(self.net_counts)
+        else:
+            sig = self.net_counts / self.net_error
+
+        axs[1].errorbar(
+            x=x,
+            xerr=xerr,
+            y=sig,
+            yerr=1,
+            fmt='o',
+            color=colors[0],
+            alpha=0.8,
+            ms=3,
+            mfc='#FFFFFFCC',
+        )
+        axs[1].axhline(0, color='k', ls=':', lw=0.5)
+
+        if xlog:
+            axs[0].set_xscale('log')
+        if ylog:
+            axs[0].set_yscale('log')
+
+        axs[0].legend()
+        axs[0].set_title(self.name)
+
+    def plot_effective_area(self, hatch: bool = True):
+        """Plot the effective area.
+
+        Parameters
+        ----------
+        hatch : bool, optional
+            Whether to add hatches in the ignored region. The default is True.
+        """
+        self._resp.plot_effective_area(self._erange if hatch else None)
+
     def plot_matrix(self, hatch: bool = True) -> None:
         """Plot the response matrix.
 
         Parameters
         ----------
         hatch : bool, optional
             Whether to add hatches in the ignored region. The default is True.
         """
-        self._resp.plot(self._erange if hatch else None)
+        self._resp.plot_matrix(self._erange if hatch else None)
 
     @property
     def name(self) -> str:
         """Data name."""
         return self._name
 
     @property
@@ -943,15 +1063,15 @@
         # get respfile
         self._respfile = get_field('RESPFILE', '', excluded_file)
 
         # get ancrfile
         self._ancrfile = get_field('ANCRFILE', '', excluded_file)
 
         # get corrfile
-        self._corrfile = get_field('CORRFILE', '', excluded_file)
+        # self._corrfile = get_field('CORRFILE', '', excluded_file)
 
         # get the background scaling factor
         back_scale = np.float64(get_field('BACKSCAL', 1.0))
         if isinstance(back_scale, np.ndarray):
             back_scale = np.array(back_scale, dtype=np.float64, order='C')
         else:
             back_scale = np.float64(back_scale)
@@ -962,15 +1082,15 @@
         if isinstance(area_scale, np.ndarray):
             area_scale = np.array(area_scale, dtype=np.float64, order='C')
         else:
             area_scale = np.float64(area_scale)
         self._area_scale = area_scale
 
         # get the correction scaling factor
-        self._corr_scale = np.float64(get_field('CORRSCAL', 0.0))
+        # self._corr_scale = np.float64(get_field('CORRSCAL', 0.0))
 
         self._header = header
         self._data = data
         self._counts = self._raw_counts = counts
         self._error = self._raw_error = error
         self._grouping = grouping
         self._exposure = exposure
@@ -1087,33 +1207,33 @@
         return self._respfile
 
     @property
     def ancrfile(self) -> str:
         """Ancillary response file."""
         return self._ancrfile
 
-    @property
-    def corrfile(self) -> str:
-        """Correction file."""
-        return self._corrfile
+    # @property
+    # def corrfile(self) -> str:
+    #     """Correction file."""
+    #     return self._corrfile
 
     @property
     def back_scale(self) -> np.float64 | NDArray:
         """Background scaling factor."""
         return self._back_scale
 
     @property
     def area_scale(self) -> np.float64 | NDArray:
         """Area scaling factor."""
         return self._area_scale
 
-    @property
-    def corr_scale(self) -> np.float64:
-        """Correction scaling factor."""
-        return self._corr_scale
+    # @property
+    # def corr_scale(self) -> np.float64:
+    #     """Correction scaling factor."""
+    #     return self._corr_scale
 
 
 class Response:
     """Handle telescope response in OGIP standards [1]_.
 
     Parameters
     ----------
@@ -1371,47 +1491,94 @@
             n = self._sparse_matrix.shape[1]
             idx = np.arange(n)
             ptr = np.append(grp_idx, n)
             grouping_matrix = csc_array((a, idx, ptr))
             matrix = self._sparse_matrix.dot(grouping_matrix)
             self._matrix = matrix.tocsc()[:, non_empty]
 
-    def plot(self, hatch_range: NDArray | None = None):
+    def plot_effective_area(self, noticed_range: NDArray | None = None):
+        """Plot the response matrix.
+
+        Parameters
+        ----------
+        noticed_range : ndarray, optional
+            Energy range to show. Other energy ranges will be hatched.
+        """
+        eff_area = self._sparse_matrix.sum(axis=1)
+        eff_area = np.clip(eff_area, a_min=0.0, a_max=None)
+
+        plt.figure()
+        plt.rcParams['axes.formatter.min_exponent'] = 3
+        plt.step(self.ph_egrid, np.append(eff_area, eff_area[-1]))
+        plt.xlim(self.ph_egrid[0], self.ph_egrid[-1])
+        plt.xlabel('Photon Energy [keV]')
+        plt.ylabel('Effective Area [cm$^2$]')
+        plt.xscale('log')
+
+        if noticed_range is not None:
+            ph_emin = self.ph_egrid[:-1]
+            ph_emax = self.ph_egrid[1:]
+            noticed_range = np.atleast_2d(noticed_range)
+            emin = np.expand_dims(noticed_range[:, 0], axis=1)
+            emax = np.expand_dims(noticed_range[:, 1], axis=1)
+            mask1 = np.less_equal(emin, ph_emin)
+            mask2 = np.less_equal(ph_emax, emax)
+            idx = [np.flatnonzero(i) for i in np.bitwise_and(mask1, mask2)]
+
+            ignored = []
+            if ph_emin[idx[0][0]] > ph_emin[0]:
+                ignored.append((ph_emin[0], ph_emin[idx[0][0]]))
+            for i in range(len(idx) - 1):
+                this_noticed_right = ph_emax[idx[i][-1]]
+                next_noticed_left = ph_emin[idx[i + 1][0]]
+                ignored.append((this_noticed_right, next_noticed_left))
+            if ph_emax[idx[-1][-1]] < ph_emax[-1]:
+                ignored.append((ph_emax[idx[-1][-1]], ph_emax[-1]))
+
+            ylim = plt.gca().get_ylim()
+            for i in ignored:
+                plt.fill_betweenx(
+                    ylim, *i, alpha=0.8, color='gray', hatch='x', zorder=10
+                )
+            plt.ylim(ylim)
+
+    def plot_matrix(self, noticed_range: NDArray | None = None):
         """Plot the response matrix.
 
         Parameters
         ----------
-        hatch_range : ndarray, optional
-            Energy range to add hatches.
+        noticed_range : ndarray, optional
+            Energy range to show. Other energy ranges will be hatched.
         """
         ch_emin, ch_emax = self._raw_channel_egrid.T
-        matrix = self._sparse_matrix.todense()
+        matrix = np.clip(self._sparse_matrix.todense(), a_min=0.0, a_max=None)
 
         # some response matrix has discontinuity in channel energy grid,
         # insert np.nan to handle this
         idx = np.flatnonzero(ch_emin[1:] - ch_emax[:-1])
         if len(idx) > 0:
             ch_emin = np.insert(ch_emin, idx + 1, ch_emax[idx])
             ch_emax = np.insert(ch_emax, idx + 1, ch_emin[idx + 1])
             matrix = np.insert(matrix, idx + 1, np.nan, axis=1)
 
         ch_egrid = np.append(ch_emin, ch_emax[-1])
         ch, ph = np.meshgrid(ch_egrid, self._ph_egrid)
         plt.figure()
-        plt.pcolormesh(ch, ph, matrix, cmap='jet')
+        plt.rcParams['axes.formatter.min_exponent'] = 3
+        plt.pcolormesh(ch, ph, matrix, cmap='magma')
         plt.xlabel('Measurement Energy [keV]')
         plt.ylabel('Photon Energy [keV]')
         plt.colorbar(label='Effective Area [cm$^2$]')
         plt.xscale('log')
         plt.yscale('log')
 
-        if hatch_range is not None:
-            hatch_range = np.atleast_2d(hatch_range)
-            emin = np.expand_dims(hatch_range[:, 0], axis=1)
-            emax = np.expand_dims(hatch_range[:, 1], axis=1)
+        if noticed_range is not None:
+            noticed_range = np.atleast_2d(noticed_range)
+            emin = np.expand_dims(noticed_range[:, 0], axis=1)
+            emax = np.expand_dims(noticed_range[:, 1], axis=1)
             mask1 = np.less_equal(emin, ch_emin)
             mask2 = np.less_equal(ch_emax, emax)
             idx = [np.flatnonzero(i) for i in np.bitwise_and(mask1, mask2)]
 
             ignored = []
             if ch_emin[idx[0][0]] > ch_emin[0]:
                 ignored.append((ch_emin[0], ch_emin[idx[0][0]]))
```

### Comparing `elisa_lib-0.1.0/src/elisa/infer/data.py` & `elisa_lib-0.1.1/src/elisa/infer/data.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/infer/fit.py` & `elisa_lib-0.1.1/src/elisa/infer/fit.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 import time
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from typing import TYPE_CHECKING
 
 import jax
 import jax.numpy as jnp
+import nautilus
 import numpy as np
 import optimistix as optx
+import ultranest
 from iminuit import Minuit
-from numpyro.infer import MCMC, NUTS, init_to_value
+from numpyro.infer import AIES, MCMC, NUTS, init_to_value
 
 from elisa.data.ogip import Data
 from elisa.infer.data import FitData
 from elisa.infer.helper import Helper, get_helper
 from elisa.infer.likelihood import _STATISTIC_OPTIONS
-from elisa.infer.nested_sampling import NestedSampler
+from elisa.infer.nested_sampling import NestedSampler, reparam_loglike
 from elisa.infer.results import MLEResult, PosteriorResult
 from elisa.models.model import Model, get_model_info
 from elisa.util.misc import add_suffix, build_namespace, make_pretty_table
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Literal
 
@@ -517,14 +519,15 @@
 
     def nuts(
         self,
         warmup=2000,
         samples=20000,
         chains: int | None = None,
         init: dict[str, float] | None = None,
+        chain_method: str = 'parallel',
         progress: bool = True,
         **nuts_kwargs: dict,
     ) -> PosteriorResult:
         """Run the No-U-Turn Sampler of :mod:`numpyro`.
 
         .. note::
             If the chains are not converged well, see ref [1]_ for more
@@ -538,14 +541,16 @@
             Number of samples to generate from each chain.
         chains : int, optional
             Number of MCMC chains to run. If there are not enough devices
             available, chains will run in sequence. Defaults to the number of
             ``jax.local_device_count()``.
         init : dict, optional
             Initial parameter for sampler to start from.
+        chain_method : str, optional
+            The chain method passed to :class:`numpyro.infer.MCMC`.
         progress : bool, optional
             Whether to show progress bar during sampling. The default is True.
         **nuts_kwargs : dict
             Extra parameters passed to :class:`numpyro.infer.NUTS`.
 
         Returns
         -------
@@ -569,39 +574,42 @@
         # the total samples number should be multiple of the device number
         if chains * samples % device_count != 0:
             samples += device_count - samples % device_count
 
         # TODO: option to let sampler starting from MLE
         if init is None:
             init = self._helper.free_default['constr_dic']
+        else:
+            init = self._helper.free_default['constr_dic'] | dict(init)
 
         default_nuts_kwargs = {
             'dense_mass': True,
             'target_accept_prob': 0.8,
             'max_tree_depth': 10,
-            'init_strategy': init_to_value(values=init),
         }
         nuts_kwargs = default_nuts_kwargs | nuts_kwargs
         nuts_kwargs['model'] = self._helper.numpyro_model
+        nuts_kwargs['init_strategy'] = init_to_value(values=init)
 
         sampler = MCMC(
             NUTS(**nuts_kwargs),
             num_warmup=warmup,
             num_samples=samples,
             num_chains=chains,
+            chain_method=chain_method,
             progress_bar=progress,
         )
 
         sampler.run(
             rng_key=jax.random.PRNGKey(self._helper.seed['mcmc']),
             extra_fields=('energy', 'num_steps'),
         )
         return PosteriorResult(sampler, self._helper, self)
 
-    def ns(
+    def jaxns(
         self,
         max_samples: int = 131072,
         num_live_points: int | None = None,
         s: int | None = None,
         k: int | None = None,
         c: int | None = None,
         num_parallel_workers: int = 1,
@@ -685,7 +693,269 @@
         )
 
         print('Start nested sampling...')
         t0 = time.time()
         sampler.run(rng_key=jax.random.PRNGKey(self._helper.seed['mcmc']))
         print(f'Sampling cost {time.time() - t0:.2f} s')
         return PosteriorResult(sampler, self._helper, self)
+
+    def ultranest(
+        self,
+        ess: int = 10000,
+        ignore_nan: bool = True,
+        *,
+        constructor_kwargs: dict | None = None,
+        termination_kwargs: dict | None = None,
+        read_file: dict | None = None,
+    ) -> PosteriorResult:
+        """Run the Nested Sampler of :mod:`ultranest`.
+
+        Parameters
+        ----------
+        ess : int, optional
+            The desired effective sample size.
+        ignore_nan : bool, optional
+            Whether to transform a NaN log probability to a large negative
+            number (-1e300). The default is True.
+
+            .. warning ::
+                Setting ``ignore_nan=True`` may fail to spot potential issues
+                with model computation.
+        constructor_kwargs : dict, optional
+            Extra parameters passed to
+            :class:`ultranest.ReactiveNestedSampler`.
+        termination_kwargs : dict, optional
+            Extra parameters passed to
+            :class:`ultranest.ReactiveNestedSampler.run()`.
+        read_file : dict, optional
+            Read the log file from a previous run. The dictionary should
+            contain the log directory and other optional parameters. It
+            should be noted that when providing this keyword argument, the
+            sampler will not run, but read the log file instead, and make
+            sure the data and model setting is the same as the previous run.
+        """
+        if constructor_kwargs is None:
+            constructor_kwargs = {}
+        else:
+            constructor_kwargs = dict(constructor_kwargs)
+
+        if termination_kwargs is None:
+            termination_kwargs = {}
+        else:
+            termination_kwargs = dict(termination_kwargs)
+
+        log_prob, transform, param_names = reparam_loglike(
+            self._helper.numpyro_model,
+            jax.random.PRNGKey(self._helper.seed['mcmc']),
+        )
+
+        @jax.jit
+        def log_prob_(params):
+            logp = log_prob(dict(zip(param_names, params)))
+            if ignore_nan:
+                return jnp.nan_to_num(logp, nan=-1e300)
+            else:
+                return logp
+
+        @jax.vmap
+        @jax.jit
+        def transform_(samples):
+            base_names = [name + '_base' for name in param_names]
+            return transform(dict(zip(base_names, samples)))
+
+        sampler = ultranest.ReactiveNestedSampler(
+            param_names=param_names, loglike=log_prob_, **constructor_kwargs
+        )
+        sampler._transform_back = transform_
+
+        if read_file is None:
+            print('Start nested sampling...')
+            t0 = time.time()
+            sampler.run(min_ess=int(ess), **termination_kwargs)
+            print(f'Sampling cost {time.time() - t0:.2f} s')
+        else:
+            read_file = dict(read_file)
+            log_dir = read_file['log_dir']
+            verbose = read_file.get('verbose', False)
+            x_dim = sampler.x_dim
+            sequence, final = ultranest.read_file(
+                log_dir, x_dim, verbose=verbose
+            )
+            sampler.results = sequence | final
+        return PosteriorResult(sampler, self._helper, self)
+
+    def nautilus(
+        self,
+        ess: int = 10000,
+        ignore_nan: bool = True,
+        *,
+        constructor_kwargs: dict | None = None,
+        termination_kwargs: dict | None = None,
+    ) -> PosteriorResult:
+        """Run the Nested Sampler of :mod:`nautilus`.
+
+        Parameters
+        ----------
+        ess : int, optional
+            The desired effective sample size.
+        ignore_nan : bool, optional
+            Whether to transform a NaN log probability to a large negative
+            number (-1e300). The default is True.
+
+            .. warning ::
+                Setting ``ignore_nan=True`` may fail to spot potential issues
+                with model computation.
+        constructor_kwargs : dict, optional
+            Extra parameters passed to
+            :class:`nautilus.Sampler`.
+        termination_kwargs : dict, optional
+            Extra parameters passed to
+            :class:`nautilus.Sampler.run()`.
+        """
+        if constructor_kwargs is None:
+            constructor_kwargs = {}
+        else:
+            constructor_kwargs = dict(constructor_kwargs)
+
+        if termination_kwargs is None:
+            termination_kwargs = {}
+        else:
+            termination_kwargs = dict(termination_kwargs)
+
+        log_prob, transform, param_names = reparam_loglike(
+            self._helper.numpyro_model,
+            jax.random.PRNGKey(self._helper.seed['mcmc']),
+        )
+
+        @jax.jit
+        def log_prob_(params):
+            logp = log_prob(dict(zip(param_names, params)))
+            if ignore_nan:
+                return jnp.nan_to_num(logp, nan=-1e300)
+            else:
+                return logp
+
+        @jax.vmap
+        @jax.jit
+        def transform_(samples):
+            base_names = [name + '_base' for name in param_names]
+            return transform(dict(zip(base_names, samples)))
+
+        prior = nautilus.Prior()
+        for param in param_names:
+            prior.add_parameter(param)
+
+        constructor_kwargs['pass_dict'] = False
+        constructor_kwargs['seed'] = self._helper.seed['mcmc']
+        constructor_kwargs['vectorized'] = False
+        constructor_kwargs.setdefault('pool', (None, jax.local_device_count()))
+        sampler = nautilus.Sampler(
+            prior=prior,
+            likelihood=log_prob_,
+            **constructor_kwargs,
+        )
+
+        termination_kwargs['discard_exploration'] = True
+        termination_kwargs.setdefault('verbose', True)
+        print('Start nested sampling...')
+        t0 = time.time()
+        sampler.run(n_eff=int(ess), **termination_kwargs)
+        print(f'Sampling cost {time.time() - t0:.2f} s')
+        sampler._transform_back = transform_
+        return PosteriorResult(sampler, self._helper, self)
+
+    def aies(
+        self,
+        warmup=2000,
+        samples=20000,
+        chains: int | None = None,
+        init: dict[str, float] | None = None,
+        chain_method: str = 'vectorized',
+        progress: bool = True,
+        moves: dict | None = None,
+        **aies_kwargs: dict,
+    ) -> PosteriorResult:
+        """Affine-Invariant Ensemble Sampling (AIES) of :mod:`numpyro`.
+
+        Affine-invariant ensemble sampling [1]_ is a gradient-free method
+        that informs Metropolis-Hastings proposals by sharing information
+        between chains. Suitable for low to moderate dimensional models.
+        Generally, num_chains should be at least twice the dimensionality
+        of the model.
+
+        .. note::
+            This kernel must be used with even `num_chains` > 1 and
+            ``chain_method='vectorized'``.
+
+        Parameters
+        ----------
+        warmup : int, optional
+            Number of warmup steps.
+        samples : int, optional
+            Number of samples to generate from each chain.
+        chains : int, optional
+            Number of MCMC chains to run. Defaults to 4 * `D`, where `D` is
+            the dimension of model parameters.
+        init : dict, optional
+            Initial parameter for sampler to start from.
+        chain_method : str, optional
+            The chain method passed to :class:`numpyro.inf.MCMC`.
+        progress : bool, optional
+            Whether to show progress bar during sampling. The default is True.
+        moves : dict, optional
+            Moves for the sampler.
+        **aies_kwargs : dict
+            Extra parameters passed to :class:`numpyro.infer.AIES`.
+
+        Returns
+        -------
+        PosteriorResult
+            The posterior sampling result.
+
+        References
+        ----------
+        .. [1] *emcee: The MCMC Hammer*
+               (https://iopscience.iop.org/article/10.1086/670067),
+               Daniel Foreman-Mackey, David W. Hogg, Dustin Lang,
+               and Jonathan Goodman.
+        """
+        if chains is None:
+            chains = 4 * len(self._helper.params_names['free'])
+        else:
+            chains = int(chains)
+
+        # TODO: option to let sampler starting from MLE
+        if init is None:
+            init = self._helper.free_default['constr_dic']
+        else:
+            init = self._helper.free_default['constr_dic'] | dict(init)
+        init = self._helper.constr_dic_to_unconstr_arr(init)
+        rng = np.random.default_rng(self._helper.seed['mcmc'])
+        jitter = 0.1 * np.abs(init)
+        low = init - jitter
+        high = init + jitter
+        init = rng.uniform(low, high, size=(chains, len(init)))
+        init = dict(zip(self._helper.params_names['free'], init.T))
+
+        aies_kwargs['model'] = self._helper.numpyro_model
+        if moves is None:
+            aies_kwargs['moves'] = {
+                AIES.DEMove(): 0.5,
+                AIES.StretchMove(): 0.5,
+            }
+        else:
+            aies_kwargs['moves'] = moves
+
+        sampler = MCMC(
+            AIES(**aies_kwargs),
+            num_warmup=warmup,
+            num_samples=samples,
+            num_chains=chains,
+            chain_method=chain_method,
+            progress_bar=progress,
+        )
+
+        sampler.run(
+            rng_key=jax.random.PRNGKey(self._helper.seed['mcmc']),
+            init_params=init,
+        )
+        return PosteriorResult(sampler, self._helper, self)
```

### Comparing `elisa_lib-0.1.0/src/elisa/infer/helper.py` & `elisa_lib-0.1.1/src/elisa/infer/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,22 @@
             jnp.asarray([i.sum(axis=-1) for i in net_counts.values()]), axis=0
         )
 
         return counts_data
 
     # ======================== count data calculator ==========================
 
-    obs_counts = {f'{k}_Non': v.spec_counts for k, v in data.items()}
+    obs_counts = {
+        f'{k}_Non': (
+            v.net_counts
+            if stat[k] in _STATISTIC_SPEC_NORMAL
+            else v.spec_counts
+        )
+        for k, v in data.items()
+    }
     obs_counts |= {
         f'{k}_Noff': v.back_counts
         for k, v in data.items()
         if stat[k] in _STATISTIC_WITH_BACK
     }
     obs_data = get_counts_data(obs_counts)
```

### Comparing `elisa_lib-0.1.0/src/elisa/infer/likelihood.py` & `elisa_lib-0.1.1/src/elisa/infer/likelihood.py`

 * *Files 10% similar despite different names*

```diff
@@ -195,17 +195,20 @@
     eff_expo = jnp.array(data.area_factor * data.spec_exposure, float)
 
     def likelihood(
         params: ParamNameValMapping,
         predictive: bool = False,
     ) -> None:
         """Gaussian likelihood defined via numpyro primitives."""
-        source_rate = resp_matrix @ model(photon_egrid, params)
+        unfold = model(photon_egrid, params)
+        unfold = jnp.clip(unfold, a_min=-1e-300, a_max=1e300)
+        source_rate = resp_matrix @ unfold
         numpyro.deterministic(name, source_rate / channel_width)
         source_counts = source_rate * eff_expo
+        source_counts = jnp.clip(source_counts, a_min=1e-30, a_max=1e15)
         spec_data = numpyro.primitives.mutable(f'{name}_Non_data', spec)
         spec_model = numpyro.deterministic(f'{name}_Non_model', source_counts)
 
         with numpyro.plate(f'{name}_plate', len(spec)):
             dist_on = BetterNormal(spec_model, error)
             numpyro.sample(
                 name=f'{name}_Non',
@@ -236,17 +239,20 @@
     eff_expo = jnp.array(data.area_factor * data.spec_exposure, float)
 
     def likelihood(
         params: ParamNameValMapping,
         predictive: bool = False,
     ) -> None:
         """Poisson likelihood defined via numpyro primitives."""
-        source_rate = resp_matrix @ model(photon_egrid, params)
+        unfold = model(photon_egrid, params)
+        unfold = jnp.clip(unfold, a_min=-1e-300, a_max=1e300)
+        source_rate = resp_matrix @ unfold
         numpyro.deterministic(name, source_rate / channel_width)
         source_counts = source_rate * eff_expo
+        source_counts = jnp.clip(source_counts, a_min=1e-30, a_max=1e15)
         spec_data = numpyro.primitives.mutable(f'{name}_Non_data', spec)
         spec_model = numpyro.deterministic(f'{name}_Non_model', source_counts)
 
         with numpyro.plate(f'{name}_plate', len(spec)):
             dist_on = BetterPoisson(spec_model)
             numpyro.sample(
                 name=f'{name}_Non',
@@ -281,17 +287,20 @@
     back_ratio = jnp.array(data.back_ratio, float)
 
     def likelihood(
         params: ParamNameValMapping,
         predictive: bool = False,
     ) -> None:
         """Poisson likelihood defined via numpyro primitives."""
-        source_rate = resp_matrix @ model(photon_egrid, params)
+        unfold = model(photon_egrid, params)
+        unfold = jnp.clip(unfold, a_min=-1e-300, a_max=1e300)
+        source_rate = resp_matrix @ unfold
         numpyro.deterministic(name, source_rate / channel_width)
         model_counts = source_rate * eff_expo + back_ratio * back
+        model_counts = jnp.clip(model_counts, a_min=1e-30, a_max=1e15)
         spec_data = numpyro.primitives.mutable(f'{name}_Non_data', spec)
         spec_model = numpyro.deterministic(f'{name}_Non_model', model_counts)
 
         with numpyro.plate(f'{name}_plate', len(spec_data)):
             dist_on = BetterPoisson(spec_model)
             numpyro.sample(
                 name=f'{name}_Non',
@@ -326,24 +335,27 @@
     channel_width = jnp.array(data.ch_width, float)
     resp_matrix = _get_resp_matrix(data)
     eff_expo = jnp.array(data.area_factor * data.spec_exposure, float)
     back_ratio = jnp.array(data.back_ratio, float)
 
     def likelihood(params: ParamNameValMapping, predictive: bool = False):
         """Poisson and Gaussian likelihood defined via numpyro primitives."""
-        model_rate = resp_matrix @ model(photon_egrid, params)
-        numpyro.deterministic(name, model_rate / channel_width)
+        unfold = model(photon_egrid, params)
+        unfold = jnp.clip(unfold, a_min=-1e-300, a_max=1e300)
+        source_rate = resp_matrix @ unfold
+        numpyro.deterministic(name, source_rate / channel_width)
         spec_data = numpyro.primitives.mutable(f'{name}_Non_data', spec)
         back_data = numpyro.primitives.mutable(f'{name}_Noff_data', back)
-        source_counts = model_rate * eff_expo
+        source_counts = source_rate * eff_expo
+        source_counts = jnp.clip(source_counts, a_min=1e-30, a_max=1e15)
         b = pgstat_background(
             source_counts, spec_data, back_data, back_error, back_ratio
         )
-        model_counts = source_counts + back_ratio * b
-        spec_model = numpyro.deterministic(f'{name}_Non_model', model_counts)
+        spec_model = source_counts + back_ratio * b
+        spec_model = numpyro.deterministic(f'{name}_Non_model', spec_model)
         back_model = numpyro.deterministic(f'{name}_Noff_model', b)
 
         with numpyro.plate(f'{name}_plate', len(spec_data)):
             dist_on = BetterPoisson(spec_model)
             dist_off = BetterNormal(back_model, back_error)
             numpyro.sample(
                 name=f'{name}_Non',
@@ -387,19 +399,22 @@
     channel_width = jnp.array(data.ch_width, float)
     resp_matrix = _get_resp_matrix(data)
     eff_expo = jnp.array(data.area_factor * data.spec_exposure, float)
     back_ratio = jnp.array(data.back_ratio, float)
 
     def likelihood(params: ParamNameValMapping, predictive: bool = False):
         """Poisson and Poisson likelihood defined via numpyro primitives."""
-        model_rate = resp_matrix @ model(photon_egrid, params)
-        numpyro.deterministic(name, model_rate / channel_width)
+        unfold = model(photon_egrid, params)
+        unfold = jnp.clip(unfold, a_min=-1e-300, a_max=1e300)
+        source_rate = resp_matrix @ unfold
+        numpyro.deterministic(name, source_rate / channel_width)
         spec_data = numpyro.primitives.mutable(f'{name}_Non_data', spec)
         back_data = numpyro.primitives.mutable(f'{name}_Noff_data', back)
-        source_counts = model_rate * eff_expo
+        source_counts = source_rate * eff_expo
+        source_counts = jnp.clip(source_counts, a_min=1e-30, a_max=1e15)
         b = wstat_background(source_counts, spec_data, back_data, back_ratio)
         model_counts = source_counts + back_ratio * b
         spec_model = numpyro.deterministic(f'{name}_Non_model', model_counts)
         back_model = numpyro.deterministic(f'{name}_Noff_model', b)
 
         with numpyro.plate(f'{name}_plate', len(spec_data)):
             dist_on = BetterPoisson(spec_model)
```

### Comparing `elisa_lib-0.1.0/src/elisa/infer/nested_sampling.py` & `elisa_lib-0.1.1/src/elisa/infer/nested_sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,15 +184,16 @@
         :param args: The arguments needed by the `model`.
         :param kwargs: The keyword arguments needed by the `model`.
         """
         from jaxns import DefaultNestedSampler, Model, Prior, TerminationCondition
 
         rng_sampling, rng_predictive = random.split(rng_key)
         # reparam the model so that latent sites have Uniform(0, 1) priors
-        prototype_trace = trace(seed(self.model, rng_key)).get_trace(*args, **kwargs)
+        seeded = jax.jit(seed(self.model, rng_key))
+        prototype_trace = trace(seeded).get_trace(*args, **kwargs)
         param_names = [
             site["name"]
             for site in prototype_trace.values()
             if site["type"] == "sample"
             and not site["is_observed"]
             and site["infer"].get("enumerate", "") != "parallel"
         ]
@@ -265,15 +266,22 @@
         )
 
         default_ns = DefaultNestedSampler(
             model=model,
             **self.constructor_kwargs,
         )
 
-        termination_reason, state = jax.jit(default_ns)(
+        # TODO: check if this is necessary
+        # jit when num_parallel_workers is 1
+        if self.constructor_kwargs['num_parallel_workers'] == 1:
+            run_default_ns = jax.jit(default_ns)
+        else:
+            run_default_ns = default_ns
+
+        termination_reason, state = run_default_ns(
             rng_sampling, term_cond=TerminationCondition(**self.termination_kwargs)
         )
         results = default_ns.to_results(
             termination_reason=termination_reason, state=state
         )
 
         # transform base samples back to original domains
@@ -345,15 +353,16 @@
         plot_diagnostics(self._results)
         plot_cornerplot(self._results)
 
 
 def reparam_loglike(model, rng_key, *args, **kwargs):
     rng_sampling, rng_predictive = random.split(rng_key)
     # reparam the model so that latent sites have Uniform(0, 1) priors
-    prototype_trace = trace(seed(model, rng_key)).get_trace(*args, **kwargs)
+    seeded = jax.jit(seed(model, rng_key))
+    prototype_trace = trace(seeded).get_trace(*args, **kwargs)
     param_names = [
         site['name']
         for site in prototype_trace.values()
         if site['type'] == 'sample'
         and not site['is_observed']
         and site['infer'].get('enumerate', '') != 'parallel'
     ]
@@ -379,34 +388,28 @@
         _validate_model(prototype_trace)
         reparam_model = enum(reparam_model, -max_plate_nesting - 1)
     else:
         log_density_ = log_density
 
     # Jaxns requires loglikelihood function to have explicit signatures.
     local_dict = {}
-    loglik_fn_def = """def loglik_fn({}):\n
-    \tparams = dict({})\n
+    loglik_fn_def = """def loglik_fn(params):\n
+    \tparams = {k + '_base': v for k, v in params.items()}\n
     \treturn log_density_(reparam_model, args, kwargs, params)[0]
-    """.format(
-        ', '.join([f'{name}_base' for name in param_names]),
-        ', '.join([f'{name}_base={name}_base' for name in param_names]),
-    )
+    """
     exec(loglik_fn_def, locals(), local_dict)
+    loglik_fn = local_dict['loglik_fn']
 
     def transform_back(samples):
         predictive = Predictive(
             reparam_model, samples, return_sites=param_names + deterministics
         )
         return predictive(rng_predictive, *args, **kwargs)
 
-    return (
-        local_dict['loglik_fn'],
-        transform_back,
-        [f'{name}_base' for name in param_names],
-    )
+    return local_dict['loglik_fn'], transform_back, param_names
 
 
 class GlobalOptimizer:
     """
     :param callable model: a call with NumPyro primitives
     :param dict constructor_kwargs: additional keyword arguments to construct an upstream
         :class:`jaxns.experimental.DefaultGlobalOptimisation` instance.
```

### Comparing `elisa_lib-0.1.0/src/elisa/infer/results.py` & `elisa_lib-0.1.1/src/elisa/infer/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 from importlib import metadata
 from typing import TYPE_CHECKING, NamedTuple
 
 import arviz as az
 import astropy.units as u
 import jax
 import jax.numpy as jnp
+import nautilus
 import numpy as np
 import numpyro
 import scipy.stats as stats
+import ultranest
 from astropy.cosmology import Planck18
 from iminuit import Minuit
 from jax.experimental.mesh_utils import create_device_mesh
-from jax.sharding import PositionalSharding
+from jax.experimental.shard_map import shard_map
+from jax.sharding import Mesh, PartitionSpec
 from numpyro.infer import MCMC
 
 from elisa.__about__ import __version__
 from elisa.infer.helper import check_params
 from elisa.infer.nested_sampling import NestedSampler
 from elisa.plot.plotter import MLEResultPlotter, PosteriorResultPlotter
 from elisa.util.misc import make_pretty_table
@@ -35,36 +38,33 @@
     from iminuit.util import FMin
 
     from elisa.infer.fit import BayesFit
     from elisa.infer.helper import Helper
     from elisa.plot.plotter import Plotter
     from elisa.util.typing import JAXArray
 
+ReactiveNestedSampler = ultranest.ReactiveNestedSampler
+Sampler = nautilus.Sampler
+
 
 class FitResult(ABC):
     """Fit result."""
 
     _helper: Helper
     _plotter: Plotter | None
     _flux_fn: Callable
     _lumin_fn: Callable
     _eiso_fn: Callable
 
     def __init__(self, helper: Helper):
         self._helper = helper
 
         models = helper.model
-        ne = {
-            name: jax.jit(model.ne, static_argnums=2)
-            for name, model in models.items()
-        }
-        ene = {
-            name: jax.jit(model.ene, static_argnums=2)
-            for name, model in models.items()
-        }
+        ne = {name: model.ne for name, model in models.items()}
+        ene = {name: model.ene for name, model in models.items()}
 
         def _flux(
             egrid: JAXArray,
             params: dict[str, JAXArray],
             energy: bool,
             comps: bool,
         ) -> dict[str, JAXArray] | dict[str, dict[str, JAXArray]]:
@@ -361,26 +361,36 @@
 
         if energy:
             unit = u.erg / u.cm**2 / u.s
         else:
             unit = u.cm**-2 / u.s
 
         mle_params = {k: v[0] for k, v in self._mle.items()}
+        if params is not None:
+            mle_params |= params
         mle_flux = self._flux_fn(egrid, mle_params, energy, comps)
 
         n = [i.size for i in boot_params.values()][0]
         if params is not None:
             params = dict(params)
             params = {k: jnp.full(n, v) for k, v in params.items()}
             boot_params = boot_params | params
         devices = create_device_mesh((jax.local_device_count(),))
-        sharding = PositionalSharding(devices)
-        boot_params = jax.device_put(boot_params, sharding)
-        boot_flux = self._flux_fn(egrid, boot_params, energy, comps)
-        boot_flux = jax.device_get(boot_flux)
+        mesh = Mesh(devices, axis_names=('i',))
+        p = PartitionSpec()
+        pi = PartitionSpec('i')
+        fn = shard_map(
+            f=self._flux_fn,
+            mesh=mesh,
+            in_specs=(p, pi, p, p),
+            out_specs=pi,
+            check_rep=False,
+        )
+        boot_flux = jax.device_get(fn(egrid, boot_params, energy, comps))
+
         cl_ = 1.0 - 2.0 * stats.norm.sf(cl) if cl >= 1.0 else cl
         q = 0.5 + np.array([-0.5, 0.5]) * cl_
         ci_fn = lambda x: np.quantile(x, q)
         intervals = jax.tree_map(ci_fn, boot_flux)
         errors = jax.tree_map(
             lambda x, y: (x - y[0], x - y[1]), mle_flux, intervals
         )
@@ -812,36 +822,46 @@
 
 
 class PosteriorResult(FitResult):
     """Result obtained from Bayesian fit."""
 
     _plotter: PosteriorResultPlotter | None = None
     _idata: az.InferenceData
+    _deviance: dict | None = None
     _mle_result: dict | None = None
     _ppc: PPCResult | None = None
     _loo: az.stats.stats_utils.ELPDData | None = None
     _waic: az.stats.stats_utils.ELPDData | None = None
     _rhat: dict[str, float] | None = None
     _divergence: int | None = None
     _pit: dict[str, tuple] | None = None
     _params: dict[str, JAXArray] | None = None
     _info_tabs: dict | None = None
 
     def __init__(
-        self, sampler: MCMC | NestedSampler, helper: Helper, fit: BayesFit
+        self,
+        sampler: MCMC | NestedSampler | ReactiveNestedSampler | Sampler,
+        helper: Helper,
+        fit: BayesFit,
     ):
-        if not isinstance(sampler, (MCMC, NestedSampler)):
+        if not isinstance(
+            sampler, (MCMC, NestedSampler, ReactiveNestedSampler, Sampler)
+        ):
             raise ValueError(f'unknown sampler type {type(sampler)}')
 
         super().__init__(helper)
         self._fit = fit
         if isinstance(sampler, MCMC):
             self._init_from_numpyro(sampler)
-        else:
+        elif isinstance(sampler, NestedSampler):
             self._init_from_jaxns(sampler)
+        elif isinstance(sampler, ReactiveNestedSampler):
+            self._init_from_ultranest(sampler)
+        else:
+            self._init_from_nautilus(sampler)
 
     def __repr__(self):
         tabs = self._tabs()
         return (
             f'Parameters\n{tabs["params"]}\n\n'
             f'Fit Statistics\n{tabs["stat"]}\n\n'
             f'Information Criterion\n{tabs["ic"]}\n\n'
@@ -868,31 +888,31 @@
             f'<summary><b>Pareto k diagnostic</b></summary>{k_tab}</details>'
             '</details>'
         )
 
     def _tabs(self):
         if self._info_tabs is not None:
             return self._info_tabs
-        params_name = self._helper.params_names['free']
-        params = self._idata['posterior'][params_name]
+        params_name = self._helper.params_names['all']
+        params = self.idata['posterior'][params_name]
         mean = params.mean()
         std = params.std(ddof=1)
         median = params.median()
         ci = params.quantile(0.5 + 0.683 * np.array([-0.5, 0.5])) - median
         ess = self.ess
         rhat = self.rhat
         rows = [
             [
                 k,
                 f'{mean[k]:.4g}',
                 f'{std[k]:.4g}',
                 f'{median[k]:.4g}',
                 f'[{ci[k][0]:.4g}, {ci[k][1]:.4g}]',
                 f'{ess[k]}',
-                f'{rhat[k]:.2f}',
+                f'{rhat[k]:.2f}' if not np.isnan(rhat[k]) else 'N/A',
             ]
             for k in params_name
         ]
         names = [
             'Parameter',
             'Mean',
             'Std',
@@ -900,37 +920,32 @@
             '68.3% Quantile CI',
             'ESS',
             'Rhat',
         ]
         params_tab = make_pretty_table(names, rows)
 
         stat_type = self._helper.statistic
-        stat_keys = [
-            f'{i}_total' if i != 'total' else i for i in self.ndata.keys()
-        ]
-        deviance = -2.0 * self._idata['log_likelihood'][stat_keys]
-        deviance_mean = deviance.mean()
-        deviance_median = deviance.median()
+        deviance = self.deviance
         rows = [
             [
                 i,
                 stat_type[i],
-                f'{deviance_mean[f"{i}_total"]:.2f}',
-                f'{deviance_median[f"{i}_total"]:.2f}',
+                f'{deviance[i]["mean"]:.2f}',
+                f'{deviance[i]["median"]:.2f}',
                 j,
             ]
             for i, j in self.ndata.items()
             if i != 'total'
         ]
         rows.append(
             [
                 'Total',
                 'stat/dof',
-                f'{deviance_mean["total"]:.2f}/{self.dof}',
-                f'{deviance_median["total"]:.2f}/{self.dof}',
+                f'{deviance["total"]["mean"]:.2f}/{self.dof}',
+                f'{deviance["total"]["median"]:.2f}/{self.dof}',
                 self.ndata['total'],
             ]
         )
         names = [
             'Data',
             'Statistic',
             'Mean',
@@ -1011,26 +1026,26 @@
             raise ValueError('cl must be non-negative')
 
         params = check_params(params, self._helper)
 
         cl_ = 1.0 - 2.0 * stats.norm.sf(cl) if cl >= 1.0 else cl
 
         if hdi:
-            median = self._idata['posterior'].median()
+            median = self.idata['posterior'].median()
             median = {
                 k: float(v) for k, v in median.data_vars.items() if k in params
             }
-            interval = az.hdi(self._idata, cl_, var_names=params)
+            interval = az.hdi(self.idata, cl_, var_names=params)
             interval = {
                 k: (float(v[0]), float(v[1]))
                 for k, v in interval.data_vars.items()
             }
         else:
             q = [0.5, 0.5 - cl_ / 2.0, 0.5 + cl_ / 2.0]
-            quantile = self._idata['posterior'].quantile(q)
+            quantile = self.idata['posterior'].quantile(q)
             quantile = {
                 k: v for k, v in quantile.data_vars.items() if k in params
             }
             median = {k: float(v[0]) for k, v in quantile.items()}
             interval = {
                 k: (float(v[1]), float(v[2])) for k, v in quantile.items()
             }
@@ -1065,19 +1080,25 @@
         post = self._params_dist
         n = [i.size for i in post.values()][0]
         if params is not None:
             params = dict(params)
             params = {k: jnp.full(n, v) for k, v in params.items()}
             post = post | params
         devices = create_device_mesh((jax.local_device_count(),))
-        sharding = PositionalSharding(devices)
-        post = jax.device_put(post, sharding)
-
-        flux = self._flux_fn(egrid, post, energy, comps)
-        flux = jax.device_get(flux)
+        mesh = Mesh(devices, axis_names=('i',))
+        p = PartitionSpec()
+        pi = PartitionSpec('i')
+        fn = shard_map(
+            f=self._flux_fn,
+            mesh=mesh,
+            in_specs=(p, pi, p, p),
+            out_specs=pi,
+            check_rep=False,
+        )
+        flux = jax.device_get(fn(egrid, post, energy, comps))
         cl_ = 1.0 - 2.0 * stats.norm.sf(cl) if cl >= 1.0 else cl
         if hdi:
             ci_fn = lambda x: az.hdi(x, cl_)
         else:
             q = 0.5 + np.array([-0.5, 0.5]) * cl_
             ci_fn = lambda x: np.quantile(x, q)
         median = jax.tree_map(lambda x: np.median(x), flux)
@@ -1353,15 +1374,15 @@
         helper = self._helper
         free_params = helper.params_names['free']
         n = int(n)
         seed = helper.seed['pred'] if seed is None else int(seed)
 
         # randomly select n samples from posterior
         rng = np.random.default_rng(seed)
-        idata = self._idata
+        idata = self.idata
         i = rng.integers(0, idata['posterior'].chain.size, n)
         j = rng.integers(0, idata['posterior'].draw.size, n)
         params = {
             k: v.values[i, j]
             for k, v in idata['posterior'][free_params].data_vars.items()
         }
         models = {
@@ -1408,16 +1429,16 @@
         """MLE result."""
         if self._mle_result is None:
             mle_result = {}
             helper = self._helper
 
             # MLE information of the model
             free_params = helper.params_names['free']
-            mle_idx = self._idata['log_likelihood']['total'].argmax(...)
-            init = self._idata['posterior'][free_params].sel(**mle_idx)
+            mle_idx = self.idata['log_likelihood']['total'].argmax(...)
+            init = self.idata['posterior'][free_params].sel(**mle_idx)
             init = {k: v.values for k, v in init.data_vars.items()}
             init = helper.constr_dic_to_unconstr_arr(init)
             mle_unconstr = self._fit._optimize_lm(init, throw=False)[0]
 
             # MLE of model params in constrained space
             mle, cov = jax.device_get(helper.get_mle(mle_unconstr))
             err = np.sqrt(np.diagonal(cov))
@@ -1452,15 +1473,15 @@
     @property
     def _params_dist(self) -> dict[str, JAXArray]:
         """Posterior parameters, the size is truncated to <= nmax."""
         if self._params is not None:
             return self._params
 
         nmax = 10000
-        post = self._idata['posterior'][self._helper.params_names['free']]
+        post = self.idata['posterior'][self._helper.params_names['free']]
         n = post.chain.size * post.draw.size
         if n > nmax:
             n = nmax - nmax % jax.local_device_count()
             rng = np.random.default_rng(self._helper.seed['mcmc'])
             i = rng.integers(0, post.chain.size, n)
             j = rng.integers(0, post.draw.size, n)
             post = {k: v.values[i, j] for k, v in post.items()}
@@ -1531,20 +1552,79 @@
             'inference_library': 'jaxns',
             'inference_library_version': metadata.version('jaxns'),
         }
 
         self._generate_idata(samples, attrs)
 
         # effective sample size
-        self._ess = {'total': int(result.ESS)}
+        ess = int(result.ESS)
+        self._ess = {p: ess for p in self._helper.params_names['all']}
         # relative mcmc efficiency
-        self._reff = float(result.ESS / result.total_num_samples)
+        self._reff = float(ess / result.total_num_samples)
         # model evidence
         self._lnZ = (float(result.log_Z_mean), float(result.log_Z_uncert))
 
+    def _init_from_ultranest(self, sampler: ReactiveNestedSampler):
+        result = sampler._transform_back(sampler.results['samples'])
+        nsamples = len(sampler.results['samples'])
+        ncores = jax.local_device_count()
+        ndrop = nsamples % ncores
+
+        # get posterior samples
+        samples = jax.tree_map(lambda x: x[None, : nsamples - ndrop], result)
+
+        # attrs for each group of arviz.InferenceData
+        attrs = {
+            'elisa_version': __version__,
+            'inference_library': 'ultranest',
+            'inference_library_version': ultranest.__version__,
+        }
+
+        self._generate_idata(samples, attrs)
+
+        # effective sample size
+        ess = int(sampler.results['ess'])
+        self._ess = {p: ess for p in self._helper.params_names['all']}
+        # relative mcmc efficiency
+        self._reff = float(ess / nsamples)
+        # model evidence
+        self._lnZ = (
+            float(sampler.results['logz']),
+            float(sampler.results['logzerr']),
+        )
+
+    def _init_from_nautilus(self, sampler: Sampler):
+        result = sampler.posterior(equal_weight=True)[0]
+        result = sampler._transform_back(result)
+        ncores = jax.local_device_count()
+
+        # get posterior samples
+        samples = jax.tree_map(
+            lambda x: x[None, : len(x) - len(x) % ncores],
+            result,
+        )
+
+        # attrs for each group of arviz.InferenceData
+        attrs = {
+            'elisa_version': __version__,
+            'inference_library': 'nautilus',
+            'inference_library_version': nautilus.__version__,
+        }
+
+        self._generate_idata(samples, attrs)
+
+        # effective sample size
+        ess = int(sampler.n_eff)
+        self._ess = {p: ess for p in self._helper.params_names['all']}
+        # relative mcmc efficiency
+        total_sample = len(sampler.posterior(equal_weight=False)[0])
+        self._reff = float(ess / total_sample)
+        # model evidence
+        self._lnZ = (float(sampler.log_z), None)
+
     def _generate_idata(self, samples, attrs, sample_stats=None):
         samples = jax.tree_map(jax.device_get, samples)
         helper = self._helper
 
         params = helper.get_params(samples)
         models = helper.get_models(samples)
         posterior = params | models
@@ -1586,14 +1666,36 @@
             posterior_predictive_attrs=attrs,
             sample_stats_attrs=attrs,
             log_likelihood_attrs=attrs,
             observed_data_attrs=attrs,
         )
 
     @property
+    def deviance(self) -> dict:
+        """Mean and median of model deviance."""
+        if self._deviance is None:
+            stat_keys = {
+                i: f'{i}_total' if i != 'total' else i
+                for i in self.ndata.keys()
+            }
+            keys = list(stat_keys.values())
+            deviance = -2.0 * self.idata['log_likelihood'][keys]
+            deviance_mean = deviance.mean()
+            deviance_median = deviance.median()
+            self._deviance = {
+                k: {
+                    'mean': float(deviance_mean[v]),
+                    'median': float(deviance_median[v]),
+                }
+                for k, v in stat_keys.items()
+            }
+
+        return self._deviance
+
+    @property
     def reff(self) -> float:
         """Relative MCMC efficiency."""
         return self._reff
 
     @property
     def ess(self) -> dict[str, int]:
         """Effective MCMC sample size."""
@@ -1608,16 +1710,16 @@
         more information.
 
         References
         ----------
         .. [1] https://arxiv.org/abs/1903.08008
         """
         if self._rhat is None:
-            params_names = self._helper.params_names['free']
-            posterior = self._idata['posterior'][params_names]
+            params_names = self._helper.params_names['all']
+            posterior = self.idata['posterior'][params_names]
 
             if len(posterior['chain']) == 1:
                 rhat = {k: float('nan') for k in posterior.data_vars.keys()}
             else:
                 rhat = {
                     k: float(v.values)
                     for k, v in az.rhat(posterior).data_vars.items()
@@ -1627,16 +1729,16 @@
 
         return self._rhat
 
     @property
     def divergence(self) -> int:
         """Number of divergent samples."""
         if self._divergence is None:
-            if 'sample_stats' in self._idata:
-                n = int(self._idata['sample_stats']['diverging'].sum())
+            if 'sample_stats' in self.idata:
+                n = int(self.idata['sample_stats']['diverging'].sum())
             else:
                 n = 0
 
             self._divergence = n
 
         return self._divergence
 
@@ -1651,15 +1753,15 @@
         References
         ----------
         .. [1] https://arxiv.org/abs/1507.04544
         .. [2] https://arxiv.org/abs/1004.2316
         """
         if self._waic is None:
             self._waic = az.waic(
-                self._idata, var_name='channels', scale='deviance'
+                self.idata, var_name='channels', scale='deviance'
             )
 
         return self._waic
 
     @property
     def loo(self) -> ELPDData:
         """Pareto-smoothed importance sampling leave-one-out cross-validation
@@ -1673,15 +1775,15 @@
         ----------
         .. [1] https://avehtari.github.io/modelselection/CV-FAQ.html
         .. [2] https://arxiv.org/abs/1507.04544
         .. [3] https://arxiv.org/abs/1507.02646
         """
         if self._loo is None:
             self._loo = az.loo(
-                self._idata,
+                self.idata,
                 var_name='channels',
                 reff=self.reff,
                 scale='deviance',
             )
 
         return self._loo
 
@@ -1692,15 +1794,15 @@
 
     @property
     def _loo_pit(self) -> dict[str, tuple]:
         """Leave-one-out probability integral transform."""
         if self._pit is not None:
             return self._pit
 
-        idata = self._idata
+        idata = self.idata
         reff = self.reff
         helper = self._helper
         stack_kwargs = {'__sample__': ('chain', 'draw')}
         log_weights, kss = az.psislw(
             -idata['log_likelihood']['channels'].stack(**stack_kwargs), reff
         )
         y_hat = idata['posterior_predictive']['channels'].stack(**stack_kwargs)
```

### Comparing `elisa_lib-0.1.0/src/elisa/models/__init__.py` & `elisa_lib-0.1.1/src/elisa/models/__init__.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/models/add.py` & `elisa_lib-0.1.1/src/elisa/models/add.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/models/conv.py` & `elisa_lib-0.1.1/src/elisa/models/conv.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/models/model.py` & `elisa_lib-0.1.1/src/elisa/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,15 +859,15 @@
         if config is not None and '__init__' not in dct:
             # signature of __init__ method
             sig1 = [
                 f"{i[0]}: 'Parameter' | float | None = None" for i in config
             ]
             sig1 += ['latex: str | None = None']
 
-            params = '{%s}' % ', '.join(f"'{i[0]}': {i[0]}" for i in config)
+            params = '{' + ', '.join(f"'{i[0]}': {i[0]}" for i in config) + '}'
 
             # signature of super().__init__ method
             sig2 = [f'params={params}', 'latex=latex']
 
             if args := getattr(cls, '_args', None):
                 sig1 = [f'{i}' for i in args] + sig1
                 sig2 = [f'{i}={i}' for i in args] + sig2
@@ -1060,15 +1060,15 @@
     _staticmethod: tuple[str, ...] = ()  # methods need to be static
     __initialized: bool = False
 
     def __init__(self, params: dict, latex: str | None):
         self._id = hex(id(self))[2:]
 
         if latex is None:
-            latex = r'\mathrm{%s}' % self.__class__.__name__
+            latex = rf'\mathrm{{{self.__class__.__name__}}}'
         self.latex = latex
 
         self._name = self.__class__.__name__
 
         # parse parameters from params, which is a dict of parameters
         for cfg in self._config:
             setattr(self, cfg.name, params[cfg.name])
```

### Comparing `elisa_lib-0.1.0/src/elisa/models/mul.py` & `elisa_lib-0.1.1/src/elisa/models/mul.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/models/parameter.py` & `elisa_lib-0.1.1/src/elisa/models/parameter.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/models/xspec.py` & `elisa_lib-0.1.1/src/elisa/models/xspec.py`

 * *Files 6% similar despite different names*

```diff
@@ -217,29 +217,29 @@
         def extend_low(egrid):
             if egrid[0] < elow:
                 raise RuntimeError(
                     f'the lower limit ({elow}) of the energy extension must '
                     f'be less than the minimum energy grid ({egrid[0]})'
                 )
             if loglow:
-                low_extension = np.geomspace(elow, egrid[0], nlow)
+                low_extension = np.geomspace(elow, egrid[0], nlow + 1)[:-1]
             else:
-                low_extension = np.linspace(elow, egrid[0], nlow)
+                low_extension = np.linspace(elow, egrid[0], nlow + 1)[:-1]
             return np.concatenate((low_extension, egrid)).astype(egrid.dtype)
 
         def extend_high(egrid):
             if egrid[-1] > ehigh:
                 raise RuntimeError(
                     f'the upper limit ({ehigh}) of the energy extension must '
                     f'be greater than the maximum energy grid ({egrid[-1]})'
                 )
             if loghigh:
-                high_extension = np.geomspace(egrid[-1], ehigh, nhigh)
+                high_extension = np.geomspace(egrid[-1], ehigh, nhigh + 1)[1:]
             else:
-                high_extension = np.linspace(egrid[-1], ehigh, nhigh)
+                high_extension = np.linspace(egrid[-1], ehigh, nhigh + 1)[1:]
             return np.concatenate((egrid, high_extension)).astype(egrid.dtype)
 
         def fn(egrid: JAXArray, params: CompIDParamValMapping) -> JAXArray:
             """The convolved model evaluation function."""
             rtype = jax.ShapeDtypeStruct((egrid.size + nlow,), egrid.dtype)
             egrid = jax.pure_callback(extend_low, rtype, egrid)
             rtype = jax.ShapeDtypeStruct((egrid.size + nhigh,), egrid.dtype)
@@ -327,39 +327,14 @@
 
     @property
     @abstractmethod
     def _convolve(self) -> XspecConvolveEval:
         pass
 
 
-# class cflux(XspecConvolution):
-#     _supported = frozenset({'add'})
-#     _config = (
-#         ParamConfig(
-#             'emin', r'\mathrm{emin}', 'keV', 1.0, 1e-10, 1e10, fixed=1
-#         ),
-#         ParamConfig(
-#             'emax', r'\mathrm{emax}', 'keV', 10.0, 1e-10, 1e10, fixed=1
-#         ),
-#         ParamConfig('log10F', r'\mathrm{F}', '', -12, -100, 100),
-#     )
-#
-#     @property
-#     def _convolve(self):
-#         spec_num = self.spec_num
-#         params_names = [p.name for p in self._config]
-#         fn = _XSMODEL['primitive']['cflux']
-#
-#         def cflux(egrid, params, flux):
-#             params = jnp.stack([params[p] for p in params_names])
-#             return fn(params, egrid, flux, spec_num)
-#
-#         return cflux
-
-
 def create_xspec_components():
     """Create Xspec model classes."""
     if not _HAS_XSPEC:
         return {}
 
     template = '''
 class {name}({component_class}):
```

### Comparing `elisa_lib-0.1.0/src/elisa/models/tables/generate_xsect_table.py` & `elisa_lib-0.1.1/src/elisa/models/tables/generate_xsect_table.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/models/tables/xsect.hdf5` & `elisa_lib-0.1.1/src/elisa/models/tables/xsect.hdf5`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/plot/data.py` & `elisa_lib-0.1.1/src/elisa/plot/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from typing import TYPE_CHECKING
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import scipy.stats as stats
 from jax.experimental.mesh_utils import create_device_mesh
-from jax.sharding import PositionalSharding
+from jax.experimental.shard_map import shard_map
+from jax.sharding import Mesh, PartitionSpec
 
 from elisa.infer.likelihood import (
     _STATISTIC_BACK_NORMAL,
     _STATISTIC_SPEC_NORMAL,
     _STATISTIC_WITH_BACK,
 )
 from elisa.plot.residuals import (
     pearson_residuals,
     pit_poisson,
     pit_poisson_normal,
     pit_poisson_poisson,
+    quantile_residuals_poisson,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
     from typing import Any, Callable, Literal
 
     from elisa.infer.results import (
@@ -115,28 +117,16 @@
 
         for f, fields in self._cached_method_with_check:
             method = getattr(self, f)
             setattr(self, f, _cache_method_with_check(self, method, fields))
 
         model = self.result._helper.model[self.name]
         self._ne = jax.jit(model.ne, static_argnums=2)
-        self._ne_vmap = jax.jit(
-            jax.vmap(self._ne, in_axes=(None, 0, None)),
-            static_argnums=2,
-        )
         self._ene = jax.jit(model.ene, static_argnums=2)
-        self._ene_vmap = jax.jit(
-            jax.vmap(self._ene, in_axes=(None, 0, None)),
-            static_argnums=2,
-        )
         self._eene = jax.jit(model.eene, static_argnums=2)
-        self._eene_vmap = jax.jit(
-            jax.vmap(self._eene, in_axes=(None, 0, None)),
-            static_argnums=2,
-        )
 
     @property
     def channel(self) -> NumPyArray:
         return self.data.channel
 
     @property
     def ch_emin(self) -> NumPyArray:
@@ -235,20 +225,27 @@
         self,
         mtype: Literal['ne', 'ene', 'eene'],
         egrid: Array,
         params: dict,
         comps: bool,
     ) -> Array | dict:
         assert mtype in {'ne', 'ene', 'eene'}
-        v = '_vmap' if len(np.shape(list(params.values())[0])) != 0 else ''
-        if v:
+        fn = getattr(self, f'_{mtype}')
+        if len(np.shape(list(params.values())[0])) != 0:
             devices = create_device_mesh((jax.local_device_count(),))
-            sharding = PositionalSharding(devices)
-            params = jax.device_put(params, sharding)
-        fn = getattr(self, f'_{mtype}{v}')
+            mesh = Mesh(devices, axis_names=('i',))
+            p = PartitionSpec()
+            pi = PartitionSpec('i')
+            fn = shard_map(
+                f=fn,
+                mesh=mesh,
+                in_specs=(p, pi, p),
+                out_specs=pi,
+                check_rep=False,
+            )
         return jax.device_get(fn(egrid, params, comps))
 
     @abstractmethod
     def unfolded_model(
         self,
         mtype: Literal['ne', 'ene', 'eene'],
         egrid: Array,
@@ -618,15 +615,36 @@
 
         if random:
             pit = np.random.default_rng(seed).uniform(pit_minus, pit)
         r = stats.norm.ppf(pit)
 
         lower = upper = False
 
-        if self.statistic in {'pgstat', 'wstat'}:
+        if self.statistic == 'chi2':
+            mask = (pit == 0.0) | (pit == 1.0)
+            if np.any(mask):
+                on_data = self.net_counts[mask]
+                on_model = self.on_models['mle'][mask]
+                error = self.net_error[mask]
+                r[mask] = (on_data - on_model) / error
+
+        elif self.statistic in {'cstat', 'pstat'}:
+            mask = (pit == 0.0) | (pit == 1.0)
+            if np.any(mask):
+                on_data = self.spec_counts[mask]
+                on_model = self.on_models['mle'][mask]
+                r[mask] = quantile_residuals_poisson(
+                    on_data,
+                    on_model,
+                    keep_sign=not random,
+                    random=random,
+                    seed=seed,
+                )
+
+        elif self.statistic in {'pgstat', 'wstat'}:
             upper_mask = pit == 0.0
             if np.any(upper_mask):
                 r[upper_mask] = stats.norm.ppf(1.0 / self._nsim)
                 upper = np.full(r.shape, False)
                 upper[upper_mask] = True
 
             lower_mask = pit == 1.0
```

### Comparing `elisa_lib-0.1.0/src/elisa/plot/errorbars.py` & `elisa_lib-0.1.1/src/elisa/plot/errorbars.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/plot/misc.py` & `elisa_lib-0.1.1/src/elisa/plot/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,39 @@
     get_contour_colors,
 )
 from elisa.util.misc import report_interval
 
 
 def plot_corner(
     idata: az.InferenceData,
+    bins: int | Sequence[int] = 40,
+    hist_bin_factor: float | Sequence[float] = 1.5,
     params: str | Sequence[str] | None = None,
     axes_scale: str | Sequence[str] = 'linear',
     levels: float | Sequence[float] | None = None,
     titles: str | Sequence[str] | None = None,
     labels: str | Sequence[str] | None = None,
     color: str = None,
     divergences: bool = True,
 ):
     """Plot posterior corner plot.
 
     Parameters
     ----------
     idata : az.InferenceData
         arviz.InferenceData object.
+    bins : int or list of int, optional
+        The number of bins to use in histograms, either as a fixed value for
+        all dimensions, or as a list of integers for each dimension.
+        The default is 40.
+    hist_bin_factor : float or list of float, optional
+        This is a factor (or list of factors, one for each dimension) that
+        will multiply the bin specifications when making the 1-D histograms.
+        This is generally used to increase the number of bins in the 1-D
+        plots to provide more resolution. The default is 1.5.
     params : str or list of str, optional
         One or more parameters to be plotted.
     axes_scale : str, or list of str, optional
         Scale to use for each parameter dimension. If only one scale is given,
         use that for all dimensions. Scale must be ``'linear'`` or ``'log'``.
     levels : float, or list of float, optional
         Credible levels to plot. If None, use 0.683 and 0.95.
@@ -120,18 +131,18 @@
         color = str(color)
 
     plt.rcParams['axes.formatter.min_exponent'] = 3
     c1, c2 = get_contour_colors(color, len(levels), 0.8, 2.0)
 
     fig = corner.corner(
         idata,
-        bins=40,
+        bins=bins,
         axes_scale=axes_scale,
         color=color,
-        hist_bin_factor=1.5,
+        hist_bin_factor=hist_bin_factor,
         titles=titles,
         labels=labels,
         show_titles=True,
         title_fmt=None,
         quantiles=[0.15865, 0.5, 0.84135],
         use_math_text=True,
         labelpad=-0.08,
```

### Comparing `elisa_lib-0.1.0/src/elisa/plot/plotter.py` & `elisa_lib-0.1.1/src/elisa/plot/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1323,24 +1323,36 @@
         }
         return data
 
     def plot_corner(
         self,
         params: str | Sequence[str] | None = None,
         color: str | None = None,
+        bins: int | Sequence[int] = 40,
+        hist_bin_factor: float | Sequence[float] = 1.5,
         fig_path: str | None = None,
     ) -> Figure:
         """Corner plot of bootstrap parameters.
 
         Parameters
         ----------
         params : str or sequence of str, optional
             Parameters to plot. The default is all spectral parameters.
         color : str, optional
             Color of the plot. The default is ``None``.
+        bins : int or list of int, optional
+            The number of bins to use in histograms, either as a fixed value
+            for all dimensions, or as a list of integers for each dimension.
+            The default is 40.
+        hist_bin_factor : float or list of float, optional
+            This is a factor (or list of factors, one for each dimension)
+            that will multiply the bin specifications when making the 1-D
+            histograms. This is generally used to increase the number of
+            bins in the 1-D plots to provide more resolution.
+            The default is 1.5.
         fig_path : str, optional
             Path to save the figure. The default is ``None``.
 
         Returns
         -------
         Figure
             The Figure object containing corner plot.
@@ -1353,14 +1365,16 @@
         axes_scale = [
             'log' if helper.params_log[p] else 'linear' for p in params
         ]
         params_titles = self.params_titles
         params_labels = self.params_labels
         fig = plot_corner(
             idata=az.from_dict(self._result._boot.params),
+            bins=bins,
+            hist_bin_factor=hist_bin_factor,
             params=params,
             axes_scale=axes_scale,
             levels=self.config.cl,
             titles=[params_titles[p] for p in params],
             labels=[params_labels[p] for p in params],
             color=color,
         )
@@ -1523,26 +1537,38 @@
         return fig
 
     def plot_corner(
         self,
         params: str | Sequence[str] | None = None,
         color: str | None = None,
         divergences: bool = True,
+        bins: int | Sequence[int] = 40,
+        hist_bin_factor: float | Sequence[float] = 1.5,
         fig_path: str | None = None,
     ) -> Figure:
         """Corner plot of posterior parameters.
 
         Parameters
         ----------
         params : str or sequence of str, optional
             Parameters to plot. The default is all spectral parameters.
         color : str, optional
             Color of the plot. The default is ``None``.
         divergences : bool, optional
             Whether to show divergent samples. The default is ``True``.
+        bins : int or list of int, optional
+            The number of bins to use in histograms, either as a fixed value
+            for all dimensions, or as a list of integers for each dimension.
+            The default is 40.
+        hist_bin_factor : float or list of float, optional
+            This is a factor (or list of factors, one for each dimension)
+            that will multiply the bin specifications when making the 1-D
+            histograms. This is generally used to increase the number of
+            bins in the 1-D plots to provide more resolution.
+            The default is 1.5.
         fig_path : str, optional
             Path to save the figure. The default is ``None``.
 
         Returns
         -------
         Figure
             The Figure object containing corner plot.
@@ -1552,14 +1578,16 @@
         axes_scale = [
             'log' if helper.params_log[p] else 'linear' for p in params
         ]
         params_titles = self.params_titles
         params_labels = self.params_labels
         fig = plot_corner(
             idata=self._result._idata,
+            bins=bins,
+            hist_bin_factor=hist_bin_factor,
             params=params,
             axes_scale=axes_scale,
             levels=self.config.cl,
             titles=[params_titles[p] for p in params],
             labels=[params_labels[p] for p in params],
             color=color,
             divergences=divergences,
```

### Comparing `elisa_lib-0.1.0/src/elisa/plot/residuals.py` & `elisa_lib-0.1.1/src/elisa/plot/residuals.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,16 +160,24 @@
         cdf_left = poisson.cdf(k1 - 1, lam1)  # when k < 0, poisson cdf is 0
         sf_right = sf
         sf_left = poisson.sf(k2 - 1, lam2)  # when k < 0, poisson sf is 1
         cdf = rng.uniform(cdf_left, cdf_right)
         sf = rng.uniform(sf_right, sf_left)
 
     r = np.empty(lam_shape)
-    r[mask1] = norm.ppf(cdf)
-    r[mask2] = norm.isf(sf)
+    r[mask1] = np.where(
+        cdf != 0.0,
+        norm.ppf(cdf),
+        (k1 - lam1) / np.sqrt(lam1),
+    )
+    r[mask2] = np.where(
+        sf != 0.0,
+        norm.isf(sf),
+        (k2 - lam2) / np.sqrt(lam2),
+    )
 
     if keep_sign:
         r = np.where(k >= lam, 1.0, -1.0) * np.abs(r)
 
     return r
```

### Comparing `elisa_lib-0.1.0/src/elisa/plot/scale.py` & `elisa_lib-0.1.1/src/elisa/plot/scale.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/plot/util.py` & `elisa_lib-0.1.1/src/elisa/plot/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from elisa.util.typing import NumPyArray as NDArray
 
 
 def get_colors(
     n: int, palette: str = 'husl'
 ) -> list[tuple[float, float, float]]:
-    if len(colors := sns.color_palette(palette)) <= n:
+    if len(colors := sns.color_palette(palette)) >= n:
         return colors[:n]
     else:
         return sns.color_palette(palette, n)
 
 
 def get_markers(n: int) -> list[str]:
     markers_cycle = cycle(['s', 'o', 'D', '^', 'd', 'p', 'h', 'H', 'D'])
```

### Comparing `elisa_lib-0.1.0/src/elisa/util/bslogu.py` & `elisa_lib-0.1.1/src/elisa/util/bslogu.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/util/config.py` & `elisa_lib-0.1.1/src/elisa/util/config.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/util/integrate.py` & `elisa_lib-0.1.1/src/elisa/util/integrate.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/util/misc.py` & `elisa_lib-0.1.1/src/elisa/util/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,14 @@
 
         tvals, _ = tree_util.tree_flatten(params_tangent)
         if any(jnp.shape(v) != () for v in tvals):
             raise NotImplementedError(
                 'JVP for non-scalar parameter is not implemented'
             )
 
-        params = lax.stop_gradient(params)
         non_zero_tangents = [not isinstance(v, SymbolicZero) for v in tvals]
         idx = [i for i, v in enumerate(non_zero_tangents) if v]
         idx_arr = jnp.array(idx)
         nbatch = sum(non_zero_tangents)
         nparam = len(tvals)
         params_ravel, revert = ravel_pytree(params)
         free_params_values = params_ravel[idx_arr]
```

### Comparing `elisa_lib-0.1.0/src/elisa/util/scipy_nquad.py` & `elisa_lib-0.1.1/src/elisa/util/scipy_nquad.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/src/elisa/util/typing.py` & `elisa_lib-0.1.1/src/elisa/util/typing.py`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/.gitignore` & `elisa_lib-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/LICENSE` & `elisa_lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elisa_lib-0.1.0/pyproject.toml` & `elisa_lib-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,40 +23,47 @@
 dependencies = [
     "arviz",
     "astropy>=5.3",
     "corner>=2.2.2",
     "h5py",
     "iminuit",
     "jax>=0.4.5",
+    "jaxlib>=0.4.5",
     "jaxns>=2.4.8",
     "matplotlib",
+    "nautilus-sampler",
     "numpy",
-    "numpyro",
+    "numpyro>=0.14.0",
     "optimistix",
     "prettytable",
     "quadax>=0.2.1",
     "scipy>=1.11.0, <=1.12.0",
     "seaborn",
     "tinygp",
     "tqdm",
+    "ultranest",
 ]
 
 
 [project.optional-dependencies]
 xspec = ["xspex"]
 test = ["pytest", "pytest-cov", "coverage[toml]"]
 docs = [
+    "ipywidgets",
+    "jupyter",
+    "jupyterlab_widgets",
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-book-theme",
     "sphinx-copybutton",
     "sphinx-design",
     "myst-nb",
     "numba",
     "numpydoc",
+    "widgetsnbextension",
 ]
 dev = ["pre-commit>=3.6.0", "ruff>=2.0"]
 
 
 [project.urls]
 Documentation = "https://github.com/wcxve/elisa#readme"
 Issues = "https://github.com/wcxve/elisa/issues"
```

