# Comparing `tmp/deltares-coastalhazardstoolkit-0.2.6.tar.gz` & `tmp/deltares_coastalhazardstoolkit-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltares-coastalhazardstoolkit-0.2.6.tar", last modified: Mon Jan 29 19:00:37 2024, max compression
+gzip compressed data, was "deltares_coastalhazardstoolkit-0.2.7.tar", last modified: Mon May  6 14:52:42 2024, max compression
```

## Comparing `deltares-coastalhazardstoolkit-0.2.6.tar` & `deltares_coastalhazardstoolkit-0.2.7.tar`

### file list

```diff
@@ -1,140 +1,142 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.876490 deltares-coastalhazardstoolkit-0.2.6/
--rw-rw-rw-   0        0        0    35823 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      923 2024-01-29 19:00:37.876490 deltares-coastalhazardstoolkit-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      948 2024-01-29 19:00:13.000000 deltares-coastalhazardstoolkit-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-29 19:00:37.876490 deltares-coastalhazardstoolkit-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.811867 deltares-coastalhazardstoolkit-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.813493 deltares-coastalhazardstoolkit-0.2.6/src/cht/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.815515 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/__init__.py
--rw-rw-rw-   0        0        0    26943 2024-01-25 22:27:26.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/bathymetry_database.py
--rw-rw-rw-   0        0        0    26344 2023-01-03 18:41:58.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/tiling.py
--rw-rw-rw-   0        0        0      803 2022-11-09 17:01:21.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/tiling_example.py
--rw-rw-rw-   0        0        0     1324 2023-01-03 19:45:23.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/tiling_example_gebco22.py
--rw-rw-rw-   0        0        0     2482 2023-10-17 19:03:39.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.815515 deltares-coastalhazardstoolkit-0.2.6/src/cht/beware/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/beware/__init__.py
--rw-rw-rw-   0        0        0    32220 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/beware/beware.py
--rw-rw-rw-   0        0        0    38019 2023-10-17 18:25:21.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/beware/beware_mvo2.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.815515 deltares-coastalhazardstoolkit-0.2.6/src/cht/delft3dfm/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/delft3dfm/__init__.py
--rw-rw-rw-   0        0        0    48600 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/delft3dfm/delft3dfm.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.815515 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-02-16 02:20:58.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/bathymetry.py
--rw-rw-rw-   0        0        0    17344 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/boundary_conditions.py
--rw-rw-rw-   0        0        0    18023 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/grid.py
--rw-rw-rw-   0        0        0    31836 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/hurrywave.py
--rw-rw-rw-   0        0        0     5013 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/hurrywave_builder.py
--rw-rw-rw-   0        0        0     6804 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/hurrywave_domain.py
--rw-rw-rw-   0        0        0     5288 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/input.py
--rw-rw-rw-   0        0        0     5454 2023-02-16 02:34:58.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/mask.py
--rw-rw-rw-   0        0        0     7393 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/observation_points.py
--rw-rw-rw-   0        0        0     4004 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/to_xugrid.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.834205 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/__init__.py
--rw-rw-rw-   0        0        0    11578 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_analysis.py
--rw-rw-rw-   0        0        0    26461 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_tc_forecast.py
--rw-rw-rw-   0        0        0    23025 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_tc_hindcast.py
--rw-rw-rw-   0        0        0     4688 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_tc_ufl_d01.py
--rw-rw-rw-   0        0        0    12331 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50.py
--rw-rw-rw-   0        0        0     9220 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50_02.py
--rw-rw-rw-   0        0        0    14130 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50_03.py
--rw-rw-rw-   0        0        0    15644 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50_04.py
--rw-rw-rw-   0        0        0     6399 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_forecast_0p25.py
--rw-rw-rw-   0        0        0     4146 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_forecast_0p25_02.py
--rw-rw-rw-   0        0        0    66883 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/meteo.py
--rw-rw-rw-   0        0        0    67045 2023-10-11 19:20:57.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/meteo3.py
--rw-rw-rw-   0        0        0     2074 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/test_coamps.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.834205 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/__init__.py
--rw-rw-rw-   0        0        0      886 2023-10-11 19:20:57.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/argo.py
--rw-rw-rw-   0        0        0     9328 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/deltares_ini.py
--rw-rw-rw-   0        0        0     3494 2023-10-11 19:20:57.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/fileops.py
--rw-rw-rw-   0        0        0     4434 2023-02-16 02:05:36.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/geometry.py
--rw-rw-rw-   0        0        0     3024 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/misc_tools.py
--rw-rw-rw-   0        0        0     4440 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/pli_file.py
--rw-rw-rw-   0        0        0     7462 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/prob_maps.py
--rw-rw-rw-   0        0        0     6472 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/sftp.py
--rw-rw-rw-   0        0        0     9845 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/tekal.py
--rw-rw-rw-   0        0        0     5317 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/xmlkit.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.834205 deltares-coastalhazardstoolkit-0.2.6/src/cht/model_builder/
--rw-rw-rw-   0        0        0    22934 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/model_builder/model_builder.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.834205 deltares-coastalhazardstoolkit-0.2.6/src/cht/nesting/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/nesting/__init__.py
--rw-rw-rw-   0        0        0     7599 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/nesting/nest1.py
--rw-rw-rw-   0        0        0    36648 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/nesting/nest2.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.845217 deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/
--rw-rw-rw-   0        0        0       92 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/__init__.py
--rw-rw-rw-   0        0        0      993 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/_ndbc.py
--rw-rw-rw-   0        0        0     1127 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/_noaa_coops.py
--rw-rw-rw-   0        0        0     1181 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/observation_stations.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.845217 deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/__init__.py
--rw-rw-rw-   0        0        0      590 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/deshoal.py
--rw-rw-rw-   0        0        0     1238 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/disper.py
--rw-rw-rw-   0        0        0     7860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/vo21.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.845217 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/__init__.py
--rw-rw-rw-   0        0        0    66271 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/quadtree.py
--rw-rw-rw-   0        0        0    11167 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/regulargrid.py
--rw-rw-rw-   0        0        0    46805 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/sfincs.py
--rw-rw-rw-   0        0        0    12920 2023-07-18 19:58:54.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/sfincs_builder.py
--rw-rw-rw-   0        0        0    48185 2023-01-05 19:25:34.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/subgrid.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/
--rw-rw-rw-   0        0        0       92 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/__init__.py
--rw-rw-rw-   0        0        0    12996 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/boundary_conditions.py
--rw-rw-rw-   0        0        0     3383 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/cross_sections.py
--rw-rw-rw-   0        0        0    49965 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/grid.py
--rw-rw-rw-   0        0        0     8806 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/input.py
--rw-rw-rw-   0        0        0    24343 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/mask.py
--rw-rw-rw-   0        0        0     3350 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/observation_points.py
--rw-rw-rw-   0        0        0     3390 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/point_sources.py
--rw-rw-rw-   0        0        0    80407 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/quadtree_grid.py
--rw-rw-rw-   0        0        0    25050 2023-10-17 18:25:21.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/quadtree_grid_snapwave.py
--rw-rw-rw-   0        0        0    18022 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/regular_grid.py
--rw-rw-rw-   0        0        0    47347 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/sfincs.py
--rw-rw-rw-   0        0        0    11719 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/sfincs_builder.py
--rw-rw-rw-   0        0        0    20663 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/snapwave.py
--rw-rw-rw-   0        0        0    50740 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/subgrid.py
--rw-rw-rw-   0        0        0     3093 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/thin_dams.py
--rw-rw-rw-   0        0        0     1707 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/wave_makers.py
--rw-rw-rw-   0        0        0     3122 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/weirs.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/snapwave/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/snapwave/__init__.py
--rw-rw-rw-   0        0        0    24908 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/snapwave/mesh.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/__init__.py
--rw-rw-rw-   0        0        0     7255 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/astro.py
--rw-rw-rw-   0        0        0     7524 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/constituent.py
--rw-rw-rw-   0        0        0     3542 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/fes2014.py
--rw-rw-rw-   0        0        0     4860 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/nodal_corrections.py
--rw-rw-rw-   0        0        0     1479 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/predict.py
--rw-rw-rw-   0        0        0      687 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/test_tide_database.py
--rw-rw-rw-   0        0        0    15388 2023-03-02 18:25:09.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/tide.py
--rw-rw-rw-   0        0        0     3365 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/tide_model.py
--rw-rw-rw-   0        0        0      965 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/tide_predict.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/tiling/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tiling/__init__.py
--rw-rw-rw-   0        0        0    33383 2023-10-11 19:20:57.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tiling/tiling.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/
--rw-rw-rw-   0        0        0    10203 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/cyclone_track_database.py
--rw-rw-rw-   0        0        0     1091 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_forecasting.py
--rw-rw-rw-   0        0        0     2406 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_meteo.py
--rw-rw-rw-   0        0        0      480 2023-05-04 16:45:00.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_track.py
--rw-rw-rw-   0        0        0     1517 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_track_reading.py
--rw-rw-rw-   0        0        0   122351 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/tropical_cyclone.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/watersheds/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/watersheds/__init__.py
--rw-rw-rw-   0        0        0     7923 2024-01-12 16:09:15.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/watersheds/watersheds.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.860864 deltares-coastalhazardstoolkit-0.2.6/src/cht/xbeach/
--rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/xbeach/__init__.py
--rw-rw-rw-   0        0        0    28069 2024-01-18 19:18:13.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/xbeach/xbeach.py
--rw-rw-rw-   0        0        0    22525 2023-11-22 16:14:10.000000 deltares-coastalhazardstoolkit-0.2.6/src/cht/xbeach/xbeach_output_morphology.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:00:37.876490 deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/
--rw-rw-rw-   0        0        0      923 2024-01-29 19:00:37.000000 deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3677 2024-01-29 19:00:37.000000 deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 19:00:37.000000 deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-01-29 19:00:37.000000 deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-29 19:00:37.000000 deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.637022 deltares_coastalhazardstoolkit-0.2.7/
+-rw-rw-rw-   0        0        0    35823 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      923 2024-05-06 14:52:42.636023 deltares_coastalhazardstoolkit-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2024-05-06 14:51:26.000000 deltares_coastalhazardstoolkit-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 14:52:42.637022 deltares_coastalhazardstoolkit-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.541792 deltares_coastalhazardstoolkit-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.543816 deltares_coastalhazardstoolkit-0.2.7/src/cht/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.549811 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/__init__.py
+-rw-rw-rw-   0        0        0    26972 2024-02-11 17:24:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/bathymetry_database.py
+-rw-rw-rw-   0        0        0    26344 2023-01-03 18:41:58.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/tiling.py
+-rw-rw-rw-   0        0        0      803 2022-11-09 17:01:21.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/tiling_example.py
+-rw-rw-rw-   0        0        0     1324 2023-01-03 19:45:23.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/tiling_example_gebco22.py
+-rw-rw-rw-   0        0        0     2482 2023-10-17 19:03:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.551128 deltares_coastalhazardstoolkit-0.2.7/src/cht/beware/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/beware/__init__.py
+-rw-rw-rw-   0        0        0    31959 2024-02-12 15:47:29.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/beware/beware.py
+-rw-rw-rw-   0        0        0    38019 2023-10-17 18:25:21.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/beware/beware_mvo2.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.552136 deltares_coastalhazardstoolkit-0.2.7/src/cht/delft3dfm/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/delft3dfm/__init__.py
+-rw-rw-rw-   0        0        0    48600 2024-01-31 16:42:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/delft3dfm/delft3dfm.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.560145 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-02-16 02:20:58.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/bathymetry.py
+-rw-rw-rw-   0        0        0    17344 2024-01-31 16:42:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/boundary_conditions.py
+-rw-rw-rw-   0        0        0    18320 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/grid.py
+-rw-rw-rw-   0        0        0    31835 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/hurrywave.py
+-rw-rw-rw-   0        0        0     5299 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/hurrywave_builder.py
+-rw-rw-rw-   0        0        0     6804 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/hurrywave_domain.py
+-rw-rw-rw-   0        0        0     5288 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/input.py
+-rw-rw-rw-   0        0        0     5454 2023-02-16 02:34:58.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/mask.py
+-rw-rw-rw-   0        0        0     7393 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/observation_points.py
+-rw-rw-rw-   0        0        0     4004 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/to_xugrid.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.569664 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/__init__.py
+-rw-rw-rw-   0        0        0    11578 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_analysis.py
+-rw-rw-rw-   0        0        0    26470 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_tc_forecast.py
+-rw-rw-rw-   0        0        0    23025 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_tc_hindcast.py
+-rw-rw-rw-   0        0        0     4688 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_tc_ufl_d01.py
+-rw-rw-rw-   0        0        0    12331 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50.py
+-rw-rw-rw-   0        0        0     9220 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50_02.py
+-rw-rw-rw-   0        0        0    14130 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50_03.py
+-rw-rw-rw-   0        0        0    15644 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50_04.py
+-rw-rw-rw-   0        0        0     6399 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_forecast_0p25.py
+-rw-rw-rw-   0        0        0     4146 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_forecast_0p25_02.py
+-rw-rw-rw-   0        0        0    66624 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/meteo.py
+-rw-rw-rw-   0        0        0    67045 2023-10-11 19:20:57.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/meteo3.py
+-rw-rw-rw-   0        0        0     2074 2023-07-18 19:58:54.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/test_coamps.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.577183 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-10-11 19:20:57.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/argo.py
+-rw-rw-rw-   0        0        0     9328 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/deltares_ini.py
+-rw-rw-rw-   0        0        0     3617 2024-02-12 15:47:29.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/fileops.py
+-rw-rw-rw-   0        0        0     4434 2023-02-16 02:05:36.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/geometry.py
+-rw-rw-rw-   0        0        0     3024 2024-01-31 16:42:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/misc_tools.py
+-rw-rw-rw-   0        0        0     4746 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/pli_file.py
+-rw-rw-rw-   0        0        0     8042 2024-02-12 15:47:29.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/prob_maps.py
+-rw-rw-rw-   0        0        0     6472 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/sftp.py
+-rw-rw-rw-   0        0        0     9845 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/tekal.py
+-rw-rw-rw-   0        0        0     5317 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/xmlkit.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.577183 deltares_coastalhazardstoolkit-0.2.7/src/cht/model_builder/
+-rw-rw-rw-   0        0        0    22155 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/model_builder/model_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.579901 deltares_coastalhazardstoolkit-0.2.7/src/cht/nesting/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/nesting/__init__.py
+-rw-rw-rw-   0        0        0     7599 2024-01-31 16:42:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/nesting/nest1.py
+-rw-rw-rw-   0        0        0    36671 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/nesting/nest2.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.582785 deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/
+-rw-rw-rw-   0        0        0       92 2023-03-02 18:25:09.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/__init__.py
+-rw-rw-rw-   0        0        0      993 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/_ndbc.py
+-rw-rw-rw-   0        0        0     1127 2023-03-02 18:25:09.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/_noaa_coops.py
+-rw-rw-rw-   0        0        0     1181 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/observation_stations.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.585021 deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/__init__.py
+-rw-rw-rw-   0        0        0      590 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/deshoal.py
+-rw-rw-rw-   0        0        0     1238 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/disper.py
+-rw-rw-rw-   0        0        0     7860 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/vo21.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.589355 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/__init__.py
+-rw-rw-rw-   0        0        0    66271 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/quadtree.py
+-rw-rw-rw-   0        0        0    11167 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/regulargrid.py
+-rw-rw-rw-   0        0        0    46521 2024-02-12 15:47:29.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/sfincs.py
+-rw-rw-rw-   0        0        0    12920 2023-07-18 19:58:54.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/sfincs_builder.py
+-rw-rw-rw-   0        0        0    48185 2023-01-05 19:25:34.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/subgrid.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.603898 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/
+-rw-rw-rw-   0        0        0       92 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/__init__.py
+-rw-rw-rw-   0        0        0    12978 2024-02-12 15:54:08.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/boundary_conditions.py
+-rw-rw-rw-   0        0        0     3383 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/cross_sections.py
+-rw-rw-rw-   0        0        0    49965 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/grid.py
+-rw-rw-rw-   0        0        0    46673 2024-03-28 17:39:17.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/grid_v2.py
+-rw-rw-rw-   0        0        0     8826 2024-02-12 15:39:36.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/input.py
+-rw-rw-rw-   0        0        0    24459 2024-02-10 18:57:03.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/mask.py
+-rw-rw-rw-   0        0        0     3350 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/observation_points.py
+-rw-rw-rw-   0        0        0     3390 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/point_sources.py
+-rw-rw-rw-   0        0        0    80407 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/quadtree_grid.py
+-rw-rw-rw-   0        0        0    25050 2023-10-17 18:25:21.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/quadtree_grid_snapwave.py
+-rw-rw-rw-   0        0        0    18022 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/regular_grid.py
+-rw-rw-rw-   0        0        0    47492 2024-02-12 15:20:28.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/sfincs.py
+-rw-rw-rw-   0        0        0    11719 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/sfincs_builder.py
+-rw-rw-rw-   0        0        0    20663 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/snapwave.py
+-rw-rw-rw-   0        0        0    51195 2024-05-06 14:30:16.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/subgrid.py
+-rw-rw-rw-   0        0        0     3093 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/thin_dams.py
+-rw-rw-rw-   0        0        0     1707 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/wave_makers.py
+-rw-rw-rw-   0        0        0     3122 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/weirs.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.604899 deltares_coastalhazardstoolkit-0.2.7/src/cht/snapwave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/snapwave/__init__.py
+-rw-rw-rw-   0        0        0    24908 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/snapwave/mesh.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.611403 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/__init__.py
+-rw-rw-rw-   0        0        0     7255 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/astro.py
+-rw-rw-rw-   0        0        0     7524 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/constituent.py
+-rw-rw-rw-   0        0        0     3542 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/fes2014.py
+-rw-rw-rw-   0        0        0     4860 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/nodal_corrections.py
+-rw-rw-rw-   0        0        0     1479 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/predict.py
+-rw-rw-rw-   0        0        0      687 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/test_tide_database.py
+-rw-rw-rw-   0        0        0    15388 2023-03-02 18:25:09.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/tide.py
+-rw-rw-rw-   0        0        0     3365 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/tide_model.py
+-rw-rw-rw-   0        0        0      965 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/tide_predict.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.612412 deltares_coastalhazardstoolkit-0.2.7/src/cht/tiling/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tiling/__init__.py
+-rw-rw-rw-   0        0        0    33383 2023-10-11 19:20:57.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tiling/tiling.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.617410 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/
+-rw-rw-rw-   0        0        0        2 2024-03-28 17:39:17.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/__init__.py
+-rw-rw-rw-   0        0        0    10203 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/cyclone_track_database.py
+-rw-rw-rw-   0        0        0     1091 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_forecasting.py
+-rw-rw-rw-   0        0        0     2406 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_meteo.py
+-rw-rw-rw-   0        0        0      480 2023-05-04 16:45:00.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_track.py
+-rw-rw-rw-   0        0        0     1517 2023-11-22 16:14:10.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_track_reading.py
+-rw-rw-rw-   0        0        0   123399 2024-02-12 15:47:29.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/tropical_cyclone.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.618410 deltares_coastalhazardstoolkit-0.2.7/src/cht/watersheds/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/watersheds/__init__.py
+-rw-rw-rw-   0        0        0     7923 2024-01-12 16:09:15.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/watersheds/watersheds.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.620916 deltares_coastalhazardstoolkit-0.2.7/src/cht/xbeach/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/xbeach/__init__.py
+-rw-rw-rw-   0        0        0    28069 2024-01-31 16:42:39.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/xbeach/xbeach.py
+-rw-rw-rw-   0        0        0    27114 2024-05-06 14:29:38.000000 deltares_coastalhazardstoolkit-0.2.7/src/cht/xbeach/xbeach_output_morphology.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:52:42.636023 deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/
+-rw-rw-rw-   0        0        0      923 2024-05-06 14:52:42.000000 deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3741 2024-05-06 14:52:42.000000 deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:52:42.000000 deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-05-06 14:52:42.000000 deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 14:52:42.000000 deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/top_level.txt
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/LICENSE` & `deltares_coastalhazardstoolkit-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/PKG-INFO` & `deltares_coastalhazardstoolkit-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltares-coastalhazardstoolkit
-Version: 0.2.6
+Version: 0.2.7
 Author-email: Maarten van Ormondt <maarten.vanormondt@deltares-usa.us>, Roel de Goede <roel.degoede@deltares.nl>, Kees Nederhoff <kees.nederhoff@deltares-usa.us>, Tim Leijnse <tim.leijnse@deltares.nl>, Panos Athanasiou <panos.athanasiou@deltares.nl>
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: geopandas>=0.8
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyproj
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/pyproject.toml` & `deltares_coastalhazardstoolkit-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.2.6"
+version = "0.2.7"
 name = "deltares-coastalhazardstoolkit"
 authors = [
     {name = "Maarten van Ormondt", email = "maarten.vanormondt@deltares-usa.us"},
     {name = "Roel de Goede", email = "roel.degoede@deltares.nl"},
     {name = "Kees Nederhoff", email = "kees.nederhoff@deltares-usa.us"},
     {name = "Tim Leijnse", email = "tim.leijnse@deltares.nl"},
     {name = "Panos Athanasiou", email = "panos.athanasiou@deltares.nl"},
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/bathymetry_database.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/bathymetry_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,20 +171,21 @@
                 ymax = np.nanmax(np.nanmax(yzb))
                 ddx = 0.05 * (xmax - xmin)
                 ddy = 0.05 * (ymax - ymin)
                 xl = [xmin - ddx, xmax + ddx]
                 yl = [ymin - ddy, ymax + ddy]
                 # Get DEM data (ddb format for now)
                 xb, yb, zb = self.get_data(dataset.name,
-                                                          xl,
-                                                          yl,
-                                                          max_cell_size=dx)
-                zb[np.where(zb < zmin)] = np.nan
-                zb[np.where(zb > zmax)] = np.nan
+                                           xl,
+                                           yl,
+                                           max_cell_size=dx)
+                # If zb equal np.nan, then there is not data
                 if not np.isnan(zb).all():
