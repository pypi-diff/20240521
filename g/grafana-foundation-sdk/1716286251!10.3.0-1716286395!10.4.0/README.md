# Comparing `tmp/grafana_foundation_sdk-1716286251!10.3.0.tar.gz` & `tmp/grafana_foundation_sdk-1716286395!10.4.0.tar.gz`

## Comparing `grafana_foundation_sdk-1716286251!10.3.0.tar` & `grafana_foundation_sdk-1716286395!10.4.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/alertgroups.py
--rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/alerting.py
--rw-r--r--   0        0        0    20808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    38877 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    21577 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    47999 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    19359 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    49050 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    68920 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    21123 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    18123 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    18300 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/expr.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    19466 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    19922 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    28505 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    32444 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    20375 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    18325 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    21222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    20840 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    23440 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    23157 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    28079 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    12347 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    18572 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    46074 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    45797 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    36403 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/alertgroups.py
--rw-r--r--   0        0        0    27221 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/alerting.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    86326 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    84422 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    91828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/expr.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    27647 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    20904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286251!10.3.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    19462 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/alerting.py
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    39410 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    22110 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    48937 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    49337 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    72017 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    21656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    18656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/expr.py
+-rw-r--r--   0        0        0    21074 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    19922 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    30092 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    18909 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    21755 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    21373 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    23973 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    23690 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    28612 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    19105 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    46607 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    46330 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0    27052 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/alerting.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    86957 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    91828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/expr.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    27647 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    21562 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716286395!10.4.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/alertgroups.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/alertgroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/alerting.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -496,14 +514,23 @@
             self._internal.options = candlestick.Options()
         assert isinstance(self._internal.options, candlestick.Options)
         legend_resource = legend.build()
         self._internal.options.legend = legend_resource
     
         return self
     
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = candlestick.Options()
+        assert isinstance(self._internal.options, candlestick.Options)
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
+    
+        return self
+    
     def include_all_fields(self, include_all_fields: bool) -> typing.Self:    
         """
         When enabled, all fields will be sent to the graph
         """
             
         if self._internal.options is None:
             self._internal.options = candlestick.Options()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -462,14 +480,26 @@
         if self._internal.options is None:
             self._internal.options = canvas.Options()
         assert isinstance(self._internal.options, canvas.Options)
         self._internal.options.pan_zoom = pan_zoom
     
         return self
     
+    def infinite_pan(self, infinite_pan: bool) -> typing.Self:    
+        """
+        Enable infinite pan
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = canvas.Options()
+        assert isinstance(self._internal.options, canvas.Options)
+        self._internal.options.infinite_pan = infinite_pan
+    
+        return self
+    
     def root(self, root: canvas.CanvasOptionsRoot) -> typing.Self:    
         """
         The root element of canvas (frame), where all canvas elements are nested
         TODO: Figure out how to define a default value for this
         """
             
         if self._internal.options is None:
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,15 +730,15 @@
 
     def __init__(self):
         self._internal = common.GraphThresholdsStyleConfig()
 
     def build(self) -> common.GraphThresholdsStyleConfig:
         return self._internal    
     
-    def mode(self, mode: common.GraphTresholdsStyleMode) -> typing.Self:        
+    def mode(self, mode: common.GraphThresholdsStyleMode) -> typing.Self:        
         self._internal.mode = mode
     
         return self
     
 
 class SingleStatBaseOptions(cogbuilder.Builder[common.SingleStatBaseOptions]):    
     """
@@ -1190,14 +1190,24 @@
         return self
     
     def sort(self, sort: common.SortOrder) -> typing.Self:        
         self._internal.sort = sort
     
         return self
     
+    def max_width(self, max_width: float) -> typing.Self:        
+        self._internal.max_width = max_width
+    
+        return self
+    
+    def max_height(self, max_height: float) -> typing.Self:        
+        self._internal.max_height = max_height
+    
+        return self
+    
 
 class TableSortByFieldState(cogbuilder.Builder[common.TableSortByFieldState]):    
     """
     Sort by field state
     """
     
     _internal: common.TableSortByFieldState
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         Day when the week starts. Expressed by the name of the day in lowercase, e.g. "monday".
         """
             
         self._internal.week_start = week_start
     
         return self
     
-    def refresh(self, refresh: typing.Union[str, typing.Literal[False]]) -> typing.Self:    
+    def refresh(self, refresh: str) -> typing.Self:    
         """
         Refresh rate of dashboard. Represented via interval string, e.g. "5s", "1m", "1h", "1d".
         """
             
         self._internal.refresh = refresh
     
         return self
@@ -859,14 +859,23 @@
         Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
         """
             
         self._internal.time_options = time_options
     
         return self
     
+    def now_delay(self, now_delay: str) -> typing.Self:    
+        """
+        Override the now time by entering a time delay. Use this option to accommodate known delays in data aggregation to avoid null values.
+        """
+            
+        self._internal.now_delay = now_delay
+    
+        return self
+    
 
 class Snapshot(cogbuilder.Builder[dashboard.Snapshot]):    
     """
     A dashboard snapshot shares an interactive dashboard publicly.
     It is a read-only version of a dashboard, and is not editable.
     It is possible to create a snapshot of a snapshot.
     Grafana strips away all sensitive information from the dashboard.
@@ -913,14 +922,23 @@
         external url, if snapshot was shared in external grafana instance
         """
             
         self._internal.external_url = external_url
     
         return self
     
+    def original_url(self, original_url: str) -> typing.Self:    
+        """
+        original url, url of the dashboard that was snapshotted
+        """
+            
+        self._internal.original_url = original_url
+    
+        return self
+    
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the snapshot
         """
             
         self._internal.id_val = id_val
     
@@ -1230,14 +1248,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -1714,28 +1750,60 @@
         Options that can be selected for a variable.
         """
             
         self._internal.options = options
     
         return self
     
-    def refresh(self, refresh: dashboard.VariableRefresh) -> typing.Self:        
+    def refresh(self, refresh: dashboard.VariableRefresh) -> typing.Self:    
+        """
+        Options to config when to refresh a variable
+        """
+            
         self._internal.refresh = refresh
     
         return self
     
     def sort(self, sort: dashboard.VariableSort) -> typing.Self:    
         """
         Options sort order
         """
             
         self._internal.sort = sort
     
         return self
     
+    def include_all(self, include_all: bool) -> typing.Self:    
+        """
+        Whether all value option is available or not
+        """
+            
+        self._internal.include_all = include_all
+    
+        return self
+    
+    def all_value(self, all_value: str) -> typing.Self:    
+        """
+        Custom all value
+        """
+            
+        self._internal.all_value = all_value
+    
+        return self
+    
+    def regex(self, regex: str) -> typing.Self:    
+        """
+        Optional field, if you want to extract part of a series name or metric node segment.
+        Named capture groups can be used to separate the display text and value.
+        """
+            
+        self._internal.regex = regex
+    
+        return self
+    
 
 class AdHocVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -1920,14 +1988,42 @@
         Whether multiple values can be selected or not from variable value list
         """
             
         self._internal.multi = multi
     
         return self
     
+    def include_all(self, include_all: bool) -> typing.Self:    
+        """
+        Whether all value option is available or not
+        """
+            
+        self._internal.include_all = include_all
+    
+        return self
+    
+    def all_value(self, all_value: str) -> typing.Self:    
+        """
+        Custom all value
+        """
+            
+        self._internal.all_value = all_value
+    
+        return self
+    
+    def regex(self, regex: str) -> typing.Self:    
+        """
+        Optional field, if you want to extract part of a series name or metric node segment.
+        Named capture groups can be used to separate the display text and value.
+        """
+            
+        self._internal.regex = regex
+    
+        return self
+    
 
 class IntervalVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -2165,8 +2261,26 @@
         """
         Options that can be selected for a variable.
         """
             
         self._internal.options = options
     
         return self
+    
+    def include_all(self, include_all: bool) -> typing.Self:    
+        """
+        Whether all value option is available or not
+        """
+            
+        self._internal.include_all = include_all
+    
+        return self
+    
+    def all_value(self, all_value: str) -> typing.Self:    
+        """
+        Custom all value
+        """
+            
+        self._internal.all_value = all_value
+    
+        return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import debug
+from ..models import news
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "debug"
+        self._internal.type_val = "news"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -426,23 +444,27 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def mode(self, mode: debug.DebugMode) -> typing.Self:        
+    def feed_url(self, feed_url: str) -> typing.Self:    
+        """
+        empty/missing will default to grafana blog
+        """
+            
         if self._internal.options is None:
-            self._internal.options = debug.Options()
-        assert isinstance(self._internal.options, debug.Options)
-        self._internal.options.mode = mode
+            self._internal.options = news.Options()
+        assert isinstance(self._internal.options, news.Options)
+        self._internal.options.feed_url = feed_url
     
         return self
     
-    def counters(self, counters: debug.UpdateConfig) -> typing.Self:        
+    def show_image(self, show_image: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = debug.Options()
-        assert isinstance(self._internal.options, debug.Options)
-        self._internal.options.counters = counters
+            self._internal.options = news.Options()
+        assert isinstance(self._internal.options, news.Options)
+        self._internal.options.show_image = show_image
     
         return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/expr.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/expr.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/gauge.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/grafanapyroscope.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files 14% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -604,14 +622,36 @@
         if self._internal.options.tooltip is None:
             self._internal.options.tooltip = heatmap.HeatmapTooltip()
         assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
         self._internal.options.tooltip.mode = mode
     
         return self
     
+    def max_height(self, max_height: float) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = heatmap.Options()
+        assert isinstance(self._internal.options, heatmap.Options)
+        if self._internal.options.tooltip is None:
+            self._internal.options.tooltip = heatmap.HeatmapTooltip()
+        assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
+        self._internal.options.tooltip.max_height = max_height
+    
+        return self
+    
+    def max_width(self, max_width: float) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = heatmap.Options()
+        assert isinstance(self._internal.options, heatmap.Options)
+        if self._internal.options.tooltip is None:
+            self._internal.options.tooltip = heatmap.HeatmapTooltip()
+        assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
+        self._internal.options.tooltip.max_width = max_width
+    
+        return self
+    
     def show_y_histogram(self) -> typing.Self:    
         """
         Controls if the tooltip shows a histogram of the y-axis values
         """
             
         if self._internal.options is None:
             self._internal.options = heatmap.Options()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -427,27 +445,41 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
+    def bucket_count(self, bucket_count: int) -> typing.Self:    
+        """
+        Bucket count (approx)
+        """
+            
+        if not bucket_count > 0:
+            raise ValueError("bucket_count must be > 0")
+        if self._internal.options is None:
+            self._internal.options = histogram.Options()
+        assert isinstance(self._internal.options, histogram.Options)
+        self._internal.options.bucket_count = bucket_count
+    
+        return self
+    
     def bucket_size(self, bucket_size: int) -> typing.Self:    
         """
         Size of each bucket
         """
             
         if self._internal.options is None:
             self._internal.options = histogram.Options()
         assert isinstance(self._internal.options, histogram.Options)
         self._internal.options.bucket_size = bucket_size
     
         return self
     
-    def bucket_offset(self, bucket_offset: int) -> typing.Self:    
+    def bucket_offset(self, bucket_offset: float) -> typing.Self:    
         """
         Offset buckets by this amount
         """
             
         if self._internal.options is None:
             self._internal.options = histogram.Options()
         assert isinstance(self._internal.options, histogram.Options)
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,23 +202,14 @@
         The version of the plugin that is used for this panel. This is used to find the plugin to display the panel and to migrate old panel configs.
         """
             
         self._internal.plugin_version = plugin_version
     
         return self
     
