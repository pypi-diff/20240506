# Comparing `tmp/ludic-0.4.1.tar.gz` & `tmp/ludic-0.4.2.tar.gz`

## Comparing `ludic-0.4.1.tar` & `ludic-0.4.2.tar`

### file list

```diff
@@ -1,82 +1,83 @@
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.1/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.1/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/catalog.md
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/getting-started.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/click_to_load.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/__init__.py
--rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/attrs.py
--rw-r--r--   0        0        0    10080 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/components.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/format.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/forms.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/headers.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/items.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/tables.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/typography.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/collect.py
--rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/themes.py
--rw-r--r--   0        0        0    22939 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/types.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/__init__.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/parsers.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/responses.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_components.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/styles/test_styles.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.1/LICENCE
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.1/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.2/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.2/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/catalog.md
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/getting-started.md
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/click_to_load.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/__init__.py
+-rw-r--r--   0        0        0    16478 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/attrs.py
+-rw-r--r--   0        0        0    10138 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/components.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/format.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/headers.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/items.py
+-rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/collect.py
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/themes.py
+-rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/responses.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_components.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.2/LICENCE
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.2/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.2/PKG-INFO
```

### Comparing `ludic-0.4.1/.pre-commit-config.yaml` & `ludic-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/CONTRIBUTING.md` & `ludic-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/mkdocs.yaml` & `ludic-0.4.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/.github/workflows/publish.yaml` & `ludic-0.4.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/.github/workflows/test.yaml` & `ludic-0.4.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/catalog.md` & `ludic-0.4.2/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/components.md` & `ludic-0.4.2/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/getting-started.md` & `ludic-0.4.2/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/htmx.md` & `ludic-0.4.2/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/index.md` & `ludic-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/styles.md` & `ludic-0.4.2/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/web-framework.md` & `ludic-0.4.2/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/docs/assets/ludic.png` & `ludic-0.4.2/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/README.md` & `ludic-0.4.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/__init__.py` & `ludic-0.4.2/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/bulk_update.py` & `ludic-0.4.2/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/click_to_edit.py` & `ludic-0.4.2/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/click_to_load.py` & `ludic-0.4.2/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/delete_row.py` & `ludic-0.4.2/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/edit_row.py` & `ludic-0.4.2/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/infinite_scroll.py` & `ludic-0.4.2/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/examples/lazy_loading.py` & `ludic-0.4.2/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/attrs.py` & `ludic-0.4.2/ludic/attrs.py`

 * *Files 3% similar despite different names*

```diff
@@ -468,14 +468,49 @@
 
 
 class SvgAttrs(GlobalAttrs, total=False):
     version: str
     xmlns: str
     height: int
     width: int
+    view_box: Annotated[str, Alias("viewBox")]
+    clip_path: Annotated[str, Alias("clip-path")]
+    clip_rule: Annotated[str, Alias("clip-rule")]
+    fill: str
+    fill_rule: Annotated[str, Alias("fill-rule")]
+    stroke: str
+    stroke_dasharray: Annotated[str, Alias("stroke-dasharray")]
+    stroke_dashoffset: Annotated[str, Alias("stroke-dashoffset")]
+    stroke_linecap: Annotated[str, Alias("stroke-linecap")]
+    stroke_linejoin: Annotated[str, Alias("stroke-linejoin")]
+    stroke_miterlimit: Annotated[str, Alias("stroke-miterlimit")]
+    stroke_opacity: Annotated[str, Alias("stroke-opacity")]
+    stroke_width: Annotated[str, Alias("stroke-width")]
+    transform: str
+
+
+class CircleAttrs(SvgAttrs, total=False):
+    cx: str
+    cy: str
+    r: str
+
+
+class LineAttrs(SvgAttrs, total=False):
+    x1: str
+    x2: str
+    y1: str
+    y2: str
+
+
+class PathAttrs(SvgAttrs, total=False):
+    d: str
+
+
+class PolylineAttrs(SvgAttrs, total=False):
+    points: str
 
 
 class IframeAttrs(GlobalAttrs, total=False):
     allow: str
     allowfullscreen: bool
     allowpaymentrequest: bool
     height: int
```

### Comparing `ludic-0.4.1/ludic/base.py` & `ludic-0.4.2/ludic/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,15 +127,18 @@
 
         if classes:
             if "class" in attrs:
                 attrs["class"] += " " + " ".join(classes)
             else:
                 attrs["class"] = " ".join(classes)
 
-        return " ".join(f'{key}="{value}"' for key, value in attrs.items())
+        return " ".join(
+            f'{key}="{value}"' if '"' not in value else f"{key}='{value}'"
+            for key, value in attrs.items()
+        )
 
     def _format_children(
         self,
         format_fun: Callable[[Any], str] = format_element,
     ) -> str:
         formatted = []
         for child in self.children:
@@ -214,28 +217,28 @@
 
         while dom != (rendered_dom := dom.render()):
             rendered_dom.context.update(dom.context)
             dom = rendered_dom
             classes += dom.classes
 
         element_tag = f"{dom.html_header}\n" if dom.html_header else ""
