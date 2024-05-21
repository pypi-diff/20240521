# Comparing `tmp/nucliadb-4.0.0.post527-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.0.post528-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,464 +1,464 @@
-Zip file size: 765457 bytes, number of entries: 462
--rw-r--r--  2.0 unx     1135 b- defN 24-May-21 08:22 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-21 08:22 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-21 08:22 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-21 08:22 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-21 08:22 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-21 08:22 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-21 08:22 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-21 08:22 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-21 08:22 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-21 08:22 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-21 08:22 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-21 08:22 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-21 08:22 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-21 08:22 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-21 08:22 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-21 08:22 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-21 08:22 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-21 08:22 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-21 08:22 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-21 08:22 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-21 08:22 nucliadb/health.py
--rw-r--r--  2.0 unx    11639 b- defN 24-May-21 08:22 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-21 08:22 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-21 08:22 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 08:22 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-21 08:22 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 24-May-21 08:22 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-21 08:22 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-21 08:22 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-21 08:22 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22091 b- defN 24-May-21 08:22 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-21 08:22 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-21 08:22 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-21 08:22 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-21 08:22 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12515 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-21 08:22 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-21 08:22 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-21 08:22 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-21 08:22 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-21 08:22 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-21 08:22 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-21 08:22 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-21 08:22 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-21 08:22 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-21 08:22 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-21 08:22 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-21 08:22 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-21 08:22 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-21 08:22 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-21 08:22 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-21 08:22 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-21 08:22 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-21 08:22 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-21 08:22 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-21 08:22 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-21 08:22 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-21 08:22 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-21 08:22 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-21 08:22 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-21 08:22 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-21 08:22 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-21 08:22 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-21 08:22 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-21 08:22 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-21 08:22 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-21 08:22 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-21 08:22 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19969 b- defN 24-May-21 08:22 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-21 08:22 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-21 08:22 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-21 08:22 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-21 08:22 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-21 08:22 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-21 08:22 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-21 08:22 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-21 08:22 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-21 08:22 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-21 08:22 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-21 08:22 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-21 08:22 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-21 08:22 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-21 08:22 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28448 b- defN 24-May-21 08:22 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-21 08:22 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-21 08:22 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-21 08:22 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-21 08:22 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-21 08:22 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-21 08:22 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-21 08:22 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27042 b- defN 24-May-21 08:22 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-21 08:22 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-21 08:22 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-21 08:22 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33193 b- defN 24-May-21 08:22 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-21 08:22 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-21 08:22 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-21 08:22 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-21 08:22 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-21 08:22 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-21 08:22 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-21 08:22 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-21 08:22 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-21 08:22 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-21 08:22 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-21 08:22 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-21 08:22 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-21 08:22 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-21 08:22 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-21 08:22 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-21 08:22 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-21 08:22 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-21 08:22 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-21 08:22 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-21 08:22 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-21 08:22 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-21 08:22 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-21 08:22 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-21 08:22 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-21 08:22 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12399 b- defN 24-May-21 08:22 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7988 b- defN 24-May-21 08:22 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-21 08:22 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-21 08:22 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-21 08:22 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-21 08:22 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-21 08:22 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-21 08:22 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-21 08:22 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-21 08:22 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-21 08:22 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-21 08:22 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-21 08:22 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-21 08:22 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-21 08:22 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-21 08:22 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-21 08:22 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-21 08:22 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-21 08:22 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-21 08:22 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-21 08:22 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-21 08:22 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-21 08:22 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-21 08:22 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-21 08:22 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-21 08:22 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-21 08:22 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-21 08:22 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-21 08:22 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-21 08:22 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-21 08:22 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-21 08:22 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-21 08:22 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-21 08:22 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-21 08:22 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-21 08:22 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-21 08:22 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-21 08:22 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-21 08:22 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-21 08:22 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-21 08:22 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-21 08:22 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-21 08:22 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-21 08:22 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-21 08:22 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-21 08:22 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-21 08:22 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-21 08:22 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-21 08:22 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-21 08:22 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-21 08:22 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-21 08:22 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-21 08:22 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-21 08:22 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-21 08:22 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-21 08:22 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-21 08:22 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-21 08:22 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-21 08:22 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-21 08:22 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-21 08:22 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-21 08:22 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5636 b- defN 24-May-21 08:22 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-21 08:22 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-21 08:22 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-21 08:22 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-21 08:22 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-21 08:22 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-21 08:22 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-21 08:22 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-21 08:22 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-21 08:22 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-21 08:22 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-21 08:22 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-21 08:22 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-21 08:22 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-21 08:22 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-21 08:22 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-21 08:22 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-21 08:22 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-21 08:22 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-21 08:22 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-21 08:22 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-21 08:22 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-21 08:22 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-21 08:22 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-21 08:22 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-21 08:22 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-21 08:22 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-21 08:22 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-21 08:22 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-21 08:22 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-21 08:22 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-21 08:22 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-21 08:22 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-21 08:22 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-21 08:22 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-21 08:22 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-21 08:22 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-21 08:22 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-21 08:22 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-21 08:22 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-21 08:22 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-21 08:22 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-21 08:22 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-21 08:22 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-21 08:22 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-21 08:22 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-21 08:22 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-21 08:22 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-21 08:22 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-21 08:22 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-21 08:22 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-21 08:22 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-21 08:22 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-21 08:22 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-21 08:22 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-21 08:22 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-21 08:22 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-21 08:22 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-21 08:22 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-21 08:22 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-21 08:22 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-21 08:22 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-21 08:22 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-21 08:22 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-21 08:22 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-21 08:22 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-21 08:22 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-21 08:22 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-21 08:22 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-21 08:22 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-21 08:22 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-21 08:22 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-21 08:22 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-21 08:22 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-21 08:22 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-21 08:22 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-21 08:22 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-21 08:22 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-21 08:22 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-21 08:22 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-21 08:22 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-21 08:22 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-21 08:22 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-21 08:22 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-21 08:22 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-21 08:22 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-21 08:22 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-21 08:22 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-21 08:22 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-21 08:22 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-21 08:22 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-21 08:22 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-21 08:22 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-21 08:22 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-21 08:22 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-21 08:22 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10747 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-21 08:22 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-21 08:22 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-21 08:22 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-21 08:22 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-21 08:22 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-21 08:22 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-21 08:22 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-21 08:22 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-21 08:22 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-21 08:22 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-21 08:22 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-21 08:22 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-21 08:22 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-21 08:22 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-21 08:22 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-21 08:22 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-21 08:22 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-21 08:22 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-21 08:22 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-21 08:22 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-21 08:22 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-21 08:22 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4423 b- defN 24-May-21 08:24 nucliadb-4.0.0.post527.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 08:24 nucliadb-4.0.0.post527.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-21 08:24 nucliadb-4.0.0.post527.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-21 08:24 nucliadb-4.0.0.post527.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-21 08:23 nucliadb-4.0.0.post527.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43350 b- defN 24-May-21 08:24 nucliadb-4.0.0.post527.dist-info/RECORD
-462 files, 2264169 bytes uncompressed, 696129 bytes compressed:  69.3%
+Zip file size: 765175 bytes, number of entries: 462
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-21 10:03 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-21 10:03 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-21 10:03 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-21 10:03 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-21 10:03 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-21 10:03 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-21 10:03 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-21 10:03 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-21 10:03 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-21 10:03 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-21 10:03 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-21 10:03 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-21 10:03 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-21 10:03 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-21 10:03 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-21 10:03 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-21 10:03 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-21 10:03 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-21 10:03 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-21 10:03 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-21 10:03 nucliadb/health.py
+-rw-r--r--  2.0 unx    11639 b- defN 24-May-21 10:03 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-21 10:03 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-21 10:03 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 10:03 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-21 10:03 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 24-May-21 10:03 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-21 10:03 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-21 10:03 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-21 10:03 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22091 b- defN 24-May-21 10:03 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-21 10:03 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-21 10:03 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-21 10:03 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-21 10:03 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12515 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-21 10:03 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-21 10:03 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-21 10:03 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-21 10:03 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-21 10:03 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-21 10:03 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-21 10:03 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1880 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-21 10:03 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-21 10:03 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-21 10:03 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-21 10:03 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-21 10:03 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-21 10:03 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-21 10:03 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-21 10:03 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-21 10:03 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-21 10:03 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-21 10:03 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-21 10:03 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-21 10:03 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-21 10:03 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-21 10:03 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-21 10:03 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-21 10:03 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-21 10:03 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-21 10:03 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-21 10:03 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-21 10:03 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-21 10:03 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-21 10:03 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-21 10:03 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-21 10:03 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19969 b- defN 24-May-21 10:03 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-21 10:03 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-21 10:03 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-21 10:03 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-21 10:03 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-21 10:03 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-21 10:03 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-21 10:03 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-21 10:03 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-21 10:03 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-21 10:03 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-21 10:03 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-21 10:03 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-21 10:03 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-21 10:03 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28448 b- defN 24-May-21 10:03 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-21 10:03 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-21 10:03 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17171 b- defN 24-May-21 10:03 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-21 10:03 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-21 10:03 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-21 10:03 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-21 10:03 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-21 10:03 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-21 10:03 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-21 10:03 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    30462 b- defN 24-May-21 10:03 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-21 10:03 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-21 10:03 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-21 10:03 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-21 10:03 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-21 10:03 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-21 10:03 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-21 10:03 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-21 10:03 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-21 10:03 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-21 10:03 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-21 10:03 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-21 10:03 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-21 10:03 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-21 10:03 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-21 10:03 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-21 10:03 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-21 10:03 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-21 10:03 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-21 10:03 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-21 10:03 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-21 10:03 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-21 10:03 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-21 10:03 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-21 10:03 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-21 10:03 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-21 10:03 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7988 b- defN 24-May-21 10:03 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-21 10:03 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-21 10:03 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-21 10:03 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-21 10:03 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-21 10:03 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-21 10:03 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-21 10:03 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-21 10:03 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-21 10:03 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-21 10:03 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-21 10:03 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-21 10:03 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-21 10:03 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-21 10:03 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-21 10:03 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-21 10:03 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-21 10:03 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-21 10:03 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-21 10:03 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-21 10:03 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-21 10:03 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-21 10:03 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-21 10:03 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-21 10:03 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-21 10:03 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-21 10:03 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-21 10:03 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-21 10:03 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-21 10:03 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-21 10:03 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-21 10:03 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-21 10:03 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-21 10:03 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-21 10:03 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-21 10:03 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-21 10:03 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-21 10:03 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-21 10:03 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-21 10:03 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-21 10:03 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-21 10:03 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-21 10:03 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-21 10:03 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-21 10:03 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-21 10:03 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-21 10:03 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-21 10:03 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-21 10:03 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-21 10:03 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-21 10:03 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-21 10:03 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-21 10:03 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-21 10:03 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-21 10:03 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-21 10:03 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-21 10:03 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-21 10:03 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-21 10:03 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-21 10:03 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-21 10:03 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-21 10:03 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-21 10:03 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-21 10:03 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-21 10:03 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-21 10:03 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-21 10:03 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-21 10:03 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-21 10:03 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-21 10:03 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-21 10:03 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-21 10:03 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-21 10:03 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-21 10:03 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-21 10:03 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-21 10:03 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-21 10:03 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-21 10:03 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-21 10:03 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-21 10:03 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-21 10:03 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-21 10:03 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-21 10:03 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-21 10:03 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-21 10:03 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-21 10:03 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-21 10:03 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-21 10:03 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-21 10:03 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-21 10:03 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-21 10:03 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-21 10:03 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-21 10:03 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-21 10:03 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-21 10:03 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-21 10:03 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-21 10:03 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-21 10:03 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-21 10:03 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-21 10:03 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-21 10:03 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-21 10:03 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-21 10:03 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-21 10:03 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-21 10:03 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-21 10:03 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-21 10:03 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-21 10:03 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-21 10:03 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-21 10:03 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-21 10:03 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-21 10:03 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-21 10:03 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-21 10:03 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-21 10:03 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-21 10:03 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-21 10:03 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-21 10:03 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-21 10:03 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-21 10:03 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-21 10:03 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-21 10:03 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-21 10:03 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-21 10:03 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-21 10:03 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-21 10:03 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-21 10:03 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-21 10:03 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-21 10:03 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-21 10:03 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-21 10:03 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-21 10:03 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-21 10:03 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-21 10:03 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-21 10:03 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-21 10:03 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-21 10:03 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-21 10:03 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-21 10:03 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-21 10:03 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-21 10:03 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-21 10:03 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-21 10:03 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-21 10:03 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-21 10:03 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-21 10:03 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-21 10:03 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-21 10:03 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-21 10:03 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-21 10:03 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-21 10:03 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-21 10:03 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-21 10:03 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-21 10:03 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-21 10:03 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-21 10:03 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-21 10:03 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-21 10:03 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-21 10:03 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-21 10:03 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-21 10:03 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-21 10:03 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-21 10:03 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-21 10:03 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-21 10:03 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-21 10:03 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-21 10:03 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-21 10:03 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-21 10:03 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-21 10:03 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-21 10:03 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-21 10:03 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-21 10:03 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-21 10:03 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-21 10:03 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-21 10:03 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-21 10:03 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-21 10:03 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-21 10:03 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4423 b- defN 24-May-21 10:05 nucliadb-4.0.0.post528.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 10:05 nucliadb-4.0.0.post528.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-21 10:05 nucliadb-4.0.0.post528.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-21 10:05 nucliadb-4.0.0.post528.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 10:04 nucliadb-4.0.0.post528.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43359 b- defN 24-May-21 10:05 nucliadb-4.0.0.post528.dist-info/RECORD
+462 files, 2260478 bytes uncompressed, 695829 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -177,14 +177,17 @@
 
 Filename: nucliadb/common/datamanagers/resources.py
 Comment: 
 
 Filename: nucliadb/common/datamanagers/rollover.py
 Comment: 
 