+                    zb[np.where(zb < zmin)] = np.nan
+                    zb[np.where(zb > zmax)] = np.nan
                     zz1 = interp2(xb, yb, zb, xzb, yzb, method=method)
                     isn = np.where(np.isnan(zz))
                     zz[isn] = zz1[isn]
 
         return zz
 
     def get_dataset(self, name):
@@ -693,7 +694,9 @@
 def yaml2dict(file_name):
     file = open(file_name,"r")
     dct = yaml.load(file, Loader=yaml.FullLoader)
     return dct
 
 
 bathymetry_database = BathymetryDatabase(None)
+
+
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/tiling.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/tiling.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/tiling_example.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/tiling_example.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/tiling_example_gebco22.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/tiling_example_gebco22.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/bathymetry/utils.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/bathymetry/utils.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/beware/beware.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/beware/beware.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,22 +361,18 @@
         self.write_bhs_file(path=path)
         self.write_btp_file(path=path)
 
     def write_bhs_file(self, file_name=None, path=None):
         # Write BEWARE bhs file
         if not path:
             path=self.path
+        if not file_name and not self.input.bhsfile:
+            return
         if not file_name:
-            if not self.input.bhsfile:
-                return
-            file_name = os.path.join(path,
-                                     self.input.bhsfile)
-            
-        if not file_name:
-            return        
+            file_name = os.path.join(path, self.input.bhsfile)  
         
         point_data = []
         for point in self.wave_boundary_point:
             if point.data is not None:
                 # df = pd.concat([df, point.data['hm0']], axis=1)
                 point_data.append(point.data['hm0'])
         df = pd.concat(point_data, axis=1)
@@ -390,23 +386,19 @@
                   header=False,
                   float_format="%0.3f")
         
     def write_btp_file(self, file_name=None, path=None):
         # Write BEWARE btp file
         if not path:
             path=self.path
+        if not file_name and not self.input.btpfile:
+            return
         if not file_name:
-            if not self.input.btpfile:
-                return
-            file_name = os.path.join(path,
-                                     self.input.btpfile)
+            file_name = os.path.join(path, self.input.btpfile)
             
-        if not file_name:
-            return
-
         point_data = []
         for point in self.wave_boundary_point:
             if point.data is not None:
                 point_data.append(point.data['tp'])
         df = pd.concat(point_data, axis=1)
 
         tmsec = pd.to_timedelta(df.index - self.input.tref, unit="s")
@@ -416,22 +408,18 @@
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
         
     def write_flow_boundary_conditions(self, file_name=None):
 
-        if not file_name:
-            if not self.input.bzsfile:
-                return
-            file_name = os.path.join(self.path,
-                                     self.input.bzsfile)
-            
-        if not file_name:
+        if not file_name and not self.input.bzsfile:
             return
+        if not file_name:
+            file_name = os.path.join(self.path, self.input.bzsfile)
 
         # Build a new DataFrame
         point_data = []
         for point in self.flow_boundary_point:
             point_data.append(point.data)
             # df = pd.concat([df, point.data], axis=1)
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/beware/beware_mvo2.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/beware/beware_mvo2.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/delft3dfm/delft3dfm.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/delft3dfm/delft3dfm.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/bathymetry.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/bathymetry.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/boundary_conditions.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/grid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
             data=data,
             coords=self.coordinates,
             dims=("n", "m"),
             attrs={"_FillValue": dtype(fill_value)},
         )
         return da
 
+    def write(self):
+        # Write out both mask and depth files
+        self.write_msk_file()
+        self.write_dep_file()
+
     def write_dep_file(self):    
         # Write depth file
         if self.model.input.variables.depfile:
             self.write_map("bed_level",
                            os.path.join(self.model.path, self.model.input.variables.depfile),
                            np.float32)
 
@@ -158,62 +163,70 @@
               exclude_zmin=-99999.0,
               exclude_zmax= 99999.0,
               boundary_polygon=None,
               boundary_zmin=-99999.0,
               boundary_zmax= 99999.0,
               quiet=True):
 
+        if include_polygon is None:
+            include_polygon = gpd.GeoDataFrame()
+        if exclude_polygon is None:
+            exclude_polygon = gpd.GeoDataFrame()
+        if boundary_polygon is None:
+            boundary_polygon = gpd.GeoDataFrame()
+
         if not quiet:
             print("Building mask mask ...")
 
         xz = self.ds["x"].values[:]
         yz = self.ds["y"].values[:]
         zz = self.ds["bed_level"].values[:]
         mask = np.zeros((self.nmax, self.mmax), dtype=int)
 
         if zmin<zmax:
             # Set initial mask based on zmin and zmax
             iok = np.where((zz>=zmin) & (zz<=zmax))
             mask[iok] = 1
                         
         # Include polygons
-        if include_polygon is not None:
+#        if include_polygon is not None:           
+        if len(include_polygon) > 0:
             for ip, polygon in include_polygon.iterrows():
                 inpol = inpolygon(xz, yz, polygon["geometry"])
                 iok   = np.where((inpol) & (zz>=include_zmin) & (zz<=include_zmax))
                 mask[iok] = 1
 
         # Exclude polygons
-        if exclude_polygon is not None:
+#        if exclude_polygon is not None:
+        if len(exclude_polygon) > 0:
             for ip, polygon in exclude_polygon.iterrows():
                 inpol = inpolygon(xz, yz, polygon["geometry"])
                 iok   = np.where((inpol) & (zz>=exclude_zmin) & (zz<=exclude_zmax))
                 mask[iok] = 0
 
         # Open boundary polygons
-        if boundary_polygon is not None:
-            if len(boundary_polygon) > 0:
-                    mskbuff = np.zeros((np.shape(mask)[0] + 2, np.shape(mask)[1] + 2), dtype=int)
-                    mskbuff[1:-1, 1:-1] = mask
-                    # Find cells that are next to an inactive cell
-                    msk4 = np.zeros((4, np.shape(mask)[0], np.shape(mask)[1]), dtype=int)
-                    msk4[0, :, :] = mskbuff[0:-2, 1:-1]
-                    msk4[1, :, :] = mskbuff[2:,   1:-1]
-                    msk4[2, :, :] = mskbuff[1:-1, 0:-2]
-                    msk4[3, :, :] = mskbuff[1:-1, 2:  ]
-                    imin = msk4.min(axis=0)
-                    for ip, polygon in boundary_polygon.iterrows():
-                        inpol = inpolygon(xz, yz, polygon["geometry"])
-                        # Only consider points that are:
-                        # 1) Inside the polygon
-                        # 2) Have a mask > 0
-                        # 3) z>=zmin
-                        # 4) z<=zmax
-                        iok   = np.where((inpol) & (imin==0) & (mask>0) & (zz>=boundary_zmin) & (zz<=boundary_zmax))
-                        mask[iok] = 2
+        if len(boundary_polygon) > 0:
+            mskbuff = np.zeros((np.shape(mask)[0] + 2, np.shape(mask)[1] + 2), dtype=int)
+            mskbuff[1:-1, 1:-1] = mask
+            # Find cells that are next to an inactive cell
+            msk4 = np.zeros((4, np.shape(mask)[0], np.shape(mask)[1]), dtype=int)
+            msk4[0, :, :] = mskbuff[0:-2, 1:-1]
+            msk4[1, :, :] = mskbuff[2:,   1:-1]
+            msk4[2, :, :] = mskbuff[1:-1, 0:-2]
+            msk4[3, :, :] = mskbuff[1:-1, 2:  ]
+            imin = msk4.min(axis=0)
+            for ip, polygon in boundary_polygon.iterrows():
+                inpol = inpolygon(xz, yz, polygon["geometry"])
+                # Only consider points that are:
+                # 1) Inside the polygon
+                # 2) Have a mask > 0
+                # 3) z>=zmin
+                # 4) z<=zmax
+                iok   = np.where((inpol) & (imin==0) & (mask>0) & (zz>=boundary_zmin) & (zz<=boundary_zmax))
+                mask[iok] = 2
 
         self.ds["mask"].values = mask                
 
 
     def mask_to_gdf(self, option="all"):
         xz = self.ds["x"].values[:]
         yz = self.ds["y"].values[:]
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/hurrywave.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/hurrywave.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,20 +384,20 @@
         if not name_list:
             name_list = []
             for st in all_stations:
                 name_list.append(st)
         
         df = pd.DataFrame(index=times, columns=name_list)
         
-        data_tmp = ddd["point_" + parameter].values
+        data_tmp = ddd["point_" + parameter]
 
         for station in name_list:
             for ist, st in enumerate(all_stations):
                 if station == st:
-                    data = data_tmp[:,ist]
+                    data = data_tmp.isel(stations=ist).values
                     data[np.isnan(data)] = -999.0
                     df[st]=data
                     break            
 
         ddd.close()
         
         return df    
@@ -734,22 +734,22 @@
                                               dem_crs,
                                               transformer_3857_to_dem,
                                               dxy,
                                               bathymetry_database)
                         ind[z<z_range[0]] = -999
                         ind[z>z_range[1]] = -999
 
-                    if self.mask:
-                        if ind.max()>=0:
-                            # Do not include points with mask<1
-                            ingrid      = np.where(ind>=0)
-                            msk         = np.zeros((256,256), dtype=int) + 1
-                            msk[ingrid] = self.mask.mask[jind[ingrid], iind[ingrid]]
-                            iex         = np.where(msk<1)
-                            ind[iex]    = -999
+                    # if self.mask:
+                    if ind.max()>=0:
+                        # Do not include points with mask<1
+                        ingrid      = np.where(ind>=0)
+                        msk         = np.zeros((256,256), dtype=int) + 1
+                        msk[ingrid] = self.grid.ds["mask"].values[jind[ingrid], iind[ingrid]]
+                        iex         = np.where(msk<1)
+                        ind[iex]    = -999
                     
                     if np.any(ind>=0):                     
                         if not path_okay:
                             if not os.path.exists(zoom_path_i):
                                 fo.mkdir(zoom_path_i)
                                 path_okay = True                             
                         # And write indices to file
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/hurrywave_builder.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/hurrywave_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 """
 Created on Sat Jun 18 09:03:08 2022
 @author: ormondt
 """
 
 import os
 from pyproj import CRS
+import geopandas as gpd
 
 from cht.model_builder.model_builder import ModelBuilder
 from cht.hurrywave.hurrywave import HurryWave
-from cht.hurrywave.hurrywave_domain import Bathymetry
-from cht.hurrywave.hurrywave_domain import Mask
-from cht.misc.geometry import RegularGrid
 import cht.misc.fileops as fo
 
 class HurryWaveBuilder(ModelBuilder):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
     def build(self,
@@ -65,59 +63,56 @@
         hw.input.variables.mskfile = mskfile
         hw.input.variables.depfile = depfile
 
         hw.input.model.path = self.model_path
         hw.input.write()
 
         ### Grid                   
+        hw.grid.build()
 
-        grid = RegularGrid(hw, self.setup_config["coordinates"]["x0"],
-                           self.setup_config["coordinates"]["y0"],
-                           self.setup_config["coordinates"]["dx"],
-                           self.setup_config["coordinates"]["dy"],
-                           self.setup_config["coordinates"]["mmax"],
-                           self.setup_config["coordinates"]["nmax"],
-                           self.setup_config["coordinates"]["rotation"],
-                           crs=crs)
-        
         ### Bathymetry
-
         if get_bathymetry:
-            # Get bathy/topo
-            bathymetry = Bathymetry()
-            bathymetry.get_bathymetry(grid, self.bathymetry_list, quiet=False)
-            # Save bathymetry
-            bathymetry.save(os.path.join(self.model_path, depfile))
+            hw.grid.get_bathymetry(self.bathymetry_list)
+            hw.grid.write_dep_file()
         
         ### Mask
-
         if make_mask:
-            mask = Mask(grid, bathymetry.z,
-                        zmin=self.setup_config["mask"]["zmin"],
-                        zmax=self.setup_config["mask"]["zmax"],
-                        include_polygons=self.include_polygons,
-                        exclude_polygons=self.exclude_polygons,
-                        open_boundary_polygons=self.open_boundary_polygons)
-            
-            hw.mask = mask
-
-            # Save
-            mask.save(os.path.join(self.model_path, mskfile))
-        else:
-            hw.mask = None
+            # Initialize polygons as None
+            include_polygon = None
+            exclude_polygon = None
+            boundary_polygon = None
+            # Read polygon files and create geodataframes
+            if self.setup_config["mask"]["include_polygon"]:
+                include_polygon = gpd.read_file(self.setup_config["mask"]["include_polygon"])
+            if self.setup_config["mask"]["exclude_polygon"]:
+                exclude_polygon = gpd.read_file(self.setup_config["mask"]["exclude_polygon"])
+            if self.setup_config["mask"]["open_boundary_polygon"]:
+                boundary_polygon = gpd.read_file(self.setup_config["mask"]["open_boundary_polygon"])
+            hw.grid.build_mask(zmin=self.setup_config["mask"]["zmin"],
+                               zmax=self.setup_config["mask"]["zmax"],
+                               include_polygon=include_polygon,
+                               include_zmin=self.setup_config["mask"]["include_zmin"],
+                               include_zmax=self.setup_config["mask"]["include_zmax"],
+                               exclude_polygon=exclude_polygon,
+                               exclude_zmin=self.setup_config["mask"]["exclude_zmin"],
+                               exclude_zmax=self.setup_config["mask"]["exclude_zmax"],
+                               boundary_polygon=boundary_polygon,
+                               boundary_zmin=self.setup_config["mask"]["open_boundary_zmin"],
+                               boundary_zmax=self.setup_config["mask"]["open_boundary_zmax"])
+            hw.grid.write_msk_file()
 
         ### Tiles        
         if make_tiles:
             dem_names = []
             z_range   = []
             zoom_range = []
             if self.setup_config["tiling"]["zmin"]>-99990.0 or self.setup_config["tiling"]["zmax"]<99990.0:
                 z_range = [self.setup_config["tiling"]["zmin"],
                            self.setup_config["tiling"]["zmax"]]
                 zoom_range = [self.setup_config["tiling"]["zoom_range_min"],
                               self.setup_config["tiling"]["zoom_range_max"]]
                 for dem in self.bathymetry_list:
-                    dem_names.append(dem.name)        
+                    dem_names.append(dem["dataset"].name)        
             hw.make_index_tiles(os.path.join(self.tile_path, "indices"),
                                 zoom_range=zoom_range,
                                 z_range=z_range,
-                                dem_names=dem_names)
+                                dem_names=dem_names)
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/hurrywave_domain.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/hurrywave_domain.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/input.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/input.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/mask.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/mask.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/observation_points.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/observation_points.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/hurrywave/to_xugrid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/hurrywave/to_xugrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_analysis.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_analysis.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_tc_forecast.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_tc_forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,18 @@
     requested_times = pd.date_range(start=time_range[0],
                       end=time_range[1],
                       freq='3H').to_pydatetime().tolist()
 
     timestep = int((requested_times[1] - requested_times[0]).total_seconds())  # get time-step of requested time assuming that the time-step stays the same
     ntime = len(requested_times)
 
