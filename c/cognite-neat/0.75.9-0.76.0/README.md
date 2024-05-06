# Comparing `tmp/cognite_neat-0.75.9.tar.gz` & `tmp/cognite_neat-0.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.75.9.tar", max compression
+gzip compressed data, was "cognite_neat-0.76.0.tar", max compression
```

## Comparing `cognite_neat-0.75.9.tar` & `cognite_neat-0.76.0.tar`

### file list

```diff
@@ -1,269 +1,270 @@
--rw-r--r--   0        0        0    11351 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/README.md
--rw-r--r--   0        0        0       61 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3529 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8127 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-03 12:45:30.942244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-03 12:45:30.946244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-03 12:45:30.946244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-03 12:45:30.946244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-03 12:45:30.946244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-03 12:45:30.950244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-03 12:45:30.950244 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-03 12:45:30.974243 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-03 12:45:30.978243 cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-03 12:45:30.982243 cognite_neat-0.75.9/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-03 12:45:30.982243 cognite_neat-0.75.9/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-03 12:45:30.986243 cognite_neat-0.75.9/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-03 12:45:30.986243 cognite_neat-0.75.9/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-03 12:45:30.986243 cognite_neat-0.75.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14980 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-03 12:45:30.990244 cognite_neat-0.75.9/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-03 12:45:30.994243 cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-03 12:45:30.998243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      176 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19608 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-03 12:45:31.002243 cognite_neat-0.75.9/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1517 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1870 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    14231 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13769 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20139 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4090 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4041 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10363 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12676 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6785 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7804 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6931 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11274 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4299 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15330 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0     6078 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0    15477 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0    11030 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0      522 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/__init__.py
--rw-r--r--   0        0        0    11024 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_base.py
--rw-r--r--   0        0        0    52602 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_dms_architect_rules.py
--rw-r--r--   0        0        0    12810 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_dms_rules_write.py
--rw-r--r--   0        0        0    30777 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_dms_schema.py
--rw-r--r--   0        0        0     2655 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_domain_rules.py
--rw-r--r--   0        0        0    22015 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_information_rules.py
--rw-r--r--   0        0        0      305 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_types/_base.py
--rw-r--r--   0        0        0     3197 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/rules/models/rules/_types/_field.py
--rw-r--r--   0        0        0       68 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12818 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-03 12:45:31.006243 cognite_neat-0.75.9/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3015 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    22491 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    10344 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4784 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-03 12:45:31.010243 cognite_neat-0.75.9/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4591 2024-05-03 12:45:31.398242 cognite_neat-0.75.9/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.9/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/README.md
+-rw-r--r--   0        0        0       61 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3529 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8127 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-06 13:20:34.396273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-06 13:20:34.400273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-05-06 13:20:34.404273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-05-06 13:20:34.404273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-05-06 13:20:34.432273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-05-06 13:20:34.432273 cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-05-06 13:20:34.440272 cognite_neat-0.76.0/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-05-06 13:20:34.440272 cognite_neat-0.76.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-06 13:20:34.440272 cognite_neat-0.76.0/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-06 13:20:34.440272 cognite_neat-0.76.0/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-06 13:20:34.444272 cognite_neat-0.76.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14980 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-06 13:20:34.448272 cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-06 13:20:34.452272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-06 13:20:34.456272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19608 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1517 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    16126 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13068 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20139 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4090 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4280 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    17827 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12676 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6785 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7804 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6931 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11397 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4299 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6242 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    19178 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    12288 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13936 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0     6078 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0    16395 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0    11030 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0      522 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/__init__.py
+-rw-r--r--   0        0        0    10876 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_base.py
+-rw-r--r--   0        0        0    58546 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_dms_architect_rules.py
+-rw-r--r--   0        0        0    12935 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_dms_rules_write.py
+-rw-r--r--   0        0        0    35870 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_dms_schema.py
+-rw-r--r--   0        0        0     2934 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_domain_rules.py
+-rw-r--r--   0        0        0    22447 2024-05-06 13:20:34.460272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_information_rules.py
+-rw-r--r--   0        0        0      305 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/rules/models/rules/_types/_field.py
+-rw-r--r--   0        0        0     6154 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12818 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3015 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    22491 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    10344 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4784 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-06 13:20:34.464272 cognite_neat-0.76.0/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4591 2024-05-06 13:20:34.852269 cognite_neat-0.76.0/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.76.0/PKG-INFO
```

### Comparing `cognite_neat-0.75.9/LICENSE` & `cognite_neat-0.76.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/README.md` & `cognite_neat-0.76.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/configuration.py` & `cognite_neat-0.76.0/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.76.0/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/explorer.py` & `cognite_neat-0.76.0/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.76.0/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.76.0/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.76.0/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.76.0/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.76.0/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.76.0/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.76.0/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.76.0/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.76.0/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.76.0/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.76.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/config.py` & `cognite_neat-0.76.0/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/constants.py` & `cognite_neat-0.76.0/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/exceptions.py` & `cognite_neat-0.76.0/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.76.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.76.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.76.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/exceptions.py` & `cognite_neat-0.76.0/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.76.0/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.76.0/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.76.0/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.76.0/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.76.0/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.76.0/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exceptions.py` & `cognite_neat-0.76.0/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import ABC
 from dataclasses import dataclass, field
 from functools import total_ordering
 
+from cognite.neat.rules.issues import IssueList
+
 
 @total_ordering
 @dataclass
 class UploadResultCore(ABC):
     name: str
 
     def __lt__(self, other: object) -> bool:
@@ -28,14 +30,15 @@
     changed: int = 0
     unchanged: int = 0
     skipped: int = 0
     failed_created: int = 0
     failed_changed: int = 0
     failed_deleted: int = 0
     error_messages: list[str] = field(default_factory=list)
+    issues: IssueList = field(default_factory=IssueList)
 
     @property
     def total(self) -> int:
         return self.created + self.deleted + self.changed + self.unchanged
 
     @property
     def failed(self) -> int:
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import warnings
 from collections.abc import Collection, Iterable
 from pathlib import Path
 from typing import Literal, TypeAlias, cast
 
 from cognite.client import CogniteClient
-from cognite.client.data_classes._base import CogniteResourceList
+from cognite.client.data_classes._base import CogniteResource, CogniteResourceList
+from cognite.client.data_classes.data_modeling import DataModelApply, DataModelId
 from cognite.client.exceptions import CogniteAPIError
 
+from cognite.neat.rules import issues
 from cognite.neat.rules._shared import Rules
