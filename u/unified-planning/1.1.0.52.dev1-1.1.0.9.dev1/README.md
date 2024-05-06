# Comparing `tmp/unified_planning-1.1.0.52.dev1.tar.gz` & `tmp/unified_planning-1.1.0.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-1.1.0.52.dev1.tar", last modified: Mon May  6 14:59:18 2024, max compression
+gzip compressed data, was "unified_planning-1.1.0.9.dev1.tar", last modified: Thu Mar 14 13:58:09 2024, max compression
```

## Comparing `unified_planning-1.1.0.52.dev1.tar` & `unified_planning-1.1.0.9.dev1.tar`

### file list

```diff
@@ -1,476 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.983420 unified_planning-1.1.0.52.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.987420 unified_planning-1.1.0.52.dev1/unified_planning/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/cmd/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/cmd/up.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.987420 unified_planning-1.1.0.52.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.991420 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/state_invariants_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30421 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    20883 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.991420 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/pddl_anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13202 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    36012 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.991420 unified_planning-1.1.0.52.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.995420 unified_planning-1.1.0.52.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39061 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    39191 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.995420 unified_planning-1.1.0.52.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.995420 unified_planning-1.1.0.52.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41221 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    82326 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    46771 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.999420 unified_planning-1.1.0.52.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    29564 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18698 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    28821 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (127)    17991 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.999420 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.003420 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.003420 unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    56290 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/problem_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/problem_kind_versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.003420 unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.003420 unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.007420 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    24752 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.007420 unified_planning-1.1.0.52.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plans/time_triggered_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.007420 unified_planning-1.1.0.52.dev1/unified_planning/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plot/causal_graph_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plot/plan_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30976 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.015420 unified_planning-1.1.0.52.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.019420 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/safe_road.anml
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.975421 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.019420 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.019420 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.019420 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    48848 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/realistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    37854 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.979421 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    34291 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    33635 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.023420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (127)    10943 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)   189505 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    33123 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    36329 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.027420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (127)    34612 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.031420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/parking_action_cost/
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/parking_action_cost/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/parking_action_cost/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/tpp_metric/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    37292 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_problem_kind_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_state_invariants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_ttp_to_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:17.987420 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-06 14:59:17.000000 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17930 2024-05-06 14:59:17.000000 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:59:17.000000 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 14:59:17.000000 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 14:59:17.000000 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 14:59:17.000000 unified_planning-1.1.0.52.dev1/unified_planning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/up_test_cases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/basic_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/depots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/metric_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/tpp/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/tpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.035420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/hierarchical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/depot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/ma_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/taxi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/block_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/depots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/farmlands/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/farmlands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/fn_counters/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/fn_counters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/linear_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/plant_watering/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/plant_watering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/problem_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/rovers/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/rovers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/sailing/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/sailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/test_01.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/test_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/test_03.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.039420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/test_01.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/test_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/test_03.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/temporal/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/temporal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/temporal/depot/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/builtin/temporal/depot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/classical/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/classical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/classical/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/classical/depots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/classical/tpp/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/classical/tpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/block_grouping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/depots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/farmlands/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/farmlands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/fn_counters/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/fn_counters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/plant_watering/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/plant_watering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/rovers/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/rovers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/sailing/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/sailing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/temporal/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/temporal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:59:18.043420 unified_planning-1.1.0.52.dev1/up_test_cases/performance/temporal/depot/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/performance/temporal/depot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-06 14:59:15.000000 unified_planning-1.1.0.52.dev1/up_test_cases/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.928569 unified_planning-1.1.0.9.dev1/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.932569 unified_planning-1.1.0.9.dev1/unified_planning/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/cmd/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/cmd/up.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.932569 unified_planning-1.1.0.9.dev1/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/state_invariants_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30421 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20883 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36012 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39061 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39191 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.940569 unified_planning-1.1.0.9.dev1/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.940569 unified_planning-1.1.0.9.dev1/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41221 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78448 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45266 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.944569 unified_planning-1.1.0.9.dev1/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29564 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28821 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17991 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.944569 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56259 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.952569 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24752 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.952569 unified_planning-1.1.0.9.dev1/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/time_triggered_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.952569 unified_planning-1.1.0.9.dev1/unified_planning/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/causal_graph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/plan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30976 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.960569 unified_planning-1.1.0.9.dev1/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/safe_road.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.920569 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48848 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/realistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37854 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.924569 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    34291 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    33635 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (127)    10943 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)   189505 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    33123 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    36329 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (127)    34612 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35427 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem_kind_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_state_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_ttp_to_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.928569 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/basic_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/depots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/metric_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/tpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/tpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/hierarchical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/depot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/ma_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/taxi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/block_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/depots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/farmlands/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/farmlands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/fn_counters/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/fn_counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/linear_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/plant_watering/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/plant_watering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/problem_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/rovers/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/rovers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/sailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/sailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/depot/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/depot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/depots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/tpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/tpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/block_grouping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/depots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/farmlands/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/farmlands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/fn_counters/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/fn_counters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/plant_watering/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/plant_watering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/rovers/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/rovers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/sailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/sailing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/depot/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/depot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/utils.py
```

### Comparing `unified_planning-1.1.0.52.dev1/LICENSE` & `unified_planning-1.1.0.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/PKG-INFO` & `unified_planning-1.1.0.9.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified_planning
-Version: 1.1.0.52.dev1
+Version: 1.1.0.9.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.1.0.52.dev1/README.md` & `unified_planning-1.1.0.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/setup.py` & `unified_planning-1.1.0.9.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/cmd/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/cmd/arg_parser.py` & `unified_planning-1.1.0.9.dev1/unified_planning/cmd/arg_parser.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/cmd/up.py` & `unified_planning-1.1.0.9.dev1/unified_planning/cmd/up.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/state_invariants_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/state_invariants_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/credits.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/engine.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/factory.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/meta_engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/compiler.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/portfolio.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/oversubscription_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/parallel.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/parallel.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/pddl_anytime_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/replanner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/results.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
 
 class FailedValidationReason(Enum):
     """Enum representing the possible reasons the plan validation failed."""
 
     INAPPLICABLE_ACTION = auto()
     UNSATISFIED_GOALS = auto()
