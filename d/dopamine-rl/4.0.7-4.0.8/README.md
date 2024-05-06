# Comparing `tmp/dopamine_rl-4.0.7.tar.gz` & `tmp/dopamine_rl-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dopamine_rl-4.0.7.tar", last modified: Mon May  6 16:58:41 2024, max compression
+gzip compressed data, was "dopamine_rl-4.0.8.tar", last modified: Mon May  6 19:45:22 2024, max compression
```

## Comparing `dopamine_rl-4.0.7.tar` & `dopamine_rl-4.0.8.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.708882 dopamine_rl-4.0.7/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      298 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/AUTHORS
--rw-r--r--   0 psc      (160661) primarygroup (89939)    11417 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/LICENSE
--rw-r--r--   0 psc      (160661) primarygroup (89939)     8009 2024-05-06 16:58:41.708598 dopamine_rl-4.0.7/PKG-INFO
--rw-r--r--   0 psc      (160661) primarygroup (89939)     6073 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/README.md
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.690804 dopamine_rl-4.0.7/dopamine/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      619 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.690983 dopamine_rl-4.0.7/dopamine/agents/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.691371 dopamine_rl-4.0.7/dopamine/agents/dqn/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/dqn/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    22347 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.691800 dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    13888 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/implicit_quantile_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.692258 dopamine_rl-4.0.7/dopamine/agents/rainbow/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/rainbow/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    21212 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/agents/rainbow/rainbow_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.692681 dopamine_rl-4.0.7/dopamine/colab/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/colab/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    10872 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/colab/utils.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.693321 dopamine_rl-4.0.7/dopamine/continuous_domains/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/continuous_domains/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    11032 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/continuous_domains/run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1675 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/continuous_domains/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.695464 dopamine_rl-4.0.7/dopamine/discrete_domains/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    20405 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/atari_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     7830 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/checkpointer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    15458 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/gym_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1645 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/iteration_statistics.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     8414 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/legacy_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/logger.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    29226 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1782 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/discrete_domains/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.696331 dopamine_rl-4.0.7/dopamine/jax/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.696529 dopamine_rl-4.0.7/dopamine/jax/agents/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.696885 dopamine_rl-4.0.7/dopamine/jax/agents/dqn/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/dqn/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    25694 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.697274 dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    17438 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.697693 dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    19224 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.698068 dopamine_rl-4.0.7/dopamine/jax/agents/quantile/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/quantile/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    12771 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/quantile/quantile_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.698482 dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    20026 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/rainbow_agent.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.698842 dopamine_rl-4.0.7/dopamine/jax/agents/sac/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/sac/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    25998 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/agents/sac/sac_agent.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     7293 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/continuous_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1670 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/losses.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    19671 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/jax/networks.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.699097 dopamine_rl-4.0.7/dopamine/labs/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.700581 dopamine_rl-4.0.7/dopamine/labs/atari_100k/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    12279 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/atari_100k_rainbow_agent.py
--rwxr-xr-x   0 psc      (160661) primarygroup (89939)    21090 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/atari_100k_runner.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     4783 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/eval_run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3546 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/normalization_utils.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    16018 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/spr_agent.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    14871 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/spr_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3664 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/atari_100k/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.700731 dopamine_rl-4.0.7/dopamine/labs/environments/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/__init__.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.701198 dopamine_rl-4.0.7/dopamine/labs/environments/brax/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/brax/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3858 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/brax/brax_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1705 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/brax/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.701641 dopamine_rl-4.0.7/dopamine/labs/environments/minatar/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/minatar/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     5406 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/environments/minatar/minatar_env.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.702476 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     5615 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/continuous_networks.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     7070 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/deepmind_control_lib.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.703445 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    10357 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/run_experiment.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    11705 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/tandem_dqn_agent.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1921 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/train.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.704591 dopamine_rl-4.0.7/dopamine/metrics/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2337 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/collector.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3683 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/collector_dispatcher.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2023 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/console_collector.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2054 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/pickle_collector.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)      870 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/statistics_instance.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1592 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/metrics/tensorboard_collector.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.705347 dopamine_rl-4.0.7/dopamine/replay_memory/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    38593 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/circular_replay_buffer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    14059 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/prioritized_replay_buffer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     6895 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/replay_memory/sum_tree.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.706803 dopamine_rl-4.0.7/dopamine/utils/
--rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/__init__.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     4604 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/agent_visualizer.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2219 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/atari_plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3883 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/bar_plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     2596 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/example_viz.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)    10742 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/example_viz_lib.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     4019 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/line_plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3239 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/plotter.py
--rw-r--r--   0 psc      (160661) primarygroup (89939)     1268 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/dopamine/utils/test_utils.py
-drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 16:58:41.708205 dopamine_rl-4.0.7/dopamine_rl.egg-info/
--rw-r--r--   0 psc      (160661) primarygroup (89939)     8009 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/PKG-INFO
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3367 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/SOURCES.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)        1 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/dependency_links.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)      240 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/requires.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)        9 2024-05-06 16:58:41.000000 dopamine_rl-4.0.7/dopamine_rl.egg-info/top_level.txt
--rw-r--r--   0 psc      (160661) primarygroup (89939)       38 2024-05-06 16:58:41.708944 dopamine_rl-4.0.7/setup.cfg
--rw-r--r--   0 psc      (160661) primarygroup (89939)     3109 2024-05-06 16:58:21.000000 dopamine_rl-4.0.7/setup.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.469796 dopamine_rl-4.0.8/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      298 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/AUTHORS
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    11417 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/LICENSE
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     8009 2024-05-06 19:45:22.469554 dopamine_rl-4.0.8/PKG-INFO
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     6073 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/README.md
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.453263 dopamine_rl-4.0.8/dopamine/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      619 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.453438 dopamine_rl-4.0.8/dopamine/agents/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.453782 dopamine_rl-4.0.8/dopamine/agents/dqn/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/dqn/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    22344 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/dqn/dqn_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.454168 dopamine_rl-4.0.8/dopamine/agents/implicit_quantile/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/implicit_quantile/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    13885 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/implicit_quantile/implicit_quantile_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.454526 dopamine_rl-4.0.8/dopamine/agents/rainbow/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/rainbow/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    21209 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/agents/rainbow/rainbow_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.454861 dopamine_rl-4.0.8/dopamine/colab/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/colab/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    10872 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/colab/utils.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.455418 dopamine_rl-4.0.8/dopamine/continuous_domains/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/continuous_domains/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    11032 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/continuous_domains/run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1675 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/continuous_domains/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.457030 dopamine_rl-4.0.8/dopamine/discrete_domains/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    20405 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/atari_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     7830 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/checkpointer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    15458 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/gym_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1645 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/iteration_statistics.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     8414 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/legacy_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3581 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/logger.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    29223 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1782 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/discrete_domains/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.457821 dopamine_rl-4.0.8/dopamine/jax/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.458007 dopamine_rl-4.0.8/dopamine/jax/agents/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.458386 dopamine_rl-4.0.8/dopamine/jax/agents/dqn/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/dqn/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    25694 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/dqn/dqn_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.458732 dopamine_rl-4.0.8/dopamine/jax/agents/full_rainbow/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/full_rainbow/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    17438 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.459081 dopamine_rl-4.0.8/dopamine/jax/agents/implicit_quantile/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/implicit_quantile/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    19224 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.459413 dopamine_rl-4.0.8/dopamine/jax/agents/quantile/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/quantile/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    12771 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/quantile/quantile_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.459761 dopamine_rl-4.0.8/dopamine/jax/agents/rainbow/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/rainbow/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    20026 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/rainbow/rainbow_agent.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.460121 dopamine_rl-4.0.8/dopamine/jax/agents/sac/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/sac/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    25998 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/agents/sac/sac_agent.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     7293 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/continuous_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1670 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/losses.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    19671 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/jax/networks.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.460292 dopamine_rl-4.0.8/dopamine/labs/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.461775 dopamine_rl-4.0.8/dopamine/labs/atari_100k/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    12279 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/atari_100k_rainbow_agent.py
+-rwxr-xr-x   0 psc      (160661) primarygroup (89939)    21090 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/atari_100k_runner.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     4783 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/eval_run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3546 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/normalization_utils.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    16018 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/spr_agent.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    14871 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/spr_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3664 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/atari_100k/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.461964 dopamine_rl-4.0.8/dopamine/labs/environments/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/environments/__init__.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.462513 dopamine_rl-4.0.8/dopamine/labs/environments/brax/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/environments/brax/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3858 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/environments/brax/brax_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1705 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/environments/brax/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.462874 dopamine_rl-4.0.8/dopamine/labs/environments/minatar/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/environments/minatar/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     5406 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/environments/minatar/minatar_env.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.463422 dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     5615 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/continuous_networks.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     7070 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/deepmind_control_lib.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.464205 dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    10357 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/run_experiment.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    11705 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/tandem_dqn_agent.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1921 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/train.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.465443 dopamine_rl-4.0.8/dopamine/metrics/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      584 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2337 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/collector.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3683 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/collector_dispatcher.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2023 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/console_collector.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2054 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/pickle_collector.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      870 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/statistics_instance.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1592 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/metrics/tensorboard_collector.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.466338 dopamine_rl-4.0.8/dopamine/replay_memory/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/replay_memory/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    38590 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/replay_memory/circular_replay_buffer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    14056 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/replay_memory/prioritized_replay_buffer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     6895 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/replay_memory/sum_tree.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.467895 dopamine_rl-4.0.8/dopamine/utils/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      601 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/__init__.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     4604 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/agent_visualizer.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2219 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/atari_plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3883 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/bar_plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     2596 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/example_viz.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)    10742 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/example_viz_lib.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     4019 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/line_plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3239 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/plotter.py
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     1268 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/dopamine/utils/test_utils.py
+drwxr-xr-x   0 psc      (160661) primarygroup (89939)        0 2024-05-06 19:45:22.469187 dopamine_rl-4.0.8/dopamine_rl.egg-info/
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     8009 2024-05-06 19:45:22.000000 dopamine_rl-4.0.8/dopamine_rl.egg-info/PKG-INFO
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3367 2024-05-06 19:45:22.000000 dopamine_rl-4.0.8/dopamine_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)        1 2024-05-06 19:45:22.000000 dopamine_rl-4.0.8/dopamine_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)      240 2024-05-06 19:45:22.000000 dopamine_rl-4.0.8/dopamine_rl.egg-info/requires.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)        9 2024-05-06 19:45:22.000000 dopamine_rl-4.0.8/dopamine_rl.egg-info/top_level.txt
+-rw-r--r--   0 psc      (160661) primarygroup (89939)       38 2024-05-06 19:45:22.469871 dopamine_rl-4.0.8/setup.cfg
+-rw-r--r--   0 psc      (160661) primarygroup (89939)     3109 2024-05-06 19:45:16.000000 dopamine_rl-4.0.8/setup.py
```

### Comparing `dopamine_rl-4.0.7/LICENSE` & `dopamine_rl-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/PKG-INFO` & `dopamine_rl-4.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopamine_rl
-Version: 4.0.7
+Version: 4.0.8
 Summary: Dopamine: A framework for flexible Reinforcement Learning research
 Home-page: https://github.com/google/dopamine
 Author: The Dopamine Team
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/dopamine
 Project-URL: Bug Reports, https://github.com/google/dopamine/issues
 Project-URL: Source, https://github.com/google/dopamine
