# Comparing `tmp/cpop-35.5.2.tar.gz` & `tmp/cpop-36.0.0.tar.gz`

## Comparing `cpop-35.5.2.tar` & `cpop-36.0.0.tar`

### file list

```diff
@@ -1,180 +1,180 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-35.5.2/.coveragerc
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.5.2/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/__init__.pyx
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/data.pyx
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/exc.pyx
--rw-r--r--   0        0        0    28638 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/hub.pyx
--rw-r--r--   0        0        0    10757 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/ref.pyx
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.5.2/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/config.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/log/basic.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/log/init.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/mods/task.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 cpop-35.5.2/src/pop/mods/test.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_ref.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_relative.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_sub.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/func/test_task.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/bad.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/dunder.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/vtrue.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.5.2/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.5.2/.gitignore
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-35.5.2/README.rst
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.5.2/pyproject.toml
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 cpop-35.5.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-36.0.0/.coveragerc
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-36.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-36.0.0/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/__init__.pyx
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/data.pyx
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    28050 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/hub.pyx
+-rw-r--r--   0        0        0    10757 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-36.0.0/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/config.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/log/basic.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/log/init.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/mods/task.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 cpop-36.0.0/src/pop/mods/test.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_ref.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_relative.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_sub.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/func/test_task.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/bad.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/dunder.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-36.0.0/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-36.0.0/.gitignore
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-36.0.0/README.rst
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-36.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 cpop-36.0.0/PKG-INFO
```

### Comparing `cpop-35.5.2/.pre-commit-config.yaml` & `cpop-36.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/Makefile` & `cpop-36.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/make.bat` & `cpop-36.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/outline.rst` & `cpop-36.0.0/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/conf.py` & `cpop-36.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/index.rst` & `cpop-36.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/app_merging.rst` & `cpop-36.0.0/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/conf.rst` & `cpop-36.0.0/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/conf_integrate.rst` & `cpop-36.0.0/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/contracts.rst` & `cpop-36.0.0/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/dyne_name.rst` & `cpop-36.0.0/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/func_alias.rst` & `cpop-36.0.0/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/glossary.rst` & `cpop-36.0.0/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/hub_overview.rst` & `cpop-36.0.0/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-36.0.0/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/learning.rst` & `cpop-36.0.0/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/pop.rst` & `cpop-36.0.0/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/pre_contract_returns.rst` & `cpop-36.0.0/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/story.rst` & `cpop-36.0.0/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/sub_patterns.rst` & `cpop-36.0.0/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/subs_overview.rst` & `cpop-36.0.0/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/topics/virtual.rst` & `cpop-36.0.0/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/docs/source/tutorial/quickstart.rst` & `cpop-36.0.0/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/__init__.pyx` & `cpop-36.0.0/src/cpop/__init__.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/contract.pyx` & `cpop-36.0.0/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/data.pyx` & `cpop-36.0.0/src/cpop/data.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     def __setattr__(self, key: str, value: object):
         if isinstance(value, dict):
             value = NamespaceDict(value)
         self[key] = value
 
 
 cdef class MultidictCache:
-    cdef dict[str, object] _cache
-    cdef list[dict[str, object]] _base_dicts
-    cdef dict[str, list[str]] _split_cache
-    cdef object _root
+    cdef:
+        dict[str, object] _cache
+        list[dict[str, object]] _base_dicts
+        dict[str, list[str]] _split_cache
+        object _root
 
     def __init__(self, base_dicts=None, parent: object = None):
         if base_dicts is None:
             base_dicts = []
         self._base_dicts = base_dicts
         self._cache = dict[str, object]()
         self._split_cache = dict[str, list[str]]()
@@ -42,14 +43,21 @@
         """
         return self._root
 
     cpdef _clear(self):
         self._cache.clear()
         self._split_cache.clear()
 
+    def __add__(self, search_path: dict[str, object]):
+        """
+        Add the new dictionary to the search base
+        """
+        self._base_dicts.append(search_path)
+        return self
+
     def __getitem__(self, key: str):
         if key in self._cache:
             return self._cache[key]
 
         if key not in self._split_cache:
             self._split_cache[key] = key.split(".")
```

### Comparing `cpop-35.5.2/src/cpop/dirs.pyx` & `cpop-36.0.0/src/cpop/dirs.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/exc.pyx` & `cpop-36.0.0/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/hub.pyx` & `cpop-36.0.0/src/cpop/hub.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,17 @@
 
         # Add the dyne for python imports to live in to the hub
         if "lib" not in self._subs:
             self._subs["lib"] = await AsyncSub(
                 self,
                 subname="lib",
                 dyne_name="lib",
-                # Allow the sub to find python modules dynamically
-                lookup_paths=[sys.modules]
             )
+            # Allow the sub to find python modules dynamically
+            self._subs["lib"] += sys.modules
 
         pop_mods = self.__init_kwargs["pop_mods"]
         if pop_mods is None:
             pop_mods = ["pop.mods"]
         if "pop" not in self._subs:
 
             # Add the pop sub to the hub, this should always use pypath and
@@ -366,15 +366,14 @@
         mod_basename: str = "",
         stop_on_failures: bool = False,
         init: bool = True,
         is_contract: bool = False,
         sub_virtual: bool = True,
         recursive_contracts_static: list[str] = None,
         default_recursive_contracts: list[str] = None,
-        lookup_paths: list[dict] = None,
         parent: object = None,
     ):
         """
         :param hub: The redistributed pop central hub
         :param subname: The name that the sub is going to take on the hub
             if nothing else is passed, it is used as the pypath
         :param pypath: One or many python paths which will be imported
@@ -406,23 +405,18 @@
             if k not in ("self", "hub", "root") and not k.startswith("_")
         }
         subs = {}
         sub_alias = {}
         imports = {}
         loaded = {}
 