+from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models.rules import InformationRules
 from cognite.neat.rules.models.rules._base import ExtensionCategory, SheetList
 from cognite.neat.rules.models.rules._dms_architect_rules import DMSContainer, DMSRules
 from cognite.neat.rules.models.rules._dms_schema import DMSSchema, PipelineSchema
 from cognite.neat.utils.cdf_loaders import (
     ContainerLoader,
     DataModelingLoader,
@@ -39,14 +42,16 @@
         include_space (set[str], optional):
             If set, only export components in the given spaces. Defaults to None which means all spaces.
         existing_handling (Literal["fail", "skip", "update", "force"], optional): How to handle existing components.
             Defaults to "update". See below for details.
         export_pipeline (bool, optional): Whether to export the pipeline. Defaults to False. This means setting
             up transformations, RAW databases and tables to populate the data model.
         instance_space (str, optional): The space to use for the instance. Defaults to None.
+        suppress_warnings (bool, optional): Suppress warnings. Defaults to False.
+
     ... note::
 
         - "fail": If any component already exists, the export will fail.
         - "skip": If any component already exists, it will be skipped.
         - "update": If any component already exists, it will be updated.
         - "force": If any component already exists, it will be deleted and recreated.
 
@@ -55,20 +60,22 @@
     def __init__(
         self,
         export_components: Component | Collection[Component] = "all",
         include_space: set[str] | None = None,
         existing_handling: Literal["fail", "skip", "update", "force"] = "update",
         export_pipeline: bool = False,
         instance_space: str | None = None,
+        suppress_warnings: bool = False,
     ):
         self.export_components = {export_components} if isinstance(export_components, str) else set(export_components)
         self.include_space = include_space
         self.existing_handling = existing_handling
         self.export_pipeline = export_pipeline
         self.instance_space = instance_space
+        self.suppress_warnings = suppress_warnings
         self._schema: DMSSchema | None = None
 
     def export_to_file(self, rules: Rules, filepath: Path) -> None:
         """Export the rules to a file(s).
 
         If the file is a directory, the components will be exported to separate files, otherwise they will be
         exported to a zip file.
@@ -111,19 +118,19 @@
             raise ValueError(f"{type(rules).__name__} cannot be exported to DMS")
 
         is_solution_model = (
             dms_rules.reference and dms_rules.metadata.external_id != dms_rules.reference.metadata.external_id
         )
         is_new_model = dms_rules.reference is None
         if is_new_model or is_solution_model:
-            return dms_rules.as_schema(self.export_pipeline, self.instance_space)
+            return dms_rules.as_schema(False, self.export_pipeline, self.instance_space)
 
         # This is an extension of an existing model.
         reference_rules = cast(DMSRules, dms_rules.reference).model_copy(deep=True)
-        reference_schema = reference_rules.as_schema(self.export_pipeline)
+        reference_schema = reference_rules.as_schema(include_ref=False, include_pipeline=self.export_pipeline)
 
         # Todo Move this to an appropriate location
         # Merging Reference with User Rules
         combined_rules = dms_rules.model_copy(deep=True)
         existing_containers = {container.class_ for container in combined_rules.containers or []}
         if combined_rules.containers is None:
             combined_rules.containers = SheetList[DMSContainer](data=[])
@@ -138,15 +145,15 @@
                 combined_rules.views.append(view)
         existing_properties = {(property_.class_, property_.property_) for property_ in combined_rules.properties}
         for property_ in reference_rules.properties:
             if (property_.class_, property_.property_) not in existing_properties:
                 property_.reference = None
                 combined_rules.properties.append(property_)
 
-        schema = combined_rules.as_schema(self.export_pipeline, self.instance_space)
+        schema = combined_rules.as_schema(True, self.export_pipeline, self.instance_space)
 
         if dms_rules.metadata.extension in (ExtensionCategory.addition, ExtensionCategory.reshape):
             # We do not freeze views as they might be changed, even for addition,
             # in case, for example, new properties are added. The validation will catch this.
             schema.frozen_ids.update(set(reference_schema.containers.as_ids()))
             schema.frozen_ids.update(set(reference_schema.node_types.as_ids()))
         return schema
@@ -202,14 +209,15 @@
         schema, to_export = self._prepare_schema_and_exporters(rules, client)
 
         # The conversion from DMS to GraphQL does not seem to be triggered even if the views
         # are changed. This is a workaround to force the conversion.
         redeploy_data_model = False
 
         for all_items, loader in to_export:
+            issue_list = IssueList()
             all_item_ids = loader.get_ids(all_items)
             skipped = sum(1 for item_id in all_item_ids if item_id in schema.frozen_ids)
             item_ids = [item_id for item_id in all_item_ids if item_id not in schema.frozen_ids]
             cdf_items = loader.retrieve(item_ids)
             cdf_item_by_id = {loader.get_id(item): item for item in cdf_items}
             items = [item for item in all_items if loader.get_id(item) in item_ids]
             to_create, to_update, unchanged, to_delete = [], [], [], []
@@ -245,14 +253,17 @@
                 skipped += len(to_update)
             elif self.existing_handling == "fail":
                 failed_changed = len(to_update)
                 changed = 0
             else:
                 raise ValueError(f"Unsupported existing_handling {self.existing_handling}")
 
+            warning_list = self._validate(loader, items)
+            issue_list.extend(warning_list)
+
             error_messages: list[str] = []
             if not dry_run:
                 if to_delete:
                     try:
                         loader.delete(to_delete)
                     except CogniteAPIError as e:
                         error_messages.append(f"Failed delete: {e.message}")
@@ -280,14 +291,15 @@
                 created=created,
                 changed=changed,
                 unchanged=len(unchanged),
                 skipped=skipped,
                 failed_created=failed_created,
                 failed_changed=failed_changed,
                 error_messages=error_messages,
+                issues=issue_list,
             )
 
             if loader.resource_name == "views" and (created or changed) and not redeploy_data_model:
                 redeploy_data_model = True
 
     def _prepare_schema_and_exporters(
         self, rules, client
@@ -303,7 +315,37 @@
         if self.export_components.intersection({"all", "data_models"}):
             to_export.append((schema.data_models, DataModelLoader(client)))
         if isinstance(schema, PipelineSchema):
             to_export.append((schema.databases, RawDatabaseLoader(client)))
             to_export.append((schema.raw_tables, RawTableLoader(client)))
             to_export.append((schema.transformations, TransformationLoader(client)))
         return schema, to_export
+
+    def _validate(self, loader: ResourceLoader, items: list[CogniteResource]) -> IssueList:
+        issue_list = IssueList()
+        if isinstance(loader, DataModelLoader):
+            models = cast(list[DataModelApply], items)
+            if other_models := self._exist_other_data_models(loader, models):
+                warning = issues.dms.OtherDataModelsInSpaceWarning(models[0].space, other_models)
+                if not self.suppress_warnings:
+                    warnings.warn(warning, stacklevel=2)
+                issue_list.append(warning)
+
+        return issue_list
+
+    @classmethod
+    def _exist_other_data_models(cls, loader: DataModelLoader, models: list[DataModelApply]) -> list[DataModelId]:
+        if not models:
+            return []
+        space = models[0].space
+        external_id = models[0].external_id
+        try:
+            data_models = loader.client.data_modeling.data_models.list(space=space, limit=25, all_versions=False)
+        except CogniteAPIError as e:
+            warnings.warn(issues.importing.APIWarning(str(e)), stacklevel=2)
+            return []
+        else:
+            return [
+                data_model.as_id()
+                for data_model in data_models
+                if (data_model.space, data_model.external_id) != (space, external_id)
+            ]
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,21 +116,14 @@
             if sheet_name in ("Metadata", "prefixes", "Reference", "is_reference"):
                 continue
             if is_reference:
                 sheet = workbook.create_sheet(f"Ref{sheet_name}")
             else:
                 sheet = workbook.create_sheet(sheet_name)
 
-            # Reorder such that the first column is class + the first field of the subclass
-            # of sheet entity. This is to make the properties/classes/views/containers sheet more readable.
-            # For example, for the properties these that means class, property, name, description
-            # instead of class, name, description, property
-            move = len(SheetEntity.model_fields) - 1  # -1 is for the class field
-            headers = headers[:1] + headers[move : move + 1] + headers[1:move] + headers[move + 1 :]
-
             main_header = self._main_header_by_sheet_name[sheet_name]
             sheet.append([main_header] + [""] * (len(headers) - 1))
             sheet.merge_cells(start_row=1, start_column=1, end_row=1, end_column=len(headers))
             sheet.append(headers)
 
             fill_colors = itertools.cycle(["CADCFC", "FFFFFF"])
             fill_color = next(fill_colors)
@@ -146,16 +139,14 @@
                     sheet.append([""] * len(headers))
                     for cell in sheet[sheet.max_row]:
                         cell.fill = PatternFill(fgColor=fill_color, patternType="solid")
                         side = Side(style="thin", color="000000")
                         cell.border = Border(left=side, right=side, top=side, bottom=side)
                     fill_color = next(fill_colors)
 
-                # Need to do the same reordering as for the headers above
-                row = row[:1] + row[move : move + 1] + row[1:move] + row[move + 1 :]
                 sheet.append(row)
                 if self._styling_level > 2 and is_properties:
                     for cell in sheet[sheet.max_row]:
                         cell.fill = PatternFill(fgColor=fill_color, patternType="solid")
                         side = Side(style="thin", color="000000")
                         cell.border = Border(left=side, right=side, top=side, bottom=side)
                 last_class = class_
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.76.0/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,20 @@
             raise NotImplementedError(f"Role {role} is not supported for {type(rules).__name__} rules")
 
         if errors == "raise":
             return output
         else:
             return output, issues
 
+    @classmethod
+    def _return_or_raise(cls, issue_list: IssueList, errors: Literal["raise", "continue"]) -> tuple[None, IssueList]:
+        if errors == "raise":
+            raise issue_list.as_errors()
+        return None, issue_list
+
     def _default_metadata(self):
         return {
             "prefix": "neat",
             "schema": "partial",
             "namespace": Namespace("http://purl.org/cognite/neat/"),
             "version": "0.1.0",
             "title": "Neat Imported Data Model",
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,23 @@
 from cognite.neat.rules.models.rules._dms_rules_write import DMSRulesWrite
 from cognite.neat.utils.auxiliary import local_import
 from cognite.neat.utils.spreadsheet import SpreadsheetRead, read_individual_sheet
 
 from ._base import BaseImporter, Rules, _handle_issues
 
 SOURCE_SHEET__TARGET_FIELD__HEADERS = [
-    ("Properties", "Properties", "Class"),
+    (
+        "Properties",
+        "Properties",
+        {
+            RoleTypes.domain_expert: "Property",
+            RoleTypes.information_architect: "Property",
+            RoleTypes.dms_architect: "View Property",
+        },
+    ),
     ("Classes", "Classes", "Class"),
     ("Containers", "Containers", "Container"),
     ("Views", "Views", "View"),
 ]
 
 MANDATORY_SHEETS_BY_ROLE: dict[RoleTypes, set[str]] = {
     role_type: {str(sheet_name) for sheet_name in RULES_PER_ROLE[role_type].mandatory_fields(use_alias=True)}
@@ -127,19 +135,23 @@
 
         if missing_sheets := expected_sheet_names.difference(set(excel_file.sheet_names)):
             self.issue_list.append(
                 issues.spreadsheet_file.SheetMissingError(cast(Path, excel_file.io), list(missing_sheets))
             )
             return None, read_info_by_sheet
 
-        for source_sheet_name, target_sheet_name, headers in SOURCE_SHEET__TARGET_FIELD__HEADERS:
+        for source_sheet_name, target_sheet_name, headers_input in SOURCE_SHEET__TARGET_FIELD__HEADERS:
             source_sheet_name = self.to_reference_sheet(source_sheet_name) if self._is_reference else source_sheet_name
 
             if source_sheet_name not in excel_file.sheet_names:
                 continue
+            if isinstance(headers_input, dict):
+                headers = headers_input[metadata.role]
+            else:
+                headers = headers_input
 
             try:
                 sheets[target_sheet_name], read_info_by_sheet[source_sheet_name] = read_individual_sheet(
                     excel_file, source_sheet_name, return_read_info=True, expected_headers=[headers]
                 )
             except Exception as e:
                 self.issue_list.append(issues.spreadsheet_file.ReadSpreadsheetsError(cast(Path, excel_file.io), str(e)))
@@ -225,20 +237,14 @@
         return self._to_output(
             rules,
             issue_list,
             errors=errors,
             role=role,
         )
 
-    @classmethod
-    def _return_or_raise(cls, issue_list: IssueList, errors: Literal["raise", "continue"]) -> tuple[None, IssueList]:
-        if errors == "raise":
-            raise issue_list.as_errors()
-        return None, issue_list
-
 
 class GoogleSheetImporter(BaseImporter):
     def __init__(self, sheet_id: str, skiprows: int = 1):
         self.sheet_id = sheet_id
         self.skiprows = skiprows
 
     @overload
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.76.0/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/issues/base.py` & `cognite_neat-0.76.0/cognite/neat/rules/issues/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                 multi_error := ctx.get("error"), MultiValueError
             ):
                 all_errors.extend(multi_error.errors)
             else:
                 all_errors.append(DefaultPydanticError.from_pydantic_error(error))
         return all_errors
 
+    def as_exception(self) -> Exception:
+        return ValueError(self.message())
+
 
 @dataclass(frozen=True)
 class DefaultPydanticError(NeatValidationError):
     type: str
     loc: tuple[int | str, ...]
     msg: str
     input: Any
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.76.0/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.76.0/cognite/neat/rules/issues/spreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,23 +172,26 @@
 
     @classmethod
     def from_pydantic_error(
         cls, error: ErrorDetails, read_info_by_sheet: dict[str, SpreadsheetRead] | None = None
     ) -> Self:
         sheet_name, _, row, column, *__ = error["loc"]
         reader = (read_info_by_sheet or {}).get(str(sheet_name), SpreadsheetRead())
-        return cls(
-            column=str(column),
-            row=reader.adjusted_row_number(int(row)),
-            actual_sheet_name=str(sheet_name),
-            type=error["type"],
-            msg=error["msg"],
-            input=error.get("input"),
-            url=str(url) if (url := error.get("url")) else None,
-        )
+        try:
+            return cls(
+                column=str(column),
+                row=reader.adjusted_row_number(int(row)),
+                actual_sheet_name=str(sheet_name),
+                type=error["type"],
+                msg=error["msg"],
+                input=error.get("input"),
+                url=str(url) if (url := error.get("url")) else None,
+            )
+        except ValueError:
+            return DefaultPydanticError.from_pydantic_error(error)  # type: ignore[return-value]
 
     def dump(self) -> dict[str, Any]:
         output = super().dump()
         output["actual_sheet_name"] = self.actual_sheet_name
         return output
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.76.0/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/entities.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import sys
 from abc import ABC, abstractmethod
 from functools import total_ordering
 from typing import Annotated, Any, ClassVar, Generic, TypeVar, cast
 
-from cognite.client.data_classes.data_modeling.ids import ContainerId, DataModelId, PropertyId, ViewId
+from cognite.client.data_classes.data_modeling.ids import ContainerId, DataModelId, NodeId, PropertyId, ViewId
 from pydantic import AnyHttpUrl, BaseModel, BeforeValidator, Field, PlainSerializer, model_serializer, model_validator
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
@@ -26,14 +26,15 @@
     object_property = "ObjectProperty"
     data_property = "DatatypeProperty"
     annotation_property = "AnnotationProperty"
     object_value_type = "object_value_type"
     data_value_type = "data_value_type"  # these are strings, floats, ...
     xsd_value_type = "xsd_value_type"
     dms_value_type = "dms_value_type"
+    dms_node = "dms_node"
     view = "view"
     reference_entity = "reference_entity"
     container = "container"
     datamodel = "datamodel"
     undefined = "undefined"
 
 
@@ -244,15 +245,15 @@
     suffix: _UnknownType = Unknown  # type: ignore[assignment]
 
     @property
     def id(self) -> str:
         return str(Unknown)
 
 
-T_ID = TypeVar("T_ID", bound=ContainerId | ViewId | DataModelId | PropertyId | None)
+T_ID = TypeVar("T_ID", bound=ContainerId | ViewId | DataModelId | PropertyId | NodeId | None)
 
 
 class DMSEntity(Entity, Generic[T_ID], ABC):
     type_: ClassVar[EntityTypes] = EntityTypes.undefined
     prefix: str = Field(alias="space")
     suffix: str = Field(alias="externalId")
 
@@ -298,31 +299,36 @@
     def from_id(cls, id: ContainerId) -> "ContainerEntity":
         return cls(space=id.space, externalId=id.external_id)
 
 
 class DMSVersionedEntity(DMSEntity[T_ID], ABC):
     version: str
 
-    def as_class(self) -> ClassEntity:
+    def as_class(self, skip_version: bool = False) -> ClassEntity:
+        if skip_version:
+            return ClassEntity(prefix=self.space, suffix=self.external_id)
         return ClassEntity(prefix=self.space, suffix=self.external_id, version=self.version)
 
 
 class ViewEntity(DMSVersionedEntity[ViewId]):
     type_: ClassVar[EntityTypes] = EntityTypes.view
 
     def as_id(
         self,
     ) -> ViewId:
         return ViewId(space=self.space, external_id=self.external_id, version=self.version)
 
     @classmethod
-    def from_id(cls, id: ViewId) -> "ViewEntity":
-        if id.version is None:
+    def from_id(cls, id: ViewId, default_version: str | None = None) -> "ViewEntity":
+        if id.version is not None:
+            return cls(space=id.space, externalId=id.external_id, version=id.version)
+        elif default_version is not None:
+            return cls(space=id.space, externalId=id.external_id, version=default_version)
+        else:
             raise ValueError("Version must be specified")
-        return cls(space=id.space, externalId=id.external_id, version=id.version)
 
 
 class DMSUnknownEntity(DMSEntity[None]):
     """This is a special entity that represents an unknown entity.
 
     The use case is for direct relations where the source is not known."""
 
@@ -372,14 +378,25 @@
     @classmethod
     def from_id(cls, id: DataModelId) -> "DataModelEntity":
         if id.version is None:
             raise ValueError("Version must be specified")
         return cls(space=id.space, externalId=id.external_id, version=id.version)
 
 
+class DMSNodeEntity(DMSEntity[NodeId]):
+    type_: ClassVar[EntityTypes] = EntityTypes.dms_node
+
+    def as_id(self) -> NodeId:
+        return NodeId(space=self.space, external_id=self.external_id)
+
+    @classmethod
+    def from_id(cls, id: NodeId) -> "DMSNodeEntity":
+        return cls(space=id.space, externalId=id.external_id)
+
+
 class ReferenceEntity(ClassEntity):
     type_: ClassVar[EntityTypes] = EntityTypes.reference_entity
     prefix: str
     property_: str | None = Field(None, alias="property")
 
     def as_view_id(self) -> ViewId:
         if isinstance(self.prefix, _UndefinedType) or isinstance(self.suffix, _UnknownType):
@@ -387,14 +404,20 @@
         return ViewId(space=self.prefix, external_id=self.suffix, version=self.version)
 
     def as_view_property_id(self) -> PropertyId:
         if self.property_ is None or self.prefix is Undefined or self.suffix is Unknown:
             raise ValueError("Property is not defined or prefix is not defined or suffix is unknown")
         return PropertyId(source=self.as_view_id(), property=self.property_)
 
+    def as_node_id(self) -> NodeId:
+        return NodeId(space=self.prefix, external_id=self.suffix)
+
+    def as_node_entity(self) -> DMSNodeEntity:
+        return DMSNodeEntity(space=self.prefix, externalId=self.suffix)
+
     def as_class_entity(self) -> ClassEntity:
         return ClassEntity(prefix=self.prefix, suffix=self.suffix, version=self.version)
 
 
 def _split_str(v: Any) -> list[str]:
     if isinstance(v, str):
         return v.replace(", ", ",").split(",")
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/__init__.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_base.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     constr,
     field_validator,
     model_serializer,
     model_validator,
 )
 from pydantic.fields import FieldInfo
 
-from cognite.neat.rules.models.entities import ClassEntity
-
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
     from typing_extensions import Self
 
@@ -136,14 +134,19 @@
 
 class ExtensionCategory(StrEnum):
     addition = "addition"
     reshape = "reshape"
     rebuild = "rebuild"
 
 
+class DataModelType(StrEnum):
+    solution = "solution"
+    enterprise = "enterprise"
+
+
 class RoleTypes(StrEnum):
     domain_expert = "domain expert"
     information_architect = "information architect"
     dms_architect = "DMS Architect"
 
 
 class MatchType(StrEnum):
@@ -270,18 +273,14 @@
         exporting a reference model.
         """
         raise NotImplementedError
 
 
 # An sheet entity is either a class or a property.
 class SheetEntity(RuleModel):
-    class_: ClassEntity = Field(alias="Class")
-    name: str | None = Field(alias="Name", default=None)
-    description: str | None = Field(alias="Description", default=None)
-
     @field_validator("*", mode="before")
     def strip_string(cls, value: Any) -> Any:
         if isinstance(value, str):
             return value.strip()
         return value
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_dms_architect_rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_dms_architect_rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 import abc
 import math
 import re
 import sys
 import warnings
 from collections import defaultdict
+from collections.abc import Callable
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, cast
 
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import PropertyType as CognitePropertyType
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex
-from cognite.client.data_classes.data_modeling.views import SingleReverseDirectRelationApply, ViewPropertyApply
+from cognite.client.data_classes.data_modeling.views import (
+    SingleEdgeConnectionApply,
+    SingleReverseDirectRelationApply,
+    ViewPropertyApply,
+)
 from pydantic import Field, field_serializer, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo, ValidationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.rules import issues
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.entities import (
     ClassEntity,
     ContainerEntity,
     ContainerEntityList,
+    DMSNodeEntity,
     DMSUnknownEntity,
     ParentClassEntity,
     ReferenceEntity,
     UnknownEntity,
     URLEntity,
     ViewEntity,
     ViewEntityList,
     ViewPropertyEntity,
 )
 from cognite.neat.rules.models.rules._domain_rules import DomainRules
+from cognite.neat.rules.models.wrapped_entities import DMSFilter, HasDataFilter, NodeTypeFilter
 
-from ._base import BaseMetadata, BaseRules, ExtensionCategory, RoleTypes, SchemaCompleteness, SheetEntity, SheetList
+from ._base import (
+    BaseMetadata,
+    BaseRules,
+    DataModelType,
+    ExtensionCategory,
+    RoleTypes,
+    SchemaCompleteness,
+    SheetEntity,
+    SheetList,
+)
 from ._dms_schema import DMSSchema, PipelineSchema
 from ._types import (
     ExternalIdType,
     PropertyType,
     StrListType,
     VersionType,
 )
@@ -63,14 +79,15 @@
     except AttributeError:
         ...
 del subclasses  # cleanup namespace
 
 
 class DMSMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.dms_architect
+    data_model_type: DataModelType = Field(DataModelType.solution, alias="dataModelType")
     schema_: SchemaCompleteness = Field(alias="schema")
     extension: ExtensionCategory = ExtensionCategory.addition
     space: ExternalIdType
     name: str | None = Field(
         None,
         description="Human readable name of the data model",
         min_length=1,
@@ -82,44 +99,52 @@
     creator: StrListType
     created: datetime = Field(
         description=("Date of the data model creation"),
     )
     updated: datetime = Field(
         description=("Date of the data model update"),
     )
-    # MyPy does not account for the field validator below that sets the default value
-    default_view_version: VersionType = Field(None)  # type: ignore[assignment]
 
     @field_validator("*", mode="before")
     def strip_string(cls, value: Any) -> Any:
         if isinstance(value, str):
             return value.strip()
         return value
 
+    @field_serializer("schema_", "extension", "data_model_type", when_used="always")
+    @staticmethod
+    def as_string(value: SchemaCompleteness | ExtensionCategory | DataModelType) -> str:
+        return str(value)
+
     @field_validator("schema_", mode="plain")
-    def as_enum(cls, value: str) -> SchemaCompleteness:
+    def as_enum_schema(cls, value: str) -> SchemaCompleteness:
         return SchemaCompleteness(value)
 
-    @model_validator(mode="before")
-    def set_default_view_version_if_missing(cls, values):
-        if "default_view_version" not in values:
-            values["default_view_version"] = values["version"]
-        return values
+    @field_validator("extension", mode="plain")
+    def as_enum_extension(cls, value: str) -> ExtensionCategory:
+        return ExtensionCategory(value)
+
+    @field_validator("data_model_type", mode="plain")
+    def as_enum_model_type(cls, value: str) -> DataModelType:
+        return DataModelType(value)
 
     @field_validator("description", mode="before")
     def nan_as_none(cls, value):
         if isinstance(value, float) and math.isnan(value):
             return None
         return value
 
     def as_space(self) -> dm.SpaceApply:
         return dm.SpaceApply(
             space=self.space,
         )
 
+    def as_data_model_id(self) -> dm.DataModelId:
+        return dm.DataModelId(space=self.space, external_id=self.external_id, version=self.version)
+
     def as_data_model(self) -> dm.DataModelApply:
         suffix = f"Creator: {', '.join(self.creator)}"
         if self.description:
             description = f"{self.description} Creator: {', '.join(self.creator)}"
         else:
             description = suffix
 
@@ -158,68 +183,69 @@
             creator=creator,
             created=datetime.now(),
             updated=datetime.now(),
         )
 
 
 class DMSProperty(SheetEntity):
-    property_: PropertyType = Field(alias="Property")
-    relation: Literal["direct", "reversedirect", "multiedge"] | None = Field(None, alias="Relation")
+    view: ViewEntity = Field(alias="View")
+    view_property: str = Field(alias="View Property")
+    name: str | None = Field(alias="Name", default=None)
+    description: str | None = Field(alias="Description", default=None)
+    connection: Literal["direct", "edge", "reverse"] | None = Field(None, alias="Connection")
     value_type: DataType | ViewPropertyEntity | ViewEntity | DMSUnknownEntity = Field(alias="Value Type")
     nullable: bool | None = Field(default=None, alias="Nullable")
-    is_list: bool | None = Field(default=None, alias="IsList")
+    is_list: bool | None = Field(default=None, alias="Is List")
     default: str | int | dict | None = Field(None, alias="Default")
     reference: URLEntity | ReferenceEntity | None = Field(default=None, alias="Reference", union_mode="left_to_right")
     container: ContainerEntity | None = Field(None, alias="Container")
-    container_property: str | None = Field(None, alias="ContainerProperty")
-    view: ViewEntity = Field(alias="View")
-    view_property: str = Field(alias="ViewProperty")
+    container_property: str | None = Field(None, alias="Container Property")
     index: StrListType | None = Field(None, alias="Index")
     constraint: StrListType | None = Field(None, alias="Constraint")
+    class_: ClassEntity = Field(alias="Class (linage)")
+    property_: PropertyType = Field(alias="Property (linage)")
 
     @field_validator("nullable")
     def direct_relation_must_be_nullable(cls, value: Any, info: ValidationInfo) -> None:
-        if info.data.get("relation") == "direct" and value is False:
+        if info.data.get("connection") == "direct" and value is False:
             raise ValueError("Direct relation must be nullable")
         return value
 
-    @field_validator("container_property", "container")
-    def reverse_direct_relation_has_no_container(cls, value, info: ValidationInfo) -> None:
-        if info.data.get("relation") == "reversedirect" and value is not None:
-            raise ValueError(f"Reverse direct relation must not have container or container property, got {value}")
-        return value
-
     @field_validator("value_type", mode="after")
-    def relations_value_type(cls, value: DataType | ClassEntity, info: ValidationInfo) -> DataType | ClassEntity:
-        if (relation := info.data["relation"]) is None:
+    def connections_value_type(
+        cls, value: ViewPropertyEntity | ViewEntity | DMSUnknownEntity, info: ValidationInfo
+    ) -> DataType | ViewPropertyEntity | ViewEntity | DMSUnknownEntity:
+        if (connection := info.data.get("connection")) is None:
             return value
-        if not isinstance(value, ViewEntity | ViewPropertyEntity | DMSUnknownEntity):
-            raise ValueError(f"Relations must have a value type that points to another view, got {value}")
-        if relation == "reversedirect" and value.property_ is None:
-            # Todo fix this error message. It have the wrong syntax for how to have a property
+        if connection == "direct" and not isinstance(value, ViewEntity | DMSUnknownEntity):
+            raise ValueError(f"Direct relation must have a value type that points to a view, got {value}")
+        elif connection == "edge" and not isinstance(value, ViewEntity):
+            raise ValueError(f"Edge connection must have a value type that points to a view, got {value}")
+        elif connection == "reverse" and not isinstance(value, ViewPropertyEntity | ViewEntity):
             raise ValueError(
-                "Reverse direct relation must set what it is the reverse property of. "
-                f"Which property in {value.versioned_id} is this the reverse of? Expecting"
-                f"{value.versioned_id}:<property>"
+                f"Reverse connection must have a value type that points to a view or view property, got {value}"
             )
         return value
 
     @field_serializer("value_type", when_used="always")
     @staticmethod
     def as_dms_type(value_type: DataType | ViewPropertyEntity | ViewEntity) -> str:
         if isinstance(value_type, DataType):
             return value_type.dms._type
         else:
             return str(value_type)
 
 
 class DMSContainer(SheetEntity):
     container: ContainerEntity = Field(alias="Container")
+    name: str | None = Field(alias="Name", default=None)
+    description: str | None = Field(alias="Description", default=None)
     reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     constraint: ContainerEntityList | None = Field(None, alias="Constraint")
+    class_: ClassEntity = Field(alias="Class (linage)")
 
     def as_container(self) -> dm.ContainerApply:
         container_id = self.container.as_id()
         constraints: dict[str, dm.Constraint] = {}
         for constraint in self.constraint or []:
             requires = dm.RequiresConstraint(constraint.as_id())
             constraints[f"{constraint.space}_{constraint.external_id}"] = requires
@@ -236,67 +262,103 @@
     @classmethod
     def from_container(cls, container: dm.ContainerApply) -> "DMSContainer":
         constraints: list[ContainerEntity] = []
         for _, constraint_obj in (container.constraints or {}).items():
             if isinstance(constraint_obj, dm.RequiresConstraint):
                 constraints.append(ContainerEntity.from_id(constraint_obj.require))
             # UniquenessConstraint it handled in the properties
+        container_entity = ContainerEntity.from_id(container.as_id())
         return cls(
-            class_=ClassEntity(prefix=container.space, suffix=container.external_id),
-            container=ContainerEntity(space=container.space, externalId=container.external_id),
+            class_=container_entity.as_class(),
+            container=container_entity,
             name=container.name or None,
             description=container.description,
             constraint=constraints or None,
         )
 
 
 class DMSView(SheetEntity):
     view: ViewEntity = Field(alias="View")
+    name: str | None = Field(alias="Name", default=None)
+    description: str | None = Field(alias="Description", default=None)
     implements: ViewEntityList | None = Field(None, alias="Implements")
     reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
-    filter_: Literal["hasData", "nodeType"] | None = Field(None, alias="Filter")
-    in_model: bool = Field(True, alias="InModel")
+    filter_: HasDataFilter | NodeTypeFilter | None = Field(None, alias="Filter")
+    in_model: bool = Field(True, alias="In Model")
+    class_: ClassEntity = Field(alias="Class (linage)")
 
     def as_view(self) -> dm.ViewApply:
         view_id = self.view.as_id()
         return dm.ViewApply(
             space=view_id.space,
             external_id=view_id.external_id,
             version=view_id.version or _DEFAULT_VERSION,
             name=self.name or None,
             description=self.description,
             implements=[parent.as_id() for parent in self.implements or []] or None,
             properties={},
         )
 
     @classmethod
-    def from_view(cls, view: dm.ViewApply, data_model_view_ids: set[dm.ViewId]) -> "DMSView":
+    def from_view(cls, view: dm.ViewApply, in_model: bool) -> "DMSView":
+        view_entity = ViewEntity.from_id(view.as_id())
+        class_entity = view_entity.as_class(skip_version=True)
+
         return cls(
-            class_=ClassEntity(prefix=view.space, suffix=view.external_id),
-            view=ViewEntity(space=view.space, externalId=view.external_id, version=view.version),
+            class_=class_entity,
+            view=view_entity,
             description=view.description,
             name=view.name,
-            implements=[
-                ViewEntity(
-                    space=parent.space, externalId=parent.external_id, version=parent.version or _DEFAULT_VERSION
-                )
-                for parent in view.implements
-            ]
-            or None,
-            in_model=view.as_id() in data_model_view_ids,
+            implements=[ViewEntity.from_id(parent, _DEFAULT_VERSION) for parent in view.implements] or None,
+            in_model=in_model,
         )
 
 
 class DMSRules(BaseRules):
     metadata: DMSMetadata = Field(alias="Metadata")
     properties: SheetList[DMSProperty] = Field(alias="Properties")
     views: SheetList[DMSView] = Field(alias="Views")
     containers: SheetList[DMSContainer] | None = Field(None, alias="Containers")
     reference: "DMSRules | None" = Field(None, alias="Reference")
 
+    @field_validator("reference")
+    def check_reference_of_reference(cls, value: "DMSRules | None", info: ValidationInfo) -> "DMSRules | None":
+        if value is None:
+            return None
+        if value.reference is not None:
+            raise ValueError("Reference rules cannot have a reference")
+        if value.metadata.data_model_type == DataModelType.solution and (metadata := info.data.get("metadata")):
+            warnings.warn(
+                issues.dms.SolutionOnTopOfSolutionModelWarning(
+                    metadata.as_data_model_id(), value.metadata.as_data_model_id()
+                ),
+                stacklevel=2,
+            )
+        return value
+
+    @field_validator("views")
+    def matching_version_and_space(cls, value: SheetList[DMSView], info: ValidationInfo) -> SheetList[DMSView]:
+        if not (metadata := info.data.get("metadata")):
+            return value
+        model_version = metadata.version
+        if different_version := [view.view.as_id() for view in value if view.view.version != model_version]:
+            warnings.warn(issues.dms.ViewModelVersionNotMatchingWarning(different_version, model_version), stacklevel=2)
+        if different_space := [view.view.as_id() for view in value if view.view.space != metadata.space]:
+            warnings.warn(issues.dms.ViewModelSpaceNotMatchingWarning(different_space, metadata.space), stacklevel=2)
+        return value
+
+    @field_validator("views")
+    def matching_version(cls, value: SheetList[DMSView], info: ValidationInfo) -> SheetList[DMSView]:
+        if not (metadata := info.data.get("metadata")):
+            return value
+        model_version = metadata.version
+        if different_version := [view.view.as_id() for view in value if view.view.version != model_version]:
+            warnings.warn(issues.dms.ViewModelVersionNotMatchingWarning(different_version, model_version), stacklevel=2)
+        return value
+
     @model_validator(mode="after")
     def consistent_container_properties(self) -> "DMSRules":
         container_properties_by_id: dict[tuple[ContainerEntity, str], list[tuple[int, DMSProperty]]] = defaultdict(list)
         for prop_no, prop in enumerate(self.properties):
             if prop.container and prop.container_property:
                 container_properties_by_id[(prop.container, prop.container_property)].append((prop_no, prop))
 
@@ -435,15 +497,15 @@
         is_solution = self.metadata.space != self.reference.metadata.space
         if is_solution:
             return self
         if self.metadata.extension is ExtensionCategory.rebuild:
             # Everything is allowed
             return self
         # Is an extension of an existing model.
-        user_schema = self.as_schema()
+        user_schema = self.as_schema(include_ref=False)
         ref_schema = self.reference.as_schema()
         new_containers = {container.as_id(): container for container in user_schema.containers}
         existing_containers = {container.as_id(): container for container in ref_schema.containers}
 
         errors: list[issues.NeatValidationError] = []
         for container_id, container in new_containers.items():
             existing_container = existing_containers.get(container_id)
@@ -536,78 +598,28 @@
 
         schema = rules.as_schema()
         errors = schema.validate()
         if errors:
             raise issues.MultiValueError(errors)
         return self
 
-    @model_serializer(mode="plain", when_used="always")
-    def dms_rules_serialization(self, info: SerializationInfo) -> dict[str, Any]:
-        kwargs = vars(info)
-        default_space = f"{self.metadata.space}:"
-        default_version = f"version={self.metadata.default_view_version}"
-        default_version_wrapped = f"({default_version})"
-        properties = []
-        field_names = (
-            ["Class", "View", "Value Type", "Container"]
-            if info.by_alias
-            else ["class_", "view", "value_type", "container"]
-        )
-        value_type_name = "Value Type" if info.by_alias else "value_type"
-        for prop in self.properties:
-            dumped = prop.model_dump(**kwargs)
-            for field_name in field_names:
-                if value := dumped.get(field_name):
-                    dumped[field_name] = value.removeprefix(default_space).removesuffix(default_version_wrapped)
-            # Value type can have a property as well
-            dumped[value_type_name] = dumped[value_type_name].replace(default_version, "")
-            properties.append(dumped)
-
-        views = []
-        field_names = ["Class", "View", "Implements"] if info.by_alias else ["class_", "view", "implements"]
-        implements_name = "Implements" if info.by_alias else "implements"
-        for view in self.views:
-            dumped = view.model_dump(**kwargs)
-            for field_name in field_names:
-                if value := dumped.get(field_name):
-                    dumped[field_name] = value.removeprefix(default_space).removesuffix(default_version_wrapped)
-            if value := dumped.get(implements_name):
-                dumped[implements_name] = ",".join(
-                    parent.strip().removeprefix(default_space).removesuffix(default_version_wrapped)
-                    for parent in value.split(",")
-                )
-            views.append(dumped)
-
-        containers = []
-        field_names = ["Class", "Container"] if info.by_alias else ["class_", "container"]
-        constraint_name = "Constraint" if info.by_alias else "constraint"
-        for container in self.containers or []:
-            dumped = container.model_dump(**kwargs)
-            for field_name in field_names:
-                if value := dumped.get(field_name):
-                    dumped[field_name] = value.removeprefix(default_space).removesuffix(default_version_wrapped)
-                if value := dumped.get(constraint_name):
-                    dumped[constraint_name] = ",".join(
-                        constraint.strip().removeprefix(default_space).removesuffix(default_version_wrapped)
-                        for constraint in value.split(",")
-                    )
-            containers.append(dumped)
-
-        output = {
-            "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
-            "Properties" if info.by_alias else "properties": properties,
-            "Views" if info.by_alias else "views": views,
-            "Containers" if info.by_alias else "containers": containers,
-        }
-        if self.reference is not None:
-            output["Reference" if info.by_alias else "reference"] = self.reference.model_dump(**kwargs)
-        return output
-
-    def as_schema(self, include_pipeline: bool = False, instance_space: str | None = None) -> DMSSchema:
-        return _DMSExporter(include_pipeline, instance_space).to_schema(self)
+    @model_serializer(mode="wrap", when_used="always")
+    def dms_rules_serialization(
+        self,
+        handler: Callable,
+        info: SerializationInfo,
+    ) -> dict[str, Any]:
+        dumped = cast(dict[str, Any], handler(self, info))
+        space, version = self.metadata.space, self.metadata.version
+        return _DMSRulesSerializer(info, space, version).clean(dumped)
+
+    def as_schema(
+        self, include_ref: bool = False, include_pipeline: bool = False, instance_space: str | None = None
+    ) -> DMSSchema:
+        return _DMSExporter(self, include_ref, include_pipeline, instance_space).to_schema()
 
     def as_information_architect_rules(self) -> "InformationRules":
         return _DMSRulesConverter(self).as_information_architect_rules()
 
     def as_domain_expert_rules(self) -> DomainRules:
         return _DMSRulesConverter(self).as_domain_rules()
 
@@ -636,24 +648,38 @@
 
     Args
         include_pipeline (bool): If True, the pipeline will be included with the schema. Pipeline means the
             raw tables and transformations necessary to populate the data model.
         instance_space (str): The space to use for the instance. Defaults to None,`Rules.metadata.space` will be used
     """
 
-    def __init__(self, include_pipeline: bool = False, instance_space: str | None = None):
+    def __init__(
+        self,
+        rules: DMSRules,
+        include_ref: bool = True,
+        include_pipeline: bool = False,
+        instance_space: str | None = None,
+    ):
+        self.include_ref = include_ref
         self.include_pipeline = include_pipeline
         self.instance_space = instance_space
+        self.rules = rules
+        self._ref_schema = rules.reference.as_schema() if rules.reference else None
+        if self._ref_schema:
+            # We skip version as that will always be missing in the reference
+            self._ref_views_by_id = {dm.ViewId(view.space, view.external_id): view for view in self._ref_schema.views}
+        else:
+            self._ref_views_by_id = {}
 
-    def to_schema(self, rules: DMSRules) -> DMSSchema:
-        container_properties_by_id, view_properties_by_id = self._gather_properties(rules)
-
-        containers = self._create_containers(rules.containers, container_properties_by_id)
+    def to_schema(self) -> DMSSchema:
+        rules = self.rules
+        container_properties_by_id, view_properties_by_id = self._gather_properties()
+        containers = self._create_containers(container_properties_by_id)
 
-        views, node_types = self._create_views_with_node_types(rules.views, view_properties_by_id)
+        views, node_types = self._create_views_with_node_types(view_properties_by_id)
 
         views_not_in_model = {view.view.as_id() for view in rules.views if not view.in_model}
         data_model = rules.metadata.as_data_model()
         data_model.views = sorted(
             [view_id for view_id in views.as_ids() if view_id not in views_not_in_model],
             key=lambda v: v.as_tuple(),  # type: ignore[union-attr]
         )
@@ -665,14 +691,24 @@
             data_models=dm.DataModelApplyList([data_model]),
             views=views,
             containers=containers,
             node_types=node_types,
         )
         if self.include_pipeline:
             return PipelineSchema.from_dms(output, self.instance_space)
+
+        if self._ref_schema and self.include_ref:
+            output.frozen_ids.update(self._ref_schema.node_types.as_ids())
+            output.frozen_ids.update(self._ref_schema.views.as_ids())
+            output.frozen_ids.update(self._ref_schema.containers.as_ids())
+            output.node_types.extend(self._ref_schema.node_types)
+            output.views.extend(self._ref_schema.views)
+            output.containers.extend(self._ref_schema.containers)
+            output.data_models.extend(self._ref_schema.data_models)
+
         return output
 
     def _create_spaces(
         self,
         metadata: DMSMetadata,
         containers: dm.ContainerApplyList,
         views: dm.ViewApplyList,
@@ -688,213 +724,85 @@
             spaces = dm.SpaceApplyList([dm.SpaceApply(space=space) for space in used_spaces])
         if self.instance_space and self.instance_space not in {space.space for space in spaces}:
             spaces.append(dm.SpaceApply(space=self.instance_space, name=self.instance_space))
         return spaces
 
     def _create_views_with_node_types(
         self,
-        dms_views: SheetList[DMSView],
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]],
     ) -> tuple[dm.ViewApplyList, dm.NodeApplyList]:
-        views = dm.ViewApplyList([dms_view.as_view() for dms_view in dms_views])
-        dms_view_by_id = {dms_view.view.as_id(): dms_view for dms_view in dms_views}
+        views = dm.ViewApplyList([dms_view.as_view() for dms_view in self.rules.views])
+        dms_view_by_id = {dms_view.view.as_id(): dms_view for dms_view in self.rules.views}
 
         for view in views:
             view_id = view.as_id()
             view.properties = {}
             if not (view_properties := view_properties_by_id.get(view_id)):
                 continue
             for prop in view_properties:
-                view_property: ViewPropertyApply
-                if prop.is_list and prop.relation == "direct":
-                    # This is not yet supported in the CDF API, a warning has already been issued, here we convert it to
-                    # a multi-edge connection.
-                    if isinstance(prop.value_type, ViewEntity):
-                        source_view_id = prop.value_type.as_id()
-                    elif isinstance(prop.value_type, ViewPropertyEntity):
-                        source_view_id = prop.value_type.as_view_id()
-                    else:
-                        raise ValueError(
-                            "Direct relation must have a view as value type. "
-                            "This should have been validated in the rules"
-                        )
-                    view_property = dm.MultiEdgeConnectionApply(
-                        type=dm.DirectRelationReference(
-                            space=source_view_id.space,
-                            external_id=f"{prop.view.external_id}.{prop.view_property}",
-                        ),
-                        source=source_view_id,
-                        direction="outwards",
-                        name=prop.name,
-                        description=prop.description,
-                    )
-                elif prop.container and prop.container_property and prop.view_property:
-                    container_prop_identifier = prop.container_property
-                    extra_args: dict[str, Any] = {}
-                    if prop.relation == "direct" and isinstance(prop.value_type, ViewEntity):
-                        extra_args["source"] = prop.value_type.as_id()
-                    elif isinstance(prop.value_type, DMSUnknownEntity):
-                        extra_args["source"] = None
-                    elif prop.relation == "direct" and not isinstance(prop.value_type, ViewEntity):
-                        raise ValueError(
-                            "Direct relation must have a view as value type. "
-                            "This should have been validated in the rules"
-                        )
-                    view_property = dm.MappedPropertyApply(
-                        container=prop.container.as_id(),
-                        container_property_identifier=container_prop_identifier,
-                        name=prop.name,
-                        description=prop.description,
-                        **extra_args,
-                    )
-                elif prop.view and prop.view_property and prop.relation == "multiedge":
-                    if isinstance(prop.value_type, ViewEntity):
-                        source_view_id = prop.value_type.as_id()
-                    else:
-                        raise ValueError(
-                            "Multiedge relation must have a view as value type. "
-                            "This should have been validated in the rules"
-                        )
-                    if isinstance(prop.reference, ReferenceEntity):
-                        ref_view_prop = prop.reference.as_view_property_id()
-                        edge_type = dm.DirectRelationReference(
-                            space=ref_view_prop.source.space,
-                            external_id=f"{ref_view_prop.source.external_id}.{ref_view_prop.property}",
-                        )
-                    else:
-                        edge_type = dm.DirectRelationReference(
-                            space=source_view_id.space,
-                            external_id=f"{prop.view.external_id}.{prop.view_property}",
-                        )
+                view_property = self._create_view_property(prop, view_properties_by_id)
+                if view_property is not None:
+                    view.properties[prop.view_property] = view_property
 
-                    view_property = dm.MultiEdgeConnectionApply(
-                        type=edge_type,
-                        source=source_view_id,
-                        direction="outwards",
-                        name=prop.name,
-                        description=prop.description,
-                    )
-                elif prop.view and prop.view_property and prop.relation == "reversedirect":
-                    if isinstance(prop.value_type, ViewPropertyEntity):
-                        source_prop_id = prop.value_type.as_id()
-                        source_view_id = cast(dm.ViewId, source_prop_id.source)
-                    else:
-                        raise ValueError(
-                            "Reverse direct relation must have a view as value type. "
-                            "This should have been validated in the rules"
-                        )
-                    source_prop = prop.value_type.property_
-                    if source_prop is None:
-                        raise ValueError(
-                            "Reverse direct relation must set what it is the reverse property of. "
-                            f"Which property in {prop.value_type.versioned_id} is this the reverse of? Expecting "
-                            f"{prop.value_type.versioned_id}:<property>"
-                        )
-                    reverse_prop = next(
-                        (
-                            prop
-                            for prop in view_properties_by_id.get(source_view_id, [])
-                            if prop.property_ == source_prop
-                        ),
-                        None,
-                    )
-                    if reverse_prop and reverse_prop.relation == "direct" and reverse_prop.is_list:
-                        warnings.warn(
-                            issues.dms.ReverseOfDirectRelationListWarning(view_id, prop.property_), stacklevel=2
-                        )
-                        if isinstance(reverse_prop.reference, ReferenceEntity):
-                            ref_view_prop = reverse_prop.reference.as_view_property_id()
-                            edge_type = dm.DirectRelationReference(
-                                space=ref_view_prop.source.space,
-                                external_id=f"{ref_view_prop.source.external_id}.{ref_view_prop.property}",
-                            )
-                        else:
-                            edge_type = dm.DirectRelationReference(
-                                space=source_prop_id.source.space,
-                                external_id=f"{reverse_prop.view.external_id}.{reverse_prop.view_property}",
-                            )
-                        view_property = dm.MultiEdgeConnectionApply(
-                            type=edge_type,
-                            source=source_prop_id.source,  # type: ignore[arg-type]
-                            direction="inwards",
-                            name=prop.name,
-                            description=prop.description,
-                        )
-                    else:
-                        args: dict[str, Any] = dict(
-                            source=source_view_id,
-                            through=dm.PropertyId(source_prop_id.source, source_prop),
-                            description=prop.description,
-                            name=prop.name,
-                        )
-                        reverse_direct_cls: dict[
-                            bool | None,
-                            type[dm.MultiReverseDirectRelationApply] | type[SingleReverseDirectRelationApply],
-                        ] = {
-                            True: dm.MultiReverseDirectRelationApply,
-                            False: SingleReverseDirectRelationApply,
-                            None: dm.MultiReverseDirectRelationApply,
-                        }
-
-                        view_property = reverse_direct_cls[prop.is_list](**args)
-                elif prop.view and prop.view_property and prop.relation:
-                    warnings.warn(
-                        issues.dms.UnsupportedRelationWarning(view_id, prop.view_property, prop.relation), stacklevel=2
-                    )
-                    continue
-                else:
-                    continue
-                prop_id = prop.view_property
-                view.properties[prop_id] = view_property
-
-        node_types = dm.NodeApplyList([])
+        data_model_type = self.rules.metadata.data_model_type
+        unique_node_types: set[dm.NodeId] = set()
         parent_views = {parent for view in views for parent in view.implements or []}
         for view in views:
-            ref_containers = sorted(view.referenced_containers(), key=lambda c: c.as_tuple())
             dms_view = dms_view_by_id.get(view.as_id())
-            has_data = dm.filters.HasData(containers=list(ref_containers)) if ref_containers else None
-            if dms_view and isinstance(dms_view.reference, ReferenceEntity):
-                # If the view is a reference, we implement the reference view,
-                # and need the filter to match the reference
-                ref_view = dms_view.reference.as_view_id()
-                node_type = dm.filters.Equals(
-                    ["node", "type"], {"space": ref_view.space, "externalId": ref_view.external_id}
-                )
-            else:
-                node_type = dm.filters.Equals(["node", "type"], {"space": view.space, "externalId": view.external_id})
-            if view.as_id() in parent_views:
-                if dms_view and dms_view.filter_ == "nodeType":
+            dms_properties = view_properties_by_id.get(view.as_id(), [])
+            view_filter = self._create_view_filter(view, dms_view, data_model_type, dms_properties)
+
+            view.filter = view_filter.as_dms_filter()
+
+            if isinstance(view_filter, NodeTypeFilter):
+                unique_node_types.update(view_filter.nodes)
+                if view.as_id() in parent_views:
                     warnings.warn(issues.dms.NodeTypeFilterOnParentViewWarning(view.as_id()), stacklevel=2)
-                    view.filter = node_type
-                    node_types.append(dm.NodeApply(space=view.space, external_id=view.external_id, sources=[]))
+            elif isinstance(view_filter, HasDataFilter) and data_model_type == DataModelType.solution:
+                if dms_view and isinstance(dms_view.reference, ReferenceEntity):
+                    references = {dms_view.reference.as_view_id()}
+                elif any(True for prop in dms_properties if isinstance(prop.reference, ReferenceEntity)):
+                    references = {
+                        prop.reference.as_view_id()
+                        for prop in dms_properties
+                        if isinstance(prop.reference, ReferenceEntity)
+                    }
                 else:
-                    view.filter = has_data
-            elif has_data is None:
-                # Child filter without container properties
-                if dms_view and dms_view.filter_ == "hasData":
-                    warnings.warn(issues.dms.HasDataFilterOnNoPropertiesViewWarning(view.as_id()), stacklevel=2)
-                view.filter = node_type
-                node_types.append(dm.NodeApply(space=view.space, external_id=view.external_id, sources=[]))
-            else:
-                if dms_view and (dms_view.filter_ == "hasData" or dms_view.filter_ is None):
-                    # Default option
-                    view.filter = has_data
-                elif dms_view and dms_view.filter_ == "nodeType":
-                    view.filter = node_type
-                    node_types.append(dm.NodeApply(space=view.space, external_id=view.external_id, sources=[]))
-                else:
-                    view.filter = has_data
-        return views, node_types
+                    continue
+                warnings.warn(
+                    issues.dms.HasDataFilterOnViewWithReferencesWarning(view.as_id(), list(references)), stacklevel=2
+                )
+
+        return views, dm.NodeApplyList(
+            [dm.NodeApply(space=node.space, external_id=node.external_id) for node in unique_node_types]
+        )
+
+    @classmethod
+    def _create_edge_type_from_prop(cls, prop: DMSProperty) -> dm.DirectRelationReference:
+        if isinstance(prop.reference, ReferenceEntity):
+            ref_view_prop = prop.reference.as_view_property_id()
+            return cls._create_edge_type_from_view_id(cast(dm.ViewId, ref_view_prop.source), ref_view_prop.property)
+        else:
+            return cls._create_edge_type_from_view_id(prop.view.as_id(), prop.view_property)
+
+    @staticmethod
+    def _create_edge_type_from_view_id(view_id: dm.ViewId, property_: str) -> dm.DirectRelationReference:
+        return dm.DirectRelationReference(
+            space=view_id.space,
+            # This is the same convention as used when converting GraphQL to DMS
+            external_id=f"{view_id.external_id}.{property_}",
+        )
 
     def _create_containers(
         self,
-        dms_container: SheetList[DMSContainer] | None,
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]],
     ) -> dm.ContainerApplyList:
-        containers = dm.ContainerApplyList([dms_container.as_container() for dms_container in dms_container or []])
+        containers = dm.ContainerApplyList(
+            [dms_container.as_container() for dms_container in self.rules.containers or []]
+        )
         container_to_drop = set()
         for container in containers:
             container_id = container.as_id()
             if not (container_properties := container_properties_by_id.get(container_id)):
                 warnings.warn(issues.dms.EmptyContainerWarning(container_id=container_id), stacklevel=2)
                 container_to_drop.add(container_id)
                 continue
@@ -902,34 +810,22 @@
                 if prop.container_property is None:
                     continue
                 if isinstance(prop.value_type, DataType):
                     type_cls = prop.value_type.dms
                 else:
                     type_cls = dm.DirectRelation
 
-                prop_id = prop.container_property
-
-                if type_cls is dm.DirectRelation:
-                    container.properties[prop_id] = dm.ContainerProperty(
-                        type=dm.DirectRelation(),
-                        nullable=prop.nullable if prop.nullable is not None else True,
-                        default_value=prop.default,
-                        name=prop.name,
-                        description=prop.description,
-                    )
-                else:
-                    type_: CognitePropertyType
-                    type_ = type_cls(is_list=prop.is_list or False)
-                    container.properties[prop_id] = dm.ContainerProperty(
-                        type=type_,
-                        nullable=prop.nullable if prop.nullable is not None else True,
-                        default_value=prop.default,
-                        name=prop.name,
-                        description=prop.description,
-                    )
+                type_ = type_cls(is_list=prop.is_list or False)
+                container.properties[prop.container_property] = dm.ContainerProperty(
+                    type=type_,
+                    nullable=prop.nullable if prop.nullable is not None else True,
+                    default_value=prop.default,
+                    name=prop.name,
+                    description=prop.description,
+                )
 
             uniqueness_properties: dict[str, set[str]] = defaultdict(set)
             for prop in container_properties:
                 if prop.container_property is not None:
                     for constraint in prop.constraint or []:
                         uniqueness_properties[constraint].add(prop.container_property)
             for constraint_name, properties in uniqueness_properties.items():
@@ -954,39 +850,183 @@
                     for name, const in container.constraints.items()
                     if not (isinstance(const, dm.RequiresConstraint) and const.require in container_to_drop)
                 }
         return dm.ContainerApplyList(
             [container for container in containers if container.as_id() not in container_to_drop]
         )
 
-    def _gather_properties(
-        self, rules: DMSRules
-    ) -> tuple[dict[dm.ContainerId, list[DMSProperty]], dict[dm.ViewId, list[DMSProperty]]]:
+    def _gather_properties(self) -> tuple[dict[dm.ContainerId, list[DMSProperty]], dict[dm.ViewId, list[DMSProperty]]]:
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]] = defaultdict(list)
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]] = defaultdict(list)
-        for prop in rules.properties:
+        for prop in self.rules.properties:
             view_id = prop.view.as_id()
             view_properties_by_id[view_id].append(prop)
 
             if prop.container and prop.container_property:
-                if prop.relation == "direct" and prop.is_list:
-                    warnings.warn(
-                        issues.dms.DirectRelationListWarning(
-                            container_id=prop.container.as_id(),
-                            view_id=prop.view.as_id(),
-                            property=prop.container_property,
-                        ),
-                        stacklevel=2,
-                    )
-                    continue
                 container_id = prop.container.as_id()
                 container_properties_by_id[container_id].append(prop)
 
         return container_properties_by_id, view_properties_by_id
 
+    def _create_view_filter(
+        self,
+        view: dm.ViewApply,
+        dms_view: DMSView | None,
+        data_model_type: DataModelType,
+        dms_properties: list[DMSProperty],
+    ) -> DMSFilter:
+        selected_filter_name = (dms_view and dms_view.filter_ and dms_view.filter_.name) or ""
+        if dms_view and dms_view.filter_ and not dms_view.filter_.is_empty:
+            # Has Explicit Filter, use it
+            return dms_view.filter_
+
+        if data_model_type == DataModelType.solution and selected_filter_name in [NodeTypeFilter.name, ""]:
+            if (
+                dms_view
+                and isinstance(dms_view.reference, ReferenceEntity)
+                and not dms_properties
+                and (ref_view := self._ref_views_by_id.get(dms_view.reference.as_view_id()))
+                and ref_view.filter
+            ):
+                # No new properties, only reference, reuse the reference filter
+                return DMSFilter.from_dms_filter(ref_view.filter)
+            else:
+                referenced_node_ids = {
+                    prop.reference.as_node_entity()
+                    for prop in dms_properties
+                    if isinstance(prop.reference, ReferenceEntity)
+                }
+                if dms_view and isinstance(dms_view.reference, ReferenceEntity):
+                    referenced_node_ids.add(dms_view.reference.as_node_entity())
+                if referenced_node_ids:
+                    return NodeTypeFilter(inner=list(referenced_node_ids))
+
+        # Enterprise Model or (Solution + HasData)
+        ref_containers = view.referenced_containers()
+        if not ref_containers or selected_filter_name == HasDataFilter.name:
+            # Child filter without container properties
+            if selected_filter_name == HasDataFilter.name:
+                warnings.warn(issues.dms.HasDataFilterOnNoPropertiesViewWarning(view.as_id()), stacklevel=2)
+            return NodeTypeFilter(inner=[DMSNodeEntity(space=view.space, externalId=view.external_id)])
+        else:
+            # HasData or not provided (this is the default)
+            return HasDataFilter(inner=[ContainerEntity.from_id(id_) for id_ in ref_containers])
+
+    def _create_view_property(
+        self, prop: DMSProperty, view_properties_by_id: dict[dm.ViewId, list[DMSProperty]]
+    ) -> ViewPropertyApply | None:
+        if prop.container and prop.container_property:
+            container_prop_identifier = prop.container_property
+            extra_args: dict[str, Any] = {}
+            if prop.connection == "direct":
+                if isinstance(prop.value_type, ViewEntity):
+                    extra_args["source"] = prop.value_type.as_id()
+                elif isinstance(prop.value_type, DMSUnknownEntity):
+                    extra_args["source"] = None
+                else:
+                    # Should have been validated.
+                    raise ValueError(
+                        "If this error occurs it is a bug in NEAT, please report"
+                        f"Debug Info, Invalid valueType direct: {prop.model_dump_json()}"
+                    )
+            elif prop.connection is not None:
+                # Should have been validated.
+                raise ValueError(
+                    "If this error occurs it is a bug in NEAT, please report"
+                    f"Debug Info, Invalid connection: {prop.model_dump_json()}"
+                )
+            return dm.MappedPropertyApply(
+                container=prop.container.as_id(),
+                container_property_identifier=container_prop_identifier,
+                name=prop.name,
+                description=prop.description,
+                **extra_args,
+            )
+        elif prop.connection == "edge":
+            if isinstance(prop.value_type, ViewEntity):
+                source_view_id = prop.value_type.as_id()
+            else:
+                # Should have been validated.
+                raise ValueError(
+                    "If this error occurs it is a bug in NEAT, please report"
+                    f"Debug Info, Invalid valueType edge: {prop.model_dump_json()}"
+                )
+            edge_cls: type[dm.EdgeConnectionApply] = dm.MultiEdgeConnectionApply
+            # If is_list is not set, we default to a MultiEdgeConnection
+            if prop.is_list is False:
+                edge_cls = SingleEdgeConnectionApply
+
+            return edge_cls(
+                type=self._create_edge_type_from_prop(prop),
+                source=source_view_id,
+                direction="outwards",
+                name=prop.name,
+                description=prop.description,
+            )
+        elif prop.connection == "reverse":
+            reverse_prop_id: str | None = None
+            if isinstance(prop.value_type, ViewPropertyEntity):
+                source_view_id = prop.value_type.as_view_id()
+                reverse_prop_id = prop.value_type.property_
+            elif isinstance(prop.value_type, ViewEntity):
+                source_view_id = prop.value_type.as_id()
+            else:
+                # Should have been validated.
+                raise ValueError(
+                    "If this error occurs it is a bug in NEAT, please report"
+                    f"Debug Info, Invalid valueType reverse connection: {prop.model_dump_json()}"
+                )
+            reverse_prop: DMSProperty | None = None
+            if reverse_prop_id is not None:
+                reverse_prop = next(
+                    (
+                        prop
+                        for prop in view_properties_by_id.get(source_view_id, [])
+                        if prop.property_ == reverse_prop_id
+                    ),
+                    None,
+                )
+
+            if reverse_prop is None:
+                warnings.warn(
+                    issues.dms.ReverseRelationMissingOtherSideWarning(source_view_id, prop.view_property),
+                    stacklevel=2,
+                )
+
+            if reverse_prop is None or reverse_prop.connection == "edge":
+                inwards_edge_cls = (
+                    dm.MultiEdgeConnectionApply if prop.is_list in [True, None] else SingleEdgeConnectionApply
+                )
+                return inwards_edge_cls(
+                    type=self._create_edge_type_from_prop(reverse_prop or prop),
+                    source=source_view_id,
+                    name=prop.name,
+                    description=prop.description,
+                    direction="inwards",
+                )
+            elif reverse_prop_id and reverse_prop and reverse_prop.connection == "direct":
+                reverse_direct_cls = (
+                    dm.MultiReverseDirectRelationApply if prop.is_list is True else SingleReverseDirectRelationApply
+                )
+                return reverse_direct_cls(
+                    source=source_view_id,
+                    through=dm.PropertyId(source=source_view_id, property=reverse_prop_id),
+                    name=prop.name,
+                    description=prop.description,
+                )
+            else:
+                return None
+
+        elif prop.view and prop.view_property and prop.connection:
+            warnings.warn(
+                issues.dms.UnsupportedConnectionWarning(prop.view.as_id(), prop.view_property, prop.connection or ""),
+                stacklevel=2,
+            )
+        return None
+
 
 class _DMSRulesConverter:
     def __init__(self, dms: DMSRules):
         self.dms = dms
 
     def as_domain_rules(self) -> "DomainRules":
         raise NotImplementedError("DomainRules not implemented yet")
@@ -1089,7 +1129,127 @@
             return None
         container = cast(ContainerEntity, property_.container)
         return ReferenceEntity(
             prefix=container.prefix,
             suffix=container.suffix,
             property=property_.container_property,
         )
+
+
+class _DMSRulesSerializer:
+    # These are the fields that need to be cleaned from the default space and version
+    PROPERTIES_FIELDS: ClassVar[list[str]] = ["class_", "view", "value_type", "container"]
+    VIEWS_FIELDS: ClassVar[list[str]] = ["class_", "view", "implements"]
+    CONTAINERS_FIELDS: ClassVar[list[str]] = ["class_", "container"]
+
+    def __init__(self, info: SerializationInfo, default_space: str, default_version: str) -> None:
+        self.default_space = f"{default_space}:"
+        self.default_version = f"version={default_version}"
+        self.default_version_wrapped = f"({self.default_version})"
+
+        self.properties_fields = self.PROPERTIES_FIELDS
+        self.views_fields = self.VIEWS_FIELDS
+        self.containers_fields = self.CONTAINERS_FIELDS
+        self.prop_name = "properties"
+        self.view_name = "views"
+        self.container_name = "containers"
+        self.metadata_name = "metadata"
+        self.prop_view = "view"
+        self.prop_view_property = "view_property"
+        self.prop_value_type = "value_type"
+        self.view_view = "view"
+        self.view_implements = "implements"
+        self.container_container = "container"
+        self.container_constraint = "constraint"
+
+        if info.by_alias:
+            self.properties_fields = [
+                DMSProperty.model_fields[field].alias or field for field in self.properties_fields
+            ]
+            self.views_fields = [DMSView.model_fields[field].alias or field for field in self.views_fields]
+            self.container_fields = [
+                DMSContainer.model_fields[field].alias or field for field in self.containers_fields
+            ]
+            self.prop_view = DMSProperty.model_fields[self.prop_view].alias or self.prop_view
+            self.prop_view_property = DMSProperty.model_fields[self.prop_view_property].alias or self.prop_view_property
+            self.prop_value_type = DMSProperty.model_fields[self.prop_value_type].alias or self.prop_value_type
+            self.view_view = DMSView.model_fields[self.view_view].alias or self.view_view
+            self.view_implements = DMSView.model_fields[self.view_implements].alias or self.view_implements
+            self.container_container = (
+                DMSContainer.model_fields[self.container_container].alias or self.container_container
+            )
+            self.container_constraint = (
+                DMSContainer.model_fields[self.container_constraint].alias or self.container_constraint
+            )
+            self.prop_name = DMSRules.model_fields[self.prop_name].alias or self.prop_name
+            self.view_name = DMSRules.model_fields[self.view_name].alias or self.view_name
+            self.container_name = DMSRules.model_fields[self.container_name].alias or self.container_name
+            self.metadata_name = DMSRules.model_fields[self.metadata_name].alias or self.metadata_name
+
+        if isinstance(info.exclude, dict):
+            # Just for happy mypy
+            exclude = cast(dict, info.exclude)
+            self.exclude_properties = exclude.get("properties", {}).get("__all__", set())
+            self.exclude_views = exclude.get("views", {}).get("__all__", set()) or set()
+            self.exclude_containers = exclude.get("containers", {}).get("__all__", set()) or set()
+            self.metadata_exclude = exclude.get("metadata", set()) or set()
+            self.exclude_top = {k for k, v in exclude.items() if not v}
+        else:
+            self.exclude_top = set(info.exclude or {})
+            self.exclude_properties = set()
+            self.exclude_views = set()
+            self.exclude_containers = set()
+            self.metadata_exclude = set()
+
+    def clean(self, dumped: dict[str, Any]) -> dict[str, Any]:
+        # Sorting to get a deterministic order
+        dumped[self.prop_name] = sorted(
+            dumped[self.prop_name]["data"], key=lambda p: (p[self.prop_view], p[self.prop_view_property])
+        )
+        dumped[self.view_name] = sorted(dumped[self.view_name]["data"], key=lambda v: v[self.view_view])
+        if self.container_name in dumped:
+            dumped[self.container_name] = sorted(
+                dumped[self.container_name]["data"], key=lambda c: c[self.container_container]
+            )
+
+        for prop in dumped[self.prop_name]:
+            for field_name in self.properties_fields:
+                if value := prop.get(field_name):
+                    prop[field_name] = value.removeprefix(self.default_space).removesuffix(self.default_version_wrapped)
+            # Value type can have a property as well
+            prop[self.prop_value_type] = prop[self.prop_value_type].replace(self.default_version, "")
+            if self.exclude_properties:
+                for field in self.exclude_properties:
+                    prop.pop(field, None)
+
+        for view in dumped[self.view_name]:
+            for field_name in self.views_fields:
+                if value := view.get(field_name):
+                    view[field_name] = value.removeprefix(self.default_space).removesuffix(self.default_version_wrapped)
+            if value := view.get(self.view_implements):
+                view[self.view_implements] = ",".join(
+                    parent.strip().removeprefix(self.default_space).removesuffix(self.default_version_wrapped)
+                    for parent in value.split(",")
+                )
+            if self.exclude_views:
+                for field in self.exclude_views:
+                    view.pop(field, None)
+
+        for container in dumped[self.container_name]:
+            for field_name in self.containers_fields:
+                if value := container.get(field_name):
+                    container[field_name] = value.removeprefix(self.default_space)
+
+            if value := container.get(self.container_constraint):
+                container[self.container_constraint] = ",".join(
+                    constraint.strip().removeprefix(self.default_space) for constraint in value.split(",")
+                )
+            if self.exclude_containers:
+                for field in self.exclude_containers:
+                    container.pop(field, None)
+
+        if self.metadata_exclude:
+            for field in self.metadata_exclude:
+                dumped[self.metadata_name].pop(field, None)
+        for field in self.exclude_top:
+            dumped.pop(field, None)
+        return dumped
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_dms_rules_write.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_dms_rules_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,77 +11,77 @@
     ContainerEntity,
     DMSUnknownEntity,
     Unknown,
     ViewEntity,
     ViewPropertyEntity,
 )
 
-from ._base import ExtensionCategory, SchemaCompleteness
+from ._base import DataModelType, ExtensionCategory, SchemaCompleteness
 from ._dms_architect_rules import DMSContainer, DMSMetadata, DMSProperty, DMSRules, DMSView
 
 
 @dataclass
 class DMSMetadataWrite:
     schema_: Literal["complete", "partial", "extended"]
     space: str
     external_id: str
     creator: str
     version: str
     extension: Literal["addition", "reshape", "rebuild"] = "addition"
+    data_model_type: Literal["solution", "enterprise"] = "solution"
     name: str | None = None
     description: str | None = None
     created: datetime | str | None = None
     updated: datetime | str | None = None
-    default_view_version: str | None = None
 
     @classmethod
     def load(cls, data: dict[str, Any] | None) -> "DMSMetadataWrite | None":
         if data is None:
             return None
         _add_alias(data, DMSMetadata)
         return cls(
             schema_=data.get("schema_"),  # type: ignore[arg-type]
             space=data.get("space"),  # type: ignore[arg-type]
             external_id=data.get("external_id"),  # type: ignore[arg-type]
             creator=data.get("creator"),  # type: ignore[arg-type]
             version=data.get("version"),  # type: ignore[arg-type]
             extension=data.get("extension", "addition"),
+            data_model_type=data.get("data_model_type", "solution"),
             name=data.get("name"),
             description=data.get("description"),
             created=data.get("created"),
             updated=data.get("updated"),
-            default_view_version=data.get("default_view_version"),
         )
 
     def dump(self) -> dict[str, Any]:
         return dict(
             schema=SchemaCompleteness(self.schema_),
             extension=ExtensionCategory(self.extension),
             space=self.space,
             externalId=self.external_id,
+            dataModelType=DataModelType(self.data_model_type),
             creator=self.creator,
             version=self.version,
             name=self.name,
             description=self.description,
             created=self.created or datetime.now(),
             updated=self.updated or datetime.now(),
-            default_view_version=self.default_view_version or self.version,
         )
 
 
 @dataclass
 class DMSPropertyWrite:
     view: str
     view_property: str | None
     value_type: str
     property_: str | None
     class_: str | None = None
     name: str | None = None
     description: str | None = None
-    relation: Literal["direct", "reversedirect", "multiedge"] | None = None
+    connection: Literal["direct", "edge", "reverse"] | None = None
     nullable: bool | None = None
     is_list: bool | None = None
     default: str | int | dict | None = None
     reference: str | None = None
     container: str | None = None
     container_property: str | None = None
     index: str | list[str] | None = None
@@ -114,15 +114,15 @@
             view=data.get("view"),  # type: ignore[arg-type]
             view_property=data.get("view_property"),  # type: ignore[arg-type]
             value_type=data.get("value_type"),  # type: ignore[arg-type]
             property_=data.get("property_"),
             class_=data.get("class_"),
             name=data.get("name"),
             description=data.get("description"),
-            relation=data.get("relation"),
+            connection=data.get("connection"),
             nullable=data.get("nullable"),
             is_list=data.get("is_list"),
             default=data.get("default"),
             reference=data.get("reference"),
             container=data.get("container"),
             container_property=data.get("container_property"),
             index=data.get("index"),
@@ -139,31 +139,31 @@
             try:
                 value_type = ViewPropertyEntity.load(self.value_type, space=default_space, version=default_version)
             except ValueError:
                 value_type = ViewEntity.load(self.value_type, space=default_space, version=default_version)
 
         return {
             "View": ViewEntity.load(self.view, space=default_space, version=default_version),
-            "ViewProperty": self.view_property,
+            "View Property": self.view_property,
             "Value Type": value_type,
-            "Property": self.property_ or self.view_property,
-            "Class": ClassEntity.load(self.class_, prefix=default_space, version=default_version)
+            "Property (linage)": self.property_ or self.view_property,
+            "Class (linage)": ClassEntity.load(self.class_, prefix=default_space, version=default_version)
             if self.class_
             else None,
             "Name": self.name,
             "Description": self.description,
-            "Relation": self.relation,
+            "Connection": self.connection,
             "Nullable": self.nullable,
-            "IsList": self.is_list,
+            "Is List": self.is_list,
             "Default": self.default,
             "Reference": self.reference,
             "Container": ContainerEntity.load(self.container, space=default_space, version=default_version)
             if self.container
             else None,
-            "ContainerProperty": self.container_property,
+            "Container Property": self.container_property,
             "Index": self.index,
             "Constraint": self.constraint,
         }
 
 
 @dataclass
 class DMSContainerWrite:
@@ -204,27 +204,29 @@
             description=data.get("description"),
             reference=data.get("reference"),
             constraint=data.get("constraint"),
         )
 
     def dump(self, default_space: str) -> dict[str, Any]:
         container = ContainerEntity.load(self.container, space=default_space)
-        return dict(
-            Container=container,
-            Class=ClassEntity.load(self.class_, prefix=default_space) if self.class_ else container.as_class(),
-            Name=self.name,
-            Description=self.description,
-            Reference=self.reference,
-            Constraint=[
+        return {
+            "Container": container,
+            "Class (linage)": ClassEntity.load(self.class_, prefix=default_space)
+            if self.class_
+            else container.as_class(),
+            "Name": self.name,
+            "Description": self.description,
+            "Reference": self.reference,
+            "Constraint": [
                 ContainerEntity.load(constraint.strip(), space=default_space)
                 for constraint in self.constraint.split(",")
             ]
             if self.constraint
             else None,
-        )
+        }
 
 
 @dataclass
 class DMSViewWrite:
     view: str
     class_: str | None = None
     name: str | None = None
@@ -264,31 +266,31 @@
             reference=data.get("reference"),
             filter_=data.get("filter_"),
             in_model=data.get("in_model", True),
         )
 
     def dump(self, default_space: str, default_version: str) -> dict[str, Any]:
         view = ViewEntity.load(self.view, space=default_space, version=default_version)
-        return dict(
-            View=view,
-            Class=ClassEntity.load(self.class_, prefix=default_space, version=default_version)
+        return {
+            "View": view,
+            "Class (linage)": ClassEntity.load(self.class_, prefix=default_space, version=default_version)
             if self.class_
             else view.as_class(),
-            Name=self.name,
-            Description=self.description,
-            Implements=[
+            "Name": self.name,
+            "Description": self.description,
+            "Implements": [
                 ViewEntity.load(implement, space=default_space, version=default_version)
                 for implement in self.implements.split(",")
             ]
             if self.implements
             else None,
-            Reference=self.reference,
-            Filter=self.filter_,
-            InModel=self.in_model,
-        )
+            "Reference": self.reference,
+            "Filter": self.filter_,
+            "In Model": self.in_model,
+        }
 
 
 @dataclass
 class DMSRulesWrite:
     metadata: DMSMetadataWrite
     properties: Sequence[DMSPropertyWrite]
     views: Sequence[DMSViewWrite]
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_dms_schema.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_dms_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import sys
 import warnings
 import zipfile
 from collections import Counter, defaultdict
-from dataclasses import dataclass, field, fields
+from dataclasses import Field, dataclass, field, fields
 from pathlib import Path
 from typing import Any, ClassVar, cast
 
 import yaml
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes import DatabaseWrite, DatabaseWriteList, TransformationWrite, TransformationWriteList
 from cognite.client.data_classes.data_modeling import ViewApply
 from cognite.client.data_classes.transformations.common import Edges, EdgeType, Nodes, ViewInfo
 
+from cognite.neat.rules import issues
 from cognite.neat.rules.issues.dms import (
     ContainerPropertyUsedMultipleTimesError,
     DirectRelationMissingSourceWarning,
     DMSSchemaError,
     DuplicatedViewInDataModelError,
     MissingContainerError,
     MissingContainerPropertyError,
@@ -102,31 +103,41 @@
     @classmethod
     def from_directory(cls, directory: str | Path) -> Self:
         """Load a schema from a directory containing YAML files.
 
         The directory is expected to follow the Cognite-Toolkit convention
         where each file is named as `resource_type.resource_name.yaml`.
         """
-        data = cls._read_directory(Path(directory))
-        return cls.load(data)
+        data, context = cls._read_directory(Path(directory))
+        return cls.load(data, context)
 
     @classmethod
-    def _read_directory(cls, directory: Path) -> dict[str, list[Any]]:
+    def _read_directory(cls, directory: Path) -> tuple[dict[str, list[Any]], dict[str, list[Path]]]:
         data: dict[str, Any] = {}
+        context: dict[str, list[Path]] = {}
         for yaml_file in directory.rglob("*.yaml"):
             if "." in yaml_file.stem:
                 resource_type = yaml_file.stem.rsplit(".", 1)[-1]
                 if attr_name := cls._FIELD_NAME_BY_RESOURCE_TYPE.get(resource_type):
                     data.setdefault(attr_name, [])
-                    loaded = yaml.safe_load(yaml_file.read_text())
+                    context.setdefault(attr_name, [])
+                    try:
+                        # Using CSafeLoader over safe_load for ~10x speedup
+                        loaded = yaml.safe_load(yaml_file.read_text())
+                    except Exception as e:
+                        warnings.warn(issues.fileread.InvalidFileFormatWarning(yaml_file, str(e)), stacklevel=2)
+                        continue
+
                     if isinstance(loaded, list):
                         data[attr_name].extend(loaded)
+                        context[attr_name].extend([yaml_file] * len(loaded))
                     else:
                         data[attr_name].append(loaded)
-        return data
+                        context[attr_name].append(yaml_file)
+        return data, context
 
     def to_directory(
         self,
         directory: str | Path,
         exclude: set[str] | None = None,
         new_line: str | None = "\n",
         encoding: str | None = "utf-8",
@@ -178,37 +189,45 @@
     @classmethod
     def from_zip(cls, zip_file: str | Path) -> Self:
         """Load a schema from a ZIP file containing YAML files.
 
         The ZIP file is expected to follow the Cognite-Toolkit convention
         where each file is named as `resource_type.resource_name.yaml`.
         """
-        data = cls._read_zip(Path(zip_file))
-        return cls.load(data)
+        data, context = cls._read_zip(Path(zip_file))
+        return cls.load(data, context)
 
     @classmethod
-    def _read_zip(cls, zip_file: Path) -> dict[str, list[Any]]:
+    def _read_zip(cls, zip_file: Path) -> tuple[dict[str, list[Any]], dict[str, list[Path]]]:
         data: dict[str, list[Any]] = {}
+        context: dict[str, list[Path]] = {}
         with zipfile.ZipFile(zip_file, "r") as zip_ref:
             for file_info in zip_ref.infolist():
                 if file_info.filename.endswith(".yaml"):
                     if "/" not in file_info.filename:
                         continue
                     filename = Path(file_info.filename.split("/")[-1])
                     if "." not in filename.stem:
                         continue
                     resource_type = filename.stem.rsplit(".", 1)[-1]
                     if attr_name := cls._FIELD_NAME_BY_RESOURCE_TYPE.get(resource_type):
                         data.setdefault(attr_name, [])
-                        loaded = yaml.safe_load(zip_ref.read(file_info).decode())
+                        context.setdefault(attr_name, [])
+                        try:
+                            loaded = yaml.safe_load(zip_ref.read(file_info).decode())
+                        except Exception as e:
+                            warnings.warn(issues.fileread.InvalidFileFormatWarning(filename, str(e)), stacklevel=2)
+                            continue
                         if isinstance(loaded, list):
                             data[attr_name].extend(loaded)
+                            context[attr_name].extend([filename] * len(loaded))
                         else:
                             data[attr_name].append(loaded)
-        return data
+                            context[attr_name].append(filename)
+        return data, context
 
     def to_zip(self, zip_file: str | Path, exclude: set[str] | None = None) -> None:
         """Save the schema to a ZIP file as YAML files. This is compatible with the Cognite-Toolkit convention.
 
         Args:
             zip_file (str | Path): The ZIP file to save the schema to.
             exclude (set[str]): A set of attributes to exclude from the output.
@@ -230,26 +249,71 @@
                         f"data_models/containers{container.external_id}.container.yaml", container.dump_yaml()
                     )
             if "node_types" not in exclude_set:
                 for node in self.node_types:
                     zip_ref.writestr(f"data_models/nodes/{node.external_id}.node.yaml", node.dump_yaml())
 
     @classmethod
