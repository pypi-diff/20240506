# Comparing `tmp/ttrpgaag-3.0.2.tar.gz` & `tmp/ttrpgaag-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttrpgaag-3.0.2.tar", last modified: Wed Apr 24 12:37:39 2024, max compression
+gzip compressed data, was "ttrpgaag-3.0.3.tar", last modified: Mon May  6 18:13:17 2024, max compression
```

## Comparing `ttrpgaag-3.0.2.tar` & `ttrpgaag-3.0.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.610753 ttrpgaag-3.0.2/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-3.0.2/LICENSE
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-3.0.2/MANIFEST.in
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1169 2024-04-24 12:37:39.610284 ttrpgaag-3.0.2/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      942 2024-04-23 18:50:06.000000 ttrpgaag-3.0.2/README.md
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.561943 ttrpgaag-3.0.2/RPG/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-04-23 18:35:00.000000 ttrpgaag-3.0.2/RPG/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/baralho.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.566280 ttrpgaag-3.0.2/RPG/dado/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-3.0.2/RPG/dado/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-3.0.2/RPG/dado/dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/dado/dados.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.569497 ttrpgaag-3.0.2/RPG/dado/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1513 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/helpers/converter_notacao_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/helpers/monta_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/rolar_dado_notacao.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/iniciativa.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.571281 ttrpgaag-3.0.2/RPG/sistemas/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.574453 ttrpgaag-3.0.2/RPG/sistemas/dnd/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.576318 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/mecanicas.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/tesouro.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.578251 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      406 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/checa_testes.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-01-22 19:11:09.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/rola_tesouro.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5270 2024-02-28 11:57:10.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/teste.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.582308 ttrpgaag-3.0.2/RPG/sistemas/pf2/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/PC.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6182 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/calcula_dano.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.589910 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/defesas_monstros.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/proficiency.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/saves.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/skills.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/tipos_ataques.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/tipos_defesas.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.592666 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/base_calcula_dano.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      856 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/proficiencias.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/proficiencia.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.595230 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1316 2024-04-23 18:43:15.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/consulta_critico.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.597636 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/criticos.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.601222 ttrpgaag-3.0.2/RPG/tabela_rolavel/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2024-04-23 17:09:37.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.605709 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-11 16:29:38.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-04-23 18:48:05.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajeita_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      724 2024-04-23 18:48:05.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajusta_resultados.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/rolamento_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-04-23 18:48:05.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/rolar_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     4480 2024-04-24 11:59:30.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/tabela_rolavel.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.609765 ttrpgaag-3.0.2/TTRPGaag.egg-info/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1169 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/SOURCES.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/dependency_links.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/top_level.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-04-24 12:37:39.610866 ttrpgaag-3.0.2/setup.cfg
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-04-24 12:23:02.000000 ttrpgaag-3.0.2/setup.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.609125 ttrpgaag-3.0.2/tests/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-3.0.2/tests/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.244079 ttrpgaag-3.0.3/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-3.0.3/LICENSE
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-3.0.3/MANIFEST.in
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1413 2024-05-06 18:13:17.243446 ttrpgaag-3.0.3/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1186 2024-05-06 18:09:05.000000 ttrpgaag-3.0.3/README.md
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.213628 ttrpgaag-3.0.3/RPG/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-05-06 18:06:00.000000 ttrpgaag-3.0.3/RPG/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-3.0.3/RPG/baralho.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.215897 ttrpgaag-3.0.3/RPG/dado/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-3.0.3/RPG/dado/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-3.0.3/RPG/dado/dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-3.0.3/RPG/dado/dados.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.217715 ttrpgaag-3.0.3/RPG/dado/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-3.0.3/RPG/dado/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1513 2024-05-06 18:06:00.000000 ttrpgaag-3.0.3/RPG/dado/helpers/converter_notacao_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-3.0.3/RPG/dado/helpers/monta_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2024-05-06 18:06:00.000000 ttrpgaag-3.0.3/RPG/dado/rolar_dado_notacao.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-3.0.3/RPG/iniciativa.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.218355 ttrpgaag-3.0.3/RPG/sistemas/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.3/RPG/sistemas/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.220398 ttrpgaag-3.0.3/RPG/sistemas/dnd/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.222995 ttrpgaag-3.0.3/RPG/sistemas/dnd/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/data/mecanicas.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/data/tesouro.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.224388 ttrpgaag-3.0.3/RPG/sistemas/dnd/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      406 2023-10-11 18:00:52.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/helpers/checa_testes.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-01-22 19:11:09.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/rola_tesouro.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5270 2024-02-28 11:57:10.000000 ttrpgaag-3.0.3/RPG/sistemas/dnd/teste.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.226374 ttrpgaag-3.0.3/RPG/sistemas/pf2/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/PC.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6182 2023-11-27 11:50:56.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/calcula_dano.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.229954 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/defesas_monstros.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/proficiency.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/saves.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/skills.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/tipos_ataques.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/data/tipos_defesas.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.232158 ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2023-11-27 11:50:56.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/base_calcula_dano.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      856 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/proficiencias.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-3.0.3/RPG/sistemas/pf2/proficiencia.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.233206 ttrpgaag-3.0.3/RPG/sistemas/rolemaster/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-3.0.3/RPG/sistemas/rolemaster/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1316 2024-04-23 18:43:15.000000 ttrpgaag-3.0.3/RPG/sistemas/rolemaster/consulta_critico.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.234564 ttrpgaag-3.0.3/RPG/sistemas/rolemaster/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.3/RPG/sistemas/rolemaster/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-3.0.3/RPG/sistemas/rolemaster/data/criticos.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.236476 ttrpgaag-3.0.3/RPG/tabela_rolavel/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2024-04-23 17:09:37.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.239586 ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 17:28:48.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-05-06 18:06:00.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/ajeita_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      724 2024-04-24 12:42:59.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/ajusta_resultados.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/rolamento_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-05-06 17:41:54.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/rolar_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     4613 2024-05-06 18:07:06.000000 ttrpgaag-3.0.3/RPG/tabela_rolavel/tabela_rolavel.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.242799 ttrpgaag-3.0.3/TTRPGaag.egg-info/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1413 2024-05-06 18:13:17.000000 ttrpgaag-3.0.3/TTRPGaag.egg-info/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-05-06 18:13:17.000000 ttrpgaag-3.0.3/TTRPGaag.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-05-06 18:13:17.000000 ttrpgaag-3.0.3/TTRPGaag.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-05-06 18:13:17.000000 ttrpgaag-3.0.3/TTRPGaag.egg-info/top_level.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-05-06 18:13:17.244250 ttrpgaag-3.0.3/setup.cfg
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-05-06 18:07:19.000000 ttrpgaag-3.0.3/setup.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-05-06 18:13:17.242258 ttrpgaag-3.0.3/tests/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-3.0.3/tests/__init__.py
```

### Comparing `ttrpgaag-3.0.2/LICENSE` & `ttrpgaag-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/PKG-INFO` & `ttrpgaag-3.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 3.0.2
+Version: 3.0.3
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
-- **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random.
+- **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia` 
   - Lista de skills em Data
   - Classe de PC para representar um personagem
 - **2.2.3** - Inclusão dos danos só de rolamento no PF2
 - **2.2.2** - Inclusão de valor do ataque do ataque atual como propriedade em PF2
```