-    def tags(self, tags: list[str]) -> typing.Self:    
-        """
-        Tags for the panel.
-        """
-            
-        self._internal.tags = tags
-    
-        return self
-    
     def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         targets_resources = [r1.build() for r1 in targets]
         self._internal.targets = targets_resources
@@ -365,14 +356,32 @@
         Controls if the timeFrom or timeShift overrides are shown in the panel header
         """
             
         self._internal.hide_time_override = hide_time_override
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def options(self, options: object) -> typing.Self:    
         """
         It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
         """
             
         self._internal.options = options
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -451,14 +469,22 @@
         if self._internal.options is None:
             self._internal.options = logs.Options()
         assert isinstance(self._internal.options, logs.Options)
         self._internal.options.show_time = show_time
     
         return self
     
+    def show_log_context_toggle(self, show_log_context_toggle: bool) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_log_context_toggle = show_log_context_toggle
+    
+        return self
+    
     def wrap_log_message(self, wrap_log_message: bool) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = logs.Options()
         assert isinstance(self._internal.options, logs.Options)
         self._internal.options.wrap_log_message = wrap_log_message
     
         return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import news
+from ..models import nodegraph
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "news"
+        self._internal.type_val = "nodeGraph"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -426,27 +444,23 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def feed_url(self, feed_url: str) -> typing.Self:    
-        """
-        empty/missing will default to grafana blog
-        """
-            
+    def nodes(self, nodes: nodegraph.NodeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = news.Options()
-        assert isinstance(self._internal.options, news.Options)
-        self._internal.options.feed_url = feed_url
+            self._internal.options = nodegraph.Options()
+        assert isinstance(self._internal.options, nodegraph.Options)
+        self._internal.options.nodes = nodes
     
         return self
     
-    def show_image(self, show_image: bool) -> typing.Self:        
+    def edges(self, edges: nodegraph.EdgeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = news.Options()
-        assert isinstance(self._internal.options, news.Options)
-        self._internal.options.show_image = show_image
+            self._internal.options = nodegraph.Options()
+        assert isinstance(self._internal.options, nodegraph.Options)
+        self._internal.options.edges = edges
     
         return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import nodegraph
+from ..models import text
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "nodeGraph"
+        self._internal.type_val = "text"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -426,23 +444,31 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def nodes(self, nodes: nodegraph.NodeOptions) -> typing.Self:        
+    def mode(self, mode: text.TextMode) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.mode = mode
+    
+        return self
+    
+    def code(self, code: text.CodeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = nodegraph.Options()
-        assert isinstance(self._internal.options, nodegraph.Options)
-        self._internal.options.nodes = nodes
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.code = code
     
         return self
     
-    def edges(self, edges: nodegraph.EdgeOptions) -> typing.Self:        
+    def content(self, content: str) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = nodegraph.Options()
-        assert isinstance(self._internal.options, nodegraph.Options)
-        self._internal.options.edges = edges
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.content = content
     
         return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/parca.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/prometheus.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/prometheus.py`

 * *Files 16% similar despite different names*

```diff
@@ -83,14 +83,20 @@
         See https://github.com/grafana/grafana/issues/48081
         """
             
         self._internal.interval_factor = interval_factor
     
         return self
     
+    def scope(self, scope: cogbuilder.Builder[prometheus.PrometheusDataqueryScope]) -> typing.Self:        
+        scope_resource = scope.build()
+        self._internal.scope = scope_resource
+    
+        return self
+    
     def ref_id(self, ref_id: str) -> typing.Self:    
         """
         A unique identifier for the query within the list of targets.
         In server side expressions, the refId is used as a variable name to identify results.
         By default, the UI will assign A->Z; however setting meaningful names may be useful.
         """
             
@@ -136,8 +142,23 @@
         An additional lower limit for the step parameter of the Prometheus query and for the
         `$__interval` and `$__rate_interval` variables.
         """
             
         self._internal.interval = interval
     
         return self
+    
+
+class PrometheusDataqueryScope(cogbuilder.Builder[prometheus.PrometheusDataqueryScope]):    
+    _internal: prometheus.PrometheusDataqueryScope
+
+    def __init__(self):
+        self._internal = prometheus.PrometheusDataqueryScope()
+
+    def build(self) -> prometheus.PrometheusDataqueryScope:
+        return self._internal    
+    
+    def matchers(self, matchers: str) -> typing.Self:        
+        self._internal.matchers = matchers
+    
+        return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files 3% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
         @deprecated Define the maximum duration to select traces. Use duration format, for example: 1.2s, 100ms
         """
             
         self._internal.max_duration = max_duration
     
         return self
     
-    def service_map_query(self, service_map_query: str) -> typing.Self:    
+    def service_map_query(self, service_map_query: typing.Union[str, list[str]]) -> typing.Self:    
         """
-        Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}
+        Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}. Providing multiple values will produce union of results for each filter, using PromQL OR operator internally.
         """
             
         self._internal.service_map_query = service_map_query
     
         return self
     
     def service_map_include_namespace(self, service_map_include_namespace: bool) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/testdata.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/testdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def __init__(self):
         self._internal = testdata.StreamingQuery()
 
     def build(self) -> testdata.StreamingQuery:
         return self._internal    
     
-    def type_val(self, type_val: typing.Literal["signal", "logs", "fetch"]) -> typing.Self:        
+    def type_val(self, type_val: typing.Literal["signal", "logs", "fetch", "traces"]) -> typing.Self:        
         self._internal.type_val = type_val
     
         return self
     
     def speed(self, speed: int) -> typing.Self:        
         self._internal.speed = speed
     
@@ -116,24 +116,29 @@
 
     def __init__(self):
         self._internal = testdata.NodesQuery()
 
     def build(self) -> testdata.NodesQuery:
         return self._internal    
     
-    def type_val(self, type_val: typing.Literal["random", "response", "random edges"]) -> typing.Self:        
+    def type_val(self, type_val: typing.Literal["random", "response_small", "response_medium", "random edges"]) -> typing.Self:        
         self._internal.type_val = type_val
     
         return self
     
     def count(self, count: int) -> typing.Self:        
         self._internal.count = count
     
         return self
     
+    def seed(self, seed: int) -> typing.Self:        
+        self._internal.seed = seed
+    
+        return self
+    
 
 class USAQuery(cogbuilder.Builder[testdata.USAQuery]):    
     _internal: testdata.USAQuery
 
     def __init__(self):
         self._internal = testdata.USAQuery()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/text.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import text
