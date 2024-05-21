# Comparing `tmp/panda_server-0.3.5.tar.gz` & `tmp/panda_server-0.3.6.tar.gz`

## Comparing `panda_server-0.3.5.tar` & `panda_server-0.3.6.tar`

### file list

```diff
@@ -1,206 +1,207 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.5/ChangeLog.txt
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.5/Dockerfile
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.5/INSTALL.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.5/INSTALL_ATLAS.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.5/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.5/PandaPkgInfo.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.5/panda-server.spec
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.5/package/hatch_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/brokerage/broker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/config_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/daemon_config.py
--rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/config/panda_config.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/Carbon.py
--rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/Configurator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/__init__.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/configurator/aux.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/master.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/master_systemd.py
--rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/cache_pilots.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/cache_schedconfig.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0        0        0    63820 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/AdderSimplePlugin.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/DataServiceUtils.py
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/__init__.py
--rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/activator.py
--rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/closer.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/closer_atlas_plugin.py
--rwxr-xr-x   0        0        0    39936 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ddm.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/ddm_handler.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/dyn_data_distributer.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/event_lookup_client_ei.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/event_picker.py
--rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/finisher.py
--rwxr-xr-x   0        0        0     7957 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper.py
--rwxr-xr-x   0        0        0   117529 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper_atlas_plugin.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper_dummy_plugin.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/dataservice/setupper_plugin_base.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/jobdispatcher/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/proxycache/__init__.py
--rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/proxycache/panda_proxy_cache.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/server/.gacl
--rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/server/panda.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/__init__.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/allowed_methods.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/panda_request.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/srvcore/srv_msg_utils.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0        0        0  1268991 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PickleFileSpec.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PickleJobSpec.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SQLManager.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0        0        0   143228 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/task_split_rules.py
--rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/taskbuffer/workflow_processor.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/SchemaChecker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/banUser.py
--rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/boostPrio.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/boostUser.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/callbackDDM.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/daod_on_demand.py
--rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/finishJob.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/finishTaskJEDI.py
--rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/getJobs.py
--rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killJob.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killTask.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/killUser.py
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignJobs.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignSite.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignTask.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reassignWaiting.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/reloadInputDS.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/setPriority.py
--rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testEvgen.py
--rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testG4sim.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testG4sim17.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testGlobalShares.py
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testReco.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testSiteMap.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/testutils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/README.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/mysetup
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/README.txt
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
--rwxr-xr-x   0        0        0    80539 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/userinterface/Client.py
--rw-r--r--   0        0        0    91540 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/userinterface/UserIF.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/userinterface/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/psnakemake_container.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/psnakemake_task.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/psnakemake_test.py
--rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.5/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/conda_meta.yaml.template
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/panda_server-httpd.conf.rpmnew.template
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/panda_server.cfg.rpmnew.template
--rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/bin/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/bin/panda_server-vomsrenew.exe.template
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/init.d/panda_server.exe.template
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/sysconfig/panda_server_env.systemd.rpmnew.template
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/systemd/panda.service.template
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/systemd/panda_daemon.service.template
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.5/templates/systemd/panda_httpd.service.template
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.5/README.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 panda_server-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 panda_server-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.6/ChangeLog.txt
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.6/Dockerfile
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.6/INSTALL.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.6/INSTALL_ATLAS.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.6/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.6/PandaPkgInfo.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.6/panda-server.spec
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.6/package/hatch_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/brokerage/broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/config/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/config/config_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/config/panda_config.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/configurator/Carbon.py
+-rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/configurator/Configurator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/configurator/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/configurator/aux.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/master.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/master_systemd.py
+-rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/cache_pilots.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/cache_schedconfig.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0        0        0    63820 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/AdderSimplePlugin.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/DataServiceUtils.py
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/__init__.py
+-rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/activator.py
+-rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/closer.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/closer_atlas_plugin.py
+-rwxr-xr-x   0        0        0    39936 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/ddm.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/ddm_handler.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/dyn_data_distributer.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/event_lookup_client_ei.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/event_picker.py
+-rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/finisher.py
+-rwxr-xr-x   0        0        0     7957 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/setupper.py
+-rwxr-xr-x   0        0        0   117529 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/setupper_atlas_plugin.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/setupper_dummy_plugin.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/dataservice/setupper_plugin_base.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/jobdispatcher/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/proxycache/__init__.py
+-rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/proxycache/panda_proxy_cache.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/server/.gacl
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/server/panda.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/allowed_methods.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/panda_request.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/srvcore/srv_msg_utils.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0        0        0  1268846 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/PickleFileSpec.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/PickleJobSpec.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/SQLManager.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0        0        0   143228 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0        0        0    27435 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/task_split_rules.py
+-rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/taskbuffer/workflow_processor.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/banUser.py
+-rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/boostUser.py
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/callbackDDM.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/daod_on_demand.py
+-rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/finishJob.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/finishTaskJEDI.py
+-rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/getJobs.py
+-rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killJob.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killTask.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/killUser.py
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/reassignJobs.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/reassignSite.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/setPriority.py
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testG4sim.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testG4sim17.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testReco.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testSiteMap.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/testutils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/alice/README.txt
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/alice/mysetup
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/lsst/README.txt
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
+-rwxr-xr-x   0        0        0    80539 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/userinterface/Client.py
+-rw-r--r--   0        0        0    91540 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/userinterface/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/psnakemake_container.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/psnakemake_task.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/psnakemake_test.py
+-rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.6/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/conda_meta.yaml.template
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/panda_server-httpd.conf.rpmnew.template
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/panda_server.cfg.rpmnew.template
+-rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/bin/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/bin/panda_server-vomsrenew.exe.template
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/init.d/panda_server.exe.template
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/sysconfig/panda_server.sysconfig_for_systemd.template
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/systemd/panda.service.template
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 panda_server-0.3.6/templates/systemd/panda_httpd.service.template
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.6/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 panda_server-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 panda_server-0.3.6/PKG-INFO
```