### Comparing `ttrpgaag-3.0.2/README.md` & `ttrpgaag-3.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
-- **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random.
+- **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia` 
   - Lista de skills em Data
   - Classe de PC para representar um personagem
 - **2.2.3** - Inclusão dos danos só de rolamento no PF2
 - **2.2.2** - Inclusão de valor do ataque do ataque atual como propriedade em PF2
```

### Comparing `ttrpgaag-3.0.2/RPG/baralho.py` & `ttrpgaag-3.0.3/RPG/baralho.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/dado/dado.py` & `ttrpgaag-3.0.3/RPG/dado/dado.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/dado/dados.py` & `ttrpgaag-3.0.3/RPG/dado/dados.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/dado/helpers/converter_notacao_dado.py` & `ttrpgaag-3.0.3/RPG/dado/helpers/converter_notacao_dado.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/dado/rolar_dado_notacao.py` & `ttrpgaag-3.0.3/RPG/dado/rolar_dado_notacao.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/iniciativa.py` & `ttrpgaag-3.0.3/RPG/iniciativa.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/dnd/data/tesouro.py` & `ttrpgaag-3.0.3/RPG/sistemas/dnd/data/tesouro.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/dnd/rola_tesouro.py` & `ttrpgaag-3.0.3/RPG/sistemas/dnd/rola_tesouro.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/dnd/teste.py` & `ttrpgaag-3.0.3/RPG/sistemas/dnd/teste.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/pf2/PC.py` & `ttrpgaag-3.0.3/RPG/sistemas/pf2/PC.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/pf2/calcula_dano.py` & `ttrpgaag-3.0.3/RPG/sistemas/pf2/calcula_dano.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/pf2/data/defesas_monstros.py` & `ttrpgaag-3.0.3/RPG/sistemas/pf2/data/defesas_monstros.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/base_calcula_dano.py` & `ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/base_calcula_dano.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/proficiencias.py` & `ttrpgaag-3.0.3/RPG/sistemas/pf2/helpers/proficiencias.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/pf2/proficiencia.py` & `ttrpgaag-3.0.3/RPG/sistemas/pf2/proficiencia.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/rolemaster/consulta_critico.py` & `ttrpgaag-3.0.3/RPG/sistemas/rolemaster/consulta_critico.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/criticos.py` & `ttrpgaag-3.0.3/RPG/sistemas/rolemaster/data/criticos.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajeita_tabela.py` & `ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/ajeita_tabela.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajusta_resultados.py` & `ttrpgaag-3.0.3/RPG/tabela_rolavel/helpers/ajusta_resultados.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/tabela_rolavel/rolar_tabela.py` & `ttrpgaag-3.0.3/RPG/tabela_rolavel/rolar_tabela.py`

 * *Files identical despite different names*

