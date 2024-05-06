# Comparing `tmp/panda_server-0.3.4.tar.gz` & `tmp/panda_server-0.3.5.tar.gz`

## Comparing `panda_server-0.3.4.tar` & `panda_server-0.3.5.tar`

### file list

```diff
@@ -1,207 +1,206 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.4/ChangeLog.txt
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.4/Dockerfile
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.4/INSTALL.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.4/INSTALL_ATLAS.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.4/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.4/PandaPkgInfo.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.4/panda-server.spec
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.4/package/hatch_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/brokerage/broker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/config_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/daemon_config.py
--rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/config/panda_config.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/Carbon.py
--rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/Configurator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/__init__.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/configurator/aux.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/master.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/master_systemd.py
--rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/cache_pilots.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/cache_schedconfig.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0        0        0    63605 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/AdderSimplePlugin.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/DataServiceUtils.py
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0        0        0     8820 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0        0        0   111777 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/__init__.py
--rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/activator.py
--rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/closer.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/closer_atlas_plugin.py
--rwxr-xr-x   0        0        0    39928 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ddm.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/ddm_handler.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/dyn_data_distributer.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/event_lookup_client_ei.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/event_picker.py
--rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/finisher.py
--rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/dataservice/forkSetupper.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/jobdispatcher/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/proxycache/__init__.py
--rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/proxycache/panda_proxy_cache.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/server/.gacl
--rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/server/panda.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/__init__.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/allowed_methods.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/panda_request.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/srvcore/srv_msg_utils.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0        0        0  1268991 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PickleFileSpec.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PickleJobSpec.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SQLManager.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0        0        0   143604 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/task_split_rules.py
--rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/taskbuffer/workflow_processor.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/SchemaChecker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/banUser.py
--rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/boostPrio.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/boostUser.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/callbackDDM.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/daod_on_demand.py
--rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/finishJob.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/finishTaskJEDI.py
--rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/getJobs.py
--rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killJob.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killTask.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/killUser.py
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignJobs.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignSite.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignTask.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reassignWaiting.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/reloadInputDS.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/setPriority.py
--rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testEvgen.py
--rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testG4sim.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testG4sim17.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testGlobalShares.py
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testReco.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testSiteMap.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/testutils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/README.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/mysetup
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/README.txt
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
--rwxr-xr-x   0        0        0    80304 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/userinterface/Client.py
--rw-r--r--   0        0        0    91604 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/userinterface/UserIF.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/userinterface/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/psnakemake_container.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/psnakemake_task.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/psnakemake_test.py
--rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.4/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/conda_meta.yaml.template
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/panda_server-httpd.conf.rpmnew.template
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/panda_server.cfg.rpmnew.template
--rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/bin/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/bin/panda_server-vomsrenew.exe.template
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/init.d/panda_server.exe.template
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/sysconfig/panda_server_env.systemd.rpmnew.template
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/systemd/panda.service.template
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/systemd/panda_daemon.service.template
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.4/templates/systemd/panda_httpd.service.template
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.4/README.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 panda_server-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 panda_server-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.5/ChangeLog.txt
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.5/Dockerfile
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.5/INSTALL.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.5/INSTALL_ATLAS.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.5/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.5/PandaPkgInfo.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.5/panda-server.spec
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.5/package/hatch_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/config_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/panda_config.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/Carbon.py
+-rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/Configurator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/aux.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/master.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/master_systemd.py
+-rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/cache_pilots.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/cache_schedconfig.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0        0        0    63820 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderSimplePlugin.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/DataServiceUtils.py
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/__init__.py
+-rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/activator.py
+-rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/closer.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/closer_atlas_plugin.py
+-rwxr-xr-x   0        0        0    39936 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ddm.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ddm_handler.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/dyn_data_distributer.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/event_lookup_client_ei.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/event_picker.py
+-rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/finisher.py
+-rwxr-xr-x   0        0        0     7957 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper.py
+-rwxr-xr-x   0        0        0   117529 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper_atlas_plugin.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper_dummy_plugin.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper_plugin_base.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/proxycache/__init__.py
+-rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/proxycache/panda_proxy_cache.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/server/.gacl
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/server/panda.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/allowed_methods.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/panda_request.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/srv_msg_utils.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0        0        0  1268991 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PickleFileSpec.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PickleJobSpec.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SQLManager.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0        0        0   143228 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/task_split_rules.py
+-rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/workflow_processor.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/banUser.py
+-rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/boostUser.py
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/callbackDDM.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/daod_on_demand.py
+-rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/finishJob.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/finishTaskJEDI.py
+-rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/getJobs.py
+-rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killJob.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killTask.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killUser.py
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignJobs.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignSite.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/setPriority.py
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testG4sim.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testG4sim17.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testReco.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testSiteMap.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testutils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/README.txt
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/mysetup
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/README.txt
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
+-rwxr-xr-x   0        0        0    80539 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/userinterface/Client.py
+-rw-r--r--   0        0        0    91540 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/userinterface/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/psnakemake_container.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/psnakemake_task.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/psnakemake_test.py
+-rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/conda_meta.yaml.template
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/panda_server-httpd.conf.rpmnew.template
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/panda_server.cfg.rpmnew.template
+-rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/bin/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/bin/panda_server-vomsrenew.exe.template
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/init.d/panda_server.exe.template
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/systemd/panda.service.template
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/systemd/panda_httpd.service.template
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.5/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.5/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 panda_server-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 panda_server-0.3.5/PKG-INFO
```

### Comparing `panda_server-0.3.4/ChangeLog.txt` & `panda_server-0.3.5/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/Dockerfile` & `panda_server-0.3.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/INSTALL.md` & `panda_server-0.3.5/INSTALL.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/INSTALL_ATLAS.md` & `panda_server-0.3.5/INSTALL_ATLAS.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/panda-server.spec` & `panda_server-0.3.5/panda-server.spec`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/package/hatch_build.py` & `panda_server-0.3.5/package/hatch_build.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/brokerage/SiteMapper.py` & `panda_server-0.3.5/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/brokerage/broker.py` & `panda_server-0.3.5/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/config/daemon_config.py` & `panda_server-0.3.5/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/config/panda_config.py` & `panda_server-0.3.5/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/configurator/Carbon.py` & `panda_server-0.3.5/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/configurator/Configurator.py` & `panda_server-0.3.5/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/configurator/aux.py` & `panda_server-0.3.5/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/master.py` & `panda_server-0.3.5/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/master_systemd.py` & `panda_server-0.3.5/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/utils.py` & `panda_server-0.3.5/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/add_main.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/add_sub.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/add_sub.py`

 * *Files 10% similar despite different names*

```diff
@@ -242,72 +242,14 @@
                     tmp_log.debug(f" killing {str(jediJobs[iJob:iJob + nJob])}")
                     Client.killJobs(jediJobs[iJob : iJob + nJob], 51, keepUnmerged=True)
                     iJob += nJob
     except Exception:
         errStr = traceback.format_exc()
         tmp_log.error(errStr)
 
-    tmp_log.debug("Fork session")
-
-    # thread for fork
-    class ForkThr(threading.Thread):
-        def __init__(self, fileName):
-            threading.Thread.__init__(self)
-            self.fileName = fileName
-
-        def run(self):
-            if "VIRTUAL_ENV" in os.environ:
-                prefix = os.environ["VIRTUAL_ENV"]
-            else:
-                prefix = ""
-            setupStr = f"source {prefix}/etc/sysconfig/panda_server; "
-            runStr = f"{panda_config.native_python}/python -Wignore "
-            runStr += panda_config.pandaPython_dir + "/dataservice/forkSetupper.py -i "
-            runStr += self.fileName
-            if self.fileName.split("/")[-1].startswith("set.NULL."):
-                runStr += " -t"
-            comStr = setupStr + runStr
-            tmp_log.debug(comStr)
-            commands_get_status_output(comStr)
-
-    # get set.* files
-    filePatt = panda_config.logdir + "/" + "set.*"
-    fileList = glob.glob(filePatt)
-
-    # the max number of threads
-    maxThr = 10
-    nThr = 0
-
-    # loop over all files
-    forkThrList = []
-    timeNow = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
-    for tmpName in fileList:
-        if not os.path.exists(tmpName):
-            continue
-        try:
-            # takes care of only recent files
-            mod_time = datetime.datetime(*(time.gmtime(os.path.getmtime(tmpName))[:7]))
-            if datetime.timedelta(minutes=1) < (timeNow - mod_time) < datetime.timedelta(hours=1):
-                cSt, cOut = commands_get_status_output("ps aux | grep fork | grep -v PYTH")
-                # if no process is running for the file
-                if cSt == 0 and tmpName not in cOut:
-                    nThr += 1
-                    thr = ForkThr(tmpName)
-                    thr.start()
-                    forkThrList.append(thr)
-                    if nThr > maxThr:
-                        break
-        except Exception:
-            errType, errValue = sys.exc_info()[:2]
-            tmp_log.error(f"{errType} {errValue}")
-
-    # join fork threads
-    for thr in forkThrList:
-        thr.join()
-
     # stop taskBuffer if created inside this script
     if tbuf is None:
         taskBuffer.cleanup(requester=requester_id)
 
     tmp_log.debug("===================== end =====================")
```

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/cache_pilots.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/cache_pilots.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/cache_schedconfig.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/cache_schedconfig.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/carbon.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/configurator.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/copyArchive.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/copyArchive.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 import math
 import os
 import re
 import sys
 import time
 import traceback
 
-import pandaserver.userinterface.Client as Client
 import requests
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandacommon.pandautils.thread_utils import GenericThread
+from urllib3.exceptions import InsecureRequestWarning
+
+import pandaserver.userinterface.Client as Client
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
 from pandaserver.jobdispatcher.Watcher import Watcher
 from pandaserver.taskbuffer import EventServiceUtils
-from urllib3.exceptions import InsecureRequestWarning
 
 # logger
 _logger = PandaLogger().getLogger("copyArchive")
 
 
 # main
 def main(argv=tuple(), tbuf=None, **kwargs):
@@ -625,47 +626,51 @@
     varMap[":lockedby"] = "jedi"
     varMap[":timeLimit"] = timeLimitJob
     varMap[":prioLimit"] = inactivePrioLimit
     varMap[":pType1"] = "pmerge"
     varMap[":rFlag1"] = 2
     stDS, resDS = taskBuffer.querySQLS(sql, varMap)
     sqlSS = "SELECT laststart FROM ATLAS_PANDAMETA.siteData "
-    sqlSS += "WHERE site=:site AND flag=:flag AND hours=:hours AND laststart<:laststart "
+    sqlSS += "WHERE site=:site AND flag=:flag AND hours=:hours "
     sqlPI = "SELECT PandaID,eventService,attemptNr FROM ATLAS_PANDA.jobsActive4 "
     sqlPI += "WHERE prodSourceLabel=:prodSourceLabel AND jobStatus IN (:jobStatus1,:jobStatus2) "
     sqlPI += "AND (modificationTime<:timeLimit OR stateChangeTime<:timeLimit) "
     sqlPI += "AND lockedby=:lockedby AND currentPriority>=:prioLimit "
     sqlPI += "AND computingSite=:site AND NOT processingType IN (:pType1) AND relocationFlag<>:rFlag1 "
     for (tmpSite,) in resDS:
         if tmpSite in sitesToDisableReassign:
             _logger.debug(f"skip reassignJobs at inactive site {tmpSite} since reassign is disabled")
             continue
         # check if the site is inactive
         varMap = {}
         varMap[":site"] = tmpSite
         varMap[":flag"] = "production"
         varMap[":hours"] = 3
-        varMap[":laststart"] = timeLimitSite
         stSS, resSS = taskBuffer.querySQLS(sqlSS, varMap)
-        if stSS is not None and len(resSS) > 0:
+        if resSS is not None and len(resSS) > 0:
+            last_start = resSS[0][0]
+        else:
+            last_start = None
+        site_status = siteMapper.getSite(tmpSite).status
+        if stSS is True and ((last_start is not None and last_start < timeLimitSite) or site_status in ["offline", "test"]):
             # get jobs
             varMap = {}
             varMap[":prodSourceLabel"] = "managed"
             varMap[":jobStatus1"] = "activated"
             varMap[":jobStatus2"] = "starting"
             varMap[":lockedby"] = "jedi"
             varMap[":timeLimit"] = timeLimitJob
             varMap[":prioLimit"] = inactivePrioLimit
             varMap[":site"] = tmpSite
             varMap[":pType1"] = "pmerge"
             varMap[":rFlag1"] = 2
             stPI, resPI = taskBuffer.querySQLS(sqlPI, varMap)
             jediJobs = []
             # reassign