-    def load(cls, data: str | dict[str, Any]) -> Self:
+    def load(cls, data: str | dict[str, list[Any]], context: dict[str, list[Path]] | None = None) -> Self:
+        """Loads a schema from a dictionary or a YAML or JSON formatted string.
+
+        Args:
+            data: The data to load the schema from. This can be a dictionary, a YAML or JSON formatted string.
+            context: This provides linage for where the data was loaded from. This is used in Warnings
+                if a single item fails to load.
+
+        Returns:
+            DMSSchema: The loaded schema.
+        """
+        context = context or {}
         if isinstance(data, str):
             # YAML is a superset of JSON, so we can use the same parser
-            data_dict = yaml.safe_load(data)
+            try:
+                data_dict = yaml.safe_load(data)
+            except Exception as e:
+                raise issues.fileread.FailedStringLoadError(".yaml", str(e)).as_exception() from None
+            if not isinstance(data_dict, dict) and all(isinstance(v, list) for v in data_dict.values()):
+                raise issues.fileread.FailedStringLoadError(
+                    "dict[str, list[Any]]", f"Invalid data structure: {type(data)}"
+                ).as_exception() from None
         else:
             data_dict = data
         loaded: dict[str, Any] = {}
         for attr in fields(cls):
             if items := data_dict.get(attr.name) or data_dict.get(to_camel(attr.name)):