-    MUTEX_CONFLICT = auto()
 
 
 class PlanGenerationResultStatus(Enum):
     """
     Enum representing the 9 possible values in the status field of a :class:`~unified_planning.engines.PlanGenerationResult`:
     SOLVED_SATISFICING        -> Valid plan found.
     SOLVED_OPTIMALLY          -> Optimal plan found.
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/environment.py` & `unified_planning-1.1.0.9.dev1/unified_planning/environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/exceptions.py` & `unified_planning-1.1.0.9.dev1/unified_planning/exceptions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/grpc/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/grpc/converter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/interop/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-1.1.0.9.dev1/unified_planning/interop/from_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-1.1.0.9.dev1/unified_planning/interop/to_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/anml_grammar.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/anml_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/anml_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/ma_pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -756,75 +756,14 @@
         ]
         while to_add:
             eff, forall_variables = to_add.pop(0)
             op = eff[0].value
             if op == "and":
                 for i in range(1, len(eff)):
                     to_add.append((eff[i], forall_variables))
-            elif op == "when":
-                if (
-                    len(eff) == 3
-                    and eff[1][0].value == "at"
-                    and eff[1][1].value == "start"
-                ):
-                    cond = self._parse_exp(
-                        problem,
-                        act,
-                        types_map,
-                        forall_variables,
-                        eff[1][2],
-                        complete_str,
-                    )
-                    if len(eff[2]) == 3 and eff[2][1].value == "start":
-                        self._add_effect(
-                            problem,
-                            act,
-                            types_map,
-                            eff[2][2],
-                            complete_str,
-                            cond,
-                            timing=up.model.StartTiming(),
-                            forall_variables=forall_variables,
-                        )
-                    else:
-                        raise UPUnsupportedProblemTypeError(
-                            "Conditional effects with different timing are not supported."
-                        )
-                elif (
-                    len(eff) == 3
-                    and eff[1][0].value == "at"
-                    and eff[1][1].value == "end"
-                ):
-                    cond = self._parse_exp(
-                        problem,
-                        act,
-                        types_map,
-                        forall_variables,
-                        eff[1][2],
-                        complete_str,
-                    )
-                    if len(eff[2]) == 3 and eff[2][1].value == "end":
-                        self._add_effect(
-                            problem,
-                            act,
-                            types_map,
-                            eff[2][2],
-                            complete_str,
-                            cond,
-                            timing=up.model.EndTiming(),
-                            forall_variables=forall_variables,
-                        )
-                    else:
-                        raise UPUnsupportedProblemTypeError(
-                            "Conditional effects with different timing are not supported."
-                        )
-                else:
-                    raise UPUnsupportedProblemTypeError(
-                        "Conditional durative effects syntax is not correct."
-                    )
             elif len(eff) == 3 and op == "at" and eff[1].value == "start":
                 self._add_effect(
                     problem,
                     act,
                     types_map,
                     eff[2],
                     complete_str,
@@ -859,15 +798,15 @@
                 start_line, start_col = eff.line_start(complete_str), eff.col_start(
                     complete_str
                 )
                 end_line, end_col = eff.line_end(complete_str), eff.col_end(
                     complete_str
                 )
                 raise SyntaxError(
-                    f"Not able to handle: {eff.value}, from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
+                    f"Not able to handle: {eff}, from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
                 )
 
     def _parse_subtask(
         self,
         e,
         method: typing.Optional[Union[htn.Method, htn.TaskNetwork]],
         problem: htn.HierarchicalProblem,
@@ -970,24 +909,21 @@
             dur_act.duration.lower
         ) or self._totalcost in self._fve.get(dur_act.duration.upper):
             return False
         for _, cl in dur_act.conditions.items():
             for c in cl:
                 if self._totalcost in self._fve.get(c):
                     return False
-        cost_found = False
         for _, el in dur_act.effects.items():
             for e in el:
-                if self._totalcost in self._fve.get(e.fluent):
-                    if cost_found:
-                        return False
-                    cost_found = True
-                if self._totalcost in self._fve.get(
-                    e.value
-                ) or self._totalcost in self._fve.get(e.condition):
+                if (
+                    self._totalcost in self._fve.get(e.fluent)
+                    or self._totalcost in self._fve.get(e.value)
+                    or self._totalcost in self._fve.get(e.condition)
+                ):
                     return False
         return True
 
     def _instantaneous_action_has_cost(self, act: up.model.InstantaneousAction):
         for c in act.preconditions:
             if self._totalcost in self._fve.get(c):
                 return False
@@ -1639,56 +1575,32 @@
                         problem, None, types_map, {}, metric, problem_str
                     )
                     if (
                         has_actions_cost
                         and optimization == "minimize"
                         and metric_exp == self._totalcost
                     ):
-                        costs: Dict[up.model.Action, up.model.Expression] = {}
+                        costs = {}
                         problem._fluents.remove(self._totalcost.fluent())
                         if self._totalcost in problem._initial_value:
                             problem._initial_value.pop(self._totalcost)
-                        start_timing, end_timing = (
-                            up.model.StartTiming(),
-                            up.model.EndTiming(),
-                        )
-                        for a in problem.actions:
-                            if isinstance(a, up.model.InstantaneousAction):
-                                cost = None
-                                for e in a.effects:
-                                    if e.fluent == self._totalcost:
-                                        cost = e
-                                        break
-                                if cost is not None:
-                                    costs[a] = cost.value
-                                    a._effects.remove(cost)
-                                    if cost.value != 1:
-                                        use_plan_length = False
-                                else:
+                        use_plan_length = all(False for _ in problem.durative_actions)
+                        for a in problem.instantaneous_actions:
+                            cost = None
+                            for e in a.effects:
+                                if e.fluent == self._totalcost:
+                                    cost = e
+                                    break
+                            if cost is not None:
+                                costs[a] = cost.value
+                                a._effects.remove(cost)
+                                if cost.value != 1:
                                     use_plan_length = False
                             else:
-                                assert isinstance(a, up.model.DurativeAction)
                                 use_plan_length = False
-                                cost, effects_list = None, None
-                                for timing, el in a.effects.items():
-                                    if timing in (start_timing, end_timing):
-                                        for e in el:
-                                            if e.fluent == self._totalcost:
-                                                if cost is not None:
-                                                    raise UPUnsupportedProblemTypeError(
-                                                        f"Action {a.name} has more than one effect modifying it's cost"
-                                                    )
-                                                cost, effects_list = e, el
-                                                break
-                                if cost is not None:
-                                    assert effects_list is not None
-                                    costs[a] = cost.value
-                                    effects_list.remove(cost)
-                                else:
-                                    use_plan_length = False
                         if use_plan_length:
                             problem.add_quality_metric(
                                 up.model.metrics.MinimizeSequentialPlanLength()
                             )
                         else:
                             problem.add_quality_metric(
                                 up.model.metrics.MinimizeActionCosts(
@@ -1768,15 +1680,23 @@
     def parse_plan(
         self,
         problem: "up.model.Problem",
         plan_filename: str,
         get_item_named: typing.Optional[
             Callable[
                 [str],
-                "up.io.pddl_writer.WithName",
+                Union[
+                    "up.model.Type",
+                    "up.model.Action",
+                    "up.model.Fluent",
+                    "up.model.Object",
+                    "up.model.Parameter",
+                    "up.model.Variable",
+                    "up.model.multi_agent.Agent",
+                ],
             ]
         ] = None,
     ) -> "up.plans.Plan":
         """
         Takes a problem, a filename and optionally a map of renaming and returns the plan parsed from the file.
 
         The format of the file must be:
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,34 +329,30 @@
         assert len(args) == 2
         return f"(= {args[0]} {args[1]})"
 
 
 class PDDLWriter:
     """
     This class can be used to write a :class:`~unified_planning.model.Problem` in `PDDL`.
-    The constructor of this class takes the problem to write and 3 flags:
+    The constructor of this class takes the problem to write and 2 flags:
     needs_requirements determines if the printed problem must have the :requirements,
     rewrite_bool_assignments determines if this writer will write
     non constant boolean assignment as conditional effects.
-    empty_preconditions determines if this writer will write ':precondition ()' in case of an instantenuous
-    action without preconditions instead of writing nothing or similar with conditions in durative actions.
     """
 
     def __init__(
         self,
         problem: "up.model.Problem",
         needs_requirements: bool = True,
         rewrite_bool_assignments: bool = False,
-        empty_preconditions: bool = False,
     ):
         self.problem = problem
         self.problem_kind = self.problem.kind
         self.needs_requirements = needs_requirements
         self.rewrite_bool_assignments = rewrite_bool_assignments
