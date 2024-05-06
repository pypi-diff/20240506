# Comparing `tmp/formio-data-1.2.6.tar.gz` & `tmp/formio-data-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formio-data-1.2.6.tar", max compression
+gzip compressed data, was "formio-data-1.2.7.tar", max compression
```

## Comparing `formio-data-1.2.6.tar` & `formio-data-1.2.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1066 2023-09-27 12:28:17.714676 formio-data-1.2.6/LICENSE
--rw-r--r--   0        0        0     8499 2024-01-16 09:09:25.600101 formio-data-1.2.6/README.md
--rw-r--r--   0        0        0     4736 2024-01-11 14:12:33.194134 formio-data-1.2.6/formiodata/builder.py
--rw-r--r--   0        0        0       94 2023-09-27 12:28:17.714676 formio-data-1.2.6/formiodata/components/__init__.py
--rw-r--r--   0        0        0     1805 2023-09-27 12:28:17.714676 formio-data-1.2.6/formiodata/components/address.py
--rw-r--r--   0        0        0      320 2024-01-11 14:09:14.416354 formio-data-1.2.6/formiodata/components/button.py
--rw-r--r--   0        0        0      175 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/checkbox.py
--rw-r--r--   0        0        0     2917 2024-01-11 14:10:30.519038 formio-data-1.2.6/formiodata/components/columns.py
--rw-r--r--   0        0        0    10317 2024-01-11 14:07:40.751507 formio-data-1.2.6/formiodata/components/component.py
--rw-r--r--   0        0        0      223 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/content.py
--rw-r--r--   0        0        0      175 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/currency.py
--rw-r--r--   0        0        0      240 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/datagrid.py
--rw-r--r--   0        0        0     6852 2024-01-16 09:12:34.918694 formio-data-1.2.6/formiodata/components/datetime.py
--rw-r--r--   0        0        0     2962 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/day.py
--rw-r--r--   0        0        0      271 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/editgrid.py
--rw-r--r--   0        0        0      172 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/email.py
--rw-r--r--   0        0        0      716 2024-01-11 14:09:06.731284 formio-data-1.2.6/formiodata/components/fieldset.py
--rw-r--r--   0        0        0     1151 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/file.py
--rw-r--r--   0        0        0     4794 2024-01-11 14:08:20.521867 formio-data-1.2.6/formiodata/components/grid_base.py
--rw-r--r--   0        0        0      311 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/htmlelement.py
--rw-r--r--   0        0        0      177 2023-09-27 12:28:17.715676 formio-data-1.2.6/formiodata/components/layout_base.py
--rw-r--r--   0        0        0      173 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/number.py
--rw-r--r--   0        0        0      994 2024-01-11 14:11:18.215465 formio-data-1.2.6/formiodata/components/panel.py
--rw-r--r--   0        0        0      175 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/password.py
--rw-r--r--   0        0        0      178 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/phoneNumber.py
--rw-r--r--   0        0        0      178 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/phone_number.py
--rw-r--r--   0        0        0     1395 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/radio.py
--rw-r--r--   0        0        0     2287 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/resource.py
--rw-r--r--   0        0        0     1656 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/select.py
--rw-r--r--   0        0        0     1226 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/selectboxes.py
--rw-r--r--   0        0        0      176 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/signature.py
--rw-r--r--   0        0        0     1998 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/survey.py
--rw-r--r--   0        0        0     1232 2024-01-11 14:09:50.463678 formio-data-1.2.6/formiodata/components/table.py
--rw-r--r--   0        0        0      978 2024-01-11 14:11:40.746666 formio-data-1.2.6/formiodata/components/tabs.py
--rw-r--r--   0        0        0      175 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/textarea.py
--rw-r--r--   0        0        0      176 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/textfield.py
--rw-r--r--   0        0        0      171 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/time.py
--rw-r--r--   0        0        0      170 2023-09-27 12:28:17.716676 formio-data-1.2.6/formiodata/components/url.py
--rw-r--r--   0        0        0     5284 2024-01-11 14:12:22.263036 formio-data-1.2.6/formiodata/form.py
--rw-r--r--   0        0        0      979 2023-09-27 12:28:17.717676 formio-data-1.2.6/formiodata/utils.py
--rw-r--r--   0        0        0      541 2024-01-16 09:14:36.749652 formio-data-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     9765 2024-01-16 09:21:56.171638 formio-data-1.2.6/setup.py
--rw-r--r--   0        0        0     9275 2024-01-16 09:21:56.172095 formio-data-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-09-27 12:28:17.714676 formio-data-1.2.7/LICENSE
+-rw-r--r--   0        0        0     8499 2024-01-16 09:09:25.600101 formio-data-1.2.7/README.md
+-rw-r--r--   0        0        0     4736 2024-01-11 14:12:33.194134 formio-data-1.2.7/formiodata/builder.py
+-rw-r--r--   0        0        0       94 2023-09-27 12:28:17.714676 formio-data-1.2.7/formiodata/components/__init__.py
+-rw-r--r--   0        0        0     1805 2023-09-27 12:28:17.714676 formio-data-1.2.7/formiodata/components/address.py
+-rw-r--r--   0        0        0      320 2024-01-11 14:09:14.416354 formio-data-1.2.7/formiodata/components/button.py
+-rw-r--r--   0        0        0      175 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/checkbox.py
+-rw-r--r--   0        0        0     2917 2024-01-11 14:10:30.519038 formio-data-1.2.7/formiodata/components/columns.py
+-rw-r--r--   0        0        0    10317 2024-01-11 14:07:40.751507 formio-data-1.2.7/formiodata/components/component.py
+-rw-r--r--   0        0        0      223 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/content.py
+-rw-r--r--   0        0        0      175 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/currency.py
+-rw-r--r--   0        0        0      240 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/datagrid.py
+-rw-r--r--   0        0        0     6840 2024-05-05 10:54:22.148439 formio-data-1.2.7/formiodata/components/datetime.py
+-rw-r--r--   0        0        0     2962 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/day.py
+-rw-r--r--   0        0        0      271 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/editgrid.py
+-rw-r--r--   0        0        0      172 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/email.py
+-rw-r--r--   0        0        0      716 2024-01-11 14:09:06.731284 formio-data-1.2.7/formiodata/components/fieldset.py
+-rw-r--r--   0        0        0     1151 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/file.py
+-rw-r--r--   0        0        0     4794 2024-01-11 14:08:20.521867 formio-data-1.2.7/formiodata/components/grid_base.py
+-rw-r--r--   0        0        0      311 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/htmlelement.py
+-rw-r--r--   0        0        0      177 2023-09-27 12:28:17.715676 formio-data-1.2.7/formiodata/components/layout_base.py
+-rw-r--r--   0        0        0      173 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/number.py
+-rw-r--r--   0        0        0      994 2024-01-11 14:11:18.215465 formio-data-1.2.7/formiodata/components/panel.py
+-rw-r--r--   0        0        0      175 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/password.py
+-rw-r--r--   0        0        0      178 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/phoneNumber.py
+-rw-r--r--   0        0        0      178 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/phone_number.py
+-rw-r--r--   0        0        0     1395 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/radio.py
+-rw-r--r--   0        0        0     2287 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/resource.py
+-rw-r--r--   0        0        0     1656 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/select.py
+-rw-r--r--   0        0        0     1226 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/selectboxes.py
+-rw-r--r--   0        0        0      176 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/signature.py
+-rw-r--r--   0        0        0     1998 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/survey.py
+-rw-r--r--   0        0        0     1232 2024-01-11 14:09:50.463678 formio-data-1.2.7/formiodata/components/table.py
+-rw-r--r--   0        0        0      978 2024-01-11 14:11:40.746666 formio-data-1.2.7/formiodata/components/tabs.py
+-rw-r--r--   0        0        0      175 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/textarea.py
+-rw-r--r--   0        0        0      176 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/textfield.py
+-rw-r--r--   0        0        0      171 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/time.py
+-rw-r--r--   0        0        0      170 2023-09-27 12:28:17.716676 formio-data-1.2.7/formiodata/components/url.py
+-rw-r--r--   0        0        0     5284 2024-01-11 14:12:22.263036 formio-data-1.2.7/formiodata/form.py
+-rw-r--r--   0        0        0      979 2023-09-27 12:28:17.717676 formio-data-1.2.7/formiodata/utils.py
+-rw-r--r--   0        0        0      541 2024-05-05 12:42:02.373935 formio-data-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     9765 2024-05-05 12:47:45.405329 formio-data-1.2.7/setup.py
+-rw-r--r--   0        0        0     9275 2024-05-05 12:47:45.405800 formio-data-1.2.7/PKG-INFO
```

### Comparing `formio-data-1.2.6/LICENSE` & `formio-data-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/README.md` & `formio-data-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/builder.py` & `formio-data-1.2.7/formiodata/builder.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/address.py` & `formio-data-1.2.7/formiodata/components/address.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/columns.py` & `formio-data-1.2.7/formiodata/components/columns.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/component.py` & `formio-data-1.2.7/formiodata/components/component.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/datetime.py` & `formio-data-1.2.7/formiodata/components/datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                     for fm_formio, fm_py in mapping.items():
                         # fm_formio are (JS) uibDateParser codes, see comment
                         # in _format_mappings
                         if not done_date_part and fm_formio in dt_format:
                             py_format = py_format.replace(fm_formio, fm_py)
                             done_date_part = True
                 py_dt = datetime.strptime(value, py_format)