-    # Get storms from endpoint metada
-    storms = check_coamps(apikey, endpoint)
+    try:
+        storms = check_coamps(apikey, endpoint)
+    except:
+        storms = {}
 
     # Check if forecast exists for the selected dates and make a dataframe
     fr = pd.DataFrame(index=requested_times)
     fr['storm_id'] = None
 
     for i, ti in enumerate(requested_times):
         fr.loc[ti, 'storm_id'] = []
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_tc_hindcast.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_tc_hindcast.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/coamps_tc_ufl_d01.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/coamps_tc_ufl_d01.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50_02.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50_02.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50_03.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50_03.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_anl_0p50_04.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_anl_0p50_04.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_forecast_0p25.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_forecast_0p25.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/gfs_forecast_0p25_02.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/gfs_forecast_0p25_02.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/meteo.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/meteo.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,18 +320,14 @@
         
         if not parameters:
             parameters = self.parameters
 
         # Merge data from netcdf files
 
         if self.source.type == "forecast":
-
-            # requested_times = pd.date_range(start=time_range[0],
-            #                           end=time_range[1],
-            #                           freq='3H').to_pydatetime().tolist()
             requested_times = pd.date_range(start=time_range[0],
                                       end=time_range[1],
                                       freq=str(self.source.time_interval) + 'H').to_pydatetime().tolist()
             requested_files = []
             for t in requested_times:
                 requested_files.append(None)
 
@@ -354,37 +350,30 @@
 
             # Use earliest forecast file available for spinup (force earlier timesteps with this file)
             ID1= next(i for i,v in enumerate(requested_files) if v is not None)
             for ind in range(ID1):
                 requested_files[ind]=requested_files[ID1]
 
             # Get rid of None values
-                # Get rid of None values
             times_to_remove = []
             for ind, file in enumerate(requested_files):
                 if not file:
                     times_to_remove.append(requested_times[ind])
             if times_to_remove:  
                 for tr in times_to_remove:
                     requested_times.remove(tr)
             requested_files = [value for value in requested_files if value != None]
 
             # Turn time array into nump array
             requested_times = np.array(requested_times)
 
         else:
-
-            # requested_times = pd.date_range(start=time_range[0],
-            #               end=time_range[1],
-            #               freq='3H').to_pydatetime().tolist()
-
             requested_files = []
             requested_times = []
             files_in_cycle = fo.list_files(os.path.join(self.path, "*.nc"))
-#            for file in files_in_cycle:                
             for ifile in range(0, len(files_in_cycle), tstride):
                 file = files_in_cycle[ifile]
                 t_file = datetime.datetime.strptime(file[-16:-3],
                                                     "%Y%m%d_%H%M")
                 if t_file>=time_range[0] and t_file<=time_range[1]:
                     requested_files.append(os.path.join(self.path, file))
                     requested_times.append(t_file)
@@ -393,20 +382,23 @@
         self.time = np.array(requested_times)
         
         if not requested_files:
             print("No meteo data files found within requested time range")
             return
 
         # Read in first file to get dimensions
-        dnc   = nc.Dataset(requested_files[0])
-        lon   = dnc["lon"][0::xystride].data
+        ds = xr.open_dataset(requested_files[0])
+        # make sure dimensions are in the right order
+        ds = ds.transpose("lat", "lon", missing_dims="warn")
+        # Get dimensions
+        lon = ds["lon"][0::xystride].values
         if lon[0]>180.0:
             lon = lon - 360.0
-        lat   = dnc["lat"][0::xystride].data
-        lat   = np.flip(lat)
+        lat = ds["lat"][0::xystride].values
+        lat = np.flip(lat)
         nrows = len(lat)
         ncols = len(lon)
         ntime = len(requested_times)
         self.x = lon
         self.y = lat
 
         for ind, param in enumerate(parameters):
@@ -424,35 +416,34 @@
                 matrix.u[:] = np.nan
                 matrix.v[:] = np.nan
             else:
                 matrix.val    = np.empty((ntime, nrows, ncols))
                 matrix.val[:] = np.nan
         
             for it, time in enumerate(requested_times):
-                
-#                print("Reading " + requested_files[it] + " ...")
-                dnc = nc.Dataset(requested_files[it])
-                uuu = dnc["wind_u"]               
+                # Read in file
+                ds = xr.open_dataset(requested_files[it])
+                # make sure dimensions are in the right order
+                ds = ds.transpose("lat", "lon", missing_dims="warn")
                 try:
-                    if param == "wind":            
-                        uuu = dnc["wind_u"][:,:].data
-                        vvv = dnc["wind_v"][:,:].data
+                    if param == "wind":
+                        uuu = ds["wind_u"].values
+                        vvv = ds["wind_v"].values
                         uuu = np.flipud(uuu[0::xystride,0::xystride])
                         vvv = np.flipud(vvv[0::xystride,0::xystride])
                         matrix.u[it,:,:] = uuu
                         matrix.v[it,:,:] = vvv
-#                        matrix.u[it,:,:] = np.flipud(dnc["wind_u"][0::xystride,0::xystride].data)
-#                        matrix.v[it,:,:] = np.flipud(dnc["wind_v"][0::xystride,0::xystride].data)
-                    else:    
-                        uuu = dnc[param][:,:].data
+                    else:
+                        uuu = ds[param].values    
                         uuu = np.flipud(uuu[0::xystride,0::xystride])
                         matrix.val[it,:,:] = uuu
-                except:
+                except Exception as e:
                     print("Could not collect " + param + " from " + requested_files[it])
-            
+                    print(str(e))
+
             self.quantity.append(matrix)        
 
 
     def read_from_delft3d(self, file_name, crs=None):
         pass
 
     def write_to_delft3d(self,
@@ -825,19 +816,25 @@
         interp = False
         if x is not None and y is not None:
             # Re-interpolate
             xg, yg = np.meshgrid(x, y)
             interp = True
         elif xlim is not None and ylim is not None:
             # Limit based on bbox
-            jlast = np.where(self.x >= xlim[1])[-1]
-            j0 = np.asarray(np.where(self.x <= xlim[0]))[0][-1]
-            j1 = np.asarray(np.where(self.x >= xlim[1]))[0][0] + 1
-            i0 = np.asarray(np.where(self.y <= ylim[0]))[0][-1]
-            i1 = np.asarray(np.where(self.y >= ylim[1]))[0][0] + 1
+            try:
+                jlast = np.where(self.x >= xlim[1])[-1]
+                j0 = np.asarray(np.where(self.x <= xlim[0]))[0][-1]
+                j1 = np.asarray(np.where(self.x >= xlim[1]))[0][0] + 1
+                i0 = np.asarray(np.where(self.y <= ylim[0]))[0][-1]
+                i1 = np.asarray(np.where(self.y >= ylim[1]))[0][0] + 1
+            except IndexError as e:
+                print(
+                    "Meteo input data does not cover domain, check meteo input and subsetting bbox"
+                )
+                raise (e)
             x = self.x[j0:j1:stride]
             y = self.y[i0:i1:stride]       
         else:    
             j0 = 0
             j1 = len(self.x) - 1
             i0 = 0
             i1 = len(self.y) - 1
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/meteo3.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/meteo3.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/meteo/test_coamps.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/meteo/test_coamps.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/argo.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/argo.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/deltares_ini.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/deltares_ini.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/fileops.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/fileops.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 
 def copy_file(src, dst):
     all_files = glob.glob(src)
     if len(all_files) == 0:
         all_files = [src]
     for full_file_name in all_files:
+        if not os.path.exists(full_file_name):
+            print(full_file_name + " does not exist")
+            return
         src_name = os.path.basename(full_file_name)
         if os.path.exists(os.path.join(dst, src_name)):
             os.remove(os.path.join(dst, src_name))
         if os.path.isdir(full_file_name):
             dstf = os.path.join(dst, os.path.basename(full_file_name))
             shutil.copytree(full_file_name, dstf)
         else:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/geometry.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/geometry.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/misc_tools.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/misc_tools.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/pli_file.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/pli_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,19 @@
         gdf_list.append(d)
     if crs is not None:     
         gdf = gpd.GeoDataFrame(gdf_list, crs=crs)
     else:
         gdf = gpd.GeoDataFrame(gdf_list)
     return gdf
 
+def pli2geojson(file_name_in, file_name_out, crs=None):
+    gdf = pli2gdf(file_name_in, crs=None)
+    gdf.to_file(file_name_out, driver='GeoJSON')
+
+
 def pol2gdf(file_name, crs=None, header=True):
     gdf_list = []
     if not header:
         df = pd.read_csv(file_name, index_col=False, header=None,
               delim_whitespace=True, names=['x', 'y'])
         line = shapely.geometry.Polygon(list(zip(df.x.values, df.y.values)))
         d = {"geometry": line}
@@ -85,14 +90,18 @@
 
     if crs is not None:     
         gdf = gpd.GeoDataFrame(gdf_list, crs=crs)
     else:
         gdf = gpd.GeoDataFrame(gdf_list)
     return gdf
 
+def pol2geojson(file_name_in, file_name_out, crs=None):
+    gdf = pol2gdf(file_name_in, crs=None)
+    gdf.to_file(file_name_out, driver='GeoJSON')
+
 def gdf2pli(gdf, file_name, header=True):
     if gdf.crs.is_geographic:
         fid = open(file_name, "w")
         for index, row in gdf.iterrows():
             nrp = len(row["geometry"].coords)
             if header:
                 fid.write("BL" + str(index + 1).zfill(4) + "\n")
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/prob_maps.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/prob_maps.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,37 +43,50 @@
     dsin.to_netcdf(path=output_file_name)
     dsin.close()
 
 def merge_nc_his(file_list, variables, prcs=None, delete=False, output_file_name=None):
 
     if prcs is None:
         prcs = [0.05, 0.5, 0.95]
-
+    
+    if len(file_list)==0:
+        print('his-file list is empty')
+        return
     nens = len(file_list)
 
     # Read first file    
     ds = xr.open_dataset(file_list[0])
+    if 'runtime' in ds.dims:
+        ds = ds.drop_dims('runtime') #hurrywave
 
-    # Read time and stations from first file
-    time = ds.time
-    stations = ds.stations
+    # Read dimensions from first file
+    dimensions = list(ds.dims.keys())
+
+    # Ensure 'time' comes first in the list of dimensions
+    dimensions = ['time'] + [dim for dim in dimensions if dim != 'time']
+
+    # Create ensemble dimension
+    new_dimensions = list(dimensions + ['ensemble'])
     ens = range(nens)
 
     # Make new data array filled with zeros with dimensions time, stations and ens
     for v in variables:
-
-        arr = xr.DataArray(data=np.zeros((len(time), len(stations), nens)),
-                           dims=['time', 'stations', 'ensemble'],
-                           coords={'time': time, 'station': stations, 'ensemble': ens})   
-        ds[v] = arr  
+        ds[v] = xr.DataArray(
+                data=np.zeros(tuple(ds.dims[dim] if dim in ds.dims else nens for dim in new_dimensions)),
+                dims=new_dimensions,
+                coords={dim: ds[dim] if dim in ds.dims else ens for dim in new_dimensions})
 
     for iens, file in enumerate(file_list):
         dsin = xr.open_dataset(file)
+
+        if 'runtime' in dsin.dims:
+            dsin = dsin.drop_dims('runtime') #hurrywave
+
         for v in variables:
-            ds[v][:,:,iens] = dsin[v]
+            ds[v][:,:,iens] = dsin[v].transpose('time', ...)
 
     for v in variables:
         ds[v].fillna(-999.0) 
         arr = ds[v].fillna(-999.0).quantile(prcs, dim="ensemble")
         for ip, p in enumerate(prcs):
             ds[v + "_" + str(round(p*100))] = arr[ip,:,:] 
         
@@ -111,20 +124,21 @@
 
     for iens, file in enumerate(file_list):
         dsin = xr.open_dataset(file)
         for v in variables:
             ds[v][:,:,:,iens] = dsin[v]
 
     for v in variables:
-        arr = ds[v].fillna(-999.0).quantile(prcs, dim="ensemble", skipna=False)
+        # arr = ds[v].fillna(-999.0).quantile(prcs, dim="ensemble", skipna=False)
+        arr = ds[v].quantile(prcs, dim="ensemble", skipna=True)
         for ip, p in enumerate(prcs):
             ds[v + "_" + str(round(p*100))] = arr[ip,:,:,:]
 
     # Remove the original variables
-    to_drop = ["zs", "zsmax", "cumprcp", "cuminf", "qinf"]
+    to_drop = ["zs", "zsmax", "cumprcp", "cuminf", "qinf", "hm0max"]
     for v in to_drop:
         if v in ds:
             ds = ds.drop(v)
         
     try:
         fo.delete_file(output_file_name)
     except:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/sftp.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/sftp.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/tekal.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/tekal.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/misc/xmlkit.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/misc/xmlkit.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/model_builder/model_builder.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/model_builder/model_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -155,18 +155,26 @@
         self.setup_config["coordinates"]["rotation"]          = 0.0
         self.setup_config["coordinates"]["crs"]               = "WGS 84"
         self.setup_config["quadtree"]                         = {}
         self.setup_config["quadtree"]["refinement_level"]     = []
         self.setup_config["mask"]                             = {}
         self.setup_config["mask"]["zmin"]                     = -99999.0
         self.setup_config["mask"]["zmax"]                     = 99999.0
-        self.setup_config["mask"]["include_polygon"]          = []
-        self.setup_config["mask"]["exclude_polygon"]          = []
-        self.setup_config["mask"]["open_boundary_polygon"]    = []
-        self.setup_config["mask"]["outflow_boundary_polygon"] = []
+        self.setup_config["mask"]["include_polygon"]          = None
+        self.setup_config["mask"]["include_zmin"]             = -99999.0
+        self.setup_config["mask"]["include_zmax"]             = 99999.0
+        self.setup_config["mask"]["exclude_polygon"]          = None
+        self.setup_config["mask"]["exclude_zmin"]             = -99999.0
+        self.setup_config["mask"]["exclude_zmax"]             = 99999.0
+        self.setup_config["mask"]["open_boundary_polygon"]    = None
+        self.setup_config["mask"]["open_boundary_zmin"]       = -99999.0
+        self.setup_config["mask"]["open_boundary_zmax"]       = 99999.0
+        self.setup_config["mask"]["outflow_boundary_polygon"] = None
+        self.setup_config["mask"]["outflow_boundary_zmin"]    = -99999.0
+        self.setup_config["mask"]["outflow_boundary_zmax"]    = 99999.0
         # self.setup_config["wave_mask"]                             = {}
         # self.setup_config["wave_mask"]["zmin"]                     = -99999.0
         # self.setup_config["wave_mask"]["zmax"]                     = 99999.0
         # self.setup_config["wave_mask"]["include_polygon"]          = []
         # self.setup_config["wave_mask"]["exclude_polygon"]          = []
         # self.setup_config["wave_mask"]["open_boundary_polygon"]    = []
         self.setup_config["subgrid"]                          = {}
@@ -231,48 +239,40 @@
         else:
             if "zmin" not in self.setup_config["mask"]:
                 self.setup_config["mask"]["zmin"] = -99999.0
             if "zmax" not in self.setup_config["mask"]:
                 self.setup_config["mask"]["zmax"] = 99999.0
 
         if "include_polygon" not in self.setup_config["mask"]:
-            self.setup_config["mask"]["include_polygon"] = []
-        if self.setup_config["mask"]["include_polygon"]:
-            for polygon in self.setup_config["mask"]["include_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
+            self.setup_config["mask"]["include_polygon"] = None
+        if "include_zmin" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["include_zmin"] = -99999.0
+        if "include_zmax" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["include_zmax"] = 99999.0
 
         if "exclude_polygon" not in self.setup_config["mask"]:
-            self.setup_config["mask"]["exclude_polygon"] = []
-        if self.setup_config["mask"]["exclude_polygon"]:
-            for polygon in self.setup_config["mask"]["exclude_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
+            self.setup_config["mask"]["exclude_polygon"] = None
+        if "exclude_zmin" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["exclude_zmin"] = -99999.0
+        if "exclude_zmax" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["exclude_zmax"] = 99999.0
 
         if "open_boundary_polygon" not in self.setup_config["mask"]:
-            self.setup_config["mask"]["open_boundary_polygon"] = []
-        if self.setup_config["mask"]["open_boundary_polygon"]:
-            for polygon in self.setup_config["mask"]["open_boundary_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
+            self.setup_config["mask"]["open_boundary_polygon"] = None
+        if "open_boundary_zmin" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["open_boundary_zmin"] = -99999.0
+        if "open_boundary_zmax" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["open_boundary_zmax"] = 99999.0
 
         if "outflow_boundary_polygon" not in self.setup_config["mask"]:
-            self.setup_config["mask"]["outflow_boundary_polygon"] = []
-        if self.setup_config["mask"]["outflow_boundary_polygon"]:
-            for polygon in self.setup_config["mask"]["outflow_boundary_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
+            self.setup_config["mask"]["outflow_boundary_polygon"] = None
+        if "outflow_boundary_zmin" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["outflow_boundary_zmin"] = -99999.0
+        if "outflow_boundary_zmax" not in self.setup_config["mask"]:
+            self.setup_config["mask"]["outflow_boundary_zmax"] = 99999.0
 
 
         if "wave_mask" not in self.setup_config:
             self.setup_config["wave_mask"] = {}
             # self.setup_config["wave_mask"]["zmin"] = -99999.0
             # self.setup_config["wave_mask"]["zmax"] = 99999.0
         else:
@@ -382,53 +382,35 @@
                 for file in level["file_list"]:
                     polygons = read_pli_file(os.path.join(self.data_path, file))
                     for p in polygons:
                         self.refinement_polygons.append(RefinementPolygon(level["level"],
                                                                           x=p.x,
                                                                           y=p.y))
             
-        # Mask polygons        
-        self.include_polygons = []
-        for polygon in self.setup_config["mask"]["include_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.include_polygons.append(MaskPolygon(x=p.x,
-                                                         y=p.y,
-                                                         zmin=polygon["zmin"],
-                                                         zmax=polygon["zmax"]))            
-    
-        self.exclude_polygons = []
-        for polygon in self.setup_config["mask"]["exclude_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.exclude_polygons.append(MaskPolygon(x=p.x,
-                                                         y=p.y,
-                                                         zmin=polygon["zmin"],
-                                                         zmax=polygon["zmax"]))            
-        self.open_boundary_polygons = []
-        for polygon in self.setup_config["mask"]["open_boundary_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.open_boundary_polygons.append(MaskPolygon(x=p.x,
-                                                   y=p.y,
-                                                   zmin=polygon["zmin"],
-                                                   zmax=polygon["zmax"]))            
+        # Mask polygons (add full paths here)       
+        if self.setup_config["mask"]["include_polygon"]:
+            self.setup_config["mask"]["include_polygon"] = os.path.join(self.data_path, self.setup_config["mask"]["include_polygon"])
     
-        self.outflow_boundary_polygons = []
-        for polygon in self.setup_config["mask"]["outflow_boundary_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.outflow_boundary_polygons.append(MaskPolygon(x=p.x,
-                                                                  y=p.y,
-                                                                  zmin=polygon["zmin"],
-                                                                  zmax=polygon["zmax"]))            
+        if self.setup_config["mask"]["exclude_polygon"]:
+            self.setup_config["mask"]["exclude_polygon"] = os.path.join(self.data_path, self.setup_config["mask"]["exclude_polygon"])
+
+        if self.setup_config["mask"]["open_boundary_polygon"]:
+            self.setup_config["mask"]["open_boundary_polygon"] = os.path.join(self.data_path, self.setup_config["mask"]["open_boundary_polygon"])
+
+
+        # This is all sfincs stuff that should be done with HydroMT    
+        # self.outflow_boundary_polygons = []
+        # for polygon in self.setup_config["mask"]["outflow_boundary_polygon"]:
+        #     polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
+        #     # Polygon file may include multiple polygons
+        #     for p in polygons:
+        #         self.outflow_boundary_polygons.append(MaskPolygon(x=p.x,
+        #                                                           y=p.y,
+        #                                                           zmin=polygon["zmin"],
+        #                                                           zmax=polygon["zmax"]))            
 
         # Wave mask polygons        
         if self.setup_config["wave_mask"]:
             self.wave_include_polygons = []
             for polygon in self.setup_config["wave_mask"]["include_polygon"]:
                 polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
                 # Polygon file may include multiple polygons
@@ -457,21 +439,20 @@
                                                        zmin=polygon["zmin"],
                                                        zmax=polygon["zmax"]))            
 
                 
         # Bathymetry and roughness
         self.bathymetry_list = []
         for dataset in self.setup_config["bathymetry"]["dataset"]:
-            self.bathymetry_list.append(BathymetryDataset(name=dataset["name"],
-                                                          source=dataset["source"],
-                                                          zmin=dataset["zmin"],
-                                                          zmax=dataset["zmax"]))
+            ds = bathymetry_database.get_dataset(dataset["name"])
+            bds = {"dataset": ds, "zmin": dataset["zmin"], "zmax": dataset["zmax"]}
+            self.bathymetry_list.append(bds)
     
-        self.roughness_list = []
-        if "dataset" in self.setup_config["roughness"]:
-            for dataset in self.setup_config["roughness"]["dataset"]:
-                self.roughness_list.append(BedRoughnessDataset(name=dataset["name"],
-                                                               source=dataset["source"],
-                                                               zlevel=dataset["zlevel"],
-                                                               roughness_deep=dataset["roughness_deep"],
-                                                               roughness_shallow=dataset["roughness_shallow"]))
+        # self.roughness_list = []
+        # if "dataset" in self.setup_config["roughness"]:
+        #     for dataset in self.setup_config["roughness"]["dataset"]:
+        #         self.roughness_list.append(BedRoughnessDataset(name=dataset["name"],
+        #                                                        source=dataset["source"],
+        #                                                        zlevel=dataset["zlevel"],
+        #                                                        roughness_deep=dataset["roughness_deep"],
+        #                                                        roughness_shallow=dataset["roughness_shallow"]))
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/nesting/nest1.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/nesting/nest1.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/nesting/nest2.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/nesting/nest2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 import glob
 import datetime 
 from cht.misc.deltares_ini import IniStruct
 from cht.tide.tide_predict import predict
 
 def nest2(overall,
           detail,
-          boundary_water_level_correction=None,
           output_path=None,
           output_file=None,
-	      option=None,
-          return_maximum=False,
-          ensemble=False,
-          ensemble_member_index=None,
           bc_path=None,
           bc_file=None,
           overall_crs=None,
-          detail_crs=None):
+          detail_crs=None,
+	      option=None,
+          boundary_water_level_correction=None,
+          return_maximum=False):
 
 
     if not boundary_water_level_correction:
         # Path of the overall output time series
         boundary_water_level_correction = 0.0
     
     if type(overall) == str:
@@ -59,154 +57,143 @@
     if detail_crs is not None:
         detail.crs = CRS(detail_crs)
 
     if overall.type.lower() == "delft3dfm":
 
         if detail.type.lower() == "delft3dfm":
             nest2_delft3dfm_in_delft3dfm(overall,
-                                         detail,
-                                         output_path,
-                                         output_file,
-                                         boundary_water_level_correction,
-                                         bc_path=bc_path)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            boundary_water_level_correction=boundary_water_level_correction)
 
         elif detail.type.lower() == "sfincs":
             nest2_sfincs_in_delft3dfm(overall,
-                                      detail,
-                                      output_path,
-                                      output_file,
-                                      boundary_water_level_correction,
-                                      bc_path=bc_path)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            boundary_water_level_correction=boundary_water_level_correction)
 
         elif detail.type.lower() == "beware":
             nest2_beware_in_delft3dfm(overall,
-                                      detail,
-                                      output_path,
-                                      output_file,
-                                      boundary_water_level_correction,
-                                      option, 
-                                      bc_path=bc_path)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            option=option,
+                                            boundary_water_level_correction=boundary_water_level_correction)
             
     elif overall.type.lower() == "sfincs":
 
         if detail.type.lower() == "sfincs":
             zs = nest2_sfincs_in_sfincs(overall,    
-                                        detail,
-                                        output_path,
-                                        output_file,
-                                        boundary_water_level_correction,
-                                        return_maximum=return_maximum,
-                                        bc_path=bc_path,
-                                        ensemble_member_index=ensemble_member_index)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            boundary_water_level_correction=boundary_water_level_correction,
+                                            return_maximum=return_maximum)
             return zs
         elif detail.type.lower() == "xbeach":
             bc = nest2_xbeach_in_sfincs(overall,
-                                        detail,
-                                        output_path,
-                                        output_file,
-                                        boundary_water_level_correction,
-                                        return_maximum=return_maximum,
-                                        bc_path=bc_path)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            boundary_water_level_correction=boundary_water_level_correction,
+                                            return_maximum=return_maximum)
             return bc
         elif detail.type.lower() == "beware":
             nest2_beware_in_sfincs(overall,
-                                   detail,
-                                   output_path,
-                                   output_file,
-                                   boundary_water_level_correction,
-                                   option,
-                                   bc_path=bc_path,
-                                   ensemble_member_index=ensemble_member_index)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            option=option,
+                                            boundary_water_level_correction=boundary_water_level_correction)
 
     elif overall.type.lower() == "hurrywave":
 
         if detail.type.lower() == "hurrywave":
             nest2_hurrywave_in_hurrywave(overall,
-                                    detail,
-                                    output_path,
-                                    output_file,
-                                    bc_path=bc_path,
-                                    ensemble_member_index=ensemble_member_index)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path)
             
         elif detail.type.lower() == "xbeach":
             bc = nest2_xbeach_in_hurrywave(overall,
-                                    detail,
-                                    output_path,
-                                    output_file,
-                                    option,
-                                    return_maximum=return_maximum,
-                                    bc_path=bc_path)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            option=option,
+                                            return_maximum=return_maximum)
             return bc
         elif detail.type.lower() == "sfincs":
             nest2_sfincs_in_hurrywave(overall,
-                                      detail,
-                                      output_path,
-                                      output_file,
-                                      bc_path=bc_path,
-                                      ensemble_member_index=ensemble_member_index)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path)
 
         elif detail.type.lower() == "beware":
             nest2_beware_in_hurrywave(overall,
-                                      detail,
-                                      output_path,
-                                      output_file,
-                                      bc_path=bc_path,
-                                      ensemble_member_index=ensemble_member_index)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path)
 
     elif overall.type.lower() == "beware":
 
         if detail.type.lower() == "sfincs":
             nest2_sfincs_in_beware(overall,
-                                    detail,
-                                    output_path,
-                                    output_file,
-                                    boundary_water_level_correction,
-                                    option,
-                                    bc_path=bc_path,
-                                    ensemble_member_index=ensemble_member_index)
+                                            detail,
+                                            output_path=output_path,
+                                            output_file=output_file,
+                                            bc_path=bc_path,
+                                            option=option,
+                                            boundary_water_level_correction=boundary_water_level_correction)
+
 
 def nest2_delft3dfm_in_delft3dfm(overall,
                                  detail,
-                                 output_path,
-                                 output_file,
-                                 boundary_water_level_correction,
-                                 bc_path=None):
-
-    if not output_file:
-        # Path of the overall output time series
-        output_file = "flow_his.nc"
-
-#    output_file = os.path.join(output_path, output_file)
+                                 output_path=None,
+                                 output_file= "flow_his.nc",
+                                 boundary_water_level_correction=0,
+                                 bc_path= None):
 
     for ind, bnd in enumerate(detail.boundary):        
         point_names = []
         for ip, point in enumerate(bnd.point):
             point_names.append(detail.name + "_" + point.name)
+
         # Return DataFrame bzs
         bzs = overall.read_timeseries_output(name_list=point_names,
                                              path=output_path,
                                              file_name=output_file)
         ts  = bzs.index
         for ip, point in enumerate(bnd.point):
             point.data = pd.Series(bzs.iloc[:,ip].values, index=ts) + boundary_water_level_correction    
     
     if bc_path is not None:
-        detail.write_flow_boundary_conditions()
+        detail.write_flow_boundary_conditions(path=bc_path) # check if this works
 
 def nest2_sfincs_in_delft3dfm(overall,
                               detail,
-                              output_path,
-                              output_file,
-                              boundary_water_level_correction,
+                              output_path=None,
+                              output_file=None,
+                              boundary_water_level_correction=0,
                               bc_path=None):
-
+    
     if not output_file:
-        # Path of the overall output time series
         output_file = "flow_his.nc"
-    
+
     point_names = []
     for point in detail.flow_boundary_point:
         point_names.append(detail.name + "_" + point.name)                    
     output_file = os.path.join(output_path, output_file)
 
     # Return DataFrame bzs
     bzs = overall.read_timeseries_output(name_list=point_names,
@@ -219,21 +206,22 @@
     
     # Write bzs file
     if bc_path is not None:
         detail.write_flow_boundary_conditions(file_name=os.path.join(bc_path, detail.input.bzsfile))
 
 def nest2_beware_in_delft3dfm(overall,
                               detail,
-                              output_path,
-                              output_file,
-                              boundary_water_level_correction,
-                              option,
+                              output_path=None,
+                              output_file=None,
+                              boundary_water_level_correction = 0,
+                              option=None,
                               bc_path=None):
 
     if option == 'flow':
+
         if not output_file:
             # Path of the overall output time series
             output_file = "flow_his.nc"
         
         point_names = []
         for point in detail.flow_boundary_point:
             point_names.append(detail.name + "_" + point.name) #reopen                   
@@ -249,15 +237,14 @@
             point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction  
         
         if bc_path is not None:
             detail.write_flow_boundary_conditions(file_name=os.path.join(bc_path, detail.input.bzsfile))
             
     if option == 'wave':
 
-
         if not output_path:
             # Path of the overall output time series
             output_path = overall.path
             
         if not output_file:
             file_name = os.path.join(output_path, "wavh-wave-nest.nc")
         else:
@@ -310,25 +297,23 @@
 
         if bc_path is not None:
             detail.write_wave_boundary_conditions(path=bc_path)
 
 
 def nest2_sfincs_in_sfincs(overall,
                            detail,
-                           output_path,
-                           output_file,
-                           boundary_water_level_correction,
+                           output_path=None,
+                           output_file=None,
+                           boundary_water_level_correction=0,
                            return_maximum=False,
-                           ensemble_member_index=None,
                            bc_path=None):
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
-    
         
     if overall.input.outputformat[0:3] == "bin":
         # ascii output        
         if not output_file:
             output_file = "zst.txt"
     else:
         # netcdf        
@@ -338,48 +323,48 @@
     point_names = []
     for point in detail.flow_boundary_point:
         point_names.append(detail.name + "_" + point.name)                    
     zstfile = os.path.join(output_path, output_file)
 
     # Return DataFrame bzs
     bzs = overall.read_timeseries_output(name_list=point_names,
-                                         file_name=zstfile,
-                                         ensemble_member_index=ensemble_member_index)
+                                         file_name=zstfile)
     ts  = bzs.index
     
     # Astro correction
     vcor = 0.0
     if detail.input.corfile:        
         vcor = get_vcor(os.path.join(detail.path, detail.input.corfile), ts)
 
     for icol, point in enumerate(detail.flow_boundary_point):
         point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction + vcor
 
     # Write bzs file
     if bc_path is not None:
         detail.write_flow_boundary_conditions(file_name=os.path.join(bc_path, detail.input.bzsfile))
 
-    # Why do we need this?
+    # zs_maximum for clustering
+    # zs_maximum for clustering
     if return_maximum:
         zmax = -999.0
         for icol, point in enumerate(detail.flow_boundary_point):
             zx = point.data.max()
             if zx>zmax:
                 zs = point.data
                 zmax = zx
         return zs                            
     else:    
         return detail.flow_boundary_point
 
 
 def nest2_xbeach_in_sfincs(overall,
                            detail,
-                           output_path,
-                           output_file,
-                           boundary_water_level_correction,
+                           output_path=None,
+                           output_file=None,
+                           boundary_water_level_correction=0,
                            return_maximum=False,
                            bc_path=None):
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
@@ -406,83 +391,85 @@
     bzs_interpolated = bzs_resampled.interpolate(method='linear')
     bzs_filtered = bzs_interpolated[detail.tref:detail.tstop]
     
     ts  = bzs_filtered.index
     for icol, point in enumerate(detail.flow_boundary_point):
         point.data = pd.Series(bzs_filtered.iloc[:,icol].values, index=ts) + boundary_water_level_correction
 
+    # Write boundary conditions
+    if bc_path is not None:
+        detail.write_flow_boundary_conditions()
+
     if return_maximum:
         zmax = -999.0
         if len(detail.flow_boundary_point) <= 2:
             for icol, point in enumerate(detail.flow_boundary_point):
                 if icol == 1:
                     break
                 zx = point.data.max()
                 if zx>zmax:
                     zs = point.data
                     zmax = zx
+                    
         elif len(detail.flow_boundary_point) == 4:
             for icol, point in enumerate(detail.flow_boundary_point):
                 if icol == 2:
                     break
                 zx = point.data.max()
                 if zx>zmax:
                     zs = point.data
                     zmax = zx
-        return zs                            
+
+        return zs                          
     else:    
         return detail.flow_boundary_point
     
     # Write boundary conditions
     if bc_path is not None:
-        detail.write_flow_boundary_conditions()
+        detail.write_flow_boundary_conditions() # check Roel
 
 def nest2_beware_in_sfincs(overall,
                            detail,
-                           output_path,
-                           output_file,
-                           boundary_water_level_correction,
-                           option,
-                           bc_path=None,
-                           ensemble_member_index=None):
+                           output_path=None,
+                           output_file=None,
+                           boundary_water_level_correction=0,
+                           option=None,
+                           bc_path=None):
 
     if option == 'flow':
         if not output_file:
             # Path of the overall output time series
             output_file = "sfincs_his.nc"
         
         point_names = []
         for point in detail.flow_boundary_point:
             point_names.append(detail.name + "_" + point.name) #reopen                   
             # point_names.append(point.name)                    
         # output_file = os.path.join(output_path, output_file)
 
         # Return DataFrame bzs
         bzs = overall.read_timeseries_output(name_list=point_names,
-                                             file_name=os.path.join(output_path,
-                                                                    output_file))
+                                             file_name=os.path.join(output_path, output_file))
 
         # Replace -999.0 with zeros. This should not happen, but easy fix for now.
         bzs = bzs.replace(-999.0,0.0)
         for icol, point in enumerate(detail.flow_boundary_point):
             point.data = pd.Series(bzs.iloc[:,icol].values, index=bzs.index) + boundary_water_level_correction    
             
         if bc_path is not None:
             detail.write_flow_boundary_conditions(file_name=os.path.join(bc_path, detail.input.bzsfile))
 
 def nest2_hurrywave_in_hurrywave(overall,
                                  detail,
-                                 output_path,
-                                 output_file,
-                                 bc_path=None,
-                                 ensemble_member_index=None):
+                                 output_path=None,
+                                 output_file=None,
+                                 bc_path=None):
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
-        
     if not output_file:
         output_file = "hurrywave_sp2.nc"
 
     file_name = os.path.join(output_path, output_file)
     
     detail.boundary_conditions.forcing = "spectra"
 
@@ -527,36 +514,38 @@
                 coords    = dict(time=times,
                                  theta=theta,
                                  sigma=sigma)
                 )
         detail.boundary_conditions.gdf.loc[ind, "spectra"] = ds.to_array()
 
     if bc_path is not None:
-        detail.boundary_conditions.write_boundary_conditions_spectra()
+        detail.boundary_conditions.write_boundary_conditions_spectra(file_name=os.path.join(bc_path, detail.input.variables.bspfile))
 
      
 def nest2_xbeach_in_hurrywave(overall,
                               detail,
-                              output_path,
-                              output_file,
-                              option,
+                              output_path=None,
+                              output_file=None,
+                              option=None,
                               return_maximum=False,
                               bc_path=None):
     
     from cht.physics.deshoal import deshoal
     from scipy import interpolate
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
 
     if option == "sp2":    
         if not output_file:
             output_file = "hurrywave_sp2.nc"
     
         file_name = os.path.join(output_path, output_file)
+
+
     
         # Open netcdf file
         ddd = xr.open_dataset(file_name)
         stations=ddd.station_name.values
         all_stations = []
         for ist, st in enumerate(stations):
             st=str(st.strip())[2:-1]
@@ -623,20 +612,20 @@
 
         ireq = []    
         for ip, point in enumerate(point_names):
             for ist,st in enumerate(all_stations):
                 if point.lower() == st.lower():
                     ireq.append(ist)            
                     break
-    
+
         for ip, point in enumerate(detail.wave_boundary_point):
-    
             hm0     = ddd.point_hm0.values[:,ireq[ip]]
             tp      = ddd.point_tp.values[:,ireq[ip]]
             zb_point = ddd.station_z.values[ip]
+
             #deshoal waveheights to offshore boundary
             hm0_deshoal = []
             if detail.zb_deshoal:
                 try:
                     zs = detail.flow_boundary_point[0].data
                     # Interpolate to wave timeseries
                     wave_secs = times.astype(float)
@@ -675,15 +664,15 @@
     
             df_filtered.insert(5,'duration', 1800)
             df_filtered.insert(6,"dtbc",1)
             
             point.data = df_filtered
 
         if bc_path is not None:
-            detail.write_wave_boundary_conditions(option=option)
+            detail.write_wave_boundary_conditions(option=option) # check roel
 
     if return_maximum:
         hmax = -999.0
         for icol, point in enumerate(detail.wave_boundary_point):
             hx = point.data["hm0"].max()
             if hx>hmax:
                 hmx = point.data["hm0"]
@@ -692,26 +681,23 @@
                     
     else:    
         return detail.wave_boundary_point
 
 
 def nest2_sfincs_in_hurrywave(overall,
                               detail,
-                              output_path,
-                              output_file,
-                              bc_path=None,
-                              ensemble_member_index=None):
+                              output_path=None,
+                              output_file=None,
+                              bc_path=None):
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
-        
     if not output_file:
         output_file = "hurrywave_his.nc"
-
-
+        
     file_name = os.path.join(output_path, output_file)
     print("Nesting in " + file_name)
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     stations=ddd.station_name.values
     all_stations = []
@@ -749,30 +735,28 @@
         df.insert(1,"tp",tp)
         df.insert(2,"wavdir",wavdir)
         df.insert(3,"dirspr",dirspr)
 
         point.data = df
 
     if bc_path is not None:
-        detail.write_wave_boundary_conditions()
+        detail.write_wave_boundary_conditions(path=bc_path)
 
 def nest2_beware_in_hurrywave(overall,
                               detail,
-                              output_path,
-                              output_file,
-                              bc_path=None,
-                              ensemble_member_index=None):
+                              output_path=None,
+                              output_file=None,
+                              bc_path=None):
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
-        
     if not output_file:
         output_file = "hurrywave_his.nc"
-
+        
     file_name = os.path.join(output_path, output_file)
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     stations=ddd.station_name.values
     all_stations = []
     for ist, st in enumerate(stations):
@@ -814,24 +798,25 @@
 
     if bc_path is not None:
         detail.write_wave_boundary_conditions(path=bc_path)
 
 
 def nest2_sfincs_in_beware(overall,
                            detail,
-                           output_path,
-                           output_file,
-                           boundary_water_level_correction,
-                           option,
-                           bc_path=None,
-                           ensemble_member_index=None):
+                           output_path=None,
+                           output_file=None,
+                           boundary_water_level_correction=0,
+                           option=None,
+                           bc_path=None):
 
     from cht.sfincs.sfincs import FlowBoundaryPoint
     from cht.sfincs.sfincs import WaveMakerForcingPoint
 
+    if not output_file:
+        output_file = "beware_his.nc"
     # Get bounding box for sfincs model
     # Convert bbox to beware crs
 
     x_range, y_range = detail.bounding_box(crs=overall.crs)
     dx = (x_range[1] - x_range[0])/10
     dy = (y_range[1] - y_range[0])/10
     x_range[0] = x_range[0] - dx
@@ -840,16 +825,14 @@
     y_range[1] = y_range[1] + dy
     
     # Read BEWARE offshore locations
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
-    if not output_file:
-        output_file = "beware_his.nc"
     file_name = os.path.join(output_path, output_file)
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     
     if option == "flow":
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/_ndbc.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/_ndbc.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/_noaa_coops.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/_noaa_coops.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/observation_stations/observation_stations.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/observation_stations/observation_stations.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/deshoal.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/deshoal.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/disper.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/disper.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/physics/vo21.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/physics/vo21.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/quadtree.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/quadtree.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/regulargrid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/regulargrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/sfincs.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/sfincs.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,23 +226,19 @@
         ts  = df.index
         for icol, point in enumerate(self.flow_boundary_point):
             point.data = pd.Series(df.iloc[:,icol].values, index=ts)
         
     def write_flow_boundary_conditions(self, file_name=None):
 
         # Write SFINCS bzs file
-        if not file_name:
-            if not self.input.bzsfile:
-                return
-            file_name = os.path.join(self.path,
-                                     self.input.bzsfile)
-            
-        if not file_name:
+        if not file_name and not self.input.bzsfile:
             return
-        
+        if not file_name:
+            file_name = os.path.join(self.path, self.input.bzsfile)
+                    
         # Build a new DataFrame
         df = pd.DataFrame()
         for point in self.flow_boundary_point:
             df = pd.concat([df, point.data], axis=1)
         tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
@@ -578,16 +574,15 @@
     ### Output ###
 
     def read_timeseries_output(
             self,
             path=None, 
             file_name=None,
             name_list=None,
-            parameter="point_zs",
-            ensemble_member_index=None,
+            parameter="point_zs"
     ):
 
         if path is None and hasattr(self, "path"):
             path = self.path
         elif path is None:
             path = os.getcwd()
 
@@ -641,18 +636,15 @@
                     name_list.append(st)
             
             df = pd.DataFrame(index=times, columns=name_list)
 
             for station in name_list:
                 for ist, st in enumerate(all_stations):
                     if station == st:
-                        if ensemble_member_index is None:
-                            wl = ddd[parameter].values[:,ist]
-                        else:
-                            wl = ddd[parameter].values[:,ist,ensemble_member_index]    
+                        wl = ddd[parameter].isel(stations=ist).values
                         wl[np.isnan(wl)] = -999.0
                         df[st]=wl
                         break            
     
             ddd.close()
                     
         return df    
@@ -688,16 +680,16 @@
                 if time<=time_range[1]:
                     it1 = it
 
             # Check if dimension nmesh2d_face exists (in which case this is a quadtree mesh)
             if 'nmesh2d_face' in dsin[varname].dims:
                 zsmax = np.nanmax(dsin[varname].values[it0:it1 + 1,:], axis=0)
             else:                
-                zsmax = np.transpose(np.nanmax(dsin.zsmax.values[it0:it1 + 1,:,:], axis=0))
-                zsmax = np.nanmax(dsin.zsmax.values[it0:it1 + 1,:,:], axis=0)
+                zsmax = np.transpose(np.nanmax(dsin[varname].values[it0:it1 + 1,:,:], axis=0))
+                zsmax = np.nanmax(dsin[varname].values[it0:it1 + 1,:,:], axis=0)
             dsin.close()
 
             return zsmax
 
 
 
         else:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/sfincs_builder.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/sfincs_builder.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs/subgrid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs/subgrid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/boundary_conditions.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/boundary_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,34 +238,34 @@
         # # Get coordinates of boundary points
         # if self.model.grid_type == "regular":
         #     da_mask = self.model.grid.ds["mask"]
         #     ibnd = np.where(da_mask.values == 2)
         #     xp = da_mask["xc"].values[ibnd]
         #     yp = da_mask["yc"].values[ibnd]
         # else:
-            mask = self.model.grid.data["mask"]
-            ibnd = np.where(mask == 2)
-            xz, yz = self.model.grid.face_coordinates()
-            xp = xz[ibnd]
-            yp = yz[ibnd]
+        mask = self.model.grid.data["mask"]
+        ibnd = np.where(mask == 2)
+        xz, yz = self.model.grid.face_coordinates()
+        xp = xz[ibnd]
+        yp = yz[ibnd]
 
 
         # Make boolean array for points that are include in a polyline 
         used = np.full(xp.shape, False, dtype=bool)
 
         polylines = []
 
         while True:
 
             if np.all(used):
                 # All boundary grid points have been used. We can stop now.
                 break
 
             # Find first of the unused points
-            i1 = np.where(used==False)[0][0]
+            i1 = np.where(used == False)[0][0]
 
             # Set this point to used
             used[i1] = True
 
             polyline = [i1] 
 
             while True:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/cross_sections.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/cross_sections.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/grid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/input.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self.nmax = 0
         self.dx = 0.1
         self.dy = 0.1
         self.x0 = 0.0
         self.y0 = 0.0
         self.rotation = 0.0
         self.latitude = 0.0
+        self.qtrfile = None
         tnow = datetime.datetime.now().replace(
             hour=0, minute=0, second=0, microsecond=0
         )
         self.tref = tnow
         self.tstart = tnow
         self.tstop = tnow + datetime.timedelta(days=1)
         self.tspinup = 60.0
@@ -52,15 +53,15 @@
         self.baro = False
         self.pavbnd = 0.0
         self.gapres = 101200.0
         self.advlim = 9999.9
         self.stopdepth = 1000.0
         self.crsgeo = False
 
-        self.qtrfile = None
+        self.sbgfile = None
         self.depfile = None
         self.mskfile = None
         self.indexfile = None
         self.cstfile = None
         self.bndfile = None
         self.bzsfile = None
         self.bzifile = None
@@ -72,15 +73,14 @@
         self.bwdfile = None
         self.bdsfile = None
         self.bcafile = None
         self.corfile = None
         self.srcfile = None
         self.disfile = None
         self.inifile = None
-        self.sbgfile = None
         self.spwfile = None
         self.amufile = None
         self.amvfile = None
         self.ampfile = None
         self.amprfile = None
         self.wndfile = None
         self.precipfile = None
@@ -170,19 +170,19 @@
             if hasattr(self.variables, ""):
                 if type(getattr(self.variables, name)) == bool:
                     if val == 0:
                         val = False       
                     else:
                         val = True    
             setattr(self.variables, name, val)
-
-        if self.variables.qtrfile:
-            self.model.grid_type = "quadtree"
-        else:
-            self.model.grid_type = "regular"
+        
+        # if self.variables.qtrfile:
+        #     self.model.grid_type = "quadtree"
+        # else:
+        #     self.model.grid_type = "regular"
 
         if self.variables.sbgfile:
             self.model.bathy_type = "subgrid"
         else:
             self.model.bathy_type = "regular"
 
     def write(self):
@@ -192,15 +192,15 @@
         # Make some adjustments
         variables = copy.copy(self.variables)
 
         if self.model.crs.is_geographic:
             variables.crsgeo = 1
             variables.latitude = None
 
-        if self.model.grid_type == "quadtree":
+        if self.model.grid.type == "quadtree":
             # Get rid of grid stuff
             variables.x0               = None
             variables.y0               = None
             variables.dx               = None
             variables.dy               = None
             variables.nmax             = None
             variables.mmax             = None
@@ -233,20 +233,20 @@
             variables.manning              = None
             variables.manning_land         = None
             variables.manning_sea          = None
             variables.rgh_lev_land         = None
 
         fid = open(input_file, "w")
         for key, value in variables.__dict__.items():
-            if not value is None:
+            if value is not None:
                 if type(value) == "float":
                     string = f"{key.ljust(20)} = {float(value)}\n"
                 elif type(value) == "int":
                     string = f"{key.ljust(20)} = {int(value)}\n"
-                elif type(value) == bool:
+                elif isinstance(value, bool):
                     if value:
                         string = f"{key.ljust(20)} = {int(1)}\n"
                     else:    
                         string = f"{key.ljust(20)} = {int(0)}\n"
                 elif type(value) == list:
                     valstr = ""
                     for v in value:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/mask.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,26 +51,27 @@
         if not quiet:
             print("Building mask ...")
 
         mask = np.zeros(self.model.grid.nr_cells, dtype=np.int8)
         x, y = self.model.grid.face_coordinates()
         z    = self.model.grid.data["z"].values[:]
 
+        # Indices are 1-based in SFINCS so subtract 1 for python 0-based indexing
         mu    = self.model.grid.data["mu"].values[:]
-        mu1   = self.model.grid.data["mu1"].values[:]
-        mu2   = self.model.grid.data["mu2"].values[:]
+        mu1   = self.model.grid.data["mu1"].values[:] - 1
+        mu2   = self.model.grid.data["mu2"].values[:] - 1
         nu    = self.model.grid.data["nu"].values[:]
-        nu1   = self.model.grid.data["nu1"].values[:]
-        nu2   = self.model.grid.data["nu2"].values[:]
+        nu1   = self.model.grid.data["nu1"].values[:] - 1
+        nu2   = self.model.grid.data["nu2"].values[:] - 1
         md    = self.model.grid.data["md"].values[:]
-        md1   = self.model.grid.data["md1"].values[:]
-        md2   = self.model.grid.data["md2"].values[:]
+        md1   = self.model.grid.data["md1"].values[:] - 1
+        md2   = self.model.grid.data["md2"].values[:] - 1
         nd    = self.model.grid.data["nd"].values[:]
-        nd1   = self.model.grid.data["nd1"].values[:]
-        nd2   = self.model.grid.data["nd2"].values[:]
+        nd1   = self.model.grid.data["nd1"].values[:] - 1 
+        nd2   = self.model.grid.data["nd2"].values[:] - 1
 
         if zmin>=zmax:
             # Do not include any points initially
             if include_polygon is None:
                 print("WARNING: Entire mask set to zeros! Please ensure zmax is greater than zmin, or provide include polygon(s) !")
                 return
         else:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/observation_points.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/observation_points.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/point_sources.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/point_sources.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/quadtree_grid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/quadtree_grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/quadtree_grid_snapwave.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/quadtree_grid_snapwave.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/regular_grid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/regular_grid.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/sfincs.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/sfincs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import math
 from pyproj import CRS
 from pyproj import Transformer
 
 from .input import SfincsInput
 
 from .subgrid import SfincsSubgridTable
-from .grid import SfincsGrid
+from .grid_v2 import SfincsGrid
 from .mask import SfincsMask
 from .boundary_conditions import SfincsBoundaryConditions
 from .observation_points import SfincsObservationPoints
 from .cross_sections import SfincsCrossSections
 from .point_sources import SfincsPointSources
 from .thin_dams import SfincsThinDams
 from .weirs import SfincsWeirs
@@ -43,15 +43,15 @@
         self.exe_path                 = None
         self.path                     = root  
         self.input                    = SfincsInput(self)
         # if crs is an integer, assume it is an EPSG code
         if isinstance(crs, int):
             crs = CRS.from_epsg(crs)
         self.crs                      = crs
-        self.grid_type                = "regular"
+        # self.grid_type                = "regular"
         self.bathy_type               = "regular"
         self.grid                     = SfincsGrid(self)
         self.mask                     = SfincsMask(self)
         self.subgrid                  = SfincsSubgridTable(self)
         self.boundary_conditions      = SfincsBoundaryConditions(self)
         self.observation_points       = SfincsObservationPoints(self)
         self.wave_makers              = SfincsWaveMakers(self)
@@ -76,15 +76,20 @@
         self.input.write()
         self.write_attribute_files()
 
     def read_attribute_files(self):
         
         self.grid = SfincsGrid(self)
 
-        if self.grid_type == "regular":
+        if self.input.variables.qtrfile:
+            self.grid.type = "quadtree"
+        else:
+            self.grid.type = "regular"
+
+        if self.grid.type == "regular":
             self.grid.build(self.input.variables.x0,
                             self.input.variables.y0,
                             self.input.variables.nmax,
                             self.input.variables.mmax,
                             self.input.variables.dx,
                             self.input.variables.dy,
                             self.input.variables.rotation)
@@ -126,15 +131,15 @@
 
         # Wave makers
         self.wave_makers.read()
 
     def write_attribute_files(self):
         """Writes all attribute files"""
 
-        if self.grid_type == "regular":
+        if self.grid.type == "regular":
             self.mask.write()
         else:    
             self.grid.write()
 
         # Boundary conditions
         self.boundary_conditions.write()
         # Observation points
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/sfincs_builder.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/sfincs_builder.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/snapwave.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/snapwave.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/subgrid.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/subgrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,51 +44,55 @@
         # Write XArray dataset to netcdf file
         self.ds.to_netcdf(file_name)
         
     def build(self,
               bathymetry_sets,
               roughness_sets,
               manning_land=0.04,
-              manning_water=0.02,
+              manning_water=0.025,
               manning_level=1.0,
-              nr_bins=10,
+              nr_bins=None,
+              nr_levels=10,
               nr_subgrid_pixels=20,
               max_gradient=5.0,
               depth_factor=1.0,
               huthresh=0.01,
               zmin=-99999.0,
               file_name="sfincs.sbg",
               quiet=False,
               progress_bar=None):  
-        
+
+        if nr_bins:
+            nr_levels = nr_bins 
+
         grid = self.model.grid
         
         # Dimensions etc
-        nbins  = nr_bins
         refi   = nr_subgrid_pixels
         npc    = grid.nr_cells    
-        nlevs  = grid.nr_refinement_levels
-        cosrot = np.cos(grid.rotation*np.pi/180)
-        sinrot = np.sin(grid.rotation*np.pi/180)
+        nr_ref_levs = grid.data.attrs["nr_levels"] # number of refinement levels
+        cosrot = np.cos(grid.data.attrs["rotation"]*np.pi/180)
+        sinrot = np.sin(grid.data.attrs["rotation"]*np.pi/180)
         nrmax  = 2000
+        zminimum = zmin
 
         # Grid neighbors
-        level = grid.data["level"].values[:]
-        n   = grid.data["n"].values[:]
-        m   = grid.data["m"].values[:]
-        nu  = grid.data["nu"].values[:]
-        nu1 = grid.data["nu1"].values[:]
-        nu2 = grid.data["nu2"].values[:]
-        mu  = grid.data["mu"].values[:]
-        mu1 = grid.data["mu1"].values[:]
-        mu2 = grid.data["mu2"].values[:]
+        level = grid.data["level"].values[:] - 1
+        n     = grid.data["n"].values[:] - 1
+        m     = grid.data["m"].values[:] - 1
+        nu    = grid.data["nu"].values[:]
+        nu1   = grid.data["nu1"].values[:] - 1
+        nu2   = grid.data["nu2"].values[:] - 1
+        mu    = grid.data["mu"].values[:]
+        mu1   = grid.data["mu1"].values[:] - 1
+        mu2   = grid.data["mu2"].values[:] - 1
 
         # U/V points 
         # Need to count the number of uv points in order allocate arrays (probably better to store this in the grid)
-        if self.model.grid_type == "quadtree":   
+        if self.model.grid.type == "quadtree":   
             # For quadtree grids, all points are stored
             index_nu1 = np.zeros(npc, dtype=int)
             index_nu2 = np.zeros(npc, dtype=int)
             index_mu1 = np.zeros(npc, dtype=int)
             index_mu2 = np.zeros(npc, dtype=int)        
             index_nm  = np.zeros(grid.nr_cells, dtype=int)
             npuv = 0
@@ -137,62 +141,62 @@
                         if grid.data["mask"].values[nu2[ip]] > 0:
                             index_nu2[ip] = npuv
                             npuv += 1
 
         # Create xarray dataset with empty arrays
         self.ds = xr.Dataset()
         self.ds.attrs["version"] = self.version
