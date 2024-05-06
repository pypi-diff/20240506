# Comparing `tmp/pidgen2-0.3.8.tar.gz` & `tmp/pidgen2-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidgen2-0.3.8.tar", last modified: Thu May  2 18:00:46 2024, max compression
+gzip compressed data, was "pidgen2-0.3.9.tar", last modified: Mon May  6 21:38:32 2024, max compression
```

## Comparing `pidgen2-0.3.8.tar` & `pidgen2-0.3.9.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:46.182192 pidgen2-0.3.8/
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    35065 2021-08-03 09:00:33.000000 pidgen2-0.3.8/LICENSE
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)       34 2023-03-22 19:27:38.000000 pidgen2-0.3.8/MANIFEST.in
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2313 2024-05-02 18:00:46.159193 pidgen2-0.3.8/PKG-INFO
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1574 2022-05-06 07:27:54.000000 pidgen2-0.3.8/README.md
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      104 2021-08-03 09:00:33.000000 pidgen2-0.3.8/pyproject.toml
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1481 2024-05-02 18:00:46.187196 pidgen2-0.3.8/setup.cfg
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.664198 pidgen2-0.3.8/src/
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.811193 pidgen2-0.3.8/src/pidgen2/
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        0 2021-08-03 09:00:33.000000 pidgen2-0.3.8/src/pidgen2/__init__.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      414 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/add_brunel.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2848 2022-06-29 14:48:08.000000 pidgen2-0.3.8/src/pidgen2/cache.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)    13726 2024-05-01 18:11:53.000000 pidgen2-0.3.8/src/pidgen2/correct.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1235 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/create_correction_example.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1255 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/create_photon_correction_example.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1232 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/create_resampling_example.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     9486 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/datasets.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)    18360 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/density_estimation.py
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.845193 pidgen2-0.3.8/src/pidgen2/examples/
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     8145 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/examples/example_correct.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     6459 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/examples/example_correct_photon.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     8165 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/examples/example_resample.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1126 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/init.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1406 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_mc_samples.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2235 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_mc_variables.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1369 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_samples.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2170 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/list_variables.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5660 2024-05-02 15:55:27.000000 pidgen2-0.3.8/src/pidgen2/mc_datasets.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    14212 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/plotting.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)    11205 2024-05-01 18:14:27.000000 pidgen2-0.3.8/src/pidgen2/resample.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     4647 2024-05-01 18:32:35.000000 pidgen2-0.3.8/src/pidgen2/resampler.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    50273 2024-05-02 17:12:20.000000 pidgen2-0.3.8/src/pidgen2/resampling.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    48522 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/resampling_new.py
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:45.972194 pidgen2-0.3.8/src/pidgen2/samples/
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5812 2024-05-02 16:50:02.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4031 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_M.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4374 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_P.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4395 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4210 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5824 2024-05-02 17:32:38.000000 pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_scale.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1011 2021-08-03 09:00:33.000000 pidgen2-0.3.8/src/pidgen2/samples/__init__.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3023 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3068 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_Brem.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3068 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4044 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGamma.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4074 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType0.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4074 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType1.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5409 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5707 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5602 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5737 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5094 2024-05-02 16:59:58.000000 pidgen2-0.3.8/src/pidgen2/samples/p_IncLc.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5461 2024-05-02 17:02:57.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     3886 2023-03-27 18:03:02.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     3087 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5103 2024-05-02 17:04:47.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcmu.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2996 2024-05-02 16:48:07.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2424 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/samples/p_Test.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5837 2024-05-02 15:56:06.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4455 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_M.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4455 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_P.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4477 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4300 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5837 2024-05-02 17:09:14.000000 pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_scale.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5223 2021-09-17 08:50:28.000000 pidgen2-0.3.8/src/pidgen2/systematics.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     7050 2024-05-01 18:15:27.000000 pidgen2-0.3.8/src/pidgen2/tuples.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5061 2021-10-10 20:12:28.000000 pidgen2-0.3.8/src/pidgen2/validate.py
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:46.150193 pidgen2-0.3.8/src/pidgen2/variables/
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1288 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1365 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1287 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1289 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1290 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1363 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1292 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1365 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1226 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLK.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1223 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLe.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1225 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLmu.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1225 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/CombDLLp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1234 2022-08-28 19:47:05.000000 pidgen2-0.3.8/src/pidgen2/variables/IsPhoton.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNK.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1276 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNp.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1276 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1271 2024-05-01 12:46:16.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK_scale.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1273 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNe.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1275 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1273 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1335 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1275 2024-04-23 09:17:45.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1272 2024-05-02 17:10:09.000000 pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1281 2022-08-26 20:52:55.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1280 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNe.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1282 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1283 2023-03-22 19:27:38.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1335 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1285 2022-08-26 20:52:40.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1213 2022-08-27 19:02:29.000000 pidgen2-0.3.8/src/pidgen2/variables/PhotonCL.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1272 2023-03-29 09:04:47.000000 pidgen2-0.3.8/src/pidgen2/variables/Test_ProbNNp.py
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1011 2021-08-03 09:00:33.000000 pidgen2-0.3.8/src/pidgen2/variables/__init__.py
-drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-02 18:00:46.154193 pidgen2-0.3.8/src/pidgen2.egg-info/
--rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2313 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/PKG-INFO
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4416 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/SOURCES.txt
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        1 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/dependency_links.txt
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      629 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/entry_points.txt
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)       61 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/requires.txt
--rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        8 2024-05-02 18:00:45.000000 pidgen2-0.3.8/src/pidgen2.egg-info/top_level.txt
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:32.083400 pidgen2-0.3.9/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    35065 2021-08-03 09:00:33.000000 pidgen2-0.3.9/LICENSE
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)       34 2023-03-22 19:27:38.000000 pidgen2-0.3.9/MANIFEST.in
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2313 2024-05-06 21:38:32.081397 pidgen2-0.3.9/PKG-INFO
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1574 2022-05-06 07:27:54.000000 pidgen2-0.3.9/README.md
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      104 2021-08-03 09:00:33.000000 pidgen2-0.3.9/pyproject.toml
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1481 2024-05-06 21:38:32.088397 pidgen2-0.3.9/setup.cfg
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:31.558400 pidgen2-0.3.9/src/
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:31.665398 pidgen2-0.3.9/src/pidgen2/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        0 2021-08-03 09:00:33.000000 pidgen2-0.3.9/src/pidgen2/__init__.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      414 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/add_brunel.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2848 2022-06-29 14:48:08.000000 pidgen2-0.3.9/src/pidgen2/cache.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)    13726 2024-05-01 18:11:53.000000 pidgen2-0.3.9/src/pidgen2/correct.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1235 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/create_correction_example.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1255 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/create_photon_correction_example.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1232 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/create_resampling_example.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     9486 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/datasets.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)    18360 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/density_estimation.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:31.702398 pidgen2-0.3.9/src/pidgen2/examples/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     8145 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/examples/example_correct.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     6459 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/examples/example_correct_photon.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     8165 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/examples/example_resample.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1126 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/init.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1406 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/list_mc_samples.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2235 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/list_mc_variables.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1369 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/list_samples.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2170 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/list_variables.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5660 2024-05-02 15:55:27.000000 pidgen2-0.3.9/src/pidgen2/mc_datasets.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    14212 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/plotting.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)    11205 2024-05-01 18:14:27.000000 pidgen2-0.3.9/src/pidgen2/resample.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     4647 2024-05-01 18:32:35.000000 pidgen2-0.3.9/src/pidgen2/resampler.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    50273 2024-05-02 17:12:20.000000 pidgen2-0.3.9/src/pidgen2/resampling.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)    48522 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/resampling_new.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:31.855397 pidgen2-0.3.9/src/pidgen2/samples/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5812 2024-05-02 16:50:02.000000 pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4031 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_M.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4374 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_P.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4395 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4210 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5824 2024-05-02 17:32:38.000000 pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1011 2021-08-03 09:00:33.000000 pidgen2-0.3.9/src/pidgen2/samples/__init__.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3023 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/e_B2JpsieeK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3068 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/e_B2JpsieeK_Brem.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     3068 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4044 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/gamma_B2KstarGamma.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4074 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/gamma_B2KstarGammaType0.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4074 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/gamma_B2KstarGammaType1.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5409 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5707 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5602 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumunopt.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5737 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5094 2024-05-02 16:59:58.000000 pidgen2-0.3.9/src/pidgen2/samples/p_IncLc.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5461 2024-05-02 17:02:57.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     3886 2023-03-27 18:03:02.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi_Prompt.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     3087 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5455 2024-05-03 09:25:38.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5103 2024-05-02 17:04:47.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Lb2Lcmu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2996 2024-05-02 16:48:07.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Lb2Lcpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     2424 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/samples/p_Test.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5837 2024-05-02 15:56:06.000000 pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4455 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_M.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4455 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_P.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4477 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4300 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     5837 2024-05-02 17:09:14.000000 pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5223 2021-09-17 08:50:28.000000 pidgen2-0.3.9/src/pidgen2/systematics.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     7050 2024-05-01 18:15:27.000000 pidgen2-0.3.9/src/pidgen2/tuples.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     5061 2021-10-10 20:12:28.000000 pidgen2-0.3.9/src/pidgen2/validate.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:32.072398 pidgen2-0.3.9/src/pidgen2/variables/
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1288 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1365 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1287 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1289 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1290 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1363 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1292 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1365 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1437 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1226 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/CombDLLK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1223 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/CombDLLe.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1225 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/CombDLLmu.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1225 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/CombDLLp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1234 2022-08-28 19:47:05.000000 pidgen2-0.3.9/src/pidgen2/variables/IsPhoton.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1276 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNp.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1276 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1274 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1271 2024-05-01 12:46:16.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNK_scale.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1273 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNe.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1275 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1273 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1335 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1275 2024-04-23 09:17:45.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1272 2024-05-02 17:10:09.000000 pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1281 2022-08-26 20:52:55.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1278 2024-05-06 21:34:05.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNK_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1280 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNe.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1282 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1283 2023-03-22 19:27:38.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1335 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1280 2024-05-03 09:26:48.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNp_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1285 2022-08-26 20:52:40.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1337 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1395 2022-05-06 07:27:54.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     1282 2024-05-06 21:34:26.000000 pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpi_scale.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1213 2022-08-27 19:02:29.000000 pidgen2-0.3.9/src/pidgen2/variables/PhotonCL.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1272 2023-03-29 09:04:47.000000 pidgen2-0.3.9/src/pidgen2/variables/Test_ProbNNp.py
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     1011 2021-08-03 09:00:33.000000 pidgen2-0.3.9/src/pidgen2/variables/__init__.py
+drwxr-xr-x   0 poluekt   (5741) lhcb      (1200)        0 2024-05-06 21:38:32.076399 pidgen2-0.3.9/src/pidgen2.egg-info/
+-rw-r--r--   0 poluekt   (5741) lhcb      (1200)     2313 2024-05-06 21:38:31.000000 pidgen2-0.3.9/src/pidgen2.egg-info/PKG-INFO
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)     4609 2024-05-06 21:38:31.000000 pidgen2-0.3.9/src/pidgen2.egg-info/SOURCES.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        1 2024-05-06 21:38:31.000000 pidgen2-0.3.9/src/pidgen2.egg-info/dependency_links.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)      629 2024-05-06 21:38:31.000000 pidgen2-0.3.9/src/pidgen2.egg-info/entry_points.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)       61 2024-05-06 21:38:31.000000 pidgen2-0.3.9/src/pidgen2.egg-info/requires.txt
+-rw-rw-r--   0 poluekt   (5741) lhcb      (1200)        8 2024-05-06 21:38:31.000000 pidgen2-0.3.9/src/pidgen2.egg-info/top_level.txt
```

### Comparing `pidgen2-0.3.8/LICENSE` & `pidgen2-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/PKG-INFO` & `pidgen2-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidgen2
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for particle identification (PID) correction for LHCb detector
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidgen2
 Author: Anton Poluektov
 Author-email: anton.poluektov@cern.ch
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidgen2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidgen2-0.3.8/README.md` & `pidgen2-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/setup.cfg` & `pidgen2-0.3.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pidgen2
-version = 0.3.8
+version = 0.3.9
 author = Anton Poluektov
 author_email = anton.poluektov@cern.ch
 description = Tools for particle identification (PID) correction for LHCb detector
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.cern.ch/lhcb-rta/pidgen2
 project_urls =
