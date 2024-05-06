# Comparing `tmp/sinergym-3.3.1.tar.gz` & `tmp/sinergym-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-3.3.1.tar", last modified: Mon Apr 22 13:59:56 2024, max compression
+gzip compressed data, was "sinergym-3.3.3.tar", last modified: Mon May  6 14:41:26 2024, max compression
```

## Comparing `sinergym-3.3.1.tar` & `sinergym-3.3.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.274805 sinergym-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-22 13:59:51.000000 sinergym-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 13:59:51.000000 sinergym-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-22 13:59:56.274805 sinergym-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-22 13:59:51.000000 sinergym-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 13:59:55.000000 sinergym-3.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 13:59:56.274805 sinergym-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-22 13:59:55.000000 sinergym-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.234806 sinergym-3.3.1/sinergym/
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.234806 sinergym-3.3.1/sinergym/config/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/config/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.234806 sinergym-3.3.1/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.238806 sinergym-3.3.1/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   151242 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   145181 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   595437 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   272977 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   512302 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   245040 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/ShopWithPVandBattery.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   389111 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/buildings/radiant_residential_building.epJSON
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.242806 sinergym-3.3.1/sinergym/data/default_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/5ZoneAutoDXVAV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/ShopWithPVandBattery.json
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/default_configuration/radiant_residential_building.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.270805 sinergym-3.3.1/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1565086 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1550279 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1621761 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1553382 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1558629 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1558423 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1601571 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1550263 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29016 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1637298 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29489 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1629153 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1639985 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1613784 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1624547 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1625209 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.274805 sinergym-3.3.1/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.274805 sinergym-3.3.1/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/simulators/eplus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.274805 sinergym-3.3.1/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)    38613 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 13:59:55.000000 sinergym-3.3.1/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:59:56.234806 sinergym-3.3.1/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-22 13:59:56.000000 sinergym-3.3.1/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-22 13:59:56.000000 sinergym-3.3.1/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:59:56.000000 sinergym-3.3.1/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-22 13:59:56.000000 sinergym-3.3.1/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 13:59:56.000000 sinergym-3.3.1/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.946107 sinergym-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-06 14:41:22.000000 sinergym-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 14:41:22.000000 sinergym-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-06 14:41:26.946107 sinergym-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-06 14:41:22.000000 sinergym-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 14:41:26.000000 sinergym-3.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-06 14:41:26.946107 sinergym-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-06 14:41:26.000000 sinergym-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.906108 sinergym-3.3.3/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.906108 sinergym-3.3.3/sinergym/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/config/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.906108 sinergym-3.3.3/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.910108 sinergym-3.3.3/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   151242 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   145181 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   595437 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   272977 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   512302 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   245040 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/ShopWithPVandBattery.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   389111 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/buildings/radiant_residential_building.epJSON
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.914108 sinergym-3.3.3/sinergym/data/default_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/5ZoneAutoDXVAV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/ShopWithPVandBattery.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/default_configuration/radiant_residential_building.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.942107 sinergym-3.3.3/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1565086 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1550279 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1621761 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1553382 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1558629 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1558423 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1601571 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1550263 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29016 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1637298 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29489 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1629153 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1639985 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1613784 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1624547 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1625209 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.946107 sinergym-3.3.3/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.946107 sinergym-3.3.3/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/simulators/eplus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.946107 sinergym-3.3.3/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44280 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:41:26.906108 sinergym-3.3.3/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 14:41:26.000000 sinergym-3.3.3/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-3.3.1/LICENSE` & `sinergym-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/PKG-INFO` & `sinergym-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 3.3.1
+Version: 3.3.3
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 3.3.1 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 3.3.3 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-3.3.1/README.md` & `sinergym-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/setup.py` & `sinergym-3.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/__init__.py` & `sinergym-3.3.3/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/config/modeling.py` & `sinergym-3.3.3/sinergym/config/modeling.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/ShopWithPVandBattery.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/ShopWithPVandBattery.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/buildings/radiant_residential_building.epJSON` & `sinergym-3.3.3/sinergym/data/buildings/radiant_residential_building.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json` & `sinergym-3.3.3/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json` & `sinergym-3.3.3/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/5ZoneAutoDXVAV.json` & `sinergym-3.3.3/sinergym/data/default_configuration/5ZoneAutoDXVAV.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json` & `sinergym-3.3.3/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json` & `sinergym-3.3.3/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json` & `sinergym-3.3.3/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/ShopWithPVandBattery.json` & `sinergym-3.3.3/sinergym/data/default_configuration/ShopWithPVandBattery.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/default_configuration/radiant_residential_building.json` & `sinergym-3.3.3/sinergym/data/default_configuration/radiant_residential_building.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-3.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-3.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy` & `sinergym-3.3.3/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw` & `sinergym-3.3.3/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-3.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-3.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-3.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-3.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-3.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-3.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-3.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-3.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-3.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-3.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-3.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-3.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/envs/eplus_env.py` & `sinergym-3.3.3/sinergym/envs/eplus_env.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/simulators/eplus.py` & `sinergym-3.3.3/sinergym/simulators/eplus.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/callbacks.py` & `sinergym-3.3.3/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/common.py` & `sinergym-3.3.3/sinergym/utils/common.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/constants.py` & `sinergym-3.3.3/sinergym/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/controllers.py` & `sinergym-3.3.3/sinergym/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/env_checker.py` & `sinergym-3.3.3/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/evaluation.py` & `sinergym-3.3.3/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/gcloud.py` & `sinergym-3.3.3/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/logger.py` & `sinergym-3.3.3/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/rewards.py` & `sinergym-3.3.3/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym/utils/wrappers.py` & `sinergym-3.3.3/sinergym/utils/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,33 +61,39 @@
     logger = Logger().getLogger(name='WRAPPER NormalizeObservation',
                                 level=LOG_WRAPPERS_LEVEL)
 
     def __init__(self,
                  env: EplusEnv,
                  automatic_update: bool = True,
                  epsilon: float = 1e-8,
-                 mean: np.float64 = None,
-                 var: np.float64 = None):
+                 mean: Union[list, np.float64] = None,
+                 var: Union[list, np.float64] = None):
         """Initializes the NormalizationWrapper. Mean and var values can be None andbeing updated during interaction with environment.
 
         Args:
             env (EplusEnv): The environment to apply the wrapper.
             automatic_update (bool, optional): Whether or not to update the mean and variance values automatically. Defaults to True.
             epsilon (float, optional): A stability parameter used when scaling the observations. Defaults to 1e-8.
             mean (np.float64, optional): The mean value used for normalization. Defaults to None.
             var (np.float64, optional): The variance value used for normalization. Defaults to None.
         """