-            _logger.debug(f"reassignJobs for JEDI at inactive site {tmpSite} laststart={resSS[0][0]}")
+            _logger.debug(f"reassignJobs for JEDI at inactive site {tmpSite} laststart={last_start} status={site_status}")
             if resPI is not None:
                 for pandaID, eventService, attemptNr in resPI:
                     if eventService in [EventServiceUtils.esMergeJobFlagNumber]:
                         _logger.debug(f"retrying es merge {pandaID} at inactive site {tmpSite}")
                         taskBuffer.retryJob(
                             pandaID,
                             {},
```

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/datasetManager.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/datasetManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import os
 import re
 import sys
 import threading
 import time
 import traceback
 
-import pandaserver.taskbuffer.ErrorCode
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandacommon.pandautils.thread_utils import GenericThread
+
+import pandaserver.taskbuffer.ErrorCode
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
 from pandaserver.dataservice import DataServiceUtils
 from pandaserver.dataservice.closer import Closer
 from pandaserver.dataservice.DataServiceUtils import select_scope
 from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.dataservice.finisher import Finisher
@@ -251,15 +252,15 @@
             except Exception:
                 pass
             self.pool.remove(self)
             self.lock.release()
 
     # close datasets
     _logger.debug("==== close datasets ====")
-    timeLimitU = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None) - datetime.timedelta(minutes=30)
+    timeLimitU = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None) - datetime.timedelta(minutes=1)
     timeLimitL = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None) - datetime.timedelta(days=3)
     closeLock = threading.Semaphore(5)
     closeProxyLock = threading.Lock()
     closeThreadPool = ThreadPool()
     maxRows = 100000
     while True:
         # lock
```

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/evpPD2P.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/metric_collector.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/pilotStreaming.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/task_evaluator.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/tmpwatch.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/daemons/scripts/worker_synchronization.py` & `panda_server-0.3.5/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda_server-0.3.5/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/AdderGen.py` & `panda_server-0.3.5/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/AdderResult.py` & `panda_server-0.3.5/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/AdderSimplePlugin.py` & `panda_server-0.3.5/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/DataServiceUtils.py` & `panda_server-0.3.5/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/ProcessLimiter.py` & `panda_server-0.3.5/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda_server-0.3.5/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/Setupper.py` & `panda_server-0.3.5/pandaserver/dataservice/setupper.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,223 +2,204 @@
 setup dataset
 
 """
 
 import sys
 import threading
 import traceback
-import uuid
+from typing import List
 
 from pandacommon.pandalogger.LogWrapper import LogWrapper
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandaserver.config import panda_config
 from pandaserver.taskbuffer import EventServiceUtils
 from pandaserver.taskbuffer.PickleJobSpec import PickleJobSpec
 
 # logger
-_logger = PandaLogger().getLogger("Setupper")
+_logger = PandaLogger().getLogger("setupper")
 
 panda_config.setupPlugin()
 
 
 # main class
 class Setupper(threading.Thread):
+    """
+    Main class for setting up the dataset.
+    """
     # constructor
     def __init__(
         self,
         taskBuffer,
-        jobs,
-        resubmit=False,
-        pandaDDM=False,
-        ddmAttempt=0,
-        forkRun=False,
-        onlyTA=False,
-        resetLocation=False,
-        firstSubmission=True,
+        jobs: List[object],
+        resubmit: bool = False,
+        panda_ddm: bool = False,
+        ddm_attempt: int = 0,
+        only_ta: bool = False,
+        first_submission: bool = True,
     ):
+        """
+        Constructor for the Setupper class.
+
+        :param taskBuffer: The buffer for tasks.
+        :param jobs: The jobs to be processed.
+        :param resubmit: A flag to indicate if the job is a resubmission. Defaults to False.
+        :param panda_ddm: A flag to indicate if PandaDDM is used. Defaults to False.
+        :param ddm_attempt: The number of attempts for DDM job. Defaults to 0.
+        :param only_ta: A flag to indicate if only task assignment should be run. Defaults to False.
+        :param first_submission: A flag to indicate if it's the first submission. Defaults to True.
+        """
         threading.Thread.__init__(self)
         self.jobs = jobs
-        self.taskBuffer = taskBuffer
+        self.task_buffer = taskBuffer
         # resubmission or not
         self.resubmit = resubmit
         # use PandaDDM
-        self.pandaDDM = pandaDDM
+        self.panda_ddm = panda_ddm
         # priority for ddm job
-        self.ddmAttempt = ddmAttempt
-        # fork another process because python doesn't release memory
-        self.forkRun = forkRun
+        self.ddm_attempt = ddm_attempt
         # run task assignment only
-        self.onlyTA = onlyTA
-        # reset locations
-        self.resetLocation = resetLocation
+        self.only_ta = only_ta
         # first submission
-        self.firstSubmission = firstSubmission
+        self.first_submission = first_submission
 
     # main
-    def run(self):
+    def run(self) -> None:
+        """
+        Main method for running the setup process.
+        """
         try:
             # make a message instance
-            tmpLog = LogWrapper(_logger, None)
+            tmp_log = LogWrapper(_logger, None)
             # run main procedure in the same process
-            if not self.forkRun:
-                tmpLog.debug("main start")
-                tmpLog.debug(f"firstSubmission={self.firstSubmission}")
-                # make Specs pickleable
-                p_job_list = []
-                for job_spec in self.jobs:
-                    p_job = PickleJobSpec()
-                    p_job.update(job_spec)
-                    p_job_list.append(p_job)
-                self.jobs = p_job_list
-                # group jobs per VO
-                voJobsMap = {}
-                ddmFreeJobs = []
-                tmpLog.debug(f"{len(self.jobs)} jobs in total")
-                for tmpJob in self.jobs:
-                    # set VO=local for DDM free
-                    if tmpJob.destinationSE == "local":
-                        tmpVO = "local"
-                    else:
-                        tmpVO = tmpJob.VO
-                    # make map
-                    voJobsMap.setdefault(tmpVO, [])
-                    voJobsMap[tmpVO].append(tmpJob)
-                # loop over all VOs
-                for tmpVO in voJobsMap:
-                    tmpJobList = voJobsMap[tmpVO]
-                    tmpLog.debug(f"vo={tmpVO} has {len(tmpJobList)} jobs")
-                    # get plugin
-                    setupperPluginClass = panda_config.getPlugin("setupper_plugins", tmpVO)
-                    if setupperPluginClass is None:
-                        # use ATLAS plug-in by default
-                        from pandaserver.dataservice.SetupperAtlasPlugin import (
-                            SetupperAtlasPlugin,
-                        )
-
-                        setupperPluginClass = SetupperAtlasPlugin
-                    tmpLog.debug(f"plugin name -> {setupperPluginClass.__name__}")
-                    try:
-                        # make plugin
-                        setupperPlugin = setupperPluginClass(
-                            self.taskBuffer,
-                            self.jobs,
-                            tmpLog,
-                            resubmit=self.resubmit,
-                            pandaDDM=self.pandaDDM,
-                            ddmAttempt=self.ddmAttempt,
-                            onlyTA=self.onlyTA,
-                            firstSubmission=self.firstSubmission,
-                        )
-                        # run plugin
-                        tmpLog.debug("run plugin")
-                        setupperPlugin.run()
-                        # go forward if not TA
-                        if not self.onlyTA:
-                            # update jobs
-                            tmpLog.debug("update jobs")
-                            self.updateJobs(setupperPlugin.jobs + setupperPlugin.jumboJobs, tmpLog)
-                            # execute post process
-                            tmpLog.debug("post execute plugin")
-                            setupperPlugin.postRun()
-                        tmpLog.debug("done plugin")
-                    except Exception:
-                        errtype, errvalue = sys.exc_info()[:2]
-                        tmpLog.error(f"plugin failed with {errtype}:{errvalue}")
-                tmpLog.debug("main end")
-            else:
-                tmpLog.debug("fork start")
-                # write jobs to file
-                import os
-
+            tmp_log.debug("main start")
+            tmp_log.debug(f"first_submission={self.first_submission}")
+            # make Specs pickleable
+            p_job_list = []
+            for job_spec in self.jobs:
+                p_job = PickleJobSpec()
+                p_job.update(job_spec)
+                p_job_list.append(p_job)
+            self.jobs = p_job_list
+            # group jobs per VO
+            vo_jobs_map = {}
+            tmp_log.debug(f"{len(self.jobs)} jobs in total")
+            for tmp_job in self.jobs:
+                # set VO=local for DDM free
+                if tmp_job.destinationSE == "local":
+                    tmp_vo = "local"
+                else:
+                    tmp_vo = tmp_job.VO
+                # make map
+                vo_jobs_map.setdefault(tmp_vo, [])
+                vo_jobs_map[tmp_vo].append(tmp_job)
+            # loop over all VOs
+            for tmp_vo in vo_jobs_map:
+                tmp_job_list = vo_jobs_map[tmp_vo]
+                tmp_log.debug(f"vo={tmp_vo} has {len(tmp_job_list)} jobs")
+                # get plugin
+                setupper_plugin_class = panda_config.getPlugin("setupper_plugins", tmp_vo)
+                if setupper_plugin_class is None:
+                    # use ATLAS plug-in by default
+                    from pandaserver.dataservice.setupper_atlas_plugin import SetupperAtlasPlugin
+                    setupper_plugin_class = SetupperAtlasPlugin
+                tmp_log.debug(f"plugin name -> {setupper_plugin_class.__name__}")
                 try:
-                    import cPickle as pickle
-                except ImportError:
-                    import pickle
-                outFileName = f"{panda_config.logdir}/set.{self.jobs[0].PandaID}_{str(uuid.uuid4())}"
-                outFile = open(outFileName, "wb")
-                pickle.dump(self.jobs, outFile, protocol=0)
-                outFile.close()
-                # run main procedure in another process because python doesn't release memory
-                com = f"cd {panda_config.home_dir_cwd} > /dev/null 2>&1; export HOME={panda_config.home_dir_cwd}; "
-                com += "env PYTHONPATH=%s:%s %s/python -Wignore %s/dataservice/forkSetupper.py -i %s" % (
-                    panda_config.pandaCommon_dir,
-                    panda_config.pandaPython_dir,
-                    panda_config.native_python,
-                    panda_config.pandaPython_dir,
-                    outFileName,
-                )
-                if self.onlyTA:
-                    com += " -t"
-                if not self.firstSubmission:
-                    com += " -f"
-                tmpLog.debug(com)
-                # execute
-                status, output = self.taskBuffer.processLimiter.getstatusoutput(com)
-                tmpLog.debug(f"return from main process: {status} {output}")
-                tmpLog.debug("fork end")
-        except Exception as e:
-            tmpLog.error(f"master failed with {str(e)} {traceback.format_exc()}")
+                    # make plugin
+                    setupper_plugin = setupper_plugin_class(
+                        self.task_buffer,
+                        self.jobs,
+                        tmp_log,
+                        resubmit=self.resubmit,
+                        panda_ddm=self.panda_ddm,
+                        ddm_attempt=self.ddm_attempt,
+                        only_ta=self.only_ta,
+                        first_submission=self.first_submission,
+                    )
+                    # run plugin
+                    tmp_log.debug("run plugin")
+                    setupper_plugin.run()
+                    # go forward if not Task Assignment
+                    if not self.only_ta:
+                        # update jobs
+                        tmp_log.debug("update jobs")
+                        self.update_jobs(setupper_plugin.jobs + setupper_plugin.jumbo_jobs, tmp_log)
+                        # execute post process
+                        tmp_log.debug("post execute plugin")
+                        setupper_plugin.post_run()
+                    tmp_log.debug("done plugin")
+                except Exception:
+                    error_type, error_value = sys.exc_info()[:2]
+                    tmp_log.error(f"plugin failed with {error_type}:{error_value}")
+            tmp_log.debug("main end")
+        except Exception as error:
+            tmp_log.error(f"master failed with {str(error)} {traceback.format_exc()}")
 
     #  update jobs
-    def updateJobs(self, jobList, tmpLog):
-        updateJobs = []
-        failedJobs = []
-        activateJobs = []
-        waitingJobs = []
-        closeJobs = []
-        # sort out jobs
-        for job in jobList:
+    def update_jobs(self, job_list: List[object], tmp_log: LogWrapper) -> None:
+        """
+        Updates the status of jobs.
+
+        :param job_list: The list of jobs to be updated.
+        :param log: The logger to be used for logging.
+        """
+        update_jobs = []
+        failed_jobs = []
+        activate_jobs = []
+        waiting_jobs = []
+        # sort jobs by status
+        for job in job_list:
             # failed jobs
             if job.jobStatus in ["failed", "cancelled"]:
-                failedJobs.append(job)
+                failed_jobs.append(job)
             # waiting
             elif job.jobStatus == "waiting":
-                waitingJobs.append(job)
+                waiting_jobs.append(job)
             # no input jobs
             elif job.dispatchDBlock == "NULL":
-                activateJobs.append(job)
+                activate_jobs.append(job)
             # normal jobs
             else:
                 # change status
                 job.jobStatus = "assigned"
-                updateJobs.append(job)
+                update_jobs.append(job)
+
         # trigger merge generation if all events are done
-        newActivateJobs = []
-        nFinished = 0
-        for job in activateJobs:
+        new_activate_jobs = []
+        n_finished = 0
+        for job in activate_jobs:
             if job.notDiscardEvents() and job.allOkEvents() and not EventServiceUtils.isEventServiceMerge(job):
-                self.taskBuffer.activateJobs([job])
+                self.task_buffer.updateJobs([job])
                 # change status
                 job.jobStatus = "finished"
-                self.taskBuffer.updateJobs([job], False)
-                nFinished += 1
+                self.task_buffer.updateJobs([job], False)
+                n_finished += 1
             else:
-                newActivateJobs.append(job)
-        activateJobs = newActivateJobs
-        tmpLog.debug(f"# of finished jobs in activated : {nFinished}")
-        newUpdateJobs = []
-        nFinished = 0
-        for job in updateJobs:
+                new_activate_jobs.append(job)
+        activate_jobs = new_activate_jobs
+        tmp_log.debug(f"# of finished jobs in activated : {n_finished}")
+        new_update_jobs = []
+        n_finished = 0
+        for job in update_jobs:
             if job.notDiscardEvents() and job.allOkEvents() and not EventServiceUtils.isEventServiceMerge(job):
-                self.taskBuffer.updateJobs([job], True)
+                self.task_buffer.updateJobs([job], True)
                 # change status
                 job.jobStatus = "finished"
-                self.taskBuffer.updateJobs([job], True)
-                nFinished += 1
+                self.task_buffer.updateJobs([job], True)
+                n_finished += 1
             else:
-                newUpdateJobs.append(job)
-        updateJobs = newUpdateJobs
-        tmpLog.debug(f"# of finished jobs in defined : {nFinished}")
+                new_update_jobs.append(job)
+        update_jobs = new_update_jobs
+        tmp_log.debug(f"# of finished jobs in defined : {n_finished}")
         # update DB
-        tmpLog.debug(f"# of activated jobs : {len(activateJobs)}")
-        self.taskBuffer.activateJobs(activateJobs)
-        tmpLog.debug(f"# of updated jobs : {len(updateJobs)}")
-        self.taskBuffer.updateJobs(updateJobs, True)
-        tmpLog.debug(f"# of failed jobs : {len(failedJobs)}")
-        self.taskBuffer.updateJobs(failedJobs, True)
-        tmpLog.debug(f"# of waiting jobs : {len(waitingJobs)}")
-        self.taskBuffer.keepJobs(waitingJobs)
+        tmp_log.debug(f"# of activated jobs : {len(activate_jobs)}")
+        self.task_buffer.activateJobs(activate_jobs)
+        tmp_log.debug(f"# of updated jobs : {len(update_jobs)}")
+        self.task_buffer.updateJobs(update_jobs, True)
+        tmp_log.debug(f"# of failed jobs : {len(failed_jobs)}")
+        self.task_buffer.updateJobs(failed_jobs, True)
+        tmp_log.debug(f"# of waiting jobs : {len(waiting_jobs)}")
+        self.task_buffer.keepJobs(waiting_jobs)
         # delete local values
-        del updateJobs
-        del failedJobs
-        del activateJobs
-        del waitingJobs
+        del update_jobs
+        del failed_jobs
+        del activate_jobs
+        del waiting_jobs
```

### Comparing `panda_server-0.3.4/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda_server-0.3.5/pandaserver/dataservice/setupper_atlas_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,2152 +6,2224 @@
 import datetime
 import re
 import sys
 import time
 import traceback
 import uuid
 
+from typing import List, Dict, Tuple, Optional
+from rucio.common.exception import DataIdentifierNotFound
+
 import pandaserver.brokerage.broker
+
 from pandaserver.brokerage.SiteMapper import SiteMapper
-from pandaserver.config import panda_config
 from pandaserver.dataservice import DataServiceUtils, ErrorCode
 from pandaserver.dataservice.DataServiceUtils import select_scope
 from pandaserver.dataservice.ddm import rucioAPI
-from pandaserver.dataservice.SetupperPluginBase import SetupperPluginBase
+from pandaserver.dataservice.setupper_plugin_base import SetupperPluginBase
 from pandaserver.taskbuffer import EventServiceUtils, JobUtils
 from pandaserver.taskbuffer.DatasetSpec import DatasetSpec
-from rucio.common.exception import (
-    DataIdentifierAlreadyExists,
-    DataIdentifierNotFound,
-    Duplicate,
-    FileAlreadyExists,
-)
+
 
 
 class SetupperAtlasPlugin(SetupperPluginBase):
+    """
+    setup dataset for ATLAS
+
+    """
     # constructor
-    def __init__(self, taskBuffer, jobs, logger, **params):
+    def __init__(self, taskBuffer, jobs: List, logger, **params: Dict) -> None:
+        """
+        Constructor for the SetupperAtlasPlugin class.
+
+        :param taskBuffer: The buffer for tasks.
+        :param jobs: The jobs to be processed.
+        :param logger: The logger to be used for logging.
+        :param params: Additional parameters.
+        """
         # defaults
-        defaultMap = {
+        default_map = {
             "resubmit": False,
-            "pandaDDM": False,
-            "ddmAttempt": 0,
-            "onlyTA": False,
-            "resetLocation": False,
-            "useNativeDQ2": True,
+            "panda_ddm": False,
+            "ddm_attempt": 0,
+            "only_ta": False,
         }
-        SetupperPluginBase.__init__(self, taskBuffer, jobs, logger, params, defaultMap)
+        SetupperPluginBase.__init__(self, taskBuffer, jobs, logger, params, default_map)
         # VUIDs of dispatchDBlocks
-        self.vuidMap = {}
+        self.vuid_map = {}
         # file list for dispDS for PandaDDM
-        self.dispFileList = {}
+        self.disp_file_list = {}
         # site mapper
-        self.siteMapper = None
+        self.site_mapper = None
         # location map
-        self.replicaMap = {}
+        self.replica_map = {}
         # all replica locations
-        self.allReplicaMap = {}
+        self.all_replica_map = {}
         # replica map for special brokerage
-        self.replicaMapForBroker = {}
+        self.replica_map_for_broker = {}
         # available files at T2
-        self.availableLFNsInT2 = {}
+        self.available_lfns_in_t2 = {}
         # list of missing datasets
-        self.missingDatasetList = {}
+        self.missing_dataset_list = {}
         # lfn ds map
-        self.lfnDatasetMap = {}
+        self.lfn_dataset_map = {}
         # missing files at T1
-        self.missingFilesInT1 = {}
+        self.missing_files_in_t1 = {}
         # source label
-        self.prodSourceLabel = None
+        self.prod_source_label = None
         self.job_label = None
 
     # main
-    def run(self):
+    def run(self) -> None:
+        """
+        Main method for running the setup process.
+        """
         try:
             self.logger.debug("start run()")
-            self._memoryCheck()
-            bunchTag = ""
-            tagJob = None
-            timeStart = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
+            self.memory_check()
+            bunch_tag = ""
+            tag_job = None
+            time_start = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
             if self.jobs is not None and len(self.jobs) > 0:
-                tagJob = self.jobs[0]
-            elif len(self.jumboJobs) > 0:
-                tagJob = self.jumboJobs[0]
-            if tagJob is not None:
-                bunchTag = f"PandaID:{tagJob.PandaID} type:{tagJob.prodSourceLabel} taskID:{tagJob.taskID} pType={tagJob.processingType}"
-                self.logger.debug(bunchTag)
-                self.prodSourceLabel = tagJob.prodSourceLabel
-                self.job_label = tagJob.job_label
+                tag_job = self.jobs[0]
+            elif len(self.jumbo_jobs) > 0:
+                tag_job = self.jumbo_jobs[0]
+            if tag_job is not None:
+                bunch_tag = f"PandaID:{tag_job.PandaID} type:{tag_job.prodSourceLabel} taskID:{tag_job.taskID} pType={tag_job.processingType}"
+                self.logger.debug(bunch_tag)
+                self.prod_source_label = tag_job.prodSourceLabel
+                self.job_label = tag_job.job_label
             # instantiate site mapper
-            self.siteMapper = SiteMapper(self.taskBuffer)
+            self.site_mapper = SiteMapper(self.task_buffer)
             # correctLFN
-            self._correctLFN()
+            self.correct_lfn()
             # run full Setupper
-            if not self.onlyTA:
+            if not self.only_ta:
                 # invoke brokerage
                 self.logger.debug("brokerSchedule")
-                self._memoryCheck()
+                self.memory_check()
                 pandaserver.brokerage.broker.schedule(
                     self.jobs,
-                    self.taskBuffer,
-                    self.siteMapper,
-                    replicaMap=self.replicaMapForBroker,
-                    t2FilesMap=self.availableLFNsInT2,
+                    self.task_buffer,
+                    self.site_mapper,
+                    replicaMap=self.replica_map_for_broker,
+                    t2FilesMap=self.available_lfns_in_t2,
                 )
                 # remove waiting jobs
-                self.removeWaitingJobs()
+                self.remove_waiting_jobs()
                 # setup dispatch dataset
                 self.logger.debug("setupSource")
-                self._memoryCheck()
-                self._setupSource()
-                self._memoryCheck()
+                self.memory_check()
+                self.setup_source()
+                self.memory_check()
                 # sort by site so that larger subs are created in the next step
                 if self.jobs != [] and self.jobs[0].prodSourceLabel in [
                     "managed",
                     "test",
                 ]:
-                    tmpJobMap = {}
-                    for tmpJob in self.jobs:
+                    tmp_job_map = {}
+                    for tmp_job in self.jobs:
                         # add site
-                        if tmpJob.computingSite not in tmpJobMap:
-                            tmpJobMap[tmpJob.computingSite] = []
+                        if tmp_job.computingSite not in tmp_job_map:
+                            tmp_job_map[tmp_job.computingSite] = []
                         # add job
-                        tmpJobMap[tmpJob.computingSite].append(tmpJob)
+                        tmp_job_map[tmp_job.computingSite].append(tmp_job)
                     # make new list
-                    tmpJobList = []
-                    for tmpSiteKey in tmpJobMap:
-                        tmpJobList += tmpJobMap[tmpSiteKey]
+                    tmp_job_list = []
+                    for jobs in tmp_job_map.values():
+                        tmp_job_list += jobs
                     # set new list
-                    self.jobs = tmpJobList
+                    self.jobs = tmp_job_list
                 # create dataset for outputs and assign destination
                 if self.jobs != [] and self.jobs[0].prodSourceLabel in [
                     "managed",
                     "test",
                 ]:
                     # count the number of jobs per _dis
-                    iBunch = 0
-                    prevDisDsName = None
-                    nJobsPerDisList = []
-                    for tmpJob in self.jobs:
-                        if prevDisDsName is not None and prevDisDsName != tmpJob.dispatchDBlock:
-                            nJobsPerDisList.append(iBunch)
-                            iBunch = 0
+                    i_bunch = 0
+                    prev_dis_ds_name = None
+                    n_jobs_per_dis_list = []
+                    for tmp_job in self.jobs:
+                        if prev_dis_ds_name is not None and prev_dis_ds_name != tmp_job.dispatchDBlock:
+                            n_jobs_per_dis_list.append(i_bunch)
+                            i_bunch = 0
                         # increment
-                        iBunch += 1
+                        i_bunch += 1
                         # set _dis name
-                        prevDisDsName = tmpJob.dispatchDBlock
+                        prev_dis_ds_name = tmp_job.dispatchDBlock
                     # remaining
-                    if iBunch != 0:
-                        nJobsPerDisList.append(iBunch)
+                    if i_bunch != 0:
+                        n_jobs_per_dis_list.append(i_bunch)
                     # split sub datasets
-                    iBunch = 0
-                    nBunchMax = 50
-                    tmpIndexJob = 0
-                    for nJobsPerDis in nJobsPerDisList:
+                    i_bunch = 0
+                    n_bunch_max = 50
+                    tmp_index_job = 0
+                    for n_jobs_per_dis in n_jobs_per_dis_list:
                         # check _dis boundary so that the same _dis doesn't contribute to many _subs
-                        if iBunch + nJobsPerDis > nBunchMax:
-                            if iBunch != 0:
-                                self._setupDestination(startIdx=tmpIndexJob, nJobsInLoop=iBunch)
-                                tmpIndexJob += iBunch
-                                iBunch = 0
+                        if i_bunch + n_jobs_per_dis > n_bunch_max:
+                            if i_bunch != 0:
+                                self.setup_destination(start_idx=tmp_index_job, n_jobs_in_loop=i_bunch)
+                                tmp_index_job += i_bunch
+                                i_bunch = 0
                         # increment
-                        iBunch += nJobsPerDis
+                        i_bunch += n_jobs_per_dis
                     # remaining
-                    if iBunch != 0:
-                        self._setupDestination(startIdx=tmpIndexJob, nJobsInLoop=iBunch)
+                    if i_bunch != 0:
+                        self.setup_destination(start_idx=tmp_index_job, n_jobs_in_loop=i_bunch)
                 else:
                     # make one sub per job so that each job doesn't have to wait for others to be done
                     if self.jobs != [] and self.jobs[0].prodSourceLabel in ["user", "panda"] and self.jobs[-1].currentPriority > 6000:
-                        for iBunch in range(len(self.jobs)):
-                            self._setupDestination(startIdx=iBunch, nJobsInLoop=1)
+                        for i_bunch in range(len(self.jobs)):
+                            self.setup_destination(start_idx=i_bunch, n_jobs_in_loop=1)
                     else:
                         # at a burst
-                        self._setupDestination()
+                        self.setup_destination()
                 # make dis datasets for existing files
-                self._memoryCheck()
-                self._makeDisDatasetsForExistingfiles()
-                self._memoryCheck()
+                self.memory_check()
+                self.make_dis_datasets_for_existing_files()
+                self.memory_check()
                 # setup jumbo jobs
-                self._setupJumbojobs()
-                self._memoryCheck()
-            regTime = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None) - timeStart
-            self.logger.debug(f"{bunchTag} took {regTime.seconds}sec")
+                self.setup_jumbo_jobs()
+                self.memory_check()
+            reg_time = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None) - time_start
+            self.logger.debug(f"{bunch_tag} took {reg_time.seconds}sec")
             self.logger.debug("end run()")
         except Exception:
-            errtype, errvalue = sys.exc_info()[:2]
-            errStr = f"run() : {errtype} {errvalue}"
-            errStr.strip()
-            errStr += traceback.format_exc()
-            self.logger.error(errStr)
+            error_type, error_value = sys.exc_info()[:2]
+            err_str = f"run() : {error_type} {error_value}"
+            err_str.strip()
+            err_str += traceback.format_exc()
+            self.logger.error(err_str)
 
     # post run
-    def postRun(self):
+    def post_run(self) -> None:
+        """
+        Post run method for running the setup process.
+        """
         try:
-            if not self.onlyTA:
+            if not self.only_ta:
                 self.logger.debug("start postRun()")
-                self._memoryCheck()
-                # subscribe sites distpatchDBlocks. this must be the last method
-                self.logger.debug("subscribeDistpatchDB")
-                self._subscribeDistpatchDB()
+                self.memory_check()
+                # subscribe sites dispatchDBlocks. this must be the last method
+                self.logger.debug("subscribeDispatchDB")
+                self.subscribe_dispatch_data_block()
                 # dynamic data placement for analysis jobs
-                self._memoryCheck()
-                self._dynamicDataPlacement()
+                self.memory_check()
+                self.dynamic_data_placement()
                 # make subscription for missing
-                self._memoryCheck()
-                self._makeSubscriptionForMissing()
-                self._memoryCheck()
+                self.memory_check()
+                self.make_subscription_for_missing()
+                self.memory_check()
                 self.logger.debug("end postRun()")
         except Exception:
-            errtype, errvalue = sys.exc_info()[:2]
-            self.logger.error(f"postRun() : {errtype} {errvalue}")
+            error_type, error_value = sys.exc_info()[:2]
+            self.logger.error(f"postRun() : {error_type} {error_value}")
 
     # make dispatchDBlocks, insert prod/dispatchDBlock to database
-    def _setupSource(self):
-        fileList = {}
-        prodList = []
-        prodError = {}
-        dispSiteMap = {}
-        dispError = {}
-        backEndMap = {}
-        dsTaskMap = dict()
-        useZipToPinMap = dict()
+    def setup_source(self) -> None:
+        """
+        Setup source method for running the setup process.
+        """
+        file_list = {}
+        prod_list = []
+        prod_error = {}
+        disp_site_map = {}
+        disp_error = {}
+        back_end_map = {}
+        ds_task_map = dict()
+        use_zip_to_pin_map = dict()
         # extract prodDBlock
         for job in self.jobs:
             # ignore failed jobs
             if job.jobStatus in ["failed", "cancelled"] or job.isCancelled():
                 continue
             # production datablock
             if job.prodDBlock != "NULL" and job.prodDBlock and (job.prodSourceLabel not in ["user", "panda"]):
                 # get VUID and record prodDBlock into DB
-                if job.prodDBlock not in prodError:
+                if job.prodDBlock not in prod_error:
                     self.logger.debug("listDatasets " + job.prodDBlock)
-                    prodError[job.prodDBlock] = ""
-                    for iDDMTry in range(3):
-                        newOut, errMsg = rucioAPI.list_datasets(job.prodDBlock)
-                        if newOut is None:
+                    prod_error[job.prodDBlock] = ""
+                    for attempt in range(3):
+                        new_out, err_msg = rucioAPI.list_datasets(job.prodDBlock)
+                        if new_out is None:
                             time.sleep(10)
                         else:
                             break
-                    if newOut is None:
-                        prodError[job.prodDBlock] = f"Setupper._setupSource() could not get VUID of prodDBlock with {errMsg}"
-                        self.logger.error(prodError[job.prodDBlock])
+                    if new_out is None:
+                        prod_error[job.prodDBlock] = f"Setupper._setupSource() could not get VUID of prodDBlock with {err_msg}"
+                        self.logger.error(prod_error[job.prodDBlock])
                     else:
-                        self.logger.debug(newOut)
+                        self.logger.debug(new_out)
                         try:
-                            vuids = newOut[job.prodDBlock]["vuids"]
-                            nfiles = 0
+                            vuids = new_out[job.prodDBlock]["vuids"]
+                            n_files = 0
                             # dataset spec
-                            ds = DatasetSpec()
-                            ds.vuid = vuids[0]
-                            ds.name = job.prodDBlock
-                            ds.type = "input"
-                            ds.status = "completed"
-                            ds.numberfiles = nfiles
-                            ds.currentfiles = nfiles
-                            prodList.append(ds)
+                            dataset = DatasetSpec()
+                            dataset.vuid = vuids[0]
+                            dataset.name = job.prodDBlock
+                            dataset.type = "input"
+                            dataset.status = "completed"
+                            dataset.numberfiles = n_files
+                            dataset.currentfiles = n_files
+                            prod_list.append(dataset)
                         except Exception:
-                            errtype, errvalue = sys.exc_info()[:2]
-                            self.logger.error(f"_setupSource() : {errtype} {errvalue}")
-                            prodError[job.prodDBlock] = "Setupper._setupSource() could not decode VUID of prodDBlock"
+                            error_type, error_value = sys.exc_info()[:2]
+                            self.logger.error(f"_setupSource() : {error_type} {error_value}")
+                            prod_error[job.prodDBlock] = "Setupper._setupSource() could not decode VUID of prodDBlock"
                 # error
-                if prodError[job.prodDBlock] != "":
+                if prod_error[job.prodDBlock] != "":
                     if job.jobStatus != "failed":
                         job.jobStatus = "failed"
                         job.ddmErrorCode = ErrorCode.EC_Setupper
-                        job.ddmErrorDiag = prodError[job.prodDBlock]
+                        job.ddmErrorDiag = prod_error[job.prodDBlock]
                         self.logger.debug(f"failed PandaID={job.PandaID} with {job.ddmErrorDiag}")
                     continue
             # dispatch datablock
             if job.dispatchDBlock != "NULL":
                 # useZipToPin mapping
-                useZipToPinMap[job.dispatchDBlock] = job.useZipToPin()
+                use_zip_to_pin_map[job.dispatchDBlock] = job.useZipToPin()
                 # src/dst sites
-                tmpSrcID = "BNL_ATLAS_1"
-                if self.siteMapper.checkCloud(job.getCloud()):
+                tmp_src_id = "BNL_ATLAS_1"
+                if self.site_mapper.checkCloud(job.getCloud()):
                     # use cloud's source
-                    tmpSrcID = self.siteMapper.getCloud(job.getCloud())["source"]
+                    tmp_src_id = self.site_mapper.getCloud(job.getCloud())["source"]
 
-                srcSiteSpec = self.siteMapper.getSite(tmpSrcID)
-                scope_src_input, scope_src_output = select_scope(srcSiteSpec, job.prodSourceLabel, job.job_label)
-                srcDQ2ID = srcSiteSpec.ddm_output[scope_src_output]
-                # use srcDQ2ID as dstDQ2ID when it is associated to dest
-                dstSiteSpec = self.siteMapper.getSite(job.computingSite)
-                scope_dst_input, scope_dst_output = select_scope(dstSiteSpec, job.prodSourceLabel, job.job_label)
-                if dstSiteSpec.ddm_endpoints_input[scope_dst_input].isAssociated(srcDQ2ID):
-                    dstDQ2ID = srcDQ2ID
+                src_site_spec = self.site_mapper.getSite(tmp_src_id)
+                _, scope_src_output = select_scope(src_site_spec, job.prodSourceLabel, job.job_label)
+                src_ddm_id = src_site_spec.ddm_output[scope_src_output]
+                # use src_ddm_id as dst_ddm_id when it is associated to dest
+                dst_site_spec = self.site_mapper.getSite(job.computingSite)
+                scope_dst_input, _ = select_scope(dst_site_spec, job.prodSourceLabel, job.job_label)
+                if dst_site_spec.ddm_endpoints_input[scope_dst_input].isAssociated(src_ddm_id):
+                    dst_ddm_id = src_ddm_id
                 else:
-                    dstDQ2ID = dstSiteSpec.ddm_input[scope_dst_input]
-                dispSiteMap[job.dispatchDBlock] = {
-                    "src": srcDQ2ID,
-                    "dst": dstDQ2ID,
+                    dst_ddm_id = dst_site_spec.ddm_input[scope_dst_input]
+                disp_site_map[job.dispatchDBlock] = {
+                    "src": src_ddm_id,
+                    "dst": dst_ddm_id,
                     "site": job.computingSite,
                 }
                 # filelist
-                if job.dispatchDBlock not in fileList:
-                    fileList[job.dispatchDBlock] = {
+                if job.dispatchDBlock not in file_list:
+                    file_list[job.dispatchDBlock] = {
                         "lfns": [],
                         "guids": [],
                         "fsizes": [],
                         "md5sums": [],
                         "chksums": [],
                     }
-                    dsTaskMap[job.dispatchDBlock] = job.jediTaskID
+                    ds_task_map[job.dispatchDBlock] = job.jediTaskID
                 # DDM backend
-                if job.dispatchDBlock not in backEndMap:
-                    backEndMap[job.dispatchDBlock] = "rucio"
+                if job.dispatchDBlock not in back_end_map:
+                    back_end_map[job.dispatchDBlock] = "rucio"
                 # collect LFN and GUID
                 for file in job.Files:
                     if file.type == "input" and file.status == "pending":
-                        if backEndMap[job.dispatchDBlock] != "rucio":
-                            tmpLFN = file.lfn
+                        if back_end_map[job.dispatchDBlock] != "rucio":
+                            tmp_lfn = file.lfn
                         else:
-                            tmpLFN = f"{file.scope}:{file.lfn}"
-                        if tmpLFN not in fileList[job.dispatchDBlock]["lfns"]:
-                            fileList[job.dispatchDBlock]["lfns"].append(tmpLFN)
-                            fileList[job.dispatchDBlock]["guids"].append(file.GUID)
+                            tmp_lfn = f"{file.scope}:{file.lfn}"
+                        if tmp_lfn not in file_list[job.dispatchDBlock]["lfns"]:
+                            file_list[job.dispatchDBlock]["lfns"].append(tmp_lfn)
+                            file_list[job.dispatchDBlock]["guids"].append(file.GUID)
                             if file.fsize in ["NULL", 0]:
-                                fileList[job.dispatchDBlock]["fsizes"].append(None)
+                                file_list[job.dispatchDBlock]["fsizes"].append(None)
                             else:
-                                fileList[job.dispatchDBlock]["fsizes"].append(int(file.fsize))
+                                file_list[job.dispatchDBlock]["fsizes"].append(int(file.fsize))
                             if file.md5sum in ["NULL", ""]:
-                                fileList[job.dispatchDBlock]["md5sums"].append(None)
+                                file_list[job.dispatchDBlock]["md5sums"].append(None)
                             elif file.md5sum.startswith("md5:"):
-                                fileList[job.dispatchDBlock]["md5sums"].append(file.md5sum)
+                                file_list[job.dispatchDBlock]["md5sums"].append(file.md5sum)
                             else:
-                                fileList[job.dispatchDBlock]["md5sums"].append(f"md5:{file.md5sum}")
+                                file_list[job.dispatchDBlock]["md5sums"].append(f"md5:{file.md5sum}")
                             if file.checksum in ["NULL", ""]:
-                                fileList[job.dispatchDBlock]["chksums"].append(None)
+                                file_list[job.dispatchDBlock]["chksums"].append(None)
                             else:
-                                fileList[job.dispatchDBlock]["chksums"].append(file.checksum)
+                                file_list[job.dispatchDBlock]["chksums"].append(file.checksum)
                         # get replica locations
-                        self.replicaMap.setdefault(job.dispatchDBlock, {})
-                        if file.dataset not in self.allReplicaMap:
+                        self.replica_map.setdefault(job.dispatchDBlock, {})
+                        if file.dataset not in self.all_replica_map:
                             if file.dataset.endswith("/"):
-                                status, out = self.getListDatasetReplicasInContainer(file.dataset, True)
+                                status, out = self.get_list_dataset_replicas_in_container(file.dataset, True)
                             else:
-                                status, out = self.getListDatasetReplicas(file.dataset)
+                                status, out = self.get_list_dataset_replicas(file.dataset)
                             if not status:
                                 self.logger.error(out)
-                                dispError[job.dispatchDBlock] = f"could not get locations for {file.dataset}"
-                                self.logger.error(dispError[job.dispatchDBlock])
+                                disp_error[job.dispatchDBlock] = f"could not get locations for {file.dataset}"
+                                self.logger.error(disp_error[job.dispatchDBlock])
                             else:
                                 self.logger.debug(out)
-                                self.allReplicaMap[file.dataset] = out
-                        if file.dataset in self.allReplicaMap:
-                            self.replicaMap[job.dispatchDBlock][file.dataset] = self.allReplicaMap[file.dataset]
+                                self.all_replica_map[file.dataset] = out
+                        if file.dataset in self.all_replica_map:
+                            self.replica_map[job.dispatchDBlock][file.dataset] = self.all_replica_map[file.dataset]
         # register dispatch dataset
-        dispList = []
-        for dispatchDBlock in fileList:
+        disp_list = []
+        for dispatch_data_block, block_data in file_list.items():
             # ignore empty dataset
-            if len(fileList[dispatchDBlock]["lfns"]) == 0:
+            if len(block_data["lfns"]) == 0:
                 continue
-            # use DQ2
-            if (not self.pandaDDM) and job.prodSourceLabel != "ddm":
+            # use Rucio
+            if (not self.panda_ddm) and job.prodSourceLabel != "ddm":
                 # register dispatch dataset
-                self.dispFileList[dispatchDBlock] = fileList[dispatchDBlock]
-                if not useZipToPinMap[dispatchDBlock]:
-                    disFiles = fileList[dispatchDBlock]
+                self.disp_file_list[dispatch_data_block] = file_list[dispatch_data_block]
+                if not use_zip_to_pin_map[dispatch_data_block]:
+                    dis_files = file_list[dispatch_data_block]
                 else:
-                    dids = fileList[dispatchDBlock]["lfns"]
-                    tmpZipStat, tmpZipOut = rucioAPI.get_zip_files(dids, None)
-                    if not tmpZipStat:
-                        self.logger.debug(f"failed to get zip files : {tmpZipOut}")
-                        tmpZipOut = {}
-                    disFiles = {"lfns": [], "guids": [], "fsizes": [], "chksums": []}
-                    for tmpLFN, tmpGUID, tmpFSize, tmpChksum in zip(
-                        fileList[dispatchDBlock]["lfns"],
-                        fileList[dispatchDBlock]["guids"],
-                        fileList[dispatchDBlock]["fsizes"],
-                        fileList[dispatchDBlock]["chksums"],
+                    dids = file_list[dispatch_data_block]["lfns"]
+                    tmp_zip_stat, tmp_zip_out = rucioAPI.get_zip_files(dids, None)
+                    if not tmp_zip_stat:
+                        self.logger.debug(f"failed to get zip files : {tmp_zip_out}")
+                        tmp_zip_out = {}
+                    dis_files = {"lfns": [], "guids": [], "fsizes": [], "chksums": []}
+                    for tmp_lfn, tmp_guid, tmp_file_size, tmp_checksum in zip(
+                        file_list[dispatch_data_block]["lfns"],
+                        file_list[dispatch_data_block]["guids"],
+                        file_list[dispatch_data_block]["fsizes"],
+                        file_list[dispatch_data_block]["chksums"],
                     ):
-                        if tmpLFN in tmpZipOut:
-                            tmpZipFileName = f"{tmpZipOut[tmpLFN]['scope']}:{tmpZipOut[tmpLFN]['name']}"
-                            if tmpZipFileName not in disFiles["lfns"]:
-                                disFiles["lfns"].append(tmpZipFileName)
-                                disFiles["guids"].append(tmpZipOut[tmpLFN]["guid"])
-                                disFiles["fsizes"].append(tmpZipOut[tmpLFN]["bytes"])
-                                disFiles["chksums"].append(tmpZipOut[tmpLFN]["adler32"])
+                        if tmp_lfn in tmp_zip_out:
+                            tmp_zip_file_name = f"{tmp_zip_out[tmp_lfn]['scope']}:{tmp_zip_out[tmp_lfn]['name']}"
+                            if tmp_zip_file_name not in dis_files["lfns"]:
+                                dis_files["lfns"].append(tmp_zip_file_name)
+                                dis_files["guids"].append(tmp_zip_out[tmp_lfn]["guid"])
+                                dis_files["fsizes"].append(tmp_zip_out[tmp_lfn]["bytes"])
+                                dis_files["chksums"].append(tmp_zip_out[tmp_lfn]["adler32"])
                         else:
-                            disFiles["lfns"].append(tmpLFN)
-                            disFiles["guids"].append(tmpGUID)
-                            disFiles["fsizes"].append(tmpFSize)
-                            disFiles["chksums"].append(tmpChksum)
-                ddmBackEnd = backEndMap[dispatchDBlock]
-                if ddmBackEnd is None:
-                    ddmBackEnd = "rucio"
+                            dis_files["lfns"].append(tmp_lfn)
+                            dis_files["guids"].append(tmp_guid)
+                            dis_files["fsizes"].append(tmp_file_size)
+                            dis_files["chksums"].append(tmp_checksum)
+                ddm_back_end = back_end_map[dispatch_data_block]
+                if ddm_back_end is None:
+                    ddm_back_end = "rucio"
                 metadata = {"hidden": True, "purge_replicas": 0}
-                if dispatchDBlock in dsTaskMap and dsTaskMap[dispatchDBlock] not in [
+                if dispatch_data_block in ds_task_map and ds_task_map[dispatch_data_block] not in [
                     "NULL",
                     0,
                 ]:
-                    metadata["task_id"] = str(dsTaskMap[dispatchDBlock])
-                tmpMsg = "registerDataset {ds} {meta}"
-                self.logger.debug(tmpMsg.format(ds=dispatchDBlock, meta=str(metadata)))
-                nDDMTry = 3
-                isOK = False
-                errStr = ""
-                for iDDMTry in range(nDDMTry):
+                    metadata["task_id"] = str(ds_task_map[dispatch_data_block])
+                tmp_msg = "registerDataset {ds} {meta}"
+                self.logger.debug(tmp_msg.format(ds=dispatch_data_block, meta=str(metadata)))
+                max_attempt = 3
+                is_ok = False
+                err_str = ""
+                for attempt in range(max_attempt):
                     try:
                         out = rucioAPI.register_dataset(
-                            dispatchDBlock,
-                            disFiles["lfns"],
-                            disFiles["guids"],
-                            disFiles["fsizes"],
-                            disFiles["chksums"],
+                            dispatch_data_block,
+                            dis_files["lfns"],
+                            dis_files["guids"],
+                            dis_files["fsizes"],
+                            dis_files["chksums"],
                             lifetime=7,
                             scope="panda",
                             metadata=metadata,
                         )
-                        isOK = True
+                        is_ok = True
                         break
                     except Exception:
-                        errType, errValue = sys.exc_info()[:2]
-                        errStr = f"{errType}:{errValue}"
-                        self.logger.error(f"registerDataset : failed with {errStr}")
-                        if iDDMTry + 1 == nDDMTry:
+                        error_type, error_value = sys.exc_info()[:2]
+                        err_str = f"{error_type}:{error_value}"
+                        self.logger.error(f"registerDataset : failed with {err_str}")
+                        if attempt + 1 == max_attempt:
                             break
-                        self.logger.debug(f"sleep {iDDMTry}/{nDDMTry}")
+                        self.logger.debug(f"sleep {attempt}/{max_attempt}")
                         time.sleep(10)
-                if not isOK:
-                    dispError[dispatchDBlock] = "Setupper._setupSource() could not register dispatchDBlock with {0}".format(errStr.split("\n")[-1])
+                if not is_ok:
+                    disp_error[dispatch_data_block] = "Setupper._setupSource() could not register dispatch_data_block with {0}".format(err_str.split("\n")[-1])
                     continue
                 self.logger.debug(out)
-                newOut = out
+                new_out = out
                 # freezeDataset dispatch dataset
-                self.logger.debug("closeDataset " + dispatchDBlock)
-                for iDDMTry in range(3):
+                self.logger.debug("closeDataset " + dispatch_data_block)
+                for attempt in range(max_attempt):
                     status = False
                     try:
-                        rucioAPI.close_dataset(dispatchDBlock)
+                        rucioAPI.close_dataset(dispatch_data_block)
                         status = True
                         break
                     except Exception:
-                        errtype, errvalue = sys.exc_info()[:2]
-                        out = f"failed to close : {errtype} {errvalue}"
+                        error_type, error_value = sys.exc_info()[:2]
+                        out = f"failed to close : {error_type} {error_value}"
                         time.sleep(10)
                 if not status:
                     self.logger.error(out)
-                    dispError[dispatchDBlock] = f"Setupper._setupSource() could not freeze dispatchDBlock with {out}"
+                    disp_error[dispatch_data_block] = f"Setupper._setupSource() could not freeze dispatch_data_block with {out}"
                     continue
             else:
                 # use PandaDDM
-                self.dispFileList[dispatchDBlock] = fileList[dispatchDBlock]
+                self.disp_file_list[dispatch_data_block] = file_list[dispatch_data_block]
                 # create a fake vuid
-                newOut = {"vuid": str(uuid.uuid4())}
+                new_out = {"vuid": str(uuid.uuid4())}
             # get VUID
             try:
-                vuid = newOut["vuid"]
+                vuid = new_out["vuid"]
                 # dataset spec. currentfiles is used to count the number of failed jobs
-                ds = DatasetSpec()
-                ds.vuid = vuid
-                ds.name = dispatchDBlock
-                ds.type = "dispatch"
-                ds.status = "defined"
-                ds.numberfiles = len(fileList[dispatchDBlock]["lfns"])
+                dataset = DatasetSpec()
+                dataset.vuid = vuid
+                dataset.name = dispatch_data_block
+                dataset.type = "dispatch"
+                dataset.status = "defined"
+                dataset.numberfiles = len(file_list[dispatch_data_block]["lfns"])
                 try:
-                    ds.currentfiles = int(sum(filter(None, fileList[dispatchDBlock]["fsizes"])) / 1024 / 1024)
+                    dataset.currentfiles = int(sum(filter(None, file_list[dispatch_data_block]["fsizes"])) / 1024 / 1024)
                 except Exception:
-                    ds.currentfiles = 0
-                dispList.append(ds)
-                self.vuidMap[ds.name] = ds.vuid
+                    dataset.currentfiles = 0
+                disp_list.append(dataset)
+                self.vuid_map[dataset.name] = dataset.vuid
             except Exception:
-                errtype, errvalue = sys.exc_info()[:2]
-                self.logger.error(f"_setupSource() : {errtype} {errvalue}")
-                dispError[dispatchDBlock] = "Setupper._setupSource() could not decode VUID dispatchDBlock"
+                error_type, error_value = sys.exc_info()[:2]
+                self.logger.error(f"_setupSource() : {error_type} {error_value}")
+                disp_error[dispatch_data_block] = "Setupper._setupSource() could not decode VUID dispatch_data_block"
         # insert datasets to DB
-        self.taskBuffer.insertDatasets(prodList + dispList)
+        self.task_buffer.insertDatasets(prod_list + disp_list)
         # job status
         for job in self.jobs:
-            if job.dispatchDBlock in dispError and dispError[job.dispatchDBlock] != "":
+            if job.dispatchDBlock in disp_error and disp_error[job.dispatchDBlock] != "":
                 if job.jobStatus != "failed":
                     job.jobStatus = "failed"
                     job.ddmErrorCode = ErrorCode.EC_Setupper
-                    job.ddmErrorDiag = dispError[job.dispatchDBlock]
+                    job.ddmErrorDiag = disp_error[job.dispatchDBlock]
                     self.logger.debug(f"failed PandaID={job.PandaID} with {job.ddmErrorDiag}")
         # delete explicitly some huge variables
-        del fileList
-        del prodList
-        del prodError
-        del dispSiteMap
+        del file_list
+        del prod_list
+        del prod_error
+        del disp_site_map
 
     # create dataset for outputs in the repository and assign destination
-    def _setupDestination(self, startIdx=-1, nJobsInLoop=50):
-        self.logger.debug(f"setupDestination idx:{startIdx} n:{nJobsInLoop}")
-        destError = {}
-        datasetList = {}
-        newnameList = {}
-        snGottenDS = []
-        if startIdx == -1:
-            jobsList = self.jobs
+    def setup_destination(self, start_idx: int = -1, n_jobs_in_loop: int = 50) -> None:
+        """
+        Setup destination method for running the setup process.
+
+        :param start_idx: The starting index for the jobs to be processed. Defaults to -1.
+        :param n_jobs_in_loop: The number of jobs to be processed in a loop. Defaults to 50.
+        """
+        self.logger.debug(f"setupDestination idx:{start_idx} n:{n_jobs_in_loop}")
+        dest_error = {}
+        dataset_list = {}
+        newname_list = {}
+        sn_gotten_ds = []
+        if start_idx == -1:
+            jobs_list = self.jobs
         else:
-            jobsList = self.jobs[startIdx : startIdx + nJobsInLoop]
-        for job in jobsList:
+            jobs_list = self.jobs[start_idx: start_idx + n_jobs_in_loop]
+        for job in jobs_list:
             # ignore failed jobs
             if job.jobStatus in ["failed", "cancelled"] or job.isCancelled():
                 continue
             for file in job.Files:
                 # ignore input files
                 if file.type in ["input", "pseudo_input"]:
                     continue
                 # don't touch with outDS for unmerge jobs
                 if job.prodSourceLabel == "panda" and job.processingType == "unmerge" and file.type != "log":
                     continue
-                # extract destinationDBlock, destinationSE and computingSite
+                # extract destinationDBlock, destinationSE and computing_site
                 dest = (
                     file.destinationDBlock,
                     file.destinationSE,
                     job.computingSite,
                     file.destinationDBlockToken,
                 )
-                if dest not in destError:
-                    destError[dest] = ""
-                    originalName = ""
+                if dest not in dest_error:
+                    dest_error[dest] = ""
+                    original_name = ""
                     if (job.prodSourceLabel == "panda") or (
                         job.prodSourceLabel in JobUtils.list_ptest_prod_sources and job.processingType in ["pathena", "prun", "gangarobot-rctest"]
                     ):
                         # keep original name
-                        nameList = [file.destinationDBlock]
+                        name_list = [file.destinationDBlock]
                     else:
                         # set freshness to avoid redundant DB lookup
-                        definedFreshFlag = None
-                        if file.destinationDBlock in snGottenDS:
+                        defined_fresh_flag = None
+                        if file.destinationDBlock in sn_gotten_ds:
                             # already checked
-                            definedFreshFlag = False
+                            defined_fresh_flag = False
                         elif job.prodSourceLabel in ["user", "test", "prod_test"]:
                             # user or test datasets are always fresh in DB
-                            definedFreshFlag = True
+                            defined_fresh_flag = True
                         # get serial number
-                        sn, freshFlag = self.taskBuffer.getSerialNumber(file.destinationDBlock, definedFreshFlag)
-                        if sn == -1:
-                            destError[dest] = f"Setupper._setupDestination() could not get serial num for {file.destinationDBlock}"
+                        serial_number, fresh_flag = self.task_buffer.getSerialNumber(file.destinationDBlock, defined_fresh_flag)
+                        if serial_number == -1:
+                            dest_error[dest] = f"Setupper._setupDestination() could not get serial num for {file.destinationDBlock}"
                             continue
-                        if file.destinationDBlock not in snGottenDS:
-                            snGottenDS.append(file.destinationDBlock)
+                        if file.destinationDBlock not in sn_gotten_ds:
+                            sn_gotten_ds.append(file.destinationDBlock)
                         # new dataset name
-                        newnameList[dest] = self.makeSubDatasetName(file.destinationDBlock, sn, job.jediTaskID)
-                        if freshFlag or self.resetLocation:
+                        newname_list[dest] = self.make_sub_dataset_name(file.destinationDBlock, serial_number, job.jediTaskID)
+                        if fresh_flag:
                             # register original dataset and new dataset
-                            nameList = [file.destinationDBlock, newnameList[dest]]
-                            originalName = file.destinationDBlock
+                            name_list = [file.destinationDBlock, newname_list[dest]]
+                            original_name = file.destinationDBlock
                         else:
                             # register new dataset only
-                            nameList = [newnameList[dest]]
+                            name_list = [newname_list[dest]]
                     # create dataset
-                    for name in nameList:
-                        computingSite = job.computingSite
-                        tmpSite = self.siteMapper.getSite(computingSite)
-                        scope_input, scope_output = select_scope(tmpSite, job.prodSourceLabel, job.job_label)
-                        if name == originalName and not name.startswith("panda.um."):
+                    for name in name_list:
+                        computing_site = job.computingSite
+                        tmp_site = self.site_mapper.getSite(computing_site)
+                        _, scope_output = select_scope(tmp_site, job.prodSourceLabel, job.job_label)
+                        if name == original_name and not name.startswith("panda.um."):
                             # for original dataset
-                            computingSite = file.destinationSE
-                        newVUID = None
-                        if (not self.pandaDDM) and (job.prodSourceLabel != "ddm") and (job.destinationSE != "local"):
+                            computing_site = file.destinationSE
+                        new_vuid = None
+                        if (not self.panda_ddm) and (job.prodSourceLabel != "ddm") and (job.destinationSE != "local"):
                             # get src and dest DDM conversion is needed for unknown sites
-                            if job.prodSourceLabel == "user" and computingSite not in self.siteMapper.siteSpecList:
-                                # DQ2 ID was set by using --destSE for analysis job to transfer output
-                                tmpSrcDDM = tmpSite.ddm_output[scope_output]
+                            if job.prodSourceLabel == "user" and computing_site not in self.site_mapper.siteSpecList:
+                                # DDM ID was set by using --destSE for analysis job to transfer output
+                                tmp_src_ddm = tmp_site.ddm_output[scope_output]
                             else:
-                                tmpSrcDDM = tmpSite.ddm_output[scope_output]
-                            if job.prodSourceLabel == "user" and file.destinationSE not in self.siteMapper.siteSpecList:
-                                # DQ2 ID was set by using --destSE for analysis job to transfer output
-                                tmpDstDDM = tmpSrcDDM
+                                tmp_src_ddm = tmp_site.ddm_output[scope_output]
+                            if job.prodSourceLabel == "user" and file.destinationSE not in self.site_mapper.siteSpecList:
+                                # DDM ID was set by using --destSE for analysis job to transfer output
+                                tmp_dst_ddm = tmp_src_ddm
                             elif DataServiceUtils.getDestinationSE(file.destinationDBlockToken) is not None:
                                 # destination is specified
-                                tmpDstDDM = DataServiceUtils.getDestinationSE(file.destinationDBlockToken)
+                                tmp_dst_ddm = DataServiceUtils.getDestinationSE(file.destinationDBlockToken)
                             else:
-                                tmpDstSite = self.siteMapper.getSite(file.destinationSE)
-                                scopeDstSite_input, scopeDstSite_output = select_scope(tmpDstSite, job.prodSourceLabel, job.job_label)
-                                tmpDstDDM = tmpDstSite.ddm_output[scopeDstSite_output]
+                                tmp_dst_site = self.site_mapper.getSite(file.destinationSE)
+                                _, scope_dst_site_output = select_scope(tmp_dst_site, job.prodSourceLabel, job.job_label)
+                                tmp_dst_ddm = tmp_dst_site.ddm_output[scope_dst_site_output]
                             # skip registration for _sub when src=dest
                             if (
                                 (
-                                    (tmpSrcDDM == tmpDstDDM and not EventServiceUtils.isMergeAtOS(job.specialHandling))
+                                    (tmp_src_ddm == tmp_dst_ddm and not EventServiceUtils.isMergeAtOS(job.specialHandling))
                                     or DataServiceUtils.getDistributedDestination(file.destinationDBlockToken) is not None
                                 )
-                                and name != originalName
+                                and name != original_name
                                 and DataServiceUtils.is_sub_dataset(name)
                             ):
                                 # create a fake vuid
-                                newVUID = str(uuid.uuid4())
+                                new_vuid = str(uuid.uuid4())
                             else:
                                 # get list of tokens
-                                tmpTokenList = file.destinationDBlockToken.split(",")
+                                tmp_token_list = file.destinationDBlockToken.split(",")
 
                                 # get locations
-                                usingT1asT2 = False
-                                if job.prodSourceLabel == "user" and computingSite not in self.siteMapper.siteSpecList:
-                                    dq2IDList = [tmpSite.ddm_output[scope_output]]
+                                using_t1_as_t2 = False
+                                if job.prodSourceLabel == "user" and computing_site not in self.site_mapper.siteSpecList:
+                                    ddm_id_list = [tmp_site.ddm_output[scope_output]]
                                 else:
                                     if (
-                                        tmpSite.cloud != job.getCloud()
+                                        tmp_site.cloud != job.getCloud()
                                         and DataServiceUtils.is_sub_dataset(name)
                                         and (job.prodSourceLabel not in ["user", "panda"])
-                                        and (not tmpSite.ddm_output[scope_output].endswith("PRODDISK"))
+                                        and (not tmp_site.ddm_output[scope_output].endswith("PRODDISK"))
                                     ):
                                         # T1 used as T2. Use both DATADISK and PRODDISK as locations while T1 PRODDISK is phasing out
-                                        dq2IDList = [tmpSite.ddm_output[scope_output]]
-                                        if scope_output in tmpSite.setokens_output and "ATLASPRODDISK" in tmpSite.setokens_output[scope_output]:
-                                            dq2IDList += [tmpSite.setokens_output[scope_output]["ATLASPRODDISK"]]
-                                        usingT1asT2 = True
+                                        ddm_id_list = [tmp_site.ddm_output[scope_output]]
+                                        if scope_output in tmp_site.setokens_output and "ATLASPRODDISK" in tmp_site.setokens_output[scope_output]:
+                                            ddm_id_list += [tmp_site.setokens_output[scope_output]["ATLASPRODDISK"]]
+                                        using_t1_as_t2 = True
                                     else:
-                                        dq2IDList = [tmpSite.ddm_output[scope_output]]
+                                        ddm_id_list = [tmp_site.ddm_output[scope_output]]
                                 # use another location when token is set
                                 if not DataServiceUtils.is_sub_dataset(name) and DataServiceUtils.getDestinationSE(file.destinationDBlockToken) is not None:
                                     # destination is specified
-                                    dq2IDList = [DataServiceUtils.getDestinationSE(file.destinationDBlockToken)]
-                                elif (not usingT1asT2) and (file.destinationDBlockToken not in ["NULL", ""]):
-                                    dq2IDList = []
-                                    for tmpToken in tmpTokenList:
+                                    ddm_id_list = [DataServiceUtils.getDestinationSE(file.destinationDBlockToken)]
+                                elif (not using_t1_as_t2) and (file.destinationDBlockToken not in ["NULL", ""]):
+                                    ddm_id_list = []
+                                    for tmp_token in tmp_token_list:
                                         # set default
-                                        dq2ID = tmpSite.ddm_output[scope_output]
-                                        # convert token to DQ2ID
-                                        if tmpToken in tmpSite.setokens_output[scope_output]:
-                                            dq2ID = tmpSite.setokens_output[scope_output][tmpToken]
+                                        ddm_id = tmp_site.ddm_output[scope_output]
+                                        # convert token to DDM ID
+                                        if tmp_token in tmp_site.setokens_output[scope_output]:
+                                            ddm_id = tmp_site.setokens_output[scope_output][tmp_token]
                                         # replace or append
-                                        if len(tmpTokenList) <= 1 or name != originalName:
+                                        if len(tmp_token_list) <= 1 or name != original_name:
                                             # use location consistent with token
-                                            dq2IDList = [dq2ID]
+                                            ddm_id_list = [ddm_id]
                                             break
                                         else:
                                             # use multiple locations for _tid
-                                            if dq2ID not in dq2IDList:
-                                                dq2IDList.append(dq2ID)
+                                            if ddm_id not in ddm_id_list:
+                                                ddm_id_list.append(ddm_id)
                                 # set hidden flag for _sub
-                                tmpActivity = None
-                                tmpLifeTime = None
-                                tmpMetadata = None
-                                if name != originalName and DataServiceUtils.is_sub_dataset(name):
-                                    tmpActivity = "Production Output"
-                                    tmpLifeTime = 14
-                                    tmpMetadata = {"hidden": True, "purge_replicas": 0}
+                                tmp_life_time = None
+                                tmp_metadata = None
+                                if name != original_name and DataServiceUtils.is_sub_dataset(name):
+                                    tmp_life_time = 14
+                                    tmp_metadata = {"hidden": True, "purge_replicas": 0}
                                 # backend
-                                ddmBackEnd = job.getDdmBackEnd()
-                                if ddmBackEnd is None:
-                                    ddmBackEnd = "rucio"
+                                ddm_back_end = job.getDdmBackEnd()
+                                if ddm_back_end is None:
+                                    ddm_back_end = "rucio"
                                 # register dataset
-                                self.logger.debug(f"registerNewDataset {name} metadata={tmpMetadata}")
-                                isOK = False
-                                for iDDMTry in range(3):
+                                self.logger.debug(f"registerNewDataset {name} metadata={tmp_metadata}")
+                                is_ok = False
+                                for _ in range(3):
                                     try:
                                         out = rucioAPI.register_dataset(
                                             name,
-                                            metadata=tmpMetadata,
-                                            lifetime=tmpLifeTime,
+                                            metadata=tmp_metadata,
+                                            lifetime=tmp_life_time,
                                         )
                                         self.logger.debug(out)
-                                        newVUID = out["vuid"]
-                                        isOK = True
+                                        new_vuid = out["vuid"]
+                                        is_ok = True
                                         break
                                     except Exception:
-                                        errType, errValue = sys.exc_info()[:2]
-                                        self.logger.error(f"registerDataset : failed with {errType}:{errValue}")
+                                        error_type, error_value = sys.exc_info()[:2]
+                                        self.logger.error(f"registerDataset : failed with {error_type}:{error_value}")
                                         time.sleep(10)
-                                if not isOK:
-                                    tmpMsg = f"Setupper._setupDestination() could not register : {name}"
-                                    destError[dest] = tmpMsg
-                                    self.logger.error(tmpMsg)
+                                if not is_ok:
+                                    tmp_msg = f"Setupper._setupDestination() could not register : {name}"
+                                    dest_error[dest] = tmp_msg
+                                    self.logger.error(tmp_msg)
                                     continue
                                 # register dataset locations
                                 if (
                                     job.lockedby == "jedi" and job.getDdmBackEnd() == "rucio" and job.prodSourceLabel in ["panda", "user"]
                                 ) or DataServiceUtils.getDistributedDestination(file.destinationDBlockToken, ignore_empty=False) is not None:
                                     # skip registerDatasetLocations
                                     status, out = True, ""
                                 elif (
-                                    name == originalName
-                                    or tmpSrcDDM != tmpDstDDM
+                                    name == original_name
+                                    or tmp_src_ddm != tmp_dst_ddm
                                     or job.prodSourceLabel == "panda"
                                     or (
                                         job.prodSourceLabel in JobUtils.list_ptest_prod_sources
                                         and job.processingType in ["pathena", "prun", "gangarobot-rctest"]
                                     )
-                                    or len(tmpTokenList) > 1
+                                    or len(tmp_token_list) > 1
                                     or EventServiceUtils.isMergeAtOS(job.specialHandling)
                                 ):
                                     # set replica lifetime to _sub
-                                    repLifeTime = None
-                                    if (name != originalName and DataServiceUtils.is_sub_dataset(name)) or (
-                                        name == originalName and name.startswith("panda.")
+                                    rep_life_time = None
+                                    if (name != original_name and DataServiceUtils.is_sub_dataset(name)) or (
+                                        name == original_name and name.startswith("panda.")
                                     ):
-                                        repLifeTime = 14
+                                        rep_life_time = 14
                                     elif name.startswith("hc_test") or name.startswith("panda.install.") or name.startswith("user.gangarbt."):
-                                        repLifeTime = 7
+                                        rep_life_time = 7
                                     # distributed datasets for es outputs
                                     grouping = None
-                                    if name != originalName and DataServiceUtils.is_sub_dataset(name) and EventServiceUtils.isEventServiceJob(job):
-                                        dq2IDList = ["type=DATADISK"]
+                                    if name != original_name and DataServiceUtils.is_sub_dataset(name) and EventServiceUtils.isEventServiceJob(job):
+                                        ddm_id_list = ["type=DATADISK"]
                                         grouping = "NONE"
                                     # register location
-                                    isOK = True
-                                    for dq2ID in dq2IDList:
+                                    is_ok = True
+                                    for ddm_id in ddm_id_list:
                                         activity = DataServiceUtils.getActivityForOut(job.prodSourceLabel)
-                                        tmpStr = "registerDatasetLocation {name} {dq2ID} lifetime={repLifeTime} activity={activity} grouping={grouping}"
+                                        new_out = "registerDatasetLocation {name} {ddm_id} lifetime={rep_life_time} activity={activity} grouping={grouping}"
                                         self.logger.debug(
-                                            tmpStr.format(
+                                            new_out.format(
                                                 name=name,
-                                                dq2ID=dq2ID,
-                                                repLifeTime=repLifeTime,
+                                                ddm_id=ddm_id,
+                                                rep_life_time=rep_life_time,
                                                 activity=activity,
                                                 grouping=grouping,
                                             )
                                         )
                                         status = False
                                         # invalid location
-                                        if dq2ID is None:
-                                            out = f"wrong location : {dq2ID}"
+                                        if ddm_id is None:
+                                            out = f"wrong location : {ddm_id}"
                                             self.logger.error(out)
                                             break
-                                        for iDDMTry in range(3):
+                                        for _ in range(3):
                                             try:
                                                 out = rucioAPI.register_dataset_location(
                                                     name,
-                                                    [dq2ID],
-                                                    lifetime=repLifeTime,
+                                                    [ddm_id],
+                                                    lifetime=rep_life_time,
                                                     activity=activity,
                                                     grouping=grouping,
                                                 )
                                                 self.logger.debug(out)
                                                 status = True
                                                 break
                                             except Exception:
-                                                errType, errValue = sys.exc_info()[:2]
-                                                out = f"{errType}:{errValue}"
+                                                error_type, error_value = sys.exc_info()[:2]
+                                                out = f"{error_type}:{error_value}"
                                                 self.logger.error(f"registerDatasetLocation : failed with {out}")
                                                 time.sleep(10)
                                         # failed
                                         if not status:
                                             break
                                 else:
                                     # skip registerDatasetLocations
                                     status, out = True, ""
                                 if not status:
-                                    destError[dest] = "Could not register location : %s %s" % (
+                                    dest_error[dest] = "Could not register location : %s %s" % (
                                         name,
                                         out.split("\n")[-1],
                                     )
                         # already failed
-                        if destError[dest] != "" and name == originalName:
+                        if dest_error[dest] != "" and name == original_name:
                             break
                         # get vuid
-                        if newVUID is None:
+                        if new_vuid is None:
                             self.logger.debug("listDatasets " + name)
-                            for iDDMTry in range(3):
-                                newOut, errMsg = rucioAPI.list_datasets(name)
-                                if newOut is None:
+                            for _ in range(3):
+                                new_out, err_msg = rucioAPI.list_datasets(name)
+                                if new_out is None:
                                     time.sleep(10)
                                 else:
                                     break
-                            if newOut is None:
-                                errMsg = f"failed to get VUID for {name} with {errMsg}"
-                                self.logger.error(errMsg)
+                            if new_out is None:
+                                err_msg = f"failed to get VUID for {name} with {err_msg}"
+                                self.logger.error(err_msg)
                             else:
-                                self.logger.debug(newOut)
-                                newVUID = newOut[name]["vuids"][0]
+                                self.logger.debug(new_out)
+                                new_vuid = new_out[name]["vuids"][0]
                         try:
                             # dataset spec
-                            ds = DatasetSpec()
-                            ds.vuid = newVUID
-                            ds.name = name
-                            ds.type = "output"
-                            ds.numberfiles = 0
-                            ds.currentfiles = 0
-                            ds.status = "defined"
+                            dataset = DatasetSpec()
+                            dataset.vuid = new_vuid
+                            dataset.name = name
+                            dataset.type = "output"
+                            dataset.numberfiles = 0
+                            dataset.currentfiles = 0
+                            dataset.status = "defined"
                             # append
-                            datasetList[(name, file.destinationSE, computingSite)] = ds
+                            dataset_list[(name, file.destinationSE, computing_site)] = dataset
                         except Exception:
                             # set status
-                            errtype, errvalue = sys.exc_info()[:2]
-                            self.logger.error(f"_setupDestination() : {errtype} {errvalue}")
-                            destError[dest] = f"Setupper._setupDestination() could not get VUID : {name}"
+                            error_type, error_value = sys.exc_info()[:2]
+                            self.logger.error(f"_setupDestination() : {error_type} {error_value}")
+                            dest_error[dest] = f"Setupper._setupDestination() could not get VUID : {name}"
                 # set new destDBlock
-                if dest in newnameList:
-                    file.destinationDBlock = newnameList[dest]
+                if dest in newname_list:
+                    file.destinationDBlock = newname_list[dest]
                 # update job status if failed
-                if destError[dest] != "":
+                if dest_error[dest] != "":
                     if job.jobStatus != "failed":
                         job.jobStatus = "failed"
                         job.ddmErrorCode = ErrorCode.EC_Setupper
-                        job.ddmErrorDiag = destError[dest]
+                        job.ddmErrorDiag = dest_error[dest]
                         self.logger.debug(f"failed PandaID={job.PandaID} with {job.ddmErrorDiag}")
                 else:
-                    newdest = (
+                    new_dest = (
                         file.destinationDBlock,
                         file.destinationSE,
                         job.computingSite,
                     )
                     # increment number of files
-                    datasetList[newdest].numberfiles = datasetList[newdest].numberfiles + 1
+                    dataset_list[new_dest].numberfiles = dataset_list[new_dest].numberfiles + 1
         # dump
-        for tmpDsKey in datasetList:
-            if DataServiceUtils.is_sub_dataset(tmpDsKey[0]):
-                self.logger.debug(f"made sub:{tmpDsKey[0]} for nFiles={datasetList[tmpDsKey].numberfiles}")
+        for dataset_name, dataset in dataset_list.items():
+            # Ensure dataset_name is a string
+            if isinstance(dataset_name, tuple):
+                dataset_name = dataset_name[0]
+            if DataServiceUtils.is_sub_dataset(dataset_name):
+                self.logger.debug(f"made sub:{dataset_name} for nFiles={dataset.numberfiles}")
         # insert datasets to DB
-        return self.taskBuffer.insertDatasets(datasetList.values())
+        return self.task_buffer.insertDatasets(dataset_list.values())
 
-    #  subscribe sites to distpatchDBlocks
-    def _subscribeDistpatchDB(self):
-        dispError = {}
-        failedJobs = []
-        ddmJobs = []
-        ddmUser = "NULL"
+    #  subscribe sites to dispatchDBlocks
+    def subscribe_dispatch_data_block(self) -> None:
+        """
+        Subscribe dispatch db method for running the setup process.
+        """
+        disp_error = {}
+        failed_jobs = []
+        ddm_jobs = []
+        ddm_user = "NULL"
         for job in self.jobs:
             # ignore failed jobs
             if job.jobStatus in ["failed", "cancelled"] or job.isCancelled():
                 continue
             # ignore no dispatch jobs
             if job.dispatchDBlock == "NULL" or job.computingSite == "NULL":
                 continue
             # backend
-            ddmBackEnd = job.getDdmBackEnd()
-            if ddmBackEnd is None:
-                ddmBackEnd = "rucio"
+            ddm_back_end = job.getDdmBackEnd()
+            if ddm_back_end is None:
+                ddm_back_end = "rucio"
             # extract dispatchDBlock and computingSite
             disp = (job.dispatchDBlock, job.computingSite)
-            if disp not in dispError:
-                dispError[disp] = ""
-                # DQ2 IDs
-                tmpSrcID = "BNL_ATLAS_1"
+            if disp not in disp_error:
+                disp_error[disp] = ""
+                # DDM IDs
+                tmp_src_id = "BNL_ATLAS_1"
                 if job.prodSourceLabel in ["user", "panda"]:
-                    tmpSrcID = job.computingSite
-                elif self.siteMapper.checkCloud(job.getCloud()):
+                    tmp_src_id = job.computingSite
+                elif self.site_mapper.checkCloud(job.getCloud()):
                     # use cloud's source
-                    tmpSrcID = self.siteMapper.getCloud(job.getCloud())["source"]
-                srcSite = self.siteMapper.getSite(tmpSrcID)
-                scope_srcSite_input, scope_srcSite_output = select_scope(srcSite, job.prodSourceLabel, job.job_label)
-                srcDQ2ID = srcSite.ddm_output[scope_srcSite_output]
+                    tmp_src_id = self.site_mapper.getCloud(job.getCloud())["source"]
+                src_site = self.site_mapper.getSite(tmp_src_id)
+                _, scope_src_site_output = select_scope(src_site, job.prodSourceLabel, job.job_label)
+                src_ddm_id = src_site.ddm_output[scope_src_site_output]
                 # destination
-                tmpDstID = job.computingSite
-                tmpSiteSpec = self.siteMapper.getSite(job.computingSite)
-                scope_tmpSite_input, scope_tmpSite_output = select_scope(tmpSiteSpec, job.prodSourceLabel, job.job_label)
-                if srcDQ2ID != tmpSiteSpec.ddm_input[scope_tmpSite_input] and srcDQ2ID in tmpSiteSpec.setokens_input[scope_tmpSite_input].values():
+                tmp_dst_id = job.computingSite
+                tmp_site_spec = self.site_mapper.getSite(job.computingSite)
+                scope_tmp_site_input, _ = select_scope(tmp_site_spec, job.prodSourceLabel, job.job_label)
+                if src_ddm_id != tmp_site_spec.ddm_input[scope_tmp_site_input] and src_ddm_id in tmp_site_spec.setokens_input[scope_tmp_site_input].values():
                     # direct usage of remote SE. Mainly for prestaging
-                    tmpDstID = tmpSrcID
-                    self.logger.debug(f"use remote SiteSpec of {tmpDstID} for {job.computingSite}")
-                # use srcDQ2ID as dstDQ2ID when it is associated to dest
-                dstSiteSpec = self.siteMapper.getSite(tmpDstID)
-                scope_dst_input, scope_dst_output = select_scope(dstSiteSpec, job.prodSourceLabel, job.job_label)
-                if dstSiteSpec.ddm_endpoints_input[scope_dst_input].isAssociated(srcDQ2ID):
-                    dstDQ2ID = srcDQ2ID
+                    tmp_dst_id = tmp_src_id
+                    self.logger.debug(f"use remote SiteSpec of {tmp_dst_id} for {job.computingSite}")
+                # use src_ddm_id as dst_ddm_id when it is associated to dest
+                dst_site_spec = self.site_mapper.getSite(tmp_dst_id)
+                scope_dst_input, _ = select_scope(dst_site_spec, job.prodSourceLabel, job.job_label)
+                if dst_site_spec.ddm_endpoints_input[scope_dst_input].isAssociated(src_ddm_id):
+                    dst_ddm_id = src_ddm_id
                 else:
-                    dstDQ2ID = dstSiteSpec.ddm_input[scope_dst_input]
+                    dst_ddm_id = dst_site_spec.ddm_input[scope_dst_input]
                 # check if missing at T1
-                missingAtT1 = False
+                missing_at_t1 = False
                 if job.prodSourceLabel in ["managed", "test"]:
-                    for tmpLFN in self.dispFileList[job.dispatchDBlock]["lfns"]:
-                        if job.getCloud() not in self.missingFilesInT1:
+                    for tmp_lfn in self.disp_file_list[job.dispatchDBlock]["lfns"]:
+                        if job.getCloud() not in self.missing_files_in_t1:
                             break
-                        if tmpLFN in self.missingFilesInT1[job.getCloud()] or tmpLFN.split(":")[-1] in self.missingFilesInT1[job.getCloud()]:
-                            missingAtT1 = True
+                        if tmp_lfn in self.missing_files_in_t1[job.getCloud()] or tmp_lfn.split(":")[-1] in self.missing_files_in_t1[job.getCloud()]:
+                            missing_at_t1 = True
                             break
-                    self.logger.debug(f"{job.dispatchDBlock} missing at T1 : {missingAtT1}")
-                # use DQ2
-                if (not self.pandaDDM) and job.prodSourceLabel != "ddm":
+                    self.logger.debug(f"{job.dispatchDBlock} missing at T1 : {missing_at_t1}")
+                # use DDM
+                if (not self.panda_ddm) and job.prodSourceLabel != "ddm":
                     # look for replica
-                    dq2ID = srcDQ2ID
-                    dq2IDList = []
+                    ddm_id = src_ddm_id
+                    ddm_id_list = []
                     # register replica
-                    isOK = False
-                    if dq2ID != dstDQ2ID or missingAtT1:
+                    is_ok = False
+                    if ddm_id != dst_ddm_id or missing_at_t1:
                         # make list
-                        if job.dispatchDBlock in self.replicaMap:
-                            # set DQ2 ID for DISK
-                            if not srcDQ2ID.endswith("_DATADISK"):
-                                hotID = re.sub("_MCDISK", "_HOTDISK", srcDQ2ID)
-                                diskID = re.sub("_MCDISK", "_DATADISK", srcDQ2ID)
-                                tapeID = re.sub("_MCDISK", "_DATATAPE", srcDQ2ID)
-                                mctapeID = re.sub("_MCDISK", "_MCTAPE", srcDQ2ID)
+                        if job.dispatchDBlock in self.replica_map:
+                            # set DDM ID for DISK
+                            if not src_ddm_id.endswith("_DATADISK"):
+                                hot_id = re.sub("_MCDISK", "_HOTDISK", src_ddm_id)
+                                disk_id = re.sub("_MCDISK", "_DATADISK", src_ddm_id)
+                                tape_id = re.sub("_MCDISK", "_DATATAPE", src_ddm_id)
+                                mc_tape_id = re.sub("_MCDISK", "_MCTAPE", src_ddm_id)
                             else:
-                                hotID = re.sub("_DATADISK", "_HOTDISK", srcDQ2ID)
-                                diskID = re.sub("_DATADISK", "_DATADISK", srcDQ2ID)
-                                tapeID = re.sub("_DATADISK", "_DATATAPE", srcDQ2ID)
-                                mctapeID = re.sub("_DATADISK", "_MCTAPE", srcDQ2ID)
-                            # DQ2 ID is mixed with TAIWAN-LCG2 and TW-FTT
+                                hot_id = re.sub("_DATADISK", "_HOTDISK", src_ddm_id)
+                                disk_id = re.sub("_DATADISK", "_DATADISK", src_ddm_id)
+                                tape_id = re.sub("_DATADISK", "_DATATAPE", src_ddm_id)
+                                mc_tape_id = re.sub("_DATADISK", "_MCTAPE", src_ddm_id)
+                            # DDM ID is mixed with TAIWAN-LCG2 and TW-FTT
                             if job.getCloud() in [
                                 "TW",
                             ]:
-                                tmpSiteSpec = self.siteMapper.getSite(tmpSrcID)
-                                scope_input, scope_output = select_scope(tmpSiteSpec, job.prodSourceLabel, job.job_label)
-                                if "ATLASDATADISK" in tmpSiteSpec.setokens_input[scope_input]:
-                                    diskID = tmpSiteSpec.setokens_input[scope_input]["ATLASDATADISK"]
-                                if "ATLASDATATAPE" in tmpSiteSpec.setokens_input[scope_input]:
-                                    tapeID = tmpSiteSpec.setokens_input[scope_input]["ATLASDATATAPE"]
-                                if "ATLASMCTAPE" in tmpSiteSpec.setokens_input[scope_input]:
-                                    mctapeID = tmpSiteSpec.setokens_input[scope_input]["ATLASMCTAPE"]
-                                hotID = "TAIWAN-LCG2_HOTDISK"
-                            for tmpDataset in self.replicaMap[job.dispatchDBlock]:
-                                tmpRepMap = self.replicaMap[job.dispatchDBlock][tmpDataset]
-                                if hotID in tmpRepMap:
+                                tmp_site_spec = self.site_mapper.getSite(tmp_src_id)
+                                scope_input, _ = select_scope(tmp_site_spec, job.prodSourceLabel, job.job_label)
+                                if "ATLASDATADISK" in tmp_site_spec.setokens_input[scope_input]:
+                                    disk_id = tmp_site_spec.setokens_input[scope_input]["ATLASDATADISK"]
+                                if "ATLASDATATAPE" in tmp_site_spec.setokens_input[scope_input]:
+                                    tape_id = tmp_site_spec.setokens_input[scope_input]["ATLASDATATAPE"]
+                                if "ATLASMCTAPE" in tmp_site_spec.setokens_input[scope_input]:
+                                    mc_tape_id = tmp_site_spec.setokens_input[scope_input]["ATLASMCTAPE"]
+                                hot_id = "TAIWAN-LCG2_HOTDISK"
+                            for tmp_dataset in self.replica_map[job.dispatchDBlock]:
+                                tmp_rep_map = self.replica_map[job.dispatchDBlock][tmp_dataset]
+                                if hot_id in tmp_rep_map:
                                     # HOTDISK
-                                    if hotID not in dq2IDList:
-                                        dq2IDList.append(hotID)
-                                if srcDQ2ID in tmpRepMap:
+                                    if hot_id not in ddm_id_list:
+                                        ddm_id_list.append(hot_id)
+                                if src_ddm_id in tmp_rep_map:
                                     # MCDISK
-                                    if srcDQ2ID not in dq2IDList:
-                                        dq2IDList.append(srcDQ2ID)
-                                if diskID in tmpRepMap:
+                                    if src_ddm_id not in ddm_id_list:
+                                        ddm_id_list.append(src_ddm_id)
+                                if disk_id in tmp_rep_map:
                                     # DATADISK
-                                    if diskID not in dq2IDList:
-                                        dq2IDList.append(diskID)
-                                if tapeID in tmpRepMap:
+                                    if disk_id not in ddm_id_list:
+                                        ddm_id_list.append(disk_id)
+                                if tape_id in tmp_rep_map:
                                     # DATATAPE
-                                    if tapeID not in dq2IDList:
-                                        dq2IDList.append(tapeID)
-                                if mctapeID in tmpRepMap:
+                                    if tape_id not in ddm_id_list:
+                                        ddm_id_list.append(tape_id)
+                                if mc_tape_id in tmp_rep_map:
                                     # MCTAPE
-                                    if mctapeID not in dq2IDList:
-                                        dq2IDList.append(mctapeID)
+                                    if mc_tape_id not in ddm_id_list:
+                                        ddm_id_list.append(mc_tape_id)
                             # consider cloudconfig.tier1se
-                            tmpCloudSEs = DataServiceUtils.getEndpointsAtT1(tmpRepMap, self.siteMapper, job.getCloud())
-                            useCloudSEs = []
-                            for tmpCloudSE in tmpCloudSEs:
-                                if tmpCloudSE not in dq2IDList:
-                                    useCloudSEs.append(tmpCloudSE)
-                            if useCloudSEs != []:
-                                dq2IDList += useCloudSEs
-                                self.logger.debug(f"use additional endpoints {str(useCloudSEs)} from cloudconfig")
+                            tmp_cloud_ses = DataServiceUtils.getEndpointsAtT1(tmp_rep_map, self.site_mapper, job.getCloud())
+                            use_cloud_ses = []
+                            for tmp_cloud_se in tmp_cloud_ses:
+                                if tmp_cloud_se not in ddm_id_list:
+                                    use_cloud_ses.append(tmp_cloud_se)
+                            if use_cloud_ses:
+                                ddm_id_list += use_cloud_ses
+                                self.logger.debug(f"use additional endpoints {str(use_cloud_ses)} from cloudconfig")
                         # use default location if empty
-                        if dq2IDList == []:
-                            dq2IDList = [dq2ID]
+                        if not ddm_id_list:
+                            ddm_id_list = [ddm_id]
                         # register dataset locations
-                        if missingAtT1:
-                            # without locatios to let DDM find sources
-                            isOK = True
-                        else:
-                            isOK = True
+                        is_ok = True
                     else:
                         # register locations later for prestaging
-                        isOK = True
-                    if not isOK:
-                        dispError[disp] = "Setupper._subscribeDistpatchDB() could not register location"
+                        is_ok = True
+                    if not is_ok:
+                        disp_error[disp] = "Setupper._subscribeDispatchDB() could not register location"
                     else:
-                        isOK = False
-                        # assign destination
-                        optSub = {
-                            "DATASET_COMPLETE_EVENT": [f"http://{panda_config.pserverhosthttp}:{panda_config.pserverporthttp}/server/panda/datasetCompleted"]
-                        }
-                        optSource = {}
-                        dq2ID = dstDQ2ID
+                        is_ok = False
+                        opt_source = {}
+                        ddm_id = dst_ddm_id
                         # prestaging
-                        if srcDQ2ID == dstDQ2ID and not missingAtT1:
+                        if src_ddm_id == dst_ddm_id and not missing_at_t1:
                             # prestage to associated endpoints
                             if job.prodSourceLabel in ["user", "panda"]:
-                                tmpSiteSpec = self.siteMapper.getSite(job.computingSite)
+                                tmp_site_spec = self.site_mapper.getSite(job.computingSite)
                                 (
-                                    scope_tmpSite_input,
-                                    scope_tmpSite_output,
-                                ) = select_scope(tmpSiteSpec, job.prodSourceLabel, job.job_label)
+                                    scope_tmp_site_input,
+                                    scope_tmp_site_output,
+                                ) = select_scope(tmp_site_spec, job.prodSourceLabel, job.job_label)
                                 # use DATADISK if possible
                                 changed = False
-                                if "ATLASDATADISK" in tmpSiteSpec.setokens_input[scope_tmpSite_input]:
-                                    tmpDq2ID = tmpSiteSpec.setokens_input[scope_tmpSite_input]["ATLASDATADISK"]
-                                    if tmpDq2ID in tmpSiteSpec.ddm_endpoints_input[scope_tmpSite_input].getLocalEndPoints():
-                                        self.logger.debug(f"use {tmpDq2ID} instead of {dq2ID} for tape prestaging")
-                                        dq2ID = tmpDq2ID
+                                if "ATLASDATADISK" in tmp_site_spec.setokens_input[scope_tmp_site_input]:
+                                    tmp_ddm_id = tmp_site_spec.setokens_input[scope_tmp_site_input]["ATLASDATADISK"]
+                                    if tmp_ddm_id in tmp_site_spec.ddm_endpoints_input[scope_tmp_site_input].getLocalEndPoints():
+                                        self.logger.debug(f"use {tmp_ddm_id} instead of {ddm_id} for tape prestaging")
+                                        ddm_id = tmp_ddm_id
                                         changed = True
                                 # use default input endpoint
                                 if not changed:
-                                    dq2ID = tmpSiteSpec.ddm_endpoints_input[scope_tmpSite_input].getDefaultRead()
-                                    self.logger.debug(f"use default_read {dq2ID} for tape prestaging")
-                            self.logger.debug(f"use {dq2ID} for tape prestaging")
+                                    ddm_id = tmp_site_spec.ddm_endpoints_input[scope_tmp_site_input].getDefaultRead()
+                                    self.logger.debug(f"use default_read {ddm_id} for tape prestaging")
+                            self.logger.debug(f"use {ddm_id} for tape prestaging")
                             # register dataset locations
-                            isOK = True
+                            is_ok = True
                         else:
-                            isOK = True
+                            is_ok = True
                             # set sources to handle T2s in another cloud and to transfer dis datasets being split in multiple sites
-                            if not missingAtT1:
-                                for tmpDQ2ID in dq2IDList:
-                                    optSource[tmpDQ2ID] = {"policy": 0}
+                            if not missing_at_t1:
+                                for tmp_ddm_id in ddm_id_list:
+                                    opt_source[tmp_ddm_id] = {"policy": 0}
                             # T1 used as T2
                             if (
-                                job.getCloud() != self.siteMapper.getSite(tmpDstID).cloud
-                                and (not dstDQ2ID.endswith("PRODDISK"))
+                                job.getCloud() != self.site_mapper.getSite(tmp_dst_id).cloud
+                                and (not dst_ddm_id.endswith("PRODDISK"))
                                 and (job.prodSourceLabel not in ["user", "panda"])
-                                and self.siteMapper.getSite(tmpDstID).cloud in ["US"]
+                                and self.site_mapper.getSite(tmp_dst_id).cloud in ["US"]
                             ):
-                                tmpDstSiteSpec = self.siteMapper.getSite(tmpDstID)
-                                scope_input, scope_output = select_scope(tmpDstSiteSpec, job.prodSourceLabel, job.job_label)
-                                seTokens = tmpDstSiteSpec.setokens_input[scope_input]
+                                tmp_dst_site_spec = self.site_mapper.getSite(tmp_dst_id)
+                                scope_input, _ = select_scope(tmp_dst_site_spec, job.prodSourceLabel, job.job_label)
+                                se_tokens = tmp_dst_site_spec.setokens_input[scope_input]
                                 # use T1_PRODDISK
-                                if "ATLASPRODDISK" in seTokens:
-                                    dq2ID = seTokens["ATLASPRODDISK"]
+                                if "ATLASPRODDISK" in se_tokens:
+                                    ddm_id = se_tokens["ATLASPRODDISK"]
                             elif job.prodSourceLabel in ["user", "panda"]:
                                 # use DATADISK
-                                tmpSiteSpec = self.siteMapper.getSite(job.computingSite)
+                                tmp_site_spec = self.site_mapper.getSite(job.computingSite)
                                 (
-                                    scope_tmpSite_input,
-                                    scope_tmpSite_output,
-                                ) = select_scope(tmpSiteSpec, job.prodSourceLabel, job.job_label)
-                                if "ATLASDATADISK" in tmpSiteSpec.setokens_input[scope_tmpSite_input]:
-                                    tmpDq2ID = tmpSiteSpec.setokens_input[scope_tmpSite_input]["ATLASDATADISK"]
-                                    if tmpDq2ID in tmpSiteSpec.ddm_endpoints_input[scope_tmpSite_input].getLocalEndPoints():
-                                        self.logger.debug(f"use {tmpDq2ID} instead of {dq2ID} for analysis input staging")
-                                        dq2ID = tmpDq2ID
+                                    scope_tmp_site_input,
+                                    scope_tmp_site_output,
+                                ) = select_scope(tmp_site_spec, job.prodSourceLabel, job.job_label)
+                                if "ATLASDATADISK" in tmp_site_spec.setokens_input[scope_tmp_site_input]:
+                                    tmp_ddm_id = tmp_site_spec.setokens_input[scope_tmp_site_input]["ATLASDATADISK"]
+                                    if tmp_ddm_id in tmp_site_spec.ddm_endpoints_input[scope_tmp_site_input].getLocalEndPoints():
+                                        self.logger.debug(f"use {tmp_ddm_id} instead of {ddm_id} for analysis input staging")
+                                        ddm_id = tmp_ddm_id
                         # set share and activity
                         if job.prodSourceLabel in ["user", "panda"]:
-                            optShare = "production"
-                            optActivity = "Analysis Input"
-                            optOwner = None
+                            opt_activity = "Analysis Input"
+                            opt_owner = None
                         else:
-                            optShare = "production"
-                            optOwner = None
+                            opt_owner = None
                             if job.processingType == "urgent" or job.currentPriority > 1000:
-                                optActivity = "Express"
+                                opt_activity = "Express"
                             else:
-                                optActivity = "Production Input"
+                                opt_activity = "Production Input"
                         # taskID
                         if job.jediTaskID not in ["NULL", 0]:
-                            optComment = f"task_id:{job.jediTaskID}"
+                            opt_comment = f"task_id:{job.jediTaskID}"
                         else:
-                            optComment = None
-                        if not isOK:
-                            dispError[disp] = "Setupper._subscribeDistpatchDB() could not register location for prestage"
+                            opt_comment = None
+                        if not is_ok:
+                            disp_error[disp] = "Setupper._subscribeDispatchDB() could not register location for prestage"
                         else:
                             # register subscription
                             self.logger.debug(
                                 "%s %s %s"
                                 % (
                                     "registerDatasetSubscription",
-                                    (job.dispatchDBlock, dq2ID),
+                                    (job.dispatchDBlock, ddm_id),
                                     {
-                                        "activity": optActivity,
+                                        "activity": opt_activity,
                                         "lifetime": 7,
-                                        "dn": optOwner,
-                                        "comment": optComment,
+                                        "dn": opt_owner,
+                                        "comment": opt_comment,
                                     },
                                 )
                             )
-                            for iDDMTry in range(3):
+                            for _ in range(3):
                                 try:
                                     status = rucioAPI.register_dataset_subscription(
                                         job.dispatchDBlock,
-                                        [dq2ID],
-                                        activity=optActivity,
+                                        [ddm_id],
+                                        activity=opt_activity,
                                         lifetime=7,
-                                        distinguished_name=optOwner,
-                                        comment=optComment,
+                                        distinguished_name=opt_owner,
+                                        comment=opt_comment,
                                     )
                                     out = "OK"
                                     break
-                                except Exception as e:
+                                except Exception as error:
                                     status = False
-                                    out = f"registerDatasetSubscription failed with {str(e)} {traceback.format_exc()}"
+                                    out = f"registerDatasetSubscription failed with {str(error)} {traceback.format_exc()}"
                                     time.sleep(10)
                             if not status:
                                 self.logger.error(out)
-                                dispError[disp] = "Setupper._subscribeDistpatchDB() could not register subscription"
+                                disp_error[disp] = "Setupper._subscribeDispatchDB() could not register subscription"
                             else:
                                 self.logger.debug(out)
             # failed jobs
-            if dispError[disp] != "":
+            if disp_error[disp] != "":
                 if job.jobStatus != "failed":
                     job.jobStatus = "failed"
                     job.ddmErrorCode = ErrorCode.EC_Setupper
-                    job.ddmErrorDiag = dispError[disp]
+                    job.ddmErrorDiag = disp_error[disp]
                     self.logger.debug(f"failed PandaID={job.PandaID} with {job.ddmErrorDiag}")
-                    failedJobs.append(job)
+                    failed_jobs.append(job)
         # update failed jobs only. succeeded jobs should be activate by DDM callback
-        self.updateFailedJobs(failedJobs)
+        self.update_failed_jobs(failed_jobs)
         # submit ddm jobs
-        if ddmJobs != []:
-            ddmRet = self.taskBuffer.storeJobs(ddmJobs, ddmUser, joinThr=True)
+        if ddm_jobs:
+            ddm_ret = self.task_buffer.storeJobs(ddm_jobs, ddm_user, joinThr=True)
             # update datasets
-            ddmIndex = 0
-            ddmDsList = []
-            for ddmPandaID, ddmJobDef, ddmJobName in ddmRet:
+            ddm_index = 0
+            ddm_ds_list = []
+            for ddm_panda_id, _, _ in ddm_ret:
                 # invalid PandaID
-                if ddmPandaID in ["NULL", None]:
+                if ddm_panda_id in ["NULL", None]:
                     continue
                 # get dispatch dataset
-                dsName = ddmJobs[ddmIndex].jobParameters.split()[-1]
-                ddmIndex += 1
-                tmpDS = self.taskBuffer.queryDatasetWithMap({"name": dsName})
-                if tmpDS is not None:
+                ds_name = ddm_jobs[ddm_index].jobParameters.split()[-1]
+                ddm_index += 1
+                tmp_ds = self.task_buffer.queryDatasetWithMap({"name": ds_name})
+                if tmp_ds is not None:
                     # set MoverID
-                    tmpDS.MoverID = ddmPandaID
-                    ddmDsList.append(tmpDS)
+                    tmp_ds.MoverID = ddm_panda_id
+                    ddm_ds_list.append(tmp_ds)
             # update
-            if ddmDsList != []:
-                self.taskBuffer.updateDatasets(ddmDsList)
+            if ddm_ds_list:
+                self.task_buffer.updateDatasets(ddm_ds_list)
 
     # correct LFN for attemptNr
-    def _correctLFN(self):
-        lfnMap = {}
-        valMap = {}
-        prodError = {}
-        missingDS = {}
-        jobsWaiting = []
-        jobsFailed = []
-        jobsProcessed = []
-        allLFNs = {}
-        allGUIDs = {}
-        allScopes = {}
-        cloudMap = {}
-        lfnDsMap = {}
-        replicaMap = {}
+    def correct_lfn(self) -> None:
+        """
+        Correct lfn method for running the setup process.
+        """
+        lfn_map = {}
+        val_map = {}
+        prod_error = {}
+        missing_ds = {}
+        jobs_waiting = []
+        jobs_failed = []
+        jobs_processed = []
+        all_lfns = {}
+        all_guids = {}
+        all_scopes = {}
+        cloud_map = {}
+        lfn_ds_map = {}
+        replica_map = {}
         self.logger.debug("go into LFN correction")
         # collect input LFNs
-        inputLFNs = set()
-        for tmpJob in self.jobs:
-            for tmpFile in tmpJob.Files:
-                if tmpFile.type == "input":
-                    inputLFNs.add(tmpFile.lfn)
-                    genLFN = re.sub("\.\d+$", "", tmpFile.lfn)
-                    inputLFNs.add(genLFN)
-                    if tmpFile.GUID not in ["NULL", "", None]:
-                        if tmpFile.dataset not in self.lfnDatasetMap:
-                            self.lfnDatasetMap[tmpFile.dataset] = {}
-                        self.lfnDatasetMap[tmpFile.dataset][tmpFile.lfn] = {
-                            "guid": tmpFile.GUID,
-                            "chksum": tmpFile.checksum,
-                            "md5sum": tmpFile.md5sum,
-                            "fsize": tmpFile.fsize,
-                            "scope": tmpFile.scope,
+        input_lfns = set()
+        for tmp_job in self.jobs:
+            for tmp_file in tmp_job.Files:
+                if tmp_file.type == "input":
+                    input_lfns.add(tmp_file.lfn)
+                    gen_lfn = re.sub("\.\d+$", "", tmp_file.lfn)
+                    input_lfns.add(gen_lfn)
+                    if tmp_file.GUID not in ["NULL", "", None]:
+                        if tmp_file.dataset not in self.lfn_dataset_map:
+                            self.lfn_dataset_map[tmp_file.dataset] = {}
+                        self.lfn_dataset_map[tmp_file.dataset][tmp_file.lfn] = {
+                            "guid": tmp_file.GUID,
+                            "chksum": tmp_file.checksum,
+                            "md5sum": tmp_file.md5sum,
+                            "fsize": tmp_file.fsize,
+                            "scope": tmp_file.scope,
                         }
         # loop over all jobs
         for job in self.jobs:
-            if self.onlyTA:
+            if self.only_ta:
                 self.logger.debug(f"start TA session {job.taskID}")
             # check if sitename is known
-            if job.computingSite != "NULL" and job.computingSite not in self.siteMapper.siteSpecList:
+            if job.computingSite != "NULL" and job.computingSite not in self.site_mapper.siteSpecList:
                 job.jobStatus = "failed"
                 job.ddmErrorCode = ErrorCode.EC_Setupper
                 job.ddmErrorDiag = f"computingSite:{job.computingSite} is unknown"
                 # append job for downstream process
-                jobsProcessed.append(job)
+                jobs_processed.append(job)
                 # error message for TA
-                if self.onlyTA:
+                if self.only_ta:
                     self.logger.error(job.ddmErrorDiag)
                 continue
             # ignore no prodDBlock jobs or container dataset
             if job.prodDBlock == "NULL":
                 # append job to processed list
-                jobsProcessed.append(job)
+                jobs_processed.append(job)
                 continue
             # check if T1
-            tmpSrcID = self.siteMapper.getCloud(job.getCloud())["source"]
-            srcSiteSpec = self.siteMapper.getSite(tmpSrcID)
-            src_scope_input, src_scope_output = select_scope(srcSiteSpec, job.prodSourceLabel, job.job_label)
+            tmp_src_id = self.site_mapper.getCloud(job.getCloud())["source"]
+            src_site_spec = self.site_mapper.getSite(tmp_src_id)
+            _, src_scope_output = select_scope(src_site_spec, job.prodSourceLabel, job.job_label)
             # could happen if wrong configuration or downtime
-            if src_scope_output in srcSiteSpec.ddm_output:
-                srcDQ2ID = srcSiteSpec.ddm_output[src_scope_output]
+            if src_scope_output in src_site_spec.ddm_output:
+                src_ddm_id = src_site_spec.ddm_output[src_scope_output]
             else:
-                errMsg = f"Source site {tmpSrcID} has no {src_scope_output} endpoint (ddm_output {srcSiteSpec.ddm_output})"
-                self.logger.error(f"< jediTaskID={job.taskID} PandaID={job.PandaID} > {errMsg}")
+                err_msg = f"Source site {tmp_src_id} has no {src_scope_output} endpoint (ddm_output {src_site_spec.ddm_output})"
+                self.logger.error(f"< jediTaskID={job.taskID} PandaID={job.PandaID} > {err_msg}")
                 job.jobStatus = "failed"
                 job.ddmErrorCode = ErrorCode.EC_RSE
-                job.ddmErrorDiag = errMsg
-                jobsFailed.append(job)
+                job.ddmErrorDiag = err_msg
+                jobs_failed.append(job)
                 continue
-            dstSiteSpec = self.siteMapper.getSite(job.computingSite)
-            dst_scope_input, dst_scope_output = select_scope(dstSiteSpec, job.prodSourceLabel, job.job_label)
+            dst_site_spec = self.site_mapper.getSite(job.computingSite)
+            dst_scope_input, _ = select_scope(dst_site_spec, job.prodSourceLabel, job.job_label)
             # could happen if wrong configuration or downtime
-            if dst_scope_input in dstSiteSpec.ddm_input:
-                dstDQ2ID = dstSiteSpec.ddm_input[dst_scope_input]
+            if dst_scope_input in dst_site_spec.ddm_input:
+                dst_ddm_id = dst_site_spec.ddm_input[dst_scope_input]
             else:
-                errMsg = f"computingsite {job.computingSite} has no {dst_scope_input} endpoint (ddm_input {dstSiteSpec.ddm_input})"
-                self.logger.error(f"< jediTaskID={job.taskID} PandaID={job.PandaID} > {errMsg}")
+                err_msg = f"computingsite {job.computingSite} has no {dst_scope_input} endpoint (ddm_input {dst_site_spec.ddm_input})"
+                self.logger.error(f"< jediTaskID={job.taskID} PandaID={job.PandaID} > {err_msg}")
                 job.jobStatus = "failed"
                 job.ddmErrorCode = ErrorCode.EC_RSE
-                job.ddmErrorDiag = errMsg
-                jobsFailed.append(job)
+                job.ddmErrorDiag = err_msg
+                jobs_failed.append(job)
                 continue
             # collect datasets
             datasets = []
             for file in job.Files:
                 if file.type == "input" and file.dispatchDBlock == "NULL" and (file.GUID == "NULL" or job.prodSourceLabel in ["managed", "test", "ptest"]):
                     if file.dataset not in datasets:
                         datasets.append(file.dataset)
-                if srcDQ2ID == dstDQ2ID and file.type == "input" and job.prodSourceLabel in ["managed", "test", "ptest"] and file.status != "ready":
-                    if job.getCloud() not in self.missingFilesInT1:
-                        self.missingFilesInT1[job.getCloud()] = set()
-                    self.missingFilesInT1[job.getCloud()].add(file.lfn)
+                if src_ddm_id == dst_ddm_id and file.type == "input" and job.prodSourceLabel in ["managed", "test", "ptest"] and file.status != "ready":
+                    if job.getCloud() not in self.missing_files_in_t1:
+                        self.missing_files_in_t1[job.getCloud()] = set()
+                    self.missing_files_in_t1[job.getCloud()].add(file.lfn)
             # get LFN list
             for dataset in datasets:
-                if dataset not in lfnMap:
-                    prodError[dataset] = ""
-                    lfnMap[dataset] = {}
+                if dataset not in lfn_map:
+                    prod_error[dataset] = ""
+                    lfn_map[dataset] = {}
                     # get LFNs
-                    status, out = self.getListFilesInDataset(dataset, inputLFNs)
+                    status, out = self.get_list_files_in_dataset(dataset, input_lfns)
                     if status != 0:
                         self.logger.error(out)
-                        prodError[dataset] = f"could not get file list of prodDBlock {dataset}"
-                        self.logger.error(prodError[dataset])
-                        # doesn't exist in DQ2
+                        prod_error[dataset] = f"could not get file list of prodDBlock {dataset}"
+                        self.logger.error(prod_error[dataset])
+                        # doesn't exist in DDM
                         if status == -1:
-                            missingDS[dataset] = f"DS:{dataset} not found in DDM"
+                            missing_ds[dataset] = f"DS:{dataset} not found in DDM"
                         else:
-                            missingDS[dataset] = out
+                            missing_ds[dataset] = out
                     else:
                         # make map (key: LFN w/o attemptNr, value: LFN with attemptNr)
                         items = out
                         try:
                             # loop over all files
-                            for tmpLFN in items:
-                                vals = items[tmpLFN]
-                                valMap[tmpLFN] = vals
-                                genLFN = re.sub("\.\d+$", "", tmpLFN)
-                                if genLFN in lfnMap[dataset]:
+                            for tmp_lfn in items:
+                                vals = items[tmp_lfn]
+                                val_map[tmp_lfn] = vals
+                                gen_lfn = re.sub("\.\d+$", "", tmp_lfn)
+                                if gen_lfn in lfn_map[dataset]:
                                     # get attemptNr
-                                    newAttNr = 0
-                                    newMat = re.search("\.(\d+)$", tmpLFN)
-                                    if newMat is not None:
-                                        newAttNr = int(newMat.group(1))
-                                    oldAttNr = 0
-                                    oldMat = re.search("\.(\d+)$", lfnMap[dataset][genLFN])
-                                    if oldMat is not None:
-                                        oldAttNr = int(oldMat.group(1))
+                                    new_att_nr = 0
+                                    new_mat = re.search("\.(\d+)$", tmp_lfn)
+                                    if new_mat is not None:
+                                        new_att_nr = int(new_mat.group(1))
+                                    old_att_nr = 0
+                                    old_mat = re.search("\.(\d+)$", lfn_map[dataset][gen_lfn])
+                                    if old_mat is not None:
+                                        old_att_nr = int(old_mat.group(1))
                                     # compare
-                                    if newAttNr > oldAttNr:
-                                        lfnMap[dataset][genLFN] = tmpLFN
+                                    if new_att_nr > old_att_nr:
+                                        lfn_map[dataset][gen_lfn] = tmp_lfn
                                 else:
-                                    lfnMap[dataset][genLFN] = tmpLFN
+                                    lfn_map[dataset][gen_lfn] = tmp_lfn
                                 # mapping from LFN to DS
-                                lfnDsMap[lfnMap[dataset][genLFN]] = dataset
+                                lfn_ds_map[lfn_map[dataset][gen_lfn]] = dataset
                         except Exception:
-                            prodError[dataset] = f"could not convert HTTP-res to map for prodDBlock {dataset}"
-                            self.logger.error(prodError[dataset])
+                            prod_error[dataset] = f"could not convert HTTP-res to map for prodDBlock {dataset}"
+                            self.logger.error(prod_error[dataset])
                             self.logger.error(out)
                     # get replica locations
-                    if (self.onlyTA or job.prodSourceLabel in ["managed", "test"]) and prodError[dataset] == "" and dataset not in replicaMap:
+                    if (self.only_ta or job.prodSourceLabel in ["managed", "test"]) and prod_error[dataset] == "" and dataset not in replica_map:
                         if dataset.endswith("/"):
-                            status, out = self.getListDatasetReplicasInContainer(dataset, True)
+                            status, out = self.get_list_dataset_replicas_in_container(dataset, True)
                         else:
-                            status, out = self.getListDatasetReplicas(dataset)
+                            status, out = self.get_list_dataset_replicas(dataset)
                         if not status:
-                            prodError[dataset] = f"could not get locations for {dataset}"
-                            self.logger.error(prodError[dataset])
+                            prod_error[dataset] = f"could not get locations for {dataset}"
+                            self.logger.error(prod_error[dataset])
                             self.logger.error(out)
                         else:
-                            replicaMap[dataset] = out
+                            replica_map[dataset] = out
                             # append except DBR
                             if not dataset.startswith("ddo"):
-                                self.replicaMapForBroker[dataset] = out
+                                self.replica_map_for_broker[dataset] = out
             # error
-            isFailed = False
+            is_failed = False
             # check for failed
             for dataset in datasets:
-                if dataset in missingDS:
+                if dataset in missing_ds:
                     job.jobStatus = "failed"
                     job.ddmErrorCode = ErrorCode.EC_GUID
-                    job.ddmErrorDiag = missingDS[dataset]
+                    job.ddmErrorDiag = missing_ds[dataset]
                     # set missing
-                    for tmpFile in job.Files:
-                        if tmpFile.dataset == dataset:
-                            tmpFile.status = "missing"
+                    for tmp_file in job.Files:
+                        if tmp_file.dataset == dataset:
+                            tmp_file.status = "missing"
                     # append
-                    jobsFailed.append(job)
-                    isFailed = True
-                    self.logger.debug(f"{job.PandaID} failed with {missingDS[dataset]}")
+                    jobs_failed.append(job)
+                    is_failed = True
+                    self.logger.debug(f"{job.PandaID} failed with {missing_ds[dataset]}")
                     break
-            if isFailed:
+            if is_failed:
                 continue
             # check for waiting
             for dataset in datasets:
-                if prodError[dataset] != "":
+                if prod_error[dataset] != "":
                     # append job to waiting list
-                    jobsWaiting.append(job)
-                    isFailed = True
+                    jobs_waiting.append(job)
+                    is_failed = True
                     # message for TA
-                    if self.onlyTA:
-                        self.logger.error(prodError[dataset])
+                    if self.only_ta:
+                        self.logger.error(prod_error[dataset])
                     break
-            if isFailed:
+            if is_failed:
                 continue
-            if not self.onlyTA:
+            if not self.only_ta:
                 # replace generic LFN with real LFN
-                replaceList = []
-                isFailed = False
+                replace_list = []
+                is_failed = False
                 for file in job.Files:
                     if file.type == "input" and file.dispatchDBlock == "NULL":
-                        addToLfnMap = True
+                        add_to_lfn_map = True
                         if file.GUID == "NULL":
                             # get LFN w/o attemptNr
                             basename = re.sub("\.\d+$", "", file.lfn)
                             if basename == file.lfn:
                                 # replace
-                                if basename in lfnMap[file.dataset]:
-                                    file.lfn = lfnMap[file.dataset][basename]
-                                    replaceList.append((basename, file.lfn))
+                                if basename in lfn_map[file.dataset]:
+                                    file.lfn = lfn_map[file.dataset][basename]
+                                    replace_list.append((basename, file.lfn))
                             # set GUID
-                            if file.lfn in valMap:
-                                file.GUID = valMap[file.lfn]["guid"]
-                                file.fsize = valMap[file.lfn]["fsize"]
-                                file.md5sum = valMap[file.lfn]["md5sum"]
-                                file.checksum = valMap[file.lfn]["chksum"]
-                                file.scope = valMap[file.lfn]["scope"]
+                            if file.lfn in val_map:
+                                file.GUID = val_map[file.lfn]["guid"]
+                                file.fsize = val_map[file.lfn]["fsize"]
+                                file.md5sum = val_map[file.lfn]["md5sum"]
+                                file.checksum = val_map[file.lfn]["chksum"]
+                                file.scope = val_map[file.lfn]["scope"]
                                 # remove white space
                                 if file.md5sum is not None:
                                     file.md5sum = file.md5sum.strip()
                                 if file.checksum is not None:
                                     file.checksum = file.checksum.strip()
                         else:
                             if job.prodSourceLabel not in ["managed", "test"]:
-                                addToLfnMap = False
+                                add_to_lfn_map = False
                         # check missing file
                         if file.GUID == "NULL" or job.prodSourceLabel in [
                             "managed",
                             "test",
                         ]:
-                            if file.lfn not in valMap:
+                            if file.lfn not in val_map:
                                 # append job to waiting list
-                                errMsg = f"GUID for {file.lfn} not found in rucio"
-                                self.logger.error(errMsg)
+                                err_msg = f"GUID for {file.lfn} not found in rucio"
+                                self.logger.error(err_msg)
                                 file.status = "missing"
-                                if job not in jobsFailed:
+                                if job not in jobs_failed:
                                     job.jobStatus = "failed"
                                     job.ddmErrorCode = ErrorCode.EC_GUID
-                                    job.ddmErrorDiag = errMsg
-                                    jobsFailed.append(job)
-                                    isFailed = True
+                                    job.ddmErrorDiag = err_msg
+                                    jobs_failed.append(job)
+                                    is_failed = True
                                 continue
-                        # add to allLFNs/allGUIDs
-                        if addToLfnMap:
-                            allLFNs.setdefault(job.getCloud(), [])
-                            allGUIDs.setdefault(job.getCloud(), [])
-                            allScopes.setdefault(job.getCloud(), [])
-                            allLFNs[job.getCloud()].append(file.lfn)
-                            allGUIDs[job.getCloud()].append(file.GUID)
-                            allScopes[job.getCloud()].append(file.scope)
+                        # add to all_lfns/all_guids
+                        if add_to_lfn_map:
+                            all_lfns.setdefault(job.getCloud(), [])
+                            all_guids.setdefault(job.getCloud(), [])
+                            all_scopes.setdefault(job.getCloud(), [])
+                            all_lfns[job.getCloud()].append(file.lfn)
+                            all_guids[job.getCloud()].append(file.GUID)
+                            all_scopes[job.getCloud()].append(file.scope)
                 # modify jobParameters
-                if not isFailed:
-                    for patt, repl in replaceList:
+                if not is_failed:
+                    for patt, repl in replace_list:
                         job.jobParameters = re.sub(f"{patt} ", f"{repl} ", job.jobParameters)
                     # append job to processed list
-                    jobsProcessed.append(job)
+                    jobs_processed.append(job)
         # return if TA only
-        if self.onlyTA:
+        if self.only_ta:
             self.logger.debug("end TA sessions")
             return
         # set data summary fields
-        for tmpJob in self.jobs:
+        for tmp_job in self.jobs:
             try:
                 # set only for production/analysis/test
-                if tmpJob.prodSourceLabel not in ["managed", "test", "user", "prod_test"] + JobUtils.list_ptest_prod_sources:
+                if tmp_job.prodSourceLabel not in ["managed", "test", "user", "prod_test"] + JobUtils.list_ptest_prod_sources:
                     continue
                 # loop over all files
-                tmpJob.nInputDataFiles = 0
-                tmpJob.inputFileBytes = 0
-                tmpInputFileProject = None
-                tmpInputFileType = None
-                for tmpFile in tmpJob.Files:
+                tmp_job.nInputDataFiles = 0
+                tmp_job.inputFileBytes = 0
+                tmp_input_file_project = None
+                tmp_input_file_type = None
+                for tmp_file in tmp_job.Files:
                     # use input files and ignore DBR/lib.tgz
-                    if tmpFile.type == "input" and (not tmpFile.dataset.startswith("ddo")) and not tmpFile.lfn.endswith(".lib.tgz"):
-                        tmpJob.nInputDataFiles += 1
-                        if tmpFile.fsize not in ["NULL", None, 0, "0"]:
-                            tmpJob.inputFileBytes += tmpFile.fsize
+                    if tmp_file.type == "input" and (not tmp_file.dataset.startswith("ddo")) and not tmp_file.lfn.endswith(".lib.tgz"):
+                        tmp_job.nInputDataFiles += 1
+                        if tmp_file.fsize not in ["NULL", None, 0, "0"]:
+                            tmp_job.inputFileBytes += tmp_file.fsize
                         # get input type and project
-                        if tmpInputFileProject is None:
-                            tmpInputItems = tmpFile.dataset.split(".")
+                        if tmp_input_file_project is None:
+                            tmp_input_items = tmp_file.dataset.split(".")
                             # input project
-                            tmpInputFileProject = tmpInputItems[0].split(":")[-1]
+                            tmp_input_file_project = tmp_input_items[0].split(":")[-1]
                             # input type. ignore user/group/groupXY
                             if (
-                                len(tmpInputItems) > 4
-                                and (not tmpInputItems[0] in ["", "NULL", "user", "group"])
-                                and (not tmpInputItems[0].startswith("group"))
-                                and not tmpFile.dataset.startswith("panda.um.")
+                                len(tmp_input_items) > 4
+                                and (not tmp_input_items[0] in ["", "NULL", "user", "group"])
+                                and (not tmp_input_items[0].startswith("group"))
+                                and not tmp_file.dataset.startswith("panda.um.")
                             ):
-                                tmpInputFileType = tmpInputItems[4]
+                                tmp_input_file_type = tmp_input_items[4]
                 # set input type and project
-                if tmpJob.prodDBlock not in ["", None, "NULL"]:
+                if tmp_job.prodDBlock not in ["", None, "NULL"]:
                     # input project
-                    if tmpInputFileProject is not None:
-                        tmpJob.inputFileProject = tmpInputFileProject
+                    if tmp_input_file_project is not None:
+                        tmp_job.inputFileProject = tmp_input_file_project
                     # input type
-                    if tmpInputFileType is not None:
-                        tmpJob.inputFileType = tmpInputFileType
+                    if tmp_input_file_type is not None:
+                        tmp_job.inputFileType = tmp_input_file_type
                 # protection
-                maxInputFileBytes = 99999999999
-                if tmpJob.inputFileBytes > maxInputFileBytes:
-                    tmpJob.inputFileBytes = maxInputFileBytes
+                max_input_file_bytes = 99999999999
+                tmp_job.inputFileBytes = min(tmp_job.inputFileBytes, max_input_file_bytes)
                 # set background-able flag
-                tmpJob.setBackgroundableFlag()
+                tmp_job.setBackgroundableFlag()
             except Exception:
-                errType, errValue = sys.exc_info()[:2]
-                self.logger.error(f"failed to set data summary fields for PandaID={tmpJob.PandaID}: {errType} {errValue}")
-        # send jobs to jobsWaiting
-        self.taskBuffer.keepJobs(jobsWaiting)
+                error_type, error_value = sys.exc_info()[:2]
+                self.logger.error(f"failed to set data summary fields for PandaID={tmp_job.PandaID}: {error_type} {error_value}")
+        # send jobs to jobs_waiting
+        self.task_buffer.keepJobs(jobs_waiting)
         # update failed job
-        self.updateFailedJobs(jobsFailed)
+        self.update_failed_jobs(jobs_failed)
         # remove waiting/failed jobs
-        self.jobs = jobsProcessed
+        self.jobs = jobs_processed
         # delete huge variables
-        del lfnMap
-        del valMap
-        del prodError
-        del jobsWaiting
-        del jobsProcessed
-        del allLFNs
-        del allGUIDs
-        del cloudMap
+        del lfn_map
+        del val_map
+        del prod_error
+        del jobs_waiting
+        del jobs_processed
+        del all_lfns
+        del all_guids
+        del cloud_map
 
     # remove waiting jobs
-    def removeWaitingJobs(self):
-        jobsWaiting = []
-        jobsProcessed = []
-        for tmpJob in self.jobs:
-            if tmpJob.jobStatus == "waiting":
-                jobsWaiting.append(tmpJob)
+    def remove_waiting_jobs(self) -> None:
+        """
+        Remove waiting jobs method for running the setup process.
+        """
+        jobs_waiting = []
+        jobs_processed = []
+        for tmp_job in self.jobs:
+            if tmp_job.jobStatus == "waiting":
+                jobs_waiting.append(tmp_job)
             else:
-                jobsProcessed.append(tmpJob)
-        # send jobs to jobsWaiting
-        self.taskBuffer.keepJobs(jobsWaiting)
+                jobs_processed.append(tmp_job)
+        # send jobs to jobs_waiting
+        self.task_buffer.keepJobs(jobs_waiting)
         # remove waiting/failed jobs
-        self.jobs = jobsProcessed
+        self.jobs = jobs_processed
 
     # memory checker
-    def _memoryCheck(self):
+    def memory_check(self) -> None:
+        """
+        Memory check method for running the setup process.
+        """
         try:
             import os
 
             proc_status = "/proc/%d/status" % os.getpid()
-            procfile = open(proc_status)
+            proc_file = open(proc_status)
             name = ""
-            vmSize = ""
-            vmRSS = ""
+            vm_size = ""
+            vm_rss = ""
             # extract Name,VmSize,VmRSS
-            for line in procfile:
+            for line in proc_file:
                 if line.startswith("Name:"):
                     name = line.split()[-1]
                     continue
                 if line.startswith("VmSize:"):
-                    vmSize = ""
+                    vm_size = ""
                     for item in line.split()[1:]:
-                        vmSize += item
+                        vm_size += item
                     continue
                 if line.startswith("VmRSS:"):
-                    vmRSS = ""
+                    vm_rss = ""
                     for item in line.split()[1:]:
-                        vmRSS += item
+                        vm_rss += item
                     continue
-            procfile.close()
-            self.logger.debug(f"MemCheck PID={os.getpid()} Name={name} VSZ={vmSize} RSS={vmRSS}")
+            proc_file.close()
+            self.logger.debug(f"MemCheck PID={os.getpid()} Name={name} VSZ={vm_size} RSS={vm_rss}")
         except Exception:
-            errtype, errvalue = sys.exc_info()[:2]
-            self.logger.error(f"memoryCheck() : {errtype} {errvalue}")
+            error_type, error_value = sys.exc_info()[:2]
+            self.logger.error(f"memoryCheck() : {error_type} {error_value}")
             self.logger.debug(f"MemCheck PID={os.getpid()} unknown")
             return
 
     # get list of files in dataset
-    def getListFilesInDataset(self, dataset, fileList=None, useCache=True):
+    def get_list_files_in_dataset(self, dataset: str, file_list: Optional[List[str]] = None, use_cache: bool = True) -> Tuple[int, List[str]]:
+        """
+        Get list files in dataset method for running the setup process.
+
+        :param dataset: The dataset to get the list of files from.
+        :param file_list: The list of files. Defaults to None.
+        :param use_cache: Whether to use cache. Defaults to True.
+        :return: A tuple containing the status and the list of files.
+        """
         # use cache data
-        if useCache and dataset in self.lfnDatasetMap:
-            return 0, self.lfnDatasetMap[dataset]
-        for iDDMTry in range(3):
+        if use_cache and dataset in self.lfn_dataset_map:
+            return 0, self.lfn_dataset_map[dataset]
+        for _ in range(3):
             try:
                 self.logger.debug("listFilesInDataset " + dataset)
-                items, tmpDummy = rucioAPI.list_files_in_dataset(dataset, file_list=fileList)
+                items, _ = rucioAPI.list_files_in_dataset(dataset, file_list=file_list)
                 status = 0
                 break
             except DataIdentifierNotFound:
                 status = -1
                 break
             except Exception:
                 status = -2
         if status != 0:
-            errType, errValue = sys.exc_info()[:2]
-            out = f"{errType} {errValue}"
+            error_type, error_value = sys.exc_info()[:2]
+            out = f"{error_type} {error_value}"
             return status, out
         # keep to avoid redundant lookup
-        self.lfnDatasetMap[dataset] = items
+        self.lfn_dataset_map[dataset] = items
         return status, items
 
     # get list of datasets in container
-    def getListDatasetInContainer(self, container):
+    def get_list_dataset_in_container(self, container: str) -> Tuple[bool, List[str]]:
+        """
+        Get list dataset in container method for running the setup process.
+
+        :param container: The container to get the list of datasets from.
+        :return: A tuple containing a boolean indicating the status and the list of datasets.
+        """
         # get datasets in container
         self.logger.debug("listDatasetsInContainer " + container)
-        for iDDMTry in range(3):
+        for _ in range(3):
             datasets, out = rucioAPI.list_datasets_in_container(container)
-            if datasets is None:
-                time.sleep(10)
-            else:
-                break
-        if datasets is None:
-            self.logger.error(out)
-            return False, out
-        return True, datasets
-
-    def getListDatasetReplicasInContainer(self, container, getMap=False):
-        # get datasets in container
+            if datasets is not None:
+                return True, datasets
+            time.sleep(10)
+        self.logger.error(out)
+        return False, out
+
+
+    # get datasets in container
+    def get_list_dataset_replicas_in_container(self, container: str, get_map: bool = False) -> Tuple[int, str]:
+        """
+        Get list dataset replicas in container method for running the setup process.
+
+        :param container: The container to get the list of dataset replicas from.
+        :param get_map: Whether to get the map. Defaults to False.
+        :return: A tuple containing the status and the map of dataset replicas.
+        """
         self.logger.debug("listDatasetsInContainer " + container)
-        for iDDMTry in range(3):
+        for _ in range(3):
             datasets, out = rucioAPI.list_datasets_in_container(container)
             if datasets is None:
                 time.sleep(10)
             else:
                 break
         if datasets is None:
             self.logger.error(out)
-            if getMap:
+            if get_map:
                 return False, out
             return 1, out
         # loop over all datasets
-        allRepMap = {}
+        all_rep_map = {}
         for dataset in datasets:
             self.logger.debug("listDatasetReplicas " + dataset)
-            status, out = self.getListDatasetReplicas(dataset)
+            status, out = self.get_list_dataset_replicas(dataset)
             self.logger.debug(out)
             if not status:
-                if getMap:
+                if get_map:
                     return False, out
                 return status, out
-            tmpRepSites = out
+            tmp_rep_sites = out
             # get map
-            if getMap:
-                allRepMap[dataset] = tmpRepSites
+            if get_map:
+                all_rep_map[dataset] = tmp_rep_sites
                 continue
             # otherwise get sum
-            for siteId in tmpRepSites:
-                statList = tmpRepSites[siteId]
-                if siteId not in allRepMap:
+            for site_id in tmp_rep_sites:
+                stat_list = tmp_rep_sites[site_id]
+                if site_id not in all_rep_map:
                     # append
-                    allRepMap[siteId] = [
-                        statList[-1],
+                    all_rep_map[site_id] = [
+                        stat_list[-1],
                     ]
                 else:
                     # add
-                    newStMap = {}
-                    for stName in allRepMap[siteId][0]:
-                        stNum = allRepMap[siteId][0][stName]
-                        if stName in statList[-1]:
+                    new_st_map = {}
+                    for st_name in all_rep_map[site_id][0]:
+                        st_num = all_rep_map[site_id][0][st_name]
+                        if st_name in stat_list[-1]:
                             # try mainly for archived=None
                             try:
-                                newStMap[stName] = stNum + statList[-1][stName]
+                                new_st_map[st_name] = st_num + stat_list[-1][st_name]
                             except Exception:
-                                newStMap[stName] = stNum
+                                new_st_map[st_name] = st_num
                         else:
-                            newStMap[stName] = stNum
-                    allRepMap[siteId] = [
-                        newStMap,
+                            new_st_map[st_name] = st_num
+                    all_rep_map[site_id] = [
+                        new_st_map,
                     ]
         # return
-        self.logger.debug(str(allRepMap))
-        if getMap:
-            return True, allRepMap
-        return 0, str(allRepMap)
+        self.logger.debug(str(all_rep_map))
+        if get_map:
+            return True, all_rep_map
+        return 0, str(all_rep_map)
 
     # get list of replicas for a dataset
-    def getListDatasetReplicas(self, dataset, getMap=True):
-        nTry = 3
-        for iDDMTry in range(nTry):
-            self.logger.debug(f"{iDDMTry}/{nTry} listDatasetReplicas {dataset}")
+    def get_list_dataset_replicas(self, dataset: str, get_map: bool = True) -> Tuple[bool, str]:
+        """
+        Get list dataset replicas method for running the setup process.
+
+        :param dataset: The dataset to get the list of replicas from.
+        :param get_map: Whether to get the map. Defaults to True.
+        :return: A tuple containing a boolean indicating the status and the map of dataset replicas.
+        """
+        for attempt in range(3):
+            self.logger.debug(f"{attempt}/{3} listDatasetReplicas {dataset}")
             status, out = rucioAPI.list_dataset_replicas(dataset)
             if status != 0:
                 time.sleep(10)
             else:
                 break
         # result
         if status != 0:
             self.logger.error(out)
             self.logger.error(f"bad response for {dataset}")
-            if getMap:
+            if get_map:
                 return False, {}
             else:
                 return 1, str({})
         try:
-            retMap = out
-            self.logger.debug(f"getListDatasetReplicas->{str(retMap)}")
-            if getMap:
-                return True, retMap
+            ret_map = out
+            self.logger.debug(f"getListDatasetReplicas->{str(ret_map)}")
+            if get_map:
+                return True, ret_map
             else:
-                return 0, str(retMap)
+                return 0, str(ret_map)
         except Exception:
             self.logger.error(out)
             self.logger.error(f"could not convert HTTP-res to replica map for {dataset}")
-            if getMap:
+            if get_map:
                 return False, {}
             else:
                 return 1, str({})
 
     # dynamic data placement for analysis jobs
-    def _dynamicDataPlacement(self):
+    def dynamic_data_placement(self) -> None:
+        """
+        Dynamic data placement method for running the setup process.
+        """
         # only first submission
-        if not self.firstSubmission:
+        if not self.first_submission:
             return
         # no jobs
         if len(self.jobs) == 0:
             return
         # only successful analysis
         if self.jobs[0].jobStatus in ["failed", "cancelled"] or self.jobs[0].isCancelled() or (not self.jobs[0].prodSourceLabel in ["user", "panda"]):
             return
         # disable for JEDI
         if self.jobs[0].lockedby == "jedi":
             return
         return
 
     # make dis datasets for existing files to avoid deletion when jobs are queued
-    def _makeDisDatasetsForExistingfiles(self):
+    def make_dis_datasets_for_existing_files(self) -> None:
+        """
+        Make dis datasets for existing files method for running the setup process.
+        """
         self.logger.debug("make dis datasets for existing files")
         # collect existing files
-        dsFileMap = {}
-        nMaxJobs = 20
-        nJobsMap = {}
-        for tmpJob in self.jobs:
+        dataset_file_map = {}
+        n_max_jobs = 20
+        n_jobs_map = {}
+        for tmp_job in self.jobs:
             # use production or test jobs only
-            if tmpJob.prodSourceLabel not in ["managed", "test"]:
+            if tmp_job.prodSourceLabel not in ["managed", "test"]:
                 continue
             # skip for prefetcher or transferType=direct
-            if tmpJob.usePrefetcher() or tmpJob.transferType == "direct":
+            if tmp_job.usePrefetcher() or tmp_job.transferType == "direct":
                 continue
             # ignore inappropriate status
-            if tmpJob.jobStatus in ["failed", "cancelled", "waiting"] or tmpJob.isCancelled():
+            if tmp_job.jobStatus in ["failed", "cancelled", "waiting"] or tmp_job.isCancelled():
                 continue
             # check cloud
-            if tmpJob.getCloud() == "ND" and self.siteMapper.getSite(tmpJob.computingSite).cloud == "ND":
+            if tmp_job.getCloud() == "ND" and self.site_mapper.getSite(tmp_job.computingSite).cloud == "ND":
                 continue
             # look for log _sub dataset to be used as a key
-            logSubDsName = ""
-            for tmpFile in tmpJob.Files:
-                if tmpFile.type == "log":
-                    logSubDsName = tmpFile.destinationDBlock
+            log_sub_ds_name = ""
+            for tmp_file in tmp_job.Files:
+                if tmp_file.type == "log":
+                    log_sub_ds_name = tmp_file.destinationDBlock
                     break
             # append site
-            destSite = self.siteMapper.getSite(tmpJob.computingSite)
-            scope_dest_input, scope_dest_output = select_scope(destSite, tmpJob.prodSourceLabel, tmpJob.job_label)
-            destDQ2ID = destSite.ddm_input[scope_dest_input]
+            dest_site = self.site_mapper.getSite(tmp_job.computingSite)
+            scope_dest_input, _ = select_scope(dest_site, tmp_job.prodSourceLabel, tmp_job.job_label)
+            dest_ddm_id = dest_site.ddm_input[scope_dest_input]
             # T1 used as T2
             if (
-                tmpJob.getCloud() != self.siteMapper.getSite(tmpJob.computingSite).cloud
-                and not destDQ2ID.endswith("PRODDISK")
-                and self.siteMapper.getSite(tmpJob.computingSite).cloud in ["US"]
+                tmp_job.getCloud() != self.site_mapper.getSite(tmp_job.computingSite).cloud
+                and not dest_ddm_id.endswith("PRODDISK")
+                and self.site_mapper.getSite(tmp_job.computingSite).cloud in ["US"]
             ):
-                tmpSiteSpec = self.siteMapper.getSite(tmpJob.computingSite)
-                scope_tmpSite_input, scope_tmpSite_output = select_scope(tmpSiteSpec, tmpJob.prodSourceLabel, tmpJob.job_label)
-                tmpSeTokens = tmpSiteSpec.setokens_input[scope_tmpSite_input]
-                if "ATLASPRODDISK" in tmpSeTokens:
-                    destDQ2ID = tmpSeTokens["ATLASPRODDISK"]
+                tmp_site_spec = self.site_mapper.getSite(tmp_job.computingSite)
+                scope_tmp_site_input, _ = select_scope(tmp_site_spec, tmp_job.prodSourceLabel, tmp_job.job_label)
+                tmp_se_tokens = tmp_site_spec.setokens_input[scope_tmp_site_input]
+                if "ATLASPRODDISK" in tmp_se_tokens:
+                    dest_ddm_id = tmp_se_tokens["ATLASPRODDISK"]
             # backend
-            ddmBackEnd = "rucio"
-            mapKeyJob = (destDQ2ID, logSubDsName)
+            ddm_back_end = "rucio"
+            map_key_job = (dest_ddm_id, log_sub_ds_name)
             # increment the number of jobs per key
-            if mapKeyJob not in nJobsMap:
-                nJobsMap[mapKeyJob] = 0
-            mapKey = (
-                destDQ2ID,
-                logSubDsName,
-                nJobsMap[mapKeyJob] // nMaxJobs,
-                ddmBackEnd,
+            if map_key_job not in n_jobs_map:
+                n_jobs_map[map_key_job] = 0
+            map_key = (
+                dest_ddm_id,
+                log_sub_ds_name,
+                n_jobs_map[map_key_job] // n_max_jobs,
+                ddm_back_end,
             )
-            nJobsMap[mapKeyJob] += 1
-            if mapKey not in dsFileMap:
-                dsFileMap[mapKey] = {}
+            n_jobs_map[map_key_job] += 1
+            if map_key not in dataset_file_map:
+                dataset_file_map[map_key] = {}
             # add files
-            for tmpFile in tmpJob.Files:
-                if tmpFile.type != "input":
+            for tmp_file in tmp_job.Files:
+                if tmp_file.type != "input":
                     continue
                 # if files are unavailable at the dest site normal dis datasets contain them
                 # or files are cached
-                if tmpFile.status not in ["ready"]:
+                if tmp_file.status not in ["ready"]:
                     continue
                 # if available at T2
-                realDestDQ2ID = (destDQ2ID,)
+                real_dest_ddm_id = (dest_ddm_id,)
                 if (
-                    tmpJob.getCloud() in self.availableLFNsInT2
-                    and tmpFile.dataset in self.availableLFNsInT2[tmpJob.getCloud()]
-                    and tmpJob.computingSite in self.availableLFNsInT2[tmpJob.getCloud()][tmpFile.dataset]["sites"]
-                    and tmpFile.lfn in self.availableLFNsInT2[tmpJob.getCloud()][tmpFile.dataset]["sites"][tmpJob.computingSite]
+                    tmp_job.getCloud() in self.available_lfns_in_t2
+                    and tmp_file.dataset in self.available_lfns_in_t2[tmp_job.getCloud()]
+                    and tmp_job.computingSite in self.available_lfns_in_t2[tmp_job.getCloud()][tmp_file.dataset]["sites"]
+                    and tmp_file.lfn in self.available_lfns_in_t2[tmp_job.getCloud()][tmp_file.dataset]["sites"][tmp_job.computingSite]
                 ):
-                    realDestDQ2ID = self.availableLFNsInT2[tmpJob.getCloud()][tmpFile.dataset]["siteDQ2IDs"][tmpJob.computingSite]
-                    realDestDQ2ID = tuple(realDestDQ2ID)
+                    real_dest_ddm_id = self.available_lfns_in_t2[tmp_job.getCloud()][tmp_file.dataset]["siteDQ2IDs"][tmp_job.computingSite]
+                    real_dest_ddm_id = tuple(real_dest_ddm_id)
                 # append
-                if realDestDQ2ID not in dsFileMap[mapKey]:
-                    dsFileMap[mapKey][realDestDQ2ID] = {
-                        "taskID": tmpJob.taskID,
-                        "PandaID": tmpJob.PandaID,
+                if real_dest_ddm_id not in dataset_file_map[map_key]:
+                    dataset_file_map[map_key][real_dest_ddm_id] = {
+                        "taskID": tmp_job.taskID,
+                        "PandaID": tmp_job.PandaID,
                         "files": {},
                     }
-                if tmpFile.lfn not in dsFileMap[mapKey][realDestDQ2ID]["files"]:
+                if tmp_file.lfn not in dataset_file_map[map_key][real_dest_ddm_id]["files"]:
                     # add scope
-                    if ddmBackEnd != "rucio":
-                        tmpLFN = tmpFile.lfn
+                    if ddm_back_end != "rucio":
+                        tmp_lfn = tmp_file.lfn
                     else:
-                        tmpLFN = f"{tmpFile.scope}:{tmpFile.lfn}"
-                    dsFileMap[mapKey][realDestDQ2ID]["files"][tmpFile.lfn] = {
-                        "lfn": tmpLFN,
-                        "guid": tmpFile.GUID,
+                        tmp_lfn = f"{tmp_file.scope}:{tmp_file.lfn}"
+                    dataset_file_map[map_key][real_dest_ddm_id]["files"][tmp_file.lfn] = {
+                        "lfn": tmp_lfn,
+                        "guid": tmp_file.GUID,
                         "fileSpecs": [],
                     }
                 # add file spec
-                dsFileMap[mapKey][realDestDQ2ID]["files"][tmpFile.lfn]["fileSpecs"].append(tmpFile)
+                dataset_file_map[map_key][real_dest_ddm_id]["files"][tmp_file.lfn]["fileSpecs"].append(tmp_file)
         # loop over all locations
-        dispList = []
-        for tmpMapKey in dsFileMap:
-            tmpDumVal = dsFileMap[tmpMapKey]
-            for tmpLocationList in tmpDumVal:
-                tmpVal = tmpDumVal[tmpLocationList]
-                for tmpLocation in tmpLocationList:
-                    tmpFileList = tmpVal["files"]
-                    if tmpFileList == {}:
+        disp_list = []
+        for _, tmp_dum_val in dataset_file_map.items():
+            for tmp_location_list in tmp_dum_val:
+                tmp_val = tmp_dum_val[tmp_location_list]
+                for tmp_location in tmp_location_list:
+                    tmp_file_list = tmp_val["files"]
+                    if tmp_file_list == {}:
                         continue
-                    nMaxFiles = 500
-                    iFiles = 0
-                    iLoop = 0
-                    while iFiles < len(tmpFileList):
-                        subFileNames = list(tmpFileList)[iFiles : iFiles + nMaxFiles]
-                        if len(subFileNames) == 0:
+                    n_max_files = 500
+                    i_files = 0
+                    i_loop = 0
+                    while i_files < len(tmp_file_list):
+                        sub_file_names = list(tmp_file_list)[i_files : i_files + n_max_files]
+                        if len(sub_file_names) == 0:
                             break
                         # dis name
-                        disDBlock = f"panda.{tmpVal['taskID']}.{time.strftime('%m.%d')}.GEN.{str(uuid.uuid4())}_dis0{iLoop}{tmpVal['PandaID']}"
-                        iFiles += nMaxFiles
+                        dis_dispatch_block = f"panda.{tmp_val['taskID']}.{time.strftime('%m.%d')}.GEN.{str(uuid.uuid4())}_dis0{i_loop}{tmp_val['PandaID']}"
+                        i_files += n_max_files
                         lfns = []
                         guids = []
                         fsizes = []
                         chksums = []
-                        tmpZipOut = {}
-                        if tmpJob.useZipToPin():
-                            dids = [tmpFileList[tmpSubFileName]["lfn"] for tmpSubFileName in subFileNames]
-                            tmpZipStat, tmpZipOut = rucioAPI.get_zip_files(dids, [tmpLocation])
-                            if not tmpZipStat:
-                                self.logger.debug(f"failed to get zip files : {tmpZipOut}")
-                                tmpZipOut = {}
-                        for tmpSubFileName in subFileNames:
-                            tmpLFN = tmpFileList[tmpSubFileName]["lfn"]
-                            if tmpLFN in tmpZipOut:
-                                tmpZipFileName = f"{tmpZipOut[tmpLFN]['scope']}:{tmpZipOut[tmpLFN]['name']}"
-                                if tmpZipFileName not in lfns:
-                                    lfns.append(tmpZipFileName)
-                                    guids.append(tmpZipOut[tmpLFN]["guid"])
-                                    fsizes.append(tmpZipOut[tmpLFN]["bytes"])
-                                    chksums.append(tmpZipOut[tmpLFN]["adler32"])
+                        tmp_zip_out = {}
+                        if tmp_job.useZipToPin():
+                            dids = [tmp_file_list[tmp_sub_file_name]["lfn"] for tmp_sub_file_name in sub_file_names]
+                            tmp_zip_stat, tmp_zip_out = rucioAPI.get_zip_files(dids, [tmp_location])
+                            if not tmp_zip_stat:
+                                self.logger.debug(f"failed to get zip files : {tmp_zip_out}")
+                                tmp_zip_out = {}
+                        for tmp_sub_file_name in sub_file_names:
+                            tmp_lfn = tmp_file_list[tmp_sub_file_name]["lfn"]
+                            if tmp_lfn in tmp_zip_out:
+                                tmp_zip_file_name = f"{tmp_zip_out[tmp_lfn]['scope']}:{tmp_zip_out[tmp_lfn]['name']}"
+                                if tmp_zip_file_name not in lfns:
+                                    lfns.append(tmp_zip_file_name)
+                                    guids.append(tmp_zip_out[tmp_lfn]["guid"])
+                                    fsizes.append(tmp_zip_out[tmp_lfn]["bytes"])
+                                    chksums.append(tmp_zip_out[tmp_lfn]["adler32"])
                             else:
-                                lfns.append(tmpLFN)
-                                guids.append(tmpFileList[tmpSubFileName]["guid"])
-                                fsizes.append(int(tmpFileList[tmpSubFileName]["fileSpecs"][0].fsize))
-                                chksums.append(tmpFileList[tmpSubFileName]["fileSpecs"][0].checksum)
+                                lfns.append(tmp_lfn)
+                                guids.append(tmp_file_list[tmp_sub_file_name]["guid"])
+                                fsizes.append(int(tmp_file_list[tmp_sub_file_name]["fileSpecs"][0].fsize))
+                                chksums.append(tmp_file_list[tmp_sub_file_name]["fileSpecs"][0].checksum)
                             # set dis name
-                            for tmpFileSpec in tmpFileList[tmpSubFileName]["fileSpecs"]:
-                                if tmpFileSpec.status in ["ready"] and tmpFileSpec.dispatchDBlock == "NULL":
-                                    tmpFileSpec.dispatchDBlock = disDBlock
+                            for tmp_file_spec in tmp_file_list[tmp_sub_file_name]["fileSpecs"]:
+                                if tmp_file_spec.status in ["ready"] and tmp_file_spec.dispatchDBlock == "NULL":
+                                    tmp_file_spec.dispatchDBlock = dis_dispatch_block
                         # register datasets
-                        iLoop += 1
-                        nDDMTry = 3
-                        isOK = False
+                        i_loop += 1
+                        max_attempt = 3
+                        is_ok = False
                         metadata = {"hidden": True, "purge_replicas": 0}
-                        if tmpVal["taskID"] not in [None, "NULL"]:
-                            metadata["task_id"] = str(tmpVal["taskID"])
-                        tmpMsg = "ext registerNewDataset {ds} {lfns} {guids} {fsizes} {chksums} {meta}"
+                        if tmp_val["taskID"] not in [None, "NULL"]:
+                            metadata["task_id"] = str(tmp_val["taskID"])
+                        tmp_msg = "ext registerNewDataset {ds} {lfns} {guids} {fsizes} {chksums} {meta}"
                         self.logger.debug(
-                            tmpMsg.format(
-                                ds=disDBlock,
+                            tmp_msg.format(
+                                ds=dis_dispatch_block,
                                 lfns=str(lfns),
                                 guids=str(guids),
                                 fsizes=str(fsizes),
                                 chksums=str(chksums),
                                 meta=str(metadata),
                             )
                         )
-                        for iDDMTry in range(nDDMTry):
+                        for attempt in range(max_attempt):
                             try:
                                 out = rucioAPI.register_dataset(
-                                    disDBlock,
+                                    dis_dispatch_block,
                                     lfns,
                                     guids,
                                     fsizes,
                                     chksums,
                                     lifetime=7,
                                     scope="panda",
                                     metadata=metadata,
                                 )
                                 self.logger.debug(out)
-                                isOK = True
+                                is_ok = True
                                 break
                             except Exception:
-                                errType, errValue = sys.exc_info()[:2]
-                                self.logger.error(f"ext registerDataset : failed with {errType}:{errValue}" + traceback.format_exc())
-                                if iDDMTry + 1 == nDDMTry:
+                                error_type, error_value = sys.exc_info()[:2]
+                                self.logger.error(f"ext registerDataset : failed with {error_type}:{error_value}" + traceback.format_exc())
+                                if attempt + 1 == max_attempt:
                                     break
-                                self.logger.debug(f"sleep {iDDMTry}/{nDDMTry}")
+                                self.logger.debug(f"sleep {attempt}/{max_attempt}")
                                 time.sleep(10)
                         # failure
-                        if not isOK:
+                        if not is_ok:
                             continue
                         # get VUID
                         try:
                             vuid = out["vuid"]
                             # dataset spec. currentfiles is used to count the number of failed jobs
-                            ds = DatasetSpec()
-                            ds.vuid = vuid
-                            ds.name = disDBlock
-                            ds.type = "dispatch"
-                            ds.status = "defined"
-                            ds.numberfiles = len(lfns)
-                            ds.currentfiles = 0
-                            dispList.append(ds)
+                            dataset = DatasetSpec()
+                            dataset.vuid = vuid
+                            dataset.name = dis_dispatch_block
+                            dataset.type = "dispatch"
+                            dataset.status = "defined"
+                            dataset.numberfiles = len(lfns)
+                            dataset.currentfiles = 0
+                            disp_list.append(dataset)
                         except Exception:
-                            errType, errValue = sys.exc_info()[:2]
-                            self.logger.error(f"ext registerNewDataset : failed to decode VUID for {disDBlock} - {errType} {errValue}")
+                            error_type, error_value = sys.exc_info()[:2]
+                            self.logger.error(f"ext registerNewDataset : failed to decode VUID for {dis_dispatch_block} - {error_type} {error_value}")
                             continue
                         # freezeDataset dispatch dataset
-                        self.logger.debug("freezeDataset " + disDBlock)
-                        for iDDMTry in range(3):
+                        self.logger.debug("freezeDataset " + dis_dispatch_block)
+                        for attempt in range(3):
                             status = False
                             try:
-                                rucioAPI.close_dataset(disDBlock)
+                                rucioAPI.close_dataset(dis_dispatch_block)
                                 status = True
                                 break
                             except Exception:
-                                errtype, errvalue = sys.exc_info()[:2]
-                                out = f"failed to close : {errtype} {errvalue}"
+                                error_type, error_value = sys.exc_info()[:2]
+                                out = f"failed to close : {error_type} {error_value}"
                                 time.sleep(10)
                         if not status:
                             self.logger.error(out)
                             continue
                         # register location
-                        isOK = False
-                        self.logger.debug(f"ext registerDatasetLocation {disDBlock} {tmpLocation} {7}days asynchronous=True")
-                        nDDMTry = 3
-                        for iDDMTry in range(nDDMTry):
+                        is_ok = False
+                        self.logger.debug(f"ext registerDatasetLocation {dis_dispatch_block} {tmp_location} {7}days asynchronous=True")
+                        max_attempt = 3
+                        for attempt in range(max_attempt):
                             try:
                                 out = rucioAPI.register_dataset_location(
-                                    disDBlock,
-                                    [tmpLocation],
+                                    dis_dispatch_block,
+                                    [tmp_location],
                                     7,
                                     activity="Production Input",
                                     scope="panda",
                                     grouping="NONE",
                                 )
                                 self.logger.debug(out)
-                                isOK = True
+                                is_ok = True
                                 break
                             except Exception:
-                                errType, errValue = sys.exc_info()[:2]
-                                self.logger.error(f"ext registerDatasetLocation : failed with {errType}:{errValue}")
-                                if iDDMTry + 1 == nDDMTry:
+                                error_type, error_value = sys.exc_info()[:2]
+                                self.logger.error(f"ext registerDatasetLocation : failed with {error_type}:{error_value}")
+                                if attempt + 1 == max_attempt:
                                     break
-                                self.logger.debug(f"sleep {iDDMTry}/{nDDMTry}")
+                                self.logger.debug(f"sleep {attempt}/{max_attempt}")
                                 time.sleep(10)
 
                         # failure
-                        if not isOK:
+                        if not is_ok:
                             continue
         # insert datasets to DB
-        self.taskBuffer.insertDatasets(dispList)
+        self.task_buffer.insertDatasets(disp_list)
         self.logger.debug("finished to make dis datasets for existing files")
         return
 
     # pin input dataset
-    def _pinInputDatasets(self):
+    def pin_input_datasets(self) -> None:
+        """
+        Pin input datasets method for running the setup process.
+        """
         self.logger.debug("pin input datasets")
         # collect input datasets and locations
-        doneList = []
-        allReplicaMap = {}
-        useShortLivedReplicasFlag = False
-        for tmpJob in self.jobs:
+        done_list = []
+        all_replica_map = {}
+        use_short_lived_replicas_flag = False
+        for tmp_job in self.jobs:
             # ignore HC jobs
-            if tmpJob.processingType.startswith("gangarobot") or tmpJob.processingType.startswith("hammercloud"):
+            if tmp_job.processingType.startswith("gangarobot") or tmp_job.processingType.startswith("hammercloud"):
                 continue
             # not pin if --useShortLivedReplicas was used
-            if tmpJob.metadata is not None and "--useShortLivedReplicas" in tmpJob.metadata:
-                if not useShortLivedReplicasFlag:
+            if tmp_job.metadata is not None and "--useShortLivedReplicas" in tmp_job.metadata:
+                if not use_short_lived_replicas_flag:
                     self.logger.debug("   skip pin due to --useShortLivedReplicas")
-                    useShortLivedReplicasFlag = True
+                    use_short_lived_replicas_flag = True
                 continue
             # use production or test or user jobs only
-            if tmpJob.prodSourceLabel not in ["managed", "test", "user"]:
+            if tmp_job.prodSourceLabel not in ["managed", "test", "user"]:
                 continue
             # ignore inappropriate status
-            if tmpJob.jobStatus in ["failed", "cancelled", "waiting"] or tmpJob.isCancelled():
+            if tmp_job.jobStatus in ["failed", "cancelled", "waiting"] or tmp_job.isCancelled():
                 continue
-            # set lifetime
-            if tmpJob.prodSourceLabel in ["managed", "test"]:
-                pinLifeTime = 7
-            else:
-                pinLifeTime = 7
             # get source
-            if tmpJob.prodSourceLabel in ["managed", "test"]:
-                tmpSrcID = self.siteMapper.getCloud(tmpJob.getCloud())["source"]
-                scope_input, scope_output = select_scope(tmpSrcID, tmpJob.prodSourceLabel, tmpJob.job_label)
-                srcDQ2ID = self.siteMapper.getSite(tmpSrcID).ddm_input[scope_input]
+            if tmp_job.prodSourceLabel in ["managed", "test"]:
+                tmp_src_id = self.site_mapper.getCloud(tmp_job.getCloud())["source"]
+                scope_input, _ = select_scope(tmp_src_id, tmp_job.prodSourceLabel, tmp_job.job_label)
+                src_ddm_id = self.site_mapper.getSite(tmp_src_id).ddm_input[scope_input]
             else:
-                tmpSrcID = self.siteMapper.getSite(tmpJob.computingSite)
-                scope_input, scope_output = select_scope(tmpSrcID, tmpJob.prodSourceLabel, tmpJob.job_label)
-                srcDQ2ID = tmpSrcID.ddm_input[scope_input]
-            # prefix of DQ2 ID
-            srcDQ2IDprefix = re.sub("_[A-Z,0-9]+DISK$", "", srcDQ2ID)
+                tmp_src_id = self.site_mapper.getSite(tmp_job.computingSite)
+                scope_input, _ = select_scope(tmp_src_id, tmp_job.prodSourceLabel, tmp_job.job_label)
+                src_ddm_id = tmp_src_id.ddm_input[scope_input]
+            # prefix of DDM ID
+            src_ddm_id_prefix = re.sub("_[A-Z,0-9]+DISK$", "", src_ddm_id)
             # loop over all files
-            for tmpFile in tmpJob.Files:
+            for tmp_file in tmp_job.Files:
                 # use input files and ignore DBR/lib.tgz
                 if (
-                    tmpFile.type == "input"
-                    and not tmpFile.lfn.endswith(".lib.tgz")
-                    and not tmpFile.dataset.startswith("ddo")
-                    and not tmpFile.dataset.startswith("user")
-                    and not tmpFile.dataset.startswith("group")
+                    tmp_file.type == "input"
+                    and not tmp_file.lfn.endswith(".lib.tgz")
+                    and not tmp_file.dataset.startswith("ddo")
+                    and not tmp_file.dataset.startswith("user")
+                    and not tmp_file.dataset.startswith("group")
                 ):
                     # ignore pre-merged datasets
-                    if tmpFile.dataset.startswith("panda.um."):
+                    if tmp_file.dataset.startswith("panda.um."):
                         continue
                     # get replica locations
-                    if tmpFile.dataset not in allReplicaMap:
-                        if tmpFile.dataset.endswith("/"):
+                    if tmp_file.dataset not in all_replica_map:
+                        if tmp_file.dataset.endswith("/"):
                             (
                                 status,
-                                tmpRepSitesMap,
-                            ) = self.getListDatasetReplicasInContainer(tmpFile.dataset, getMap=True)
+                                tmp_rep_sites_map,
+                            ) = self.get_list_dataset_replicas_in_container(tmp_file.dataset, get_map=True)
+                            status = status == 0
                             if status == 0:
                                 status = True
                             else:
                                 status = False
                         else:
-                            status, tmpRepSites = self.getListDatasetReplicas(tmpFile.dataset)
-                            tmpRepSitesMap = {}
-                            tmpRepSitesMap[tmpFile.dataset] = tmpRepSites
+                            status, tmp_rep_sites = self.get_list_dataset_replicas(tmp_file.dataset)
+                            tmp_rep_sites_map = {}
+                            tmp_rep_sites_map[tmp_file.dataset] = tmp_rep_sites
                         # append
                         if status:
-                            allReplicaMap[tmpFile.dataset] = tmpRepSitesMap
+                            all_replica_map[tmp_file.dataset] = tmp_rep_sites_map
                         else:
                             # set empty to avoid further lookup
-                            allReplicaMap[tmpFile.dataset] = {}
+                            all_replica_map[tmp_file.dataset] = {}
                         # loop over constituent datasets
-                        self.logger.debug(f"pin DQ2 prefix={srcDQ2IDprefix}")
-                        for tmpDsName in allReplicaMap[tmpFile.dataset]:
-                            tmpRepSitesMap = allReplicaMap[tmpFile.dataset][tmpDsName]
+                        self.logger.debug(f"pin DDM prefix={src_ddm_id_prefix}")
+                        for tmp_ds_name in all_replica_map[tmp_file.dataset]:
+                            tmp_rep_sites_map = all_replica_map[tmp_file.dataset][tmp_ds_name]
                             # loop over locations
-                            for tmpRepSite in tmpRepSitesMap:
+                            for tmp_rep_site in tmp_rep_sites_map:
                                 if (
-                                    tmpRepSite.startswith(srcDQ2IDprefix)
-                                    and "TAPE" not in tmpRepSite
-                                    and "_LOCALGROUP" not in tmpRepSite
-                                    and "_DAQ" not in tmpRepSite
-                                    and "_TZERO" not in tmpRepSite
-                                    and "_USERDISK" not in tmpRepSite
-                                    and "_RAW" not in tmpRepSite
-                                    and "SCRATCH" not in tmpRepSite
+                                    tmp_rep_site.startswith(src_ddm_id_prefix)
+                                    and "TAPE" not in tmp_rep_site
+                                    and "_LOCALGROUP" not in tmp_rep_site
+                                    and "_DAQ" not in tmp_rep_site
+                                    and "_TZERO" not in tmp_rep_site
+                                    and "_USERDISK" not in tmp_rep_site
+                                    and "_RAW" not in tmp_rep_site
+                                    and "SCRATCH" not in tmp_rep_site
                                 ):
-                                    tmpKey = (tmpDsName, tmpRepSite)
+                                    tmp_key = (tmp_ds_name, tmp_rep_site)
                                     # already done
-                                    if tmpKey in doneList:
+                                    if tmp_key in done_list:
                                         continue
                                     # append to avoid repetition
-                                    doneList.append(tmpKey)
+                                    done_list.append(tmp_key)
                                     # set pin lifetime
                                     # status = self.setReplicaMetadata(tmpDsName,tmpRepSite,'pin_lifetime','%s days' % pinLifeTime)
-        # retrun
+        # return
         self.logger.debug("pin input datasets done")
         return
 
     # make T1 subscription for missing files
-    def _makeSubscriptionForMissing(self):
+    def make_subscription_for_missing(self) -> None:
+        """
+        Make subscription for missing method for running the setup process.
+        """
         self.logger.debug("make subscriptions for missing files")
         # collect datasets
-        missingList = {}
-        for tmpCloud in self.missingDatasetList:
-            tmpMissDatasets = self.missingDatasetList[tmpCloud]
+        missing_list = {}
+        for tmp_cloud, tmp_miss_datasets in self.missing_dataset_list.items():
             # append cloud
-            if tmpCloud not in missingList:
-                missingList[tmpCloud] = []
+            if tmp_cloud not in missing_list:
+                missing_list[tmp_cloud] = []
             # loop over all datasets
-            for tmpDsName in tmpMissDatasets:
-                tmpMissFiles = tmpMissDatasets[tmpDsName]
+            for tmp_ds_name in tmp_miss_datasets:
+                tmp_miss_files = tmp_miss_datasets[tmp_ds_name]
                 # check if datasets in container are used
-                if tmpDsName.endswith("/"):
+                if tmp_ds_name.endswith("/"):
                     # convert container to datasets
-                    tmpStat, tmpDsList = self.getListDatasetInContainer(tmpDsName)
-                    if not tmpStat:
-                        self.logger.error(f"failed to get datasets in container:{tmpDsName}")
+                    tmp_stat, tmp_ds_list = self.get_list_dataset_in_container(tmp_ds_name)
+                    if not tmp_stat:
+                        self.logger.error(f"failed to get datasets in container:{tmp_ds_name}")
                         continue
                     # check if each dataset is actually used
-                    for tmpConstDsName in tmpDsList:
+                    for tmp_const_ds_name in tmp_ds_list:
                         # skip if already checked
-                        if tmpDsName in missingList[tmpCloud]:
+                        if tmp_ds_name in missing_list[tmp_cloud]:
                             continue
                         # get files in each dataset
-                        tmpStat, tmpFilesInDs = self.getListFilesInDataset(tmpConstDsName)
-                        if not tmpStat:
-                            self.logger.error(f"failed to get files in dataset:{tmpConstDsName}")
+                        tmp_stat, tmp_files_in_ds = self.get_list_files_in_dataset(tmp_const_ds_name)
+                        if not tmp_stat:
+                            self.logger.error(f"failed to get files in dataset:{tmp_const_ds_name}")
                             continue
                         # loop over all files to check the dataset is used
-                        for tmpLFN in tmpMissFiles:
+                        for tmp_lfn in tmp_miss_files:
                             # append if used
-                            if tmpLFN in tmpFilesInDs:
-                                missingList[tmpCloud].append(tmpConstDsName)
+                            if tmp_lfn in tmp_files_in_ds:
+                                missing_list[tmp_cloud].append(tmp_const_ds_name)
                                 break
                 else:
                     # append dataset w/o checking
-                    if tmpDsName not in missingList[tmpCloud]:
-                        missingList[tmpCloud].append(tmpDsName)
+                    if tmp_ds_name not in missing_list[tmp_cloud]:
+                        missing_list[tmp_cloud].append(tmp_ds_name)
         # make subscriptions
-        for tmpCloud in missingList:
-            missDsNameList = missingList[tmpCloud]
+        for tmp_cloud, miss_ds_name_list in missing_list.items():
             # get distination
-            tmpDstID = self.siteMapper.getCloud(tmpCloud)["source"]
-            tmpDstSpec = self.siteMapper.getSite(tmpDstID)
-            scope_input, scope_output = select_scope(tmpDstSpec, self.prodSourceLabel, self.job_label)
-            dstDQ2ID = tmpDstSpec.ddm_input[scope_input]
+            tmp_dst_id = self.site_mapper.getCloud(tmp_cloud)["source"]
+            tmp_dst_spec = self.site_mapper.getSite(tmp_dst_id)
+            scope_input, _ = select_scope(tmp_dst_spec, self.prod_source_label, self.job_label)
+            dst_ddm_id = tmp_dst_spec.ddm_input[scope_input]
             # register subscription
-            for missDsName in missDsNameList:
-                self.logger.debug(f"make subscription at {dstDQ2ID} for missing {missDsName}")
-                self.makeSubscription(missDsName, dstDQ2ID)
+            for miss_ds_name in miss_ds_name_list:
+                self.logger.debug(f"make subscription at {dst_ddm_id} for missing {miss_ds_name}")
+                self.make_subscription(miss_ds_name, dst_ddm_id)
         # retrun
         self.logger.debug("make subscriptions for missing files done")
         return
 
     # make subscription
-    def makeSubscription(self, dataset, dq2ID):
-        # return for failuer
-        retFailed = False
-        self.logger.debug(f"registerDatasetSubscription {dataset} {dq2ID}")
-        nTry = 3
-        for iDDMTry in range(nTry):
+    def make_subscription(self, dataset: str, ddm_id: str) -> bool:
+        """
+        Make subscription method for running the setup process.
+
+        :param dataset: The dataset to make the subscription for.
+        :param ddm_id: The DDM ID.
+        :return: A boolean indicating whether the subscription was made successfully.
+        """
+        # return for failure
+        ret_failed = False
+        self.logger.debug(f"registerDatasetSubscription {dataset} {ddm_id}")
+        for _ in range(3):
             try:
                 # register subscription
-                status = rucioAPI.register_dataset_subscription(dataset, [dq2ID], activity="Production Input")
+                status = rucioAPI.register_dataset_subscription(dataset, [ddm_id], activity="Production Input")
                 out = "OK"
                 break
             except Exception:
                 status = False
-                errType, errValue = sys.exc_info()[:2]
-                out = f"{errType} {errValue}"
+                error_type, error_value = sys.exc_info()[:2]
+                out = f"{error_type} {error_value}"
                 time.sleep(10)
         # result
         if not status:
             self.logger.error(out)
-            return retFailed
+            return ret_failed
         # update
         self.logger.debug(f"{status} {out}")
         # return
         return True
 
     # setup jumbo jobs
-    def _setupJumbojobs(self):
-        if len(self.jumboJobs) == 0:
+    def setup_jumbo_jobs(self) -> None:
+        """
+        Setup jumbo jobs method for running the setup process.
+        """
+        if len(self.jumbo_jobs) == 0:
             return
         self.logger.debug("setup jumbo jobs")
         # get files in datasets
-        dsLFNsMap = {}
-        failedDS = set()
-        for jumboJobSpec in self.jumboJobs:
-            for tmpFileSpec in jumboJobSpec.Files:
+        datasets_lfns_map = {}
+        failed_ds = set()
+        for jumbo_job_spec in self.jumbo_jobs:
+            for tmp_file_spec in jumbo_job_spec.Files:
                 # only input
-                if tmpFileSpec.type not in ["input"]:
+                if tmp_file_spec.type not in ["input"]:
                     continue
                 # get files
-                if tmpFileSpec.dataset not in dsLFNsMap:
-                    if tmpFileSpec.dataset not in failedDS:
-                        tmpStat, tmpMap = self.getListFilesInDataset(tmpFileSpec.dataset, useCache=False)
+                if tmp_file_spec.dataset not in datasets_lfns_map:
+                    if tmp_file_spec.dataset not in failed_ds:
+                        tmp_stat, tmp_map = self.get_list_files_in_dataset(tmp_file_spec.dataset, use_cache=False)
                         # failed
-                        if tmpStat != 0:
-                            failedDS.add(tmpFileSpec.dataset)
-                            self.logger.debug(f"failed to get files in {tmpFileSpec.dataset} with {tmpMap}")
+                        if tmp_stat != 0:
+                            failed_ds.add(tmp_file_spec.dataset)
+                            self.logger.debug(f"failed to get files in {tmp_file_spec.dataset} with {tmp_map}")
                         else:
                             # append
-                            dsLFNsMap[tmpFileSpec.dataset] = tmpMap
+                            datasets_lfns_map[tmp_file_spec.dataset] = tmp_map
                 # set failed if file lookup failed
-                if tmpFileSpec.dataset in failedDS:
-                    jumboJobSpec.jobStatus = "failed"
-                    jumboJobSpec.ddmErrorCode = ErrorCode.EC_GUID
-                    jumboJobSpec.ddmErrorDiag = f"failed to get files in {tmpFileSpec.dataset}"
+                if tmp_file_spec.dataset in failed_ds:
+                    jumbo_job_spec.jobStatus = "failed"
+                    jumbo_job_spec.ddmErrorCode = ErrorCode.EC_GUID
+                    jumbo_job_spec.ddmErrorDiag = f"failed to get files in {tmp_file_spec.dataset}"
                     break
         # make dis datasets
-        okJobs = []
-        ngJobs = []
-        for jumboJobSpec in self.jumboJobs:
+        ok_jobs = []
+        ng_jobs = []
+        for jumbo_job_spec in self.jumbo_jobs:
             # skip failed
-            if jumboJobSpec.jobStatus == "failed":
-                ngJobs.append(jumboJobSpec)
+            if jumbo_job_spec.jobStatus == "failed":
+                ng_jobs.append(jumbo_job_spec)
                 continue
             # get datatype
             try:
-                tmpDataType = jumboJobSpec.prodDBlock.split(".")[-2]
-                if len(tmpDataType) > 20:
-                    raise RuntimeError(f"data type is too log : {len(tmpDataType)} chars")
+                tmp_data_type = jumbo_job_spec.prodDBlock.split(".")[-2]
+                if len(tmp_data_type) > 20:
+                    raise RuntimeError(f"data type is too log : {len(tmp_data_type)} chars")
             except Exception:
                 # default
-                tmpDataType = "GEN"
+                tmp_data_type = "GEN"
             # files for jumbo job
-            lfnsForJumbo = self.taskBuffer.getLFNsForJumbo(jumboJobSpec.jediTaskID)
+            lfns_for_jumbo = self.task_buffer.getLFNsForJumbo(jumbo_job_spec.jediTaskID)
             # make dis dataset name
-            dispatchDBlock = f"panda.{jumboJobSpec.taskID}.{time.strftime('%m.%d.%H%M')}.{tmpDataType}.jumbo_dis{jumboJobSpec.PandaID}"
+            dispatch_data_block = f"panda.{jumbo_job_spec.taskID}.{time.strftime('%m.%d.%H%M')}.{tmp_data_type}.jumbo_dis{jumbo_job_spec.PandaID}"
             # collect file attributes
             lfns = []
             guids = []
             sizes = []
             checksums = []
-            for tmpFileSpec in jumboJobSpec.Files:
+            for tmp_file_spec in jumbo_job_spec.Files:
                 # only input
-                if tmpFileSpec.type not in ["input"]:
+                if tmp_file_spec.type not in ["input"]:
                     continue
-                for tmpLFN in dsLFNsMap[tmpFileSpec.dataset]:
-                    tmpVar = dsLFNsMap[tmpFileSpec.dataset][tmpLFN]
-                    tmpLFN = f"{tmpVar['scope']}:{tmpLFN}"
-                    if tmpLFN not in lfnsForJumbo:
+                for tmp_lfn in datasets_lfns_map[tmp_file_spec.dataset]:
+                    tmp_var = datasets_lfns_map[tmp_file_spec.dataset][tmp_lfn]
+                    tmp_lfn = f"{tmp_var['scope']}:{tmp_lfn}"
+                    if tmp_lfn not in lfns_for_jumbo:
                         continue
-                    lfns.append(tmpLFN)
-                    guids.append(tmpVar["guid"])
-                    sizes.append(tmpVar["fsize"])
-                    checksums.append(tmpVar["chksum"])
+                    lfns.append(tmp_lfn)
+                    guids.append(tmp_var["guid"])
+                    sizes.append(tmp_var["fsize"])
+                    checksums.append(tmp_var["chksum"])
                 # set dis dataset
-                tmpFileSpec.dispatchDBlock = dispatchDBlock
+                tmp_file_spec.dispatchDBlock = dispatch_data_block
             # register and subscribe dis dataset
             if len(lfns) != 0:
                 # set dis dataset
-                jumboJobSpec.dispatchDBlock = dispatchDBlock
+                jumbo_job_spec.dispatchDBlock = dispatch_data_block
                 # register dis dataset
                 try:
-                    self.logger.debug(f"registering jumbo dis dataset {dispatchDBlock} with {len(lfns)} files")
-                    out = rucioAPI.register_dataset(dispatchDBlock, lfns, guids, sizes, checksums, lifetime=14)
+                    self.logger.debug(f"registering jumbo dis dataset {dispatch_data_block} with {len(lfns)} files")
+                    out = rucioAPI.register_dataset(dispatch_data_block, lfns, guids, sizes, checksums, lifetime=14)
                     vuid = out["vuid"]
-                    rucioAPI.close_dataset(dispatchDBlock)
+                    rucioAPI.close_dataset(dispatch_data_block)
                 except Exception:
-                    errType, errValue = sys.exc_info()[:2]
-                    self.logger.debug(f"failed to register jumbo dis dataset {dispatchDBlock} with {errType}:{errValue}")
-                    jumboJobSpec.jobStatus = "failed"
-                    jumboJobSpec.ddmErrorCode = ErrorCode.EC_Setupper
-                    jumboJobSpec.ddmErrorDiag = f"failed to register jumbo dispatch dataset {dispatchDBlock}"
-                    ngJobs.append(jumboJobSpec)
+                    error_type, error_value = sys.exc_info()[:2]
+                    self.logger.debug(f"failed to register jumbo dis dataset {dispatch_data_block} with {error_type}:{error_value}")
+                    jumbo_job_spec.jobStatus = "failed"
+                    jumbo_job_spec.ddmErrorCode = ErrorCode.EC_Setupper
+                    jumbo_job_spec.ddmErrorDiag = f"failed to register jumbo dispatch dataset {dispatch_data_block}"
+                    ng_jobs.append(jumbo_job_spec)
                     continue
                 # subscribe dis dataset
                 try:
-                    tmpSiteSpec = self.siteMapper.getSite(jumboJobSpec.computingSite)
-                    scope_input, scope_output = select_scope(
-                        tmpSiteSpec,
-                        jumboJobSpec.prodSourceLabel,
-                        jumboJobSpec.job_label,
+                    tmp_site_spec = self.site_mapper.getSite(jumbo_job_spec.computingSite)
+                    scope_input, _ = select_scope(
+                        tmp_site_spec,
+                        jumbo_job_spec.prodSourceLabel,
+                        jumbo_job_spec.job_label,
                     )
-                    endPoint = tmpSiteSpec.ddm_input[scope_input]
-                    self.logger.debug(f"subscribing jumbo dis dataset {dispatchDBlock} to {endPoint}")
+                    end_point = tmp_site_spec.ddm_input[scope_input]
+                    self.logger.debug(f"subscribing jumbo dis dataset {dispatch_data_block} to {end_point}")
                     rucioAPI.register_dataset_subscription(
-                        dispatchDBlock,
-                        [endPoint],
+                        dispatch_data_block,
+                        [end_point],
                         lifetime=14,
                         activity="Production Input",
                     )
                 except Exception:
-                    errType, errValue = sys.exc_info()[:2]
-                    self.logger.debug(f"failed to subscribe jumbo dis dataset {dispatchDBlock} to {endPoint} with {errType}:{errValue}")
-                    jumboJobSpec.jobStatus = "failed"
-                    jumboJobSpec.ddmErrorCode = ErrorCode.EC_Setupper
-                    jumboJobSpec.ddmErrorDiag = f"failed to subscribe jumbo dispatch dataset {dispatchDBlock} to {endPoint}"
-                    ngJobs.append(jumboJobSpec)
+                    error_type, error_value = sys.exc_info()[:2]
+                    self.logger.debug(f"failed to subscribe jumbo dis dataset {dispatch_data_block} to {end_point} with {error_type}:{error_value}")
+                    jumbo_job_spec.jobStatus = "failed"
+                    jumbo_job_spec.ddmErrorCode = ErrorCode.EC_Setupper
+                    jumbo_job_spec.ddmErrorDiag = f"failed to subscribe jumbo dispatch dataset {dispatch_data_block} to {end_point}"
+                    ng_jobs.append(jumbo_job_spec)
                     continue
                 # add dataset in DB
-                ds = DatasetSpec()
-                ds.vuid = vuid
-                ds.name = dispatchDBlock
-                ds.type = "dispatch"
-                ds.status = "defined"
-                ds.numberfiles = len(lfns)
-                ds.currentfiles = 0
-                self.taskBuffer.insertDatasets([ds])
+                dataset = DatasetSpec()
+                dataset.vuid = vuid
+                dataset.name = dispatch_data_block
+                dataset.type = "dispatch"
+                dataset.status = "defined"
+                dataset.numberfiles = len(lfns)
+                dataset.currentfiles = 0
+                self.task_buffer.insertDatasets([dataset])
             # set destination
-            jumboJobSpec.destinationSE = jumboJobSpec.computingSite
-            for tmpFileSpec in jumboJobSpec.Files:
-                if tmpFileSpec.type in ["output", "log"] and DataServiceUtils.getDistributedDestination(tmpFileSpec.destinationDBlockToken) is None:
-                    tmpFileSpec.destinationSE = jumboJobSpec.computingSite
-            okJobs.append(jumboJobSpec)
+            jumbo_job_spec.destinationSE = jumbo_job_spec.computingSite
+            for tmp_file_spec in jumbo_job_spec.Files:
+                if tmp_file_spec.type in ["output", "log"] and DataServiceUtils.getDistributedDestination(tmp_file_spec.destinationDBlockToken) is None:
+                    tmp_file_spec.destinationSE = jumbo_job_spec.computingSite
+            ok_jobs.append(jumbo_job_spec)
         # update failed jobs
-        self.updateFailedJobs(ngJobs)
-        self.jumboJobs = okJobs
+        self.update_failed_jobs(ng_jobs)
+        self.jumbo_jobs = ok_jobs
         self.logger.debug("done for jumbo jobs")
         return
 
     # make sub dataset name
-    def makeSubDatasetName(self, original_name, sn, task_id):
+    def make_sub_dataset_name(self, original_name: str, serial_number: int, task_id: int) -> str:
+        """
+        Make sub dataset name method for running the setup process.
+
+        :param original_name: The original name of the dataset.
+        :param serial_number: The serial number.
+        :param task_id: The task ID.
+        :return: The sub dataset name.
+        """
         try:
             task_id = int(task_id)
             if original_name.startswith("user") or original_name.startswith("panda"):
                 part_name = ".".join(original_name.split(".")[:3])
             else:
                 part_name = ".".join(original_name.split(".")[:2]) + ".NA." + ".".join(original_name.split(".")[3:5])
-            return f"{part_name}.{task_id}_sub{sn}"
+            return f"{part_name}.{task_id}_sub{serial_number}"
         except Exception:
-            return f"{original_name}_sub{sn}"
+            return f"{original_name}_sub{serial_number}"
```

### Comparing `panda_server-0.3.4/pandaserver/dataservice/activator.py` & `panda_server-0.3.5/pandaserver/dataservice/activator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/closer.py` & `panda_server-0.3.5/pandaserver/dataservice/closer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/closer_atlas_plugin.py` & `panda_server-0.3.5/pandaserver/dataservice/closer_atlas_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/ddm.py` & `panda_server-0.3.5/pandaserver/dataservice/ddm.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import hashlib
 import re
 import sys
 import traceback
 
 from typing import Dict, List
 
-from pandaserver.srvcore import CoreUtils
 from rucio.client import Client as RucioClient
 from rucio.common.exception import (
     DataIdentifierAlreadyExists,
     DataIdentifierNotFound,
     Duplicate,
     DuplicateContent,
     DuplicateRule,
     FileAlreadyExists,
     UnsupportedOperation,
 )
+from pandaserver.srvcore import CoreUtils
 
 
 # rucio
 class RucioAPI:
     """
     A class to interact with Rucio API
     """
@@ -906,16 +906,16 @@
                         account = client.get_account(user_name)
                         user_info = {"nickname": account["account"], "email": account["email"]}
                 except Exception:
                     pass
                 if user_info is not None:
                     return_value = True
                     break
-        except Exception as e:
-            error_message = f"{str(e)}"
+        except Exception as error:
+            error_message = f"{str(error)}"
             user_info = error_message
         return return_value, user_info
 
 
 # instantiate
 rucioAPI = RucioAPI()
 del RucioAPI
```

### Comparing `panda_server-0.3.4/pandaserver/dataservice/ddm_handler.py` & `panda_server-0.3.5/pandaserver/dataservice/ddm_handler.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/dyn_data_distributer.py` & `panda_server-0.3.5/pandaserver/dataservice/dyn_data_distributer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/event_lookup_client_ei.py` & `panda_server-0.3.5/pandaserver/dataservice/event_lookup_client_ei.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/event_picker.py` & `panda_server-0.3.5/pandaserver/dataservice/event_picker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/dataservice/finisher.py` & `panda_server-0.3.5/pandaserver/dataservice/finisher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda_server-0.3.5/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/jobdispatcher/JobDispatcher.py` & `panda_server-0.3.5/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/jobdispatcher/Protocol.py` & `panda_server-0.3.5/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/jobdispatcher/Watcher.py` & `panda_server-0.3.5/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/proxycache/panda_proxy_cache.py` & `panda_server-0.3.5/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/server/panda.py` & `panda_server-0.3.5/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/srvcore/CoreUtils.py` & `panda_server-0.3.5/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/srvcore/MailUtils.py` & `panda_server-0.3.5/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/srvcore/allowed_methods.py` & `panda_server-0.3.5/pandaserver/srvcore/allowed_methods.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/srvcore/oidc_utils.py` & `panda_server-0.3.5/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/srvcore/panda_request.py` & `panda_server-0.3.5/pandaserver/srvcore/panda_request.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/srvcore/srv_msg_utils.py` & `panda_server-0.3.5/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/CloudSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/ConBridge.py` & `panda_server-0.3.5/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/DBProxyPool.py` & `panda_server-0.3.5/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/DatasetSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/DdmSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/ErrorCode.py` & `panda_server-0.3.5/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/EventServiceUtils.py` & `panda_server-0.3.5/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/FileSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/GlobalShares.py` & `panda_server-0.3.5/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/Initializer.py` & `panda_server-0.3.5/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/JobSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/JobUtils.py` & `panda_server-0.3.5/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/NucleusSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/OraDBProxy.py` & `panda_server-0.3.5/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/PickleFileSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/PickleFileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/PickleJobSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/PickleJobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/PrioUtil.py` & `panda_server-0.3.5/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/ProcessGroups.py` & `panda_server-0.3.5/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/ResourceSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/SQLDumper.py` & `panda_server-0.3.5/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/SQLManager.py` & `panda_server-0.3.5/pandaserver/taskbuffer/SQLManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/SiteSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/TaskBuffer.py` & `panda_server-0.3.5/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # logger
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
 from pandaserver.dataservice.closer import Closer
 from pandaserver.dataservice.ProcessLimiter import ProcessLimiter
-from pandaserver.dataservice.Setupper import Setupper
+from pandaserver.dataservice.setupper import Setupper
 from pandaserver.srvcore import CoreUtils
 from pandaserver.taskbuffer import ErrorCode, EventServiceUtils, JobUtils, ProcessGroups
 from pandaserver.taskbuffer.DBProxyPool import DBProxyPool
 
 _logger = PandaLogger().getLogger("TaskBuffer")
 
 
@@ -168,18 +168,16 @@
 
     # store Jobs into DB
     def storeJobs(
         self,
         jobs,
         user,
         joinThr=False,
-        forkSetupper=False,
         fqans=[],
         hostname="",
-        resetLocInSetupper=False,
         checkSpecialHandling=True,
         toPending=False,
         oldPandaIDs=None,
         relationType=None,
         userVO="atlas",
         esJobsetMap=None,
         getEsJobsetMap=False,
@@ -551,28 +549,24 @@
             self.proxyPool.putProxy(proxy)
             # set up dataset
             if not toPending:
                 if joinThr:
                     thr = Setupper(
                         self,
                         newJobs,
-                        pandaDDM=usePandaDDM,
-                        forkRun=forkSetupper,
-                        resetLocation=resetLocInSetupper,
+                        panda_ddm=usePandaDDM,
                     )
                     thr.start()
                     thr.join()
                 else:
                     # cannot use 'thr =' because it may trigger garbage collector
                     Setupper(
                         self,
                         newJobs,
-                        pandaDDM=usePandaDDM,
-                        forkRun=forkSetupper,
-                        resetLocation=resetLocInSetupper,
+                        panda_ddm=usePandaDDM,
                     ).start()
             # return jobIDs
             tmpLog.debug("end successfully")
             if getEsJobsetMap:
                 return (ret, esJobsetMap, unprocessedMap)
             return ret
         except Exception as e:
@@ -1608,15 +1602,14 @@
 
     # reassign jobs
     def reassignJobs(
         self,
         ids,
         attempt=0,
         joinThr=False,
-        forkSetupper=False,
         forPending=False,
         firstSubmission=True,
     ):
         tmpLog = LogWrapper(_logger, "reassignJobs")
         tmpLog.debug(f"start for {len(ids)} IDs")
         # get DB proxy
         proxy = self.proxyPool.getProxy()
@@ -1684,29 +1677,27 @@
         # setup dataset
         if jobs != []:
             if joinThr:
                 thr = Setupper(
                     self,
                     jobs,
                     resubmit=True,
-                    ddmAttempt=attempt,
-                    forkRun=forkSetupper,
-                    firstSubmission=firstSubmission,
+                    ddm_attempt=attempt,
+                    first_submission=firstSubmission,
                 )
                 thr.start()
                 thr.join()
             else:
                 # cannot use 'thr =' because it may trigger garbage collector
                 Setupper(
                     self,
                     jobs,
                     resubmit=True,
-                    ddmAttempt=attempt,
-                    forkRun=forkSetupper,
-                    firstSubmission=firstSubmission,
+                    ddm_attempt=attempt,
+                    first_submission=firstSubmission,
                 ).start()
         tmpLog.debug("done")
         # return
         return True
 
     # awake jobs in jobsWaiting
     def awakeJobs(self, ids):
```

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda_server-0.3.5/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/Utils.py` & `panda_server-0.3.5/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/WorkerSpec.py` & `panda_server-0.3.5/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/WrappedCursor.py` & `panda_server-0.3.5/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/WrappedPickle.py` & `panda_server-0.3.5/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/retryModule.py` & `panda_server-0.3.5/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/task_split_rules.py` & `panda_server-0.3.5/pandaserver/taskbuffer/task_split_rules.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/taskbuffer/workflow_processor.py` & `panda_server-0.3.5/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/SchemaChecker.py` & `panda_server-0.3.5/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/banUser.py` & `panda_server-0.3.5/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/boostPrio.py` & `panda_server-0.3.5/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/boostUser.py` & `panda_server-0.3.5/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/callbackDDM.py` & `panda_server-0.3.5/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/daod_on_demand.py` & `panda_server-0.3.5/pandaserver/test/daod_on_demand.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/finishJob.py` & `panda_server-0.3.5/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/getJobs.py` & `panda_server-0.3.5/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/killJob.py` & `panda_server-0.3.5/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/killJobLowPrio.py` & `panda_server-0.3.5/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/killJobsInTask.py` & `panda_server-0.3.5/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/killProdJobs.py` & `panda_server-0.3.5/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/killTask.py` & `panda_server-0.3.5/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/killUser.py` & `panda_server-0.3.5/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/reassignSite.py` & `panda_server-0.3.5/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/reassignTask.py` & `panda_server-0.3.5/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/reassignWaiting.py` & `panda_server-0.3.5/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/reloadInputDS.py` & `panda_server-0.3.5/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/sendCommandToJob.py` & `panda_server-0.3.5/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/setDebugMode.py` & `panda_server-0.3.5/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/setPriority.py` & `panda_server-0.3.5/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testEvgen.py` & `panda_server-0.3.5/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testEvgen17.py` & `panda_server-0.3.5/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testG4sim.py` & `panda_server-0.3.5/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testG4sim17.py` & `panda_server-0.3.5/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda_server-0.3.5/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testGlobalShares.py` & `panda_server-0.3.5/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testJobFlowATLAS.py` & `panda_server-0.3.5/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testReco.py` & `panda_server-0.3.5/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testSimulReco14.py` & `panda_server-0.3.5/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testSiteMap.py` & `panda_server-0.3.5/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/testutils.py` & `panda_server-0.3.5/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/lsst/lsstSubmit.py` & `panda_server-0.3.5/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh` & `panda_server-0.3.5/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/userinterface/Client.py` & `panda_server-0.3.5/pandaserver/userinterface/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 try:
     import cPickle as pickle
 except ImportError:
     import pickle
 
 import json
 
+from pandacommon.pandautils.net_utils import replace_hostname_in_url_randomly
+
 from pandaserver.srvcore.CoreUtils import commands_get_status_output
 
 # configuration
 try:
     baseURL = os.environ["PANDA_URL"]
 except Exception:
     baseURL = "http://pandaserver.cern.ch:25080/server/panda"
@@ -151,14 +153,15 @@
                 self.idToken = None
         else:
             self.oidc = False
 
     # GET method
     def get(self, url, data):
         use_https = is_https(url)
+        url = replace_hostname_in_url_randomly(url)
         # make command
         com = f"{self.path} --silent --get"
         if not self.verifyHost:
             com += " --insecure"
         elif "X509_CERT_DIR" in os.environ:
             com += f" --capath {os.environ['X509_CERT_DIR']}"
         elif os.path.exists("/etc/grid-security/certificates"):
@@ -208,14 +211,15 @@
         if self.verbose:
             print(ret)
         return ret
 
     # POST method
     def post(self, url, data, via_file=False):
         use_https = is_https(url)
+        url = replace_hostname_in_url_randomly(url)
         # make command
         com = f"{self.path} --silent"
         if not self.verifyHost:
             com += " --insecure"
         elif "X509_CERT_DIR" in os.environ:
             com += f" --capath {os.environ['X509_CERT_DIR']}"
         elif os.path.exists("/etc/grid-security/certificates"):
@@ -274,14 +278,15 @@
         if self.verbose:
             print(ret)
         return ret
 
     # PUT method
     def put(self, url, data):
         use_https = is_https(url)
+        url = replace_hostname_in_url_randomly(url)
         # make command
         com = f"{self.path} --silent"
         if not self.verifyHost:
             com += " --insecure"
         elif "X509_CERT_DIR" in os.environ:
             com += f" --capath {os.environ['X509_CERT_DIR']}"
         elif os.path.exists("/etc/grid-security/certificates"):
```

### Comparing `panda_server-0.3.4/pandaserver/userinterface/UserIF.py` & `panda_server-0.3.5/pandaserver/userinterface/UserIF.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
             except AttributeError:
                 _logger.error("submitJobs : checking username for userVO[%s]: username not found, defaulting to %s. %s %s" % (userVO, user))
 
         # store jobs
         ret = self.taskBuffer.storeJobs(
             jobs,
             user,
-            forkSetupper=False,
             fqans=userFQANs,
             hostname=host,
             toPending=toPending,
             userVO=userVO,
         )
         _logger.debug(f"submitJobs {user} ->:{len(ret)}")
 
@@ -493,15 +492,14 @@
     # reassign jobs
     def reassignJobs(self, idsStr, user, host, forPending, firstSubmission):
         # deserialize IDs
         ids = WrappedPickle.loads(idsStr)
         # reassign jobs
         ret = self.taskBuffer.reassignJobs(
             ids,
-            forkSetupper=False,
             forPending=forPending,
             firstSubmission=firstSubmission,
         )
         # serialize
         return WrappedPickle.dumps(ret)
 
     # resubmit jobs
```

### Comparing `panda_server-0.3.4/pandaserver/workflow/pcwl_test.py` & `panda_server-0.3.5/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/pcwl_utils.py` & `panda_server-0.3.5/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/psnakemake_container.json` & `panda_server-0.3.5/pandaserver/workflow/psnakemake_container.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/psnakemake_task.json` & `panda_server-0.3.5/pandaserver/workflow/psnakemake_task.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/psnakemake_test.py` & `panda_server-0.3.5/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/workflow_utils.py` & `panda_server-0.3.5/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/snakeparser/extensions.py` & `panda_server-0.3.5/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/snakeparser/log.py` & `panda_server-0.3.5/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/snakeparser/parser.py` & `panda_server-0.3.5/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pandaserver/workflow/snakeparser/utils.py` & `panda_server-0.3.5/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/conda_meta.yaml.template` & `panda_server-0.3.5/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda_server-0.3.5/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/panda_server-httpd.conf.rpmnew.template` & `panda_server-0.3.5/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/panda_server.cfg.rpmnew.template` & `panda_server-0.3.5/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/bin/panda_server-makeSlsXml.exe.template` & `panda_server-0.3.5/templates/bin/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/bin/panda_server-vomsrenew.exe.template` & `panda_server-0.3.5/templates/bin/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/init.d/panda_daemon.exe.template` & `panda_server-0.3.5/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/init.d/panda_httpd.exe.template` & `panda_server-0.3.5/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/init.d/panda_server.exe.template` & `panda_server-0.3.5/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/logrotate.d/panda_server.logrotate.template` & `panda_server-0.3.5/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda_server-0.3.5/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda_server-0.3.5/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/LICENSE.txt` & `panda_server-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.4/pyproject.toml` & `panda_server-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "PanDA Server Package"
 readme = "README.md"
 license = {text = "Apache-2.0"}
 authors = [
     { name = "PanDA Team", email = "panda-support@cern.ch" },
 ]
 dependencies = [
-    'panda-common>=0.0.34',
+    'panda-common>=0.1.1',
     'panda-client-light>=1.5.55',
     'pyOpenSSL',
     'python-daemon',
     'mod_wsgi',
     'stomp.py',
     'pyyaml',
     'pyjwt',
```

### Comparing `panda_server-0.3.4/PKG-INFO` & `panda_server-0.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panda-server
-Version: 0.3.4
+Version: 0.3.5
 Summary: PanDA Server Package
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <panda-support@cern.ch>
 License: Apache-2.0
 License-File: LICENSE.txt
 Requires-Python: >=3.8
 Requires-Dist: cwl-utils>=0.13
@@ -13,15 +13,15 @@
 Requires-Dist: idds-common
 Requires-Dist: idds-doma
 Requires-Dist: idds-workflow>=1.1.0
 Requires-Dist: mod-wsgi
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: panda-client-light>=1.5.55
-Requires-Dist: panda-common>=0.0.34
+Requires-Dist: panda-common>=0.1.1
 Requires-Dist: psutil>=5.4.8
 Requires-Dist: pyjwt
 Requires-Dist: pyopenssl
 Requires-Dist: python-daemon
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: ruamel-yaml
```