-                val = datetime.fromisoformat(py_dt)
+                val = py_dt.isoformat()
                 super(self.__class__, self.__class__).value.fset(self, val)
             return
         else:
             dt = self._fromisoformat(value)
             py_dt_format = formio_dt_format = component.raw.get('format')
             mapping = self._format_mappings()
```

### Comparing `formio-data-1.2.6/formiodata/components/day.py` & `formio-data-1.2.7/formiodata/components/day.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/fieldset.py` & `formio-data-1.2.7/formiodata/components/fieldset.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/file.py` & `formio-data-1.2.7/formiodata/components/file.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/grid_base.py` & `formio-data-1.2.7/formiodata/components/grid_base.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/panel.py` & `formio-data-1.2.7/formiodata/components/panel.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/radio.py` & `formio-data-1.2.7/formiodata/components/radio.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/resource.py` & `formio-data-1.2.7/formiodata/components/resource.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/select.py` & `formio-data-1.2.7/formiodata/components/select.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/selectboxes.py` & `formio-data-1.2.7/formiodata/components/selectboxes.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/survey.py` & `formio-data-1.2.7/formiodata/components/survey.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/table.py` & `formio-data-1.2.7/formiodata/components/table.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/components/tabs.py` & `formio-data-1.2.7/formiodata/components/tabs.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/form.py` & `formio-data-1.2.7/formiodata/form.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/formiodata/utils.py` & `formio-data-1.2.7/formiodata/utils.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.2.6/pyproject.toml` & `formio-data-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formio-data"
-version = "1.2.6"
+version = "1.2.7"
 homepage = "https://github.com/novacode-nl/python-formio-data"
 description = "formio.js JSON-data API"
 readme = "README.md"
 authors = ["Bob Leers <bob@novacode.nl>"]
 license = "MIT"
 packages = [ { include = "formiodata/**/*.py" } ]
 exclude = ["tests/*"]