+Filename: nucliadb/common/datamanagers/synonyms.py
+Comment: 
+
 Filename: nucliadb/common/datamanagers/utils.py
 Comment: 
 
 Filename: nucliadb/common/http_clients/__init__.py
 Comment: 
 
 Filename: nucliadb/common/http_clients/auth.py
@@ -351,17 +354,14 @@
 
 Filename: nucliadb/ingest/orm/metrics.py
 Comment: 
 
 Filename: nucliadb/ingest/orm/resource.py
 Comment: 
 
-Filename: nucliadb/ingest/orm/synonyms.py
-Comment: 
-
 Filename: nucliadb/ingest/orm/utils.py
 Comment: 
 
 Filename: nucliadb/ingest/orm/processor/__init__.py
 Comment: 
 
 Filename: nucliadb/ingest/orm/processor/auditing.py
@@ -1362,26 +1362,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.0.post527.dist-info/METADATA
+Filename: nucliadb-4.0.0.post528.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.0.post527.dist-info/WHEEL
+Filename: nucliadb-4.0.0.post528.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.0.post527.dist-info/entry_points.txt
+Filename: nucliadb-4.0.0.post528.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post527.dist-info/top_level.txt
+Filename: nucliadb-4.0.0.post528.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post527.dist-info/zip-safe
+Filename: nucliadb-4.0.0.post528.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.0.post527.dist-info/RECORD
+Filename: nucliadb-4.0.0.post528.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/datamanagers/__init__.py