-        self.ds["z_zmin"] = xr.DataArray(np.zeros(npc), dims=["cells"])
-        self.ds["z_zmax"] = xr.DataArray(np.zeros(npc), dims=["cells"])
-        self.ds["z_volmax"] = xr.DataArray(np.zeros(npc), dims=["cells"])
-        self.ds["z_level"] = xr.DataArray(np.zeros((npc, nbins)), dims=["cells", "bins"])
-        self.ds["uv_zmin"] = xr.DataArray(np.zeros(npuv), dims=["uv_points"])
-        self.ds["uv_zmax"] = xr.DataArray(np.zeros(npuv), dims=["uv_points"])
-        self.ds["uv_havg"] = xr.DataArray(np.zeros((npuv, nbins)), dims=["uv_points", "bins"])
-        self.ds["uv_nrep"] = xr.DataArray(np.zeros((npuv, nbins)), dims=["uv_points", "bins"])
-        self.ds["uv_pwet"] = xr.DataArray(np.zeros((npuv, nbins)), dims=["uv_points", "bins"])
-        self.ds["uv_ffit"] = xr.DataArray(np.zeros(npuv), dims=["uv_points"])
-        self.ds["uv_navg"] = xr.DataArray(np.zeros(npuv), dims=["uv_points"])
+        self.ds["z_zmin"] = xr.DataArray(np.zeros(npc), dims=["np"])
+        self.ds["z_zmax"] = xr.DataArray(np.zeros(npc), dims=["np"])
+        self.ds["z_volmax"] = xr.DataArray(np.zeros(npc), dims=["np"])
+        self.ds["z_level"] = xr.DataArray(np.zeros((npc, nr_levels)), dims=["np", "levels"])
+        self.ds["uv_zmin"] = xr.DataArray(np.zeros(npuv), dims=["npuv"])
+        self.ds["uv_zmax"] = xr.DataArray(np.zeros(npuv), dims=["npuv"])
+        self.ds["uv_havg"] = xr.DataArray(np.zeros((npuv, nr_levels)), dims=["npuv", "levels"])
+        self.ds["uv_nrep"] = xr.DataArray(np.zeros((npuv, nr_levels)), dims=["npuv", "levels"])
+        self.ds["uv_pwet"] = xr.DataArray(np.zeros((npuv, nr_levels)), dims=["npuv", "levels"])
+        self.ds["uv_ffit"] = xr.DataArray(np.zeros(npuv), dims=["npuv"])
+        self.ds["uv_navg"] = xr.DataArray(np.zeros(npuv), dims=["npuv"])
         
         # Determine first indices and number of cells per refinement level
-        ifirst = np.zeros(nlevs, dtype=int)
-        ilast  = np.zeros(nlevs, dtype=int)
-        nr_cells_per_level = np.zeros(nlevs, dtype=int)
+        ifirst = np.zeros(nr_ref_levs, dtype=int)
+        ilast  = np.zeros(nr_ref_levs, dtype=int)
+        nr_cells_per_level = np.zeros(nr_ref_levs, dtype=int)
         ireflast = -1
         for ic in range(npc):
             if level[ic]>ireflast:
                 ifirst[level[ic]] = ic
                 ireflast = level[ic]
-        for ilev in range(nlevs - 1):
+        for ilev in range(nr_ref_levs - 1):
             ilast[ilev] = ifirst[ilev + 1] - 1
-        ilast[nlevs - 1] = grid.nr_cells - 1
-        for ilev in range(nlevs):
+        ilast[nr_ref_levs - 1] = grid.nr_cells - 1
+        for ilev in range(nr_ref_levs):
             nr_cells_per_level[ilev] = ilast[ilev] - ifirst[ilev] + 1 
 
         # Loop through all levels
-        for ilev in range(nlevs):
+        for ilev in range(nr_ref_levs):
 
             if not quiet:
                 print("++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++")
-                print("Processing level " + str(ilev + 1) + " of " + str(nlevs) + " ...")
+                print("Processing level " + str(ilev + 1) + " of " + str(nr_ref_levs) + " ...")
             
             # Make blocks off cells in this level only
             cell_indices_in_level = np.arange(ifirst[ilev], ilast[ilev] + 1, dtype=int)
             nr_cells_in_level = np.size(cell_indices_in_level)
             
             if nr_cells_in_level == 0:
                 continue
 
             n0 = np.min(n[ifirst[ilev]:ilast[ilev] + 1])
             n1 = np.max(n[ifirst[ilev]:ilast[ilev] + 1]) # + 1 # add extra cell to compute u and v in the last row/column
             m0 = np.min(m[ifirst[ilev]:ilast[ilev] + 1])
             m1 = np.max(m[ifirst[ilev]:ilast[ilev] + 1]) # + 1 # add extra cell to compute u and v in the last row/column
             
-            dx   = grid.dx/2**ilev      # cell size
-            dy   = grid.dy/2**ilev      # cell size
+            dx   = grid.data.attrs["dx"]/2**ilev      # cell size
+            dy   = grid.data.attrs["dy"]/2**ilev      # cell size
             dxp  = dx/refi              # size of subgrid pixel
             dyp  = dy/refi              # size of subgrid pixel
             
             nrcb = int(np.floor(nrmax/refi))         # nr of regular cells in a block            
             nrbn = int(np.ceil((n1 - n0 + 1)/nrcb))  # nr of blocks in n direction
             nrbm = int(np.ceil((m1 - m0 + 1)/nrcb))  # nr of blocks in m direction
 
@@ -233,45 +237,51 @@
                     y00 = 0.5*dyp + bn0*refi*dyp
                     y01 = y00 + (bn1 - bn0 + 1)*refi*dyp
                     
                     x0 = np.arange(x00, x01, dxp)
                     y0 = np.arange(y00, y01, dyp)
                     xg0, yg0 = np.meshgrid(x0, y0)
                     # Rotate and translate
-                    xg = grid.x0 + cosrot*xg0 - sinrot*yg0
-                    yg = grid.y0 + sinrot*xg0 + cosrot*yg0                    
+                    xg = grid.data.attrs["x0"] + cosrot*xg0 - sinrot*yg0
+                    yg = grid.data.attrs["y0"] + sinrot*xg0 + cosrot*yg0                    
 
                     # Clear variables
                     del x0, y0, xg0, yg0
                     
                     # Get bathymetry on subgrid from bathymetry database
-                    zg = bathymetry_database.get_bathymetry_on_grid(xg, yg,
-                                                                    self.model.crs,
-                                                                    bathymetry_sets)
+                    try: 
+                        zg = bathymetry_database.get_bathymetry_on_grid(xg, yg,
+                                                                        self.model.crs,
+                                                                        bathymetry_sets)
+                    except:
+                        pass   
                     
                     # Multiply zg with depth factor (had to use 0.9746 to get arrival
                     # times right in the Pacific)
                     zg = zg*depth_factor
 
                     # Set minimum depth                    
-                    zg = np.maximum(zg, zmin)
+                    zg = np.maximum(zg, zminimum)
 
                     # Manning's n values
                     
                     # Initialize roughness of subgrid at NaN
                     manning_grid = np.full(np.shape(xg), np.nan)
 
                     if roughness_sets: # this still needs to be implemented
                         manning_grid = bathymetry_database.get_bathymetry_on_grid(xg, yg,
                                                                         self.model.crs,
                                                                         roughness_sets)
 
                     # Fill in remaining NaNs with default values
                     isn = np.where(np.isnan(manning_grid))
-                    manning_grid[(isn and np.where(zg<=manning_level))] = manning_water
+                    try:
+                        manning_grid[(isn and np.where(zg<=manning_level))] = manning_water
+                    except:
+                        pass
                     manning_grid[(isn and np.where(zg>manning_level))] = manning_land
                     
                     # Now compute subgrid properties
 
                     # First we loop through all the possible cells in this block
                     index_cells_in_block = np.zeros(nrcb*nrcb, dtype=int)
                     # Loop through all cells in this level
@@ -283,14 +293,17 @@
                             index_cells_in_block[nr_cells_in_block] = indx
                             nr_cells_in_block += 1
                     index_cells_in_block = index_cells_in_block[0:nr_cells_in_block]
 
                     if not quiet:
                         print("Number of active cells in block    : " + str(nr_cells_in_block))
 
+
+                    # Parallel from here
+
                     # Loop through all active cells in this block
                     for ic in range(nr_cells_in_block):
                         
                         indx = index_cells_in_block[ic]
 
                         # First the volumes in the cells
                         nn  = (n[indx] - bn0) * refi
@@ -305,15 +318,15 @@
                             dypm = dyp*111111.0
                         else:
                             dxpm = dxp
                             dypm = dyp
                         
                         zv  = zgc.flatten()   
                         zvmin = -20.0
-                        z, v, zmin, zmax, zmean = subgrid_v_table(zv, dxpm, dypm, nbins, zvmin, max_gradient)
+                        z, v, zmin, zmax, zmean = subgrid_v_table(zv, dxpm, dypm, nr_levels, zvmin, max_gradient)
 
                         # Check if this is an active point 
                         if index_nm[indx] > -1:
                             self.ds["z_zmin"][index_nm[indx]]    = zmin
                             self.ds["z_zmax"][index_nm[indx]]    = zmax
                             self.ds["z_volmax"][index_nm[indx]]  = v[-1]
                             self.ds["z_level"][index_nm[indx],:] = z
@@ -328,15 +341,15 @@
                                 zgu = np.transpose(zgu)
                                 zv  = zgu.flatten()
                                 manning = manning_grid[nn : nn + refi, mm : mm + refi]
                                 manning = np.transpose(manning)
                                 manning = manning.flatten()
                                 iuv = index_mu1[indx]
                                 if iuv>=0:
-                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nbins, huthresh)
+                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nr_levels, huthresh)
                                     self.ds["uv_zmin"][iuv]   = zmin
                                     self.ds["uv_zmax"][iuv]   = zmax
                                     self.ds["uv_havg"][iuv,:] = havg
                                     self.ds["uv_nrep"][iuv,:] = nrep
                                     self.ds["uv_pwet"][iuv,:] = pwet
                                     self.ds["uv_ffit"][iuv]   = ffit
                                     self.ds["uv_navg"][iuv]   = navg
@@ -348,15 +361,15 @@
                                 zgu = np.transpose(zgu)
                                 zv  = zgu.flatten()
                                 manning = manning_grid[nn : nn + int(refi/2), mm : mm + int(refi/2)]
                                 manning = np.transpose(manning)
                                 manning = manning.flatten()
                                 iuv = index_mu1[indx]
                                 if iuv>=0:
-                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nbins, huthresh)
+                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nr_levels, huthresh)
                                     self.ds["uv_zmin"][iuv]   = zmin
                                     self.ds["uv_zmax"][iuv]   = zmax
                                     self.ds["uv_havg"][iuv,:] = havg
                                     self.ds["uv_nrep"][iuv,:] = nrep
                                     self.ds["uv_pwet"][iuv,:] = pwet
                                     self.ds["uv_ffit"][iuv]   = ffit
                                     self.ds["uv_navg"][iuv]   = navg
@@ -367,15 +380,15 @@
                                 zgu = np.transpose(zgu)
                                 zv  = zgu.flatten()
                                 manning = manning_grid[nn : nn + int(refi/2), mm : mm + int(refi/2)]
                                 manning = np.transpose(manning)
                                 manning = manning.flatten()
                                 iuv = index_mu2[indx]
                                 if iuv>=0:
-                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nbins, huthresh)
+                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nr_levels, huthresh)
                                     self.ds["uv_zmin"][iuv]   = zmin
                                     self.ds["uv_zmax"][iuv]   = zmax
                                     self.ds["uv_havg"][iuv,:] = havg
                                     self.ds["uv_nrep"][iuv,:] = nrep
                                     self.ds["uv_pwet"][iuv,:] = pwet
                                     self.ds["uv_ffit"][iuv]   = ffit
                                     self.ds["uv_navg"][iuv]   = navg
@@ -387,15 +400,15 @@
                                 mm = (m[indx] - bm0)*refi
                                 zgu = zg[nn : nn + refi, mm : mm + refi]
                                 zv  = zgu.flatten()
                                 manning = manning_grid[nn : nn + refi, mm : mm + refi]
                                 manning = manning.flatten()
                                 iuv = index_nu1[indx]
                                 if iuv>=0:
-                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nbins, huthresh)
+                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nr_levels, huthresh)
                                     self.ds["uv_zmin"][iuv]   = zmin
                                     self.ds["uv_zmax"][iuv]   = zmax
                                     self.ds["uv_havg"][iuv,:] = havg
                                     self.ds["uv_nrep"][iuv,:] = nrep
                                     self.ds["uv_pwet"][iuv,:] = pwet
                                     self.ds["uv_ffit"][iuv]   = ffit
                                     self.ds["uv_navg"][iuv]   = navg
@@ -405,15 +418,15 @@
                                 mm = (m[indx] - bm0)*refi
                                 zgu = zg[nn : nn + int(refi/2), mm : mm + int(refi/2)]
                                 zv  = zgu.flatten()
                                 manning = manning_grid[nn : nn + int(refi/2), mm : mm + int(refi/2)]
                                 manning = manning.flatten()
                                 iuv = index_nu1[indx]
                                 if iuv>=0:
-                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nbins, huthresh)
+                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nr_levels, huthresh)
                                     self.ds["uv_zmin"][iuv]   = zmin
                                     self.ds["uv_zmax"][iuv]   = zmax
                                     self.ds["uv_havg"][iuv,:] = havg
                                     self.ds["uv_nrep"][iuv,:] = nrep
                                     self.ds["uv_pwet"][iuv,:] = pwet
                                     self.ds["uv_ffit"][iuv]   = ffit
                                     self.ds["uv_navg"][iuv]   = navg
@@ -422,15 +435,15 @@
                                 mm = (m[indx] - bm0)*refi + int(refi/2)
                                 zgu = zg[nn : nn + int(refi/2), mm : mm + int(refi/2)]
                                 zv  = zgu.flatten()
                                 manning = manning_grid[nn : nn + int(refi/2), mm : mm + int(refi/2)]
                                 manning = manning.flatten()
                                 iuv = index_nu2[indx]
                                 if iuv>=0:
-                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nbins, huthresh)
+                                    zmin, zmax, havg, nrep, pwet, ffit, navg, zz = subgrid_q_table(zv, manning, nr_levels, huthresh)
                                     self.ds["uv_zmin"][iuv]   = zmin
                                     self.ds["uv_zmax"][iuv]   = zmax
                                     self.ds["uv_havg"][iuv,:] = havg
                                     self.ds["uv_nrep"][iuv,:] = nrep
                                     self.ds["uv_pwet"][iuv,:] = pwet
                                     self.ds["uv_ffit"][iuv]   = ffit
                                     self.ds["uv_navg"][iuv]   = navg
@@ -465,20 +478,20 @@
         
 #         file = open(file_name, "rb")
         
 #         # File version        
 # #        self.version      = np.fromfile(file, dtype="i4", count=1)[0]
 #         self.nr_cells     = np.fromfile(file, dtype="i4", count=1)[0]
 #         self.nr_uv_points = np.fromfile(file, dtype="i4", count=1)[0]
-#         self.nbins        = np.fromfile(file, dtype="i4", count=1)[0]
+#         self.nlevels        = np.fromfile(file, dtype="i4", count=1)[0]
 #         self.z_zmin       = np.fromfile(file, dtype="f4", count=self.nr_cells)
 #         self.z_zmax       = np.fromfile(file, dtype="f4", count=self.nr_cells)
 #         self.z_zmean      = np.fromfile(file, dtype="f4", count=self.nr_cells)
 #         self.z_volmax     = np.fromfile(file, dtype="f4", count=self.nr_cells)
-#         self.z_depth      = np.zeros((self.nbins, self.nr_cells), dtype=float)
+#         self.z_depth      = np.zeros((self.nlevels, self.nr_cells), dtype=float)
 #         for ibin in range(self.nbins):
 #             self.z_depth[ibin,:] = np.fromfile(file, dtype="f4", count=self.nr_cells)
 #         self.uv_zmin      = np.fromfile(file, dtype="f4", count=self.nr_uv_points)
 #         self.uv_zmax      = np.fromfile(file, dtype="f4", count=self.nr_uv_points)
 #         self.uv_hrep      = np.zeros((self.nbins, self.nr_uv_points), dtype=float)
 #         for ibin in range(self.nbins):
 #             self.uv_hrep[ibin,:] = np.fromfile(file, dtype="f4", count=self.nr_uv_points)
@@ -857,15 +870,15 @@
 #             self.save(file_name, grid.mask)
 
 
 
 
 
 # @njit
-def subgrid_v_table(elevation, dx, dy, nbins, zvolmin, max_gradient):
+def subgrid_v_table(elevation, dx, dy, nlevels, zvolmin, max_gradient):
     """
     map vector of elevation values into a hypsometric volume - depth relationship for one grid cell
     Parameters
     ----------
     elevation : np.ndarray (nr of pixels in one cell) containing subgrid elevation values for one grid cell [m]
     dx: float, x-directional cell size (typically not known at this level) [m]
     dy: float, y-directional cell size (typically not known at this level) [m]
@@ -895,54 +908,54 @@
         
     depth = ele_sort - ele_sort.min()
 
     volume = np.cumsum((np.diff(depth) * dx * dy) * np.arange(len(depth))[1:])
     # add trailing zero for first value
     volume = np.concatenate([np.array([0]), volume])
     
-    # Resample volumes to discrete bins
-    steps = np.arange(nbins)/(nbins - 1)
+    # Resample volumes to discrete levels
+    steps = np.arange(nlevels)/(nlevels - 1)
     V = steps*volume.max()
-    dvol = volume.max()/(nbins - 1)
+    dvol = volume.max()/(nlevels - 1)
     z = interpolate.interp1d(volume, ele_sort)(V)
     dzdh = get_dzdh(z, V, a)
     n = 0
-    while ((dzdh.max() > max_gradient and not(np.isclose(dzdh.max(), max_gradient))) and n < nbins):
+    while ((dzdh.max() > max_gradient and not(np.isclose(dzdh.max(), max_gradient))) and n < nlevels):
         # reshape until gradient is satisfactory
         idx = np.where(dzdh == dzdh.max())[0]
         z[idx + 1] = z[idx] + max_gradient*(dvol/a)
         dzdh = get_dzdh(z, V, a)
         n += 1
     return z, V, elevation.min(), z.max(), ele_sort.mean()
 
-def subgrid_q_table(elevation, manning, nbins, huthresh):
+def subgrid_q_table(elevation, manning, nlevels, huthresh):
     """
     map vector of elevation values into a hypsometric hydraulic radius - depth relationship for one u/v point
     Parameters
     ----------
     elevation : np.ndarray (nr of pixels in one cell) containing subgrid elevation values for one grid cell [m]
     manning : np.ndarray (nr of pixels in one cell) containing subgrid manning roughness values for one grid cell [s m^(-1/3)]