-                loaded[attr.name] = attr.type.load(items)
+                try:
+                    loaded[attr.name] = attr.type.load(items)
+                except Exception as e:
+                    loaded[attr.name] = cls._load_individual_resources(items, attr, str(e), context.get(attr.name, []))
         return cls(**loaded)
 
+    @classmethod
+    def _load_individual_resources(cls, items: list, attr: Field, trigger_error: str, resource_context) -> list[Any]:
+        resources = attr.type([])
+        if not hasattr(attr.type, "_RESOURCE"):
+            warnings.warn(
+                issues.fileread.FailedLoadWarning(Path("UNKNOWN"), attr.type.__name__, trigger_error), stacklevel=2
+            )
+            return resources
+        # Fallback to load individual resources.
+        single_cls = attr.type._RESOURCE
+        for no, item in enumerate(items):
+            try:
+                loaded_instance = single_cls.load(item)
+            except Exception as e:
+                try:
+                    filepath = resource_context[no]
+                except IndexError:
+                    filepath = Path("UNKNOWN")
+                # We use repr(e) instead of str(e) to include the exception type in the warning message
+                warnings.warn(issues.fileread.FailedLoadWarning(filepath, single_cls.__name__, repr(e)), stacklevel=2)
+            else:
+                resources.append(loaded_instance)
+        return resources
+
     def dump(self, camel_case: bool = True, sort: bool = True) -> dict[str, Any]:
         """Dump the schema to a dictionary that can be serialized to JSON.
 
         Args:
             camel_case (bool): If True, the keys in the output dictionary will be in camel case.
             sort (bool): If True, the items in the output dictionary will be sorted by their ID.
                 This is useful for deterministic output which is useful for comparing schemas.
@@ -406,14 +470,26 @@
                 "The maximum number of iterations was reached while resolving referenced containers."
                 "There might be referenced containers that are not included in the list of containers.",
                 RuntimeWarning,
                 stacklevel=2,
             )
         return None
 
+    def referenced_spaces(self) -> set[str]:
+        referenced_spaces = {container.space for container in self.containers}
+        referenced_spaces |= {view.space for view in self.views}
+        referenced_spaces |= {container.space for view in self.views for container in view.referenced_containers()}
+        referenced_spaces |= {parent.space for view in self.views for parent in view.implements or []}
+        referenced_spaces |= {node.space for node in self.node_types}
+        referenced_spaces |= {model.space for model in self.data_models}
+        referenced_spaces |= {view.space for model in self.data_models for view in model.views or []}
+        referenced_spaces |= {s.space for s in self.spaces}
+
+        return referenced_spaces
+
 
 @dataclass
 class PipelineSchema(DMSSchema):
     transformations: TransformationWriteList = field(default_factory=lambda: TransformationWriteList([]))
     databases: DatabaseWriteList = field(default_factory=lambda: DatabaseWriteList([]))
     raw_tables: RawTableWriteList = field(default_factory=lambda: RawTableWriteList([]))
 
@@ -425,26 +501,33 @@
     def __post_init__(self):
         existing_databases = {database.name for database in self.databases}
         table_database = {table.database for table in self.raw_tables}
         if missing := table_database - existing_databases:
             self.databases.extend([DatabaseWrite(name=database) for database in missing])
 
     @classmethod
-    def _read_directory(cls, directory: Path) -> dict[str, list[Any]]:
-        data = super()._read_directory(directory)
+    def _read_directory(cls, directory: Path) -> tuple[dict[str, list[Any]], dict[str, list[Path]]]:
+        data, context = super()._read_directory(directory)
         for yaml_file in directory.rglob("*.yaml"):
             if yaml_file.parent.name in ("transformations", "raw"):
                 attr_name = cls._FIELD_NAME_BY_RESOURCE_TYPE.get(yaml_file.parent.name, yaml_file.parent.name)
                 data.setdefault(attr_name, [])
-                loaded = yaml.safe_load(yaml_file.read_text())
+                context.setdefault(attr_name, [])
+                try:
+                    loaded = yaml.safe_load(yaml_file.read_text())
+                except Exception as e:
+                    warnings.warn(issues.fileread.InvalidFileFormatWarning(yaml_file, str(e)), stacklevel=2)
+                    continue
                 if isinstance(loaded, list):
                     data[attr_name].extend(loaded)
+                    context[attr_name].extend([yaml_file] * len(loaded))
                 else:
                     data[attr_name].append(loaded)
-        return data
+                    context[attr_name].append(yaml_file)
+        return data, context
 
     def to_directory(
         self,
         directory: str | Path,
         exclude: set[str] | None = None,
         new_line: str | None = "\n",
         encoding: str | None = "utf-8",
@@ -479,31 +562,38 @@
             if "raw" not in exclude_set:
                 # The RAW Databases are not written to file. This is because cognite-toolkit expects the RAW databases
                 # to be in the same file as the RAW tables.
                 for raw_table in self.raw_tables:
                     zip_ref.writestr(f"raw/{raw_table.name}.yaml", raw_table.dump_yaml())
 
     @classmethod
-    def _read_zip(cls, zip_file: Path) -> dict[str, list[Any]]:
-        data = super()._read_zip(zip_file)
+    def _read_zip(cls, zip_file: Path) -> tuple[dict[str, list[Any]], dict[str, list[Path]]]:
+        data, context = super()._read_zip(zip_file)
         with zipfile.ZipFile(zip_file, "r") as zip_ref:
             for file_info in zip_ref.infolist():
                 if file_info.filename.endswith(".yaml"):
                     if "/" not in file_info.filename:
                         continue
                     filepath = Path(file_info.filename)
                     if (parent := filepath.parent.name) in ("transformations", "raw"):
                         attr_name = cls._FIELD_NAME_BY_RESOURCE_TYPE.get(parent, parent)
                         data.setdefault(attr_name, [])
-                        loaded = yaml.safe_load(zip_ref.read(file_info).decode())
+                        context.setdefault(attr_name, [])
+                        try:
+                            loaded = yaml.safe_load(zip_ref.read(file_info).decode())
+                        except Exception as e:
+                            warnings.warn(issues.fileread.InvalidFileFormatWarning(filepath, str(e)), stacklevel=2)
+                            continue
                         if isinstance(loaded, list):
                             data[attr_name].extend(loaded)
+                            context[attr_name].extend([filepath] * len(loaded))
                         else:
                             data[attr_name].append(loaded)
-        return data
+                            context[attr_name].append(filepath)
+        return data, context
 
     @classmethod
     def from_dms(cls, schema: DMSSchema, instance_space: str | None = None) -> "PipelineSchema":
         if not schema.data_models:
             raise ValueError("PipelineSchema must contain at least one data model")
         first_data_model = schema.data_models[0]
         # The database name is limited to 32 characters
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_domain_rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_domain_rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 
 class DomainMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.domain_expert
     creator: StrOrListType
 
 
 class DomainProperty(SheetEntity):
+    class_: ClassEntity = Field(alias="Class")
     property_: PropertyType = Field(alias="Property")
+    name: str | None = Field(alias="Name", default=None)
+    description: str | None = Field(alias="Description", default=None)
     value_type: DataType | ClassEntity = Field(alias="Value Type")
     min_count: int | None = Field(alias="Min Count", default=None)
     max_count: int | float | None = Field(alias="Max Count", default=None)
 
     @field_serializer("max_count", when_used="json-unless-none")
     def serialize_max_count(self, value: int | float | None) -> int | float | None | str:
         if isinstance(value, float) and math.isinf(value):
@@ -38,14 +41,16 @@
     def parse_max_count(cls, value: int | float | None) -> int | float | None:
         if value is None:
             return float("inf")
         return value
 
 
 class DomainClass(SheetEntity):
+    class_: ClassEntity = Field(alias="Class")
+    name: str | None = Field(alias="Name", default=None)
     description: str | None = Field(None, alias="Description")
     parent: ParentEntityList | None = Field(alias="Parent Class")
 
 
 class DomainRules(RuleModel):
     metadata: DomainMetadata = Field(alias="Metadata")
     properties: SheetList[DomainProperty] = Field(alias="Properties")
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_information_rules.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_information_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     TransformationRuleType,
     Traversal,
     parse_rule,
 )
 
 from ._base import (
     BaseMetadata,
+    DataModelType,
     ExtensionCategory,
     ExtensionCategoryType,
     MatchType,
     RoleTypes,
     RuleModel,
     SchemaCompleteness,
     SheetEntity,
@@ -71,14 +72,15 @@
     from typing import Self
 else:
     from typing_extensions import Self
 
 
 class InformationMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.information_architect
+    data_model_type: DataModelType = Field(DataModelType.solution, alias="dataModelType")
     schema_: SchemaCompleteness = Field(alias="schema")
     extension: ExtensionCategoryType | None = ExtensionCategory.addition
     prefix: PrefixType
     namespace: NamespaceType
 
     name: str = Field(
         alias="title",
@@ -119,14 +121,17 @@
         class_: The class ID of the class.
         description: A description of the class.
         parent: The parent class of the class.
         reference: Reference of the source of the information for given resource
         match_type: The match type of the resource being described and the source entity.
     """
 