```diff
@@ -24,21 +24,32 @@
 #   - Manage keys of K/V Storage and try not to leak them
 #   - Transactions are managed OUTSIDE of the datamanagers module
 #   - There shouldn't be ANY db commits in the datamanagers module, that is handled outside right now.
 #   - Module level functions only
 #   - First argument is always a transaction, all other arguments are keyword arguments and must be explicit
 #     (better for readability and code editors)
 # ==============================================================================
-from . import cluster, entities, exceptions, kb, labels, processing, resources, rollover
+from . import (
+    cluster,
+    entities,
+    exceptions,
+    kb,
+    labels,
+    processing,
+    resources,
+    rollover,
+    synonyms,
+)
 from .utils import with_transaction
 
 __all__ = (
     "cluster",
-    "kb",
     "entities",
+    "exceptions",
+    "kb",
     "labels",
+    "processing",
     "resources",
     "rollover",
-    "processing",
-    "exceptions",
+    "synonyms",
     "with_transaction",
 )
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -42,15 +42,14 @@
 from nucliadb.ingest import SERVICE_NAME, logger
 from nucliadb.ingest.orm.exceptions import KnowledgeBoxConflict
 from nucliadb.ingest.orm.resource import (
     KB_RESOURCE_SLUG,
     KB_RESOURCE_SLUG_BASE,
     Resource,
 )
-from nucliadb.ingest.orm.synonyms import Synonyms
 from nucliadb.ingest.orm.utils import (
     choose_matryoshka_dimension,
     compute_paragraph_key,
     get_basic,
     set_basic,
 )
 from nucliadb.migrator.utils import get_latest_version
@@ -72,15 +71,14 @@
 
 class KnowledgeBox:
     def __init__(self, txn: Transaction, storage: Storage, kbid: str):
         self.txn = txn
         self.storage = storage
         self.kbid = kbid
         self._config: Optional[KnowledgeBoxConfig] = None
-        self.synonyms = Synonyms(self.txn, self.kbid)
 
     async def get_config(self) -> Optional[KnowledgeBoxConfig]:
         if self._config is None:
             async with datamanagers.with_transaction() as txn:
                 config = await datamanagers.kb.get_config(txn, kbid=self.kbid)
             if config is not None:
                 self._config = config
@@ -256,23 +254,23 @@
 
     async def del_labelset(self, id: str):
         await datamanagers.labels.delete_labelset(
             self.txn, kbid=self.kbid, labelset_id=id
         )
 
     async def get_synonyms(self, synonyms: PBSynonyms):
-        pbsyn = await self.synonyms.get()
+        pbsyn = await datamanagers.synonyms.get(self.txn, kbid=self.kbid)
         if pbsyn is not None:
             synonyms.CopyFrom(pbsyn)
 
     async def set_synonyms(self, synonyms: PBSynonyms):
-        await self.synonyms.set(synonyms)
+        await datamanagers.synonyms.set(self.txn, kbid=self.kbid, synonyms=synonyms)
 
     async def delete_synonyms(self):
-        await self.synonyms.clear()
+        await datamanagers.synonyms.delete(self.txn, kbid=self.kbid)
 
     @classmethod
     async def purge(cls, driver: Driver, kbid: str):
         """
         Deletes all kb parts
 
         It takes care of signaling the nodes related to this kb that they
```