+from ..models import debug
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "text"
+        self._internal.type_val = "debug"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -246,14 +246,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -426,31 +444,23 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def mode(self, mode: text.TextMode) -> typing.Self:        
+    def mode(self, mode: debug.DebugMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = text.Options()
-        assert isinstance(self._internal.options, text.Options)
+            self._internal.options = debug.Options()
+        assert isinstance(self._internal.options, debug.Options)
         self._internal.options.mode = mode
     
         return self
     
-    def code(self, code: text.CodeOptions) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = text.Options()
-        assert isinstance(self._internal.options, text.Options)
-        self._internal.options.code = code
-    
-        return self
-    
-    def content(self, content: str) -> typing.Self:        
+    def counters(self, counters: debug.UpdateConfig) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = text.Options()
-        assert isinstance(self._internal.options, text.Options)
-        self._internal.options.content = content
+            self._internal.options = debug.Options()
+        assert isinstance(self._internal.options, debug.Options)
+        self._internal.options.counters = counters
     
         return self
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/trend.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/builders/xychart.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,32 @@
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
+    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
+        """
+        Sets panel queries cache timeout.
+        """
+            
+        self._internal.cache_timeout = cache_timeout
+    
+        return self
+    
+    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
+        """
+        Overrides the data source configured time-to-live for a query cache item in milliseconds
+        """
+            
+        self._internal.query_caching_ttl = query_caching_ttl
+    
+        return self
+    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/plugins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import parca
-from ..models import prometheus
-from ..models import trend
-from ..models import cloudwatch
-from ..models import elasticsearch
-from ..models import stat
-from ..models import xychart
-from ..models import geomap
-from ..models import nodegraph
 from ..models import azuremonitor
-from ..models import candlestick
+from ..models import datagrid
 from ..models import logs
-from ..models import news
+from ..models import parca
+from ..models import statetimeline
 from ..models import table
-from ..models import tempo
-from ..models import loki
-from ..models import timeseries
-from ..models import googlecloudmonitoring
+from ..models import testdata
 from ..models import dashboardlist
+from ..models import histogram
+from ..models import loki
+from ..models import piechart
+from ..models import xychart
+from ..models import debug
+from ..models import gauge
 from ..models import grafanapyroscope
+from ..models import news
+from ..models import candlestick
+from ..models import cloudwatch
+from ..models import elasticsearch
+from ..models import nodegraph
+from ..models import text
+from ..models import timeseries
+from ..models import trend
+from ..models import bargauge
 from ..models import alertgroups
 from ..models import annotationslist
-from ..models import canvas
-from ..models import debug
-from ..models import statushistory
 from ..models import barchart
-from ..models import datagrid
-from ..models import testdata
-from ..models import bargauge
+from ..models import canvas
+from ..models import googlecloudmonitoring
+from ..models import tempo
+from ..models import geomap
 from ..models import heatmap
-from ..models import piechart
-from ..models import statetimeline
-from ..models import text
-from ..models import gauge
-from ..models import histogram
+from ..models import prometheus
+from ..models import stat
+from ..models import statushistory
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
     cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/alertgroups.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/alerting.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/alerting.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,18 +90,18 @@
             args["provenance"] = data["provenance"]
         if "template" in data:
             args["template"] = data["template"]        
 
         return cls(**args)
 
 
-# Matchers is a slice of Matchers that is sortable, implements Stringer, and
-# provides a Matches method to match a LabelSet against all Matchers in the
-# slice. Note that some users of Matchers might require it to be sorted.
-ObjectMatchers: typing.TypeAlias = 'Matchers'
+ObjectMatcher: typing.TypeAlias = list[str]
+
+
+ObjectMatchers: typing.TypeAlias = list['ObjectMatcher']
 
 
 Provenance: typing.TypeAlias = str
 
 
 class RelativeTimeRange:
     """
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,34 +114,37 @@
     # Sets the color strategy for the candlesticks
     color_strategy: 'ColorStrategy'
     # Map fields to appropriate dimension
     fields: 'CandlestickFieldMap'
     # Set which colors are used when the price movement is up or down
     colors: 'CandlestickColors'
     legend: common.VizLegendOptions
+    tooltip: common.VizTooltipOptions
     # When enabled, all fields will be sent to the graph
     include_all_fields: typing.Optional[bool]
 
-    def __init__(self, mode: typing.Optional['VizDisplayMode'] = None, candle_style: typing.Optional['CandleStyle'] = None, color_strategy: typing.Optional['ColorStrategy'] = None, fields: typing.Optional['CandlestickFieldMap'] = None, colors: typing.Optional['CandlestickColors'] = None, legend: typing.Optional[common.VizLegendOptions] = None, include_all_fields: typing.Optional[bool] = False):
+    def __init__(self, mode: typing.Optional['VizDisplayMode'] = None, candle_style: typing.Optional['CandleStyle'] = None, color_strategy: typing.Optional['ColorStrategy'] = None, fields: typing.Optional['CandlestickFieldMap'] = None, colors: typing.Optional['CandlestickColors'] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, include_all_fields: typing.Optional[bool] = False):
         self.mode = mode if mode is not None else VizDisplayMode.CANDLES_VOLUME
         self.candle_style = candle_style if candle_style is not None else CandleStyle.CANDLES
         self.color_strategy = color_strategy if color_strategy is not None else ColorStrategy.OPEN_CLOSE
         self.fields = fields if fields is not None else CandlestickFieldMap()
         self.colors = colors if colors is not None else CandlestickColors(down="red", flat="gray", up="green")
         self.legend = legend if legend is not None else common.VizLegendOptions()
+        self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
         self.include_all_fields = include_all_fields
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
             "candleStyle": self.candle_style,
             "colorStrategy": self.color_strategy,
             "fields": self.fields,
             "colors": self.colors,
             "legend": self.legend,
+            "tooltip": self.tooltip,
         }
         if self.include_all_fields is not None:
             payload["includeAllFields"] = self.include_all_fields
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
@@ -155,14 +158,16 @@
             args["color_strategy"] = data["colorStrategy"]
         if "fields" in data:
             args["fields"] = CandlestickFieldMap.from_json(data["fields"])
         if "colors" in data:
             args["colors"] = CandlestickColors.from_json(data["colors"])
         if "legend" in data:
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
+        if "tooltip" in data:
+            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
         if "includeAllFields" in data:
             args["include_all_fields"] = data["includeAllFields"]        
 
         return cls(**args)
 
 
 FieldConfig: typing.TypeAlias = common.GraphFieldConfig
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,43 +330,49 @@
 class Options:
     # Enable inline editing
     inline_editing: bool
     # Show all available element types
     show_advanced_types: bool
     # Enable pan and zoom
     pan_zoom: bool
+    # Enable infinite pan
+    infinite_pan: bool
     # The root element of canvas (frame), where all canvas elements are nested
     # TODO: Figure out how to define a default value for this
     root: 'CanvasOptionsRoot'
 
-    def __init__(self, inline_editing: bool = True, show_advanced_types: bool = True, pan_zoom: bool = True, root: typing.Optional['CanvasOptionsRoot'] = None):
+    def __init__(self, inline_editing: bool = True, show_advanced_types: bool = True, pan_zoom: bool = True, infinite_pan: bool = True, root: typing.Optional['CanvasOptionsRoot'] = None):
         self.inline_editing = inline_editing
         self.show_advanced_types = show_advanced_types
         self.pan_zoom = pan_zoom
+        self.infinite_pan = infinite_pan
         self.root = root if root is not None else CanvasOptionsRoot()
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "inlineEditing": self.inline_editing,
             "showAdvancedTypes": self.show_advanced_types,
             "panZoom": self.pan_zoom,
+            "infinitePan": self.infinite_pan,
             "root": self.root,
         }
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "inlineEditing" in data:
             args["inline_editing"] = data["inlineEditing"]
         if "showAdvancedTypes" in data:
             args["show_advanced_types"] = data["showAdvancedTypes"]
         if "panZoom" in data:
             args["pan_zoom"] = data["panZoom"]
+        if "infinitePan" in data:
+            args["infinite_pan"] = data["infinitePan"]
         if "root" in data:
             args["root"] = CanvasOptionsRoot.from_json(data["root"])        
 
         return cls(**args)
 
 
 class CanvasOptionsRoot:
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,15 +896,15 @@
         return cls(**args)
 
 
 CloudWatchQuery: typing.TypeAlias = typing.Union['CloudWatchMetricsQuery', 'CloudWatchLogsQuery', 'CloudWatchAnnotationQuery']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchAnnotationQuery], typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery]]] = {"Annotations": CloudWatchAnnotationQuery, "Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery}
+    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery], typing.Type[CloudWatchAnnotationQuery]]] = {"Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery, "Annotations": CloudWatchAnnotationQuery}
     return cogruntime.DataqueryConfig(
         identifier="cloudwatch",
         from_json_hook=lambda data: decoding_map[data["queryMode"]].from_json(data),
     )
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1037,15 +1037,15 @@
         
         if "hideFrom" in data:
             args["hide_from"] = HideSeriesConfig.from_json(data["hideFrom"])        
 
         return cls(**args)
 
 
-class GraphTresholdsStyleMode(enum.StrEnum):
+class GraphThresholdsStyleMode(enum.StrEnum):
     """
     TODO docs
     """
 
     OFF = "off"
     LINE = "line"
     DASHED = "dashed"
@@ -1056,18 +1056,18 @@
 
 
 class GraphThresholdsStyleConfig:
     """
     TODO docs
     """
 
-    mode: 'GraphTresholdsStyleMode'
+    mode: 'GraphThresholdsStyleMode'
 
-    def __init__(self, mode: typing.Optional['GraphTresholdsStyleMode'] = None):
-        self.mode = mode if mode is not None else GraphTresholdsStyleMode.OFF
+    def __init__(self, mode: typing.Optional['GraphThresholdsStyleMode'] = None):
+        self.mode = mode if mode is not None else GraphThresholdsStyleMode.OFF
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
         }
         return payload
 
@@ -1745,34 +1745,46 @@
 class VizTooltipOptions:
     """
     TODO docs
     """
 
     mode: 'TooltipDisplayMode'
     sort: 'SortOrder'
+    max_width: typing.Optional[float]
+    max_height: typing.Optional[float]
 
-    def __init__(self, mode: typing.Optional['TooltipDisplayMode'] = None, sort: typing.Optional['SortOrder'] = None):
+    def __init__(self, mode: typing.Optional['TooltipDisplayMode'] = None, sort: typing.Optional['SortOrder'] = None, max_width: typing.Optional[float] = None, max_height: typing.Optional[float] = None):
         self.mode = mode if mode is not None else TooltipDisplayMode.SINGLE
         self.sort = sort if sort is not None else SortOrder.ASCENDING
+        self.max_width = max_width
+        self.max_height = max_height
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
             "sort": self.sort,
         }
+        if self.max_width is not None:
+            payload["maxWidth"] = self.max_width
+        if self.max_height is not None:
+            payload["maxHeight"] = self.max_height
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "mode" in data:
             args["mode"] = data["mode"]
         if "sort" in data:
-            args["sort"] = data["sort"]        
+            args["sort"] = data["sort"]
+        if "maxWidth" in data:
+            args["max_width"] = data["maxWidth"]
+        if "maxHeight" in data:
+            args["max_height"] = data["maxHeight"]        
 
         return cls(**args)
 
 
 Labels: typing.TypeAlias = dict[str, str]
 
 
@@ -1791,14 +1803,15 @@
     GRADIENT_GAUGE = "gradient-gauge"
     LCD_GAUGE = "lcd-gauge"
     JSON_VIEW = "json-view"
     BASIC_GAUGE = "basic"
     IMAGE = "image"
     GAUGE = "gauge"
     SPARKLINE = "sparkline"
+    DATA_LINKS = "data-links"
     CUSTOM = "custom"
 
 
 class TableCellBackgroundDisplayMode(enum.StrEnum):
     """
     Display mode to the "Colored Background" display
     mode for table cells. Either displays a solid color (basic mode)
@@ -1977,14 +1990,36 @@
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         return cls(**args)
 
 
+class TableDataLinksCellOptions:
+    """
+    Show data links in the cell
+    """
+
+    type_val: typing.Literal["data-links"]
+
+    def __init__(self, ):
+        self.type_val = "data-links"
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "type": self.type_val,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        return cls(**args)
+
+
 class TableBarGaugeCellOptions:
     """
     Gauge cell options
     """
 
     type_val: typing.Literal["gauge"]
     mode: typing.Optional['BarGaugeDisplayMode']
@@ -2274,15 +2309,15 @@
     SM = "sm"
     MD = "md"
     LG = "lg"
 
 
 # Table cell options. Each cell has a display mode
 # and other potential options for that display.
-TableCellOptions: typing.TypeAlias = typing.Union['TableAutoCellOptions', 'TableSparklineCellOptions', 'TableBarGaugeCellOptions', 'TableColoredBackgroundCellOptions', 'TableColorTextCellOptions', 'TableImageCellOptions', 'TableJsonViewCellOptions']
+TableCellOptions: typing.TypeAlias = typing.Union['TableAutoCellOptions', 'TableSparklineCellOptions', 'TableBarGaugeCellOptions', 'TableColoredBackgroundCellOptions', 'TableColorTextCellOptions', 'TableImageCellOptions', 'TableDataLinksCellOptions', 'TableJsonViewCellOptions']
 
 
 # Use UTC/GMT timezone
 TimeZoneUtc: typing.Literal["utc"] = "utc"
 
 
 # Use the timezone defined by end user web browser
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # When set to true, the dashboard will redraw panels at an interval matching the pixel width.
     # This will keep data "moving left" regardless of the query refresh rate. This setting helps
     # avoid dashboards presenting stale live data
     live_now: typing.Optional[bool]
     # Day when the week starts. Expressed by the name of the day in lowercase, e.g. "monday".
     week_start: typing.Optional[str]
     # Refresh rate of dashboard. Represented via interval string, e.g. "5s", "1m", "1h", "1d".
-    refresh: typing.Optional[typing.Union[str, typing.Literal[False]]]
+    refresh: typing.Optional[str]
     # Version of the JSON schema, incremented each time a Grafana update brings
     # changes to said schema.
     schema_version: int
     # Version of the dashboard, incremented each time the dashboard is updated.
     version: typing.Optional[int]
     # List of dashboard panels
     panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]]