```

### Comparing `pidgen2-0.3.8/src/pidgen2/cache.py` & `pidgen2-0.3.9/src/pidgen2/cache.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/correct.py` & `pidgen2-0.3.9/src/pidgen2/correct.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/create_correction_example.py` & `pidgen2-0.3.9/src/pidgen2/create_correction_example.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/create_photon_correction_example.py` & `pidgen2-0.3.9/src/pidgen2/create_photon_correction_example.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/create_resampling_example.py` & `pidgen2-0.3.9/src/pidgen2/create_resampling_example.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/datasets.py` & `pidgen2-0.3.9/src/pidgen2/datasets.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/density_estimation.py` & `pidgen2-0.3.9/src/pidgen2/density_estimation.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/examples/example_correct.py` & `pidgen2-0.3.9/src/pidgen2/examples/example_correct.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/examples/example_correct_photon.py` & `pidgen2-0.3.9/src/pidgen2/examples/example_correct_photon.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/examples/example_resample.py` & `pidgen2-0.3.9/src/pidgen2/examples/example_resample.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/init.py` & `pidgen2-0.3.9/src/pidgen2/init.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/list_mc_samples.py` & `pidgen2-0.3.9/src/pidgen2/list_mc_samples.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/list_mc_variables.py` & `pidgen2-0.3.9/src/pidgen2/list_mc_variables.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/list_samples.py` & `pidgen2-0.3.9/src/pidgen2/list_samples.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/list_variables.py` & `pidgen2-0.3.9/src/pidgen2/list_variables.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/mc_datasets.py` & `pidgen2-0.3.9/src/pidgen2/mc_datasets.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/plotting.py` & `pidgen2-0.3.9/src/pidgen2/plotting.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/resample.py` & `pidgen2-0.3.9/src/pidgen2/resample.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/resampler.py` & `pidgen2-0.3.9/src/pidgen2/resampler.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/resampling.py` & `pidgen2-0.3.9/src/pidgen2/resampling.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/resampling_new.py` & `pidgen2-0.3.9/src/pidgen2/resampling_new.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi.py` & `pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_M.py` & `pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_M.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_P.py` & `pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_P.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py` & `pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_PIDKgt4.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py` & `pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_PtEta.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/K_Dstar2Dpi_scale.py` & `pidgen2-0.3.9/src/pidgen2/samples/K_Dstar2Dpi_scale.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/__init__.py` & `pidgen2-0.3.9/src/pidgen2/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK.py` & `pidgen2-0.3.9/src/pidgen2/samples/e_B2JpsieeK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_Brem.py` & `pidgen2-0.3.9/src/pidgen2/samples/e_B2JpsieeK_Brem.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py` & `pidgen2-0.3.9/src/pidgen2/samples/e_B2JpsieeK_NoBrem.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGamma.py` & `pidgen2-0.3.9/src/pidgen2/samples/gamma_B2KstarGamma.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType0.py` & `pidgen2-0.3.9/src/pidgen2/samples/gamma_B2KstarGammaType0.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/gamma_B2KstarGammaType1.py` & `pidgen2-0.3.9/src/pidgen2/samples/gamma_B2KstarGammaType1.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu.py` & `pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py` & `pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt.py` & `pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumunopt.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py` & `pidgen2-0.3.9/src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_IncLc.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_IncLc.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi_Prompt.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcmu.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_Lb2Lcmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_Lb2Lcpi.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_Lb2Lcpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/p_Test.py` & `pidgen2-0.3.9/src/pidgen2/samples/p_Test.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi.py` & `pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_M.py` & `pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_M.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_P.py` & `pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_P.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py` & `pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py` & `pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_PtEta.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/samples/pi_Dstar2Dpi_scale.py` & `pidgen2-0.3.9/src/pidgen2/samples/pi_Dstar2Dpi_scale.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/systematics.py` & `pidgen2-0.3.9/src/pidgen2/systematics.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/tuples.py` & `pidgen2-0.3.9/src/pidgen2/tuples.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/validate.py` & `pidgen2-0.3.9/src/pidgen2/validate.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNKNotpip.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpNotpiK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py` & `pidgen2-0.3.9/src/pidgen2/variables/Brunel_MC15TuneV1_ProbNNpiNotKp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/CombDLLK.py` & `pidgen2-0.3.9/src/pidgen2/variables/CombDLLK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/CombDLLe.py` & `pidgen2-0.3.9/src/pidgen2/variables/CombDLLe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/CombDLLmu.py` & `pidgen2-0.3.9/src/pidgen2/variables/CombDLLmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/CombDLLp.py` & `pidgen2-0.3.9/src/pidgen2/variables/CombDLLp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/IsPhoton.py` & `pidgen2-0.3.9/src/pidgen2/variables/IsPhoton.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNp.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV2_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNKNotpip.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNK_scale.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNK_scale.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNe.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNp.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpNotpiK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNe.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNe.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNmu.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNp.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpi.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py` & `pidgen2-0.3.9/src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/PhotonCL.py` & `pidgen2-0.3.9/src/pidgen2/variables/PhotonCL.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/Test_ProbNNp.py` & `pidgen2-0.3.9/src/pidgen2/variables/Test_ProbNNp.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2/variables/__init__.py` & `pidgen2-0.3.9/src/pidgen2/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pidgen2-0.3.8/src/pidgen2.egg-info/PKG-INFO` & `pidgen2-0.3.9/src/pidgen2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidgen2
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for particle identification (PID) correction for LHCb detector
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidgen2
 Author: Anton Poluektov
 Author-email: anton.poluektov@cern.ch
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidgen2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidgen2-0.3.8/src/pidgen2.egg-info/SOURCES.txt` & `pidgen2-0.3.9/src/pidgen2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 src/pidgen2/samples/mu_Jpsi2mumu_isMuon.py
 src/pidgen2/samples/mu_Jpsi2mumunopt.py
 src/pidgen2/samples/mu_Jpsi2mumunopt_isMuon.py
 src/pidgen2/samples/p_IncLc.py
 src/pidgen2/samples/p_Lambda2ppi.py
 src/pidgen2/samples/p_Lambda2ppi_Prompt.py
 src/pidgen2/samples/p_Lambda2ppi_Prompt_PIDpgt0.py