+        # Check mean and var format if it is defined
+        mean = np.float64(mean) if mean is not None else None
+        var = np.float64(var) if var is not None else None
+        # Save normalization configuration for whole python process
         gym.utils.RecordConstructorArgs.__init__(
             self, epsilon=epsilon, mean=mean, var=var)
         gym.Wrapper.__init__(self, env)
+
         self.num_envs = 1
         self.is_vector_env = False
         self.automatic_update = automatic_update
 
         self.unwrapped_observation = None
+        # Initialize normalization calibration
         self.obs_rms = RunningMeanStd(shape=self.observation_space.shape)
         self.obs_rms.mean = mean if mean is not None else self.obs_rms.mean
         self.obs_rms.var = var if var is not None else self.obs_rms.var
         self.epsilon = epsilon
 
         self.logger.info('Wrapper initialized.')
 
@@ -105,16 +111,40 @@
     def reset(self, **kwargs):
         """Resets the environment and normalizes the observation."""
         obs, info = self.env.reset(**kwargs)
 
         # Save original obs in class attribute
         self.unwrapped_observation = deepcopy(obs)
 
+        # Update normalization calibration if it is required
+        self._save_normalization_calibration()
+
         return self.normalize(np.array([obs]))[0], info
 
+    def close(self):
+        """Close the environment and save normalization calibration."""
+        self.env.close()
+        # Update normalization calibration if it is required
+        self._save_normalization_calibration()
+
+    # ----------------------- Wrappers extra functionality ----------------------- #
+
+    def _save_normalization_calibration(self):
+        """Saves the normalization calibration data in the output folder as txt files.
+        """
+        if hasattr(self, "mean") and hasattr(self, "var"):
+            self.logger.info(
+                'Saving normalization calibration data... [{}]'.format(
+                    self.name))
+            # Save in txt in output folder
+            np.savetxt(fname=self.get_wrapper_attr(
+                'workspace_path') + '/mean.txt', X=self.mean)
+            np.savetxt(fname=self.get_wrapper_attr(
+                'workspace_path') + '/var.txt', X=self.var)
+
     def deactivate_update(self):
         """
         Deactivates the automatic update of the normalization wrapper.
         After calling this method, the normalization wrapper will not update its calibration automatically.
         """
         self.automatic_update = False
 
@@ -122,22 +152,28 @@
         """
         Activates the automatic update of the normalization wrapper.
         After calling this method, the normalization wrapper will update its calibration automatically.
         """
         self.automatic_update = True
 
     @property
-    def mean(self):
+    def mean(self) -> Optional[np.float64]:
         """Returns the mean value of the observations."""
-        return self.obs_rms.mean
+        if hasattr(self, 'obs_rms'):
+            return self.obs_rms.mean
+        else:
+            return None
 
     @property
-    def var(self):
+    def var(self) -> Optional[np.float64]:
         """Returns the variance value of the observations."""
