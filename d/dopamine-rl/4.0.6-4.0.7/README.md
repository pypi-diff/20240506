# Comparing `tmp/dopamine_rl-4.0.6.tar.gz` & `tmp/dopamine_rl-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dopamine_rl-4.0.6.tar", last modified: Wed Sep 21 20:18:34 2022, max compression
+gzip compressed data, was "dopamine_rl-4.0.7.tar", last modified: Mon May  6 16:58:41 2024, max compression
```

## Comparing `dopamine_rl-4.0.6.tar` & `dopamine_rl-4.0.7.tar`

### file list

```diff
@@ -1,116 +1,120 @@
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.814723 dopamine_rl-4.0.6/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      298 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/AUTHORS
--rw-r--r--   0 psc      (160661) primarygroup (89939)    11417 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/LICENSE
--rw-r--r--   0 psc      (160661) primarygroup (89939)     7564 2022-09-21 20:18:34.814356 dopamine_rl-4.0.6/PKG-INFO
--rw-r--r--   0 psc      (160661) primarygroup (89939)     6073 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/README.md
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.752388 dopamine_rl-4.0.6/dopamine/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      619 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.753095 dopamine_rl-4.0.6/dopamine/agents/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.754419 dopamine_rl-4.0.6/dopamine/agents/dqn/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/dqn/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    22525 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.755973 dopamine_rl-4.0.6/dopamine/agents/implicit_quantile/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/implicit_quantile/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    14220 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/implicit_quantile/implicit_quantile_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.757586 dopamine_rl-4.0.6/dopamine/agents/rainbow/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/rainbow/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    21519 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/agents/rainbow/rainbow_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.759421 dopamine_rl-4.0.6/dopamine/colab/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/colab/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    10911 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/colab/utils.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.761180 dopamine_rl-4.0.6/dopamine/continuous_domains/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/continuous_domains/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    11511 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/continuous_domains/run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1673 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/continuous_domains/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.767172 dopamine_rl-4.0.6/dopamine/discrete_domains/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    19941 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/atari_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     8047 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/checkpointer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    15550 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/gym_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1646 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/iteration_statistics.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     8675 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/legacy_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3610 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/logger.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    29147 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1780 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/discrete_domains/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.769872 dopamine_rl-4.0.6/dopamine/jax/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.771002 dopamine_rl-4.0.6/dopamine/jax/agents/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.772207 dopamine_rl-4.0.6/dopamine/jax/agents/dqn/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/dqn/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    27400 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.773995 dopamine_rl-4.0.6/dopamine/jax/agents/full_rainbow/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/full_rainbow/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    16581 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.775730 dopamine_rl-4.0.6/dopamine/jax/agents/implicit_quantile/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/implicit_quantile/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    20492 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.778005 dopamine_rl-4.0.6/dopamine/jax/agents/quantile/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/quantile/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    12997 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/quantile/quantile_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.779876 dopamine_rl-4.0.6/dopamine/jax/agents/rainbow/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/rainbow/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    21157 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/rainbow/rainbow_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.781648 dopamine_rl-4.0.6/dopamine/jax/agents/sac/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/sac/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    26038 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/agents/sac/sac_agent.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     7310 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/continuous_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1757 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/losses.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    17304 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/jax/networks.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.782938 dopamine_rl-4.0.6/dopamine/labs/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.785883 dopamine_rl-4.0.6/dopamine/labs/atari_100k/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/atari_100k/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     6166 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/atari_100k/atari_100k_rainbow_agent.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     4836 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/atari_100k/eval_run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2818 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/atari_100k/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.786514 dopamine_rl-4.0.6/dopamine/labs/environments/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/environments/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.788424 dopamine_rl-4.0.6/dopamine/labs/environments/brax/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/environments/brax/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3764 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/environments/brax/brax_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1704 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/environments/brax/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.789697 dopamine_rl-4.0.6/dopamine/labs/environments/minatar/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/environments/minatar/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     5483 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/environments/minatar/minatar_env.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.791993 dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     5699 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/continuous_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     6992 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/deepmind_control_lib.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.795241 dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    10572 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    12156 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/tandem_dqn_agent.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1916 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.799136 dopamine_rl-4.0.6/dopamine/metrics/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      585 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2345 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/collector.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3675 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/collector_dispatcher.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2056 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/console_collector.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2057 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/pickle_collector.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)      869 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/statistics_instance.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1588 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/metrics/tensorboard_collector.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.802625 dopamine_rl-4.0.6/dopamine/replay_memory/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/replay_memory/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    38788 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/replay_memory/circular_replay_buffer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    14258 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/replay_memory/prioritized_replay_buffer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     6915 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/replay_memory/sum_tree.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.810531 dopamine_rl-4.0.6/dopamine/utils/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      602 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     4651 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/agent_visualizer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2320 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/atari_plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3889 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/bar_plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2671 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/example_viz.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    10811 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/example_viz_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     4047 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/line_plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3264 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1261 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/dopamine/utils/test_utils.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2022-09-21 20:18:34.813612 dopamine_rl-4.0.6/dopamine_rl.egg-info/
--rw-r--r--   0 psc      (160661) primarygroup (89939)     7564 2022-09-21 20:18:34.000000 dopamine_rl-4.0.6/dopamine_rl.egg-info/PKG-INFO
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3194 2022-09-21 20:18:34.000000 dopamine_rl-4.0.6/dopamine_rl.egg-info/SOURCES.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)        1 2022-09-21 20:18:34.000000 dopamine_rl-4.0.6/dopamine_rl.egg-info/dependency_links.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)      227 2022-09-21 20:18:34.000000 dopamine_rl-4.0.6/dopamine_rl.egg-info/requires.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)        9 2022-09-21 20:18:34.000000 dopamine_rl-4.0.6/dopamine_rl.egg-info/top_level.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)       38 2022-09-21 20:18:34.814870 dopamine_rl-4.0.6/setup.cfg
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3091 2022-09-21 17:38:26.000000 dopamine_rl-4.0.6/setup.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.708882 dopamine_rl-4.0.7/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      298 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/AUTHORS
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    11417 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/LICENSE
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     8009 2024-05-06 16:58:41.708598 dopamine_rl-4.0.7/PKG-INFO
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     6073 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/README.md
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.690804 dopamine_rl-4.0.7/dopamine/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      619 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.690983 dopamine_rl-4.0.7/dopamine/agents/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.691371 dopamine_rl-4.0.7/dopamine/agents/dqn/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/dqn/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    22347 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/dqn/dqn_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.691800 dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    13888 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/implicit_quantile_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.692258 dopamine_rl-4.0.7/dopamine/agents/rainbow/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/rainbow/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    21212 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/rainbow/rainbow_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.692681 dopamine_rl-4.0.7/dopamine/colab/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/colab/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    10872 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/colab/utils.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.693321 dopamine_rl-4.0.7/dopamine/continuous_domains/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/continuous_domains/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    11032 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/continuous_domains/run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1675 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/continuous_domains/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.695464 dopamine_rl-4.0.7/dopamine/discrete_domains/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    20405 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/atari_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     7830 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/checkpointer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    15458 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/gym_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1645 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/iteration_statistics.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     8414 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/legacy_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/logger.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    29226 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1782 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.696331 dopamine_rl-4.0.7/dopamine/jax/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.696529 dopamine_rl-4.0.7/dopamine/jax/agents/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.696885 dopamine_rl-4.0.7/dopamine/jax/agents/dqn/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/dqn/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    25694 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/dqn/dqn_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.697274 dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    17438 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.697693 dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    19224 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.698068 dopamine_rl-4.0.7/dopamine/jax/agents/quantile/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/quantile/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    12771 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/quantile/quantile_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.698482 dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    20026 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/rainbow_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.698842 dopamine_rl-4.0.7/dopamine/jax/agents/sac/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/sac/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    25998 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/sac/sac_agent.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     7293 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/continuous_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1670 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/losses.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    19671 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/networks.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.699097 dopamine_rl-4.0.7/dopamine/labs/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.700581 dopamine_rl-4.0.7/dopamine/labs/atari_100k/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    12279 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/atari_100k_rainbow_agent.py
+-rwxr-xr-x   0 psc      (160661) primarygroup (89939)    21090 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/atari_100k_runner.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     4783 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/eval_run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3546 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/normalization_utils.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    16018 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/spr_agent.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    14871 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/spr_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3664 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.700731 dopamine_rl-4.0.7/dopamine/labs/environments/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.701198 dopamine_rl-4.0.7/dopamine/labs/environments/brax/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/brax/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3858 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/brax/brax_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1705 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/brax/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.701641 dopamine_rl-4.0.7/dopamine/labs/environments/minatar/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/minatar/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     5406 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/minatar/minatar_env.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.702476 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     5615 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/continuous_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     7070 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/deepmind_control_lib.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.703445 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    10357 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    11705 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/tandem_dqn_agent.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1921 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.704591 dopamine_rl-4.0.7/dopamine/metrics/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2337 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/collector.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3683 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/collector_dispatcher.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2023 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/console_collector.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2054 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/pickle_collector.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      870 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/statistics_instance.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1592 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/tensorboard_collector.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.705347 dopamine_rl-4.0.7/dopamine/replay_memory/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    38593 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/circular_replay_buffer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    14059 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/prioritized_replay_buffer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     6895 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/sum_tree.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.706803 dopamine_rl-4.0.7/dopamine/utils/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     4604 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/agent_visualizer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2219 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/atari_plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3883 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/bar_plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2596 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/example_viz.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    10742 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/example_viz_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     4019 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/line_plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3239 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1268 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/test_utils.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.708205 dopamine_rl-4.0.7/dopamine_rl.egg-info/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     8009 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/PKG-INFO
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3367 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)        1 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      240 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/requires.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)        9 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/top_level.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)       38 2024-05-06 16:58:41.708944 dopamine_rl-4.0.7/setup.cfg
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3109 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/setup.py
```

### Comparing `dopamine_rl-4.0.6/LICENSE` & `dopamine_rl-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.6/PKG-INFO` & `dopamine_rl-4.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dopamine_rl
-Version: 4.0.6
+Version: 4.0.7
 Summary: Dopamine: A framework for flexible Reinforcement Learning research
 Home-page: https://github.com/google/dopamine
 Author: The Dopamine Team
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/dopamine
 Project-URL: Bug Reports, https://github.com/google/dopamine/issues
 Project-URL: Source, https://github.com/google/dopamine
 Keywords: dopamine,reinforcement,machine,learning,research
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -27,14 +26,29 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: tensorflow>=2.2.0
+Requires-Dist: gin-config>=0.3.0
+Requires-Dist: absl-py>=0.9.0
+Requires-Dist: opencv-python>=3.4.8.29
+Requires-Dist: gym<=0.25.2
+Requires-Dist: flax>=0.2.0
+Requires-Dist: jax>=0.1.72
+Requires-Dist: jaxlib>=0.1.51
+Requires-Dist: Pillow>=7.0.0
+Requires-Dist: numpy>=1.16.4
+Requires-Dist: pygame>=1.9.2
+Requires-Dist: pandas>=0.24.2
+Requires-Dist: tf_slim>=1.0
+Requires-Dist: tensorflow-probability>=0.13.0
+Requires-Dist: tqdm>=4.64.1
 
 # Dopamine
 [Getting Started](#getting-started) |
 [Docs][docs] |
 [Baseline Results][baselines] |
 [Changelist](https://google.github.io/dopamine/docs/changelist)
 
@@ -204,9 +218,7 @@
 [prioritized_replay]: https://arxiv.org/abs/1511.05952
 [c51]: http://proceedings.mlr.press/v70/bellemare17a.html
 [rainbow]: https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/download/17204/16680
 [iqn]: https://arxiv.org/abs/1806.06923
 [sac]: https://arxiv.org/abs/1812.05905
 [dopamine_paper]: https://arxiv.org/abs/1812.06110
 [vitualenv]: https://docs.python.org/3/library/venv.html#creating-virtual-environments
-
-
```

### Comparing `dopamine_rl-4.0.6/README.md` & `dopamine_rl-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.6/dopamine/__init__.py` & `dopamine_rl-4.0.7/dopamine/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.6/dopamine/agents/__init__.py` & `dopamine_rl-4.0.7/dopamine/agents/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/agents/dqn/__init__.py` & `dopamine_rl-4.0.7/dopamine/agents/dqn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/agents/dqn/dqn_agent.py` & `dopamine_rl-4.0.7/dopamine/agents/dqn/dqn_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from __future__ import print_function
 
 import math
 import os
 import random
 
 from absl import logging
-
 from dopamine.discrete_domains import atari_lib
 from dopamine.replay_memory import circular_replay_buffer
 import gin.tf
 import numpy as np
 import tensorflow as tf
 
 
@@ -55,57 +54,61 @@
     epsilon: float, the final value to which to decay the epsilon parameter.
 
   Returns:
     A float, the current epsilon value computed according to the schedule.
   """
   steps_left = decay_period + warmup_steps - step
   bonus = (1.0 - epsilon) * steps_left / decay_period
-  bonus = np.clip(bonus, 0., 1. - epsilon)
+  bonus = np.clip(bonus, 0.0, 1.0 - epsilon)
   return epsilon + bonus
 
 
 @gin.configurable
-def identity_epsilon(unused_decay_period, unused_step, unused_warmup_steps,
-                     epsilon):
+def identity_epsilon(
+    unused_decay_period, unused_step, unused_warmup_steps, epsilon
+):
   return epsilon
 
 
 @gin.configurable
 class DQNAgent(object):
   """An implementation of the DQN agent."""
 
-  def __init__(self,
-               sess,
-               num_actions,
-               observation_shape=atari_lib.NATURE_DQN_OBSERVATION_SHAPE,
-               observation_dtype=atari_lib.NATURE_DQN_DTYPE,
-               stack_size=atari_lib.NATURE_DQN_STACK_SIZE,
-               network=atari_lib.NatureDQNNetwork,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=20000,
-               update_period=4,
-               target_update_period=8000,
-               epsilon_fn=linearly_decaying_epsilon,
-               epsilon_train=0.01,
-               epsilon_eval=0.001,
-               epsilon_decay_period=250000,
-               tf_device='/cpu:*',
-               eval_mode=False,
-               use_staging=False,
-               max_tf_checkpoints_to_keep=4,
-               optimizer=tf.compat.v1.train.RMSPropOptimizer(
-                   learning_rate=0.00025,
-                   decay=0.95,
-                   momentum=0.0,
-                   epsilon=0.00001,
-                   centered=True),
-               summary_writer=None,
-               summary_writing_frequency=500,
-               allow_partial_reload=False):
+  def __init__(
+      self,
+      sess,
+      num_actions,
+      observation_shape=atari_lib.NATURE_DQN_OBSERVATION_SHAPE,
+      observation_dtype=atari_lib.NATURE_DQN_DTYPE,
+      stack_size=atari_lib.NATURE_DQN_STACK_SIZE,
+      network=atari_lib.NatureDQNNetwork,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=20000,
+      update_period=4,
+      target_update_period=8000,
+      epsilon_fn=linearly_decaying_epsilon,
+      epsilon_train=0.01,
+      epsilon_eval=0.001,
+      epsilon_decay_period=250000,
+      tf_device='/cpu:*',
+      eval_mode=False,
+      use_staging=False,
+      max_tf_checkpoints_to_keep=4,
+      optimizer=tf.compat.v1.train.RMSPropOptimizer(
+          learning_rate=0.00025,
+          decay=0.95,
+          momentum=0.0,
+          epsilon=0.00001,
+          centered=True,
+      ),
+      summary_writer=None,
+      summary_writing_frequency=500,
+      allow_partial_reload=False,
+  ):
     """Initializes the agent and constructs the components of its graph.
 
     Args:
       sess: `tf.compat.v1.Session`, for executing ops.
       num_actions: int, number of actions the agent can take at any state.
       observation_shape: tuple of ints describing the observation shape.
       observation_dtype: tf.DType, specifies the type of the observations. Note
@@ -119,54 +122,57 @@
       gamma: float, discount factor with the usual RL meaning.
       update_horizon: int, horizon at which updates are performed, the 'n' in
         n-step update.
       min_replay_history: int, number of transitions that should be experienced
         before the agent begins training its value function.
       update_period: int, period between DQN updates.
       target_update_period: int, update period for the target network.
-      epsilon_fn: function expecting 4 parameters:
-        (decay_period, step, warmup_steps, epsilon). This function should return
-        the epsilon value used for exploration during training.
+      epsilon_fn: function expecting 4 parameters: (decay_period, step,
+        warmup_steps, epsilon). This function should return the epsilon value
+        used for exploration during training.
       epsilon_train: float, the value to which the agent's epsilon is eventually
         decayed during training.
       epsilon_eval: float, epsilon used when evaluating the agent.
       epsilon_decay_period: int, length of the epsilon decay schedule.
       tf_device: str, Tensorflow device on which the agent's graph is executed.
       eval_mode: bool, True for evaluation and False for training.
       use_staging: bool, when True use a staging area to prefetch the next
         training batch, speeding training up by about 30%.
       max_tf_checkpoints_to_keep: int, the number of TensorFlow checkpoints to
         keep.
       optimizer: `tf.compat.v1.train.Optimizer`, for training the value
         function.
       summary_writer: SummaryWriter object for outputting training statistics.
-        Summary writing disabled if set to None.
-        May also be a str specifying the base directory, in which case the
-        SummaryWriter will be created by the agent.
+        Summary writing disabled if set to None. May also be a str specifying
+        the base directory, in which case the SummaryWriter will be created by
+        the agent.
       summary_writing_frequency: int, frequency with which summaries will be
         written. Lower values will result in slower training.
       allow_partial_reload: bool, whether we allow reloading a partial agent
         (for instance, only the network parameters).
     """
     assert isinstance(observation_shape, tuple)
-    logging.info('Creating %s agent with the following parameters:',
-                 self.__class__.__name__)
+    logging.info(
+        'Creating %s agent with the following parameters:',
+        self.__class__.__name__,
+    )
     logging.info('\t gamma: %f', gamma)
     logging.info('\t update_horizon: %f', update_horizon)
     logging.info('\t min_replay_history: %d', min_replay_history)
     logging.info('\t update_period: %d', update_period)
     logging.info('\t target_update_period: %d', target_update_period)
     logging.info('\t epsilon_train: %f', epsilon_train)
     logging.info('\t epsilon_eval: %f', epsilon_eval)
     logging.info('\t epsilon_decay_period: %d', epsilon_decay_period)
     logging.info('\t tf_device: %s', tf_device)
     logging.info('\t use_staging: %s', use_staging)
     logging.info('\t optimizer: %s', optimizer)
-    logging.info('\t max_tf_checkpoints_to_keep: %d',
-                 max_tf_checkpoints_to_keep)
+    logging.info(
+        '\t max_tf_checkpoints_to_keep: %d', max_tf_checkpoints_to_keep
+    )
 
     self.num_actions = num_actions
     self.observation_shape = tuple(observation_shape)
     self.observation_dtype = observation_dtype
     self.stack_size = stack_size
     self.network = network
     self.gamma = gamma
@@ -201,30 +207,33 @@
 
     with tf.device(tf_device):
       # Create a placeholder for the state input to the DQN network.
       # The last axis indicates the number of consecutive frames stacked.
       state_shape = (1,) + self.observation_shape + (stack_size,)
       self.state = np.zeros(state_shape)
       self.state_ph = tf.compat.v1.placeholder(
-          self.observation_dtype, state_shape, name='state_ph')
+          self.observation_dtype, state_shape, name='state_ph'
+      )
       self._replay = self._build_replay_buffer(use_staging)
 
       self._build_networks()
 
       self._train_op = self._build_train_op()
       self._sync_qt_ops = self._build_sync_op()
 
     if self.summary_writer is not None:
       # All tf.summaries should have been defined prior to running this.
       self._merged_summaries = tf.compat.v1.summary.merge_all()
 
     var_map = atari_lib.maybe_transform_variable_names(
-        tf.compat.v1.global_variables())
+        tf.compat.v1.global_variables()
+    )
     self._saver = tf.compat.v1.train.Saver(
-        var_list=var_map, max_to_keep=max_tf_checkpoints_to_keep)
+        var_list=var_map, max_to_keep=max_tf_checkpoints_to_keep
+    )
 
     # Variables to be initialized by the agent once it interacts with the
     # environment.
     self._observation = None
     self._last_observation = None
 
     if self.summary_writer is not None:
@@ -233,14 +242,15 @@
 
   def _create_network(self, name):
     """Builds the convolutional network used to compute the agent's Q-values.
 
     Args:
       name: str, this name is passed to the tf.keras.Model and used to create
         variable scope under the hood by the tf.keras.Model.
+
     Returns:
       network: tf.keras.Model, the network instantiated by the Keras model.
     """
     network = self.network(self.num_actions, name=name)
     return network
 
   def _build_networks(self):
@@ -264,15 +274,16 @@
     self._net_outputs = self.online_convnet(self.state_ph)
     # TODO(bellemare): Ties should be broken. They are unlikely to happen when
     # using a deep network, but may affect performance with a linear
     # approximation scheme.
     self._q_argmax = tf.argmax(self._net_outputs.q_values, axis=1)[0]
     self._replay_net_outputs = self.online_convnet(self._replay.states)
     self._replay_next_target_net_outputs = self.target_convnet(
-        self._replay.next_states)
+        self._replay.next_states
+    )
 
   def _build_replay_buffer(self, use_staging):
     """Creates the replay buffer used by the agent.
 
     Args:
       use_staging: bool, if True, uses a staging area to prefetch data for
         faster training.
@@ -282,51 +293,57 @@
     """
     return circular_replay_buffer.WrappedReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         use_staging=use_staging,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
-        observation_dtype=self.observation_dtype.as_numpy_dtype)
+        observation_dtype=self.observation_dtype.as_numpy_dtype,
+    )
 
   def _build_target_q_op(self):
     """Build an op used as a target for the Q-value.
 
     Returns:
       target_q_op: An op calculating the Q-value.
     """
     # Get the maximum Q-value across the actions dimension.
     replay_next_qt_max = tf.reduce_max(
-        self._replay_next_target_net_outputs.q_values, 1)
+        self._replay_next_target_net_outputs.q_values, 1
+    )
     # Calculate the Bellman target value.
     #   Q_t = R_t + \gamma^N * Q'_t+1
     # where,
     #   Q'_t+1 = \argmax_a Q(S_t+1, a)
     #          (or) 0 if S_t is a terminal state,
     # and
     #   N is the update horizon (by default, N=1).
     return self._replay.rewards + self.cumulative_gamma * replay_next_qt_max * (
-        1. - tf.cast(self._replay.terminals, tf.float32))
+        1.0 - tf.cast(self._replay.terminals, tf.float32)
+    )
 
   def _build_train_op(self):
     """Builds a training op.
 
     Returns:
       train_op: An op performing one step of training from replay data.
     """
     replay_action_one_hot = tf.one_hot(
-        self._replay.actions, self.num_actions, 1., 0., name='action_one_hot')
+        self._replay.actions, self.num_actions, 1.0, 0.0, name='action_one_hot'
+    )
     replay_chosen_q = tf.reduce_sum(
         self._replay_net_outputs.q_values * replay_action_one_hot,
         axis=1,
-        name='replay_chosen_q')
+        name='replay_chosen_q',
+    )
 
     target = tf.stop_gradient(self._build_target_q_op())
     loss = tf.compat.v1.losses.huber_loss(
-        target, replay_chosen_q, reduction=tf.losses.Reduction.NONE)
+        target, replay_chosen_q, reduction=tf.losses.Reduction.NONE
+    )
     if self.summary_writer is not None:
       with tf.compat.v1.variable_scope('Losses'):
         tf.compat.v1.summary.scalar('HuberLoss', tf.reduce_mean(loss))
     return self.optimizer.minimize(tf.reduce_mean(loss))
 
   def _build_sync_op(self):
     """Builds ops for assigning weights from online to target network.
@@ -335,20 +352,22 @@
       ops: A list of ops assigning weights from online to target network.
     """
     # Get trainable variables from online and target DQNs
     sync_qt_ops = []
     scope = tf.compat.v1.get_default_graph().get_name_scope()
     trainables_online = tf.compat.v1.get_collection(
         tf.compat.v1.GraphKeys.TRAINABLE_VARIABLES,
-        scope=os.path.join(scope, 'Online'))
+        scope=os.path.join(scope, 'Online'),
+    )
     trainables_target = tf.compat.v1.get_collection(
         tf.compat.v1.GraphKeys.TRAINABLE_VARIABLES,
-        scope=os.path.join(scope, 'Target'))
+        scope=os.path.join(scope, 'Target'),
+    )
 
-    for (w_online, w_target) in zip(trainables_online, trainables_target):
+    for w_online, w_target in zip(trainables_online, trainables_target):
       # Assign weights from online to target network.
       sync_qt_ops.append(w_target.assign(w_online, use_locking=True))
     return sync_qt_ops
 
   def begin_episode(self, observation):
     """Returns the agent's first action for this episode.
 
@@ -414,15 +433,16 @@
     if self.eval_mode:
       epsilon = self.epsilon_eval
     else:
       epsilon = self.epsilon_fn(
           self.epsilon_decay_period,
           self.training_steps,
           self.min_replay_history,
-          self.epsilon_train)
+          self.epsilon_train,
+      )
     if random.random() <= epsilon:
       # Choose a random action with probability epsilon.
       return random.randint(0, self.num_actions - 1)
     else:
       # Choose the action with highest Q-value at the current state.
       return self._sess.run(self._q_argmax, {self.state_ph: self.state})
 
@@ -437,17 +457,19 @@
     multiple of target update period.
     """
     # Run a train op at the rate of self.update_period if enough training steps
     # have been run. This matches the Nature DQN behaviour.
     if self._replay.memory.add_count > self.min_replay_history:
       if self.training_steps % self.update_period == 0:
         self._sess.run(self._train_op)
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
           summary = self._sess.run(self._merged_summaries)
           self.summary_writer.add_summary(summary, self.training_steps)
 
       if self.training_steps % self.target_update_period == 0:
         self._sess.run(self._sync_qt_ops)
 
     self.training_steps += 1
@@ -508,15 +530,16 @@
     """
     if not tf.io.gfile.exists(checkpoint_dir):
       return None
     # Call the Tensorflow saver to checkpoint the graph.
     self._saver.save(
         self._sess,
         os.path.join(checkpoint_dir, 'tf_ckpt'),
-        global_step=iteration_number)
+        global_step=iteration_number,
+    )
     # Checkpoint the out-of-graph replay buffer.
     self._replay.save(checkpoint_dir, iteration_number)
     bundle_dictionary = {}
     bundle_dictionary['state'] = self.state
     bundle_dictionary['training_steps'] = self.training_steps
     return bundle_dictionary
 
@@ -528,16 +551,16 @@
     checkpoint_dir. If the checkpoint_dir does not exist, will not reset the
       agent's state.
 
     Args:
       checkpoint_dir: str, path to the checkpoint saved by tf.Save.
       iteration_number: int, checkpoint version, used when restoring the replay
         buffer.
-      bundle_dictionary: dict, containing additional Python objects owned by
-        the agent.
+      bundle_dictionary: dict, containing additional Python objects owned by the
+        agent.
 
     Returns:
       bool, True if unbundling was successful.
     """
     try:
       # self._replay.load() will throw a NotFoundError if it does not find all
       # the necessary files.
@@ -552,11 +575,12 @@
         if key in bundle_dictionary:
           self.__dict__[key] = bundle_dictionary[key]
     elif not self.allow_partial_reload:
       return False
     else:
       logging.warning("Unable to reload the agent's parameters!")
     # Restore the agent's TensorFlow graph.
-    self._saver.restore(self._sess,
-                        os.path.join(checkpoint_dir,
-                                     'tf_ckpt-{}'.format(iteration_number)))
+    self._saver.restore(
+        self._sess,
+        os.path.join(checkpoint_dir, 'tf_ckpt-{}'.format(iteration_number)),
+    )
     return True
```

### Comparing `dopamine_rl-4.0.6/dopamine/agents/implicit_quantile/__init__.py` & `dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/agents/implicit_quantile/implicit_quantile_agent.py` & `dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/implicit_quantile_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,49 +30,51 @@
 import tensorflow as tf
 
 
 @gin.configurable
 class ImplicitQuantileAgent(rainbow_agent.RainbowAgent):
   """An extension of Rainbow to perform implicit quantile regression."""
 
-  def __init__(self,
-               sess,
-               num_actions,
-               network=atari_lib.ImplicitQuantileNetwork,
-               kappa=1.0,
-               num_tau_samples=32,
-               num_tau_prime_samples=32,
-               num_quantile_samples=32,
-               quantile_embedding_dim=64,
-               double_dqn=False,
-               summary_writer=None,
-               summary_writing_frequency=500):
+  def __init__(
+      self,
+      sess,
+      num_actions,
+      network=atari_lib.ImplicitQuantileNetwork,
+      kappa=1.0,
+      num_tau_samples=32,
+      num_tau_prime_samples=32,
+      num_quantile_samples=32,
+      quantile_embedding_dim=64,
+      double_dqn=False,
+      summary_writer=None,
+      summary_writing_frequency=500,
+  ):
     """Initializes the agent and constructs the Graph.
 
     Most of this constructor's parameters are IQN-specific hyperparameters whose
     values are taken from Dabney et al. (2018).
 
     Args:
       sess: `tf.compat.v1.Session` object for running associated ops.
       num_actions: int, number of actions the agent can take at any state.
-      network: tf.Keras.Model, expects three parameters:
-        (num_actions, quantile_embedding_dim, network_type). This class is used
-        to generate network instances that are used by the agent. Each
-        instantiation would have different set of variables. See
+      network: tf.Keras.Model, expects three parameters: (num_actions,
+        quantile_embedding_dim, network_type). This class is used to generate
+        network instances that are used by the agent. Each instantiation would
+        have different set of variables. See
         dopamine.discrete_domains.atari_lib.NatureDQNNetwork as an example.
       kappa: float, Huber loss cutoff.
       num_tau_samples: int, number of online quantile samples for loss
         estimation.
       num_tau_prime_samples: int, number of target quantile samples for loss
         estimation.
       num_quantile_samples: int, number of quantile samples for computing
         Q-values.
       quantile_embedding_dim: int, embedding dimension for the quantile input.
-      double_dqn: boolean, whether to perform double DQN style learning
-        as described in Van Hasselt et al.: https://arxiv.org/abs/1509.06461.
+      double_dqn: boolean, whether to perform double DQN style learning as
+        described in Van Hasselt et al.: https://arxiv.org/abs/1509.06461.
       summary_writer: SummaryWriter object for outputting training statistics.
         Summary writing disabled if set to None.
       summary_writing_frequency: int, frequency with which summaries will be
         written. Lower values will result in slower training.
     """
     self.kappa = kappa
     # num_tau_samples = N below equation (3) in the paper.
@@ -87,27 +89,30 @@
     self.double_dqn = double_dqn
 
     super(ImplicitQuantileAgent, self).__init__(
         sess=sess,
         num_actions=num_actions,
         network=network,
         summary_writer=summary_writer,
-        summary_writing_frequency=summary_writing_frequency)
+        summary_writing_frequency=summary_writing_frequency,
+    )
 
   def _create_network(self, name):
     r"""Builds an Implicit Quantile ConvNet.
 
     Args:
       name: str, this name is passed to the tf.keras.Model and used to create
         variable scope under the hood by the tf.keras.Model.
+
     Returns:
       network: tf.keras.Model, the network instantiated by the Keras model.
     """
-    network = self.network(self.num_actions, self.quantile_embedding_dim,
-                           name=name)
+    network = self.network(
+        self.num_actions, self.quantile_embedding_dim, name=name
+    )
     return network
 
   def _build_networks(self):
     """Builds the IQN computations needed for acting and training.
 
     These are:
       self.online_convnet: For computing the current state's quantile values.
@@ -120,115 +125,127 @@
         quantile values.
     """
     self.online_convnet = self._create_network(name='Online')
     self.target_convnet = self._create_network(name='Target')
 
     # Compute the Q-values which are used for action selection in the current
     # state.
-    self._net_outputs = self.online_convnet(self.state_ph,
-                                            self.num_quantile_samples)
+    self._net_outputs = self.online_convnet(
+        self.state_ph, self.num_quantile_samples
+    )
     # Shape of self._net_outputs.quantile_values:
     # num_quantile_samples x num_actions.
     # e.g. if num_actions is 2, it might look something like this:
     # Vals for Quantile .2  Vals for Quantile .4  Vals for Quantile .6
     #    [[0.1, 0.5],         [0.15, -0.3],          [0.15, -0.2]]
     # Q-values = [(0.1 + 0.15 + 0.15)/3, (0.5 + 0.15 + -0.2)/3].
     self._q_values = tf.reduce_mean(self._net_outputs.quantile_values, axis=0)
     self._q_argmax = tf.argmax(self._q_values, axis=0)
 
-    self._replay_net_outputs = self.online_convnet(self._replay.states,
-                                                   self.num_tau_samples)
+    self._replay_net_outputs = self.online_convnet(
+        self._replay.states, self.num_tau_samples
+    )
     # Shape: (num_tau_samples x batch_size) x num_actions.
     self._replay_net_quantile_values = self._replay_net_outputs.quantile_values
     self._replay_net_quantiles = self._replay_net_outputs.quantiles
 
     # Do the same for next states in the replay buffer.
     self._replay_net_target_outputs = self.target_convnet(
-        self._replay.next_states, self.num_tau_prime_samples)
+        self._replay.next_states, self.num_tau_prime_samples
+    )
     # Shape: (num_tau_prime_samples x batch_size) x num_actions.
     vals = self._replay_net_target_outputs.quantile_values
     self._replay_net_target_quantile_values = vals
 
     # Compute Q-values which are used for action selection for the next states
     # in the replay buffer. Compute the argmax over the Q-values.
     if self.double_dqn:
-      outputs_action = self.online_convnet(self._replay.next_states,
-                                           self.num_quantile_samples)
+      outputs_action = self.online_convnet(
+          self._replay.next_states, self.num_quantile_samples
+      )
     else:
-      outputs_action = self.target_convnet(self._replay.next_states,
-                                           self.num_quantile_samples)
+      outputs_action = self.target_convnet(
+          self._replay.next_states, self.num_quantile_samples
+      )
 
     # Shape: (num_quantile_samples x batch_size) x num_actions.
     target_quantile_values_action = outputs_action.quantile_values
     # Shape: num_quantile_samples x batch_size x num_actions.
-    target_quantile_values_action = tf.reshape(target_quantile_values_action,
-                                               [self.num_quantile_samples,
-                                                self._replay.batch_size,
-                                                self.num_actions])
+    target_quantile_values_action = tf.reshape(
+        target_quantile_values_action,
+        [self.num_quantile_samples, self._replay.batch_size, self.num_actions],
+    )
     # Shape: batch_size x num_actions.
-    self._replay_net_target_q_values = tf.squeeze(tf.reduce_mean(
-        target_quantile_values_action, axis=0))
+    self._replay_net_target_q_values = tf.squeeze(
+        tf.reduce_mean(target_quantile_values_action, axis=0)
+    )
     self._replay_next_qt_argmax = tf.argmax(
-        self._replay_net_target_q_values, axis=1)
+        self._replay_net_target_q_values, axis=1
+    )
 
   def _build_target_quantile_values_op(self):
     """Build an op used as a target for return values at given quantiles.
 
     Returns:
       An op calculating the target quantile return.
     """
     batch_size = tf.shape(self._replay.rewards)[0]
     # Shape of rewards: (num_tau_prime_samples x batch_size) x 1.
     rewards = self._replay.rewards[:, None]
     rewards = tf.tile(rewards, [self.num_tau_prime_samples, 1])
 
-    is_terminal_multiplier = 1. - tf.cast(self._replay.terminals, tf.float32)
+    is_terminal_multiplier = 1.0 - tf.cast(self._replay.terminals, tf.float32)
     # Incorporate terminal state to discount factor.
     # size of gamma_with_terminal: (num_tau_prime_samples x batch_size) x 1.
     gamma_with_terminal = self.cumulative_gamma * is_terminal_multiplier
-    gamma_with_terminal = tf.tile(gamma_with_terminal[:, None],
-                                  [self.num_tau_prime_samples, 1])
+    gamma_with_terminal = tf.tile(
+        gamma_with_terminal[:, None], [self.num_tau_prime_samples, 1]
+    )
 
     # Get the indices of the maximium Q-value across the action dimension.
     # Shape of replay_next_qt_argmax: (num_tau_prime_samples x batch_size) x 1.
 
     replay_next_qt_argmax = tf.tile(
-        self._replay_next_qt_argmax[:, None], [self.num_tau_prime_samples, 1])
+        self._replay_next_qt_argmax[:, None], [self.num_tau_prime_samples, 1]
+    )
 
     # Shape of batch_indices: (num_tau_prime_samples x batch_size) x 1.
-    batch_indices = tf.cast(tf.range(
-        self.num_tau_prime_samples * batch_size)[:, None], tf.int64)
+    batch_indices = tf.cast(
+        tf.range(self.num_tau_prime_samples * batch_size)[:, None], tf.int64
+    )
 
     # Shape of batch_indexed_target_values:
     # (num_tau_prime_samples x batch_size) x 2.
     batch_indexed_target_values = tf.concat(
-        [batch_indices, replay_next_qt_argmax], axis=1)
+        [batch_indices, replay_next_qt_argmax], axis=1
+    )
 
     # Shape of next_target_values: (num_tau_prime_samples x batch_size) x 1.
     target_quantile_values = tf.gather_nd(
-        self._replay_net_target_quantile_values,
-        batch_indexed_target_values)[:, None]
+        self._replay_net_target_quantile_values, batch_indexed_target_values
+    )[:, None]
 
     return rewards + gamma_with_terminal * target_quantile_values
 
   def _build_train_op(self):
     """Builds a training op.
 
     Returns:
       train_op: An op performing one step of training from replay data.
     """
     batch_size = tf.shape(self._replay.rewards)[0]
 
     target_quantile_values = tf.stop_gradient(
-        self._build_target_quantile_values_op())
+        self._build_target_quantile_values_op()
+    )
     # Reshape to self.num_tau_prime_samples x batch_size x 1 since this is
     # the manner in which the target_quantile_values are tiled.
-    target_quantile_values = tf.reshape(target_quantile_values,
-                                        [self.num_tau_prime_samples,
-                                         batch_size, 1])
+    target_quantile_values = tf.reshape(
+        target_quantile_values, [self.num_tau_prime_samples, batch_size, 1]
+    )
     # Transpose dimensions so that the dimensionality is batch_size x
     # self.num_tau_prime_samples x 1 to prepare for computation of
     # Bellman errors.
     # Final shape of target_quantile_values:
     # batch_size x num_tau_prime_samples x 1.
     target_quantile_values = tf.transpose(target_quantile_values, [1, 0, 2])
 
@@ -241,58 +258,76 @@
     # quantiles when using the tf.gather_nd function (see below).
     reshaped_actions = self._replay.actions[:, None]
     reshaped_actions = tf.tile(reshaped_actions, [self.num_tau_samples, 1])
     # Shape of reshaped_actions: (num_tau_samples x batch_size) x 2.
     reshaped_actions = tf.concat([indices, reshaped_actions], axis=1)
 
     chosen_action_quantile_values = tf.gather_nd(
-        self._replay_net_quantile_values, reshaped_actions)
+        self._replay_net_quantile_values, reshaped_actions
+    )
     # Reshape to self.num_tau_samples x batch_size x 1 since this is the manner
     # in which the quantile values are tiled.
-    chosen_action_quantile_values = tf.reshape(chosen_action_quantile_values,
-                                               [self.num_tau_samples,
-                                                batch_size, 1])
+    chosen_action_quantile_values = tf.reshape(
+        chosen_action_quantile_values, [self.num_tau_samples, batch_size, 1]
+    )
     # Transpose dimensions so that the dimensionality is batch_size x
     # self.num_tau_samples x 1 to prepare for computation of
     # Bellman errors.
     # Final shape of chosen_action_quantile_values:
     # batch_size x num_tau_samples x 1.
     chosen_action_quantile_values = tf.transpose(
-        chosen_action_quantile_values, [1, 0, 2])
+        chosen_action_quantile_values, [1, 0, 2]
+    )
 
     # Shape of bellman_erors and huber_loss:
     # batch_size x num_tau_prime_samples x num_tau_samples x 1.
-    bellman_errors = target_quantile_values[
-        :, :, None, :] - chosen_action_quantile_values[:, None, :, :]
+    bellman_errors = (
+        target_quantile_values[:, :, None, :]
+        - chosen_action_quantile_values[:, None, :, :]
+    )
     # The huber loss (see Section 2.3 of the paper) is defined via two cases:
     # case_one: |bellman_errors| <= kappa
     # case_two: |bellman_errors| > kappa
     huber_loss_case_one = (
-        tf.cast(tf.abs(bellman_errors) <= self.kappa, tf.float32) *
-        0.5 * bellman_errors ** 2)
+        tf.cast(tf.abs(bellman_errors) <= self.kappa, tf.float32)
+        * 0.5
+        * bellman_errors**2
+    )
     huber_loss_case_two = (
-        tf.cast(tf.abs(bellman_errors) > self.kappa, tf.float32) *
-        self.kappa * (tf.abs(bellman_errors) - 0.5 * self.kappa))
+        tf.cast(tf.abs(bellman_errors) > self.kappa, tf.float32)
+        * self.kappa
+        * (tf.abs(bellman_errors) - 0.5 * self.kappa)
+    )
     huber_loss = huber_loss_case_one + huber_loss_case_two
 
     # Reshape replay_quantiles to batch_size x num_tau_samples x 1
     replay_quantiles = tf.reshape(
-        self._replay_net_quantiles, [self.num_tau_samples, batch_size, 1])
+        self._replay_net_quantiles, [self.num_tau_samples, batch_size, 1]
+    )
     replay_quantiles = tf.transpose(replay_quantiles, [1, 0, 2])
 
     # Tile by num_tau_prime_samples along a new dimension. Shape is now
     # batch_size x num_tau_prime_samples x num_tau_samples x 1.
     # These quantiles will be used for computation of the quantile huber loss
     # below (see section 2.3 of the paper).
     replay_quantiles = tf.cast(
-        tf.tile(replay_quantiles[:, None, :, :],
-                [1, self.num_tau_prime_samples, 1, 1]), tf.float32)
+        tf.tile(
+            replay_quantiles[:, None, :, :],
+            [1, self.num_tau_prime_samples, 1, 1],
+        ),
+        tf.float32,
+    )
     # Shape: batch_size x num_tau_prime_samples x num_tau_samples x 1.
-    quantile_huber_loss = (tf.abs(replay_quantiles - tf.stop_gradient(
-        tf.cast(bellman_errors < 0, tf.float32))) * huber_loss) / self.kappa
+    quantile_huber_loss = (
+        tf.abs(
+            replay_quantiles
+            - tf.stop_gradient(tf.cast(bellman_errors < 0, tf.float32))
+        )
+        * huber_loss
+    ) / self.kappa
     # Sum over current quantile value (num_tau_samples) dimension,
     # average over target quantile value (num_tau_prime_samples) dimension.
     # Shape: batch_size x num_tau_prime_samples x 1.
     loss = tf.reduce_sum(quantile_huber_loss, axis=2)
     # Shape: batch_size x 1.
     loss = tf.reduce_mean(loss, axis=1)
```

### Comparing `dopamine_rl-4.0.6/dopamine/agents/rainbow/__init__.py` & `dopamine_rl-4.0.7/dopamine/agents/rainbow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/agents/rainbow/rainbow_agent.py` & `dopamine_rl-4.0.7/dopamine/agents/rainbow/rainbow_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,69 +46,72 @@
 import tensorflow as tf
 
 
 @gin.configurable
 class RainbowAgent(dqn_agent.DQNAgent):
   """A compact implementation of a simplified Rainbow agent."""
 
-  def __init__(self,
-               sess,
-               num_actions,
-               observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
-               observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
-               stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
-               network=atari_lib.RainbowNetwork,
-               num_atoms=51,
-               vmin=None,
-               vmax=10.,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=20000,
-               update_period=4,
-               target_update_period=8000,
-               epsilon_fn=dqn_agent.linearly_decaying_epsilon,
-               epsilon_train=0.01,
-               epsilon_eval=0.001,
-               epsilon_decay_period=250000,
-               replay_scheme='prioritized',
-               tf_device='/cpu:*',
-               use_staging=False,
-               optimizer=tf.compat.v1.train.AdamOptimizer(
-                   learning_rate=0.00025, epsilon=0.0003125),
-               summary_writer=None,
-               summary_writing_frequency=500):
+  def __init__(
+      self,
+      sess,
+      num_actions,
+      observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
+      observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
+      stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
+      network=atari_lib.RainbowNetwork,
+      num_atoms=51,
+      vmin=None,
+      vmax=10.0,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=20000,
+      update_period=4,
+      target_update_period=8000,
+      epsilon_fn=dqn_agent.linearly_decaying_epsilon,
+      epsilon_train=0.01,
+      epsilon_eval=0.001,
+      epsilon_decay_period=250000,
+      replay_scheme='prioritized',
+      tf_device='/cpu:*',
+      use_staging=False,
+      optimizer=tf.compat.v1.train.AdamOptimizer(
+          learning_rate=0.00025, epsilon=0.0003125
+      ),
+      summary_writer=None,
+      summary_writing_frequency=500,
+  ):
     """Initializes the agent and constructs the components of its graph.
 
     Args:
       sess: `tf.compat.v1.Session`, for executing ops.
       num_actions: int, number of actions the agent can take at any state.
       observation_shape: tuple of ints or an int. If single int, the observation
         is assumed to be a 2D square.
       observation_dtype: tf.DType, specifies the type of the observations. Note
         that if your inputs are continuous, you should set this to tf.float32.
       stack_size: int, number of frames to use in state stack.
-      network: tf.Keras.Model, expects four parameters:
-        (num_actions, num_atoms, support, network_type).  This class is used to
-        generate network instances that are used by the agent. Each
-        instantiation would have different set of variables. See
+      network: tf.Keras.Model, expects four parameters: (num_actions, num_atoms,
+        support, network_type).  This class is used to generate network
+        instances that are used by the agent. Each instantiation would have
+        different set of variables. See
         dopamine.discrete_domains.atari_lib.RainbowNetwork as an example.
       num_atoms: int, the number of buckets of the value function distribution.
       vmin: float, the value distribution support is [vmin, vmax]. If None, we
         set it to be -vmax.
       vmax: float, the value distribution support is [vmin, vmax].
       gamma: float, discount factor with the usual RL meaning.
       update_horizon: int, horizon at which updates are performed, the 'n' in
         n-step update.
       min_replay_history: int, number of transitions that should be experienced
         before the agent begins training its value function.
       update_period: int, period between DQN updates.
       target_update_period: int, update period for the target network.
-      epsilon_fn: function expecting 4 parameters:
-        (decay_period, step, warmup_steps, epsilon). This function should return
-        the epsilon value used for exploration during training.
+      epsilon_fn: function expecting 4 parameters: (decay_period, step,
+        warmup_steps, epsilon). This function should return the epsilon value
+        used for exploration during training.
       epsilon_train: float, the value to which the agent's epsilon is eventually
         decayed during training.
       epsilon_eval: float, epsilon used when evaluating the agent.
       epsilon_decay_period: int, length of the epsilon decay schedule.
       replay_scheme: str, 'prioritized' or 'uniform', the sampling scheme of the
         replay memory.
       tf_device: str, Tensorflow device on which the agent's graph is executed.
@@ -148,27 +151,30 @@
         epsilon_train=epsilon_train,
         epsilon_eval=epsilon_eval,
         epsilon_decay_period=epsilon_decay_period,
         tf_device=tf_device,
         use_staging=use_staging,
         optimizer=self.optimizer,
         summary_writer=summary_writer,
-        summary_writing_frequency=summary_writing_frequency)
+        summary_writing_frequency=summary_writing_frequency,
+    )
 
   def _create_network(self, name):
     """Builds a convolutional network that outputs Q-value distributions.
 
     Args:
       name: str, this name is passed to the tf.keras.Model and used to create
         variable scope under the hood by the tf.keras.Model.
+
     Returns:
       network: tf.keras.Model, the network instantiated by the Keras model.
     """
-    network = self.network(self.num_actions, self._num_atoms, self._support,
-                           name=name)
+    network = self.network(
+        self.num_actions, self._num_atoms, self._support, name=name
+    )
     return network
 
   def _build_replay_buffer(self, use_staging):
     """Creates the replay buffer used by the agent.
 
     Args:
       use_staging: bool, if True, uses a staging area to prefetch data for
@@ -186,15 +192,16 @@
     # sets all priorities to the same value (which yields uniform sampling).
     return prioritized_replay_buffer.WrappedPrioritizedReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         use_staging=use_staging,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
-        observation_dtype=self.observation_dtype.as_numpy_dtype)
+        observation_dtype=self.observation_dtype.as_numpy_dtype,
+    )
 
   def _build_target_distribution(self):
     """Builds the C51 target distribution as per Bellemare et al. (2017).
 
     First, we compute the support of the Bellman target, r + gamma Z'. Where Z'
     is the support of the next state distribution:
 
@@ -217,57 +224,62 @@
 
     # size of tiled_support: batch_size x num_atoms
     tiled_support = tf.tile(self._support, [batch_size])
     tiled_support = tf.reshape(tiled_support, [batch_size, self._num_atoms])
 
     # size of target_support: batch_size x num_atoms
 
-    is_terminal_multiplier = 1. - tf.cast(self._replay.terminals, tf.float32)
+    is_terminal_multiplier = 1.0 - tf.cast(self._replay.terminals, tf.float32)
     # Incorporate terminal state to discount factor.
     # size of gamma_with_terminal: batch_size x 1
     gamma_with_terminal = self.cumulative_gamma * is_terminal_multiplier
     gamma_with_terminal = gamma_with_terminal[:, None]
 
     target_support = rewards + gamma_with_terminal * tiled_support
 
     # size of next_qt_argmax: 1 x batch_size
     next_qt_argmax = tf.argmax(
-        self._replay_next_target_net_outputs.q_values, axis=1)[:, None]
+        self._replay_next_target_net_outputs.q_values, axis=1
+    )[:, None]
     batch_indices = tf.range(tf.cast(batch_size, tf.int64))[:, None]
     # size of next_qt_argmax: batch_size x 2
     batch_indexed_next_qt_argmax = tf.concat(
-        [batch_indices, next_qt_argmax], axis=1)
+        [batch_indices, next_qt_argmax], axis=1
+    )
 
     # size of next_probabilities: batch_size x num_atoms
     next_probabilities = tf.gather_nd(
         self._replay_next_target_net_outputs.probabilities,
-        batch_indexed_next_qt_argmax)
+        batch_indexed_next_qt_argmax,
+    )
 
-    return project_distribution(target_support, next_probabilities,
-                                self._support)
+    return project_distribution(
+        target_support, next_probabilities, self._support
+    )
 
   def _build_train_op(self):
     """Builds a training op.
 
     Returns:
       train_op: An op performing one step of training from replay data.
     """
     target_distribution = tf.stop_gradient(self._build_target_distribution())
 
     # size of indices: batch_size x 1.
     indices = tf.range(tf.shape(self._replay_net_outputs.logits)[0])[:, None]
     # size of reshaped_actions: batch_size x 2.
     reshaped_actions = tf.concat([indices, self._replay.actions[:, None]], 1)
     # For each element of the batch, fetch the logits for its selected action.
-    chosen_action_logits = tf.gather_nd(self._replay_net_outputs.logits,
-                                        reshaped_actions)
+    chosen_action_logits = tf.gather_nd(
+        self._replay_net_outputs.logits, reshaped_actions
+    )
 
     loss = tf.nn.softmax_cross_entropy_with_logits(
-        labels=target_distribution,
-        logits=chosen_action_logits)
+        labels=target_distribution, logits=chosen_action_logits
+    )
 
     if self._replay_scheme == 'prioritized':
       # The original prioritized experience replay uses a linear exponent
       # schedule 0.4 -> 1.0. Comparing the schedule to a fixed exponent of 0.5
       # on 5 games (Asterix, Pong, Q*Bert, Seaquest, Space Invaders) suggested
       # a fixed exponent actually performs better, except on Pong.
       probs = self._replay.transition['sampling_probabilities']
@@ -278,15 +290,16 @@
       # but in both cases it is set to 0.5 - for simplicity's sake we leave it
       # as is here, using the more direct tf.sqrt(). Taking the square root
       # "makes sense", as we are dealing with a squared loss.
       # Add a small nonzero value to the loss to avoid 0 priority items. While
       # technically this may be okay, setting all items to 0 priority will cause
       # troubles, and also result in 1.0 / 0.0 = NaN correction terms.
       update_priorities_op = self._replay.tf_set_priority(
-          self._replay.indices, tf.sqrt(loss + 1e-10))
+          self._replay.indices, tf.sqrt(loss + 1e-10)
+      )
 
       # Weight the loss by the inverse priorities.
       loss = loss_weights * loss
     else:
       update_priorities_op = tf.no_op()
 
     with tf.control_dependencies([update_priorities_op]):
@@ -294,20 +307,17 @@
         with tf.compat.v1.variable_scope('Losses'):
           tf.compat.v1.summary.scalar('CrossEntropyLoss', tf.reduce_mean(loss))
       # Schaul et al. reports a slightly different rule, where 1/N is also
       # exponentiated by beta. Not doing so seems more reasonable, and did not
       # impact performance in our experiments.
       return self.optimizer.minimize(tf.reduce_mean(loss)), loss
 
-  def _store_transition(self,
-                        last_observation,
-                        action,
-                        reward,
-                        is_terminal,
-                        priority=None):
+  def _store_transition(
+      self, last_observation, action, reward, is_terminal, priority=None
+  ):
     """Stores a transition when in training mode.
 
     Executes a tf session and executes replay buffer ops in order to store the
     following tuple in the replay buffer (last_observation, action, reward,
     is_terminal, priority).
 
     Args:
@@ -319,24 +329,25 @@
       priority: Float. Priority of sampling the transition. If None, the default
         priority will be used. If replay scheme is uniform, the default priority
         is 1. If the replay scheme is prioritized, the default priority is the
         maximum ever seen [Schaul et al., 2015].
     """
     if priority is None:
       if self._replay_scheme == 'uniform':
-        priority = 1.
+        priority = 1.0
       else:
         priority = self._replay.memory.sum_tree.max_recorded_priority
 
     if not self.eval_mode:
       self._replay.add(last_observation, action, reward, is_terminal, priority)
 
 
-def project_distribution(supports, weights, target_support,
-                         validate_args=False):
+def project_distribution(
+    supports, weights, target_support, validate_args=False
+):
   """Projects a batch of (support, weights) onto target_support.
 
   Based on equation (7) in (Bellemare et al., 2017):
     https://arxiv.org/abs/1707.06887
   In the rest of the comments we will refer to this equation simply as Eq7.
 
   This code is not easy to digest, so we will use a running example to clarify
@@ -357,16 +368,16 @@
     weights: Tensor of shape (batch_size, num_dims) defining weights on the
       original support points. Although for the CategoricalDQN agent these
       weights are probabilities, it is not required that they are.
     target_support: Tensor of shape (num_dims) defining support of the projected
       distribution. The values must be monotonically increasing. Vmin and Vmax
       will be inferred from the first and last elements of this tensor,
       respectively. The values in this tensor must be equally spaced.
-    validate_args: Whether we will verify the contents of the
-      target_support parameter.
+    validate_args: Whether we will verify the contents of the target_support
+      parameter.
 
   Returns:
     A Tensor of shape (batch_size, num_dims) with the projection of a batch of
     (support, weights) onto target_support.
 
   Raises:
     ValueError: If target_support has no dimensions, or if shapes of supports,
@@ -380,33 +391,43 @@
   supports[0].shape.assert_is_compatible_with(target_support.shape)
   target_support.shape.assert_has_rank(1)
   if validate_args:
     # Assert that supports and weights have the same shapes.
     validate_deps.append(
         tf.Assert(
             tf.reduce_all(tf.equal(tf.shape(supports), tf.shape(weights))),
-            [supports, weights]))
+            [supports, weights],
+        )
+    )
     # Assert that elements of supports and target_support have the same shape.
     validate_deps.append(
         tf.Assert(
             tf.reduce_all(
-                tf.equal(tf.shape(supports)[1], tf.shape(target_support))),
-            [supports, target_support]))
+                tf.equal(tf.shape(supports)[1], tf.shape(target_support))
+            ),
+            [supports, target_support],
+        )
+    )
     # Assert that target_support has a single dimension.
     validate_deps.append(
         tf.Assert(
-            tf.equal(tf.size(tf.shape(target_support)), 1), [target_support]))
+            tf.equal(tf.size(tf.shape(target_support)), 1), [target_support]
+        )
+    )
     # Assert that the target_support is monotonically increasing.
     validate_deps.append(
-        tf.Assert(tf.reduce_all(target_support_deltas > 0), [target_support]))
+        tf.Assert(tf.reduce_all(target_support_deltas > 0), [target_support])
+    )
     # Assert that the values in target_support are equally spaced.
     validate_deps.append(
         tf.Assert(
             tf.reduce_all(tf.equal(target_support_deltas, delta_z)),
-            [target_support]))
+            [target_support],
+        )
+    )
 
   with tf.control_dependencies(validate_deps):
     # Ex: `v_min, v_max = 4, 8`.
     v_min, v_max = target_support[0], target_support[-1]
     # Ex: `batch_size = 2`.
     batch_size = tf.shape(supports)[0]
     # `N` in Eq7.
@@ -434,16 +455,17 @@
     #                                  [ 8.]]
     #                                 [[ 4.]
     #                                  [ 5.]
     #                                  [ 6.]
     #                                  [ 7.]
     #                                  [ 8.]]]`.
     reshaped_target_support = tf.tile(target_support[:, None], [batch_size, 1])
-    reshaped_target_support = tf.reshape(reshaped_target_support,
-                                         [batch_size, num_dims, 1])
+    reshaped_target_support = tf.reshape(
+        reshaped_target_support, [batch_size, num_dims, 1]
+    )
     # numerator = `|clipped_support - z_i|` in Eq7.
     # Ex: `numerator = [[[[ 0.  0.  0.  2.  4.]
     #                     [ 1.  1.  1.  1.  3.]
     #                     [ 2.  2.  2.  0.  2.]
     #                     [ 3.  3.  3.  1.  1.]
     #                     [ 4.  4.  4.  2.  0.]]
     #                    [[ 0.  0.  0.  1.  2.]
```

### Comparing `dopamine_rl-4.0.6/dopamine/colab/__init__.py` & `dopamine_rl-4.0.7/dopamine/colab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/colab/utils.py` & `dopamine_rl-4.0.7/dopamine/colab/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,33 +22,81 @@
 import pickle
 import sys
 
 
 
 import numpy as np
 import pandas as pd
-
 import tensorflow as tf
 
 FILE_PREFIX = 'log'
 ITERATION_PREFIX = 'iteration_'
 
-ALL_GAMES = ['AirRaid', 'Alien', 'Amidar', 'Assault', 'Asterix', 'Asteroids',
-             'Atlantis', 'BankHeist', 'BattleZone', 'BeamRider', 'Berzerk',
-             'Bowling', 'Boxing', 'Breakout', 'Carnival', 'Centipede',
-             'ChopperCommand', 'CrazyClimber', 'DemonAttack', 'DoubleDunk',
-             'ElevatorAction', 'Enduro', 'FishingDerby', 'Freeway', 'Frostbite',
-             'Gopher', 'Gravitar', 'Hero', 'IceHockey', 'Jamesbond',
-             'JourneyEscape', 'Kangaroo', 'Krull', 'KungFuMaster',
-             'MontezumaRevenge', 'MsPacman', 'NameThisGame', 'Phoenix',
-             'Pitfall', 'Pong', 'Pooyan', 'PrivateEye', 'Qbert', 'Riverraid',
-             'RoadRunner', 'Robotank', 'Seaquest', 'Skiing', 'Solaris',
-             'SpaceInvaders', 'StarGunner', 'Tennis', 'TimePilot', 'Tutankham',
-             'UpNDown', 'Venture', 'VideoPinball', 'WizardOfWor', 'YarsRevenge',
-             'Zaxxon']
+ALL_GAMES = [
+    'AirRaid',
+    'Alien',
+    'Amidar',
+    'Assault',
+    'Asterix',
+    'Asteroids',
+    'Atlantis',
+    'BankHeist',
+    'BattleZone',
+    'BeamRider',
+    'Berzerk',
+    'Bowling',
+    'Boxing',
+    'Breakout',
+    'Carnival',
+    'Centipede',
+    'ChopperCommand',
+    'CrazyClimber',
+    'DemonAttack',
+    'DoubleDunk',
+    'ElevatorAction',
+    'Enduro',
+    'FishingDerby',
+    'Freeway',
+    'Frostbite',
+    'Gopher',
+    'Gravitar',
+    'Hero',
+    'IceHockey',
+    'Jamesbond',
+    'JourneyEscape',
+    'Kangaroo',
+    'Krull',
+    'KungFuMaster',
+    'MontezumaRevenge',
+    'MsPacman',
+    'NameThisGame',
+    'Phoenix',
+    'Pitfall',
+    'Pong',
+    'Pooyan',
+    'PrivateEye',
+    'Qbert',
+    'Riverraid',
+    'RoadRunner',
+    'Robotank',
+    'Seaquest',
+    'Skiing',
+    'Solaris',
+    'SpaceInvaders',
+    'StarGunner',
+    'Tennis',
+    'TimePilot',
+    'Tutankham',
+    'UpNDown',
+    'Venture',
+    'VideoPinball',
+    'WizardOfWor',
+    'YarsRevenge',
+    'Zaxxon',
+]
 MUJOCO_GAMES = ['Ant', 'HalfCheetah', 'Hopper', 'Humanoid', 'Walker2d']
 
 
 def load_baselines(base_dir, verbose=False):
   """Reads in the baseline experimental data from a specified base directory.
 
   Args:
@@ -61,16 +109,17 @@
   experimental_data = {}
   for game in ALL_GAMES:
     for agent in ['dqn', 'c51', 'rainbow', 'iqn']:
       game_data_file = os.path.join(base_dir, agent, '{}.pkl'.format(game))
       if not tf.io.gfile.exists(game_data_file):
         if verbose:
           # pylint: disable=superfluous-parens
-          print('Unable to load data for agent {} on game {}'.format(agent,
-                                                                     game))
+          print(
+              'Unable to load data for agent {} on game {}'.format(agent, game)
+          )
           # pylint: enable=superfluous-parens
         continue
       with tf.io.gfile.GFile(game_data_file, 'rb') as f:
         if sys.version_info.major >= 3:
           # pylint: disable=unexpected-keyword-arg
           single_agent_data = pickle.load(f, encoding='latin1')
           # pylint: enable=unexpected-keyword-arg
@@ -78,34 +127,36 @@
           single_agent_data = pickle.load(f)
         single_agent_data['agent'] = agent
         # The dataframe rows are all read as 'objects', which causes a
         # ValueError when merging below. We cast the numerics to float64s to
         # avoid this.
         for field_name in single_agent_data.keys():
           try:
-            single_agent_data[field_name] = (
-                single_agent_data[field_name].astype(np.float64))
+            single_agent_data[field_name] = single_agent_data[
+                field_name
+            ].astype(np.float64)
           except ValueError:
             # This will catch any non-numerics that cannot be cast to float64.
             continue
         if game in experimental_data:
           experimental_data[game] = experimental_data[game].merge(
-              single_agent_data, how='outer')
+              single_agent_data, how='outer'
+          )
         else:
           experimental_data[game] = single_agent_data
   return experimental_data
 
 
 def load_statistics(log_path, iteration_number=None, verbose=True):
   """Reads in a statistics object from log_path.
 
   Args:
     log_path: string, provides the full path to the training/eval statistics.
-    iteration_number: The iteration number of the statistics object we want
-      to read. If set to None, load the latest version.
+    iteration_number: The iteration number of the statistics object we want to
+      read. If set to None, load the latest version.
     verbose: Whether to output information about the load procedure.
 
   Returns:
     data: The requested statistics object.
     iteration: The corresponding iteration number.
 
   Raises:
@@ -157,15 +208,15 @@
   glob = os.path.join(path, '{}_[0-9]*'.format(FILE_PREFIX))
   log_files = tf.io.gfile.glob(glob)
 
   if not log_files:
     raise ValueError('No log data found at {}'.format(path))
 
   def extract_iteration(x):
-    return int(x[x.rfind('_') + 1:])
+    return int(x[x.rfind('_') + 1 :])
 
   latest_iteration = max(extract_iteration(x) for x in log_files)
   return latest_iteration
 
 
 def summarize_data(data, summary_keys):
   """Processes log data into a per-iteration summary.
@@ -198,21 +249,22 @@
       if iter_key in data:
         current_value = np.mean(data[iter_key][key])
       summary[key].append(current_value)
 
   return summary
 
 
-def read_experiment(log_path,
-                    parameter_set=None,
-                    job_descriptor='',
-                    iteration_number=None,
-                    summary_keys=('train_episode_returns',
-                                  'eval_episode_returns'),
-                    verbose=False):
+def read_experiment(
+    log_path,
+    parameter_set=None,
+    job_descriptor='',
+    iteration_number=None,
+    summary_keys=('train_episode_returns', 'eval_episode_returns'),
+    verbose=False,
+):
   """Reads in a set of experimental results from log_path.
 
   The provided parameter_set is an ordered_dict which
     1) defines the parameters of this experiment,
     2) defines the order in which they occur in the job descriptor.
 
   The method reads all experiments of the form
@@ -253,40 +305,46 @@
 
   column_names = keys + ['iteration'] + list(summary_keys)
   num_parameter_settings = len([_ for _ in itertools.product(*ordered_values)])
   expected_num_iterations = 200
   expected_num_rows = num_parameter_settings * expected_num_iterations
 
   # Create DataFrame with predicted number of rows.
-  data_frame = pd.DataFrame(index=np.arange(0, expected_num_rows),
-                            columns=column_names)
+  data_frame = pd.DataFrame(
+      index=np.arange(0, expected_num_rows), columns=column_names
+  )
   row_index = 0
 
   # Now take their cross product. This generates tuples of the form
   # (p1, p2, p3, ...) where p1, p2, p3 are parameter values for the first,
   # second, etc. parameters as ordered in value_set.
   for parameter_tuple in itertools.product(*ordered_values):
     if job_descriptor is not None:
       name = job_descriptor.format(*parameter_tuple)
     else:
       # Construct name for values.
-      name = '-'.join([keys[i] + '_' + str(parameter_tuple[i])
-                       for i in range(len(keys))])
+      name = '-'.join(
+          [keys[i] + '_' + str(parameter_tuple[i]) for i in range(len(keys))]
+      )
 
     experiment_path = '{}/{}/logs'.format(log_path, name)
 
     raw_data, last_iteration = load_statistics(
-        experiment_path, iteration_number=iteration_number, verbose=verbose)
+        experiment_path, iteration_number=iteration_number, verbose=verbose
+    )
 
     summary = summarize_data(raw_data, summary_keys)
     for iteration in range(last_iteration + 1):
       # The row contains all the parameters, the iteration, and finally the
       # requested values.
-      row_data = (list(parameter_tuple) + [iteration] +
-                  [summary[key][iteration] for key in summary_keys])
+      row_data = (
+          list(parameter_tuple)
+          + [iteration]
+          + [summary[key][iteration] for key in summary_keys]
+      )
       data_frame.loc[row_index] = row_data
 
       row_index += 1
 
   # The dataframe rows are all read as 'objects', which causes a
   # ValueError when merging below. We cast the numerics to float64s to
   # avoid this.
```

### Comparing `dopamine_rl-4.0.6/dopamine/continuous_domains/__init__.py` & `dopamine_rl-4.0.7/dopamine/continuous_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.6/dopamine/continuous_domains/run_experiment.py` & `dopamine_rl-4.0.7/dopamine/continuous_domains/run_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,42 +36,45 @@
 load_gin_configs = base_run_experiment.load_gin_configs
 
 
 @gin.configurable
 def create_continuous_agent(
     environment: gym_lib.GymPreprocessing,
     agent_name: str,
-    summary_writer: Optional[tensorboard.SummaryWriter] = None
+    summary_writer: Optional[tensorboard.SummaryWriter] = None,
 ) -> dqn_agent.JaxDQNAgent:
   """Creates an agent.
 
   Args:
     environment:  A gym environment.
     agent_name: str, name of the agent to create.
-    summary_writer: A Tensorflow summary writer to pass to the agent
-      for in-agent training statistics in Tensorboard.
+    summary_writer: A Tensorflow summary writer to pass to the agent for
+      in-agent training statistics in Tensorboard.
 
   Returns:
     An RL agent.
 
   Raises:
     ValueError: If `agent_name` is not in supported list.
   """
   assert agent_name is not None
   if agent_name == 'sac':
     assert isinstance(environment.action_space, spaces.Box)
     assert isinstance(environment.observation_space, spaces.Box)
     return sac_agent.SACAgent(
         action_shape=environment.action_space.shape,
-        action_limits=(environment.action_space.low,
-                       environment.action_space.high),
+        action_limits=(
+            environment.action_space.low,
+            environment.action_space.high,
+        ),
         observation_shape=environment.observation_space.shape,
         action_dtype=environment.action_space.dtype,
         observation_dtype=environment.observation_space.dtype,
-        summary_writer=summary_writer)
+        summary_writer=summary_writer,
+    )
   else:
     raise ValueError(f'Unknown agent: {agent_name}')
 
 
 @gin.configurable
 def create_continuous_runner(base_dir, schedule='continuous_train_and_eval'):
   """Creates an experiment Runner.
@@ -101,27 +104,29 @@
 class ContinuousRunner(base_run_experiment.Runner):
   """Object that handles running Dopamine experiments.
 
   This is mostly the same as discrete_domains.Runner, but is written solely for
   JAX/Flax agents.
   """
 
-  def __init__(self,
-               base_dir,
-               create_agent_fn,
-               create_environment_fn=gym_lib.create_gym_environment,
-               checkpoint_file_prefix='ckpt',
-               logging_file_prefix='log',
-               log_every_n=1,
-               num_iterations=200,
-               training_steps=250000,
-               evaluation_steps=125000,
-               max_steps_per_episode=1000,
-               clip_rewards=False,
-               use_legacy_logger=True):
+  def __init__(
+      self,
+      base_dir,
+      create_agent_fn,
+      create_environment_fn=gym_lib.create_gym_environment,
+      checkpoint_file_prefix='ckpt',
+      logging_file_prefix='log',
+      log_every_n=1,
+      num_iterations=200,
+      training_steps=250000,
+      evaluation_steps=125000,
+      max_steps_per_episode=1000,
+      clip_rewards=False,
+      use_legacy_logger=True,
+  ):
     """Initialize the Runner object in charge of running a full experiment.
 
     Args:
       base_dir: str, the base directory to host all required sub-directories.
       create_agent_fn: A function that takes as argument an environment, and
         returns an agent.
       create_environment_fn: A function which receives a problem name and
@@ -155,23 +160,26 @@
     self._evaluation_steps = evaluation_steps
     self._max_steps_per_episode = max_steps_per_episode
     self._base_dir = base_dir
     self._clip_rewards = clip_rewards
     self._create_directories()
     self._summary_writer = tensorboard.SummaryWriter(base_dir)
     self._environment = create_environment_fn()
-    self._agent = create_agent_fn(self._environment,
-                                  summary_writer=self._summary_writer)
+    self._agent = create_agent_fn(
+        self._environment, summary_writer=self._summary_writer
+    )
     self._initialize_checkpointer_and_maybe_resume(checkpoint_file_prefix)
 
     # Create a collector dispatcher for metrics reporting.
     self._collector_dispatcher = collector_dispatcher.CollectorDispatcher(
-        self._base_dir)
+        self._base_dir
+    )
     set_collector_dispatcher_fn = getattr(
-        self._agent, 'set_collector_dispatcher', None)
+        self._agent, 'set_collector_dispatcher', None
+    )
     if callable(set_collector_dispatcher_fn):
       set_collector_dispatcher_fn(self._collector_dispatcher)
 
   @property
   def _use_legacy_logger(self):
     if not hasattr(self, '_legacy_logger_enabled'):
       return True
@@ -185,50 +193,59 @@
 
   @property
   def _fine_grained_print_to_console(self):
     if not hasattr(self, '_fine_grained_print_to_console_enabled'):
       return True
     return self._fine_grained_print_to_console_enabled
 
-  def _save_tensorboard_summaries(self, iteration,
-                                  num_episodes_train,
-                                  average_reward_train,
-                                  num_episodes_eval,
-                                  average_reward_eval,
-                                  average_steps_per_second):
+  def _save_tensorboard_summaries(
+      self,
+      iteration,
+      num_episodes_train,
+      average_reward_train,
+      num_episodes_eval,
+      average_reward_eval,
+      average_steps_per_second,
+  ):
     """Save statistics as tensorboard summaries.
 
     Args:
       iteration: int, The current iteration number.
       num_episodes_train: int, number of training episodes run.
       average_reward_train: float, The average training reward.
       num_episodes_eval: int, number of evaluation episodes run.
       average_reward_eval: float, The average evaluation reward.
       average_steps_per_second: float, The average number of steps per second.
     """
-    metrics = [('Train/NumEpisodes', num_episodes_train),
-               ('Train/AverageReturns', average_reward_train),
-               ('Train/AverageStepsPerSecond', average_steps_per_second),
-               ('Eval/NumEpisodes', num_episodes_eval),
-               ('Eval/AverageReturns', average_reward_eval)]
+    metrics = [
+        ('Train/NumEpisodes', num_episodes_train),
+        ('Train/AverageReturns', average_reward_train),
+        ('Train/AverageStepsPerSecond', average_steps_per_second),
+        ('Eval/NumEpisodes', num_episodes_eval),
+        ('Eval/AverageReturns', average_reward_eval),
+    ]
     for name, value in metrics:
       self._summary_writer.scalar(name, value, iteration)
     self._summary_writer.flush()
 
 
 @gin.configurable
 class ContinuousTrainRunner(ContinuousRunner):
   """Object that handles running experiments.
 
   This is mostly the same as discrete_domains.TrainRunner, but is written solely
   for JAX/Flax agents.
   """
 
-  def __init__(self, base_dir, create_agent_fn,
-               create_environment_fn=gym_lib.create_gym_environment):
+  def __init__(
+      self,
+      base_dir,
+      create_agent_fn,
+      create_environment_fn=gym_lib.create_gym_environment,
+  ):
     """Initialize the TrainRunner object in charge of running a full experiment.
 
     Args:
       base_dir: str, the base directory to host all required sub-directories.
       create_agent_fn: A function that takes as args a Tensorflow session and an
         environment, and returns an agent.
       create_environment_fn: A function which receives a problem name and
@@ -250,35 +267,42 @@
         Tensorboard summaries.
 
     Returns:
       A dict containing summary statistics for this iteration.
     """
     statistics = iteration_statistics.IterationStatistics()
     num_episodes_train, average_reward_train, average_steps_per_second = (
-        self._run_train_phase(statistics))
+        self._run_train_phase(statistics)
+    )
 
     if self._has_collector_dispatcher:
       self._collector_dispatcher.write([
-          statistics_instance.StatisticsInstance('Train/NumEpisodes',
-                                                 num_episodes_train,
-                                                 iteration),
-          statistics_instance.StatisticsInstance('Train/AverageReturns',
-                                                 average_reward_train,
-                                                 iteration),
-          statistics_instance.StatisticsInstance('Train/AverageStepsPerSecond',
-                                                 average_steps_per_second,
-                                                 iteration),
+          statistics_instance.StatisticsInstance(
+              'Train/NumEpisodes', num_episodes_train, iteration
+          ),
+          statistics_instance.StatisticsInstance(
+              'Train/AverageReturns', average_reward_train, iteration
+          ),
+          statistics_instance.StatisticsInstance(
+              'Train/AverageStepsPerSecond', average_steps_per_second, iteration
+          ),
       ])
-    self._save_tensorboard_summaries(iteration, num_episodes_train,
-                                     average_reward_train,
-                                     average_steps_per_second)
+    self._save_tensorboard_summaries(
+        iteration,
+        num_episodes_train,
+        average_reward_train,
+        average_steps_per_second,
+    )
     return statistics.data_lists
 
-  def _save_tensorboard_summaries(self, iteration, num_episodes,
-                                  average_reward, average_steps_per_second):
+  def _save_tensorboard_summaries(
+      self, iteration, num_episodes, average_reward, average_steps_per_second
+  ):
     """Save statistics as tensorboard summaries."""
-    metrics = [('Train/NumEpisodes', num_episodes),
-               ('Train/AverageReturns', average_reward),
-               ('Train/AverageStepsPerSecond', average_steps_per_second)]
+    metrics = [
+        ('Train/NumEpisodes', num_episodes),
+        ('Train/AverageReturns', average_reward),
+        ('Train/AverageStepsPerSecond', average_steps_per_second),
+    ]
     for name, value in metrics:
       self._summary_writer.scalar(name, value, iteration)
     self._summary_writer.flush()
```

### Comparing `dopamine_rl-4.0.6/dopamine/continuous_domains/train.py` & `dopamine_rl-4.0.7/dopamine/continuous_domains/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,28 @@
 
 from absl import app
 from absl import flags
 from absl import logging
 
 from dopamine.continuous_domains import run_experiment
 
-flags.DEFINE_string('base_dir', None,
-                    'Base directory to host all required sub-directories.')
+flags.DEFINE_string(
+    'base_dir', None, 'Base directory to host all required sub-directories.'
+)
 flags.DEFINE_multi_string(
-    'gin_files', [], 'List of paths to gin configuration files (e.g.'
-    '"dopamine/jax/agents/sac/configs/sac.gin").')
+    'gin_files',
+    [],
+    'List of paths to gin configuration files (e.g.'
+    '"dopamine/jax/agents/sac/configs/sac.gin").',
+)
 flags.DEFINE_multi_string(
-    'gin_bindings', [],
-    'Gin bindings to override the values set in the config files.')
+    'gin_bindings',
+    [],
+    'Gin bindings to override the values set in the config files.',
+)
 
 FLAGS = flags.FLAGS
 
 
 def main(unused_argv):
   """Main method.
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/__init__.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/atari_lib.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/atari_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,19 @@
 
 NATURE_DQN_OBSERVATION_SHAPE = (84, 84)  # Size of downscaled Atari 2600 frame.
 NATURE_DQN_DTYPE = tf.uint8  # DType of Atari 2600 observations.
 NATURE_DQN_STACK_SIZE = 4  # Number of frames in the state stack.
 
 DQNNetworkType = collections.namedtuple('dqn_network', ['q_values'])
 RainbowNetworkType = collections.namedtuple(
-    'c51_network', ['q_values', 'logits', 'probabilities'])
+    'c51_network', ['q_values', 'logits', 'probabilities']
+)
 ImplicitQuantileNetworkType = collections.namedtuple(
-    'iqn_network', ['quantile_values', 'quantiles'])
+    'iqn_network', ['quantile_values', 'quantiles']
+)
 
 
 
 
 @gin.configurable
 def create_atari_environment(game_name=None, sticky_actions=True):
   """Wraps an Atari 2600 Gym environment with some basic preprocessing.
@@ -108,17 +110,18 @@
   """Maps old variable names to the new ones.
 
   The resulting dictionary can be passed to the tf.compat.v1.train.Saver to load
   legacy checkpoints into Keras models.
 
   Args:
     variables: list, of all variables to be transformed.
-    legacy_checkpoint_load: bool, if True the variable names are mapped to
-        the legacy names as appeared in `tf.slim` based agents. Use this if
-        you want to load checkpoints saved before tf.keras.Model upgrade.
+    legacy_checkpoint_load: bool, if True the variable names are mapped to the
+      legacy names as appeared in `tf.slim` based agents. Use this if you want
+      to load checkpoints saved before tf.keras.Model upgrade.
+
   Returns:
     dict or None, of <new_names, var>.
   """
   logging.info('legacy_checkpoint_load: %s', legacy_checkpoint_load)
   if legacy_checkpoint_load:
     name_map = {}
     for var in variables:
@@ -143,36 +146,56 @@
     super(NatureDQNNetwork, self).__init__(name=name)
 
     self.num_actions = num_actions
     # Defining layers.
     activation_fn = tf.keras.activations.relu
     # Setting names of the layers manually to make variable names more similar
     # with tf.slim variable names/checkpoints.
-    self.conv1 = tf.keras.layers.Conv2D(32, [8, 8], strides=4, padding='same',
-                                        activation=activation_fn, name='Conv')
-    self.conv2 = tf.keras.layers.Conv2D(64, [4, 4], strides=2, padding='same',
-                                        activation=activation_fn, name='Conv')
-    self.conv3 = tf.keras.layers.Conv2D(64, [3, 3], strides=1, padding='same',
-                                        activation=activation_fn, name='Conv')
+    self.conv1 = tf.keras.layers.Conv2D(
+        32,
+        [8, 8],
+        strides=4,
+        padding='same',
+        activation=activation_fn,
+        name='Conv',
+    )
+    self.conv2 = tf.keras.layers.Conv2D(
+        64,
+        [4, 4],
+        strides=2,
+        padding='same',
+        activation=activation_fn,
+        name='Conv',
+    )
+    self.conv3 = tf.keras.layers.Conv2D(
+        64,
+        [3, 3],
+        strides=1,
+        padding='same',
+        activation=activation_fn,
+        name='Conv',
+    )
     self.flatten = tf.keras.layers.Flatten()
-    self.dense1 = tf.keras.layers.Dense(512, activation=activation_fn,
-                                        name='fully_connected')
+    self.dense1 = tf.keras.layers.Dense(
+        512, activation=activation_fn, name='fully_connected'
+    )
     self.dense2 = tf.keras.layers.Dense(num_actions, name='fully_connected')
 
   def call(self, state):
     """Creates the output tensor/op given the state tensor as input.
 
     See https://www.tensorflow.org/api_docs/python/tf/keras/Model for more
     information on this. Note that tf.keras.Model implements `call` which is
     wrapped by `__call__` function by tf.keras.Model.
 
     Parameters created here will have scope according to the `name` argument
     given at `.__init__()` call.
     Args:
       state: Tensor, input tensor.
+
     Returns:
       collections.namedtuple, output ops (graph mode) or output tensors (eager).
     """
     x = tf.cast(state, tf.float32)
     x = x / 255
     x = self.conv1(x)
     x = self.conv2(x)
@@ -196,44 +219,71 @@
       name: str, used to crete scope for network parameters.
     """
     super(RainbowNetwork, self).__init__(name=name)
     activation_fn = tf.keras.activations.relu
     self.num_actions = num_actions
     self.num_atoms = num_atoms
     self.support = support
+
     def kernel_initializer():
       return tf.keras.initializers.VarianceScaling(
-          scale=1.0 / np.sqrt(3.0), mode='fan_in', distribution='uniform')
+          scale=1.0 / np.sqrt(3.0), mode='fan_in', distribution='uniform'
+      )
+
     # Defining layers.
     self.conv1 = tf.keras.layers.Conv2D(
-        32, [8, 8], strides=4, padding='same', activation=activation_fn,
-        kernel_initializer=kernel_initializer(), name='Conv')
+        32,
+        [8, 8],
+        strides=4,
+        padding='same',
+        activation=activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='Conv',
+    )
     self.conv2 = tf.keras.layers.Conv2D(
-        64, [4, 4], strides=2, padding='same', activation=activation_fn,
-        kernel_initializer=kernel_initializer(), name='Conv')
+        64,
+        [4, 4],
+        strides=2,
+        padding='same',
+        activation=activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='Conv',
+    )
     self.conv3 = tf.keras.layers.Conv2D(
-        64, [3, 3], strides=1, padding='same', activation=activation_fn,
-        kernel_initializer=kernel_initializer(), name='Conv')
+        64,
+        [3, 3],
+        strides=1,
+        padding='same',
+        activation=activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='Conv',
+    )
     self.flatten = tf.keras.layers.Flatten()
     self.dense1 = tf.keras.layers.Dense(
-        512, activation=activation_fn,
-        kernel_initializer=kernel_initializer(), name='fully_connected')
+        512,
+        activation=activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='fully_connected',
+    )
     self.dense2 = tf.keras.layers.Dense(
-        num_actions * num_atoms, kernel_initializer=kernel_initializer(),
-        name='fully_connected')
+        num_actions * num_atoms,
+        kernel_initializer=kernel_initializer(),
+        name='fully_connected',
+    )
 
   def call(self, state):
     """Creates the output tensor/op given the state tensor as input.
 
     See https://www.tensorflow.org/api_docs/python/tf/keras/Model for more
     information on this. Note that tf.keras.Model implements `call` which is
     wrapped by `__call__` function by tf.keras.Model.
 
     Args:
       state: Tensor, input tensor.
+
     Returns:
       collections.namedtuple, output ops (graph mode) or output tensors (eager).
     """
     x = tf.cast(state, tf.float32)
     x = x / 255
     x = self.conv1(x)
     x = self.conv2(x)
@@ -259,73 +309,106 @@
       name: str, used to create scope for network parameters.
     """
     super(ImplicitQuantileNetwork, self).__init__(name=name)
     self.num_actions = num_actions
     self.quantile_embedding_dim = quantile_embedding_dim
     # We need the activation function during `call`, therefore set the field.
     self.activation_fn = tf.keras.activations.relu
+
     def kernel_initializer():
       return tf.keras.initializers.VarianceScaling(
-          scale=1.0 / np.sqrt(3.0), mode='fan_in', distribution='uniform')
+          scale=1.0 / np.sqrt(3.0), mode='fan_in', distribution='uniform'
+      )
+
     self.kernel_initializer = kernel_initializer
     # Defining layers.
     self.conv1 = tf.keras.layers.Conv2D(
-        32, [8, 8], strides=4, padding='same', activation=self.activation_fn,
-        kernel_initializer=kernel_initializer(), name='Conv')
+        32,
+        [8, 8],
+        strides=4,
+        padding='same',
+        activation=self.activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='Conv',
+    )
     self.conv2 = tf.keras.layers.Conv2D(
-        64, [4, 4], strides=2, padding='same', activation=self.activation_fn,
-        kernel_initializer=kernel_initializer(), name='Conv')
+        64,
+        [4, 4],
+        strides=2,
+        padding='same',
+        activation=self.activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='Conv',
+    )
     self.conv3 = tf.keras.layers.Conv2D(
-        64, [3, 3], strides=1, padding='same', activation=self.activation_fn,
-        kernel_initializer=kernel_initializer(), name='Conv')
+        64,
+        [3, 3],
+        strides=1,
+        padding='same',
+        activation=self.activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='Conv',
+    )
     self.flatten = tf.keras.layers.Flatten()
     self.dense1 = tf.keras.layers.Dense(
-        512, activation=self.activation_fn,
-        kernel_initializer=kernel_initializer(), name='fully_connected')
+        512,
+        activation=self.activation_fn,
+        kernel_initializer=kernel_initializer(),
+        name='fully_connected',
+    )
     self.dense2 = tf.keras.layers.Dense(
-        num_actions, kernel_initializer=kernel_initializer(),
-        name='fully_connected')
+        num_actions,
+        kernel_initializer=kernel_initializer(),
+        name='fully_connected',
+    )
 
   def call(self, state, num_quantiles):
     """Creates the output tensor/op given the state tensor as input.
 
     See https://www.tensorflow.org/api_docs/python/tf/keras/Model for more
     information on this. Note that tf.keras.Model implements `call` which is
     wrapped by `__call__` function by tf.keras.Model.
 
     Args:
       state: `tf.Tensor`, contains the agent's current state.
       num_quantiles: int, number of quantile inputs.
+
     Returns:
       collections.namedtuple, that contains (quantile_values, quantiles).
     """
     batch_size = state.get_shape().as_list()[0]
     x = tf.cast(state, tf.float32)
     x = x / 255
     x = self.conv1(x)
     x = self.conv2(x)
     x = self.conv3(x)
     x = self.flatten(x)
     state_vector_length = x.get_shape().as_list()[-1]
     state_net_tiled = tf.tile(x, [num_quantiles, 1])
     quantiles_shape = [num_quantiles * batch_size, 1]
     quantiles = tf.random.uniform(
-        quantiles_shape, minval=0, maxval=1, dtype=tf.float32)
+        quantiles_shape, minval=0, maxval=1, dtype=tf.float32
+    )
     quantile_net = tf.tile(quantiles, [1, self.quantile_embedding_dim])
     pi = tf.constant(math.pi)
-    quantile_net = tf.cast(tf.range(
-        1, self.quantile_embedding_dim + 1, 1), tf.float32) * pi * quantile_net
+    quantile_net = (
+        tf.cast(tf.range(1, self.quantile_embedding_dim + 1, 1), tf.float32)
+        * pi
+        * quantile_net
+    )
     quantile_net = tf.cos(quantile_net)
     # Create the quantile layer in the first call. This is because
     # number of output units depends on the input shape. Therefore, we can only
     # create the layer during the first forward call, not during `.__init__()`.
     if not hasattr(self, 'dense_quantile'):
       self.dense_quantile = tf.keras.layers.Dense(
-          state_vector_length, activation=self.activation_fn,
-          kernel_initializer=self.kernel_initializer())
+          state_vector_length,
+          activation=self.activation_fn,
+          kernel_initializer=self.kernel_initializer(),
+      )
     quantile_net = self.dense_quantile(quantile_net)
     x = tf.multiply(state_net_tiled, quantile_net)
     x = self.dense1(x)
     quantile_values = self.dense2(x)
     return ImplicitQuantileNetworkType(quantile_values, quantiles)
 
 
@@ -342,57 +425,70 @@
     * Downsample the screen to a square image (defaults to 84x84).
 
   More generally, this class follows the preprocessing guidelines set down in
   Machado et al. (2018), "Revisiting the Arcade Learning Environment:
   Evaluation Protocols and Open Problems for General Agents".
   """
 
-  def __init__(self, environment, frame_skip=4, terminal_on_life_loss=False,
-               screen_size=84):
+  def __init__(
+      self,
+      environment,
+      frame_skip=4,
+      terminal_on_life_loss=False,
+      screen_size=84,
+  ):
     """Constructor for an Atari 2600 preprocessor.
 
     Args:
       environment: Gym environment whose observations are preprocessed.
       frame_skip: int, the frequency at which the agent experiences the game.
       terminal_on_life_loss: bool, If True, the step() method returns
         is_terminal=True whenever a life is lost. See Mnih et al. 2015.
       screen_size: int, size of a resized Atari 2600 frame.
 
     Raises:
       ValueError: if frame_skip or screen_size are not strictly positive.
     """
     if frame_skip <= 0:
-      raise ValueError('Frame skip should be strictly positive, got {}'.
-                       format(frame_skip))
+      raise ValueError(
+          'Frame skip should be strictly positive, got {}'.format(frame_skip)
+      )
     if screen_size <= 0:
-      raise ValueError('Target screen size should be strictly positive, got {}'.
-                       format(screen_size))
+      raise ValueError(
+          'Target screen size should be strictly positive, got {}'.format(
+              screen_size
+          )
+      )
 
     self.environment = environment
     self.terminal_on_life_loss = terminal_on_life_loss
     self.frame_skip = frame_skip
     self.screen_size = screen_size
 
     obs_dims = self.environment.observation_space
     # Stores temporary observations used for pooling over two successive
     # frames.
     self.screen_buffer = [
         np.empty((obs_dims.shape[0], obs_dims.shape[1]), dtype=np.uint8),
-        np.empty((obs_dims.shape[0], obs_dims.shape[1]), dtype=np.uint8)
+        np.empty((obs_dims.shape[0], obs_dims.shape[1]), dtype=np.uint8),
     ]
 
     self.game_over = False
     self.lives = 0  # Will need to be set by reset().
 
   @property
   def observation_space(self):
     # Return the observation space adjusted to match the shape of the processed
     # observations.
-    return Box(low=0, high=255, shape=(self.screen_size, self.screen_size, 1),
-               dtype=np.uint8)
+    return Box(
+        low=0,
+        high=255,
+        shape=(self.screen_size, self.screen_size, 1),
+        dtype=np.uint8,
+    )
 
   @property
   def action_space(self):
     return self.environment.action_space
 
   @property
   def reward_range(self):
@@ -420,18 +516,17 @@
 
   def render(self, mode):
     """Renders the current screen, before preprocessing.
 
     This calls the Gym API's render() method.
 
     Args:
-      mode: Mode argument for the environment's render() method.
-        Valid values (str) are:
-          'rgb_array': returns the raw ALE image.
-          'human': renders to display via the Gym renderer.
+      mode: Mode argument for the environment's render() method. Valid values
+        (str) are: 'rgb_array': returns the raw ALE image. 'human': renders to
+        display via the Gym renderer.
 
     Returns:
       if mode='rgb_array': numpy array, the most recent screen.
       if mode='human': bool, whether the rendering was successful.
     """
     return self.environment.render(mode)
 
@@ -452,15 +547,15 @@
       observation: numpy array, the observation following the action.
       reward: float, the reward following the action.
       is_terminal: bool, whether the environment has reached a terminal state.
         This is true when a life is lost and terminal_on_life_loss, or when the
         episode is over.
       info: Gym API's info data structure.
     """
-    accumulated_reward = 0.
+    accumulated_reward = 0.0
 
     for time_step in range(self.frame_skip):
       # We bypass the Gym observation altogether and directly fetch the
       # grayscale image from the ALE. This is a little faster.
       _, reward, game_over, info = self.environment.step(action)
       accumulated_reward += reward
 
@@ -505,15 +600,20 @@
     For efficiency, the transformation is done in-place in self.screen_buffer.
 
     Returns:
       transformed_screen: numpy array, pooled, resized screen.
     """
     # Pool if there are enough screens to do so.
     if self.frame_skip > 1:
-      np.maximum(self.screen_buffer[0], self.screen_buffer[1],
-                 out=self.screen_buffer[0])
-
-    transformed_image = cv2.resize(self.screen_buffer[0],
-                                   (self.screen_size, self.screen_size),
-                                   interpolation=cv2.INTER_AREA)
+      np.maximum(
+          self.screen_buffer[0],
+          self.screen_buffer[1],
+          out=self.screen_buffer[0],
+      )
+
+    transformed_image = cv2.resize(
+        self.screen_buffer[0],
+        (self.screen_size, self.screen_size),
+        interpolation=cv2.INTER_AREA,
+    )
     int_image = np.asarray(transformed_image, dtype=np.uint8)
     return np.expand_dims(int_image, axis=2)
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/checkpointer.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/checkpointer.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,62 +47,67 @@
 from __future__ import division
 from __future__ import print_function
 
 import os
 import pickle
 
 from absl import logging
-
 import gin
 import tensorflow as tf
 
 
 @gin.configurable
-def get_latest_checkpoint_number(base_directory,
-                                 override_number=None,
-                                 sentinel_file_identifier='checkpoint'):
+def get_latest_checkpoint_number(
+    base_directory, override_number=None, sentinel_file_identifier='checkpoint'
+):
   """Returns the version number of the latest completed checkpoint.
 
   Args:
     base_directory: str, directory in which to look for checkpoint files.
-    override_number: None or int, allows the user to manually override
-      the checkpoint number via a gin-binding.
+    override_number: None or int, allows the user to manually override the
+      checkpoint number via a gin-binding.
     sentinel_file_identifier: str, prefix used by checkpointer for naming
       sentinel files.
 
   Returns:
     int, the iteration number of the latest checkpoint, or -1 if none was found.
   """
   if override_number is not None:
     return override_number
 
   sentinel = 'sentinel_{}_complete.*'.format(sentinel_file_identifier)
   glob = os.path.join(base_directory, sentinel)
+
   def extract_iteration(x):
-    return int(x[x.rfind('.') + 1:])
+    return int(x[x.rfind('.') + 1 :])
+
   try:
     checkpoint_files = tf.io.gfile.glob(glob)
   except tf.errors.NotFoundError:
     return -1
   try:
     latest_iteration = max(extract_iteration(x) for x in checkpoint_files)
     return latest_iteration
   except ValueError:
     return -1
 
 
 @gin.configurable
 class Checkpointer(object):
-  """Class for managing checkpoints for Dopamine agents.
-  """
+  """Class for managing checkpoints for Dopamine agents."""
 
-  def __init__(self, base_directory, checkpoint_file_prefix='ckpt',
-               sentinel_file_identifier='checkpoint', checkpoint_frequency=1,
-               checkpoint_duration=4,
-               keep_every=None):
+  def __init__(
+      self,
+      base_directory,
+      checkpoint_file_prefix='ckpt',
+      sentinel_file_identifier='checkpoint',
+      checkpoint_frequency=1,
+      checkpoint_duration=4,
+      keep_every=None,
+  ):
     """Initializes Checkpointer.
 
     Args:
       base_directory: str, directory where all checkpoints are saved/loaded.
       checkpoint_file_prefix: str, prefix to use for naming checkpoint files.
       sentinel_file_identifier: str, prefix to use for naming sentinel files.
       checkpoint_frequency: int, the frequency at which to checkpoint.
@@ -113,25 +118,27 @@
     Raises:
       ValueError: if base_directory is empty, or not creatable.
     """
     if not base_directory:
       raise ValueError('No path provided to Checkpointer.')
     self._checkpoint_file_prefix = checkpoint_file_prefix
     self._sentinel_file_prefix = 'sentinel_{}_complete'.format(
-        sentinel_file_identifier)
+        sentinel_file_identifier
+    )
     self._checkpoint_frequency = checkpoint_frequency
     self._checkpoint_duration = checkpoint_duration
     self._keep_every = keep_every
     self._base_directory = base_directory
     try:
       tf.io.gfile.makedirs(base_directory)
     except tf.errors.PermissionDeniedError as permission_error:
       # We catch the PermissionDeniedError and issue a more useful exception.
-      raise ValueError('Unable to create checkpoint path: {}.'.format(
-          base_directory)) from permission_error
+      raise ValueError(
+          'Unable to create checkpoint path: {}.'.format(base_directory)
+      ) from permission_error
 
   def _generate_filename(self, file_prefix, iteration_number):
     """Returns a checkpoint filename from prefix and iteration number."""
     filename = '{}.{}'.format(file_prefix, iteration_number)
     return os.path.join(self._base_directory, filename)
 
   def _save_data_to_file(self, data, filename):
@@ -146,43 +153,49 @@
       iteration_number: int, the current iteration number for this checkpoint.
       data: Any (picklable) python object containing the data to store in the
         checkpoint.
     """
     if iteration_number % self._checkpoint_frequency != 0:
       return
 
-    filename = self._generate_filename(self._checkpoint_file_prefix,
-                                       iteration_number)
+    filename = self._generate_filename(
+        self._checkpoint_file_prefix, iteration_number
+    )
     self._save_data_to_file(data, filename)
-    filename = self._generate_filename(self._sentinel_file_prefix,
-                                       iteration_number)
+    filename = self._generate_filename(
+        self._sentinel_file_prefix, iteration_number
+    )
     with tf.io.gfile.GFile(filename, 'wb') as fout:
       fout.write('done')
 
     self._clean_up_old_checkpoints(iteration_number)
 
   def _clean_up_old_checkpoints(self, iteration_number):
     """Removes sufficiently old checkpoints."""
     # After writing a the checkpoint and sentinel file, we garbage collect files
     # that are self._checkpoint_duration * self._checkpoint_frequency
     # versions old.
-    stale_iteration_number = iteration_number - (self._checkpoint_frequency *
-                                                 self._checkpoint_duration)
+    stale_iteration_number = iteration_number - (
+        self._checkpoint_frequency * self._checkpoint_duration
+    )
 
     # If keep_every has been set, we spare every keep_every'th checkpoint
-    if (self._keep_every is not None
-        and (stale_iteration_number %
-             (self._keep_every*self._checkpoint_frequency) == 0)):
+    if self._keep_every is not None and (
+        stale_iteration_number % (self._keep_every * self._checkpoint_frequency)
+        == 0
+    ):
       return
 
     if stale_iteration_number >= 0:
-      stale_file = self._generate_filename(self._checkpoint_file_prefix,
-                                           stale_iteration_number)
-      stale_sentinel = self._generate_filename(self._sentinel_file_prefix,
-                                               stale_iteration_number)
+      stale_file = self._generate_filename(
+          self._checkpoint_file_prefix, stale_iteration_number
+      )
+      stale_sentinel = self._generate_filename(
+          self._sentinel_file_prefix, stale_iteration_number
+      )
       try:
         tf.io.gfile.remove(stale_file)
         tf.io.gfile.remove(stale_sentinel)
       except tf.errors.NotFoundError:
         # Ignore if file not found.
         logging.info('Unable to remove %s or %s.', stale_file, stale_sentinel)
 
@@ -198,10 +211,11 @@
     Args:
       iteration_number: The checkpoint iteration number to try to load.
 
     Returns:
       If the checkpoint files exist, two unpickled objects that were passed in
         as data to save_checkpoint; returns None if the files do not exist.
     """
-    checkpoint_file = self._generate_filename(self._checkpoint_file_prefix,
-                                              iteration_number)
+    checkpoint_file = self._generate_filename(
+        self._checkpoint_file_prefix, iteration_number
+    )
     return self._load_data_from_file(checkpoint_file)
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/gym_lib.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/gym_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 import gin
 import gym
 from gym.wrappers.time_limit import TimeLimit
 import numpy as np
 import tensorflow as tf
 
 
-CARTPOLE_MIN_VALS = np.array([-2.4, -5., -math.pi/12., -math.pi*2.])
-CARTPOLE_MAX_VALS = np.array([2.4, 5., math.pi/12., math.pi*2.])
-ACROBOT_MIN_VALS = np.array([-1., -1., -1., -1., -5., -5.])
-ACROBOT_MAX_VALS = np.array([1., 1., 1., 1., 5., 5.])
+CARTPOLE_MIN_VALS = np.array([-2.4, -5.0, -math.pi / 12.0, -math.pi * 2.0])
+CARTPOLE_MAX_VALS = np.array([2.4, 5.0, math.pi / 12.0, math.pi * 2.0])
+ACROBOT_MIN_VALS = np.array([-1.0, -1.0, -1.0, -1.0, -5.0, -5.0])
+ACROBOT_MAX_VALS = np.array([1.0, 1.0, 1.0, 1.0, 5.0, 5.0])
 MOUNTAINCAR_MIN_VALS = np.array([-1.2, -0.07])
 MOUNTAINCAR_MAX_VALS = np.array([0.6, 0.07])
 gin.constant('gym_lib.CARTPOLE_OBSERVATION_SHAPE', (4, 1))
 gin.constant('gym_lib.CARTPOLE_OBSERVATION_DTYPE', tf.float64)
 gin.constant('gym_lib.CARTPOLE_STACK_SIZE', 1)
 gin.constant('gym_lib.ACROBOT_OBSERVATION_SHAPE', (6, 1))
 gin.constant('gym_lib.ACROBOT_OBSERVATION_DTYPE', tf.float64)
@@ -86,50 +86,58 @@
   return env
 
 
 @gin.configurable
 class BasicDiscreteDomainNetwork(tf.keras.layers.Layer):
   """The fully connected network used to compute the agent's Q-values.
 
-    This sub network used within various other models. Since it is an inner
-    block, we define it as a layer. These sub networks normalize their inputs to
-    lie in range [-1, 1], using min_/max_vals. It supports both DQN- and
-    Rainbow- style networks.
-    Attributes:
-      min_vals: float, minimum attainable values (must be same shape as
-        `state`).
-      max_vals: float, maximum attainable values (must be same shape as
-        `state`).
-      num_actions: int, number of actions.
-      num_atoms: int or None, if None will construct a DQN-style network,
-        otherwise will construct a Rainbow-style network.
-      name: str, used to create scope for network parameters.
-      activation_fn: function, passed to the layer constructors.
+  This sub network used within various other models. Since it is an inner
+  block, we define it as a layer. These sub networks normalize their inputs to
+  lie in range [-1, 1], using min_/max_vals. It supports both DQN- and
+  Rainbow- style networks.
+  Attributes:
+    min_vals: float, minimum attainable values (must be same shape as `state`).
+    max_vals: float, maximum attainable values (must be same shape as `state`).
+    num_actions: int, number of actions.
+    num_atoms: int or None, if None will construct a DQN-style network,
+      otherwise will construct a Rainbow-style network.
+    name: str, used to create scope for network parameters.
+    activation_fn: function, passed to the layer constructors.
   """
 
-  def __init__(self, min_vals, max_vals, num_actions,
-               num_atoms=None, name=None,
-               activation_fn=tf.keras.activations.relu):
+  def __init__(
+      self,
+      min_vals,
+      max_vals,
+      num_actions,
+      num_atoms=None,
+      name=None,
+      activation_fn=tf.keras.activations.relu,
+  ):
     super(BasicDiscreteDomainNetwork, self).__init__(name=name)
     self.num_actions = num_actions
     self.num_atoms = num_atoms
     self.min_vals = min_vals
     self.max_vals = max_vals
     # Defining layers.
     self.flatten = tf.keras.layers.Flatten()
-    self.dense1 = tf.keras.layers.Dense(512, activation=activation_fn,
-                                        name='fully_connected')
-    self.dense2 = tf.keras.layers.Dense(512, activation=activation_fn,
-                                        name='fully_connected')
+    self.dense1 = tf.keras.layers.Dense(
+        512, activation=activation_fn, name='fully_connected'
+    )
+    self.dense2 = tf.keras.layers.Dense(
+        512, activation=activation_fn, name='fully_connected'
+    )
     if num_atoms is None:
-      self.last_layer = tf.keras.layers.Dense(num_actions,
-                                              name='fully_connected')
+      self.last_layer = tf.keras.layers.Dense(
+          num_actions, name='fully_connected'
+      )
     else:
-      self.last_layer = tf.keras.layers.Dense(num_actions * num_atoms,
-                                              name='fully_connected')
+      self.last_layer = tf.keras.layers.Dense(
+          num_actions * num_atoms, name='fully_connected'
+      )
 
   def call(self, state):
     """Creates the output tensor/op given the state tensor as input."""
     x = tf.cast(state, tf.float32)
     x = self.flatten(x)
     if self.min_vals is not None:
       x -= self.min_vals
@@ -152,15 +160,16 @@
 
     Args:
       num_actions: int, number of actions.
       name: str, used to create scope for network parameters.
     """
     super(CartpoleDQNNetwork, self).__init__(name=name)
     self.net = BasicDiscreteDomainNetwork(
-        CARTPOLE_MIN_VALS, CARTPOLE_MAX_VALS, num_actions)
+        CARTPOLE_MIN_VALS, CARTPOLE_MAX_VALS, num_actions
+    )
 
   def call(self, state):
     """Creates the output tensor/op given the state tensor as input."""
     x = self.net(state)
     return atari_lib.DQNNetworkType(x)
 
 
@@ -182,15 +191,16 @@
     self.order = order
     self.min_vals = min_vals
     self.max_vals = max_vals
     terms = itertools.product(range(order + 1), repeat=nvars)
 
     # Removing first iterate because it corresponds to the constant bias
     self.multipliers = tf.constant(
-        [list(map(int, x)) for x in terms][1:], dtype=tf.float32)
+        [list(map(int, x)) for x in terms][1:], dtype=tf.float32
+    )
 
   def scale(self, values):
     shifted = values - self.min_vals
     if self.max_vals is None:
       return shifted
 
     return shifted / (self.max_vals - self.min_vals)
@@ -201,16 +211,17 @@
     return tf.cos(np.pi * tf.matmul(scaled, self.multipliers, transpose_b=True))
 
 
 @gin.configurable
 class FourierDQNNetwork(tf.keras.Model):
   """Keras model for DQN."""
 
-  def __init__(self, min_vals, max_vals, num_actions, fourier_basis_order=3,
-               name=None):
+  def __init__(
+      self, min_vals, max_vals, num_actions, fourier_basis_order=3, name=None
+  ):
     """Builds the function approximator used to compute the agent's Q-values.
 
     It uses the features of the FourierBasis class and a linear layer
     without bias.
 
     Value Function Approximation in Reinforcement Learning using the Fourier
     Basis", Konidaris, Osentoski and Thomas (2011).
@@ -227,29 +238,31 @@
     super(FourierDQNNetwork, self).__init__(name=name)
     self.num_actions = num_actions
     self.fourier_basis_order = fourier_basis_order
     self.min_vals = min_vals
     self.max_vals = max_vals
     # Defining layers.
     self.flatten = tf.keras.layers.Flatten()
-    self.last_layer = tf.keras.layers.Dense(num_actions, use_bias=False,
-                                            name='fully_connected')
+    self.last_layer = tf.keras.layers.Dense(
+        num_actions, use_bias=False, name='fully_connected'
+    )
 
   def call(self, state):
     """Creates the output tensor/op given the state tensor as input."""
     x = tf.cast(state, tf.float32)
     x = self.flatten(x)
     # Since FourierBasis needs the shape of the input, we can only initialize
     # it during the first forward pass when we know the shape of the input.
     if not hasattr(self, 'feature_generator'):
       self.feature_generator = FourierBasis(
           x.get_shape().as_list()[-1],
           self.min_vals,
           self.max_vals,
-          order=self.fourier_basis_order)
+          order=self.fourier_basis_order,
+      )
     x = self.feature_generator.compute_features(x)
     x = self.last_layer(x)
     return atari_lib.DQNNetworkType(x)
 
 
 @gin.configurable
 class CartpoleFourierDQNNetwork(FourierDQNNetwork):
@@ -261,15 +274,16 @@
     It uses the Fourier basis features and a linear function approximator.
 
     Args:
       num_actions: int, number of actions.
       name: str, used to create scope for network parameters.
     """
     super(CartpoleFourierDQNNetwork, self).__init__(
-        CARTPOLE_MIN_VALS, CARTPOLE_MAX_VALS, num_actions, name=name)
+        CARTPOLE_MIN_VALS, CARTPOLE_MAX_VALS, num_actions, name=name
+    )
 
 
 @gin.configurable
 class CartpoleRainbowNetwork(tf.keras.Model):
   """Keras Rainbow network for Cartpole."""
 
   def __init__(self, num_actions, num_atoms, support, name=None):
@@ -281,15 +295,16 @@
       num_actions: int, number of actions.
       num_atoms: int, the number of buckets of the value function distribution.
       support: tf.linspace, the support of the Q-value distribution.
       name: str, used to create scope for network parameters.
     """
     super(CartpoleRainbowNetwork, self).__init__(name=name)
     self.net = BasicDiscreteDomainNetwork(
-        CARTPOLE_MIN_VALS, CARTPOLE_MAX_VALS, num_actions, num_atoms=num_atoms)
+        CARTPOLE_MIN_VALS, CARTPOLE_MAX_VALS, num_actions, num_atoms=num_atoms
+    )
     self.num_actions = num_actions
     self.num_atoms = num_atoms
     self.support = support
 
   def call(self, state):
     x = self.net(state)
     logits = tf.reshape(x, [-1, self.num_actions, self.num_atoms])
@@ -309,15 +324,16 @@
 
     Args:
       num_actions: int, number of actions.
       name: str, used to create scope for network parameters.
     """
     super(AcrobotDQNNetwork, self).__init__(name=name)
     self.net = BasicDiscreteDomainNetwork(
-        ACROBOT_MIN_VALS, ACROBOT_MAX_VALS, num_actions)
+        ACROBOT_MIN_VALS, ACROBOT_MAX_VALS, num_actions
+    )
 
   def call(self, state):
     x = self.net(state)
     return atari_lib.DQNNetworkType(x)
 
 
 @gin.configurable
@@ -331,15 +347,16 @@
 
     Args:
       num_actions: int, number of actions.
       name: str, used to create scope for network parameters.
     """
 
     super(AcrobotFourierDQNNetwork, self).__init__(
-        ACROBOT_MIN_VALS, ACROBOT_MAX_VALS, num_actions, name=name)
+        ACROBOT_MIN_VALS, ACROBOT_MAX_VALS, num_actions, name=name
+    )
 
 
 @gin.configurable
 class AcrobotRainbowNetwork(tf.keras.Model):
   """Keras Rainbow network for Acrobot."""
 
   def __init__(self, num_actions, num_atoms, support, name=None):
@@ -351,15 +368,16 @@
       num_actions: int, number of actions.
       num_atoms: int, the number of buckets of the value function distribution.
       support: Tensor, the support of the Q-value distribution.
       name: str, used to create scope for network parameters.
     """
     super(AcrobotRainbowNetwork, self).__init__(name=name)
     self.net = BasicDiscreteDomainNetwork(
-        ACROBOT_MIN_VALS, ACROBOT_MAX_VALS, num_actions, num_atoms=num_atoms)
+        ACROBOT_MIN_VALS, ACROBOT_MAX_VALS, num_actions, num_atoms=num_atoms
+    )
     self.num_actions = num_actions
     self.num_atoms = num_atoms
     self.support = support
 
   def call(self, state):
     x = self.net(state)
     logits = tf.reshape(x, [-1, self.num_actions, self.num_atoms])
@@ -397,15 +415,16 @@
 
     Args:
       num_actions: int, number of actions.
       name: str, used to create scope for network parameters.
     """
     super(MountainCarDQNNetwork, self).__init__(name=name)
     self.net = BasicDiscreteDomainNetwork(
-        MOUNTAINCAR_MIN_VALS, MOUNTAINCAR_MAX_VALS, num_actions)
+        MOUNTAINCAR_MIN_VALS, MOUNTAINCAR_MAX_VALS, num_actions
+    )
 
   def call(self, state):
     """Creates the output tensor/op given the state tensor as input."""
     x = self.net(state)
     return atari_lib.DQNNetworkType(x)
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/iteration_statistics.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/iteration_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A class for storing iteration-specific metrics.
-"""
+"""A class for storing iteration-specific metrics."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 
 class IterationStatistics(object):
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/legacy_networks.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/legacy_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,55 +52,59 @@
     net: _network_type object containing the tensors output by the network.
   """
   model = atari_lib.RainbowNetwork(num_actions, num_atoms, support)
   net = model(state)
   return network_type(net.q_values, net.logits, net.probabilities)
 
 
-def implicit_quantile_network(num_actions, quantile_embedding_dim,
-                              network_type, state, num_quantiles):
+def implicit_quantile_network(
+    num_actions, quantile_embedding_dim, network_type, state, num_quantiles
+):
   """The Implicit Quantile ConvNet.
 
   Args:
     num_actions: int, number of actions.
     quantile_embedding_dim: int, embedding dimension for the quantile input.
     network_type: namedtuple, collection of expected values to return.
     state: `tf.Tensor`, contains the agent's current state.
     num_quantiles: int, number of quantile inputs.
 
   Returns:
     net: _network_type object containing the tensors output by the network.
   """
   model = atari_lib.ImplicitQuantileNetwork(num_actions, quantile_embedding_dim)
   net = model(state, num_quantiles)
-  return network_type(quantile_values=net.quantile_values,
-                      quantiles=net.quantiles)
+  return network_type(
+      quantile_values=net.quantile_values, quantiles=net.quantiles
+  )
 
 
 ### Generic Gym networks ###
 
 
 @gin.configurable
-def _basic_discrete_domain_network(min_vals, max_vals, num_actions, state,
-                                   num_atoms=None):
+def _basic_discrete_domain_network(
+    min_vals, max_vals, num_actions, state, num_atoms=None
+):
   """Builds a basic network for discrete domains, rescaling inputs to [-1, 1].
 
   Args:
     min_vals: float, minimum attainable values (must be same shape as `state`).
     max_vals: float, maximum attainable values (must be same shape as `state`).
     num_actions: int, number of actions.
     state: `tf.Tensor`, the state input.
     num_atoms: int or None, if None will construct a DQN-style network,
       otherwise will construct a Rainbow-style network.
 
   Returns:
     The Q-values for DQN-style agents or logits for Rainbow-style agents.
   """
-  layer = gym_lib.BasicDiscreteDomainNetwork(min_vals, max_vals, num_actions,
-                                             num_atoms)
+  layer = gym_lib.BasicDiscreteDomainNetwork(
+      min_vals, max_vals, num_actions, num_atoms
+  )
   return layer(state)
 
 
 @gin.configurable
 def cartpole_dqn_network(num_actions, network_type, state):
   """Builds the deep network used to compute the agent's Q-values.
 
@@ -116,35 +120,34 @@
   """
   model = gym_lib.CartpoleDQNNetwork(num_actions)
   net = model(state)
   return network_type(net.q_values)
 
 
 @gin.configurable
-def fourier_dqn_network(min_vals,
-                        max_vals,
-                        num_actions,
-                        state,
-                        fourier_basis_order=3):
+def fourier_dqn_network(
+    min_vals, max_vals, num_actions, state, fourier_basis_order=3
+):
   """Builds the function approximator used to compute the agent's Q-values.
 
   It uses FourierBasis features and a linear layer.
 
   Args:
     min_vals: float, minimum attainable values (must be same shape as `state`).
     max_vals: float, maximum attainable values (must be same shape as `state`).
     num_actions: int, number of actions.
     state: `tf.Tensor`, contains the agent's current state.
     fourier_basis_order: int, order of the Fourier basis functions.
 
   Returns:
     The Q-values for DQN-style agents or logits for Rainbow-style agents.
   """
-  model = gym_lib.FourierDQNNetwork(min_vals, max_vals, num_actions,
-                                    fourier_basis_order)
+  model = gym_lib.FourierDQNNetwork(
+      min_vals, max_vals, num_actions, fourier_basis_order
+  )
   return model(state).q_values
 
 
 def cartpole_fourier_dqn_network(num_actions, network_type, state):
   """Builds the function approximator used to compute the agent's Q-values.
 
   It uses the Fourier basis features and a linear function approximator.
@@ -159,16 +162,17 @@
   """
   model = gym_lib.CartpoleFourierDQNNetwork(num_actions)
   net = model(state)
   return network_type(net.q_values)
 
 
 @gin.configurable
-def cartpole_rainbow_network(num_actions, num_atoms, support, network_type,
-                             state):
+def cartpole_rainbow_network(
+    num_actions, num_atoms, support, network_type, state
+):
   """Build the deep network used to compute the agent's Q-value distributions.
 
   Args:
     num_actions: int, number of actions.
     num_atoms: int, the number of buckets of the value function distribution.
     support: tf.linspace, the support of the Q-value distribution.
     network_type: `namedtuple`, collection of expected values to return.
@@ -217,16 +221,17 @@
   """
   model = gym_lib.AcrobotFourierDQNNetwork(num_actions)
   net = model(state)
   return network_type(net.q_values)
 
 
 @gin.configurable
-def acrobot_rainbow_network(num_actions, num_atoms, support, network_type,
-                            state):
+def acrobot_rainbow_network(
+    num_actions, num_atoms, support, network_type, state
+):
   """Build the deep network used to compute the agent's Q-value distributions.
 
   Args:
     num_actions: int, number of actions.
     num_atoms: int, the number of buckets of the value function distribution.
     support: tf.linspace, the support of the Q-value distribution.
     network_type: `namedtuple`, collection of expected values to return.
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/logger.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from __future__ import division
 from __future__ import print_function
 
 import os
 import pickle
 
 from absl import logging
-
 import gin.tf
 import tensorflow as tf
 
 
 @gin.configurable
 class Logger(object):
   """Class for maintaining a dictionary of data to log."""
@@ -52,15 +51,16 @@
       tf.io.gfile.makedirs(logging_dir)
     except tf.errors.PermissionDeniedError:
       # If it already exists, ignore exception.
       pass
     if not tf.io.gfile.exists(logging_dir):
       logging.warning(
           'Could not create directory %s, logging will be disabled.',
-          logging_dir)
+          logging_dir,
+      )
       self._logging_enabled = False
       return
     self._logging_dir = logging_dir
 
   def __setitem__(self, key, value):
     """This method will set an entry at key with value in the dictionary.
 
@@ -77,31 +77,31 @@
     filename = '{}_{}'.format(filename_prefix, iteration_number)
     return os.path.join(self._logging_dir, filename)
 
   def log_to_file(self, filename_prefix, iteration_number):
     """Save the pickled dictionary to a file.
 
     Args:
-      filename_prefix: str, name of the file to use (without iteration
-        number).
+      filename_prefix: str, name of the file to use (without iteration number).
       iteration_number: int, the iteration number, appended to the end of
         filename_prefix.
     """
     if not self._logging_enabled:
       logging.warning('Logging is disabled.')
       return
     log_file = self._generate_filename(filename_prefix, iteration_number)
     with tf.io.gfile.GFile(log_file, 'w') as fout:
       pickle.dump(self.data, fout, protocol=pickle.HIGHEST_PROTOCOL)
     # After writing a checkpoint file, we garbage collect the log file
     # that is logs_duration versions old.
     stale_iteration_number = iteration_number - self._logs_duration
     if stale_iteration_number >= 0:
-      stale_file = self._generate_filename(filename_prefix,
-                                           stale_iteration_number)
+      stale_file = self._generate_filename(
+          filename_prefix, stale_iteration_number
+      )
       try:
         tf.io.gfile.remove(stale_file)
       except tf.errors.NotFoundError:
         # Ignore if file not found.
         pass
 
   def is_logging_enabled(self):
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/run_experiment.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/run_experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,102 +19,126 @@
 from __future__ import print_function
 
 import os
 import sys
 import time
 
 from absl import logging
-
 from dopamine.agents.dqn import dqn_agent
 from dopamine.agents.implicit_quantile import implicit_quantile_agent
 from dopamine.agents.rainbow import rainbow_agent
 from dopamine.discrete_domains import atari_lib
 from dopamine.discrete_domains import checkpointer
 from dopamine.discrete_domains import iteration_statistics
 from dopamine.discrete_domains import logger
 from dopamine.jax.agents.dqn import dqn_agent as jax_dqn_agent
 from dopamine.jax.agents.full_rainbow import full_rainbow_agent
 from dopamine.jax.agents.implicit_quantile import implicit_quantile_agent as jax_implicit_quantile_agent
 from dopamine.jax.agents.quantile import quantile_agent as jax_quantile_agent
 from dopamine.jax.agents.rainbow import rainbow_agent as jax_rainbow_agent
+from dopamine.labs.moes.agents import dqn_moe_agent
+from dopamine.labs.moes.agents import full_rainbow_moe_agent
+from dopamine.labs.moes.agents import rainbow_100k_moe_agent
 from dopamine.metrics import collector_dispatcher
 from dopamine.metrics import statistics_instance
 import gin.tf
 import numpy as np
 import tensorflow as tf
+import tqdm.auto as tqdm
 
 
 def load_gin_configs(gin_files, gin_bindings):
   """Loads gin configuration files.
 
   Args:
     gin_files: list, of paths to the gin configuration files for this
       experiment.
-    gin_bindings: list, of gin parameter bindings to override the values in
-      the config files.
+    gin_bindings: list, of gin parameter bindings to override the values in the
+      config files.
   """
-  gin.parse_config_files_and_bindings(gin_files,
-                                      bindings=gin_bindings,
-                                      skip_unknown=False)
+  gin.parse_config_files_and_bindings(
+      gin_files, bindings=gin_bindings, skip_unknown=False
+  )
 
 
 @gin.configurable
-def create_agent(sess, environment, agent_name=None, summary_writer=None,
-                 debug_mode=False):
+def create_agent(
+    sess, environment, agent_name=None, summary_writer=None, debug_mode=False
+):
   """Creates an agent.
 
   Args:
     sess: A `tf.compat.v1.Session` object for running associated ops.
     environment: A gym environment (e.g. Atari 2600).
     agent_name: str, name of the agent to create.
-    summary_writer: A Tensorflow summary writer to pass to the agent
-      for in-agent training statistics in Tensorboard.
+    summary_writer: A Tensorflow summary writer to pass to the agent for
+      in-agent training statistics in Tensorboard.
     debug_mode: bool, whether to output Tensorboard summaries. If set to true,
       the agent will output in-episode statistics to Tensorboard. Disabled by
       default as this results in slower training.
 
   Returns:
     agent: An RL agent.
 
   Raises:
     ValueError: If `agent_name` is not in supported list.
   """
   assert agent_name is not None
   if not debug_mode:
     summary_writer = None
   if agent_name.startswith('dqn'):
-    return dqn_agent.DQNAgent(sess, num_actions=environment.action_space.n,
-                              summary_writer=summary_writer)
+    return dqn_agent.DQNAgent(
+        sess,
+        num_actions=environment.action_space.n,
+        summary_writer=summary_writer,
+    )
   elif agent_name == 'rainbow':
     return rainbow_agent.RainbowAgent(
-        sess, num_actions=environment.action_space.n,
-        summary_writer=summary_writer)
+        sess,
+        num_actions=environment.action_space.n,
+        summary_writer=summary_writer,
+    )
   elif agent_name == 'implicit_quantile':
     return implicit_quantile_agent.ImplicitQuantileAgent(
-        sess, num_actions=environment.action_space.n,
-        summary_writer=summary_writer)
+        sess,
+        num_actions=environment.action_space.n,
+        summary_writer=summary_writer,
+    )
   elif agent_name == 'jax_dqn':
-    return jax_dqn_agent.JaxDQNAgent(num_actions=environment.action_space.n,
-                                     summary_writer=summary_writer)
+    return jax_dqn_agent.JaxDQNAgent(
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
   elif agent_name == 'jax_quantile':
     return jax_quantile_agent.JaxQuantileAgent(
-        num_actions=environment.action_space.n,
-        summary_writer=summary_writer)
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
   elif agent_name == 'jax_rainbow':
     return jax_rainbow_agent.JaxRainbowAgent(
-        num_actions=environment.action_space.n,
-        summary_writer=summary_writer)
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
   elif agent_name == 'full_rainbow':
     return full_rainbow_agent.JaxFullRainbowAgent(
-        num_actions=environment.action_space.n,
-        summary_writer=summary_writer)
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
   elif agent_name == 'jax_implicit_quantile':
     return jax_implicit_quantile_agent.JaxImplicitQuantileAgent(
-        num_actions=environment.action_space.n,
-        summary_writer=summary_writer)
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
+  elif agent_name == 'moe_dqn':
+    return dqn_moe_agent.DQNMoEAgent(
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
+  elif agent_name == 'moe_full_rainbow':
+    return full_rainbow_moe_agent.JaxFullRainbowMoEAgent(
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
+  elif agent_name == 'moe_der':
+    return rainbow_100k_moe_agent.Atari100kRainbowMoEAgent(
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
   else:
     raise ValueError('Unknown agent: {}'.format(agent_name))
 
 
 @gin.configurable
 def create_runner(base_dir, schedule='continuous_train_and_eval'):
   """Creates an experiment Runner.
@@ -156,28 +180,30 @@
   def create_agent(sess, environment):
     return dqn_agent.DQNAgent(sess, num_actions=environment.action_space.n)
   runner = Runner(base_dir, create_agent, atari_lib.create_atari_environment)
   runner.run()
   ```
   """
 
-  def __init__(self,
-               base_dir,
-               create_agent_fn,
-               create_environment_fn=atari_lib.create_atari_environment,
-               checkpoint_file_prefix='ckpt',
-               logging_file_prefix='log',
-               log_every_n=1,
-               num_iterations=200,
-               training_steps=250000,
-               evaluation_steps=125000,
-               max_steps_per_episode=27000,
-               clip_rewards=True,
-               use_legacy_logger=True,
-               fine_grained_print_to_console=True):
+  def __init__(
+      self,
+      base_dir,
+      create_agent_fn,
+      create_environment_fn=atari_lib.create_atari_environment,
+      checkpoint_file_prefix='ckpt',
+      logging_file_prefix='log',
+      log_every_n=1,
+      num_iterations=200,
+      training_steps=250000,
+      evaluation_steps=125000,
+      max_steps_per_episode=27000,
+      clip_rewards=True,
+      use_legacy_logger=True,
+      fine_grained_print_to_console=True,
+  ):
     """Initialize the Runner object in charge of running a full experiment.
 
     Args:
       base_dir: str, the base directory to host all required sub-directories.
       create_agent_fn: A function that takes as args a Tensorflow session and an
         environment, and returns an agent.
       create_environment_fn: A function which receives a problem name and
@@ -222,27 +248,30 @@
     self._environment = create_environment_fn()
     # The agent is now in charge of setting up the session.
     self._sess = None
     # We're using a bit of a hack in that we pass in _base_dir instead of an
     # actually SummaryWriter. This is because the agent is now in charge of the
     # session, but needs to create the SummaryWriter before creating the ops,
     # and in order to do so, it requires the base directory.
-    self._agent = create_agent_fn(self._sess, self._environment,
-                                  summary_writer=self._base_dir)
+    self._agent = create_agent_fn(
+        self._sess, self._environment, summary_writer=self._base_dir
+    )
     if hasattr(self._agent, '_sess'):
       self._sess = self._agent._sess
     self._summary_writer = self._agent.summary_writer
 
     self._initialize_checkpointer_and_maybe_resume(checkpoint_file_prefix)
 
     # Create a collector dispatcher for metrics reporting.
     self._collector_dispatcher = collector_dispatcher.CollectorDispatcher(
-        self._base_dir)
+        self._base_dir
+    )
     set_collector_dispatcher_fn = getattr(
-        self._agent, 'set_collector_dispatcher', None)
+        self._agent, 'set_collector_dispatcher', None
+    )
     if callable(set_collector_dispatcher_fn):
       set_collector_dispatcher_fn(self._collector_dispatcher)
 
   @property
   def _use_legacy_logger(self):
     if not hasattr(self, '_legacy_logger_enabled'):
       return True
@@ -262,15 +291,16 @@
 
   def _create_directories(self):
     """Create necessary sub-directories."""
     self._checkpoint_dir = os.path.join(self._base_dir, 'checkpoints')
     if self._use_legacy_logger:
       logging.warning(
           'DEPRECATION WARNING: Logger is being deprecated. '
-          'Please switch to CollectorDispatcher!')
+          'Please switch to CollectorDispatcher!'
+      )
       self._logger = logger.Logger(os.path.join(self._base_dir, 'logs'))
 
   def _initialize_checkpointer_and_maybe_resume(self, checkpoint_file_prefix):
     """Reloads the latest checkpoint if it exists.
 
     This method will first create a `Checkpointer` object and then call
     `checkpointer.get_latest_checkpoint_number` to determine if there is a valid
@@ -286,34 +316,40 @@
     Args:
       checkpoint_file_prefix: str, the checkpoint file prefix.
 
     Returns:
       start_iteration: int, the iteration number to start the experiment from.
       experiment_checkpointer: `Checkpointer` object for the experiment.
     """
-    self._checkpointer = checkpointer.Checkpointer(self._checkpoint_dir,
-                                                   checkpoint_file_prefix)
+    self._checkpointer = checkpointer.Checkpointer(
+        self._checkpoint_dir, checkpoint_file_prefix
+    )
     self._start_iteration = 0
     # Check if checkpoint exists. Note that the existence of checkpoint 0 means
     # that we have finished iteration 0 (so we will start from iteration 1).
     latest_checkpoint_version = checkpointer.get_latest_checkpoint_number(
-        self._checkpoint_dir)
+        self._checkpoint_dir
+    )
     if latest_checkpoint_version >= 0:
       experiment_data = self._checkpointer.load_checkpoint(
-          latest_checkpoint_version)
+          latest_checkpoint_version
+      )
       if self._agent.unbundle(
-          self._checkpoint_dir, latest_checkpoint_version, experiment_data):
+          self._checkpoint_dir, latest_checkpoint_version, experiment_data
+      ):
         if experiment_data is not None:
           assert 'logs' in experiment_data
           assert 'current_iteration' in experiment_data
           if self._use_legacy_logger:
             self._logger.data = experiment_data['logs']
           self._start_iteration = experiment_data['current_iteration'] + 1
-        logging.info('Reloaded checkpoint and will start from iteration %d',
-                     self._start_iteration)
+        logging.info(
+            'Reloaded checkpoint and will start from iteration %d',
+            self._start_iteration,
+        )
 
   def _initialize_episode(self):
     """Initialization for a new episode.
 
     Returns:
       action: int, the initial action chosen by the agent.
     """
@@ -349,15 +385,15 @@
   def _run_one_episode(self):
     """Executes a full trajectory of the agent interacting with the environment.
 
     Returns:
       The number of steps taken and the total reward.
     """
     step_number = 0
-    total_reward = 0.
+    total_reward = 0.0
 
     action = self._initialize_episode()
     is_terminal = False
 
     # Keep interacting until we reach a terminal state.
     while True:
       observation, reward, is_terminal = self._run_one_step(action)
@@ -365,16 +401,18 @@
       total_reward += reward
       step_number += 1
 
       if self._clip_rewards:
         # Perform reward clipping.
         reward = np.clip(reward, -1, 1)
 
-      if (self._environment.game_over or
-          step_number == self._max_steps_per_episode):
+      if (
+          self._environment.game_over
+          or step_number == self._max_steps_per_episode
+      ):
         # Stop the run loop once we reach the true end of episode.
         break
       elif is_terminal:
         # If we lose a life but the episode is not over, signal an artificial
         # end of episode to the agent.
         self._end_episode(reward, is_terminal)
         action = self._agent.begin_episode(observation)
@@ -399,31 +437,33 @@
 
     Returns:
       Tuple containing the number of steps taken in this phase (int), the sum of
         returns (float), and the number of episodes performed (int).
     """
     step_count = 0
     num_episodes = 0
-    sum_returns = 0.
+    sum_returns = 0.0
 
     while step_count < min_steps:
       episode_length, episode_return = self._run_one_episode()
       statistics.append({
           '{}_episode_lengths'.format(run_mode_str): episode_length,
-          '{}_episode_returns'.format(run_mode_str): episode_return
+          '{}_episode_returns'.format(run_mode_str): episode_return,
       })
       step_count += episode_length
       sum_returns += episode_return
       num_episodes += 1
       if self._fine_grained_print_to_console:
         # We use sys.stdout.write instead of logging so as to flush frequently
         # without generating a line break.
-        sys.stdout.write('Steps executed: {} '.format(step_count) +
-                         'Episode length: {} '.format(episode_length) +
-                         'Return: {}\r'.format(episode_return))
+        sys.stdout.write(
+            'Steps executed: {} '.format(step_count)
+            + 'Episode length: {} '.format(episode_length)
+            + 'Return: {}\r'.format(episode_return)
+        )
         sys.stdout.flush()
     return step_count, sum_returns, num_episodes
 
   def _run_train_phase(self, statistics):
     """Run training phase.
 
     Args:
@@ -435,25 +475,29 @@
       average_reward: float, The average reward generated in this phase.
       average_steps_per_second: float, The average number of steps per second.
     """
     # Perform the training phase, during which the agent learns.
     self._agent.eval_mode = False
     start_time = time.time()
     number_steps, sum_returns, num_episodes = self._run_one_phase(
-        self._training_steps, statistics, 'train')
+        self._training_steps, statistics, 'train'
+    )
     average_return = sum_returns / num_episodes if num_episodes > 0 else 0.0
     statistics.append({'train_average_return': average_return})
     time_delta = time.time() - start_time
     average_steps_per_second = number_steps / time_delta
     statistics.append(
-        {'train_average_steps_per_second': average_steps_per_second})
-    logging.info('Average undiscounted return per training episode: %.2f',
-                 average_return)
-    logging.info('Average training steps per second: %.2f',
-                 average_steps_per_second)
+        {'train_average_steps_per_second': average_steps_per_second}
+    )
+    logging.info(
+        'Average undiscounted return per training episode: %.2f', average_return
+    )
+    logging.info(
+        'Average training steps per second: %.2f', average_steps_per_second
+    )
     return num_episodes, average_return, average_steps_per_second
 
   def _run_eval_phase(self, statistics):
     """Run evaluation phase.
 
     Args:
       statistics: `IterationStatistics` object which records the experimental
@@ -462,18 +506,21 @@
     Returns:
       num_episodes: int, The number of episodes run in this phase.
       average_reward: float, The average reward generated in this phase.
     """
     # Perform the evaluation phase -- no learning.
     self._agent.eval_mode = True
     _, sum_returns, num_episodes = self._run_one_phase(
-        self._evaluation_steps, statistics, 'eval')
+        self._evaluation_steps, statistics, 'eval'
+    )
     average_return = sum_returns / num_episodes if num_episodes > 0 else 0.0
-    logging.info('Average undiscounted return per evaluation episode: %.2f',
-                 average_return)
+    logging.info(
+        'Average undiscounted return per evaluation episode: %.2f',
+        average_return,
+    )
     statistics.append({'eval_average_return': average_return})
     return num_episodes, average_return
 
   def _run_one_iteration(self, iteration):
     """Runs one iteration of agent/environment interaction.
 
     An iteration involves running several episodes until a certain number of
@@ -486,49 +533,56 @@
 
     Returns:
       A dict containing summary statistics for this iteration.
     """
     statistics = iteration_statistics.IterationStatistics()
     logging.info('Starting iteration %d', iteration)
     num_episodes_train, average_reward_train, average_steps_per_second = (
-        self._run_train_phase(statistics))
-    num_episodes_eval, average_reward_eval = self._run_eval_phase(
-        statistics)
+        self._run_train_phase(statistics)
+    )
+    num_episodes_eval, average_reward_eval = self._run_eval_phase(statistics)
 
     if self._has_collector_dispatcher:
       self._collector_dispatcher.write([
-          statistics_instance.StatisticsInstance('Train/NumEpisodes',
-                                                 num_episodes_train,
-                                                 iteration),
-          statistics_instance.StatisticsInstance('Train/AverageReturns',
-                                                 average_reward_train,
-                                                 iteration),
-          statistics_instance.StatisticsInstance('Train/AverageStepsPerSecond',
-                                                 average_steps_per_second,
-                                                 iteration),
-          statistics_instance.StatisticsInstance('Eval/NumEpisodes',
-                                                 num_episodes_eval,
-                                                 iteration),
-          statistics_instance.StatisticsInstance('Eval/AverageReturns',
-                                                 average_reward_eval,
-                                                 iteration),
+          statistics_instance.StatisticsInstance(
+              'Train/NumEpisodes', num_episodes_train, iteration
+          ),
+          statistics_instance.StatisticsInstance(
+              'Train/AverageReturns', average_reward_train, iteration
+          ),
+          statistics_instance.StatisticsInstance(
+              'Train/AverageStepsPerSecond', average_steps_per_second, iteration
+          ),
+          statistics_instance.StatisticsInstance(
+              'Eval/NumEpisodes', num_episodes_eval, iteration
+          ),
+          statistics_instance.StatisticsInstance(
+              'Eval/AverageReturns', average_reward_eval, iteration
+          ),
       ])
     if self._summary_writer is not None:
-      self._save_tensorboard_summaries(iteration, num_episodes_train,
-                                       average_reward_train, num_episodes_eval,
-                                       average_reward_eval,
-                                       average_steps_per_second)
+      self._save_tensorboard_summaries(
+          iteration,
+          num_episodes_train,
+          average_reward_train,
+          num_episodes_eval,
+          average_reward_eval,
+          average_steps_per_second,
+      )
     return statistics.data_lists
 
-  def _save_tensorboard_summaries(self, iteration,
-                                  num_episodes_train,
-                                  average_reward_train,
-                                  num_episodes_eval,
-                                  average_reward_eval,
-                                  average_steps_per_second):
+  def _save_tensorboard_summaries(
+      self,
+      iteration,
+      num_episodes_train,
+      average_reward_train,
+      num_episodes_eval,
+      average_reward_eval,
+      average_steps_per_second,
+  ):
     """Save statistics as tensorboard summaries.
 
     Args:
       iteration: int, The current iteration number.
       num_episodes_train: int, number of training episodes run.
       average_reward_train: float, The average training reward.
       num_episodes_eval: int, number of evaluation episodes run.
@@ -536,38 +590,51 @@
       average_steps_per_second: float, The average number of steps per second.
     """
     if self._summary_writer is None:
       return
 
     if self._sess is None:
       with self._summary_writer.as_default():
-        tf.summary.scalar('Train/NumEpisodes', num_episodes_train,
-                          step=iteration)
-        tf.summary.scalar('Train/AverageReturns', average_reward_train,
-                          step=iteration)
-        tf.summary.scalar('Train/AverageStepsPerSecond',
-                          average_steps_per_second, step=iteration)
+        tf.summary.scalar(
+            'Train/NumEpisodes', num_episodes_train, step=iteration
+        )
+        tf.summary.scalar(
+            'Train/AverageReturns', average_reward_train, step=iteration
+        )
+        tf.summary.scalar(
+            'Train/AverageStepsPerSecond',
+            average_steps_per_second,
+            step=iteration,
+        )
         tf.summary.scalar('Eval/NumEpisodes', num_episodes_eval, step=iteration)
-        tf.summary.scalar('Eval/AverageReturns', average_reward_eval,
-                          step=iteration)
+        tf.summary.scalar(
+            'Eval/AverageReturns', average_reward_eval, step=iteration
+        )
       self._summary_writer.flush()
     else:
-      summary = tf.compat.v1.Summary(value=[
-          tf.compat.v1.Summary.Value(
-              tag='Train/NumEpisodes', simple_value=num_episodes_train),
-          tf.compat.v1.Summary.Value(
-              tag='Train/AverageReturns', simple_value=average_reward_train),
-          tf.compat.v1.Summary.Value(
-              tag='Train/AverageStepsPerSecond',
-              simple_value=average_steps_per_second),
-          tf.compat.v1.Summary.Value(
-              tag='Eval/NumEpisodes', simple_value=num_episodes_eval),
-          tf.compat.v1.Summary.Value(
-              tag='Eval/AverageReturns', simple_value=average_reward_eval)
-      ])
+      summary = tf.compat.v1.Summary(
+          value=[
+              tf.compat.v1.Summary.Value(
+                  tag='Train/NumEpisodes', simple_value=num_episodes_train
+              ),
+              tf.compat.v1.Summary.Value(
+                  tag='Train/AverageReturns', simple_value=average_reward_train
+              ),
+              tf.compat.v1.Summary.Value(
+                  tag='Train/AverageStepsPerSecond',
+                  simple_value=average_steps_per_second,
+              ),
+              tf.compat.v1.Summary.Value(
+                  tag='Eval/NumEpisodes', simple_value=num_episodes_eval
+              ),
+              tf.compat.v1.Summary.Value(
+                  tag='Eval/AverageReturns', simple_value=average_reward_eval
+              ),
+          ]
+      )
       self._summary_writer.add_summary(summary, iteration)
 
   def _log_experiment(self, iteration, statistics):
     """Records the results of the current iteration.
 
     Args:
       iteration: int, iteration number.
@@ -582,31 +649,39 @@
 
   def _checkpoint_experiment(self, iteration):
     """Checkpoint experiment data.
 
     Args:
       iteration: int, iteration number for checkpointing.
     """
-    experiment_data = self._agent.bundle_and_checkpoint(self._checkpoint_dir,
-                                                        iteration)
+    experiment_data = self._agent.bundle_and_checkpoint(
+        self._checkpoint_dir, iteration
+    )
     if experiment_data:
       experiment_data['current_iteration'] = iteration
       if self._use_legacy_logger:
         experiment_data['logs'] = self._logger.data
       self._checkpointer.save_checkpoint(iteration, experiment_data)
 
   def run_experiment(self):
     """Runs a full experiment, spread over multiple iterations."""
     logging.info('Beginning training...')
     if self._num_iterations <= self._start_iteration:
-      logging.warning('num_iterations (%d) < start_iteration(%d)',
-                      self._num_iterations, self._start_iteration)
+      logging.warning(
+          'num_iterations (%d) < start_iteration(%d)',
+          self._num_iterations,
+          self._start_iteration,
+      )
       return
 
-    for iteration in range(self._start_iteration, self._num_iterations):
+    for iteration in tqdm.tqdm(
+        range(self._start_iteration, self._num_iterations),
+        initial=self._start_iteration,
+        total=self._num_iterations,
+    ):
       statistics = self._run_one_iteration(iteration)
       if self._use_legacy_logger:
         self._log_experiment(iteration, statistics)
       self._checkpoint_experiment(iteration)
       if self._has_collector_dispatcher:
         self._collector_dispatcher.flush()
     if self._summary_writer is not None:
@@ -620,28 +695,33 @@
   """Object that handles running experiments.
 
   The `TrainRunner` differs from the base `Runner` class in that it does not
   the evaluation phase. Checkpointing and logging for the train phase are
   preserved as before.
   """
 
-  def __init__(self, base_dir, create_agent_fn,
-               create_environment_fn=atari_lib.create_atari_environment):
+  def __init__(
+      self,
+      base_dir,
+      create_agent_fn,
+      create_environment_fn=atari_lib.create_atari_environment,
+  ):
     """Initialize the TrainRunner object in charge of running a full experiment.
 
     Args:
       base_dir: str, the base directory to host all required sub-directories.
       create_agent_fn: A function that takes as args a Tensorflow session and an
         environment, and returns an agent.
       create_environment_fn: A function which receives a problem name and
         creates a Gym environment for that problem (e.g. an Atari 2600 game).
     """
     logging.info('Creating TrainRunner ...')
-    super(TrainRunner, self).__init__(base_dir, create_agent_fn,
-                                      create_environment_fn)
+    super(TrainRunner, self).__init__(
+        base_dir, create_agent_fn, create_environment_fn
+    )
     self._agent.eval_mode = False
 
   def _run_one_iteration(self, iteration):
     """Runs one iteration of agent/environment interaction.
 
     An iteration involves running several episodes until a certain number of
     steps are obtained. This method differs from the `_run_one_iteration` method
@@ -652,51 +732,65 @@
         Tensorboard summaries.
 
     Returns:
       A dict containing summary statistics for this iteration.
     """
     statistics = iteration_statistics.IterationStatistics()
     num_episodes_train, average_reward_train, average_steps_per_second = (
-        self._run_train_phase(statistics))
+        self._run_train_phase(statistics)
+    )
 
     self._collector_dispatcher.write([
-        statistics_instance.StatisticsInstance('Train/NumEpisodes',
-                                               num_episodes_train,
-                                               iteration),
-        statistics_instance.StatisticsInstance('Train/AverageReturns',
-                                               average_reward_train,
-                                               iteration),
-        statistics_instance.StatisticsInstance('Train/AverageStepsPerSecond',
-                                               average_steps_per_second,
-                                               iteration),
+        statistics_instance.StatisticsInstance(
+            'Train/NumEpisodes', num_episodes_train, iteration
+        ),
+        statistics_instance.StatisticsInstance(
+            'Train/AverageReturns', average_reward_train, iteration
+        ),
+        statistics_instance.StatisticsInstance(
+            'Train/AverageStepsPerSecond', average_steps_per_second, iteration
+        ),
     ])
     if self._summary_writer is not None:
-      self._save_tensorboard_summaries(iteration, num_episodes_train,
-                                       average_reward_train,
-                                       average_steps_per_second)
+      self._save_tensorboard_summaries(
+          iteration,
+          num_episodes_train,
+          average_reward_train,
+          average_steps_per_second,
+      )
     return statistics.data_lists
 
-  def _save_tensorboard_summaries(self, iteration, num_episodes,
-                                  average_reward, average_steps_per_second):
+  def _save_tensorboard_summaries(
+      self, iteration, num_episodes, average_reward, average_steps_per_second
+  ):
     """Save statistics as tensorboard summaries."""
     if self._summary_writer is None:
       return
 
     if self._sess is None:
       with self._summary_writer.as_default():
         tf.summary.scalar('Train/NumEpisodes', num_episodes, step=iteration)
-        tf.summary.scalar('Train/AverageReturns', average_reward,
-                          step=iteration)
-        tf.summary.scalar('Train/AverageStepsPerSecond',
-                          average_steps_per_second, step=iteration)
+        tf.summary.scalar(
+            'Train/AverageReturns', average_reward, step=iteration
+        )
+        tf.summary.scalar(
+            'Train/AverageStepsPerSecond',
+            average_steps_per_second,
+            step=iteration,
+        )
       self._summary_writer.flush()
     else:
-      summary = tf.compat.v1.Summary(value=[
-          tf.compat.v1.Summary.Value(
-              tag='Train/NumEpisodes', simple_value=num_episodes),
-          tf.compat.v1.Summary.Value(
-              tag='Train/AverageReturns', simple_value=average_reward),
-          tf.compat.v1.Summary.Value(
-              tag='Train/AverageStepsPerSecond',
-              simple_value=average_steps_per_second),
-      ])
+      summary = tf.compat.v1.Summary(
+          value=[
+              tf.compat.v1.Summary.Value(
+                  tag='Train/NumEpisodes', simple_value=num_episodes
+              ),
+              tf.compat.v1.Summary.Value(
+                  tag='Train/AverageReturns', simple_value=average_reward
+              ),
+              tf.compat.v1.Summary.Value(
+                  tag='Train/AverageStepsPerSecond',
+                  simple_value=average_steps_per_second,
+              ),
+          ]
+      )
       self._summary_writer.add_summary(summary, iteration)
```

### Comparing `dopamine_rl-4.0.6/dopamine/discrete_domains/train.py` & `dopamine_rl-4.0.7/dopamine/discrete_domains/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,30 @@
 from absl import flags
 from absl import logging
 
 from dopamine.discrete_domains import run_experiment
 import tensorflow as tf
 
 
-flags.DEFINE_string('base_dir', None,
-                    'Base directory to host all required sub-directories.')
+flags.DEFINE_string(
+    'base_dir', None, 'Base directory to host all required sub-directories.'
+)
 flags.DEFINE_multi_string(
-    'gin_files', [], 'List of paths to gin configuration files (e.g.'
-    '"dopamine/agents/dqn/dqn.gin").')
+    'gin_files',
+    [],
+    'List of paths to gin configuration files (e.g.'
+    '"dopamine/agents/dqn/dqn.gin").',
+)
 flags.DEFINE_multi_string(
-    'gin_bindings', [],
+    'gin_bindings',
+    [],
     'Gin bindings to override the values set in the config files '
     '(e.g. "DQNAgent.epsilon_train=0.1",'
-    '      "create_environment.game_name="Pong"").')
+    '      "create_environment.game_name="Pong"").',
+)
 
 
 FLAGS = flags.FLAGS
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/dqn/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/dqn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/dqn/dqn_agent.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/dqn/dqn_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,34 +10,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Compact implementation of a DQN agent in JAx."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import collections
 import functools
 import inspect
 import math
 import time
 
 from absl import logging
-
 from dopamine.agents.dqn import dqn_agent
 from dopamine.jax import losses
 from dopamine.jax import networks
 from dopamine.metrics import statistics_instance
 from dopamine.replay_memory import circular_replay_buffer
 from dopamine.replay_memory import prioritized_replay_buffer
-from flax import core
-from flax.training import checkpoints
 import gin
 import jax
 import jax.numpy as jnp
 import numpy as onp
 import optax
 import tensorflow as tf
 
@@ -45,16 +38,22 @@
 NATURE_DQN_OBSERVATION_SHAPE = dqn_agent.NATURE_DQN_OBSERVATION_SHAPE
 NATURE_DQN_DTYPE = jnp.uint8
 NATURE_DQN_STACK_SIZE = dqn_agent.NATURE_DQN_STACK_SIZE
 identity_epsilon = dqn_agent.identity_epsilon
 
 
 @gin.configurable
-def create_optimizer(name='adam', learning_rate=6.25e-5, beta1=0.9, beta2=0.999,
-                     eps=1.5e-4, centered=False):
+def create_optimizer(
+    name='adam',
+    learning_rate=6.25e-5,
+    beta1=0.9,
+    beta2=0.999,
+    eps=1.5e-4,
+    centered=False,
+):
   """Create an optimizer for training.
 
   Currently, only the Adam and RMSProp optimizers are supported.
 
   Args:
     name: str, name of the optimizer to create.
     learning_rate: float, learning rate to use in the optimizer.
@@ -63,58 +62,75 @@
     eps: float, epsilon parameter for the optimizer.
     centered: bool, centered parameter for RMSProp.
 
   Returns:
     An optax optimizer.
   """
   if name == 'adam':
-    logging.info('Creating Adam optimizer with settings lr=%f, beta1=%f, '
-                 'beta2=%f, eps=%f', learning_rate, beta1, beta2, eps)
+    logging.info(
+        'Creating Adam optimizer with settings lr=%f, beta1=%f, '
+        'beta2=%f, eps=%f',
+        learning_rate,
+        beta1,
+        beta2,
+        eps,
+    )
     return optax.adam(learning_rate, b1=beta1, b2=beta2, eps=eps)
   elif name == 'rmsprop':
-    logging.info('Creating RMSProp optimizer with settings lr=%f, beta2=%f, '
-                 'eps=%f', learning_rate, beta2, eps)
-    return optax.rmsprop(learning_rate, decay=beta2, eps=eps,
-                         centered=centered)
+    logging.info(
+        'Creating RMSProp optimizer with settings lr=%f, beta2=%f, eps=%f',
+        learning_rate,
+        beta2,
+        eps,
+    )
+    return optax.rmsprop(learning_rate, decay=beta2, eps=eps, centered=centered)
   elif name == 'sgd':
-    logging.info('Creating SGD optimizer with settings '
-                 'lr=%f', learning_rate)
+    logging.info('Creating SGD optimizer with settings lr=%f', learning_rate)
     return optax.sgd(learning_rate)
   else:
     raise ValueError('Unsupported optimizer {}'.format(name))
 
 
 @functools.partial(jax.jit, static_argnums=(0, 3, 10, 11))
-def train(network_def, online_params, target_params, optimizer, optimizer_state,
-          states, actions, next_states, rewards, terminals, cumulative_gamma,
-          loss_type='mse'):
+def train(
+    network_def,
+    online_params,
+    target_params,
+    optimizer,
+    optimizer_state,
+    states,
+    actions,
+    next_states,
+    rewards,
+    terminals,
+    cumulative_gamma,
+    loss_type='mse',
+):
   """Run the training step."""
+
   def loss_fn(params, target):
     def q_online(state):
       return network_def.apply(params, state)
 
     q_values = jax.vmap(q_online)(states).q_values
     q_values = jnp.squeeze(q_values)
     replay_chosen_q = jax.vmap(lambda x, y: x[y])(q_values, actions)
     if loss_type == 'huber':
       return jnp.mean(jax.vmap(losses.huber_loss)(target, replay_chosen_q))
     return jnp.mean(jax.vmap(losses.mse_loss)(target, replay_chosen_q))
 
   def q_target(state):
     return network_def.apply(target_params, state)
 
-  target = target_q(q_target,
-                    next_states,
-                    rewards,
-                    terminals,
-                    cumulative_gamma)
+  target = target_q(q_target, next_states, rewards, terminals, cumulative_gamma)
   grad_fn = jax.value_and_grad(loss_fn)
   loss, grad = grad_fn(online_params, target)
-  updates, optimizer_state = optimizer.update(grad, optimizer_state,
-                                              params=online_params)
+  updates, optimizer_state = optimizer.update(
+      grad, optimizer_state, params=online_params
+  )
   online_params = optax.apply_updates(online_params, updates)
   return optimizer_state, online_params, loss
 
 
 def target_q(target_network, next_states, rewards, terminals, cumulative_gamma):
   """Compute the target Q-value."""
   q_vals = jax.vmap(target_network, in_axes=(0))(next_states).q_values
@@ -123,16 +139,17 @@
   # Calculate the Bellman target value.
   #   Q_t = R_t + \gamma^N * Q'_t+1
   # where,
   #   Q'_t+1 = \argmax_a Q(S_t+1, a)
   #          (or) 0 if S_t is a terminal state,
   # and
   #   N is the update horizon (by default, N=1).
-  return jax.lax.stop_gradient(rewards + cumulative_gamma * replay_next_qt_max *
-                               (1. - terminals))
+  return jax.lax.stop_gradient(
+      rewards + cumulative_gamma * replay_next_qt_max * (1.0 - terminals)
+  )
 
 
 @gin.configurable
 @functools.partial(jax.jit, static_argnums=(0, 2, 3))
 def linearly_decaying_epsilon(decay_period, step, warmup_steps, epsilon):
   """Returns the current epsilon for the agent's epsilon-greedy policy.
 
@@ -149,22 +166,33 @@
     epsilon: float, the final value to which to decay the epsilon parameter.
 
   Returns:
     A float, the current epsilon value computed according to the schedule.
   """
   steps_left = decay_period + warmup_steps - step
   bonus = (1.0 - epsilon) * steps_left / decay_period
-  bonus = jnp.clip(bonus, 0., 1. - epsilon)
+  bonus = jnp.clip(bonus, 0.0, 1.0 - epsilon)
   return epsilon + bonus
 
 
 @functools.partial(jax.jit, static_argnums=(0, 4, 5, 6, 7, 8, 10, 11))
-def select_action(network_def, params, state, rng, num_actions, eval_mode,
-                  epsilon_eval, epsilon_train, epsilon_decay_period,
-                  training_steps, min_replay_history, epsilon_fn):
+def select_action(
+    network_def,
+    params,
+    state,
+    rng,
+    num_actions,
+    eval_mode,
+    epsilon_eval,
+    epsilon_train,
+    epsilon_decay_period,
+    training_steps,
+    min_replay_history,
+    epsilon_fn,
+):
   """Select an action from the set of available actions.
 
   Chooses an action randomly with probability self._calculate_epsilon(), and
   otherwise acts greedily according to the current Q-value estimates.
 
   Args:
     network_def: Linen Module to use for inference.
@@ -182,56 +210,64 @@
       (static_argnum).
     epsilon_fn: function used to calculate epsilon value (static_argnum).
 
   Returns:
     rng: Jax random number generator.
     action: int, the selected action.
   """
-  epsilon = jnp.where(eval_mode,
-                      epsilon_eval,
-                      epsilon_fn(epsilon_decay_period,
-                                 training_steps,
-                                 min_replay_history,
-                                 epsilon_train))
+  epsilon = jnp.where(
+      eval_mode,
+      epsilon_eval,
+      epsilon_fn(
+          epsilon_decay_period,
+          training_steps,
+          min_replay_history,
+          epsilon_train,
+      ),
+  )
 
   rng, rng1, rng2 = jax.random.split(rng, num=3)
   p = jax.random.uniform(rng1)
-  return rng, jnp.where(p <= epsilon,
-                        jax.random.randint(rng2, (), 0, num_actions),
-                        jnp.argmax(network_def.apply(params, state).q_values))
+  return rng, jnp.where(
+      p <= epsilon,
+      jax.random.randint(rng2, (), 0, num_actions),
+      jnp.argmax(network_def.apply(params, state).q_values),
+  )
 
 
 @gin.configurable
 class JaxDQNAgent(object):
   """A JAX implementation of the DQN agent."""
 
-  def __init__(self,
-               num_actions,
-               observation_shape=NATURE_DQN_OBSERVATION_SHAPE,
-               observation_dtype=NATURE_DQN_DTYPE,
-               stack_size=NATURE_DQN_STACK_SIZE,
-               network=networks.NatureDQNNetwork,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=20000,
-               update_period=4,
-               target_update_period=8000,
-               epsilon_fn=linearly_decaying_epsilon,
-               epsilon_train=0.01,
-               epsilon_eval=0.001,
-               epsilon_decay_period=250000,
-               eval_mode=False,
-               optimizer='adam',
-               summary_writer=None,
-               summary_writing_frequency=500,
-               allow_partial_reload=False,
-               seed=None,
-               loss_type='mse',
-               preprocess_fn=None,
-               collector_allowlist=('tensorboard',)):
+  def __init__(
+      self,
+      num_actions,
+      observation_shape=NATURE_DQN_OBSERVATION_SHAPE,
+      observation_dtype=NATURE_DQN_DTYPE,
+      stack_size=NATURE_DQN_STACK_SIZE,
+      network=networks.NatureDQNNetwork,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=20000,
+      update_period=4,
+      target_update_period=8000,
+      epsilon_fn=linearly_decaying_epsilon,
+      epsilon_train=0.01,
+      epsilon_eval=0.001,
+      epsilon_decay_period=250000,
+      eval_mode=False,
+      optimizer='adam',
+      summary_writer=None,
+      summary_writing_frequency=500,
+      allow_partial_reload=False,
+      seed=None,
+      loss_type='mse',
+      preprocess_fn=None,
+      collector_allowlist=('tensorboard',),
+  ):
     """Initializes the agent and constructs the necessary components.
 
     Note: We are using the Adam optimizer by default for JaxDQN, which differs
           from the original NatureDQN and the dopamine TensorFlow version. In
           the experiments we have ran, we have found that using Adam yields
           improved training performance.
 
@@ -244,17 +280,17 @@
       gamma: float, discount factor with the usual RL meaning.
       update_horizon: int, horizon at which updates are performed, the 'n' in
         n-step update.
       min_replay_history: int, number of transitions that should be experienced
         before the agent begins training its value function.
       update_period: int, period between DQN updates.
       target_update_period: int, update period for the target network.
-      epsilon_fn: function expecting 4 parameters:
-        (decay_period, step, warmup_steps, epsilon). This function should return
-        the epsilon value used for exploration during training.
+      epsilon_fn: function expecting 4 parameters: (decay_period, step,
+        warmup_steps, epsilon). This function should return the epsilon value
+        used for exploration during training.
       epsilon_train: float, the value to which the agent's epsilon is eventually
         decayed during training.
       epsilon_eval: float, epsilon used when evaluating the agent.
       epsilon_decay_period: int, length of the epsilon decay schedule.
       eval_mode: bool, True for evaluation and False for training.
       optimizer: str, name of optimizer to use.
       summary_writer: SummaryWriter object for outputting training statistics.
@@ -263,24 +299,26 @@
       summary_writing_frequency: int, frequency with which summaries will be
         written. Lower values will result in slower training.
       allow_partial_reload: bool, whether we allow reloading a partial agent
         (for instance, only the network parameters).
       seed: int, a seed for DQN's internal RNG, used for initialization and
         sampling actions. If None, will use the current time in nanoseconds.
       loss_type: str, whether to use Huber or MSE loss during training.
-      preprocess_fn: function expecting the input state as parameter which
-        it preprocesses (such as normalizing the pixel values between 0 and 1)
+      preprocess_fn: function expecting the input state as parameter which it
+        preprocesses (such as normalizing the pixel values between 0 and 1)
         before passing it to the Q-network. Defaults to None.
       collector_allowlist: list of str, if using CollectorDispatcher, this can
         be used to specify which Collectors to log to.
     """
     assert isinstance(observation_shape, tuple)
     seed = int(time.time() * 1e6) if seed is None else seed
-    logging.info('Creating %s agent with the following parameters:',
-                 self.__class__.__name__)
+    logging.info(
+        'Creating %s agent with the following parameters:',
+        self.__class__.__name__,
+    )
     logging.info('\t gamma: %f', gamma)
     logging.info('\t update_horizon: %f', update_horizon)
     logging.info('\t min_replay_history: %d', min_replay_history)
     logging.info('\t update_period: %d', update_period)
     logging.info('\t target_update_period: %d', target_update_period)
     logging.info('\t epsilon_train: %f', epsilon_train)
     logging.info('\t epsilon_eval: %f', epsilon_eval)
@@ -296,16 +334,17 @@
     self.observation_shape = tuple(observation_shape)
     self.observation_dtype = observation_dtype
     self.stack_size = stack_size
     if preprocess_fn is None:
       self.network_def = network(num_actions=num_actions)
       self.preprocess_fn = networks.identity_preprocess_fn
     else:
-      self.network_def = network(num_actions=num_actions,
-                                 inputs_preprocessed=True)
+      self.network_def = network(
+          num_actions=num_actions, inputs_preprocessed=True
+      )
       self.preprocess_fn = preprocess_fn
     self.gamma = gamma
     self.update_horizon = update_horizon
     self.cumulative_gamma = math.pow(gamma, update_horizon)
     self.min_replay_history = min_replay_history
     self.target_update_period = target_update_period
     self.epsilon_fn = epsilon_fn
@@ -338,27 +377,29 @@
     # Variables to be initialized by the agent once it interacts with the
     # environment.
     self._observation = None
     self._last_observation = None
 
   def _build_networks_and_optimizer(self):
     self._rng, rng = jax.random.split(self._rng)
-    self.online_params = self.network_def.init(rng, x=self.state)
+    state = self.preprocess_fn(self.state)
+    self.online_params = self.network_def.init(rng, x=state)
     self.optimizer = create_optimizer(self._optimizer_name)
     self.optimizer_state = self.optimizer.init(self.online_params)
     self.target_network_params = self.online_params
 
   def _build_replay_buffer(self):
     """Creates the replay buffer used by the agent."""
     return circular_replay_buffer.OutOfGraphReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
-        observation_dtype=self.observation_dtype)
+        observation_dtype=self.observation_dtype,
+    )
 
   def _sample_from_replay_buffer(self):
     samples = self._replay.sample_transition_batch()
     types = self._replay.get_transition_elements()
     self.replay_elements = collections.OrderedDict()
     for element, element_type in zip(samples, types):
       self.replay_elements[element_type.name] = element
@@ -398,26 +439,28 @@
     """
     self._reset_state()
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._train_step()
 
-    self._rng, self.action = select_action(self.network_def,
-                                           self.online_params,
-                                           self.preprocess_fn(self.state),
-                                           self._rng,
-                                           self.num_actions,
-                                           self.eval_mode,
-                                           self.epsilon_eval,
-                                           self.epsilon_train,
-                                           self.epsilon_decay_period,
-                                           self.training_steps,
-                                           self.min_replay_history,
-                                           self.epsilon_fn)
+    self._rng, self.action = select_action(
+        self.network_def,
+        self.online_params,
+        self.preprocess_fn(self.state),
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+    )
     self.action = onp.asarray(self.action)
     return self.action
 
   def step(self, reward, observation):
     """Records the most recent transition and returns the agent's next action.
 
     We store the observation of the last time step since we want to store it
@@ -433,26 +476,28 @@
     self._last_observation = self._observation
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._store_transition(self._last_observation, self.action, reward, False)
       self._train_step()
 
-    self._rng, self.action = select_action(self.network_def,
-                                           self.online_params,
-                                           self.preprocess_fn(self.state),
-                                           self._rng,
-                                           self.num_actions,
-                                           self.eval_mode,
-                                           self.epsilon_eval,
-                                           self.epsilon_train,
-                                           self.epsilon_decay_period,
-                                           self.training_steps,
-                                           self.min_replay_history,
-                                           self.epsilon_fn)
+    self._rng, self.action = select_action(
+        self.network_def,
+        self.online_params,
+        self.preprocess_fn(self.state),
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+    )
     self.action = onp.asarray(self.action)
     return self.action
 
   def end_episode(self, reward, terminal=True):
     """Signals the end of the episode to the agent.
 
     We store the observation of the current time step, which is the last
@@ -462,18 +507,20 @@
       reward: float, the last reward from the environment.
       terminal: bool, whether the last state-action led to a terminal state.
     """
     if not self.eval_mode:
       argspec = inspect.getfullargspec(self._store_transition)
       if 'episode_end' in argspec.args or 'episode_end' in argspec.kwonlyargs:
         self._store_transition(
-            self._observation, self.action, reward, terminal, episode_end=True)
+            self._observation, self.action, reward, terminal, episode_end=True
+        )
       else:
         logging.warning(
-            '_store_transition function doesn\'t have episode_end arg.')
+            "_store_transition function doesn't have episode_end arg."
+        )
         self._store_transition(self._observation, self.action, reward, terminal)
 
   def _train_step(self):
     """Runs a single training step.
 
     Runs training if both:
       (1) A minimum number of frames have been added to the replay buffer.
@@ -497,40 +544,48 @@
             self.optimizer_state,
             states,
             self.replay_elements['action'],
             next_states,
             self.replay_elements['reward'],
             self.replay_elements['terminal'],
             self.cumulative_gamma,
-            self._loss_type)
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+            self._loss_type,
+        )
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
           with self.summary_writer.as_default():
             tf.summary.scalar('HuberLoss', loss, step=self.training_steps)
           self.summary_writer.flush()
           if hasattr(self, 'collector_dispatcher'):
             self.collector_dispatcher.write(
-                [statistics_instance.StatisticsInstance(
-                    'Loss', onp.asarray(loss), step=self.training_steps),
-                 ],
-                collector_allowlist=self._collector_allowlist)
+                [
+                    statistics_instance.StatisticsInstance(
+                        'Loss', onp.asarray(loss), step=self.training_steps
+                    ),
+                ],
+                collector_allowlist=self._collector_allowlist,
+            )
       if self.training_steps % self.target_update_period == 0:
         self._sync_weights()
 
     self.training_steps += 1
 
-  def _store_transition(self,
-                        last_observation,
-                        action,
-                        reward,
-                        is_terminal,
-                        *args,
-                        priority=None,
-                        episode_end=False):
+  def _store_transition(
+      self,
+      last_observation,
+      action,
+      reward,
+      is_terminal,
+      *args,
+      priority=None,
+      episode_end=False
+  ):
     """Stores a transition when in training mode.
 
     Stores the following tuple in the replay buffer (last_observation, action,
     reward, is_terminal, priority).
 
     Args:
       last_observation: Last observation, type determined via observation_type
@@ -540,35 +595,37 @@
       is_terminal: Boolean indicating if the current state is a terminal state.
       *args: Any, other items to be added to the replay buffer.
       priority: Float. Priority of sampling the transition. If None, the default
         priority will be used. If replay scheme is uniform, the default priority
         is 1. If the replay scheme is prioritized, the default priority is the
         maximum ever seen [Schaul et al., 2015].
       episode_end: bool, whether this transition is the last for the episode.
-        This can be different than terminal when ending the episode because
-        of a timeout, for example.
+        This can be different than terminal when ending the episode because of a
+        timeout, for example.
     """
     is_prioritized = isinstance(
         self._replay,
-        prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer)
+        prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer,
+    )
     if is_prioritized and priority is None:
       if self._replay_scheme == 'uniform':
-        priority = 1.
+        priority = 1.0
       else:
         priority = self._replay.sum_tree.max_recorded_priority
 
     if not self.eval_mode:
       self._replay.add(
           last_observation,
           action,
           reward,
           is_terminal,
           *args,
           priority=priority,
-          episode_end=episode_end)
+          episode_end=episode_end
+      )
 
   def bundle_and_checkpoint(self, checkpoint_dir, iteration_number):
     """Returns a self-contained bundle of the agent's state.
 
     This is used for checkpointing. It will return a dictionary containing all
     non-TensorFlow objects (to be saved into a file by the caller), and it saves
     all TensorFlow objects into a checkpoint file.
@@ -587,15 +644,15 @@
     # Checkpoint the out-of-graph replay buffer.
     self._replay.save(checkpoint_dir, iteration_number)
     bundle_dictionary = {
         'state': self.state,
         'training_steps': self.training_steps,
         'online_params': self.online_params,
         'optimizer_state': self.optimizer_state,
-        'target_params': self.target_network_params
+        'target_params': self.target_network_params,
     }
     return bundle_dictionary
 
   def unbundle(self, checkpoint_dir, iteration_number, bundle_dictionary):
     """Restores the agent from a checkpoint.
 
     Restores the agent's Python objects to those specified in bundle_dictionary,
@@ -603,16 +660,16 @@
     checkpoint_dir. If the checkpoint_dir does not exist, will not reset the
       agent's state.
 
     Args:
       checkpoint_dir: str, path to the checkpoint saved.
       iteration_number: int, checkpoint version, used when restoring the replay
         buffer.
-      bundle_dictionary: dict, containing additional Python objects owned by
-        the agent.
+      bundle_dictionary: dict, containing additional Python objects owned by the
+        agent.
 
     Returns:
       bool, True if unbundling was successful.
     """
     try:
       # self._replay.load() will throw a NotFoundError if it does not find all
       # the necessary files.
@@ -621,26 +678,16 @@
       if not self.allow_partial_reload:
         # If we don't allow partial reloads, we will return False.
         return False
       logging.warning('Unable to reload replay buffer!')
     if bundle_dictionary is not None:
       self.state = bundle_dictionary['state']
       self.training_steps = bundle_dictionary['training_steps']
-      if isinstance(bundle_dictionary['online_params'], core.FrozenDict):
-        self.online_params = bundle_dictionary['online_params']
-        self.target_network_params = bundle_dictionary['target_params']
-      else:  # Load pre-linen checkpoint.
-        self.online_params = core.FrozenDict({
-            'params': checkpoints.convert_pre_linen(
-                bundle_dictionary['online_params']).unfreeze()
-        })
-        self.target_network_params = core.FrozenDict({
-            'params': checkpoints.convert_pre_linen(
-                bundle_dictionary['target_params']).unfreeze()
-        })
+      self.online_params = bundle_dictionary['online_params']
+      self.target_network_params = bundle_dictionary['target_params']
       # We load the optimizer state or recreate it with the new online weights.
       if 'optimizer_state' in bundle_dictionary:
         self.optimizer_state = bundle_dictionary['optimizer_state']
       else:
         self.optimizer_state = self.optimizer.init(self.online_params)
     elif not self.allow_partial_reload:
       return False
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/full_rainbow/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,102 +40,180 @@
 import jax
 import jax.numpy as jnp
 import numpy as onp
 import optax
 import tensorflow as tf
 
 
+@gin.configurable
+def zero_epsilon(
+    unused_decay_period, unused_step, unused_warmup_steps, unused_epsilon
+):
+  return 0.0
+
+
 @functools.partial(jax.jit, static_argnums=(0, 4, 5, 6, 7, 8, 10, 11))
-def select_action(network_def, params, state, rng, num_actions, eval_mode,
-                  epsilon_eval, epsilon_train, epsilon_decay_period,
-                  training_steps, min_replay_history, epsilon_fn, support):
+def select_action(
+    network_def,
+    params,
+    state,
+    rng,
+    num_actions,
+    eval_mode,
+    epsilon_eval,
+    epsilon_train,
+    epsilon_decay_period,
+    training_steps,
+    min_replay_history,
+    epsilon_fn,
+    support,
+):
   """Select an action from the set of available actions."""
   epsilon = jnp.where(
-      eval_mode, epsilon_eval,
-      epsilon_fn(epsilon_decay_period, training_steps, min_replay_history,
-                 epsilon_train))
+      eval_mode,
+      epsilon_eval,
+      epsilon_fn(
+          epsilon_decay_period,
+          training_steps,
+          min_replay_history,
+          epsilon_train,
+      ),
+  )
 
   rng, rng1, rng2, rng3 = jax.random.split(rng, num=4)
   p = jax.random.uniform(rng1)
   best_actions = jnp.argmax(
-      network_def.apply(params, state, key=rng2, eval_mode=eval_mode,
-                        support=support).q_values)
-  return rng, jnp.where(p <= epsilon,
-                        jax.random.randint(rng3, (), 0, num_actions),
-                        best_actions)
+      network_def.apply(
+          params, state, key=rng2, eval_mode=eval_mode, support=support
+      ).q_values
+  )
+  return rng, jnp.where(
+      p <= epsilon, jax.random.randint(rng3, (), 0, num_actions), best_actions
+  )
 
 
 @functools.partial(jax.vmap, in_axes=(None, 0, None))
 def get_logits(model, states, rng):
   return model(states, key=rng).logits
 
 
 @functools.partial(jax.vmap, in_axes=(None, 0, None))
 def get_q_values(model, states, rng):
   return model(states, key=rng).q_values
 
 
-@functools.partial(jax.jit, static_argnums=(0, 3, 12, 13, 14))
-def train(network_def, online_params, target_params, optimizer, optimizer_state,
-          states, actions, next_states, rewards, terminals, loss_weights,
-          support, cumulative_gamma, double_dqn, distributional, rng):
+@functools.partial(
+    jax.jit,
+    static_argnames=(
+        'network_def',
+        'optimizer',
+        'cumulative_gamma',
+        'double_dqn',
+        'distributional',
+        'mse_loss',
+    ),
+)
+def train(
+    network_def,
+    online_params,
+    target_params,
+    optimizer,
+    optimizer_state,
+    states,
+    actions,
+    next_states,
+    rewards,
+    terminals,
+    loss_weights,
+    support,
+    cumulative_gamma,
+    double_dqn,
+    distributional,
+    mse_loss,
+    rng,
+):
   """Run a training step."""
 
   # Split the current rng into 2 for updating the rng after this call
   rng, rng1, rng2 = jax.random.split(rng, num=3)
 
   def q_online(state, key):
     return network_def.apply(online_params, state, key=key, support=support)
 
   def q_target(state, key):
     return network_def.apply(target_params, state, key=key, support=support)
 
   def loss_fn(params, target, loss_multipliers):
     """Computes the distributional loss for C51 or huber loss for DQN."""
+
     def q_online(state, key):
       return network_def.apply(params, state, key=key, support=support)
 
     if distributional:
       logits = get_logits(q_online, states, rng)
       logits = jnp.squeeze(logits)
       # Fetch the logits for its selected action. We use vmap to perform this
       # indexing across the batch.
       chosen_action_logits = jax.vmap(lambda x, y: x[y])(logits, actions)
       loss = jax.vmap(losses.softmax_cross_entropy_loss_with_logits)(
-          target, chosen_action_logits)
+          target, chosen_action_logits
+      )
     else:
       q_values = get_q_values(q_online, states, rng)
       q_values = jnp.squeeze(q_values)
       replay_chosen_q = jax.vmap(lambda x, y: x[y])(q_values, actions)
-      loss = jax.vmap(losses.huber_loss)(target, replay_chosen_q)
+
+      loss = losses.mse_loss if mse_loss else losses.huber_loss
+      loss = jax.vmap(loss)(target, replay_chosen_q)
 
     mean_loss = jnp.mean(loss_multipliers * loss)
     return mean_loss, loss
 
   # Use the weighted mean loss for gradient computation.
   grad_fn = jax.value_and_grad(loss_fn, has_aux=True)
-  target = target_output(q_online, q_target, next_states, rewards,
-                         terminals, support, cumulative_gamma, double_dqn,
-                         distributional, rng1)
+  target = target_output(
+      q_online,
+      q_target,
+      next_states,
+      rewards,
+      terminals,
+      support,
+      cumulative_gamma,
+      double_dqn,
+      distributional,
+      rng1,
+  )
 
   # Get the unweighted loss without taking its mean for updating priorities.
   (mean_loss, loss), grad = grad_fn(online_params, target, loss_weights)
-  updates, optimizer_state = optimizer.update(grad, optimizer_state,
-                                              params=online_params)
+  updates, optimizer_state = optimizer.update(
+      grad, optimizer_state, params=online_params
+  )
   online_params = optax.apply_updates(online_params, updates)
   return optimizer_state, online_params, loss, mean_loss, rng2
 
 
 @functools.partial(
-    jax.vmap, in_axes=(None, None, 0, 0, 0, None, None, None, None, None))
-def target_output(model, target_network, next_states, rewards, terminals,
-                  support, cumulative_gamma, double_dqn, distributional, rng):
+    jax.vmap, in_axes=(None, None, 0, 0, 0, None, None, None, None, None)
+)
+def target_output(
+    model,
+    target_network,
+    next_states,
+    rewards,
+    terminals,
+    support,
+    cumulative_gamma,
+    double_dqn,
+    distributional,
+    rng,
+):
   """Builds the C51 target distribution or DQN target Q-values."""
 
-  is_terminal_multiplier = 1. - terminals.astype(jnp.float32)
+  is_terminal_multiplier = 1.0 - terminals.astype(jnp.float32)
   # Incorporate terminal state to discount factor.
   gamma_with_terminal = cumulative_gamma * is_terminal_multiplier
 
   target_network_dist = target_network(next_states, key=rng)
   if double_dqn:
     # Use the current network for the action selection
     next_state_target_outputs = model(next_states, key=rng)
@@ -147,52 +225,57 @@
 
   if distributional:
     # Compute the target Q-value distribution
     probabilities = jnp.squeeze(target_network_dist.probabilities)
     next_probabilities = probabilities[next_qt_argmax]
     target_support = rewards + gamma_with_terminal * support
     target = rainbow_agent.project_distribution(
-        target_support, next_probabilities, support)
+        target_support, next_probabilities, support
+    )
   else:
     # Compute the target Q-value
     next_q_values = jnp.squeeze(target_network_dist.q_values)
     replay_next_qt_max = next_q_values[next_qt_argmax]
     target = rewards + gamma_with_terminal * replay_next_qt_max
 
   return jax.lax.stop_gradient(target)
 
 
 @gin.configurable
 class JaxFullRainbowAgent(dqn_agent.JaxDQNAgent):
   """A compact implementation of the full Rainbow agent."""
 
-  def __init__(self,
-               num_actions,
-               noisy=True,
-               dueling=True,
-               double_dqn=True,
-               distributional=True,
-               num_updates_per_train_step=1,
-               network=networks.FullRainbowNetwork,
-               num_atoms=51,
-               vmax=10.,
-               vmin=None,
-               epsilon_fn=dqn_agent.linearly_decaying_epsilon,
-               replay_scheme='prioritized',
-               summary_writer=None,
-               seed=None,
-               preprocess_fn=None):
+  def __init__(
+      self,
+      num_actions,
+      noisy=True,
+      dueling=True,
+      double_dqn=True,
+      distributional=True,
+      mse_loss=False,
+      num_updates_per_train_step=1,
+      network=networks.FullRainbowNetwork,
+      num_atoms=51,
+      vmax=10.0,
+      vmin=None,
+      epsilon_fn=dqn_agent.linearly_decaying_epsilon,
+      replay_scheme='prioritized',
+      summary_writer=None,
+      seed=None,
+      preprocess_fn=None,
+  ):
     """Initializes the agent and constructs the necessary components.
 
     Args:
       num_actions: int, number of actions the agent can take at any state.
       noisy: bool, Whether to use noisy networks or not.
       dueling: bool, Whether to use dueling network architecture or not.
       double_dqn: bool, Whether to use Double DQN or not.
       distributional: bool, whether to use distributional RL or not.
+      mse_loss: bool, mse loss function.
       num_updates_per_train_step: int, Number of gradient updates every training
         step. Defaults to 1.
       network: flax.linen Module, neural network used by the agent initialized
         by shape in _create_network below. See
         dopamine.jax.networks.RainbowNetwork as an example.
       num_atoms: int, the number of buckets of the value function distribution.
       vmax: float, the value distribution support is [vmin, vmax].
@@ -201,70 +284,81 @@
       epsilon_fn: function expecting 4 parameters: (decay_period, step,
         warmup_steps, epsilon). This function should return the epsilon value
         used for exploration during training.
       replay_scheme: str, 'prioritized' or 'uniform', the sampling scheme of the
         replay memory.
       summary_writer: SummaryWriter object, for outputting training statistics.
       seed: int, a seed for Jax RNG and initialization.
-      preprocess_fn: function expecting the input state as parameter which
-        it preprocesses (such as normalizing the pixel values between 0 and 1)
+      preprocess_fn: function expecting the input state as parameter which it
+        preprocesses (such as normalizing the pixel values between 0 and 1)
         before passing it to the Q-network. Defaults to None.
     """
-    logging.info('Creating %s agent with the following parameters:',
-                 self.__class__.__name__)
+    logging.info(
+        'Creating %s agent with the following parameters:',
+        self.__class__.__name__,
+    )
     logging.info('\t double_dqn: %s', double_dqn)
     logging.info('\t noisy_networks: %s', noisy)
     logging.info('\t dueling_dqn: %s', dueling)
     logging.info('\t distributional: %s', distributional)
+    logging.info('\t mse_loss: %d', mse_loss)
     logging.info('\t num_atoms: %d', num_atoms)
     logging.info('\t replay_scheme: %s', replay_scheme)
-    logging.info('\t num_updates_per_train_step: %d',
-                 num_updates_per_train_step)
+    logging.info(
+        '\t num_updates_per_train_step: %d', num_updates_per_train_step
+    )
     # We need this because some tools convert round floats into ints.
     vmax = float(vmax)
     self._num_atoms = num_atoms
     vmin = vmin if vmin else -vmax
     self._support = jnp.linspace(vmin, vmax, num_atoms)
     self._replay_scheme = replay_scheme
     self._double_dqn = double_dqn
     self._noisy = noisy
     self._dueling = dueling
     self._distributional = distributional
+    self._mse_loss = mse_loss
     self._num_updates_per_train_step = num_updates_per_train_step
 
     super().__init__(
         num_actions=num_actions,
         network=functools.partial(
-            network, num_atoms=num_atoms,
+            network,
+            num_atoms=num_atoms,
             noisy=self._noisy,
             dueling=self._dueling,
-            distributional=self._distributional),
-        epsilon_fn=dqn_agent.identity_epsilon if self._noisy else epsilon_fn,
+            distributional=self._distributional,
+        ),
+        epsilon_fn=zero_epsilon if self._noisy else epsilon_fn,
         summary_writer=summary_writer,
         seed=seed,
-        preprocess_fn=preprocess_fn)
+        preprocess_fn=preprocess_fn,
+    )
 
   def _build_networks_and_optimizer(self):
     self._rng, rng = jax.random.split(self._rng)
-    self.online_params = self.network_def.init(rng, x=self.state,
-                                               support=self._support)
+    state = self.preprocess_fn(self.state)
+    self.online_params = self.network_def.init(
+        rng, x=state, support=self._support
+    )
     self.optimizer = dqn_agent.create_optimizer(self._optimizer_name)
     self.optimizer_state = self.optimizer.init(self.online_params)
     self.target_network_params = self.online_params
 
   def _build_replay_buffer(self):
     """Creates the replay buffer used by the agent."""
     if self._replay_scheme not in ['uniform', 'prioritized']:
       raise ValueError('Invalid replay scheme: {}'.format(self._replay_scheme))
     return prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
-        observation_dtype=self.observation_dtype)
+        observation_dtype=self.observation_dtype,
+    )
 
   def _training_step_update(self):
     """Gradient update during every training step."""
 
     self._sample_from_replay_buffer()
     states = self.preprocess_fn(self.replay_elements['state'])
     next_states = self.preprocess_fn(self.replay_elements['next_state'])
@@ -278,73 +372,99 @@
       # Weight the loss by the inverse priorities.
       loss_weights = 1.0 / jnp.sqrt(probs + 1e-10)
       loss_weights /= jnp.max(loss_weights)
     else:
       # Uniform weights if not using prioritized replay.
       loss_weights = jnp.ones(states.shape[0])
 
-    (self.optimizer_state, self.online_params,
-     loss, mean_loss, self._rng) = train(
-         self.network_def, self.online_params, self.target_network_params,
-         self.optimizer, self.optimizer_state, states,
-         self.replay_elements['action'], next_states,
-         self.replay_elements['reward'], self.replay_elements['terminal'],
-         loss_weights, self._support, self.cumulative_gamma, self._double_dqn,
-         self._distributional, self._rng)
+    (self.optimizer_state, self.online_params, loss, mean_loss, self._rng) = (
+        train(
+            self.network_def,
+            self.online_params,
+            self.target_network_params,
+            self.optimizer,
+            self.optimizer_state,
+            states,
+            self.replay_elements['action'],
+            next_states,
+            self.replay_elements['reward'],
+            self.replay_elements['terminal'],
+            loss_weights,
+            self._support,
+            self.cumulative_gamma,
+            self._double_dqn,
+            self._distributional,
+            self._mse_loss,
+            self._rng,
+        )
+    )
 
     if self._replay_scheme == 'prioritized':
       # Rainbow and prioritized replay are parametrized by an exponent
       # alpha, but in both cases it is set to 0.5 - for simplicity's sake we
       # leave it as is here, using the more direct sqrt(). Taking the square
       # root "makes sense", as we are dealing with a squared loss.  Add a
       # small nonzero value to the loss to avoid 0 priority items. While
       # technically this may be okay, setting all items to 0 priority will
       # cause troubles, and also result in 1.0 / 0.0 = NaN correction terms.
-      self._replay.set_priority(self.replay_elements['indices'],
-                                jnp.sqrt(loss + 1e-10))
-
-    if self.summary_writer is not None:
+      self._replay.set_priority(
+          self.replay_elements['indices'], jnp.sqrt(loss + 1e-10)
+      )
+
+    if (
+        self.summary_writer is not None
+        and self.training_steps > 0
+        and self.training_steps % self.summary_writing_frequency == 0
+    ):
       with self.summary_writer.as_default():
-        tf.summary.scalar('CrossEntropyLoss', mean_loss,
-                          step=self.training_steps)
+        tf.summary.scalar(
+            'CrossEntropyLoss', mean_loss, step=self.training_steps
+        )
       self.summary_writer.flush()
       if hasattr(self, 'collector_dispatcher'):
         self.collector_dispatcher.write(
-            [statistics_instance.StatisticsInstance(
-                'Loss', onp.asarray(mean_loss), step=self.training_steps),
-             ],
-            collector_allowlist=self._collector_allowlist)
-
-  def _store_transition(self,
-                        last_observation,
-                        action,
-                        reward,
-                        is_terminal,
-                        *args,
-                        priority=None,
-                        episode_end=False):
+            [
+                statistics_instance.StatisticsInstance(
+                    'Loss', onp.asarray(mean_loss), step=self.training_steps
+                ),
+            ],
+            collector_allowlist=self._collector_allowlist,
+        )
+
+  def _store_transition(
+      self,
+      last_observation,
+      action,
+      reward,
+      is_terminal,
+      *args,
+      priority=None,
+      episode_end=False
+  ):
     """Stores a transition when in training mode."""
     is_prioritized = isinstance(
         self._replay,
-        prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer)
+        prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer,
+    )
     if is_prioritized and priority is None:
       if self._replay_scheme == 'uniform':
-        priority = 1.
+        priority = 1.0
       else:
         priority = self._replay.sum_tree.max_recorded_priority
 
     if not self.eval_mode:
       self._replay.add(
           last_observation,
           action,
           reward,
           is_terminal,
           *args,
           priority=priority,
-          episode_end=episode_end)
+          episode_end=episode_end
+      )
 
   def _train_step(self):
     """Runs a single training step.
 
     Runs training if both:
       (1) A minimum number of frames have been added to the replay buffer.
       (2) `training_steps` is a multiple of `update_period`.
@@ -368,31 +488,51 @@
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._train_step()
 
     state = self.preprocess_fn(self.state)
     self._rng, self.action = select_action(
-        self.network_def, self.online_params, state, self._rng,
-        self.num_actions, self.eval_mode, self.epsilon_eval, self.epsilon_train,
-        self.epsilon_decay_period, self.training_steps, self.min_replay_history,
-        self.epsilon_fn, self._support)
+        self.network_def,
+        self.online_params,
+        state,
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+        self._support,
+    )
     self.action = onp.asarray(self.action)
     return self.action
 
   def step(self, reward, observation):
     """Records the most recent transition and returns the agent's next action."""
     self._last_observation = self._observation
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._store_transition(self._last_observation, self.action, reward, False)
       self._train_step()
 
     state = self.preprocess_fn(self.state)
     self._rng, self.action = select_action(
-        self.network_def, self.online_params, state, self._rng,
-        self.num_actions, self.eval_mode, self.epsilon_eval, self.epsilon_train,
-        self.epsilon_decay_period, self.training_steps, self.min_replay_history,
-        self.epsilon_fn, self._support)
+        self.network_def,
+        self.online_params,
+        state,
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+        self._support,
+    )
     self.action = onp.asarray(self.action)
     return self.action
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/implicit_quantile/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,19 +34,29 @@
 import optax
 import tensorflow as tf
 
 
 @functools.partial(
     jax.vmap,
     in_axes=(None, None, None, 0, 0, 0, None, None, None, None, 0),
-    out_axes=(0, 0))
-def target_quantile_values(network_def, online_params, target_params,
-                           next_states, rewards, terminals,
-                           num_tau_prime_samples, num_quantile_samples,
-                           cumulative_gamma, double_dqn, rng):
+    out_axes=(0, 0),
+)
+def target_quantile_values(
+    network_def,
+    online_params,
+    target_params,
+    next_states,
+    rewards,
+    terminals,
+    num_tau_prime_samples,
+    num_quantile_samples,
+    cumulative_gamma,
+    double_dqn,
+    rng,
+):
   """Build the target for return values at given quantiles.
 
   Args:
     network_def: Linen Module used for inference.
     online_params: Parameters used for the online network.
     target_params: Parameters used for the target network.
     next_states: numpy array of batched next states.
@@ -59,93 +69,118 @@
     rng: Jax random number generator.
 
   Returns:
     Jax random number generator.
     The target quantile values.
   """
   rewards = jnp.tile(rewards, [num_tau_prime_samples])
-  is_terminal_multiplier = 1. - terminals.astype(jnp.float32)
+  is_terminal_multiplier = 1.0 - terminals.astype(jnp.float32)
   # Incorporate terminal state to discount factor.
   gamma_with_terminal = cumulative_gamma * is_terminal_multiplier
   gamma_with_terminal = jnp.tile(gamma_with_terminal, [num_tau_prime_samples])
   rng, rng1, rng2 = jax.random.split(rng, num=3)
   # Compute Q-values which are used for action selection for the next states
   # in the replay buffer. Compute the argmax over the Q-values.
   if double_dqn:
-    outputs_action = network_def.apply(online_params,
-                                       next_states,
-                                       num_quantiles=num_quantile_samples,
-                                       rng=rng1)
+    outputs_action = network_def.apply(
+        online_params, next_states, num_quantiles=num_quantile_samples, rng=rng1
+    )
   else:
-    outputs_action = network_def.apply(target_params,
-                                       next_states,
-                                       num_quantiles=num_quantile_samples,
-                                       rng=rng1)
+    outputs_action = network_def.apply(
+        target_params, next_states, num_quantiles=num_quantile_samples, rng=rng1
+    )
   target_quantile_values_action = outputs_action.quantile_values
-  target_q_values = jnp.squeeze(
-      jnp.mean(target_quantile_values_action, axis=0))
+  target_q_values = jnp.squeeze(jnp.mean(target_quantile_values_action, axis=0))
   # Shape: batch_size.
   next_qt_argmax = jnp.argmax(target_q_values)
   # Get the indices of the maximium Q-value across the action dimension.
   # Shape of next_qt_argmax: (num_tau_prime_samples x batch_size).
   next_state_target_outputs = network_def.apply(
-      target_params,
-      next_states,
-      num_quantiles=num_tau_prime_samples,
-      rng=rng2)
+      target_params, next_states, num_quantiles=num_tau_prime_samples, rng=rng2
+  )
   next_qt_argmax = jnp.tile(next_qt_argmax, [num_tau_prime_samples])
-  target_quantile_vals = (
-      jax.vmap(lambda x, y: x[y])(next_state_target_outputs.quantile_values,
-                                  next_qt_argmax))
+  target_quantile_vals = jax.vmap(lambda x, y: x[y])(
+      next_state_target_outputs.quantile_values, next_qt_argmax
+  )
   target_quantile_vals = rewards + gamma_with_terminal * target_quantile_vals
   # We return with an extra dimension, which is expected by train.
   return rng, jax.lax.stop_gradient(target_quantile_vals[:, None])
 
 
 @functools.partial(jax.jit, static_argnums=(0, 3, 10, 11, 12, 13, 14, 15))
-def train(network_def, online_params, target_params, optimizer, optimizer_state,
-          states, actions, next_states, rewards, terminals, num_tau_samples,
-          num_tau_prime_samples, num_quantile_samples, cumulative_gamma,
-          double_dqn, kappa, rng):
+def train(
+    network_def,
+    online_params,
+    target_params,
+    optimizer,
+    optimizer_state,
+    states,
+    actions,
+    next_states,
+    rewards,
+    terminals,
+    num_tau_samples,
+    num_tau_prime_samples,
+    num_quantile_samples,
+    cumulative_gamma,
+    double_dqn,
+    kappa,
+    rng,
+):
   """Run a training step."""
   batch_size = states.shape[0]
+
   def loss_fn(params, rng_input, target_quantile_vals):
     def online(state, key):
-      return network_def.apply(params, state, num_quantiles=num_tau_samples,
-                               rng=key)
+      return network_def.apply(
+          params, state, num_quantiles=num_tau_samples, rng=key
+      )
 
     batched_rng = jnp.stack(jax.random.split(rng_input, num=batch_size))
     model_output = jax.vmap(online)(states, batched_rng)
     quantile_values = model_output.quantile_values
     quantiles = model_output.quantiles
     chosen_action_quantile_values = jax.vmap(lambda x, y: x[:, y][:, None])(
-        quantile_values, actions)
+        quantile_values, actions
+    )
     # Shape of bellman_erors and huber_loss:
     # batch_size x num_tau_prime_samples x num_tau_samples x 1.
-    bellman_errors = (target_quantile_vals[:, :, None, :] -
-                      chosen_action_quantile_values[:, None, :, :])
+    bellman_errors = (
+        target_quantile_vals[:, :, None, :]
+        - chosen_action_quantile_values[:, None, :, :]
+    )
     # The huber loss (see Section 2.3 of the paper) is defined via two cases:
     # case_one: |bellman_errors| <= kappa
     # case_two: |bellman_errors| > kappa
     huber_loss_case_one = (
-        (jnp.abs(bellman_errors) <= kappa).astype(jnp.float32) *
-        0.5 * bellman_errors ** 2)
+        (jnp.abs(bellman_errors) <= kappa).astype(jnp.float32)
+        * 0.5
+        * bellman_errors**2
+    )
     huber_loss_case_two = (
-        (jnp.abs(bellman_errors) > kappa).astype(jnp.float32) *
-        kappa * (jnp.abs(bellman_errors) - 0.5 * kappa))
+        (jnp.abs(bellman_errors) > kappa).astype(jnp.float32)
+        * kappa
+        * (jnp.abs(bellman_errors) - 0.5 * kappa)
+    )
     huber_loss = huber_loss_case_one + huber_loss_case_two
     # Tile by num_tau_prime_samples along a new dimension. Shape is now
     # batch_size x num_tau_prime_samples x num_tau_samples x 1.
     # These quantiles will be used for computation of the quantile huber loss
     # below (see section 2.3 of the paper).
-    quantiles = jnp.tile(quantiles[:, None, :, :],
-                         [1, num_tau_prime_samples, 1, 1]).astype(jnp.float32)
+    quantiles = jnp.tile(
+        quantiles[:, None, :, :], [1, num_tau_prime_samples, 1, 1]
+    ).astype(jnp.float32)
     # Shape: batch_size x num_tau_prime_samples x num_tau_samples x 1.
-    quantile_huber_loss = (jnp.abs(quantiles - jax.lax.stop_gradient(
-        (bellman_errors < 0).astype(jnp.float32))) * huber_loss) / kappa
+    quantile_huber_loss = (
+        jnp.abs(
+            quantiles
+            - jax.lax.stop_gradient((bellman_errors < 0).astype(jnp.float32))
+        )
+        * huber_loss
+    ) / kappa
     # Sum over current quantile value (num_tau_samples) dimension,
     # average over target quantile value (num_tau_prime_samples) dimension.
     # Shape: batch_size x num_tau_prime_samples x 1.
     loss = jnp.sum(quantile_huber_loss, axis=2)
     loss = jnp.mean(loss, axis=1)
     return jnp.mean(loss)
 
@@ -158,29 +193,42 @@
       next_states,
       rewards,
       terminals,
       num_tau_prime_samples,
       num_quantile_samples,
       cumulative_gamma,
       double_dqn,
-      batched_target_rng)
+      batched_target_rng,
+  )
   grad_fn = jax.value_and_grad(loss_fn)
   rng, rng_input = jax.random.split(rng)
   loss, grad = grad_fn(online_params, rng_input, target_quantile_vals)
-  updates, optimizer_state = optimizer.update(grad, optimizer_state,
-                                              params=online_params)
+  updates, optimizer_state = optimizer.update(
+      grad, optimizer_state, params=online_params
+  )
   online_params = optax.apply_updates(online_params, updates)
   return rng, optimizer_state, online_params, loss
 
 
 @functools.partial(jax.jit, static_argnums=(0, 4, 5, 6, 7, 8, 9, 11, 12))
-def select_action(network_def, params, state, rng, num_quantile_samples,
-                  num_actions, eval_mode, epsilon_eval, epsilon_train,
-                  epsilon_decay_period, training_steps, min_replay_history,
-                  epsilon_fn):
+def select_action(
+    network_def,
+    params,
+    state,
+    rng,
+    num_quantile_samples,
+    num_actions,
+    eval_mode,
+    epsilon_eval,
+    epsilon_train,
+    epsilon_decay_period,
+    training_steps,
+    min_replay_history,
+    epsilon_fn,
+):
   """Select an action from the set of available actions.
 
   Chooses an action randomly with probability self._calculate_epsilon(), and
   otherwise acts greedily according to the current Q-value estimates.
 
   Args:
     network_def: Linen Module to use for inference.
@@ -199,62 +247,74 @@
       (static_argnum).
     epsilon_fn: function used to calculate epsilon value (static_argnum).
 
   Returns:
     Jax random number generator.
     int, the selected action.
   """
-  epsilon = jnp.where(eval_mode,
-                      epsilon_eval,
-                      epsilon_fn(epsilon_decay_period,
-                                 training_steps,
-                                 min_replay_history,
-                                 epsilon_train))
+  epsilon = jnp.where(
+      eval_mode,
+      epsilon_eval,
+      epsilon_fn(
+          epsilon_decay_period,
+          training_steps,
+          min_replay_history,
+          epsilon_train,
+      ),
+  )
 
   rng, rng1, rng2 = jax.random.split(rng, num=3)
   p = jax.random.uniform(rng1)
-  return rng, jnp.where(p <= epsilon,
-                        jax.random.randint(rng2, (), 0, num_actions),
-                        jnp.argmax(jnp.mean(
-                            network_def.apply(
-                                params, state,
-                                num_quantiles=num_quantile_samples,
-                                rng=rng2).quantile_values, axis=0), axis=0))
+  return rng, jnp.where(
+      p <= epsilon,
+      jax.random.randint(rng2, (), 0, num_actions),
+      jnp.argmax(
+          jnp.mean(
+              network_def.apply(
+                  params, state, num_quantiles=num_quantile_samples, rng=rng2
+              ).quantile_values,
+              axis=0,
+          ),
+          axis=0,
+      ),
+  )
 
 
 @gin.configurable
 class JaxImplicitQuantileAgent(dqn_agent.JaxDQNAgent):
   """An extension of Rainbow to perform implicit quantile regression."""
 
-  def __init__(self,
-               num_actions,
-               observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
-               observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
-               stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
-               network=networks.ImplicitQuantileNetwork,
-               kappa=1.0,
-               num_tau_samples=32,
-               num_tau_prime_samples=32,
-               num_quantile_samples=32,
-               quantile_embedding_dim=64,
-               double_dqn=False,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=20000,
-               update_period=4,
-               target_update_period=8000,
-               epsilon_fn=dqn_agent.linearly_decaying_epsilon,
-               epsilon_train=0.01,
-               epsilon_eval=0.001,
-               epsilon_decay_period=250000,
-               replay_scheme='prioritized',
-               optimizer='adam',
-               summary_writer=None,
-               summary_writing_frequency=500,
-               seed=None):
+  def __init__(
+      self,
+      num_actions,
+      observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
+      observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
+      stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
+      network=networks.ImplicitQuantileNetwork,
+      kappa=1.0,
+      num_tau_samples=32,
+      num_tau_prime_samples=32,
+      num_quantile_samples=32,
+      quantile_embedding_dim=64,
+      double_dqn=False,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=20000,
+      update_period=4,
+      target_update_period=8000,
+      epsilon_fn=dqn_agent.linearly_decaying_epsilon,
+      epsilon_train=0.01,
+      epsilon_eval=0.001,
+      epsilon_decay_period=250000,
+      replay_scheme='prioritized',
+      optimizer='adam',
+      summary_writer=None,
+      summary_writing_frequency=500,
+      seed=None,
+  ):
     """Initializes the agent and constructs the necessary components.
 
     Most of this constructor's parameters are IQN-specific hyperparameters whose
     values are taken from Dabney et al. (2018).
 
     Args:
       num_actions: int, number of actions the agent can take at any state.
@@ -270,39 +330,39 @@
       num_tau_samples: int, number of online quantile samples for loss
         estimation.
       num_tau_prime_samples: int, number of target quantile samples for loss
         estimation.
       num_quantile_samples: int, number of quantile samples for computing
         Q-values.
       quantile_embedding_dim: int, embedding dimension for the quantile input.
-      double_dqn: boolean, whether to perform double DQN style learning
-        as described in Van Hasselt et al.: https://arxiv.org/abs/1509.06461.
+      double_dqn: boolean, whether to perform double DQN style learning as
+        described in Van Hasselt et al.: https://arxiv.org/abs/1509.06461.
       gamma: float, discount factor with the usual RL meaning.
       update_horizon: int, horizon at which updates are performed, the 'n' in
         n-step update.
       min_replay_history: int, number of transitions that should be experienced
         before the agent begins training its value function.
       update_period: int, period between DQN updates.
       target_update_period: int, update period for the target network.
-      epsilon_fn: function expecting 4 parameters:
-        (decay_period, step, warmup_steps, epsilon). This function should return
-        the epsilon value used for exploration during training.
+      epsilon_fn: function expecting 4 parameters: (decay_period, step,
+        warmup_steps, epsilon). This function should return the epsilon value
+        used for exploration during training.
       epsilon_train: float, the value to which the agent's epsilon is eventually
         decayed during training.
       epsilon_eval: float, epsilon used when evaluating the agent.
       epsilon_decay_period: int, length of the epsilon decay schedule.
       replay_scheme: str, 'prioritized' or 'uniform', the sampling scheme of the
         replay memory.
       optimizer: str, name of optimizer to use.
       summary_writer: SummaryWriter object for outputting training statistics.
         Summary writing disabled if set to None.
       summary_writing_frequency: int, frequency with which summaries will be
         written. Lower values will result in slower training.
-      seed: int, a seed for internal RNG, used for initialization and
-        sampling actions. If None, will use the current time in nanoseconds.
+      seed: int, a seed for internal RNG, used for initialization and sampling
+        actions. If None, will use the current time in nanoseconds.
     """
     self.kappa = kappa
     # num_tau_samples = N below equation (3) in the paper.
     self.num_tau_samples = num_tau_samples
     # num_tau_prime_samples = N' below equation (3) in the paper.
     self.num_tau_prime_samples = num_tau_prime_samples
     # num_quantile_samples = k below equation (3) in the paper.
@@ -314,34 +374,36 @@
 
     super(JaxImplicitQuantileAgent, self).__init__(
         num_actions=num_actions,
         observation_shape=observation_shape,
         observation_dtype=observation_dtype,
         stack_size=stack_size,
         network=functools.partial(
-            network, quantile_embedding_dim=quantile_embedding_dim),
+            network, quantile_embedding_dim=quantile_embedding_dim
+        ),
         gamma=gamma,
         update_horizon=update_horizon,
         min_replay_history=min_replay_history,
         update_period=update_period,
         target_update_period=target_update_period,
         epsilon_fn=epsilon_fn,
         epsilon_train=epsilon_train,
         epsilon_eval=epsilon_eval,
         epsilon_decay_period=epsilon_decay_period,
         optimizer=optimizer,
         summary_writer=summary_writer,
         summary_writing_frequency=summary_writing_frequency,
-        seed=seed)
+        seed=seed,
+    )
 
   def _build_networks_and_optimizer(self):
     self._rng, rng = jax.random.split(self._rng)
     self.online_params = self.network_def.init(
-        rng, x=self.state, num_quantiles=self.num_tau_samples,
-        rng=self._rng)
+        rng, x=self.state, num_quantiles=self.num_tau_samples, rng=self._rng
+    )
     self.optimizer = dqn_agent.create_optimizer(self._optimizer_name)
     self.optimizer_state = self.optimizer.init(self.online_params)
     self.target_network_params = self.online_params
 
   def begin_episode(self, observation):
     """Returns the agent's first action for this episode.
 
@@ -353,27 +415,29 @@
     """
     self._reset_state()
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._train_step()
 
-    self._rng, self.action = select_action(self.network_def,
-                                           self.online_params,
-                                           self.state,
-                                           self._rng,
-                                           self.num_quantile_samples,
-                                           self.num_actions,
-                                           self.eval_mode,
-                                           self.epsilon_eval,
-                                           self.epsilon_train,
-                                           self.epsilon_decay_period,
-                                           self.training_steps,
-                                           self.min_replay_history,
-                                           self.epsilon_fn)
+    self._rng, self.action = select_action(
+        self.network_def,
+        self.online_params,
+        self.state,
+        self._rng,
+        self.num_quantile_samples,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+    )
     self.action = onp.asarray(self.action)
     return self.action
 
   def step(self, reward, observation):
     """Records the most recent transition and returns the agent's next action.
 
     We store the observation of the last time step since we want to store it
@@ -389,27 +453,29 @@
     self._last_observation = self._observation
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._store_transition(self._last_observation, self.action, reward, False)
       self._train_step()
 
-    self._rng, self.action = select_action(self.network_def,
-                                           self.online_params,
-                                           self.preprocess_fn(self.state),
-                                           self._rng,
-                                           self.num_quantile_samples,
-                                           self.num_actions,
-                                           self.eval_mode,
-                                           self.epsilon_eval,
-                                           self.epsilon_train,
-                                           self.epsilon_decay_period,
-                                           self.training_steps,
-                                           self.min_replay_history,
-                                           self.epsilon_fn)
+    self._rng, self.action = select_action(
+        self.network_def,
+        self.online_params,
+        self.preprocess_fn(self.state),
+        self._rng,
+        self.num_quantile_samples,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+    )
     self.action = onp.asarray(self.action)
     return self.action
 
   def _train_step(self):
     """Runs a single training step.
 
     Runs training if both:
@@ -435,24 +501,30 @@
             self.replay_elements['terminal'],
             self.num_tau_samples,
             self.num_tau_prime_samples,
             self.num_quantile_samples,
             self.cumulative_gamma,
             self.double_dqn,
             self.kappa,
-            self._rng)
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+            self._rng,
+        )
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
           with self.summary_writer.as_default():
             tf.summary.scalar('QuantileLoss', loss, step=self.training_steps)
           self.summary_writer.flush()
           if hasattr(self, 'collector_dispatcher'):
             self.collector_dispatcher.write(
-                [statistics_instance.StatisticsInstance(
-                    'Loss', onp.asarray(loss), step=self.training_steps),
-                 ],
-                collector_allowlist=self._collector_allowlist)
+                [
+                    statistics_instance.StatisticsInstance(
+                        'Loss', onp.asarray(loss), step=self.training_steps
+                    ),
+                ],
+                collector_allowlist=self._collector_allowlist,
+            )
       if self.training_steps % self.target_update_period == 0:
         self._sync_weights()
 
     self.training_steps += 1
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/quantile/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/quantile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/quantile/quantile_agent.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/quantile/quantile_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,115 +33,135 @@
 import jax.numpy as jnp
 import numpy as np
 import optax
 import tensorflow as tf
 
 
 @functools.partial(jax.vmap, in_axes=(None, 0, 0, 0, None))
-def target_distribution(target_network, next_states, rewards, terminals,
-                        cumulative_gamma):
+def target_distribution(
+    target_network, next_states, rewards, terminals, cumulative_gamma
+):
   """Builds the Quantile target distribution as per Dabney et al. (2017).
 
   Args:
     target_network: Jax Module used for the target network.
     next_states: numpy array of batched next states.
     rewards: numpy array of batched rewards.
     terminals: numpy array of batched terminals.
     cumulative_gamma: float, cumulative gamma to use.
 
   Returns:
     The target distribution from the replay.
   """
-  is_terminal_multiplier = 1. - terminals.astype(jnp.float32)
+  is_terminal_multiplier = 1.0 - terminals.astype(jnp.float32)
   # Incorporate terminal state to discount factor.
   gamma_with_terminal = cumulative_gamma * is_terminal_multiplier
   next_state_target_outputs = target_network(next_states)
   q_values = jnp.squeeze(next_state_target_outputs.q_values)
   next_qt_argmax = jnp.argmax(q_values)
   logits = jnp.squeeze(next_state_target_outputs.logits)
   next_logits = logits[next_qt_argmax]
   return jax.lax.stop_gradient(rewards + gamma_with_terminal * next_logits)
 
 
 @functools.partial(jax.jit, static_argnums=(0, 3, 10, 11, 12))
-def train(network_def, online_params, target_params, optimizer, optimizer_state,
-          states, actions, next_states, rewards, terminals, kappa, num_atoms,
-          cumulative_gamma):
+def train(
+    network_def,
+    online_params,
+    target_params,
+    optimizer,
+    optimizer_state,
+    states,
+    actions,
+    next_states,
+    rewards,
+    terminals,
+    kappa,
+    num_atoms,
+    cumulative_gamma,
+):
   """Run a training step."""
+
   def loss_fn(params, target):
     def q_online(state):
       return network_def.apply(params, state)
 
     logits = jax.vmap(q_online)(states).logits
     logits = jnp.squeeze(logits)
     # Fetch the logits for its selected action. We use vmap to perform this
     # indexing across the batch.
     chosen_action_logits = jax.vmap(lambda x, y: x[y])(logits, actions)
-    bellman_errors = (target[:, None, :] -
-                      chosen_action_logits[:, :, None])  # Input `u' of Eq. 9.
+    bellman_errors = (
+        target[:, None, :] - chosen_action_logits[:, :, None]
+    )  # Input `u' of Eq. 9.
     # Eq. 9 of paper.
-    huber_loss = (
-        (jnp.abs(bellman_errors) <= kappa).astype(jnp.float32) *
-        0.5 * bellman_errors ** 2 +
-        (jnp.abs(bellman_errors) > kappa).astype(jnp.float32) *
-        kappa * (jnp.abs(bellman_errors) - 0.5 * kappa))
-
-    tau_hat = ((jnp.arange(num_atoms, dtype=jnp.float32) + 0.5) /
-               num_atoms)  # Quantile midpoints.  See Lemma 2 of paper.
+    huber_loss = (jnp.abs(bellman_errors) <= kappa).astype(
+        jnp.float32
+    ) * 0.5 * bellman_errors**2 + (jnp.abs(bellman_errors) > kappa).astype(
+        jnp.float32
+    ) * kappa * (
+        jnp.abs(bellman_errors) - 0.5 * kappa
+    )
+
+    tau_hat = (
+        jnp.arange(num_atoms, dtype=jnp.float32) + 0.5
+    ) / num_atoms  # Quantile midpoints.  See Lemma 2 of paper.
     # Eq. 10 of paper.
     tau_bellman_diff = jnp.abs(
-        tau_hat[None, :, None] - (bellman_errors < 0).astype(jnp.float32))
+        tau_hat[None, :, None] - (bellman_errors < 0).astype(jnp.float32)
+    )
     quantile_huber_loss = tau_bellman_diff * huber_loss
     # Sum over tau dimension, average over target value dimension.
     loss = jnp.sum(jnp.mean(quantile_huber_loss, 2), 1)
     return jnp.mean(loss), loss
 
   def q_target(state):
     return network_def.apply(target_params, state)
 
   grad_fn = jax.value_and_grad(loss_fn, has_aux=True)
-  target = target_distribution(q_target,
-                               next_states,
-                               rewards,
-                               terminals,
-                               cumulative_gamma)
+  target = target_distribution(
+      q_target, next_states, rewards, terminals, cumulative_gamma
+  )
   (mean_loss, loss), grad = grad_fn(online_params, target)
-  updates, optimizer_state = optimizer.update(grad, optimizer_state,
-                                              params=online_params)
+  updates, optimizer_state = optimizer.update(
+      grad, optimizer_state, params=online_params
+  )
   online_params = optax.apply_updates(online_params, updates)
   return optimizer_state, online_params, loss, mean_loss
 
 
 @gin.configurable
 class JaxQuantileAgent(dqn_agent.JaxDQNAgent):
   """An implementation of Quantile regression DQN agent."""
 
-  def __init__(self,
-               num_actions,
-               observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
-               observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
-               stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
-               network=networks.QuantileNetwork,
-               kappa=1.0,
-               num_atoms=200,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=50000,
-               update_period=4,
-               target_update_period=10000,
-               epsilon_fn=dqn_agent.linearly_decaying_epsilon,
-               epsilon_train=0.1,
-               epsilon_eval=0.05,
-               epsilon_decay_period=1000000,
-               replay_scheme='prioritized',
-               optimizer='adam',
-               summary_writer=None,
-               summary_writing_frequency=500,
-               seed=None,
-               allow_partial_reload=False):
+  def __init__(
+      self,
+      num_actions,
+      observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
+      observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
+      stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
+      network=networks.QuantileNetwork,
+      kappa=1.0,
+      num_atoms=200,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=50000,
+      update_period=4,
+      target_update_period=10000,
+      epsilon_fn=dqn_agent.linearly_decaying_epsilon,
+      epsilon_train=0.1,
+      epsilon_eval=0.05,
+      epsilon_decay_period=1000000,
+      replay_scheme='prioritized',
+      optimizer='adam',
+      summary_writer=None,
+      summary_writing_frequency=500,
+      seed=None,
+      allow_partial_reload=False,
+  ):
     """Initializes the agent and constructs the Graph.
 
     Args:
       num_actions: Int, number of actions the agent can take at any state.
       observation_shape: tuple of ints or an int. If single int, the observation
         is assumed to be a 2D square.
       observation_dtype: DType, specifies the type of the observations. Note
@@ -162,16 +182,16 @@
       epsilon_fn: Function expecting 4 parameters: (decay_period, step,
         warmup_steps, epsilon), and which returns the epsilon value used for
         exploration during training.
       epsilon_train: Float, final epsilon for training.
       epsilon_eval: Float, epsilon during evaluation.
       epsilon_decay_period: Int, number of steps for epsilon to decay.
       replay_scheme: String, replay memory scheme to be used. Choices are:
-        uniform - Standard (DQN) replay buffer (Mnih et al., 2015)
-        prioritized - Prioritized replay buffer (Schaul et al., 2015)
+        uniform - Standard (DQN) replay buffer (Mnih et al., 2015) prioritized -
+        Prioritized replay buffer (Schaul et al., 2015)
       optimizer: str, name of optimizer to use.
       summary_writer: SummaryWriter object for outputting training statistics.
         Summary writing disabled if set to None.
       summary_writing_frequency: int, frequency with which summaries will be
         written. Lower values will result in slower training.
       seed: int, a seed for DQN's internal RNG, used for initialization and
         sampling actions. If None, will use the current time in nanoseconds.
@@ -197,15 +217,16 @@
         epsilon_train=epsilon_train,
         epsilon_eval=epsilon_eval,
         epsilon_decay_period=epsilon_decay_period,
         optimizer=optimizer,
         summary_writer=summary_writer,
         summary_writing_frequency=summary_writing_frequency,
         seed=seed,
-        allow_partial_reload=allow_partial_reload)
+        allow_partial_reload=allow_partial_reload,
+    )
 
   def _build_networks_and_optimizer(self):
     self._rng, rng = jax.random.split(self._rng)
     self.online_params = self.network_def.init(rng, x=self.state)
     self.optimizer = dqn_agent.create_optimizer(self._optimizer_name)
     self.optimizer_state = self.optimizer.init(self.online_params)
     self.target_network_params = self.online_params
@@ -217,15 +238,16 @@
     # Both replay schemes use the same data structure, but the 'uniform' scheme
     # sets all priorities to the same value (which yields uniform sampling).
     return prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
-        observation_dtype=self.observation_dtype)
+        observation_dtype=self.observation_dtype,
+    )
 
   def _train_step(self):
     """Runs a single training step.
 
     Runs training if both:
       (1) A minimum number of frames have been added to the replay buffer.
       (2) `training_steps` is a multiple of `update_period`.
@@ -245,15 +267,16 @@
             self.preprocess_fn(self.replay_elements['state']),
             self.replay_elements['action'],
             self.preprocess_fn(self.replay_elements['next_state']),
             self.replay_elements['reward'],
             self.replay_elements['terminal'],
             self._kappa,
             self._num_atoms,
-            self.cumulative_gamma)
+            self.cumulative_gamma,
+        )
         if self._replay_scheme == 'prioritized':
           # The original prioritized experience replay uses a linear exponent
           # schedule 0.4 -> 1.0. Comparing the schedule to a fixed exponent of
           # 0.5 on 5 games (Asterix, Pong, Q*Bert, Seaquest, Space Invaders)
           # suggested a fixed exponent actually performs better, except on Pong.
           probs = self.replay_elements['sampling_probabilities']
           loss_weights = 1.0 / jnp.sqrt(probs + 1e-10)
@@ -262,30 +285,37 @@
           # Rainbow and prioritized replay are parametrized by an exponent
           # alpha, but in both cases it is set to 0.5 - for simplicity's sake we
           # leave it as is here, using the more direct sqrt(). Taking the square
           # root "makes sense", as we are dealing with a squared loss.  Add a
           # small nonzero value to the loss to avoid 0 priority items. While
           # technically this may be okay, setting all items to 0 priority will
           # cause troubles, and also result in 1.0 / 0.0 = NaN correction terms.
-          self._replay.set_priority(self.replay_elements['indices'],
-                                    jnp.sqrt(loss + 1e-10))
+          self._replay.set_priority(
+              self.replay_elements['indices'], jnp.sqrt(loss + 1e-10)
+          )
 
           # Weight the loss by the inverse priorities.
           loss = loss_weights * loss
           mean_loss = jnp.mean(loss)
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
           with self.summary_writer.as_default():
-            tf.summary.scalar('QuantileLoss', mean_loss,
-                              step=self.training_steps)
+            tf.summary.scalar(
+                'QuantileLoss', mean_loss, step=self.training_steps
+            )
           self.summary_writer.flush()
           if hasattr(self, 'collector_dispatcher'):
             self.collector_dispatcher.write(
-                [statistics_instance.StatisticsInstance(
-                    'Loss', np.asarray(mean_loss), step=self.training_steps),
-                 ],
-                collector_allowlist=self._collector_allowlist)
+                [
+                    statistics_instance.StatisticsInstance(
+                        'Loss', np.asarray(mean_loss), step=self.training_steps
+                    ),
+                ],
+                collector_allowlist=self._collector_allowlist,
+            )
       if self.training_steps % self.target_update_period == 0:
         self._sync_weights()
 
     self.training_steps += 1
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/rainbow/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/rainbow/rainbow_agent.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/rainbow_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,54 +49,66 @@
 import jax.numpy as jnp
 import numpy as onp
 import optax
 import tensorflow as tf
 
 
 @functools.partial(jax.jit, static_argnums=(0, 3, 12))
-def train(network_def, online_params, target_params, optimizer, optimizer_state,
-          states, actions, next_states, rewards, terminals, loss_weights,
-          support, cumulative_gamma):
+def train(
+    network_def,
+    online_params,
+    target_params,
+    optimizer,
+    optimizer_state,
+    states,
+    actions,
+    next_states,
+    rewards,
+    terminals,
+    loss_weights,
+    support,
+    cumulative_gamma,
+):
   """Run a training step."""
+
   def loss_fn(params, target, loss_multipliers):
     def q_online(state):
       return network_def.apply(params, state, support)
 
     logits = jax.vmap(q_online)(states).logits
     # Fetch the logits for its selected action. We use vmap to perform this
     # indexing across the batch.
     chosen_action_logits = jax.vmap(lambda x, y: x[y])(logits, actions)
     loss = jax.vmap(losses.softmax_cross_entropy_loss_with_logits)(
-        target,
-        chosen_action_logits)
+        target, chosen_action_logits
+    )
     mean_loss = jnp.mean(loss_multipliers * loss)
     return mean_loss, loss
 
   def q_target(state):
     return network_def.apply(target_params, state, support)
 
   grad_fn = jax.value_and_grad(loss_fn, has_aux=True)
-  target = target_distribution(q_target,
-                               next_states,
-                               rewards,
-                               terminals,
-                               support,
-                               cumulative_gamma)
+  target = target_distribution(
+      q_target, next_states, rewards, terminals, support, cumulative_gamma
+  )
 
   # Get the unweighted loss without taking its mean for updating priorities.
   (mean_loss, loss), grad = grad_fn(online_params, target, loss_weights)
-  updates, optimizer_state = optimizer.update(grad, optimizer_state,
-                                              params=online_params)
+  updates, optimizer_state = optimizer.update(
+      grad, optimizer_state, params=online_params
+  )
   online_params = optax.apply_updates(online_params, updates)
   return optimizer_state, online_params, loss, mean_loss
 
 
 @functools.partial(jax.vmap, in_axes=(None, 0, 0, 0, None, None))
-def target_distribution(target_network, next_states, rewards, terminals,
-                        support, cumulative_gamma):
+def target_distribution(
+    target_network, next_states, rewards, terminals, support, cumulative_gamma
+):
   """Builds the C51 target distribution as per Bellemare et al. (2017).
 
   First, we compute the support of the Bellman target, r + gamma Z'. Where Z'
   is the support of the next state distribution:
 
     * Evenly spaced in [-vmax, vmax] if the current state is nonterminal;
     * 0 otherwise (duplicated num_atoms times).
@@ -114,31 +126,44 @@
     terminals: numpy array of batched terminals.
     support: support for the distribution.
     cumulative_gamma: float, cumulative gamma to use.
 
   Returns:
     The target distribution from the replay.
   """
-  is_terminal_multiplier = 1. - terminals.astype(jnp.float32)
+  is_terminal_multiplier = 1.0 - terminals.astype(jnp.float32)
   # Incorporate terminal state to discount factor.
   gamma_with_terminal = cumulative_gamma * is_terminal_multiplier
   target_support = rewards + gamma_with_terminal * support
   next_state_target_outputs = target_network(next_states)
   q_values = jnp.squeeze(next_state_target_outputs.q_values)
   next_qt_argmax = jnp.argmax(q_values)
   probabilities = jnp.squeeze(next_state_target_outputs.probabilities)
   next_probabilities = probabilities[next_qt_argmax]
   return jax.lax.stop_gradient(
-      project_distribution(target_support, next_probabilities, support))
+      project_distribution(target_support, next_probabilities, support)
+  )
 
 
 @functools.partial(jax.jit, static_argnums=(0, 4, 5, 6, 7, 8, 10, 11))
-def select_action(network_def, params, state, rng, num_actions, eval_mode,
-                  epsilon_eval, epsilon_train, epsilon_decay_period,
-                  training_steps, min_replay_history, epsilon_fn, support):
+def select_action(
+    network_def,
+    params,
+    state,
+    rng,
+    num_actions,
+    eval_mode,
+    epsilon_eval,
+    epsilon_train,
+    epsilon_decay_period,
+    training_steps,
+    min_replay_history,
+    epsilon_fn,
+    support,
+):
   """Select an action from the set of available actions.
 
   Chooses an action randomly with probability self._calculate_epsilon(), and
   otherwise acts greedily according to the current Q-value estimates.
 
   Args:
     network_def: Linen Module to use for inference.
@@ -157,57 +182,64 @@
     epsilon_fn: function used to calculate epsilon value (static_argnum).
     support: support for the distribution.
 
   Returns:
     rng: Jax random number generator.
     action: int, the selected action.
   """
-  epsilon = jnp.where(eval_mode,
-                      epsilon_eval,
-                      epsilon_fn(epsilon_decay_period,
-                                 training_steps,
-                                 min_replay_history,
-                                 epsilon_train))
+  epsilon = jnp.where(
+      eval_mode,
+      epsilon_eval,
+      epsilon_fn(
+          epsilon_decay_period,
+          training_steps,
+          min_replay_history,
+          epsilon_train,
+      ),
+  )
 
   rng, rng1, rng2 = jax.random.split(rng, num=3)
   p = jax.random.uniform(rng1)
   return rng, jnp.where(
       p <= epsilon,
       jax.random.randint(rng2, (), 0, num_actions),
-      jnp.argmax(network_def.apply(params, state, support).q_values))
+      jnp.argmax(network_def.apply(params, state, support).q_values),
+  )
 
 
 @gin.configurable
 class JaxRainbowAgent(dqn_agent.JaxDQNAgent):
   """A compact implementation of a simplified Rainbow agent."""
 
-  def __init__(self,
-               num_actions,
-               observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
-               observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
-               stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
-               network=networks.RainbowNetwork,
-               num_atoms=51,
-               vmin=None,
-               vmax=10.,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=20000,
-               update_period=4,
-               target_update_period=8000,
-               epsilon_fn=dqn_agent.linearly_decaying_epsilon,
-               epsilon_train=0.01,
-               epsilon_eval=0.001,
-               epsilon_decay_period=250000,
-               replay_scheme='prioritized',
-               optimizer='adam',
-               seed=None,
-               summary_writer=None,
-               summary_writing_frequency=500,
-               allow_partial_reload=False):
+  def __init__(
+      self,
+      num_actions,
+      observation_shape=dqn_agent.NATURE_DQN_OBSERVATION_SHAPE,
+      observation_dtype=dqn_agent.NATURE_DQN_DTYPE,
+      stack_size=dqn_agent.NATURE_DQN_STACK_SIZE,
+      network=networks.RainbowNetwork,
+      num_atoms=51,
+      vmin=None,
+      vmax=10.0,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=20000,
+      update_period=4,
+      target_update_period=8000,
+      epsilon_fn=dqn_agent.linearly_decaying_epsilon,
+      epsilon_train=0.01,
+      epsilon_eval=0.001,
+      epsilon_decay_period=250000,
+      replay_scheme='prioritized',
+      optimizer='adam',
+      seed=None,
+      summary_writer=None,
+      summary_writing_frequency=500,
+      allow_partial_reload=False,
+  ):
     """Initializes the agent and constructs the necessary components.
 
     Args:
       num_actions: int, number of actions the agent can take at any state.
       observation_shape: tuple of ints or an int. If single int, the observation
         is assumed to be a 2D square.
       observation_dtype: DType, specifies the type of the observations. Note
@@ -222,17 +254,17 @@
       gamma: float, discount factor with the usual RL meaning.
       update_horizon: int, horizon at which updates are performed, the 'n' in
         n-step update.
       min_replay_history: int, number of transitions that should be experienced
         before the agent begins training its value function.
       update_period: int, period between DQN updates.
       target_update_period: int, update period for the target network.
-      epsilon_fn: function expecting 4 parameters:
-        (decay_period, step, warmup_steps, epsilon). This function should return
-        the epsilon value used for exploration during training.
+      epsilon_fn: function expecting 4 parameters: (decay_period, step,
+        warmup_steps, epsilon). This function should return the epsilon value
+        used for exploration during training.
       epsilon_train: float, the value to which the agent's epsilon is eventually
         decayed during training.
       epsilon_eval: float, epsilon used when evaluating the agent.
       epsilon_decay_period: int, length of the epsilon decay schedule.
       replay_scheme: str, 'prioritized' or 'uniform', the sampling scheme of the
         replay memory.
       optimizer: str, name of optimizer to use.
@@ -254,35 +286,37 @@
     self._replay_scheme = replay_scheme
 
     super(JaxRainbowAgent, self).__init__(
         num_actions=num_actions,
         observation_shape=observation_shape,
         observation_dtype=observation_dtype,
         stack_size=stack_size,
-        network=functools.partial(network,
-                                  num_atoms=num_atoms),
+        network=functools.partial(network, num_atoms=num_atoms),
         gamma=gamma,
         update_horizon=update_horizon,
         min_replay_history=min_replay_history,
         update_period=update_period,
         target_update_period=target_update_period,
         epsilon_fn=epsilon_fn,
         epsilon_train=epsilon_train,
         epsilon_eval=epsilon_eval,
         epsilon_decay_period=epsilon_decay_period,
         optimizer=optimizer,
         seed=seed,
         summary_writer=summary_writer,
         summary_writing_frequency=summary_writing_frequency,
-        allow_partial_reload=allow_partial_reload)
+        allow_partial_reload=allow_partial_reload,
+    )
 
   def _build_networks_and_optimizer(self):
     self._rng, rng = jax.random.split(self._rng)
-    self.online_params = self.network_def.init(rng, x=self.state,
-                                               support=self._support)
+    state = self.preprocess_fn(self.state)
+    self.online_params = self.network_def.init(
+        rng, x=state, support=self._support
+    )
     self.optimizer = dqn_agent.create_optimizer(self._optimizer_name)
     self.optimizer_state = self.optimizer.init(self.online_params)
     self.target_network_params = self.online_params
 
   def _build_replay_buffer(self):
     """Creates the replay buffer used by the agent."""
     if self._replay_scheme not in ['uniform', 'prioritized']:
@@ -290,15 +324,16 @@
     # Both replay schemes use the same data structure, but the 'uniform' scheme
     # sets all priorities to the same value (which yields uniform sampling).
     return prioritized_replay_buffer.OutOfGraphPrioritizedReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
-        observation_dtype=self.observation_dtype)
+        observation_dtype=self.observation_dtype,
+    )
 
   # TODO(psc): Refactor this so we have a class _select_action that calls
   # select_action with the right parameters. This will allow us to avoid
   # overriding begin_episode.
   def begin_episode(self, observation):
     """Returns the agent's first action for this episode.
 
@@ -310,27 +345,29 @@
     """
     self._reset_state()
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._train_step()
 
-    self._rng, self.action = select_action(self.network_def,
-                                           self.online_params,
-                                           self.state,
-                                           self._rng,
-                                           self.num_actions,
-                                           self.eval_mode,
-                                           self.epsilon_eval,
-                                           self.epsilon_train,
-                                           self.epsilon_decay_period,
-                                           self.training_steps,
-                                           self.min_replay_history,
-                                           self.epsilon_fn,
-                                           self._support)
+    self._rng, self.action = select_action(
+        self.network_def,
+        self.online_params,
+        self.preprocess_fn(self.state),
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+        self._support,
+    )
     # TODO(psc): Why a numpy array? Why not an int?
     self.action = onp.asarray(self.action)
     return self.action
 
   def step(self, reward, observation):
     """Records the most recent transition and returns the agent's next action.
 
@@ -347,27 +384,29 @@
     self._last_observation = self._observation
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._store_transition(self._last_observation, self.action, reward, False)
       self._train_step()
 
-    self._rng, self.action = select_action(self.network_def,
-                                           self.online_params,
-                                           self.preprocess_fn(self.state),
-                                           self._rng,
-                                           self.num_actions,
-                                           self.eval_mode,
-                                           self.epsilon_eval,
-                                           self.epsilon_train,
-                                           self.epsilon_decay_period,
-                                           self.training_steps,
-                                           self.min_replay_history,
-                                           self.epsilon_fn,
-                                           self._support)
+    self._rng, self.action = select_action(
+        self.network_def,
+        self.online_params,
+        self.preprocess_fn(self.state),
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+        self._support,
+    )
     self.action = onp.asarray(self.action)
     return self.action
 
   def _train_step(self):
     """Runs a single training step.
 
     Runs training if both:
@@ -402,59 +441,67 @@
             self.preprocess_fn(self.replay_elements['state']),
             self.replay_elements['action'],
             self.preprocess_fn(self.replay_elements['next_state']),
             self.replay_elements['reward'],
             self.replay_elements['terminal'],
             loss_weights,
             self._support,
-            self.cumulative_gamma)
+            self.cumulative_gamma,
+        )
 
         if self._replay_scheme == 'prioritized':
           # Rainbow and prioritized replay are parametrized by an exponent
           # alpha, but in both cases it is set to 0.5 - for simplicity's sake we
           # leave it as is here, using the more direct sqrt(). Taking the square
           # root "makes sense", as we are dealing with a squared loss.  Add a
           # small nonzero value to the loss to avoid 0 priority items. While
           # technically this may be okay, setting all items to 0 priority will
           # cause troubles, and also result in 1.0 / 0.0 = NaN correction terms.
-          self._replay.set_priority(self.replay_elements['indices'],
-                                    jnp.sqrt(loss + 1e-10))
-
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+          self._replay.set_priority(
+              self.replay_elements['indices'], jnp.sqrt(loss + 1e-10)
+          )
+
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
           with self.summary_writer.as_default():
-            tf.summary.scalar('CrossEntropyLoss', mean_loss,
-                              step=self.training_steps)
+            tf.summary.scalar(
+                'CrossEntropyLoss', mean_loss, step=self.training_steps
+            )
           self.summary_writer.flush()
           if hasattr(self, 'collector_dispatcher'):
             self.collector_dispatcher.write(
-                [statistics_instance.StatisticsInstance(
-                    'Loss', onp.asarray(mean_loss), step=self.training_steps),
-                 ],
-                collector_allowlist=self._collector_allowlist)
+                [
+                    statistics_instance.StatisticsInstance(
+                        'Loss', onp.asarray(mean_loss), step=self.training_steps
+                    ),
+                ],
+                collector_allowlist=self._collector_allowlist,
+            )
       if self.training_steps % self.target_update_period == 0:
         self._sync_weights()
 
     self.training_steps += 1
 
 
 def project_distribution(supports, weights, target_support):
   """Projects a batch of (support, weights) onto target_support.
 
   Based on equation (7) in (Bellemare et al., 2017):
     https://arxiv.org/abs/1707.06887
   In the rest of the comments we will refer to this equation simply as Eq7.
 
   Args:
-    supports: Jax array of shape (num_dims) defining supports for
-      the distribution.
-    weights: Jax array of shape (num_dims) defining weights on the
-      original support points. Although for the CategoricalDQN agent these
-      weights are probabilities, it is not required that they are.
+    supports: Jax array of shape (num_dims) defining supports for the
+      distribution.
+    weights: Jax array of shape (num_dims) defining weights on the original
+      support points. Although for the CategoricalDQN agent these weights are
+      probabilities, it is not required that they are.
     target_support: Jax array of shape (num_dims) defining support of the
       projected distribution. The values must be monotonically increasing. Vmin
       and Vmax will be inferred from the first and last elements of this Jax
       array, respectively. The values in this Jax array must be equally spaced.
 
   Returns:
     A Jax array of shape (num_dims) with the projection of a batch
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/sac/__init__.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/sac/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/agents/sac/sac_agent.py` & `dopamine_rl-4.0.7/dopamine/jax/agents/sac/sac_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,47 +45,51 @@
 import jax.numpy as jnp
 import numpy as onp
 import optax
 import tensorflow as tf
 
 
 try:
-  logging.warning(
-      ('Setting tf to CPU only, to avoid OOM. '
-       'See https://jax.readthedocs.io/en/latest/gpu_memory_allocation.html '
-       'for more information.'))
+  logging.warning((
+      'Setting tf to CPU only, to avoid OOM. '
+      'See https://jax.readthedocs.io/en/latest/gpu_memory_allocation.html '
+      'for more information.'
+  ))
   tf.config.set_visible_devices([], 'GPU')
 except tf.errors.NotFoundError:
-  logging.info(
-      ('Unable to modify visible devices. '
-       'If you don\'t have a GPU, this is expected.'))
+  logging.info((
+      'Unable to modify visible devices. '
+      "If you don't have a GPU, this is expected."
+  ))
 
 
 gin.constant('sac_agent.IMAGE_DTYPE', onp.uint8)
 gin.constant('sac_agent.STATE_DTYPE', onp.float32)
 
 
 @functools.partial(jax.jit, static_argnums=(0, 1, 2))
-def train(network_def: nn.Module,
-          optim: optax.GradientTransformation,
-          alpha_optim: optax.GradientTransformation,
-          optimizer_state: jnp.ndarray,
-          alpha_optimizer_state: jnp.ndarray,
-          network_params: flax.core.FrozenDict,
-          target_params: flax.core.FrozenDict,
-          log_alpha: jnp.ndarray,
-          key: jnp.ndarray,
-          states: jnp.ndarray,
-          actions: jnp.ndarray,
-          next_states: jnp.ndarray,
-          rewards: jnp.ndarray,
-          terminals: jnp.ndarray,
-          cumulative_gamma: float,
-          target_entropy: float,
-          reward_scale_factor: float) -> Mapping[str, Any]:
+def train(
+    network_def: nn.Module,
+    optim: optax.GradientTransformation,
+    alpha_optim: optax.GradientTransformation,
+    optimizer_state: jnp.ndarray,
+    alpha_optimizer_state: jnp.ndarray,
+    network_params: flax.core.FrozenDict,
+    target_params: flax.core.FrozenDict,
+    log_alpha: jnp.ndarray,
+    key: jnp.ndarray,
+    states: jnp.ndarray,
+    actions: jnp.ndarray,
+    next_states: jnp.ndarray,
+    rewards: jnp.ndarray,
+    terminals: jnp.ndarray,
+    cumulative_gamma: float,
+    target_entropy: float,
+    reward_scale_factor: float,
+) -> Mapping[str, Any]:
   """Run the training step.
 
   Returns a list of updated values and losses.
 
   Args:
     network_def: The SAC network definition.
     optim: The SAC optimizer (which also wraps the SAC parameters).
@@ -112,18 +116,23 @@
   # Get the models from all the optimizers.
   frozen_params = network_params  # For use in loss_fn without apply gradients
 
   batch_size = states.shape[0]
   actions = jnp.reshape(actions, (batch_size, -1))  # Flatten
 
   def loss_fn(
-      params: flax.core.FrozenDict, log_alpha: flax.core.FrozenDict,
-      state: jnp.ndarray, action: jnp.ndarray, reward: jnp.ndarray,
-      next_state: jnp.ndarray, terminal: jnp.ndarray,
-      rng: jnp.ndarray) -> Tuple[jnp.ndarray, Mapping[str, jnp.ndarray]]:
+      params: flax.core.FrozenDict,
+      log_alpha: flax.core.FrozenDict,
+      state: jnp.ndarray,
+      action: jnp.ndarray,
+      reward: jnp.ndarray,
+      next_state: jnp.ndarray,
+      terminal: jnp.ndarray,
+      rng: jnp.ndarray,
+  ) -> Tuple[jnp.ndarray, Mapping[str, jnp.ndarray]]:
     """Calculates the loss for one transition.
 
     Args:
       params: Parameters for the SAC network.
       log_alpha: SAC's log_alpha parameter.
       state: A single state vector.
       action: A single action vector.
@@ -136,43 +145,49 @@
       A tuple containing 1) the combined SAC loss and 2) a mapping containing
         statistics from the loss step.
     """
     rng1, rng2 = jax.random.split(rng, 2)
 
     # J_Q(\theta) from equation (5) in paper.
     q_value_1, q_value_2 = network_def.apply(
-        params, state, action, method=network_def.critic)
+        params, state, action, method=network_def.critic
+    )
     q_value_1 = jnp.squeeze(q_value_1)
     q_value_2 = jnp.squeeze(q_value_2)
 
     target_outputs = network_def.apply(target_params, next_state, rng1, True)
     target_q_value_1, target_q_value_2 = target_outputs.critic
     target_q_value = jnp.squeeze(
-        jnp.minimum(target_q_value_1, target_q_value_2))
+        jnp.minimum(target_q_value_1, target_q_value_2)
+    )
 
-    alpha_value = jnp.exp(log_alpha)
+    alpha_value = jnp.exp(log_alpha)  # pytype: disable=wrong-arg-types  # numpy-scalars
     log_prob = target_outputs.actor.log_probability
     target = reward_scale_factor * reward + cumulative_gamma * (
-        target_q_value - alpha_value * log_prob) * (1. - terminal)
+        target_q_value - alpha_value * log_prob
+    ) * (1.0 - terminal)
     target = jax.lax.stop_gradient(target)
     critic_loss_1 = losses.mse_loss(q_value_1, target)
     critic_loss_2 = losses.mse_loss(q_value_2, target)
     critic_loss = jnp.mean(critic_loss_1 + critic_loss_2)
 
     # J_{\pi}(\phi) from equation (9) in paper.
     mean_action, sampled_action, action_log_prob = network_def.apply(
-        params, state, rng2, method=network_def.actor)
+        params, state, rng2, method=network_def.actor
+    )
 
     # We use frozen_params so that gradients can flow back to the actor without
     # being used to update the critic.
     q_value_no_grad_1, q_value_no_grad_2 = network_def.apply(
-        frozen_params, state, sampled_action, method=network_def.critic)
+        frozen_params, state, sampled_action, method=network_def.critic
+    )
     no_grad_q_value = jnp.squeeze(
-        jnp.minimum(q_value_no_grad_1, q_value_no_grad_2))
-    alpha_value = jnp.exp(jax.lax.stop_gradient(log_alpha))
+        jnp.minimum(q_value_no_grad_1, q_value_no_grad_2)
+    )
+    alpha_value = jnp.exp(jax.lax.stop_gradient(log_alpha))  # pytype: disable=wrong-arg-types  # numpy-scalars
     policy_loss = jnp.mean(alpha_value * action_log_prob - no_grad_q_value)
 
     # J(\alpha) from equation (18) in paper.
     entropy_diff = -action_log_prob - target_entropy
     alpha_loss = jnp.mean(log_alpha * jax.lax.stop_gradient(entropy_diff))
 
     # Giving a smaller weight to the critic empirically gives better results
@@ -181,37 +196,48 @@
         'critic_loss': critic_loss,
         'policy_loss': policy_loss,
         'alpha_loss': alpha_loss,
         'critic_value_1': q_value_1,
         'critic_value_2': q_value_2,
         'target_value_1': target_q_value_1,
         'target_value_2': target_q_value_2,
-        'mean_action': mean_action
+        'mean_action': mean_action,
     }
 
   grad_fn = jax.vmap(
       jax.value_and_grad(loss_fn, argnums=(0, 1), has_aux=True),
-      in_axes=(None, None, 0, 0, 0, 0, 0, 0))
+      in_axes=(None, None, 0, 0, 0, 0, 0, 0),
+  )
 
   rng = jnp.stack(jax.random.split(key, num=batch_size))
-  (_, aux_vars), gradients = grad_fn(network_params, log_alpha, states, actions,
-                                     rewards, next_states, terminals, rng)
+  (_, aux_vars), gradients = grad_fn(
+      network_params,
+      log_alpha,
+      states,
+      actions,
+      rewards,
+      next_states,
+      terminals,
+      rng,
+  )
 
   # This calculates the mean gradient/aux_vars using the individual
   # gradients/aux_vars from each item in the batch.
   gradients = jax.tree_map(functools.partial(jnp.mean, axis=0), gradients)
   aux_vars = jax.tree_map(functools.partial(jnp.mean, axis=0), aux_vars)
   network_gradient, alpha_gradient = gradients
 
   # Apply gradients to all the optimizers.
-  updates, optimizer_state = optim.update(network_gradient, optimizer_state,
-                                          params=network_params)
+  updates, optimizer_state = optim.update(
+      network_gradient, optimizer_state, params=network_params
+  )
   network_params = optax.apply_updates(network_params, updates)
   alpha_updates, alpha_optimizer_state = alpha_optim.update(
-      alpha_gradient, alpha_optimizer_state, params=log_alpha)
+      alpha_gradient, alpha_optimizer_state, params=log_alpha
+  )
   log_alpha = optax.apply_updates(log_alpha, alpha_updates)
 
   # Compile everything in a dict.
   returns = {
       'network_params': network_params,
       'log_alpha': log_alpha,
       'optimizer_state': optimizer_state,
@@ -246,48 +272,51 @@
 
   Returns:
     rng: Jax random number generator.
     action: int, the selected action.
   """
   rng, rng2 = jax.random.split(rng)
   greedy_a, sampled_a, _ = network_def.apply(
-      params, state, rng2, method=network_def.actor)
+      params, state, rng2, method=network_def.actor
+  )
   return rng, jnp.where(eval_mode, greedy_a, sampled_a)
 
 
 @gin.configurable
 class SACAgent(dqn_agent.JaxDQNAgent):
   """A JAX implementation of the SAC agent."""
 
-  def __init__(self,
-               action_shape,
-               action_limits,
-               observation_shape,
-               action_dtype=jnp.float32,
-               observation_dtype=jnp.float32,
-               reward_scale_factor=1.0,
-               stack_size=1,
-               network=continuous_networks.SACNetwork,
-               num_layers=2,
-               hidden_units=256,
-               gamma=0.99,
-               update_horizon=1,
-               min_replay_history=20000,
-               update_period=1,
-               target_update_type='soft',
-               target_update_period=1000,
-               target_smoothing_coefficient=0.005,
-               target_entropy=None,
-               eval_mode=False,
-               optimizer='adam',
-               summary_writer=None,
-               summary_writing_frequency=500,
-               allow_partial_reload=False,
-               seed=None,
-               collector_allowlist=('tensorboard')):
+  def __init__(
+      self,
+      action_shape,
+      action_limits,
+      observation_shape,
+      action_dtype=jnp.float32,
+      observation_dtype=jnp.float32,
+      reward_scale_factor=1.0,
+      stack_size=1,
+      network=continuous_networks.SACNetwork,
+      num_layers=2,
+      hidden_units=256,
+      gamma=0.99,
+      update_horizon=1,
+      min_replay_history=20000,
+      update_period=1,
+      target_update_type='soft',
+      target_update_period=1000,
+      target_smoothing_coefficient=0.005,
+      target_entropy=None,
+      eval_mode=False,
+      optimizer='adam',
+      summary_writer=None,
+      summary_writing_frequency=500,
+      allow_partial_reload=False,
+      seed=None,
+      collector_allowlist='tensorboard',
+  ):
     r"""Initializes the agent and constructs the necessary components.
 
     Args:
       action_shape: int or tuple, dimensionality of the action space.
       action_limits: pair of lower and higher bounds for actions.
       observation_shape: tuple of ints describing the observation shape.
       action_dtype: jnp.dtype, specifies the type of the actions.
@@ -335,46 +364,50 @@
       action_shape = (action_shape,)
 
     # If target_entropy is None, set to default value.
     if target_entropy is None:
       action_dim = functools.reduce(operator.mul, action_shape, 1.0)
       target_entropy = -0.5 * action_dim
     seed = int(time.time() * 1e6) if seed is None else seed
-    logging.info('Creating %s agent with the following parameters:',
-                 self.__class__.__name__)
+    logging.info(
+        'Creating %s agent with the following parameters:',
+        self.__class__.__name__,
+    )
     logging.info('\t action_shape: %s', action_shape)
     logging.info('\t action_dtype: %s', action_dtype)
     logging.info('\t action_limits: %s', action_limits)
     logging.info('\t observation_shape: %s', observation_shape)
     logging.info('\t observation_dtype: %s', observation_dtype)
     logging.info('\t reward_scale_factor: %f', reward_scale_factor)
     logging.info('\t num_layers: %d', num_layers)
     logging.info('\t hidden_units: %d', hidden_units)
     logging.info('\t gamma: %f', gamma)
     logging.info('\t update_horizon: %f', update_horizon)
     logging.info('\t min_replay_history: %d', min_replay_history)
     logging.info('\t update_period: %d', update_period)
     logging.info('\t target_update_type: %s', target_update_type)
     logging.info('\t target_update_period: %d', target_update_period)
-    logging.info('\t target_smoothing_coefficient: %f',
-                 target_smoothing_coefficient)
+    logging.info(
+        '\t target_smoothing_coefficient: %f', target_smoothing_coefficient
+    )
     logging.info('\t target_entropy: %f', target_entropy)
     logging.info('\t optimizer: %s', optimizer)
     logging.info('\t seed: %d', seed)
 
     self.action_shape = action_shape
     self.action_dtype = action_dtype
     self.observation_shape = tuple(observation_shape)
     self.observation_dtype = observation_dtype
     self.reward_scale_factor = reward_scale_factor
     self.stack_size = stack_size
     self.action_limits = action_limits
     action_limits = tuple(tuple(x.reshape(-1)) for x in action_limits)
-    self.network_def = network(action_shape, num_layers, hidden_units,
-                               action_limits)
+    self.network_def = network(
+        action_shape, num_layers, hidden_units, action_limits
+    )
     self.gamma = gamma
     self.update_horizon = update_horizon
     self.cumulative_gamma = math.pow(gamma, update_horizon)
     self.min_replay_history = min_replay_history
     self.update_period = update_period
     self.target_update_type = target_update_type
     self.target_update_period = target_update_period
@@ -421,28 +454,34 @@
     return circular_replay_buffer.OutOfGraphReplayBuffer(
         observation_shape=self.observation_shape,
         stack_size=self.stack_size,
         update_horizon=self.update_horizon,
         gamma=self.gamma,
         observation_dtype=self.observation_dtype,
         action_shape=self.action_shape,
-        action_dtype=self.action_dtype)
+        action_dtype=self.action_dtype,
+    )
 
   def _maybe_sync_weights(self):
     """Syncs the target weights with the online weights."""
-    if (self.target_update_type == 'hard' and
-        self.training_steps % self.target_update_period != 0):
+    if (
+        self.target_update_type == 'hard'
+        and self.training_steps % self.target_update_period != 0
+    ):
       return
 
     def _sync_weights(target_p, online_p):
-      return (self.target_smoothing_coefficient * online_p +
-              (1 - self.target_smoothing_coefficient) * target_p)
-
-    self.target_params = jax.tree_map(_sync_weights, self.target_params,
-                                      self.network_params)
+      return (
+          self.target_smoothing_coefficient * online_p
+          + (1 - self.target_smoothing_coefficient) * target_p
+      )
+
+    self.target_params = jax.tree_map(
+        _sync_weights, self.target_params, self.network_params
+    )
 
   def begin_episode(self, observation):
     """Returns the agent's first action for this episode.
 
     Args:
       observation: numpy array, the environment's initial observation.
 
@@ -452,22 +491,30 @@
     self._reset_state()
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._train_step()
 
     if self._replay.add_count > self.min_replay_history:
-      self._rng, self.action = select_action(self.network_def,
-                                             self.network_params, self.state,
-                                             self._rng, self.eval_mode)
+      self._rng, self.action = select_action(
+          self.network_def,
+          self.network_params,
+          self.state,
+          self._rng,
+          self.eval_mode,
+      )
     else:
       self._rng, action_rng = jax.random.split(self._rng)
-      self.action = jax.random.uniform(action_rng, self.action_shape,
-                                       self.action_dtype, self.action_limits[0],
-                                       self.action_limits[1])
+      self.action = jax.random.uniform(
+          action_rng,
+          self.action_shape,
+          self.action_dtype,
+          self.action_limits[0],
+          self.action_limits[1],
+      )
     self.action = onp.asarray(self.action)
     return self.action
 
   def step(self, reward, observation):
     """Records the most recent transition and returns the agent's next action.
 
     We store the observation of the last time step since we want to store it
@@ -484,22 +531,30 @@
     self._record_observation(observation)
 
     if not self.eval_mode:
       self._store_transition(self._last_observation, self.action, reward, False)
       self._train_step()
 
     if self._replay.add_count > self.min_replay_history:
-      self._rng, self.action = select_action(self.network_def,
-                                             self.network_params, self.state,
-                                             self._rng, self.eval_mode)
+      self._rng, self.action = select_action(
+          self.network_def,
+          self.network_params,
+          self.state,
+          self._rng,
+          self.eval_mode,
+      )
     else:
       self._rng, action_rng = jax.random.split(self._rng)
-      self.action = jax.random.uniform(action_rng, self.action_shape,
-                                       self.action_dtype, self.action_limits[0],
-                                       self.action_limits[1])
+      self.action = jax.random.uniform(
+          action_rng,
+          self.action_shape,
+          self.action_dtype,
+          self.action_limits[0],
+          self.action_limits[1],
+      )
     self.action = onp.asarray(self.action)
     return self.action
 
   def _train_step(self):
     """Runs a single training step.
 
     Runs training if both:
@@ -511,45 +566,62 @@
     """
     if self._replay.add_count > self.min_replay_history:
       if self.training_steps % self.update_period == 0:
         self._sample_from_replay_buffer()
         self._rng, key = jax.random.split(self._rng)
 
         train_returns = train(
-            self.network_def, self.network_optimizer, self.alpha_optimizer,
-            self.optimizer_state, self.alpha_optimizer_state,
-            self.network_params, self.target_params, self.log_alpha,
-            key, self.replay_elements['state'],
-            self.replay_elements['action'], self.replay_elements['next_state'],
-            self.replay_elements['reward'], self.replay_elements['terminal'],
-            self.cumulative_gamma, self.target_entropy,
-            self.reward_scale_factor)
+            self.network_def,
+            self.network_optimizer,
+            self.alpha_optimizer,
+            self.optimizer_state,
+            self.alpha_optimizer_state,
+            self.network_params,
+            self.target_params,
+            self.log_alpha,
+            key,
+            self.replay_elements['state'],
+            self.replay_elements['action'],
+            self.replay_elements['next_state'],
+            self.replay_elements['reward'],
+            self.replay_elements['terminal'],
+            self.cumulative_gamma,
+            self.target_entropy,
+            self.reward_scale_factor,
+        )
 
         self.network_params = train_returns['network_params']
         self.optimizer_state = train_returns['optimizer_state']
         self.log_alpha = train_returns['log_alpha']
         self.alpha_optimizer_state = train_returns['alpha_optimizer_state']
 
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
 
           statistics = []
           for k in train_returns:
             if k.startswith('Losses') or k.startswith('Values'):
-              self.summary_writer.scalar(k, train_returns[k],
-                                         self.training_steps)
+              self.summary_writer.scalar(
+                  k, train_returns[k], self.training_steps
+              )
               if hasattr(self, 'collector_dispatcher'):
                 statistics.append(
                     statistics_instance.StatisticsInstance(
-                        k, onp.asarray(train_returns[k]),
-                        step=self.training_steps))
+                        k,
+                        onp.asarray(train_returns[k]),
+                        step=self.training_steps,
+                    )
+                )
           if hasattr(self, 'collector_dispatcher'):
             self.collector_dispatcher.write(
-                statistics, collector_allowlist=self._collector_allowlist)
+                statistics, collector_allowlist=self._collector_allowlist
+            )
           self.summary_writer.flush()
         self._maybe_sync_weights()
     self.training_steps += 1
 
   def bundle_and_checkpoint(self, checkpoint_dir, iteration_number):
     """Returns a self-contained bundle of the agent's state.
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/continuous_networks.py` & `dopamine_rl-4.0.7/dopamine/jax/continuous_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,37 +27,41 @@
 
 tfd = tfp.distributions
 tfb = tfp.bijectors
 
 
 class SacActorOutput(NamedTuple):
   """The output of a SAC actor."""
+
   mean_action: jnp.ndarray
   sampled_action: jnp.ndarray
   log_probability: jnp.ndarray
 
 
 class SacCriticOutput(NamedTuple):
   """The output of a SAC critic."""
+
   q_value1: jnp.ndarray
   q_value2: jnp.ndarray
 
 
 class SacOutput(NamedTuple):
   """The output of a SACNetwork, including the actor and critic outputs."""
+
   actor: SacActorOutput
   critic: SacCriticOutput
 
 
 class _Tanh(tfb.Tanh):
 
   def _inverse(self, y):
     # We perform clipping in the _inverse function, as is done in TF-Agents.
     y = jnp.where(
-        jnp.less_equal(jnp.abs(y), 1.), tf.clip(y, -0.99999997, 0.99999997), y)
+        jnp.less_equal(jnp.abs(y), 1.0), tf.clip(y, -0.99999997, 0.99999997), y
+    )
     return jnp.arctanh(y)
 
 
 def _transform_distribution(dist, mean, magnitude):
   """Scales the input normal distribution to be within the action limits.
 
   Args:
@@ -72,50 +76,52 @@
       tfb.Shift(mean)(tfb.Scale(magnitude)),
       _Tanh(),
   ])
   dist = tfd.TransformedDistribution(dist, bijectors)
   return dist
 
 
-def _shifted_uniform(minval=0., maxval=1.0, dtype=jnp.float32):
-
+def _shifted_uniform(minval=0.0, maxval=1.0, dtype=jnp.float32):
   def init(key, shape, dtype=dtype):
     return jax.random.uniform(
-        key, shape=shape, minval=minval, maxval=maxval, dtype=dtype)
+        key, shape=shape, minval=minval, maxval=maxval, dtype=dtype
+    )
 
   return init
 
 
 class SACCriticNetwork(nn.Module):
   """A simple critic network used in SAC."""
+
   num_layers: int = 2
   hidden_units: int = 256
 
   @nn.compact
   def __call__(self, state: jnp.ndarray, action: jnp.ndarray) -> jnp.ndarray:
     kernel_initializer = jax.nn.initializers.glorot_uniform()
 
     # Preprocess inputs
     a = action.reshape(-1)  # flatten
     x = state.astype(jnp.float32)
     x = x.reshape(-1)  # flatten
     x = jnp.concatenate((x, a))
 
     for _ in range(self.num_layers):
-      x = nn.Dense(
-          features=self.hidden_units, kernel_init=kernel_initializer)(
-              x)
+      x = nn.Dense(features=self.hidden_units, kernel_init=kernel_initializer)(
+          x
+      )
       x = nn.relu(x)
 
     return nn.Dense(features=1, kernel_init=kernel_initializer)(x)
 
 
 @gin.configurable
 class SACNetwork(nn.Module):
   """Non-convolutional value and policy networks for SAC."""
+
   action_shape: Tuple[int, ...]
   num_layers: int = 2
   hidden_units: int = 256
   action_limits: Optional[Tuple[Tuple[float, ...], Tuple[float, ...]]] = None
 
   def setup(self):
     action_dim = functools.reduce(operator.mul, self.action_shape, 1)
@@ -128,20 +134,20 @@
     self._critic2 = SACCriticNetwork(self.num_layers, self.hidden_units)
 
     self._actor_layers = [
         nn.Dense(features=self.hidden_units, kernel_init=kernel_initializer)
         for _ in range(self.num_layers)
     ]
     self._actor_final_layer = nn.Dense(
-        features=action_dim * 2, kernel_init=kernel_initializer)
+        features=action_dim * 2, kernel_init=kernel_initializer
+    )
 
-  def __call__(self,
-               state: jnp.ndarray,
-               key: jnp.ndarray,
-               mean_action: bool = True) -> SacOutput:
+  def __call__(
+      self, state: jnp.ndarray, key: jnp.ndarray, mean_action: bool = True
+  ) -> SacOutput:
     """Calls the SAC actor/critic networks.
 
     This has two important purposes:
       1. It is used to initialize all parameters of both networks.
       2. It is used to efficiently calculate the outputs of both the actor
         and critic networks on a single input.
 
@@ -220,8 +226,9 @@
       state: An input state.
       action: An action to compute the value of.
 
     Returns:
       A named tuple containing the Q values of each network.
     """
     return SacCriticOutput(
-        self._critic1(state, action), self._critic2(state, action))
+        self._critic1(state, action), self._critic2(state, action)
+    )
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/losses.py` & `dopamine_rl-4.0.7/dopamine/jax/losses.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Various losses used by the Dopamine JAX agents."""
 from flax import linen as nn
 import jax.numpy as jnp
 
 
-def huber_loss(targets: jnp.array,
-               predictions: jnp.array,
-               delta: float = 1.0) -> jnp.ndarray:
+def huber_loss(
+    targets: jnp.ndarray, predictions: jnp.ndarray, delta: float = 1.0
+) -> jnp.ndarray:
   """Implementation of the Huber loss with threshold delta.
 
   Let `x = |targets - predictions|`, the Huber loss is defined as:
   `0.5 * x^2` if `x <= delta`
   `0.5 * delta^2 + delta * (x - delta)` otherwise.
 
   Args:
@@ -31,21 +31,20 @@
     predictions: Prediction values.
     delta: Threshold.
 
   Returns:
     Huber loss.
   """
   x = jnp.abs(targets - predictions)
-  return jnp.where(x <= delta,
-                   0.5 * x**2,
-                   0.5 * delta**2 + delta * (x - delta))
+  return jnp.where(x <= delta, 0.5 * x**2, 0.5 * delta**2 + delta * (x - delta))
 
 
-def mse_loss(targets: jnp.array, predictions: jnp.array) -> jnp.ndarray:
+def mse_loss(targets: jnp.ndarray, predictions: jnp.ndarray) -> jnp.ndarray:
   """Implementation of the mean squared error loss."""
   return jnp.power((targets - predictions), 2)
 
 
-def softmax_cross_entropy_loss_with_logits(labels: jnp.array,
-                                           logits: jnp.array) -> jnp.ndarray:
+def softmax_cross_entropy_loss_with_logits(
+    labels: jnp.ndarray, logits: jnp.ndarray
+) -> jnp.ndarray:
   """Implementation of the softmax cross entropy loss."""
   return -jnp.sum(labels * nn.log_softmax(logits))
```

### Comparing `dopamine_rl-4.0.6/dopamine/jax/networks.py` & `dopamine_rl-4.0.7/dopamine/jax/networks.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,79 +13,175 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Various networks for Jax Dopamine agents."""
 
 import itertools
 import time
 from typing import Optional, Sequence, Tuple, Union
-
+from absl import logging
 from dopamine.discrete_domains import atari_lib
 from flax import linen as nn
 import gin
 import jax
 import jax.numpy as jnp
 import numpy as onp
 
 
 gin.constant('jax_networks.CARTPOLE_OBSERVATION_DTYPE', jnp.float64)
-gin.constant('jax_networks.CARTPOLE_MIN_VALS',
-             (-2.4, -5., -onp.pi/12., -onp.pi*2.))
-gin.constant('jax_networks.CARTPOLE_MAX_VALS',
-             (2.4, 5., onp.pi/12., onp.pi*2.))
+gin.constant(
+    'jax_networks.CARTPOLE_MIN_VALS',
+    (-2.4, -5.0, -onp.pi / 12.0, -onp.pi * 2.0),
+)
+gin.constant(
+    'jax_networks.CARTPOLE_MAX_VALS', (2.4, 5.0, onp.pi / 12.0, onp.pi * 2.0)
+)
 gin.constant('jax_networks.ACROBOT_OBSERVATION_DTYPE', jnp.float64)
-gin.constant('jax_networks.ACROBOT_MIN_VALS',
-             (-1., -1., -1., -1., -5., -5.))
-gin.constant('jax_networks.ACROBOT_MAX_VALS',
-             (1., 1., 1., 1., 5., 5.))
+gin.constant(
+    'jax_networks.ACROBOT_MIN_VALS', (-1.0, -1.0, -1.0, -1.0, -5.0, -5.0)
+)
+gin.constant('jax_networks.ACROBOT_MAX_VALS', (1.0, 1.0, 1.0, 1.0, 5.0, 5.0))
 gin.constant('jax_networks.LUNAR_OBSERVATION_DTYPE', jnp.float64)
 gin.constant('jax_networks.MOUNTAINCAR_OBSERVATION_DTYPE', jnp.float64)
 gin.constant('jax_networks.MOUNTAINCAR_MIN_VALS', (-1.2, -0.07))
 gin.constant('jax_networks.MOUNTAINCAR_MAX_VALS', (0.6, 0.07))
 
 
 def preprocess_atari_inputs(x):
   """Input normalization for Atari 2600 input frames."""
-  return x.astype(jnp.float32) / 255.
+  return x.astype(jnp.float32) / 255.0
 
 
 identity_preprocess_fn = lambda x: x
 
 
+@gin.configurable
+class Stack(nn.Module):
+  """Stack of pooling and convolutional blocks with residual connections."""
+
+  num_ch: int
+  num_blocks: int
+  use_max_pooling: bool = True
+
+  @nn.compact
+  def __call__(self, x):
+    initializer = nn.initializers.xavier_uniform()
+    conv_out = nn.Conv(
+        features=self.num_ch,
+        kernel_size=(3, 3),
+        strides=1,
+        kernel_init=initializer,
+        padding='SAME',
+    )(x)
+    if self.use_max_pooling:
+      conv_out = nn.max_pool(
+          conv_out, window_shape=(3, 3), padding='SAME', strides=(2, 2)
+      )
+
+    for _ in range(self.num_blocks):
+      block_input = conv_out
+      conv_out = nn.relu(conv_out)
+      conv_out = nn.Conv(
+          features=self.num_ch, kernel_size=(3, 3), strides=1, padding='SAME'
+      )(conv_out)
+      conv_out = nn.relu(conv_out)
+      conv_out = nn.Conv(
+          features=self.num_ch, kernel_size=(3, 3), strides=1, padding='SAME'
+      )(conv_out)
+      conv_out += block_input
+
+    return conv_out
+
+
+@gin.configurable
+class ImpalaEncoder(nn.Module):
+  """Impala Network which also outputs penultimate representation layers."""
+
+  nn_scale: int = 1
+  stack_sizes: Tuple[int, ...] = (16, 32, 32)
+  num_blocks: int = 2
+
+  def setup(self):
+    logging.info('\t Creating %s ...', self.__class__.__name__)
+    logging.info('\t Creating ImpalaDQNNetwork ...')
+    logging.info('\t num_blocks: %s', self.num_blocks)
+    logging.info('\t nn_scale: %s', self.nn_scale)
+    logging.info('\t stack_sizes: %s', self.stack_sizes)
+    self._stacks = [
+        Stack(num_ch=stack_size * self.nn_scale, num_blocks=self.num_blocks)
+        for stack_size in self.stack_sizes
+    ]
+
+  @nn.compact
+  def __call__(self, x):
+    for stack in self._stacks:
+      x = stack(x)
+    return nn.relu(x)
+
+
+### DQN Network with ImpalaEncoder ###
+@gin.configurable
+class ImpalaDQNNetwork(nn.Module):
+  """The convolutional network used to compute the agent's Q-values."""
+
+  num_actions: int
+  inputs_preprocessed: bool = False
+  nn_scale: int = 1
+
+  def setup(self):
+    self.encoder = ImpalaEncoder(nn_scale=self.nn_scale)
+
+  @nn.compact
+  def __call__(self, x):
+    initializer = nn.initializers.xavier_uniform()
+    if not self.inputs_preprocessed:
+      x = preprocess_atari_inputs(x)
+    x = self.encoder(x)
+    x = x.reshape((-1))  # flatten
+    x = nn.Dense(features=512, kernel_init=initializer)(x)
+    x = nn.relu(x)
+    q_values = nn.Dense(features=self.num_actions, kernel_init=initializer)(x)
+    return atari_lib.DQNNetworkType(q_values)
+
+
 ### DQN Networks ###
 @gin.configurable
 class NatureDQNNetwork(nn.Module):
   """The convolutional network used to compute the agent's Q-values."""
+
   num_actions: int
   inputs_preprocessed: bool = False
 
   @nn.compact
   def __call__(self, x):
     initializer = nn.initializers.xavier_uniform()
     if not self.inputs_preprocessed:
       x = preprocess_atari_inputs(x)
-    x = nn.Conv(features=32, kernel_size=(8, 8), strides=(4, 4),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(4, 4), strides=(2, 2),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=32, kernel_size=(8, 8), strides=(4, 4), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(4, 4), strides=(2, 2), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape((-1))  # flatten
     x = nn.Dense(features=512, kernel_init=initializer)(x)
     x = nn.relu(x)
-    q_values = nn.Dense(features=self.num_actions,
-                        kernel_init=initializer)(x)
+    q_values = nn.Dense(features=self.num_actions, kernel_init=initializer)(x)
     return atari_lib.DQNNetworkType(q_values)
 
 
 @gin.configurable
 class ClassicControlDQNNetwork(nn.Module):
   """Jax DQN network for classic control environments."""
+
   num_actions: int
   num_layers: int = 2
   hidden_units: int = 512
   min_vals: Union[None, Tuple[float, ...]] = None
   max_vals: Union[None, Tuple[float, ...]] = None
   inputs_preprocessed: bool = False
 
@@ -93,17 +189,19 @@
     if self.min_vals is not None:
       assert self.max_vals is not None
       self._min_vals = jnp.array(self.min_vals)
       self._max_vals = jnp.array(self.max_vals)
     initializer = nn.initializers.xavier_uniform()
     self.layers = [
         nn.Dense(features=self.hidden_units, kernel_init=initializer)
-        for _ in range(self.num_layers)]
-    self.final_layer = nn.Dense(features=self.num_actions,
-                                kernel_init=initializer)
+        for _ in range(self.num_layers)
+    ]
+    self.final_layer = nn.Dense(
+        features=self.num_actions, kernel_init=initializer
+    )
 
   def __call__(self, x):
     if not self.inputs_preprocessed:
       x = x.astype(jnp.float32)
       x = x.reshape((-1))  # flatten
       if self.min_vals is not None:
         x -= self._min_vals
@@ -126,28 +224,31 @@
   Adapted from Will Dabney's (wdabney@) TF implementation for JAX.
 
   From the paper:
   G.D. Konidaris, S. Osentoski and P.S. Thomas. (2011)
   Value Function Approximation in Reinforcement Learning using the Fourier Basis
   """
 
-  def __init__(self,
-               nvars: int,
-               min_vals: Union[float, Sequence[float]] = 0.0,
-               max_vals: Optional[Union[float, Sequence[float]]] = None,
-               order: int = 3):
+  def __init__(
+      self,
+      nvars: int,
+      min_vals: Union[float, Sequence[float]] = 0.0,
+      max_vals: Optional[Union[float, Sequence[float]]] = None,
+      order: int = 3,
+  ):
     self.order = order
     self.min_vals = jnp.array(min_vals)
     self.max_vals = max_vals
     terms = itertools.product(range(order + 1), repeat=nvars)
     if max_vals is not None:
       assert len(self.min_vals) == len(self.max_vals)
       self.max_vals = jnp.array(self.max_vals)
       self.denominator = [
-          max_vals[i] - min_vals[i] for i in range(len(min_vals))]
+          max_vals[i] - min_vals[i] for i in range(len(min_vals))
+      ]
 
     # Removing first iterate because it corresponds to the constant bias
     self.multipliers = jnp.array([list(map(int, x)) for x in terms][1:])
 
   def scale(self, values):
     shifted = values - self.min_vals
     if self.max_vals is None:
@@ -160,70 +261,81 @@
     scaled = jnp.array(self.scale(features))
     return jnp.cos(jnp.pi * jnp.matmul(scaled, jnp.transpose(self.multipliers)))
 
 
 @gin.configurable
 class JaxFourierDQNNetwork(nn.Module):
   """Fourier-basis for DQN-like agents."""
+
   num_actions: int
   min_vals: Optional[Sequence[float]] = None
   max_vals: Optional[Sequence[float]] = None
   fourier_basis_order: int = 3
 
   @nn.compact
   def __call__(self, x):
     initializer = nn.initializers.xavier_uniform()
     x = x.astype(jnp.float32)
     x = x.reshape((-1))  # flatten
-    x = FourierBasis(x.shape[-1], self.min_vals, self.max_vals,
-                     order=self.fourier_basis_order).compute_features(x)
-    q_values = nn.Dense(features=self.num_actions,
-                        kernel_init=initializer, use_bias=False)(x)
+    x = FourierBasis(
+        x.shape[-1],
+        self.min_vals,
+        self.max_vals,
+        order=self.fourier_basis_order,
+    ).compute_features(x)
+    q_values = nn.Dense(
+        features=self.num_actions, kernel_init=initializer, use_bias=False
+    )(x)
     return atari_lib.DQNNetworkType(q_values)
 
 
 ### Rainbow Networks ###
 @gin.configurable
 class RainbowNetwork(nn.Module):
   """Convolutional network used to compute the agent's return distributions."""
+
   num_actions: int
   num_atoms: int
   inputs_preprocessed: bool = False
 
   @nn.compact
   def __call__(self, x, support):
     initializer = nn.initializers.variance_scaling(
-        scale=1.0 / jnp.sqrt(3.0),
-        mode='fan_in',
-        distribution='uniform')
+        scale=1.0 / jnp.sqrt(3.0), mode='fan_in', distribution='uniform'
+    )
     if not self.inputs_preprocessed:
       x = preprocess_atari_inputs(x)
-    x = nn.Conv(features=32, kernel_size=(8, 8), strides=(4, 4),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(4, 4), strides=(2, 2),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=32, kernel_size=(8, 8), strides=(4, 4), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(4, 4), strides=(2, 2), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape((-1))  # flatten
     x = nn.Dense(features=512, kernel_init=initializer)(x)
     x = nn.relu(x)
-    x = nn.Dense(features=self.num_actions * self.num_atoms,
-                 kernel_init=initializer)(x)
+    x = nn.Dense(
+        features=self.num_actions * self.num_atoms, kernel_init=initializer
+    )(x)
     logits = x.reshape((self.num_actions, self.num_atoms))
     probabilities = nn.softmax(logits)
     q_values = jnp.sum(support * probabilities, axis=1)
     return atari_lib.RainbowNetworkType(q_values, logits, probabilities)
 
 
 @gin.configurable
 class ClassicControlRainbowNetwork(nn.Module):
   """Jax Rainbow network for classic control environments."""
+
   num_actions: int
   num_atoms: int
   num_layers: int = 2
   hidden_units: int = 512
   min_vals: Union[None, Tuple[float, ...]] = None
   max_vals: Union[None, Tuple[float, ...]] = None
   inputs_preprocessed: bool = False
@@ -231,17 +343,19 @@
   def setup(self):
     if self.min_vals is not None:
       self._min_vals = jnp.array(self.min_vals)
       self._max_vals = jnp.array(self.max_vals)
     initializer = nn.initializers.xavier_uniform()
     self.layers = [
         nn.Dense(features=self.hidden_units, kernel_init=initializer)
-        for _ in range(self.num_layers)]
-    self.final_layer = nn.Dense(features=self.num_actions * self.num_atoms,
-                                kernel_init=initializer)
+        for _ in range(self.num_layers)
+    ]
+    self.final_layer = nn.Dense(
+        features=self.num_actions * self.num_atoms, kernel_init=initializer
+    )
 
   def __call__(self, x, support):
     if not self.inputs_preprocessed:
       x = x.astype(jnp.float32)
       x = x.reshape((-1))  # flatten
       if self.min_vals is not None:
         x -= self._min_vals
@@ -256,87 +370,97 @@
     q_values = jnp.sum(support * probabilities, axis=1)
     return atari_lib.RainbowNetworkType(q_values, logits, probabilities)
 
 
 ### Implicit Quantile Networks ###
 class ImplicitQuantileNetwork(nn.Module):
   """The Implicit Quantile Network (Dabney et al., 2018).."""
+
   num_actions: int
   quantile_embedding_dim: int
   inputs_preprocessed: bool = False
 
   @nn.compact
   def __call__(self, x, num_quantiles, rng):
     initializer = nn.initializers.variance_scaling(
-        scale=1.0 / jnp.sqrt(3.0),
-        mode='fan_in',
-        distribution='uniform')
+        scale=1.0 / jnp.sqrt(3.0), mode='fan_in', distribution='uniform'
+    )
     if not self.inputs_preprocessed:
       x = preprocess_atari_inputs(x)
-    x = nn.Conv(features=32, kernel_size=(8, 8), strides=(4, 4),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(4, 4), strides=(2, 2),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=32, kernel_size=(8, 8), strides=(4, 4), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(4, 4), strides=(2, 2), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape((-1))  # flatten
     state_vector_length = x.shape[-1]
     state_net_tiled = jnp.tile(x, [num_quantiles, 1])
     quantiles_shape = [num_quantiles, 1]
     quantiles = jax.random.uniform(rng, shape=quantiles_shape)
     quantile_net = jnp.tile(quantiles, [1, self.quantile_embedding_dim])
     quantile_net = (
         jnp.arange(1, self.quantile_embedding_dim + 1, 1).astype(jnp.float32)
         * onp.pi
-        * quantile_net)
+        * quantile_net
+    )
     quantile_net = jnp.cos(quantile_net)
-    quantile_net = nn.Dense(features=state_vector_length,
-                            kernel_init=initializer)(quantile_net)
+    quantile_net = nn.Dense(
+        features=state_vector_length, kernel_init=initializer
+    )(quantile_net)
     quantile_net = nn.relu(quantile_net)
     x = state_net_tiled * quantile_net
     x = nn.Dense(features=512, kernel_init=initializer)(x)
     x = nn.relu(x)
-    quantile_values = nn.Dense(features=self.num_actions,
-                               kernel_init=initializer)(x)
+    quantile_values = nn.Dense(
+        features=self.num_actions, kernel_init=initializer
+    )(x)
     return atari_lib.ImplicitQuantileNetworkType(quantile_values, quantiles)
 
 
 ### Quantile Networks ###
 @gin.configurable
 class QuantileNetwork(nn.Module):
   """Convolutional network used to compute the agent's return quantiles."""
+
   num_actions: int
   num_atoms: int
   inputs_preprocessed: bool = False
 
   @nn.compact
   def __call__(self, x):
     initializer = nn.initializers.variance_scaling(
-        scale=1.0 / jnp.sqrt(3.0),
-        mode='fan_in',
-        distribution='uniform')
+        scale=1.0 / jnp.sqrt(3.0), mode='fan_in', distribution='uniform'
+    )
     if not self.inputs_preprocessed:
       x = preprocess_atari_inputs(x)
-    x = nn.Conv(features=32, kernel_size=(8, 8), strides=(4, 4),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(4, 4), strides=(2, 2),
-                kernel_init=initializer)(x)
-    x = nn.relu(x)
-    x = nn.Conv(features=64, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=32, kernel_size=(8, 8), strides=(4, 4), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(4, 4), strides=(2, 2), kernel_init=initializer
+    )(x)
+    x = nn.relu(x)
+    x = nn.Conv(
+        features=64, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape((-1))  # flatten
     x = nn.Dense(features=512, kernel_init=initializer)(x)
     x = nn.relu(x)
-    x = nn.Dense(features=self.num_actions * self.num_atoms,
-                 kernel_init=initializer)(x)
+    x = nn.Dense(
+        features=self.num_actions * self.num_atoms, kernel_init=initializer
+    )(x)
     logits = x.reshape((self.num_actions, self.num_atoms))
     probabilities = nn.softmax(logits)
     q_values = jnp.mean(logits, axis=1)
     return atari_lib.RainbowNetworkType(q_values, logits, probabilities)
 
 
 ### Noisy Nets for FullRainbowNetwork ###
@@ -344,29 +468,29 @@
 class NoisyNetwork(nn.Module):
   """Noisy Network from Fortunato et al. (2018).
 
   Attributes:
     rng_key: jax.interpreters.xla.DeviceArray, key for JAX RNG.
     eval_mode: bool, whether to turn off noise during evaluation.
   """
-  rng_key: jax.interpreters.xla.DeviceArray
+
+  rng_key: jax.Array
   eval_mode: bool = False
 
   @staticmethod
   def sample_noise(key, shape):
     return jax.random.normal(key, shape)
 
   @staticmethod
   def f(x):
     # See (10) and (11) in Fortunato et al. (2018).
     return jnp.multiply(jnp.sign(x), jnp.power(jnp.abs(x), 0.5))
 
   @nn.compact
   def __call__(self, x, features, bias=True, kernel_init=None):
-
     def mu_init(key, shape):
       # Initialization of mean noise parameters (Section 3.2)
       low = -1 / jnp.power(x.shape[0], 0.5)
       high = 1 / jnp.power(x.shape[0], 0.5)
       return jax.random.uniform(key, minval=low, maxval=high, shape=shape)
 
     def sigma_init(key, shape, dtype=jnp.float32):  # pylint: disable=unused-argument
@@ -398,32 +522,36 @@
     b = b_mu + jnp.multiply(b_sigma, b_epsilon)
     return jnp.where(bias, ret + b, ret)
 
 
 ### FullRainbowNetwork ###
 def feature_layer(key, noisy, eval_mode=False):
   """Network feature layer depending on whether noisy_nets are used on or not."""
+
   def noisy_net(x, features):
     return NoisyNetwork(rng_key=key, eval_mode=eval_mode)(x, features)
+
   def dense_net(x, features):
     return nn.Dense(features, kernel_init=nn.initializers.xavier_uniform())(x)
+
   return noisy_net if noisy else dense_net
 
 
 @gin.configurable
 class FullRainbowNetwork(nn.Module):
   """Jax Rainbow network for Full Rainbow.
 
   Attributes:
     num_actions: int, number of actions the agent can take at any state.
     num_atoms: int, the number of buckets of the value function distribution.
     noisy: bool, Whether to use noisy networks.
     dueling: bool, Whether to use dueling network architecture.
     distributional: bool, whether to use distributional RL.
   """
+
   num_actions: int
   num_atoms: int
   noisy: bool = True
   dueling: bool = True
   distributional: bool = True
   inputs_preprocessed: bool = False
 
@@ -435,21 +563,23 @@
 
     if not self.inputs_preprocessed:
       x = preprocess_atari_inputs(x)
 
     hidden_sizes = [32, 64, 64]
     kernel_sizes = [8, 4, 3]
     stride_sizes = [4, 2, 1]
-    for hidden_size, kernel_size, stride_size in zip(hidden_sizes, kernel_sizes,
-                                                     stride_sizes):
+    for hidden_size, kernel_size, stride_size in zip(
+        hidden_sizes, kernel_sizes, stride_sizes
+    ):
       x = nn.Conv(
           features=hidden_size,
           kernel_size=(kernel_size, kernel_size),
           strides=(stride_size, stride_size),
-          kernel_init=nn.initializers.xavier_uniform())(x)
+          kernel_init=nn.initializers.xavier_uniform(),
+      )(x)
       x = nn.relu(x)
     x = x.reshape((-1))  # flatten
 
     net = feature_layer(key, self.noisy, eval_mode=eval_mode)
     x = net(x, features=512)  # Single hidden layer of size 512
     x = nn.relu(x)
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/atari_100k/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/atari_100k/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/atari_100k/eval_run_experiment.py` & `dopamine_rl-4.0.7/dopamine/labs/atari_100k/eval_run_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,17 @@
 import jax
 
 
 @gin.configurable
 class MaxEpisodeEvalRunner(run_experiment.Runner):
   """Runner for evaluating using a fixed number of episodes rather than steps."""
 
-  def __init__(self,
-               base_dir,
-               create_agent_fn,
-               num_eval_episodes=100,
-               max_noops=30):
+  def __init__(
+      self, base_dir, create_agent_fn, num_eval_episodes=100, max_noops=30
+  ):
     """Specify the number of evaluation episodes."""
     super().__init__(base_dir, create_agent_fn)
     self._num_eval_episodes = num_eval_episodes
     logging.info('Num evaluation episodes: %d', num_eval_episodes)
     self._evaluation_steps = None
     self._max_noops = max_noops
 
@@ -49,15 +47,16 @@
       initial_observation = self._run_no_ops()
     return self._agent.begin_episode(initial_observation)
 
   def _run_no_ops(self):
     """Executes `num_noops` no-ops in the environment."""
     self._agent._rng, rng = jax.random.split(self._agent._rng)  # pylint: disable=protected-access
     num_noops = jax.random.randint(
-        rng, shape=(), minval=0, maxval=self._max_noops)
+        rng, shape=(), minval=0, maxval=self._max_noops
+    )
     for _ in range(num_noops):
       # Assumes raw action 0 is always no-op
       self._environment.environment.ale.act(0)
     if self._environment.environment.ale.game_over():
       observation = self._environment.reset()
     else:
       observation = self._environment._pool_and_resize()  # pylint: disable=protected-access
@@ -77,31 +76,33 @@
 
     Returns:
       Tuple containing the number of steps taken in this phase (int), the sum of
         returns (float), and the number of episodes performed (int).
     """
     step_count = 0
     num_episodes = 0
-    sum_returns = 0.
+    sum_returns = 0.0
 
     while num_episodes < max_episodes:
       episode_length, episode_return = self._run_one_episode()
       statistics.append({
           '{}_episode_lengths'.format(run_mode_str): episode_length,
-          '{}_episode_returns'.format(run_mode_str): episode_return
+          '{}_episode_returns'.format(run_mode_str): episode_return,
       })
       step_count += episode_length
       sum_returns += episode_return
       num_episodes += 1
       # We use sys.stdout.write instead of logging so as to flush frequently
       # without generating a line break.
-      sys.stdout.write('Steps executed: {} '.format(step_count) +
-                       'Episode length: {} '.format(episode_length) +
-                       'Num episodes: {} '.format(num_episodes) +
-                       'Return: {}\r'.format(episode_return))
+      sys.stdout.write(
+          'Steps executed: {} '.format(step_count)
+          + 'Episode length: {} '.format(episode_length)
+          + 'Num episodes: {} '.format(num_episodes)
+          + 'Return: {}\r'.format(episode_return)
+      )
       sys.stdout.flush()
     return step_count, sum_returns, num_episodes
 
   def _run_eval_phase(self, statistics):
     """Run evaluation phase.
 
     Args:
@@ -111,13 +112,16 @@
     Returns:
       num_episodes: int, The number of episodes run in this phase.
       average_reward: float, The average reward generated in this phase.
     """
     # Perform the evaluation phase -- no learning.
     self._agent.eval_mode = True
     _, sum_returns, num_episodes = self._run_one_phase_fix_episodes(
-        self._num_eval_episodes, statistics, 'eval')
+        self._num_eval_episodes, statistics, 'eval'
+    )
     average_return = sum_returns / num_episodes if num_episodes > 0 else 0.0
-    logging.info('Average undiscounted return per evaluation episode: %.2f',
-                 average_return)
+    logging.info(
+        'Average undiscounted return per evaluation episode: %.2f',
+        average_return,
+    )
     statistics.append({'eval_average_return': average_return})
     return num_episodes, average_return
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/atari_100k/train.py` & `dopamine_rl-4.0.7/dopamine/labs/atari_100k/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,38 +22,67 @@
 
 from absl import app
 from absl import flags
 from absl import logging
 from dopamine.discrete_domains import run_experiment
 from dopamine.discrete_domains import train as base_train
 from dopamine.labs.atari_100k import atari_100k_rainbow_agent
+from dopamine.labs.atari_100k import atari_100k_runner
 from dopamine.labs.atari_100k import eval_run_experiment
+from dopamine.labs.atari_100k import spr_agent
 import numpy as np
 import tensorflow as tf
 
+.learning.deepmind.xmanager2.client.google as xm  # pylint: disable=unused-import
+
+
 
 FLAGS = flags.FLAGS
-AGENTS = ['DER', 'DrQ', 'OTRainbow', 'DrQ_eps']
+AGENTS = ['DER', 'DrQ', 'OTRainbow', 'DrQ_eps', 'SPR']
 
 # flags are defined when importing run_xm_preprocessing
 flags.DEFINE_enum('agent', 'DER', AGENTS, 'Name of the agent.')
 flags.DEFINE_integer('run_number', 1, 'Run number.')
-flags.DEFINE_boolean('max_episode_eval', True,
-                     'Whether to use `MaxEpisodeEvalRunner` or not.')
+flags.DEFINE_boolean(
+    'max_episode_eval', True, 'Whether to use `MaxEpisodeEvalRunner` or not.'
+)
+flags.DEFINE_boolean(
+    'legacy_runner',
+    False,
+    (
+        'Whether to use the legacy MaxEpisodeEvalRunner.'
+        ' This runner does not run parallel evaluation environments and may be'
+        ' easier to understand, but will be noticeably slower. It also does not'
+        ' guarantee that a precise number of training steps will be collected,'
+        ' which clashes with the technical definition of Atari 100k.'
+    ),
+)
+
+
+def create_agent(
+    sess,  # pylint: disable=unused-argument
+    environment,
+    seed,
+    agent_name: str,
+    summary_writer=None,
+):
+  """Helper function for creating full rainbow-based Atari 100k agent."""
 
+  if agent_name == 'SPR':
+    return spr_agent.SPRAgent(
+        num_actions=environment.action_space.n,
+        seed=seed,
+        summary_writer=summary_writer,
+    )
 
-def create_agent(sess,  # pylint: disable=unused-argument
-                 environment,
-                 seed,
-                 summary_writer=None):
-  """Helper function for creating full rainbow-based Atari 100k agent."""
   return atari_100k_rainbow_agent.Atari100kRainbowAgent(
       num_actions=environment.action_space.n,
       seed=seed,
-      summary_writer=summary_writer)
+      summary_writer=summary_writer,
+  )
 
 
 def set_random_seed(seed):
   """Set random seed for reproducibility."""
   logging.info('Setting random seed: %d', seed)
   os.environ['PYTHONHASHSEED'] = str(seed)
   tf.random.set_seed(seed)
@@ -69,20 +98,24 @@
   logging.set_verbosity(logging.INFO)
   tf.compat.v1.enable_v2_behavior()
 
   base_dir = FLAGS.base_dir
   gin_files, gin_bindings = FLAGS.gin_files, FLAGS.gin_bindings
   run_experiment.load_gin_configs(gin_files, gin_bindings)
   # Set the Jax agent seed using the run number
-  create_agent_fn = functools.partial(create_agent, seed=FLAGS.run_number)
-  if FLAGS.max_episode_eval:
+  create_agent_fn = functools.partial(
+      create_agent, seed=FLAGS.run_number, agent_name=FLAGS.agent
+  )
+  if FLAGS.legacy_runner:
     runner_fn = eval_run_experiment.MaxEpisodeEvalRunner
     logging.info('Using MaxEpisodeEvalRunner for evaluation.')
     runner = runner_fn(base_dir, create_agent_fn)
   else:
-    runner = run_experiment.Runner(base_dir, create_agent_fn)
+    runner = atari_100k_runner.DataEfficientAtariRunner(
+        base_dir, create_agent_fn
+    )
   runner.run_experiment()
 
 
 if __name__ == '__main__':
   flags.mark_flag_as_required('base_dir')
   app.run(main)
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/environments/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/environments/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/environments/brax/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/environments/brax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/environments/brax/brax_lib.py` & `dopamine_rl-4.0.7/dopamine/labs/environments/brax/brax_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     seed = int(time.time() * 1e6) if seed is None else seed
     self._rng = jax.random.PRNGKey(seed)
     self._rng, rng = jax.random.split(self._rng)
     self._state = self.env.reset(rng=rng)
 
   @property
   def observation_space(self) -> onp.ndarray:
-    return self._state.obs.shape
+    return self._state.obs.shape  # pytype: disable=bad-return-type  # jax-ndarray
 
   @property
   def action_space(self) -> int:
     return self.env.action_size
 
   @property
   def reward_range(self):
@@ -54,57 +54,62 @@
   def metadata(self):
     pass  # Unused
 
   def reset(self) -> onp.ndarray:
     self.game_over = False
     self._rng, rng = jax.random.split(self._rng)
     self._state = self.env.reset(rng=rng)
-    return self._state.obs
+    return self._state.obs  # pytype: disable=bad-return-type  # jax-ndarray
 
-  def step(self, action) -> Tuple[onp.ndarray, onp.ndarray, bool,
-                                  Mapping[Any, Any]]:
+  def step(
+      self, action
+  ) -> Tuple[onp.ndarray, onp.ndarray, bool, Mapping[Any, Any]]:
     self._state = jax.jit(self.env.step)(self._state, action)
     self.game_over = self._state.done
-    return (onp.array(self._state.obs),
-            onp.array(self._state.reward),
-            self._state.done,
-            self._state.info)
+    return (
+        onp.array(self._state.obs),
+        onp.array(self._state.reward),
+        self._state.done,
+        self._state.info,
+    )
 
 
 @gin.configurable
 def create_brax_environment(env_name, seed=None) -> BraxEnv:
   """Helper function for creating a Brax environment."""
   return BraxEnv(env_name, seed=seed)
 
 
 @gin.configurable
 def create_brax_agent(
     environment: BraxEnv,
     agent_name: str = 'sac_brax',
-    summary_writer: Optional[tensorboard.SummaryWriter] = None
+    summary_writer: Optional[tensorboard.SummaryWriter] = None,
 ) -> dqn_agent.JaxDQNAgent:
   """Creates an agent for Brax."""
   assert agent_name is not None
   if agent_name == 'sac_brax':
     return sac_agent.SACAgent(
         action_shape=(environment.action_space,),
-        action_limits=(-1 * onp.ones(environment.action_space),
-                       onp.ones(environment.action_space)),
+        action_limits=(
+            -1 * onp.ones(environment.action_space),
+            onp.ones(environment.action_space),
+        ),
         observation_shape=environment.observation_space,
         action_dtype=onp.float32,
         observation_dtype=onp.float64,
-        summary_writer=summary_writer)
+        summary_writer=summary_writer,
+    )
   else:
     raise ValueError(f'Unknown agent: {agent_name}')
 
 
 @gin.configurable
 def create_brax_runner(
-    base_dir: str,
-    schedule: str = 'continuous_train_and_eval'
+    base_dir: str, schedule: str = 'continuous_train_and_eval'
 ) -> run_experiment.ContinuousRunner:
   """Creates a Brax experiment Runner."""
   assert base_dir is not None
   # Continuously runs training and evaluation until max num_iterations is hit.
   if schedule == 'continuous_train_and_eval':
     return run_experiment.ContinuousRunner(base_dir, create_brax_agent)
   # Continuously runs training until max num_iterations is hit.
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/environments/brax/train.py` & `dopamine_rl-4.0.7/dopamine/labs/environments/brax/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,28 @@
 from absl import app
 from absl import flags
 from absl import logging
 
 from dopamine.continuous_domains import run_experiment
 from dopamine.labs.environments.brax import brax_lib
 
-flags.DEFINE_string('base_dir', None,
-                    'Base directory to host all required sub-directories.')
+flags.DEFINE_string(
+    'base_dir', None, 'Base directory to host all required sub-directories.'
+)
 flags.DEFINE_multi_string(
-    'gin_files', [], 'List of paths to gin configuration files (e.g.'
-    '"dopamine/labs/environments/brax/sac_brax.gin").')
+    'gin_files',
+    [],
+    'List of paths to gin configuration files (e.g.'
+    '"dopamine/labs/environments/brax/sac_brax.gin").',
+)
 flags.DEFINE_multi_string(
-    'gin_bindings', [],
-    'Gin bindings to override the values set in the config files.')
+    'gin_bindings',
+    [],
+    'Gin bindings to override the values set in the config files.',
+)
 
 FLAGS = flags.FLAGS
 
 
 def main(unused_argv):
   """Main method.
 
@@ -48,8 +54,7 @@
   runner = brax_lib.create_brax_runner(base_dir)
   runner.run_experiment()
 
 
 if __name__ == '__main__':
   flags.mark_flag_as_required('base_dir')
   app.run(main)
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/environments/minatar/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/environments/minatar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/environments/minatar/minatar_env.py` & `dopamine_rl-4.0.7/dopamine/labs/environments/minatar/minatar_env.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,85 +87,92 @@
       if jax.random.uniform(rng) < self.action_repeat_probability:
         action_to_use = self._prev_action
     self._prev_action = action
     return super().step(action_to_use)
 
 
 @gin.configurable
-def create_minatar_env(game_name,
-                       sticky_actions=False,
-                       action_repeat_probability=0.25,
-                       seed=None):
+def create_minatar_env(
+    game_name, sticky_actions=False, action_repeat_probability=0.25, seed=None
+):
   """Helper function for creating Minatar environment."""
   if sticky_actions:
     return StickyMinAtarEnv(
         game_name,
         action_repeat_probability=action_repeat_probability,
-        seed=seed)
+        seed=seed,
+    )
   return MinAtarEnv(game_name)
 
 
 @gin.configurable
 class MinatarDQNNetwork(nn.Module):
   """JAX DQN Network for Minatar environments."""
+
   num_actions: int
   inputs_preprocessed: bool = True
 
   @nn.compact
   def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
     initializer = nn.initializers.xavier_uniform()
     x = x.astype(jnp.float32)
-    x = nn.Conv(features=16, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=16, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape(-1)  # flatten
     q_values = nn.Dense(features=self.num_actions, kernel_init=initializer)(x)
     return atari_lib.DQNNetworkType(q_values)
 
 
 @gin.configurable
 class MinatarRainbowNetwork(nn.Module):
   """Jax Rainbow network for Minatar."""
+
   num_actions: int
   num_atoms: int
   inputs_preprocessed: bool = True
 
   @nn.compact
   def __call__(self, x: jnp.ndarray, support: jnp.ndarray) -> jnp.ndarray:
     initializer = nn.initializers.xavier_uniform()
     x = x.astype(jnp.float32)
-    x = nn.Conv(features=16, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=16, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape(-1)  # flatten
-    x = nn.Dense(features=self.num_actions * self.num_atoms,
-                 kernel_init=initializer)(x)
+    x = nn.Dense(
+        features=self.num_actions * self.num_atoms, kernel_init=initializer
+    )(x)
     logits = x.reshape((self.num_actions, self.num_atoms))
     probabilities = nn.softmax(logits)
     q_values = jnp.sum(support * probabilities, axis=1)
     return atari_lib.RainbowNetworkType(q_values, logits, probabilities)
 
 
 @gin.configurable
 class MinatarQuantileNetwork(nn.Module):
   """Convolutional network used to compute the agent's return quantiles."""
+
   num_actions: int
   num_atoms: int
   inputs_preprocessed: bool = True
 
   @nn.compact
   def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
     initializer = jax.nn.initializers.variance_scaling(
-        scale=1.0 / jnp.sqrt(3.0),
-        mode='fan_in',
-        distribution='uniform')
+        scale=1.0 / jnp.sqrt(3.0), mode='fan_in', distribution='uniform'
+    )
     x = x.astype(jnp.float32)
-    x = nn.Conv(features=16, kernel_size=(3, 3), strides=(1, 1),
-                kernel_init=initializer)(x)
+    x = nn.Conv(
+        features=16, kernel_size=(3, 3), strides=(1, 1), kernel_init=initializer
+    )(x)
     x = nn.relu(x)
     x = x.reshape(-1)  # flatten
-    x = nn.Dense(features=self.num_actions * self.num_atoms,
-                 kernel_init=initializer)(x)
+    x = nn.Dense(
+        features=self.num_actions * self.num_atoms, kernel_init=initializer
+    )(x)
     logits = x.reshape((self.num_actions, self.num_atoms))
     probabilities = nn.softmax(logits)
     q_values = jnp.mean(logits, axis=1)
     return atari_lib.RainbowNetworkType(q_values, logits, probabilities)
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/continuous_networks.py` & `dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/continuous_networks.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import jax
 from jax import numpy as jnp
 
 
 @dataclasses.dataclass
 class SACEncoderOutputs:
   """The output of a SACEncoder."""
+
   critic_z: jnp.ndarray
   actor_z: jnp.ndarray
 
 
 class SACEncoderNetwork(nn.Module):
   """An encoder network for soft actor critic.
 
@@ -49,76 +50,71 @@
 
     # Flatten the last dimension (normally to deal with stacked rgb frames)
     if len(x.shape) > 3:
       x = x.reshape((*x.shape[:2], -1))
 
     kernel_init = nn.initializers.orthogonal()
     x = nn.Conv(
-        features=32,
-        kernel_size=(3, 3),
-        strides=(2, 2),
-        kernel_init=kernel_init)(x)
+        features=32, kernel_size=(3, 3), strides=(2, 2), kernel_init=kernel_init
+    )(x)
     x = nn.relu(x)
     x = nn.Conv(
-        features=32,
-        kernel_size=(3, 3),
-        strides=(1, 1),
-        kernel_init=kernel_init)(x)
+        features=32, kernel_size=(3, 3), strides=(1, 1), kernel_init=kernel_init
+    )(x)
     x = nn.relu(x)
     x = nn.Conv(
-        features=32,
-        kernel_size=(3, 3),
-        strides=(1, 1),
-        kernel_init=kernel_init)(x)
+        features=32, kernel_size=(3, 3), strides=(1, 1), kernel_init=kernel_init
+    )(x)
     x = nn.relu(x)
     x = nn.Conv(
-        features=32,
-        kernel_size=(3, 3),
-        strides=(1, 1),
-        kernel_init=kernel_init)(x)
+        features=32, kernel_size=(3, 3), strides=(1, 1), kernel_init=kernel_init
+    )(x)
     x = nn.relu(x)
     x = jnp.reshape(x, -1)  # Flatten
 
     critic_z = nn.Dense(features=50, kernel_init=kernel_init)(x)
     critic_z = nn.LayerNorm()(critic_z)
     critic_z = nn.tanh(critic_z)
 
     # Only the critic should train the convolution layers, so stop the
     # gradients from the actor.
-    actor_z = nn.Dense(
-        features=50, kernel_init=kernel_init)(
-            jax.lax.stop_gradient(x))
+    actor_z = nn.Dense(features=50, kernel_init=kernel_init)(
+        jax.lax.stop_gradient(x)
+    )
     actor_z = nn.LayerNorm()(actor_z)
     actor_z = nn.tanh(actor_z)
 
     return SACEncoderOutputs(critic_z, actor_z)
 
 
 @gin.configurable
 class SACConvNetwork(nn.Module):
   """A convolutional value and policy networks for SAC.
 
   This uses the SAC-AE network for processing images. For more information,
   view SACEncoderNetwork.
   """
+
   action_shape: Tuple[int, ...]
   num_layers: int = 2
   hidden_units: int = 256
   action_limits: Optional[Tuple[Tuple[float, ...], Tuple[float, ...]]] = None
 
   def setup(self):
     self._encoder = SACEncoderNetwork()
     self._sac_network = continuous_networks.SACNetwork(
-        self.action_shape, self.num_layers,
-        self.hidden_units, self.action_limits)
-
-  def __call__(self,
-               state: jnp.ndarray,
-               key: jnp.ndarray,
-               mean_action: bool = True) -> continuous_networks.SacOutput:
+        self.action_shape,
+        self.num_layers,
+        self.hidden_units,
+        self.action_limits,
+    )
+
+  def __call__(
+      self, state: jnp.ndarray, key: jnp.ndarray, mean_action: bool = True
+  ) -> continuous_networks.SacOutput:
     """Calls the SAC actor/critic networks.
 
     This has two important purposes:
       1. It is used to initialize all parameters of both networks.
       2. It is used to efficiently calculate the outputs of both the actor
         and critic networks on a single input.
 
@@ -131,21 +127,24 @@
 
     Returns:
       A named tuple containing the outputs from both networks.
     """
     encoding = self._encoder(state)
 
     actor_output = self._sac_network.actor(encoding.actor_z, key)
-    action = actor_output.mean_action if mean_action else actor_output.sampled_action
+    action = (
+        actor_output.mean_action if mean_action else actor_output.sampled_action
+    )
     critic_output = self._sac_network.critic(encoding.critic_z, action)
 
     return continuous_networks.SacOutput(actor_output, critic_output)
 
-  def actor(self, state: jnp.ndarray,
-            key: jnp.ndarray) -> continuous_networks.SacActorOutput:
+  def actor(
+      self, state: jnp.ndarray, key: jnp.ndarray
+  ) -> continuous_networks.SacActorOutput:
     """Calls the SAC actor network.
 
     This can be called using network_def.apply(..., method=network_def.actor).
 
     Args:
       state: An input state.
       key: A PRNGKey to use to sample an action from the actor's output
@@ -154,16 +153,17 @@
     Returns:
       A named tuple containing a sampled action, the mean action, and the
         likelihood of the sampled action.
     """
     encoding = self._encoder(state)
     return self._sac_network.actor(encoding.actor_z, key)
 
-  def critic(self, state: jnp.ndarray,
-             action: jnp.ndarray) -> continuous_networks.SacCriticOutput:
+  def critic(
+      self, state: jnp.ndarray, action: jnp.ndarray
+  ) -> continuous_networks.SacCriticOutput:
     """Calls the SAC critic network.
 
     SAC uses two Q networks to reduce overestimation bias.
     This can be called using network_def.apply(..., method=network_def.critic).
 
     Args:
       state: An input state.
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/sac_from_pixels/deepmind_control_lib.py` & `dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/deepmind_control_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,28 +32,30 @@
 import numpy as np
 
 
 @gin.configurable
 def create_deepmind_control_environment(
     domain_name: str = gin.REQUIRED,
     task_name: str = gin.REQUIRED,
-    use_image_observations: bool = gin.REQUIRED) -> gym.Env:
+    use_image_observations: bool = gin.REQUIRED,
+) -> gym.Env:
   """Wraps a Deepmind Control Suite environment with some basic preprocessing.
 
   Args:
     domain_name: The name of the environment to run.
     task_name: The name of the task to run.
     use_image_observations: If True, the created environment will return image
       observations. Else, it will return the state vector.
 
   Returns:
     A Gym environment with some standard preprocessing.
   """
   env = suite.load(
-      domain_name, task_name, environment_kwargs={'flat_observation': True})
+      domain_name, task_name, environment_kwargs={'flat_observation': True}
+  )
 
   # Wrap the returned environment in a class which conforms to the API expected
   # by Dopamine.
   if use_image_observations:
     env = DeepmindControlWithImagesPreprocessing(env)
   else:
     env = DeepmindControlPreprocessing(env)
@@ -106,15 +108,16 @@
     return spaces.Box(low=low, high=high, dtype=np.float32)
 
   @property
   def action_space(self) -> spaces.Box:
     """The action space for the processed environment."""
     action_spec = self.environment.action_spec()
     return spaces.Box(
-        low=action_spec.minimum, high=action_spec.maximum, dtype=np.float32)
+        low=action_spec.minimum, high=action_spec.maximum, dtype=np.float32
+    )
 
   @property
   def reward_range(self) -> Tuple[float, float]:
     """The reward range for the processed environment."""
     return (-float('inf'), float('inf'))
 
   @property
@@ -128,16 +131,16 @@
     Returns:
       An initial observation.
     """
     timestep = self.environment.reset()
     return self._get_observation(timestep)
 
   def step(
-      self,
-      action: np.ndarray) -> Tuple[np.ndarray, float, bool, Mapping[Any, Any]]:
+      self, action: np.ndarray
+  ) -> Tuple[np.ndarray, float, bool, Mapping[Any, Any]]:
     """Steps the environment.
 
     Args:
       action: The action to apply.
 
     Returns:
       An (observation, reward, is_terminal, info) tuple. For more information,
@@ -160,38 +163,49 @@
 
     observation = self._get_observation(timestep)
 
     return observation, accumulated_reward, done, {}
 
   def _get_observation(self, timestep: dm_env.TimeStep) -> np.ndarray:
     return np.concatenate(
-        [timestep.observation[k] for k in timestep.observation])
+        [timestep.observation[k] for k in timestep.observation]
+    )
 
 
 class DeepmindControlWithImagesPreprocessing(DeepmindControlPreprocessing):
   """A DM Control Suite preprocessing wrapper for image observations."""
 
-  def __init__(self,
-               env: control.Environment,
-               observation_shape: Tuple[int, int] = (84, 84)):
+  def __init__(
+      self,
+      env: control.Environment,
+      observation_shape: Tuple[int, int] = (84, 84),
+  ):
     """Constructor for preprocessing wrapper.
 
     Args:
       env: The environment to wrap.
-      observation_shape: The size to reshape the images to. This corresponds
-        to (height, width). The output shape will be (height, width, 3), with
-        3 corresponding to RGB channels.
+      observation_shape: The size to reshape the images to. This corresponds to
+        (height, width). The output shape will be (height, width, 3), with 3
+        corresponding to RGB channels.
     """
     super(DeepmindControlWithImagesPreprocessing, self).__init__(env)
 
     self._shape = observation_shape
 
   @property
   def observation_space(self) -> spaces.Box:
-    return spaces.Box(low=0, high=255, shape=(*self._shape, 3,), dtype=np.uint8)
+    return spaces.Box(
+        low=0,
+        high=255,
+        shape=(
+            *self._shape,
+            3,
+        ),
+        dtype=np.uint8,
+    )
 
   def _get_observation(self, timestep: dm_env.TimeStep) -> np.ndarray:
     return self._render_image()
 
   def _render_image(self) -> np.ndarray:
     """Renders the environment and processes the image.
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/__init__.py` & `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/run_experiment.py` & `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/run_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,57 +25,57 @@
 from dopamine.labs.tandem_dqn import tandem_dqn_agent
 import gin
 import numpy as np
 import tensorflow as tf
 
 
 @gin.configurable
-def create_tandem_agents_and_checkpoints(sess, environment, agent_name='dqn',
-                                         summary_writer=None, debug_mode=False):
+def create_tandem_agents_and_checkpoints(
+    sess, environment, agent_name='dqn', summary_writer=None, debug_mode=False
+):
   """Creates a tandem agent.
 
   Args:
     sess: TF session, unused since we are in JAX.
     environment: A gym environment (e.g. Atari 2600).
     agent_name: str, name of the agent to create.
-    summary_writer: A Tensorflow summary writer to pass to the agent
-      for in-agent training statistics in Tensorboard.
+    summary_writer: A Tensorflow summary writer to pass to the agent for
+      in-agent training statistics in Tensorboard.
     debug_mode: bool, unused.
 
   Returns:
     An active and passive agent.
   """
   assert agent_name is not None
   del sess
   del debug_mode
   if agent_name == 'dqn':
     return tandem_dqn_agent.TandemDQNAgent(
-        num_actions=environment.action_space.n, summary_writer=summary_writer)
+        num_actions=environment.action_space.n, summary_writer=summary_writer
+    )
   else:
     raise ValueError('Unknown agent: {}'.format(agent_name))
 
 
 @gin.configurable
 class TandemRunner(run_experiment.Runner):
   """Runner class to run Tandem RL experiments."""
 
-  def __init__(self,
-               base_dir,
-               create_agent_fn,
-               suite='atari'):
+  def __init__(self, base_dir, create_agent_fn, suite='atari'):
     if suite == 'atari':
       create_environment_fn = atari_lib.create_atari_environment
     elif suite == 'classic':
       create_environment_fn = gym_lib.create_gym_environment
     elif suite == 'minatar':
       create_environment_fn = minatar_env.create_minatar_env
     else:
       raise ValueError(f'Unknown suite: {suite}')
-    super().__init__(base_dir, create_agent_fn,
-                     create_environment_fn=create_environment_fn)
+    super().__init__(
+        base_dir, create_agent_fn, create_environment_fn=create_environment_fn
+    )
 
   def _initialize_episode(self, agent_type='active'):
     """Initialization for a new episode.
 
     Args:
       agent_type: str, the type of agent to run.
 
@@ -91,31 +91,33 @@
     Args:
       agent_type: str, the type of agent to run.
 
     Returns:
       The number of steps taken and the total reward.
     """
     step_number = 0
-    total_reward = 0.
+    total_reward = 0.0
 
     action = self._initialize_episode(agent_type)
     is_terminal = False
 
     # Keep interacting until we reach a terminal state.
     while True:
       observation, reward, is_terminal = self._run_one_step(action)
 
       total_reward += reward
       step_number += 1
 
       # Perform reward clipping.
       reward = np.clip(reward, -1, 1)
 
-      if (self._environment.game_over or
-          step_number == self._max_steps_per_episode):
+      if (
+          self._environment.game_over
+          or step_number == self._max_steps_per_episode
+      ):
         # Stop the run loop once we reach the true end of episode.
         break
       elif is_terminal:
         # If we lose a life but the episode is not over, signal an artificial
         # end of episode to the agent.
         if agent_type == 'active':
           self._agent.end_episode(reward)
@@ -123,16 +125,17 @@
       else:
         action = self._agent.step(agent_type, reward, observation)
 
     self._end_episode(reward)
 
     return step_number, total_reward
 
-  def _run_one_phase(self, min_steps, statistics, run_mode_str,
-                     agent_type='active'):
+  def _run_one_phase(
+      self, min_steps, statistics, run_mode_str, agent_type='active'
+  ):
     """Runs the agent/environment loop until a desired number of steps.
 
     We follow the Machado et al., 2017 convention of running full episodes,
     and terminating once we've run a minimum number of steps.
 
     Args:
       min_steps: int, minimum number of steps to generate in this phase.
@@ -143,32 +146,36 @@
 
     Returns:
       Tuple containing the number of steps taken in this phase (int), the sum of
         returns (float), and the number of episodes performed (int).
     """
     step_count = 0
     num_episodes = 0
-    sum_returns = 0.
+    sum_returns = 0.0
 
     while step_count < min_steps:
       episode_length, episode_return = self._run_one_episode(agent_type)
       statistics.append({
-          '{}_{}_episode_lengths'.format(run_mode_str,
-                                         agent_type): episode_length,
-          '{}_{}_episode_returns'.format(run_mode_str,
-                                         agent_type): episode_return
+          '{}_{}_episode_lengths'.format(
+              run_mode_str, agent_type
+          ): episode_length,
+          '{}_{}_episode_returns'.format(
+              run_mode_str, agent_type
+          ): episode_return,
       })
       step_count += episode_length
       sum_returns += episode_return
       num_episodes += 1
       # We use sys.stdout.write instead of logging so as to flush frequently
       # without generating a line break.
-      sys.stdout.write('Steps executed: {} '.format(step_count) +
-                       'Episode length: {} '.format(episode_length) +
-                       'Return: {}\r'.format(episode_return))
+      sys.stdout.write(
+          'Steps executed: {} '.format(step_count)
+          + 'Episode length: {} '.format(episode_length)
+          + 'Return: {}\r'.format(episode_return)
+      )
       sys.stdout.flush()
     return step_count, sum_returns, num_episodes
 
   def _run_eval_phase(self, statistics, agent_type='active'):
     """Run evaluation phase on both passive and active learners.
 
     Args:
@@ -179,18 +186,22 @@
     Returns:
       num_episodes: int, The number of episodes run in this phase.
       average_reward: float, The average reward generated in this phase.
     """
     # Perform the evaluation phase -- no learning.
     self._agent.eval_mode = True
     _, sum_returns, num_episodes = self._run_one_phase(
-        self._evaluation_steps, statistics, 'eval', agent_type)
+        self._evaluation_steps, statistics, 'eval', agent_type
+    )
     average_return = sum_returns / num_episodes if num_episodes > 0 else 0.0
-    logging.info('Average undiscounted return per eval episode (%s): %.2f',
-                 agent_type, average_return)
+    logging.info(
+        'Average undiscounted return per eval episode (%s): %.2f',
+        agent_type,
+        average_return,
+    )
     statistics.append({f'{agent_type}_eval_average_return': average_return})
     return num_episodes, average_return
 
   def _run_one_iteration(self, iteration):
     """Runs one iteration of agent/environment interaction.
 
     An iteration involves running several episodes until a certain number of
@@ -203,65 +214,83 @@
 
     Returns:
       A dict containing summary statistics for this iteration.
     """
     statistics = iteration_statistics.IterationStatistics()
     logging.info('Starting iteration %d', iteration)
     num_episodes_train, average_reward_train, average_steps_per_second = (
-        self._run_train_phase(statistics))
+        self._run_train_phase(statistics)
+    )
     active_num_episodes_eval, active_average_reward_eval = self._run_eval_phase(
-        statistics, 'active')
+        statistics, 'active'
+    )
     passive_num_episodes_eval, passive_average_reward_eval = (
-        self._run_eval_phase(statistics, 'passive'))
+        self._run_eval_phase(statistics, 'passive')
+    )
 
-    self._save_tensorboard_summaries(iteration, num_episodes_train,
-                                     average_reward_train,
-                                     active_num_episodes_eval,
-                                     active_average_reward_eval,
-                                     passive_num_episodes_eval,
-                                     passive_average_reward_eval,
-                                     average_steps_per_second)
+    self._save_tensorboard_summaries(
+        iteration,
+        num_episodes_train,
+        average_reward_train,
+        active_num_episodes_eval,
+        active_average_reward_eval,
+        passive_num_episodes_eval,
+        passive_average_reward_eval,
+        average_steps_per_second,
+    )
     return statistics.data_lists
 
-  def _save_tensorboard_summaries(self, iteration,
-                                  num_episodes_train,
-                                  average_reward_train,
-                                  active_num_episodes_eval,
-                                  active_average_reward_eval,
-                                  passive_num_episodes_eval,
-                                  passive_average_reward_eval,
-                                  average_steps_per_second):
+  def _save_tensorboard_summaries(
+      self,
+      iteration,
+      num_episodes_train,
+      average_reward_train,
+      active_num_episodes_eval,
+      active_average_reward_eval,
+      passive_num_episodes_eval,
+      passive_average_reward_eval,
+      average_steps_per_second,
+  ):
     """Save statistics as tensorboard summaries.
 
     Args:
       iteration: int, The current iteration number.
       num_episodes_train: int, number of training episodes run.
       average_reward_train: float, The average training reward.
       active_num_episodes_eval: int, number of active evaluation episodes run.
       active_average_reward_eval: float, The average active evaluation reward.
       passive_num_episodes_eval: int, number of passive evaluation episodes run.
       passive_average_reward_eval: float, The average passive evaluation reward.
       average_steps_per_second: float, The average number of steps per second.
     """
-    summary = tf.compat.v1.Summary(value=[
-        tf.compat.v1.Summary.Value(
-            tag='Train/NumEpisodes', simple_value=num_episodes_train),
-        tf.compat.v1.Summary.Value(
-            tag='Train/AverageReturns', simple_value=average_reward_train),
-        tf.compat.v1.Summary.Value(
-            tag='Train/AverageStepsPerSecond',
-            simple_value=average_steps_per_second),
-        tf.compat.v1.Summary.Value(
-            tag='Eval/ActiveNumEpisodes',
-            simple_value=active_num_episodes_eval),
-        tf.compat.v1.Summary.Value(
-            tag='Eval/ActiveAverageReturns',
-            simple_value=active_average_reward_eval),
-        tf.compat.v1.Summary.Value(
-            tag='Eval/PassiveNumEpisodes',
-            simple_value=passive_num_episodes_eval),
-        tf.compat.v1.Summary.Value(
-            tag='Eval/PassiveAverageReturns',
-            simple_value=passive_average_reward_eval)
-    ])
+    summary = tf.compat.v1.Summary(
+        value=[
+            tf.compat.v1.Summary.Value(
+                tag='Train/NumEpisodes', simple_value=num_episodes_train
+            ),
+            tf.compat.v1.Summary.Value(
+                tag='Train/AverageReturns', simple_value=average_reward_train
+            ),
+            tf.compat.v1.Summary.Value(
+                tag='Train/AverageStepsPerSecond',
+                simple_value=average_steps_per_second,
+            ),
+            tf.compat.v1.Summary.Value(
+                tag='Eval/ActiveNumEpisodes',
+                simple_value=active_num_episodes_eval,
+            ),
+            tf.compat.v1.Summary.Value(
+                tag='Eval/ActiveAverageReturns',
+                simple_value=active_average_reward_eval,
+            ),
+            tf.compat.v1.Summary.Value(
+                tag='Eval/PassiveNumEpisodes',
+                simple_value=passive_num_episodes_eval,
+            ),
+            tf.compat.v1.Summary.Value(
+                tag='Eval/PassiveAverageReturns',
+                simple_value=passive_average_reward_eval,
+            ),
+        ]
+    )
     self._summary_writer.add_summary(summary, iteration)
     self._summary_writer.flush()
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/tandem_dqn_agent.py` & `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/tandem_dqn_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,31 @@
 import jax.numpy as jnp
 import numpy as onp
 import optax
 import tensorflow as tf
 
 
 @functools.partial(jax.jit, static_argnums=(0, 3, 10, 11, 12))
-def train(network_def, online_params, target_params, optimizer, optimizer_state,
-          states, actions, next_states, rewards, terminals, cumulative_gamma,
-          loss_type='huber', double_dqn=True):
+def train(
+    network_def,
+    online_params,
+    target_params,
+    optimizer,
+    optimizer_state,
+    states,
+    actions,
+    next_states,
+    rewards,
+    terminals,
+    cumulative_gamma,
+    loss_type='huber',
+    double_dqn=True,
+):
   """Run the training step."""
+
   def loss_fn(params, target):
     def q_online(state):
       return network_def.apply(params, state)
 
     q_values = jax.vmap(q_online)(states).q_values
     q_values = jnp.squeeze(q_values)
     replay_chosen_q = jax.vmap(lambda x, y: x[y])(q_values, actions)
@@ -47,89 +60,104 @@
 
   def q_online(state):
     return network_def.apply(online_params, state)
 
   def q_target(state):
     return network_def.apply(target_params, state)
 
-  target = target_q(q_online,
-                    q_target,
-                    next_states,
-                    rewards,
-                    terminals,
-                    cumulative_gamma,
-                    double_dqn)
+  target = target_q(
+      q_online,
+      q_target,
+      next_states,
+      rewards,
+      terminals,
+      cumulative_gamma,
+      double_dqn,
+  )
   grad_fn = jax.value_and_grad(loss_fn)
   loss, grad = grad_fn(online_params, target)
   updates, optimizer_state = optimizer.update(grad, optimizer_state)
   online_params = optax.apply_updates(online_params, updates)
   return optimizer_state, online_params, loss
 
 
-def target_q(online_network, target_network, next_states, rewards, terminals,
-             cumulative_gamma, double_dqn):
+def target_q(
+    online_network,
+    target_network,
+    next_states,
+    rewards,
+    terminals,
+    cumulative_gamma,
+    double_dqn,
+):
   """Compute the target Q-value."""
   if double_dqn:
-    next_state_q_vals_for_argmax = jax.vmap(
-        online_network, in_axes=(0))(next_states).q_values
+    next_state_q_vals_for_argmax = jax.vmap(online_network, in_axes=(0))(
+        next_states
+    ).q_values
   else:
-    next_state_q_vals_for_argmax = jax.vmap(
-        target_network, in_axes=(0))(next_states).q_values
+    next_state_q_vals_for_argmax = jax.vmap(target_network, in_axes=(0))(
+        next_states
+    ).q_values
   next_state_q_vals_for_argmax = jnp.squeeze(next_state_q_vals_for_argmax)
   next_argmax = jnp.argmax(next_state_q_vals_for_argmax, axis=1)
-  q_values = jax.vmap(
-      target_network, in_axes=(0))(next_states).q_values
+  q_values = jax.vmap(target_network, in_axes=(0))(next_states).q_values
   replay_next_qt_max = jax.vmap(lambda t, u: t[u])(q_values, next_argmax)
-  return jax.lax.stop_gradient(rewards + cumulative_gamma * replay_next_qt_max *
-                               (1. - terminals))
+  return jax.lax.stop_gradient(
+      rewards + cumulative_gamma * replay_next_qt_max * (1.0 - terminals)
+  )
 
 
 @gin.configurable
 class TandemDQNAgent(dqn_agent.JaxDQNAgent):
   """Tandem DQN agent."""
 
   def __init__(self, num_actions, double_dqn=True, summary_writer=None):
     self._double_dqn = double_dqn
     super().__init__(num_actions, summary_writer=summary_writer)
 
   def _build_networks_and_optimizer(self):
     self._rng, active_rng, passive_rng = jax.random.split(self._rng, 3)
     # Initialize active networks.
-    self.active_online_params = self.network_def.init(active_rng,
-                                                      x=self.state)
+    self.active_online_params = self.network_def.init(active_rng, x=self.state)
     self.active_optimizer = dqn_agent.create_optimizer(self._optimizer_name)
     self.active_optimizer_state = self.active_optimizer.init(
-        self.active_online_params)
+        self.active_online_params
+    )
     self.active_target_params = self.active_online_params
     # Initialize passive network with the regular network.
-    self.passive_online_params = self.network_def.init(passive_rng,
-                                                       x=self.state)
+    self.passive_online_params = self.network_def.init(
+        passive_rng, x=self.state
+    )
     self.passive_optimizer = dqn_agent.create_optimizer(self._optimizer_name)
     self.passive_optimizer_state = self.passive_optimizer.init(
-        self.passive_online_params)
+        self.passive_online_params
+    )
     self.passive_target_params = self.passive_online_params
 
   def _sync_weights(self):
     """Syncs the target_params with the online_params."""
     self.active_target_params = self.active_online_params
     self.passive_target_params = self.passive_online_params
 
   def _select_action(self, params):
-    self._rng, action = dqn_agent.select_action(self.network_def,
-                                                params,
-                                                self.state,
-                                                self._rng,
-                                                self.num_actions,
-                                                self.eval_mode,
-                                                self.epsilon_eval,
-                                                self.epsilon_train,
-                                                self.epsilon_decay_period,
-                                                self.training_steps,
-                                                self.min_replay_history,
-                                                self.epsilon_fn)
+    self._rng, action = dqn_agent.select_action(
+        self.network_def,
+        params,
+        self.state,
+        self._rng,
+        self.num_actions,
+        self.eval_mode,
+        self.epsilon_eval,
+        self.epsilon_train,
+        self.epsilon_decay_period,
+        self.training_steps,
+        self.min_replay_history,
+        self.epsilon_fn,
+    )
     action = onp.asarray(action)
     return action
 
   def begin_episode(self, agent_type, observation):
     self._reset_state()
     self._record_observation(observation)
     if agent_type == 'passive':
@@ -149,15 +177,16 @@
     self._record_observation(observation)
     if agent_type == 'passive':
       params = self.passive_online_params
     else:
       params = self.active_online_params
       if not self.eval_mode:
         self._store_transition(
-            self._last_observation, self.action, reward, False)
+            self._last_observation, self.action, reward, False
+        )
         self._train_step()
 
     action = self._select_action(params)
     if agent_type == 'active':
       self.action = onp.asarray(action)
     return action
 
@@ -185,37 +214,47 @@
                 self.active_optimizer_state,
                 self.replay_elements['state'],
                 self.replay_elements['action'],
                 self.replay_elements['next_state'],
                 self.replay_elements['reward'],
                 self.replay_elements['terminal'],
                 self.cumulative_gamma,
-                self._double_dqn))
-        (self.passive_optimizer_state, self.passive_online_params,
-         passive_loss) = dqn_agent.train(
-             self.network_def,
-             self.passive_online_params,
-             self.passive_target_params,
-             self.passive_optimizer,
-             self.passive_optimizer_state,
-             self.replay_elements['state'],
-             self.replay_elements['action'],
-             self.replay_elements['next_state'],
-             self.replay_elements['reward'],
-             self.replay_elements['terminal'],
-             self.cumulative_gamma,
-             self._double_dqn)
-        if (self.summary_writer is not None and
-            self.training_steps > 0 and
-            self.training_steps % self.summary_writing_frequency == 0):
+                self._double_dqn,
+            )
+        )
+        (
+            self.passive_optimizer_state,
+            self.passive_online_params,
+            passive_loss,
+        ) = dqn_agent.train(
+            self.network_def,
+            self.passive_online_params,
+            self.passive_target_params,
+            self.passive_optimizer,
+            self.passive_optimizer_state,
+            self.replay_elements['state'],
+            self.replay_elements['action'],
+            self.replay_elements['next_state'],
+            self.replay_elements['reward'],
+            self.replay_elements['terminal'],
+            self.cumulative_gamma,
+            self._double_dqn,
+        )
+        if (
+            self.summary_writer is not None
+            and self.training_steps > 0
+            and self.training_steps % self.summary_writing_frequency == 0
+        ):
           with self.summary_writer.as_default():
-            tf.summary.scalar('Losses/Active', active_loss,
-                              step=self.training_steps)
-            tf.summary.scalar('Losses/Passive', passive_loss,
-                              step=self.training_steps)
+            tf.summary.scalar(
+                'Losses/Active', active_loss, step=self.training_steps
+            )
+            tf.summary.scalar(
+                'Losses/Passive', passive_loss, step=self.training_steps
+            )
           self.summary_writer.flush()
       if self.training_steps % self.target_update_period == 0:
         self._sync_weights()
 
     self.training_steps += 1
 
   def bundle_and_checkpoint(self, checkpoint_dir, iteration_number):
@@ -258,16 +297,16 @@
     checkpoint_dir. If the checkpoint_dir does not exist, will not reset the
       agent's state.
 
     Args:
       checkpoint_dir: str, path to the checkpoint saved.
       iteration_number: int, checkpoint version, used when restoring the replay
         buffer.
-      bundle_dictionary: dict, containing additional Python objects owned by
-        the agent.
+      bundle_dictionary: dict, containing additional Python objects owned by the
+        agent.
 
     Returns:
       bool, True if unbundling was successful.
     """
     try:
       # self._replay.load() will throw a NotFoundError if it does not find all
       # the necessary files.
@@ -282,14 +321,15 @@
       self.training_steps = bundle_dictionary['training_steps']
       self.active_online_params = bundle_dictionary['active_online_params']
       self.passive_online_params = bundle_dictionary['passive_online_params']
       self.active_target_params = bundle_dictionary['active_target_params']
       self.passive_target_params = bundle_dictionary['passive_target_params']
       # We recreate the optimizer with the new online weights.
       self.active_optimizer_state = bundle_dictionary['active_optimizer_state']
-      self.passive_optimizer_state = (
-          bundle_dictionary['passive_optimizer_state'])
+      self.passive_optimizer_state = bundle_dictionary[
+          'passive_optimizer_state'
+      ]
     elif not self.allow_partial_reload:
       return False
     else:
       logging.warning("Unable to reload the agent's parameters!")
     return True
```

### Comparing `dopamine_rl-4.0.6/dopamine/labs/tandem_dqn/train.py` & `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/train.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,30 @@
 
 from dopamine.discrete_domains import run_experiment as base_run_experiment
 from dopamine.labs.tandem_dqn import run_experiment
 import tensorflow as tf
 
 
 
-flags.DEFINE_string('base_dir', None,
-                    'Base directory to host all required sub-directories.')
+flags.DEFINE_string(
+    'base_dir', None, 'Base directory to host all required sub-directories.'
+)
 flags.DEFINE_multi_string(
-    'gin_files', [], 'List of paths to gin configuration files (e.g.'
-    '"dopamine/agents/dqn/dqn.gin").')
+    'gin_files',
+    [],
+    'List of paths to gin configuration files (e.g.'
+    '"dopamine/agents/dqn/dqn.gin").',
+)
 flags.DEFINE_multi_string(
-    'gin_bindings', [],
+    'gin_bindings',
+    [],
     'Gin bindings to override the values set in the config files '
     '(e.g. "DQNAgent.epsilon_train=0.1",'
-    '      "create_environment.game_name="Pong"").')
+    '      "create_environment.game_name="Pong"").',
+)
 
 FLAGS = flags.FLAGS
 
 
 def main(unused_argv):
   """Main method.
 
@@ -48,14 +54,15 @@
   tf.compat.v1.disable_v2_behavior()
 
   base_dir = FLAGS.base_dir
   gin_files = FLAGS.gin_files
   gin_bindings = FLAGS.gin_bindings
   base_run_experiment.load_gin_configs(gin_files, gin_bindings)
   runner = run_experiment.TandemRunner(
-      base_dir, run_experiment.create_tandem_agents_and_checkpoints)
+      base_dir, run_experiment.create_tandem_agents_and_checkpoints
+  )
   runner.run_experiment()
 
 
 if __name__ == '__main__':
   flags.mark_flag_as_required('base_dir')
   app.run(main)
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/__init__.py` & `dopamine_rl-4.0.7/dopamine/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/collector.py` & `dopamine_rl-4.0.7/dopamine/metrics/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 from dopamine.metrics import statistics_instance
 import tensorflow as tf
 
 
 class Collector(abc.ABC):
   """Abstract class for defining metric collectors."""
 
-  def __init__(self, base_dir: Optional[str],
-               extra_supported_types: Sequence[str] = ()):
+  def __init__(
+      self, base_dir: Optional[str], extra_supported_types: Sequence[str] = ()
+  ):
     if base_dir is not None:
       self._base_dir = osp.join(base_dir, 'metrics', self.get_name())
       # Try to create logging directory.
       try:
         tf.io.gfile.makedirs(self._base_dir)
       except tf.errors.PermissionDeniedError:
         # If it already exists, ignore exception.
@@ -57,16 +58,16 @@
     pass
 
   def check_type(self, data_type: str) -> bool:
     return data_type in self._supported_types
 
   @abc.abstractmethod
   def write(
-      self,
-      statistics: Sequence[statistics_instance.StatisticsInstance]) -> None:
+      self, statistics: Sequence[statistics_instance.StatisticsInstance]
+  ) -> None:
     pass
 
   def flush(self) -> None:
     pass
 
   def close(self) -> None:
     pass
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/collector_dispatcher.py` & `dopamine_rl-4.0.7/dopamine/metrics/collector_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,27 +66,29 @@
 class CollectorDispatcher(object):
   """Class for collecting and reporting Dopamine metrics."""
 
   def __init__(
       self,
       base_dir: Optional[str],
       # TODO(psc): Consider using sets instead.
-      collectors: Sequence[str] = ('console', 'pickle', 'tensorboard')):
+      collectors: Sequence[str] = ('console', 'pickle', 'tensorboard'),
+  ):
     self._collectors = []
     for c in collectors:
       if c not in AVAILABLE_COLLECTORS:
         logging.warning('Collector %s not recognized, ignoring.', c)
         continue
       self._collectors.append(AVAILABLE_COLLECTORS[c](base_dir))
       logging.info('Added collector %s.', c)
 
   def write(
       self,
       statistics: Sequence[statistics_instance.StatisticsInstance],
-      collector_allowlist: Sequence[str] = ()) -> None:
+      collector_allowlist: Sequence[str] = (),
+  ) -> None:
     """Write a list of statistics to various collectors.
 
     Args:
       statistics: A list of of StatisticsInstances to write.
       collector_allowlist: A list of Collectors to include in this call to
         write. This is to enable users to, for instance, which Collectors will
         be used to write fine-grained statistics. If collector_allowlist is
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/console_collector.py` & `dopamine_rl-4.0.7/dopamine/metrics/console_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,30 +24,28 @@
 import tensorflow as tf
 
 
 @gin.configurable(allowlist=['save_to_file'])
 class ConsoleCollector(collector.Collector):
   """Collector class for reporting statistics to the console."""
 
-  def __init__(self,
-               base_dir: Union[str, None],
-               save_to_file: bool = True):
+  def __init__(self, base_dir: Union[str, None], save_to_file: bool = True):
     super().__init__(base_dir)
     if self._base_dir is not None and save_to_file:
       self._log_file = osp.join(self._base_dir, 'console.log')
       self._log_file_writer = tf.io.gfile.GFile(self._log_file, 'w')
     else:
       self._log_file = None
 
   def get_name(self) -> str:
     return 'console'
 
   def write(
-      self,
-      statistics: Sequence[statistics_instance.StatisticsInstance]) -> None:
+      self, statistics: Sequence[statistics_instance.StatisticsInstance]
+  ) -> None:
     step_string = ''
     for s in statistics:
       if not self.check_type(s.type):
         continue
       step_string += f'[Iteration {s.step}]: {s.name} = {s.value}\n'
     # Only write out if step_string is non-empty
     if step_string:
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/pickle_collector.py` & `dopamine_rl-4.0.7/dopamine/metrics/pickle_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     self._statistics = collections.defaultdict(listdict)
     self._file_number = 0
 
   def get_name(self) -> str:
     return 'pickle'
 
   def write(
-      self,
-      statistics: Sequence[statistics_instance.StatisticsInstance]) -> None:
+      self, statistics: Sequence[statistics_instance.StatisticsInstance]
+  ) -> None:
     # This Collector is trying to write metrics as close as possible to what
     # is currently written by the Dopamine Logger, so as to be as compatible
     # with user's plotting setups.
     for s in statistics:
       if not self.check_type(s.type):
         continue
       self._statistics[f'iteration_{s.step}'][s.name].append(s.value)
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/statistics_instance.py` & `dopamine_rl-4.0.7/dopamine/metrics/statistics_instance.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 import dataclasses
 from typing import Any
 
 
 @dataclasses.dataclass
 class StatisticsInstance:
   """Statistics to be passed to each of the collectors."""
+
   name: str
   value: Any
   step: int
   type: str = 'scalar'
```

### Comparing `dopamine_rl-4.0.6/dopamine/metrics/tensorboard_collector.py` & `dopamine_rl-4.0.7/dopamine/metrics/tensorboard_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,25 @@
 
 class TensorboardCollector(collector.Collector):
   """Collector class for reporting statistics on Tensorboard."""
 
   def __init__(self, base_dir: str):
     if not isinstance(base_dir, str):
       raise ValueError(
-          'Must specify a base directory for TensorboardCollector.')
+          'Must specify a base directory for TensorboardCollector.'
+      )
     super().__init__(base_dir)
     self.summary_writer = tf.summary.create_file_writer(self._base_dir)
 
   def get_name(self) -> str:
     return 'tensorboard'
 
   def write(
-      self,
-      statistics: Sequence[statistics_instance.StatisticsInstance]) -> None:
+      self, statistics: Sequence[statistics_instance.StatisticsInstance]
+  ) -> None:
     with self.summary_writer.as_default():
       for s in statistics:
         if not self.check_type(s.type):
           continue
         tf.summary.scalar(s.name, s.value, step=s.step)
 
   def flush(self):
```

### Comparing `dopamine_rl-4.0.6/dopamine/replay_memory/__init__.py` & `dopamine_rl-4.0.7/dopamine/replay_memory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/replay_memory/circular_replay_buffer.py` & `dopamine_rl-4.0.7/dopamine/replay_memory/circular_replay_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
 
 # Defines a type describing part of the tuple returned by the replay
 # memory. Each element of the tuple is a tensor of shape [batch, ...] where
 # ... is defined the 'shape' field of ReplayElement. The tensor type is
 # given by the 'type' field. The 'name' field is for convenience and ease of
 # debugging.
-ReplayElement = (
-    collections.namedtuple('shape_type', ['name', 'shape', 'type']))
+ReplayElement = collections.namedtuple('shape_type', ['name', 'shape', 'type'])
 
 # A prefix that can not collide with variable names for checkpoint files.
 STORE_FILENAME_PREFIX = '$store$_'
 
 
 def modulo_range(start, length, modulo):
   for i in range(length):
@@ -67,21 +66,23 @@
   It handles special cases in a circular buffer in the beginning and the end.
 
   Args:
     cursor: int, the position of the cursor.
     replay_capacity: int, the size of the replay memory.
     stack_size: int, the size of the stacks returned by the replay memory.
     update_horizon: int, the agent's update horizon.
+
   Returns:
     np.array of size stack_size with the invalid indices.
   """
   assert cursor < replay_capacity
-  return np.array(
-      [(cursor - update_horizon + i) % replay_capacity
-       for i in range(stack_size + update_horizon)])
+  return np.array([
+      (cursor - update_horizon + i) % replay_capacity
+      for i in range(stack_size + update_horizon)
+  ])
 
 
 @gin.configurable
 class OutOfGraphReplayBuffer(object):
   """A simple out-of-graph Replay Buffer.
 
   Stores transitions, state, action, reward, next_state, terminal (and any
@@ -93,46 +94,48 @@
   at sample time.
 
   Attributes:
     add_count: int, counter of how many transitions have been added (including
       the blank ones at the beginning of an episode).
     invalid_range: np.array, an array with the indices of cursor-related invalid
       transitions
-    episode_end_indices: set[int], a set of indices corresponding to the
-      end of an episode.
+    episode_end_indices: set[int], a set of indices corresponding to the end of
+      an episode.
   """
 
-  def __init__(self,
-               observation_shape,
-               stack_size,
-               replay_capacity,
-               batch_size,
-               update_horizon=1,
-               gamma=0.99,
-               max_sample_attempts=1000,
-               extra_storage_types=None,
-               observation_dtype=np.uint8,
-               terminal_dtype=np.uint8,
-               action_shape=(),
-               action_dtype=np.int32,
-               reward_shape=(),
-               reward_dtype=np.float32,
-               checkpoint_duration=4,
-               keep_every=None):
+  def __init__(
+      self,
+      observation_shape,
+      stack_size,
+      replay_capacity,
+      batch_size,
+      update_horizon=1,
+      gamma=0.99,
+      max_sample_attempts=1000,
+      extra_storage_types=None,
+      observation_dtype=np.uint8,
+      terminal_dtype=np.uint8,
+      action_shape=(),
+      action_dtype=np.int32,
+      reward_shape=(),
+      reward_dtype=np.float32,
+      checkpoint_duration=4,
+      keep_every=None,
+  ):
     """Initializes OutOfGraphReplayBuffer.
 
     Args:
       observation_shape: tuple of ints.
       stack_size: int, number of frames to use in state stack.
       replay_capacity: int, number of transitions to keep in memory.
       batch_size: int.
       update_horizon: int, length of update ('n' in n-step update).
-      gamma: int, the discount factor.
-      max_sample_attempts: int, the maximum number of attempts allowed to
-        get a sample.
+      gamma: float, the discount factor.
+      max_sample_attempts: int, the maximum number of attempts allowed to get a
+        sample.
       extra_storage_types: list of ReplayElements defining the type of the extra
         contents that will be stored and returned by sample_transition_batch.
       observation_dtype: np.dtype, type of the observations. Defaults to
         np.uint8 for Atari 2600.
       terminal_dtype: np.dtype, type of the terminals. Defaults to np.uint8 for
         Atari 2600.
       action_shape: tuple of ints, the shape for the action vector. Empty tuple
@@ -147,20 +150,22 @@
 
     Raises:
       ValueError: If replay_capacity is too small to hold at least one
         transition.
     """
     assert isinstance(observation_shape, tuple)
     if replay_capacity < update_horizon + stack_size:
-      raise ValueError('There is not enough capacity to cover '
-                       'update_horizon and stack_size.')
+      raise ValueError(
+          'There is not enough capacity to cover update_horizon and stack_size.'
+      )
 
     logging.info(
         'Creating a %s replay memory with the following parameters:',
-        self.__class__.__name__)
+        self.__class__.__name__,
+    )
     logging.info('\t observation_shape: %s', str(observation_shape))
     logging.info('\t observation_dtype: %s', str(observation_dtype))
     logging.info('\t terminal_dtype: %s', str(terminal_dtype))
     logging.info('\t stack_size: %d', stack_size)
     logging.info('\t replay_capacity: %d', replay_capacity)
     logging.info('\t batch_size: %d', batch_size)
     logging.info('\t update_horizon: %d', update_horizon)
@@ -189,35 +194,38 @@
     self._create_storage()
     self.add_count = np.array(0)
     self.invalid_range = np.zeros((self._stack_size))
     # When the horizon is > 1, we compute the sum of discounted rewards as a dot
     # product using the precomputed vector <gamma^0, gamma^1, ..., gamma^{n-1}>.
     self._cumulative_discount_vector = np.array(
         [math.pow(self._gamma, n) for n in range(update_horizon)],
-        dtype=np.float32)
+        dtype=np.float32,
+    )
     self._next_experience_is_episode_start = True
     self.episode_end_indices = set()
     self._checkpoint_duration = checkpoint_duration
     self._keep_every = keep_every
 
   @property
   def _episode_end_indices(self):
-    logging.warning('The name `_episode_end_indices` will be deprecated '
-                    'in a future version of Dopamine. Please use '
-                    '`episode_end_indices` instead.')
+    logging.warning(
+        'The name `_episode_end_indices` will be deprecated '
+        'in a future version of Dopamine. Please use '
+        '`episode_end_indices` instead.'
+    )
     return self.episode_end_indices
 
   def _create_storage(self):
-    """Creates the numpy arrays used to store transitions.
-    """
+    """Creates the numpy arrays used to store transitions."""
     self._store = {}
     for storage_element in self.get_storage_signature():
       array_shape = [self._replay_capacity] + list(storage_element.shape)
       self._store[storage_element.name] = np.empty(
-          array_shape, dtype=storage_element.type)
+          array_shape, dtype=storage_element.type
+      )
 
   def get_add_args_signature(self):
     """The signature of the add function.
 
     Note - Derived classes may return a different signature.
 
     Returns:
@@ -231,43 +239,46 @@
 
     Note - Derived classes may return a different signature.
 
     Returns:
       list of ReplayElements defining the type of the contents stored.
     """
     storage_elements = [
-        ReplayElement('observation', self._observation_shape,
-                      self._observation_dtype),
+        ReplayElement(
+            'observation', self._observation_shape, self._observation_dtype
+        ),
         ReplayElement('action', self._action_shape, self._action_dtype),
         ReplayElement('reward', self._reward_shape, self._reward_dtype),
-        ReplayElement('terminal', (), self._terminal_dtype)
+        ReplayElement('terminal', (), self._terminal_dtype),
     ]
 
     for extra_replay_element in self._extra_storage_types:
       storage_elements.append(extra_replay_element)
     return storage_elements
 
   def _add_zero_transition(self):
-    """Adds a padding transition filled with zeros (Used in episode beginnings).
-    """
+    """Adds a padding transition filled with zeros (Used in episode beginnings)."""
     zero_transition = []
     for element_type in self.get_add_args_signature():
       zero_transition.append(
-          np.zeros(element_type.shape, dtype=element_type.type))
+          np.zeros(element_type.shape, dtype=element_type.type)
+      )
     self.episode_end_indices.discard(self.cursor())  # If present
     self._add(*zero_transition)
 
-  def add(self,
-          observation,
-          action,
-          reward,
-          terminal,
-          *args,
-          priority=None,
-          episode_end=False):
+  def add(
+      self,
+      observation,
+      action,
+      reward,
+      terminal,
+      *args,
+      priority=None,
+      episode_end=False
+  ):
     """Adds a transition to the replay memory.
 
     This function checks the types and handles the padding at the beginning of
     an episode. Then it calls the _add function.
 
     Since the next_observation in the transition will be the observation added
     next there is no need to pass it.
@@ -275,25 +286,25 @@
     If the replay memory is at capacity the oldest transition will be discarded.
 
     Args:
       observation: np.array with shape observation_shape.
       action: int, the action in the transition.
       reward: float, the reward received in the transition.
       terminal: np.dtype, acts as a boolean indicating whether the transition
-                was terminal (1) or not (0).
+        was terminal (1) or not (0).
       *args: extra contents with shapes and dtypes according to
         extra_storage_types.
-      priority: float, unused in the circular replay buffer, but may be used
-        in child classes like PrioritizedReplayBuffer.
-      episode_end: bool, whether this experience is the last experience in
-        the episode. This is useful for tasks that terminate due to time-out,
-        but do not end on a terminal state. Overloading 'terminal' may not
-        be sufficient in this case, since 'terminal' is passed to the agent
-        for training. 'episode_end' allows the replay buffer to determine
-        episode boundaries without passing that information to the agent.
+      priority: float, unused in the circular replay buffer, but may be used in
+        child classes like PrioritizedReplayBuffer.
+      episode_end: bool, whether this experience is the last experience in the
+        episode. This is useful for tasks that terminate due to time-out, but do
+        not end on a terminal state. Overloading 'terminal' may not be
+        sufficient in this case, since 'terminal' is passed to the agent for
+        training. 'episode_end' allows the replay buffer to determine episode
+        boundaries without passing that information to the agent.
     """
     if priority is not None:
       args = args + (priority,)
 
     self._check_add_types(observation, action, reward, terminal, *args)
     if self._next_experience_is_episode_start:
       for _ in range(self._stack_size - 1):
@@ -313,46 +324,53 @@
   def _add(self, *args):
     """Internal add method to add to the storage arrays.
 
     Args:
       *args: All the elements in a transition.
     """
     self._check_args_length(*args)
-    transition = {e.name: args[idx]
-                  for idx, e in enumerate(self.get_add_args_signature())}
+    transition = {
+        e.name: args[idx] for idx, e in enumerate(self.get_add_args_signature())
+    }
     self._add_transition(transition)
 
   def _add_transition(self, transition):
     """Internal add method to add transition dictionary to storage arrays.
 
     Args:
-      transition: The dictionary of names and values of the transition
-                  to add to the storage.
+      transition: The dictionary of names and values of the transition to add to
+        the storage.
     """
     cursor = self.cursor()
     for arg_name in transition:
       self._store[arg_name][cursor] = transition[arg_name]
 
     self.add_count += 1
     self.invalid_range = invalid_range(
-        self.cursor(), self._replay_capacity, self._stack_size,
-        self._update_horizon)
+        self.cursor(),
+        self._replay_capacity,
+        self._stack_size,
+        self._update_horizon,
+    )
 
   def _check_args_length(self, *args):
     """Check if args passed to the add method have the same length as storage.
 
     Args:
       *args: Args for elements used in storage.
 
     Raises:
       ValueError: If args have wrong length.
     """
     if len(args) != len(self.get_add_args_signature()):
-      raise ValueError('Add expects {} elements, received {}'.format(
-          len(self.get_add_args_signature()), len(args)))
+      raise ValueError(
+          'Add expects {} elements, received {}'.format(
+              len(self.get_add_args_signature()), len(args)
+          )
+      )
 
   def _check_add_types(self, *args):
     """Checks if args passed to the add method match those of the storage.
 
     Args:
       *args: Args whose types need to be validated.
 
@@ -367,16 +385,19 @@
         # TODO(b/80536437). This is not efficient when arg_element is a list.
         arg_shape = np.array(arg_element).shape
       else:
         # Assume it is scalar.
         arg_shape = tuple()
       store_element_shape = tuple(store_element.shape)
       if arg_shape != store_element_shape:
-        raise ValueError('arg has shape {}, expected {}'.format(
-            arg_shape, store_element_shape))
+        raise ValueError(
+            'arg has shape {}, expected {}'.format(
+                arg_shape, store_element_shape
+            )
+        )
 
   def is_empty(self):
     """Is the Replay Buffer empty?"""
     return self.add_count == 0
 
   def is_full(self):
     """Is the Replay Buffer full?"""
@@ -399,52 +420,56 @@
     Returns:
       np.array, with shape [end_index - start_index, array.shape[1:]].
     """
     assert end_index > start_index, 'end_index must be larger than start_index'
     assert end_index >= 0
     assert start_index < self._replay_capacity
     if not self.is_full():
-      assert end_index <= self.cursor(), (
-          'Index {} has not been added.'.format(start_index))
+      assert end_index <= self.cursor(), 'Index {} has not been added.'.format(
+          start_index
+      )
 
     # Fast slice read when there is no wraparound.
     if start_index % self._replay_capacity < end_index % self._replay_capacity:
       return_array = array[start_index:end_index, ...]
     # Slow list read.
     else:
-      indices = [(start_index + i) % self._replay_capacity
-                 for i in range(end_index - start_index)]
+      indices = [
+          (start_index + i) % self._replay_capacity
+          for i in range(end_index - start_index)
+      ]
       return_array = array[indices, ...]
     return return_array
 
   def get_observation_stack(self, index):
     return self._get_element_stack(index, 'observation')
 
   def _get_element_stack(self, index, element_name):
-    state = self.get_range(self._store[element_name],
-                           index - self._stack_size + 1, index + 1)
+    state = self.get_range(
+        self._store[element_name], index - self._stack_size + 1, index + 1
+    )
     # The stacking axis is 0 but the agent expects as the last axis.
     return np.moveaxis(state, 0, -1)
 
   def get_terminal_stack(self, index):
-    return self.get_range(self._store['terminal'], index - self._stack_size + 1,
-                          index + 1)
+    return self.get_range(
+        self._store['terminal'], index - self._stack_size + 1, index + 1
+    )
 
   def is_valid_transition(self, index):
     """Checks if the index contains a valid transition.
 
     Checks for collisions with the end of episodes and the current position
     of the cursor.
 
     Args:
       index: int, the index to the state in the transition.
 
     Returns:
       Is the index valid: Boolean.
-
     """
     # Check the index is in the valid range
     if index < 0 or index >= self._replay_capacity:
       return False
     if not self.is_full():
       # The indices and next_indices must be smaller than the cursor.
       if index >= self.cursor() - self._update_horizon:
@@ -508,32 +533,38 @@
       min_id = self.cursor() - self._replay_capacity + self._stack_size - 1
       max_id = self.cursor() - self._update_horizon
     else:
       # add_count < self._replay_capacity
       min_id = self._stack_size - 1
       max_id = self.cursor() - self._update_horizon
       if max_id <= min_id:
-        raise RuntimeError('Cannot sample a batch with fewer than stack size '
-                           '({}) + update_horizon ({}) transitions.'.
-                           format(self._stack_size, self._update_horizon))
+        raise RuntimeError(
+            'Cannot sample a batch with fewer than stack size '
+            '({}) + update_horizon ({}) transitions.'.format(
+                self._stack_size, self._update_horizon
+            )
+        )
 
     indices = []
     attempt_count = 0
-    while (len(indices) < batch_size and
-           attempt_count < self._max_sample_attempts):
+    while (
+        len(indices) < batch_size and attempt_count < self._max_sample_attempts
+    ):
       index = np.random.randint(min_id, max_id) % self._replay_capacity
       if self.is_valid_transition(index):
         indices.append(index)
       else:
         attempt_count += 1
     if len(indices) != batch_size:
       raise RuntimeError(
           'Max sample attempts: Tried {} times but only sampled {}'
-          ' valid indices. Batch size is {}'.
-          format(self._max_sample_attempts, len(indices), batch_size))
+          ' valid indices. Batch size is {}'.format(
+              self._max_sample_attempts, len(indices), batch_size
+          )
+      )
 
     return indices
 
   def sample_transition_batch(self, batch_size=None, indices=None):
     """Returns a batch of transitions (including any extra contents).
 
     If get_transition_elements has been overridden and defines elements not
@@ -567,88 +598,107 @@
     if indices is None:
       indices = self.sample_index_batch(batch_size)
     assert len(indices) == batch_size
 
     transition_elements = self.get_transition_elements(batch_size)
     batch_arrays = self._create_batch_arrays(batch_size)
     for batch_element, state_index in enumerate(indices):
-      trajectory_indices = [(state_index + j) % self._replay_capacity
-                            for j in range(self._update_horizon)]
+      trajectory_indices = [
+          (state_index + j) % self._replay_capacity
+          for j in range(self._update_horizon)
+      ]
       trajectory_terminals = self._store['terminal'][trajectory_indices]
       is_terminal_transition = trajectory_terminals.any()
       if not is_terminal_transition:
         trajectory_length = self._update_horizon
       else:
         # np.argmax of a bool array returns the index of the first True.
-        trajectory_length = np.argmax(trajectory_terminals.astype(bool),
-                                      0) + 1
+        trajectory_length = np.argmax(trajectory_terminals.astype(bool), 0) + 1
       next_state_index = state_index + trajectory_length
-      trajectory_discount_vector = (
-          self._cumulative_discount_vector[:trajectory_length])
-      trajectory_rewards = self.get_range(self._store['reward'], state_index,
-                                          next_state_index)
+      trajectory_discount_vector = self._cumulative_discount_vector[
+          :trajectory_length
+      ]
+      trajectory_rewards = self.get_range(
+          self._store['reward'], state_index, next_state_index
+      )
 
       # Fill the contents of each array in the sampled batch.
       assert len(transition_elements) == len(batch_arrays)
       for element_array, element in zip(batch_arrays, transition_elements):
         if element.name == 'state':
           element_array[batch_element] = self.get_observation_stack(state_index)
         elif element.name == 'reward':
           # compute the discounted sum of rewards in the trajectory.
           element_array[batch_element] = np.sum(
-              trajectory_discount_vector * trajectory_rewards, axis=0)
+              trajectory_discount_vector * trajectory_rewards, axis=0
+          )
         elif element.name == 'next_state':
           element_array[batch_element] = self.get_observation_stack(
-              (next_state_index) % self._replay_capacity)
+              (next_state_index) % self._replay_capacity
+          )
         elif element.name in ('next_action', 'next_reward'):
-          element_array[batch_element] = (
-              self._store[element.name.lstrip('next_')][(next_state_index) %
-                                                        self._replay_capacity])
+          element_array[batch_element] = self._store[
+              element.name.lstrip('next_')
+          ][(next_state_index) % self._replay_capacity]
         elif element.name == 'terminal':
           element_array[batch_element] = is_terminal_transition
         elif element.name == 'indices':
           element_array[batch_element] = state_index
         elif element.name in self._store.keys():
-          element_array[batch_element] = (
-              self._store[element.name][state_index])
+          element_array[batch_element] = self._store[element.name][state_index]
         # We assume the other elements are filled in by the subclass.
 
     return batch_arrays
 
   def get_transition_elements(self, batch_size=None):
     """Returns a 'type signature' for sample_transition_batch.
 
     Args:
       batch_size: int, number of transitions returned. If None, the default
         batch_size will be used.
+
     Returns:
       signature: A namedtuple describing the method's return type signature.
     """
     batch_size = self._batch_size if batch_size is None else batch_size
 
     transition_elements = [
-        ReplayElement('state', (batch_size,) + self._state_shape,
-                      self._observation_dtype),
-        ReplayElement('action', (batch_size,) + self._action_shape,
-                      self._action_dtype),
-        ReplayElement('reward', (batch_size,) + self._reward_shape,
-                      self._reward_dtype),
-        ReplayElement('next_state', (batch_size,) + self._state_shape,
-                      self._observation_dtype),
-        ReplayElement('next_action', (batch_size,) + self._action_shape,
-                      self._action_dtype),
-        ReplayElement('next_reward', (batch_size,) + self._reward_shape,
-                      self._reward_dtype),
+        ReplayElement(
+            'state', (batch_size,) + self._state_shape, self._observation_dtype
+        ),
+        ReplayElement(
+            'action', (batch_size,) + self._action_shape, self._action_dtype
+        ),
+        ReplayElement(
+            'reward', (batch_size,) + self._reward_shape, self._reward_dtype
+        ),
+        ReplayElement(
+            'next_state',
+            (batch_size,) + self._state_shape,
+            self._observation_dtype,
+        ),
+        ReplayElement(
+            'next_action',
+            (batch_size,) + self._action_shape,
+            self._action_dtype,
+        ),
+        ReplayElement(
+            'next_reward',
+            (batch_size,) + self._reward_shape,
+            self._reward_dtype,
+        ),
         ReplayElement('terminal', (batch_size,), self._terminal_dtype),
-        ReplayElement('indices', (batch_size,), np.int32)
+        ReplayElement('indices', (batch_size,), np.int32),
     ]
     for element in self._extra_storage_types:
       transition_elements.append(
-          ReplayElement(element.name, (batch_size,) + tuple(element.shape),
-                        element.type))
+          ReplayElement(
+              element.name, (batch_size,) + tuple(element.shape), element.type
+          )
+      )
     return transition_elements
 
   def _generate_filename(self, checkpoint_dir, name, suffix):
     return os.path.join(checkpoint_dir, '{}_ckpt.{}.gz'.format(name, suffix))
 
   def _return_checkpointable_elements(self):
     """Return the dict of elements of the class for checkpointing.
@@ -670,16 +720,16 @@
     """Save the OutOfGraphReplayBuffer attributes into a file.
 
     This method will save all the replay buffer's state in a single file.
 
     Args:
       checkpoint_dir: str, the directory where numpy checkpoint files should be
         saved.
-      iteration_number: int, iteration_number to use as a suffix in naming
-        numpy checkpoint files.
+      iteration_number: int, iteration_number to use as a suffix in naming numpy
+        checkpoint files.
     """
     if not tf.io.gfile.exists(checkpoint_dir):
       return
 
     checkpointable_elements = self._return_checkpointable_elements()
 
     for attr in checkpointable_elements:
@@ -687,34 +737,36 @@
       with tf.io.gfile.GFile(filename, 'wb') as f:
         with gzip.GzipFile(fileobj=f, mode='wb') as outfile:
           # Checkpoint the np arrays in self._store with np.save instead of
           # pickling the dictionary is critical for file size and performance.
           # STORE_FILENAME_PREFIX indicates that the variable is contained in
           # self._store.
           if attr.startswith(STORE_FILENAME_PREFIX):
-            array_name = attr[len(STORE_FILENAME_PREFIX):]
+            array_name = attr[len(STORE_FILENAME_PREFIX) :]
             np.save(outfile, self._store[array_name], allow_pickle=False)
           # Some numpy arrays might not be part of storage
           elif isinstance(self.__dict__[attr], np.ndarray):
             np.save(outfile, self.__dict__[attr], allow_pickle=False)
           else:
             pickle.dump(self.__dict__[attr], outfile)
 
       # After writing a checkpoint file, we garbage collect the checkpoint file
       # that is four versions old.
       stale_iteration_number = iteration_number - self._checkpoint_duration
 
       # If keep_every has been set, we spare every keep_every'th checkpoint.
-      if (self._keep_every is not None and
-          (stale_iteration_number % self._keep_every == 0)):
+      if self._keep_every is not None and (
+          stale_iteration_number % self._keep_every == 0
+      ):
         return
 
       if stale_iteration_number >= 0:
-        stale_filename = self._generate_filename(checkpoint_dir, attr,
-                                                 stale_iteration_number)
+        stale_filename = self._generate_filename(
+            checkpoint_dir, attr, stale_iteration_number
+        )
         try:
           tf.io.gfile.remove(stale_filename)
         except tf.errors.NotFoundError:
           pass
 
   def load(self, checkpoint_dir, suffix):
     """Restores the object from bundle_dictionary and numpy checkpoints.
@@ -732,85 +784,91 @@
     # We will first make sure we have all the necessary files available to avoid
     # loading a partially-specified (i.e. corrupted) replay buffer.
     for attr in save_elements:
       filename = self._generate_filename(checkpoint_dir, attr, suffix)
 
       if not tf.io.gfile.exists(filename):
         if attr == 'episode_end_indices':
-          logging.warning('Unable to find episode_end_indices. This is '
-                          'expected for old checkpoints.')
+          logging.warning(
+              'Unable to find episode_end_indices. This is '
+              'expected for old checkpoints.'
+          )
           skip_episode_end_indices = True
           continue
 
-        raise tf.errors.NotFoundError(None, None,
-                                      'Missing file: {}'.format(filename))
+        raise tf.errors.NotFoundError(
+            None, None, 'Missing file: {}'.format(filename)
+        )
     # If we've reached this point then we have verified that all expected files
     # are available.
     for attr in save_elements:
       if attr == 'episode_end_indices' and skip_episode_end_indices:
         continue
 
       filename = self._generate_filename(checkpoint_dir, attr, suffix)
       with tf.io.gfile.GFile(filename, 'rb') as f:
         with gzip.GzipFile(fileobj=f) as infile:
           if attr.startswith(STORE_FILENAME_PREFIX):
-            array_name = attr[len(STORE_FILENAME_PREFIX):]
+            array_name = attr[len(STORE_FILENAME_PREFIX) :]
             self._store[array_name] = np.load(infile, allow_pickle=False)
           elif isinstance(self.__dict__[attr], np.ndarray):
             self.__dict__[attr] = np.load(infile, allow_pickle=False)
           else:
             self.__dict__[attr] = pickle.load(infile)
 
 
 @gin.configurable(
-    denylist=['observation_shape', 'stack_size', 'update_horizon', 'gamma'])
+    denylist=['observation_shape', 'stack_size', 'update_horizon', 'gamma']
+)
 class WrappedReplayBuffer(object):
   """Wrapper of OutOfGraphReplayBuffer with an in graph sampling mechanism.
 
   Usage:
     To add a transition:  call the add function.
 
     To sample a batch:    Construct operations that depend on any of the
                           tensors is the transition dictionary. Every sess.run
                           that requires any of these tensors will sample a new
                           transition.
   """
 
-  def __init__(self,
-               observation_shape,
-               stack_size,
-               use_staging=False,
-               replay_capacity=1000000,
-               batch_size=32,
-               update_horizon=1,
-               gamma=0.99,
-               wrapped_memory=None,
-               max_sample_attempts=1000,
-               extra_storage_types=None,
-               observation_dtype=np.uint8,
-               terminal_dtype=np.uint8,
-               action_shape=(),
-               action_dtype=np.int32,
-               reward_shape=(),
-               reward_dtype=np.float32):
+  def __init__(
+      self,
+      observation_shape,
+      stack_size,
+      use_staging=False,
+      replay_capacity=1000000,
+      batch_size=32,
+      update_horizon=1,
+      gamma=0.99,
+      wrapped_memory=None,
+      max_sample_attempts=1000,
+      extra_storage_types=None,
+      observation_dtype=np.uint8,
+      terminal_dtype=np.uint8,
+      action_shape=(),
+      action_dtype=np.int32,
+      reward_shape=(),
+      reward_dtype=np.float32,
+  ):
     """Initializes WrappedReplayBuffer.
 
     Args:
       observation_shape: tuple of ints.
       stack_size: int, number of frames to use in state stack.
-      use_staging: bool, when True it would use a staging area to prefetch
-        the next sampling batch.
+      use_staging: bool, when True it would use a staging area to prefetch the
+        next sampling batch.
       replay_capacity: int, number of transitions to keep in memory.
       batch_size: int.
       update_horizon: int, length of update ('n' in n-step update).
       gamma: int, the discount factor.
-      wrapped_memory: The 'inner' memory data structure. If None,
-        it creates the standard DQN replay memory.
-      max_sample_attempts: int, the maximum number of attempts allowed to
-        get a sample.
+      wrapped_memory: The 'inner' memory data structure. If None, it creates the
+        standard DQN replay memory.
+      max_sample_attempts: int, the maximum number of attempts allowed to get a
+        sample.
       extra_storage_types: list of ReplayElements defining the type of the extra
         contents that will be stored and returned by sample_transition_batch.
       observation_dtype: np.dtype, type of the observations. Defaults to
         np.uint8 for Atari 2600.
       terminal_dtype: np.dtype, type of the terminals. Defaults to np.uint8 for
         Atari 2600.
       action_shape: tuple of ints, the shape for the action vector. Empty tuple
@@ -823,15 +881,16 @@
     Raises:
       ValueError: If update_horizon is not positive.
       ValueError: If discount factor is not in [0, 1].
     """
     if replay_capacity < update_horizon + 1:
       raise ValueError(
           'Update horizon ({}) should be significantly smaller '
-          'than replay capacity ({}).'.format(update_horizon, replay_capacity))
+          'than replay capacity ({}).'.format(update_horizon, replay_capacity)
+      )
     if not update_horizon >= 1:
       raise ValueError('Update horizon must be positive.')
     if not 0.0 <= gamma <= 1.0:
       raise ValueError('Discount factor (gamma) must be in [0, 1].')
 
     self.batch_size = batch_size
 
@@ -849,15 +908,16 @@
           max_sample_attempts,
           observation_dtype=observation_dtype,
           terminal_dtype=terminal_dtype,
           extra_storage_types=extra_storage_types,
           action_shape=action_shape,
           action_dtype=action_dtype,
           reward_shape=reward_shape,
-          reward_dtype=reward_dtype)
+          reward_dtype=reward_dtype,
+      )
 
     self.create_sampling_ops(use_staging)
 
   def add(self, observation, action, reward, terminal, *args):
     """Adds a transition to the replay memory.
 
     Since the next_observation in the transition will be the observation added
@@ -866,38 +926,40 @@
     If the replay memory is at capacity the oldest transition will be discarded.
 
     Args:
       observation: np.array with shape observation_shape.
       action: int, the action in the transition.
       reward: float, the reward received in the transition.
       terminal: np.dtype, acts as a boolean indicating whether the transition
-                was terminal (1) or not (0).
+        was terminal (1) or not (0).
       *args: extra contents with shapes and dtypes according to
         extra_storage_types.
     """
     self.memory.add(observation, action, reward, terminal, *args)
 
   def create_sampling_ops(self, use_staging):
     """Creates the ops necessary to sample from the replay buffer.
 
     Creates the transition dictionary containing the sampling tensors.
 
     Args:
-      use_staging: bool, when True it would use a staging area to prefetch
-        the next sampling batch.
+      use_staging: bool, when True it would use a staging area to prefetch the
+        next sampling batch.
     """
     if use_staging:
       logging.warning('use_staging=True is no longer supported')
     with tf.name_scope('sample_replay'):
       with tf.device('/cpu:*'):
         transition_type = self.memory.get_transition_elements()
         transition_tensors = tf.numpy_function(
-            self.memory.sample_transition_batch, [],
+            self.memory.sample_transition_batch,
+            [],
             [return_entry.type for return_entry in transition_type],
-            name='replay_sample_py_func')
+            name='replay_sample_py_func',
+        )
         self._set_transition_shape(transition_tensors, transition_type)
         # Unpack sample transition into member variables.
         self.unpack_transition(transition_tensors, transition_type)
 
   def _set_transition_shape(self, transition, transition_type):
     """Set shape for each element in the transition.
```

### Comparing `dopamine_rl-4.0.6/dopamine/replay_memory/prioritized_replay_buffer.py` & `dopamine_rl-4.0.7/dopamine/replay_memory/prioritized_replay_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,46 +30,49 @@
 import gin.tf
 import numpy as np
 import tensorflow as tf
 
 
 @gin.configurable
 class OutOfGraphPrioritizedReplayBuffer(
-    circular_replay_buffer.OutOfGraphReplayBuffer):
+    circular_replay_buffer.OutOfGraphReplayBuffer
+):
   """An out-of-graph Replay Buffer for Prioritized Experience Replay.
 
   See circular_replay_buffer.py for details.
   """
 
-  def __init__(self,
-               observation_shape,
-               stack_size,
-               replay_capacity,
-               batch_size,
-               update_horizon=1,
-               gamma=0.99,
-               max_sample_attempts=1000,
-               extra_storage_types=None,
-               observation_dtype=np.uint8,
-               terminal_dtype=np.uint8,
-               action_shape=(),
-               action_dtype=np.int32,
-               reward_shape=(),
-               reward_dtype=np.float32):
+  def __init__(
+      self,
+      observation_shape,
+      stack_size,
+      replay_capacity,
+      batch_size,
+      update_horizon=1,
+      gamma=0.99,
+      max_sample_attempts=1000,
+      extra_storage_types=None,
+      observation_dtype=np.uint8,
+      terminal_dtype=np.uint8,
+      action_shape=(),
+      action_dtype=np.int32,
+      reward_shape=(),
+      reward_dtype=np.float32,
+  ):
     """Initializes OutOfGraphPrioritizedReplayBuffer.
 
     Args:
       observation_shape: tuple of ints.
       stack_size: int, number of frames to use in state stack.
       replay_capacity: int, number of transitions to keep in memory.
       batch_size: int.
       update_horizon: int, length of update ('n' in n-step update).
-      gamma: int, the discount factor.
-      max_sample_attempts: int, the maximum number of attempts allowed to
-        get a sample.
+      gamma: float, the discount factor.
+      max_sample_attempts: int, the maximum number of attempts allowed to get a
+        sample.
       extra_storage_types: list of ReplayElements defining the type of the extra
         contents that will be stored and returned by sample_transition_batch.
       observation_dtype: np.dtype, type of the observations. Defaults to
         np.uint8 for Atari 2600.
       terminal_dtype: np.dtype, type of the terminals. Defaults to np.uint8 for
         Atari 2600.
       action_shape: tuple of ints, the shape for the action vector. Empty tuple
@@ -89,30 +92,32 @@
         max_sample_attempts=max_sample_attempts,
         extra_storage_types=extra_storage_types,
         observation_dtype=observation_dtype,
         terminal_dtype=terminal_dtype,
         action_shape=action_shape,
         action_dtype=action_dtype,
         reward_shape=reward_shape,
-        reward_dtype=reward_dtype)
+        reward_dtype=reward_dtype,
+    )
 
     self.sum_tree = sum_tree.SumTree(replay_capacity)
 
   def get_add_args_signature(self):
     """The signature of the add function.
 
     The signature is the same as the one for OutOfGraphReplayBuffer, with an
     added priority.
 
     Returns:
       list of ReplayElements defining the type of the argument signature needed
         by the add function.
     """
-    parent_add_signature = super(OutOfGraphPrioritizedReplayBuffer,
-                                 self).get_add_args_signature()
+    parent_add_signature = super(
+        OutOfGraphPrioritizedReplayBuffer, self
+    ).get_add_args_signature()
     add_signature = parent_add_signature + [
         ReplayElement('priority', (), np.float32)
     ]
     return add_signature
 
   def _add(self, *args):
     """Internal add method to add to the underlying memory arrays.
@@ -155,16 +160,18 @@
     indices = self.sum_tree.stratified_sample(batch_size)
     allowed_attempts = self._max_sample_attempts
     for i in range(len(indices)):
       if not self.is_valid_transition(indices[i]):
         if allowed_attempts == 0:
           raise RuntimeError(
               'Max sample attempts: Tried {} times but only sampled {}'
-              ' valid indices. Batch size is {}'.
-              format(self._max_sample_attempts, i, batch_size))
+              ' valid indices. Batch size is {}'.format(
+                  self._max_sample_attempts, i, batch_size
+              )
+          )
         index = indices[i]
         while not self.is_valid_transition(index) and allowed_attempts > 0:
           # If index i is not valid keep sampling others. Note that this
           # is not stratified.
           index = self.sum_tree.sample()
           allowed_attempts -= 1
         indices[i] = index
@@ -184,128 +191,136 @@
       indices: None or list of ints, the indices of every transition in the
         batch. If None, sample the indices uniformly.
 
     Returns:
       transition_batch: tuple of np.arrays with the shape and type as in
         get_transition_elements().
     """
-    transition = (super(OutOfGraphPrioritizedReplayBuffer, self).
-                  sample_transition_batch(batch_size, indices))
+    transition = super(
+        OutOfGraphPrioritizedReplayBuffer, self
+    ).sample_transition_batch(batch_size, indices)
     transition_elements = self.get_transition_elements(batch_size)
     transition_names = [e.name for e in transition_elements]
     probabilities_index = transition_names.index('sampling_probabilities')
     indices_index = transition_names.index('indices')
     indices = transition[indices_index]
     # The parent returned an empty array for the probabilities. Fill it with the
     # contents of the sum tree.
     transition[probabilities_index][:] = self.get_priority(indices)
     return transition
 
   def set_priority(self, indices, priorities):
     """Sets the priority of the given elements according to Schaul et al.
 
     Args:
-      indices: np.array with dtype int32, of indices in range
-        [0, replay_capacity).
+      indices: np.array with dtype int32, of indices in range [0,
+        replay_capacity).
       priorities: float, the corresponding priorities.
     """
-    assert indices.dtype == np.int32, ('Indices must be integers, '
-                                       'given: {}'.format(indices.dtype))
+    assert (
+        indices.dtype == np.int32
+    ), 'Indices must be integers, given: {}'.format(indices.dtype)
     # Convert JAX arrays to NumPy arrays first, since it is faster to iterate
     # over the entirety of a NumPy array than a JAX array.
     priorities = np.asarray(priorities)
     for index, priority in zip(indices, priorities):
       self.sum_tree.set(index, priority)
 
   def get_priority(self, indices):
     """Fetches the priorities correspond to a batch of memory indices.
 
     For any memory location not yet used, the corresponding priority is 0.
 
     Args:
-      indices: np.array with dtype int32, of indices in range
-        [0, replay_capacity).
+      indices: np.array with dtype int32, of indices in range [0,
+        replay_capacity).
 
     Returns:
       priorities: float, the corresponding priorities.
     """
     assert indices.shape, 'Indices must be an array.'
-    assert indices.dtype == np.int32, ('Indices must be int32s, '
-                                       'given: {}'.format(indices.dtype))
+    assert (
+        indices.dtype == np.int32
+    ), 'Indices must be int32s, given: {}'.format(indices.dtype)
     batch_size = len(indices)
     priority_batch = np.empty((batch_size), dtype=np.float32)
     for i, memory_index in enumerate(indices):
       priority_batch[i] = self.sum_tree.get(memory_index)
     return priority_batch
 
   def get_transition_elements(self, batch_size=None):
     """Returns a 'type signature' for sample_transition_batch.
 
     Args:
       batch_size: int, number of transitions returned. If None, the default
         batch_size will be used.
+
     Returns:
       signature: A namedtuple describing the method's return type signature.
     """
-    parent_transition_type = (
-        super(OutOfGraphPrioritizedReplayBuffer,
-              self).get_transition_elements(batch_size))
+    parent_transition_type = super(
+        OutOfGraphPrioritizedReplayBuffer, self
+    ).get_transition_elements(batch_size)
     probablilities_type = [
         ReplayElement('sampling_probabilities', (batch_size,), np.float32)
     ]
     return parent_transition_type + probablilities_type
 
 
 @gin.configurable(
-    denylist=['observation_shape', 'stack_size', 'update_horizon', 'gamma'])
+    denylist=['observation_shape', 'stack_size', 'update_horizon', 'gamma']
+)
 class WrappedPrioritizedReplayBuffer(
-    circular_replay_buffer.WrappedReplayBuffer):
+    circular_replay_buffer.WrappedReplayBuffer
+):
   """Wrapper of OutOfGraphPrioritizedReplayBuffer with in-graph sampling.
 
   Usage:
 
     * To add a transition:  Call the add function.
 
     * To sample a batch:  Query any of the tensors in the transition dictionary.
                           Every sess.run that requires any of these tensors will
                           sample a new transition.
   """
 
-  def __init__(self,
-               observation_shape,
-               stack_size,
-               use_staging=False,
-               replay_capacity=1000000,
-               batch_size=32,
-               update_horizon=1,
-               gamma=0.99,
-               wrapped_memory=None,
-               max_sample_attempts=1000,
-               extra_storage_types=None,
-               observation_dtype=np.uint8,
-               terminal_dtype=np.uint8,
-               action_shape=(),
-               action_dtype=np.int32,
-               reward_shape=(),
-               reward_dtype=np.float32):
+  def __init__(
+      self,
+      observation_shape,
+      stack_size,
+      use_staging=False,
+      replay_capacity=1000000,
+      batch_size=32,
+      update_horizon=1,
+      gamma=0.99,
+      wrapped_memory=None,
+      max_sample_attempts=1000,
+      extra_storage_types=None,
+      observation_dtype=np.uint8,
+      terminal_dtype=np.uint8,
+      action_shape=(),
+      action_dtype=np.int32,
+      reward_shape=(),
+      reward_dtype=np.float32,
+  ):
     """Initializes WrappedPrioritizedReplayBuffer.
 
     Args:
       observation_shape: tuple of ints.
       stack_size: int, number of frames to use in state stack.
-      use_staging: bool, when True it would use a staging area to prefetch
-        the next sampling batch.
+      use_staging: bool, when True it would use a staging area to prefetch the
+        next sampling batch.
       replay_capacity: int, number of transitions to keep in memory.
       batch_size: int.
       update_horizon: int, length of update ('n' in n-step update).
       gamma: int, the discount factor.
       wrapped_memory: The 'inner' memory data structure. If None, use the
         default prioritized replay.
-      max_sample_attempts: int, the maximum number of attempts allowed to
-        get a sample.
+      max_sample_attempts: int, the maximum number of attempts allowed to get a
+        sample.
       extra_storage_types: list of ReplayElements defining the type of the extra
         contents that will be stored and returned by sample_transition_batch.
       observation_dtype: np.dtype, type of the observations. Defaults to
         np.uint8 for Atari 2600.
       terminal_dtype: np.dtype, type of the terminals. Defaults to np.uint8 for
         Atari 2600.
       action_shape: tuple of ints, the shape for the action vector. Empty tuple
@@ -317,18 +332,24 @@
 
     Raises:
       ValueError: If update_horizon is not positive.
       ValueError: If discount factor is not in [0, 1].
     """
     if wrapped_memory is None:
       wrapped_memory = OutOfGraphPrioritizedReplayBuffer(
-          observation_shape, stack_size, replay_capacity, batch_size,
-          update_horizon, gamma, max_sample_attempts,
+          observation_shape,
+          stack_size,
+          replay_capacity,
+          batch_size,
+          update_horizon,
+          gamma,
+          max_sample_attempts,
           extra_storage_types=extra_storage_types,
-          observation_dtype=observation_dtype)
+          observation_dtype=observation_dtype,
+      )
 
     super(WrappedPrioritizedReplayBuffer, self).__init__(
         observation_shape,
         stack_size,
         use_staging,
         replay_capacity,
         batch_size,
@@ -337,37 +358,43 @@
         wrapped_memory=wrapped_memory,
         extra_storage_types=extra_storage_types,
         observation_dtype=observation_dtype,
         terminal_dtype=terminal_dtype,
         action_shape=action_shape,
         action_dtype=action_dtype,
         reward_shape=reward_shape,
-        reward_dtype=reward_dtype)
+        reward_dtype=reward_dtype,
+    )
 
   def tf_set_priority(self, indices, priorities):
     """Sets the priorities for the given indices.
 
     Args:
       indices: tf.Tensor with dtype int32 and shape [n].
       priorities: tf.Tensor with dtype float and shape [n].
 
     Returns:
        A tf op setting the priorities for prioritized sampling.
     """
     return tf.numpy_function(
-        self.memory.set_priority, [indices, priorities], [],
-        name='prioritized_replay_set_priority_py_func')
+        self.memory.set_priority,
+        [indices, priorities],
+        [],
+        name='prioritized_replay_set_priority_py_func',
+    )
 
   def tf_get_priority(self, indices):
     """Gets the priorities for the given indices.
 
     Args:
       indices: tf.Tensor with dtype int32 and shape [n].
 
     Returns:
       priorities: tf.Tensor with dtype float and shape [n], the priorities at
         the indices.
     """
     return tf.numpy_function(
-        self.memory.get_priority, [indices],
+        self.memory.get_priority,
+        [indices],
         tf.float32,
-        name='prioritized_replay_get_priority_py_func')
+        name='prioritized_replay_get_priority_py_func',
+    )
```

### Comparing `dopamine_rl-4.0.6/dopamine/replay_memory/sum_tree.py` & `dopamine_rl-4.0.7/dopamine/replay_memory/sum_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,17 @@
         data structure.
 
     Raises:
       ValueError: If requested capacity is not positive.
     """
     assert isinstance(capacity, int)
     if capacity <= 0:
-      raise ValueError('Sum tree capacity should be positive. Got: {}'.
-                       format(capacity))
+      raise ValueError(
+          'Sum tree capacity should be positive. Got: {}'.format(capacity)
+      )
 
     self.nodes = []
     tree_depth = int(math.ceil(np.log2(capacity)))
     level_size = 1
     for _ in range(tree_depth + 1):
       nodes_at_this_depth = np.zeros(level_size)
       self.nodes.append(nodes_at_this_depth)
@@ -99,28 +100,28 @@
   def sample(self, query_value=None):
     """Samples an element from the sum tree.
 
     Each element has probability p_i / sum_j p_j of being picked, where p_i is
     the (positive) value associated with node i (possibly unnormalized).
 
     Args:
-      query_value: float in [0, 1], used as the random value to select a
-      sample. If None, will select one randomly in [0, 1).
+      query_value: float in [0, 1], used as the random value to select a sample.
+        If None, will select one randomly in [0, 1).
 
     Returns:
       int, a random element from the sum tree.
 
     Raises:
       Exception: If the sum tree is empty (i.e. its node values sum to 0), or if
         the supplied query_value is larger than the total sum.
     """
     if self._total_priority() == 0.0:
       raise Exception('Cannot sample from an empty sum tree.')
 
-    if query_value and (query_value < 0. or query_value > 1.):
+    if query_value and (query_value < 0.0 or query_value > 1.0):
       raise ValueError('query_value must be in [0, 1].')
 
     # Sample a value in range [0, R), where R is the value stored at the root.
     query_value = random.random() if query_value is None else query_value
     query_value *= self._total_priority()
 
     # Now traverse the sum tree.
@@ -146,34 +147,36 @@
     Let R be the value at the root (total value of sum tree). This method will
     divide [0, R) into batch_size segments, pick a random number from each of
     those segments, and use that random number to sample from the sum_tree. This
     is as specified in Schaul et al. (2015).
 
     Args:
       batch_size: int, the number of strata to use.
+
     Returns:
       list of batch_size elements sampled from the sum tree.
 
     Raises:
       Exception: If the sum tree is empty (i.e. its node values sum to 0).
     """
     if self._total_priority() == 0.0:
       raise Exception('Cannot sample from an empty sum tree.')
 
-    bounds = np.linspace(0., 1., batch_size + 1)
+    bounds = np.linspace(0.0, 1.0, batch_size + 1)
     assert len(bounds) == batch_size + 1
-    segments = [(bounds[i], bounds[i+1]) for i in range(batch_size)]
+    segments = [(bounds[i], bounds[i + 1]) for i in range(batch_size)]
     query_values = [random.uniform(x[0], x[1]) for x in segments]
     return [self.sample(query_value=x) for x in query_values]
 
   def get(self, node_index):
     """Returns the value of the leaf node corresponding to the index.
 
     Args:
       node_index: The index of the leaf node.
+
     Returns:
       The value of the leaf node.
     """
     return self.nodes[-1][node_index]
 
   def set(self, node_index, value):
     """Sets the value of a leaf node and updates internal nodes accordingly.
@@ -185,21 +188,23 @@
         nonnegative. Setting value = 0 will cause the element to never be
         sampled.
 
     Raises:
       ValueError: If the given value is negative.
     """
     if value < 0.0:
-      raise ValueError('Sum tree values should be nonnegative. Got {}'.
-                       format(value))
+      raise ValueError(
+          'Sum tree values should be nonnegative. Got {}'.format(value)
+      )
     self.max_recorded_priority = max(value, self.max_recorded_priority)
 
     delta_value = value - self.nodes[-1][node_index]
 
     # Now traverse back the tree, adjusting all sums along the way.
     for nodes_at_this_depth in reversed(self.nodes):
       # Note: Adding a delta leads to some tolerable numerical inaccuracies.
       nodes_at_this_depth[node_index] += delta_value
       node_index //= 2
 
-    assert node_index == 0, ('Sum tree traversal failed, final node index '
-                             'is not 0.')
+    assert (
+        node_index == 0
+    ), 'Sum tree traversal failed, final node index is not 0.'
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/__init__.py` & `dopamine_rl-4.0.7/dopamine/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/agent_visualizer.py` & `dopamine_rl-4.0.7/dopamine/utils/agent_visualizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,32 +23,35 @@
 from __future__ import division
 from __future__ import print_function
 
 import os
 import subprocess
 
 
+
 import gin
 import numpy as np
 from PIL import Image
 import pygame
 
 
 @gin.configurable
 class AgentVisualizer(object):
   """Code to visualize an agent's behaviour."""
 
-  def __init__(self,
-               record_path,
-               plotters,
-               screen_width=160,
-               screen_height=210,
-               render_rate=1,
-               file_types=('png', ''),
-               filename_format='frame_{:06d}'):
+  def __init__(
+      self,
+      record_path,
+      plotters,
+      screen_width=160,
+      screen_height=210,
+      render_rate=1,
+      file_types=('png', ''),
+      filename_format='frame_{:06d}',
+  ):
     """Constructor for the AgentVisualizer class.
 
     This class generates a series of images built by a set of Plotters. These
     images are then saved to disk.
 
     It can optionally generate a video by concatenating all the images with
     ffmpeg.
@@ -66,48 +69,50 @@
     self.plotters = plotters
     self.screen_width = screen_width
     self.screen_height = screen_height
     self.render_rate = render_rate
     self.file_types = file_types
     self.filename_format = filename_format
     self.step = 0
-    self.record_frame = np.zeros((self.screen_height, self.screen_width, 3),
-                                 dtype=np.uint8)
+    self.record_frame = np.zeros(
+        (self.screen_height, self.screen_width, 3), dtype=np.uint8
+    )
     # This is necessary to avoid a `pygame.error: No available video device`
     # error.
     os.environ['SDL_VIDEODRIVER'] = 'dummy'
     pygame.init()
-    self.screen = pygame.display.set_mode((self.screen_width,
-                                           self.screen_height),
-                                          0, 32)
+    self.screen = pygame.display.set_mode(
+        (self.screen_width, self.screen_height), 0, 32
+    )
 
   def visualize(self):
     if self.step % self.render_rate == 0:
       self.screen.fill((0, 0, 0))
       for plotter in self.plotters:
         self.screen = self.screen.copy()  # To avoid locked Surfaces issue.
         self.screen.blit(plotter.draw(), (plotter.x, plotter.y))
       self.save_frame()
     self.step += 1
 
   def save_frame(self):
     """Save a frame to disk and generate a video, if enabled."""
-    screen_buffer = (
-        np.frombuffer(self.screen.get_buffer(), dtype=np.int32)
-        .reshape(self.screen_height, self.screen_width))
-    sb = screen_buffer[:, 0:self.screen_width]
+    screen_buffer = np.frombuffer(
+        self.screen.get_buffer(), dtype=np.int32
+    ).reshape(self.screen_height, self.screen_width)
+    sb = screen_buffer[:, 0 : self.screen_width]
     self.record_frame[..., 2] = sb % 256
     self.record_frame[..., 1] = (sb >> 8) % 256
     self.record_frame[..., 0] = (sb >> 16) % 256
     frame_number = self.step // self.render_rate
     for file_type in self.file_types:
       if not file_type:
         continue
-      filename = (
-          self.filename_format.format(frame_number) + '.{}'.format(file_type))
+      filename = self.filename_format.format(frame_number) + '.{}'.format(
+          file_type
+      )
       im = Image.fromarray(self.record_frame)
       im.save(os.path.join(self.record_path, filename))
 
   def generate_video(self, video_file='video.mp4'):
     """Generates a video, requires 'png' be in file_types.
 
     Note that this will issue a `subprocess.call` to `ffmpeg`, so only use this
@@ -117,10 +122,25 @@
       video_file: str, name of video file to generate.
     """
     if 'png' not in self.file_types:
       return
     os.chdir(self.record_path)
     file_regex = self.filename_format.replace('{:', '%').replace('}', '')
     file_regex += '.png'
-    subprocess.call(['ffmpeg', '-r', '30', '-f', 'image2', '-s', '1920x1080',
-                     '-i', file_regex, '-vcodec', 'libx264', '-crf', '25',
-                     '-pix_fmt', 'yuv420p', video_file])
+    subprocess.call([
+        'ffmpeg',
+        '-r',
+        '30',
+        '-f',
+        'image2',
+        '-s',
+        '1920x1080',
+        '-i',
+        file_regex,
+        '-vcodec',
+        'libx264',
+        '-crf',
+        '25',
+        '-pix_fmt',
+        'yuv420p',
+        video_file,
+    ])
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/atari_plotter.py` & `dopamine_rl-4.0.7/dopamine/utils/atari_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""AtariPlotter used for rendering Atari 2600 frames.
-"""
+"""AtariPlotter used for rendering Atari 2600 frames."""
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 
+
 from dopamine.utils import plotter
 import gin
 import numpy as np
 import pygame
 
 
 @gin.configurable
@@ -39,32 +39,34 @@
   }
 
   def __init__(self, parameter_dict=None):
     """Constructor for AtariPlotter.
 
     Args:
       parameter_dict: None or dict of parameter specifications for
-        visualization. If an expected parameter is present, its value will
-        be used, otherwise it will use defaults.
+        visualization. If an expected parameter is present, its value will be
+        used, otherwise it will use defaults.
     """
     super(AtariPlotter, self).__init__(parameter_dict)
     assert 'environment' in self.parameters
-    self.game_surface = pygame.Surface((self.parameters['input_width'],
-                                        self.parameters['input_height']))
+    self.game_surface = pygame.Surface(
+        (self.parameters['input_width'], self.parameters['input_height'])
+    )
 
   def draw(self):
     """Render the Atari 2600 frame.
 
     Returns:
       object to be rendered by AgentVisualizer.
     """
     environment = self.parameters['environment']
-    numpy_surface = np.frombuffer(self.game_surface.get_buffer(),
-                                  dtype=np.int32)
+    numpy_surface = np.frombuffer(
+        self.game_surface.get_buffer(), dtype=np.int32
+    )
     obs = environment.render(mode='rgb_array').astype(np.int32)
     obs = np.transpose(obs)
     obs = np.swapaxes(obs, 1, 2)
     obs = obs[2] | (obs[1] << 8) | (obs[0] << 16)
     np.copyto(numpy_surface, obs.ravel())
-    return pygame.transform.scale(self.game_surface,
-                                  (self.parameters['width'],
-                                   self.parameters['height']))
+    return pygame.transform.scale(
+        self.game_surface, (self.parameters['width'], self.parameters['height'])
+    )
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/bar_plotter.py` & `dopamine_rl-4.0.7/dopamine/utils/bar_plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 this should be a non-issue.
 """
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 
+
 from dopamine.utils import plotter
 import gin
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pygame
 
@@ -47,31 +48,33 @@
       'height': 210,
       'fontsize': 30,
       'bg_color': '#f8f7f2',
       'face_color': '#ffffff',
       'colors': COLORS,
       'max_width': 500,
       'figsize': (12, 9),
-      'font': {'family': 'Bitstream Vera Sans',
-               'weight': 'regular',
-               'size': 26},
+      'font': {
+          'family': 'Bitstream Vera Sans',
+          'weight': 'regular',
+          'size': 26,
+      },
   }
 
   def __init__(self, parameter_dict=None):
     """Constructor for BarPlotter.
 
     This expects a callable 'get_bar_data_fn' in the parameters, which will
     return a list of distributions for each of the actions.  Typically, this
     will be a callback from the agent, which will return some useful information
     about its performance.
 
     Args:
       parameter_dict: None or dict of parameter specifications for
-        visualization. If an expected parameter is present, its value will
-        be used, otherwise it will use defaults.
+        visualization. If an expected parameter is present, its value will be
+        used, otherwise it will use defaults.
     """
     super(BarPlotter, self).__init__(parameter_dict)
     assert 'get_bar_data_fn' in self.parameters
     self.fig = plt.figure(frameon=False, figsize=self.parameters['figsize'])
     self.plot = self.fig.add_subplot(111)
     self.plot_surface = None
     # This sets the font used by the plotter to be the desired font.
@@ -87,23 +90,25 @@
       object to be rendered by AgentVisualizer.
     """
     self._setup_plot()
     num_colors = len(self.parameters['colors'])
     bar_data = self.parameters['get_bar_data_fn']()
     num_actions, num_bins = bar_data.shape
     for i in range(num_actions):
-      self.plot.bar(np.arange(num_bins), bar_data[i],
-                    color=self.parameters['colors'][i % num_colors])
+      self.plot.bar(
+          np.arange(num_bins),
+          bar_data[i],
+          color=self.parameters['colors'][i % num_colors],
+      )
     if 'legend' in self.parameters:
       self.plot.legend(self.parameters['legend'])
     self.fig.canvas.draw()
     # Now transfer to surface.
     width, height = self.fig.canvas.get_width_height()
     if self.plot_surface is None:
       self.plot_surface = pygame.Surface((width, height))
     plot_buffer = np.frombuffer(self.fig.canvas.buffer_rgba(), np.uint32)
-    surf_buffer = np.frombuffer(self.plot_surface.get_buffer(),
-                                dtype=np.int32)
+    surf_buffer = np.frombuffer(self.plot_surface.get_buffer(), dtype=np.int32)
     np.copyto(surf_buffer, plot_buffer)
     return pygame.transform.smoothscale(
-        self.plot_surface,
-        (self.parameters['width'], self.parameters['height']))
+        self.plot_surface, (self.parameters['width'], self.parameters['height'])
+    )
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/example_viz.py` & `dopamine_rl-4.0.7/dopamine/utils/example_viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,34 +37,41 @@
 """
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 
+
 from absl import app
 from absl import flags
 from dopamine.utils import example_viz_lib
 
 flags.DEFINE_string('agent', 'dqn', 'Agent to visualize.')
 flags.DEFINE_string('game', 'Breakout', 'Game to visualize.')
 flags.DEFINE_string('root_dir', '/tmp/dopamine/', 'Root directory.')
-flags.DEFINE_string('restore_checkpoint', None,
-                    'Path to checkpoint to restore for visualizing.')
+flags.DEFINE_string(
+    'restore_checkpoint', None, 'Path to checkpoint to restore for visualizing.'
+)
 flags.DEFINE_integer('num_steps', 2000, 'Number of steps to run.')
 flags.DEFINE_boolean(
-    'use_legacy_checkpoint', False,
-    'Set to true if loading from a legacy (pre-Keras) checkpoint.')
+    'use_legacy_checkpoint',
+    False,
+    'Set to true if loading from a legacy (pre-Keras) checkpoint.',
+)
 
 FLAGS = flags.FLAGS
 
 
 def main(_):
-  example_viz_lib.run(agent=FLAGS.agent,
-                      game=FLAGS.game,
-                      num_steps=FLAGS.num_steps,
-                      root_dir=FLAGS.root_dir,
-                      restore_ckpt=FLAGS.restore_checkpoint,
-                      use_legacy_checkpoint=FLAGS.use_legacy_checkpoint)
+  example_viz_lib.run(
+      agent=FLAGS.agent,
+      game=FLAGS.game,
+      num_steps=FLAGS.num_steps,
+      root_dir=FLAGS.root_dir,
+      restore_ckpt=FLAGS.restore_checkpoint,
+      use_legacy_checkpoint=FLAGS.use_legacy_checkpoint,
+  )
+
 
 if __name__ == '__main__':
   app.run(main)
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/example_viz_lib.py` & `dopamine_rl-4.0.7/dopamine/utils/example_viz_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,44 +48,48 @@
 import tf_slim
 
 
 class MyDQNAgent(dqn_agent.DQNAgent):
   """Sample DQN agent to visualize Q-values and rewards."""
 
   def __init__(self, sess, num_actions, summary_writer=None):
-    super(MyDQNAgent, self).__init__(sess, num_actions,
-                                     summary_writer=summary_writer)
+    super(MyDQNAgent, self).__init__(
+        sess, num_actions, summary_writer=summary_writer
+    )
     self.q_values = [[] for _ in range(num_actions)]
     self.rewards = []
 
   def step(self, reward, observation):
     self.rewards.append(reward)
     return super(MyDQNAgent, self).step(reward, observation)
 
   def _select_action(self):
     action = super(MyDQNAgent, self)._select_action()
-    q_vals = self._sess.run(self._net_outputs.q_values,
-                            {self.state_ph: self.state})[0]
+    q_vals = self._sess.run(
+        self._net_outputs.q_values, {self.state_ph: self.state}
+    )[0]
     for i in range(len(q_vals)):
       self.q_values[i].append(q_vals[i])
     return action
 
   def reload_checkpoint(self, checkpoint_path, use_legacy_checkpoint=False):
     if use_legacy_checkpoint:
       variables_to_restore = atari_lib.maybe_transform_variable_names(
-          tf.compat.v1.global_variables(), legacy_checkpoint_load=True)
+          tf.compat.v1.global_variables(), legacy_checkpoint_load=True
+      )
     else:
       global_vars = set([x.name for x in tf.compat.v1.global_variables()])
       ckpt_vars = [
           '{}:0'.format(name)
           for name, _ in tf.train.list_variables(checkpoint_path)
       ]
       include_vars = list(global_vars.intersection(set(ckpt_vars)))
       variables_to_restore = tf_slim.get_variables_to_restore(
-          include=include_vars)
+          include=include_vars
+      )
     if variables_to_restore:
       reloader = tf.compat.v1.train.Saver(var_list=variables_to_restore)
       reloader.restore(self._sess, checkpoint_path)
       logging.info('Done restoring from %s', checkpoint_path)
     else:
       logging.info('Nothing to restore!')
 
@@ -96,62 +100,72 @@
     return [np.cumsum(self.rewards)]
 
 
 class MyRainbowAgent(rainbow_agent.RainbowAgent):
   """Sample Rainbow agent to visualize Q-values and rewards."""
 
   def __init__(self, sess, num_actions, summary_writer=None):
-    super(MyRainbowAgent, self).__init__(sess, num_actions,
-                                         summary_writer=summary_writer)
+    super(MyRainbowAgent, self).__init__(
+        sess, num_actions, summary_writer=summary_writer
+    )
     self.rewards = []
 
   def step(self, reward, observation):
     self.rewards.append(reward)
     return super(MyRainbowAgent, self).step(reward, observation)
 
   def reload_checkpoint(self, checkpoint_path, use_legacy_checkpoint=False):
     if use_legacy_checkpoint:
       variables_to_restore = atari_lib.maybe_transform_variable_names(
-          tf.compat.v1.global_variables(), legacy_checkpoint_load=True)
+          tf.compat.v1.global_variables(), legacy_checkpoint_load=True
+      )
     else:
       global_vars = set([x.name for x in tf.compat.v1.global_variables()])
       ckpt_vars = [
           '{}:0'.format(name)
           for name, _ in tf.train.list_variables(checkpoint_path)
       ]
       include_vars = list(global_vars.intersection(set(ckpt_vars)))
       variables_to_restore = tf_slim.get_variables_to_restore(
-          include=include_vars)
+          include=include_vars
+      )
     if variables_to_restore:
       reloader = tf.compat.v1.train.Saver(var_list=variables_to_restore)
       reloader.restore(self._sess, checkpoint_path)
       logging.info('Done restoring from %s', checkpoint_path)
     else:
       logging.info('Nothing to restore!')
 
   def get_probabilities(self):
-    return self._sess.run(tf.squeeze(self._net_outputs.probabilities),
-                          {self.state_ph: self.state})
+    return self._sess.run(
+        tf.squeeze(self._net_outputs.probabilities), {self.state_ph: self.state}
+    )
 
   def get_rewards(self):
     return [np.cumsum(self.rewards)]
 
 
 class MyRunner(run_experiment.Runner):
   """Sample Runner class to generate visualizations."""
 
-  def __init__(self, base_dir, trained_agent_ckpt_path, create_agent_fn,
-               use_legacy_checkpoint=False):
+  def __init__(
+      self,
+      base_dir,
+      trained_agent_ckpt_path,
+      create_agent_fn,
+      use_legacy_checkpoint=False,
+  ):
     self._trained_agent_ckpt_path = trained_agent_ckpt_path
     self._use_legacy_checkpoint = use_legacy_checkpoint
     super(MyRunner, self).__init__(base_dir, create_agent_fn)
 
   def _initialize_checkpointer_and_maybe_resume(self, checkpoint_file_prefix):
-    self._agent.reload_checkpoint(self._trained_agent_ckpt_path,
-                                  self._use_legacy_checkpoint)
+    self._agent.reload_checkpoint(
+        self._trained_agent_ckpt_path, self._use_legacy_checkpoint
+    )
     self._start_iteration = 0
 
   def _run_one_iteration(self, iteration):
     statistics = iteration_statistics.IterationStatistics()
     logging.info('Starting iteration %d', iteration)
     _, _ = self._run_eval_phase(statistics)
     return statistics.data_lists
@@ -161,26 +175,31 @@
       tf.io.gfile.makedirs(record_path)
     self._agent.eval_mode = True
 
     # Set up the game playback rendering.
     atari_params = {'environment': self._environment}
     atari_plot = atari_plotter.AtariPlotter(parameter_dict=atari_params)
     # Plot the rewards received next to it.
-    reward_params = {'x': atari_plot.parameters['width'],
-                     'xlabel': 'Timestep',
-                     'ylabel': 'Reward',
-                     'title': 'Rewards',
-                     'get_line_data_fn': self._agent.get_rewards}
+    reward_params = {
+        'x': atari_plot.parameters['width'],
+        'xlabel': 'Timestep',
+        'ylabel': 'Reward',
+        'title': 'Rewards',
+        'get_line_data_fn': self._agent.get_rewards,
+    }
     reward_plot = line_plotter.LinePlotter(parameter_dict=reward_params)
     action_names = [
-        'Action {}'.format(x) for x in range(self._agent.num_actions)]
+        'Action {}'.format(x) for x in range(self._agent.num_actions)
+    ]
     # Plot Q-values (DQN) or Q-value distributions (Rainbow).
-    q_params = {'x': atari_plot.parameters['width'] // 2,
-                'y': atari_plot.parameters['height'],
-                'legend': action_names}
+    q_params = {
+        'x': atari_plot.parameters['width'] // 2,
+        'y': atari_plot.parameters['height'],
+        'legend': action_names,
+    }
     if 'DQN' in self._agent.__class__.__name__:
       q_params['xlabel'] = 'Timestep'
       q_params['ylabel'] = 'Q-Value'
       q_params['title'] = 'Q-Values'
       q_params['get_line_data_fn'] = self._agent.get_q_values
       q_plot = line_plotter.LinePlotter(parameter_dict=q_params)
     elif 'Implicit' in self._agent.__class__.__name__:
@@ -192,25 +211,30 @@
     else:
       q_params['xlabel'] = 'Return'
       q_params['ylabel'] = 'Return probability'
       q_params['title'] = 'Return distribution'
       q_params['get_bar_data_fn'] = self._agent.get_probabilities
       q_plot = bar_plotter.BarPlotter(parameter_dict=q_params)
     screen_width = (
-        atari_plot.parameters['width'] + reward_plot.parameters['width'])
+        atari_plot.parameters['width'] + reward_plot.parameters['width']
+    )
     screen_height = (
-        atari_plot.parameters['height'] + q_plot.parameters['height'])
+        atari_plot.parameters['height'] + q_plot.parameters['height']
+    )
     # Dimensions need to be divisible by 2:
     if screen_width % 2 > 0:
       screen_width += 1
     if screen_height % 2 > 0:
       screen_height += 1
     visualizer = agent_visualizer.AgentVisualizer(
-        record_path=record_path, plotters=[atari_plot, reward_plot, q_plot],
-        screen_width=screen_width, screen_height=screen_height)
+        record_path=record_path,
+        plotters=[atari_plot, reward_plot, q_plot],
+        screen_width=screen_width,
+        screen_height=screen_height,
+    )
     global_step = 0
     while global_step < num_global_steps:
       initial_observation = self._environment.reset()
       action = self._agent.begin_episode(initial_observation)
       while True:
         observation, reward, is_terminal, _ = self._environment.step(action)
         global_step += 1
@@ -223,32 +247,41 @@
         else:
           action = self._agent.step(reward, observation)
       self._end_episode(reward)
     visualizer.generate_video()
 
 
 def create_dqn_agent(sess, environment, summary_writer=None):
-  return MyDQNAgent(sess, num_actions=environment.action_space.n,
-                    summary_writer=summary_writer)
+  return MyDQNAgent(
+      sess,
+      num_actions=environment.action_space.n,
+      summary_writer=summary_writer,
+  )
 
 
 def create_rainbow_agent(sess, environment, summary_writer=None):
-  return MyRainbowAgent(sess, num_actions=environment.action_space.n,
-                        summary_writer=summary_writer)
+  return MyRainbowAgent(
+      sess,
+      num_actions=environment.action_space.n,
+      summary_writer=summary_writer,
+  )
 
 
-def create_runner(base_dir, trained_agent_ckpt_path, agent='dqn',
-                  use_legacy_checkpoint=False):
+def create_runner(
+    base_dir, trained_agent_ckpt_path, agent='dqn', use_legacy_checkpoint=False
+):
   create_agent = create_dqn_agent if agent == 'dqn' else create_rainbow_agent
-  return MyRunner(base_dir, trained_agent_ckpt_path, create_agent,
-                  use_legacy_checkpoint)
+  return MyRunner(
+      base_dir, trained_agent_ckpt_path, create_agent, use_legacy_checkpoint
+  )
 
 
-def run(agent, game, num_steps, root_dir, restore_ckpt,
-        use_legacy_checkpoint=False):
+def run(
+    agent, game, num_steps, root_dir, restore_ckpt, use_legacy_checkpoint=False
+):
   """Main entrypoint for running and generating visualizations.
 
   Args:
     agent: str, agent type to use.
     game: str, Atari 2600 game to run.
     num_steps: int, number of steps to play game.
     root_dir: str, root directory where files will be stored.
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/line_plotter.py` & `dopamine_rl-4.0.7/dopamine/utils/line_plotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 this should be a non-issue.
 """
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 
+
 from dopamine.utils import plotter
 import gin
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pygame
 
@@ -47,32 +48,34 @@
       'height': 210,
       'fontsize': 30,
       'bg_color': '#f8f7f2',
       'face_color': '#ffffff',
       'colors': COLORS,
       'max_width': 500,
       'figsize': (12, 9),
-      'font': {'family': 'Bitstream Vera Sans',
-               'weight': 'regular',
-               'size': 26},
+      'font': {
+          'family': 'Bitstream Vera Sans',
+          'weight': 'regular',
+          'size': 26,
+      },
       'linewidth': 5,
   }
 
   def __init__(self, parameter_dict=None):
     """Constructor for LinePlotter.
 
     This expects a callable 'get_line_data_fn' in the parameters, which
     will return a list of list of floats, each one representing a line
     to be drawn. Typically, this will be a callback from the agent,
     which will return some useful information about its performance.
 
     Args:
       parameter_dict: None or dict of parameter specifications for
-        visualization. If an expected parameter is present, its value will
-        be used, otherwise it will use defaults.
+        visualization. If an expected parameter is present, its value will be
+        used, otherwise it will use defaults.
     """
     super(LinePlotter, self).__init__(parameter_dict)
     assert 'get_line_data_fn' in self.parameters
     self.fig = plt.figure(frameon=False, figsize=self.parameters['figsize'])
     self.plot = self.fig.add_subplot(111)
     self.plot_surface = None
     matplotlib.rc('font', **self.parameters['font'])
@@ -87,27 +90,28 @@
       object to be rendered by AgentVisualizer.
     """
     self._setup_plot()
     num_colors = len(self.parameters['colors'])
     max_xlim = 0
     line_data = self.parameters['get_line_data_fn']()
     for i in range(len(line_data)):
-      self.plot.plot(line_data[i],
-                     linewidth=self.parameters['linewidth'],
-                     color=self.parameters['colors'][i % num_colors])
+      self.plot.plot(
+          line_data[i],
+          linewidth=self.parameters['linewidth'],
+          color=self.parameters['colors'][i % num_colors],
+      )
       max_xlim = max(max_xlim, len(line_data[i]))
     min_xlim = max(0, max_xlim - self.parameters['max_width'])
     self.plot.set_xlim(min_xlim, max_xlim)
     if 'legend' in self.parameters:
       self.plot.legend(self.parameters['legend'])
     self.fig.canvas.draw()
     # Now transfer to surface.
     width, height = self.fig.canvas.get_width_height()
     if self.plot_surface is None:
       self.plot_surface = pygame.Surface((width, height))
     plot_buffer = np.frombuffer(self.fig.canvas.buffer_rgba(), np.uint32)
-    surf_buffer = np.frombuffer(self.plot_surface.get_buffer(),
-                                dtype=np.int32)
+    surf_buffer = np.frombuffer(self.plot_surface.get_buffer(), dtype=np.int32)
     np.copyto(surf_buffer, plot_buffer)
     return pygame.transform.smoothscale(
-        self.plot_surface,
-        (self.parameters['width'], self.parameters['height']))
+        self.plot_surface, (self.parameters['width'], self.parameters['height'])
+    )
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/plotter.py` & `dopamine_rl-4.0.7/dopamine/utils/plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,49 +27,53 @@
 from __future__ import print_function
 
 import abc
 
 
 class Plotter(object):
   """Abstract base class for plotters."""
+
   __metaclass__ = abc.ABCMeta
 
   def __init__(self, parameter_dict=None):
     """Constructor for a Plotter, each child class must define _defaults.
 
     It will ensure there are values for 'x' and 'y' in `self.parameters`. The
     other key/values will come from either `parameter_dict` or, if not specified
     there, from `self._defaults`.
 
     Args:
       parameter_dict: None or dict of parameter specifications for
-        visualization. If an expected parameter is present, its value will
-        be used, otherwise it will use defaults.
+        visualization. If an expected parameter is present, its value will be
+        used, otherwise it will use defaults.
     """
     self.parameters = {'x': 0, 'y': 0}
     self.parameters.update(self._defaults)
     self.parameters.update(parameter_dict)
 
   def _setup_plot(self):
     """Helpful common functionality when rendering matplotlib-style plots."""
     self.plot.cla()  # Clear current figure.
     self.fig.patch.set_facecolor(self.parameters['face_color'])
     try:
       self.plot.set_facecolor(self.parameters['bg_color'])
     except AttributeError:
       self.plot.set_axis_bgcolor(self.parameters['bg_color'])
     if 'xlabel' in self.parameters:
-      self.plot.set_xlabel(self.parameters['xlabel'],
-                           fontsize=self.parameters['fontsize'] - 2)
+      self.plot.set_xlabel(
+          self.parameters['xlabel'], fontsize=self.parameters['fontsize'] - 2
+      )
     if 'ylabel' in self.parameters:
-      self.plot.set_ylabel(self.parameters['ylabel'],
-                           fontsize=self.parameters['fontsize'] - 2)
+      self.plot.set_ylabel(
+          self.parameters['ylabel'], fontsize=self.parameters['fontsize'] - 2
+      )
     if 'title' in self.parameters:
-      self.plot.set_title(self.parameters['title'],
-                          fontsize=self.parameters['fontsize'] + 2)
+      self.plot.set_title(
+          self.parameters['title'], fontsize=self.parameters['fontsize'] + 2
+      )
     if 'xticks' in self.parameters:
       self.plot.set_xticks(self.parameters['xticks'])
     if 'xticklabels' in self.parameters:
       self.plot.set_xticklabels(self.parameters['xticklabels'])
 
     self.plot.tick_params(labelsize=self.parameters['fontsize'])
```

### Comparing `dopamine_rl-4.0.6/dopamine/utils/test_utils.py` & `dopamine_rl-4.0.7/dopamine/utils/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,11 +30,12 @@
   def __init__(self, is_jax=False):
     if is_jax:
       self.add = mock.Mock()
       self.add_count = 0
       self.sum_tree = mock.Mock()
     else:
       with tf.compat.v1.variable_scope(
-          'MockReplayBuffer', reuse=tf.compat.v1.AUTO_REUSE):
+          'MockReplayBuffer', reuse=tf.compat.v1.AUTO_REUSE
+      ):
         self.add = mock.Mock()
         self.memory = mock.Mock()
         self.memory.add_count = 0
```

### Comparing `dopamine_rl-4.0.6/dopamine_rl.egg-info/PKG-INFO` & `dopamine_rl-4.0.7/dopamine_rl.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: dopamine-rl
-Version: 4.0.6
+Name: dopamine_rl
+Version: 4.0.7
 Summary: Dopamine: A framework for flexible Reinforcement Learning research
 Home-page: https://github.com/google/dopamine
 Author: The Dopamine Team
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/dopamine
 Project-URL: Bug Reports, https://github.com/google/dopamine/issues
 Project-URL: Source, https://github.com/google/dopamine
 Keywords: dopamine,reinforcement,machine,learning,research
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -27,14 +26,29 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: tensorflow>=2.2.0
+Requires-Dist: gin-config>=0.3.0
+Requires-Dist: absl-py>=0.9.0
+Requires-Dist: opencv-python>=3.4.8.29
+Requires-Dist: gym<=0.25.2
+Requires-Dist: flax>=0.2.0
+Requires-Dist: jax>=0.1.72
+Requires-Dist: jaxlib>=0.1.51
+Requires-Dist: Pillow>=7.0.0
+Requires-Dist: numpy>=1.16.4
+Requires-Dist: pygame>=1.9.2
+Requires-Dist: pandas>=0.24.2
+Requires-Dist: tf_slim>=1.0
+Requires-Dist: tensorflow-probability>=0.13.0
+Requires-Dist: tqdm>=4.64.1
 
 # Dopamine
 [Getting Started](#getting-started) |
 [Docs][docs] |
 [Baseline Results][baselines] |
 [Changelist](https://google.github.io/dopamine/docs/changelist)
 
@@ -204,9 +218,7 @@
 [prioritized_replay]: https://arxiv.org/abs/1511.05952
 [c51]: http://proceedings.mlr.press/v70/bellemare17a.html
 [rainbow]: https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/download/17204/16680
 [iqn]: https://arxiv.org/abs/1806.06923
 [sac]: https://arxiv.org/abs/1812.05905
 [dopamine_paper]: https://arxiv.org/abs/1812.06110
 [vitualenv]: https://docs.python.org/3/library/venv.html#creating-virtual-environments
-
-
```

### Comparing `dopamine_rl-4.0.6/dopamine_rl.egg-info/SOURCES.txt` & `dopamine_rl-4.0.7/dopamine_rl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,19 @@
 dopamine/jax/agents/rainbow/__init__.py
 dopamine/jax/agents/rainbow/rainbow_agent.py
 dopamine/jax/agents/sac/__init__.py
 dopamine/jax/agents/sac/sac_agent.py
 dopamine/labs/__init__.py
 dopamine/labs/atari_100k/__init__.py
 dopamine/labs/atari_100k/atari_100k_rainbow_agent.py
+dopamine/labs/atari_100k/atari_100k_runner.py
 dopamine/labs/atari_100k/eval_run_experiment.py
+dopamine/labs/atari_100k/normalization_utils.py
+dopamine/labs/atari_100k/spr_agent.py
+dopamine/labs/atari_100k/spr_networks.py
 dopamine/labs/atari_100k/train.py
 dopamine/labs/environments/__init__.py
 dopamine/labs/environments/brax/__init__.py
 dopamine/labs/environments/brax/brax_lib.py
 dopamine/labs/environments/brax/train.py
 dopamine/labs/environments/minatar/__init__.py
 dopamine/labs/environments/minatar/minatar_env.py
```

### Comparing `dopamine_rl-4.0.6/setup.py` & `dopamine_rl-4.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,50 +38,47 @@
     'jaxlib >= 0.1.51',
     'Pillow >= 7.0.0',
     'numpy >= 1.16.4',
     'pygame >= 1.9.2',
     'pandas >= 0.24.2',
     'tf_slim >= 1.0',
     'tensorflow-probability >= 0.13.0',
+    'tqdm >= 4.64.1',
 ]
 
 dopamine_description = (
-    'Dopamine: A framework for flexible Reinforcement Learning research')
+    'Dopamine: A framework for flexible Reinforcement Learning research'
+)
 
 setup(
     name='dopamine_rl',
-    version='4.0.6',
+    version='4.0.7',
     description=dopamine_description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/google/dopamine',
     author='The Dopamine Team',
     classifiers=[
         'Development Status :: 4 - Beta',
-
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
-
         'License :: OSI Approved :: Apache Software License',
-
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3 :: Only',
-
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
-
     ],
     keywords='dopamine, reinforcement, machine, learning, research',
     include_package_data=True,
     packages=find_packages(exclude=['docs']),
     package_data={'testdata': ['testdata/*.gin']},
     install_requires=install_requires,
     python_requires='>=3.5,<4',
```