```

### Comparing `formio-data-1.2.6/setup.py` & `formio-data-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {':python_version <= "3.6"': ['python-dateutil>=2.8.2,<3.0.0'],
  'json_logic': ['json_logic_qubit>=0.9.1,<0.10.0']}
 
 setup_kwargs = {
     'name': 'formio-data',
-    'version': '1.2.6',
+    'version': '1.2.7',
     'description': 'formio.js JSON-data API',
     'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.\\\nIt\'s main aim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\n\'2009-10-16\'\n\n>> print(form.input_components[\'birthday\'].to_date())\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.to_datetime(), fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n###################\n# validation errors\n###################\n\n>> print(form.validation_errors())\n{\n    \'companyName\': \'Company Name is required\',\n    \'editgridActivities\': [\n        {\'description\': \'Description is required\'},\n        {},  # no validation error (row 2)\n        {},  # no validation error (row 3)\n        {\'description\': \'Description is required\', \'startDate\': \'Start Date is required\'}\n    ]\n}\n\n#############################\n# component path (properties)\n#############################\n\n# datagrid input\n>> datagridMeasurements = builder.components[\'datagridMeasurements\']\n\n# builder_path\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path)\n>>     for row in datagridMeasurements.rows\n>> ]\n[<panelComponent>, <columnsComponent>, <datagridComponent>, <datetimeComponent>]\n\n# builder_path_key\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'pageMeasurements\', \'columnsExternal\', \'datagridMeasurements\', \'measurementDatetime\']\n\n# builder_path_labels\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Page Measurements\', \'Columns External\', \'Data Grid Measurements\', \'Measurement Datetime\']\n\n# builder_input_path\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path)\n>>     for row in datagridMeasurements.rows\n>> ]\n[<datagridComponent>, <datetimeComponent>]\n\n# builder_input_path_key\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'datagridMeasurements\', \'measurementDatetime\']\n\n# builder_input_path_labels\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Data Grid Measurements\', \'Measurement Datetime\']\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n\n##########################\n# components class mapping\n##########################\n\n# Below an example which verbosely shows the feature:\n# - First set a custom component type \'custom_editgrid\' in the Builder JSON schema.\n# - Check (assert) whether the component object is an instance of the mapped editgridComponent.\n# This code is also present in the unittest (file): tests/test_component_class_mapping.py\n\nschema_dict = json.loads(self.builder_json)\n\n# change \'editgrid\' type to \'custom_editgrid\'\nfor comp in schema_dict[\'components\']:\n    if comp[\'key\'] == \'editGrid\':\n        comp[\'type\'] = \'custom_editgrid\'\n\ncomponent_class_mapping = {\'custom_editgrid\': editgridComponent}\nbuilder = Builder(\n    schema_json,\n    component_class_mapping=component_class_mapping,\n)\n\ncustom_editgrid = builder.components[\'editGrid\']\nself.assertIsInstance(custom_editgrid, editgridComponent)\nself.assertEqual(custom_editgrid.type, \'custom_editgrid\')\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `fileStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
     'author': 'Bob Leers',
     'author_email': 'bob@novacode.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/novacode-nl/python-formio-data',
```

### Comparing `formio-data-1.2.6/PKG-INFO` & `formio-data-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formio-data
-Version: 1.2.6
+Version: 1.2.7
 Summary: formio.js JSON-data API
 Home-page: https://github.com/novacode-nl/python-formio-data
 License: MIT
 Author: Bob Leers
 Author-email: bob@novacode.nl
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