### Comparing `panda_server-0.3.5/ChangeLog.txt` & `panda_server-0.3.6/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/Dockerfile` & `panda_server-0.3.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/INSTALL.md` & `panda_server-0.3.6/INSTALL.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/INSTALL_ATLAS.md` & `panda_server-0.3.6/INSTALL_ATLAS.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/panda-server.spec` & `panda_server-0.3.6/panda-server.spec`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/package/hatch_build.py` & `panda_server-0.3.6/package/hatch_build.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/brokerage/SiteMapper.py` & `panda_server-0.3.6/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/brokerage/broker.py` & `panda_server-0.3.6/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/config/daemon_config.py` & `panda_server-0.3.6/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/config/panda_config.py` & `panda_server-0.3.6/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/configurator/Carbon.py` & `panda_server-0.3.6/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/configurator/Configurator.py` & `panda_server-0.3.6/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/configurator/aux.py` & `panda_server-0.3.6/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/master.py` & `panda_server-0.3.6/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/master_systemd.py` & `panda_server-0.3.6/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/utils.py` & `panda_server-0.3.6/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/add_main.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/add_sub.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/cache_pilots.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/cache_pilots.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/cache_schedconfig.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/cache_schedconfig.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/carbon.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/configurator.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/copyArchive.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/datasetManager.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/evpPD2P.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/metric_collector.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/pilotStreaming.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/task_evaluator.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/tmpwatch.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/daemons/scripts/worker_synchronization.py` & `panda_server-0.3.6/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda_server-0.3.6/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/AdderGen.py` & `panda_server-0.3.6/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/AdderResult.py` & `panda_server-0.3.6/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/AdderSimplePlugin.py` & `panda_server-0.3.6/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/DataServiceUtils.py` & `panda_server-0.3.6/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/ProcessLimiter.py` & `panda_server-0.3.6/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda_server-0.3.6/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/activator.py` & `panda_server-0.3.6/pandaserver/dataservice/activator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/closer.py` & `panda_server-0.3.6/pandaserver/dataservice/closer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/closer_atlas_plugin.py` & `panda_server-0.3.6/pandaserver/dataservice/closer_atlas_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/ddm.py` & `panda_server-0.3.6/pandaserver/dataservice/ddm.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/ddm_handler.py` & `panda_server-0.3.6/pandaserver/dataservice/ddm_handler.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/dyn_data_distributer.py` & `panda_server-0.3.6/pandaserver/dataservice/dyn_data_distributer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/event_lookup_client_ei.py` & `panda_server-0.3.6/pandaserver/dataservice/event_lookup_client_ei.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/event_picker.py` & `panda_server-0.3.6/pandaserver/dataservice/event_picker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/finisher.py` & `panda_server-0.3.6/pandaserver/dataservice/finisher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/setupper.py` & `panda_server-0.3.6/pandaserver/dataservice/setupper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/setupper_atlas_plugin.py` & `panda_server-0.3.6/pandaserver/dataservice/setupper_atlas_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/setupper_dummy_plugin.py` & `panda_server-0.3.6/pandaserver/dataservice/setupper_dummy_plugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/dataservice/setupper_plugin_base.py` & `panda_server-0.3.6/pandaserver/dataservice/setupper_plugin_base.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda_server-0.3.6/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/jobdispatcher/JobDispatcher.py` & `panda_server-0.3.6/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/jobdispatcher/Protocol.py` & `panda_server-0.3.6/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/jobdispatcher/Watcher.py` & `panda_server-0.3.6/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/proxycache/panda_proxy_cache.py` & `panda_server-0.3.6/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/server/panda.py` & `panda_server-0.3.6/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/srvcore/CoreUtils.py` & `panda_server-0.3.6/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/srvcore/MailUtils.py` & `panda_server-0.3.6/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/srvcore/allowed_methods.py` & `panda_server-0.3.6/pandaserver/srvcore/allowed_methods.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/srvcore/oidc_utils.py` & `panda_server-0.3.6/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/srvcore/panda_request.py` & `panda_server-0.3.6/pandaserver/srvcore/panda_request.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/srvcore/srv_msg_utils.py` & `panda_server-0.3.6/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/CloudSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/ConBridge.py` & `panda_server-0.3.6/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/DBProxyPool.py` & `panda_server-0.3.6/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/DatasetSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/DdmSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/ErrorCode.py` & `panda_server-0.3.6/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/EventServiceUtils.py` & `panda_server-0.3.6/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/FileSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/GlobalShares.py` & `panda_server-0.3.6/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/Initializer.py` & `panda_server-0.3.6/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/JobSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/JobUtils.py` & `panda_server-0.3.6/pandaserver/taskbuffer/JobUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -194,7 +194,21 @@
     state_objects = json.loads(state, object_hook=as_python_object)
     jobs = []
     for job_state in state_objects:
         job_spec = JobSpec()
         job_spec.load_from_json_serializable(job_state)
         jobs.append(job_spec)
     return jobs