-        # tracks what has been setattr-ed on this sub for performance; if something needs to be
-        # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
-        if lookup_paths is None:
-            lookup_paths = []
-
         _root = root or hub
         self._parent = parent or _root
 
-        super().__init__([loaded, imports, subs, sub_alias] + lookup_paths, parent=self._parent)
+        super().__init__([loaded, imports, subs, sub_alias], parent=self._parent)
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._loaded = loaded
         self._reload_mods = {}
         self._alias = []
         self._loaded_all = False
@@ -548,23 +542,17 @@
             elif isinstance(v, Iterable):
                 if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
             elif isinstance(v, cpop.loader.BASE_TYPES):
                 attrs[k] = v
 
         init_kwargs = self.__init_kwargs.copy()
-        lookup_paths = []
-        for dict_ in (init_kwargs.pop("lookup_paths", None) or []):
-            if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in dict_.values()):
-                lookup_paths.append(dict_)
-
-        init_kwargs["lookup_paths"] = lookup_paths
 
         return dict(
-            init_kwargs=lookup_paths,
+            init_kwargs=init_kwargs,
             loaded={
                 item: dict(
                     iface=iface, bname=bname, state=self._loaded[item].__getstate__()
                 )
                 for item, (iface, bname) in self._reload_mods.items()
             },
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
```

### Comparing `cpop-35.5.2/src/cpop/loader.pyx` & `cpop-36.0.0/src/cpop/loader.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/ref.pyx` & `cpop-36.0.0/src/cpop/ref.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/scanner.pyx` & `cpop-36.0.0/src/cpop/scanner.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/cpop/verify.pyx` & `cpop-36.0.0/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/config.yaml` & `cpop-36.0.0/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/log/basic.py` & `cpop-36.0.0/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/log/init.py` & `cpop-36.0.0/src/pop/log/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/log/timed_rolling.py` & `cpop-36.0.0/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/mods/config.py` & `cpop-36.0.0/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/mods/contract.py` & `cpop-36.0.0/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/mods/sub.py` & `cpop-36.0.0/src/pop/mods/sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     omit_vars: bool = False,
     mod_basename: str = "pop.sub",
     stop_on_failures: bool = False,
     init: bool = True,
     recursive_contracts_static: list[str] = None,
     default_recursive_contracts: list[str] = None,
     python_import: str = None,
-    lookup_paths: list[dict] = None,
 ):
     """
     Add a new subsystem to the hub
     :param hub: The redistributed pop central hub
     :param subname: The name that the sub is going to take on the hub
         if nothing else is passed, it is used as the dyne_name
     :param sub: The sub to use as the root to add to
@@ -53,15 +52,14 @@
         Allow plugins to be loaded into a separate namespace.
     :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue loading this sub
     :param init: bool: determine whether or not we process __init__ functions
     :param recursive_contracts_static: Load additional recursive contract paths from a specific directory
     :param default_recursive_contracts: Specifies that a specific recursive contract plugin will be applied as a default
         to all plugins
     :param python_import: Load a module from python onto the sub
-    :param lookup_paths: A list of dictionaries where the Sub will resolve getattr from
     """
     if python_import:
         subname = subname if subname else python_import.split(".")[0]
     if pypath:
         pypath = cpop.hub.ex_path(pypath)
         subname = subname if subname else pypath[0].split(".")[-1]
     elif static:
@@ -96,15 +94,14 @@
         omit_vars=omit_vars,
         mod_basename=mod_basename,
         stop_on_failures=stop_on_failures,
         init=init,
         sub_virtual=getattr(root, "_subvirt", True),
         recursive_contracts_static=recursive_contracts_static,
         default_recursive_contracts=default_recursive_contracts,
-        lookup_paths=lookup_paths,
     )
     # init the sub (init.py:__init__) after it can be referenced on the hub!
     await root._subs[subname]._sub_init()
     await root._subs[subname]._load_all()
     for alias in root._subs[subname]._alias:
         root._sub_alias[alias] = root._subs[subname]
```

### Comparing `cpop-35.5.2/src/pop/mods/task.py` & `cpop-36.0.0/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/src/pop/mods/test.py` & `cpop-36.0.0/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/conftest.py` & `cpop-36.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/contracts/ctx.py` & `cpop-36.0.0/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/contracts/many.py` & `cpop-36.0.0/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/contracts/test.py` & `cpop-36.0.0/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_basic.py` & `cpop-36.0.0/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_config.py` & `cpop-36.0.0/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_contract_ctx.py` & `cpop-36.0.0/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_fail.py` & `cpop-36.0.0/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_log.py` & `cpop-36.0.0/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_no_raise_on_pre_failure.py` & `cpop-36.0.0/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_raise_on_pre_failure.py` & `cpop-36.0.0/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_ref.py` & `cpop-36.0.0/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_relative.py` & `cpop-36.0.0/tests/func/test_relative.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/func/test_serial.py` & `cpop-36.0.0/tests/func/test_serial.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-36.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-36.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/mods/proc.py` & `cpop-36.0.0/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/mods/test.py` & `cpop-36.0.0/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/regression/contract_masking/test_contract_masking.py` & `cpop-36.0.0/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-36.0.0/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/tpath/cn/contract/test.py` & `cpop-36.0.0/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/unit/test_contract.py` & `cpop-36.0.0/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/tests/unit/test_sigs.py` & `cpop-36.0.0/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/.gitignore` & `cpop-36.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/README.rst` & `cpop-36.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.5.2/pyproject.toml` & `cpop-36.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython", "hatch-compile-yaml>=18.0.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "35.5.2"
+version = "36.0.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-35.5.2/PKG-INFO` & `cpop-36.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 35.5.2
+Version: 36.0.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