```

### Comparing `dopamine_rl-4.0.7/README.md` & `dopamine_rl-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/__init__.py` & `dopamine_rl-4.0.8/dopamine/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/agents/__init__.py` & `dopamine_rl-4.0.8/dopamine/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/agents/dqn/__init__.py` & `dopamine_rl-4.0.8/dopamine/agents/dqn/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/agents/dqn/dqn_agent.py` & `dopamine_rl-4.0.8/dopamine/agents/dqn/dqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import math
 import os
 import random
 
 from absl import logging
 from dopamine.discrete_domains import atari_lib
 from dopamine.replay_memory import circular_replay_buffer
-import gin.tf
+import gin
 import numpy as np
 import tensorflow as tf
 
 
 # These are aliases which are used by other classes.
 NATURE_DQN_OBSERVATION_SHAPE = atari_lib.NATURE_DQN_OBSERVATION_SHAPE
 NATURE_DQN_DTYPE = atari_lib.NATURE_DQN_DTYPE
```

### Comparing `dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/__init__.py` & `dopamine_rl-4.0.8/dopamine/agents/implicit_quantile/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/agents/implicit_quantile/implicit_quantile_agent.py` & `dopamine_rl-4.0.8/dopamine/agents/implicit_quantile/implicit_quantile_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from __future__ import division
 from __future__ import print_function
 
 
 
 from dopamine.agents.rainbow import rainbow_agent
 from dopamine.discrete_domains import atari_lib