@@ -60,15 +60,15 @@
     # See https://grafana.com/docs/grafana/latest/dashboards/build-dashboards/annotate-visualizations/
     annotations: 'AnnotationContainer'
     # Links with references to other dashboards or external websites.
     links: typing.Optional[list['DashboardLink']]
     # Snapshot options. They are present only if the dashboard is a snapshot.
     snapshot: typing.Optional['Snapshot']
 
-    def __init__(self, id_val: typing.Optional[int] = None, uid: typing.Optional[str] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, revision: typing.Optional[int] = None, gnet_id: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, timezone: typing.Optional[str] = "browser", editable: typing.Optional[bool] = True, graph_tooltip: typing.Optional['DashboardCursorSync'] = None, time: typing.Optional['DashboardDashboardTime'] = None, timepicker: typing.Optional['TimePickerConfig'] = None, fiscal_year_start_month: typing.Optional[int] = 0, live_now: typing.Optional[bool] = None, week_start: typing.Optional[str] = None, refresh: typing.Optional[typing.Union[str, typing.Literal[False]]] = None, schema_version: int = 36, version: typing.Optional[int] = None, panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]] = None, templating: typing.Optional['DashboardDashboardTemplating'] = None, annotations: typing.Optional['AnnotationContainer'] = None, links: typing.Optional[list['DashboardLink']] = None, snapshot: typing.Optional['Snapshot'] = None):
+    def __init__(self, id_val: typing.Optional[int] = None, uid: typing.Optional[str] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, revision: typing.Optional[int] = None, gnet_id: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, timezone: typing.Optional[str] = "browser", editable: typing.Optional[bool] = True, graph_tooltip: typing.Optional['DashboardCursorSync'] = None, time: typing.Optional['DashboardDashboardTime'] = None, timepicker: typing.Optional['TimePickerConfig'] = None, fiscal_year_start_month: typing.Optional[int] = 0, live_now: typing.Optional[bool] = None, week_start: typing.Optional[str] = None, refresh: typing.Optional[str] = None, schema_version: int = 36, version: typing.Optional[int] = None, panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]] = None, templating: typing.Optional['DashboardDashboardTemplating'] = None, annotations: typing.Optional['AnnotationContainer'] = None, links: typing.Optional[list['DashboardLink']] = None, snapshot: typing.Optional['Snapshot'] = None):
         self.id_val = id_val
         self.uid = uid
         self.title = title
         self.description = description
         self.revision = revision
         self.gnet_id = gnet_id
         self.tags = tags
@@ -408,32 +408,43 @@
     datasource: typing.Optional['DataSourceRef']
     # Shows current selected variable text/value on the dashboard
     current: typing.Optional['VariableOption']
     # Whether multiple values can be selected or not from variable value list
     multi: typing.Optional[bool]
     # Options that can be selected for a variable.
     options: typing.Optional[list['VariableOption']]
+    # Options to config when to refresh a variable
     refresh: typing.Optional['VariableRefresh']
     # Options sort order
     sort: typing.Optional['VariableSort']
+    # Whether all value option is available or not
+    include_all: typing.Optional[bool]
+    # Custom all value
+    all_value: typing.Optional[str]
+    # Optional field, if you want to extract part of a series name or metric node segment.
+    # Named capture groups can be used to separate the display text and value.
+    regex: typing.Optional[str]
 
-    def __init__(self, type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: typing.Optional[bool] = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, object]] = None, datasource: typing.Optional['DataSourceRef'] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None):
+    def __init__(self, type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: typing.Optional[bool] = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, object]] = None, datasource: typing.Optional['DataSourceRef'] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None, include_all: typing.Optional[bool] = False, all_value: typing.Optional[str] = None, regex: typing.Optional[str] = None):
         self.type_val = type_val if type_val is not None else VariableType.QUERY
         self.name = name
         self.label = label
         self.hide = hide
         self.skip_url_sync = skip_url_sync
         self.description = description
         self.query = query
         self.datasource = datasource
         self.current = current
         self.multi = multi
         self.options = options
         self.refresh = refresh
         self.sort = sort
+        self.include_all = include_all
+        self.all_value = all_value
+        self.regex = regex
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
             "name": self.name,
         }
         if self.label is not None:
@@ -454,14 +465,20 @@
             payload["multi"] = self.multi
         if self.options is not None:
             payload["options"] = self.options
         if self.refresh is not None:
             payload["refresh"] = self.refresh
         if self.sort is not None:
             payload["sort"] = self.sort
+        if self.include_all is not None:
+            payload["includeAll"] = self.include_all
+        if self.all_value is not None:
+            payload["allValue"] = self.all_value
+        if self.regex is not None:
+            payload["regex"] = self.regex
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
@@ -485,15 +502,21 @@
         if "multi" in data:
             args["multi"] = data["multi"]
         if "options" in data:
             args["options"] = data["options"]
         if "refresh" in data:
             args["refresh"] = data["refresh"]
         if "sort" in data:
-            args["sort"] = data["sort"]        
+            args["sort"] = data["sort"]
+        if "includeAll" in data:
+            args["include_all"] = data["includeAll"]
+        if "allValue" in data:
+            args["all_value"] = data["allValue"]
+        if "regex" in data:
+            args["regex"] = data["regex"]        
 
         return cls(**args)
 
 
 class VariableOption:
     """
     Option to be selected in a variable.
@@ -721,14 +744,15 @@
     `textbox`: Display a free text input field with an optional default value.
     `custom`: Define the variable options manually using a comma-separated list.
     `system`: Variables defined by Grafana. See: https://grafana.com/docs/grafana/latest/dashboards/variables/add-template-variables/#global-variables
     """
 
     QUERY = "query"
     ADHOC = "adhoc"