## nucliadb/ingest/service/writer.py

```diff
@@ -47,27 +47,25 @@
     GetEntitiesGroupResponse,
     GetEntitiesRequest,
     GetEntitiesResponse,
     GetLabelSetRequest,
     GetLabelSetResponse,
     GetLabelsRequest,
     GetLabelsResponse,
-    GetSynonymsResponse,
     IndexResource,
     IndexStatus,
     ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse,
     ListMembersRequest,
     ListMembersResponse,
     NewEntitiesGroupRequest,
     NewEntitiesGroupResponse,
     OpStatusWriter,
     SetEntitiesRequest,
     SetLabelsRequest,
-    SetSynonymsRequest,
     SetVectorsRequest,
     SetVectorsResponse,
     UpdateEntitiesGroupRequest,
     UpdateEntitiesGroupResponse,
     UploadBinaryData,
     WriterStatusRequest,
     WriterStatusResponse,
@@ -75,15 +73,14 @@
 
 from nucliadb import learning_proxy
 from nucliadb.common import datamanagers
 from nucliadb.common.cluster.exceptions import AlreadyExists, EntitiesGroupNotFound
 from nucliadb.common.cluster.manager import get_index_nodes
 from nucliadb.common.cluster.utils import get_shard_manager
 from nucliadb.common.datamanagers.exceptions import KnowledgeBoxNotFound
-from nucliadb.common.maindb.driver import Transaction
 from nucliadb.common.maindb.utils import setup_driver
 from nucliadb.ingest import SERVICE_NAME, logger
 from nucliadb.ingest.orm.entities import EntitiesManager
 from nucliadb.ingest.orm.exceptions import KnowledgeBoxConflict
 from nucliadb.ingest.orm.knowledgebox import KnowledgeBox as KnowledgeBoxORM
 from nucliadb.ingest.orm.processor import Processor, sequence_manager
 from nucliadb.ingest.orm.resource import Resource as ResourceORM
@@ -540,79 +537,14 @@
                 logger.error("Error in ingest gRPC servicer", exc_info=True)
                 response.status = OpStatusWriter.Status.ERROR
             else:
                 await txn.commit()
                 response.status = OpStatusWriter.Status.OK
             return response
 
-    async def GetSynonyms(  # type: ignore
-        self, request: KnowledgeBoxID, context=None
-    ) -> GetSynonymsResponse:
-        kbid = request
-        response = GetSynonymsResponse()
-        txn: Transaction
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, kbid)
-            if kbobj is None:
-                response.status.status = OpStatusWriter.Status.NOTFOUND
-                return response
-            try:
-                await kbobj.get_synonyms(response.synonyms)
-                response.status.status = OpStatusWriter.Status.OK
-                return response
-            except Exception as e:
-                errors.capture_exception(e)
-                logger.exception("Errors getting synonyms")
-                response.status.status = OpStatusWriter.Status.ERROR
-                return response
-
-    async def SetSynonyms(  # type: ignore
-        self, request: SetSynonymsRequest, context=None
-    ) -> OpStatusWriter:
-        kbid = request.kbid
-        response = OpStatusWriter()
-        txn: Transaction
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, kbid)
-            if kbobj is None:
-                response.status = OpStatusWriter.Status.NOTFOUND
-                return response
-            try:
-                await kbobj.set_synonyms(request.synonyms)
-                await txn.commit()
-                response.status = OpStatusWriter.Status.OK
-                return response
-            except Exception as e:
-                errors.capture_exception(e)
-                logger.exception("Errors setting synonyms")
-                response.status = OpStatusWriter.Status.ERROR
-                return response
-
-    async def DelSynonyms(  # type: ignore
-        self, request: KnowledgeBoxID, context=None
-    ) -> OpStatusWriter:
-        kbid = request
-        response = OpStatusWriter()
-        txn: Transaction
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, kbid)
-            if kbobj is None:
-                response.status = OpStatusWriter.Status.NOTFOUND
-                return response
-            try:
-                await kbobj.delete_synonyms()
-                await txn.commit()
-                response.status = OpStatusWriter.Status.OK
-                return response
-            except Exception as e:
-                errors.capture_exception(e)
-                logger.exception("Errors deleting synonyms")
-                response.status = OpStatusWriter.Status.ERROR
-                return response
-
     async def Status(  # type: ignore
         self, request: WriterStatusRequest, context=None
     ) -> WriterStatusResponse:
         logger.info("Status Call")
         response = WriterStatusResponse()
         async with self.driver.transaction() as txn:
             async for _, slug in datamanagers.kb.get_kbs(txn):
```