-        return self.obs_rms.var
+        if hasattr(self, 'obs_rms'):
+            return self.obs_rms.mean
+        else:
+            return None
 
     def set_mean(self, mean: np.float64):
         """Sets the mean value of the observations."""
         try:
             assert len(mean) == self.observation_space.shape[0]
         except AssertionError as err:
             self.logger.error(
@@ -919,14 +955,105 @@
         return action_
 
     def action(self, action: Any):
         action_ = deepcopy(action)
         action_ = self.get_wrapper_attr('reverting_action')(action_)
         return action_
 
+
+class ReduceObservationWrapper(gym.Wrapper):
+
+    logger = Logger().getLogger(name='WRAPPER ReduceObservationWrapper',
+                                level=LOG_WRAPPERS_LEVEL)
+
+    def __init__(self,
+                 env: EplusEnv,
+                 obs_reduction: List[str]):
+        """Wrapper to reduce the observation space of the environment. These variables removed from
+        the space are included in the info dictionary. This way they are recordable but not used in DRL process.
+
+        Args:
+            env (EplusEnv): Original environment.
+            obs_reduction (List[str]): List of observation variables to be removed.
+        """
+        super().__init__(env)
+
+        # Check if the variables to be removed are in the observation space
+        try:
+            assert all(
+                var in self.get_wrapper_attr('observation_variables')
+                for var in obs_reduction)
+        except AssertionError as err:
+            self.logger.error(
+                'Some observation variable to be removed is not defined in the original observation space.')
+            raise err
+
+        # Update observation space
+        self.observation_space = gym.spaces.Box(
+            low=-5e6,
+            high=5e6,
+            shape=(
+                self.env.observation_space.shape[0] -
+                len(obs_reduction),
+            ),
+            dtype=np.float32)
+
+        # Separate removed variables from observation variables
+        self.observation_variables = list(
+            filter(
+                lambda x: x not in obs_reduction, deepcopy(
+                    self.get_wrapper_attr('observation_variables'))))
+        self.removed_observation_variables = obs_reduction
+
+        self.logger.info('Wrapper initialized.')
+
+    def step(self, action: Union[int, np.ndarray]
+             ) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Any]]:
+        """Sends action to the environment. Separating removed variables from observation values and adding it to info dict.
+
+        Args:
+            action (Union[int, float, np.integer, np.ndarray, List[Any], Tuple[Any]]): Action selected by the agent.
+
+        Returns:
+            Tuple[np.ndarray, float, bool, Dict[str, Any]]: Observation for next timestep, reward obtained, Whether the episode has ended or not, Whether episode has been truncated or not, and a dictionary with extra information
+        """
+        obs, reward, terminated, truncated, info = self.env.step(action)
+
+        # Processig obs to delete removed variables and add them to info
+        obs_dict = dict(
+            zip(self.env.get_wrapper_attr('observation_variables'), obs))
+        reduced_obs_dict = {
+            key: obs_dict[key] for key in self.get_wrapper_attr('observation_variables')}
+        removed_obs_dict = {key: obs_dict[key] for key in self.get_wrapper_attr(
+            'removed_observation_variables')}
+        info['removed_observation'] = removed_obs_dict
+
+        return np.array(list(reduced_obs_dict.values())
+                        ), reward, terminated, truncated, info
+
+    def reset(self,
+              seed: Optional[int] = None,
+              options: Optional[Dict[str,
+                                     Any]] = None) -> Tuple[np.ndarray,
+                                                            Dict[str,
+                                                                 Any]]:
+        """Sends action to the environment. Separating removed variables from observation values and adding it to info dict"""
+        obs, info = self.env.reset(seed=seed, options=options)
+
+        # Processig obs to delete removed variables and add them to info
+        obs_dict = dict(
+            zip(self.env.get_wrapper_attr('observation_variables'), obs))
+        reduced_obs_dict = {
+            key: obs_dict[key] for key in self.get_wrapper_attr('observation_variables')}
+        removed_obs_dict = {key: obs_dict[key] for key in self.get_wrapper_attr(
+            'removed_observation_variables')}
+        info['removed_observation'] = removed_obs_dict
+
+        return np.array(list(reduced_obs_dict.values())), info
+
     # ---------------------- Specific environment wrappers ---------------------#
 
 
 class OfficeGridStorageSmoothingActionConstraintsWrapper(
         gym.ActionWrapper):  # pragma: no cover
     def __init__(self, env):
         assert env.building_path.split(
```

### Comparing `sinergym-3.3.1/sinergym.egg-info/PKG-INFO` & `sinergym-3.3.3/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 3.3.1
+Version: 3.3.3
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 3.3.1 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 3.3.3 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-3.3.1/sinergym.egg-info/SOURCES.txt` & `sinergym-3.3.3/sinergym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinergym-3.3.1/sinergym.egg-info/requires.txt` & `sinergym-3.3.3/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*