-import gin.tf
+import gin
 import tensorflow as tf
 
 
 @gin.configurable
 class ImplicitQuantileAgent(rainbow_agent.RainbowAgent):
   """An extension of Rainbow to perform implicit quantile regression."""
```

### Comparing `dopamine_rl-4.0.7/dopamine/agents/rainbow/__init__.py` & `dopamine_rl-4.0.8/dopamine/agents/rainbow/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/agents/rainbow/rainbow_agent.py` & `dopamine_rl-4.0.8/dopamine/agents/rainbow/rainbow_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from __future__ import print_function
 
 
 
 from dopamine.agents.dqn import dqn_agent
 from dopamine.discrete_domains import atari_lib
 from dopamine.replay_memory import prioritized_replay_buffer
-import gin.tf
+import gin
 import tensorflow as tf
 
 
 @gin.configurable
 class RainbowAgent(dqn_agent.DQNAgent):
   """A compact implementation of a simplified Rainbow agent."""
```

### Comparing `dopamine_rl-4.0.7/dopamine/colab/__init__.py` & `dopamine_rl-4.0.8/dopamine/colab/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/colab/utils.py` & `dopamine_rl-4.0.8/dopamine/colab/utils.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/continuous_domains/__init__.py` & `dopamine_rl-4.0.8/dopamine/continuous_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/continuous_domains/run_experiment.py` & `dopamine_rl-4.0.8/dopamine/continuous_domains/run_experiment.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/continuous_domains/train.py` & `dopamine_rl-4.0.8/dopamine/continuous_domains/train.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/__init__.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/atari_lib.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/atari_lib.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/checkpointer.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/checkpointer.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/gym_lib.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/gym_lib.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/iteration_statistics.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/iteration_statistics.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/legacy_networks.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/legacy_networks.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/logger.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from __future__ import division
 from __future__ import print_function
 
 import os
 import pickle
 
 from absl import logging