## nucliadb/reader/api/v1/services.py

```diff
@@ -20,26 +20,24 @@
 import asyncio
 from typing import Optional, Union
 
 from fastapi import HTTPException
 from fastapi.responses import StreamingResponse
 from fastapi_versioning import version  # type: ignore
 from google.protobuf.json_format import MessageToDict
-from nucliadb_protos.knowledgebox_pb2 import KnowledgeBoxID
+from nucliadb_protos.knowledgebox_pb2 import Synonyms
 from nucliadb_protos.writer_pb2 import (
     GetEntitiesGroupRequest,
     GetEntitiesGroupResponse,
     GetLabelSetRequest,
     GetLabelSetResponse,
     GetLabelsRequest,
     GetLabelsResponse,
-    GetSynonymsResponse,
     ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse,
-    OpStatusWriter,
 )
 from starlette.requests import Request
 
 from nucliadb.common import datamanagers
 from nucliadb.common.cluster.settings import in_standalone_mode
 from nucliadb.common.context.fastapi import get_app_context
 from nucliadb.common.http_clients import processing
@@ -213,25 +211,23 @@
     tags=["Knowledge Box Services"],
     response_model=KnowledgeBoxSynonyms,
     openapi_extra={"x-operation_order": 2},
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_custom_synonyms(request: Request, kbid: str):
-    ingest = get_ingest()
-    pbrequest = KnowledgeBoxID(uuid=kbid)
-    pbresponse: GetSynonymsResponse = await ingest.GetSynonyms(pbrequest)  # type: ignore
-    if pbresponse.status.status == OpStatusWriter.Status.OK:
-        return KnowledgeBoxSynonyms.from_message(pbresponse.synonyms)
-    elif pbresponse.status.status == OpStatusWriter.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    elif pbresponse.status.status == OpStatusWriter.Status.ERROR:
-        raise HTTPException(
-            status_code=500, detail="Error getting synonyms of a Knowledge box"
-        )
+    async with datamanagers.with_transaction(read_only=True) as txn:
+        if not datamanagers.kb.exists_kb(txn, kbid=kbid):
+            raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+        synonyms = await datamanagers.synonyms.get(txn, kbid=kbid)
+
+    if synonyms is None:
+        synonyms = Synonyms()
+
+    return KnowledgeBoxSynonyms.from_message(synonyms)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/notifications",
     status_code=200,
     summary="Knowledge Box Notifications Stream",
     description="Provides a stream of activity notifications for the given Knowledge Box. The stream will be automatically closed after 2 minutes.",  # noqa: E501
```

## nucliadb/search/search/query.py