+        children_str = dom._format_children() if dom.children else ""
 
-        hidden = dom.html_name == "__hidden__"
-        element_tag += "" if hidden else f"<{dom.html_name}"
+        if dom.html_name == "__hidden__":
+            element_tag += children_str
+            return element_tag
 
-        if not hidden and (dom.has_attributes() or classes):
+        element_tag += f"<{dom.html_name}"
+        if dom.has_attributes() or classes:
             attributes_str = dom._format_attributes(classes, is_html=True)
             element_tag += f" {attributes_str}"
 
         if dom.children or dom.always_pair:
-            children_str = dom._format_children()
-            element_tag += (
-                children_str if hidden else f">{children_str}</{dom.html_name}>"
-            )
-        elif not hidden:
+            element_tag += f">{children_str}</{dom.html_name}>"
+        else:
             element_tag += " />"
 
         return element_tag
 
     def attrs_for(self, cls: type["BaseElement"]) -> dict[str, Any]:
         """Get the attributes of this component that are defined in the given element.
```

### Comparing `ludic-0.4.1/ludic/components.py` & `ludic-0.4.2/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/format.py` & `ludic-0.4.2/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/html.py` & `ludic-0.4.2/ludic/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .attrs import (
     AreaAttrs,
     AudioAttrs,
     BaseAttrs,
     BlockquoteAttrs,
     ButtonAttrs,
     CanvasAttrs,
+    CircleAttrs,
     ColAttrs,
     DataAttrs,
     DelAttrs,
     DetailsAttrs,
     DialogAttrs,
     EmbedAttrs,
     FieldsetAttrs,
@@ -23,24 +24,27 @@
     HyperlinkAttrs,
     IframeAttrs,
     ImgAttrs,
     InputAttrs,
     InsAttrs,
     LabelAttrs,
     LiAttrs,
+    LineAttrs,
     MapAttrs,
     MetaAttrs,
     MeterAttrs,
     NoAttrs,
     ObjectAttrs,
     OlAttrs,
     OptgroupAttrs,
     OptionAttrs,
     OutputAttrs,
     ParamAttrs,
+    PathAttrs,
+    PolylineAttrs,
     ProgressAttrs,
     QAttrs,
     ScriptAttrs,
     SelectAttrs,
     SourceAttrs,
     StyleAttrs,
     SvgAttrs,
@@ -198,14 +202,30 @@
     html_name = "img"
 
 
 class svg(Element[AnyChildren, SvgAttrs]):
     html_name = "svg"
 
 
+class circle(Element[AnyChildren, CircleAttrs]):
+    html_name = "circle"
+
+
+class line(Element[AnyChildren, LineAttrs]):
+    html_name = "line"
+
+
+class path(Element[AnyChildren, PathAttrs]):
+    html_name = "path"
+
+
+class polyline(Element[AnyChildren, PolylineAttrs]):
+    html_name = "polyline"
+
+
 class b(Element[AnyChildren, GlobalAttrs]):
     html_name = "b"
 
 
 class i(Element[AnyChildren, GlobalAttrs]):
     html_name = "i"
```

### Comparing `ludic-0.4.1/ludic/types.py` & `ludic-0.4.2/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/utils.py` & `ludic-0.4.2/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/catalog/buttons.py` & `ludic-0.4.2/ludic/catalog/buttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         lambda theme: {
             (".btn.link", ".box .btn.link"): {
                 "color": theme.colors.dark,
                 "background": "none",
                 "border": "none",
                 "text-decoration": "none",
                 "display": "inline-block",
+                "line-height": 1,
             },
             (".btn.link.active", ".btn.link.active:hover"): {
                 "background-color": theme.colors.light,
             },
             (".box .btn.link.active", ".box .btn.link.active:hover"): {
                 "color": theme.colors.light,
                 "background-color": theme.colors.dark,
```

### Comparing `ludic-0.4.1/ludic/catalog/forms.py` & `ludic-0.4.2/ludic/catalog/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                     "display": "block",
                     "font-weight": "bold",
                     "margin": f"{theme.sizes.xxxs} 0 {theme.sizes.xxs}",
                 },
                 "input": {
                     "inline-size": "100%",
                     "padding": f"{theme.sizes.xxxs} {theme.sizes.xs}",
-                    "border": f"1px solid {theme.colors.light.darken(0.2)}",
+                    "border": f"1px solid {theme.colors.light.darken(2)}",
                     "border-radius": theme.rounding.normal,
                     "box-sizing": "border-box",
                     "font-size": theme.fonts.size * 0.9,
                 },
             }
         }
     )
```

### Comparing `ludic-0.4.1/ludic/catalog/headers.py` & `ludic-0.4.2/ludic/catalog/headers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     """Component representing a clickable anchor."""
 
     classes = ["anchor"]
     styles = style.use(
         lambda theme: {
             "a.anchor": {
                 "font-family": theme.fonts.serif,
-                "font-size": theme.fonts.size * 2.5,
-                "color": theme.colors.light.darken(0.1),
+                "color": theme.colors.light.darken(1),
                 "text-decoration": "none",
             },
             "a.anchor:hover": {
                 "color": theme.colors.dark,
                 "text-decoration": "none",
             },
         }
@@ -34,98 +33,119 @@
     def render(self) -> a:
         return a(
             self.children[0] if self.children else "#", href=f"#{self.attrs["target"]}"
         )
 
 
 class WithAnchorAttrs(GlobalAttrs, total=False):
-    anchor: Anchor
+    anchor: Anchor | bool
 
 
 class WithAnchor(ComponentStrict[h1 | h2 | h3 | h4 | str, WithAnchorAttrs]):
     """Component which renders its content (header) with a clickable anchor."""
 
     classes = ["with-anchor"]
     styles = style.use(
         lambda theme: {
             ".with-anchor": {
                 "display": "flex",
                 "flex-wrap": "wrap",
                 "justify-content": "flex-start",
             },
+            ".with-anchor > h1 + a": {
+                "margin-inline-start": theme.sizes.m,
+                "font-size": theme.headers.h1.size,
+            },
             ".with-anchor > h2 + a": {
                 "margin-inline-start": theme.sizes.s,
+                "font-size": theme.headers.h2.size,
+            },
+            ".with-anchor > h3 + a": {
+                "margin-inline-start": theme.sizes.xs,
+                "font-size": theme.headers.h3.size,
+            },
+            ".with-anchor > h4 + a": {
+                "margin-inline-start": theme.sizes.xxs,
+                "font-size": theme.headers.h4.size,
             },
         }
     )
 
     @override
     def render(self) -> div:
         element: h1 | h2 | h3 | h4
-        if isinstance(self.children[0], str):
-            element = h1(self.children[0])
-        else:
+        if isinstance(self.children[0], h1 | h2 | h3 | h4):
             element = self.children[0]
+        else:
+            element = h1(*self.children)
 
         element.attrs.setdefault("id", text_to_kebab(element.text))
         id = element.attrs["id"]
 
         return div(
             element,
-            (self.attrs["anchor"] if "anchor" in self.attrs else Anchor(target=id)),
+            (
+                self.attrs["anchor"]
+                if isinstance(self.attrs.get("anchor"), Anchor)
+                else Anchor(target=id)
+            ),
         )
 
 
 class H1(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h1 with an optional clickable anchor."""
 
     @override
     def render(self) -> h1 | WithAnchor:
-        header = h1(self.children[0], **self.attrs_for(h1))
-        if anchor := self.attrs.get("anchor"):
+        header = h1(*self.children, **self.attrs_for(h1))
+        anchor = self.attrs.get("anchor")
+        if anchor:
             return WithAnchor(header, anchor=anchor)
-        elif self.theme.headers.h1.anchor:
+        elif self.theme.headers.h1.anchor and anchor is not False:
             return WithAnchor(header)
         else:
             return header
 
 
 class H2(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h2 with an optional clickable anchor."""
 
     @override
     def render(self) -> h2 | WithAnchor:
-        header = h2(self.children[0], **self.attrs_for(h2))
-        if anchor := self.attrs.get("anchor"):
+        header = h2(*self.children, **self.attrs_for(h2))
+        anchor = self.attrs.get("anchor")
+        if anchor:
             return WithAnchor(header, anchor=anchor)
-        elif self.theme.headers.h2.anchor:
+        elif self.theme.headers.h2.anchor and anchor is not False:
             return WithAnchor(header)
         else:
             return header
 
 
 class H3(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h3 with an optional clickable anchor."""
 
     @override
     def render(self) -> h3 | WithAnchor:
-        header = h3(self.children[0], **self.attrs_for(h3))
-        if anchor := self.attrs.get("anchor"):
+        header = h3(*self.children, **self.attrs_for(h3))
+        anchor = self.attrs.get("anchor")
+        if anchor:
             return WithAnchor(header, anchor=anchor)
-        elif self.theme.headers.h3.anchor:
+        elif self.theme.headers.h3.anchor and anchor is not False:
             return WithAnchor(header)
         else:
             return header
 
 
 class H4(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h4 with an optional clickable anchor."""
 
     @override
     def render(self) -> h4 | WithAnchor:
-        header = h4(self.children[0], **self.attrs_for(h4))
-        if anchor := self.attrs.get("anchor"):
+        header = h4(*self.children, **self.attrs_for(h4))
+        anchor = self.attrs.get("anchor")
+        if anchor:
             return WithAnchor(header, anchor=anchor)
-        elif self.theme.headers.h4.anchor:
+        elif self.theme.headers.h4.anchor and anchor is not False:
             return WithAnchor(header)
         else:
             return header
```

### Comparing `ludic-0.4.1/ludic/catalog/items.py` & `ludic-0.4.2/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/catalog/layouts.py` & `ludic-0.4.2/ludic/catalog/layouts.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         lambda theme: {
             ".box": {
                 "padding": theme.sizes.xl,
                 "color": theme.colors.dark,
             },
             ".box:not(.transparent)": {
                 "border": (
-                    f"{theme.borders.thin} solid {theme.colors.light.darken(0.05)}"
+                    f"{theme.borders.thin} solid {theme.colors.light.darken(1)}"
                 ),
                 "border-radius": theme.rounding.more,
                 "background-color": theme.colors.light,
             },
             ".box:not(.transparent) *": {
                 "color": "inherit",
             },
@@ -140,15 +140,15 @@
             ".cluster": {
                 "display": "flex",
                 "flex-wrap": "wrap",
                 "gap": theme.sizes.l,
                 "justify-content": "flex-start",
                 "align-items": "center",
             },
-            ".cluster.center": {
+            ".cluster.centered": {
                 "justify-content": "center",
             },
             ".cluster.flex-end": {
                 "justify-content": "flex-end",
             },
             ".cluster.small": {
                 "gap": theme.sizes.xxs,
@@ -186,15 +186,15 @@
 
     classes = ["with-sidebar"]
     styles = style.use(
         lambda theme: {
             ".with-sidebar": {
                 "display": "flex",
                 "flex-wrap": "wrap",
-                "gap": theme.sizes.xxl,
+                "gap": theme.sizes.xxxxl,
             },
             ".with-sidebar > .sidebar": (
                 {
                     "flex-basis": theme.layouts.sidebar.side_width,
                     "flex-grow": 1,
                 }
                 if theme.layouts.sidebar.side_width
```

### Comparing `ludic-0.4.1/ludic/catalog/lists.py` & `ludic-0.4.2/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/catalog/loaders.py` & `ludic-0.4.2/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/catalog/navigation.py` & `ludic-0.4.2/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/catalog/pages.py` & `ludic-0.4.2/ludic/catalog/pages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+import json
 from typing import override
 
 from ludic.attrs import Attrs, NoAttrs
-from ludic.html import body, head, html, script, style, title
-from ludic.types import AnyChildren, Component, ComponentStrict
+from ludic.html import body, head, html, link, meta, script, style, title
+from ludic.types import AnyChildren, BaseElement, Component, ComponentStrict
 
 
 class HtmlHeadAttrs(Attrs, total=False):
     title: str
+    favicon: str
+    load_styles: bool
+    htmx_config: dict[str, str]
 
 
 class HtmlBodyAttrs(Attrs, total=False):
     htmx_path: str
     htmx_enabled: bool
     htmx_version: str
 
 
 class Head(Component[AnyChildren, HtmlHeadAttrs]):
     @override
     def render(self) -> head:
-        return head(
-            title(self.attrs.get("title", "Ludic App")),
-            style.load(cache=True),
-            *self.children,
-        )
+        elements: list[BaseElement] = [title(self.attrs.get("title", "Ludic App"))]
+
+        if favicon := self.attrs.get("favicon"):
+            elements.append(link(rel="icon", href=favicon, type="image/x-icon"))
+        if config := self.attrs.get("htmx_config", {"defaultSwapStyle": "outerHTML"}):
+            elements.append(meta(name="htmx-config", content=json.dumps(config)))
+        if self.attrs.get("load_styles", True):
+            elements.append(style.load(cache=True))
+
+        return head(*elements, *self.children)
 
 
 class Body(Component[AnyChildren, HtmlBodyAttrs]):
     @override
     def render(self) -> body:
         scripts = []
         if htmx_path := self.attrs.get("htmx_path"):
@@ -77,26 +86,25 @@
                 "font-family": theme.fonts.serif,
             },
             "h6": {
                 "font-size": theme.headers.h6.size,
                 "font-family": theme.fonts.serif,
             },
             "a": {
-                "color": theme.colors.primary.darken(0.3),
+                "color": theme.colors.primary.darken(2),
                 "text-decoration": "none",
             },
             "a:hover": {
                 "text-decoration": "underline",
             },
             "pre": {
                 "overflow": "auto",
             },
             ("code", "pre", "pre *"): {
                 "font-family": theme.fonts.mono,
-                "font-size": theme.fonts.size * 0.9,
             },
             "dl": {
                 "margin-block": "0",
             },
             "dl dt": {
                 "margin-block-start": theme.sizes.xxs,
             },
@@ -106,21 +114,27 @@
             "dt": {
                 "font-weight": "bold",
             },
             "dd": {
                 "margin-left": "0",
             },
             ("ul", "ol"): {
-                "padding-inline-start": theme.sizes.xl,
+                "padding-inline-start": theme.sizes.xxl,
+            },
+            ("ul > li + li", "ol > li + li", "li > * + *"): {
+                "margin-block-start": theme.sizes.xs,
+            },
+            "ul > li::marker": {
+                "font-size": theme.fonts.size * 1.2,
             },
             ("img", "svg"): {
                 "width": "100%",
             },
             "button": {
-                "line-height": theme.line_height - 0.2,
+                "line-height": 1,
             },
             # utilities
             ".text-align-center": {
                 "text-align": "center",
             },
             ".text-align-right": {
                 "text-align": "right",
```

### Comparing `ludic-0.4.1/ludic/catalog/quotes.py` & `ludic-0.4.2/ludic/catalog/quotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,29 @@
     classes = ["quote"]
     styles = style.use(
         lambda theme: {
             ".quote": {
                 "blockquote": {
                     "background-color": theme.colors.light,
                     "border-left": (
-                        f"{theme.borders.thick} solid {theme.colors.light.darken(0.05)}"
+                        f"{theme.borders.thick} solid {theme.colors.light.darken(1)}"
                     ),
                     "margin-bottom": theme.sizes.xxs,
                     "padding": f"{theme.sizes.l} {theme.sizes.m}",
                 },
                 "blockquote p": {
                     "font-size": theme.fonts.size,
                 },
                 "footer": {
                     "font-size": theme.fonts.size * 0.9,
-                    "color": theme.colors.dark.lighten(0.5),
+                    "color": theme.colors.dark.lighten(1),
                 },
                 "footer a": {
                     "text-decoration": "none",
-                    "color": theme.colors.dark.darken(0.5),
+                    "color": theme.colors.dark.darken(1),
                 },
                 "footer a:hover": {
                     "text-decoration": "underline",
                 },
             }
         }
     )
```

### Comparing `ludic-0.4.1/ludic/catalog/tables.py` & `ludic-0.4.2/ludic/catalog/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,21 +132,21 @@
                 "inline-size": "100%",  # type: ignore
                 "border-collapse": "collapse",  # type: ignore
                 "thead": {
                     "background-color": theme.colors.light,
                 },
                 "tr th": {
                     "border": (
-                        f"{theme.borders.thin} solid {theme.colors.light.darken(0.1)}"
+                        f"{theme.borders.thin} solid {theme.colors.light.darken(1)}"
                     ),
                     "padding": f"{theme.sizes.xxs} {theme.sizes.xxxs}",
                 },
                 "tr td": {
                     "border": (
-                        f"{theme.borders.thin} solid {theme.colors.light.darken(0.1)}"
+                        f"{theme.borders.thin} solid {theme.colors.light.darken(1)}"
                     ),
                     "padding": f"{theme.sizes.xxs} {theme.sizes.xxxs}",
                 },
             },
         }
     )
```

### Comparing `ludic-0.4.1/ludic/catalog/typography.py` & `ludic-0.4.2/ludic/catalog/typography.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     """
 
     classes = ["code"]
     styles = style.use(
         lambda theme: {
             ".code": {
                 "background-color": theme.colors.light,
-                "padding": f"{theme.sizes.xxxxs * 0.5} {theme.sizes.xxs}",
-                "border": f"1px solid {theme.colors.light.darken(0.2)}",
+                "padding": f"{theme.sizes.xxxxs * 0.3} {theme.sizes.xxxs}",
                 "border-radius": theme.rounding.less,
+                "font-size": theme.fonts.size * 0.9,
             }
         }
     )
 
     @override
     def render(self) -> code:
         return code(*self.children, **self.attrs)
@@ -115,14 +115,15 @@
 
     classes = ["code-block"]
     styles = style.use(
         lambda theme: {
             ".code-block": {
                 "background-color": theme.colors.light,
                 "padding": theme.sizes.l,
+                "font-size": theme.fonts.size * 0.9,
             },
         }
     )
 
     @override
     def render(self) -> pre:
         content = "".join(self.children)
```

### Comparing `ludic-0.4.1/ludic/catalog/utils.py` & `ludic-0.4.2/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/styles/collect.py` & `ludic-0.4.2/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/styles/themes.py` & `ludic-0.4.2/ludic/styles/themes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, TypeVar
 
-from .types import Color, Size
+from .types import Color, ColorRange, Size
 
 if TYPE_CHECKING:
     from ludic.types import BaseElement
 
 _T = TypeVar("_T", bound="BaseElement")
 
 
 @dataclass
 class Colors:
     """Colors for a theme."""
 
-    primary: Color = Color("#4ecdc4")
-    secondary: Color = Color("#fefefe")
-    success: Color = Color("#c7f464")
-    info: Color = Color("#fce303")
-    warning: Color = Color("#fc9003")
-    danger: Color = Color("#e32929")
+    primary: Color = ColorRange(["#276662", "#4ecdc4", "#dbf5f3"])
+    secondary: Color = ColorRange(["#f1f1f1", "#fefefe", "#fff"])
+    success: Color = ColorRange(["#637a32", "#c7f464", "#eefbd0"])
+    info: Color = ColorRange(["#978801", "#fce303", "#fef9cc"])
+    warning: Color = ColorRange(["#7e4801", "#fc9003", "#fee8cc"])
+    danger: Color = ColorRange(["#711414", "#e32929", "#f9d4d4"])
 
     light: Color = Color("#f8f8f8")
     dark: Color = Color("#414549")
 
     white: Color = Color("#fff")
     black: Color = Color("#222")
 
@@ -38,15 +38,15 @@
 
 @dataclass
 class Headers:
     """Headers for a theme."""
 
     h1: Header = field(default_factory=lambda: Header(size=Size(3, "em"), anchor=False))
     h2: Header = field(
-        default_factory=lambda: Header(size=Size(2.5, "em"), anchor=True)
+        default_factory=lambda: Header(size=Size(2.5, "em"), anchor=False)
     )
     h3: Header = field(default_factory=lambda: Header(size=Size(2, "em"), anchor=False))
     h4: Header = field(
         default_factory=lambda: Header(size=Size(1.5, "em"), anchor=False)
     )
     h5: Header = field(
         default_factory=lambda: Header(size=Size(1.25, "em"), anchor=False)
@@ -58,32 +58,32 @@
 class Fonts:
     """Font sizes for a theme."""
 
     plain: str = "Helvetica Neue, Helvetica, Arial, sans-serif"
     serif: str = "Georgia, serif"
     mono: str = "Space Mono, Roboto Mono, monospace"
 
-    size: Size = Size(1.02, "em")
+    size: Size = Size(1, "em")
 
 
 @dataclass
 class Sizes:
     """Size for a theme."""
 
     xxxxs: Size = Size(0.39)
     xxxs: Size = Size(0.47)
     xxs: Size = Size(0.57)
     xs: Size = Size(0.69)
     s: Size = Size(0.84)
     m: Size = Size(1)
-    l: Size = Size(1.19)  # noqa
-    xl: Size = Size(1.39)
-    xxl: Size = Size(1.61)
-    xxxl: Size = Size(1.83)
-    xxxxl: Size = Size(2.04)
+    l: Size = Size(1.16)  # noqa
+    xl: Size = Size(1.4)
+    xxl: Size = Size(1.68)
+    xxxl: Size = Size(2.01)
+    xxxxl: Size = Size(2.41)
 
 
 @dataclass
 class Borders:
     """Border sizes for a theme."""
 
     thin: Size = Size(0.1)
@@ -132,15 +132,15 @@
 
 
 @dataclass
 class Theme(metaclass=ABCMeta):
     """An abstract base class for theme configuration."""
 
     measure: Size = Size(110, "ch")
-    line_height: float = 1.4
+    line_height: float = 1.5
 
     fonts: Fonts = field(default_factory=Fonts)
     colors: Colors = field(default_factory=Colors)
     sizes: Sizes = field(default_factory=Sizes)
 
     borders: Borders = field(default_factory=Borders)
     rounding: Rounding = field(default_factory=Rounding)
```

### Comparing `ludic-0.4.1/ludic/styles/types.py` & `ludic-0.4.2/ludic/styles/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,48 +15,96 @@
     """Color class."""
 
     @property
     def rgb(self) -> tuple[int, int, int]:
         """RGB color."""
         return hex_to_rgb(self)
 
-    def darken(self, factor: float = 0.5) -> Self:
-        """Darken color by a given factor.
+    def darken(self, shift: int = 1) -> Self:
+        """Pick darker color from the range by given shift.
 
         Args:
-            factor (float, optional): Darkening factor. Defaults to 0.5.
+            shift (int, optional): Darkening shift. Defaults to 1.
 
         Returns:
             str: Darkened color.
         """
-        return type(self)(darken_color(self, factor))
+        return type(self)(darken_color(self, shift / 20))
 
-    def lighten(self, factor: float = 0.5) -> Self:
-        """Lighten color by a given factor.
+    def lighten(self, shift: int = 1) -> Self:
+        """Pick lighter color from the range by given shift.
 
         Args:
-            factor (float, optional): Lightening factor. Defaults to 0.5.
+            shift (int, optional): Lightening shift. Defaults to 1.
 
         Returns:
             str: Lightened color.
         """
-        return type(self)(lighten_color(self, factor))
+        return type(self)(lighten_color(self, shift / 20))
 
     def readable(self) -> Self:
         """Get lighter or darker variant of the given color depending on the luminance.
 
         Args:
             color (str): Color to find the readable opposite for.
 
         Returns:
             str: Readable opposite of the given color.
         """
         return type(self)(pick_readable_color_for(self))
 
 
+class ColorRange(Color):
+    """Color class."""
+
+    variants: list[str]
+    position: int
+
+    def __new__(
+        cls, variants: list[str] | str, position: int | None = None
+    ) -> "ColorRange":
+        if isinstance(variants, str):
+            variants = [variants]
+
+        new_position = position or (len(variants) // 2)
+
+        self = super().__new__(cls, variants[new_position])
+        self.variants = variants
+        self.position = new_position
+        return self
+
+    def darken(self, shift: int = 1) -> Self:
+        """Pick darker color from the range by given shift.
+
+        Args:
+            shift (int, optional): Darkening shift. Defaults to 1.
+
+        Returns:
+            str: Darkened color.
+        """
+        if 0 <= self.position - shift < len(self.variants):
+            return type(self)(self.variants, self.position - shift)
+        else:
+            return type(self)(self.variants, 0)
+
+    def lighten(self, shift: int = 1) -> Self:
+        """Pick lighter color from the range by given shift.
+
+        Args:
+            shift (int, optional): Lightening shift. Defaults to 1.
+
+        Returns:
+            str: Lightened color.
+        """
+        if 0 <= self.position + shift < len(self.variants):
+            return type(self)(self.variants, self.position + shift)
+        else:
+            return type(self)(self.variants, len(self.variants) - 1)
+
+
 class Size(str):
     """Size class."""
 
     value: float
     unit: SizeUnit = "rem"
 
     def __new__(cls, value: float, unit: SizeUnit = "rem") -> "Size":
```

### Comparing `ludic-0.4.1/ludic/styles/utils.py` & `ludic-0.4.2/ludic/styles/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     Args:
         color (str): Color to find the readable opposite for.
 
     Returns:
         str: Readable opposite of the given color.
     """
     rgb = color if isinstance(color, tuple) else hex_to_rgb(color)
-    _, luminance, _ = colorsys.rgb_to_hls(*rgb)
-    return "#000" if luminance > 140 else "#fff"
+    return "#000" if sum(rgb) > 400 else "#fff"
 
 
 def scale_color(color: str, factor: float = 0.5) -> str:
     """Scale a color by a given factor.
 
     Args:
         color (str): Color to scale.
```

### Comparing `ludic-0.4.1/ludic/web/app.py` & `ludic-0.4.2/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/datastructures.py` & `ludic-0.4.2/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/endpoints.py` & `ludic-0.4.2/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/exceptions.py` & `ludic-0.4.2/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/parsers.py` & `ludic-0.4.2/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/requests.py` & `ludic-0.4.2/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/responses.py` & `ludic-0.4.2/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/ludic/web/routing.py` & `ludic-0.4.2/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/test_elements.py` & `ludic-0.4.2/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/test_examples.py` & `ludic-0.4.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/test_exceptions.py` & `ludic-0.4.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/test_formatting.py` & `ludic-0.4.2/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/test_types.py` & `ludic-0.4.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/styles/__init__.py` & `ludic-0.4.2/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/styles/test_styles.py` & `ludic-0.4.2/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/tests/styles/test_themes.py` & `ludic-0.4.2/tests/styles/test_themes.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,31 +27,38 @@
 
     assert theme.colors.primary.rgb == (194, 231, 253)
     assert theme.colors.white.rgb == (255, 255, 255)
     assert theme.colors.light.rgb == (238, 238, 238)
     assert theme.colors.dark.rgb == (51, 51, 51)
     assert theme.colors.black.rgb == (0, 0, 0)
 
-    assert theme.colors.white.darken(0.5).rgb == (127, 127, 127)
-    assert theme.colors.white.darken(1).rgb == (1, 1, 1)
-    assert theme.colors.black.lighten(0.5).rgb == (127, 127, 127)
-    assert theme.colors.black.lighten(1).rgb == (255, 255, 255)
+    assert theme.colors.white.darken(10).rgb == (127, 127, 127)
+    assert theme.colors.white.darken(20).rgb == (1, 1, 1)
+    assert theme.colors.black.lighten(10).rgb == (127, 127, 127)
+    assert theme.colors.black.lighten(20).rgb == (255, 255, 255)
 
-    assert theme.colors.light.darken(0.5).rgb == (119, 119, 119)
-    assert theme.colors.dark.lighten(0.5).rgb == (153, 153, 153)
+    assert theme.colors.light.darken(10).rgb == (119, 119, 119)
+    assert theme.colors.dark.lighten(10).rgb == (153, 153, 153)
 
-    assert theme.colors.primary.darken(0.5).rgb == (97, 115, 126)
+    assert theme.colors.primary.darken(10).rgb == (97, 115, 126)
 
 
 def test_theme_font_sizes() -> None:
     theme = FooTheme(fonts=Fonts(size=Size(10, "px")))
 
     assert theme.fonts.size == "10px"
     assert theme.fonts.plain == "Helvetica Neue, Helvetica, Arial, sans-serif"
 
+    assert theme.fonts.size - 1 == "9px"
+    assert theme.fonts.size + 5 == "15px"
+    assert theme.fonts.size * 2 == "20px"
+
+    assert theme.fonts.size + "2" == "10px"
+    assert theme.fonts.size - "ab" == "10px"
+
 
 def test_themes_switching() -> None:
     foo, bar = FooTheme(), BarTheme()
 
     set_default_theme(foo)
     assert get_default_theme() == foo
     set_default_theme(bar)
```

#### html2text {}

```diff
@@ -3,36 +3,38 @@
 get_default_theme, set_default_theme, ) from ludic.styles.types import Color,
 Size from ludic.types import Component from . import BarTheme, FooTheme def
 test_theme_colors() -> None: theme = FooTheme( colors=Colors( primary=Color
 ("#c2e7fd"), white=Color("#fff"), light=Color("#eee"), dark=Color("#333"),
 black=Color("#000"), ) ) assert theme.colors.primary.rgb == (194, 231, 253)
 assert theme.colors.white.rgb == (255, 255, 255) assert theme.colors.light.rgb
 == (238, 238, 238) assert theme.colors.dark.rgb == (51, 51, 51) assert
-theme.colors.black.rgb == (0, 0, 0) assert theme.colors.white.darken(0.5).rgb
-== (127, 127, 127) assert theme.colors.white.darken(1).rgb == (1, 1, 1) assert
-theme.colors.black.lighten(0.5).rgb == (127, 127, 127) assert
-theme.colors.black.lighten(1).rgb == (255, 255, 255) assert
-theme.colors.light.darken(0.5).rgb == (119, 119, 119) assert
-theme.colors.dark.lighten(0.5).rgb == (153, 153, 153) assert
-theme.colors.primary.darken(0.5).rgb == (97, 115, 126) def
-test_theme_font_sizes() -> None: theme = FooTheme(fonts=Fonts(size=Size(10,
-"px"))) assert theme.fonts.size == "10px" assert theme.fonts.plain ==
-"Helvetica Neue, Helvetica, Arial, sans-serif" def test_themes_switching() -
-> None: foo, bar = FooTheme(), BarTheme() set_default_theme(foo) assert
-get_default_theme() == foo set_default_theme(bar) assert get_default_theme() ==
-bar def test_element_theme_switching() -> None: foo = FooTheme() bar = BarTheme
-() set_default_theme(bar) class C1(Component[str, GlobalAttrs]): styles =
-style.use( lambda theme: { "#c1 a": {"color": theme.colors.warning}, } )
-@override def render(self) -> div: return div( b("Hello, ", style={"color":
-self.theme.colors.secondary}), a(*self.children, href="https://example.com"),
-id="c1", ) class C2(Component[str, GlobalAttrs]): styles = style.use( lambda
-theme: { "#c2 a": {"color": theme.colors.danger}, } ) @override def render
-(self) -> div: return div( foo.use(C1(*self.children)), id="c2", style=
-{"background-color": self.theme.colors.primary}, ) assert C2("World").to_html()
-== ( f'
+theme.colors.black.rgb == (0, 0, 0) assert theme.colors.white.darken(10).rgb ==
+(127, 127, 127) assert theme.colors.white.darken(20).rgb == (1, 1, 1) assert
+theme.colors.black.lighten(10).rgb == (127, 127, 127) assert
+theme.colors.black.lighten(20).rgb == (255, 255, 255) assert
+theme.colors.light.darken(10).rgb == (119, 119, 119) assert
+theme.colors.dark.lighten(10).rgb == (153, 153, 153) assert
+theme.colors.primary.darken(10).rgb == (97, 115, 126) def test_theme_font_sizes
+() -> None: theme = FooTheme(fonts=Fonts(size=Size(10, "px"))) assert
+theme.fonts.size == "10px" assert theme.fonts.plain == "Helvetica Neue,
+Helvetica, Arial, sans-serif" assert theme.fonts.size - 1 == "9px" assert
+theme.fonts.size + 5 == "15px" assert theme.fonts.size * 2 == "20px" assert
+theme.fonts.size + "2" == "10px" assert theme.fonts.size - "ab" == "10px" def
+test_themes_switching() -> None: foo, bar = FooTheme(), BarTheme()
+set_default_theme(foo) assert get_default_theme() == foo set_default_theme(bar)
+assert get_default_theme() == bar def test_element_theme_switching() -> None:
+foo = FooTheme() bar = BarTheme() set_default_theme(bar) class C1(Component
+[str, GlobalAttrs]): styles = style.use( lambda theme: { "#c1 a": {"color":
+theme.colors.warning}, } ) @override def render(self) -> div: return div( b
+("Hello, ", style={"color": self.theme.colors.secondary}), a(*self.children,
+href="https://example.com"), id="c1", ) class C2(Component[str, GlobalAttrs]):
+styles = style.use( lambda theme: { "#c2 a": {"color": theme.colors.danger}, }
+) @override def render(self) -> div: return div( foo.use(C1(*self.children)),
+id="c2", style={"background-color": self.theme.colors.primary}, ) assert C2
+("World").to_html() == ( f'
 ' '
 ' f'HHeelllloo,, ' '_W_o_r_l_d' "
 " "
 " ) # fmt: skip assert style.from_components(C1, C2).to_html() == ( '
 " ) # fmt: skip set_default_theme(foo) assert style.from_components(C1,
 C2).to_html() == ( '
 " ) # fmt: skip
```

### Comparing `ludic-0.4.1/.gitignore` & `ludic-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/LICENCE` & `ludic-0.4.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/README.md` & `ludic-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/pyproject.toml` & `ludic-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.1/PKG-INFO` & `ludic-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.1
+Version: 0.4.2
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