+    GROUPBY = "groupby"
     CONSTANT = "constant"
     DATASOURCE = "datasource"
     INTERVAL = "interval"
     TEXTBOX = "textbox"
     CUSTOM = "custom"
     SYSTEM = "system"
 
@@ -1217,43 +1241,53 @@
 class TimePickerConfig:
     """
     Time picker configuration
     It defines the default config for the time picker and the refresh picker for the specific dashboard.
     """
 
     # Whether timepicker is visible or not.
-    hidden: bool
+    hidden: typing.Optional[bool]
     # Interval options available in the refresh picker dropdown.
-    refresh_intervals: list[str]
+    refresh_intervals: typing.Optional[list[str]]
     # Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
-    time_options: list[str]
+    time_options: typing.Optional[list[str]]
+    # Override the now time by entering a time delay. Use this option to accommodate known delays in data aggregation to avoid null values.
+    now_delay: typing.Optional[str]
 
-    def __init__(self, hidden: bool = False, refresh_intervals: typing.Optional[list[str]] = None, time_options: typing.Optional[list[str]] = None):
+    def __init__(self, hidden: typing.Optional[bool] = False, refresh_intervals: typing.Optional[list[str]] = None, time_options: typing.Optional[list[str]] = None, now_delay: typing.Optional[str] = None):
         self.hidden = hidden
         self.refresh_intervals = refresh_intervals if refresh_intervals is not None else ["5s", "10s", "30s", "1m", "5m", "15m", "30m", "1h", "2h", "1d"]
         self.time_options = time_options if time_options is not None else ["5m", "15m", "1h", "6h", "12h", "24h", "2d", "7d", "30d"]
+        self.now_delay = now_delay
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "hidden": self.hidden,
-            "refresh_intervals": self.refresh_intervals,
-            "time_options": self.time_options,
         }
+        if self.hidden is not None:
+            payload["hidden"] = self.hidden
+        if self.refresh_intervals is not None:
+            payload["refresh_intervals"] = self.refresh_intervals
+        if self.time_options is not None:
+            payload["time_options"] = self.time_options
+        if self.now_delay is not None:
+            payload["nowDelay"] = self.now_delay
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "hidden" in data:
             args["hidden"] = data["hidden"]
         if "refresh_intervals" in data:
             args["refresh_intervals"] = data["refresh_intervals"]
         if "time_options" in data:
-            args["time_options"] = data["time_options"]        
+            args["time_options"] = data["time_options"]
+        if "nowDelay" in data:
+            args["now_delay"] = data["nowDelay"]        
 
         return cls(**args)
 
 
 class DashboardCursorSync(enum.IntEnum):
     """
     0 for no shared crosshair or tooltip (default).
@@ -1279,14 +1313,16 @@
     created: str
     # Time when the snapshot expires, default is never to expire
     expires: str
     # Is the snapshot saved in an external grafana instance
     external: bool
     # external url, if snapshot was shared in external grafana instance
     external_url: str
+    # original url, url of the dashboard that was snapshotted
+    original_url: str
     # Unique identifier of the snapshot
     id_val: int
     # Optional, defined the unique key of the snapshot, required if external is true
     key: str
     # Optional, name of the snapshot
     name: str
     # org id of the snapshot
@@ -1294,33 +1330,35 @@
     # last time when the snapshot was updated
     updated: str
     # url of the snapshot, if snapshot was shared internally
     url: typing.Optional[str]
     # user id of the snapshot creator
     user_id: int
 
-    def __init__(self, created: str = "", expires: str = "", external: bool = False, external_url: str = "", id_val: int = 0, key: str = "", name: str = "", org_id: int = 0, updated: str = "", url: typing.Optional[str] = None, user_id: int = 0):
+    def __init__(self, created: str = "", expires: str = "", external: bool = False, external_url: str = "", original_url: str = "", id_val: int = 0, key: str = "", name: str = "", org_id: int = 0, updated: str = "", url: typing.Optional[str] = None, user_id: int = 0):
         self.created = created
         self.expires = expires
         self.external = external
         self.external_url = external_url
+        self.original_url = original_url
         self.id_val = id_val
         self.key = key
         self.name = name
         self.org_id = org_id
         self.updated = updated
         self.url = url
         self.user_id = user_id
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "created": self.created,
             "expires": self.expires,
             "external": self.external,
             "externalUrl": self.external_url,
+            "originalUrl": self.original_url,
             "id": self.id_val,
             "key": self.key,
             "name": self.name,
             "orgId": self.org_id,
             "updated": self.updated,
             "userId": self.user_id,
         }
@@ -1336,14 +1374,16 @@
             args["created"] = data["created"]
         if "expires" in data:
             args["expires"] = data["expires"]
         if "external" in data:
             args["external"] = data["external"]
         if "externalUrl" in data:
             args["external_url"] = data["externalUrl"]
+        if "originalUrl" in data:
+            args["original_url"] = data["originalUrl"]
         if "id" in data:
             args["id_val"] = data["id"]
         if "key" in data:
             args["key"] = data["key"]
         if "name" in data:
             args["name"] = data["name"]
         if "orgId" in data:
@@ -1365,16 +1405,14 @@
 
     # The panel plugin type id. This is used to find the plugin to display the panel.
     type_val: str
     # Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
     id_val: typing.Optional[int]
     # The version of the plugin that is used for this panel. This is used to find the plugin to display the panel and to migrate old panel configs.
     plugin_version: typing.Optional[str]
-    # Tags for the panel.
-    tags: typing.Optional[list[str]]
     # Depends on the panel plugin. See the plugin documentation for details.
     targets: typing.Optional[list[cogvariants.Dataquery]]
     # Panel title.
     title: typing.Optional[str]
     # Panel description.
     description: typing.Optional[str]
     # Whether to display the panel without a background.
@@ -1418,24 +1456,27 @@
     # Note: Panel time overrides have no effect when the dashboard’s time range is absolute.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_shift: typing.Optional[str]
     # Controls if the timeFrom or timeShift overrides are shown in the panel header
     hide_time_override: typing.Optional[bool]
     # Dynamically load the panel
     library_panel: typing.Optional['LibraryPanelRef']
+    # Sets panel queries cache timeout.
+    cache_timeout: typing.Optional[str]
+    # Overrides the data source configured time-to-live for a query cache item in milliseconds
+    query_caching_ttl: typing.Optional[float]
     # It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
     options: typing.Optional[object]
     # Field options allow you to change how the data is displayed in your visualizations.
     field_config: typing.Optional['FieldConfigSource']
 
-    def __init__(self, type_val: str = "", id_val: typing.Optional[int] = None, plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional['DataSourceRef'] = None, grid_pos: typing.Optional['GridPos'] = None, links: typing.Optional[list['DashboardLink']] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list['DataTransformerConfig']] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, library_panel: typing.Optional['LibraryPanelRef'] = None, options: typing.Optional[object] = None, field_config: typing.Optional['FieldConfigSource'] = None):
+    def __init__(self, type_val: str = "", id_val: typing.Optional[int] = None, plugin_version: typing.Optional[str] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional['DataSourceRef'] = None, grid_pos: typing.Optional['GridPos'] = None, links: typing.Optional[list['DashboardLink']] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list['DataTransformerConfig']] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, library_panel: typing.Optional['LibraryPanelRef'] = None, cache_timeout: typing.Optional[str] = None, query_caching_ttl: typing.Optional[float] = None, options: typing.Optional[object] = None, field_config: typing.Optional['FieldConfigSource'] = None):
         self.type_val = type_val
         self.id_val = id_val
         self.plugin_version = plugin_version
-        self.tags = tags
         self.targets = targets
         self.title = title
         self.description = description
         self.transparent = transparent
         self.datasource = datasource
         self.grid_pos = grid_pos
         self.links = links
@@ -1445,27 +1486,27 @@
         self.max_data_points = max_data_points
         self.transformations = transformations
         self.interval = interval
         self.time_from = time_from
         self.time_shift = time_shift
         self.hide_time_override = hide_time_override
         self.library_panel = library_panel
+        self.cache_timeout = cache_timeout
+        self.query_caching_ttl = query_caching_ttl
         self.options = options
         self.field_config = field_config
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
         }
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.plugin_version is not None:
             payload["pluginVersion"] = self.plugin_version
-        if self.tags is not None:
-            payload["tags"] = self.tags
         if self.targets is not None:
             payload["targets"] = self.targets
         if self.title is not None:
             payload["title"] = self.title
         if self.description is not None:
             payload["description"] = self.description
         if self.transparent is not None:
@@ -1492,14 +1533,18 @@
             payload["timeFrom"] = self.time_from
         if self.time_shift is not None:
             payload["timeShift"] = self.time_shift
         if self.hide_time_override is not None:
             payload["hideTimeOverride"] = self.hide_time_override
         if self.library_panel is not None:
             payload["libraryPanel"] = self.library_panel
+        if self.cache_timeout is not None:
+            payload["cacheTimeout"] = self.cache_timeout
+        if self.query_caching_ttl is not None:
+            payload["queryCachingTTL"] = self.query_caching_ttl
         if self.options is not None:
             payload["options"] = self.options
         if self.field_config is not None:
             payload["fieldConfig"] = self.field_config
         return payload
 
     @classmethod
@@ -1508,16 +1553,14 @@
         
         if "type" in data:
             args["type_val"] = data["type"]
         if "id" in data:
             args["id_val"] = data["id"]
         if "pluginVersion" in data:
             args["plugin_version"] = data["pluginVersion"]
-        if "tags" in data:
-            args["tags"] = data["tags"]
         if "targets" in data:
             args["targets"] = [cogruntime.dataquery_from_json(dataquery_json, data["datasource"]["type"] if data.get("datasource") is not None and data["datasource"].get("type", "") != "" else "") for dataquery_json in data["targets"]]
         if "title" in data:
             args["title"] = data["title"]
         if "description" in data:
             args["description"] = data["description"]
         if "transparent" in data:
@@ -1544,14 +1587,18 @@
             args["time_from"] = data["timeFrom"]
         if "timeShift" in data:
             args["time_shift"] = data["timeShift"]
         if "hideTimeOverride" in data:
             args["hide_time_override"] = data["hideTimeOverride"]
         if "libraryPanel" in data:
             args["library_panel"] = LibraryPanelRef.from_json(data["libraryPanel"])
+        if "cacheTimeout" in data:
+            args["cache_timeout"] = data["cacheTimeout"]
+        if "queryCachingTTL" in data:
+            args["query_caching_ttl"] = data["queryCachingTTL"]
         if "options" in data:
             config = cogruntime.panelcfg_config(data.get("type", ""))
             if config is not None and config.options_from_json_hook is not None:
                 args["options"] = config.options_from_json_hook(data["options"])
             else:
                 args["options"] = data["options"]
         if "fieldConfig" in data:
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/expr.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..cog import variants as cogvariants
 
 
 Expr: typing.TypeAlias = typing.Union['TypeMath', 'TypeReduce', 'TypeResample', 'TypeClassicConditions', 'TypeThreshold', 'TypeSql']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[TypeSql], typing.Type[TypeMath], typing.Type[TypeReduce], typing.Type[TypeResample], typing.Type[TypeClassicConditions], typing.Type[TypeThreshold]]] = {"sql": TypeSql, "math": TypeMath, "reduce": TypeReduce, "resample": TypeResample, "classic_conditions": TypeClassicConditions, "threshold": TypeThreshold}
+    decoding_map: dict[str, typing.Union[typing.Type[TypeReduce], typing.Type[TypeResample], typing.Type[TypeClassicConditions], typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath]]] = {"reduce": TypeReduce, "resample": TypeResample, "classic_conditions": TypeClassicConditions, "threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath}
     return cogruntime.DataqueryConfig(
         identifier="__expr__",
         from_json_hook=lambda data: decoding_map[data["type"]].from_json(data),
     )
 
 
 class TypeMath(cogvariants.Dataquery):
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/gauge.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/grafanapyroscope.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,40 +292,52 @@
 class HeatmapTooltip:
     """
     Controls tooltip options
     """
 
     # Controls how the tooltip is shown
     mode: common.TooltipDisplayMode
+    max_height: typing.Optional[float]
+    max_width: typing.Optional[float]
     # Controls if the tooltip shows a histogram of the y-axis values
     y_histogram: typing.Optional[bool]
     # Controls if the tooltip shows a color scale in header
     show_color_scale: typing.Optional[bool]
 
-    def __init__(self, mode: typing.Optional[common.TooltipDisplayMode] = None, y_histogram: typing.Optional[bool] = None, show_color_scale: typing.Optional[bool] = None):
+    def __init__(self, mode: typing.Optional[common.TooltipDisplayMode] = None, max_height: typing.Optional[float] = None, max_width: typing.Optional[float] = None, y_histogram: typing.Optional[bool] = None, show_color_scale: typing.Optional[bool] = None):
         self.mode = mode if mode is not None else common.TooltipDisplayMode.SINGLE
+        self.max_height = max_height
+        self.max_width = max_width
         self.y_histogram = y_histogram
         self.show_color_scale = show_color_scale
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
         }
+        if self.max_height is not None:
+            payload["maxHeight"] = self.max_height
+        if self.max_width is not None:
+            payload["maxWidth"] = self.max_width
         if self.y_histogram is not None:
             payload["yHistogram"] = self.y_histogram
         if self.show_color_scale is not None:
             payload["showColorScale"] = self.show_color_scale
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "mode" in data:
             args["mode"] = data["mode"]
+        if "maxHeight" in data:
+            args["max_height"] = data["maxHeight"]
+        if "maxWidth" in data:
+            args["max_width"] = data["maxWidth"]
         if "yHistogram" in data:
             args["y_histogram"] = data["yHistogram"]
         if "showColorScale" in data:
             args["show_color_scale"] = data["showColorScale"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/histogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,47 +2,54 @@
 
 import typing
 from ..models import common
 from ..cog import runtime as cogruntime
 
 
 class Options:
+    # Bucket count (approx)
+    bucket_count: typing.Optional[int]
     # Size of each bucket
     bucket_size: typing.Optional[int]
     # Offset buckets by this amount
-    bucket_offset: typing.Optional[int]
+    bucket_offset: typing.Optional[float]
     legend: common.VizLegendOptions
     tooltip: common.VizTooltipOptions
     # Combines multiple series into a single histogram
     combine: typing.Optional[bool]
 
-    def __init__(self, bucket_size: typing.Optional[int] = None, bucket_offset: typing.Optional[int] = 0, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, combine: typing.Optional[bool] = None):
+    def __init__(self, bucket_count: typing.Optional[int] = 30, bucket_size: typing.Optional[int] = None, bucket_offset: typing.Optional[float] = 0, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, combine: typing.Optional[bool] = None):
+        self.bucket_count = bucket_count
         self.bucket_size = bucket_size
         self.bucket_offset = bucket_offset
         self.legend = legend if legend is not None else common.VizLegendOptions()
         self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
         self.combine = combine
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "legend": self.legend,
             "tooltip": self.tooltip,
         }
+        if self.bucket_count is not None:
+            payload["bucketCount"] = self.bucket_count
         if self.bucket_size is not None:
             payload["bucketSize"] = self.bucket_size
         if self.bucket_offset is not None:
             payload["bucketOffset"] = self.bucket_offset
         if self.combine is not None:
             payload["combine"] = self.combine
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
+        if "bucketCount" in data:
+            args["bucket_count"] = data["bucketCount"]
         if "bucketSize" in data:
             args["bucket_size"] = data["bucketSize"]
         if "bucketOffset" in data:
             args["bucket_offset"] = data["bucketOffset"]
         if "legend" in data:
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
         if "tooltip" in data:
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,16 +167,14 @@
 
 
 class LibrarypanelLibraryPanelModel:
     # The panel plugin type id. This is used to find the plugin to display the panel.
     type_val: str
     # The version of the plugin that is used for this panel. This is used to find the plugin to display the panel and to migrate old panel configs.
     plugin_version: typing.Optional[str]
-    # Tags for the panel.
-    tags: typing.Optional[list[str]]
     # Depends on the panel plugin. See the plugin documentation for details.
     targets: typing.Optional[list[cogvariants.Dataquery]]
     # Panel title.
     title: typing.Optional[str]
     # Panel description.
     description: typing.Optional[str]
     # Whether to display the panel without a background.
@@ -216,23 +214,26 @@
     # Overrides the time range for individual panels by shifting its start and end relative to the time picker.
     # For example, you can shift the time range for the panel to be two hours earlier than the dashboard time picker setting `2h`.
     # Note: Panel time overrides have no effect when the dashboard’s time range is absolute.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_shift: typing.Optional[str]
     # Controls if the timeFrom or timeShift overrides are shown in the panel header
     hide_time_override: typing.Optional[bool]
+    # Sets panel queries cache timeout.
+    cache_timeout: typing.Optional[str]
+    # Overrides the data source configured time-to-live for a query cache item in milliseconds
+    query_caching_ttl: typing.Optional[float]
     # It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
     options: typing.Optional[object]
     # Field options allow you to change how the data is displayed in your visualizations.
     field_config: typing.Optional[dashboard.FieldConfigSource]
 
-    def __init__(self, type_val: str = "", plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional[dashboard.DataSourceRef] = None, links: typing.Optional[list[dashboard.DashboardLink]] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list[dashboard.DataTransformerConfig]] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, options: typing.Optional[object] = None, field_config: typing.Optional[dashboard.FieldConfigSource] = None):
+    def __init__(self, type_val: str = "", plugin_version: typing.Optional[str] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional[dashboard.DataSourceRef] = None, links: typing.Optional[list[dashboard.DashboardLink]] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list[dashboard.DataTransformerConfig]] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, cache_timeout: typing.Optional[str] = None, query_caching_ttl: typing.Optional[float] = None, options: typing.Optional[object] = None, field_config: typing.Optional[dashboard.FieldConfigSource] = None):
         self.type_val = type_val
         self.plugin_version = plugin_version
-        self.tags = tags
         self.targets = targets
         self.title = title
         self.description = description
         self.transparent = transparent
         self.datasource = datasource
         self.links = links
         self.repeat = repeat
@@ -240,25 +241,25 @@
         self.max_per_row = max_per_row
         self.max_data_points = max_data_points
         self.transformations = transformations
         self.interval = interval
         self.time_from = time_from
         self.time_shift = time_shift
         self.hide_time_override = hide_time_override
+        self.cache_timeout = cache_timeout
+        self.query_caching_ttl = query_caching_ttl
         self.options = options
         self.field_config = field_config
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
         }
         if self.plugin_version is not None:
             payload["pluginVersion"] = self.plugin_version
-        if self.tags is not None:
-            payload["tags"] = self.tags
         if self.targets is not None:
             payload["targets"] = self.targets
         if self.title is not None:
             payload["title"] = self.title
         if self.description is not None:
             payload["description"] = self.description
         if self.transparent is not None:
@@ -281,30 +282,32 @@
             payload["interval"] = self.interval
         if self.time_from is not None:
             payload["timeFrom"] = self.time_from
         if self.time_shift is not None:
             payload["timeShift"] = self.time_shift
         if self.hide_time_override is not None:
             payload["hideTimeOverride"] = self.hide_time_override
+        if self.cache_timeout is not None:
+            payload["cacheTimeout"] = self.cache_timeout
+        if self.query_caching_ttl is not None:
+            payload["queryCachingTTL"] = self.query_caching_ttl
         if self.options is not None:
             payload["options"] = self.options
         if self.field_config is not None:
             payload["fieldConfig"] = self.field_config
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
             args["type_val"] = data["type"]
         if "pluginVersion" in data:
             args["plugin_version"] = data["pluginVersion"]
-        if "tags" in data:
-            args["tags"] = data["tags"]
         if "targets" in data:
             args["targets"] = [cogruntime.dataquery_from_json(dataquery_json, data["datasource"]["type"] if data.get("datasource") is not None and data["datasource"].get("type", "") != "" else "") for dataquery_json in data["targets"]]
         if "title" in data:
             args["title"] = data["title"]
         if "description" in data:
             args["description"] = data["description"]
         if "transparent" in data:
@@ -327,14 +330,18 @@
             args["interval"] = data["interval"]
         if "timeFrom" in data:
             args["time_from"] = data["timeFrom"]
         if "timeShift" in data:
             args["time_shift"] = data["timeShift"]
         if "hideTimeOverride" in data:
             args["hide_time_override"] = data["hideTimeOverride"]
+        if "cacheTimeout" in data:
+            args["cache_timeout"] = data["cacheTimeout"]
+        if "queryCachingTTL" in data:
+            args["query_caching_ttl"] = data["queryCachingTTL"]
         if "options" in data:
             args["options"] = data["options"]
         if "fieldConfig" in data:
             args["field_config"] = dashboard.FieldConfigSource.from_json(data["fieldConfig"])        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 from ..cog import runtime as cogruntime
 
 
 class Options:
     show_labels: bool
     show_common_labels: bool
     show_time: bool
+    show_log_context_toggle: bool
     wrap_log_message: bool
     prettify_log_message: bool
     enable_log_details: bool
     sort_order: common.LogsSortOrder
     dedup_strategy: common.LogsDedupStrategy
 
-    def __init__(self, show_labels: bool = False, show_common_labels: bool = False, show_time: bool = False, wrap_log_message: bool = False, prettify_log_message: bool = False, enable_log_details: bool = False, sort_order: typing.Optional[common.LogsSortOrder] = None, dedup_strategy: typing.Optional[common.LogsDedupStrategy] = None):
+    def __init__(self, show_labels: bool = False, show_common_labels: bool = False, show_time: bool = False, show_log_context_toggle: bool = False, wrap_log_message: bool = False, prettify_log_message: bool = False, enable_log_details: bool = False, sort_order: typing.Optional[common.LogsSortOrder] = None, dedup_strategy: typing.Optional[common.LogsDedupStrategy] = None):
         self.show_labels = show_labels
         self.show_common_labels = show_common_labels
         self.show_time = show_time
+        self.show_log_context_toggle = show_log_context_toggle
         self.wrap_log_message = wrap_log_message
         self.prettify_log_message = prettify_log_message
         self.enable_log_details = enable_log_details
         self.sort_order = sort_order if sort_order is not None else common.LogsSortOrder.DESCENDING
         self.dedup_strategy = dedup_strategy if dedup_strategy is not None else common.LogsDedupStrategy.NONE
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "showLabels": self.show_labels,
             "showCommonLabels": self.show_common_labels,
             "showTime": self.show_time,
+            "showLogContextToggle": self.show_log_context_toggle,
             "wrapLogMessage": self.wrap_log_message,
             "prettifyLogMessage": self.prettify_log_message,
             "enableLogDetails": self.enable_log_details,
             "sortOrder": self.sort_order,
             "dedupStrategy": self.dedup_strategy,
         }
         return payload
@@ -44,14 +47,16 @@
         
         if "showLabels" in data:
             args["show_labels"] = data["showLabels"]
         if "showCommonLabels" in data:
             args["show_common_labels"] = data["showCommonLabels"]
         if "showTime" in data:
             args["show_time"] = data["showTime"]
+        if "showLogContextToggle" in data:
+            args["show_log_context_toggle"] = data["showLogContextToggle"]
         if "wrapLogMessage" in data:
             args["wrap_log_message"] = data["wrapLogMessage"]
         if "prettifyLogMessage" in data:
             args["prettify_log_message"] = data["prettifyLogMessage"]
         if "enableLogDetails" in data:
             args["enable_log_details"] = data["enableLogDetails"]
         if "sortOrder" in data:
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/loki.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     STREAM = "stream"
 
 
 class SupportingQueryType(enum.StrEnum):
     LOGS_VOLUME = "logsVolume"
     LOGS_SAMPLE = "logsSample"
     DATA_SAMPLE = "dataSample"
+    INFINITE_SCROLL = "infiniteScroll"
 
 
 class LokiQueryDirection(enum.StrEnum):
     FORWARD = "forward"
     BACKWARD = "backward"
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/preferences.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/prometheus.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/prometheus.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     # Query format to determine how to display data points in panel. It can be "time_series", "table", "heatmap"
     format_val: typing.Optional['PromQueryFormat']
     # Series name override or template. Ex. {{hostname}} will be replaced with label value for hostname
     legend_format: typing.Optional[str]
     # @deprecated Used to specify how many times to divide max data points by. We use max data points under query options
     # See https://github.com/grafana/grafana/issues/48081
     interval_factor: typing.Optional[float]
+    scope: typing.Optional['PrometheusDataqueryScope']
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
     # true if query is disabled (ie should not be returned to the dashboard)
     # Note this does not always imply that the query should not be executed since
     # the results from a hidden query may be used as the input to other queries (SSE etc)
@@ -51,23 +52,24 @@
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
     # An additional lower limit for the step parameter of the Prometheus query and for the
     # `$__interval` and `$__rate_interval` variables.
     interval: typing.Optional[str]
 
-    def __init__(self, expr: typing.Optional[str] = None, instant: typing.Optional[bool] = None, range_val: typing.Optional[bool] = None, exemplar: typing.Optional[bool] = None, editor_mode: typing.Optional['QueryEditorMode'] = None, format_val: typing.Optional['PromQueryFormat'] = None, legend_format: typing.Optional[str] = None, interval_factor: typing.Optional[float] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None, interval: typing.Optional[str] = None):
+    def __init__(self, expr: typing.Optional[str] = None, instant: typing.Optional[bool] = None, range_val: typing.Optional[bool] = None, exemplar: typing.Optional[bool] = None, editor_mode: typing.Optional['QueryEditorMode'] = None, format_val: typing.Optional['PromQueryFormat'] = None, legend_format: typing.Optional[str] = None, interval_factor: typing.Optional[float] = None, scope: typing.Optional['PrometheusDataqueryScope'] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None, interval: typing.Optional[str] = None):
         self.expr = expr
         self.instant = instant
         self.range_val = range_val
         self.exemplar = exemplar
         self.editor_mode = editor_mode
         self.format_val = format_val
         self.legend_format = legend_format
         self.interval_factor = interval_factor
+        self.scope = scope
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.datasource = datasource
         self.interval = interval
 
     def to_json(self) -> dict[str, object]:
@@ -85,14 +87,16 @@
             payload["editorMode"] = self.editor_mode
         if self.format_val is not None:
             payload["format"] = self.format_val
         if self.legend_format is not None:
             payload["legendFormat"] = self.legend_format
         if self.interval_factor is not None:
             payload["intervalFactor"] = self.interval_factor
+        if self.scope is not None:
+            payload["scope"] = self.scope
         if self.ref_id is not None:
             payload["refId"] = self.ref_id
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
         if self.datasource is not None:
@@ -117,14 +121,16 @@
             args["editor_mode"] = data["editorMode"]
         if "format" in data:
             args["format_val"] = data["format"]
         if "legendFormat" in data:
             args["legend_format"] = data["legendFormat"]
         if "intervalFactor" in data:
             args["interval_factor"] = data["intervalFactor"]
+        if "scope" in data:
+            args["scope"] = PrometheusDataqueryScope.from_json(data["scope"])
         if "refId" in data:
             args["ref_id"] = data["refId"]
         if "hide" in data:
             args["hide"] = data["hide"]
         if "queryType" in data:
             args["query_type"] = data["queryType"]
         if "datasource" in data:
@@ -138,8 +144,30 @@
 def variant_config() -> cogruntime.DataqueryConfig:
     return cogruntime.DataqueryConfig(
         identifier="prometheus",
         from_json_hook=Dataquery.from_json,
     )
 
 
+class PrometheusDataqueryScope:
+    matchers: str
+
+    def __init__(self, matchers: str = ""):
+        self.matchers = matchers
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "matchers": self.matchers,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "matchers" in data:
+            args["matchers"] = data["matchers"]        
+
+        return cls(**args)
+
+
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/stat.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/table.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/table.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/tempo.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     service_name: typing.Optional[str]
     # @deprecated Query traces by span name
     span_name: typing.Optional[str]
     # @deprecated Define the minimum duration to select traces. Use duration format, for example: 1.2s, 100ms
     min_duration: typing.Optional[str]
     # @deprecated Define the maximum duration to select traces. Use duration format, for example: 1.2s, 100ms
     max_duration: typing.Optional[str]
-    # Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}
-    service_map_query: typing.Optional[str]
+    # Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}. Providing multiple values will produce union of results for each filter, using PromQL OR operator internally.
+    service_map_query: typing.Optional[typing.Union[str, list[str]]]
     # Use service.namespace in addition to service.name to uniquely identify a service.
     service_map_include_namespace: typing.Optional[bool]
     # Defines the maximum number of traces that are returned from Tempo
     limit: typing.Optional[int]
     # Defines the maximum number of spans per spanset that are returned from Tempo
     spss: typing.Optional[int]
     filters: list['TraceqlFilter']
@@ -45,15 +45,15 @@
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
     # The type of the table that is used to display the search results
     table_type: typing.Optional['SearchTableType']
 
-    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, query: typing.Optional[str] = None, search: typing.Optional[str] = None, service_name: typing.Optional[str] = None, span_name: typing.Optional[str] = None, min_duration: typing.Optional[str] = None, max_duration: typing.Optional[str] = None, service_map_query: typing.Optional[str] = None, service_map_include_namespace: typing.Optional[bool] = None, limit: typing.Optional[int] = None, spss: typing.Optional[int] = None, filters: typing.Optional[list['TraceqlFilter']] = None, group_by: typing.Optional[list['TraceqlFilter']] = None, datasource: typing.Optional[object] = None, table_type: typing.Optional['SearchTableType'] = None):
+    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, query: typing.Optional[str] = None, search: typing.Optional[str] = None, service_name: typing.Optional[str] = None, span_name: typing.Optional[str] = None, min_duration: typing.Optional[str] = None, max_duration: typing.Optional[str] = None, service_map_query: typing.Optional[typing.Union[str, list[str]]] = None, service_map_include_namespace: typing.Optional[bool] = None, limit: typing.Optional[int] = None, spss: typing.Optional[int] = None, filters: typing.Optional[list['TraceqlFilter']] = None, group_by: typing.Optional[list['TraceqlFilter']] = None, datasource: typing.Optional[object] = None, table_type: typing.Optional['SearchTableType'] = None):
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.query = query
         self.search = search
         self.service_name = service_name
         self.span_name = span_name
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/testdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
     CSV_CONTENT = "csv_content"
     TRACE = "trace"
     MANUAL_ENTRY = "manual_entry"
     VARIABLES_QUERY = "variables-query"
 
 
 class StreamingQuery:
-    type_val: typing.Literal["signal", "logs", "fetch"]
+    type_val: typing.Literal["signal", "logs", "fetch", "traces"]
     speed: int
     spread: int
     noise: int
     bands: typing.Optional[int]
     url: typing.Optional[str]
 
-    def __init__(self, type_val: typing.Optional[typing.Literal["signal", "logs", "fetch"]] = None, speed: int = 0, spread: int = 0, noise: int = 0, bands: typing.Optional[int] = None, url: typing.Optional[str] = None):
+    def __init__(self, type_val: typing.Optional[typing.Literal["signal", "logs", "fetch", "traces"]] = None, speed: int = 0, spread: int = 0, noise: int = 0, bands: typing.Optional[int] = None, url: typing.Optional[str] = None):
         self.type_val = type_val if type_val is not None else "signal"
         self.speed = speed
         self.spread = spread
         self.noise = noise
         self.bands = bands
         self.url = url
 
@@ -171,38 +171,44 @@
         if "last" in data:
             args["last"] = data["last"]        
 
         return cls(**args)
 
 
 class NodesQuery:
-    type_val: typing.Optional[typing.Literal["random", "response", "random edges"]]
+    type_val: typing.Optional[typing.Literal["random", "response_small", "response_medium", "random edges"]]
     count: typing.Optional[int]
+    seed: typing.Optional[int]
 
-    def __init__(self, type_val: typing.Optional[typing.Literal["random", "response", "random edges"]] = None, count: typing.Optional[int] = None):
+    def __init__(self, type_val: typing.Optional[typing.Literal["random", "response_small", "response_medium", "random edges"]] = None, count: typing.Optional[int] = None, seed: typing.Optional[int] = None):
         self.type_val = type_val
         self.count = count
+        self.seed = seed
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.type_val is not None:
             payload["type"] = self.type_val
         if self.count is not None:
             payload["count"] = self.count
+        if self.seed is not None:
+            payload["seed"] = self.seed
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
             args["type_val"] = data["type"]
         if "count" in data:
-            args["count"] = data["count"]        
+            args["count"] = data["count"]
+        if "seed" in data:
+            args["seed"] = data["seed"]        
 
         return cls(**args)
 
 
 class USAQuery:
     mode: typing.Optional[str]
     period: typing.Optional[str]
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/text.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/trend.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1716286395!10.4.0/grafana_foundation_sdk/models/xychart.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 
         return cls(**args)
 
 
 class ScatterSeriesConfig:
     x: typing.Optional[str]
     y: typing.Optional[str]
+    name: typing.Optional[str]
     show: typing.Optional['ScatterShow']
     point_size: typing.Optional[common.ScaleDimensionConfig]
     point_color: typing.Optional[common.ColorDimensionConfig]
     line_color: typing.Optional[common.ColorDimensionConfig]
     line_width: typing.Optional[int]
     line_style: typing.Optional[common.LineStyle]
     label: typing.Optional[common.VisibilityMode]
@@ -206,21 +207,22 @@
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
     axis_centered_zero: typing.Optional[bool]
-    name: typing.Optional[str]
+    frame: typing.Optional[float]
     label_value: typing.Optional[common.TextDimensionConfig]
     axis_border_show: typing.Optional[bool]
 
-    def __init__(self, x: typing.Optional[str] = None, y: typing.Optional[str] = None, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, name: typing.Optional[str] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, x: typing.Optional[str] = None, y: typing.Optional[str] = None, name: typing.Optional[str] = None, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, frame: typing.Optional[float] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_border_show: typing.Optional[bool] = None):
         self.x = x
         self.y = y
+        self.name = name
         self.show = show if show is not None else ScatterShow.POINTS
         self.point_size = point_size
         self.point_color = point_color
         self.line_color = line_color
         self.line_width = line_width
         self.line_style = line_style
         self.label = label if label is not None else common.VisibilityMode.AUTO
@@ -230,25 +232,27 @@
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
         self.axis_centered_zero = axis_centered_zero
-        self.name = name
+        self.frame = frame
         self.label_value = label_value
         self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.x is not None:
             payload["x"] = self.x
         if self.y is not None:
             payload["y"] = self.y
+        if self.name is not None:
+            payload["name"] = self.name
         if self.show is not None:
             payload["show"] = self.show
         if self.point_size is not None:
             payload["pointSize"] = self.point_size
         if self.point_color is not None:
             payload["pointColor"] = self.point_color
         if self.line_color is not None:
@@ -275,30 +279,32 @@
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
         if self.axis_centered_zero is not None:
             payload["axisCenteredZero"] = self.axis_centered_zero
-        if self.name is not None:
-            payload["name"] = self.name
+        if self.frame is not None:
+            payload["frame"] = self.frame
         if self.label_value is not None:
             payload["labelValue"] = self.label_value
         if self.axis_border_show is not None:
             payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "x" in data:
             args["x"] = data["x"]
         if "y" in data:
             args["y"] = data["y"]
+        if "name" in data:
+            args["name"] = data["name"]
         if "show" in data:
             args["show"] = data["show"]
         if "pointSize" in data:
             args["point_size"] = common.ScaleDimensionConfig.from_json(data["pointSize"])
         if "pointColor" in data:
             args["point_color"] = common.ColorDimensionConfig.from_json(data["pointColor"])
         if "lineColor" in data:
@@ -325,16 +331,16 @@
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
         if "axisCenteredZero" in data:
             args["axis_centered_zero"] = data["axisCenteredZero"]
-        if "name" in data:
-            args["name"] = data["name"]
+        if "frame" in data:
+            args["frame"] = data["frame"]
         if "labelValue" in data:
             args["label_value"] = common.TextDimensionConfig.from_json(data["labelValue"])
         if "axisBorderShow" in data:
             args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/LICENSE.md` & `grafana_foundation_sdk-1716286395!10.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/README.md` & `grafana_foundation_sdk-1716286395!10.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v10.3.x.**
+> This branch contains **types and builders generated for Grafana v10.4.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1716286251!10.3.0'
+python3 -m pip install 'grafana_foundation_sdk==1716286395!10.4.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/pyproject.toml` & `grafana_foundation_sdk-1716286395!10.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1716286251!10.3.0"
+version = "1716286395!10.4.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1716286251!10.3.0/PKG-INFO` & `grafana_foundation_sdk-1716286395!10.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1716286251!10.3.0
+Version: 1716286395!10.4.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -21,21 +21,21 @@
 Description-Content-Type: text/markdown
 
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v10.3.x.**
+> This branch contains **types and builders generated for Grafana v10.4.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1716286251!10.3.0'
+python3 -m pip install 'grafana_foundation_sdk==1716286395!10.4.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