```diff
@@ -22,15 +22,14 @@
 from datetime import datetime
 from typing import Any, Awaitable, Optional, Union
 
 from async_lru import alru_cache
 from nucliadb_protos.noderesources_pb2 import Resource
 
 from nucliadb.common import datamanagers
-from nucliadb.ingest.orm.synonyms import Synonyms
 from nucliadb.middleware.transaction import get_read_only_transaction
 from nucliadb.search import logger
 from nucliadb.search.predict import SendToPredictError, convert_relations
 from nucliadb.search.search.filters import (
     convert_to_node_filters,
     flat_filter_labels,
     has_classification_label_filters,
@@ -703,15 +702,15 @@
     ResourceProcessingStatus.EXPIRED: Resource.ResourceStatus.EXPIRED,
 }
 
 
 @query_parse_dependency_observer.wrap({"type": "synonyms"})
 async def get_kb_synonyms(kbid: str) -> Optional[knowledgebox_pb2.Synonyms]:
     txn = await get_read_only_transaction()
-    return await Synonyms(txn, kbid).get()
+    return await datamanagers.synonyms.get(txn, kbid=kbid)
 
 
 @query_parse_dependency_observer.wrap({"type": "entities_meta_cache"})
 async def get_entities_meta_cache(kbid: str) -> datamanagers.entities.EntitiesMetaCache:
     txn = await get_read_only_transaction()
     return await datamanagers.entities.get_entities_meta_cache(txn, kbid=kbid)
```

## nucliadb/writer/api/v1/services.py

```diff
@@ -15,30 +15,29 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 from fastapi import HTTPException, Response
 from fastapi_versioning import version
-from nucliadb_protos.knowledgebox_pb2 import KnowledgeBoxID
 from nucliadb_protos.knowledgebox_pb2 import Label as LabelPB
 from nucliadb_protos.knowledgebox_pb2 import LabelSet as LabelSetPB
 from nucliadb_protos.writer_pb2 import (
     DelEntitiesRequest,
     DelLabelsRequest,
     NewEntitiesGroupRequest,
     NewEntitiesGroupResponse,
     OpStatusWriter,
     SetLabelsRequest,
-    SetSynonymsRequest,
     UpdateEntitiesGroupRequest,
     UpdateEntitiesGroupResponse,
 )
 from starlette.requests import Request
 
+from nucliadb.common import datamanagers
 from nucliadb.models.responses import (
     HTTPConflict,
     HTTPInternalServerError,
     HTTPNotFound,
 )
 from nucliadb.writer.api.v1.router import KB_PREFIX, api
 from nucliadb_models.entities import (
@@ -250,43 +249,37 @@
     summary="Set Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def set_custom_synonyms(request: Request, kbid: str, item: KnowledgeBoxSynonyms):
-    ingest = get_ingest()
-    pbrequest = SetSynonymsRequest()
-    pbrequest.kbid.uuid = kbid
-    pbrequest.synonyms.CopyFrom(item.to_message())
-    status: OpStatusWriter = await ingest.SetSynonyms(pbrequest)  # type: ignore
-    if status.status == OpStatusWriter.Status.OK:
-        return Response(status_code=204)
-    elif status.status == OpStatusWriter.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    elif status.status == OpStatusWriter.Status.ERROR:
-        raise HTTPException(
-            status_code=500, detail="Error setting synonyms of a Knowledge box"
-        )
+    synonyms = item.to_message()
+
+    async with datamanagers.with_transaction() as txn:
+        if not datamanagers.kb.exists_kb(txn, kbid=kbid):
+            raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+
+        await datamanagers.synonyms.set(txn, kbid=kbid, synonyms=synonyms)
+        await txn.commit()
+
+    return Response(status_code=204)
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=204,
     summary="Delete Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 3},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_custom_synonyms(request: Request, kbid: str):
-    ingest = get_ingest()
-    pbrequest = KnowledgeBoxID(uuid=kbid)
-    status: OpStatusWriter = await ingest.DelSynonyms(pbrequest)  # type: ignore
-    if status.status == OpStatusWriter.Status.OK:
-        return Response(status_code=204)
-    elif status.status == OpStatusWriter.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    elif status.status == OpStatusWriter.Status.ERROR:
-        raise HTTPException(
-            status_code=500, detail="Error deleting synonyms of a Knowledge box"
-        )
+    async with datamanagers.with_transaction() as txn:
+        if not datamanagers.kb.exists_kb(txn, kbid=kbid):
+            raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+
+        await datamanagers.synonyms.delete(txn, kbid=kbid)
+        await txn.commit()
+
+    return Response(status_code=204)
```

## Comparing `nucliadb-4.0.0.post527.dist-info/METADATA` & `nucliadb-4.0.0.post528.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.0.post527
+Version: 4.0.0.post528
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post527
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post527
-Requires-Dist: nucliadb-protos >=4.0.0.post527
-Requires-Dist: nucliadb-models >=4.0.0.post527
+Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post528
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post528
+Requires-Dist: nucliadb-protos >=4.0.0.post528
+Requires-Dist: nucliadb-models >=4.0.0.post528
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.0.post527.dist-info/entry_points.txt` & `nucliadb-4.0.0.post528.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.0.post527.dist-info/RECORD` & `nucliadb-4.0.0.post528.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,24 @@
 nucliadb/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=Rgw6w8vICjieoqhvhoHZ6mUgXbJpyXHvqpFPQ96N1yA,13712
 nucliadb/common/cluster/standalone/index_node.py,sha256=aKpkAEosp9qbd-77fYgE1AAnDc-6ER05cA_HJtkeBT0,4683
 nucliadb/common/cluster/standalone/service.py,sha256=tJI5Gc-cu4uprC84bcLQr4CMW0hBS9T2YX_Ex6zeyuI,3444
 nucliadb/common/cluster/standalone/utils.py,sha256=Y6Ni9P5piE9EeacQb4L5-o_TisAk2fl4btLwAV3tt8g,3545
 nucliadb/common/context/__init__.py,sha256=BuPPLOpTTzgD4oRb6mgmjPu-gRIaq4NeZTjx8FxAIV0,3440
 nucliadb/common/context/fastapi.py,sha256=qsxQ8s5dl67uCATrwdJCXA9JDfVn3DqxgsiWf6MUJhE,1628