-import gin.tf
+import gin
 import tensorflow as tf
 
 
 @gin.configurable
 class Logger(object):
   """Class for maintaining a dictionary of data to log."""
```

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/run_experiment.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/run_experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from dopamine.jax.agents.quantile import quantile_agent as jax_quantile_agent
 from dopamine.jax.agents.rainbow import rainbow_agent as jax_rainbow_agent
 from dopamine.labs.moes.agents import dqn_moe_agent
 from dopamine.labs.moes.agents import full_rainbow_moe_agent
 from dopamine.labs.moes.agents import rainbow_100k_moe_agent
 from dopamine.metrics import collector_dispatcher
 from dopamine.metrics import statistics_instance
-import gin.tf
+import gin
 import numpy as np
 import tensorflow as tf
 import tqdm.auto as tqdm
 
 
 def load_gin_configs(gin_files, gin_bindings):
   """Loads gin configuration files.
```

### Comparing `dopamine_rl-4.0.7/dopamine/discrete_domains/train.py` & `dopamine_rl-4.0.8/dopamine/discrete_domains/train.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/dqn/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/dqn/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/dqn/dqn_agent.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/full_rainbow/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/full_rainbow/full_rainbow_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/implicit_quantile/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/implicit_quantile/implicit_quantile_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/quantile/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/quantile/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/quantile/quantile_agent.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/quantile/quantile_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/rainbow/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/rainbow/rainbow_agent.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/rainbow/rainbow_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/sac/__init__.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/sac/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/agents/sac/sac_agent.py` & `dopamine_rl-4.0.8/dopamine/jax/agents/sac/sac_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/continuous_networks.py` & `dopamine_rl-4.0.8/dopamine/jax/continuous_networks.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/losses.py` & `dopamine_rl-4.0.8/dopamine/jax/losses.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/jax/networks.py` & `dopamine_rl-4.0.8/dopamine/jax/networks.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/atari_100k_rainbow_agent.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/atari_100k_rainbow_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/atari_100k_runner.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/atari_100k_runner.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/eval_run_experiment.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/eval_run_experiment.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/normalization_utils.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/normalization_utils.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/spr_agent.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/spr_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/spr_networks.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/spr_networks.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/atari_100k/train.py` & `dopamine_rl-4.0.8/dopamine/labs/atari_100k/train.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/environments/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/environments/brax/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/environments/brax/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/environments/brax/brax_lib.py` & `dopamine_rl-4.0.8/dopamine/labs/environments/brax/brax_lib.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/environments/brax/train.py` & `dopamine_rl-4.0.8/dopamine/labs/environments/brax/train.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/environments/minatar/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/environments/minatar/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/environments/minatar/minatar_env.py` & `dopamine_rl-4.0.8/dopamine/labs/environments/minatar/minatar_env.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/continuous_networks.py` & `dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/continuous_networks.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/sac_from_pixels/deepmind_control_lib.py` & `dopamine_rl-4.0.8/dopamine/labs/sac_from_pixels/deepmind_control_lib.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/__init__.py` & `dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/run_experiment.py` & `dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/run_experiment.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/tandem_dqn_agent.py` & `dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/tandem_dqn_agent.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/labs/tandem_dqn/train.py` & `dopamine_rl-4.0.8/dopamine/labs/tandem_dqn/train.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/__init__.py` & `dopamine_rl-4.0.8/dopamine/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/collector.py` & `dopamine_rl-4.0.8/dopamine/metrics/collector.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/collector_dispatcher.py` & `dopamine_rl-4.0.8/dopamine/metrics/collector_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/console_collector.py` & `dopamine_rl-4.0.8/dopamine/metrics/console_collector.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/pickle_collector.py` & `dopamine_rl-4.0.8/dopamine/metrics/pickle_collector.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/statistics_instance.py` & `dopamine_rl-4.0.8/dopamine/metrics/statistics_instance.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/metrics/tensorboard_collector.py` & `dopamine_rl-4.0.8/dopamine/metrics/tensorboard_collector.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/replay_memory/__init__.py` & `dopamine_rl-4.0.8/dopamine/replay_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/replay_memory/circular_replay_buffer.py` & `dopamine_rl-4.0.8/dopamine/replay_memory/circular_replay_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import collections
 import gzip
 import math
 import os
 import pickle
 
 from absl import logging