-    nbins : int, number of vertical bins [-]
+    nlevels : int, number of vertical levels [-]
     huthresh : float, threshold depth [m]
     Returns
     -------
     zmin : float, minimum elevation [m]
     zmax : float, maximum elevation [m]
-    havg : np.ndarray (nbins) grid-average depth for vertical levels [m]
-    nrep : np.ndarray (nbins) representative roughness for vertical levels [m1/3/s] ?
-    pwet : np.ndarray (nbins) wet fraction for vertical levels [-] ?
+    havg : np.ndarray (nlevels) grid-average depth for vertical levels [m]
+    nrep : np.ndarray (nlevels) representative roughness for vertical levels [m1/3/s] ?
+    pwet : np.ndarray (nlevels) wet fraction for vertical levels [-] ?
     navg : float, grid-average Manning's n [m 1/3 / s]
     ffit : float, fitting coefficient [-]
-    zz   : np.ndarray (nbins) elevation of vertical levels [m]
+    zz   : np.ndarray (nlevels) elevation of vertical levels [m]
     """
 
-    havg = np.zeros(nbins)
-    nrep = np.zeros(nbins)
-    pwet = np.zeros(nbins)
-    zz   = np.zeros(nbins)
+    havg = np.zeros(nlevels)
+    nrep = np.zeros(nlevels)
+    pwet = np.zeros(nlevels)
+    zz   = np.zeros(nlevels)
 
     n   = int(np.size(elevation)) # Nr of pixels in grid cell
     n05 = int(n/2)
 
     dd_a      = elevation[0:n05]
     dd_b      = elevation[n05:]
     manning_a = manning[0:n05]
@@ -959,21 +972,21 @@
     zmax = max(zmax_a, zmax_b)
     
     # Make sure zmax is a bit higher than zmin
     if zmax<zmin + 0.001:
        zmax = max(zmax, zmin + 0.001)
 
     # Determine bin size
-    dbin = (zmax - zmin)/(nbins - 1)
+    dbin = (zmax - zmin)/(nlevels - 1)
 
     # Grid mean roughness
     navg = np.mean(manning)
      
-    # Loop through bins
-    for ibin in range(nbins):
+    # Loop through levels
+    for ibin in range(nlevels):
 
         # Top of bin
         zbin = zmin + ibin * dbin
         zz[ibin] = zbin
         
         # ibelow = np.where(elevation<=zbin)                           # index of pixels below bin level
         h      = np.maximum(zbin - elevation, 0.0)    # water depth in each pixel
@@ -994,39 +1007,34 @@
         
         q_ab   = np.minimum(q_a, q_b)
 
         q_all = h**(5.0/3.0)/manning               # Determine 'flux' for each pixel
         q_all = np.mean(q_all)                    # Wet-average flux through all the pixels
         
         # Weighted average of q_ab and q_all
-        w = (ibin) / (nbins - 1)
+        w = (ibin) / (nlevels - 1)
         q = (1.0 - w) * q_ab + w * q_all
 
         nrep[ibin] = hmean**(5.0/3.0) / q  # Representative n for qmean and hmean
 
-        # if ibin == nbins - 1:
+        # if ibin == nlevels - 1:
         #     nrep_top = hmean**(5.0/3.0) / q
         #     hmean_top = hmean
 
     nrep_top = nrep[-1]    
     havg_top = havg[-1]
 
     ### Fitting for nrep above zmax
 
     # Determine nfit at zfit
     zfit  = zmax + zmax - zmin
     h     = np.maximum(zfit - elevation, 0.0)      # water depth in each pixel
     hfit  = havg_top + zmax - zmin                 # mean water depth in cell as computed in SFINCS (assuming linear relation between water level and water depth above zmax)
     q     = h**(5.0/3.0)/manning                   # unit discharge in each pixel
     qmean = np.mean(q)                             # combined unit discharge for cell
-    if qmean<1.0e-10:
-        shite=1
-    if hfit<0.0:
-        shite=2    
-        
 
     nfit  = hfit**(5.0/3.0) / qmean
     
     # Actually apply fit on gn2 (this is what is used in sfincs)
     gnavg2 = 9.81 * navg**2
     gnavg_top2 = 9.81 * nrep_top**2
 
@@ -1042,11 +1050,9 @@
         else:
             if nfit < navg:
                 nfit = nrep_top + 0.9*(navg - nrep_top)
             if nfit > nrep_top:
                 nfit = nrep_top + 0.1*(navg - nrep_top)
         gnfit2 = 9.81 * nfit**2
         ffit = (((gnavg2 - gnavg_top2) / (gnavg2 - gnfit2)) - 1) / (zfit - zmax)
-        if ffit<0.0:
-            shite=1
          
     return zmin, zmax, havg, nrep, pwet, ffit, navg, zz
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/thin_dams.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/thin_dams.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/wave_makers.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/wave_makers.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/sfincs2/weirs.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/sfincs2/weirs.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/snapwave/mesh.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/snapwave/mesh.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/astro.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/astro.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/constituent.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/constituent.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/fes2014.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/fes2014.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/nodal_corrections.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/nodal_corrections.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/predict.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/predict.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/test_tide_database.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/test_tide_database.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/tide.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/tide.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/tide_model.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/tide_model.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tide/tide_predict.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tide/tide_predict.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tiling/tiling.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tiling/tiling.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/cyclone_track_database.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/cyclone_track_database.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_forecasting.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_meteo.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_meteo.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/test_track_reading.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/test_track_reading.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/tropical_cyclone/tropical_cyclone.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/tropical_cyclone/tropical_cyclone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1882,14 +1882,44 @@
         with fiona.open(filename, "w", "ESRI Shapefile", schema) as c:
             counter = 0
             for linestring in multilinestring.geoms:
                 # Write the linestring to the shapefile
                 c.write({'geometry': mapping(linestring), 'properties': {'id': counter}})
                 counter += 1
 
+    # Write out geojson
+    def to_geojson(self, filename=None, text="var track_ensemble ="):
+        import cht.misc.misc_tools
+
+        # Make path (if needed)
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+
+        # Get the tracks in line format
+        lines = []
+        ids = []
+        for nn, member in enumerate(self.members):
+            coordinates = []
+            for it in range(len(member.track)):
+                coordinates.append(
+                    (member.track.geometry[it].x, member.track.geometry[it].y)
+                )
+            line = LineString(coordinates)
+            lines.append(line)
+            ids.append(member.name)
+        multilinestring = MultiLineString(lines)
+
+        # Write multilinestring to geojson
+        features = []
+        features.append(Feature(geometry=multilinestring))
+        feature_collection = FeatureCollection(features)
+
+        cht.misc.misc_tools.write_json_js(filename, feature_collection, text)
+
+        return feature_collection
+
     # Write them out to a spiderweb
     def to_spiderweb(self, folder_path, format_type='ascii'):
         # Make path (if needed)
         os.makedirs(folder_path, exist_ok=True)
 
         # Loop over ensemble members and write them out
         for member in self.members:
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/watersheds/watersheds.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/watersheds/watersheds.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/xbeach/xbeach.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/xbeach/xbeach.py`

 * *Files identical despite different names*

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/cht/xbeach/xbeach_output_morphology.py` & `deltares_coastalhazardstoolkit-0.2.7/src/cht/xbeach/xbeach_output_morphology.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,14 @@
             self.MHW = max(wls)
             self.MLW = min(wls)
         else:
             self.MHW = 0
             self.MLW = 0
         if 'id' in kwargs:
             self.id = str(kwargs.get('id'))
-            
 
         self.x = x
         self.z = z
         self.zend = zbend
         
         if win:  # if window for smoothing is provided apply smoothing (should be mutliple of dx)
             if smoothing == 'moving_average':
@@ -76,15 +75,15 @@
             x0, ind = x0[-1], ind[-1]  # get last one in case there are more
         if norm:
             self.offset = self.x[ind] 
             self.x = self.x - self.offset
         self.x_shoreline = self.x[ind]  # get grid value (not interpolated)
         
 
-    def dune_crest(self, zmin=6, prom_l=0.1, prom_r=3, width=1, fr_x_min=None, fr_x_max=None, **kwargs):
+    def dune_crest(self, zmin=6, prom_l=1, prom_r=1, width=1, fr_x_min=None, fr_x_max=None, **kwargs):
         """
         Find cross-shore location of max dune crest and foredune
 
         -Input-:
         zmin (float)        -> for foredune keep peaks that have an elevation larger than this value
         prom_l(r) (float)   -> for foredune find peaks with a prominences of at least this value (left and right)
         width (float)       -> for foredune find peaks with a width of at least this value
@@ -95,56 +94,60 @@
         x_dc_max (float)       -> cross-shore location of max-dune crest
         """
 
         ind_shor = np.argwhere(self.x == self.x_shoreline)[0][0]  # find index of shoreline
 
         # find location of maximum dune crest across the profile
         try:
-            self.x_dc_max = self.x[np.argmax(self.z)]
+            x_dc_max = self.x[np.argmax(self.z)]
+            x_dc_max_post = self.x[np.argmax(self.zend)]
         except:
-            self.x_dc_max = np.nan
+            x_dc_max = np.nan
+            x_dc_max_post = np.nan
 
         # find most seaward (1st dune row) fore-dune location (use height/width filtering)
         try:
             peaks, properties = signal.find_peaks(self.z[0:ind_shor],
                                                   width=int(np.round(width / (self.x[1] - self.x[0]))))
-            filt1 = list(np.where(self.x[0:ind_shor][properties['right_bases'][:-1]] > self.x[0:ind_shor][peaks[1:]]))[0]
-            filt2 = list(np.where(self.x[0:ind_shor][properties['left_bases'][1:]] < self.x[0:ind_shor][peaks[:-1]]))[0]
-            properties['right_bases'][filt1] = properties['left_bases'][filt1 + 1]
-            properties['left_bases'][filt2+1] = properties['right_bases'][filt2]
-            promin_l = self.z[0:ind_shor][peaks] - self.z[0:ind_shor][properties['left_bases']]
-            promin_r = self.z[0:ind_shor][peaks] - self.z[0:ind_shor][properties['right_bases']]
             
-            mask = (self.z[peaks] > zmin) & (promin_l > prom_l) & (promin_r > prom_r)
-            #peaks = peaks[mask]  # filter for minimum elevation and prominence if given # EQ: test with just picking the peak closest to the shoreline
             if fr_x_min is not None:
                 peaks = peaks[(self.x[peaks] < self.x_shoreline+fr_x_min) & (self.x[peaks] > self.x_shoreline-fr_x_max)]  # filter for cross-shore location
-            if 'max_prom_r' in kwargs:
-                promin_r = promin_r[mask]
-                self.x_dc_fr = self.x[peaks[promin_r == np.nanmax(promin_r)]][0]
-            else:
-                #self.x_dc_fr = self.x[peaks[-1]] # A) first peak landward of shoreline
-                maxpeakid = np.where(self.z[peaks] == np.amax(self.z[peaks]))
-                self.x_dc_fr = self.x[peaks[maxpeakid]] # B) highest peak landward of shoreline (within fr_x_min)
+           
+            maxpeakid = np.where(self.z[peaks] == np.amax(self.z[peaks]))
+            self.x_dc_fr = self.x[peaks[maxpeakid]] # B) highest peak landward of shoreline (within fr_x_min)
         except:
-            self.x_dc_fr = np.nan
+            self.x_dc_fr = self.x[0]#np.nan
 
-        self.z_dc_max = self.z[self.x == self.x_dc_max][0]
+        # now same for post-storm profile: find most seaward (1st dune row) fore-dune location
+        try:
+            peakspost, properties = signal.find_peaks(self.zend[0:ind_shor],
+                                                  width=int(np.round(width / (self.x[1] - self.x[0]))))
+            
+            if fr_x_min is not None:
+                peakspost = peakspost[(self.x[peakspost] < self.x_shoreline+fr_x_min) & (self.x[peakspost] > self.x_shoreline-fr_x_max)]  # filter for cross-shore location
+            
+            #self.x_dc_fr = self.x[peaks[-1]] # A) first peak landward of shoreline
+            maxpeakidpost = np.where(self.zend[peakspost] == np.amax(self.zend[peakspost]))
+            self.x_dc_fr_post = self.x[peakspost[maxpeakidpost]] # B) highest peak landward of shoreline (within fr_x_min)
+        except:
+            self.x_dc_fr_post = self.x[0]#np.nan
+
+
+        self.z_dc_max = self.z[self.x == x_dc_max][0]
         self.z_dc_fr = self.z[self.x == self.x_dc_fr][0]
+        self.x_dc_max = x_dc_max
+
+        self.z_dc_fr_post = self.zend[self.x == self.x_dc_fr_post][0]
+        self.x_dc_max_post = x_dc_max_post
+        #return x_dc_max, self.x_dc_fr
 
-        return self.x_dc_max, self.x_dc_fr
-    
-    
-    
-    
     def dune_vol(self):
         """Function to the dune volume (between dune crest and shoreline in m^2/m)"""
         pass
         
-        
     def plot(self, ax=None, plot_show=False, **kwargs):
         """
         Plot profile
 
         kwargs:
         'water_levels' --> ndarray, [MHW,MLW]
         'plot_dir'     --> path
@@ -161,18 +164,19 @@
             ax.set_xlim(kwargs.get('xlim'))
         if 'ylim' in kwargs:
             ax.set_ylim(kwargs.get('ylim'))
         if 'water_levels' in kwargs:
             wl = kwargs.get('water_levels')
             #ax.plot(self.x, np.repeat(wl[0], len(self.z)), 'k-', linewidth=0.4, zorder=-2)
             #ax.plot(self.x, np.repeat(wl[1], len(self.z)), 'k-', linewidth=0.4, zorder=-2)
-            ax.fill_between(self.x, np.repeat(self.MHW, len(self.z)), np.nanmin(self.z), color='#a8d7ed', zorder=-2)
-        ax.fill_between(self.x, self.z, np.nanmin(self.z), color='#e8cea9', zorder=-1)
-        ax.plot(self.x, self.zend, 'k--', linewidth=0.8, zorder=1, label='Post-storm bed level')
-        ax.plot(self.x, self.zsmax, 'b--', linewidth=0.8, zorder=1, label='max zs-max')
+            ax.fill_between(self.x, np.repeat(self.MHW, len(self.z)), np.nanmin(self.z), color='#a8d7ed', zorder=-3)
+        ax.fill_between(self.x, self.z, np.nanmin(self.z), color='#e8cea9', zorder=-2, label='Pre-storm bed level')
+        ax.fill_between(self.x, self.zend, np.nanmin(self.zend), color='#c98c36', zorder=-1, alpha=0.5, label='Post-storm bed level')
+        #ax.plot(self.x, self.zend, 'k--', linewidth=0.8, zorder=1, label='Post-storm bed level')
+        ax.plot(self.x, self.zsmax, 'b--', linewidth=0.8, zorder=0, label='max zs-max')
         ax.plot(self.x, self.zsmean, 'b-', linewidth=0.8, zorder=0, label='max zs-mean')
         # ax.grid(linewidth=0.4, color='k', linestyle='--', alpha=0.5, zorder=0)
         if  hasattr(self, 'x_dc_fr') and ~np.isnan(self.x_dc_fr):
             ax.scatter(self.x_dc_fr, self.z_dc_fr, s=25, marker=CARETDOWN,
                        linewidths=0.2, facecolor='k', zorder=2,
                        label='Foredune crest', clip_on=False)
         
@@ -180,29 +184,29 @@
             ax.scatter(self.x_dt, self.z_dt, s=20, marker="o", edgecolors='k',
                        linewidths=0.2, facecolor='r', zorder=2, label='Dune toe')
         if hasattr(self, 'x_shoreline') and~np.isnan(self.x_shoreline):
             ax.scatter(self.x_shoreline, self.MHW, s=10, marker="s", edgecolors='k',
                        linewidths=0.2, facecolor='r', zorder=2, label='Shoreline')
         if hasattr(self, 'regimeno'):
             ax.scatter(self.x_dc_fr, self.z_dc_fr_zbend, s=25, marker=CARETDOWN,
-                       linewidths=0.2, facecolor=None, zorder=2,
-                       label='regime = {:.0f}'.format(self.regimeno), clip_on=False)
+                       linewidths=0.2, facecolor='#666666', zorder=2,
+                       label=self.regimena, clip_on=False) # 'regime = {:.0f}'.format(self.regimeno)
+        if hasattr(self, 'erosionregimeno'):
+            ax.scatter(self.x_dc_fr_post, self.z_dc_fr_post, s=25, marker=CARETDOWN,
+                       linewidths=0.2, facecolor='#009900', zorder=2,
+                       label=self.erosionregimena, clip_on=False)
         ax.legend(loc=0, prop={'size': 8})
 
         if plot_show:
-            plt.show()
+            plt.show(block=False)
         if 'plot_dir' in kwargs:
             plot_dir = kwargs.get('plot_dir')
-            plt.savefig(os.path.join(plot_dir, f'profile_{self.id}.png'), dpi=100, bbox_inches='tight')
+            plt.savefig(os.path.join(plot_dir, f'profile_{self.id}.png'), dpi=200, bbox_inches='tight')
             plt.close()
             