-        self.empty_preconditions = empty_preconditions
         # otn represents the old to new renamings
         self.otn_renamings: Dict[
             WithName,
             str,
         ] = {}
         # nto represents the new to old renamings
         self.nto_renamings: Dict[
@@ -576,16 +572,14 @@
                     for p in (c.simplify() for c in m.preconditions):
                         if not p.is_true():
                             if p.is_and():
                                 precond_str.extend(map(converter.convert, p.args))
                             else:
                                 precond_str.append(converter.convert(p))
                     out.write(f'\n  :precondition (and {" ".join(precond_str)})')
-                elif len(m.preconditions) == 0 and self.empty_preconditions:
-                    out.write(f"\n  :precondition ()")
                 self._write_task_network(m, out, converter)
                 out.write(")\n")
 
         for a in self.problem.actions:
             if isinstance(a, up.model.InstantaneousAction):
                 if any(p.simplify().is_false() for p in a.preconditions):
                     continue
@@ -604,16 +598,14 @@
                     for p in (c.simplify() for c in a.preconditions):
                         if not p.is_true():
                             if p.is_and():
                                 precond_str.extend(map(converter.convert, p.args))
                             else:
                                 precond_str.append(converter.convert(p))
                     out.write(f'\n  :precondition (and {" ".join(precond_str)})')
-                elif len(a.preconditions) == 0 and self.empty_preconditions:
-                    out.write(f"\n  :precondition ()")
                 if len(a.effects) > 0:
                     out.write("\n  :effect (and")
                     for e in a.effects:
                         _write_effect(
                             e,
                             None,
                             out,
@@ -671,16 +663,14 @@
                             else:
                                 if not interval.is_left_open():
                                     out.write(f"(at start {converter.convert(c)})")
                                 out.write(f"(over all {converter.convert(c)})")
                                 if not interval.is_right_open():
                                     out.write(f"(at end {converter.convert(c)})")
                     out.write(")")
-                elif len(a.conditions) == 0 and self.empty_preconditions:
-                    out.write(f"\n  :condition (and )")
                 if len(a.effects) > 0:
                     out.write("\n  :effect (and")
                     for t, el in a.effects.items():
                         for e in el:
                             _write_effect(
                                 e,
                                 t,
@@ -800,16 +790,16 @@
             )
         out.write(")\n")
 
     def _write_plan(self, plan: Plan, out: IO[str]):
         def _format_action_instance(action_instance: ActionInstance) -> str:
             param_str = ""
             if action_instance.actual_parameters:
-                param_str = f" {' '.join((self._get_mangled_name(p.object()) for p in action_instance.actual_parameters))}"
-            return f"({self._get_mangled_name(action_instance.action)}{param_str})"
+                param_str = f" {' '.join((p.object().name for p in action_instance.actual_parameters))}"
+            return f"({action_instance.action.name}{param_str})"
 
         if isinstance(plan, SequentialPlan):
             for ai in plan.actions:
                 out.write(f"{_format_action_instance(ai)}\n")
         elif isinstance(plan, TimeTriggeredPlan):
             for s, ai, dur in plan.timed_actions:
                 start = s.numerator if s.denominator == 1 else float(s)
@@ -920,15 +910,22 @@
         try:
             return self.nto_renamings[name]
         except KeyError:
             raise UPException(f"The name {name} does not correspond to any item.")
 
     def get_pddl_name(
         self,
-        item: WithName,
+        item: Union[
+            "up.model.Type",
+            "up.model.Action",
+            "up.model.Fluent",
+            "up.model.Object",
+            "up.model.Parameter",
+            "up.model.Variable",
+        ],
     ) -> str:
         """
         This method takes an item in the :class:`~unified_planning.model.Problem` and returns the chosen name for the same item in the `PDDL` problem
         or `PDDL` domain generated by this `PDDLWriter`.
 
         :param item: The `unified_planning` entity renamed by this `PDDLWriter`.
         :return: The `PDDL` name of the given item.
@@ -1094,82 +1091,59 @@
         forall_str = f"(forall ({mid_str})"
     simplified_cond = effect.condition.simplify()
     if non_const_bool_ass:
         assert effect.is_assignment()
         positive_cond = (simplified_cond & effect.value).simplify()
         if not positive_cond.is_false():
             out.write(forall_str)
-            if not positive_cond.is_true():
-                out.write(" (when ")
-                if timing is not None:
-                    if timing.is_from_start():
-                        out.write(f" (at start")
-                    else:
-                        out.write(f" (at end")
-                out.write(f"{converter.convert(positive_cond)}")
-                if timing is not None:
-                    out.write(")")
-                out.write(f" {converter.convert(effect.fluent)})")
             if timing is not None:
                 if timing.is_from_start():
                     out.write(f" (at start")
                 else:
                     out.write(f" (at end")
             if positive_cond.is_true():
                 out.write(f" {converter.convert(effect.fluent)}")
+            else:
+                out.write(
+                    f" (when {converter.convert(positive_cond)} {converter.convert(effect.fluent)})"
+                )
             if timing is not None:
                 out.write(")")
             if effect.is_forall():
                 out.write(")")
         negative_cond = (simplified_cond & effect.value.Not()).simplify()
         if not negative_cond.is_false():
             out.write(forall_str)
-            if not negative_cond.is_true():
-                out.write(" (when")
-                if timing is not None:
-                    if timing.is_from_start():
-                        out.write(f" (at start")
-                    else:
-                        out.write(f" (at end")
-                    out.write(f" (at start")
-                out.write(f" {converter.convert(negative_cond)}")
-                if timing is not None:
-                    out.write(")")
-                out.write(f" (not {converter.convert(effect.fluent)}))")
             if timing is not None:
                 if timing.is_from_start():
                     out.write(f" (at start")
                 else:
                     out.write(f" (at end")
             if negative_cond.is_true():
                 out.write(f" {converter.convert(effect.fluent)}")
+            else:
+                out.write(
+                    f" (when {converter.convert(negative_cond)} (not {converter.convert(effect.fluent)}))"
+                )
             if timing is not None:
                 out.write(")")
             if effect.is_forall():
                 out.write(")")
         return
 
     if simplified_cond.is_false():
         return
     out.write(forall_str)
-    if not simplified_cond.is_true():
-        out.write(f" (when")
-        if timing is not None:
-            if timing.is_from_start():
-                out.write(f" (at start")
-            else:
-                out.write(f" (at end")
-        out.write(f" {converter.convert(effect.condition)}")
-        if timing is not None:
-            out.write(")")
     if timing is not None:
         if timing.is_from_start():
             out.write(f" (at start")
         else:
             out.write(f" (at end")
+    if not simplified_cond.is_true():
+        out.write(f" (when {converter.convert(effect.condition)}")
     simplified_value = effect.value.simplify()
     fluent = converter.convert(effect.fluent)
     if simplified_value.is_true():
         out.write(f" {fluent}")
     elif simplified_value.is_false():
         out.write(f" (not {fluent})")
     elif effect.is_increase():
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/io/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/action.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/contingent_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/delta_stn.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/delta_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/effect.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/effect.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,36 +57,34 @@
         fluent: "up.model.fnode.FNode",
         value: "up.model.fnode.FNode",
         condition: "up.model.fnode.FNode",
         kind: EffectKind = EffectKind.ASSIGN,
         forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         fve = fluent.environment.free_vars_extractor
-        fluents_in_fluent = set(fve.get(fluent))
+        fluents_in_fluent = fve.get(fluent)
         fluents_in_fluent.remove(fluent)
         if fluents_in_fluent:
             raise UPProblemDefinitionError(
                 f"The fluent: {fluent} contains other fluents in his arguments: {fluents_in_fluent}"
             )
         self._fluent = fluent
         self._value = value
         self._condition = condition
         self._kind = kind
         fvo = fluent.environment.free_vars_oracle
-        free_vars: Set["up.model.variable.Variable"] = set(
-            fvo.get_free_variables(fluent)
-        )
+        free_vars: Set["up.model.variable.Variable"] = fvo.get_free_variables(fluent)
         free_vars.update(fvo.get_free_variables(value))
         free_vars.update(fvo.get_free_variables(condition))
 
         def free_vars_without_duplicates() -> Iterator["up.model.variable.Variable"]:
             # store seen variables to avoid duplicates
             seen: Set["up.model.variable.Variable"] = set()
             for v in forall:
-                if v in free_vars and v not in seen:
+                if v in free_vars and not v in seen:
                     seen.add(v)
                     assert isinstance(
                         v, up.model.variable.Variable
                     ), "Typing not respected"
                     yield v
             unbounded_vars = free_vars.difference(seen)
             if unbounded_vars:
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/expression.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/expression.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/fluent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/fluent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/fnode.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/fnode.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/htn/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/htn/method.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/method.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/ordering.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/htn/task.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task_network.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/metrics.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/actions_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/agents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/fluents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/initial_state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/objects_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/time_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/user_types_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
 
     def _update_problem_kind_condition(self, exp: "up.model.fnode.FNode"):
         ops = self._operators_extractor.get(exp)
         if OperatorKind.EQUALS in ops:
             self._kind.set_conditions_kind("EQUALITIES")
         if OperatorKind.NOT in ops:
             self._kind.set_conditions_kind("NEGATIVE_CONDITIONS")
-        if OperatorKind.OR in ops or OperatorKind.IMPLIES in ops:
+        if OperatorKind.OR in ops:
             self._kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         if OperatorKind.EXISTS in ops:
             self._kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         if OperatorKind.FORALL in ops:
             self._kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
 
     def _update_problem_kind_type(self, type: "up.model.types.Type"):
@@ -389,18 +389,18 @@
             )
             if (
                 numeric_type.lower_bound is not None
                 or numeric_type.upper_bound is not None
             ):
                 self._kind.set_numbers("BOUNDED_TYPES")
             if fluent.type.is_int_type():
-                self._kind.set_fluents_type("INT_FLUENTS")
+                self.kind.set_fluents_type("INT_FLUENTS")
             else:
                 assert fluent.type.is_real_type()
-                self._kind.set_fluents_type("REAL_FLUENTS")
+                self.kind.set_fluents_type("REAL_FLUENTS")
         elif fluent.type.is_user_type():
             self._kind.set_fluents_type("OBJECT_FLUENTS")
         for p in fluent.signature:
             self._update_problem_kind_type(p.type)
 
     def _update_problem_kind_action(self, action: "up.model.action.Action"):
         for p in action.parameters:
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/object.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/object.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/operators.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/parameter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/parameter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,15 +862,15 @@
         exp: "up.model.fnode.FNode",
     ):
         ops = self.operators_extractor.get(exp)
         if OperatorKind.EQUALS in ops:
             self.kind.set_conditions_kind("EQUALITIES")
         if OperatorKind.NOT in ops:
             self.kind.set_conditions_kind("NEGATIVE_CONDITIONS")
-        if OperatorKind.OR in ops or OperatorKind.IMPLIES in ops:
+        if OperatorKind.OR in ops:
             self.kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         if OperatorKind.EXISTS in ops:
             self.kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         if OperatorKind.FORALL in ops:
             self.kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         is_linear, _, _ = self.linear_checker.get_fluents(exp)
         if not is_linear:
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/problem_kind.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/problem_kind_versioning.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind_versioning.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/activity.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/chronicle.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/scheduling/scheduling_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/state.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/state.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from abc import ABC, abstractmethod
-from functools import reduce
-from operator import xor
 from typing import Dict, List, Optional, Tuple
 import unified_planning as up
 from unified_planning.exceptions import UPUsageError, UPValueError
 
 
 class State(ABC):
     """This is an abstract class representing a classical `State`"""
@@ -60,55 +58,28 @@
         """
         max_ancestors = type(self).MAX_ANCESTORS
         if max_ancestors is not None and max_ancestors < 1:
             raise UPValueError(
                 f"The max_ancestor field of a class extending UPState must be > 0 or None: in the class {type(self)} it is set to {type(self).MAX_ANCESTORS}"
             )
         self._father = _father
-        self._values = values.copy()
+        self._values = values
         if _father is None:
             self._ancestors = 0
         else:
             self._ancestors = _father._ancestors + 1
-        self._hash: Optional[int] = None
-
-    def _condense_state(self):
-        """
-        Important NOTE: This method modifies the internal variables of the state.
-        This method condenses all the ancestors hierarchy into a new dictionary,
-        sets it as the new values of this state, sets the self._father to None
-        and self._ancestors to 0.
-        """
-        if self._father is not None:
-            current_instance: Optional[UPState] = self
-            condensed_values: Dict["up.model.FNode", "up.model.FNode"] = {}
-            while current_instance is not None:
-                for k, v in current_instance._values.items():
-                    condensed_values.setdefault(k, v)
-                current_instance = current_instance._father
-
-            self._values = condensed_values
-            self._ancestors = 0
-            self._father = None
 
     def __repr__(self) -> str:
-        self._condense_state()
-        return str(self._values)
-
-    def __hash__(self) -> int:
-        self._condense_state()
-        if self._hash is None:
-            self._hash = reduce(xor, map(hash, self._values.items()), 0)
-        assert self._hash is not None
-        return self._hash
-
-    def __eq__(self, oth: object) -> bool:
-        if isinstance(oth, UPState) and hash(self) == hash(oth):
-            return self._values == oth._values
-        return False
+        current_instance: Optional[UPState] = self
+        mappings: Dict["up.model.FNode", "up.model.FNode"] = {}
+        while current_instance is not None:
+            for k, v in current_instance._values.items():
+                mappings.setdefault(k, v)
+            current_instance = current_instance._father
+        return str(mappings)
 
     def get_value(self, fluent: "up.model.FNode") -> "up.model.FNode":
         """
         This method retrieves the value of the given fluent in the `State`.
         NOTE that the searched fluent must be set in the state otherwise an
         exception is raised.
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/action.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     A motion model describes how a movable object moves with respect to time
     and is usually expressed as an equation of motion governing the transition of
     object states, such as position and velocity.
     """
 
     REEDSSHEPP = auto()
     SE2 = auto()
-    SE3 = auto()
 
 
 class MovableObject(Object):
     """
     This class represents a movable object.
 
     A movable object is an object able to move in an environment
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/tamp/types.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/timing.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/timing.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/type_manager.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/type_manager.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/types.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/variable.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 """
 This module defines the Variable class.
 A Variable has a name and a type.
 """
 
 
-from typing import List, Optional, FrozenSet
+from typing import List, Optional, Set
 from unified_planning.environment import Environment, get_environment
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
 import unified_planning
 import unified_planning.model.walkers as walkers
 import unified_planning.model.operators as op
 
@@ -175,40 +175,40 @@
 class FreeVarsOracle(walkers.DagWalker):
     # We have only few categories for this walker.
     #
     # - Quantifiers need to exclude bounded variables
     # - Other operators need to return the union of all their sons
     # - Constants have no impact
 
-    def get_free_variables(self, expression: FNode) -> FrozenSet[Variable]:
-        """Returns the FrozenSet of Symbols appearing free in the expression."""
+    def get_free_variables(self, expression: FNode) -> Set[Variable]:
+        """Returns the set of Symbols appearing free in the expression."""
         return self.walk(expression)
 
     @walkers.handles(OperatorKind.VARIABLE_EXP)
     def walk_variable_exp(
-        self, expression: FNode, args: List[FrozenSet[Variable]], **kwargs
-    ) -> FrozenSet[Variable]:
+        self, expression: FNode, args: List[Set[Variable]], **kwargs
+    ) -> Set[Variable]:
         # pylint: disable=unused-argument
-        return frozenset((expression.variable(),))
+        return {expression.variable()}
 
     @walkers.handles(OperatorKind.EXISTS, OperatorKind.FORALL)
     def walk_quantifier(
-        self, expression: FNode, args: List[FrozenSet[Variable]], **kwargs
-    ) -> FrozenSet[Variable]:
+        self, expression: FNode, args: List[Set[Variable]], **kwargs
+    ) -> Set[Variable]:
         # pylint: disable=unused-argument
         return args[0].difference(expression.variables())
 
     @walkers.handles(op.CONSTANTS)
     def walk_constant(
-        self, expression: FNode, args: List[FrozenSet[Variable]], **kwargs
-    ) -> FrozenSet[Variable]:
+        self, expression: FNode, args: List[Set[Variable]], **kwargs
+    ) -> Set[Variable]:
         # pylint: disable=unused-argument
-        return frozenset()
+        return set()
 
     @walkers.handles(
         set(OperatorKind)
         - {OperatorKind.VARIABLE_EXP, OperatorKind.EXISTS, OperatorKind.FORALL}
     )
     def walk_all(
-        self, expression: FNode, args: List[FrozenSet[Variable]], **kwargs
-    ) -> FrozenSet[Variable]:
-        return frozenset(v for s in args for v in s)
+        self, expression: FNode, args: List[Set[Variable]], **kwargs
+    ) -> Set[Variable]:
+        return {v for s in args for v in s}
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/any.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/any.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/operators_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,37 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from itertools import chain
 import unified_planning.model.walkers as walkers
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
-from typing import Iterator, List, FrozenSet
+from typing import List, Set
 
 
-class FreeVarsExtractor(walkers.dag.DagWalker):
-    """This expression walker returns all the `fluent` expression in the given expression."""
+class OperatorsExtractor(walkers.dag.DagWalker):
+    """This expression walker returns all the operators of a given expression."""
 
     def __init__(self):
         walkers.dag.DagWalker.__init__(self)
 
-    def get(self, expression: FNode) -> FrozenSet[FNode]:
+    def get(self, expression: FNode) -> Set[OperatorKind]:
         """
-        Returns all the `fluent expressions` in the given expression.
+        Returns all the operators of the given expression.
 
-        :param expression: The expression containing the `fluent expressions` to be returned.
-        :return: The FrozenSet of `fluent expressions` appearing in the given expression.
+        :param expression: The target expression.
+        :return: The set containing all the operators appearing in the given expression.
         """
         return self.walk(expression)
 
     @walkers.handles(OperatorKind)
     def walk_all_types(
-        self, expression: FNode, args: List[FrozenSet[FNode]]
-    ) -> FrozenSet[FNode]:
-        res_generator: Iterator[FNode] = (x for y in args for x in y)
-        if expression.is_fluent_exp():
-            res_generator = chain(res_generator, (expression,))
-        return frozenset(res_generator)
+        self, expression: FNode, args: List[Set[OperatorKind]]
+    ) -> Set[OperatorKind]:
+        return set(x for y in args for x in y) | {expression.node_type}
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/generic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/linear_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/names_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/free_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,27 +15,31 @@
 
 import unified_planning.model.walkers as walkers
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
 from typing import List, Set
 
 
-class OperatorsExtractor(walkers.dag.DagWalker):
-    """This expression walker returns all the operators of a given expression."""
+class FreeVarsExtractor(walkers.dag.DagWalker):
+    """This expression walker returns all the `fluent` expression in the given expression."""
 
     def __init__(self):
         walkers.dag.DagWalker.__init__(self)
 
-    def get(self, expression: FNode) -> Set[OperatorKind]:
+    def get(self, expression: FNode) -> Set[FNode]:
         """
-        Returns all the operators of the given expression.
+        Returns all the `fluent expressions` in the given expression.
 
-        :param expression: The target expression.
-        :return: The set containing all the operators appearing in the given expression.
+        :param expression: The expression containing the `fluent expressions` to be returned.
+        :return: The set of `fluent expressions` appearing in the given expression.
         """
-        return self.walk(expression)
+        ret = self.walk(expression)
+        return (
+            ret.copy()
+        )  # return a copy, otherwise modifications of the returned set will invalidate memoization
 
     @walkers.handles(OperatorKind)
-    def walk_all_types(
-        self, expression: FNode, args: List[Set[OperatorKind]]
-    ) -> Set[OperatorKind]:
-        return set(x for y in args for x in y) | {expression.node_type}
+    def walk_all_types(self, expression: FNode, args: List[Set[FNode]]) -> Set[FNode]:
+        res = set(x for y in args for x in y)
+        if expression.is_fluent_exp():
+            res |= {expression}
+        return res
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/simplifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from fractions import Fraction
 from collections import OrderedDict
-from typing import List, Optional, FrozenSet, Union, cast
+from typing import Dict, List, Optional, Set, Union, cast
 import unified_planning as up
 import unified_planning.environment
 import unified_planning.model.walkers as walkers
 from unified_planning.model.fnode import FNode
 from unified_planning.model.types import _UserType
 import unified_planning.model.operators as op
 
@@ -174,15 +174,15 @@
         elif sl == sr:
             return self.manager.TRUE()
         else:
             return self.manager.Implies(sl, sr)
 
     def walk_exists(self, expression: FNode, args: List[FNode]) -> FNode:
         assert len(args) == 1
-        free_vars: FrozenSet[
+        free_vars: Set[
             "up.model.variable.Variable"
         ] = self.environment.free_vars_oracle.get_free_variables(args[0])
         vars = set(var for var in expression.variables() if var in free_vars)
         # Here we check if the arg is in the form:
         # phi(l_i) and l_i == x with phi and x general formulae and l_i a variable
         # bounded to this Exists.
         # if it is, it can be simplified with phi(x) and l_i is removed from the free variables.
@@ -220,15 +220,15 @@
         if vars:
             return self.manager.Exists(new_arg, *vars)
         else:
             return new_arg
 
     def walk_forall(self, expression: FNode, args: List[FNode]) -> FNode:
         assert len(args) == 1
-        free_vars: FrozenSet[
+        free_vars: Set[
             "up.model.variable.Variable"
         ] = self.environment.free_vars_oracle.get_free_variables(args[0])
         vars = tuple(var for var in expression.variables() if var in free_vars)
         if len(vars) == 0:
             return args[0]
         return self.manager.Forall(args[0], *vars)
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/state_evaluator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/type_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/contingent_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/hierarchical_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/schedule.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/schedule.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/sequential_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/time_triggered_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plot/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plot/causal_graph_plot.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/causal_graph_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plot/plan_plot.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/plan_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/plot/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/shortcuts.py` & `unified_planning-1.1.0.9.dev1/unified_planning/shortcuts.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/forall.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/match.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/safe_road.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/safe_road.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/hierarchical.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/minimals.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,18 @@
     da.add_effect(EndTiming(), x, True)
     da.add_condition(TimeInterval(StartTiming(), EndTiming()), y)
     problem = Problem("basic_tils")
     problem.add_fluent(x)
     problem.add_fluent(y)
     problem.add_action(da)
     problem.set_initial_value(x, False)
-    problem.add_timed_effect(GlobalStartTiming(5), x, False)
+    problem.add_timed_effect(StartTiming(5), x, False)
     problem.set_initial_value(y, False)
-    problem.add_timed_effect(GlobalStartTiming(2), y, True)
-    problem.add_timed_effect(GlobalStartTiming(8), y, False)
+    problem.add_timed_effect(StartTiming(2), y, True)
+    problem.add_timed_effect(StartTiming(8), y, False)
     problem.add_goal(x)
     t_plan = up.plans.TimeTriggeredPlan([(Fraction(6), da(), Fraction(1))])
     invalid_t_plans: List[up.plans.Plan] = [
         # condition not established
         up.plans.TimeTriggeredPlan([(Fraction(1), da(), Fraction(1))]),
         # effect would be undone by TIL
         up.plans.TimeTriggeredPlan([(Fraction(3), da(), Fraction(1))]),
@@ -482,15 +482,15 @@
     task.add_precondition(Equals(value, 1))
     task.add_effect(value, 2)
     problem = Problem("basic_numeric_with_timed_effect")
     problem.add_fluent(value)
     problem.add_action(task)
     problem.set_initial_value(value, 1)
     problem.add_goal(Equals(value, 2))
-    problem.add_timed_effect(GlobalStartTiming(1), value, 1)
+    problem.add_timed_effect(StartTiming(1), value, 1)
     t_plan = up.plans.TimeTriggeredPlan(
         [(Fraction(2), up.plans.ActionInstance(task), None)]
     )
     problems["basic_numeric_with_timed_effect"] = TestCase(
         problem=problem, solvable=True, valid_plans=[t_plan]
     )
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/realistic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/examples.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/examples.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/scheduling/jobshop.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/jobshop.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/testing_variants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/enhsp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_anytime.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_anytime.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_contingent_pddl.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_credits.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_dnf.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_factory.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_htn.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_htn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_infix_notation.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_ma_conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_model.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,16 @@
     unittest_TestCase,
     main,
     skipIfNoOneshotPlannerForProblemKind,
 )
 from unified_planning.io import PDDLWriter, PDDLReader
 from unified_planning.test.examples import get_example_problems
 from unified_planning.exceptions import UPProblemDefinitionError
-from unified_planning.model.metrics import MinimizeSequentialPlanLength
-from unified_planning.plans import SequentialPlan
 from unified_planning.model.problem_kind import simple_numeric_kind
+from unified_planning.model.metrics import MinimizeSequentialPlanLength
 from unified_planning.model.types import _UserType
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 PDDL_DOMAINS_PATH = os.path.join(FILE_PATH, "pddl")
 
 
@@ -340,35 +339,14 @@
             pddl_domain,
         )
         self.assertIn(
             ":effect (and (at start (not (handfree))) (at end (fuse_mended ?f)) (at end (handfree))))",
             pddl_domain,
         )
 
-    def test_renamings(self):
-        problem = self.problems["hierarchical_blocks_world"].problem
-        problem = problem.clone()
-        move = problem.action("move")
-        move.name = "move-move"
-
-        Block = problem.user_type("Block")
-        block_4 = Object("block-4", Block)
-        problem.add_object(block_4)
-
-        w = PDDLWriter(problem)
-        plan = SequentialPlan(
-            [move(block_4, problem.object("block_3"), problem.object("block_2"))]
-        )
-        plan_str = w.get_plan(plan)
-
-        r = PDDLReader()
-        test_plan = r.parse_plan_string(problem, plan_str, w.get_item_named)
-
-        self.assertEqual(plan, test_plan)
-
     def test_depot_reader(self):
         reader = PDDLReader()
 
         domain_filename = os.path.join(PDDL_DOMAINS_PATH, "depot", "domain.pddl")
         problem_filename = os.path.join(PDDL_DOMAINS_PATH, "depot", "problem.pddl")
         problem = reader.parse_problem(domain_filename, problem_filename)
 
@@ -443,41 +421,14 @@
 
         with open(domain_filename, "r", encoding="utf-8") as file:
             domain_str = file.read()
         with open(problem_filename, "r", encoding="utf-8") as file:
             problem_str = file.read()
 
         problem_2 = reader.parse_problem_string(domain_str, problem_str)
-        self.assertEqual(problem, problem_2)
-
-    def test_parking_reader(self):
-        reader = PDDLReader()
-
-        domain_filename = os.path.join(
-            PDDL_DOMAINS_PATH, "parking_action_cost", "domain.pddl"
-        )
-        problem_filename = os.path.join(
-            PDDL_DOMAINS_PATH, "parking_action_cost", "problem.pddl"
-        )
-        problem = reader.parse_problem(domain_filename, problem_filename)
-
-        self.assertIsNotNone(problem)
-        self.assertEqual(len(problem.fluents), 5)
-        self.assertEqual(len(problem.actions), 4)
-        self.assertEqual(len(list(problem.objects(problem.user_type("car")))), 2)
-        self.assertEqual(len(list(problem.objects(problem.user_type("curb")))), 4)
-        self.assertEqual(len(problem.quality_metrics), 1)
-        self.assertTrue(problem.quality_metrics[0].is_minimize_action_costs())
-
-        with open(domain_filename, "r", encoding="utf-8") as file:
-            domain_str = file.read()
-        with open(problem_filename, "r", encoding="utf-8") as file:
-            problem_str = file.read()
-
-        problem_2 = reader.parse_problem_string(domain_str, problem_str)
         self.assertEqual(problem, problem_2)
 
     def _test_htn_transport_reader(self, problem):
         assert isinstance(problem, up.model.htn.HierarchicalProblem)
         self.assertEqual(5, len(problem.fluents))
         self.assertEqual(4, len(problem.actions))
         self.assertEqual(
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_plan_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_problem_kind_versioning.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem_kind_versioning.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_protobuf_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_pyperplan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_quantifier_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_replanner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_state_invariants.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_state_invariants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_substituter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_tamp.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_temporal.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_temporal.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraint.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_ttp_to_stn.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_ttp_to_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/test/test_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-1.1.0.9.dev1/unified_planning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-planning
-Version: 1.1.0.52.dev1
+Version: 1.1.0.9.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-1.1.0.9.dev1/unified_planning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,14 @@
 unified_planning/test/test_pyperplan.py
 unified_planning/test/test_quantifier_remover.py
 unified_planning/test/test_replanner.py
 unified_planning/test/test_scheduling.py
 unified_planning/test/test_sequential_simulator.py
 unified_planning/test/test_simplifier.py
 unified_planning/test/test_simulated_effects.py
-unified_planning/test/test_state.py
 unified_planning/test/test_state_invariants.py
 unified_planning/test/test_stn_plan.py
 unified_planning/test/test_substituter.py
 unified_planning/test/test_tamp.py
 unified_planning/test/test_tarski_converter.py
 unified_planning/test/test_tarski_grounder.py
 unified_planning/test/test_temporal.py
@@ -298,16 +297,14 @@
 unified_planning/test/pddl/depot/problem.pddl
 unified_planning/test/pddl/htn-transport/domain.hddl
 unified_planning/test/pddl/htn-transport/problem.hddl
 unified_planning/test/pddl/matchcellar/domain.pddl
 unified_planning/test/pddl/matchcellar/problem.pddl
 unified_planning/test/pddl/miconic/domain.pddl
 unified_planning/test/pddl/miconic/problem.pddl
-unified_planning/test/pddl/parking_action_cost/domain.pddl
-unified_planning/test/pddl/parking_action_cost/problem.pddl
 unified_planning/test/pddl/robot_fastener/domain.pddl
 unified_planning/test/pddl/robot_fastener/problem.pddl
 unified_planning/test/pddl/safe_road/domain.pddl
 unified_planning/test/pddl/safe_road/problem.pddl
 unified_planning/test/pddl/sailing/domain.pddl
 unified_planning/test/pddl/sailing/problem.pddl
 unified_planning/test/pddl/tpp_metric/domain.pddl
```

### Comparing `unified_planning-1.1.0.52.dev1/unified_planning.egg-info/requires.txt` & `unified_planning-1.1.0.9.dev1/unified_planning.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/basic_problems.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/basic_problems.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/classical/metric_problems.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/metric_problems.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/hierarchical/__init__.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/hierarchical/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/depot.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/depot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/logistic.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/logistic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/ma_basic.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/ma_basic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/multiagent/taxi.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/taxi.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/block_grouping.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/block_grouping.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/linear_effects.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/linear_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/problem_basic.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/problem_basic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/sailing/__init__.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/sailing/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/test_01.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_01.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/test_02.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_02.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/construction/test_03.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_03.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/test_01.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_01.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/test_02.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_02.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/builtin/tamp/office/test_03.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_03.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/performance/numeric/block_grouping.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/block_grouping.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/report.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -685,27 +685,19 @@
     else:
         packages = ["builtin", "unified_planning.test"]
         packages.extend(parsed_args.extra_packages)
 
     problem_test_cases = get_test_cases_from_packages(packages)
 
     filters = parsed_args.filters
-    blocks = parsed_args.blocks
     if filters:
+        # Filter only the names that have at least one of the given filters in them
         problem_test_cases = dict(
             filter(
-                lambda name_value: any(p in name_value[0] for p in filters)
-                and all(p not in name_value[0] for p in blocks),
-                problem_test_cases.items(),
-            )
-        )
-    elif blocks:
-        problem_test_cases = dict(
-            filter(
-                lambda name_value: all(p not in name_value[0] for p in blocks),
+                lambda name_value: any(p in name_value[0] for p in filters),
                 problem_test_cases.items(),
             )
         )
 
     timeout: Optional[float] = parsed_args.timeout
     assert timeout is not None
     if timeout <= 0:
```

### Comparing `unified_planning-1.1.0.52.dev1/up_test_cases/utils.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,25 +207,14 @@
         type=str,
         nargs="+",
         help="Runs only the test that contains one of the given filters; if no filters are specified, runs the engines on all the problems.",
         dest="filters",
         default=[],
     )
 
-    parser.add_argument(
-        "-b",
-        "--block",
-        "--blocks",
-        type=str,
-        nargs="+",
-        help="Block all the problems that contain one of the block words; if no blocks are specified, runs the engines on all the problems.",
-        dest="blocks",
-        default=[],
-    )
-
     mutually_exclusive = parser.add_mutually_exclusive_group()
 
     mutually_exclusive.add_argument(
         "-e",
         "--extra-packages",
         type=str,
         nargs="+",
```