+
+
+# get resource type for a job
+def get_resource_type_job(resource_map: list, job_spec: JobSpec) -> str:
+    """
+    Get the resource type for a job based on the job's resource type and the list of resource types.
+    :param resource_map: The list of resource types.
+    :param job_spec: The job.
+    :return: The resource type.
+    """
+    for resource_spec in resource_map:
+        if resource_spec.match_job(job_spec):
+            return resource_spec.resource_name
+    return "Undefined"
```

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/NucleusSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/OraDBProxy.py` & `panda_server-0.3.6/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -22825,22 +22825,17 @@
                 job_spec.PandaID,
                 job_spec.minRamCount,
                 type(job_spec.minRamCount),
                 job_spec.coreCount,
                 type(job_spec.coreCount),
             )
         )
-
-        for resource_spec in resource_map:
-            if resource_spec.match_job(job_spec):
-                tmp_log.debug(f"done. resource_type is {resource_spec.resource_name}")
-                return resource_spec.resource_name
-
-        tmp_log.debug("done. resource_type is Undefined")
-        return "Undefined"
+        resource_type = JobUtils.get_resource_type_job(resource_map, job_spec)
+        tmp_log.debug(f"done. resource_type is {resource_type}")
+        return resource_type
 
     # update stat of workers
     def reportWorkerStats(self, harvesterID, siteName, paramsList):
         comment = " /* DBProxy.reportWorkerStats */"
         methodName = comment.split(" ")[-2].split(".")[-1]
         tmpLog = LogWrapper(
             _logger,
```

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/PickleFileSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/PickleFileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/PickleJobSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/PickleJobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/PrioUtil.py` & `panda_server-0.3.6/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/ProcessGroups.py` & `panda_server-0.3.6/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/ResourceSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/SQLDumper.py` & `panda_server-0.3.6/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/SQLManager.py` & `panda_server-0.3.6/pandaserver/taskbuffer/SQLManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/SiteSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/TaskBuffer.py` & `panda_server-0.3.6/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda_server-0.3.6/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/Utils.py` & `panda_server-0.3.6/pandaserver/taskbuffer/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import datetime
+import gc
 import gzip
 import json
 import os
 import re
 import struct
 import sys
 import traceback
 import uuid
 import zlib
 from typing import Generator
 
 from pandacommon.pandalogger.LogWrapper import LogWrapper
 from pandacommon.pandalogger.PandaLogger import PandaLogger
+from werkzeug.datastructures import FileStorage
+
 from pandaserver.config import panda_config
 from pandaserver.jobdispatcher import Protocol
 from pandaserver.srvcore import CoreUtils
 from pandaserver.srvcore.panda_request import PandaRequest
 from pandaserver.userinterface import Client
-from werkzeug.datastructures import FileStorage
 
 _logger = PandaLogger().getLogger("Utils")
 
 IGNORED_SUFFIX = [".out"]
 
 # File size limits
 MB = 1024 * 1024