-nucliadb/common/datamanagers/__init__.py,sha256=nr-HLFp_3u3SZeVYMvi5ew_VGGLYNO1cQWWAXfB9b1Y,1813
+nucliadb/common/datamanagers/__init__.py,sha256=BEBU1dnrSWjQIe1DzBN5jJJHyR4C_Bp2_GDivoxPlrg,1880
 nucliadb/common/datamanagers/cluster.py,sha256=Rc_gWufL-Fx3zQ7WlgCFYBPQD9fPjUvHkyW0QK6hBSg,1451
 nucliadb/common/datamanagers/entities.py,sha256=vQe_xdyqqsII0wmqKWp1yxVTFmB67Tc6bnVxezRUVK0,5383
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
 nucliadb/common/datamanagers/resources.py,sha256=5RA4m_YhUJGSm7Ygq3ytcEQEk1eZNddELRKfHoQN0LU,8719
 nucliadb/common/datamanagers/rollover.py,sha256=oxrvnCWM69MG7liMekwQx8TXuNzwixEKJT_--f5Uf-0,5634
+nucliadb/common/datamanagers/synonyms.py,sha256=f7m3N7SXoYSDWvrNDcAeWoWVAHKI8ByZhnBrZ8rVdec,1548
 nucliadb/common/datamanagers/utils.py,sha256=Ll17Pbn1AunTUcGjrk7F2d1SJ0RBOejdmAAlE1BaNmM,1631
 nucliadb/common/http_clients/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/http_clients/auth.py,sha256=9A1k-H121W3lAFRl_XxGizcxUw_qw1STDZqJOC2Kpyw,2146
 nucliadb/common/http_clients/exceptions.py,sha256=47Y8OjkaGV_F18G07FpJhOzgWKUIexhlILyuVtICz8s,1100
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
 nucliadb/common/http_clients/pypi.py,sha256=VHIUjwJEJVntVUo_FRoXIo8sLmluy7sa9-iXSITcrMY,1540
 nucliadb/common/http_clients/utils.py,sha256=b7FCaOSf21UVE9OqDhBpWetxP2nguV_gKwBBb9dYifI,1551
@@ -110,25 +111,24 @@
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=SUVp5MqMW9LN4Wx7vB23SsSAmEAn8eug4qdPnkdxEyM,4531
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=VeOdXmlqYVWQnB4iL934d1QI2t7__KWz8gcfP4QSnTQ,28448
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
-nucliadb/ingest/orm/knowledgebox.py,sha256=urKMAL8Rj0Unen5AZ4Au-Z-176Vk1mOiXTUF4PnqMMs,17167
+nucliadb/ingest/orm/knowledgebox.py,sha256=wthcza3ngRDLE4ebS_FMofIPqJzFT3PPoXPnGo2n748,17171
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=gmmVw8tkAcH8oYQdfuxSrRhD8KZ4mh0oPs3SML2RGtY,60444
-nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
 nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
 nucliadb/ingest/orm/processor/__init__.py,sha256=sVQkEd-TGjTUMHGXJS3IIEtydLD-jSOoAYQK05pO_rA,27042
 nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/service/writer.py,sha256=WCdV-EK4WBEbNS7RPGkj0Kp0txW7MEVRc2lSyKUg7Ls,33193
+nucliadb/ingest/service/writer.py,sha256=OffZlErS9ndAEnTptFnbwOJqEXujvKd9Dbsgf5vSh3I,30462
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
 nucliadb/ingest/tests/fixtures.py,sha256=L4HeWexZwgpzPl872er2sAisfrW0OdmgOvx7SzCDrWM,24060
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=kUUrdaR-iDFjmkip025rpYP5v6x3MIXLWd_n_c8-DXY,2500
@@ -183,15 +183,15 @@
 nucliadb/reader/api/v1/download.py,sha256=ZO_KjjF9qM4K_xcEW7c1S0ZnieGkhv3Yu2E4kSU9F_s,12392
 nucliadb/reader/api/v1/export_import.py,sha256=nBYEwFnKUJYsiXUlbfKIL_jI9Ec5UVZE-2fCbK1rfQk,6459
 nucliadb/reader/api/v1/knowledgebox.py,sha256=Pd71iqTVRgx5u_Gb2LegDTQ3gGTKbVLsAvgcZne5_lM,3641
 nucliadb/reader/api/v1/learning_collector.py,sha256=6XDrfEZffqPrFYGj9TDfWOS1wcy3n9DRu35aH6-2WRA,2099
 nucliadb/reader/api/v1/learning_config.py,sha256=T1bxwsNDnVaeW9lkO4WTO9RHjz6GhYCJwvS1_MNYTes,4472
 nucliadb/reader/api/v1/resource.py,sha256=GkCjExN6wUyIKKgZ9FliDFcPj_VGMhw9KJobYWZf5N8,13951
 nucliadb/reader/api/v1/router.py,sha256=eyNmEGSP9zHkCIG5XlAXl6sukq950B7gFT3X2peMtIE,1011