-import gin.tf
+import gin
 import numpy as np
 import tensorflow as tf
 
 
 # Defines a type describing part of the tuple returned by the replay
 # memory. Each element of the tuple is a tensor of shape [batch, ...] where
 # ... is defined the 'shape' field of ReplayElement. The tensor type is
```

### Comparing `dopamine_rl-4.0.7/dopamine/replay_memory/prioritized_replay_buffer.py` & `dopamine_rl-4.0.8/dopamine/replay_memory/prioritized_replay_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from __future__ import print_function
 
 
 
 from dopamine.replay_memory import circular_replay_buffer
 from dopamine.replay_memory import sum_tree
 from dopamine.replay_memory.circular_replay_buffer import ReplayElement
-import gin.tf
+import gin
 import numpy as np
 import tensorflow as tf
 
 
 @gin.configurable
 class OutOfGraphPrioritizedReplayBuffer(
     circular_replay_buffer.OutOfGraphReplayBuffer
```

### Comparing `dopamine_rl-4.0.7/dopamine/replay_memory/sum_tree.py` & `dopamine_rl-4.0.8/dopamine/replay_memory/sum_tree.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/__init__.py` & `dopamine_rl-4.0.8/dopamine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/agent_visualizer.py` & `dopamine_rl-4.0.8/dopamine/utils/agent_visualizer.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/atari_plotter.py` & `dopamine_rl-4.0.8/dopamine/utils/atari_plotter.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/bar_plotter.py` & `dopamine_rl-4.0.8/dopamine/utils/bar_plotter.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/example_viz.py` & `dopamine_rl-4.0.8/dopamine/utils/example_viz.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/example_viz_lib.py` & `dopamine_rl-4.0.8/dopamine/utils/example_viz_lib.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/line_plotter.py` & `dopamine_rl-4.0.8/dopamine/utils/line_plotter.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/plotter.py` & `dopamine_rl-4.0.8/dopamine/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine/utils/test_utils.py` & `dopamine_rl-4.0.8/dopamine/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/dopamine_rl.egg-info/PKG-INFO` & `dopamine_rl-4.0.8/dopamine_rl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopamine_rl
-Version: 4.0.7
+Version: 4.0.8
 Summary: Dopamine: A framework for flexible Reinforcement Learning research
 Home-page: https://github.com/google/dopamine
 Author: The Dopamine Team
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/dopamine
 Project-URL: Bug Reports, https://github.com/google/dopamine/issues
 Project-URL: Source, https://github.com/google/dopamine
```

### Comparing `dopamine_rl-4.0.7/dopamine_rl.egg-info/SOURCES.txt` & `dopamine_rl-4.0.8/dopamine_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dopamine_rl-4.0.7/setup.py` & `dopamine_rl-4.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 dopamine_description = (
     'Dopamine: A framework for flexible Reinforcement Learning research'
 )
 
 setup(
     name='dopamine_rl',
-    version='4.0.7',
+    version='4.0.8',
     description=dopamine_description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/google/dopamine',
     author='The Dopamine Team',
     classifiers=[
         'Development Status :: 4 - Beta',
```