-   
-            
-            
-            
     def sallenger_regimes(self, zsmean, zsmax, eps=0.005):
         """
         determine sallenger regimes for each profile
        
         -Input-:
         zmean (float)   -> mean zs output from XBeach over time for the profile, [time,crossshore(nx)]
         zsmax (float)   -> max zs output from XBeach over time for the profile, [time,crossshore(nx)]
@@ -215,42 +219,78 @@
         zsmean = np.nanmax(zsmean,axis=0)
         zsmax = np.nanmax(zsmax,axis=0)
     
         ind_crest = np.argwhere(self.x == self.x_dc_fr)[0][0]  # find index of dune crest
 
         if zsmean[ind_crest] > self.MHW: #collision
             regimeno = 1
+            regimena = 'collision'
         if zsmax[ind_crest]-eps > self.zend[ind_crest]: #overwash
             regimeno = 2
+            regimena = 'overwash'
         if zsmean[ind_crest]-eps > self.zend[ind_crest]: #inundation
             regimeno = 3
+            regimena = 'inundation'
         if self.zend[ind_crest] < self.MHW: #breach
             regimeno = 4
+            regimena = 'breaching'
    
         
         self.z_dc_fr_zbend = self.zend[ind_crest]
         self.zsmax = zsmax
         self.zsmean = zsmean
         self.regimeno = regimeno
+        self.regimena = regimena
     
-        return regimeno, ind_crest
-    
+        return regimeno, regimena, ind_crest
     
+    def erosion_regimes(self):
+        """
+        determine erosion regimes for each profile
+       
+        -Input-:
+        
+        -Output-:
+        erosionregimeno (float) -> erosion regime number 1 = minor erosion, 2 = beach/dune face erosion, 3 = dune retreat, 4 = breach
+        maxeroid {float}        -> index of point where dune/beach erosion is starting    
+        """
+
     
-    def euclidean_distance(x1, y1, x2, y2):
-        return np.sqrt((x2 - x1)**2 + (y2 - y1)**2)
+        ind_shor = np.argwhere(self.x == self.x_shoreline)[0][0]  # find index of shoreline
+        ind_crest = np.argwhere(self.x == self.x_dc_fr)[0][0]  # find index of dune crest pre-storm
+        ind_crest_post = np.argwhere(self.x == self.x_dc_fr_post)[0][0]  # find index of dune crest post-storm
+        
+        # find most landward point where we find erosion, starting from the shoreline point
+        dz = self.z - self.zend
+        maxeroid = next((index for index, value in enumerate(reversed(dz[0:ind_shor])) if value <= 0), None) #not 0 bed level change, but use a treshhold of ~5cm
+        maxeroid = ind_shor - 1 - maxeroid
+
+
+        if maxeroid is None: 
+            erosionregimeno, erosionregimena = 1, 'minor erosion'
+        elif (ind_crest_post == ind_crest) and (self.z[ind_crest] == self.zend[ind_crest_post]): 
+            erosionregimeno, erosionregimena = 2, 'beach/dune face erosion'
+        elif (ind_crest_post != ind_crest) and (self.zend[ind_crest] > self.MHW): 
+           erosionregimeno, erosionregimena = 3, 'dune retreat'
+        elif self.zend[ind_crest] < self.MHW: 
+            erosionregimeno, erosionregimena = 4, 'breaching'
+   
+        
+        self.erosionregimeno = erosionregimeno
+        self.erosionregimena = erosionregimena
+        self.maxeroid = maxeroid
     
+        return erosionregimeno, erosionregimena, maxeroid
+ 
     
 class Map:
 
     def __init__(self, x2D, y2D, zb02D, zbend2D, plot_dir):
         """
-        Class for the 2-d beach map output
-        
-        
+        Class for the 2-d beach map output from XBeach        
         """
         self.x = x2D
         self.y = y2D
         self.zend = zbend2D
         self.z0 = zb02D
         self.plot_dir = plot_dir
         
@@ -261,60 +301,61 @@
         -Input-:
             plot_dir    -> provide path to save the figure
         
         -Output-:
 
         """
         
-        cmap = np.loadtxt(r'p:\11206085-onr-fhics\03_cosmos\configurations\GMT_globe.txt')
+        cmap = np.loadtxt(os.path.abspath('..//misc//GMT_globe.txt'))
         cmap = cmap/255
         newcmp = ListedColormap(cmap, name='test')
         
         
         fig = plt.figure(figsize=(20, 10))
         gs = fig.add_gridspec(1, 3, hspace=0, wspace=0)
         ax = gs.subplots(sharey=True)
 
         for ii in range(1,4):
             if ii == 1:
                 var = self.z0
                 cmap=newcmp
-                climv = 10
+                climv = 20
                 cblabel = 'bed level [m to NAVD88]'
                 titlab = 'pre-storm bed level'
             if ii == 2:
                 var = self.zend
                 cmap=newcmp
-                climv = 10
+                climv = 20
                 cblabel = 'bed level [m to NAVD88]'
                 titlab = 'post-storm bed level'
             if ii == 3:
                 var = self.zend - self.z0
                 cmap='RdBu'
-                climv = 3
+                climv = 2
                 cblabel = 'sed-ero [m]'
-                titlab = 'sedimetation-erosion (post-pre)'
+                titlab = 'sedimentation-erosion (post-pre)'
                 
             plt.subplot(1, 3, ii)
             plt.pcolor(self.x,self.y,var, cmap=cmap, vmin=-climv, vmax=climv)
             plt.colorbar(label=cblabel, location='bottom')
-            plt.contour(self.x,self.y,self.z0,levels=[0], colors='gray', linewidths=0.3)
+            plt.contour(self.x,self.y,self.z0,levels=[0], colors='black', linewidths=0.3)
             plt.title(titlab)
             plt.axis('equal')
             if 'axis' in kwargs:
                 axis = kwargs.get('axis')
                 plt.axis([axis])
         #for axi in fig.get_axes():
          #   axi.label_outer()
-        plt.show()
+
+
+        plt.show(block=False)
         if 'plot_dir' in kwargs:
             plot_dir = kwargs.get('plot_dir')
-            fig.savefig(os.path.join(plot_dir, 'map_modeled_bedlevels'), dpi=300, bbox_inches='tight')
-
-        
+            fig.savefig(os.path.join(plot_dir, 'map_modeled_bedlevels'), dpi=500, bbox_inches='tight')
+  
     def plot_sallengerregimes(self, **kwargs):
         
         """
         plot sallenger regimes for each alongshore transect on a 2D XBeach model input bathy map
        
         -Input-:
             plot_dir    -> provide path to save the figure
@@ -325,15 +366,15 @@
         
         cmap = np.loadtxt(r'p:\11206085-onr-fhics\03_cosmos\configurations\GMT_globe.txt')
         cmap = cmap/255
         newcmp = ListedColormap(cmap, name='test')
         
         figure, ax = plt.subplots(1, 1)
 
-        plt.pcolor(self.x,self.y,self.zend, cmap=newcmp, vmin=-10, vmax=10)
+        plt.pcolor(self.x,self.y,self.zend, cmap=newcmp, vmin=-20, vmax=20)
         plt.colorbar(label='bed level [m to NAVD88]')
         
         df = pd.DataFrame({'x': self.x_crest,
                    'y': self.y_crest,
                    'regime': self.regimenos,
                    'regimename': self.regimename})
         groups = df.groupby('regimename')
@@ -345,19 +386,63 @@
         plt.xlabel('x [m]')
         plt.ylabel('y [m]')
         
         plt.axis('equal')            
         # plt.axis([df['x'].min(), df['x'].max(), df['y'].min(), df['y'].max()])
         plt.ylim([df['y'].min(), df['y'].max()])
         # plt.xlim([df['x'].min(), df['x'].max()])
-        plt.show()
+        plt.show(block=False)
         
         if 'plot_dir' in kwargs:
             plot_dir = kwargs.get('plot_dir')
-            figure.savefig(os.path.join(plot_dir, 'map_regimes'), dpi=300, bbox_inches='tight')
+            figure.savefig(os.path.join(plot_dir, 'map_regimes'), dpi=500, bbox_inches='tight')
+
+    def plot_erosionregimes(self, **kwargs):
+        
+        """
+        plot erosion regimes for each alongshore transect on a 2D XBeach model input bathy map
+       
+        -Input-:
+            plot_dir    -> provide path to save the figure
+        
+        -Output-:
+
+        """
+        
+        cmap = np.loadtxt(r'p:\11206085-onr-fhics\03_cosmos\configurations\GMT_globe.txt')
+        cmap = cmap/255
+        newcmp = ListedColormap(cmap, name='test')
+        
+        figure, ax = plt.subplots(1, 1)
+
+        plt.pcolor(self.x,self.y,self.zend, cmap=newcmp, vmin=-20, vmax=20)
+        plt.colorbar(label='bed level [m to NAVD88]')
+        
+        df = pd.DataFrame({'x': self.x_crest,
+                   'y': self.y_crest,
+                   'regime': self.erosionregimenos,
+                   'regimename': self.erosionregimename})
+        groups = df.groupby('regimename')
+        regimecolors = {'minor erosion': 'green', 'beach/dune face erosion': 'yellow', 'dune retreat': 'orange', 'breaching': 'red'}
+        for reg, dffs in groups:
+            plt.scatter(dffs.x, dffs.y, s=3, label=reg, facecolor=regimecolors[reg], edgecolors='k', linewidths=0.1)
+        plt.legend(loc=0, title="Erosion regime")
+    
+        plt.xlabel('x [m]')
+        plt.ylabel('y [m]')
+        
+        plt.axis('equal')            
+        # plt.axis([df['x'].min(), df['x'].max(), df['y'].min(), df['y'].max()])
+        plt.ylim([df['y'].min(), df['y'].max()])
+        # plt.xlim([df['x'].min(), df['x'].max()])
+        plt.show(block=False)
+        
+        if 'plot_dir' in kwargs:
+            plot_dir = kwargs.get('plot_dir')
+            figure.savefig(os.path.join(plot_dir, 'map_erosionregimes'), dpi=500, bbox_inches='tight')
     
     def alongshore_sallenger_regimes(self, zsmean, zsmax, MHW=0, plot_transects=False, plot_map=False):
         """
         get sallenger regimes for each alongshore transect in a 2D XBeach model
         this uses Profile.sallanger_regimes to calculate the regime per profile
        
         -Input-:
@@ -371,69 +456,83 @@
         y_crest ((list)) -> y-coordinate of the dune crest used to calculate regime, in coord-system as used by XBeach model
         """
         
         regimenos = []
         x_crest = []
         y_crest = []
         regimename = []
+        erosionregimenos = []
+        erosionregimename = []
 
         for idy in range(0, self.x.shape[0]):                            
             
-            distance = Profile.euclidean_distance(self.x[idy,-1], self.y[idy,-1], self.x[idy,:], self.y[idy,:])
-            
-            # we have to flip the profiles, since beachpy defines profiles land --> ocean
-            # isn't there a better way to do this?
-            distance_fl = np.flip(distance)
-            zb0_fl = np.flip(self.z0[idy,:])
-            zbend_fl = np.flip(self.zend[idy,:])
-            zsmax_fl = np.flip(zsmax[:,idy,:])
-            zsmean_fl = np.flip(zsmean[:,idy,:])
-            
-            # Create profile object using beachpy
-            profile = Profile(x=distance_fl, z=zb0_fl, zbend=zbend_fl ,ref='MHW', wls=[0.0, MHW], dx=2, id=idy)
-            # Get dune crests (foredune and maximum) 
-            x_dc_max, x_dc_fr = profile.dune_crest(zmin=MHW,fr_x_max=200,fr_x_min=2)    
-            # Get sallenger regimes 
-            regimeno, ind_crest  = profile.sallenger_regimes(zsmean_fl, zsmax_fl)
-            regimenos.append(regimeno)
-            
-            if regimeno == 1:
-                regimename.append('collision')
-            if regimeno == 2:
-                regimename.append('overwash')
-            if regimeno == 3:
-                regimename.append('inundation')
-            if regimeno == 4:
-                regimename.append('breaching')
+            try:
+                distance = euclidean_distance(self.x[idy,-1], self.y[idy,-1], self.x[idy,:], self.y[idy,:])
+                
+                # we have to flip the profiles, since beachpy defines profiles land --> ocean
+                distance_fl = np.flip(distance)
+                zb0_fl = np.flip(self.z0[idy,:])
+                zbend_fl = np.flip(self.zend[idy,:])
+                zsmax_fl = np.flip(zsmax[:,idy,:])
+                zsmean_fl = np.flip(zsmean[:,idy,:])
+                
+                # Create profile object using beachpy
+                profile = Profile(x=distance_fl, z=zb0_fl, zbend=zbend_fl ,ref='MHW', wls=[0.0, MHW], dx=2, id=idy)
+                # Get dune crests (foredune and maximum, both pre- and post-storm) 
+                profile.dune_crest(zmin=MHW,fr_x_min=150,fr_x_max=300)    
                 
-            # keep in mind that we flipped the profiles first, so need to flip back to get coordinates!!
-            ind_crestxy = self.x.shape[1] - ind_crest
-            x_crest.append(self.x[idy,ind_crestxy]) 
-            y_crest.append(self.y[idy,ind_crestxy])
-
-            if plot_transects:
-                # plot only a couple of transects 
-                if idy in range(0, self.x.shape[0], 20):
-                    profile.plot(xlim=[x_dc_fr-400, x_dc_fr+400],ylim=[-3, np.nanmax(zb0_fl)+1], water_levels=[0.0, 0.5], plot_dir=self.plot_dir, plot_show=True)
+                # Get sallenger regimes 
+                try:
+                    regimeno, regimena, ind_crest = profile.sallenger_regimes(zsmean_fl, zsmax_fl)
+                except:
+                    regimeno, regimena = 5, 'unknown'
+                regimenos.append(regimeno)
+                regimename.append(regimena)
+                
+                # get erosion regimes
+                try:
+                    erosionregimeno, erosionregimena, maxeroid = profile.erosion_regimes()
+                except:
+                    erosionregimeno, erosionregimena = 5, 'unknown'
+                erosionregimenos.append(erosionregimeno)
+                erosionregimename.append(erosionregimena)
+                        
                     
+                # keep in mind that we flipped the profiles first, so need to flip back to get coordinates!!
+                ind_crestxy = self.x.shape[1] - ind_crest - 1
+                x_crest.append(self.x[idy,ind_crestxy]) 
+                y_crest.append(self.y[idy,ind_crestxy])
+
+                if plot_transects:
+                    # plot only a couple of transects 
+                    if idy in range(0, self.x.shape[0], 15):
+                        profile.plot(xlim=[profile.x_dc_fr-100, profile.x_dc_fr+200],ylim=[-5, np.nanmax(zb0_fl)+1], water_levels=[0.0, 0.5], plot_dir=self.plot_dir, plot_show=True)
+            except Exception as e:
+                print(str(e))                
+
         self.x_crest = x_crest
         self.y_crest = y_crest
         self.regimenos = regimenos
         self.regimename = regimename
+        self.erosionregimenos = erosionregimenos
+        self.erosionregimename = erosionregimename
         
         if plot_map:
             Map.plot_sallengerregimes(self, plot_dir=self.plot_dir)
+            Map.plot_erosionregimes(self, plot_dir=self.plot_dir)
         
         # return values, or save as a csv?
 
-        return x_crest, y_crest, regimenos
+        return x_crest, y_crest, regimenos, erosionregimenos
 
 
+# EXTRA FUNCTIONS
+def euclidean_distance(x1, y1, x2, y2):
+    return np.sqrt((x2 - x1)**2 + (y2 - y1)**2)
 
-""" extra functions """
 def interp_nan(x_or, z_or, dx):
     """
     interpolates on a new x grid defined by the x of the first and last non-nan element in z_or
 
     -Inputs-:
     x_or (ndarray)  --> original cross-shore locations
     z_or (ndarray)  --> original elevations of x_or points
@@ -447,15 +546,14 @@
     x_or, z_or = x_or[nonnan], z_or[nonnan]
     # x_or = abs(x_or - x_or[0])
     x = np.arange(x_or[0], x_or[-1] + dx, dx)  # make new grid with first and last non-nan points
     y = np.interp(x, x_or, z_or)  # linearly interpolate elevation values
 
     return x, y
 
-
 def mov_average(x, z, win):
     """
     smooths z values using a moving average filter with windows of size win
 
     -Inputs-:
     x (ndarray)             --> cross-shore locations
     z (ndarray)             --> original elevations of x_or points
@@ -465,15 +563,14 @@
     z_smoothed (ndarray)    --> new smoothed elevations
     """
     n = int(np.round(win / (x[1] - x[0])))  # window is found by taking into account x-resolution and window size
     B = 1 / n * np.ones(n)
     z_smoothed = signal.filtfilt(B, 1, z)
     return z_smoothed
 
-
 def hanning_filter(x, z, window):
     """
     smooths z values using a hanning filter with windows of size window
 
     -Inputs-:
     x (ndarray)             --> cross-shore locations
     z (ndarray)             --> original elevations of x_or points
@@ -483,18 +580,16 @@
     z_smoothed (ndarray)    --> new smoothed elevations
     """
     window_han = int(np.round(window / (x[1] - x[0])))  # window is found by taking into account x-resolution and
     # window size
     with warnings.catch_warnings():  # avoid RuntimeWarning when window is smaller than grid spacing
         warnings.simplefilter("ignore", category=RuntimeWarning)
         han = np.divide(signal.hanning(window_han), np.sum(np.hanning(window_han)))
-    # z_smoothed = signal.filtfilt(han, 1, z, padtype=None)
-    # z_smoothed = signal.filtfilt(han, 1, z, padtype='odd')
+
     z_smoothed = signal.filtfilt(han, 1, z, padtype='even')
-    # z_smoothed = signal.filtfilt(han, 1, z, padtype='constant')
     return z_smoothed
 
 def zero_crossing(x, z, indices=False):
     """
     function to find zero-crossing and their indices
     adapted from PyAstronomy.pyaC.zerocross1d
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO` & `deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltares-coastalhazardstoolkit
-Version: 0.2.6
+Version: 0.2.7
 Author-email: Maarten van Ormondt <maarten.vanormondt@deltares-usa.us>, Roel de Goede <roel.degoede@deltares.nl>, Kees Nederhoff <kees.nederhoff@deltares-usa.us>, Tim Leijnse <tim.leijnse@deltares.nl>, Panos Athanasiou <panos.athanasiou@deltares.nl>
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: geopandas>=0.8
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyproj
```

### Comparing `deltares-coastalhazardstoolkit-0.2.6/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt` & `deltares_coastalhazardstoolkit-0.2.7/src/deltares_coastalhazardstoolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 src/cht/sfincs/sfincs.py
 src/cht/sfincs/sfincs_builder.py
 src/cht/sfincs/subgrid.py
 src/cht/sfincs2/__init__.py
 src/cht/sfincs2/boundary_conditions.py
 src/cht/sfincs2/cross_sections.py
 src/cht/sfincs2/grid.py
+src/cht/sfincs2/grid_v2.py
 src/cht/sfincs2/input.py
 src/cht/sfincs2/mask.py
 src/cht/sfincs2/observation_points.py
 src/cht/sfincs2/point_sources.py
 src/cht/sfincs2/quadtree_grid.py
 src/cht/sfincs2/quadtree_grid_snapwave.py
 src/cht/sfincs2/regular_grid.py
@@ -94,14 +95,15 @@
 src/cht/tide/predict.py
 src/cht/tide/test_tide_database.py
 src/cht/tide/tide.py
 src/cht/tide/tide_model.py
 src/cht/tide/tide_predict.py
 src/cht/tiling/__init__.py
 src/cht/tiling/tiling.py
+src/cht/tropical_cyclone/__init__.py
 src/cht/tropical_cyclone/cyclone_track_database.py
 src/cht/tropical_cyclone/test_forecasting.py
 src/cht/tropical_cyclone/test_meteo.py
 src/cht/tropical_cyclone/test_track.py
 src/cht/tropical_cyclone/test_track_reading.py
 src/cht/tropical_cyclone/tropical_cyclone.py
 src/cht/watersheds/__init__.py
```