+src/pidgen2/samples/p_Lambda2ppi_scale.py
 src/pidgen2/samples/p_Lb2Lcmu.py
 src/pidgen2/samples/p_Lb2Lcpi.py
 src/pidgen2/samples/p_Test.py
 src/pidgen2/samples/pi_Dstar2Dpi.py
 src/pidgen2/samples/pi_Dstar2Dpi_M.py
 src/pidgen2/samples/pi_Dstar2Dpi_P.py
 src/pidgen2/samples/pi_Dstar2Dpi_PIDKlt2.py
@@ -97,18 +98,21 @@
 src/pidgen2/variables/MC12TuneV3_ProbNNpi.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpiNotK.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpiNotKp.py
 src/pidgen2/variables/MC12TuneV3_ProbNNpi_scale.py
 src/pidgen2/variables/MC15TuneV1_ProbNNK.py
 src/pidgen2/variables/MC15TuneV1_ProbNNKNotpi.py
 src/pidgen2/variables/MC15TuneV1_ProbNNKNotpip.py
+src/pidgen2/variables/MC15TuneV1_ProbNNK_scale.py
 src/pidgen2/variables/MC15TuneV1_ProbNNe.py
 src/pidgen2/variables/MC15TuneV1_ProbNNmu.py
 src/pidgen2/variables/MC15TuneV1_ProbNNp.py
 src/pidgen2/variables/MC15TuneV1_ProbNNpNotK.py
 src/pidgen2/variables/MC15TuneV1_ProbNNpNotpiK.py
+src/pidgen2/variables/MC15TuneV1_ProbNNp_scale.py
 src/pidgen2/variables/MC15TuneV1_ProbNNpi.py
 src/pidgen2/variables/MC15TuneV1_ProbNNpiNotK.py
 src/pidgen2/variables/MC15TuneV1_ProbNNpiNotKp.py
+src/pidgen2/variables/MC15TuneV1_ProbNNpi_scale.py
 src/pidgen2/variables/PhotonCL.py
 src/pidgen2/variables/Test_ProbNNp.py
 src/pidgen2/variables/__init__.py
```

### Comparing `pidgen2-0.3.8/src/pidgen2.egg-info/entry_points.txt` & `pidgen2-0.3.9/src/pidgen2.egg-info/entry_points.txt`

 * *Files identical despite different names*