+    class_: ClassEntity = Field(alias="Class")
+    name: str | None = Field(alias="Name", default=None)
+    description: str | None = Field(alias="Description", default=None)
     parent: ParentEntityList | None = Field(alias="Parent Class", default=None)
     reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     match_type: MatchType | None = Field(alias="Match Type", default=None)
     comment: str | None = Field(alias="Comment", default=None)
 
 
 class InformationProperty(SheetEntity):
@@ -146,15 +151,18 @@
         match_type: The match type of the resource being described and the source entity.
         rule_type: Rule type for the transformation from source to target representation
                    of knowledge graph. Defaults to None (no transformation)
         rule: Actual rule for the transformation from source to target representation of
               knowledge graph. Defaults to None (no transformation)
     """
 
+    class_: ClassEntity = Field(alias="Class")
     property_: PropertyType = Field(alias="Property")
+    name: str | None = Field(alias="Name", default=None)
+    description: str | None = Field(alias="Description", default=None)
     value_type: DataType | ClassEntity | UnknownEntity = Field(alias="Value Type", union_mode="left_to_right")
     min_count: int | None = Field(alias="Min Count", default=None)
     max_count: int | float | None = Field(alias="Max Count", default=None)
     default: Any | None = Field(alias="Default", default=None)
     reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     match_type: MatchType | None = Field(alias="Match Type", default=None)
     rule_type: str | TransformationRuleType | None = Field(alias="Rule Type", default=None)
@@ -426,15 +434,15 @@
             for cls_ in self.information.classes
         ]
 
         classes_without_properties: set[str] = set()
         for class_ in self.information.classes:
             properties: list[DMSProperty] = properties_by_class.get(class_.class_.versioned_id, [])
             if not properties or all(
-                isinstance(prop.value_type, ViewPropertyEntity) and prop.relation != "direct" for prop in properties
+                isinstance(prop.value_type, ViewPropertyEntity) and prop.connection != "direct" for prop in properties
             ):
                 classes_without_properties.add(class_.class_.versioned_id)
 
         containers: list[DMSContainer] = []
         for class_ in self.information.classes:
             if class_.class_.versioned_id in classes_without_properties:
                 continue
@@ -476,39 +484,38 @@
         elif isinstance(prop.value_type, UnknownEntity):
             value_type = DMSUnknownEntity()
         elif isinstance(prop.value_type, ClassEntity):
             value_type = prop.value_type.as_view_entity(default_space, default_version)
         else:
             raise ValueError(f"Unsupported value type: {prop.value_type.type_}")
 
-        relation: Literal["direct", "multiedge"] | None = None
+        relation: Literal["direct", "edge", "reverse"] | None = None
         if isinstance(value_type, ViewEntity | ViewPropertyEntity):
-            relation = "multiedge" if prop.is_list else "direct"
+            relation = "edge" if prop.is_list else "direct"
 
         container: ContainerEntity | None = None
         container_property: str | None = None
         is_list: bool | None = prop.is_list
         nullable: bool | None = not prop.is_mandatory
-        if relation == "multiedge":
-            is_list = None
+        if relation == "edge":
             nullable = None
         elif relation == "direct":
             nullable = True
             container, container_property = cls._get_container(prop, default_space)
         else:
             container, container_property = cls._get_container(prop, default_space)
 
         return DMSProperty(
             class_=prop.class_,
             name=prop.name,
             property_=prop.property_,
             value_type=value_type,
             nullable=nullable,
             is_list=is_list,
-            relation=relation,
+            connection=relation,
             default=prop.default,
             reference=prop.reference,
             container=container,
             container_property=container_property,
             view=prop.class_.as_view_entity(default_space, default_version),
             view_property=prop.property_,
         )
```

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_types/_base.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/rules/models/rules/_types/_field.py` & `cognite_neat-0.76.0/cognite/neat/rules/models/rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/cdf.py` & `cognite_neat-0.76.0/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.76.0/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/exceptions.py` & `cognite_neat-0.76.0/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.76.0/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/text.py` & `cognite_neat-0.76.0/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/utils.py` & `cognite_neat-0.76.0/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/utils/xml.py` & `cognite_neat-0.76.0/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.76.0/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/base.py` & `cognite_neat-0.76.0/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.76.0/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.76.0/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/manager.py` & `cognite_neat-0.76.0/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.76.0/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.76.0/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/model.py` & `cognite_neat-0.76.0/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.76.0/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/tasks.py` & `cognite_neat-0.76.0/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/cognite/neat/workflows/triggers.py` & `cognite_neat-0.76.0/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.9/pyproject.toml` & `cognite_neat-0.76.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.75.9"
+version = "0.76.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.75.9/PKG-INFO` & `cognite_neat-0.76.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.75.9
+Version: 0.76.0
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