@@ -86,24 +88,33 @@
         file (FileStorage): werkzeug.FileStorage object to be uploaded.
 
     Returns:
         string: "True" if the upload was successful, otherwise an error message.
     """
 
     tmp_log = LogWrapper(_logger, f"putFile-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}")
+    tmp_log.debug(f"start")
 
     # check if using secure connection and the proxy is not limited
     if not Protocol.isSecure(panda_request):
+        tmp_log.error("no HTTPS")
+        tmp_log.debug("trigger garbage collection")
+        gc.collect()
+        tmp_log.debug("end")
         return ERROR_NOT_SECURE
     if "/CN=limited proxy" in panda_request.subprocess_env["SSL_CLIENT_S_DN"]:
+        tmp_log.error("limited proxy is used")
+        tmp_log.debug("trigger garbage collection")
+        gc.collect()
+        tmp_log.debug("end")
         return ERROR_LIMITED_PROXY
 
     # user name
     user_name = CoreUtils.clean_user_id(panda_request.subprocess_env["SSL_CLIENT_S_DN"])
-    tmp_log.debug(f"start {user_name} {file.filename}")
+    tmp_log.debug(f"user_name={user_name} file_path={file.filename}")
 
     # get file size limit
     if not file.filename.startswith("sources."):
         no_build = True
         size_limit = SANDBOX_NO_BUILD_LIMIT
     else:
         no_build = False
@@ -116,14 +127,16 @@
     if content_length > size_limit:
         error_message = f"{ERROR_SIZE_LIMIT} {content_length}>{size_limit}."
         if no_build:
             error_message += " Please submit the job without --noBuild/--libDS since those options impose a tighter size limit"
         else:
             error_message += " Please remove redundant files from your work area"
         tmp_log.error(error_message)
+        tmp_log.debug("trigger garbage collection")
+        gc.collect()
         tmp_log.debug("end")
         return error_message
 
     # write to file
     try:
         file_name = file.filename.split("/")[-1]
         full_path = f"{panda_config.cache_dir}/{file_name}"
@@ -146,14 +159,16 @@
             ]:
                 file_content = gzip.compress(file_content)
             file_object.write(file_content)
 
     except Exception:
         error_message = ERROR_WRITE
         tmp_log.error(error_message)
+        tmp_log.debug("trigger garbage collection")
+        gc.collect()
         tmp_log.debug("end")
         return error_message
 
     # calculate the checksum
     try:
         # decode Footer
         footer = file_content[-8:]
@@ -186,15 +201,18 @@
                 error_message = f"ERROR : failed to register sandbox to DB with {status_client} {output_client}"
                 tmp_log.error(error_message)
                 tmp_log.debug("end")
                 return error_message
 
             tmp_log.debug(f"inserted sandbox to DB with {output_client}")
 
+    tmp_log.debug("trigrer garbage collection")
+    gc.collect()
     tmp_log.debug("end")
+
     return "True"
 
 
 def putEventPickingRequest(
     panda_request: PandaRequest,
     runEventList="",
     eventPickDataType="",
```

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/WorkerSpec.py` & `panda_server-0.3.6/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/WrappedCursor.py` & `panda_server-0.3.6/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/WrappedPickle.py` & `panda_server-0.3.6/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/retryModule.py` & `panda_server-0.3.6/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/task_split_rules.py` & `panda_server-0.3.6/pandaserver/taskbuffer/task_split_rules.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/taskbuffer/workflow_processor.py` & `panda_server-0.3.6/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/SchemaChecker.py` & `panda_server-0.3.6/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/banUser.py` & `panda_server-0.3.6/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/boostPrio.py` & `panda_server-0.3.6/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/boostUser.py` & `panda_server-0.3.6/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/callbackDDM.py` & `panda_server-0.3.6/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/daod_on_demand.py` & `panda_server-0.3.6/pandaserver/test/daod_on_demand.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/finishJob.py` & `panda_server-0.3.6/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/getJobs.py` & `panda_server-0.3.6/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/killJob.py` & `panda_server-0.3.6/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/killJobLowPrio.py` & `panda_server-0.3.6/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/killJobsInTask.py` & `panda_server-0.3.6/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/killProdJobs.py` & `panda_server-0.3.6/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/killTask.py` & `panda_server-0.3.6/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/killUser.py` & `panda_server-0.3.6/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/reassignSite.py` & `panda_server-0.3.6/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/reassignTask.py` & `panda_server-0.3.6/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/reassignWaiting.py` & `panda_server-0.3.6/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/reloadInputDS.py` & `panda_server-0.3.6/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/sendCommandToJob.py` & `panda_server-0.3.6/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/setDebugMode.py` & `panda_server-0.3.6/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/setPriority.py` & `panda_server-0.3.6/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testEvgen.py` & `panda_server-0.3.6/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testEvgen17.py` & `panda_server-0.3.6/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testG4sim.py` & `panda_server-0.3.6/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testG4sim17.py` & `panda_server-0.3.6/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda_server-0.3.6/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testGlobalShares.py` & `panda_server-0.3.6/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testJobFlowATLAS.py` & `panda_server-0.3.6/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testReco.py` & `panda_server-0.3.6/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testSimulReco14.py` & `panda_server-0.3.6/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testSiteMap.py` & `panda_server-0.3.6/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/testutils.py` & `panda_server-0.3.6/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda_server-0.3.6/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda_server-0.3.6/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/lsst/lsstSubmit.py` & `panda_server-0.3.6/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda_server-0.3.6/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda_server-0.3.6/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh` & `panda_server-0.3.6/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/userinterface/Client.py` & `panda_server-0.3.6/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/userinterface/UserIF.py` & `panda_server-0.3.6/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/pcwl_test.py` & `panda_server-0.3.6/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/pcwl_utils.py` & `panda_server-0.3.6/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/psnakemake_container.json` & `panda_server-0.3.6/pandaserver/workflow/psnakemake_container.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/psnakemake_task.json` & `panda_server-0.3.6/pandaserver/workflow/psnakemake_task.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/psnakemake_test.py` & `panda_server-0.3.6/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/workflow_utils.py` & `panda_server-0.3.6/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/snakeparser/extensions.py` & `panda_server-0.3.6/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/snakeparser/log.py` & `panda_server-0.3.6/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/snakeparser/parser.py` & `panda_server-0.3.6/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pandaserver/workflow/snakeparser/utils.py` & `panda_server-0.3.6/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/conda_meta.yaml.template` & `panda_server-0.3.6/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda_server-0.3.6/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/panda_server-httpd.conf.rpmnew.template` & `panda_server-0.3.6/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/panda_server.cfg.rpmnew.template` & `panda_server-0.3.6/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/bin/panda_server-makeSlsXml.exe.template` & `panda_server-0.3.6/templates/bin/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/bin/panda_server-vomsrenew.exe.template` & `panda_server-0.3.6/templates/bin/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/init.d/panda_daemon.exe.template` & `panda_server-0.3.6/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/init.d/panda_httpd.exe.template` & `panda_server-0.3.6/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/init.d/panda_server.exe.template` & `panda_server-0.3.6/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/logrotate.d/panda_server.logrotate.template` & `panda_server-0.3.6/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda_server-0.3.6/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# Configuration file for the httpd service.
+# Configuration file for the httpd service launched not through systemd,
+# e.g. in container where some parameters are dynamically set via env
+# variables while systemd services don't inherit env variables from PID1
+
 
 @@virtual_env_setup@@
 
 OPTIONS="-f ${VIRTUAL_ENV}/etc/panda/panda_server-httpd.conf"
 
 # for WSGI
 #OPTIONS="-f ${VIRTUAL_ENV}/etc/panda/panda_server-httpd-FastCGI.conf"
```

### Comparing `panda_server-0.3.5/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda_server-0.3.6/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # python venv
-@@virtual_env_setup@@
+VIRTUAL_ENV=@@virtual_env@@
 
-OPTIONS="-f ${VIRTUAL_ENV}/etc/panda/panda_server-httpd.conf"
+OPTIONS="-f @@virtual_env@@/etc/panda/panda_server-httpd.conf"
 
 # reset PATH/LD_LIBRARY_PATH since atlpan's ones break grid-tools
-PATH=${VIRTUAL_ENV}/bin:/bin:/usr/local/bin:/usr/bin
+PATH=@@virtual_env@@/bin:/bin:/usr/local/bin:/usr/bin
 LD_LIBRARY_PATH=
 
 # for DQ2
 X509_CERT_DIR=/etc/grid-security/certificates
 RUCIO_ACCOUNT=panda
 RUCIO_APPID=pandasrv
```

### Comparing `panda_server-0.3.5/LICENSE.txt` & `panda_server-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/pyproject.toml` & `panda_server-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.5/PKG-INFO` & `panda_server-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panda-server
-Version: 0.3.5
+Version: 0.3.6
 Summary: PanDA Server Package
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <panda-support@cern.ch>
 License: Apache-2.0
 License-File: LICENSE.txt
 Requires-Python: >=3.8
 Requires-Dist: cwl-utils>=0.13
```

