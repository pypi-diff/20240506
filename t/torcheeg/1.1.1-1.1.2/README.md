# Comparing `tmp/torcheeg-1.1.1.tar.gz` & `tmp/torcheeg-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcheeg-1.1.1.tar", last modified: Wed Jan  3 07:04:58 2024, max compression
+gzip compressed data, was "torcheeg-1.1.2.tar", last modified: Mon May  6 14:23:26 2024, max compression
```

## Comparing `torcheeg-1.1.1.tar` & `torcheeg-1.1.2.tar`

### file list

```diff
@@ -1,286 +1,300 @@
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1097 2023-12-13 05:11:19.000000 torcheeg-1.1.1/LICENSE
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       33 2023-12-13 05:11:20.000000 torcheeg-1.1.1/MANIFEST.in
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18902 2024-01-03 07:04:58.888563 torcheeg-1.1.1/PKG-INFO
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18943 2023-12-25 11:44:41.000000 torcheeg-1.1.1/README.md
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18266 2023-12-13 05:11:20.000000 torcheeg-1.1.1/README.rst
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       38 2024-01-03 07:04:58.888563 torcheeg-1.1.1/setup.cfg
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1507 2024-01-03 06:24:01.000000 torcheeg-1.1.1/setup.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.868563 torcheeg-1.1.1/test/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/__init__.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.868563 torcheeg-1.1.1/test/datasets/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/datasets/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8587 2024-01-03 05:39:36.000000 torcheeg-1.1.1/test/datasets/test_emotion_recognition.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4210 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/datasets/test_folder.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3037 2024-01-03 05:17:31.000000 torcheeg-1.1.1/test/datasets/test_hooks.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2317 2023-12-13 05:22:06.000000 torcheeg-1.1.1/test/datasets/test_motor_imagery.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2345 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/datasets/test_personal_identification.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1120 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/datasets/test_ssvep.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.868563 torcheeg-1.1.1/test/io/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/io/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3264 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/io/test_eeg_signal.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2240 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/io/test_meta_info.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.868563 torcheeg-1.1.1/test/model_selection/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      974 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_k_fold.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1198 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_k_fold_cross_subject.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1004 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_k_fold_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1016 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_k_fold_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1223 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_k_fold_per_subject_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1231 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_k_fold_per_subject_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1028 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_leave_one_subject_out.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      892 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_split.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      938 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_split_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      946 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_split_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1162 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_split_per_subject_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1170 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_split_per_subject_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      910 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/model_selection/test_subcategory.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/test/models/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/models/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5487 2023-12-13 05:22:06.000000 torcheeg-1.1.1/test/models/test_cnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1098 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/models/test_ddpm.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1637 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/models/test_flow.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3734 2023-12-13 05:22:06.000000 torcheeg-1.1.1/test/models/test_gan.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2653 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/models/test_gnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      858 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/models/test_rnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3272 2023-12-13 05:22:06.000000 torcheeg-1.1.1/test/models/test_transformer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1762 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/models/test_vae.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/test/trainers/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/trainers/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2436 2023-12-13 11:32:05.000000 torcheeg-1.1.1/test/trainers/test_classifier_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4335 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/trainers/test_ddpm_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6949 2023-12-13 05:22:06.000000 torcheeg-1.1.1/test/trainers/test_domain_adaption_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4589 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/trainers/test_gan_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1721 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/trainers/test_glow_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8904 2023-12-13 05:22:06.000000 torcheeg-1.1.1/test/trainers/test_imbalance_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1656 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/trainers/test_self_supervised_trainer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3263 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/trainers/test_vae_trainer.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/test/transforms/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/transforms/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2597 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/transforms/test_any.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2107 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/transforms/test_label.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10083 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/transforms/test_numpy.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1893 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/transforms/test_pyg.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5400 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/transforms/test_torch.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/test/utils/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/utils/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2473 2023-12-13 05:11:20.000000 torcheeg-1.1.1/test/utils/test_visualize.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/torcheeg/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1113 2024-01-03 06:23:52.000000 torcheeg-1.1.1/torcheeg/__init__.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/torcheeg/datasets/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       47 2023-12-25 06:26:45.000000 torcheeg-1.1.1/torcheeg/datasets/__init__.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/torcheeg/datasets/constants/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       94 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/__init__.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/torcheeg/datasets/constants/clinical/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/clinical/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2511 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/clinical/tuh_tueg.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      149 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2334 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/amigos.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2927 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/bci2022.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3114 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/deap.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2257 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/dreamer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3117 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/mahnob.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4414 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/mped.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4414 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/seed.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4466 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/seed_iv.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/constants/motor_imagery/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/motor_imagery/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      152 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/datasets/constants/motor_imagery/bciciv_2a.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/constants/personal_identification/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       19 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/personal_identification/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5720 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/personal_identification/m3cv.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1781 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/region_1020.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/constants/ssvep/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       28 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/ssvep/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5264 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/ssvep/tsu_benchmark.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18994 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/standard_1005.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5273 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/standard_1020.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4952 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/constants/utils.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/functional/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       20 2023-12-25 06:33:15.000000 torcheeg-1.1.1/torcheeg/datasets/functional/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5496 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/functional/hooks.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/moabb/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      182 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/moabb/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    11440 2023-12-26 15:42:03.000000 torcheeg-1.1.1/torcheeg/datasets/moabb/moabb_dataset.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/module/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      253 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/datasets/module/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    19892 2023-12-26 18:03:29.000000 torcheeg-1.1.1/torcheeg/datasets/module/base_dataset.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8234 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/csv_folder_dataset.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      374 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    17288 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/amigos.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15508 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/bci2022.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15272 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/deap.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    16015 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/dreamer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    17666 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/mahnob.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    12695 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/mped_feature.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13445 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13594 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed_feature.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14134 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed_iv.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13276 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed_iv_feature.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9941 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/folder_dataset.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/module/motor_imagery/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       38 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/datasets/module/motor_imagery/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13130 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/motor_imagery/bciciv_2a.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/module/personal_identification/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       29 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/module/personal_identification/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13882 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/personal_identification/m3cv.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/datasets/module/sspev/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       46 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/datasets/module/sspev/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13850 2023-12-26 16:04:55.000000 torcheeg-1.1.1/torcheeg/datasets/module/sspev/tsu_benchmark.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.876562 torcheeg-1.1.1/torcheeg/io/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       69 2023-12-25 06:26:57.000000 torcheeg-1.1.1/torcheeg/io/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13295 2023-12-25 10:55:17.000000 torcheeg-1.1.1/torcheeg/io/eeg_signal.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2655 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/io/meta_info.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/model_selection/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      500 2023-12-25 06:27:08.000000 torcheeg-1.1.1/torcheeg/model_selection/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6544 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7147 2023-12-26 18:07:02.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold_cross_subject.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7452 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7422 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8595 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold_per_subject.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9809 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold_per_subject_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9655 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/k_fold_per_subject_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4685 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/leave_one_subject_out.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4719 2023-12-26 17:51:50.000000 torcheeg-1.1.1/torcheeg/model_selection/split.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6353 2024-01-03 06:57:40.000000 torcheeg-1.1.1/torcheeg/model_selection/split_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5542 2024-01-03 06:57:40.000000 torcheeg-1.1.1/torcheeg/model_selection/split_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5790 2023-12-26 17:51:50.000000 torcheeg-1.1.1/torcheeg/model_selection/split_per_subject_cross_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5650 2024-01-03 06:57:40.000000 torcheeg-1.1.1/torcheeg/model_selection/split_per_subject_groupby_trial.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7290 2023-12-26 18:06:48.000000 torcheeg-1.1.1/torcheeg/model_selection/subcategory.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      161 2023-12-25 06:27:11.000000 torcheeg-1.1.1/torcheeg/models/__init__.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/cnn/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      327 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/models/cnn/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3577 2023-12-27 19:11:06.000000 torcheeg-1.1.1/torcheeg/models/cnn/ccnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5668 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/eegnet.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4434 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/fbccnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8220 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/fbcnet.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14963 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/models/cnn/fbmsnet.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5310 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/mtcnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    16897 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/sst_emotion_net.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5692 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/stnet.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6468 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/cnn/tsception.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/ddpm/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       51 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/ddpm/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9722 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/ddpm/bcddpm.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9035 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/ddpm/bddpm.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/flow/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       51 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/flow/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    26078 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/flow/bcglow.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    25315 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/flow/bglow.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/gan/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       66 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/models/gan/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8935 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/gan/bcgan.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6725 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/gan/bgan.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13164 2024-01-03 06:44:02.000000 torcheeg-1.1.1/torcheeg/models/gan/eegfusenet.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/gnn/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       51 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/gnn/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6391 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/gnn/dgcnn.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    12959 2023-12-28 03:07:27.000000 torcheeg-1.1.1/torcheeg/models/gnn/lggnet.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/pyg/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      351 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/pyg/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3712 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/pyg/gin.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8315 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/pyg/rgnn.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.880563 torcheeg-1.1.1/torcheeg/models/rnn/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       43 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/rnn/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2763 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/rnn/gru.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2832 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/rnn/lstm.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/models/transformer/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      198 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/models/transformer/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9484 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/transformer/arjun_vit.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7722 2024-01-03 06:43:05.000000 torcheeg-1.1.1/torcheeg/models/transformer/atcnet.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10508 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/transformer/conformer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    11152 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/transformer/simple_vit.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7153 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/transformer/vanilla_transformer.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10907 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/transformer/vit.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/models/vae/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       40 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/vae/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9182 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/vae/bcvae.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7810 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/models/vae/bvae.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/trainers/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      178 2023-12-25 06:27:43.000000 torcheeg-1.1.1/torcheeg/trainers/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10465 2023-12-28 04:32:57.000000 torcheeg-1.1.1/torcheeg/trainers/classifier.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      211 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8226 2023-12-13 05:43:26.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/ada.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15049 2024-01-03 06:48:32.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/center.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5542 2023-12-13 05:43:26.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/coral.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6549 2023-12-13 05:43:26.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/dan.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5319 2023-12-13 05:43:26.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/dann.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9824 2023-12-25 06:37:33.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/dann_like.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5265 2023-12-13 05:43:26.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/ddc.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9222 2023-12-13 05:43:26.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/jan.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8823 2023-12-25 06:37:58.000000 torcheeg-1.1.1/torcheeg/trainers/domain_adaption/mmd_like.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15777 2023-12-25 06:36:32.000000 torcheeg-1.1.1/torcheeg/trainers/finetune.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/trainers/generative/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      192 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/trainers/generative/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    22474 2023-12-25 06:38:21.000000 torcheeg-1.1.1/torcheeg/trainers/generative/beta_vae.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    42024 2023-12-25 06:38:55.000000 torcheeg-1.1.1/torcheeg/trainers/generative/ddpm.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    23261 2023-12-25 06:39:14.000000 torcheeg-1.1.1/torcheeg/trainers/generative/glow.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5474 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/trainers/generative/utils.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    23999 2023-12-27 18:36:24.000000 torcheeg-1.1.1/torcheeg/trainers/generative/wgan_gp.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/trainers/imbalance/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      161 2023-12-13 05:22:06.000000 torcheeg-1.1.1/torcheeg/trainers/imbalance/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6839 2023-12-19 13:35:44.000000 torcheeg-1.1.1/torcheeg/trainers/imbalance/eq.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8031 2023-12-19 13:35:44.000000 torcheeg-1.1.1/torcheeg/trainers/imbalance/focal.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6294 2023-12-19 13:32:28.000000 torcheeg-1.1.1/torcheeg/trainers/imbalance/la.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9272 2023-12-19 13:35:44.000000 torcheeg-1.1.1/torcheeg/trainers/imbalance/ldam.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6154 2023-12-19 13:35:44.000000 torcheeg-1.1.1/torcheeg/trainers/imbalance/wce.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/trainers/self_supervised/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       64 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/trainers/self_supervised/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    19671 2023-12-25 10:55:17.000000 torcheeg-1.1.1/torcheeg/trainers/self_supervised/byol.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14727 2023-12-25 06:40:11.000000 torcheeg-1.1.1/torcheeg/trainers/self_supervised/sim_clr.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/transforms/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      111 2023-12-25 06:20:36.000000 torcheeg-1.1.1/torcheeg/transforms/__init__.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.884563 torcheeg-1.1.1/torcheeg/transforms/any/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      107 2023-12-25 06:22:09.000000 torcheeg-1.1.1/torcheeg/transforms/any/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2381 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/any/baseline.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1897 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/any/compose.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1482 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/any/lambd.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1502 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/any/pdb.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3640 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/base_transform.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/torcheeg/transforms/label/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      107 2023-12-25 06:22:19.000000 torcheeg-1.1.1/torcheeg/transforms/label/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4237 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/label/binary.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1409 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/label/fix.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1878 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/label/mapping.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1839 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/label/select.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1583 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/label/string.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/torcheeg/transforms/numpy/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      287 2023-12-25 06:24:23.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    21569 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/band.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    39443 2023-12-25 06:22:57.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/band_pyeeg.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2190 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/coefficient.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8367 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/concatenate.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5176 2023-12-25 06:47:33.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/correlation.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2301 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/downsample.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1101 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/flatten.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8225 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/normalize.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3900 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/pick.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3234 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/rearrange.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7336 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/spectrum.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10547 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/numpy/to.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/torcheeg/transforms/pyg/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      325 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/pyg/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13305 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/pyg/to.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/torcheeg/transforms/torch/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       88 2023-12-25 06:21:03.000000 torcheeg-1.1.1/torcheeg/transforms/torch/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2538 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/torch/contrastive.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    42770 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/torch/random.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2600 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/transforms/torch/resize.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1609 2023-12-28 03:31:28.000000 torcheeg-1.1.1/torcheeg/transforms/torch/to.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/torcheeg/utils/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      248 2023-12-26 15:20:27.000000 torcheeg-1.1.1/torcheeg/utils/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2415 2023-12-26 16:04:05.000000 torcheeg-1.1.1/torcheeg/utils/file.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.888563 torcheeg-1.1.1/torcheeg/utils/pyg/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      345 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/utils/pyg/__init__.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3283 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/utils/pyg/visualize.py
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14337 2023-12-13 05:11:20.000000 torcheeg-1.1.1/torcheeg/utils/visualize.py
-drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-01-03 07:04:58.872563 torcheeg-1.1.1/torcheeg.egg-info/
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18902 2024-01-03 07:04:58.000000 torcheeg-1.1.1/torcheeg.egg-info/PKG-INFO
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9012 2024-01-03 07:04:58.000000 torcheeg-1.1.1/torcheeg.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        1 2024-01-03 07:04:58.000000 torcheeg-1.1.1/torcheeg.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      393 2024-01-03 07:04:58.000000 torcheeg-1.1.1/torcheeg.egg-info/requires.txt
--rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       14 2024-01-03 07:04:58.000000 torcheeg-1.1.1/torcheeg.egg-info/top_level.txt
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.947766 torcheeg-1.1.2/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1097 2024-05-06 14:21:07.000000 torcheeg-1.1.2/LICENSE
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       33 2024-05-06 14:21:07.000000 torcheeg-1.1.2/MANIFEST.in
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    19380 2024-05-06 14:23:26.947766 torcheeg-1.1.2/PKG-INFO
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    19647 2024-05-06 14:21:07.000000 torcheeg-1.1.2/README.md
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18744 2024-05-06 14:21:07.000000 torcheeg-1.1.2/README.rst
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       38 2024-05-06 14:23:26.947766 torcheeg-1.1.2/setup.cfg
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1522 2024-05-06 14:22:16.000000 torcheeg-1.1.2/setup.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.923766 torcheeg-1.1.2/test/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/__init__.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.927766 torcheeg-1.1.2/test/datasets/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10515 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/test_emotion_recognition.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4210 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/test_folder.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2317 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/test_motor_imagery.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2345 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/test_personal_identification.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1133 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/test_sleep_stage_detection.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1120 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/datasets/test_ssvep.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.927766 torcheeg-1.1.2/test/io/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/io/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3264 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/io/test_eeg_signal.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2240 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/io/test_meta_info.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.927766 torcheeg-1.1.2/test/model_selection/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      974 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_k_fold.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1198 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_k_fold_cross_subject.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1004 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_k_fold_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1016 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_k_fold_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1223 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_k_fold_per_subject_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1231 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_k_fold_per_subject_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1028 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_leave_one_subject_out.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      892 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_split.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      938 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_split_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      946 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_split_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1162 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_split_per_subject_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1170 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_split_per_subject_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      910 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/model_selection/test_subcategory.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.927766 torcheeg-1.1.2/test/models/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5487 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_cnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1098 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_ddpm.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1637 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_flow.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3734 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_gan.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2628 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_gnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      858 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_rnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3272 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_transformer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1762 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/models/test_vae.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.927766 torcheeg-1.1.2/test/trainers/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2436 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_classifier_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4335 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_ddpm_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6949 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_domain_adaption_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4589 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_gan_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1721 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_glow_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8904 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_imbalance_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1656 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_self_supervised_trainer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3263 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/trainers/test_vae_trainer.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.927766 torcheeg-1.1.2/test/transforms/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2597 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/test_any.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3765 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/test_hooks.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2107 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/test_label.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10083 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/test_numpy.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1893 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/test_pyg.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5400 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/transforms/test_torch.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/test/utils/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/utils/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2667 2024-05-06 14:21:07.000000 torcheeg-1.1.2/test/utils/test_visualize.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1113 2024-05-06 14:22:16.000000 torcheeg-1.1.2/torcheeg/__init__.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       21 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/__init__.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       94 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/__init__.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/clinical/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/clinical/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2511 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/clinical/tuh_tueg.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      192 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2334 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/amigos.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2927 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/bci2022.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3114 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/deap.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2257 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/dreamer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2978 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/faced.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3117 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/mahnob.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4414 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/mped.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4414 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/seed.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4466 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/seed_iv.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4449 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/seed_v.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/motor_imagery/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/motor_imagery/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      716 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/motor_imagery/bciciv_2a.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/personal_identification/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       19 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/personal_identification/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5720 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/personal_identification/m3cv.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1781 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/region_1020.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/sleep_stage_detection/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/sleep_stage_detection/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       61 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/sleep_stage_detection/sleep_edfx.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/constants/ssvep/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       28 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/ssvep/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5264 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/ssvep/tsu_benchmark.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18994 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/standard_1005.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5273 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/standard_1020.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4952 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/constants/utils.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/moabb/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      182 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/moabb/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    11589 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/moabb/moabb_dataset.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg/datasets/module/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      289 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    20013 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/base_dataset.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8330 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/csv_folder_dataset.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      535 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    17820 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/amigos.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    16282 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/bci2022.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15443 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/deap.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    16221 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/dreamer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14699 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/faced.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    12441 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/faced_feature.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    18142 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/mahnob.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13080 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/mped_feature.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13890 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13987 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_feature.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14618 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_iv.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13681 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_iv_feature.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15372 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_v.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    11296 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_v_feature.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10030 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/folder_dataset.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/datasets/module/motor_imagery/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       38 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/motor_imagery/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13225 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/motor_imagery/bciciv_2a.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/datasets/module/personal_identification/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       29 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/personal_identification/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14306 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/personal_identification/m3cv.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/datasets/module/sleep_stage_detection/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       40 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/sleep_stage_detection/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14482 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/sleep_stage_detection/sleep_edfx.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/datasets/module/ssvep/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       46 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/ssvep/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13086 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/datasets/module/ssvep/tsu_benchmark.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/io/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       69 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/io/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13295 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/io/eeg_signal.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2655 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/io/meta_info.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/model_selection/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      500 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6732 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7347 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold_cross_subject.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7650 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7622 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8991 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold_per_subject.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10225 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold_per_subject_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10075 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/k_fold_per_subject_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4886 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/leave_one_subject_out.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5068 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/split.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6714 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/split_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5905 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/split_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5992 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/split_per_subject_cross_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6157 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/split_per_subject_groupby_trial.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7492 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/model_selection/subcategory.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.935766 torcheeg-1.1.2/torcheeg/models/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      161 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/__init__.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/cnn/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      327 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3964 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/ccnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5973 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/eegnet.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4813 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/fbccnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8534 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/fbcnet.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13168 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/fbmsnet.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5836 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/mtcnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    17419 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/sst_emotion_net.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6070 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/stnet.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7278 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/cnn/tsception.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/ddpm/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       51 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/ddpm/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9761 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/ddpm/bcddpm.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9108 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/ddpm/bddpm.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/flow/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       51 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/flow/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    26156 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/flow/bcglow.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    25399 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/flow/bglow.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/gan/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       66 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gan/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9016 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gan/bcgan.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6812 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gan/bgan.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13257 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gan/eegfusenet.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/gnn/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       51 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gnn/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6564 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gnn/dgcnn.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13205 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/gnn/lggnet.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/pyg/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      351 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/pyg/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4124 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/pyg/gin.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8619 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/pyg/rgnn.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/rnn/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       43 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/rnn/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3034 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/rnn/gru.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3105 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/rnn/lstm.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/transformer/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      199 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9820 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/arjun_vit.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7801 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/atcnet.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10725 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/conformer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    11891 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/simple_vit.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7477 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/vanilla_transformer.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    11313 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/transformer/vit.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/models/vae/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       40 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/vae/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9259 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/vae/bcvae.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7886 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/models/vae/bvae.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/trainers/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      178 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10463 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/classifier.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.939766 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      211 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8775 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/ada.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    14066 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/center.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6098 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/coral.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7093 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/dan.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5933 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/dann.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9824 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/dann_like.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5809 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/ddc.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9771 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/jan.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8823 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/domain_adaption/mmd_like.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15775 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/finetune.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/trainers/generative/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      192 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/generative/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    22503 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/generative/beta_vae.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    42060 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/generative/ddpm.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    23181 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/generative/glow.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5474 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/generative/utils.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    23919 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/generative/wgan_gp.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/trainers/imbalance/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      161 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/imbalance/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6730 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/imbalance/eq.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7923 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/imbalance/focal.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6185 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/imbalance/la.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9164 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/imbalance/ldam.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     6046 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/imbalance/wce.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/trainers/self_supervised/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       64 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/self_supervised/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    20039 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/self_supervised/byol.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15140 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/trainers/self_supervised/sim_clr.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/transforms/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      132 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/__init__.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/transforms/any/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      107 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/any/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2461 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/any/baseline.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2046 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/any/compose.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1518 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/any/lambd.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1593 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/any/pdb.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3640 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/base_transform.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/transforms/hooks/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       52 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/hooks/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13065 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/hooks/after_hook.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2604 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/hooks/before_hook.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/transforms/label/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      107 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/label/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4382 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/label/binary.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1481 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/label/fix.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1936 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/label/mapping.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1919 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/label/select.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1609 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/label/string.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/transforms/numpy/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      287 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    21821 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/band.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    39803 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/band_pyeeg.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2226 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/coefficient.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8563 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/concatenate.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     5248 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/correlation.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2337 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/downsample.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1145 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/flatten.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     8336 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/normalize.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     4013 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/pick.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3270 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/rearrange.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     7482 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/spectrum.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    10794 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/numpy/to.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.943766 torcheeg-1.1.2/torcheeg/transforms/pyg/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      325 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/pyg/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    13400 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/pyg/to.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.947766 torcheeg-1.1.2/torcheeg/transforms/torch/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       88 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/torch/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2566 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/torch/contrastive.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    42806 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/torch/random.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2636 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/torch/resize.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     1645 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/transforms/torch/to.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.947766 torcheeg-1.1.2/torcheeg/utils/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      248 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/utils/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     2415 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/utils/file.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.947766 torcheeg-1.1.2/torcheeg/utils/pyg/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      345 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/utils/pyg/__init__.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     3492 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/utils/pyg/visualize.py
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    15933 2024-05-06 14:21:07.000000 torcheeg-1.1.2/torcheeg/utils/visualize.py
+drwxrwxr-x   0 zhangzhi  (1001) zhangzhi  (1001)        0 2024-05-06 14:23:26.931766 torcheeg-1.1.2/torcheeg.egg-info/
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)    19380 2024-05-06 14:23:26.000000 torcheeg-1.1.2/torcheeg.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)     9693 2024-05-06 14:23:26.000000 torcheeg-1.1.2/torcheeg.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)        1 2024-05-06 14:23:26.000000 torcheeg-1.1.2/torcheeg.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)      405 2024-05-06 14:23:26.000000 torcheeg-1.1.2/torcheeg.egg-info/requires.txt
+-rw-rw-r--   0 zhangzhi  (1001) zhangzhi  (1001)       14 2024-05-06 14:23:26.000000 torcheeg-1.1.2/torcheeg.egg-info/top_level.txt
```

### Comparing `torcheeg-1.1.1/LICENSE` & `torcheeg-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/PKG-INFO` & `torcheeg-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheeg
-Version: 1.1.1
+Version: 1.1.2
 Summary: TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG aims to provide a plug-and-play EEG analysis tool, so that researchers can quickly reproduce EEG analysis work and start new EEG analysis research without paying attention to technical details unrelated to the research focus.
 Home-page: https://github.com/tczhangzhi/torcheeg
 Author: TorchEEG Team
 Author-email: tczhangzhi@gmail.com
 License: MIT
 Keywords: PyTorch,EEG
 Requires-Python: >=3.7
@@ -16,15 +16,16 @@
 
 TorchEEG
 ========
 
 |PyPI Version| |Docs Status| |Downloads| |Join the Chat|
 
 `Documentation <https://torcheeg.readthedocs.io/>`__ \| `TorchEEG
-Examples <https://github.com/tczhangzhi/torcheeg/tree/main/examples>`__
+Examples <https://github.com/torcheeg/torcheeg/tree/main/examples>`__ \|
+`Paper <https://www.sciencedirect.com/science/article/pii/S0957417424004159>`__
 
 TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG
 aims to provide a plug-and-play EEG analysis tool, so that researchers
 can quickly reproduce EEG analysis work and start new EEG analysis
 research without paying attention to technical details unrelated to the
 research focus.
 
@@ -267,15 +268,15 @@
 e.g. ``./tmp_in/data_preprocessed_python``.
 
 .. code:: python
 
    from torcheeg.datasets import DEAPDataset
    from torcheeg import transforms
 
-   from torcheeg.datasets.constants.emotion_recognition.deap import \
+   from torcheeg.datasets.constants import \
        DEAP_CHANNEL_LOCATION_DICT
 
    dataset = DEAPDataset(
        io_path=f'./tmp_out/examples_pipeline/deap',
        root_path='./tmp_in/data_preprocessed_python',
        offline_transform=transforms.Compose([
            transforms.BandDifferentialEntropy(apply_to_baseline=True),
@@ -378,14 +379,30 @@
 License
 -------
 
 TorchEEG has a MIT license, as found in the
 `LICENSE <https://github.com/tczhangzhi/torcheeg/blob/main/LICENSE>`__
 file.
 
+Citation
+--------
+
+If you find this project useful for your research, please cite:
+
+.. code:: latex
+
+   @article{zhang2024torcheeg,
+       title = {{TorchEEGEMO}: A deep learning toolbox towards {EEG}-based emotion recognition},
+       journal = {Expert Systems with Applications},
+       pages = {123550},
+       year = {2024},
+       issn = {0957-4174},
+       author = {Zhi Zhang and Sheng-hua Zhong and Yan Liu}
+   }
+
 .. |PyPI Version| image:: https://badge.fury.io/py/torcheeg.svg
    :target: https://pypi.python.org/pypi/torcheeg
 .. |Docs Status| image:: https://readthedocs.org/projects/torcheeg/badge/?version=latest
    :target: https://torcheeg.readthedocs.io/en/latest/?badge=latest
 .. |Downloads| image:: https://pepy.tech/badge/torcheeg
    :target: https://pepy.tech/project/torcheeg
 .. |Join the Chat| image:: https://badges.gitter.im/torcheeg/community.svg
```

### Comparing `torcheeg-1.1.1/README.md` & `torcheeg-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 --------------------------------------------------------------------------------
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Docs Status][docs-image]][docs-url]
 [![Downloads][pepy-image]][pepy-url]
 [![Join the Chat][gitter-image]][gitter-url]
 
-**[Documentation](https://torcheeg.readthedocs.io/)** | **[TorchEEG Examples](https://github.com/torcheeg/torcheeg/tree/main/examples)**
+**[Documentation](https://torcheeg.readthedocs.io/)** | **[TorchEEG Examples](https://github.com/torcheeg/torcheeg/tree/main/examples)** | **[Paper](https://www.sciencedirect.com/science/article/pii/S0957417424004159)**
 
 TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG aims to provide a plug-and-play EEG analysis tool, so that researchers can quickly reproduce EEG analysis work and start new EEG analysis research without paying attention to technical details unrelated to the research focus.
 
 TorchEEG specifies a unified data input-output format (IO) and implement commonly used EEG databases, allowing users to quickly access benchmark datasets and define new custom datasets. The datasets that have been defined so far include emotion recognition and so on. According to papers published in the field of EEG analysis, TorchEEG provides data preprocessing methods commonly used for EEG signals, and provides plug-and-play API for both offline and online pre-proocessing. Offline processing allow users to process once and use any times, speeding up the training process. Online processing allows users to save time when creating new data processing methods. TorchEEG also provides deep learning models following published papers for EEG analysis, including convolutional neural networks, graph convolutional neural networks, and Transformers.
 
 ## Installation
 
@@ -142,15 +142,15 @@
 
 The `torcheeg.datasets` module contains dataset classes for many real-world EEG datasets. In this tutorial, we use the `DEAP` dataset. We first go to the official website to apply for data download permission according to the introduction of [DEAP dataset](https://www.eecs.qmul.ac.uk/mmv/datasets/deap/), and download the dataset. Next, we need to specify the download location of the dataset in the `root_path` parameter. For the DEAP dataset, we specify the path to the `data_preprocessed_python` folder, e.g. `./tmp_in/data_preprocessed_python`.
 
 ```python
 from torcheeg.datasets import DEAPDataset
 from torcheeg import transforms
 
-from torcheeg.datasets.constants.emotion_recognition.deap import \
+from torcheeg.datasets.constants import \
     DEAP_CHANNEL_LOCATION_DICT
 
 dataset = DEAPDataset(
     io_path=f'./tmp_out/examples_pipeline/deap',
     root_path='./tmp_in/data_preprocessed_python',
     offline_transform=transforms.Compose([
         transforms.BandDifferentialEntropy(apply_to_baseline=True),
@@ -251,41 +251,63 @@
         <a href="https://github.com/talhaanwarch">
             <img src="https://avatars.githubusercontent.com/u/37379131?v=4" width="100;" alt="talhaanwarch"/>
             <br />
             <sub><b>Talha Anwar</b></sub>
         </a>
     </td>
     <td align="center">
+        <a href="https://github.com/wufei-png">
+            <img src="https://avatars.githubusercontent.com/u/63766429?v=4" width="100;" alt="wufei-png"/>
+            <br />
+            <sub><b>Wu Fei</b></sub>
+        </a>
+    </td>
+    <td align="center">
         <a href="https://github.com/MicheleBarsotti">
             <img src="https://avatars.githubusercontent.com/u/48720814?v=4" width="100;" alt="MicheleBarsotti"/>
             <br />
             <sub><b>Meekele_b</b></sub>
         </a>
     </td>
     <td align="center">
         <a href="https://github.com/dawin2015">
             <img src="https://avatars.githubusercontent.com/u/12325204?v=4" width="100;" alt="dawin2015"/>
             <br />
             <sub><b>Liu-darong</b></sub>
         </a>
-    </td>
+    </td></tr>
+<tr>
     <td align="center">
         <a href="https://github.com/Nhix00">
             <img src="https://avatars.githubusercontent.com/u/75837033?v=4" width="100;" alt="Nhix00"/>
             <br />
             <sub><b>Nhix</b></sub>
         </a>
-    </td></tr>
-<tr>
+    </td>
     <td align="center">
         <a href="https://github.com/gitter-badger">
             <img src="https://avatars.githubusercontent.com/u/8518239?v=4" width="100;" alt="gitter-badger"/>
             <br />
             <sub><b>The Gitter Badger</b></sub>
         </a>
     </td></tr>
 </table>
 <!-- readme: collaborators,contributors -end -->
 
 ## License
 
-TorchEEG has a MIT license, as found in the [LICENSE](https://github.com/torcheeg/torcheeg/blob/main/LICENSE) file.
+TorchEEG has a MIT license, as found in the [LICENSE](https://github.com/torcheeg/torcheeg/blob/main/LICENSE) file.
+
+## Citation
+
+If you find this project useful for your research, please cite:
+
+```latex
+@article{zhang2024torcheeg,
+    title = {{TorchEEGEMO}: A deep learning toolbox towards {EEG}-based emotion recognition},
+    journal = {Expert Systems with Applications},
+    pages = {123550},
+    year = {2024},
+    issn = {0957-4174},
+    author = {Zhi Zhang and Sheng-hua Zhong and Yan Liu}
+}
+```
```

### Comparing `torcheeg-1.1.1/README.rst` & `torcheeg-1.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 TorchEEG
 ========
 
 |PyPI Version| |Docs Status| |Downloads| |Join the Chat|
 
 `Documentation <https://torcheeg.readthedocs.io/>`__ \| `TorchEEG
-Examples <https://github.com/tczhangzhi/torcheeg/tree/main/examples>`__
+Examples <https://github.com/torcheeg/torcheeg/tree/main/examples>`__ \|
+`Paper <https://www.sciencedirect.com/science/article/pii/S0957417424004159>`__
 
 TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG
 aims to provide a plug-and-play EEG analysis tool, so that researchers
 can quickly reproduce EEG analysis work and start new EEG analysis
 research without paying attention to technical details unrelated to the
 research focus.
 
@@ -251,15 +252,15 @@
 e.g. ``./tmp_in/data_preprocessed_python``.
 
 .. code:: python
 
    from torcheeg.datasets import DEAPDataset
    from torcheeg import transforms
 
-   from torcheeg.datasets.constants.emotion_recognition.deap import \
+   from torcheeg.datasets.constants import \
        DEAP_CHANNEL_LOCATION_DICT
 
    dataset = DEAPDataset(
        io_path=f'./tmp_out/examples_pipeline/deap',
        root_path='./tmp_in/data_preprocessed_python',
        offline_transform=transforms.Compose([
            transforms.BandDifferentialEntropy(apply_to_baseline=True),
@@ -362,14 +363,30 @@
 License
 -------
 
 TorchEEG has a MIT license, as found in the
 `LICENSE <https://github.com/tczhangzhi/torcheeg/blob/main/LICENSE>`__
 file.
 
+Citation
+--------
+
+If you find this project useful for your research, please cite:
+
+.. code:: latex
+
+   @article{zhang2024torcheeg,
+       title = {{TorchEEGEMO}: A deep learning toolbox towards {EEG}-based emotion recognition},
+       journal = {Expert Systems with Applications},
+       pages = {123550},
+       year = {2024},
+       issn = {0957-4174},
+       author = {Zhi Zhang and Sheng-hua Zhong and Yan Liu}
+   }
+
 .. |PyPI Version| image:: https://badge.fury.io/py/torcheeg.svg
    :target: https://pypi.python.org/pypi/torcheeg
 .. |Docs Status| image:: https://readthedocs.org/projects/torcheeg/badge/?version=latest
    :target: https://torcheeg.readthedocs.io/en/latest/?badge=latest
 .. |Downloads| image:: https://pepy.tech/badge/torcheeg
    :target: https://pepy.tech/project/torcheeg
 .. |Join the Chat| image:: https://badges.gitter.im/torcheeg/community.svg
```

### Comparing `torcheeg-1.1.1/setup.py` & `torcheeg-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 URL = 'https://github.com/tczhangzhi/torcheeg'
 
 install_requires = [
-    'tqdm>=4.64.0', 'numpy>=1.21.5', 'pandas>=1.3.5', 'scipy>=1.7.3',
-    'scikit-learn>=1.0.2', 'lmdb>=1.3.0', 'einops>=0.4.1', 'mne>=1.0.3',
-    'xmltodict>=0.13.0', 'networkx>=2.6.3', 'PyWavelets>=1.3.0',
+    'tqdm>=4.64.0', 'numpy>=1.21.5', 'pandas>=1.3.5', 'xlrd>=2.0.1',
+    'scipy>=1.7.3', 'scikit-learn>=1.0.2', 'lmdb>=1.3.0', 'einops>=0.4.1',
+    'mne>=1.0.3', 'xmltodict>=0.13.0', 'networkx>=2.6.3', 'PyWavelets>=1.3.0',
     'spectrum>=0.8.1', 'torchmetrics>=0.10.0', 'mne_connectivity>=0.4.0',
     'pytorch-lightning>=1.9.5'
 ]
 
 test_requires = ['pytest>=7.1.2']
 
 example_requires = []
@@ -25,15 +25,15 @@
 
 moabb_requires = ['moabb>=0.5.0']
 
 readme = open('README.rst').read()
 
 setup(
     name='torcheeg',
-    version='1.1.1',
+    version='1.1.2',
     description=
     'TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG aims to provide a plug-and-play EEG analysis tool, so that researchers can quickly reproduce EEG analysis work and start new EEG analysis research without paying attention to technical details unrelated to the research focus.',
     license='MIT',
     author='TorchEEG Team',
     author_email='tczhangzhi@gmail.com',
     keywords=['PyTorch', 'EEG'],
     url=URL,
```

### Comparing `torcheeg-1.1.1/test/datasets/test_emotion_recognition.py` & `torcheeg-1.1.2/test/datasets/test_emotion_recognition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,93 @@
 import os
 import random
 import shutil
 import unittest
 
 from torcheeg import transforms
-from torcheeg.datasets import (AMIGOSDataset, DEAPDataset, DREAMERDataset,
-                               MAHNOBDataset, SEEDDataset, SEEDFeatureDataset,
-                               SEEDIVDataset, SEEDIVFeatureDataset,
-                               MPEDFeatureDataset, BCI2022Dataset)
+from torcheeg.datasets import (
+    AMIGOSDataset, BCI2022Dataset, DEAPDataset, DREAMERDataset, FACEDDataset,
+    FACEDFeatureDataset, MAHNOBDataset, MPEDFeatureDataset, SEEDDataset,
+    SEEDFeatureDataset, SEEDIVDataset, SEEDIVFeatureDataset, SEEDVDataset,
+    SEEDVFeatureDataset)
 
 
 class TestEmotionRecognitionDataset(unittest.TestCase):
+
     def setUp(self):
         if os.path.exists('./tmp_out/'):
             shutil.rmtree('./tmp_out/')
         os.mkdir('./tmp_out/')
 
+    def test_faced_dataset(self):
+        io_path = f'./tmp_out/faced_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
+        root_path = './tmp_in/Processed_data'
+
+        dataset = FACEDDataset(io_path=io_path,
+                               root_path=root_path,
+                               online_transform=transforms.ToTensor(),
+                               label_transform=transforms.Select('emotion'),
+                               num_worker=4)
+        self.assertEqual(len(dataset), 103320)  # 123 subjects * 28 videos * 30s
+        first_item = dataset[0]
+        self.assertEqual(first_item[0].shape, (30, 250))
+        last_item = dataset[103319]
+        self.assertEqual(last_item[0].shape, (30, 250))
+
+    def test_faced_feature_dataset(self):
+        io_path = f'./tmp_out/faced_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
+        root_path = './tmp_in/EEG_Features/DE'
+
+        dataset = FACEDFeatureDataset(
+            io_path=io_path,
+            root_path=root_path,
+            online_transform=transforms.ToTensor(),
+            label_transform=transforms.Select('emotion'),
+            num_worker=4)
+
+        self.assertEqual(len(dataset),
+                         103320)  # 123 subjects * 28 videos * 30 s
+        first_item = dataset[0]
+        self.assertEqual(first_item[0].shape, (30, 5))
+        last_item = dataset[103319]
+        self.assertEqual(last_item[0].shape, (30, 5))
+
+    def test_seed_v_dataset(self):
+        io_path = f'./tmp_out/seed_v_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
+        root_path = './tmp_in/EEG_raw'
+
+        dataset = SEEDVDataset(io_path=io_path,
+                               root_path=root_path,
+                               online_transform=transforms.ToTensor(),
+                               label_transform=transforms.Select('emotion'),
+                               num_worker=4)
+
+        self.assertEqual(len(dataset), 29168)
+        first_item = dataset[0]
+        self.assertEqual(first_item[0].shape, (62, 800))
+        last_item = dataset[29167]
+        self.assertEqual(last_item[0].shape, (62, 800))
+
+    def test_seed_v_feature_dataset(self):
+        io_path = f'./tmp_out/seed_v_feature_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
+        root_path = './tmp_in/EEG_DE_features'
+
+        dataset = SEEDVFeatureDataset(
+            io_path=io_path,
+            root_path=root_path,
+            online_transform=transforms.ToTensor(),
+            label_transform=transforms.Select('emotion'),
+            num_worker=4)
+
+        self.assertEqual(len(dataset), 29168)
+        first_item = dataset[0]
+        self.assertEqual(first_item[0].shape, (62, 5))
+        last_item = dataset[29167]
+        self.assertEqual(last_item[0].shape, (62, 5))
+
     def test_mped_feature_dataset(self):
         io_path = f'./tmp_out/mped_feature_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
         root_path = './tmp_in/EEG_feature'
 
         dataset = MPEDFeatureDataset(
             io_path=io_path,
             root_path=root_path,
@@ -108,33 +176,14 @@
 
         self.assertEqual(len(dataset), 85744)
         first_item = dataset[0]
         self.assertEqual(first_item[0].shape, (14, 128))
         last_item = dataset[85743]
         self.assertEqual(last_item[0].shape, (14, 128))
 
-    def test_seed_dataset(self):
-        io_path = f'./tmp_out/seed_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
-        root_path = './tmp_in/Preprocessed_EEG'
-
-        dataset = SEEDDataset(io_path=io_path,
-                              root_path=root_path,
-                              online_transform=transforms.ToTensor(),
-                              label_transform=transforms.Compose([
-                                  transforms.Select('emotion'),
-                                  transforms.Lambda(lambda x: int(x) + 1),
-                              ]),
-                              num_worker=4)
-
-        self.assertEqual(len(dataset), 152730)
-        first_item = dataset[0]
-        self.assertEqual(first_item[0].shape, (62, 200))
-        last_item = dataset[152729]
-        self.assertEqual(last_item[0].shape, (62, 200))
-
     def test_seed_feature_dataset(self):
         io_path = f'./tmp_out/seed_feature_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
         root_path = './tmp_in/ExtractedFeatures'
 
         dataset = SEEDFeatureDataset(
             io_path=io_path,
             root_path=root_path,
```

### Comparing `torcheeg-1.1.1/test/datasets/test_folder.py` & `torcheeg-1.1.2/test/datasets/test_folder.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/datasets/test_hooks.py` & `torcheeg-1.1.2/test/transforms/test_any.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,75 @@
-import os
-import random
-import shutil
 import unittest
 
-from torcheeg import transforms
-from torcheeg.datasets import DEAPDataset
-from torcheeg.datasets.functional.hooks import before_trial_normalize, after_trial_normalize, after_trial_moving_avg
-
-
-class TestHooks(unittest.TestCase):
-    def setUp(self):
-        if os.path.exists('./tmp_out/'):
-            shutil.rmtree('./tmp_out/')
-        os.mkdir('./tmp_out/')
-
-    def test_before_trial_after_trial(self):
-        io_path = f'./tmp_out/deap_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
-        root_path = './tmp_in/data_preprocessed_python'
-
-        dataset = DEAPDataset(io_path=io_path,
-                              root_path=root_path,
-                              online_transform=transforms.ToTensor(),
-                              label_transform=transforms.Compose([
-                                  transforms.Select('valence'),
-                                  transforms.Binary(5.0),
-                              ]),
-                              num_worker=4,
-                              before_trial=before_trial_normalize)
-        self.assertEqual(len(dataset), 76800)
-        first_item = dataset[0]
-        self.assertEqual(first_item[0].shape, (32, 128))
-        last_item = dataset[76799]
-        self.assertEqual(last_item[0].shape, (32, 128))
-
-        io_path = f'./tmp_out/deap_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
-        dataset = DEAPDataset(io_path=io_path,
-                              root_path=root_path,
-                              online_transform=transforms.ToTensor(),
-                              label_transform=transforms.Compose([
-                                  transforms.Select('valence'),
-                                  transforms.Binary(5.0),
-                              ]),
-                              num_worker=4,
-                              after_trial=after_trial_normalize)
-        self.assertEqual(len(dataset), 76800)
-        first_item = dataset[0]
-        self.assertEqual(first_item[0].shape, (32, 128))
-        last_item = dataset[76799]
-        self.assertEqual(last_item[0].shape, (32, 128))
-
-        io_path = f'./tmp_out/deap_{"".join(random.sample("zyxwvutsrqponmlkjihgfedcba", 20))}'
-        dataset = DEAPDataset(io_path=io_path,
-                              root_path=root_path,
-                              online_transform=transforms.ToTensor(),
-                              label_transform=transforms.Compose([
-                                  transforms.Select('valence'),
-                                  transforms.Binary(5.0),
-                              ]),
-                              num_worker=4,
-                              after_trial=after_trial_moving_avg)
-        self.assertEqual(len(dataset), 76800)
-        first_item = dataset[0]
-        self.assertEqual(first_item[0].shape, (32, 128))
-        last_item = dataset[76799]
-        self.assertEqual(last_item[0].shape, (32, 128))
+import torch
+import numpy as np
+
+from torcheeg.transforms import BaselineRemoval, Lambda, Compose, ToTensor, Resize, RandomNoise, RandomMask, BandDifferentialEntropy, MeanStdNormalize, ToGrid, Select, Binary
+from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+
+
+class TestAnyTransforms(unittest.TestCase):
+    def test_to_baseline_removal(self):
+        transform = Compose([
+            ToTensor(apply_to_baseline=True),
+            Resize(size=(64, 64), apply_to_baseline=True),
+            RandomNoise(p=0.1),
+            RandomMask(p=0.1),
+            BaselineRemoval()
+        ])
+        transformed_eeg = transform(eeg=np.random.randn(128, 9, 9),
+                                    baseline=np.random.randn(128, 9, 9))['eeg']
+        self.assertTrue(tuple(transformed_eeg.shape), (128, 64, 64))
+
+        eeg = np.random.randn(128, 9, 9)
+        transform = BaselineRemoval()
+        transformed_eeg = transform(eeg=eeg, baseline=np.ones(
+            (128, 9, 9)))['eeg']
+        self.assertTrue(np.abs(eeg - (transformed_eeg + 1.0)).sum() < 1e-6)
+        
+        transform = BaselineRemoval()
+        transformed_eeg = transform(eeg=eeg)['eeg']
+        self.assertTrue(np.abs(eeg - transformed_eeg).sum() < 1e-6)
+
+    def test_lambda(self):
+        # label
+        transform = Lambda(lambd=lambda x: x + 1)
+        self.assertEqual(transform(y=1)['y'], 2)
+        # torch
+        transform = Lambda(targets=['eeg'], lambd=lambda x: x + 1)
+        self.assertEqual(
+            tuple(transform(eeg=torch.randn(32, 128))['eeg'].shape), (32, 128))
+        # numpy
+        self.assertEqual(
+            transform(eeg=np.random.randn(32, 128))['eeg'].shape, (32, 128))
+
+    def test_compose(self):
+        # torch
+        transform = Compose([
+            ToTensor(),
+            Resize(size=(64, 64)),
+            RandomNoise(p=0.1),
+            RandomMask(p=0.1)
+        ])
+
+        self.assertEqual(
+            tuple(transform(eeg=np.random.randn(128, 9, 9))['eeg'].shape),
+            (128, 64, 64))
+
+        # numpy
+        transform = Compose([
+            BandDifferentialEntropy(),
+            MeanStdNormalize(),
+            ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+        ])
+        self.assertEqual(
+            tuple(transform(eeg=np.random.randn(32, 128))['eeg'].shape),
+            (4, 9, 9))
+
+        # label
+        info = {'valence': 4.5, 'arousal': 5.5, 'subject_id': 7}
+        transform = Compose([Select(key='valence'), Binary(threshold=5.0)])
+        self.assertEqual(transform(y=info)['y'], 0)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `torcheeg-1.1.1/test/datasets/test_motor_imagery.py` & `torcheeg-1.1.2/test/datasets/test_motor_imagery.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/datasets/test_personal_identification.py` & `torcheeg-1.1.2/test/datasets/test_personal_identification.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/datasets/test_ssvep.py` & `torcheeg-1.1.2/test/datasets/test_ssvep.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/io/test_eeg_signal.py` & `torcheeg-1.1.2/test/io/test_eeg_signal.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/io/test_meta_info.py` & `torcheeg-1.1.2/test/io/test_meta_info.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_k_fold.py` & `torcheeg-1.1.2/test/model_selection/test_k_fold.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_k_fold_cross_subject.py` & `torcheeg-1.1.2/test/model_selection/test_k_fold_cross_subject.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_k_fold_cross_trial.py` & `torcheeg-1.1.2/test/model_selection/test_k_fold_cross_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_k_fold_groupby_trial.py` & `torcheeg-1.1.2/test/model_selection/test_k_fold_groupby_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_k_fold_per_subject_cross_trial.py` & `torcheeg-1.1.2/test/model_selection/test_k_fold_per_subject_cross_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_k_fold_per_subject_groupby_trial.py` & `torcheeg-1.1.2/test/model_selection/test_k_fold_per_subject_groupby_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_leave_one_subject_out.py` & `torcheeg-1.1.2/test/model_selection/test_leave_one_subject_out.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_split.py` & `torcheeg-1.1.2/test/model_selection/test_split.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_split_cross_trial.py` & `torcheeg-1.1.2/test/model_selection/test_split_cross_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_split_groupby_trial.py` & `torcheeg-1.1.2/test/model_selection/test_split_groupby_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_split_per_subject_cross_trial.py` & `torcheeg-1.1.2/test/model_selection/test_split_per_subject_cross_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_split_per_subject_groupby_trial.py` & `torcheeg-1.1.2/test/model_selection/test_split_per_subject_groupby_trial.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/model_selection/test_subcategory.py` & `torcheeg-1.1.2/test/model_selection/test_subcategory.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_cnn.py` & `torcheeg-1.1.2/test/models/test_cnn.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_ddpm.py` & `torcheeg-1.1.2/test/models/test_ddpm.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_flow.py` & `torcheeg-1.1.2/test/models/test_flow.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_gan.py` & `torcheeg-1.1.2/test/models/test_gan.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_gnn.py` & `torcheeg-1.1.2/test/models/test_gnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import torch
 from torch_geometric.data import Batch, Data
 
-from torcheeg.datasets.constants.emotion_recognition.deap import \
+from torcheeg.datasets.constants import \
     DEAP_GENERAL_REGION_LIST
 from torcheeg.models import DGCNN, LGGNet
 from torcheeg.models.pyg import GIN, RGNN
 
 
 class TestGNN(unittest.TestCase):
```

### Comparing `torcheeg-1.1.1/test/models/test_rnn.py` & `torcheeg-1.1.2/test/models/test_rnn.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_transformer.py` & `torcheeg-1.1.2/test/models/test_transformer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/models/test_vae.py` & `torcheeg-1.1.2/test/models/test_vae.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_classifier_trainer.py` & `torcheeg-1.1.2/test/trainers/test_classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_ddpm_trainer.py` & `torcheeg-1.1.2/test/trainers/test_ddpm_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_domain_adaption_trainer.py` & `torcheeg-1.1.2/test/trainers/test_domain_adaption_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_gan_trainer.py` & `torcheeg-1.1.2/test/trainers/test_gan_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_glow_trainer.py` & `torcheeg-1.1.2/test/trainers/test_glow_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_imbalance_trainer.py` & `torcheeg-1.1.2/test/trainers/test_imbalance_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_self_supervised_trainer.py` & `torcheeg-1.1.2/test/trainers/test_self_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/trainers/test_vae_trainer.py` & `torcheeg-1.1.2/test/trainers/test_vae_trainer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/transforms/test_any.py` & `torcheeg-1.1.2/test/transforms/test_pyg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,48 @@
 import unittest
 
-import torch
 import numpy as np
+import torch
+from torch_geometric.data import Data
+from torcheeg.datasets.constants import DEAP_ADJACENCY_MATRIX
+from torcheeg.transforms.pyg import ToDynamicG, ToG
+
+
+class TestPyGTransforms(unittest.TestCase):
+    def test_to_g(self):
+        eeg = np.random.randn(32, 128)
+        transformed_eeg = ToG(DEAP_ADJACENCY_MATRIX)(eeg=eeg)['eeg']
+        self.assertTrue(isinstance(transformed_eeg, Data))
+
+        eeg = torch.randn(32, 128)
+        transformed_eeg = ToG(DEAP_ADJACENCY_MATRIX)(eeg=eeg)['eeg']
+        self.assertTrue(isinstance(transformed_eeg, Data))
+
+    def test_to_dynamic_g(self):
+        eeg = np.random.randn(32, 128)
+        transform = ToDynamicG(edge_func='gaussian_distance', sigma=1.0, top_k=10, complete_graph=False)
+        transformed_eeg = transform(eeg=eeg)['eeg']
+        self.assertTrue(isinstance(transformed_eeg, Data))
 
-from torcheeg.transforms import BaselineRemoval, Lambda, Compose, ToTensor, Resize, RandomNoise, RandomMask, BandDifferentialEntropy, MeanStdNormalize, ToGrid, Select, Binary
-from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        eeg = torch.randn(32, 128)
+        transform = ToDynamicG(edge_func='gaussian_distance', sigma=1.0, top_k=10, complete_graph=False)
+        transformed_eeg = transform(eeg=eeg)['eeg']
+        self.assertTrue(isinstance(transformed_eeg, Data))
 
+        eeg = np.random.randn(32, 128)
+        transform = ToDynamicG(edge_func='absolute_pearson_correlation_coefficient', threshold=0.1, binary=True)
+        transformed_eeg = transform(eeg=eeg)['eeg']
+        self.assertTrue(isinstance(transformed_eeg, Data))
 
-class TestAnyTransforms(unittest.TestCase):
-    def test_to_baseline_removal(self):
-        transform = Compose([
-            ToTensor(apply_to_baseline=True),
-            Resize(size=(64, 64), apply_to_baseline=True),
-            RandomNoise(p=0.1),
-            RandomMask(p=0.1),
-            BaselineRemoval()
-        ])
-        transformed_eeg = transform(eeg=np.random.randn(128, 9, 9),
-                                    baseline=np.random.randn(128, 9, 9))['eeg']
-        self.assertTrue(tuple(transformed_eeg.shape), (128, 64, 64))
-
-        eeg = np.random.randn(128, 9, 9)
-        transform = BaselineRemoval()
-        transformed_eeg = transform(eeg=eeg, baseline=np.ones(
-            (128, 9, 9)))['eeg']
-        self.assertTrue(np.abs(eeg - (transformed_eeg + 1.0)).sum() < 1e-6)
-        
-        transform = BaselineRemoval()
+        eeg = np.random.randn(32, 128)
+        transform = ToDynamicG(edge_func='phase_locking_value')
         transformed_eeg = transform(eeg=eeg)['eeg']
-        self.assertTrue(np.abs(eeg - transformed_eeg).sum() < 1e-6)
+        self.assertTrue(isinstance(transformed_eeg, Data))
 
-    def test_lambda(self):
-        # label
-        transform = Lambda(lambd=lambda x: x + 1)
-        self.assertEqual(transform(y=1)['y'], 2)
-        # torch
-        transform = Lambda(targets=['eeg'], lambd=lambda x: x + 1)
-        self.assertEqual(
-            tuple(transform(eeg=torch.randn(32, 128))['eeg'].shape), (32, 128))
-        # numpy
-        self.assertEqual(
-            transform(eeg=np.random.randn(32, 128))['eeg'].shape, (32, 128))
-
-    def test_compose(self):
-        # torch
-        transform = Compose([
-            ToTensor(),
-            Resize(size=(64, 64)),
-            RandomNoise(p=0.1),
-            RandomMask(p=0.1)
-        ])
-
-        self.assertEqual(
-            tuple(transform(eeg=np.random.randn(128, 9, 9))['eeg'].shape),
-            (128, 64, 64))
-
-        # numpy
-        transform = Compose([
-            BandDifferentialEntropy(),
-            MeanStdNormalize(),
-            ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-        ])
-        self.assertEqual(
-            tuple(transform(eeg=np.random.randn(32, 128))['eeg'].shape),
-            (4, 9, 9))
-
-        # label
-        info = {'valence': 4.5, 'arousal': 5.5, 'subject_id': 7}
-        transform = Compose([Select(key='valence'), Binary(threshold=5.0)])
-        self.assertEqual(transform(y=info)['y'], 0)
+        eeg = np.random.randn(32, 128)
+        transform = ToDynamicG(edge_func=lambda x, y: (x * y).mean())
+        transformed_eeg = transform(eeg=eeg)['eeg']
+        self.assertTrue(isinstance(transformed_eeg, Data))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `torcheeg-1.1.1/test/transforms/test_label.py` & `torcheeg-1.1.2/test/transforms/test_label.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/transforms/test_numpy.py` & `torcheeg-1.1.2/test/transforms/test_numpy.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/transforms/test_pyg.py` & `torcheeg-1.1.2/torcheeg/transforms/any/compose.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,69 @@
-import unittest
+from typing import Callable, List
 
-import numpy as np
-import torch
-from torch_geometric.data import Data
-from torcheeg.datasets.constants import DEAP_ADJACENCY_MATRIX
-from torcheeg.transforms.pyg import ToDynamicG, ToG
-
-
-class TestPyGTransforms(unittest.TestCase):
-    def test_to_g(self):
-        eeg = np.random.randn(32, 128)
-        transformed_eeg = ToG(DEAP_ADJACENCY_MATRIX)(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
-
-        eeg = torch.randn(32, 128)
-        transformed_eeg = ToG(DEAP_ADJACENCY_MATRIX)(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
-
-    def test_to_dynamic_g(self):
-        eeg = np.random.randn(32, 128)
-        transform = ToDynamicG(edge_func='gaussian_distance', sigma=1.0, top_k=10, complete_graph=False)
-        transformed_eeg = transform(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
-
-        eeg = torch.randn(32, 128)
-        transform = ToDynamicG(edge_func='gaussian_distance', sigma=1.0, top_k=10, complete_graph=False)
-        transformed_eeg = transform(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
-
-        eeg = np.random.randn(32, 128)
-        transform = ToDynamicG(edge_func='absolute_pearson_correlation_coefficient', threshold=0.1, binary=True)
-        transformed_eeg = transform(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
-
-        eeg = np.random.randn(32, 128)
-        transform = ToDynamicG(edge_func='phase_locking_value')
-        transformed_eeg = transform(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
-
-        eeg = np.random.randn(32, 128)
-        transform = ToDynamicG(edge_func=lambda x, y: (x * y).mean())
-        transformed_eeg = transform(eeg=eeg)['eeg']
-        self.assertTrue(isinstance(transformed_eeg, Data))
+from ..base_transform import BaseTransform
 
 
-if __name__ == '__main__':
-    unittest.main()
+class Compose(BaseTransform):
+    r'''
+    Compose several transforms together. Consistent with :obj:`torchvision.transforms.Compose`'s behavior.
+
+    .. code-block:: python
+
+        from torcheeg import transforms
+
+        t = transforms.Compose([
+            transforms.ToTensor(),
+            transforms.Resize(size=(64, 64)),
+            transforms.RandomNoise(p=0.1),
+            transforms.RandomMask(p=0.1)
+        ])
+        t(eeg=torch.randn(128, 9, 9))['eeg'].shape
+        >>> (128, 64, 64)
+
+    :obj:`Compose` supports transformers with different data dependencies. The above example combines multiple torch-based transformers, the following example shows a sequence of numpy-based transformer.
+
+    .. code-block:: python
+
+        from torcheeg import transforms
+
+        t = transforms.Compose([
+            transforms.BandDifferentialEntropy(),
+            transforms.MeanStdNormalize(),
+            transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+        ])
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
+        >>> (128, 9, 9)
+
+    Args:
+        transforms (list): The list of transforms to compose.
+
+    .. automethod:: __call__
+    '''
+    def __init__(self, transforms: List[Callable]):
+        super(Compose, self).__init__()
+        self.transforms = transforms
+
+    def __call__(self, *args, **kwargs) -> any:
+        r'''
+        Args:
+            x (any): The input.
+
+        Returns:
+            any: The transformed output.
+        '''
+        if args:
+            raise KeyError("Please pass data as named parameters.")
+
+        for t in self.transforms:
+            kwargs = t(**kwargs)
+        return kwargs
+
+    def __repr__(self) -> str:
+        format_string = self.__class__.__name__ + '('
+        for i, t in enumerate(self.transforms):
+            if i:
+                format_string += ','
+            format_string += '\n'
+            format_string += f'    {t}'
+        format_string += '\n)'
+        return format_string
```

### Comparing `torcheeg-1.1.1/test/transforms/test_torch.py` & `torcheeg-1.1.2/test/transforms/test_torch.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/test/utils/test_visualize.py` & `torcheeg-1.1.2/test/utils/test_visualize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 import numpy as np
 import torch
-from torcheeg.datasets.constants.emotion_recognition.deap import (DEAP_ADJACENCY_MATRIX, DEAP_CHANNEL_LIST,
-                                                                  DEAP_CHANNEL_LOCATION_DICT, DEAP_LOCATION_LIST)
-from torcheeg.datasets.constants.emotion_recognition.seed import \
+from torcheeg.datasets.constants import (DEAP_ADJACENCY_MATRIX, DEAP_CHANNEL_LIST,
+                                                                  DEAP_CHANNEL_LOCATION_DICT)
+from torcheeg.datasets.constants import \
     SEED_CHANNEL_LIST, SEED_GENERAL_REGION_LIST
 from torcheeg.transforms.pyg import ToG
 from torcheeg.utils import (plot_2d_tensor, plot_3d_tensor, plot_feature_topomap, plot_raw_topomap, plot_signal,
                             plot_adj_connectivity)
 from torcheeg.utils.pyg import plot_graph
 
 
@@ -21,14 +21,18 @@
 
     def test_plot_feature_topomap(self):
         mock_eeg = torch.randn(32, 4)
         img = plot_feature_topomap(mock_eeg,
                                    channel_list=DEAP_CHANNEL_LIST,
                                    feature_list=["theta", "alpha", "beta", "gamma"])
         self.assertEqual(img.shape, (347, 1550, 4))
+        img = plot_feature_topomap(mock_eeg,
+                                   channel_list=DEAP_CHANNEL_LIST,
+                                   feature_list=["theta", "alpha", "beta", "gamma"],fig_shape=(2,2))
+        self.assertEqual(img.shape, (784, 774, 4))
 
     def test_plot_signal(self):
         mock_eeg = torch.randn(32, 128)
         img = plot_signal(mock_eeg, channel_list=DEAP_CHANNEL_LIST, sampling_rate=128)
         self.assertEqual(img.shape, (773, 727, 4))
 
     def test_plot_3d_tensor(self):
```

### Comparing `torcheeg-1.1.1/torcheeg/__init__.py` & `torcheeg-1.1.2/torcheeg/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import mne
 import logging
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 
 def set_log_level(level: str = "INFO", third_party: str = "CRITICAL"):
     """
     Set log level for torcheeg.
 
     Args:
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/clinical/tuh_tueg.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/clinical/tuh_tueg.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/amigos.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/amigos.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/bci2022.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/bci2022.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/deap.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/deap.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/dreamer.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/dreamer.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/mahnob.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/mahnob.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/mped.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/mped.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/seed.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/seed.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/emotion_recognition/seed_iv.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/emotion_recognition/seed_iv.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/personal_identification/m3cv.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/personal_identification/m3cv.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/region_1020.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/region_1020.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/ssvep/tsu_benchmark.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/ssvep/tsu_benchmark.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/standard_1005.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/standard_1005.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/standard_1020.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/standard_1020.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/constants/utils.py` & `torcheeg-1.1.2/torcheeg/datasets/constants/utils.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/datasets/moabb/moabb_dataset.py` & `torcheeg-1.1.2/torcheeg/datasets/moabb/moabb_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     '''
     Mother of all BCI Benchmarks (MoABB) aims at building a comprehensive benchmark of popular Brain-Computer Interface (BCI) algorithms applied on an extensive list of freely available EEG datasets. This class implements the conversion of MOABB datasets to TorchEEG datasets, allowing to import any MOABB datasets to use them like TorchEEG datasets.
 
     A tiny case shows the use of :obj:`MOABBDataset`:
 
     .. code-block:: python
         
+        from moabb.datasets import BNCI2014001
+        from moabb.paradigms import LeftRightImagery
+        
+        from torcheeg import transforms
         import torcheeg.datasets.moabb as moabb_dataset
 
         dataset = BNCI2014001()
         dataset.subject_list = [1, 2, 3]
         paradigm = LeftRightImagery()
         dataset = moabb_dataset.MOABBDataset(dataset=dataset,
                                paradigm=paradigm,
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/base_dataset.py` & `torcheeg-1.1.2/torcheeg/datasets/module/base_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,16 @@
             log.info(
                 f'🔍 | Detected cached processing results, reading cache from {self.io_path}.'
             )
             # get all records
             records = os.listdir(io_path)
             # filter the records with the prefix '_record_'
             records = list(filter(lambda x: '_record_' in x, records))
+            # sort the records
+            records = sorted(records, key=lambda x: int(x.split('_')[2]))
 
             # for every record, get the io_path, and init the info_io and eeg_io
             eeg_io_router = {}
             info_merged = []
 
             assert len(
                 records
@@ -292,36 +294,36 @@
         if after_trial is None and after_session is None and after_subject is None:
             return
 
         if 'subject_id' in self.info.columns:
             subject_df = self.info.groupby('subject_id')
         else:
             subject_df = [(None, self.info)]
-            if not after_subject is None:
-                log.info(
-                    "No subject_id column found in info, after_subject hook is ignored."
-                )
+            # if not after_subject is None:
+            #     log.info(
+            #         "No subject_id column found in info, after_subject hook is ignored."
+            #     )
         if after_subject is None:
             after_subject = lambda x: x
 
         for _, subject_info in subject_df:
 
             subject_record_list = []
             subject_index_list = []
             subject_samples = []
 
             # check if have a session_id column
             if 'session_id' in subject_info.columns:
                 session_df = subject_info.groupby('session_id')
             else:
                 session_df = [(None, subject_info)]
-                if not after_session is None:
-                    log.info(
-                        "No session_id column found in info, after_session hook is ignored."
-                    )
+                # if not after_session is None:
+                #     log.info(
+                #         "No session_id column found in info, after_session hook is ignored."
+                #     )
             if after_session is None:
                 after_session = lambda x: x
 
             for _, session_info in session_df:
 
                 # check if have a trial_id column
                 if 'trial_id' in session_info.columns:
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/csv_folder_dataset.py` & `torcheeg-1.1.2/torcheeg/datasets/module/csv_folder_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         # | sub1       | 0        | 0     | './data/label1/sub1.fif' |
         # | sub1       | 1        | 1     | './data/label2/sub1.fif' |
         # | sub1       | 2        | 2     | './data/label3/sub1.fif' |
         # | sub2       | 0        | 0     | './data/label1/sub2.fif' |
         # | sub2       | 1        | 1     | './data/label2/sub2.fif' |
         # | sub2       | 2        | 2     | './data/label3/sub2.fif' |
 
+        from torcheeg.datasets import CSVFolderDataset
+        from torcheeg import transforms
+
         def default_read_fn(file_path, **kwargs):
             # Load EEG file
             raw = mne.io.read_raw(file_path)
             # Convert raw to epochs
             epochs = mne.make_fixed_length_epochs(raw, duration=1)
             # Return EEG data
             return epochs
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/amigos.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/amigos.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,19 @@
     - ...
     - Data_Preprocessed_P40.mat
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import AMIGOSDataset
+        from torcheeg import transforms
+
+        from torcheeg.datasets.constants.emotion_recognition.amigos import AMIGOS_CHANNEL_LOCATION_DICT
+
         dataset = AMIGOSDataset(root_path='./data_preprocessed',
                                 offline_transform=transforms.Compose([
                                     transforms.BandDifferentialEntropy(),
                                     transforms.ToGrid(AMIGOS_CHANNEL_LOCATION_DICT)
                                 ]),
                                 online_transform=transforms.ToTensor(),
                                 label_transform=transforms.Compose([
@@ -50,14 +55,17 @@
         # coresponding baseline signal (torch.Tensor[4, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import AMIGOSDataset
+        from torcheeg import transforms
+
         dataset = AMIGOSDataset(root_path='./data_preprocessed',
                                 online_transform=transforms.Compose(
                                     [transforms.To2d(),
                                     transforms.ToTensor()]),
                                 label_transform=transforms.Compose([
                                     transforms.Select('valence'),
                                     transforms.Binary(5.0),
@@ -67,14 +75,20 @@
         # coresponding baseline signal (torch.Tensor[14, 128]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
     
+        from torcheeg.datasets import AMIGOSDataset
+        from torcheeg import transforms
+        from torcheeg.transforms.pyg import ToG
+
+        from torcheeg.datasets.constants.emotion_recognition.amigos import AMIGOS_ADJACENCY_MATRIX
+
         dataset = AMIGOSDataset(root_path='./data_preprocessed',
                                 online_transform=transforms.Compose(
                                     [ToG(AMIGOS_ADJACENCY_MATRIX)]),
                                 label_transform=transforms.Compose([
                                     transforms.Select('valence'),
                                     transforms.Binary(5.0),
                                 ]))
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/bci2022.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/bci2022.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,18 @@
         + sub59
         + ...
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import BCI2022Dataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import BCI2022_CHANNEL_LOCATION_DICT
+
         dataset = BCI2022Dataset(root_path='./TrainSet',
                                  offline_transform=transforms.Compose([
                                      transforms.BandDifferentialEntropy(),
                                      transforms.ToGrid(BCI2022_CHANNEL_LOCATION_DICT)
                                  ]),
                                  online_transform=transforms.ToTensor(),
                                  label_transform=transforms.Select('emotion'))
@@ -129,32 +133,47 @@
         # coresponding baseline signal (torch.Tensor[4, 8, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import BCI2022Dataset
+        from torcheeg import transforms
+
         dataset = BCI2022Dataset(root_path='./TrainSet',
                                  online_transform=transforms.Compose(
                                      [transforms.ToTensor(),
-                                     transforms.To2d()]),
-                                 label_transform=transforms.Select('emotion'))
+                                      transforms.To2d()]),
+                                 label_transform=transforms.Compose([
+                                     transforms.Select('emotion'),
+                                     transforms.Lambda(lambda x: x + 1)
+                                 ]))
+
         print(dataset[0])
         # EEG signal (torch.Tensor[30, 250]),
         # coresponding baseline signal (torch.Tensor[30, 250]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import BCI2022Dataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import BCI2022_ADJACENCY_MATRIX
+        
         dataset = BCI2022Dataset(root_path='./TrainSet',
                                  online_transform=transforms.Compose(
                                      [transforms.ToG(BCI2022_ADJACENCY_MATRIX)]),
-                                 label_transform=transforms.Select('emotion'))
+                                 label_transform=transforms.Compose([
+                                     transforms.Select('emotion'),
+                                     transforms.Lambda(lambda x: x + 1)
+                                 ]))
+
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
         # coresponding baseline signal (torch_geometric.data.Data),
         # label (int)
 
     Args:
         root_path (str): Downloaded data files in pickle (the TrainSet folder in unzipped 2022EmotionPublic.zip) formats (default: :obj:`'./TrainSet'`)
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/deap.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/dreamer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,118 +1,121 @@
 import os
-import pickle as pkl
-
-from typing import Any, Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Tuple, Union, Any
 
+import scipy.io as scio
 from ..base_dataset import BaseDataset
 from ....utils import get_random_dir_path
 
 
-class DEAPDataset(BaseDataset):
+class DREAMERDataset(BaseDataset):
     r'''
-    A multimodal dataset for the analysis of human affective states. This class generates training samples and test samples according to the given parameters, and caches the generated results in a unified input and output format (IO). The relevant information of the dataset is as follows:
-    
-    - Author: Koelstra et al.
-    - Year: 2012
-    - Download URL: https://www.eecs.qmul.ac.uk/mmv/datasets/deap/download.html
-    - Reference: Koelstra S, Muhl C, Soleymani M, et al. DEAP: A database for emotion analysis; using physiological signals[J]. IEEE transactions on affective computing, 2011, 3(1): 18-31.
-    - Stimulus: 40 one-minute long excerpts from music videos.
-    - Signals: Electroencephalogram (32 channels at 512Hz, downsampled to 128Hz), skinconductance level (SCL), respiration amplitude, skin temperature,electrocardiogram, blood volume by plethysmograph, electromyograms ofZygomaticus and Trapezius muscles (EMGs), electrooculogram (EOG), face video (for 22 participants).
-    - Rating: Arousal, valence, like/dislike, dominance (all ona scale from 1 to 9), familiarity (on a scale from 1 to 5).
-    
-    In order to use this dataset, the download folder :obj:`data_preprocessed_python` is required, containing the following files:
-    
-    - s01.dat
-    - s02.dat
-    - s03.dat
-    - ...
-    - s32.dat
+    A multi-modal database consisting of electroencephalogram and electrocardiogram signals recorded during affect elicitation by means of audio-visual stimuli. This class generates training samples and test samples according to the given parameters, and caches the generated results in a unified input and output format (IO). The relevant information of the dataset is as follows:
+
+    - Author: Katsigiannis et al.
+    - Year: 2017
+    - Download URL: https://zenodo.org/record/546113
+    - Reference: Katsigiannis S, Ramzan N. DREAMER: A database for emotion recognition through EEG and ECG signals from wireless low-cost off-the-shelf devices[J]. IEEE journal of biomedical and health informatics, 2017, 22(1): 98-107.
+    - Stimulus: 18 movie clips. 
+    - Signals: Electroencephalogram (14 channels at 128Hz), and electrocardiogram (2 channels at 256Hz) of 23 subjects.
+    - Rating: Arousal, valence, like/dislike, dominance, familiarity (all ona scale from 1 to 5).
+
+    In order to use this dataset, the download file :obj:`DREAMER.mat` is required.
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
-    
-        dataset = DEAPDataset(root_path='./data_preprocessed_python',
-                              offline_transform=transforms.Compose([
-                                  transforms.BandDifferentialEntropy(),
-                                  transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                              ]),
-                              online_transform=transforms.ToTensor(),
-                              label_transform=transforms.Compose([
-                                  transforms.Select('valence'),
-                                  transforms.Binary(5.0),
-                              ]))
+
+        from torcheeg.datasets import DREAMERDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DREAMER_CHANNEL_LOCATION_DICT
+
+        dataset = DREAMERDataset(mat_path='./DREAMER.mat',
+                                 offline_transform=transforms.Compose([
+                                     transforms.BandDifferentialEntropy(),
+                                     transforms.ToGrid(DREAMER_CHANNEL_LOCATION_DICT)
+                                 ]),
+                                 online_transform=transforms.ToTensor(),
+                                 label_transform=transforms.Compose([
+                                     transforms.Select('valence'),
+                                     transforms.Binary(3.0),
+                                 ]))
         print(dataset[0])
         # EEG signal (torch.Tensor[4, 9, 9]),
         # coresponding baseline signal (torch.Tensor[4, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(root_path='./data_preprocessed_python',
-                              online_transform=transforms.Compose([
-                                  transforms.To2d(),
-                                  transforms.ToTensor()
-                              ]),
-                              label_transform=transforms.Compose([
-                                  transforms.Select(['valence', 'arousal']),
-                                  transforms.Binary(5.0),
-                                  transforms.BinariesToCategory()
-                              ]))
+        from torcheeg.datasets import DREAMERDataset
+        from torcheeg import transforms
+
+        dataset = DREAMERDataset(mat_path='./DREAMER.mat',
+                                 online_transform=transforms.Compose([
+                                     transforms.To2d(),
+                                     transforms.ToTensor()
+                                 ]),
+                                 label_transform=transforms.Compose([
+                                     transforms.Select(['valence', 'arousal']),
+                                     transforms.Binary(3.0),
+                                     transforms.BinariesToCategory()
+                                 ]))
         print(dataset[0])
-        # EEG signal (torch.Tensor[1, 32, 128]),
-        # coresponding baseline signal (torch.Tensor[1, 32, 128]),
+        # EEG signal (torch.Tensor[1, 14, 128]),
+        # coresponding baseline signal (torch.Tensor[1, 14, 128]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
-        dataset = DEAPDataset(root_path='./data_preprocessed_python',
-                              online_transform=transforms.Compose([
-                                  ToG(DEAP_ADJACENCY_MATRIX)
-                              ]),
-                              label_transform=transforms.Compose([
-                                  transforms.Select('arousal'),
-                                  transforms.Binary(5.0)
-                              ]))
+        
+        from torcheeg.datasets import DREAMERDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DREAMER_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
+        dataset = DREAMERDataset(mat_path='./DREAMER.mat',
+                                 online_transform=transforms.Compose([
+                                     ToG(DREAMER_ADJACENCY_MATRIX)
+                                 ]),
+                                 label_transform=transforms.Compose([
+                                     transforms.Select('arousal'),
+                                     transforms.Binary(3.0)
+                                 ]))
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
         # coresponding baseline signal (torch_geometric.data.Data),
         # label (int)
-
-    In particular, TorchEEG utilizes the producer-consumer model to allow multi-process data preprocessing. If your data preprocessing is time consuming, consider increasing :obj:`num_worker` for higher speedup. If running under Windows, please use the proper idiom in the main module:
-
+    
     Args:
-        root_path (str): Downloaded data files in pickled python/numpy (unzipped data_preprocessed_python.zip) formats (default: :obj:`'./data_preprocessed_python'`)
+        mat_path (str): Downloaded data files in pickled matlab formats (default: :obj:`'./DREAMER.mat'`)
         chunk_size (int): Number of data points included in each EEG chunk as training or test samples. If set to -1, the EEG signal of a trial is used as a sample of a chunk. (default: :obj:`128`)
         overlap (int): The number of overlapping data points between different chunks when dividing EEG chunks. (default: :obj:`0`)
-        num_channel (int): Number of channels used, of which the first 32 channels are EEG signals. (default: :obj:`32`)
-        num_baseline (int): Number of baseline signal chunks used. (default: :obj:`3`)
-        baseline_chunk_size (int): Number of data points included in each baseline signal chunk. The baseline signal in the DEAP dataset has a total of 384 data points. (default: :obj:`128`)
+        num_channel (int): Number of channels used, of which the first 14 channels are EEG signals. (default: :obj:`14`)
+        num_baseline (int): Number of baseline signal chunks used. (default: :obj:`61`)
+        baseline_chunk_size (int): Number of data points included in each baseline signal chunk. The baseline signal in the DREAMER dataset has a total of 7808 data points. (default: :obj:`128`)
         online_transform (Callable, optional): The transformation of the EEG signals and baseline EEG signals. The input is a :obj:`np.ndarray`, and the ouput is used as the first and second value of each element in the dataset. (default: :obj:`None`)
         offline_transform (Callable, optional): The usage is the same as :obj:`online_transform`, but executed before generating IO intermediate results. (default: :obj:`None`)
         label_transform (Callable, optional): The transformation of the label. The input is an information dictionary, and the ouput is used as the third value of each element in the dataset. (default: :obj:`None`)
         before_trial (Callable, optional): The hook performed on the trial to which the sample belongs. It is performed before the offline transformation and thus typically used to implement context-dependent sample transformations, such as moving averages, etc. The input of this hook function is a 2D EEG signal with shape (number of electrodes, number of data points), whose ideal output shape is also (number of electrodes, number of data points).
         after_trial (Callable, optional): The hook performed on the trial to which the sample belongs. It is performed after the offline transformation and thus typically used to implement context-dependent sample transformations, such as moving averages, etc. The input and output of this hook function should be a sequence of dictionaries representing a sequence of EEG samples. Each dictionary contains two key-value pairs, indexed by :obj:`eeg` (the EEG signal matrix) and :obj:`key` (the index in the database) respectively.
         io_path (str): The path to generated unified data IO, cached as an intermediate result. If set to None, a random path will be generated. (default: :obj:`None`)
         io_size (int): Maximum size database may grow to; used to size the memory mapping. If database grows larger than ``map_size``, an exception will be raised and the user must close and reopen. (default: :obj:`1048576`)
         io_mode (str): Storage mode of EEG signal. When io_mode is set to :obj:`lmdb`, TorchEEG provides an efficient database (LMDB) for storing EEG signals. LMDB may not perform well on limited operating systems, where a file system based EEG signal storage is also provided. When io_mode is set to :obj:`pickle`, pickle-based persistence files are used. When io_mode is set to :obj:`memory`, memory are used. (default: :obj:`lmdb`)
         num_worker (int): Number of subprocesses to use for data loading. 0 means that the data will be loaded in the main process. (default: :obj:`0`)
-        verbose (bool): Whether to display logs during processing, such as progress bars, etc. (default: :obj:`True`)
+        verbose (bool): Whether to display logs during processing, such as progress bars, etc. (default: :obj:`True`)       
     '''
 
     def __init__(self,
-                 root_path: str = './data_preprocessed_python',
+                 mat_path: str = './DREAMER.mat',
                  chunk_size: int = 128,
                  overlap: int = 0,
-                 num_channel: int = 32,
-                 num_baseline: int = 3,
+                 num_channel: int = 14,
+                 num_baseline: int = 61,
                  baseline_chunk_size: int = 128,
                  online_transform: Union[None, Callable] = None,
                  offline_transform: Union[None, Callable] = None,
                  label_transform: Union[None, Callable] = None,
                  before_trial: Union[None, Callable] = None,
                  after_trial: Union[Callable, None] = None,
                  after_session: Union[Callable, None] = None,
@@ -123,15 +126,15 @@
                  num_worker: int = 0,
                  verbose: bool = True):
         if io_path is None:
             io_path = get_random_dir_path(dir_prefix='datasets')
 
         # pass all arguments to super class
         params = {
-            'root_path': root_path,
+            'mat_path': mat_path,
             'chunk_size': chunk_size,
             'overlap': overlap,
             'num_channel': num_channel,
             'num_baseline': num_baseline,
             'baseline_chunk_size': baseline_chunk_size,
             'online_transform': online_transform,
             'offline_transform': offline_transform,
@@ -148,65 +151,77 @@
         }
         super().__init__(**params)
         # save all arguments to __dict__
         self.__dict__.update(params)
 
     @staticmethod
     def process_record(file: Any = None,
-                       root_path: str = './data_preprocessed_python',
+                       mat_path: str = './DREAMER.mat',
                        chunk_size: int = 128,
                        overlap: int = 0,
-                       num_channel: int = 32,
-                       num_baseline: int = 3,
+                       num_channel: int = 14,
+                       num_baseline: int = 61,
                        baseline_chunk_size: int = 128,
                        before_trial: Union[None, Callable] = None,
                        offline_transform: Union[None, Callable] = None,
                        **kwargs):
-        file_name = file  # an element from file name list
-
-        # derive the given arguments (kwargs)
-        with open(os.path.join(root_path, file_name), 'rb') as f:
-            pkl_data = pkl.load(f, encoding='iso-8859-1')
-
-        samples = pkl_data['data']  # trial(40), channel(32), timestep(63*128)
-        labels = pkl_data['labels']
-        subject_id = file_name
+        subject = file
+        mat_data = scio.loadmat(mat_path,
+                                verify_compressed_data_integrity=False)
+
+        trial_len = len(
+            mat_data['DREAMER'][0, 0]['Data'][0,
+                                              0]['EEG'][0,
+                                                        0]['stimuli'][0,
+                                                                      0])  # 18
 
         write_pointer = 0
 
-        for trial_id in range(len(samples)):
-
+        # loop for each trial
+        for trial_id in range(trial_len):
             # extract baseline signals
-            trial_samples = samples[
-                trial_id, :num_channel]  # channel(32), timestep(63*128)
-            if before_trial:
-                trial_samples = before_trial(trial_samples)
-
-            trial_baseline_sample = trial_samples[:, :baseline_chunk_size *
-                                                  num_baseline]  # channel(32), timestep(3*128)
-            trial_baseline_sample = trial_baseline_sample.reshape(
-                num_channel, num_baseline,
-                baseline_chunk_size).mean(axis=1)  # channel(32), timestep(128)
+            trial_baseline_sample = mat_data['DREAMER'][0, 0]['Data'][
+                0, subject]['EEG'][0, 0]['baseline'][0, 0][trial_id, 0]
+            trial_baseline_sample = trial_baseline_sample[:, :num_channel].swapaxes(
+                1, 0)  # channel(14), timestep(61*128)
+            trial_baseline_sample = trial_baseline_sample[:, :num_baseline *
+                                                          baseline_chunk_size].reshape(
+                                                              num_channel,
+                                                              num_baseline,
+                                                              baseline_chunk_size
+                                                          ).mean(
+                                                              axis=1
+                                                          )  # channel(14), timestep(128)
 
             # record the common meta info
-            trial_meta_info = {'subject_id': subject_id, 'trial_id': trial_id}
-            trial_rating = labels[trial_id]
+            trial_meta_info = {'subject_id': subject, 'trial_id': trial_id}
 
-            for label_index, label_name in enumerate(
-                ['valence', 'arousal', 'dominance', 'liking']):
-                trial_meta_info[label_name] = trial_rating[label_index]
+            trial_meta_info['valence'] = mat_data['DREAMER'][0, 0]['Data'][
+                0, subject]['ScoreValence'][0, 0][trial_id, 0]
+            trial_meta_info['arousal'] = mat_data['DREAMER'][0, 0]['Data'][
+                0, subject]['ScoreArousal'][0, 0][trial_id, 0]
+            trial_meta_info['dominance'] = mat_data['DREAMER'][0, 0]['Data'][
+                0, subject]['ScoreDominance'][0, 0][trial_id, 0]
+
+            trial_samples = mat_data['DREAMER'][0, 0]['Data'][
+                0, subject]['EEG'][0, 0]['stimuli'][0, 0][trial_id, 0]
+            trial_samples = trial_samples[:, :num_channel].swapaxes(
+                1, 0)  # channel(14), timestep(n*128)
 
-            start_at = baseline_chunk_size * num_baseline
+            if before_trial:
+                trial_samples = before_trial(trial_samples)
+
+            start_at = 0
             if chunk_size <= 0:
                 dynamic_chunk_size = trial_samples.shape[1] - start_at
             else:
                 dynamic_chunk_size = chunk_size
 
             # chunk with chunk size
-            end_at = start_at + dynamic_chunk_size
+            end_at = dynamic_chunk_size
             # calculate moving step
             step = dynamic_chunk_size - overlap
 
             while end_at <= trial_samples.shape[1]:
                 clip_sample = trial_samples[:, start_at:end_at]
 
                 t_eeg = clip_sample
@@ -216,44 +231,48 @@
                     t = offline_transform(eeg=clip_sample,
                                           baseline=trial_baseline_sample)
                     t_eeg = t['eeg']
                     t_baseline = t['baseline']
 
                 # put baseline signal into IO
                 if not 'baseline_id' in trial_meta_info:
-                    trial_base_id = f'{file_name}_{write_pointer}'
+                    trial_base_id = f'{subject}_{write_pointer}'
                     yield {'eeg': t_baseline, 'key': trial_base_id}
                     write_pointer += 1
                     trial_meta_info['baseline_id'] = trial_base_id
 
-                clip_id = f'{file_name}_{write_pointer}'
+                clip_id = f'{subject}_{write_pointer}'
                 write_pointer += 1
 
                 # record meta info for each signal
                 record_info = {
                     'start_at': start_at,
                     'end_at': end_at,
                     'clip_id': clip_id
                 }
                 record_info.update(trial_meta_info)
                 yield {'eeg': t_eeg, 'key': clip_id, 'info': record_info}
 
                 start_at = start_at + step
                 end_at = start_at + dynamic_chunk_size
 
-    def set_records(self,
-                    root_path: str = './data_preprocessed_python',
-                    **kwargs):
+    def set_records(self, mat_path: str = './DREAMER.mat', **kwargs):
         assert os.path.exists(
-            root_path
-        ), f'root_path ({root_path}) does not exist. Please download the dataset and set the root_path to the downloaded path.'
-        return os.listdir(root_path)
+            mat_path
+        ), f'mat_path ({mat_path}) does not exist. Please download the dataset and set the mat_path to the downloaded path.'
+
+        mat_data = scio.loadmat(mat_path,
+                                verify_compressed_data_integrity=False)
+
+        subject_len = len(mat_data['DREAMER'][0, 0]['Data'][0])  # 23
+        return list(range(subject_len))
 
     def __getitem__(self, index: int) -> Tuple:
         info = self.read_info(index)
+
         eeg_index = str(info['clip_id'])
         eeg_record = str(info['_record_id'])
         eeg = self.read_eeg(eeg_record, eeg_index)
 
         baseline_index = str(info['baseline_id'])
         baseline = self.read_eeg(eeg_record, baseline_index)
 
@@ -268,15 +287,15 @@
 
         return signal, label
 
     @property
     def repr_body(self) -> Dict:
         return dict(
             super().repr_body, **{
-                'root_path': self.root_path,
+                'mat_path': self.mat_path,
                 'chunk_size': self.chunk_size,
                 'overlap': self.overlap,
                 'num_channel': self.num_channel,
                 'num_baseline': self.num_baseline,
                 'baseline_chunk_size': self.baseline_chunk_size,
                 'online_transform': self.online_transform,
                 'offline_transform': self.offline_transform,
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/dreamer.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_v.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,120 @@
 import os
-from typing import Callable, Dict, Tuple, Union, Any
+from typing import Any, Callable, Dict, Tuple, Union
+
+import mne
 
-import scipy.io as scio
-from ..base_dataset import BaseDataset
 from ....utils import get_random_dir_path
+from ..base_dataset import BaseDataset
+
+mne.set_log_level('CRITICAL')
 
 
-class DREAMERDataset(BaseDataset):
+class SEEDVDataset(BaseDataset):
     r'''
-    A multi-modal database consisting of electroencephalogram and electrocardiogram signals recorded during affect elicitation by means of audio-visual stimuli. This class generates training samples and test samples according to the given parameters, and caches the generated results in a unified input and output format (IO). The relevant information of the dataset is as follows:
+    The SEED-V dataset provided by the BCMI laboratory, which is led by Prof. Bao-Liang Lu. This class generates training samples and test samples according to the given parameters, and caches the generated results in a unified input and output format (IO). The relevant information of the dataset is as follows:
 
-    - Author: Katsigiannis et al.
-    - Year: 2017
-    - Download URL: https://zenodo.org/record/546113
-    - Reference: Katsigiannis S, Ramzan N. DREAMER: A database for emotion recognition through EEG and ECG signals from wireless low-cost off-the-shelf devices[J]. IEEE journal of biomedical and health informatics, 2017, 22(1): 98-107.
-    - Stimulus: 18 movie clips. 
-    - Signals: Electroencephalogram (14 channels at 128Hz), and electrocardiogram (2 channels at 256Hz) of 23 subjects.
-    - Rating: Arousal, valence, like/dislike, dominance, familiarity (all ona scale from 1 to 5).
+    - Author: Liu et al.
+    - Year: 2021
+    - Download URL: https://bcmi.sjtu.edu.cn/home/seed/seed-v.html
+    - Reference: Liu W, Qiu J L, Zheng W L, et al. Comparing recognition performance and robustness of multimodal deep learning models for multimodal emotion recognition[J]. IEEE Transactions on Cognitive and Developmental Systems, 2021, 14(2): 715-729.
+    - Stimulus: 15 pieces of stimulating material.
+    - Signals: Electroencephalogram (62 channels at 200Hz) and eye movement data of 20 subjects (20 females). Each subject conducts the experiments in three sessions, and each session contains 15 trials (3 per emotional category) totally 20 people x 3 sessions x 15 trials.
+    - Rating: disgust (0), fear (1), sad (2), neutral (3), happy (4).
 
-    In order to use this dataset, the download file :obj:`DREAMER.mat` is required.
+    In order to use this dataset, the download folder :obj:`EEG_raw` is required, containing the following files:
+    
+    - 10_1_20180507.cnt
+    - 10_2_20180524.cnt
+    - 10_3_20180626.cnt
+    - ...
+    - 9_3_20180728.cnt
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
-        dataset = DREAMERDataset(mat_path='./DREAMER.mat',
-                                 offline_transform=transforms.Compose([
-                                     transforms.BandDifferentialEntropy(),
-                                     transforms.ToGrid(DREAMER_CHANNEL_LOCATION_DICT)
-                                 ]),
-                                 online_transform=transforms.ToTensor(),
-                                 label_transform=transforms.Compose([
-                                     transforms.Select('valence'),
-                                     transforms.Binary(3.0),
-                                 ]))
+        from torcheeg.datasets import SEEDVDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_V_CHANNEL_LOCATION_DICT
+        
+        dataset = SEEDVDataset(root_path='./EEG_raw',
+                                offline_transform=transforms.Compose([
+                                    transforms.BandDifferentialEntropy(),
+                                    transforms.ToGrid(SEED_V_CHANNEL_LOCATION_DICT)
+                                ]),
+                                online_transform=transforms.ToTensor(),
+                                label_transform=transforms.Compose([
+                                    transforms.Select('emotion'),
+                                    transforms.Lambda(lambda x: x + 1)
+                                ]))
         print(dataset[0])
         # EEG signal (torch.Tensor[4, 9, 9]),
         # coresponding baseline signal (torch.Tensor[4, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
-        dataset = DREAMERDataset(mat_path='./DREAMER.mat',
-                                 online_transform=transforms.Compose([
-                                     transforms.To2d(),
-                                     transforms.ToTensor()
-                                 ]),
-                                 label_transform=transforms.Compose([
-                                     transforms.Select(['valence', 'arousal']),
-                                     transforms.Binary(3.0),
-                                     transforms.BinariesToCategory()
-                                 ]))
+        from torcheeg.datasets import SEEDVDataset
+        from torcheeg import transforms
+
+        dataset = SEEDVDataset(root_path='./EEG_raw',
+                                online_transform=transforms.Compose([
+                                    transforms.ToTensor(),
+                                    transforms.To2d()
+                                ]),
+                                label_transform=transforms.Select('emotion'))
         print(dataset[0])
-        # EEG signal (torch.Tensor[1, 14, 128]),
-        # coresponding baseline signal (torch.Tensor[1, 14, 128]),
+        # EEG signal (torch.Tensor[62, 200]),
+        # coresponding baseline signal (torch.Tensor[62, 200]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
-        dataset = DREAMERDataset(mat_path='./DREAMER.mat',
-                                 online_transform=transforms.Compose([
-                                     ToG(DREAMER_ADJACENCY_MATRIX)
-                                 ]),
-                                 label_transform=transforms.Compose([
-                                     transforms.Select('arousal'),
-                                     transforms.Binary(3.0)
-                                 ]))
+
+        from torcheeg.datasets import SEEDVDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_V_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
+        dataset = SEEDVDataset(root_path='./EEG_raw',
+                                online_transform=transforms.Compose([
+                                    ToG(SEED_V_ADJACENCY_MATRIX)
+                                ]),
+                                label_transform=transforms.Select('emotion'))
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
         # coresponding baseline signal (torch_geometric.data.Data),
         # label (int)
-
-    In particular, TorchEEG utilizes the producer-consumer model to allow multi-process data preprocessing. If your data preprocessing is time consuming, consider increasing :obj:`num_worker` for higher speedup. If running under Windows, please use the proper idiom in the main module:
-    
+        
     Args:
-        mat_path (str): Downloaded data files in pickled matlab formats (default: :obj:`'./DREAMER.mat'`)
-        chunk_size (int): Number of data points included in each EEG chunk as training or test samples. If set to -1, the EEG signal of a trial is used as a sample of a chunk. (default: :obj:`128`)
+        root_path (str): Downloaded data files in matlab (unzipped EEG_raw.zip) formats (default: :obj:`'./EEG_raw'`)
+        chunk_size (int): Number of data points included in each EEG chunk as training or test samples. If set to -1, the EEG signal of a trial is used as a sample of a chunk. (default: :obj:`800`)
         overlap (int): The number of overlapping data points between different chunks when dividing EEG chunks. (default: :obj:`0`)
-        num_channel (int): Number of channels used, of which the first 14 channels are EEG signals. (default: :obj:`14`)
-        num_baseline (int): Number of baseline signal chunks used. (default: :obj:`61`)
-        baseline_chunk_size (int): Number of data points included in each baseline signal chunk. The baseline signal in the DREAMER dataset has a total of 7808 data points. (default: :obj:`128`)
+        num_channel (int): Number of channels used, of which the first 62 channels are EEG signals. (default: :obj:`62`)
         online_transform (Callable, optional): The transformation of the EEG signals and baseline EEG signals. The input is a :obj:`np.ndarray`, and the ouput is used as the first and second value of each element in the dataset. (default: :obj:`None`)
         offline_transform (Callable, optional): The usage is the same as :obj:`online_transform`, but executed before generating IO intermediate results. (default: :obj:`None`)
         label_transform (Callable, optional): The transformation of the label. The input is an information dictionary, and the ouput is used as the third value of each element in the dataset. (default: :obj:`None`)
         before_trial (Callable, optional): The hook performed on the trial to which the sample belongs. It is performed before the offline transformation and thus typically used to implement context-dependent sample transformations, such as moving averages, etc. The input of this hook function is a 2D EEG signal with shape (number of electrodes, number of data points), whose ideal output shape is also (number of electrodes, number of data points).
         after_trial (Callable, optional): The hook performed on the trial to which the sample belongs. It is performed after the offline transformation and thus typically used to implement context-dependent sample transformations, such as moving averages, etc. The input and output of this hook function should be a sequence of dictionaries representing a sequence of EEG samples. Each dictionary contains two key-value pairs, indexed by :obj:`eeg` (the EEG signal matrix) and :obj:`key` (the index in the database) respectively.
         io_path (str): The path to generated unified data IO, cached as an intermediate result. If set to None, a random path will be generated. (default: :obj:`None`)
         io_size (int): Maximum size database may grow to; used to size the memory mapping. If database grows larger than ``map_size``, an exception will be raised and the user must close and reopen. (default: :obj:`1048576`)
         io_mode (str): Storage mode of EEG signal. When io_mode is set to :obj:`lmdb`, TorchEEG provides an efficient database (LMDB) for storing EEG signals. LMDB may not perform well on limited operating systems, where a file system based EEG signal storage is also provided. When io_mode is set to :obj:`pickle`, pickle-based persistence files are used. When io_mode is set to :obj:`memory`, memory are used. (default: :obj:`lmdb`)
         num_worker (int): Number of subprocesses to use for data loading. 0 means that the data will be loaded in the main process. (default: :obj:`0`)
-        verbose (bool): Whether to display logs during processing, such as progress bars, etc. (default: :obj:`True`)       
+        verbose (bool): Whether to display logs during processing, such as progress bars, etc. (default: :obj:`True`)    
     '''
 
     def __init__(self,
-                 mat_path: str = './DREAMER.mat',
-                 chunk_size: int = 128,
+                 root_path: str = './EEG_raw',
+                 chunk_size: int = 800,
                  overlap: int = 0,
-                 num_channel: int = 14,
-                 num_baseline: int = 61,
-                 baseline_chunk_size: int = 128,
+                 num_channel: int = 62,
                  online_transform: Union[None, Callable] = None,
                  offline_transform: Union[None, Callable] = None,
                  label_transform: Union[None, Callable] = None,
                  before_trial: Union[None, Callable] = None,
                  after_trial: Union[Callable, None] = None,
                  after_session: Union[Callable, None] = None,
                  after_subject: Union[Callable, None] = None,
@@ -116,20 +124,18 @@
                  num_worker: int = 0,
                  verbose: bool = True):
         if io_path is None:
             io_path = get_random_dir_path(dir_prefix='datasets')
 
         # pass all arguments to super class
         params = {
-            'mat_path': mat_path,
+            'root_path': root_path,
             'chunk_size': chunk_size,
             'overlap': overlap,
             'num_channel': num_channel,
-            'num_baseline': num_baseline,
-            'baseline_chunk_size': baseline_chunk_size,
             'online_transform': online_transform,
             'offline_transform': offline_transform,
             'label_transform': label_transform,
             'before_trial': before_trial,
             'after_trial': after_trial,
             'after_session': after_session,
             'after_subject': after_subject,
@@ -141,156 +147,173 @@
         }
         super().__init__(**params)
         # save all arguments to __dict__
         self.__dict__.update(params)
 
     @staticmethod
     def process_record(file: Any = None,
-                       mat_path: str = './DREAMER.mat',
-                       chunk_size: int = 128,
+                       chunk_size: int = 800,
                        overlap: int = 0,
-                       num_channel: int = 14,
-                       num_baseline: int = 61,
-                       baseline_chunk_size: int = 128,
+                       num_channel: int = 62,
                        before_trial: Union[None, Callable] = None,
                        offline_transform: Union[None, Callable] = None,
                        **kwargs):
-        subject = file
-        mat_data = scio.loadmat(mat_path,
-                                verify_compressed_data_integrity=False)
-
-        trial_len = len(
-            mat_data['DREAMER'][0, 0]['Data'][0,
-                                              0]['EEG'][0,
-                                                        0]['stimuli'][0,
-                                                                      0])  # 18
+        file_name = os.path.basename(file)
+        # split with _, the first part is the subject_id, the second part is the session_id, the third part is the date
+        subject_id, session_id, date = file_name.split('_')[:3]
+
+        labels = [[4, 1, 3, 2, 0, 4, 1, 3, 2, 0, 4, 1, 3, 2, 0],
+                  [2, 1, 3, 0, 4, 4, 0, 3, 2, 1, 3, 4, 1, 2, 0],
+                  [2, 1, 3, 0, 4, 4, 0, 3, 2, 1, 3, 4, 1, 2, 0]]
+
+        trial_labels = labels[int(session_id) - 1]
+
+        eeg_raw = mne.io.read_raw_cnt(file)
+
+        useless_ch = ['M1', 'M2', 'VEO', 'HEO']
+        eeg_raw.drop_channels(useless_ch)
+
+        data_matrix = eeg_raw.get_data()
+
+        start_end_list = [
+            {
+                'start_seconds': [
+                    30, 132, 287, 555, 773, 982, 1271, 1628, 1730, 2025, 2227,
+                    2435, 2667, 2932, 3204
+                ],
+                'end_seconds': [
+                    102, 228, 524, 742, 920, 1240, 1568, 1697, 1994, 2166, 2401,
+                    2607, 2901, 3172, 3359
+                ]
+            },
+            {
+                'start_seconds': [
+                    30, 299, 548, 646, 836, 1000, 1091, 1392, 1657, 1809, 1966,
+                    2186, 2333, 2490, 2741
+                ],
+                'end_seconds': [
+                    267, 488, 614, 773, 967, 1059, 1331, 1622, 1777, 1908, 2153,
+                    2302, 2428, 2709, 2817
+                ]
+            },
+            {
+                'start_seconds': [
+                    30, 353, 478, 674, 825, 908, 1200, 1346, 1451, 1711, 2055,
+                    2307, 2457, 2726, 2888
+                ],
+                'end_seconds': [
+                    321, 418, 643, 764, 877, 1147, 1284, 1418, 1679, 1996, 2275,
+                    2425, 2664, 2857, 3066
+                ]
+            },
+        ]
+        start_seconds = start_end_list[int(session_id) - 1]['start_seconds']
+        end_seconds = start_end_list[int(session_id) - 1]['end_seconds']
 
         write_pointer = 0
 
-        # loop for each trial
-        for trial_id in range(trial_len):
-            # extract baseline signals
-            trial_baseline_sample = mat_data['DREAMER'][0, 0]['Data'][
-                0, subject]['EEG'][0, 0]['baseline'][0, 0][trial_id, 0]
-            trial_baseline_sample = trial_baseline_sample[:, :num_channel].swapaxes(
-                1, 0)  # channel(14), timestep(61*128)
-            trial_baseline_sample = trial_baseline_sample[:, :num_baseline *
-                                                          baseline_chunk_size].reshape(
-                                                              num_channel,
-                                                              num_baseline,
-                                                              baseline_chunk_size
-                                                          ).mean(
-                                                              axis=1
-                                                          )  # channel(14), timestep(128)
-
-            # record the common meta info
-            trial_meta_info = {'subject_id': subject, 'trial_id': trial_id}
-
-            trial_meta_info['valence'] = mat_data['DREAMER'][0, 0]['Data'][
-                0, subject]['ScoreValence'][0, 0][trial_id, 0]
-            trial_meta_info['arousal'] = mat_data['DREAMER'][0, 0]['Data'][
-                0, subject]['ScoreArousal'][0, 0][trial_id, 0]
-            trial_meta_info['dominance'] = mat_data['DREAMER'][0, 0]['Data'][
-                0, subject]['ScoreDominance'][0, 0][trial_id, 0]
-
-            trial_samples = mat_data['DREAMER'][0, 0]['Data'][
-                0, subject]['EEG'][0, 0]['stimuli'][0, 0][trial_id, 0]
-            trial_samples = trial_samples[:, :num_channel].swapaxes(
-                1, 0)  # channel(14), timestep(n*128)
+        for trial_id, (start_second,
+                       end_second) in enumerate(zip(start_seconds,
+                                                    end_seconds)):
+
+            trial_meta_info = {
+                'subject_id': subject_id,
+                'session_id': session_id,
+                'date': date,
+                'trial_id': trial_id,
+                'emotion': trial_labels[trial_id]
+            }
+
+            trial_samples = data_matrix[:,
+                                        start_second * 1000:end_second * 1000]
+
+            # downsample to 200Hz
+            trial_samples = trial_samples[:, ::5]
+
+            #  EEG data are then processed with a bandpass filter between 1 Hz and 75 Hz.
+            trial_samples = mne.filter.filter_data(trial_samples,
+                                                   sfreq=200,
+                                                   l_freq=1,
+                                                   h_freq=75)
 
-            if before_trial:
+            if not before_trial is None:
                 trial_samples = before_trial(trial_samples)
 
+            # extract experimental signals
             start_at = 0
             if chunk_size <= 0:
                 dynamic_chunk_size = trial_samples.shape[1] - start_at
             else:
                 dynamic_chunk_size = chunk_size
 
             # chunk with chunk size
             end_at = dynamic_chunk_size
             # calculate moving step
             step = dynamic_chunk_size - overlap
 
             while end_at <= trial_samples.shape[1]:
-                clip_sample = trial_samples[:, start_at:end_at]
+                clip_sample = trial_samples[:num_channel, start_at:end_at]
 
                 t_eeg = clip_sample
-                t_baseline = trial_baseline_sample
-
                 if not offline_transform is None:
-                    t = offline_transform(eeg=clip_sample,
-                                          baseline=trial_baseline_sample)
-                    t_eeg = t['eeg']
-                    t_baseline = t['baseline']
-
-                # put baseline signal into IO
-                if not 'baseline_id' in trial_meta_info:
-                    trial_base_id = f'{subject}_{write_pointer}'
-                    yield {'eeg': t_baseline, 'key': trial_base_id}
-                    write_pointer += 1
-                    trial_meta_info['baseline_id'] = trial_base_id
+                    t_eeg = offline_transform(eeg=clip_sample)['eeg']
 
-                clip_id = f'{subject}_{write_pointer}'
+                clip_id = f'{file_name}_{write_pointer}'
                 write_pointer += 1
 
-                # record meta info for each signal
                 record_info = {
+                    'clip_id': clip_id,
                     'start_at': start_at,
-                    'end_at': end_at,
-                    'clip_id': clip_id
+                    'end_at': end_at
                 }
                 record_info.update(trial_meta_info)
+
                 yield {'eeg': t_eeg, 'key': clip_id, 'info': record_info}
 
                 start_at = start_at + step
                 end_at = start_at + dynamic_chunk_size
 
-    def set_records(self, mat_path: str = './DREAMER.mat', **kwargs):
+    def set_records(self, root_path: str = './EEG_raw', **kwargs):
         assert os.path.exists(
-            mat_path
-        ), f'mat_path ({mat_path}) does not exist. Please download the dataset and set the mat_path to the downloaded path.'
-
-        mat_data = scio.loadmat(mat_path,
-                                verify_compressed_data_integrity=False)
+            root_path
+        ), f'root_path ({root_path}) does not exist. Please download the dataset and set the root_path to the downloaded path.'
 
-        subject_len = len(mat_data['DREAMER'][0, 0]['Data'][0])  # 23
-        return list(range(subject_len))
+        file_list = os.listdir(root_path)
+        file_list = [
+            os.path.join(root_path, file) for file in file_list
+            if file.endswith('.cnt')
+        ]
+        return file_list
 
-    def __getitem__(self, index: int) -> Tuple:
+    def __getitem__(self, index: int) -> Tuple[any, any, int, int, int]:
         info = self.read_info(index)
 
         eeg_index = str(info['clip_id'])
         eeg_record = str(info['_record_id'])
         eeg = self.read_eeg(eeg_record, eeg_index)
 
-        baseline_index = str(info['baseline_id'])
-        baseline = self.read_eeg(eeg_record, baseline_index)
-
         signal = eeg
         label = info
 
         if self.online_transform:
-            signal = self.online_transform(eeg=eeg, baseline=baseline)['eeg']
+            signal = self.online_transform(eeg=eeg)['eeg']
 
         if self.label_transform:
             label = self.label_transform(y=info)['y']
 
         return signal, label
 
     @property
     def repr_body(self) -> Dict:
         return dict(
             super().repr_body, **{
-                'mat_path': self.mat_path,
+                'root_path': self.root_path,
                 'chunk_size': self.chunk_size,
                 'overlap': self.overlap,
                 'num_channel': self.num_channel,
-                'num_baseline': self.num_baseline,
-                'baseline_chunk_size': self.baseline_chunk_size,
                 'online_transform': self.online_transform,
                 'offline_transform': self.offline_transform,
                 'label_transform': self.label_transform,
                 'before_trial': self.before_trial,
                 'after_trial': self.after_trial,
                 'num_worker': self.num_worker,
                 'verbose': self.verbose,
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/mahnob.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/mahnob.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,18 @@
       + Part_30_S_Trial20_emotion.bdf
       + session.xml
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
     
+        from torcheeg.datasets import MAHNOBDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import MAHNOB_CHANNEL_LOCATION_DICT
+
         dataset = MAHNOBDataset(root_path='./Sessions',
                                 offline_transform=transforms.Compose([
                                     transforms.BandDifferentialEntropy(),
                                     transforms.ToGrid(MAHNOB_CHANNEL_LOCATION_DICT)
                                 ]),
                                 online_transform=transforms.ToTensor(),
                                 label_transform=transforms.Compose([
@@ -52,14 +56,17 @@
         # EEG signal (torch.Tensor[4, 9, 9]),
         # coresponding baseline signal (torch.Tensor[4, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
+    
+        from torcheeg.datasets import MAHNOBDataset
+        from torcheeg import transforms
 
         dataset = MAHNOBDataset(root_path='./Sessions',
                                 online_transform=transforms.Compose([
                                     transforms.To2d(),
                                     transforms.ToTensor()
                                 ]),
                                 label_transform=transforms.Compose([
@@ -71,15 +78,20 @@
         # EEG signal (torch.Tensor[1, 32, 128]),
         # coresponding baseline signal (torch.Tensor[1, 32, 128]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import MAHNOBDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import MAHNOB_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+
         dataset = MAHNOBDataset(root_path='./Sessions',
                                 online_transform=transforms.Compose([
                                     ToG(MAHNOB_ADJACENCY_MATRIX)
                                 ]),
                                 label_transform=transforms.Compose([
                                     transforms.Select('feltArsl'),
                                     transforms.Binary(5.0)
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/mped_feature.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/mped_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     - ...
     - STFT
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import MPEDFeatureDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import MPED_CHANNEL_LOCATION_DICT
+
         dataset = MPEDFeatureDataset(root_path='./EEG_feature',
                                      features=['PSD'],
                                      offline_transform=transforms.ToGrid       (MPED_CHANNEL_LOCATION_DICT),
                                      online_transform=transforms.ToTensor(),
                                      label_transform=transforms.Compose([
                                          transforms.Select('emotion')
                                      ]))
@@ -43,15 +47,20 @@
         # EEG signal (torch.Tensor[5, 9, 9]),
         # coresponding baseline signal (torch.Tensor[5, 9, 9]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import MPEDFeatureDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import MPED_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+
         dataset = MPEDFeatureDataset(root_path='./Preprocessed_EEG',
                                      features=['PSD'],
                                      online_transform=ToG(MPED_ADJACENCY_MATRIX),
                                      label_transform=transforms.Compose([
                                          transforms.Select('emotion')
                                      ]))
         print(dataset[0])
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     - ...
     - 9_20140704.mat
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_CHANNEL_LOCATION_DICT
+
         dataset = SEEDDataset(root_path='./Preprocessed_EEG',
                               offline_transform=transforms.Compose([
                                   transforms.BandDifferentialEntropy(),
                                   transforms.ToGrid(SEED_CHANNEL_LOCATION_DICT)
                               ]),
                               online_transform=transforms.ToTensor(),
                               label_transform=transforms.Compose([
@@ -45,39 +49,47 @@
         # coresponding baseline signal (torch.Tensor[4, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg import transforms
+
         dataset = SEEDDataset(root_path='./Preprocessed_EEG',
                               online_transform=transforms.Compose([
                                   transforms.ToTensor(),
                                   transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select('emotion'),
-                                  transforms.Lambda(x: x + 1)
+                                  transforms.Lambda(lambda x: x + 1)
                               ]))
         print(dataset[0])
         # EEG signal (torch.Tensor[62, 200]),
         # coresponding baseline signal (torch.Tensor[62, 200]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
         dataset = SEEDDataset(root_path='./Preprocessed_EEG',
                               online_transform=transforms.Compose([
                                   ToG(SEED_ADJACENCY_MATRIX)
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select('emotion'),
-                                  transforms.Lambda(x: x + 1)
+                                  transforms.Lambda(lambda x: x + 1)
                               ]))
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
         # coresponding baseline signal (torch_geometric.data.Data),
         # label (int)
 
     Args:
@@ -166,15 +178,14 @@
 
         trial_ids = [key for key in samples.keys() if 'eeg' in key]
 
         write_pointer = 0
         # loop for each trial
         for trial_id in trial_ids:
 
-            # extract baseline signals
             trial_samples = samples[trial_id]  # channel(62), timestep(n*200)
             if before_trial:
                 trial_samples = before_trial(trial_samples)
 
             # record the common meta info
             trial_meta_info = {
                 'subject_id': subject,
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed_feature.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     - ...
     - 9_20140704.mat
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import SEEDFeatureDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_CHANNEL_LOCATION_DICT
+
         dataset = SEEDFeatureDataset(root_path='./ExtractedFeatures',
                                      feature=['de_movingAve'],
                                      offline_transform=transforms.ToGrid       (SEED_CHANNEL_LOCATION_DICT),
                                      online_transform=transforms.ToTensor(),
                                      label_transform=transforms.Compose([
                                          transforms.Select('emotion'),
                                          transforms.Lambda(lambda x: x + 1)
@@ -45,15 +49,20 @@
         # EEG signal (torch.Tensor[5, 9, 9]),
         # coresponding baseline signal (torch.Tensor[5, 9, 9]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import SEEDFeatureDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
         dataset = SEEDFeatureDataset(root_path='./Preprocessed_EEG',
                                      features=['de_movingAve'],
                                      online_transform=ToG(SEED_ADJACENCY_MATRIX),
                                      label_transform=transforms.Compose([
                                          transforms.Select('emotion'),
                                          transforms.Lambda(x: x + 1)
                                      ]))
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed_iv.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_iv.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class SEEDIVDataset(BaseDataset):
     r'''
     The SEED-IV dataset provided by the BCMI laboratory, which is led by Prof. Bao-Liang Lu. This class generates training samples and test samples according to the given parameters, and caches the generated results in a unified input and output format (IO). The relevant information of the dataset is as follows:
 
     - Author: Zheng et al.
     - Year: 2018
-    - Download URL: https://ieeexplore.ieee.org/abstract/document/8283814
+    - Download URL: https://bcmi.sjtu.edu.cn/home/seed/seed-iv.html
     - Reference: Zheng W L, Liu W, Lu Y, et al. Emotionmeter: A multimodal framework for recognizing human emotions[J]. IEEE transactions on cybernetics, 2018, 49(3): 1110-1122.
     - Stimulus: 168 film clips.
     - Signals: Electroencephalogram (62 channels at 200Hz) and eye movement data of 15 subjects (8 females). Each subject conducts the experiments in three sessions, and each session contains 24 trials (6 per emotional category) totally 15 people x 3 sessions x 24 trials.
     - Rating: neutral (0), sad (1), fear (2), and happy (3).
 
     In order to use this dataset, the download folder :obj:`eeg_raw_data` is required, containing the following files:
     
@@ -27,18 +27,22 @@
     - ...
     - 9_20140704.mat
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import SEEDIVDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_IV_CHANNEL_LOCATION_DICT
+        
         dataset = SEEDIVDataset(root_path='./eeg_raw_data',
                                 offline_transform=transforms.Compose([
                                     transforms.BandDifferentialEntropy(),
-                                    transforms.ToGrid(SEEDIV_CHANNEL_LOCATION_DICT)
+                                    transforms.ToGrid(SEED_IV_CHANNEL_LOCATION_DICT)
                                 ]),
                                 online_transform=transforms.ToTensor(),
                                 label_transform=transforms.Compose([
                                     transforms.Select('emotion'),
                                     transforms.Lambda(lambda x: x + 1)
                                 ]))
         print(dataset[0])
@@ -46,29 +50,37 @@
         # coresponding baseline signal (torch.Tensor[4, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import SEEDIVDataset
+        from torcheeg import transforms
+
         dataset = SEEDIVDataset(root_path='./eeg_raw_data',
                                 online_transform=transforms.Compose([
                                     transforms.ToTensor(),
                                     transforms.To2d()
                                 ]),
                                 label_transform=transforms.Select('emotion'))
         print(dataset[0])
         # EEG signal (torch.Tensor[62, 200]),
         # coresponding baseline signal (torch.Tensor[62, 200]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import SEEDIVDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEEDIV_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
         dataset = SEEDIVDataset(root_path='./eeg_raw_data',
                                 online_transform=transforms.Compose([
                                     ToG(SEED_IV_ADJACENCY_MATRIX)
                                 ]),
                                 label_transform=transforms.Select('emotion'))
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/emotion_recognition/seed_iv_feature.py` & `torcheeg-1.1.2/torcheeg/datasets/module/emotion_recognition/seed_iv_feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class SEEDIVFeatureDataset(BaseDataset):
     r'''
     The SEED-IV dataset provided by the BCMI laboratory, which is led by Prof. Bao-Liang Lu. Since the SEED dataset provides features based on matlab, this class implements the processing of these feature files to initialize the dataset. The relevant information of the dataset is as follows:
 
     - Author: Zheng et al.
     - Year: 2018
-    - Download URL: https://ieeexplore.ieee.org/abstract/document/8283814
+    - Download URL: https://bcmi.sjtu.edu.cn/home/seed/seed-iv.html
     - Reference: Zheng W L, Liu W, Lu Y, et al. Emotionmeter: A multimodal framework for recognizing human emotions[J]. IEEE transactions on cybernetics, 2018, 49(3): 1110-1122.
     - Stimulus: 168 film clips.
     - Signals: Electroencephalogram (62 channels at 200Hz) and eye movement data of 15 subjects (8 females). Each subject conducts the experiments in three sessions, and each session contains 24 trials (6 per emotional category) totally 15 people x 3 sessions x 24 trials.
     - Rating: neutral (0), sad (1), fear (2), and happy (3).
     - Features: de_movingAve, de_LDS, psd_movingAve, psd_LDS, dasm_movingAve, dasm_LDS, rasm_movingAve, rasm_LDS, asm_movingAve, asm_LDS, dcau_movingAve, dcau_LDS of 4-second long windows
 
     In order to use this dataset, the download folder :obj:`eeg_feature_smooth` is required, containing the following folder:
@@ -27,28 +27,37 @@
     - 2
     - 3
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import SEEDIVFeatureDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_IV_CHANNEL_LOCATION_DICT
+        
         dataset = SEEDIVFeatureDataset(root_path='./eeg_feature_smooth',
                                        features=['de_movingAve'],
-                                       offline_transform=transforms.ToGrid         (SEED_CHANNEL_LOCATION_DICT),
+                                       offline_transform=transforms.ToGrid         (SEED_IV_CHANNEL_LOCATION_DICT),
                                        online_transform=transforms.ToTensor(),
                                        label_transform=transforms.Select('emotion'))
         print(dataset[0])
         # EEG signal (torch.Tensor[5, 9, 9]),
         # coresponding baseline signal (torch.Tensor[5, 9, 9]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import SEEDIVFeatureDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
         dataset = SEEDIVFeatureDataset(root_path='./eeg_feature_smooth',
                                        features=['de_movingAve'],
                                        online_transform=ToG(SEED_ADJACENCY_MATRIX),
                                        label_transform=transforms.Select('emotion'))
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
         # coresponding baseline signal (torch_geometric.data.Data),
@@ -197,17 +206,17 @@
                     t_eeg = offline_transform(eeg=clip_sample)['eeg']
 
                 clip_id = f'{file_name}_{write_pointer}'
                 write_pointer += 1
 
                 # record meta info for each signal
                 record_info = {
-                    'start_at': i * 400,
+                    'start_at': i * 800,
                     'end_at': (i + 1) *
-                    400,  # The size of the sliding time windows for feature extraction is 4 seconds.
+                    800,  # The size of the sliding time windows for feature extraction is 4 seconds.
                     'clip_id': clip_id
                 }
                 record_info.update(trial_meta_info)
                 yield {'eeg': t_eeg, 'key': clip_id, 'info': record_info}
 
     def set_records(self, root_path: str = './eeg_feature_smooth', **kwargs):
         assert os.path.exists(
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/folder_dataset.py` & `torcheeg-1.1.2/torcheeg/datasets/module/folder_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,18 @@
         sub02
         |- label01.edf
         |- label02.edf
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import FolderDataset
+        from torcheeg import transforms
+
         sfreq = 128  # Sampling rate
         n_channels = 14  # Number of channels
         duration = 5  # Data collected for 5 seconds
         for i in range(num_files):
             n_samples = sfreq * duration
             data = np.random.randn(n_channels, n_samples)
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/motor_imagery/bciciv_2a.py` & `torcheeg-1.1.2/torcheeg/datasets/module/motor_imagery/bciciv_2a.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     - ...
     - http://bnci-horizon-2020.eu/database/data-sets/001-2014/A09E.mat
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import BCICIV2aDataset
+        from torcheeg import transforms
+
         dataset = BCICIV2aDataset(root_path='./BCICIV_2a_mat',
                                   online_transform=transforms.Compose([
                                       transforms.To2d(),
                                       transforms.ToTensor()
                                   ]),
                                   label_transform=transforms.Compose([
                                       transforms.Select('label'),
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/personal_identification/m3cv.py` & `torcheeg-1.1.2/torcheeg/datasets/module/personal_identification/m3cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     - Calibration (unzipped Calibration.zip)
     - Testing (unzipped Testing.zip)
     - Enrollment (unzipped Enrollment.zip)
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import M3CVDataset
+        from torcheeg import transforms
+
         dataset = M3CVDataset(root_path='./aistudio',
                               offline_transform=transforms.Compose([
                                   transforms.BandDifferentialEntropy(),
                                   transforms.ToGrid(M3CV_CHANNEL_LOCATION_DICT)
                               ]),
                               online_transform=transforms.ToTensor(),
                               label_transform=transforms.Compose([
@@ -45,14 +48,17 @@
         # coresponding baseline signal (torch.Tensor[1000, 9, 9]),
         # label (int)
 
     Another example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import M3CVDataset
+        from torcheeg import transforms
+    
         dataset = M3CVDataset(io_path=f'./m3cv',
                               root_path='./aistudio',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
@@ -63,15 +69,20 @@
         # EEG signal (torch.Tensor[1, 65, 1000]),
         # coresponding baseline signal (torch.Tensor[1, 65, 1000]),
         # label (int)
 
     An example dataset for GNN-based methods:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import M3CVDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants.personal_identification.m3cv import M3CV_ADJACENCY_MATRIX
+        from torcheeg.transforms.pyg import ToG
+        
         dataset = M3CVDataset(io_path=f'./m3cv',
                               root_path='./aistudio',
                               online_transform=transforms.Compose([
                                   ToG(M3CV_ADJACENCY_MATRIX)
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select('SubjectID'),
```

### Comparing `torcheeg-1.1.1/torcheeg/datasets/module/sspev/tsu_benchmark.py` & `torcheeg-1.1.2/torcheeg/datasets/module/ssvep/tsu_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     - ...
     - S35.mat
 
     An example dataset for CNN-based methods:
 
     .. code-block:: python
 
+        from torcheeg.datasets import TSUBenckmarkDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants.ssvep.tsubenchmark import TSUBenckmark_CHANNEL_LOCATION_DICT
+
         dataset = TSUBenckmarkDataset(root_path='./TSUBenchmark',
                                       offline_transform=transforms.Compose([
                                           transforms.BandDifferentialEntropy(),
                                           transforms.ToGrid(TSUBenckmark_CHANNEL_LOCATION_DICT)
                                       ]),
                                       online_transform=transforms.ToTensor(),
                                       label_transform=transforms.Select(['trial_id']))
@@ -69,30 +73,14 @@
                                           ToG(TSUBenckmark_ADJACENCY_MATRIX)
                                       ]),
                                       label_transform=transforms.Select(['trial_id']))
         print(dataset[0])
         # EEG signal (torch_geometric.data.Data),
         # coresponding baseline signal (torch_geometric.data.Data),
         # label (int)
-        
-    In particular, TorchEEG utilizes the producer-consumer model to allow multi-process data preprocessing. If your data preprocessing is time consuming, consider increasing :obj:`num_worker` for higher speedup. If running under Windows, please use the proper idiom in the main module:
-
-    .. code-block:: python
-    
-        if __name__ == '__main__':
-            dataset = TSUBenckmarkDataset(root_path='./TSUBenchmark',
-                                          online_transform=transforms.Compose([
-                                              ToG(TSUBenckmark_ADJACENCY_MATRIX)
-                                          ]),
-                                          label_transform=transforms.Select(['freq']),
-                                          num_worker=4)
-            print(dataset[0])
-            # EEG signal (torch_geometric.data.Data),
-            # coresponding baseline signal (torch_geometric.data.Data),
-            # label (int)
 
     Args:
         root_path (str): Downloaded data files in matlab (unzipped TSUBenchmark.zip) formats (default: :obj:`'./TSUBenchmark'`)
         chunk_size (int): Number of data points included in each EEG chunk as training or test samples. (default: :obj:`250`)
         overlap (int): The number of overlapping data points between different chunks when dividing EEG chunks. (default: :obj:`0`)
         num_channel (int): Number of channels used, of which the first 64 channels are EEG signals. (default: :obj:`64`)
         online_transform (Callable, optional): The transformation of the EEG signals and baseline EEG signals. The input is a :obj:`np.ndarray`, and the ouput is used as the first and second value of each element in the dataset. (default: :obj:`None`)
```

### Comparing `torcheeg-1.1.1/torcheeg/io/eeg_signal.py` & `torcheeg-1.1.2/torcheeg/io/eeg_signal.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/io/meta_info.py` & `torcheeg-1.1.2/torcheeg/io/meta_info.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         :alt: The schematic diagram of KFold
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFold
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFold(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold_cross_subject.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold_cross_subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,19 @@
         :alt: The schematic diagram of KFoldCrossSubject
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldCrossSubject
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldCrossSubject(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold_cross_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold_cross_trial.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         :alt: The schematic diagram of KFoldCrossTrial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldCrossTrial
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldCrossTrial(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold_groupby_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold_groupby_trial.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         :alt: The schematic diagram of KFoldGroupbyTrial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldGroupbyTrial
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldGroupbyTrial(n_splits=5, shuffle=False)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold_per_subject.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold_per_subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,19 @@
         :alt: The schematic diagram of KFoldPerSubject
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.model_selection import KFoldPerSubject
+        from torcheeg.utils import DataLoader
+
         cv = KFoldPerSubject(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.ToTensor(),
                                   transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
@@ -43,14 +48,19 @@
             test_loader = DataLoader(test_dataset)
             ...
     
     :obj:`KFoldPerSubject` allows the user to specify the index of the subject of interest, when the user need to report the performance on each subject.
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.model_selection import KFoldPerSubject
+        from torcheeg.utils import DataLoader
+
         cv = KFoldPerSubject(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold_per_subject_cross_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold_per_subject_cross_trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         :alt: The schematic diagram of KFoldPerSubjectCrossTrial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldPerSubjectCrossTrial
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldPerSubjectCrossTrial(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.ToTensor(),
                                   transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
@@ -44,14 +49,19 @@
             test_loader = DataLoader(test_dataset)
             ...
     
     :obj:`KFoldPerSubjectCrossTrial` allows the user to specify the index of the subject of interest, when the user need to report the performance on each subject.
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldPerSubjectCrossTrial
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldPerSubjectCrossTrial(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/k_fold_per_subject_groupby_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/k_fold_per_subject_groupby_trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         :alt: The schematic diagram of KFoldPerSubjectGroupbyTrial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldPerSubjectGroupbyTrial
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldPerSubjectGroupbyTrial(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.ToTensor(),
                                   transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
@@ -44,14 +49,19 @@
             test_loader = DataLoader(test_dataset)
             ...
     
     :obj:`KFoldPerSubjectGroupbyTrial` allows the user to specify the index of the subject of interest, when the user need to report the performance on each subject.
 
     .. code-block:: python
 
+        from torcheeg.model_selection import KFoldPerSubjectGroupbyTrial
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = KFoldPerSubjectGroupbyTrial(n_splits=5, shuffle=True)
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/leave_one_subject_out.py` & `torcheeg-1.1.2/torcheeg/model_selection/leave_one_subject_out.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,19 @@
         :alt: The schematic diagram of LeaveOneSubjectOut
         :align: center
 
     |
     
     .. code-block:: python
 
+        from torcheeg.model_selection import LeaveOneSubjectOut
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         cv = LeaveOneSubjectOut()
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.ToTensor(),
                                   transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/split.py` & `torcheeg-1.1.2/torcheeg/model_selection/split.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,19 @@
         :alt: The schematic diagram of train_test_split
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg.model_selection import train_test_split
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
                                   transforms.To2d(),
                                   transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select(['valence', 'arousal']),
@@ -56,16 +61,17 @@
         random_state (int, optional): When shuffle is :obj:`True`, :obj:`random_state` affects the ordering of the indices, which controls the randomness of each fold. Otherwise, this parameter has no effect. (default: :obj:`None`)
         split_path (str): The path to data partition information. If the path exists, read the existing partition from the path. If the path does not exist, the current division method will be saved for next use. If set to None, a random path will be generated. (default: :obj:`None`)
     '''
     if split_path is None:
         split_path = get_random_dir_path(dir_prefix='model_selection')
 
     if not os.path.exists(split_path):
+        log.info(f'📊 | Create the split of train and test set.')
         log.info(
-            f'📊 | Create the split of train and test set. Please set split_path to {split_path} for the next run, if you want to use the same setting for the experiment.'
+            f'😊 | Please set \033[92msplit_path\033[0m to \033[92m{split_path}\033[0m for the next run, if you want to use the same setting for the experiment.'
         )
         os.makedirs(split_path)
         info = dataset.info
 
         n_samples = len(dataset)
         indices = np.arange(n_samples)
         train_index, test_index = model_selection.train_test_split(
@@ -77,15 +83,18 @@
         test_info = info.iloc[test_index]
 
         train_info.to_csv(os.path.join(split_path, 'train.csv'), index=False)
         test_info.to_csv(os.path.join(split_path, 'test.csv'), index=False)
 
     else:
         log.info(
-            f'Read the split of train and test set from {split_path}. If you want to use the same setting for the experiment, please set split_path to {split_path} for the next run.'
+            f'📊 | Detected existing split of train and test set, use existing split from {split_path}.'
+        )
+        log.info(
+            f'💡 | If the dataset is re-generated, you need to re-generate the split of the dataset instead of using the previous split.'
         )
 
     train_info = pd.read_csv(os.path.join(split_path, 'train.csv'))
     test_info = pd.read_csv(os.path.join(split_path, 'test.csv'))
 
     train_dataset = copy(dataset)
     train_dataset.info = train_info
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/split_cross_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/split_per_subject_cross_trial.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,119 +10,111 @@
 from torcheeg.datasets.module.base_dataset import BaseDataset
 
 from ..utils import get_random_dir_path
 
 log = logging.getLogger('torcheeg')
 
 
-def train_test_split_cross_trial(dataset: BaseDataset,
-                                 test_size: float = 0.2,
-                                 shuffle: bool = False,
-                                 random_state: Union[float, None] = None,
-                                 split_path: Union[None, str] = None):
+def train_test_split_per_subject_cross_trial(dataset: BaseDataset,
+                                             test_size: float = 0.2,
+                                             subject: str = 's01.dat',
+                                             shuffle: bool = False,
+                                             random_state: Union[float,
+                                                                 None] = None,
+                                             split_path: Union[None, str] = None):
     r'''
-    A tool function for cross-validations, to divide the training set and the test set. It is suitable for experiments with large dataset volume and no need to use k-fold cross-validations. Parts of trials are sampled according to a certain proportion as the test dataset, and samples from other trials are used as training samples. In most literatures, 20% of the data are sampled for testing.
+    A tool function for cross-validations, to divide the training set and the test set. It is suitable for subject dependent experiments with large dataset volume and no need to use k-fold cross-validations. For the first step, the EEG signal samples of the specified user are selected. Then, parts of trials are sampled according to a certain proportion as the test dataset, and samples from other trials are used as training samples. In most literatures, 20% of the data are sampled for testing.
 
-    :obj:`train_test_split_cross_trial` devides training set and the test set at the dimension of each trial. For example, when :obj:`test_size=0.2`, the first 80% of samples of each trial are used for training, and the last 20% of samples are used for testing. It is more consistent with real applications and can test the generalization of the model to a certain extent.
-
-    .. image:: _static/train_test_split_cross_trial.png
-        :alt: The schematic diagram of train_test_split_cross_trial
+    .. image:: _static/train_test_split_per_subject_cross_trial.png
+        :alt: The schematic diagram of train_test_split_per_subject_cross_trial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg.model_selection import train_test_split_per_subject_cross_trial
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
-                                  transforms.To2d(),
-                                  transforms.ToTensor()
+                                  transforms.ToTensor(),
+                                  transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select(['valence', 'arousal']),
                                   transforms.Binary(5.0),
                                   transforms.BinariesToCategory()
                               ]))
 
-        train_dataset, test_dataset = train_test_split_cross_trial(dataset=dataset)
+        train_dataset, test_dataset = train_test_split_per_subject_cross_trial(dataset=dataset)
 
         train_loader = DataLoader(train_dataset)
         test_loader = DataLoader(test_dataset)
         ...
 
     Args:
         dataset (BaseDataset): Dataset to be divided.
         test_size (int):  If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the test split. If int, represents the absolute number of test samples. (default: :obj:`0.2`)
+        subject (str): The subject whose EEG samples will be used for training and test. (default: :obj:`s01.dat`)
         shuffle (bool): Whether to shuffle the data before splitting into batches. Note that the samples within each split will not be shuffled. (default: :obj:`False`)
         random_state (int, optional): When shuffle is :obj:`True`, :obj:`random_state` affects the ordering of the indices, which controls the randomness of each fold. Otherwise, this parameter has no effect. (default: :obj:`None`)
         split_path (str): The path to data partition information. If the path exists, read the existing partition from the path. If the path does not exist, the current division method will be saved for next use. If set to None, a random path will be generated. (default: :obj:`None`)
     '''
     if split_path is None:
         split_path = get_random_dir_path(dir_prefix='model_selection')
 
     if not os.path.exists(split_path):
+        log.info(f'📊 | Create the split of train and test set.')
         log.info(
-            f'📊 | Create the split of train and test set. Please set split_path to {split_path} for the next run, if you want to use the same setting for the experiment.'
+            f'😊 | Please set \033[92msplit_path\033[0m to \033[92m{split_path}\033[0m for the next run, if you want to use the same setting for the experiment.'
         )
         os.makedirs(split_path)
         info = dataset.info
         subjects = list(set(info['subject_id']))
 
-        train_info = None
-        test_info = None
+        assert subject in subjects, f'The subject should be in the subject list {subjects}.'
 
-        for subject in subjects:
-            subject_info = info[info['subject_id'] == subject]
-            trial_ids = list(set(subject_info['trial_id']))
-
-            train_index_trial_ids, test_index_trial_ids = model_selection.train_test_split(
-                trial_ids,
-                test_size=test_size,
-                shuffle=shuffle,
-                random_state=random_state)
-
-            if len(train_index_trial_ids) == 0 or len(
-                    test_index_trial_ids) == 0:
-                raise ValueError(
-                    f'The number of training or testing trials for subject {subject} is zero.'
-                )
-
-            train_trial_ids = np.array(
-                trial_ids)[train_index_trial_ids].tolist()
-            test_trial_ids = np.array(trial_ids)[test_index_trial_ids].tolist()
-
-            subject_train_info = []
-            for train_trial_id in train_trial_ids:
-                subject_train_info.append(
-                    subject_info[subject_info['trial_id'] == train_trial_id])
-            subject_train_info = pd.concat(subject_train_info,
-                                           ignore_index=True)
-
-            subject_test_info = []
-            for test_trial_id in test_trial_ids:
-                subject_test_info.append(
-                    subject_info[subject_info['trial_id'] == test_trial_id])
-            subject_test_info = pd.concat(subject_test_info, ignore_index=True)
-
-            if train_info is None and test_info is None:
-                train_info = [subject_train_info]
-                test_info = [subject_test_info]
-            else:
-                train_info.append(subject_train_info)
-                test_info.append(subject_test_info)
+        subject_info = info[info['subject_id'] == subject]
+        trial_ids = list(set(subject_info['trial_id']))
 
+        train_trial_ids, test_trial_ids = model_selection.train_test_split(
+            trial_ids,
+            test_size=test_size,
+            shuffle=shuffle,
+            random_state=random_state)
+
+        if len(train_trial_ids) == 0 or len(test_trial_ids) == 0:
+            raise ValueError(
+                f'The number of training or testing trials for subject {subject} is zero.'
+            )
+
+        train_info = []
+        for train_trial_id in train_trial_ids:
+            train_info.append(
+                subject_info[subject_info['trial_id'] == train_trial_id])
         train_info = pd.concat(train_info, ignore_index=True)
+
+        test_info = []
+        for test_trial_id in test_trial_ids:
+            test_info.append(
+                subject_info[subject_info['trial_id'] == test_trial_id])
         test_info = pd.concat(test_info, ignore_index=True)
 
         train_info.to_csv(os.path.join(split_path, 'train.csv'), index=False)
         test_info.to_csv(os.path.join(split_path, 'test.csv'), index=False)
 
     else:
         log.info(
-            f'Read the split of train and test set from {split_path}. If you want to use the same setting for the experiment, please set split_path to {split_path} for the next run.'
+            f'📊 | Detected existing split of train and test set, use existing split from {split_path}.'
+        )
+        log.info(
+            f'💡 | If the dataset is re-generated, you need to re-generate the split of the dataset instead of using the previous split.'
         )
 
     train_info = pd.read_csv(os.path.join(split_path, 'train.csv'))
     test_info = pd.read_csv(os.path.join(split_path, 'test.csv'))
 
     train_dataset = copy(dataset)
     train_dataset.info = train_info
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/split_groupby_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/split_per_subject_groupby_trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,100 +10,114 @@
 from torcheeg.datasets.module.base_dataset import BaseDataset
 
 from ..utils import get_random_dir_path
 
 log = logging.getLogger('torcheeg')
 
 
-def train_test_split_groupby_trial(dataset: BaseDataset,
-                                   test_size: float = 0.2,
-                                   shuffle: bool = False,
-                                   random_state: Union[float, None] = None,
-                                   split_path: Union[None, str] = None):
+def train_test_split_per_subject_groupby_trial(dataset: BaseDataset,
+                                               test_size: float = 0.2,
+                                               subject: str = 's01.dat',
+                                               shuffle: bool = False,
+                                               random_state: Union[float,
+                                                                   None] = None,
+                                               split_path: Union[None,
+                                                                 str] = None):
     r'''
-    A tool function for cross-validations, to divide the training set and the test set. It is suitable for experiments with large dataset volume and no need to use k-fold cross-validations. The test samples are sampled according to a certain proportion, and other samples are used as training samples. In most literatures, 20% of the data are sampled for testing.
+    A tool function for cross-validations, to divide the training set and the test set. It is suitable for subject dependent experiments with large dataset volume and no need to use k-fold cross-validations. For the first step, the EEG signal samples of the specified user are selected. Then, the test samples are sampled according to a certain proportion for each trial for this subject, and other samples are used as training samples. In most literatures, 20% of the data are sampled for testing.
 
-    :obj:`train_test_split_groupby_trial` devides training set and the test set at the dimension of each trial. For example, when :obj:`test_size=0.2`, the first 80% of samples of each trial are used for training, and the last 20% of samples are used for testing. It is more consistent with real applications and can test the generalization of the model to a certain extent.
-
-    .. image:: _static/train_test_split_groupby_trial.png
-        :alt: The schematic diagram of train_test_split_groupby_trial
+    .. image:: _static/train_test_split_per_subject_groupby_trial.png
+        :alt: The schematic diagram of train_test_split_per_subject_groupby_trial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg.model_selection import train_test_split_per_subject_groupby_trial
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
-                                  transforms.To2d(),
-                                  transforms.ToTensor()
+                                  transforms.ToTensor(),
+                                  transforms.To2d()
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select(['valence', 'arousal']),
                                   transforms.Binary(5.0),
                                   transforms.BinariesToCategory()
                               ]))
 
-        train_dataset, test_dataset = train_test_split_groupby_trial(dataset=dataset)
+        train_dataset, test_dataset = train_test_split_per_subject_groupby_trial(dataset=dataset)
 
         train_loader = DataLoader(train_dataset)
         test_loader = DataLoader(test_dataset)
         ...
 
     Args:
         dataset (BaseDataset): Dataset to be divided.
         test_size (int):  If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the test split. If int, represents the absolute number of test samples. (default: :obj:`0.2`)
+        subject (str): The subject whose EEG samples will be used for training and test. (default: :obj:`s01.dat`)
         shuffle (bool): Whether to shuffle the data before splitting into batches. Note that the samples within each split will not be shuffled. (default: :obj:`False`)
         random_state (int, optional): When shuffle is :obj:`True`, :obj:`random_state` affects the ordering of the indices, which controls the randomness of each fold. Otherwise, this parameter has no effect. (default: :obj:`None`)
         split_path (str): The path to data partition information. If the path exists, read the existing partition from the path. If the path does not exist, the current division method will be saved for next use. If set to None, a random path will be generated. (default: :obj:`None`)
     '''
     if split_path is None:
         split_path = get_random_dir_path(dir_prefix='model_selection')
 
     if not os.path.exists(split_path):
+        log.info(f'📊 | Create the split of train and test set.')
         log.info(
-            f'📊 | Create the split of train and test set. Please set split_path to {split_path} for the next run, if you want to use the same setting for the experiment.'
+            f'😊 | Please set \033[92msplit_path\033[0m to \033[92m{split_path}\033[0m for the next run, if you want to use the same setting for the experiment.'
         )
         os.makedirs(split_path)
         info = dataset.info
         subjects = list(set(info['subject_id']))
-        trial_ids = list(set(info['trial_id']))
+
+        assert subject in subjects, f'The subject should be in the subject list {subjects}.'
+
+        subject_info = info[info['subject_id'] == subject]
+        trial_ids = list(set(subject_info['trial_id']))
 
         train_info = None
         test_info = None
 
-        for subject in subjects:
-            for trial_id in trial_ids:
-                cur_info = info[(info['subject_id'] == subject)
-                                & (info['trial_id'] == trial_id)].reset_index()
-
-                n_samples = len(cur_info)
-                indices = np.arange(n_samples)
-                train_index, test_index = model_selection.train_test_split(
-                    indices,
-                    test_size=test_size,
-                    random_state=random_state,
-                    shuffle=shuffle)
-
-                if train_info is None and test_info is None:
-                    train_info = [cur_info.iloc[train_index]]
-                    test_info = [cur_info.iloc[test_index]]
-                else:
-                    train_info.append(cur_info.iloc[train_index])
-                    test_info.append(cur_info.iloc[test_index])
+        for trial_id in trial_ids:
+            cur_info = info[(info['subject_id'] == subject)
+                            & (info['trial_id'] == trial_id)].reset_index()
+            n_samples = len(cur_info)
+            indices = np.arange(n_samples)
+
+            train_index, test_index = model_selection.train_test_split(
+                indices,
+                test_size=test_size,
+                random_state=random_state,
+                shuffle=shuffle)
+
+            if train_info is None and test_info is None:
+                train_info = [cur_info.iloc[train_index]]
+                test_info = [cur_info.iloc[test_index]]
+            else:
+                train_info.append(cur_info.iloc[train_index])
+                test_info.append(cur_info.iloc[test_index])
 
         train_info = pd.concat(train_info, ignore_index=True)
         test_info = pd.concat(test_info, ignore_index=True)
 
         train_info.to_csv(os.path.join(split_path, 'train.csv'), index=False)
         test_info.to_csv(os.path.join(split_path, 'test.csv'), index=False)
 
     else:
         log.info(
-            f'Read the split of train and test set from {split_path}. If you want to use the same setting for the experiment, please set split_path to {split_path} for the next run.'
+            f'📊 | Detected existing split of train and test set, use existing split from {split_path}.'
+        )
+        log.info(
+            f'💡 | If the dataset is re-generated, you need to re-generate the split of the dataset instead of using the previous split.'
         )
 
     train_info = pd.read_csv(os.path.join(split_path, 'train.csv'))
     test_info = pd.read_csv(os.path.join(split_path, 'test.csv'))
 
     train_dataset = copy(dataset)
     train_dataset.info = train_info
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/split_per_subject_cross_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/split_cross_trial.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,105 +10,128 @@
 from torcheeg.datasets.module.base_dataset import BaseDataset
 
 from ..utils import get_random_dir_path
 
 log = logging.getLogger('torcheeg')
 
 
-def train_test_split_per_subject_cross_trial(dataset: BaseDataset,
-                                             test_size: float = 0.2,
-                                             subject: str = 's01.dat',
-                                             shuffle: bool = False,
-                                             random_state: Union[float,
-                                                                 None] = None,
-                                             split_path: Union[None, str] = None):
+def train_test_split_cross_trial(dataset: BaseDataset,
+                                 test_size: float = 0.2,
+                                 shuffle: bool = False,
+                                 random_state: Union[float, None] = None,
+                                 split_path: Union[None, str] = None):
     r'''
-    A tool function for cross-validations, to divide the training set and the test set. It is suitable for subject dependent experiments with large dataset volume and no need to use k-fold cross-validations. For the first step, the EEG signal samples of the specified user are selected. Then, parts of trials are sampled according to a certain proportion as the test dataset, and samples from other trials are used as training samples. In most literatures, 20% of the data are sampled for testing.
+    A tool function for cross-validations, to divide the training set and the test set. It is suitable for experiments with large dataset volume and no need to use k-fold cross-validations. Parts of trials are sampled according to a certain proportion as the test dataset, and samples from other trials are used as training samples. In most literatures, 20% of the data are sampled for testing.
 
-    .. image:: _static/train_test_split_per_subject_cross_trial.png
-        :alt: The schematic diagram of train_test_split_per_subject_cross_trial
+    :obj:`train_test_split_cross_trial` devides training set and the test set at the dimension of each trial. For example, when :obj:`test_size=0.2`, the first 80% of samples of each trial are used for training, and the last 20% of samples are used for testing. It is more consistent with real applications and can test the generalization of the model to a certain extent.
+
+    .. image:: _static/train_test_split_cross_trial.png
+        :alt: The schematic diagram of train_test_split_cross_trial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg.model_selection import train_test_split_cross_trial
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
-                                  transforms.ToTensor(),
-                                  transforms.To2d()
+                                  transforms.To2d(),
+                                  transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select(['valence', 'arousal']),
                                   transforms.Binary(5.0),
                                   transforms.BinariesToCategory()
                               ]))
 
-        train_dataset, test_dataset = train_test_split_per_subject_cross_trial(dataset=dataset)
+        train_dataset, test_dataset = train_test_split_cross_trial(dataset=dataset)
 
         train_loader = DataLoader(train_dataset)
         test_loader = DataLoader(test_dataset)
         ...
 
     Args:
         dataset (BaseDataset): Dataset to be divided.
         test_size (int):  If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the test split. If int, represents the absolute number of test samples. (default: :obj:`0.2`)
-        subject (str): The subject whose EEG samples will be used for training and test. (default: :obj:`s01.dat`)
         shuffle (bool): Whether to shuffle the data before splitting into batches. Note that the samples within each split will not be shuffled. (default: :obj:`False`)
         random_state (int, optional): When shuffle is :obj:`True`, :obj:`random_state` affects the ordering of the indices, which controls the randomness of each fold. Otherwise, this parameter has no effect. (default: :obj:`None`)
         split_path (str): The path to data partition information. If the path exists, read the existing partition from the path. If the path does not exist, the current division method will be saved for next use. If set to None, a random path will be generated. (default: :obj:`None`)
     '''
     if split_path is None:
         split_path = get_random_dir_path(dir_prefix='model_selection')
 
     if not os.path.exists(split_path):
+        log.info(f'📊 | Create the split of train and test set.')
         log.info(
-            f'📊 | Create the split of train and test set. Please set split_path to {split_path} for the next run, if you want to use the same setting for the experiment.'
+            f'😊 | Please set \033[92msplit_path\033[0m to \033[92m{split_path}\033[0m for the next run, if you want to use the same setting for the experiment.'
         )
         os.makedirs(split_path)
         info = dataset.info
         subjects = list(set(info['subject_id']))
 
-        assert subject in subjects, f'The subject should be in the subject list {subjects}.'
+        train_info = None
+        test_info = None
 
-        subject_info = info[info['subject_id'] == subject]
-        trial_ids = list(set(info['trial_id']))
+        for subject in subjects:
+            subject_info = info[info['subject_id'] == subject]
+            trial_ids = list(set(subject_info['trial_id']))
+
+            train_index_trial_ids, test_index_trial_ids = model_selection.train_test_split(
+                trial_ids,
+                test_size=test_size,
+                shuffle=shuffle,
+                random_state=random_state)
+
+            if len(train_index_trial_ids) == 0 or len(
+                    test_index_trial_ids) == 0:
+                raise ValueError(
+                    f'The number of training or testing trials for subject {subject} is zero.'
+                )
+
+            train_trial_ids = np.array(
+                trial_ids)[train_index_trial_ids].tolist()
+            test_trial_ids = np.array(trial_ids)[test_index_trial_ids].tolist()
+
+            subject_train_info = []
+            for train_trial_id in train_trial_ids:
+                subject_train_info.append(
+                    subject_info[subject_info['trial_id'] == train_trial_id])
+            subject_train_info = pd.concat(subject_train_info,
+                                           ignore_index=True)
+
+            subject_test_info = []
+            for test_trial_id in test_trial_ids:
+                subject_test_info.append(
+                    subject_info[subject_info['trial_id'] == test_trial_id])
+            subject_test_info = pd.concat(subject_test_info, ignore_index=True)
+
+            if train_info is None and test_info is None:
+                train_info = [subject_train_info]
+                test_info = [subject_test_info]
+            else:
+                train_info.append(subject_train_info)
+                test_info.append(subject_test_info)
 
-        train_index_trial_ids, test_index_trial_ids = model_selection.train_test_split(
-            trial_ids,
-            test_size=test_size,
-            shuffle=shuffle,
-            random_state=random_state)
-
-        if len(train_index_trial_ids) == 0 or len(test_index_trial_ids) == 0:
-            raise ValueError(
-                f'The number of training or testing trials for subject {subject} is zero.'
-            )
-
-        train_trial_ids = np.array(trial_ids)[train_index_trial_ids].tolist()
-        test_trial_ids = np.array(trial_ids)[test_index_trial_ids].tolist()
-
-        train_info = []
-        for train_trial_id in train_trial_ids:
-            train_info.append(
-                subject_info[subject_info['trial_id'] == train_trial_id])
         train_info = pd.concat(train_info, ignore_index=True)
-
-        test_info = []
-        for test_trial_id in test_trial_ids:
-            test_info.append(
-                subject_info[subject_info['trial_id'] == test_trial_id])
         test_info = pd.concat(test_info, ignore_index=True)
 
         train_info.to_csv(os.path.join(split_path, 'train.csv'), index=False)
         test_info.to_csv(os.path.join(split_path, 'test.csv'), index=False)
 
     else:
         log.info(
-            f'Read the split of train and test set from {split_path}. If you want to use the same setting for the experiment, please set split_path to {split_path} for the next run.'
+            f'📊 | Detected existing split of train and test set, use existing split from {split_path}.'
+        )
+        log.info(
+            f'💡 | If the dataset is re-generated, you need to re-generate the split of the dataset instead of using the previous split.'
         )
 
     train_info = pd.read_csv(os.path.join(split_path, 'train.csv'))
     test_info = pd.read_csv(os.path.join(split_path, 'test.csv'))
 
     train_dataset = copy(dataset)
     train_dataset.info = train_info
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/split_per_subject_groupby_trial.py` & `torcheeg-1.1.2/torcheeg/model_selection/split_groupby_trial.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,103 +10,109 @@
 from torcheeg.datasets.module.base_dataset import BaseDataset
 
 from ..utils import get_random_dir_path
 
 log = logging.getLogger('torcheeg')
 
 
-def train_test_split_per_subject_groupby_trial(dataset: BaseDataset,
-                                               test_size: float = 0.2,
-                                               subject: str = 's01.dat',
-                                               shuffle: bool = False,
-                                               random_state: Union[float,
-                                                                   None] = None,
-                                               split_path: Union[None, str] = None):
+def train_test_split_groupby_trial(dataset: BaseDataset,
+                                   test_size: float = 0.2,
+                                   shuffle: bool = False,
+                                   random_state: Union[float, None] = None,
+                                   split_path: Union[None, str] = None):
     r'''
-    A tool function for cross-validations, to divide the training set and the test set. It is suitable for subject dependent experiments with large dataset volume and no need to use k-fold cross-validations. For the first step, the EEG signal samples of the specified user are selected. Then, the test samples are sampled according to a certain proportion for each trial for this subject, and other samples are used as training samples. In most literatures, 20% of the data are sampled for testing.
+    A tool function for cross-validations, to divide the training set and the test set. It is suitable for experiments with large dataset volume and no need to use k-fold cross-validations. The test samples are sampled according to a certain proportion, and other samples are used as training samples. In most literatures, 20% of the data are sampled for testing.
 
-    .. image:: _static/train_test_split_per_subject_groupby_trial.png
-        :alt: The schematic diagram of train_test_split_per_subject_groupby_trial
+    :obj:`train_test_split_groupby_trial` devides training set and the test set at the dimension of each trial. For example, when :obj:`test_size=0.2`, the first 80% of samples of each trial are used for training, and the last 20% of samples are used for testing. It is more consistent with real applications and can test the generalization of the model to a certain extent.
+
+    .. image:: _static/train_test_split_groupby_trial.png
+        :alt: The schematic diagram of train_test_split_groupby_trial
         :align: center
 
     |
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg.model_selection import train_test_split_groupby_trial
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+
         dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               online_transform=transforms.Compose([
-                                  transforms.ToTensor(),
-                                  transforms.To2d()
+                                  transforms.To2d(),
+                                  transforms.ToTensor()
                               ]),
                               label_transform=transforms.Compose([
                                   transforms.Select(['valence', 'arousal']),
                                   transforms.Binary(5.0),
                                   transforms.BinariesToCategory()
                               ]))
 
-        train_dataset, test_dataset = train_test_split_per_subject_groupby_trial(dataset=dataset)
+        train_dataset, test_dataset = train_test_split_groupby_trial(dataset=dataset)
 
         train_loader = DataLoader(train_dataset)
         test_loader = DataLoader(test_dataset)
         ...
 
     Args:
         dataset (BaseDataset): Dataset to be divided.
         test_size (int):  If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the test split. If int, represents the absolute number of test samples. (default: :obj:`0.2`)
-        subject (str): The subject whose EEG samples will be used for training and test. (default: :obj:`s01.dat`)
         shuffle (bool): Whether to shuffle the data before splitting into batches. Note that the samples within each split will not be shuffled. (default: :obj:`False`)
         random_state (int, optional): When shuffle is :obj:`True`, :obj:`random_state` affects the ordering of the indices, which controls the randomness of each fold. Otherwise, this parameter has no effect. (default: :obj:`None`)
         split_path (str): The path to data partition information. If the path exists, read the existing partition from the path. If the path does not exist, the current division method will be saved for next use. If set to None, a random path will be generated. (default: :obj:`None`)
     '''
     if split_path is None:
         split_path = get_random_dir_path(dir_prefix='model_selection')
 
     if not os.path.exists(split_path):
+        log.info(f'📊 | Create the split of train and test set.')
         log.info(
-            f'📊 | Create the split of train and test set. Please set split_path to {split_path} for the next run, if you want to use the same setting for the experiment.'
+            f'😊 | Please set \033[92msplit_path\033[0m to \033[92m{split_path}\033[0m for the next run, if you want to use the same setting for the experiment.'
         )
         os.makedirs(split_path)
         info = dataset.info
         subjects = list(set(info['subject_id']))
-
-        assert subject in subjects, f'The subject should be in the subject list {subjects}.'
-
         trial_ids = list(set(info['trial_id']))
 
         train_info = None
         test_info = None
 
-        for trial_id in trial_ids:
-            cur_info = info[(info['subject_id'] == subject)
-                            & (info['trial_id'] == trial_id)].reset_index()
-            n_samples = len(cur_info)
-            indices = np.arange(n_samples)
-
-            train_index, test_index = model_selection.train_test_split(
-                indices,
-                test_size=test_size,
-                random_state=random_state,
-                shuffle=shuffle)
-
-            if train_info is None and test_info is None:
-                train_info = [cur_info.iloc[train_index]]
-                test_info = [cur_info.iloc[test_index]]
-            else:
-                train_info.append(cur_info.iloc[train_index])
-                test_info.append(cur_info.iloc[test_index])
+        for subject in subjects:
+            for trial_id in trial_ids:
+                cur_info = info[(info['subject_id'] == subject)
+                                & (info['trial_id'] == trial_id)].reset_index()
+
+                n_samples = len(cur_info)
+                indices = np.arange(n_samples)
+                train_index, test_index = model_selection.train_test_split(
+                    indices,
+                    test_size=test_size,
+                    random_state=random_state,
+                    shuffle=shuffle)
+
+                if train_info is None and test_info is None:
+                    train_info = [cur_info.iloc[train_index]]
+                    test_info = [cur_info.iloc[test_index]]
+                else:
+                    train_info.append(cur_info.iloc[train_index])
+                    test_info.append(cur_info.iloc[test_index])
 
         train_info = pd.concat(train_info, ignore_index=True)
         test_info = pd.concat(test_info, ignore_index=True)
 
         train_info.to_csv(os.path.join(split_path, 'train.csv'), index=False)
         test_info.to_csv(os.path.join(split_path, 'test.csv'), index=False)
 
     else:
         log.info(
-            f'Read the split of train and test set from {split_path}. If you want to use the same setting for the experiment, please set split_path to {split_path} for the next run.'
+            f'📊 | Detected existing split of train and test set, use existing split from {split_path}.'
+        )
+        log.info(
+            f'💡 | If the dataset is re-generated, you need to re-generate the split of the dataset instead of using the previous split.'
         )
 
     train_info = pd.read_csv(os.path.join(split_path, 'train.csv'))
     test_info = pd.read_csv(os.path.join(split_path, 'test.csv'))
 
     train_dataset = copy(dataset)
     train_dataset.info = train_info
```

### Comparing `torcheeg-1.1.1/torcheeg/model_selection/subcategory.py` & `torcheeg-1.1.2/torcheeg/model_selection/subcategory.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     r'''
     A tool class for separating out subsets of specified categories, often used to extract data for a certain type of paradigm, or for a certain type of task. Each subset in the formed subset list contains only one type of data.
     
     Common usage:
 
     .. code-block:: python
 
+        from torcheeg.datasets import M3CVDataset
+        from torcheeg.model_selection import Subcategory
+        from torcheeg import transforms
+        from torcheeg.utils import DataLoader
+        
         cv = Subcategory()
         dataset = M3CVDataset(root_path='./aistudio',
                               online_transform=transforms.Compose(
                                   [transforms.To2d(),
                                    transforms.ToTensor()]),
                               label_transform=transforms.Compose([
                                   transforms.Select('subject_id'),
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/ccnn.py` & `torcheeg-1.1.2/torcheeg/models/cnn/ccnn.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,36 @@
     - URL: https://link.springer.com/chapter/10.1007/978-3-030-04239-4_39
     - Related Project: https://github.com/ynulonger/DE_CNN
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.BandDifferentialEntropy(),
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    online_transform=transforms.ToTensor(),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        from torcheeg.models import CCNN
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              offline_transform=transforms.Compose([
+                                  transforms.BandDifferentialEntropy(),
+                                  transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+                              ]),
+                              online_transform=transforms.ToTensor(),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = CCNN(num_classes=2, in_channels=4, grid_size=(9, 9))
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         in_channels (int): The feature dimension of each electrode. (default: :obj:`4`)
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
         dropout (float): Probability of an element to be zeroed in the dropout layers. (default: :obj:`0.25`)
     '''
     def __init__(self, in_channels: int = 4, grid_size: Tuple[int, int] = (9, 9), num_classes: int = 2, dropout: float = 0.5):
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/eegnet.py` & `torcheeg-1.1.2/torcheeg/models/cnn/eegnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,42 @@
     - URL: https://arxiv.org/abs/1611.08024
     - Related Project: https://github.com/braindecode/braindecode/tree/master/braindecode
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    online_transform=transforms.Compose([
-                        transforms.To2d()
-                        transforms.ToTensor(),
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import EEGNet
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              online_transform=transforms.Compose([
+                                  transforms.To2d(),
+                                  transforms.ToTensor(),
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = EEGNet(chunk_size=128,
                        num_electrodes=32,
                        dropout=0.5,
                        kernel_1=64,
                        kernel_2=16,
                        F1=8,
                        F2=16,
                        D=2,
                        num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         chunk_size (int): Number of data points included in each EEG chunk, i.e., :math:`T` in the paper. (default: :obj:`151`)
         num_electrodes (int): The number of electrodes, i.e., :math:`C` in the paper. (default: :obj:`60`)
         F1 (int): The filter number of block 1, i.e., :math:`F_1` in the paper. (default: :obj:`8`)
         F2 (int): The filter number of block 2, i.e., :math:`F_2` in the paper. (default: :obj:`16`)
         D (int): The depth multiplier (number of spatial filters), i.e., :math:`D` in the paper. (default: :obj:`2`)
         num_classes (int): The number of classes to predict, i.e., :math:`N` in the paper. (default: :obj:`2`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/fbccnn.py` & `torcheeg-1.1.2/torcheeg/models/cnn/fbccnn.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,26 +11,35 @@
     - Paper: Pan B, Zheng W. Emotion Recognition Based on EEG Using Generative Adversarial Nets and Convolutional Neural Network[J]. Computational and Mathematical Methods in Medicine, 2021.
     - URL: https://www.hindawi.com/journals/cmmm/2021/2520394/
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    online_transform=transforms.Compose([
-                        transforms.BandPowerSpectralDensity(),
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        from torcheeg.models import FBCCNN
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              online_transform=transforms.Compose([
+                                  transforms.BandPowerSpectralDensity(),
+                                  transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = FBCCNN(num_classes=2, in_channels=4, grid_size=(9, 9))
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         in_channels (int): The feature dimension of each electrode, i.e., :math:`N` in the paper. (default: :obj:`4`)
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
     '''
     def __init__(self, in_channels: int = 4, grid_size: Tuple[int, int] = (9, 9), num_classes: int = 2):
         super(FBCCNN, self).__init__()
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/fbcnet.py` & `torcheeg-1.1.2/torcheeg/models/cnn/fbcnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,31 +95,39 @@
     - URL: https://arxiv.org/abs/2104.01233
     - Related Project: https://github.com/ravikiran-mane/FBCNet
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    chunk_size=512,
-                    num_baseline=1,
-                    baseline_chunk_size=512,
-                    offline_transform=transforms.BandSignal(),
-                    online_transform=transforms.ToTensor(),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import FBCNet
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              chunk_size=512,
+                              num_baseline=1,
+                              baseline_chunk_size=512,
+                              offline_transform=transforms.BandSignal(),
+                              online_transform=transforms.ToTensor(),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = FBCNet(num_classes=2,
                        num_electrodes=32,
                        chunk_size=512,
                        in_channels=4,
                        num_S=32)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         num_electrodes (int): The number of electrodes. (default: :obj:`28`)
         chunk_size (int): Number of data points included in each EEG chunk. (default: :obj:`1000`)
         in_channels (int): The number of channels of the signal corresponding to each electrode. If the original signal is used as input, in_channels is set to 1; if the original signal is split into multiple sub-bands, in_channels is set to the number of bands. (default: :obj:`9`)
         num_S (int): The number of spatial convolution block. (default: :obj:`32`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
         temporal (str): The temporal layer used, with options including VarLayer, StdLayer, LogVarLayer, MeanLayer, and MaxLayer, used to compute statistics using different techniques in the temporal dimension. (default: :obj:`LogVarLayer`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/fbmsnet.py` & `torcheeg-1.1.2/torcheeg/models/gnn/lggnet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,358 +1,328 @@
-import torch.nn.functional as F
-from typing import Tuple, Optional
+import math
+
 import torch
 import torch.nn as nn
-from .fbcnet import VarLayer, MaxLayer, StdLayer, LogVarLayer, LinearWithConstraint, MeanLayer, swish,Conv2dWithConstraint
+import torch.nn.functional as F
+from torch.nn.modules.module import Module
+from torch.nn.parameter import Parameter
 
 
-## CONV_SAME_PADDING
-def _calc_same_pad(i: int, k: int, s: int, d: int):
-    return max((-(i // -s) - 1) * s + (k - 1) * d + 1 - i, 0)
-
-
-def _same_pad_arg(input_size, kernel_size, stride, dilation, **_):
-    ih, iw = input_size
-    kh, kw = kernel_size
-    pad_h = _calc_same_pad(ih, kh, stride[0], dilation[0])
-    pad_w = _calc_same_pad(iw, kw, stride[1], dilation[1])
-    return [pad_w // 2, pad_w - pad_w // 2, pad_h // 2, pad_h - pad_h // 2]
-
-def conv2d_same(x,
-                weight: torch.Tensor,
-                bias: Optional[torch.Tensor] = None,
-                stride: Tuple[int, int] = (1, 1),
-                padding: Tuple[int, int] = (0, 0),
-                dilation: Tuple[int, int] = (1, 1),
-                groups: int = 1):
-    ih, iw = x.size()[-2:]
-    kh, kw = weight.size()[-2:]
-    pad_h = _calc_same_pad(ih, kh, stride[0], dilation[0])
-    pad_w = _calc_same_pad(iw, kw, stride[1], dilation[1])
-    x = F.pad(x,
-              [pad_w // 2, pad_w - pad_w // 2, pad_h // 2, pad_h - pad_h // 2])
-    return F.conv2d(x, weight, bias, stride, (0, 0), dilation, groups)
-
-
-class SamePadConv2d(nn.Conv2d):
-    """ Tensorflow like 'SAME' convolution wrapper for 2D convolutions
-    """
+class ChannelAttention(nn.Module):
+    def __init__(self, in_channelsnel, ratio=2):
+        super(ChannelAttention, self).__init__()
+        self.max_pool = nn.AdaptiveMaxPool2d(1)
+        self.avg_pool = nn.AdaptiveAvgPool2d(1)
+        self.fc1 = nn.Conv2d(in_channelsnel,
+                             in_channelsnel // ratio,
+                             1,
+                             bias=False)
+        self.relu1 = nn.ReLU()
+        self.fc2 = nn.Conv2d(in_channelsnel // ratio,
+                             in_channelsnel,
+                             1,
+                             bias=False)
+        self.sigmoid = nn.Sigmoid()
 
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 dilation=1,
-                 groups=1,
-                 bias=True):
-        super(SamePadConv2d,
-              self).__init__(in_channels, out_channels, kernel_size, stride, 0,
-                             dilation, groups, bias)
+    def forward(self, x):
+        avg_pool_out = self.avg_pool(x)
+        max_pool_out = self.max_pool(x)
+        avg_pool_out = self.fc2(self.relu1(self.fc1(avg_pool_out)))
+        max_pool_out = self.fc2(self.relu1(self.fc1(max_pool_out)))
+        out = max_pool_out + avg_pool_out
+        return self.sigmoid(out)
+
+
+class SpatialAttention(nn.Module):
+    def __init__(self, kernel_size=7):
+        super(SpatialAttention, self).__init__()
+        assert kernel_size in (3, 7), 'Kernel size must be 3 or 7.'
+        padding = 3 if kernel_size == 7 else 1
+        self.conv1 = nn.Conv2d(2, 1, kernel_size, padding=padding, bias=False)
+        self.sigmoid = nn.Sigmoid()
 
     def forward(self, x):
-        return conv2d_same(x, self.weight, self.bias, self.stride,
-                           self.padding, self.dilation, self.groups)
+        max_pool_out, _ = torch.max(x, dim=1, keepdim=True)
+        avg_pool_out = torch.mean(x, dim=1, keepdim=True)
+        out = torch.cat([avg_pool_out, max_pool_out], dim=1)
+        out = self.conv1(out)
+        return self.sigmoid(out)
 
 
-## MIX_CONV
-def create_conv2d_pad(in_chs, out_chs, kernel_size, **kwargs):
-    padding = kwargs.pop('padding', '')
-    kwargs.setdefault('bias', False)
-    padding, is_dynamic = get_padding_value(padding, kernel_size, **kwargs)
-    if is_dynamic:
-        return SamePadConv2d(in_chs, out_chs, kernel_size, **kwargs)
-    else:
-        if isinstance(kernel_size, tuple):
-            padding = (0, padding)
-        return nn.Conv2d(in_chs,
-                         out_chs,
-                         kernel_size,
-                         padding=padding,
-                         **kwargs)
-
-
-def _is_static_pad(kernel_size, stride=1, dilation=1, **_):
-    return stride == 1 and (dilation * (kernel_size - 1)) % 2 == 0
-
-
-def _get_padding(kernel_size, stride=1, dilation=1, **_):
-    if isinstance(kernel_size, tuple):
-        kernel_size = max(kernel_size)
-    padding = ((stride - 1) + dilation * (kernel_size - 1)) // 2
-    return padding
-
-
-def _split_channels(num_chan, num_groups):
-    split = [num_chan // num_groups for _ in range(num_groups)]
-    split[0] += num_chan - sum(split)
-    return split
-
-
-def get_padding_value(padding, kernel_size, **kwargs):
-    dynamic = False
-    if isinstance(padding, str):
-        # for any string padding, the padding will be calculated for you, one of three ways
-        padding = padding.lower()
-        if padding == 'same':
-            dynamic = True
-            padding = 0
-
-        elif padding == 'valid':
-            # 'VALID' padding, same as padding=0
-            padding = 0
-        else:
-            # Default to PyTorch style 'same'-ish symmetric padding
-            dynamic = True
-            padding = 0
-    else:
-        dynamic = True
-        padding = 0
-    return padding, dynamic
+class CBAMBlock(nn.Module):
+    def __init__(self, in_channelsnel, ratio=2, kernel_size=7):
+        super(CBAMBlock, self).__init__()
+        self.cha_att = ChannelAttention(in_channelsnel, ratio=ratio)
+        self.spa_att = SpatialAttention(kernel_size=kernel_size)
 
+    def forward(self, x):
+        out = x * self.cha_att(x)
+        out = out * self.spa_att(out)
+        return out
 
-class MixedConv2d(nn.ModuleDict):
-    """ Mixed Grouped Convolution
-    Based on MDConv and GroupedConv in MixNet impl:
-      https://github.com/tensorflow/tpu/blob/master/models/official/mnasnet/mixnet/custom_layers.py
-    """
 
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size=3,
-                 stride=1,
-                 padding='same',
-                 dilation=1,
-                 depthwise=False,
-                 **kwargs):
-        super(MixedConv2d, self).__init__()
-
-        kernel_size = kernel_size if isinstance(kernel_size,
-                                                list) else [kernel_size]
-        num_groups = len(kernel_size)
-        in_splits = _split_channels(in_channels, num_groups)
-        out_splits = _split_channels(out_channels, num_groups)
-        self.in_channels = sum(in_splits)
-        self.out_channels = sum(out_splits)
-
-        for idx, (k, in_ch,
-                  out_ch) in enumerate(zip(kernel_size, in_splits,
-                                           out_splits)):
-            conv_groups = out_ch if depthwise else 1
-            self.add_module(
-                str(idx),
-                create_conv2d_pad(in_ch,
-                                  out_ch,
-                                  k,
-                                  stride=stride,
-                                  padding=padding,
-                                  dilation=dilation,
-                                  groups=conv_groups,
-                                  **kwargs))
-        self.splits = in_splits
+class PowerLayer(nn.Module):
+    def __init__(self, kernel_size, stride):
+        super(PowerLayer, self).__init__()
+        self.pooling = nn.AvgPool2d(kernel_size=(1, kernel_size),
+                                    stride=(1, stride))
 
     def forward(self, x):
-        x_split = torch.split(x, self.splits, 1)
-        x_out = [conv(x_split[i]) for i, conv in enumerate(self.values())]
-        x = torch.cat(x_out, 1)
-        return x
+        return torch.log(self.pooling(x.pow(2)))
 
 
+class Aggregator():
+    def __init__(self, region_list):
+        self.region_list = region_list
 
+    def forward(self, x):
+        output = []
+        for region_index in range(len(self.region_list)):
+            region_x = x[:, self.region_list[region_index], :]
+            aggr_region_x = torch.mean(region_x, dim=1)
+            output.append(aggr_region_x)
+        return torch.stack(output, dim=1)
 
 
-class FBMSNet(nn.Module):
-    r'''
-        FBMSNet, a novel multiscale temporal convolutional neural network for MI decoding tasks, employs Mixed Conv to extract multiscale temporal features which  enhance the intra-class compactness and improve the inter-class separability with the joint supervision of the center loss andcenter loss.
+class GraphConvolution(Module):
+    def __init__(self, in_channels, out_channels, bias=True):
+        super(GraphConvolution, self).__init__()
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.weight = Parameter(torch.FloatTensor(in_channels, out_channels))
 
-        - Paper: FBMSNet: A Filter-Bank Multi-Scale Convolutional Neural Network for EEG-Based Motor Imagery Decoding
-        - URL: https://ieeexplore.ieee.org/document/9837422
-        - Related Project: https://github.com/Want2Vanish/FBMSNet
-
-        Below is a example to explain how to use this model. Firstly we should transform eeg signal to several nonoverlapping frequency bands by :obj:`torcheeg.transforms.BandSignal` 
-
-        .. code-block:: python
-
-            # Define 9 nonoverlapping frequency bands, each with a 4 Hz bandwidth and spanning from 4 to 40 Hz.
-            Freq_range_per_band = {'sub band1': [4, 8],
-                                'sub band2': [8, 12],
-                                'sub band3': [12, 16],
-                                'sub band4': [16, 20],
-                                'sub band5': [20, 24],
-                                'sub band6': [24, 28],
-                                'sub band7': [28, 32],
-                                'sub band8': [32, 36],
-                                'sub band9': [36, 40]}
-            dataset =BCICIV2aDataset(io_path=f'./tmp_out/bciciv2a/band_9_filters',
-                                    root_path='./BCICIV_2a_mat',
-                                    chunk_size=512,
-                                    offline_transform=transforms.BandSignal(band_dict=Freq_range_per_band,
-                                                                            sampling_rate=250),
-                                    online_transform=transforms.ToTensor(),
-                                    label_transform=transforms.Compose([
-                                    transforms.Select('label'),
-                                    transforms.Lambda(lambda x:x-1),
-                        ]))
-            data = Dataloader(dataset)
-
-            model = FBMSNet(num_classes=4,
-                            num_electrodes=22,
-                            chunk_size=512,
-                            in_channels=9 )
-
-        There are two ways to use the model. The first one, the effective way to get the prediction result but it don't output the decoded feature. 
-
-        .. code-block:: python
-
-            x,y = next(iter(data))
-            pred = model(x)
-
-        To obtain the decoded feature, use :obj:`decoder` method. If we want to obtain prediction results based on the encoded features, use :obj:`classifier` method.
-
-        .. code-block:: python
-
-            x,y = next(iter(data))
-            feature = model.decoder(x)
-            pred = model.classifier(feature)
+        if bias:
+            self.bias = Parameter(
+                torch.zeros((1, 1, out_channels), dtype=torch.float32))
+        else:
+            self.register_parameter('bias', None)
+        nn.init.xavier_uniform_(self.weight, gain=1.414)
 
-        Args:
-            num_electrodes (int): The number of electrodes. 
-            chunk_size (int): Number of data points included in each EEG chunk. 
-            in_channels (int): The number of channels of the signal corresponding to each electrode. If the original signal is used as input, in_channels is set to 1; if the original signal is split into multiple sub-bands, in_channels is set to the number of bands. (default: :obj:`9`)
-            num_classes (int): The number of classes to predict. (default: :obj:`4`)
-            stride_factor (int): The stride factor. Please make sure the chunk_size parameter is a  multiple of stride_factor parameter in order to init model successfully. (default: :obj:`4`)
-            temporal (str): The temporal layer used, with options including VarLayer, StdLayer, LogVarLayer, MeanLayer, and MaxLayer, used to compute statistics using different techniques in the temporal dimension. (default: :obj:`LogVarLayer`)
-            num_feature (int): The number of Mixed Conv output channels which can stand for various kinds of feature. (default: :obj:`36`)
-            dilatability (int): The expansion multiple of the channels after the input bands pass through spatial convolutional blocks. (default: :obj:`8`
+    def reset_parameters(self):
+        stdv = 1. / math.sqrt(self.weight.size(1))
+        self.weight.data.uniform_(-stdv, stdv)
+        if self.bias is not None:
+            self.bias.data.uniform_(-stdv, stdv)
+
+    def forward(self, x, adj):
+        output = torch.matmul(x, self.weight) - self.bias
+        output = F.relu(torch.matmul(adj, output))
+        return output
 
-        .. automethod:: decoder
-        .. automethod:: classifier
-    '''
 
-    def __init__(self,
-                 in_channels: int,
-                 num_electrodes: int,
-                 chunk_size: int,
-                 num_classes: int = 4,
-                 stride_factor: int = 4,
-                 temporal: str = 'LogVarLayer',
-                 num_feature: int = 36,
-                 dilatability: int = 8):
+class LGGNet(nn.Module):
+    r'''
+    DLocal-Global-Graph Networks (LGGNet). For more details, please refer to the following information.
 
-        super(FBMSNet, self).__init__()
+    - Paper: Ding Y, Robinson N, Zeng Q, et al. LGGNet: learning from Local-global-graph representations for brain-computer interface[J]. arXiv preprint arXiv:2105.02786, 2021.
+    - URL: https://arxiv.org/abs/2105.02786
+    - Related Project: https://github.com/yi-ding-cs/LGG
+
+    Below is a recommended suite for use in emotion recognition tasks:
+
+    .. code-block:: python
+
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg.models import LGGNet
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import SEED_GENERAL_REGION_LIST
+
+        dataset = SEEDDataset(root_path='./Preprocessed_EEG',
+                              offline_transform=transforms.Compose([
+                                  transforms.MeanStdNormalize(),
+                                  transforms.To2d()
+                              ]),
+                              online_transform=transforms.Compose([
+                                  transforms.ToTensor()
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('emotion'),
+                                  transforms.Lambda(lambda x: x + 1)
+                              ]))
+        model = LGGNet(region_list=SEED_GENERAL_REGION_LIST, chunk_size=128, num_electrodes=32, hid_channels=32, num_classes=2)
+        
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
+    The current built-in :obj:`region_list` includs:
+
+    - torcheeg.datasets.constants.emotion_recognition.amigos.AMIGOS_GENERAL_REGION_LIST
+    - torcheeg.datasets.constants.emotion_recognition.amigos.AMIGOS_FRONTAL_REGION_LIST
+    - torcheeg.datasets.constants.emotion_recognition.amigos.AMIGOS_HEMISPHERE_REGION_LIST
+    - torcheeg.datasets.constants.emotion_recognition.deap.DEAP_GENERAL_REGION_LIST
+    - ...
+    - torcheeg.datasets.constants.emotion_recognition.dreamer.DREAMER_GENERAL_REGION_LIST
+    - ...
+    - torcheeg.datasets.constants.emotion_recognition.mahnob.MAHNOB_GENERAL_REGION_LIST
+    - ...
+    - torcheeg.datasets.constants.emotion_recognition.seed.SEED_GENERAL_REGION_LIST
+    - ...
+
+    Args:
+        region_list (list): The local graph structure defined according to the 10-20 system, where the electrodes are divided into different brain regions.
+        in_channels (int): The feature dimension of each electrode. (default: :obj:`1`)
+        num_electrodes (int): The number of electrodes. (default: :obj:`32`)
+        chunk_size (int): Number of data points included in each EEG chunk. (default: :obj:`128`)
+        sampling_rate (int): The sampling rate of the EEG signals, i.e., :math:`f_s` in the paper. (default: :obj:`128`)
+        num_T (int): The number of multi-scale 1D temporal kernels in the dynamic temporal layer, i.e., :math:`T` kernels in the paper. (default: :obj:`64`)
+        hid_channels (int): The number of hidden nodes in the first fully connected layer. (default: :obj:`32`)
+        dropout (float): Probability of an element to be zeroed in the dropout layers. (default: :obj:`0.5`)
+        pool_kernel_size (int): The kernel size of pooling layers in the temporal blocks (default: :obj:`16`)
+        pool_stride (int): The stride of pooling layers in the temporal blocks (default: :obj:`4`)
+        num_classes (int): The number of classes to predict. (default: :obj:`2`)
+    '''
+    def __init__(self,
+                 region_list,
+                 in_channels: int = 1,
+                 num_electrodes: int = 32,
+                 chunk_size: int = 128,
+                 sampling_rate: int = 128,
+                 num_T: int = 64,
+                 hid_channels: int = 32,
+                 dropout: float = 0.5,
+                 pool_kernel_size: int = 16,
+                 pool_stride: int = 4,
+                 num_classes: int = 2):
+        super(LGGNet, self).__init__()
+        self.region_list = region_list
+        self.inception_window = [0.5, 0.25, 0.125]
 
         self.num_classes = num_classes
         self.in_channels = in_channels
         self.num_electrodes = num_electrodes
         self.chunk_size = chunk_size
-        self.stride_factor = stride_factor
-
-        try:
-            self.mixConv2d = nn.Sequential(
-                MixedConv2d(in_channels=in_channels,
-                            out_channels=num_feature,
-                            kernel_size=[(1, 15), (1, 31), (1, 63), (1, 125)],
-                            stride=1,
-                            padding='',
-                            dilation=1,
-                            depthwise=False),
-                nn.BatchNorm2d(num_feature),
-            )
-            self.scb = self.SCB(in_chan=num_feature,
-                                out_chan=num_feature * dilatability,
-                                num_electrodes=int(num_electrodes))
-
-            # Formulate the temporal agreegator
-            if temporal == 'VarLayer':
-                self.temporal_layer = VarLayer(dim=3)
-            elif temporal == 'StdLayer':
-                self.temporal_layer = StdLayer(dim=3)
-            elif temporal == 'LogVarLayer':
-                self.temporal_layer = LogVarLayer(dim=3)
-            elif temporal == 'MeanLayer':
-                self.temporal_layer = MeanLayer(dim=3)
-            elif temporal == 'MaxLayer':
-                self.temporal_layer = MaxLayer(dim=3)
-            else:
-                raise NotImplementedError
-
-            self.center_dim = self.feature_dim(in_channels, num_electrodes,
-                                               chunk_size)[-1]
-
-            self.fc = self.LastBlock(self.center_dim, num_classes)
-        except:
-            raise Exception(
-                "Model init failed: The Chunksize must be a  multiple of stride_factor.Please modify values of stride_factor or chunk_size."
-            )
-
-    def SCB(self,
-            in_chan,
-            out_chan,
-            num_electrodes,
-            weight_norm=True,
-            *args,
-            **kwargs):
-        return nn.Sequential(
-            Conv2dWithConstraint(in_chan,
-                                 out_chan, (num_electrodes, 1),
-                                 groups=in_chan,
-                                 max_norm=2,
-                                 weight_norm=weight_norm,
-                                 padding=0), nn.BatchNorm2d(out_chan), swish())
-
-    def LastBlock(self, inF, outF, weight_norm=True, *args, **kwargs):
-        return nn.Sequential(
-            LinearWithConstraint(inF,
-                                 outF,
-                                 max_norm=0.5,
-                                 weight_norm=weight_norm,
-                                 *args,
-                                 **kwargs), nn.LogSoftmax(dim=1))
-
-    def decoder(self, x):
-        r'''
-        Args:
-            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, in_channel, num_electrodes, chunk_size ]`. Here, :obj:`n` corresponds to the batch size, :obj:`in_channels` corresponds to the number of sub bands.
+        self.sampling_rate = sampling_rate
+        self.num_T = num_T
+        self.hid_channels = hid_channels
+        self.dropout = dropout
+        self.pool_kernel_size = pool_kernel_size
+        self.pool_stride = pool_stride
+        self.in_channels = in_channels
+        self.num_electrodes = num_electrodes
 
-        Returns:
-           torch.Tensor[size of batch, length of deep feature code]: The extracted deep features.
-        '''
-        x = self.mixConv2d(x)
-        x = self.scb(x)
-        x = x.reshape([
-            *x.shape[0:2], self.stride_factor,
-            int(x.shape[3] / self.stride_factor)
-        ])
-        x = self.temporal_layer(x)
-        return torch.flatten(x, start_dim=1)
+        self.t_block1 = self.temporal_block(
+            self.in_channels, self.num_T,
+            (1, int(self.inception_window[0] * self.sampling_rate)),
+            self.pool_kernel_size, self.pool_stride)
+        self.t_block2 = self.temporal_block(
+            self.in_channels, self.num_T,
+            (1, int(self.inception_window[1] * self.sampling_rate)),
+            self.pool_kernel_size, self.pool_stride)
+        self.t_block3 = self.temporal_block(
+            self.in_channels, self.num_T,
+            (1, int(self.inception_window[2] * self.sampling_rate)),
+            self.pool_kernel_size, self.pool_stride)
+
+        self.bn_t1 = nn.BatchNorm2d(self.num_T)
+        self.bn_t2 = nn.BatchNorm2d(self.num_T)
+
+        self.cbam = CBAMBlock(num_electrodes)
+
+        self.conv1x1 = nn.Sequential(
+            nn.Conv2d(num_T, num_T, kernel_size=(1, 1), stride=(1, 1)),
+            nn.LeakyReLU(), nn.AvgPool2d((1, 2)))
+
+        self.avg_pool = nn.AvgPool2d((1, 2))
+
+        feature_dim = self.feature_dim
+        self.local_filter_weight = nn.Parameter(torch.FloatTensor(
+            self.num_electrodes, feature_dim),
+                                                requires_grad=True)
+        self.local_filter_bias = nn.Parameter(torch.zeros(
+            (1, self.num_electrodes, 1), dtype=torch.float32),
+                                              requires_grad=True)
+
+        self.aggregate = Aggregator(self.region_list)
+        num_region = len(self.region_list)
+
+        self.global_adj = nn.Parameter(torch.FloatTensor(
+            num_region, num_region),
+                                       requires_grad=True)
+
+        self.bn_g1 = nn.BatchNorm1d(num_region)
+        self.bn_g2 = nn.BatchNorm1d(num_region)
+
+        self.gcn = GraphConvolution(feature_dim, hid_channels)
+
+        self.fc = nn.Sequential(
+            nn.Dropout(p=dropout),
+            nn.Linear(int(num_region * hid_channels), num_classes))
 
-    def classifier(self, feature):
-        r'''
-        With feature which is ouput by decoder inputed,the classifier ouput the predicted probability that the samples belong to the classes. 
+        nn.init.xavier_uniform_(self.local_filter_weight)
+        nn.init.xavier_uniform_(self.global_adj)
 
-        Args:
-            feature (torch.Tensor): The extracted deep features. The ideal input shape is :obj:`[batch size,1152]`where feature dim is fixed as :obj:`1152`.
-        Returns:
-           torch.Tensor[size of batch, num_classes]: The predicted probability that the samples belong to the classes.
-        '''
-        return self.fc(feature)
+    def temporal_block(self, in_channels, out_channels, kernel_size,
+                       pool_kernel_size, pool_stride):
+        return nn.Sequential(
+            nn.Conv2d(in_channels,
+                      out_channels,
+                      kernel_size=kernel_size,
+                      stride=(1, 1)),
+            PowerLayer(kernel_size=pool_kernel_size, stride=pool_stride))
 
     def forward(self, x):
         r'''
         Args:
-            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, in_channel, num_electrodes, chunk_size ]`. Here, :obj:`n` corresponds to the batch size
+            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 1, 32, 128]`. Here, :obj:`n` corresponds to the batch size, :obj:`32` corresponds to :obj:`num_electrodes`, and :obj:`chunk_size` corresponds to :obj:`chunk_size`.
 
         Returns:
-            torch.Tensor[size of batch,number of classes]: The predicted probability that the samples belong to the classes.
+            torch.Tensor[number of sample, number of classes]: the predicted probability that the samples belong to the classes.
         '''
-        f = self.decoder(x)
-        return self.classifier(f)
+        t1 = self.t_block1(x)
+        t2 = self.t_block2(x)
+        t3 = self.t_block3(x)
+        x = torch.cat((t1, t2, t3), dim=-1)
+
+        x = self.bn_t1(x)
+
+        x = x.permute(0, 2, 1, 3)
+        x = self.cbam(x)
+        x = self.avg_pool(x)
+
+        x = x.flatten(start_dim=2)
+        x = self.local_filter(x)
+        x = self.aggregate.forward(x)
+        adj = self.get_adj(x)
+        x = self.bn_g1(x)
+        
+        x = self.gcn(x, adj)
+        x = self.bn_g2(x)
+        x = x.view(x.shape[0], -1)
+        x = self.fc(x)
+        return x
+
+    @property
+    def feature_dim(self):
+        mock_eeg = torch.randn(
+            (1, self.in_channels, self.num_electrodes, self.chunk_size))
+
+        t1 = self.t_block1(mock_eeg)
+        t2 = self.t_block2(mock_eeg)
+        t3 = self.t_block3(mock_eeg)
+        mock_eeg = torch.cat((t1, t2, t3), dim=-1)
+
+        mock_eeg = self.bn_t1(mock_eeg)
+        mock_eeg = self.conv1x1(mock_eeg)
+        mock_eeg = self.bn_t2(mock_eeg)
+        mock_eeg = mock_eeg.permute(0, 2, 1, 3)
+        mock_eeg = mock_eeg.flatten(start_dim=2)
+        return mock_eeg.shape[-1]
+
+    def local_filter(self, x):
+        w = self.local_filter_weight.unsqueeze(0).repeat(x.shape[0], 1, 1)
+        x = F.relu(torch.mul(x, w) - self.local_filter_bias)
+        return x
 
-    def feature_dim(self, in_channels, num_electrodes, chunk_size):
-        data = torch.ones((1, in_channels, num_electrodes, chunk_size))
-        x = self.mixConv2d(data)
-        x = self.scb(x)
-        x = x.reshape([*x.shape[0:2], self.stride_factor, -1])
-        x = self.temporal_layer(x)
-        x = torch.flatten(x, start_dim=1)
-        return x.size()
+    def get_adj(self, x, self_loop=True):
+        adj = torch.bmm(x, x.permute(0, 2, 1))
+        num_nodes = adj.shape[-1]
+        adj = F.relu(adj * (self.global_adj + self.global_adj.transpose(1, 0)))
+        if self_loop:
+            adj = adj + torch.eye(num_nodes).to(x.device)
+        rowsum = torch.sum(adj, dim=-1)
+        mask = torch.zeros_like(rowsum)
+        mask[rowsum == 0] = 1
+        rowsum += mask
+        d_inv_sqrt = torch.pow(rowsum, -0.5)
+        d_mat_inv_sqrt = torch.diag_embed(d_inv_sqrt)
+        adj = torch.bmm(torch.bmm(d_mat_inv_sqrt, adj), d_mat_inv_sqrt)
+        return adj
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/mtcnn.py` & `torcheeg-1.1.2/torcheeg/models/cnn/mtcnn.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,40 +11,50 @@
     - Paper: Rudakov E, Laurent L, Cousin V, et al. Multi-Task CNN model for emotion recognition from EEG Brain maps[C]//2021 4th International Conference on Bio-Engineering for Smart Technologies (BioSMART). IEEE, 2021: 1-4.
     - URL: https://ieeexplore.ieee.org/abstract/document/9677807
     - Related Project: https://github.com/dolphin-in-a-coma/multi-task-cnn-eeg-emotion/
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
-    
+
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT, DEAP_CHANNEL_LIST
+        from torcheeg.models import MTCNN
+        from torcheeg.datasets.constants.emotion_recognition.utils import format_channel_location_dict
+        from torch.utils.data import DataLoader
+
         DEAP_LOCATION_LIST = [['-', '-', 'AF3', 'FP1', '-', 'FP2', 'AF4', '-', '-'],
                               ['F7', '-', 'F3', '-', 'FZ', '-', 'F4', '-', 'F8'],
                               ['-', 'FC5', '-', 'FC1', '-', 'FC2', '-', 'FC6', '-'],
                               ['T7', '-', 'C3', '-', 'CZ', '-', 'C4', '-', 'T8'],
                               ['-', 'CP5', '-', 'CP1', '-', 'CP2', '-', 'CP6', '-'],
                               ['P7', '-', 'P3', '-', 'PZ', '-', 'P4', '-', 'P8'],
                               ['-', '-', '-', 'PO3', '-', 'PO4', '-', '-', '-'],
                               ['-', '-', '-', 'O1', 'OZ', 'O2', '-', '-', '-']]
         DEAP_CHANNEL_LOCATION_DICT = format_channel_location_dict(DEAP_CHANNEL_LIST, DEAP_LOCATION_LIST)
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    online_transform=transforms.Compose([
-                        transforms.Concatenate([
-                            transforms.BandDifferentialEntropy(),
-                            transforms.BandPowerSpectralDensity()
-                        ]),
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              online_transform=transforms.Compose([
+                                  transforms.Concatenate([
+                                      transforms.BandDifferentialEntropy(),
+                                      transforms.BandPowerSpectralDensity()
+                                  ]),
+                                  transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = MTCNN(num_classes=2, in_channels=8, grid_size=(8, 9), dropout=0.2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         in_channels (int): The feature dimension of each electrode, i.e., :math:`N` in the paper. (default: :obj:`4`)
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(8, 9)`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
         dropout (float): Probability of an element to be zeroed in the dropout layers. (default: :obj:`0.2`)
     '''
     def __init__(self,
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/sst_emotion_net.py` & `torcheeg-1.1.2/torcheeg/models/cnn/sst_emotion_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,41 +14,50 @@
     - URL: https://dl.acm.org/doi/abs/10.1145/3394171.3413724
     - Related Project: https://github.com/ziyujia/SST-EmotionNet
     - Related Project: https://github.com/LexieLiu01/SST-Emotion-Net-Pytorch-Version-
     
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
-    
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.BaselineRemoval(),
-                        transforms.Concatenate([
-                            transforms.Compose([
-                                transforms.BandDifferentialEntropy(sampling_rate=128),
-                                transforms.MeanStdNormalize()
-                            ]),
-                            transforms.Compose([
-                                transforms.Downsample(num_points=32),
-                                transforms.MinMaxNormalize()
-                            ])
-                        ]),
-                        transforms.ToInterpolatedGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    online_transform=transforms.Compose([
-                        transforms.ToTensor(),
-                        transforms.Resize((16, 16))
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        from torcheeg.models import SSTEmotionNet
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              offline_transform=transforms.Compose([
+                                  transforms.BaselineRemoval(),
+                                  transforms.Concatenate([
+                                      transforms.Compose([
+                                          transforms.BandDifferentialEntropy(sampling_rate=128),
+                                          transforms.MeanStdNormalize()
+                                      ]),
+                                      transforms.Compose([
+                                          transforms.Downsample(num_points=32),
+                                          transforms.MinMaxNormalize()
+                                      ])
+                                  ]),
+                                  transforms.ToInterpolatedGrid(DEAP_CHANNEL_LOCATION_DICT)
+                              ]),
+                              online_transform=transforms.Compose([
+                                  transforms.ToTensor(),
+                                  transforms.Resize((16, 16))
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = SSTEmotionNet(temporal_in_channels=32, spectral_in_channels=4, grid_size=(16, 16), num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(16, 16)`)
         spectral_in_channels (int): How many 2D maps are stacked in the 3D spatial-spectral representation. (default: :obj:`5`)
         temporal_in_channels (int): How many 2D maps are stacked in the 3D spatial-temporal representation. (default: :obj:`25`)
         spectral_depth (int): The number of layers in spatial-spectral stream. (default: :obj:`16`)
         temporal_depth (int): The number of layers in spatial-temporal stream. (default: :obj:`22`)
         spectral_growth_rate (int): The growth rate of spatial-spectral stream. (default: :obj:`12`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/stnet.py` & `torcheeg-1.1.2/torcheeg/models/gnn/dgcnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,167 @@
-from typing import Tuple
-
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
 
 
-class InceptionConv2d(nn.Module):
-    def __init__(self, in_channels: int, out_channels: int, bias: bool = True):
-        super().__init__()
-        self.conv5x5 = nn.Conv2d(in_channels, out_channels, kernel_size=5, stride=1, padding=2, bias=bias)
-        self.conv3x3 = nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=1, bias=bias)
-        self.conv1x1 = nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0, bias=bias)
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.conv5x5(x) + self.conv3x3(x) + self.conv1x1(x)
-
+class GraphConvolution(nn.Module):
+    def __init__(self, in_channels: int, out_channels: int, bias: bool=False):
 
-class SeparableConv2d(nn.Module):
-    def __init__(self,
-                 in_channels: int,
-                 out_channels: int,
-                 kernel_size: int = 3,
-                 stride: int = 1,
-                 padding: int = 1,
-                 bias: bool = True):
-        super().__init__()
-        self.depth = nn.Conv2d(in_channels,
-                               in_channels,
-                               kernel_size=kernel_size,
-                               stride=stride,
-                               padding=padding,
-                               groups=in_channels,
-                               bias=bias)
-        self.point = nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=stride, padding=0, bias=bias)
+        super(GraphConvolution, self).__init__()
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        x = self.depth(x)
-        x = self.point(x)
-        return x
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.weight = nn.Parameter(torch.FloatTensor(in_channels, out_channels))
+        nn.init.xavier_normal_(self.weight)
+        self.bias = None
+        if bias:
+            self.bias = nn.Parameter(torch.FloatTensor(out_channels))
+            nn.init.zeros_(self.bias)
+
+    def forward(self, x: torch.Tensor, adj: torch.Tensor) -> torch.Tensor:
+        out = torch.matmul(adj, x)
+        out = torch.matmul(out, self.weight)
+        if self.bias is not None:
+            return out + self.bias
+        else:
+            return out
+
+
+class Linear(nn.Module):
+    def __init__(self, in_channels: int, out_channels: int, bias: bool=True):
+        super(Linear, self).__init__()
+        self.linear = nn.Linear(in_channels, out_channels, bias=bias)
+        nn.init.xavier_normal_(self.linear.weight)
+        if bias:
+            nn.init.zeros_(self.linear.bias)
+
+    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
+        return self.linear(inputs)
+
+
+def normalize_A(A: torch.Tensor, symmetry: bool=False) -> torch.Tensor:
+    A = F.relu(A)
+    if symmetry:
+        A = A + torch.transpose(A, 0, 1)
+        d = torch.sum(A, 1)
+        d = 1 / torch.sqrt(d + 1e-10)
+        D = torch.diag_embed(d)
+        L = torch.matmul(torch.matmul(D, A), D)
+    else:
+        d = torch.sum(A, 1)
+        d = 1 / torch.sqrt(d + 1e-10)
+        D = torch.diag_embed(d)
+        L = torch.matmul(torch.matmul(D, A), D)
+    return L
+
+
+def generate_cheby_adj(A: torch.Tensor, num_layers: int) -> torch.Tensor:
+    support = []
+    for i in range(num_layers):
+        if i == 0:
+            support.append(torch.eye(A.shape[1]).to(A.device))
+        elif i == 1:
+            support.append(A)
+        else:
+            temp = torch.matmul(support[-1], A)
+            support.append(temp)
+    return support
+
+
+class Chebynet(nn.Module):
+    def __init__(self, in_channels: int, num_layers: int, out_channels: int):
+        super(Chebynet, self).__init__()
+        self.num_layers = num_layers
+        self.gc1 = nn.ModuleList()
+        for i in range(num_layers):
+            self.gc1.append(GraphConvolution(in_channels, out_channels))
+
+    def forward(self, x: torch.Tensor, L: torch.Tensor) -> torch.Tensor:
+        adj = generate_cheby_adj(L, self.num_layers)
+        for i in range(len(self.gc1)):
+            if i == 0:
+                result = self.gc1[i](x, adj[i])
+            else:
+                result = result+  self.gc1[i](x, adj[i])
+        result = F.relu(result)
+        return result
 
 
-class STNet(nn.Module):
+class DGCNN(nn.Module):
     r'''
-    Spatio-temporal Network (STNet). For more details, please refer to the following information.
+    Dynamical Graph Convolutional Neural Networks (DGCNN). For more details, please refer to the following information.
 
-    - Paper: Zhang Z, Zhong S, Liu Y. GANSER: A Self-supervised Data Augmentation Framework for EEG-based Emotion Recognition[J]. IEEE Transactions on Affective Computing, 2022.
-    - URL: https://ieeexplore.ieee.org/abstract/document/9763358/
-    - Related Project: https://github.com/tczhangzhi/GANSER-PyTorch
+    - Paper: Song T, Zheng W, Song P, et al. EEG emotion recognition using dynamical graph convolutional neural networks[J]. IEEE Transactions on Affective Computing, 2018, 11(3): 532-541.
+    - URL: https://ieeexplore.ieee.org/abstract/document/8320798
+    - Related Project: https://github.com/xueyunlong12589/DGCNN
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    online_transform=transforms.ToTensor(),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
-        model = STNet(num_classes=2, chunk_size=128, grid_size=(9, 9), dropout=0.2)
+        from torcheeg.models import DGCNN
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg import transforms
+
+        dataset = SEEDDataset(root_path='./Preprocessed_EEG',
+                              offline_transform=transforms.BandDifferentialEntropy(band_dict={
+                                  "delta": [1, 4],
+                                  "theta": [4, 8],
+                                  "alpha": [8, 14],
+                                  "beta": [14, 31],
+                                  "gamma": [31, 49]
+                              }),
+                              online_transform=transforms.Compose([
+                                  transforms.ToTensor()
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('emotion'),
+                                  transforms.Lambda(lambda x: x + 1)
+                              ]))
+
+        model = DGCNN(in_channels=5, num_electrodes=62, hid_channels=32, num_layers=2, num_classes=2)
+
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
 
     Args:
-        chunk_size (int): Number of data points included in each EEG chunk, i.e., :math:`T` in the paper. (default: :obj:`128`)
-        grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
+        in_channels (int): The feature dimension of each electrode. (default: :obj:`5`)
+        num_electrodes (int): The number of electrodes. (default: :obj:`62`)
+        num_layers (int): The number of graph convolutional layers. (default: :obj:`2`)
+        hid_channels (int): The number of hidden nodes in the first fully connected layer. (default: :obj:`32`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
-        dropout (float): Probability of an element to be zeroed in the dropout layers. (default: :obj:`0.2`)
     '''
     def __init__(self,
-                 chunk_size: int = 128,
-                 grid_size: Tuple[int, int] = (9, 9),
-                 num_classes: int = 2,
-                 dropout: float = 0.2):
-        super(STNet, self).__init__()
+                 in_channels: int = 5,
+                 num_electrodes: int = 62,
+                 num_layers: int = 2,
+                 hid_channels: int = 32,
+                 num_classes: int = 2):
+        super(DGCNN, self).__init__()
+        self.in_channels = in_channels
+        self.num_electrodes = num_electrodes
+        self.hid_channels = hid_channels
+        self.num_layers = num_layers
         self.num_classes = num_classes
-        self.chunk_size = chunk_size
-        self.dropout = dropout
-        self.grid_size = grid_size
-
-        self.layer1 = nn.Conv2d(chunk_size, 256, kernel_size=3, stride=1, padding=1, bias=True)
-        self.layer2 = nn.Conv2d(256, 128, kernel_size=5, stride=1, padding=2, bias=True)
-        self.layer3 = nn.Conv2d(128, 64, kernel_size=5, stride=1, padding=2, bias=True)
-        self.layer4 = SeparableConv2d(64, 32, kernel_size=5, stride=1, padding=2, bias=True)
-        self.layer5 = InceptionConv2d(32, 16)
-
-        self.drop_selu = nn.Sequential(nn.Dropout(p=dropout), nn.SELU())
-
-        self.lin1 = nn.Linear(self.feature_dim, 1024, bias=True)
-        self.lin2 = nn.Linear(1024, num_classes, bias=True)
-
-    @property
-    def feature_dim(self):
-        with torch.no_grad():
-            mock_eeg = torch.zeros(1, self.chunk_size, *self.grid_size)
-
-            mock_eeg = self.layer1(mock_eeg)
-            mock_eeg = self.drop_selu(mock_eeg)
-            mock_eeg = self.layer2(mock_eeg)
-            mock_eeg = self.drop_selu(mock_eeg)
-            mock_eeg = self.layer3(mock_eeg)
-            mock_eeg = self.drop_selu(mock_eeg)
-            mock_eeg = self.layer4(mock_eeg)
-            mock_eeg = self.drop_selu(mock_eeg)
-            mock_eeg = self.layer5(mock_eeg)
-            mock_eeg = self.drop_selu(mock_eeg)
-            mock_eeg = mock_eeg.flatten(start_dim=1)
 
-            return mock_eeg.shape[1]
+        self.layer1 = Chebynet(in_channels, num_layers, hid_channels)
+        self.BN1 = nn.BatchNorm1d(in_channels)
+        self.fc1 = Linear(num_electrodes * hid_channels, 64)
+        self.fc2 = Linear(64, num_classes)
+        self.A = nn.Parameter(torch.FloatTensor(num_electrodes, num_electrodes))
+        nn.init.xavier_normal_(self.A)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         r'''
         Args:
-            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 128, 9, 9]`. Here, :obj:`n` corresponds to the batch size, :obj:`128` corresponds to :obj:`chunk_size`, and :obj:`(9, 9)` corresponds to :obj:`grid_size`.
+            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 62, 5]`. Here, :obj:`n` corresponds to the batch size, :obj:`62` corresponds to :obj:`num_electrodes`, and :obj:`5` corresponds to :obj:`in_channels`.
 
         Returns:
             torch.Tensor[number of sample, number of classes]: the predicted probability that the samples belong to the classes.
         '''
-        x = self.layer1(x)
-        x = self.drop_selu(x)
-        x = self.layer2(x)
-        x = self.drop_selu(x)
-        x = self.layer3(x)
-        x = self.drop_selu(x)
-        x = self.layer4(x)
-        x = self.drop_selu(x)
-        x = self.layer5(x)
-        x = self.drop_selu(x)
-        x = x.flatten(start_dim=1)
-        x = self.lin1(x)
-        x = self.drop_selu(x)
-        x = self.lin2(x)
-        return x
+        x = self.BN1(x.transpose(1, 2)).transpose(1, 2)
+        L = normalize_A(self.A)
+        result = self.layer1(x, L)
+        result = result.reshape(x.shape[0], -1)
+        result = F.relu(self.fc1(result))
+        result = self.fc2(result)
+        return result
```

### Comparing `torcheeg-1.1.1/torcheeg/models/cnn/tsception.py` & `torcheeg-1.1.2/torcheeg/models/cnn/tsception.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,53 +10,63 @@
     - URL: https://arxiv.org/abs/2104.02935
     - Related Project: https://github.com/yi-ding-cs/TSception
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    chunk_size=512,
-                    num_baseline=1,
-                    baseline_chunk_size=512,
-                    offline_transform=transforms.Compose([
-                        PickElectrode(PickElectrode.to_index_list(
-                        ['FP1', 'AF3', 'F3', 'F7',
-                        'FC5', 'FC1', 'C3', 'T7',
-                        'CP5', 'CP1', 'P3', 'P7',
-                        'PO3','O1', 'FP2', 'AF4',
-                        'F4', 'F8', 'FC6', 'FC2',
-                        'C4', 'T8', 'CP6', 'CP2',
-                        'P4', 'P8', 'PO4', 'O2'], DEAP_CHANNEL_LIST)),
-                        transforms.To2d()
-                    ]),
-                    online_transform=transforms.ToTensor(),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LIST
+        from torcheeg.models import TSCeption
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              chunk_size=512,
+                              num_baseline=1,
+                              baseline_chunk_size=512,
+                              offline_transform=transforms.Compose([
+                                  transforms.PickElectrode(PickElectrode.to_index_list(
+                                  ['FP1', 'AF3', 'F3', 'F7',
+                                  'FC5', 'FC1', 'C3', 'T7',
+                                  'CP5', 'CP1', 'P3', 'P7',
+                                  'PO3','O1', 'FP2', 'AF4',
+                                  'F4', 'F8', 'FC6', 'FC2',
+                                  'C4', 'T8', 'CP6', 'CP2',
+                                  'P4', 'P8', 'PO4', 'O2'], DEAP_CHANNEL_LIST)),
+                                  transforms.To2d()
+                              ]),
+                              online_transform=transforms.ToTensor(),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = TSCeption(num_classes=2,
                           num_electrodes=28,
                           sampling_rate=128,
                           num_T=15,
                           num_S=15,
                           hid_channels=32,
                           dropout=0.5)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         num_electrodes (int): The number of electrodes. (default: :obj:`28`)
         num_T (int): The number of multi-scale 1D temporal kernels in the dynamic temporal layer, i.e., :math:`T` kernels in the paper. (default: :obj:`15`)
         num_S (int): The number of multi-scale 1D spatial kernels in the asymmetric spatial layer. (default: :obj:`15`)
         in_channels (int): The number of channels of the signal corresponding to each electrode. If the original signal is used as input, in_channels is set to 1; if the original signal is split into multiple sub-bands, in_channels is set to the number of bands. (default: :obj:`1`)
         hid_channels (int): The number of hidden nodes in the first fully connected layer. (default: :obj:`32`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
         sampling_rate (int): The sampling rate of the EEG signals, i.e., :math:`f_s` in the paper. (default: :obj:`128`)
         dropout (float): Probability of an element to be zeroed in the dropout layers. (default: :obj:`0.5`)
     '''
+
     def __init__(self,
                  num_electrodes: int = 28,
                  num_T: int = 15,
                  num_S: int = 15,
                  in_channels: int = 1,
                  hid_channels: int = 32,
                  num_classes: int = 2,
@@ -73,33 +83,47 @@
         self.sampling_rate = sampling_rate
         self.dropout = dropout
 
         self.inception_window = [0.5, 0.25, 0.125]
         self.pool = 8
         # by setting the convolutional kernel being (1,lenght) and the strids being 1 we can use conv2d to
         # achieve the 1d convolution operation
-        self.Tception1 = self.conv_block(in_channels, num_T, (1, int(self.inception_window[0] * sampling_rate)), 1, self.pool)
-        self.Tception2 = self.conv_block(in_channels, num_T, (1, int(self.inception_window[1] * sampling_rate)), 1, self.pool)
-        self.Tception3 = self.conv_block(in_channels, num_T, (1, int(self.inception_window[2] * sampling_rate)), 1, self.pool)
-
-        self.Sception1 = self.conv_block(num_T, num_S, (int(num_electrodes), 1), 1, int(self.pool * 0.25))
-        self.Sception2 = self.conv_block(num_T, num_S, (int(num_electrodes * 0.5), 1), (int(num_electrodes * 0.5), 1),
+        self.Tception1 = self.conv_block(
+            in_channels, num_T,
+            (1, int(self.inception_window[0] * sampling_rate)), 1, self.pool)
+        self.Tception2 = self.conv_block(
+            in_channels, num_T,
+            (1, int(self.inception_window[1] * sampling_rate)), 1, self.pool)
+        self.Tception3 = self.conv_block(
+            in_channels, num_T,
+            (1, int(self.inception_window[2] * sampling_rate)), 1, self.pool)
+
+        self.Sception1 = self.conv_block(num_T, num_S, (int(num_electrodes), 1),
+                                         1, int(self.pool * 0.25))
+        self.Sception2 = self.conv_block(num_T, num_S,
+                                         (int(num_electrodes * 0.5), 1),
+                                         (int(num_electrodes * 0.5), 1),
                                          int(self.pool * 0.25))
         self.fusion_layer = self.conv_block(num_S, num_S, (3, 1), 1, 4)
         self.BN_t = nn.BatchNorm2d(num_T)
         self.BN_s = nn.BatchNorm2d(num_S)
         self.BN_fusion = nn.BatchNorm2d(num_S)
 
-        self.fc = nn.Sequential(nn.Linear(num_S, hid_channels), nn.ReLU(), nn.Dropout(dropout),
+        self.fc = nn.Sequential(nn.Linear(num_S, hid_channels), nn.ReLU(),
+                                nn.Dropout(dropout),
                                 nn.Linear(hid_channels, num_classes))
 
-    def conv_block(self, in_channels: int, out_channels: int, kernel: int, stride: int, pool_kernel: int) -> nn.Module:
+    def conv_block(self, in_channels: int, out_channels: int, kernel: int,
+                   stride: int, pool_kernel: int) -> nn.Module:
         return nn.Sequential(
-            nn.Conv2d(in_channels=in_channels, out_channels=out_channels, kernel_size=kernel, stride=stride),
-            nn.LeakyReLU(), nn.AvgPool2d(kernel_size=(1, pool_kernel), stride=(1, pool_kernel)))
+            nn.Conv2d(in_channels=in_channels,
+                      out_channels=out_channels,
+                      kernel_size=kernel,
+                      stride=stride), nn.LeakyReLU(),
+            nn.AvgPool2d(kernel_size=(1, pool_kernel), stride=(1, pool_kernel)))
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         r'''
         Args:
             x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 1, 28, 512]`. Here, :obj:`n` corresponds to the batch size, :obj:`1` corresponds to number of channels for convolution, :obj:`28` corresponds to :obj:`num_electrodes`, and :obj:`512` corresponds to the input dimension for each electrode.
 
         Returns:
```

### Comparing `torcheeg-1.1.1/torcheeg/models/ddpm/bcddpm.py` & `torcheeg-1.1.2/torcheeg/models/ddpm/bcddpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,17 @@
     - URL: https://arxiv.org/abs/2006.11239
     - Related Project: https://github.com/dome272/Diffusion-Models-pytorch
 
     Below is a recommended suite for use in EEG generation:
 
     .. code-block:: python
 
-        .. code-block:: python
+        import torch
+
+        from torcheeg.models.ddpm import BCUNet
 
         noise = torch.randn(1, 4, 9, 9)
         t = torch.randint(low=1, high=1000, size=(1, ))
         y = torch.randint(low=0, high=2, size=(1, ))
         unet = BCUNet(num_classes=2)
         fake_X = unet(noise, t, y)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/ddpm/bddpm.py` & `torcheeg-1.1.2/torcheeg/models/ddpm/bddpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,18 @@
     - URL: https://arxiv.org/abs/2006.11239
     - Related Project: https://github.com/dome272/Diffusion-Models-pytorch
 
     Below is a recommended suite for use in EEG generation:
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models import BUNet
+        
         noise = torch.randn(1, 4, 9, 9)
         t = torch.randint(low=1, high=1000, size=(1, ))
         unet = BUNet()
         fake_X = unet(noise, t)
 
     Args:
         in_channels (int): The feature dimension of each electrode. (default: :obj:`4`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/flow/bcglow.py` & `torcheeg-1.1.2/torcheeg/models/flow/bcglow.py`

 * *Files 2% similar despite different names*

```diff
@@ -622,14 +622,18 @@
     - Related Project: https://github.com/y0ast/Glow-PyTorch
     - Related Project: https://github.com/ikostrikov/pytorch-flows/
 
     Below is a recommended suite for use in EEG generation:
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models.flow import BGlow
+        
         eeg = torch.randn(1, 4, 32, 32)
         y = torch.randint(0, 2, (2, ))
         model = BGlow(num_classes=2)
         nll_loss, y_logits = model(eeg, y)
         fake_X = model.sample(y=y, temperature=1.0)
 
     Args:
```

### Comparing `torcheeg-1.1.1/torcheeg/models/flow/bglow.py` & `torcheeg-1.1.2/torcheeg/models/flow/bglow.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,14 +623,18 @@
     - Related Project: https://github.com/y0ast/Glow-PyTorch/
     - Related Project: https://github.com/ikostrikov/pytorch-flows/
 
     Below is a recommended suite for use in EEG generation:
     
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models.flow.bglow import BGlow
+        
         eeg = torch.randn(1, 4, 32, 32)
         model = BGlow()
         nll_loss = model(eeg)
         fake_X = model(num=1, temperature=1.0)
 
     Args:
         in_channels (int): The feature dimension of each electrode. (default: :obj:`4`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/gan/bcgan.py` & `torcheeg-1.1.2/torcheeg/models/gan/bcgan.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     r'''
     GAN-based methods formulate a zero-sum game between the generator and the discriminator. The generator is optimized to generate simulation samples that are indistinguishable by the discriminator, and the discriminator is optimized to discriminate false samples generated by the generator. This class provide a baseline implementation for the generator. In particular, the expected labels are additionally provided to guide the generator to generate samples of the specified class from the random noise.
 
     - Related Project: https://github.com/eriklindernoren/PyTorch-GAN/
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models.gan.bcgan import BCGenerator
+
         g_model = BCGenerator(in_channels=128, num_classes=3)
         z = torch.normal(mean=0, std=1, size=(1, 128))
         y = torch.randint(low=0, high=3, size=(1,))
         fake_X = g_model(z, y)
 
     Args:
         in_channels (int): The input feature dimension (of noise vectors). (default: :obj:`128`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/gan/bgan.py` & `torcheeg-1.1.2/torcheeg/models/gan/bgan.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 class BGenerator(nn.Module):
     r'''
     TorchEEG provides an EEG feature generator based on CNN architecture and GAN for generating EEG grid representations of different frequency bands based on a given class label.
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models.gan.bgan import BGenerator
+        
         g_model = BGenerator(in_channels=128)
         z = torch.normal(mean=0, std=1, size=(1, 128))
         fake_X = g_model(z)
 
     Args:
         in_channels (int): The input feature dimension (of noise vectors). (default: :obj:`128`)
         out_channels (int): The generated feature dimension of each electrode. (default: :obj:`4`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/gan/eegfusenet.py` & `torcheeg-1.1.2/torcheeg/models/gan/eegfusenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     EEGFuseNet: A hybrid unsupervised network which can fuse high-dimensional EEG to obtain deep feature characterization and generate similar signals. For more details, please refer to the following information.
 
     - Paper: Z. Liang, R. Zhou, L. Zhang, L. Li, G. Huang, Z. Zhang, and S. Ishii, EEGFuseNet: Hybrid Unsupervised Deep Feature Characterization and Fusion for High-Dimensional EEG With an #Application to Emotion Recognition, IEEE Transactions on Neural Systems and Rehabilitation Engineering, 29, pp. 1913-1925, 2021.
     - URL: https://github.com/KAZABANA/EEGfusenet
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models.gan.eegfusenet import EEGfuseNet
+        
         model = EEGfuseNet(num_electrodes=20,
                            hid_channels_gru=16,
                            num_layers_gru=1,
                            hid_channels_cnn=1,
                            chunk_size=128)
         input = torch.rand(2, 1, 20, 128)
         output, features = model(output)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/gnn/dgcnn.py` & `torcheeg-1.1.2/torcheeg/models/transformer/vanilla_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,187 @@
+from typing import Tuple
+
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
+from einops import rearrange, repeat
+from einops.layers.torch import Rearrange
+from torch import nn
+
+
+class FeedForward(nn.Module):
+    def __init__(self, in_channels: int, hid_channels: int):
+        super().__init__()
+        self.net = nn.Sequential(
+            nn.LayerNorm(in_channels),
+            nn.Linear(in_channels, hid_channels),
+            nn.GELU(),
+            nn.Linear(hid_channels, in_channels),
+        )
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return self.net(x)
 
 
-class GraphConvolution(nn.Module):
-    def __init__(self, in_channels: int, out_channels: int, bias: bool=False):
+class Attention(nn.Module):
+    def __init__(self,
+                 hid_channels: int,
+                 heads: int = 8,
+                 head_channels: int = 64):
+        super().__init__()
+        inner_channels = head_channels * heads
+        self.heads = heads
+        self.scale = head_channels**-0.5
+        self.norm = nn.LayerNorm(hid_channels)
 
-        super(GraphConvolution, self).__init__()
+        self.attend = nn.Softmax(dim=-1)
 
-        self.in_channels = in_channels
-        self.out_channels = out_channels
-        self.weight = nn.Parameter(torch.FloatTensor(in_channels, out_channels))
-        nn.init.xavier_normal_(self.weight)
-        self.bias = None
-        if bias:
-            self.bias = nn.Parameter(torch.FloatTensor(out_channels))
-            nn.init.zeros_(self.bias)
-
-    def forward(self, x: torch.Tensor, adj: torch.Tensor) -> torch.Tensor:
-        out = torch.matmul(adj, x)
-        out = torch.matmul(out, self.weight)
-        if self.bias is not None:
-            return out + self.bias
-        else:
-            return out
-
-
-class Linear(nn.Module):
-    def __init__(self, in_channels: int, out_channels: int, bias: bool=True):
-        super(Linear, self).__init__()
-        self.linear = nn.Linear(in_channels, out_channels, bias=bias)
-        nn.init.xavier_normal_(self.linear.weight)
-        if bias:
-            nn.init.zeros_(self.linear.bias)
-
-    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
-        return self.linear(inputs)
-
-
-def normalize_A(A: torch.Tensor, symmetry: bool=False) -> torch.Tensor:
-    A = F.relu(A)
-    if symmetry:
-        A = A + torch.transpose(A, 0, 1)
-        d = torch.sum(A, 1)
-        d = 1 / torch.sqrt(d + 1e-10)
-        D = torch.diag_embed(d)
-        L = torch.matmul(torch.matmul(D, A), D)
-    else:
-        d = torch.sum(A, 1)
-        d = 1 / torch.sqrt(d + 1e-10)
-        D = torch.diag_embed(d)
-        L = torch.matmul(torch.matmul(D, A), D)
-    return L
-
-
-def generate_cheby_adj(A: torch.Tensor, num_layers: int) -> torch.Tensor:
-    support = []
-    for i in range(num_layers):
-        if i == 0:
-            support.append(torch.eye(A.shape[1]).to(A.device))
-        elif i == 1:
-            support.append(A)
-        else:
-            temp = torch.matmul(support[-1], A)
-            support.append(temp)
-    return support
-
-
-class Chebynet(nn.Module):
-    def __init__(self, in_channels: int, num_layers: int, out_channels: int):
-        super(Chebynet, self).__init__()
-        self.num_layers = num_layers
-        self.gc1 = nn.ModuleList()
-        for i in range(num_layers):
-            self.gc1.append(GraphConvolution(in_channels, out_channels))
-
-    def forward(self, x: torch.Tensor, L: torch.Tensor) -> torch.Tensor:
-        adj = generate_cheby_adj(L, self.num_layers)
-        for i in range(len(self.gc1)):
-            if i == 0:
-                result = self.gc1[i](x, adj[i])
-            else:
-                result += self.gc1[i](x, adj[i])
-        result = F.relu(result)
-        return result
+        self.to_qkv = nn.Linear(hid_channels, inner_channels * 3, bias=False)
+        self.to_out = nn.Linear(inner_channels, hid_channels, bias=False)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        x = self.norm(x)
+
+        qkv = self.to_qkv(x).chunk(3, dim=-1)
+        q, k, v = map(
+            lambda t: rearrange(t, 'b n (h d) -> b h n d', h=self.heads), qkv)
+
+        dots = torch.matmul(q, k.transpose(-1, -2)) * self.scale
+
+        attn = self.attend(dots)
+
+        out = torch.matmul(attn, v)
+        out = rearrange(out, 'b h n d -> b n (h d)')
+        return self.to_out(out)
+
+
+class Transformer(nn.Module):
+    def __init__(self, hid_channels: int, depth: int, heads: int,
+                 head_channels: int, mlp_channels: int):
+        super().__init__()
+        self.layers = nn.ModuleList([])
+        for _ in range(depth):
+            self.layers.append(
+                nn.ModuleList([
+                    Attention(hid_channels,
+                              heads=heads,
+                              head_channels=head_channels),
+                    FeedForward(hid_channels, mlp_channels)
+                ]))
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        for attn, ff in self.layers:
+            x = attn(x) + x
+            x = ff(x) + x
+        return x
 
 
-class DGCNN(nn.Module):
+class VanillaTransformer(nn.Module):
     r'''
-    Dynamical Graph Convolutional Neural Networks (DGCNN). For more details, please refer to the following information.
+    A vanilla version of the transformer adapted on EEG analysis. For more details, please refer to the following information. 
 
-    - Paper: Song T, Zheng W, Song P, et al. EEG emotion recognition using dynamical graph convolutional neural networks[J]. IEEE Transactions on Affective Computing, 2018, 11(3): 532-541.
-    - URL: https://ieeexplore.ieee.org/abstract/document/8320798
-    - Related Project: https://github.com/xueyunlong12589/DGCNN
+    It is worth noting that this model is not designed for EEG analysis, but shows good performance and can serve as a good research start.
+
+    - Paper: Vaswani A, Shazeer N, Parmar N, et al. Attention is all you need[J]. Advances in neural information processing systems, 2017, 30.
+    - URL: https://arxiv.org/abs/1706.03762
+    - Related Project: https://github.com/huggingface/transformers
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = SEEDDataset(io_path=f'./seed',
-                              root_path='./Preprocessed_EEG',
-                              offline_transform=transforms.BandDifferentialEntropy(band_dict={
-                                  "delta": [1, 4],
-                                  "theta": [4, 8],
-                                  "alpha": [8, 14],
-                                  "beta": [14, 31],
-                                  "gamma": [31, 49]
-                              }),
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg.models import VanillaTransformer
+        from torcheeg import transforms
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              offline_transform=transforms.To2d(),
                               online_transform=transforms.Compose([
-                                  transforms.ToTensor()
+                                  transforms.ToTensor(),
                               ]),
                               label_transform=transforms.Compose([
-                                  transforms.Select('emotion'),
-                                  transforms.Lambda(lambda x: x + 1)
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
                               ]))
-        model = DGCNN(in_channels=5, num_electrodes=62, hid_channels=32, num_layers=2, num_classes=2)
+
+        model = VanillaTransformer(chunk_size=128,
+                            num_electrodes=32,
+                            patch_size=32,
+                            hid_channels=32,
+                            depth=3,
+                            heads=4,
+                            head_channels=64,
+                            mlp_channels=64,
+                            num_classes=2)
+        
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
 
     Args:
-        in_channels (int): The feature dimension of each electrode. (default: :obj:`5`)
-        num_electrodes (int): The number of electrodes. (default: :obj:`62`)
-        num_layers (int): The number of graph convolutional layers. (default: :obj:`2`)
-        hid_channels (int): The number of hidden nodes in the first fully connected layer. (default: :obj:`32`)
+        chunk_size (int): Number of data points included in each EEG chunk. (default: :obj:`128`)
+        grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
+        patch_size (tuple): The size (resolution) of each input patch. (default: :obj:`(3, 3)`)
+        hid_channels (int): The feature dimension of embeded patch. (default: :obj:`32`)
+        depth (int): The number of attention layers for each transformer block. (default: :obj:`3`)
+        heads (int): The number of attention heads for each attention layer. (default: :obj:`4`)
+        head_channels (int): The dimension of each attention head for each attention layer. (default: :obj:`8`)
+        mlp_channels (int): The number of hidden nodes in the fully connected layer of each transformer block. (default: :obj:`64`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
     '''
     def __init__(self,
-                 in_channels: int = 5,
-                 num_electrodes: int = 62,
-                 num_layers: int = 2,
+                 num_electrodes: int = 32,
+                 chunk_size: int = 128,
+                 t_patch_size: int = 32,
                  hid_channels: int = 32,
+                 depth: int = 3,
+                 heads: int = 4,
+                 head_channels: int = 8,
+                 mlp_channels: int = 64,
                  num_classes: int = 2):
-        super(DGCNN, self).__init__()
-        self.in_channels = in_channels
+        super(VanillaTransformer, self).__init__()
         self.num_electrodes = num_electrodes
+        self.chunk_size = chunk_size
+        self.t_patch_size = t_patch_size
         self.hid_channels = hid_channels
-        self.num_layers = num_layers
+        self.depth = depth
+        self.heads = heads
+        self.head_channels = head_channels
+        self.mlp_channels = mlp_channels
         self.num_classes = num_classes
 
-        self.layer1 = Chebynet(in_channels, num_layers, hid_channels)
-        self.BN1 = nn.BatchNorm1d(in_channels)
-        self.fc1 = Linear(num_electrodes * hid_channels, 64)
-        self.fc2 = Linear(64, num_classes)
-        self.A = nn.Parameter(torch.FloatTensor(num_electrodes, num_electrodes))
-        nn.init.xavier_normal_(self.A)
+        assert chunk_size % t_patch_size == 0, f'EEG chunk size {chunk_size} must be divisible by the patch size {t_patch_size}.'
+
+        self.to_patch_embedding = nn.Sequential(
+            Rearrange('b c (w p) -> b (c w) p', p=t_patch_size),
+            nn.Linear(t_patch_size, hid_channels),
+        )
+        num_patches = num_electrodes * (chunk_size // t_patch_size)
+        self.pos_embedding = nn.Parameter(
+            torch.randn(1, num_patches + 1, hid_channels))
+        self.cls_token = nn.Parameter(torch.randn(1, 1, hid_channels))
+
+        self.transformer = Transformer(hid_channels, depth, heads,
+                                       head_channels, mlp_channels)
+
+        self.linear_head = nn.Sequential(nn.LayerNorm(hid_channels),
+                                         nn.Linear(hid_channels, num_classes))
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         r'''
         Args:
-            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 62, 5]`. Here, :obj:`n` corresponds to the batch size, :obj:`62` corresponds to :obj:`num_electrodes`, and :obj:`5` corresponds to :obj:`in_channels`.
+            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 1, 32, 128]`. Here, :obj:`n` corresponds to the batch size, :obj:`32` corresponds to :obj:`num_electrodes`, and :obj:`chunk_size` corresponds to :obj:`chunk_size`.
 
         Returns:
             torch.Tensor[number of sample, number of classes]: the predicted probability that the samples belong to the classes.
         '''
-        x = self.BN1(x.transpose(1, 2)).transpose(1, 2)
-        L = normalize_A(self.A)
-        result = self.layer1(x, L)
-        result = result.reshape(x.shape[0], -1)
-        result = F.relu(self.fc1(result))
-        result = self.fc2(result)
-        return result
+        x = self.to_patch_embedding(x)
+
+        b, n, _ = x.shape
+
+        cls_tokens = repeat(self.cls_token, '1 1 d -> b 1 d', b=b)
+        x = torch.cat((cls_tokens, x), dim=1)
+
+        x += self.pos_embedding[:, :(n + 1)]
+
+        x = self.transformer(x)
+        x = x.mean(dim=1)
+
+        return self.linear_head(x)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/gnn/lggnet.py` & `torcheeg-1.1.2/torcheeg/models/transformer/vit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,321 +1,267 @@
-import math
+from typing import Tuple
 
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn.modules.module import Module
-from torch.nn.parameter import Parameter
-
-
-class ChannelAttention(nn.Module):
-    def __init__(self, in_channelsnel, ratio=2):
-        super(ChannelAttention, self).__init__()
-        self.max_pool = nn.AdaptiveMaxPool2d(1)
-        self.avg_pool = nn.AdaptiveAvgPool2d(1)
-        self.fc1 = nn.Conv2d(in_channelsnel,
-                             in_channelsnel // ratio,
-                             1,
-                             bias=False)
-        self.relu1 = nn.ReLU()
-        self.fc2 = nn.Conv2d(in_channelsnel // ratio,
-                             in_channelsnel,
-                             1,
-                             bias=False)
-        self.sigmoid = nn.Sigmoid()
-
-    def forward(self, x):
-        avg_pool_out = self.avg_pool(x)
-        max_pool_out = self.max_pool(x)
-        avg_pool_out = self.fc2(self.relu1(self.fc1(avg_pool_out)))
-        max_pool_out = self.fc2(self.relu1(self.fc1(max_pool_out)))
-        out = max_pool_out + avg_pool_out
-        return self.sigmoid(out)
-
-
-class SpatialAttention(nn.Module):
-    def __init__(self, kernel_size=7):
-        super(SpatialAttention, self).__init__()
-        assert kernel_size in (3, 7), 'Kernel size must be 3 or 7.'
-        padding = 3 if kernel_size == 7 else 1
-        self.conv1 = nn.Conv2d(2, 1, kernel_size, padding=padding, bias=False)
-        self.sigmoid = nn.Sigmoid()
-
-    def forward(self, x):
-        max_pool_out, _ = torch.max(x, dim=1, keepdim=True)
-        avg_pool_out = torch.mean(x, dim=1, keepdim=True)
-        out = torch.cat([avg_pool_out, max_pool_out], dim=1)
-        out = self.conv1(out)
-        return self.sigmoid(out)
-
-
-class CBAMBlock(nn.Module):
-    def __init__(self, in_channelsnel, ratio=2, kernel_size=7):
-        super(CBAMBlock, self).__init__()
-        self.cha_att = ChannelAttention(in_channelsnel, ratio=ratio)
-        self.spa_att = SpatialAttention(kernel_size=kernel_size)
-
-    def forward(self, x):
-        out = x * self.cha_att(x)
-        out = out * self.spa_att(out)
-        return out
-
-
-class PowerLayer(nn.Module):
-    def __init__(self, kernel_size, stride):
-        super(PowerLayer, self).__init__()
-        self.pooling = nn.AvgPool2d(kernel_size=(1, kernel_size),
-                                    stride=(1, stride))
-
-    def forward(self, x):
-        return torch.log(self.pooling(x.pow(2)))
-
-
-class Aggregator():
-    def __init__(self, region_list):
-        self.region_list = region_list
-
-    def forward(self, x):
-        output = []
-        for region_index in range(len(self.region_list)):
-            region_x = x[:, self.region_list[region_index], :]
-            aggr_region_x = torch.mean(region_x, dim=1)
-            output.append(aggr_region_x)
-        return torch.stack(output, dim=1)
-
-
-class GraphConvolution(Module):
-    def __init__(self, in_channels, out_channels, bias=True):
-        super(GraphConvolution, self).__init__()
-        self.in_channels = in_channels
-        self.out_channels = out_channels
-        self.weight = Parameter(torch.FloatTensor(in_channels, out_channels))
-
-        if bias:
-            self.bias = Parameter(
-                torch.zeros((1, 1, out_channels), dtype=torch.float32))
-        else:
-            self.register_parameter('bias', None)
-        nn.init.xavier_uniform_(self.weight, gain=1.414)
-
-    def reset_parameters(self):
-        stdv = 1. / math.sqrt(self.weight.size(1))
-        self.weight.data.uniform_(-stdv, stdv)
-        if self.bias is not None:
-            self.bias.data.uniform_(-stdv, stdv)
-
-    def forward(self, x, adj):
-        output = torch.matmul(x, self.weight) - self.bias
-        output = F.relu(torch.matmul(adj, output))
-        return output
+from einops import rearrange, repeat
+from einops.layers.torch import Rearrange
+from torch import nn
 
 
-class LGGNet(nn.Module):
+def pair(t):
+    return t if isinstance(t, tuple) else (t, t)
+
+
+class PreNorm(nn.Module):
+    def __init__(self, in_channels: int, fn: nn.Module):
+        super(PreNorm, self).__init__()
+        self.norm = nn.LayerNorm(in_channels)
+        self.fn = fn
+
+    def forward(self, x, **kwargs):
+        return self.fn(self.norm(x), **kwargs)
+
+
+class FeedForward(nn.Module):
+    def __init__(self,
+                 in_channels: int,
+                 hid_channels: int,
+                 dropout: float = 0.):
+        super(FeedForward, self).__init__()
+        self.net = nn.Sequential(nn.Linear(in_channels, hid_channels),
+                                 nn.GELU(), nn.Dropout(dropout),
+                                 nn.Linear(hid_channels, in_channels),
+                                 nn.Dropout(dropout))
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return self.net(x)
+
+
+class Attention(nn.Module):
+    def __init__(self,
+                 hid_channels: int,
+                 heads: int = 8,
+                 head_channels: int = 64,
+                 dropout: float = 0.):
+        super(Attention, self).__init__()
+        inner_channels = head_channels * heads
+        project_out = not (heads == 1 and head_channels == hid_channels)
+
+        self.heads = heads
+        self.scale = head_channels**-0.5
+
+        self.attend = nn.Softmax(dim=-1)
+        self.dropout = nn.Dropout(dropout)
+
+        self.to_qkv = nn.Linear(hid_channels, inner_channels * 3, bias=False)
+
+        self.to_out = nn.Sequential(
+            nn.Linear(inner_channels, hid_channels),
+            nn.Dropout(dropout)) if project_out else nn.Identity()
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        qkv = self.to_qkv(x).chunk(3, dim=-1)
+        q, k, v = map(
+            lambda t: rearrange(t, 'b n (h d) -> b h n d', h=self.heads), qkv)
+
+        dots = torch.matmul(q, k.transpose(-1, -2)) * self.scale
+
+        attn = self.attend(dots)
+        attn = self.dropout(attn)
+
+        out = torch.matmul(attn, v)
+        out = rearrange(out, 'b h n d -> b n (h d)')
+        return self.to_out(out)
+
+
+class Transformer(nn.Module):
+    def __init__(self,
+                 hid_channels: int,
+                 depth: int,
+                 heads: int,
+                 head_channels: int,
+                 mlp_channels: int,
+                 dropout: float = 0.):
+        super(Transformer, self).__init__()
+        self.layers = nn.ModuleList([])
+        for _ in range(depth):
+            self.layers.append(
+                nn.ModuleList([
+                    PreNorm(
+                        hid_channels,
+                        Attention(hid_channels,
+                                  heads=heads,
+                                  head_channels=head_channels,
+                                  dropout=dropout)),
+                    PreNorm(
+                        hid_channels,
+                        FeedForward(hid_channels, mlp_channels,
+                                    dropout=dropout))
+                ]))
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        for attn, ff in self.layers:
+            x = attn(x) + x
+            x = ff(x) + x
+        return x
+
+
+class ViT(nn.Module):
     r'''
-    DLocal-Global-Graph Networks (LGGNet). For more details, please refer to the following information.
+    The Vision Transformer. For more details, please refer to the following information. It is worth noting that this model is not designed for EEG analysis, but shows good performance and can serve as a good research start.
 
-    - Paper: Ding Y, Robinson N, Zeng Q, et al. LGGNet: learning from Local-global-graph representations for brain-computer interface[J]. arXiv preprint arXiv:2105.02786, 2021.
-    - URL: https://arxiv.org/abs/2105.02786
-    - Related Project: https://github.com/yi-ding-cs/LGG
+    - Paper: Dosovitskiy A, Beyer L, Kolesnikov A, et al. An image is worth 16x16 words: Transformers for image recognition at scale[J]. arXiv preprint arXiv:2010.11929, 2020.
+    - URL: https://arxiv.org/abs/2010.11929
+    - Related Project: https://github.com/lucidrains/vit-pytorch
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = SEEDDataset(io_path=f'./seed',
-                              root_path='./Preprocessed_EEG',
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import ViT
+        from torch.utils.data import DataLoader
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
                               offline_transform=transforms.Compose([
-                                  transforms.MeanStdNormalize(),
-                                  transforms.To2d()
+                                  transforms.MinMaxNormalize(axis=-1),
+                                  transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
                               ]),
                               online_transform=transforms.Compose([
-                                  transforms.ToTensor()
+                                  transforms.ToTensor(),
                               ]),
                               label_transform=transforms.Compose([
-                                  transforms.Select('emotion'),
-                                  transforms.Lambda(lambda x: x + 1)
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
                               ]))
-        model = LGGNet(region_list=SEED_GENERAL_REGION_LIST, chunk_size=128, num_electrodes=32, hid_channels=32, num_classes=2)
 
-    The current built-in :obj:`region_list` includs:
+        model = ViT(chunk_size=128,
+                    grid_size=(9, 9),
+                    t_patch_size=32,
+                    num_classes=2)
 
-    - torcheeg.datasets.constants.emotion_recognition.amigos.AMIGOS_GENERAL_REGION_LIST
-    - torcheeg.datasets.constants.emotion_recognition.amigos.AMIGOS_FRONTAL_REGION_LIST
-    - torcheeg.datasets.constants.emotion_recognition.amigos.AMIGOS_HEMISPHERE_REGION_LIST
-    - torcheeg.datasets.constants.emotion_recognition.deap.DEAP_GENERAL_REGION_LIST
-    - ...
-    - torcheeg.datasets.constants.emotion_recognition.dreamer.DREAMER_GENERAL_REGION_LIST
-    - ...
-    - torcheeg.datasets.constants.emotion_recognition.mahnob.MAHNOB_GENERAL_REGION_LIST
-    - ...
-    - torcheeg.datasets.constants.emotion_recognition.seed.SEED_GENERAL_REGION_LIST
-    - ...
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
+    It can also be used for the analysis of features such as DE, PSD, etc:
+
+    .. code-block:: python
+
+        dataset = DEAPDataset(io_path=f'./deap',
+                    root_path='./data_preprocessed_python',
+                    offline_transform=transforms.Compose([
+                        transforms.BandDifferentialEntropy(sampling_rate=128),
+                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+                    ]),
+                    online_transform=transforms.Compose([
+                        transforms.ToTensor(),
+                    ]),
+                    label_transform=transforms.Compose([
+                        transforms.Select('valence'),
+                        transforms.Binary(5.0),
+                    ]))
+        model = ViT(chunk_size=4,
+                    grid_size=(9, 9),
+                    t_patch_size=1,
+                    num_classes=2)
 
     Args:
-        region_list (list): The local graph structure defined according to the 10-20 system, where the electrodes are divided into different brain regions.
-        in_channels (int): The feature dimension of each electrode. (default: :obj:`1`)
-        num_electrodes (int): The number of electrodes. (default: :obj:`32`)
-        chunk_size (int): Number of data points included in each EEG chunk. (default: :obj:`128`)
-        sampling_rate (int): The sampling rate of the EEG signals, i.e., :math:`f_s` in the paper. (default: :obj:`128`)
-        num_T (int): The number of multi-scale 1D temporal kernels in the dynamic temporal layer, i.e., :math:`T` kernels in the paper. (default: :obj:`64`)
-        hid_channels (int): The number of hidden nodes in the first fully connected layer. (default: :obj:`32`)
-        dropout (float): Probability of an element to be zeroed in the dropout layers. (default: :obj:`0.5`)
-        pool_kernel_size (int): The kernel size of pooling layers in the temporal blocks (default: :obj:`16`)
-        pool_stride (int): The stride of pooling layers in the temporal blocks (default: :obj:`4`)
-        num_classes (int): The number of classes to predict. (default: :obj:`2`)
+        chunk_size (int): Number of data points included in each EEG chunk as training or test samples. (default: :obj:`128`)
+        grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
+        t_patch_size (int): The size of each input patch at the temporal (chunk size) dimension. (default: :obj:`32`)
+        s_patch_size (tuple): The size (resolution) of each input patch at the spatial (grid size) dimension. (default: :obj:`(3, 3)`)
+        hid_channels (int): The feature dimension of embeded patch. (default: :obj:`32`)
+        depth (int): The number of attention layers for each transformer block. (default: :obj:`3`)
+        heads (int): The number of attention heads for each attention layer. (default: :obj:`4`)
+        head_channels (int): The dimension of each attention head for each attention layer. (default: :obj:`8`)
+        mlp_channels (int): The number of hidden nodes in the fully connected layer of each transformer block. (default: :obj:`64`)
+        num_classes (int): The number of classes to predict. (default: :obj:`0.0`)
+        embed_dropout (float): Probability of an element to be zeroed in the dropout layers of the embedding layers. (default: :obj:`0.0`)
+        dropout (float): Probability of an element to be zeroed in the dropout layers of the transformer layers. (default: :obj:`0.0`)
+        pool_func (str): The pool function before the classifier, optionally including :obj:`cls` and :obj:`mean`, where :obj:`cls` represents selecting classification-related token and :obj:`mean` represents the average pooling. (default: :obj:`cls`)
     '''
     def __init__(self,
-                 region_list,
-                 in_channels: int = 1,
-                 num_electrodes: int = 32,
                  chunk_size: int = 128,
-                 sampling_rate: int = 128,
-                 num_T: int = 64,
+                 grid_size: Tuple[int, int] = (9, 9),
+                 t_patch_size: int = 32,
+                 s_patch_size: Tuple[int, int] = (3, 3),
                  hid_channels: int = 32,
-                 dropout: float = 0.5,
-                 pool_kernel_size: int = 16,
-                 pool_stride: int = 4,
-                 num_classes: int = 2):
-        super(LGGNet, self).__init__()
-        self.region_list = region_list
-        self.inception_window = [0.5, 0.25, 0.125]
-
-        self.num_classes = num_classes
-        self.in_channels = in_channels
-        self.num_electrodes = num_electrodes
+                 depth: int = 3,
+                 heads: int = 4,
+                 head_channels: int = 64,
+                 mlp_channels: int = 64,
+                 num_classes: int = 2,
+                 embed_dropout: float = 0.,
+                 dropout: float = 0.,
+                 pool_func: str = 'cls'):
+        super(ViT, self).__init__()
         self.chunk_size = chunk_size
-        self.sampling_rate = sampling_rate
-        self.num_T = num_T
-        self.hid_channels = hid_channels
+        self.grid_size = grid_size
+        self.t_patch_size = t_patch_size
+        self.s_patch_size = s_patch_size
         self.dropout = dropout
-        self.pool_kernel_size = pool_kernel_size
-        self.pool_stride = pool_stride
-        self.in_channels = in_channels
-        self.num_electrodes = num_electrodes
-
-        self.t_block1 = self.temporal_block(
-            self.in_channels, self.num_T,
-            (1, int(self.inception_window[0] * self.sampling_rate)),
-            self.pool_kernel_size, self.pool_stride)
-        self.t_block2 = self.temporal_block(
-            self.in_channels, self.num_T,
-            (1, int(self.inception_window[1] * self.sampling_rate)),
-            self.pool_kernel_size, self.pool_stride)
-        self.t_block3 = self.temporal_block(
-            self.in_channels, self.num_T,
-            (1, int(self.inception_window[2] * self.sampling_rate)),
-            self.pool_kernel_size, self.pool_stride)
-
-        self.bn_t1 = nn.BatchNorm2d(self.num_T)
-        self.bn_t2 = nn.BatchNorm2d(self.num_T)
-
-        self.cbam = CBAMBlock(num_electrodes)
-
-        self.conv1x1 = nn.Sequential(
-            nn.Conv2d(num_T, num_T, kernel_size=(1, 1), stride=(1, 1)),
-            nn.LeakyReLU(), nn.AvgPool2d((1, 2)))
-
-        self.avg_pool = nn.AvgPool2d((1, 2))
-
-        feature_dim = self.feature_dim
-        self.local_filter_weight = nn.Parameter(torch.FloatTensor(
-            self.num_electrodes, feature_dim),
-                                                requires_grad=True)
-        self.local_filter_bias = nn.Parameter(torch.zeros(
-            (1, self.num_electrodes, 1), dtype=torch.float32),
-                                              requires_grad=True)
-
-        self.aggregate = Aggregator(self.region_list)
-        num_region = len(self.region_list)
-
-        self.global_adj = nn.Parameter(torch.FloatTensor(
-            num_region, num_region),
-                                       requires_grad=True)
-
-        self.bn_g1 = nn.BatchNorm1d(num_region)
-        self.bn_g2 = nn.BatchNorm1d(num_region)
-
-        self.gcn = GraphConvolution(feature_dim, hid_channels)
-
-        self.fc = nn.Sequential(
-            nn.Dropout(p=dropout),
-            nn.Linear(int(num_region * hid_channels), num_classes))
-
-        nn.init.xavier_uniform_(self.local_filter_weight)
-        nn.init.xavier_uniform_(self.global_adj)
-
-    def temporal_block(self, in_channels, out_channels, kernel_size,
-                       pool_kernel_size, pool_stride):
-        return nn.Sequential(
-            nn.Conv2d(in_channels,
-                      out_channels,
-                      kernel_size=kernel_size,
-                      stride=(1, 1)),
-            PowerLayer(kernel_size=pool_kernel_size, stride=pool_stride))
+        self.hid_channels = hid_channels
+        self.depth = depth
+        self.heads = heads
+        self.head_channels = head_channels
+        self.mlp_channels = mlp_channels
+        self.pool_func = pool_func
+        self.embed_dropout = embed_dropout
+        self.num_classes = num_classes
+
+        grid_height, grid_width = pair(grid_size)
+        patch_height, patch_width = pair(s_patch_size)
+
+        assert grid_height % patch_height == 0 and grid_width % patch_width == 0, f'EEG grid size {grid_size} must be divisible by the spatial patch size {s_patch_size}.'
+        assert chunk_size % t_patch_size == 0, f'EEG chunk size {chunk_size} must be divisible by the temporal patch size {t_patch_size}.'
+
+        num_patches = (chunk_size // t_patch_size) * (
+            grid_height // patch_height) * (grid_width // patch_width)
+        patch_channels = t_patch_size * patch_height * patch_width
+        assert pool_func in {
+            'cls', 'mean'
+        }, 'pool_func must be either cls (cls token) or mean (mean pooling).'
+
+        self.to_patch_embedding = nn.Sequential(
+            Rearrange('b (c p0) (h p1) (w p2) -> b c h w (p1 p2 p0)',
+                      p0=t_patch_size,
+                      p1=patch_height,
+                      p2=patch_width),
+            nn.Linear(patch_channels, hid_channels),
+        )
+
+        self.pos_embedding = nn.Parameter(
+            torch.randn(1, num_patches + 1, hid_channels))
+        self.cls_token = nn.Parameter(torch.randn(1, 1, hid_channels))
+        self.dropout = nn.Dropout(embed_dropout)
+
+        self.transformer = Transformer(hid_channels, depth, heads,
+                                       head_channels, mlp_channels, dropout)
+
+        self.pool_func = pool_func
 
-    def forward(self, x):
+        self.mlp_head = nn.Sequential(nn.LayerNorm(hid_channels),
+                                      nn.Linear(hid_channels, num_classes))
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         r'''
         Args:
-            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 1, 32, 128]`. Here, :obj:`n` corresponds to the batch size, :obj:`32` corresponds to :obj:`num_electrodes`, and :obj:`chunk_size` corresponds to :obj:`chunk_size`.
+            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 128, 9, 9]`. Here, :obj:`n` corresponds to the batch size, :obj:`128` corresponds to :obj:`chunk_size`, and :obj:`(9, 9)` corresponds to :obj:`grid_size`.
 
         Returns:
             torch.Tensor[number of sample, number of classes]: the predicted probability that the samples belong to the classes.
         '''
-        t1 = self.t_block1(x)
-        t2 = self.t_block2(x)
-        t3 = self.t_block3(x)
-        x = torch.cat((t1, t2, t3), dim=-1)
-
-        x = self.bn_t1(x)
-
-        x = x.permute(0, 2, 1, 3)
-        x = self.cbam(x)
-        x = self.avg_pool(x)
-
-        x = x.flatten(start_dim=2)
-        x = self.local_filter(x)
-        x = self.aggregate.forward(x)
-        adj = self.get_adj(x)
-        x = self.bn_g1(x)
-        
-        x = self.gcn(x, adj)
-        x = self.bn_g2(x)
-        x = x.view(x.shape[0], -1)
-        x = self.fc(x)
-        return x
+        x = self.to_patch_embedding(x)
+        x = rearrange(x, 'b ... d -> b (...) d')
+        b, n, _ = x.shape
 
-    @property
-    def feature_dim(self):
-        mock_eeg = torch.randn(
-            (1, self.in_channels, self.num_electrodes, self.chunk_size))
-
-        t1 = self.t_block1(mock_eeg)
-        t2 = self.t_block2(mock_eeg)
-        t3 = self.t_block3(mock_eeg)
-        mock_eeg = torch.cat((t1, t2, t3), dim=-1)
-
-        mock_eeg = self.bn_t1(mock_eeg)
-        mock_eeg = self.conv1x1(mock_eeg)
-        mock_eeg = self.bn_t2(mock_eeg)
-        mock_eeg = mock_eeg.permute(0, 2, 1, 3)
-        mock_eeg = mock_eeg.flatten(start_dim=2)
-        return mock_eeg.shape[-1]
-
-    def local_filter(self, x):
-        w = self.local_filter_weight.unsqueeze(0).repeat(x.shape[0], 1, 1)
-        x = F.relu(torch.mul(x, w) - self.local_filter_bias)
-        return x
+        cls_tokens = repeat(self.cls_token, '1 1 d -> b 1 d', b=b)
+        x = torch.cat((cls_tokens, x), dim=1)
+        x += self.pos_embedding[:, :(n + 1)]
+        x = self.dropout(x)
+
+        x = self.transformer(x)
+
+        x = x.mean(dim=1) if self.pool_func == 'mean' else x[:, 0]
 
-    def get_adj(self, x, self_loop=True):
-        adj = torch.bmm(x, x.permute(0, 2, 1))
-        num_nodes = adj.shape[-1]
-        adj = F.relu(adj * (self.global_adj + self.global_adj.transpose(1, 0)))
-        if self_loop:
-            adj = adj + torch.eye(num_nodes).to(x.device)
-        rowsum = torch.sum(adj, dim=-1)
-        mask = torch.zeros_like(rowsum)
-        mask[rowsum == 0] = 1
-        rowsum += mask
-        d_inv_sqrt = torch.pow(rowsum, -0.5)
-        d_mat_inv_sqrt = torch.diag_embed(d_inv_sqrt)
-        adj = torch.bmm(torch.bmm(d_mat_inv_sqrt, adj), d_mat_inv_sqrt)
-        return adj
+        return self.mlp_head(x)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/pyg/gin.py` & `torcheeg-1.1.2/torcheeg/models/pyg/gin.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,34 @@
     - URL: https://www.worldscientific.com/worldscibooks/10.1142/q0282#t=aboutBook
     - Related Project: https://github.com/xiangzhang1015/Deep-Learning-for-BCI/blob/master/pythonscripts/4-3_GIN.py
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.BandDifferentialEntropy(),
-                    online_transform=ToG(SEED_STANDARD_ADJACENCY_MATRIX),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.transforms.pyg import ToG
+        from torcheeg.datasets.constants import SEED_STANDARD_ADJACENCY_MATRIX
+        from torcheeg.models import GIN
+        from torch_geometric.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              offline_transform=transforms.BandDifferentialEntropy(),
+                              online_transform=ToG(SEED_STANDARD_ADJACENCY_MATRIX),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = GIN(in_channels=4, hid_channels=64, num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         in_channels (int): The feature dimension of each electrode. (default: :obj:`4`)
         hid_channels (int): The number of hidden nodes in the GRU layers and the fully connected layer. (default: :obj:`64`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
     '''
     def __init__(self,
                  in_channels: int = 4,
```

### Comparing `torcheeg-1.1.1/torcheeg/models/pyg/rgnn.py` & `torcheeg-1.1.2/torcheeg/models/pyg/rgnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,32 +97,42 @@
     - URL: https://ieeexplore.ieee.org/abstract/document/9091308
     - Related Project: https://github.com/zhongpeixiang/RGNN
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = SEEDDataset(io_path=f'./seed',
-                              root_path='./Preprocessed_EEG',
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg.models import RGNN
+        from torcheeg.transforms.pyg import ToG
+        from torcheeg.datasets.constants import SEED_STANDARD_ADJACENCY_MATRIX
+        from torch_geometric.data import DataLoader
+
+
+        dataset = SEEDDataset(root_path='./Preprocessed_EEG',
                               offline_transform=transforms.BandDifferentialEntropy(),
                               online_transform=ToG(SEED_STANDARD_ADJACENCY_MATRIX),
                               label_transform=transforms.Compose([
                                   transforms.Select('emotion'),
                                   transforms.Lambda(lambda x: int(x) + 1),
                               ]),
                               num_worker=8)
+
         model = RGNN(adj=torch.Tensor(SEED_STANDARD_ADJACENCY_MATRIX),
                      in_channels=5,
                      num_electrodes=62,
                      hid_channels=32,
                      num_layers=2,
                      num_classes=3,
                      dropout=0.7,
                      learn_edge_weights=True)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         adj (torch.Tensor): The adjacency matrix corresponding to the EEG representation, where 1.0 means the node is adjacent and 0.0 means the node is not adjacent. The matrix shape should be [num_electrodes, num_electrodes].
         num_electrodes (int): The number of electrodes. (default: :obj:`62`)
         in_channels (int): The feature dimension of each electrode. (default: :obj:`5`)
         num_layers (int): The number of graph convolutional layers. (default: :obj:`2`)
         hid_channels (int): The number of hidden nodes in the first fully connected layer. (default: :obj:`32`)
         num_classes (int): The number of classes to predict. (default: :obj:`3`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/rnn/gru.py` & `torcheeg-1.1.2/torcheeg/models/rnn/gru.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,31 @@
     - URL: https://www.worldscientific.com/worldscibooks/10.1142/q0282#t=aboutBook
     - Related Project: https://github.com/xiangzhang1015/Deep-Learning-for-BCI/blob/master/pythonscripts/4-1-2_GRU.py
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    online_transform=transforms.ToTensor(),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import GRU
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              online_transform=transforms.ToTensor(),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = GRU(num_electrodes=32, hid_channels=64, num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         num_electrodes (int): The number of electrodes, i.e., :math:`C` in the paper. (default: :obj:`32`)
         hid_channels (int): The number of hidden nodes in the GRU layers and the fully connected layer. (default: :obj:`64`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
     '''
     def __init__(self,
                  num_electrodes: int = 32,
```

### Comparing `torcheeg-1.1.1/torcheeg/models/rnn/lstm.py` & `torcheeg-1.1.2/torcheeg/models/rnn/lstm.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,30 @@
     - URL: https://www.worldscientific.com/worldscibooks/10.1142/q0282#t=aboutBook
     - Related Project: https://github.com/xiangzhang1015/Deep-Learning-for-BCI/blob/master/pythonscripts/4-1-1_LSTM.py
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    online_transform=transforms.ToTensor(),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
-        model = GRU(num_electrodes=32, hid_channels=64, num_classes=2)
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import LSTM
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              online_transform=transforms.ToTensor(),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
+        model = LSTM(num_electrodes=32, hid_channels=64, num_classes=2)
+
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
 
     Args:
         num_electrodes (int): The number of electrodes, i.e., :math:`C` in the paper. (default: :obj:`32`)
         hid_channels (int): The number of hidden nodes in the GRU layers and the fully connected layer. (default: :obj:`64`)
         num_classes (int): The number of classes to predict. (default: :obj:`2`)
     '''
     def __init__(self,
```

### Comparing `torcheeg-1.1.1/torcheeg/models/transformer/arjun_vit.py` & `torcheeg-1.1.2/torcheeg/models/transformer/arjun_vit.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,32 +113,40 @@
     - Paper: Arjun A, Rajpoot A S, Panicker M R. Introducing attention mechanism for eeg signals: Emotion recognition with vision transformers[C]//2021 43rd Annual International Conference of the IEEE Engineering in Medicine & Biology Society (EMBC). IEEE, 2021: 5723-5726.
     - URL: https://ieeexplore.ieee.org/abstract/document/9629837
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.MeanStdNormalize(),
-                        transforms.To2d()
-                    ]),
-                    online_transform=transforms.Compose([
-                        transforms.ToTensor(),
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import ArjunViT
+        from torch.utils.data import DataLoader
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              offline_transform=transforms.Compose([
+                                  transforms.MeanStdNormalize(),
+                                  transforms.To2d()
+                              ]),
+                              online_transform=transforms.Compose([
+                                  transforms.ToTensor(),
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = ArjunViT(chunk_size=128,
                          t_patch_size=50,
                          num_electrodes=32,
                          num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
        num_electrodes (int): The number of electrodes. (default: :obj:`32`)
         chunk_size (int): Number of data points included in each EEG chunk. (default: :obj:`128`)
         t_patch_size (int): The size of each input patch at the temporal (chunk size) dimension. (default: :obj:`32`)
         patch_size (tuple): The size (resolution) of each input patch. (default: :obj:`(3, 3)`)
         hid_channels (int): The feature dimension of embeded patch. (default: :obj:`32`)
         depth (int): The number of attention layers for each transformer block. (default: :obj:`3`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/transformer/atcnet.py` & `torcheeg-1.1.2/torcheeg/models/transformer/atcnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,25 @@
     r'''
     ATCNet: An attention-based temporal convolutional network forEEG-based motor imagery classiﬁcation.For more details ,please refer to the following information:
 
     - Paper: H. Altaheri, G. Muhammad and M. Alsulaiman, "Physics-Informed Attention Temporal Convolutional Network for EEG-Based Motor Imagery Classification," in IEEE Transactions on Industrial Informatics, vol. 19, no. 2, pp. 2249-2258, Feb. 2023, doi: 10.1109/TII.2022.3197419.
     - URL: https://github.com/Altaheri/EEG-ATCNet
 
     .. code-block:: python
-    
+        
+        import torch
+        
+        from torcheeg.models import ATCNet
+
         model = ATCNet(in_channels=1,
                        num_classes=4,
                        num_windows=3,
                        num_electrodes=22,
                        chunk_size=128)
+
         input = torch.rand(2, 1, 22, 128) # (batch_size, in_channels, num_electrodes,chunk_size) 
         output = model(input)
 
     Args:
         in_channels (int): The number of channels of the signal corresponding to each electrode. If the original signal is used as input, in_channels is set to 1; if the original signal is split into multiple sub-bands, in_channels is set to the number of bands. (default: :obj:`1`)
         num_electrodes (int): The number of electrodes. (default: :obj:`32`)
         num_classes (int): The number of classes to predict. (default: :obj:`4`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/transformer/conformer.py` & `torcheeg-1.1.2/torcheeg/models/transformer/conformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,35 +166,43 @@
     - URL: https://ieeexplore.ieee.org/document/9991178
     - Related Project: https://github.com/eeyhsong/EEG-Conformer
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
-        dataset = SEEDDataset(io_path=f'./seed',
-                              root_path='./Preprocessed_EEG',
+        from torcheeg.models import Conformer
+        from torcheeg.datasets import SEEDDataset
+        from torcheeg import transforms
+        from torch.utils.data import DataLoader
+
+        dataset = SEEDDataset(root_path='./Preprocessed_EEG',
                               offline_transform=transforms.Compose([
                                   transforms.MinMaxNormalize(axis=-1),
                                   transforms.To2d()
                               ]),
                               online_transform=transforms.ToTensor(),
                               label_transform=transforms.Compose([
                                   transforms.Select('emotion'),
                                   transforms.Lambda(lambda x: x + 1)
                               ]))
+
         model = Conformer(num_electrodes=62,
                           sampling_rate=200,
                           hid_channels=40,
                           depth=6,
                           heads=10,
                           dropout=0.5,
                           forward_expansion=4,
                           forward_dropout=0.5,
                           num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         num_electrodes (int): The number of electrodes. (default: :obj:`62`)
         sampling_rate (int): The sampling rate of EEG signals. (default: :obj:`200`)
         hid_channels (int): The feature dimension of embeded patch. (default: :obj:`40`)
         depth (int): The number of attention layers for each transformer block. (default: :obj:`6`)
         heads (int): The number of attention heads for each attention layer. (default: :obj:`10`)
         dropout (float): The dropout rate of the attention layer. (default: :obj:`0.5`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/transformer/simple_vit.py` & `torcheeg-1.1.2/torcheeg/models/transformer/simple_vit.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,60 +139,79 @@
     - URL: https://arxiv.org/abs/2205.01580
     - Related Project: https://github.com/lucidrains/vit-pytorch
 
     Below is a recommended suite for use in emotion recognition tasks:
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import SimpleViT
+        from torch.utils.data import DataLoader
+
         dataset = DEAPDataset(io_path=f'./deap',
                     root_path='./data_preprocessed_python',
                     offline_transform=transforms.Compose([
                         transforms.MinMaxNormalize(axis=-1),
                         transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
                     ]),
                     online_transform=transforms.Compose([
                         transforms.ToTensor(),
                     ]),
                     label_transform=transforms.Compose([
                         transforms.Select('valence'),
                         transforms.Binary(5.0),
                     ]))
+
         model = SimpleViT(chunk_size=128,
                           grid_size=(9, 9),
                           t_patch_size=32,
                           num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     It can also be used for the analysis of features such as DE, PSD, etc:
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.BandDifferentialEntropy({
-                            "delta": [1, 4],
-                            "theta": [4, 8],
-                            "alpha": [8, 14],
-                            "beta": [14, 31],
-                            "gamma": [31, 49]
-                        }),
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    online_transform=transforms.Compose([
-                        transforms.ToTensor(),
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.models import SimpleViT
+        from torch.utils.data import DataLoader
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+
+
+        dataset = DEAPDataset(root_path='./data_preprocessed_python',
+                              offline_transform=transforms.Compose([
+                                  transforms.BandDifferentialEntropy({
+                                      "delta": [1, 4],
+                                      "theta": [4, 8],
+                                      "alpha": [8, 14],
+                                      "beta": [14, 31],
+                                      "gamma": [31, 49]
+                                  }),
+                                  transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+                              ]),
+                              online_transform=transforms.Compose([
+                                  transforms.ToTensor(),
+                              ]),
+                              label_transform=transforms.Compose([
+                                  transforms.Select('valence'),
+                                  transforms.Binary(5.0),
+                              ]))
+
         model = SimpleViT(chunk_size=5,
                           grid_size=(9, 9),
                           t_patch_size=1,
                           num_classes=2)
 
+        x, y = next(iter(DataLoader(dataset, batch_size=64)))
+        model(x)
+
     Args:
         chunk_size (int): Number of data points included in each EEG chunk as training or test samples. (default: :obj:`128`)
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
         patch_size (tuple): The size (resolution) of each input patch. (default: :obj:`(3, 3)`)
         t_patch_size (int): The size of each input patch at the temporal (chunk size) dimension. (default: :obj:`32`)
         s_patch_size (tuple): The size (resolution) of each input patch at the spatial (grid size) dimension. (default: :obj:`(3, 3)`)
         hid_channels (int): The feature dimension of embeded patch. (default: :obj:`32`)
```

### Comparing `torcheeg-1.1.1/torcheeg/models/transformer/vit.py` & `torcheeg-1.1.2/torcheeg/models/vae/bcvae.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,258 +1,205 @@
 from typing import Tuple
 
 import torch
-from einops import rearrange, repeat
-from einops.layers.torch import Rearrange
-from torch import nn
+import torch.nn as nn
 
 
-def pair(t):
-    return t if isinstance(t, tuple) else (t, t)
-
-
-class PreNorm(nn.Module):
-    def __init__(self, in_channels: int, fn: nn.Module):
-        super(PreNorm, self).__init__()
-        self.norm = nn.LayerNorm(in_channels)
-        self.fn = fn
-
-    def forward(self, x, **kwargs):
-        return self.fn(self.norm(x), **kwargs)
+class BCEncoder(nn.Module):
+    r'''
+    TorchEEG provides an EEG feature encoder based on CNN architecture and CVAE for generating EEG grid representations of different frequency bands based on a given class label. In particular, the expected labels are additionally provided to guide the encoder to derive the mean and standard deviation vectors of the given expected labels and input data.
 
+    - Related Project: https://github.com/timbmg/VAE-CVAE-MNIST/blob/master/models.py
 
-class FeedForward(nn.Module):
-    def __init__(self,
-                 in_channels: int,
-                 hid_channels: int,
-                 dropout: float = 0.):
-        super(FeedForward, self).__init__()
-        self.net = nn.Sequential(nn.Linear(in_channels, hid_channels),
-                                 nn.GELU(), nn.Dropout(dropout),
-                                 nn.Linear(hid_channels, in_channels),
-                                 nn.Dropout(dropout))
+    .. code-block:: python
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.net(x)
+        import torch
 
+        from torcheeg.models import BCEncoder
+        
+        encoder = BCEncoder(in_channels=4, num_classes=3)
+        y = torch.randint(low=0, high=3, size=(1,))
+        mock_eeg = torch.randn(1, 4, 9, 9)
+        mu, logvar = encoder(mock_eeg, y)
 
-class Attention(nn.Module):
+    Args:
+        in_channels (int): The feature dimension of each electrode. (default: :obj:`4`)
+        grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
+        hid_channels (int): The number of hidden nodes in the first convolutional layer, which is also used as the dimension of output mu and logvar. (default: :obj:`32`)
+        num_classes (int): The number of classes. (default: :obj:`2`)
+    '''
     def __init__(self,
-                 hid_channels: int,
-                 heads: int = 8,
-                 head_channels: int = 64,
-                 dropout: float = 0.):
-        super(Attention, self).__init__()
-        inner_channels = head_channels * heads
-        project_out = not (heads == 1 and head_channels == hid_channels)
-
-        self.heads = heads
-        self.scale = head_channels**-0.5
-
-        self.attend = nn.Softmax(dim=-1)
-        self.dropout = nn.Dropout(dropout)
-
-        self.to_qkv = nn.Linear(hid_channels, inner_channels * 3, bias=False)
-
-        self.to_out = nn.Sequential(
-            nn.Linear(inner_channels, hid_channels),
-            nn.Dropout(dropout)) if project_out else nn.Identity()
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        qkv = self.to_qkv(x).chunk(3, dim=-1)
-        q, k, v = map(
-            lambda t: rearrange(t, 'b n (h d) -> b h n d', h=self.heads), qkv)
+                 in_channels: int = 4,
+                 grid_size: Tuple[int, int] = (9, 9),
+                 hid_channels: int = 64,
+                 num_classes: int = 3):
+        super(BCEncoder, self).__init__()
 
-        dots = torch.matmul(q, k.transpose(-1, -2)) * self.scale
+        self.in_channels = in_channels
+        self.grid_size = grid_size
+        self.hid_channels = hid_channels
+        self.num_classes = num_classes
 
-        attn = self.attend(dots)
-        attn = self.dropout(attn)
+        self.label_embeding = nn.Embedding(
+            num_classes, in_channels * grid_size[0] * grid_size[1])
+        self.conv1 = nn.Sequential(
+            nn.Conv2d(in_channels * 2,
+                      hid_channels,
+                      kernel_size=3,
+                      stride=1,
+                      padding=1,
+                      bias=True), nn.BatchNorm2d(hid_channels), nn.LeakyReLU())
+        self.conv2 = nn.Sequential(
+            nn.Conv2d(hid_channels,
+                      hid_channels * 2,
+                      kernel_size=3,
+                      stride=2,
+                      padding=1,
+                      bias=True), nn.BatchNorm2d(hid_channels * 2),
+            nn.LeakyReLU())
+        self.conv3 = nn.Sequential(
+            nn.Conv2d(hid_channels * 2,
+                      hid_channels * 2,
+                      kernel_size=3,
+                      stride=1,
+                      padding=1,
+                      bias=True), nn.BatchNorm2d(hid_channels * 2),
+            nn.LeakyReLU())
+        self.conv4 = nn.Sequential(
+            nn.Conv2d(hid_channels * 2,
+                      hid_channels * 4,
+                      kernel_size=3,
+                      stride=2,
+                      padding=1,
+                      bias=True), nn.BatchNorm2d(hid_channels * 4),
+            nn.LeakyReLU())
+
+        feature_dim = self.feature_dim()
+        self.fc_mu = nn.Linear(feature_dim, self.hid_channels)
+        self.fc_var = nn.Linear(feature_dim, self.hid_channels)
+
+    def feature_dim(self):
+        with torch.no_grad():
+            mock_y = torch.randint(low=0, high=self.num_classes, size=(1, ))
+            mock_eeg = torch.zeros(1, self.in_channels, *self.grid_size)
+
+            label_emb = self.label_embeding(mock_y)
+            label_emb = label_emb.reshape(mock_eeg.shape)
+            mock_eeg = torch.cat([mock_eeg, label_emb], dim=1)
+
+            mock_eeg = self.conv1(mock_eeg)
+            mock_eeg = self.conv2(mock_eeg)
+            mock_eeg = self.conv3(mock_eeg)
+            mock_eeg = self.conv4(mock_eeg)
 
-        out = torch.matmul(attn, v)
-        out = rearrange(out, 'b h n d -> b n (h d)')
-        return self.to_out(out)
+        return mock_eeg.flatten(start_dim=1).shape[-1]
 
+    def forward(self, x: torch.Tensor, y: torch.Tensor):
+        r'''
+        Args:
+            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 4, 9, 9]`. Here, :obj:`n` corresponds to the batch size, :obj:`4` corresponds to :obj:`in_channels`, and :obj:`(9, 9)` corresponds to :obj:`grid_size`.
+            y (torch.Tensor): Category labels (int) for a batch of samples The shape should be :obj:`[n,]`. Here, :obj:`n` corresponds to the batch size.
 
-class Transformer(nn.Module):
-    def __init__(self,
-                 hid_channels: int,
-                 depth: int,
-                 heads: int,
-                 head_channels: int,
-                 mlp_channels: int,
-                 dropout: float = 0.):
-        super(Transformer, self).__init__()
-        self.layers = nn.ModuleList([])
-        for _ in range(depth):
-            self.layers.append(
-                nn.ModuleList([
-                    PreNorm(
-                        hid_channels,
-                        Attention(hid_channels,
-                                  heads=heads,
-                                  head_channels=head_channels,
-                                  dropout=dropout)),
-                    PreNorm(
-                        hid_channels,
-                        FeedForward(hid_channels, mlp_channels,
-                                    dropout=dropout))
-                ]))
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        for attn, ff in self.layers:
-            x = attn(x) + x
-            x = ff(x) + x
-        return x
+        Returns:
+            tuple[2,]: The mean and standard deviation vectors obtained by encoder. The shapes of the feature vectors are all :obj:`[n, 64]`. Here, :obj:`n` corresponds to the batch size, and :obj:`64` corresponds to :obj:`hid_channels`.
+        '''
+        label_emb = self.label_embeding(y)
+        label_emb = label_emb.reshape(x.shape)
+        x = torch.cat([x, label_emb], dim=1)
+        x = self.conv1(x)
+        x = self.conv2(x)
+        x = self.conv3(x)
+        x = self.conv4(x)
+        x = x.flatten(start_dim=1)
+        mu = self.fc_mu(x)
+        var = self.fc_var(x)
+        return mu, var
 
 
-class ViT(nn.Module):
+class BCDecoder(nn.Module):
     r'''
-    The Vision Transformer. For more details, please refer to the following information. It is worth noting that this model is not designed for EEG analysis, but shows good performance and can serve as a good research start.
-
-    - Paper: Dosovitskiy A, Beyer L, Kolesnikov A, et al. An image is worth 16x16 words: Transformers for image recognition at scale[J]. arXiv preprint arXiv:2010.11929, 2020.
-    - URL: https://arxiv.org/abs/2010.11929
-    - Related Project: https://github.com/lucidrains/vit-pytorch
+    TorchEEG provides an EEG feature decoder based on CNN architecture and CVAE for generating EEG grid representations of different frequency bands based on a given class label. In particular, the expected labels are additionally provided to guide the decoder to reconstruct samples of the specified class.
 
-    Below is a recommended suite for use in emotion recognition tasks:
+    - Related Project: https://github.com/timbmg/VAE-CVAE-MNIST/blob/master/models.py
 
     .. code-block:: python
 
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.MinMaxNormalize(axis=-1),
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    online_transform=transforms.Compose([
-                        transforms.ToTensor(),
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
-        model = ViT(chunk_size=128,
-                    grid_size=(9, 9),
-                    t_patch_size=32,
-                    num_classes=2)
-
-    It can also be used for the analysis of features such as DE, PSD, etc:
-
-    .. code-block:: python
-
-        dataset = DEAPDataset(io_path=f'./deap',
-                    root_path='./data_preprocessed_python',
-                    offline_transform=transforms.Compose([
-                        transforms.BandDifferentialEntropy(sampling_rate=128),
-                        transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-                    ]),
-                    online_transform=transforms.Compose([
-                        transforms.ToTensor(),
-                    ]),
-                    label_transform=transforms.Compose([
-                        transforms.Select('valence'),
-                        transforms.Binary(5.0),
-                    ]))
-        model = ViT(chunk_size=4,
-                    grid_size=(9, 9),
-                    t_patch_size=1,
-                    num_classes=2)
+        encoder = BCEncoder(in_channels=4, num_classes=3)
+        decoder = BCDecoder(in_channels=64, out_channels=4, num_classes=3)
+        y = torch.randint(low=0, high=3, size=(1,))
+        mock_eeg = torch.randn(1, 4, 9, 9)
+        mu, logvar = encoder(mock_eeg, y)
+        std = torch.exp(0.5 * logvar)
+        eps = torch.randn_like(std)
+        z = eps * std + mu
+        fake_X = decoder(z, y)
 
     Args:
-        chunk_size (int): Number of data points included in each EEG chunk as training or test samples. (default: :obj:`128`)
+        in_channels (int): The input feature dimension (of noise vectors). (default: :obj:`64`)
+        out_channels (int): The generated feature dimension of each electrode. (default: :obj:`4`)
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
-        t_patch_size (int): The size of each input patch at the temporal (chunk size) dimension. (default: :obj:`32`)
-        s_patch_size (tuple): The size (resolution) of each input patch at the spatial (grid size) dimension. (default: :obj:`(3, 3)`)
-        hid_channels (int): The feature dimension of embeded patch. (default: :obj:`32`)
-        depth (int): The number of attention layers for each transformer block. (default: :obj:`3`)
-        heads (int): The number of attention heads for each attention layer. (default: :obj:`4`)
-        head_channels (int): The dimension of each attention head for each attention layer. (default: :obj:`8`)
-        mlp_channels (int): The number of hidden nodes in the fully connected layer of each transformer block. (default: :obj:`64`)
-        num_classes (int): The number of classes to predict. (default: :obj:`0.0`)
-        embed_dropout (float): Probability of an element to be zeroed in the dropout layers of the embedding layers. (default: :obj:`0.0`)
-        dropout (float): Probability of an element to be zeroed in the dropout layers of the transformer layers. (default: :obj:`0.0`)
-        pool_func (str): The pool function before the classifier, optionally including :obj:`cls` and :obj:`mean`, where :obj:`cls` represents selecting classification-related token and :obj:`mean` represents the average pooling. (default: :obj:`cls`)
     '''
     def __init__(self,
-                 chunk_size: int = 128,
+                 in_channels: int = 64,
+                 out_channels: int = 4,
                  grid_size: Tuple[int, int] = (9, 9),
-                 t_patch_size: int = 32,
-                 s_patch_size: Tuple[int, int] = (3, 3),
-                 hid_channels: int = 32,
-                 depth: int = 3,
-                 heads: int = 4,
-                 head_channels: int = 64,
-                 mlp_channels: int = 64,
-                 num_classes: int = 2,
-                 embed_dropout: float = 0.,
-                 dropout: float = 0.,
-                 pool_func: str = 'cls'):
-        super(ViT, self).__init__()
-        self.chunk_size = chunk_size
+                 num_classes: int = 3):
+        super(BCDecoder, self).__init__()
+
+        self.in_channels = in_channels
+        self.out_channels = out_channels
         self.grid_size = grid_size
-        self.t_patch_size = t_patch_size
-        self.s_patch_size = s_patch_size
-        self.dropout = dropout
-        self.hid_channels = hid_channels
-        self.depth = depth
-        self.heads = heads
-        self.head_channels = head_channels
-        self.mlp_channels = mlp_channels
-        self.pool_func = pool_func
-        self.embed_dropout = embed_dropout
         self.num_classes = num_classes
 
-        grid_height, grid_width = pair(grid_size)
-        patch_height, patch_width = pair(s_patch_size)
-
-        assert grid_height % patch_height == 0 and grid_width % patch_width == 0, f'EEG grid size {grid_size} must be divisible by the spatial patch size {s_patch_size}.'
-        assert chunk_size % t_patch_size == 0, f'EEG chunk size {chunk_size} must be divisible by the temporal patch size {t_patch_size}.'
-
-        num_patches = (chunk_size // t_patch_size) * (
-            grid_height // patch_height) * (grid_width // patch_width)
-        patch_channels = t_patch_size * patch_height * patch_width
-        assert pool_func in {
-            'cls', 'mean'
-        }, 'pool_func must be either cls (cls token) or mean (mean pooling).'
-
-        self.to_patch_embedding = nn.Sequential(
-            Rearrange('b (c p0) (h p1) (w p2) -> b c h w (p1 p2 p0)',
-                      p0=t_patch_size,
-                      p1=patch_height,
-                      p2=patch_width),
-            nn.Linear(patch_channels, hid_channels),
-        )
-
-        self.pos_embedding = nn.Parameter(
-            torch.randn(1, num_patches + 1, hid_channels))
-        self.cls_token = nn.Parameter(torch.randn(1, 1, hid_channels))
-        self.dropout = nn.Dropout(embed_dropout)
-
-        self.transformer = Transformer(hid_channels, depth, heads,
-                                       head_channels, mlp_channels, dropout)
-
-        self.pool_func = pool_func
-
-        self.mlp_head = nn.Sequential(nn.LayerNorm(hid_channels),
-                                      nn.Linear(hid_channels, num_classes))
+        self.label_embeding = nn.Embedding(num_classes, in_channels)
+        self.deproj = nn.Sequential(
+            nn.Linear(in_channels * 2, in_channels * 4 * 3 * 3), nn.LeakyReLU())
+
+        self.deconv1 = nn.Sequential(
+            nn.ConvTranspose2d(in_channels * 4,
+                               in_channels * 2,
+                               kernel_size=3,
+                               stride=2,
+                               padding=1,
+                               bias=True), nn.BatchNorm2d(in_channels * 2),
+            nn.LeakyReLU())
+        self.deconv2 = nn.Sequential(
+            nn.ConvTranspose2d(in_channels * 2,
+                               in_channels * 2,
+                               kernel_size=3,
+                               stride=1,
+                               padding=1,
+                               bias=True), nn.BatchNorm2d(in_channels * 2),
+            nn.LeakyReLU())
+        self.deconv3 = nn.Sequential(
+            nn.ConvTranspose2d(in_channels * 2,
+                               in_channels,
+                               kernel_size=3,
+                               stride=2,
+                               padding=1,
+                               bias=True), nn.BatchNorm2d(in_channels),
+            nn.LeakyReLU())
+        self.deconv4 = nn.ConvTranspose2d(in_channels,
+                                          out_channels,
+                                          kernel_size=3,
+                                          stride=1,
+                                          padding=1,
+                                          bias=True)
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
+    def forward(self, x: torch.Tensor, y: torch.Tensor):
         r'''
         Args:
-            x (torch.Tensor): EEG signal representation, the ideal input shape is :obj:`[n, 128, 9, 9]`. Here, :obj:`n` corresponds to the batch size, :obj:`128` corresponds to :obj:`chunk_size`, and :obj:`(9, 9)` corresponds to :obj:`grid_size`.
+            x (torch.Tensor): Given the mean and standard deviation vectors, the feature vector :obj:`z` obtained using the reparameterization technique. The shapes of the feature vector should be :obj:`[n, 64]`. Here, :obj:`n` corresponds to the batch size, and :obj:`64` corresponds to :obj:`in_channels`.
+            y (torch.Tensor): Category labels (int) for a batch of samples The shape should be :obj:`[n,]`. Here, :obj:`n` corresponds to the batch size.
 
         Returns:
-            torch.Tensor[number of sample, number of classes]: the predicted probability that the samples belong to the classes.
+            torch.Tensor[n, 4, 9, 9]: the decoded results, which should have the same shape as the input noise, i.e., :obj:`[n, 4, 9, 9]`. Here, :obj:`n` corresponds to the batch size, :obj:`4` corresponds to :obj:`in_channels`, and :obj:`(9, 9)` corresponds to :obj:`grid_size`.
         '''
-        x = self.to_patch_embedding(x)
-        x = rearrange(x, 'b ... d -> b (...) d')
-        b, n, _ = x.shape
-
-        cls_tokens = repeat(self.cls_token, '1 1 d -> b 1 d', b=b)
-        x = torch.cat((cls_tokens, x), dim=1)
-        x += self.pos_embedding[:, :(n + 1)]
-        x = self.dropout(x)
-
-        x = self.transformer(x)
-
-        x = x.mean(dim=1) if self.pool_func == 'mean' else x[:, 0]
-
-        return self.mlp_head(x)
+        label_emb = self.label_embeding(y)
+        x = torch.cat([x, label_emb], dim=-1)
+        x = self.deproj(x)
+        x = x.view(-1, self.in_channels * 4, 3, 3)
+        x = self.deconv1(x)
+        x = self.deconv2(x)
+        x = self.deconv3(x)
+        x = self.deconv4(x)
+        return x
```

### Comparing `torcheeg-1.1.1/torcheeg/models/vae/bvae.py` & `torcheeg-1.1.2/torcheeg/models/vae/bvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 class BEncoder(nn.Module):
     r'''
     The variational autoencoder consists of two parts, an encoder, and a decoder. The encoder compresses the input into the latent space. The decoder receives as input the information sampled from the latent space and produces it as similar as possible to ground truth. The latent vector should approach the gaussian distribution supervised by KL divergence based on the variation trick. This class implement the encoder part.
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.models import BEncoder
+        
         encoder = BEncoder(in_channels=4)
         mock_eeg = torch.randn(1, 4, 9, 9)
         mu, logvar = encoder(mock_eeg)
 
     Args:
         in_channels (int): The feature dimension of each electrode. (default: :obj:`4`)
         grid_size (tuple): Spatial dimensions of grid-like EEG representation. (default: :obj:`(9, 9)`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/classifier.py` & `torcheeg-1.1.2/torcheeg/trainers/classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc',
         'kappa'
     ]
 
     for metric in metric_list:
         if metric not in allowed_metrics:
             raise ValueError(
-                f"{metric} is not allowed. Please choose 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', 'kappa'."
+                f"{metric} is not allowed. Please choose 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', 'kappa'."
             )
     metric_dict = {
         'accuracy':
         torchmetrics.Accuracy(task='multiclass',
                               num_classes=num_classes,
                               top_k=1),
         'precision':
@@ -66,15 +66,15 @@
         Args:
             model (nn.Module): The classification model, and the dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
             num_classes (int, optional): The number of categories in the dataset. If :obj:`None`, the number of categories will be inferred from the attribute :obj:`num_classes` of the model. (defualt: :obj:`None`)
             lr (float): The learning rate. (default: :obj:`0.001`)
             weight_decay (float): The weight decay. (default: :obj:`0.0`)
             devices (int): The number of devices to use. (default: :obj:`1`)
             accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
         
         .. automethod:: fit
         .. automethod:: test
     '''
 
     def __init__(self,
                  model: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/ada.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/ada.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,22 +79,41 @@
 
     - Paper: Haeusser P, Frerix T, Mordvintsev A, et al. Associative domain adaptation[C]//Proceedings of the IEEE international conference on computer vision. 2017: 2765-2773.
     - URL: https://arxiv.org/abs/1708.00938
     - Related Project: https://github.com/stes/torch-assoc
 
     .. code-block:: python
 
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import ADATrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        class Classifier(CCNN):
+            def forward(self, x):
+                x = self.lin1(x)
+                x = self.lin2(x)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
+        classifier = Classifier(in_channels=5, num_classes=3)
+
         trainer = ADATrainer(extractor,
-                            classifier,
-                            num_classes=10,
-                            devices=1,
-                            weight_visit=0.6,
-                            accelerator='gpu')
-        trainer.fit(source_loader, target_loader, val_loader)
-        trainer.test(test_loader)
+                             classifier,
+                             num_classes=3,
+                             devices=1,
+                             weight_visit=0.6,
+                             accelerator='gpu')
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         classifier (nn.Module): The classification model learns the classification task with the source labeled data based on the feature of the feature extraction model. The dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
         num_classes (int, optional): The number of categories in the dataset. (default: :obj:`None`)
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay (float): The weight decay. (default: :obj:`0.0`)
@@ -102,15 +121,15 @@
         weight_visit (float): The weight of the visit loss. (default: :obj:`1.0`)
         weight_domain (float): The weight of the associative loss (default: :obj:`1.0`)
         weight_scheduler (bool): Whether to use a scheduler for the weight of the associative loss, growing from 0 to 1 following the schedule from the DANN paper. (default: :obj:`False`)
         lr_scheduler (bool): Whether to use a scheduler for the learning rate, as defined in the DANN paper. (default: :obj:`False`)
         warmup_epochs (int): The number of epochs for the warmup phase, during which the weight of the associative loss is 0. (default: :obj:`0`)
         devices (int): The number of devices to use. (default: :obj:`1`)
         accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
 
     .. automethod:: fit
     .. automethod:: test
     '''
     def __init__(self,
                  extractor: nn.Module,
                  classifier: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/center.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/center.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,123 +64,94 @@
             label.unsqueeze(1).expand(feature.size()).long(), diff)
         grad_centers = grad_centers / counts.view(-1, 1)
         return -grad_output * diff / batch_size, None, grad_centers / batch_size, None
 
 
 class CenterLossTrainer(ClassifierTrainer):
     r'''
-        A trainer trains classification model contains a decoder and a classifier. As for Center loss, it can make the output of the decoder close to the mean of decoded features within the same class. PLease refer to the following infomation to comprehend how the center loss works.
+        A trainer trains classification model contains a extractor and a classifier. As for Center loss, it can make the output of the extractor close to the mean of decoded features within the same class. PLease refer to the following infomation to comprehend how the center loss works.
 
         - Paper: FBMSNet: A Filter-Bank Multi-Scale Convolutional Neural Network for EEG-Based Motor Imagery Decoding
         - URL: https://ieeexplore.ieee.org/document/9837422
         - Related Project: https://github.com/Want2Vanish/FBMSNet
 
-        .. code-block:: python
-
-            trainer = CenterLossTrainer(decoder = decoder, 
-                                             classifier = classifier,
-                                             num_classes = your_classes,
-                                             feature_dim = your_decoded_dim)
-                                             
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
-
-        The model structure is required to contains a decoder block which generates the deep feature code and a classifier connected to the decoder to judge which class the feature code belong to.
-        Firstly, we should prepare a :obj:`decoder` model and a :obj:`classifier` model for  decoding and classifying from decoding ouput respectly. 
-        Here we take FBMSNet as example. :obj:`torcheeg.models.FBMSNet` contains decoder and classifer method already and what We need to do is just to inherit the model to define a decoder and a classifier,and then override the :obj:`forward` method . 
+        The model structure is required to contains a extractor block which generates the deep feature code and a classifier connected to the extractor to judge which class the feature code belong to.
+        Firstly, we should prepare a :obj:`extractor` model and a :obj:`classifier` model for  decoding and classifying from decoding ouput respectly. 
+        Here we take FBMSNet as example. :obj:`torcheeg.models.FBMSNet` contains extractor and classifer method already and what We need to do is just to inherit the model to define a extractor and a classifier,and then override the :obj:`forward` method . 
 
         .. code-block:: python
 
             from torcheeg.models import FBMSNet
+            from torcheeg.trainers import CenterLossTrainer
 
-            class FBMSDecoder(FBMSNet):
-                def forward(self,x):
-                    return self.decoder(x)
-
-            class FBMSClassifier(FBMSNet):
-                def forward(self,x):
-                    return 
+            class Extractor(FBMSNet):
+                def forward(self, x):
+                    x = self.mixConv2d(x)
+                    x = self.scb(x)
+                    x = x.reshape([
+                        *x.shape[0:2], self.stride_factor,
+                        int(x.shape[3] / self.stride_factor)
+                    ])
+                    x = self.temporal_layer(x)
+                    return torch.flatten(x, start_dim=1)
+
+            class Classifier(FBMSNet):
+                def forward(self, x):
+                    return self.fc(x)
                 
-            decoder  = FBMSDecoder(num_classes=4,
+            extractor  = Extractor(num_classes=4,
                                    num_electrodes=22,
                                    chunk_size=512,
                                    in_channels=9)
 
-            classifier = FBMSClassifier(num_classes=4,
-                                        num_electrodes=22,
-                                        chunk_size=512,
-                                        in_channels=9)
+            classifier = Classifier(num_classes=4,
+                                    num_electrodes=22,
+                                    chunk_size=512,
+                                    in_channels=9)
             
-            trainer = CenterLossTrainer(decoder=decoder, 
+            trainer = CenterLossTrainer(extractor=extractor, 
                                         classifier=classifier,
                                         num_classes=4,
                                         feature_dim=1152)
         
-        Custom model is OK. Feel free to refer to  this example:
-    
-        .. code-block:: python
-
-
-            class MyDecoder(nn.Module):
-                def __init__(self):
-                    self.layer = nn.Linear(128,64)   #(input dim, decoded dim)
-
-                def forward(self,x):
-                    return self.layer(x)
-
-            class MyClassifier(nn.Module):
-                def __init__(self):
-                    self.layer = nn.Linear(64,2)      #(decoded dim, num_classes)
-
-                def forward(self,x):classifier
-                    return self.layer(x)
-                
-            decoder  = MyDecoder()
-            classifier = MyClassifier()
-
-            trainer = CenterLossTrainer(decoder = decoder, 
-                                             classifier = classifier,
-                                             num_classes = 2,
-                                             feature_dim = 64)
-        
         Args:
-            decoder (nn.Module): The decoder which transforms eegsignal into 1D feature code.
-            classifier (nn.Module): The classifier that predict from the decoder output which class the siginals belong to.
-            feature_dim (int): The dimemsion of decoder output code whose mean values we can loosely regard as the "center". 
+            extractor (nn.Module): The extractor which transforms eegsignal into 1D feature code.
+            classifier (nn.Module): The classifier that predict from the extractor output which class the siginals belong to.
+            feature_dim (int): The dimemsion of extractor output code whose mean values we can loosely regard as the "center". 
             num_classes (int, optional): The number of categories in the dataset. 
             lammda (float): The weight of the center loss in total loss. (default: :obj:`5e-4`)
             lr (float): The learning rate. (default: :obj:`0.001`)
             weight_decay (float): The weight decay. (default: :obj:`0.0`)
             devices (int): The number of devices to use. (default: :obj:`1`)
             accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`['accuracy', 'precision', 'recall', 'f1score']`)
+            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`['accuracy', 'precision', 'recall', 'f1score']`)
 
         .. automethod:: fit
         .. automethod:: test
     '''
 
     def __init__(
             self,
-            decoder,
+            extractor,
             classifier,
             feature_dim: int,
             num_classes: int,
             lammda: float = 0.0005,
             lr: float = 1e-3,
             weight_decay: float = 0.0,
             devices: int = 1,
             accelerator: str = "cpu",
             metrics: List[str] = ['accuracy', 'precision', 'recall',
                                   'f1score']):
 
         super(CenterLossTrainer,
-              self).__init__(decoder, num_classes, lr, weight_decay, devices,
+              self).__init__(extractor, num_classes, lr, weight_decay, devices,
                              accelerator, metrics)
 
-        self.decoder = decoder
+        self.extractor = extractor
         self.classifier = classifier
         self.center_loss = CentersLoss(num_classes, feature_dim)
         self.lammda = lammda
         self.automatic_optimization = False
         self.feature_dim = feature_dim
 
     def init_metrics(self, metrics: List[str], num_classes: int) -> None:
@@ -226,15 +197,15 @@
         center_optimizer, model_optimizer = self.optimizers(True)
 
         # zero_grad
         center_optimizer.zero_grad()
         model_optimizer.zero_grad()
 
         # center loss
-        feat = self.decoder(x)
+        feat = self.extractor(x)
         centerloss = self.center_loss(y, feat)
 
         # prediction cross entropy loss
         y_hat = self.classifier(feat)
         pre_loss = self.ce_fn(y_hat, y)
 
         # total loss
@@ -279,15 +250,15 @@
         # reset the metrics
         self.__reset_metric()
 
     def validation_step(self, batch: Tuple[torch.Tensor],
                         batch_idx: int) -> torch.Tensor:
         x, y = batch
         # calculate feat y_pred
-        feat = self.decoder(x)
+        feat = self.extractor(x)
         y_hat = self.classifier(feat)
 
         # get loss (pred_loss,center loss,total_loss)
         pre_loss = self.ce_fn(y_hat, y)
         centerloss = self.center_loss(y, feat)
         loss = pre_loss + self.lammda * centerloss
 
@@ -329,15 +300,15 @@
                 str += f"{key}: {value:.3f} "
         log.info(str + '\n')
 
     def test_step(self, batch: Tuple[torch.Tensor],
                   batch_idx: int) -> torch.Tensor:
         x, y = batch
         # centerloss
-        feat = self.decoder(x)
+        feat = self.extractor(x)
         centerloss = self.center_loss(y, feat)
 
         # predict loss
         y_hat = self.classifier(feat)
         pre_loss = self.ce_fn(y_hat, y)
 
         #Total loss
@@ -367,15 +338,15 @@
                 str += f"{key}: {value:.3f} "
         log.info(str + '\n')
 
         self.test_loss.reset()
         self.test_metrics.reset()
 
     def configure_optimizers(self):
-        parameters = list(self.decoder.parameters())
+        parameters = list(self.extractor.parameters())
         parameters.extend(list(self.classifier.parameters()))
         trainable_parameters = list(
             filter(lambda p: p.requires_grad, parameters))
         model_optimizer = torch.optim.Adam(trainable_parameters,
                                            lr=self.lr,
                                            weight_decay=self.weight_decay)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/coral.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/coral.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,36 +32,55 @@
 
     - Paper: Sun B, Saenko K. Deep CORAL: Correlation alignment for deep domain adaptation[C]//European conference on computer vision. Springer, Cham, 2016: 443-450.
     - URL: https://arxiv.org/abs/1607.01719
     - Related Project: https://github.com/adapt-python/adapt/blob/master/adapt/feature_based/_deepCORAL.py
 
     .. code-block:: python
 
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import CORALTrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        class Classifier(CCNN):
+            def forward(self, x):
+                x = self.lin1(x)
+                x = self.lin2(x)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
+        classifier = Classifier(in_channels=5, num_classes=3)
+
         trainer = CORALTrainer(extractor,
-                             classifier,
-                             num_classes=10,
-                             devices=1,
-                             weight_domain=1.0,
-                             accelerator='gpu')
-        trainer.fit(source_loader, target_loader, val_loader)
-        trainer.test(test_loader)
+                               classifier,
+                               num_classes=3,
+                               devices=1,
+                               weight_domain=1.0,
+                               accelerator='gpu')
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         classifier (nn.Module): The classification model learns the classification task with the source labeled data based on the feature of the feature extraction model. The dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function. 
         num_classes (int, optional): The number of categories in the dataset. (default: :obj:`None`)
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay (float): The weight decay. (default: :obj:`0.0`)
         weight_domain (float): The weight of the CORAL loss. (default: :obj:`1.0`)
         weight_scheduler (bool): Whether to use a scheduler for the weight of the CORAL loss, growing from 0 to 1 following the schedule from the DANN paper. (default: :obj:`False`)
         lr_scheduler (bool): Whether to use a scheduler for the learning rate, as defined in the DANN paper. (default: :obj:`False`)
         warmup_epochs (int): The number of epochs for the warmup phase, during which the weight of the CORAL loss is 0. (default: :obj:`0`)
         devices (int): The number of devices to use. (default: :obj:`1`)
         accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
 
     .. automethod:: fit
     .. automethod:: test
     '''
     def __init__(self,
                  extractor: nn.Module,
                  classifier: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/dan.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/ddc.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,92 +2,73 @@
 
 import torch
 import torch.nn as nn
 
 from .mmd_like import _MMDLikeTrainer
 
 
-def guassian_kernel(x_source,
-                    x_target,
-                    mul_kernel=2.0,
-                    num_kernels=5,
-                    sigma=None):
-    n_samples = int(x_source.shape[0]) + int(x_target.shape[0])
-    total = torch.cat([x_source, x_target], dim=0)
-    total0 = total.unsqueeze(0).expand(int(total.size(0)), int(total.size(0)),
-                                       int(total.size(1)))
-    total1 = total.unsqueeze(1).expand(int(total.size(0)), int(total.size(0)),
-                                       int(total.size(1)))
-    L2_distance = ((total0 - total1)**2).sum(2)
-    if sigma:
-        bandwidth = sigma
-    else:
-        bandwidth = torch.sum(L2_distance.data) / (n_samples**2 - n_samples)
-    bandwidth /= mul_kernel**(num_kernels // 2)
-    bandwidth_list = [bandwidth * (mul_kernel**i) for i in range(num_kernels)]
-    kernel_val = [
-        torch.exp(-L2_distance / bandwidth_temp)
-        for bandwidth_temp in bandwidth_list
-    ]
-    return sum(kernel_val)
-
-
-def maximum_mean_discrepancy(x_source,
-                             x_target,
-                             mul_kernel=2.0,
-                             num_kernels=5,
-                             sigma=None):
-    batch_size = int(x_source.shape[0])
-    kernels = guassian_kernel(x_source,
-                              x_target,
-                              mul_kernel=mul_kernel,
-                              num_kernels=num_kernels,
-                              sigma=sigma)
-    XX = kernels[:batch_size, :batch_size]
-    YY = kernels[batch_size:, batch_size:]
-    XY = kernels[:batch_size, batch_size:]
-    YX = kernels[batch_size:, :batch_size]
-    loss = torch.mean(XX + YY - XY - YX)
+def maximum_mean_discrepancy_linear(x_source, x_target):
+    delta = x_source - x_target
+    loss = torch.mean(torch.mm(delta, torch.transpose(delta, 0, 1)))
     return loss
 
 
-class DANTrainer(_MMDLikeTrainer):
+class DDCTrainer(_MMDLikeTrainer):
     r'''
-    This class supports the implementation of Deep Adaptation Network (DAN) for deep domain adaptation.
+    The individual differences and nonstationary of EEG signals make it difficult for deep learning models trained on the training set of subjects to correctly classify test samples from unseen subjects, since the training set and test set come from different data distributions. Domain adaptation is used to address the problem of distribution drift between training and test sets and thus achieves good performance in subject-independent (cross-subject) scenarios. This class supports the implementation of Deep Domain Confusion (DDC) for deep domain adaptation.
 
-    NOTE: DAN belongs to unsupervised domain adaptation methods, which only use labeled source and unlabeled target data. This means that the target dataset does not have to return labels.
+    NOTE: DDC belongs to unsupervised domain adaptation methods, which only use labeled source and unlabeled target data. This means that the target dataset does not have to return labels.
 
-    - Paper: Long M, Cao Y, Wang J, et al. Learning transferable features with deep adaptation networks[C]//International conference on machine learning. PMLR, 2015: 97-105.
-    - URL: https://proceedings.mlr.press/v37/long15
-    - Related Project: https://github.com/jindongwang/transferlearning/blob/cfaf1174dff7390a861cc4abd5ede37dfa1063f5/code/deep/DAN/DAN.py
+    - Paper: Tzeng E, Hoffman J, Zhang N, et al. Deep domain confusion: Maximizing for domain invariance[J]. arXiv preprint arXiv:1412.3474, 2014.
+    - URL: https://arxiv.org/abs/1412.3474
+    - Related Project: https://github.com/syorami/DDC-transfer-learning/blob/master/DDC.py
 
     .. code-block:: python
 
-        trainer = DANTrainer(extractor,
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import DDCTrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        class Classifier(CCNN):
+            def forward(self, x):
+                x = self.lin1(x)
+                x = self.lin2(x)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
+        classifier = Classifier(in_channels=5, num_classes=3)
+
+        trainer = DDCTrainer(extractor,
                              classifier,
-                             num_classes=10,
+                             num_classes=3,
                              devices=1,
                              weight_domain=1.0,
                              accelerator='gpu')
-        trainer.fit(source_loader, target_loader, val_loader)
-        trainer.test(test_loader)
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         classifier (nn.Module): The classification model learns the classification task with the source labeled data based on the feature of the feature extraction model. The dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function. 
         num_classes (int, optional): The number of categories in the dataset. (default: :obj:`None`)
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay (float): The weight decay. (default: :obj:`0.0`)
-        weight_domain (float): The weight of the DAN loss. (default: :obj:`1.0`)
-        weight_scheduler (bool): Whether to use a scheduler for the weight of the DAN loss, growing from 0 to 1 following the schedule from the DANN paper. (default: :obj:`False`)
-        lr_scheduler (bool): Whether to use a scheduler for the learning rate, as defined in the DANN paper. (default: :obj:`False`)
-        warmup_epochs (int): The number of epochs for the warmup phase, during which the weight of the DAN loss is 0. (default: :obj:`0`)
+        weight_domain (float): The weight of the DDC loss. (default: :obj:`1.0`)
+        weight_scheduler (bool): Whether to use a scheduler for the weight of the DDC loss, growing from 0 to 1 following the schedule from the DDCN paper. (default: :obj:`False`)
+        lr_scheduler (bool): Whether to use a scheduler for the learning rate, as defined in the DDCN paper. (default: :obj:`False`)
+        warmup_epochs (int): The number of epochs for the warmup phase, during which the weight of the DDC loss is 0. (default: :obj:`0`)
         devices (int): The number of devices to use. (default: :obj:`1`)
         accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
 
     .. automethod:: fit
     .. automethod:: test
     '''
     def __init__(self,
                  extractor: nn.Module,
                  classifier: nn.Module,
@@ -98,31 +79,32 @@
                  weight_scheduler: bool = True,
                  lr_scheduler_gamma: float = 0.0,
                  lr_scheduler_decay: float = 0.75,
                  warmup_epochs: int = 0,
                  devices: int = 1,
                  accelerator: str = "cpu",
                  metrics: List[str] = ["accuracy"]):
-        super(DANTrainer, self).__init__(extractor=extractor,
-                                         classifier=classifier,
-                                         num_classes=num_classes,
-                                         lr=lr,
-                                         weight_decay=weight_decay,
-                                         weight_domain=weight_domain,
-                                        weight_scheduler=weight_scheduler,
-                                         lr_scheduler_gamma=lr_scheduler_gamma,
-                                         lr_scheduler_decay=lr_scheduler_decay,
-                                         warmup_epochs=warmup_epochs,
-                                         devices=devices,
-                                         accelerator=accelerator,
-                                         metrics=metrics)
+        super(DDCTrainer,
+              self).__init__(extractor=extractor,
+                             classifier=classifier,
+                             num_classes=num_classes,
+                             lr=lr,
+                             weight_decay=weight_decay,
+                             weight_domain=weight_domain,
+                             weight_scheduler=weight_scheduler,
+                             lr_scheduler_gamma=lr_scheduler_gamma,
+                             lr_scheduler_decay=lr_scheduler_decay,
+                             warmup_epochs=warmup_epochs,
+                             devices=devices,
+                             accelerator=accelerator,
+                             metrics=metrics)
 
     def _domain_loss_fn(self, x_source_feat: torch.Tensor,
                         x_target_feat: torch.Tensor) -> torch.Tensor:
 
         batch_size = min(len(x_source_feat), len(x_target_feat))
         if len(x_source_feat) != len(x_target_feat):
             # use the smaller batch size
             x_source_feat = x_source_feat[:batch_size]
             x_target_feat = x_target_feat[:batch_size]
 
-        return maximum_mean_discrepancy(x_source_feat, x_target_feat)
+        return maximum_mean_discrepancy_linear(x_source_feat, x_target_feat)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/dann.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/dann.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,37 +13,57 @@
 
     - Paper: Ganin Y, Ustinova E, Ajakan H, et al. Domain-adversarial training of neural networks[J]. The journal of machine learning research, 2016, 17(1): 2096-2030.
     - URL: https://arxiv.org/abs/1505.07818
     - Related Project: https://github.com/fungtion/DANN/blob/master/train/main.py
 
     .. code-block:: python
 
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import DANNTrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        class Classifier(CCNN):
+            def forward(self, x):
+                x = self.lin1(x)
+                x = self.lin2(x)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
+        classifier = Classifier(in_channels=5, num_classes=3)
+        domain_classifier = Classifier(in_channels=5, num_classes=2)
+
         trainer = DANNTrainer(extractor,
                               classifier,
                               domain_classifier,
-                              num_classes=10,
+                              num_classes=3,
                               devices=1,
                               accelerator='gpu')
-        trainer.fit(source_loader, target_loader, val_loader)
-        trainer.test(test_loader)
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         classifier (nn.Module): The classification model learns the classification task with the source labeled data based on the feature of the feature extraction model. The dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
         domain_classifier (nn.Module): The classification model, learning to discriminate between the source and target domains based on the feature of the feature extraction model. The dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function or a gradient reverse layer (which is already included in the implementation).
         num_classes (int, optional): The number of categories in the dataset. (default: :obj:`None`)
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay (float): The weight decay. (default: :obj:`0.0`)
         weight_domain (float): The weight of the DANN loss (default: :obj:`1.0`)
         alpha_scheduler (bool): Whether to use a scheduler for the alpha of the DANN loss, growing from 0 to 1 following the schedule from the DANN paper. (default: :obj:`True`)
         lr_scheduler (bool): Whether to use a scheduler for the learning rate, as defined in the DANN paper. (default: :obj:`False`)
         warmup_epochs (int): The number of epochs for the warmup phase, during which the weight of the DANN loss is 0. (default: :obj:`0`)
         devices (int): The number of devices to use. (default: :obj:`1`)
         accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
 
     .. automethod:: fit
     .. automethod:: test
     '''
     def __init__(self,
                  extractor: nn.Module,
                  classifier: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/dann_like.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/dann_like.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/jan.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/jan.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,22 +54,41 @@
 
     - Paper: Long M, Zhu H, Wang J, et al. Deep transfer learning with joint adaptation networks[C]//International conference on machine learning. PMLR, 2017: 2208-2217.
     - URL: http://proceedings.mlr.press/v70/long17a.html
     - Related Project: https://github.com/criteo-research/pytorch-ada
 
     .. code-block:: python
 
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import JANTrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        class Classifier(CCNN):
+            def forward(self, x):
+                x = self.lin1(x)
+                x = self.lin2(x)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
+        classifier = Classifier(in_channels=5, num_classes=3)
+
         trainer = JANTrainer(extractor,
-                            classifier,
-                            num_classes=10,
-                            devices=1,
-                            weight_visit=0.6,
-                            accelerator='gpu')
-        trainer.fit(source_loader, target_loader, val_loader)
-        trainer.test(test_loader)
+                             classifier,
+                             num_classes=3,
+                             devices=1,
+                             weight_visit=0.6,
+                             accelerator='gpu')
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         classifier (nn.Module): The classification model learns the classification task with the source labeled data based on the feature of the feature extraction model. The dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
         num_classes (int, optional): The number of categories in the dataset. (default: :obj:`None`)
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay (float): The weight decay. (default: :obj:`0.0`)
@@ -77,15 +96,15 @@
         num_kernel (tuple of int): The number of kernels for the Gaussian kernel. (default: :obj:`(5, 1)`)
         weight_domain (float): The weight of the associative loss (default: :obj:`1.0`)
         lr_scheduler (bool): Whether to use a scheduler for the weight of the associative loss, growing from 0 to 1 following the schedule from the DANN paper. (default: :obj:`False`)
         lr_scheduler (bool): Whether to use a scheduler for the learning rate, as defined in the DANN paper. (default: :obj:`False`)
         warmup_epochs (int): The number of epochs for the warmup phase, during which the weight of the associative loss is 0. (default: :obj:`0`)
         devices (int): The number of devices to use. (default: :obj:`1`)
         accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+        metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
 
     .. automethod:: fit
     .. automethod:: test
     '''
     def __init__(self,
                  extractor: nn.Module,
                  classifier: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/domain_adaption/mmd_like.py` & `torcheeg-1.1.2/torcheeg/trainers/domain_adaption/mmd_like.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/trainers/finetune.py` & `torcheeg-1.1.2/torcheeg/trainers/finetune.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 def classification_metrics(metric_list: List[str], num_classes: int):
     allowed_metrics = ['precision', 'recall', 'f1score', 'accuracy']
 
     for metric in metric_list:
         if metric not in allowed_metrics:
             raise ValueError(
-                f"{metric} is not allowed. Please choose 'precision', 'recall', 'f1_score', 'accuracy'"
+                f"{metric} is not allowed. Please choose 'precision', 'recall', 'f1score', 'accuracy'"
             )
     metric_dict = {
         'accuracy':
         torchmetrics.Accuracy(task='multiclass',
                               num_classes=num_classes,
                               top_k=1),
         'precision':
@@ -148,15 +148,15 @@
             milestones (list of int): The milestones of the learning rate scheduler. (default: :obj:`[100]`)
             freeze_epochs (int): The number of epochs to freeze the layers. (default: :obj:`10`)
             freeze_layers (list of str): The names of the layers to freeze. (default: :obj:`[]`)
             warmup_epochs (int): The number of epochs to warmup the learning rate. (default: :obj:`10`)
             warmup_lr (float): The learning rate to warmup to. (default: :obj:`1e-5`)
             devices (int): The number of devices to use. (default: :obj:`1`)
             accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
         
         .. automethod:: fit
         .. automethod:: test
     '''
     def __init__(self,
                  model: nn.Module,
                  num_classes: int,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/generative/beta_vae.py` & `torcheeg-1.1.2/torcheeg/trainers/generative/beta_vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
     - Paper: Gulrajani I, Ahmed F, Arjovsky M, et al. Improved training of wasserstein gans[J]. Advances in neural information processing systems, 2017, 30.
     - URL: https://arxiv.org/abs/1704.00028
     - Related Project: https://github.com/eriklindernoren/PyTorch-GAN
 
     .. code-block:: python
         
+        from torcheeg.models import BEncoder, BDecoder
+        from torcheeg.trainers import BetaVAETrainer
+
         encoder = BEncoder(in_channels=4)
         decoder = BDecoder(in_channels=64, out_channels=4)
         trainer = BetaVAETrainer(encoder, decoder)
-        trainer.fit(train_loader, val_loader)
-        trainer.test(test_loader)
 
     Args:
         encoder (nn.Module): The encoder, whose inputs are EEG signals, outputs are two batches of vectors of the same dimension, representing the mean and variance estimated in the reparameterization trick.
         decoder (nn.Module): The decoder generating EEG signals from hidden variables encoded by the encoder.
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay: (float): The weight decay (L2 penalty). (default: :obj:`0.0`)
         beta: (float): The weight of the KL divergence in the loss function. When beta is 1, the model is a standard VAE. (default: :obj:`1.0`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/generative/ddpm.py` & `torcheeg-1.1.2/torcheeg/trainers/generative/ddpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,19 @@
 
     - Paper: Ho J, Chen X, Srinivas A, et al. Denoising diffusion probabilistic models[J]. arXiv preprint arXiv:2006.11239, 2020.
     - URL: https://arxiv.org/abs/2006.11239
     - Related Project: https://github.com/Stability-AI/stablediffusion
 
     .. code-block:: python
         
+        from torcheeg.trainers import DDPMTrainer
+        from torcheeg.models import BUNet
+
+        model = BUNet(in_channels=4)
         trainer = DDPMTrainer(model)
-        trainer.fit(train_loader, val_loader, max_epochs=1)
-        trainer.test(test_loader)
 
     Args:
         model (nn.Module): The denoising model takes the noisy samples and the current denoising conditions as input to predict the denoised samples. In this class, the current denoising condition is the current denoising time step. Typically, this model will be a UNet.
         lr (float): The learning rate. (default: :obj:`1e-4`)
         weight_decay (float): The weight decay. (default: :obj:`0.0`)
         timesteps (int): The number of steps in the diffusion process. (default: :obj:`1000`)
         beta_schedule (str): The schedule of the beta. Available options are: 'linear', 'cosine', 'sqrt_linear', 'sqrt'. (default: :obj:`"linear"`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/generative/glow.py` & `torcheeg-1.1.2/torcheeg/trainers/generative/glow.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     - URL: https://proceedings.neurips.cc/paper/2018/hash/d139db6a236200b21cc7f752979132d0-Abstract.html
     - Related Project: https://github.com/chaiyujin/glow-pytorch
 
     .. code-block:: python
         
         model = BGlow(in_channels=4)
         trainer = GlowTrainer(model)
-        trainer.fit(train_loader, val_loader)
-        trainer.test(test_loader)
 
     Args:
         model (nn.Module): Normalized flow model, it needs to implement two interfaces, log_probs and sample. Among them, log_probs takes the original sample as input to calculate the log probs to the target distribution, and sample takes num and temperature as input to calculate the generated sample.
         lr (float): The learning rate. (default: :obj:`0.0001`)
         weight_decay: (float): The weight decay (L2 penalty). (default: :obj:`0.0`)
         temperature (float): The temperature. (default: :obj:`1.0`)
         max_grad_clip (float): The maximum norm of the gradients will be clipped to this value. If set to 0, no clipping will be performed. (default: :obj:`0.0`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/generative/utils.py` & `torcheeg-1.1.2/torcheeg/trainers/generative/utils.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/trainers/generative/wgan_gp.py` & `torcheeg-1.1.2/torcheeg/trainers/generative/wgan_gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,14 @@
     - Related Project: https://github.com/eriklindernoren/PyTorch-GAN
 
     .. code-block:: python
         
         g_model = BGenerator(in_channels=128)
         d_model = BDiscriminator(in_channels=4)
         trainer = WGANGPTrainer(generator, discriminator)
-        trainer.fit(train_loader, val_loader)
-        trainer.test(test_loader)
 
     Args:
         generator (nn.Module): The generator model for EEG signal generation, whose inputs are Gaussian distributed random vectors, outputs are generated EEG signals. The dimensions of the input vector should be defined on the :obj:`in_channel` attribute. The output layer does not need to have a softmax activation function.
         discriminator (nn.Module): The discriminator model to determine whether the EEG signal is real or generated, and the dimension of its output should be equal to the one (i.e., the score to distinguish the real and the fake). The output layer does not need to have a sigmoid activation function.
         generator_lr (float): The learning rate of the generator. (default: :obj:`0.0001`)
         discriminator_lr (float): The learning rate of the discriminator. (default: :obj:`0.0001`)
         weight_gradient_penalty (float): The weight of gradient penalty loss to trade-off between the adversarial training loss and gradient penalty loss. (default: :obj:`1.0`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/imbalance/eq.py` & `torcheeg-1.1.2/torcheeg/trainers/imbalance/eq.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,33 +50,31 @@
     
         - Paper: Tan J, Wang C, Li B, et al. Equalization loss for long-tailedobject recognition[C]//Proceedings of the IEEE/CVF conference on computervision and pattern recognition. 2020: 11662-11671.
         - URL: https://openaccess.thecvf.com/content_CVPR_2020/papersTan_Equalization_Loss_for_Long-Tailed_Object_Recognition_CVPR_2020_paper.pdf
         - Related Project: https://github.com/tztztztztz/eql.detectron2
 
         .. code-block:: python
 
-            trainer = EQLossTrainer(model, num_classes=2, class_frequency=train_loader)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
+            from torcheeg.models import CCNN
+            from torcheeg.trainers import EQLossTrainer
 
+            model = CCNN(in_channels=5, num_classes=2)
             trainer = EQLossTrainer(model, num_classes=2, class_frequency=[10, 20], gamma=0.9, lambd=0.005)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
 
         Args:
             model (nn.Module): The classification model, and the dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
             num_classes (int): The number of classes in the dataset.
             class_frequency (List[int] or Dataloader): The frequency of each class in the dataset. It can be a list of integers or a dataloader to calculate the frequency of each class in the dataset, traversing the data batch (:obj:`torch.utils.data.dataloader.DataLoader`, :obj:`torch_geometric.loader.DataLoader`, etc). (default: :obj:`None`)
             gamma (float): The gamma parameter. (default: :obj:`0.9`)
             lambd (float): The lambd parameter. (default: :obj:`0.005`)
             lr (float): The learning rate. (default: :obj:`0.001`)
             weight_decay (float): The weight decay. (default: :obj:`0.0`)
             devices (int): The number of devices to use. (default: :obj:`1`)
             accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
         
         .. automethod:: fit
         .. automethod:: test
     '''
 
     def __init__(self,
                  model: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/imbalance/focal.py` & `torcheeg-1.1.2/torcheeg/trainers/imbalance/focal.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,21 +48,19 @@
 
         - Paper: Lin T Y, Goyal P, Girshick R, et al. Focal loss for dense object detection[C]//Proceedings of the IEEE international conference on computer vision. 2017: 2980-2988.
         - URL: https://openaccess.thecvf.com/content_ICCV_2017/papers/Lin_Focal_Loss_for_ICCV_2017_paper.pdf
         - Related Project: https://github.com/clcarwin/focal_loss_pytorch
 
         .. code-block:: python
 
-            trainer = FocalLossTrainer(model, num_classes=2, class_frequency=train_loader)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
+            from torcheeg.models import CCNN
+            from torcheeg.trainers import FocalLossTrainer
 
+            model = CCNN(in_channels=5, num_classes=2)
             trainer = FocalLossTrainer(model, num_classes=2, class_frequency=[10, 20], gamma=1.0)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
 
         Args:
             model (nn.Module): The classification model, and the dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
             num_classes (int): The number of classes in the dataset.
             class_frequency (List[int] or Dataloader): The frequency of each class in the dataset. It can be a list of integers or a dataloader to calculate the frequency of each class in the dataset, traversing the data batch (:obj:`torch.utils.data.dataloader.DataLoader`, :obj:`torch_geometric.loader.DataLoader`, etc). (default: :obj:`None`)
             gamma (float): The gamma parameter. (default: :obj:`1.0`)
             rule (str): The rule to adjust the weight of each class. Available options are: 'none', 'reweight', 'drw' (deferred re-balancing optimization schedule). (default: :obj:`none`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/imbalance/la.py` & `torcheeg-1.1.2/torcheeg/trainers/imbalance/la.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,33 +44,31 @@
 
         - Paper: Menon A K, Jayasumana S, Rawat A S, et al. Long-tail learning via logit adjustment[J]. arXiv preprint arXiv:2007.07314, 2020.
         - URL: https://arxiv.org/abs/2007.07314
         - Related Project: https://github.com/Chumsy0725/logit-adj-pytorch
 
         .. code-block:: python
 
-            trainer = LALossTrainer(model, num_classes=2, class_frequency=train_loader)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
+            from torcheeg.models import CCNN
+            from torcheeg.trainers import LALossTrainer
 
+            model = CCNN(in_channels=5, num_classes=2)
             trainer = LALossTrainer(model, num_classes=2, class_frequency=[10, 20], tau=1.0)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
 
         Args:
             model (nn.Module): The classification model, and the dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
             num_classes (int): The number of classes in the dataset.
             class_frequency (List[int] or Dataloader): The frequency of each class in the dataset. It can be a list of integers or a dataloader to calculate the frequency of each class in the dataset, traversing the data batch (:obj:`torch.utils.data.dataloader.DataLoader`, :obj:`torch_geometric.loader.DataLoader`, etc). (default: :obj:`None`)
             tau (float): The temperature parameter. (default: :obj:`1.0`)
             eps (float): The epsilon parameter. (default: :obj:`1e-12`)
             lr (float): The learning rate. (default: :obj:`0.001`)
             weight_decay (float): The weight decay. (default: :obj:`0.0`)
             devices (int): The number of devices to use. (default: :obj:`1`)
             accelerator (str): The accelerator to use. Available options are: 'cpu', 'gpu'. (default: :obj:`"cpu"`)
-            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1_score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
+            metrics (list of str): The metrics to use. Available options are: 'precision', 'recall', 'f1score', 'accuracy', 'matthews', 'auroc', and 'kappa'. (default: :obj:`["accuracy"]`)
         
         .. automethod:: fit
         .. automethod:: test
     '''
 
     def __init__(self,
                  model: nn.Module,
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/imbalance/ldam.py` & `torcheeg-1.1.2/torcheeg/trainers/imbalance/ldam.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,21 +65,19 @@
 
         - Paper: Cao K, Wei C, Gaidon A, et al. Learning imbalanced datasets with label-distribution-aware margin loss[J]. Advances in neural information processing systems, 2019, 32.
         - URL: https://proceedings.neurips.cc/paper_files/paper/2019/file/621461af90cadfdaf0e8d4cc25129f91-Paper.pdf
         - Related Project: https://github.com/kaidic/LDAM-DRW
 
         .. code-block:: python
 
-            trainer = LDAMLossTrainer(model, num_classes=2, class_frequency=train_loader)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
+            from torcheeg.models import CCNN
+            from torcheeg.trainers import LDAMLossTrainer
 
+            model = CCNN(in_channels=5, num_classes=2)
             trainer = LDAMLossTrainer(model, num_classes=2, class_frequency=[10, 20], max_margin=0.5, scaling=30)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
 
         Args:
             model (nn.Module): The classification model, and the dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
             num_classes (int): The number of classes in the dataset.
             class_frequency (List[int] or Dataloader): The frequency of each class in the dataset. It can be a list of integers or a dataloader to calculate the frequency of each class in the dataset, traversing the data batch (:obj:`torch.utils.data.dataloader.DataLoader`, :obj:`torch_geometric.loader.DataLoader`, etc). (default: :obj:`None`)
             max_margin (float): The maximum margin. (default: :obj:`0.5`)
             rule (str): The rule to adjust the weight of each class. Available options are: 'none', 'reweight', 'drw' (deferred re-balancing optimization schedule). (default: :obj:`'none'`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/imbalance/wce.py` & `torcheeg-1.1.2/torcheeg/trainers/imbalance/wce.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,19 @@
         
 class WCELossTrainer(ClassifierTrainer):
     r'''
         A trainer class for EEG classification with Weighted Cross Entropy (WCE) loss for imbalanced datasets.
 
         .. code-block:: python
 
-            trainer = WCELossTrainer(model, num_classes=2, class_frequency=train_loader)
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
+            from torcheeg.models import CCNN
+            from torcheeg.trainers import WCELossTrainer
 
+            model = CCNN(in_channels=5, num_classes=2)
             trainer = WCELossTrainer(model, num_classes=2, class_frequency=[10, 20])
-            trainer.fit(train_loader, val_loader)
-            trainer.test(test_loader)
 
         Args:
             model (nn.Module): The classification model, and the dimension of its output should be equal to the number of categories in the dataset. The output layer does not need to have a softmax activation function.
             num_classes (int): The number of classes in the dataset.
             class_frequency (List[int] or Dataloader): The frequency of each class in the dataset. It can be a list of integers or a dataloader to calculate the frequency of each class in the dataset, traversing the data batch (:obj:`torch.utils.data.dataloader.DataLoader`, :obj:`torch_geometric.loader.DataLoader`, etc). (default: :obj:`None`)
             gamma (float): The gamma parameter. (default: :obj:`1.0`)
             rule (str): The rule to adjust the weight of each class. Available options are: 'reweight', 'drw' (deferred re-balancing optimization schedule). (default: :obj:`reweight`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/self_supervised/byol.py` & `torcheeg-1.1.2/torcheeg/trainers/self_supervised/byol.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,41 @@
 
     - Paper: Grill J B, Strub F, Altché F, et al. Bootstrap your own latent-a new approach to self-supervised learning[J]. Advances in neural information processing systems, 2020, 33: 21271-21284.
     - URL: https://proceedings.neurips.cc/paper/2020/hash/f3ada80d5c4ee70142b17b1048576b2958e-Abstract.html
     - Related Project: https://github.com/lucidrains/byol-pytorch
 
     .. code-block:: python
 
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import BYOLTrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
+
         trainer = BYOLTrainer(extractor,
                               extract_channels=256,
                               devices=1,
                               accelerator='gpu')
-        trainer.fit(train_loader, val_loader)
 
     NOTE: The first element of each batch in :obj:`train_loader` and :obj:`val_loader` should be a two-tuple, representing two random transformations (views) of data. You can use :obj:`Contrastive` to achieve this functionality.
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        
         contras_dataset = DEAPDataset(
             io_path=f'./io/deap',
             root_path='./data_preprocessed_python',
             offline_transform=transforms.Compose([
                 transforms.BandDifferentialEntropy(sampling_rate=128,
                                                 apply_to_baseline=True),
                 transforms.BaselineRemoval(),
@@ -49,18 +66,14 @@
                     transforms.RandomNoise(p=0.5)]),
                                     num_views=2)
             ]),
             chunk_size=128,
             baseline_chunk_size=128,
             num_baseline=3)
 
-        trainer = BYOLTrainer(extractor,
-                              extract_channels=256,
-                              devices=1,
-                              accelerator='gpu')
         trainer.fit(train_loader, val_loader)
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         extract_channels (int): The feature dimensions of the output of the feature extraction model.
         proj_channels (int): The feature dimensions of the output of the projection head. (default: :obj:`256`)
         proj_hid_channels (int): The feature dimensions of the hidden layer of the projection head. (default: :obj:`512`)
```

### Comparing `torcheeg-1.1.1/torcheeg/trainers/self_supervised/sim_clr.py` & `torcheeg-1.1.2/torcheeg/trainers/self_supervised/sim_clr.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,39 @@
 
     - Paper: Chen T, Kornblith S, Norouzi M, et al. A simple framework for contrastive learning of visual representations[C]//International conference on machine learning. PMLR, 2020: 1597-1607.
     - URL: http://proceedings.mlr.press/v119/chen20j.html
     - Related Project: https://github.com/sthalles/SimCLR
 
     .. code-block:: python
 
+        from torcheeg.models import CCNN
+        from torcheeg.trainers import BYOLTrainer
+
+        class Extractor(CCNN):
+            def forward(self, x):
+                x = self.conv1(x)
+                x = self.conv2(x)
+                x = self.conv3(x)
+                x = self.conv4(x)
+                x = x.flatten(start_dim=1)
+                return x
+
+        extractor = Extractor(in_channels=5, num_classes=3)
         trainer = SimCLRTrainer(extractor,
                                 devices=1,
                                 accelerator='gpu')
-        trainer.fit(train_loader, val_loader)
 
     NOTE: The first element of each batch in :obj:`train_loader` and :obj:`val_loader` should be a two-tuple, representing two random transformations (views) of data. You can use :obj:`Contrastive` to achieve this functionality.
 
     .. code-block:: python
 
+        from torcheeg.datasets import DEAPDataset
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        
         contras_dataset = DEAPDataset(
             io_path=f'./io/deap',
             root_path='./data_preprocessed_python',
             offline_transform=transforms.Compose([
                 transforms.BandDifferentialEntropy(sampling_rate=128,
                                                 apply_to_baseline=True),
                 transforms.BaselineRemoval(),
@@ -47,17 +63,14 @@
                     transforms.RandomNoise(p=0.5)]),
                                     num_views=2)
             ]),
             chunk_size=128,
             baseline_chunk_size=128,
             num_baseline=3)
 
-        trainer = SimCLRTrainer(extractor,
-                                devices=1,
-                                accelerator='gpu')
         trainer.fit(train_loader, val_loader)
 
     Args:
         extractor (nn.Module): The feature extraction model learns the feature representation of the EEG signal by forcing the correlation matrixes of source and target data to be close.
         extract_channels (int): The feature dimensions of the output of the feature extraction model.
         proj_channels (int): The feature dimensions of the output of the projection head. (default: :obj:`256`)
         proj_hid_channels (int): The feature dimensions of the hidden layer of the projection head. (default: :obj:`512`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/any/baseline.py` & `torcheeg-1.1.2/torcheeg/transforms/any/baseline.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,24 @@
     r'''
     A transform method to subtract the baseline signal (the signal recorded before the emotional stimulus), the nosie signal is removed from the emotional signal unrelated to the emotional stimulus.
     
     TorchEEG recommends using this class in online_transform for higher processing speed. Even though, this class is also supported in offline_transform. Usually, the baseline needs the same transformation as the experimental signal, please add :obj:`apply_to_baseline=True` to all transforms before this operation to ensure that the transformation is performed on the baseline signal
 
     .. code-block:: python
 
-        transform = Compose([
-            BandDifferentialEntropy(apply_to_baseline=True),
-            ToTensor(apply_to_baseline=True),
-            BaselineRemoval(),
-            ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+        from torcheeg import transforms
+
+        t = transforms.Compose([
+            transforms.BandDifferentialEntropy(apply_to_baseline=True),
+            transforms.ToTensor(apply_to_baseline=True),
+            transforms.BaselineRemoval(),
+            transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
         ])
 
-        transform(eeg=np.random.randn(32, 128), baseline=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128), baseline=np.random.randn(32, 128))['eeg'].shape
         >>> (4, 9, 9)
     
     .. automethod:: __call__
     '''
     def __init__(self):
         super(BaselineRemoval, self).__init__(apply_to_baseline=False)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/any/lambd.py` & `torcheeg-1.1.2/torcheeg/transforms/any/lambd.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 class Lambda(BaseTransform):
     r'''
     Apply a user-defined lambda as a transform.
 
     .. code-block:: python
 
-        transform = Lambda(targets=['y'], lambda x: x + 1)
-        transform(y=1)['y']
+        from torcheeg import transforms
+
+        t = transforms.Lambda(targets=['y'], lambda x: x + 1)
+        t(y=1)['y']
         >>> 2
 
     Args:
         targets (list): What data to transform via the Lambda. (default: :obj:`['eeg', 'baseline', 'y']`)
         lambd (Callable): Lambda/function to be used for transform.
 
     .. automethod:: __call__
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/any/pdb.py` & `torcheeg-1.1.2/torcheeg/transforms/any/pdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 
 class PDB(BaseTransform):
     r'''
     For debugging, insert breakpoints in transforms. The transformation itself does not change the input data.
 
     .. code-block:: python
 
-        transform = Compose([
-            ToTensor(),
-            Resize(size=(64, 64)),
-            PDB(),
-            RandomNoise(p=0.1),
-            RandomMask(p=0.1)
+        from torcheeg import transforms
+
+        t = transforms.Compose([
+            transforms.ToTensor(),
+            transforms.Resize(size=(64, 64)),
+            transforms.PDB(),
+            transforms.RandomNoise(p=0.1),
+            transforms.RandomMask(p=0.1)
         ])
-        transform(eeg=torch.randn(128, 9, 9))['eeg'].shape
+        t(eeg=torch.randn(128, 9, 9))['eeg'].shape
         >>> (128, 64, 64)
     
     Args:
         targets (list): What data to transform via the PDB. (default: :obj:`['eeg', 'baseline', 'y']`)
 
     .. automethod:: __call__
     '''
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/base_transform.py` & `torcheeg-1.1.2/torcheeg/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/transforms/label/binary.py` & `torcheeg-1.1.2/torcheeg/transforms/label/binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 
 class Binary(LabelTransform):
     r'''
     Binarize the label according to a certain threshold. Labels larger than the threshold are set to 1, and labels smaller than the threshold are set to 0.
     
     .. code-block:: python
 
-        transform = Binary(threshold=5.0)
-        transform(y=4.5)['y']
+        from torcheeg import transforms
+
+        t = transforms.Binary(threshold=5.0)
+        t(y=4.5)['y']
         >>> 0
 
     :obj:`Binary` allows simultaneous binarization using the same threshold for multiple labels.
 
     .. code-block:: python
 
-        transform = Binary(threshold=5.0)
-        transform(y=[4.5, 5.5])['y']
+        from torcheeg import transforms
+
+        t = transforms.Binary(threshold=5.0)
+        t(y=[4.5, 5.5])['y']
         >>> [0, 1]
 
     Args:
         threshold (float): Threshold used during binarization.
 
     .. automethod:: __call__
     '''
@@ -55,24 +59,28 @@
 
 class BinaryOneVSRest(LabelTransform):
     r'''
     Binarize the label following the fashion of the one-vs-rest strategy. When label is the specified positive category label, the label is set to 1, when the label is any other category label, the label is set to 0.
     
     .. code-block:: python
 
-        transform = BinaryOneVSRest(positive=1)
-        transform(y=2)['y']
+        from torcheeg import transforms
+
+        t = BinaryOneVSRest(positive=1)
+        t(y=2)['y']
         >>> 0
 
     :obj:`Binary` allows simultaneous binarization using the same threshold for multiple labels.
 
     .. code-block:: python
 
-        transform = BinaryOneVSRest(positive=1)
-        transform(y=[1, 2])['y']
+        from torcheeg import transforms
+
+        t = transforms.BinaryOneVSRest(positive=1)
+        t(y=[1, 2])['y']
         >>> [1, 0]
 
     Args:
         positive (int): The specified positive category label.
 
     .. automethod:: __call__
     '''
@@ -95,22 +103,24 @@
 
 class BinariesToCategory(LabelTransform):
     r'''
     Convert multiple binary labels into one multiclass label. Multiclass labels represent permutations of binary labels. Commonly used to combine two binary classification tasks into a single quad classification task.
     
     .. code-block:: python
 
-        transform = BinariesToCategory()
-        transform(y=[0, 0])['y']
+        from torcheeg import transforms
+
+        t = transforms.BinariesToCategory()
+        t(y=[0, 0])['y']
         >>> 0
-        transform(y=[0, 1])['y']
+        t(y=[0, 1])['y']
         >>> 1
-        transform(y=[1, 0])['y']
+        t(y=[1, 0])['y']
         >>> 2
-        transform(y=[1, 1])['y']
+        t(y=[1, 1])['y']
         >>> 3
     
     .. automethod:: __call__
     '''
     def __call__(self, *args, y: List, **kwargs) -> int:
         r'''
         Args:
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/label/fix.py` & `torcheeg-1.1.2/torcheeg/transforms/label/fix.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 
 class FixCategory(LabelTransform):
     r'''
     Returns a pre-set label for all samples, usually used to supplement the dataset with new categories.
 
     .. code-block:: python
 
-        transform = FixCategory(value=0)
-        transform(y=3)['y']
+        from torcheeg import transforms
+
+        t = transforms.FixCategory(value=0)
+        t(y=3)['y']
         >>> 0
 
     :obj:`FixCategory` allows multiple values to be selected and returned as a list. Suitable for multi-classification tasks or multi-task learning.
 
     .. code-block:: python
 
-        transform = FixCategory(value=[0, 1])
-        transform(y=[1, 2])['y']
+        from torcheeg import transforms
+
+        t = transforms.FixCategory(value=[0, 1])
+        t(y=[1, 2])['y']
         >>> [0, 1]
 
     Args:
         value (str or list): The pre-set label.
 
     .. automethod:: __call__
     '''
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/label/mapping.py` & `torcheeg-1.1.2/torcheeg/transforms/label/mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 
 class Mapping(LabelTransform):
     r'''
     Mapping the label according to a certain dictionary.
     
     .. code-block:: python
 
-        transform = Mapping({
+        from torcheeg import transforms
+
+        t = Mapping({
             'left_hand': 0,
             'right_hand': 1,
         })
-        transform(y='left_hand')['y']
+        t(y='left_hand')['y']
         >>> 0
 
     :obj:`Mapping` allows simultaneous binarization using the same threshold for multiple labels.
 
     .. code-block:: python
 
-        transform = Mapping({
+        from torcheeg import transforms
+        
+        t = Mapping({
             'left_hand': 0,
             'right_hand': 1,
             'left_feet': 0,
             'right_feet': 1
         })
-        transform(y=['left_hand', 'left_feet'])['y']
+        t(y=['left_hand', 'left_feet'])['y']
         >>> [0, 0]
 
     Args:
         map_dict (float): The mapping dictionary.
         default (float, optional): The default value when the input label is not in the dictionary. (default: :obj:`-1`)
 
     .. automethod:: __call__
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/label/select.py` & `torcheeg-1.1.2/torcheeg/transforms/label/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 
 class Select(LabelTransform):
     r'''
     Select part of the value from the information dictionary.
 
     .. code-block:: python
 
-        transform = Select(key='valence')
-        transform(y={'valence': 4.5, 'arousal': 5.5, 'subject_id': 7})['y']
+        from torcheeg import transforms
+
+        t = transforms.Select(key='valence')
+        t(y={'valence': 4.5, 'arousal': 5.5, 'subject_id': 7})['y']
         >>> 4.5
 
     :obj:`Select` allows multiple values to be selected and returned as a list. Suitable for multi-classification tasks or multi-task learning.
 
     .. code-block:: python
+        
+        from torcheeg import transforms
 
-        transform = Select(key=['valence', 'arousal'])
-        transform(y={'valence': 4.5, 'arousal': 5.5, 'subject_id': 7})['y']
+        t = transforms.Select(key=['valence', 'arousal'])
+        t(y={'valence': 4.5, 'arousal': 5.5, 'subject_id': 7})['y']
         >>> [4.5, 5.5]
 
     Args:
         key (str or list): The selected key can be a key string or a list of keys.
 
     .. automethod:: __call__
     '''
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/label/string.py` & `torcheeg-1.1.2/torcheeg/transforms/label/string.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 
 class StringToInt(LabelTransform):
     r'''
     Identify numbers in strings and convert strings to numbers. If there is no number in the string, the output corresponding to the string is 0.
     
     .. code-block:: python
 
-        transform = StringToInt()
-        transform(y='None')['y']
+        from torcheeg import transforms
+
+        t = transforms.StringToInt()
+        t(y='None')['y']
         >>> 0
 
-        transform = StringToInt()
-        transform(y='sub001')['y']
+        t = transforms.StringToInt()
+        t(y='sub001')['y']
         >>> 1
 
     :obj:`StringToInt` allows converting a list of strings to a list of numbers with the same conversion behavior as a single string.
 
     .. code-block:: python
 
-        transform = StringToInt()
-        transform(y=['sub001', '4'])['y']
+        t = transforms.StringToInt()
+        t(y=['sub001', '4'])['y']
         >>> 1, 4
 
     .. automethod:: __call__
     '''
     def __init__(self):
         super(StringToInt, self).__init__()
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/band.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/band.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,18 @@
 
 class BandSignal(BandTransform):
     r'''
     A transform method to split the EEG signal into signals in different sub-bands.
 
     .. code-block:: python
 
-        transform = BandSignal()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandSignal()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (4, 32, 128)
 
     Args:
         sampling_rate (int): The original sampling rate of EEG signals in Hz. (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -117,16 +119,18 @@
     - Related Paper: Li D, Xie L, Chai B, et al. Spatial-frequency convolutional self-attention network for EEG emotion recognition[J]. Applied Soft Computing, 2022, 122: 108740.
     - Related Project: https://github.com/qeebeast7/SFCSAN/
 
     In most cases, choosing :obj:`BandDifferentialEntropy` and :obj:`BandDifferentialEntropyV1` does not make much difference. If you have other comments, please feel free to pull request.
     
     .. code-block:: python
 
-        transform = BandDifferentialEntropy()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandDifferentialEntropy()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The original sampling rate of EEG signals in Hz. (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -156,16 +160,18 @@
     A transform method for calculating the differential entropy of EEG signals in several sub-bands with EEG signals as input. This version calculates the differential entropy based on the relationship between the differential entropy and the average power spectral density, which is identical to the processing of the SEED dataset.
 
     - Related Paper: Shi L C, Jiao Y Y, Lu B L. Differential entropy feature for EEG-based vigilance estimation[C]//2013 35th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC). IEEE, 2013: 6627-6630.
     - Related Project: https://github.com/ziyujia/Signal-feature-extraction_DE-and-PSD
 
     .. code-block:: python
 
-        transform = BandDifferentialEntropyV1()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandDifferentialEntropyV1()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The original sampling rate of EEG signals in Hz. (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -249,16 +255,18 @@
 
 class BandPowerSpectralDensity(EEGTransform):
     r'''
     A transform method for calculating the power spectral density of EEG signals in several sub-bands with EEG signals as input.
 
     .. code-block:: python
 
-        transform = BandPowerSpectralDensity()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandPowerSpectralDensity()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The sampling rate of EEG signals in Hz. (default: :obj:`128`)
         fft_n (int): Computes the one-dimensional n-point discrete Fourier Transform (DFT) with the efficient Fast Fourier Transform (FFT) algorithm. If set to None, it will automatically match sampling_rate. (default: :obj:`None`)
         num_window (int): Welch's method computes an estimate of the power spectral density by dividing the data into non-overlapping segments, where the num_window denotes the number of windows. (default: :obj:`1`)
         order (int): The order of the filter. (default: :obj:`5`)
@@ -343,16 +351,18 @@
 
 class BandMeanAbsoluteDeviation(BandTransform):
     r'''
     A transform method for calculating the mean absolute deviation of EEG signals in several sub-bands with EEG signals as input.
 
     .. code-block:: python
 
-        transform = BandMeanAbsoluteDeviation()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandMeanAbsoluteDeviation()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The original sampling rate of EEG signals in Hz. (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the mean absolute deviation of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
     
@@ -378,16 +388,18 @@
 
 class BandKurtosis(BandTransform):
     r'''
     A transform method for calculating the kurtosis of EEG signals in several sub-bands with EEG signals as input.
 
     .. code-block:: python
 
-        transform = BandKurtosis()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandKurtosis()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The original sampling rate of EEG signals in Hz. (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the kurtosis of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
     
@@ -425,16 +437,18 @@
 
 class BandSkewness(BandTransform):
     r'''
     A transform method for calculating the skewness of EEG signals in several sub-bands with EEG signals as input.
 
     .. code-block:: python
 
-        transform = BandSkewness()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandSkewness()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The original sampling rate of EEG signals in Hz. (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the skewness of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/band_pyeeg.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/band_pyeeg.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,16 +83,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/entropy.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandApproximateEntropy()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandApproximateEntropy()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         M (int): A positive integer represents the length of each compared run of data. (default: :obj:`5`)
         R (float): A positive real number specifies a filtering level. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -171,16 +173,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/entropy.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandSampleEntropy()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandSampleEntropy()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         M (int): A positive integer represents the length of each compared run of data. (default: :obj:`5`)
         R (float): A positive real number specifies a filtering level. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -255,16 +259,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/entropy.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandSVDEntropy()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandSVDEntropy()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         Tau (int): A positive integer represents the embedding time delay which controls the number of time periods between elements of each of the new column vectors. (default: :obj:`1`)
         DE (int): A positive integer represents the ength of the embedding dimension. (default: :obj:`1`)
         W (np.ndarray, optional): A list of normalized singular values of the embedding matrix (can be preset for speeding up). (default: :obj:`None`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
@@ -334,16 +340,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/detrended_fluctuation_analysis.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandDetrendedFluctuationAnalysis()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandDetrendedFluctuationAnalysis()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         Ave (float, optional): The average value of the time series. (default: :obj:`None`)
         L (List[np.array]): Box sizes to partition/slice/segment the integrated sequence into boxes. At least two boxes are needed, and it should be a list of integers in ascending order. (default: :obj:`np.array`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -437,16 +445,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/fractal_dimension.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandHiguchiFractalDimension()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandHiguchiFractalDimension()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         K_max (int): The max number of new self-similar time series applying Higuchi's algorithm. (default: :obj:`6`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
@@ -515,16 +525,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/hjorth_mobility_complexity.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandHjorth()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandHjorth()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         D (np.ndarray, optional): The first order differential sequence of the time series (can be preset for speeding up). (default: :obj:`None`)
         mode (str): Options include mobility, complexity, and both, which are used to calculate hjorth mobility, hjorth complexity, and concatenate the two, respectively. (default: :obj:`mobility`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -607,16 +619,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/hurst.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandHurst()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandHurst()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     If the output H=0.5,the behavior of the EEG signals is similar to random walk. If H<0.5, the EEG signals cover less "distance" than a random walk, vice verse.
     
     .. automethod:: __call__
     '''
     def __call__(self,
@@ -665,16 +679,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/fractal_dimension.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandHiguchiFractalDimension()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandHiguchiFractalDimension()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         D (np.ndarray, optional): The first order differential sequence of the time series (can be preset for speeding up). (default: :obj:`None`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
@@ -753,16 +769,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/fractal_dimension.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandBinPower()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandBinPower()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         sampling_rate (int): The original sampling rate in Hz (default: :obj:`128`)
         order (int): The order of the filter. (default: :obj:`5`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -826,16 +844,18 @@
     - URL: https://www.hindawi.com/journals/cin/2011/406391/
     - Related Project: https://github.com/forrestbao/pyeeg/blob/master/pyeeg/entropy.py
 
     Please cite the above paper if you use this module.
 
     .. code-block:: python
 
-        transform = BandSampleEntropy()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.BandSampleEntropy()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         power_ratio (np.ndarray, optional): A list of normalized signal power in the set of sub-bands (can be preset for speeding up). (default: :obj:`None`)
         band_dict: (dict): Band name and the critical sampling rate or frequencies. By default, the differential entropy of the four sub-bands, theta, alpha, beta and gamma, is calculated. (default: :obj:`{...}`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/coefficient.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/coefficient.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 class ARRCoefficient(EEGTransform):
     r'''
     Calculate autoregression reflection coefficients on the input data.
 
     .. code-block:: python
 
-        transform = ARRCoefficient(order=4)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.ARRCoefficient(order=4)
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 4)
 
     Args:
         order (int): The order of autoregressive process to be fitted. (default: :obj:`4`)
         norm (str): Use a biased or unbiased correlation. (default: :obj:`biased`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/concatenate.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/concatenate.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 class Concatenate(EEGTransform):
     r'''
     Merge the calculation results of multiple transforms, which are used when feature fusion is required.
 
     .. code-block:: python
 
-        transform = Concatenate([
-            BandDifferentialEntropy(),
-            BandMeanAbsoluteDeviation()
+        from torcheeg import transforms
+
+        t = transforms.Concatenate([
+            transforms.BandDifferentialEntropy(),
+            transforms.BandMeanAbsoluteDeviation()
         ])
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 8)
 
     Args:
         transforms (list, tuple): a sequence of transforms.
         axis (int): The axis along which the arrays will be joined. If axis is None, arrays are flattened before use (default: :obj:`-1`).
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
@@ -81,38 +83,42 @@
 
 class MapChunk(EEGTransform):
     r'''
     Divide the input EEG signal into multiple chunks according to chunk_size and overlap, and then apply a transofrm to each chunk, and combine the calculation results of a transofrm on all chunks. It is used when feature fusion is required.
 
     .. code-block:: python
 
-        transform = MapChunk(
-            BandDifferentialEntropy(),
+        from torcheeg import transforms
+
+        t = transforms.MapChunk(
+            transforms.BandDifferentialEntropy(),
             chunk_size=250,
             overlap=0
         )
-        transform(eeg=np.random.randn(64, 1000))['eeg'].shape
+        t(eeg=np.random.randn(64, 1000))['eeg'].shape
         >>> (64, 16)
 
     TorchEEG allows feature fusion at multiple scales:
 
     .. code-block:: python
 
-        transform = Concatenate([
-            MapChunk(
-                BandDifferentialEntropy()
+        from torcheeg import transforms
+
+        t = transforms.Concatenate([
+            transforms.MapChunk(
+                transforms.BandDifferentialEntropy()
                 chunk_size=250,
                 overlap=0),  # 4 chunk * 4-dim feature
-            MapChunk(
-                BandDifferentialEntropy()
+            transforms.MapChunk(
+                transforms.BandDifferentialEntropy()
                 chunk_size=500,
                 overlap=0),  # 2 chunk * 4-dim feature
-            BandDifferentialEntropy()  # 1 chunk * 4-dim feature
+            transforms.BandDifferentialEntropy()  # 1 chunk * 4-dim feature
         ])
-        transform(eeg=np.random.randn(64, 1000))['eeg'].shape
+        t(eeg=np.random.randn(64, 1000))['eeg'].shape
         >>> (64, 28) # 4 * 4 + 2 * 4 + 1 * 4
 
     Args:
         transform (EEGTransform): a transform
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
     .. automethod:: __call__
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/correlation.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,18 @@
 
 class PearsonCorrelation(CorrelationTransform):
     r'''
     A transform method to calculate the correlation coefficients between the EEG signals of different electrodes.
 
     .. code-block:: python
 
-        transform = PearsonCorrelation()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.PearsonCorrelation()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (1, 32, 32)
 
     Args:
         absolute (bool): Whether to take the absolute value of the correlation coefficient. (default: :obj:`128`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
     .. automethod:: __call__
@@ -87,16 +89,18 @@
 
 class PhaseLockingCorrelation(CorrelationTransform):
     r'''
     A transform method to calculate the phase locking values between the EEG signals of different electrodes.
 
     .. code-block:: python
 
-        transform = PhaseLockingCorrelation()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.PhaseLockingCorrelation()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (1, 32, 32)
 
     Args:
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
     .. automethod:: __call__
     '''
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/downsample.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/downsample.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 class Downsample(EEGTransform):
     r'''
     Downsample the EEG signal to a specified number of data points.
 
     .. code-block:: python
 
-        transform = Downsample(num_points=32, axis=-1)
+        from torcheeg import transforms
+
+        t = transforms.Downsample(num_points=32, axis=-1)
         # normalize along the first dimension (electrode dimension)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 32)
 
     Args:
         num_points (int): The number of data points after downsampling.
         axis (int, optional): The dimension to normalize, when no dimension is specified, the entire data is normalized. (default: :obj:`-1`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/flatten.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/flatten.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 class Flatten(EEGTransform):
     r'''
     Flatten the input EEG representation.
 
     .. code-block:: python
 
-        transform = Flatten()
-        transform(eeg=np.random.randn(62, 5))['eeg'].shape
+        from torcheeg import transforms
+        
+        t = transforms.Flatten()
+        t(eeg=np.random.randn(62, 5))['eeg'].shape
         >>> (310,)
 
     .. automethod:: __call__
     '''
     def __call__(self,
                  *args,
                  eeg: np.ndarray,
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/normalize.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 class MeanStdNormalize(EEGTransform):
     r'''
     Perform z-score normalization on the input data. This class allows the user to define the dimension of normalization and the used statistic.
 
     .. code-block:: python
 
-        transform = MeanStdNormalize(axis=0)
+        from torcheeg import transforms
+
+        t = transforms.MeanStdNormalize(axis=0)
         # normalize along the first dimension (electrode dimension)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 128)
 
-        transform = MeanStdNormalize(axis=1)
+        t = transforms.MeanStdNormalize(axis=1)
         # normalize along the second dimension (temproal dimension)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 128)
 
     Args:
         mean (np.array, optional): The mean used in the normalization process, allowing the user to provide mean statistics in :obj:`np.ndarray` format. When statistics are not provided, use the statistics of the current sample for normalization.
         std (np.array, optional): The standard deviation used in the normalization process, allowing the user to provide tandard deviation statistics in :obj:`np.ndarray` format. When statistics are not provided, use the statistics of the current sample for normalization.
         axis (int, optional): The dimension to normalize, when no dimension is specified, the entire data is normalized.
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -89,22 +91,26 @@
 
 class MinMaxNormalize(EEGTransform):
     r'''
     Perform min-max normalization on the input data. This class allows the user to define the dimension of normalization and the used statistic.
 
     .. code-block:: python
 
-        transform = MinMaxNormalize(axis=0)
+        from torcheeg import transforms
+
+        t = transforms.MinMaxNormalize(axis=0)
         # normalize along the first dimension (electrode dimension)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 128)
 
-        transform = MinMaxNormalize(axis=1)
+        from torcheeg import transforms
+        
+        t = transforms.MinMaxNormalize(axis=1)
         # normalize along the second dimension (temproal dimension)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 128)
 
     Args:
         min (np.array, optional): The minimum used in the normalization process, allowing the user to provide minimum statistics in :obj:`np.ndarray` format. When statistics are not provided, use the statistics of the current sample for normalization.
         max (np.array, optional): The maximum used in the normalization process, allowing the user to provide maximum statistics in :obj:`np.ndarray` format. When statistics are not provided, use the statistics of the current sample for normalization.
         axis (int, optional): The dimension to normalize, when no dimension is specified, the entire data is normalized.
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/pick.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/pick.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 
 class PickElectrode(EEGTransform):
     r'''
     Select parts of electrode signals based on a given electrode index list.
 
     .. code-block:: python
 
-        transform = PickElectrode(PickElectrode.to_index_list(
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LIST
+
+        t = transforms.PickElectrode(transforms.PickElectrode.to_index_list(
             ['FP1', 'AF3', 'F3', 'F7',
              'FC5', 'FC1', 'C3', 'T7',
              'CP5', 'CP1', 'P3', 'P7',
              'PO3','O1', 'FP2', 'AF4',
              'F4', 'F8', 'FC6', 'FC2',
              'C4', 'T8', 'CP6', 'CP2',
              'P4', 'P8', 'PO4', 'O2'], DEAP_CHANNEL_LIST))
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (28, 128)
 
     Args:
         pick_list (np.ndarray): Selected electrode list. Should consist of integers representing the corresponding electrode indices. :obj:`to_index_list` can be used to obtain an index list when we only know the names of the electrode and not their indices.
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
 
     .. automethod:: __call__
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/rearrange.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/rearrange.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 class RearrangeElectrode(EEGTransform):
     r'''
     Select parts of electrode signals based on a given electrode index list.
 
     .. code-block:: python
 
-        transform = RearrangeElectrode(
+        from torcheeg import transforms
+
+        t = transforms.RearrangeElectrode(
             source=['FP1', 'F3', 'F7'],
             target=['F3', 'F7', 'FP1', 'AF2'],
             missing='mean'
         )
-        transform(eeg=np.random.randn(3, 128))['eeg'].shape
+        t(eeg=np.random.randn(3, 128))['eeg'].shape
         >>> (4, 128)
 
     Args:
         source (list): The list of electrode names to be rearranged.
         target (list): The list of electrode names to be rearranged to.
         missing (str): The method to deal with missing electrodes. (default: :obj:`'random'`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/spectrum.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/spectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,36 +10,42 @@
 
 class CWTSpectrum(EEGTransform):
     r'''
         A transform method to convert EEG signals of each channel into spectrograms using wavelet transform.
 
         .. code-block:: python
 
-            transform = CWTSpectrum()
-            transform(eeg=np.random.randn(32, 1000))['eeg'].shape
+            from torcheeg import transforms
+
+            t = transforms.CWTSpectrum()
+            t(eeg=np.random.randn(32, 1000))['eeg'].shape
             >>> (32, 128, 1000)
 
         Part of the existing work uses :obj:`Resize` to warp the output spectrum to a specified size suitable for CNN processing.
 
         .. code-block:: python
 
-            transform = Compose([
+            from torcheeg import transforms
+        
+            t = Compose([
                 CWTSpectrum(),
                 ToTensor(),
                 Resize([260, 260])
             ])
-            transform(eeg=np.random.randn(32, 1000))['eeg'].shape
+            t(eeg=np.random.randn(32, 1000))['eeg'].shape
             >>> (32, 128, 1000)
 
         When contourf is set to True, a spectrogram of filled contours will be generated for each channel and converted to np.ndarray and returned. This option is usually used for single-channel analysis or visualization of a single channel.
 
         .. code-block:: python
 
-            transform = CWTSpectrum(contourf=True)
-            transform(eeg=np.random.randn(32, 1000))['eeg'].shape
+            from torcheeg import transforms
+
+            t = CWTSpectrum(contourf=True)
+            t(eeg=np.random.randn(32, 1000))['eeg'].shape
             >>> (32, 480, 640, 4)
 
         Args:
             sampling_rate (int): The sampling period for the frequencies output in Hz. (default: :obj:`128`)
             wavelet (str): Wavelet to use. Options include: cgau1, cgau2, cgau3, cgau4, cgau5, cgau6, cgau7, cgau8, cmor, fbsp, gaus1, gaus2 , gaus3, gaus4, gaus5, gaus6, gaus7, gaus8, mexh, morl, shan. (default: :obj:`'morl'`)
             total_scale: (int): The total wavelet scales to use. (default: :obj:`128`)
             contourf: (bool): Whether to output the np.ndarray corresponding to the image with content of filled contours. (default: :obj:`False`)
@@ -133,16 +139,18 @@
 
 class DWTDecomposition(EEGTransform):
     r'''    
         Splitting the EEG signal from each electrode into two functions using wavelet decomposition.
 
         .. code-block:: python
 
-            transform = DWTDecomposition()
-            transform(eeg=np.random.randn(32, 1000))['eeg'].shape
+            from torcheeg import transforms
+
+            t = transforms.DWTDecomposition()
+            t(eeg=np.random.randn(32, 1000))['eeg'].shape
             >>> (32, 500)
 
         Args:
             apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
         
         .. automethod:: __call__
     '''
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/numpy/to.py` & `torcheeg-1.1.2/torcheeg/transforms/numpy/to.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 class To2d(EEGTransform):
     r'''
     Taking the electrode index as the row index and the temporal index as the column index, a two-dimensional EEG signal representation with the size of [number of electrodes, number of data points] is formed. While PyTorch performs convolution on the 2d tensor, an additional channel dimension is required, thus we append an additional dimension.
 
     .. code-block:: python
 
-        transform = To2d()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.To2d()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (1, 32, 128)
 
     .. automethod:: __call__
     '''
     def __call__(self,
                  *args,
                  eeg: np.ndarray,
@@ -45,16 +47,19 @@
     - datasets.constants.emotion_recognition.deap.DEAP_CHANNEL_LOCATION_DICT
     - datasets.constants.emotion_recognition.dreamer.DREAMER_CHANNEL_LOCATION_DICT
     - datasets.constants.emotion_recognition.seed.SEED_CHANNEL_LOCATION_DICT
     - ...
 
     .. code-block:: python
 
-        transform = ToGrid(DEAP_CHANNEL_LOCATION_DICT)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+
+        t = transforms.ToGrid(DEAP_CHANNEL_LOCATION_DICT)
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (128, 9, 9)
 
     Args:
         channel_location_dict (dict): Electrode location information. Represented in dictionary form, where :obj:`key` corresponds to the electrode name and :obj:`value` corresponds to the row index and column index of the electrode on the grid.
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
     
     .. automethod:: __call__
@@ -140,16 +145,19 @@
     - datasets.constants.emotion_recognition.deap.DEAP_CHANNEL_LOCATION_DICT
     - datasets.constants.emotion_recognition.dreamer.DREAMER_CHANNEL_LOCATION_DICT
     - datasets.constants.emotion_recognition.seed.SEED_CHANNEL_LOCATION_DICT
     - ...
 
     .. code-block:: python
     
-        transform = ToInterpolatedGrid(DEAP_CHANNEL_LOCATION_DICT)
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+
+        t = ToInterpolatedGrid(DEAP_CHANNEL_LOCATION_DICT)
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (128, 9, 9)
 
     Especially, missing values on the grid are supplemented using cubic interpolation
 
     Args:
         channel_location_dict (dict): Electrode location information. Represented in dictionary form, where :obj:`key` corresponds to the electrode name and :obj:`value` corresponds to the row index and column index of the electrode on the grid.
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/pyg/to.py` & `torcheeg-1.1.2/torcheeg/transforms/pyg/to.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,19 @@
     - datasets.constants.emotion_recognition.deap.DEAP_ADJACENCY_MATRIX
     - datasets.constants.emotion_recognition.dreamer.DREAMER_ADJACENCY_MATRIX
     - datasets.constants.emotion_recognition.seed.SEED_ADJACENCY_MATRIX
     - ...
 
     .. code-block:: python
 
-        transform = ToG(adj=DEAP_ADJACENCY_MATRIX)
-        transform(eeg=np.random.randn(32, 128))['eeg']
+        from torcheeg.transforms.pyg import ToG
+        from torcheeg.datasets.constants import DEAP_ADJACENCY_MATRIX
+
+        t = ToG(adj=DEAP_ADJACENCY_MATRIX)
+        t(eeg=np.random.randn(32, 128))['eeg']
         >>> torch_geometric.data.Data
 
     Args:
         adj (list): An adjacency matrix represented by a 2D array, each element in the adjacency matrix represents the electrode-to-electrode edge weight. Please keep the order of electrodes in the rows and columns of the adjacency matrix consistent with the EEG signal to be transformed.
         add_self_loop (bool): Whether to add self-loop edges to the graph. (default: :obj:`True`)
         threshold (float, optional): Used to cut edges when not None. Edges whose weights exceed a threshold are retained. (default: :obj:`None`)
         top_k (int, optional): Used to cut edges when not None. Keep the k edges connected to each node with the largest weights. (default: :obj:`None`)
@@ -123,28 +126,30 @@
 
     - Gaussian Distance
     - Absolute Pearson Correlation Coefficient
     - Phase Locking Value
 
     .. code-block:: python
 
-        transform = ToDynamicG(edge_func='gaussian_distance', sigma=1.0, top_k=10, complete_graph=False)
-        transform(eeg=np.random.randn(32, 128))['eeg']
+        from torcheeg.transforms.pyg import ToDynamicG
+
+        t = ToDynamicG(edge_func='gaussian_distance', sigma=1.0, top_k=10, complete_graph=False)
+        t(eeg=np.random.randn(32, 128))['eeg']
         >>> Data(edge_index=[2, 320], x=[32, 128], edge_weight=[320])
 
-        transform = ToDynamicG(edge_func='absolute_pearson_correlation_coefficient', threshold=0.1, binary=True)
-        transform(eeg=np.random.randn(32, 128))['eeg']
+        t = ToDynamicG(edge_func='absolute_pearson_correlation_coefficient', threshold=0.1, binary=True)
+        t(eeg=np.random.randn(32, 128))['eeg']
         >>> Data(edge_index=[2, 310], x=[32, 128], edge_weight=[310])
 
-        transform = ToDynamicG(edge_func='phase_locking_value')
-        transform(eeg=np.random.randn(32, 128))['eeg']
+        t = ToDynamicG(edge_func='phase_locking_value')
+        t(eeg=np.random.randn(32, 128))['eeg']
         >>> Data(edge_index=[2, 992], x=[32, 128], edge_weight=[992])
 
-        transform = ToDynamicG(edge_func=lambda x, y: (x * y).mean())
-        transform(eeg=np.random.randn(32, 128))['eeg']
+        t = ToDynamicG(edge_func=lambda x, y: (x * y).mean())
+        t(eeg=np.random.randn(32, 128))['eeg']
         >>> Data(edge_index=[2, 1024], x=[32, 128], edge_weight=[1024])
 
     Args:
         edge_func (str or Callable): Algorithms for computing functional connections. You can use the algorithms provided by TorchEEG, including gaussian_distance, absolute_pearson_correlation_coefficient and phase_locking_value. Or you can use custom functions by passing a callable object containing two parameters representing the signal of the two electrodes, and other named parameters (passed in when initializing the transform), and outputs the value of the functional connection between the two electrodes. (default: :obj:`gaussian_distance`)
         add_self_loop (bool): Whether to add self-loop edges to the graph. (default: :obj:`True`)
         threshold (float, optional): Used to cut edges when not None. Edges whose weights exceed a threshold are retained. (default: :obj:`None`)
         top_k (int, optional): Used to cut edges when not None. Keep the k edges connected to each node with the largest weights. (default: :obj:`None`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/torch/contrastive.py` & `torcheeg-1.1.2/torcheeg/transforms/torch/contrastive.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 
 class Contrastive(EEGTransform):
     r'''
     To allow efficient training, we need to prepare the data loading such that we sample two different, random augmentations for each EEG in the batch. The easiest way to do this is by creating a transformation that, when being called, applies a set of data augmentations to an EEG twice.
 
     .. code-block:: python
 
-        transform = Contrastive(RandomNoise(), num_views=2)
-        transform(eeg=torch.randn(32, 128))['eeg'][0].shape
+        from torcheeg import transforms
+
+        t = Contrastive(transforms.RandomNoise(), num_views=2)
+        t(eeg=torch.randn(32, 128))['eeg'][0].shape
         >>> (32, 128)
-        transform(eeg=torch.randn(32, 128))['eeg'][1].shape
+        t(eeg=torch.randn(32, 128))['eeg'][1].shape
         >>> (32, 128)
 
     .. automethod:: __call__
     '''
 
     def __init__(self,
                  transform: List[EEGTransform],
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/torch/random.py` & `torcheeg-1.1.2/torcheeg/transforms/torch/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 
 class RandomNoise(RandomEEGTransform):
     '''
     Add random noise conforming to the normal distribution on the EEG signal.
     
     .. code-block:: python
 
-        transform = RandomNoise(p=0.5)
-        transform(eeg=torch.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.RandomNoise(p=0.5)
+        t(eeg=torch.randn(32, 128))['eeg'].shape
         >>> (32, 128)
 
     Args:
         mean (float): The mean of the normal distribution of noise. (default: :obj:`0.0`)
         std (float): The standard deviation of the normal distribution of noise. (default: :obj:`0.0`)
         p (float): Probability of adding noise to EEG signal samples. Should be between 0.0 and 1.0, where 0.0 means no noise is added to every sample and 1.0 means that noise is added to every sample. (default: :obj:`0.5`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
@@ -119,15 +121,15 @@
         Returns:
             torch.Tensor: The output EEG signal after applying a random mask.
         '''
         return super().__call__(*args, eeg=eeg, baseline=baseline, **kwargs)
 
     def random_apply(self, eeg: torch.Tensor, **kwargs) -> torch.Tensor:
         mask = torch.rand_like(eeg)
-        mask = (mask < self.ratio).to(eeg.dtype)
+        mask = (mask > self.ratio).to(eeg.dtype)
         return eeg * mask
 
     @property
     def repr_body(self) -> Dict:
         return dict(super().repr_body, **{'ratio': self.ratio})
 
 
@@ -170,15 +172,15 @@
             torch.Tensor: The output EEG signal after applying a random mask.
         '''
         return super().__call__(*args, eeg=eeg, baseline=baseline, **kwargs)
 
     def random_apply(self, eeg: torch.Tensor, **kwargs) -> torch.Tensor:
         # mask at the electrode dimension
         mask = torch.rand(eeg.shape[1], device=eeg.device)
-        mask = (mask < self.ratio).to(eeg.dtype)
+        mask = (mask > self.ratio).to(eeg.dtype)
         # to the same shape of eeg
         mask = mask.unsqueeze(0).unsqueeze(2).repeat(eeg.shape[0], 1,
                                                      eeg.shape[2])
         return eeg * mask
 
     @property
     def repr_body(self) -> Dict:
@@ -224,15 +226,15 @@
             torch.Tensor: The output EEG signal after applying a random mask.
         '''
         return super().__call__(*args, eeg=eeg, baseline=baseline, **kwargs)
 
     def random_apply(self, eeg: torch.Tensor, **kwargs) -> torch.Tensor:
         # mask at the electrode dimension
         mask = torch.rand(eeg.shape[1], eeg.shape[2], device=eeg.device)
-        mask = (mask < self.ratio).to(eeg.dtype)
+        mask = (mask > self.ratio).to(eeg.dtype)
         mask = mask.unsqueeze(0).repeat(eeg.shape[0], 1, 1)
         return eeg * mask
 
     @property
     def repr_body(self) -> Dict:
         return dict(super().repr_body, **{'ratio': self.ratio})
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/torch/resize.py` & `torcheeg-1.1.2/torcheeg/transforms/torch/resize.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 class Resize(EEGTransform):
     r'''
     Use an interpolation algorithm to scale a grid-like EEG signal at the spatial dimension.
 
     .. code-block:: python
 
-        transform = ToTensor(size=(64, 64))
-        transform(eeg=torch.randn(128, 9, 9))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.ToTensor(size=(64, 64))
+        t(eeg=torch.randn(128, 9, 9))['eeg'].shape
         >>> (128, 64, 64)
 
     Args:
         size (tuple): The output spatial size.
         interpolation (str): The interpolation algorithm used for upsampling, can be nearest, linear, bilinear, bicubic, trilinear, and area. (default: :obj:`'nearest'`)
         apply_to_baseline: (bool): Whether to act on the baseline signal at the same time, if the baseline is passed in when calling. (default: :obj:`False`)
```

### Comparing `torcheeg-1.1.1/torcheeg/transforms/torch/to.py` & `torcheeg-1.1.2/torcheeg/transforms/torch/to.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 class ToTensor(EEGTransform):
     r'''
     Convert a :obj:`numpy.ndarray` to tensor. Different from :obj:`torchvision`, tensors are returned without scaling.
 
     .. code-block:: python
 
-        transform = ToTensor()
-        transform(eeg=np.random.randn(32, 128))['eeg'].shape
+        from torcheeg import transforms
+
+        t = transforms.ToTensor()
+        t(eeg=np.random.randn(32, 128))['eeg'].shape
         >>> (32, 128)
 
     Args:
         apply_to_baseline (bool): Whether to apply the transform to the baseline signal. (default: :obj:`False`)
 
     .. automethod:: __call__
     '''
```

### Comparing `torcheeg-1.1.1/torcheeg/utils/file.py` & `torcheeg-1.1.2/torcheeg/utils/file.py`

 * *Files identical despite different names*

### Comparing `torcheeg-1.1.1/torcheeg/utils/pyg/visualize.py` & `torcheeg-1.1.2/torcheeg/utils/pyg/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 
     - datasets.constants.emotion_recognition.deap.DEAP_CHANNEL_LOCATION_DICT
     - datasets.constants.emotion_recognition.dreamer.DREAMER_CHANNEL_LOCATION_DICT
     - datasets.constants.emotion_recognition.seed.SEED_CHANNEL_LOCATION_DICT
     - ...
 
     .. code-block:: python
+        
+        from torcheeg.utils.pyg import plot_graph
+        from torcheeg.datasets.constants import DEAP_CHANNEL_LOCATION_DICT
+        from torcheeg.transforms.pyg import ToG
+        import numpy as np
 
         eeg = np.random.randn(32, 128)
         g = ToG(DEAP_ADJACENCY_MATRIX)(eeg=eeg)['eeg']
         img = plot_graph(g)
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_graph.png
```

### Comparing `torcheeg-1.1.1/torcheeg/utils/visualize.py` & `torcheeg-1.1.2/torcheeg/utils/visualize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import io
-import itertools
-import random
-from typing import Dict, List, Union
+from typing import List, Tuple, Union
 
 import matplotlib
 import matplotlib.pyplot as plt
 import mne
 import numpy as np
 import PIL
 import torch
@@ -32,14 +30,17 @@
                      plot_second_list: List[int] = [0.0, 0.25, 0.5, 0.75],
                      montage: mne.channels.DigMontage = default_montage):
     r'''
     Plot a topographic map of the input raw EEG signal as image.
 
     .. code-block:: python
 
+        from torcheeg.utils import plot_raw_topomap
+        from torcheeg.constants import DEAP_CHANNEL_LIST
+
         eeg = torch.randn(32, 128)
         img = plot_raw_topomap(eeg,
                          channel_list=DEAP_CHANNEL_LIST,
                          sampling_rate=128)
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_raw_topomap.png
@@ -83,20 +84,24 @@
     plt.show()
     return np.array(img)
 
 
 def plot_feature_topomap(tensor: torch.Tensor,
                          channel_list: List[str],
                          feature_list: Union[List[str], None] = None,
-                         montage: mne.channels.DigMontage = default_montage):
+                         montage: mne.channels.DigMontage = default_montage,
+                         fig_shape: Tuple[int, int] = None):
     r'''
     Plot a topographic map of the input EEG features as image.
 
     .. code-block:: python
 
+        from torcheeg.utils import plot_feature_topomap
+        from torcheeg.constants import DEAP_CHANNEL_LIST
+
         eeg = torch.randn(32, 4)
         img = plot_feature_topomap(eeg,
                          channel_list=DEAP_CHANNEL_LIST,
                          feature_list=["theta", "alpha", "beta", "gamma"])
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_feature_topomap.png
@@ -106,14 +111,15 @@
     |
 
     Args:
         tensor (torch.Tensor): The input EEG signal, the shape should be [number of channels, dimensions of features].
         channel_list (list): The channel name lists corresponding to the input EEG signal. If the dataset in TorchEEG is used, please refer to the CHANNEL_LIST related constants in the :obj:`torcheeg.constants` module.
         feature_list (list): . The names of feature dimensions displayed on the output image, whose length should be consistent with the dimensions of features. If set to None, the dimension index of the feature is used instead. (default: :obj:`None`)
         montage (any): Channel positions and digitization points defined in obj:`mne`. (default: :obj:`mne.channels.make_standard_montage('standard_1020')`)
+        fig_shape (Tuple[int, int], optional): The shape of the sub graphs (width, height). If `None`, the layout is automatically set to (1, len(feature_list)). (default: :obj:`None`)
     
     Returns:
         np.ndarray: The output image in the form of :obj:`np.ndarray`.
     '''
     ch_types = ['eeg'] * len(channel_list)
     info = mne.create_info(ch_names=channel_list, ch_types=ch_types, sfreq=128)
     tensor = tensor.detach().cpu().numpy()
@@ -122,24 +128,43 @@
                      match_case=False,
                      on_missing='ignore')
 
     if feature_list is None:
         feature_list = list(range(tensor.shape[1]))
     num_subplots = len(feature_list)
 
-    fig, axes = plt.subplots(1, num_subplots, figsize=(num_subplots * 5, 5))
+    if fig_shape == None:
+        fig_shape = (1, num_subplots)
+    else:
+        if len(fig_shape) != 2:
+            raise ValueError(
+                "fig_shape only support 2d graph, so just contain width and height"
+            )
+        if not all(isinstance(n, int) and n > 0 for n in fig_shape):
+            raise ValueError(
+                "width and height in fig_shape must be positive integers")
+        if fig_shape[0] * fig_shape[1] != num_subplots:
+            raise ValueError(
+                f"The product of width and height in fig_shape must equal feature_list length: {num_subplots}"
+            )
+
+    fig, axes = plt.subplots(fig_shape[0],
+                             fig_shape[1],
+                             figsize=(fig_shape[1] * 5, fig_shape[0] * 5),
+                             squeeze=False)
 
     if num_subplots > 1:
         for i, (label) in enumerate(feature_list):
+            row, col = i // fig_shape[1], i % fig_shape[1]
             mne.viz.plot_topomap(tensor[:, i],
                                  info,
-                                 axes=axes[i],
+                                 axes=axes[row, col],
                                  show=False,
                                  sphere=(0., 0., 0., 0.11))
-            axes[i].set_title(label, {
+            axes[row, col].set_title(label, {
                 'fontsize': 24,
                 'fontname': 'Liberation Serif'
             })
     else:
         mne.viz.plot_topomap(tensor[:, 0],
                              info,
                              axes=axes,
@@ -160,14 +185,19 @@
                 sampling_rate: int,
                 montage: mne.channels.DigMontage = default_montage):
     r'''
     Plot signal values of the input raw EEG as image.
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.utils import plot_signal
+        from torcheeg.constants import DEAP_CHANNEL_LIST
+
         eeg = torch.randn(32, 128)
         img = plot_signal(eeg,
                           channel_list=DEAP_CHANNEL_LIST,
                           sampling_rate=128)
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_signal.png
@@ -201,14 +231,16 @@
 def plot_3d_tensor(tensor: torch.Tensor,
                    color: Union[colors.Colormap, str] = 'hsv'):
     r'''
     Visualize a 3-D matrices in 3-D space.
 
     .. code-block:: python
 
+        from torcheeg.utils import plot_3d_tensor
+
         eeg = torch.randn(128, 9, 9)
         img = plot_3d_tensor(eeg)
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_3d_tensor.png
         :alt: The output image of plot_3d_tensor
         :align: center
@@ -246,14 +278,18 @@
 def plot_2d_tensor(tensor: torch.Tensor,
                    color: Union[colors.Colormap, str] = 'hsv'):
     r'''
     Visualize a 2-D matrices in 2-D space.
 
     .. code-block:: python
 
+        import torch
+
+        from torcheeg.utils import plot_2d_tensor
+
         eeg = torch.randn(9, 9)
         img = plot_2d_tensor(eeg)
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_2d_tensor.png
         :alt: The output image of plot_2d_tensor
         :align: center
@@ -287,14 +323,19 @@
                           num_connectivity: int = 60,
                           linewidth: float = 1.5):
     r'''
     Visualize connectivity between nodes in an adjacency matrix, using circular networks.
 
     .. code-block:: python
 
+        import torch
+        
+        from torcheeg.utils import plot_adj_connectivity
+        from torcheeg.constants import SEED_CHANNEL_LIST
+        
         adj = torch.randn(62, 62) # relationship between 62 electrodes
         img = plot_adj_connectivity(adj, SEED_CHANNEL_LIST)
         # If using jupyter, the output image will be drawn on notebooks.
 
     .. image:: _static/plot_adj_connectivity.png
         :alt: The output image of plot_adj_connectivity
         :align: center
@@ -345,17 +386,15 @@
                 electrode_colors[i] = region_colors[region_index]
                 i += 1
 
         adj = new_adj
         channel_list = new_channel_list
         node_colors = electrode_colors
 
-    node_angles = circular_layout(channel_list,
-                                  channel_list,
-                                  start_pos=90)
+    node_angles = circular_layout(channel_list, channel_list, start_pos=90)
     # Plot the graph using node colors from the FreeSurfer parcellation. We only
     # show the 300 strongest connections.
     fig, ax = plt.subplots(figsize=(8, 8),
                            facecolor='white',
                            subplot_kw=dict(polar=True))
     plot_connectivity_circle(adj,
                              channel_list,
```

### Comparing `torcheeg-1.1.1/torcheeg.egg-info/PKG-INFO` & `torcheeg-1.1.2/torcheeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheeg
-Version: 1.1.1
+Version: 1.1.2
 Summary: TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG aims to provide a plug-and-play EEG analysis tool, so that researchers can quickly reproduce EEG analysis work and start new EEG analysis research without paying attention to technical details unrelated to the research focus.
 Home-page: https://github.com/tczhangzhi/torcheeg
 Author: TorchEEG Team
 Author-email: tczhangzhi@gmail.com
 License: MIT
 Keywords: PyTorch,EEG
 Requires-Python: >=3.7
@@ -16,15 +16,16 @@
 
 TorchEEG
 ========
 
 |PyPI Version| |Docs Status| |Downloads| |Join the Chat|
 
 `Documentation <https://torcheeg.readthedocs.io/>`__ \| `TorchEEG
-Examples <https://github.com/tczhangzhi/torcheeg/tree/main/examples>`__
+Examples <https://github.com/torcheeg/torcheeg/tree/main/examples>`__ \|
+`Paper <https://www.sciencedirect.com/science/article/pii/S0957417424004159>`__
 
 TorchEEG is a library built on PyTorch for EEG signal analysis. TorchEEG
 aims to provide a plug-and-play EEG analysis tool, so that researchers
 can quickly reproduce EEG analysis work and start new EEG analysis
 research without paying attention to technical details unrelated to the
 research focus.
 
@@ -267,15 +268,15 @@
 e.g. ``./tmp_in/data_preprocessed_python``.
 
 .. code:: python
 
    from torcheeg.datasets import DEAPDataset
    from torcheeg import transforms
 
-   from torcheeg.datasets.constants.emotion_recognition.deap import \
+   from torcheeg.datasets.constants import \
        DEAP_CHANNEL_LOCATION_DICT
 
    dataset = DEAPDataset(
        io_path=f'./tmp_out/examples_pipeline/deap',
        root_path='./tmp_in/data_preprocessed_python',
        offline_transform=transforms.Compose([
            transforms.BandDifferentialEntropy(apply_to_baseline=True),
@@ -378,14 +379,30 @@
 License
 -------
 
 TorchEEG has a MIT license, as found in the
 `LICENSE <https://github.com/tczhangzhi/torcheeg/blob/main/LICENSE>`__
 file.
 
+Citation
+--------
+
+If you find this project useful for your research, please cite:
+
+.. code:: latex
+
+   @article{zhang2024torcheeg,
+       title = {{TorchEEGEMO}: A deep learning toolbox towards {EEG}-based emotion recognition},
+       journal = {Expert Systems with Applications},
+       pages = {123550},
+       year = {2024},
+       issn = {0957-4174},
+       author = {Zhi Zhang and Sheng-hua Zhong and Yan Liu}
+   }
+
 .. |PyPI Version| image:: https://badge.fury.io/py/torcheeg.svg
    :target: https://pypi.python.org/pypi/torcheeg
 .. |Docs Status| image:: https://readthedocs.org/projects/torcheeg/badge/?version=latest
    :target: https://torcheeg.readthedocs.io/en/latest/?badge=latest
 .. |Downloads| image:: https://pepy.tech/badge/torcheeg
    :target: https://pepy.tech/project/torcheeg
 .. |Join the Chat| image:: https://badges.gitter.im/torcheeg/community.svg
```

### Comparing `torcheeg-1.1.1/torcheeg.egg-info/SOURCES.txt` & `torcheeg-1.1.2/torcheeg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 README.md
 README.rst
 setup.py
 test/__init__.py
 test/datasets/__init__.py
 test/datasets/test_emotion_recognition.py
 test/datasets/test_folder.py
-test/datasets/test_hooks.py
 test/datasets/test_motor_imagery.py
 test/datasets/test_personal_identification.py
+test/datasets/test_sleep_stage_detection.py
 test/datasets/test_ssvep.py
 test/io/__init__.py
 test/io/test_eeg_signal.py
 test/io/test_meta_info.py
 test/model_selection/__init__.py
 test/model_selection/test_k_fold.py
 test/model_selection/test_k_fold_cross_subject.py
@@ -44,14 +44,15 @@
 test/trainers/test_gan_trainer.py
 test/trainers/test_glow_trainer.py
 test/trainers/test_imbalance_trainer.py
 test/trainers/test_self_supervised_trainer.py
 test/trainers/test_vae_trainer.py
 test/transforms/__init__.py
 test/transforms/test_any.py
+test/transforms/test_hooks.py
 test/transforms/test_label.py
 test/transforms/test_numpy.py
 test/transforms/test_pyg.py
 test/transforms/test_torch.py
 test/utils/__init__.py
 test/utils/test_visualize.py
 torcheeg/__init__.py
@@ -69,49 +70,57 @@
 torcheeg/datasets/constants/clinical/__init__.py
 torcheeg/datasets/constants/clinical/tuh_tueg.py
 torcheeg/datasets/constants/emotion_recognition/__init__.py
 torcheeg/datasets/constants/emotion_recognition/amigos.py
 torcheeg/datasets/constants/emotion_recognition/bci2022.py
 torcheeg/datasets/constants/emotion_recognition/deap.py
 torcheeg/datasets/constants/emotion_recognition/dreamer.py
+torcheeg/datasets/constants/emotion_recognition/faced.py
 torcheeg/datasets/constants/emotion_recognition/mahnob.py
 torcheeg/datasets/constants/emotion_recognition/mped.py
 torcheeg/datasets/constants/emotion_recognition/seed.py
 torcheeg/datasets/constants/emotion_recognition/seed_iv.py
+torcheeg/datasets/constants/emotion_recognition/seed_v.py
 torcheeg/datasets/constants/motor_imagery/__init__.py
 torcheeg/datasets/constants/motor_imagery/bciciv_2a.py
 torcheeg/datasets/constants/personal_identification/__init__.py
 torcheeg/datasets/constants/personal_identification/m3cv.py
+torcheeg/datasets/constants/sleep_stage_detection/__init__.py
+torcheeg/datasets/constants/sleep_stage_detection/sleep_edfx.py
 torcheeg/datasets/constants/ssvep/__init__.py
 torcheeg/datasets/constants/ssvep/tsu_benchmark.py
-torcheeg/datasets/functional/__init__.py
-torcheeg/datasets/functional/hooks.py
 torcheeg/datasets/moabb/__init__.py
 torcheeg/datasets/moabb/moabb_dataset.py
 torcheeg/datasets/module/__init__.py
 torcheeg/datasets/module/base_dataset.py
 torcheeg/datasets/module/csv_folder_dataset.py
 torcheeg/datasets/module/folder_dataset.py
 torcheeg/datasets/module/emotion_recognition/__init__.py
 torcheeg/datasets/module/emotion_recognition/amigos.py
 torcheeg/datasets/module/emotion_recognition/bci2022.py
 torcheeg/datasets/module/emotion_recognition/deap.py
 torcheeg/datasets/module/emotion_recognition/dreamer.py
+torcheeg/datasets/module/emotion_recognition/faced.py
+torcheeg/datasets/module/emotion_recognition/faced_feature.py
 torcheeg/datasets/module/emotion_recognition/mahnob.py
 torcheeg/datasets/module/emotion_recognition/mped_feature.py
 torcheeg/datasets/module/emotion_recognition/seed.py
 torcheeg/datasets/module/emotion_recognition/seed_feature.py
 torcheeg/datasets/module/emotion_recognition/seed_iv.py
 torcheeg/datasets/module/emotion_recognition/seed_iv_feature.py
+torcheeg/datasets/module/emotion_recognition/seed_v.py
+torcheeg/datasets/module/emotion_recognition/seed_v_feature.py
 torcheeg/datasets/module/motor_imagery/__init__.py
 torcheeg/datasets/module/motor_imagery/bciciv_2a.py
 torcheeg/datasets/module/personal_identification/__init__.py
 torcheeg/datasets/module/personal_identification/m3cv.py
-torcheeg/datasets/module/sspev/__init__.py
-torcheeg/datasets/module/sspev/tsu_benchmark.py
+torcheeg/datasets/module/sleep_stage_detection/__init__.py
+torcheeg/datasets/module/sleep_stage_detection/sleep_edfx.py
+torcheeg/datasets/module/ssvep/__init__.py
+torcheeg/datasets/module/ssvep/tsu_benchmark.py
 torcheeg/io/__init__.py
 torcheeg/io/eeg_signal.py
 torcheeg/io/meta_info.py
 torcheeg/model_selection/__init__.py
 torcheeg/model_selection/k_fold.py
 torcheeg/model_selection/k_fold_cross_subject.py
 torcheeg/model_selection/k_fold_cross_trial.py
@@ -197,14 +206,17 @@
 torcheeg/transforms/__init__.py
 torcheeg/transforms/base_transform.py
 torcheeg/transforms/any/__init__.py
 torcheeg/transforms/any/baseline.py
 torcheeg/transforms/any/compose.py
 torcheeg/transforms/any/lambd.py
 torcheeg/transforms/any/pdb.py
+torcheeg/transforms/hooks/__init__.py
+torcheeg/transforms/hooks/after_hook.py
+torcheeg/transforms/hooks/before_hook.py
 torcheeg/transforms/label/__init__.py
 torcheeg/transforms/label/binary.py
 torcheeg/transforms/label/fix.py
 torcheeg/transforms/label/mapping.py
 torcheeg/transforms/label/select.py
 torcheeg/transforms/label/string.py
 torcheeg/transforms/numpy/__init__.py
```