-nucliadb/reader/api/v1/services.py,sha256=PssrduMSIbZuSxPBYMIvjpQpzCWZ-lzFkdjlAGQHYwE,12399
+nucliadb/reader/api/v1/services.py,sha256=OSQXi-QcuhS_LDzwzntiLgP16jIYwTn48iypdzYayTQ,12115
 nucliadb/reader/reader/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/reader/notifications.py,sha256=2In2E-2FUawjqNWKaxqrw_rB2hTzgAXVV5yFhF4gHOA,7988
 nucliadb/reader/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/tests/conftest.py,sha256=RH5huJVfSZ9cQgzEWC_xViGbXUelZFuHmrOnWb-FpEU,1224
 nucliadb/reader/tests/fixtures.py,sha256=pVrolKyIQaUA01Coe8WHG6OuliqREnzq8DJnnfPF8_k,4345
 nucliadb/reader/tests/test_list_resources.py,sha256=yKsG6MLh4_cB7Yhov0OoBAVCJCXnpuQmT453R1oVQ6Q,2748
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
@@ -231,15 +231,15 @@
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
 nucliadb/search/search/find.py,sha256=_cGdIfSqpaxm01SqTbcQCQJtadeiL71HB4zEIBj1dM4,4612
 nucliadb/search/search/find_merge.py,sha256=vhq14MFE7N9-9SNlg66LNUr6YAhR9cW22oDpmjvQhL0,17152
 nucliadb/search/search/merge.py,sha256=-srmB1gZEuMa9c2_hLTD1ihjJwDhdB6wnp9b7ljxuIM,21282
 nucliadb/search/search/metrics.py,sha256=4xQm4Q0_-R1bgMtnrbm-YaClEFR8HE6wDk9lunCrhjo,1130
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
 nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
-nucliadb/search/search/query.py,sha256=cq6BFwnLdfAfrcGhJfW3DNlVvY1Vk7JGoO2TVFgJ8sU,31127
+nucliadb/search/search/query.py,sha256=U5GL6z6sjViFcRiQfk_lRZizC3AM0EjkSWh3OY9wQxA,31093
 nucliadb/search/search/shards.py,sha256=0p_BWLEVrK87htqhavZ2ixA2l253FPQnre3RpThtZco,3018
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/chat/ask.py,sha256=4yLOqeIJDKt5zVl78knppDqfgeMqZjRUEIiEbQxfDkM,16676
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
 nucliadb/search/search/chat/prompt.py,sha256=W98mZrhrscjkxVJ02OM7veAQ1fjMrNDSZ1CUSaECCCk,20793
@@ -420,15 +420,15 @@
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
 nucliadb/writer/api/v1/export_import.py,sha256=SucHn2UX0hKRpfs_AYv8MNq-DPu1DIlSORd_K4N-cjk,6571
 nucliadb/writer/api/v1/field.py,sha256=Yi0F1IUin2TaQXyh9QDSwwzrqfjKw7nrAVbfnhl7z3o,24482
 nucliadb/writer/api/v1/knowledgebox.py,sha256=624Uv5_UHacWLv1p2YoMAR7oFPUlM9VgmiwsuJezqWk,5248
 nucliadb/writer/api/v1/learning_config.py,sha256=GaYaagjBrVG9ZxrWQyVQfqGMQV3tAJjqJ5CStaKhktU,2058
 nucliadb/writer/api/v1/resource.py,sha256=BBgRL4pQydm1arcsRCV-Y8FB1OBDggjQ9yZzxGVWivg,18893
 nucliadb/writer/api/v1/router.py,sha256=RjuoWLpZer6Kl2BW_wznpNo6XL3BOpdTGqXZCn3QrrQ,1034
-nucliadb/writer/api/v1/services.py,sha256=jzgAck-Y9IsF8mSyPqFjV2TFqlt2Ccr9kn7tX5HuF7Q,10747
+nucliadb/writer/api/v1/services.py,sha256=uK6XZnbw3zGT83SzPMFgQPLLU4IFrT3g-0_VOj2DXbA,10216
 nucliadb/writer/api/v1/upload.py,sha256=hkyXA_YlvH5j9jdf48rdmUuSf8T29hUXwBD0DNgLUP0,30857
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=7Y1vfuKDv1b3e7NCjEvDg8mktGR1rnzHaC5_qNj-3YQ,16319
@@ -450,13 +450,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.0.post527.dist-info/METADATA,sha256=RiPNmi9I22vKkN3N9Iq9MBorh2mRpCh-7Rg8zos0Te8,4423
-nucliadb-4.0.0.post527.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.0.post527.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.0.post527.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.0.post527.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.0.post527.dist-info/RECORD,,
+nucliadb-4.0.0.post528.dist-info/METADATA,sha256=DYKfgw-h83ZkRcnZKHLEiiCbkNU1ZRzirjbSZ6GYB1g,4423
+nucliadb-4.0.0.post528.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.0.post528.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.0.post528.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.0.post528.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.0.post528.dist-info/RECORD,,
```