### Comparing `ttrpgaag-3.0.2/RPG/tabela_rolavel/tabela_rolavel.py` & `ttrpgaag-3.0.3/RPG/tabela_rolavel/tabela_rolavel.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,8 +82,12 @@
 
     @property
     def rolamento(self):
         return self._dado_rolado
 
     @property
     def resultado(self):
+        if type(self._resultado) is TabelaRolavel:
+            self._resultado.rolar()
+            return self._resultado.resultado
+
         return self._resultado
```

### Comparing `ttrpgaag-3.0.2/TTRPGaag.egg-info/PKG-INFO` & `ttrpgaag-3.0.3/TTRPGaag.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 3.0.2
+Version: 3.0.3
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **3.0.3** - `TabelaRolavel` agora aceita e rola o resultado de outra tabela caso esse seja o resultado. Por exemplo: a tabela de tesouro pode fazer rolar na tabela de armas mágicas. Se cair esse resultado, já vai entregar o devido resultado
 - **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
-- **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random.
+- **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia` 
   - Lista de skills em Data
   - Classe de PC para representar um personagem
 - **2.2.3** - Inclusão dos danos só de rolamento no PF2
 - **2.2.2** - Inclusão de valor do ataque do ataque atual como propriedade em PF2
```

### Comparing `ttrpgaag-3.0.2/TTRPGaag.egg-info/SOURCES.txt` & `ttrpgaag-3.0.3/TTRPGaag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

