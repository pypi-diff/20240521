# Comparing `tmp/tooz-6.1.0.tar.gz` & `tmp/tooz-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooz-6.1.0.tar", last modified: Fri Mar 15 15:12:48 2024, max compression
+gzip compressed data, was "tooz-6.2.0.tar", last modified: Tue May 21 09:34:21 2024, max compression
```

## Comparing `tooz-6.1.0.tar` & `tooz-6.2.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.082680 tooz-6.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-03-15 15:12:21.000000 tooz-6.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-03-15 15:12:21.000000 tooz-6.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-15 15:12:21.000000 tooz-6.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2024-03-15 15:12:21.000000 tooz-6.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4005 2024-03-15 15:12:47.000000 tooz-6.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2024-03-15 15:12:21.000000 tooz-6.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26255 2024-03-15 15:12:47.000000 tooz-6.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-15 15:12:21.000000 tooz-6.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2254 2024-03-15 15:12:48.082680 tooz-6.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-03-15 15:12:21.000000 tooz-6.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-15 15:12:21.000000 tooz-6.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.054679 tooz-6.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.058679 tooz-6.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.058679 tooz-6.1.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.058679 tooz-6.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.058679 tooz-6.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/compatibility.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6890 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.058679 tooz-6.1.0/doc/source/user/tutorial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/coordinator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/group_membership.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/hashring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/leader_election.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/lock.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-03-15 15:12:21.000000 tooz-6.1.0/doc/source/user/tutorial/partitioner.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.062679 tooz-6.1.0/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/coordinator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/coordinator_heartbeat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/group_membership.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/group_membership_watch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/leader_election.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/lock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2024-03-15 15:12:21.000000 tooz-6.1.0/examples/partitioner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.062679 tooz-6.1.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-03-15 15:12:21.000000 tooz-6.1.0/playbooks/stop-redis.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.050679 tooz-6.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.066679 tooz-6.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/add-consul-acl-support-2f0869681129f7e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/bug-2012226-67752e8cae8489ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/bug-2056656-f71dca8a61138f95.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/consul-heartbeat-support-3ec69e2ace537dc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/deprecate-etcd3-driver-551608037d79222b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/deprecate-zake-driver-eee8fcdfc5a88907.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/etcd-3.4-eee8300c942a1263.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/etcd3-etcd3gw-tls-support-618ab207706e67af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/etcd3-group-support-b039cf19f4a268a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/etcd3gw-api-version-discovery-3e9943c73fae48d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/etcd3gw-group-support-598832a8764a8aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/etcd3gw_create_new_lease_if_expired_during_refresh-1d631d36c21ea28c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/fix-redis-socket_keepalive-type-32b41b746f426efb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/hashring-0470f9119ef63d49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/partitioner-4005767d287dc7c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/redis-health-check-f5e3cb15dd3ac90c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/redis-username-9c552b61db4cfbec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/remove-etcd3-driver-dbce7649a08036c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/remove-strict-redis-555f0f4e369480e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/sentinel-ssl-and-auth-5cccced6685099b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.070679 tooz-6.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.070679 tooz-6.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.070679 tooz-6.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-15 15:12:21.000000 tooz-6.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2024-03-15 15:12:21.000000 tooz-6.1.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2024-03-15 15:12:21.000000 tooz-6.1.0/run-examples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2024-03-15 15:12:21.000000 tooz-6.1.0/run-tests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1167 2024-03-15 15:12:21.000000 tooz-6.1.0/setup-consul-env.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      725 2024-03-15 15:12:21.000000 tooz-6.1.0/setup-etcd-env.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2024-03-15 15:12:48.082680 tooz-6.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-03-15 15:12:21.000000 tooz-6.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-03-15 15:12:21.000000 tooz-6.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.070679 tooz-6.1.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2024-03-15 15:12:21.000000 tooz-6.1.0/tools/compat-matrix.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.074679 tooz-6.1.0/tooz/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31903 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.078680 tooz-6.1.0/tooz/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20676 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/consul.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9415 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/etcd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15786 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20581 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8685 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/ipc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20371 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/memcached.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/mysql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8171 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/pgsql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32016 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2431 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/zake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24765 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/drivers/zookeeper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3932 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/partitioner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.078680 tooz-6.1.0/tooz/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2550 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.082680 tooz-6.1.0/tooz/tests/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/test_etcd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2926 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/test_etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/test_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/test_memcache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4034 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/test_mysql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4061 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/drivers/test_postgresql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40879 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/test_coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/test_hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/test_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7922 2024-03-15 15:12:21.000000 tooz-6.1.0/tooz/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:12:48.074679 tooz-6.1.0/tooz.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2254 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4242 2024-03-15 15:12:48.000000 tooz-6.1.0/tooz.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2024-03-15 15:12:47.000000 tooz-6.1.0/tooz.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2484 2024-03-15 15:12:21.000000 tooz-6.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.515914 tooz-6.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-21 09:33:52.000000 tooz-6.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-05-21 09:33:52.000000 tooz-6.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-05-21 09:33:52.000000 tooz-6.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2024-05-21 09:33:52.000000 tooz-6.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4044 2024-05-21 09:34:21.000000 tooz-6.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2024-05-21 09:33:52.000000 tooz-6.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26594 2024-05-21 09:34:21.000000 tooz-6.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-21 09:33:52.000000 tooz-6.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2254 2024-05-21 09:34:21.515914 tooz-6.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-05-21 09:33:52.000000 tooz-6.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-05-21 09:33:52.000000 tooz-6.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/compatibility.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6890 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/doc/source/user/tutorial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/coordinator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/group_membership.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/hashring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/leader_election.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/lock.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-05-21 09:33:52.000000 tooz-6.2.0/doc/source/user/tutorial/partitioner.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/coordinator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/coordinator_heartbeat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/group_membership.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/group_membership_watch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/leader_election.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/lock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2024-05-21 09:33:52.000000 tooz-6.2.0/examples/partitioner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.503914 tooz-6.2.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-05-21 09:33:52.000000 tooz-6.2.0/playbooks/stop-redis.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.495914 tooz-6.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.507914 tooz-6.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/add-consul-acl-support-2f0869681129f7e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/bug-2012226-67752e8cae8489ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/bug-2056656-f71dca8a61138f95.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/consul-heartbeat-support-3ec69e2ace537dc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/deprecate-etcd3-driver-551608037d79222b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/deprecate-zake-driver-eee8fcdfc5a88907.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/etcd-3.4-eee8300c942a1263.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/etcd3-etcd3gw-tls-support-618ab207706e67af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/etcd3-group-support-b039cf19f4a268a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/etcd3gw-api-version-discovery-3e9943c73fae48d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/etcd3gw-group-support-598832a8764a8aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/etcd3gw_create_new_lease_if_expired_during_refresh-1d631d36c21ea28c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/fix-redis-socket_keepalive-type-32b41b746f426efb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/hashring-0470f9119ef63d49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/partitioner-4005767d287dc7c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/redis-health-check-f5e3cb15dd3ac90c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/redis-username-9c552b61db4cfbec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/remove-etcd3-driver-dbce7649a08036c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/remove-strict-redis-555f0f4e369480e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/sentinel-ssl-and-auth-5cccced6685099b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.511914 tooz-6.2.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.511914 tooz-6.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.511914 tooz-6.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-21 09:33:52.000000 tooz-6.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2024-05-21 09:33:52.000000 tooz-6.2.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2024-05-21 09:33:52.000000 tooz-6.2.0/run-examples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2024-05-21 09:33:52.000000 tooz-6.2.0/run-tests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1167 2024-05-21 09:33:52.000000 tooz-6.2.0/setup-consul-env.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      725 2024-05-21 09:33:52.000000 tooz-6.2.0/setup-etcd-env.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2024-05-21 09:34:21.515914 tooz-6.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-05-21 09:33:52.000000 tooz-6.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-05-21 09:33:52.000000 tooz-6.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.511914 tooz-6.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2024-05-21 09:33:52.000000 tooz-6.2.0/tools/compat-matrix.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.511914 tooz-6.2.0/tooz/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31903 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/coordination.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.515914 tooz-6.2.0/tooz/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20676 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/consul.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9415 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/etcd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15786 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20581 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8685 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/ipc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20371 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/memcached.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/mysql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8171 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/pgsql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31981 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2431 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/zake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24765 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/drivers/zookeeper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3932 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/partitioner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.515914 tooz-6.2.0/tooz/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2550 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.515914 tooz-6.2.0/tooz/tests/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/test_etcd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2926 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/test_etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/test_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/test_memcache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4034 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/test_mysql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4061 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/drivers/test_postgresql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40879 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/test_coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/test_hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/test_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7922 2024-05-21 09:33:52.000000 tooz-6.2.0/tooz/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-21 09:34:21.511914 tooz-6.2.0/tooz.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2254 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4242 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2024-05-21 09:34:21.000000 tooz-6.2.0/tooz.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2454 2024-05-21 09:33:52.000000 tooz-6.2.0/tox.ini
```

### Comparing `tooz-6.1.0/.pre-commit-config.yaml` & `tooz-6.2.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-# We from the Oslo project decided to pin repos based on the
-# commit hash instead of the version tag to prevend arbitrary
-# code from running in developer's machines.  To update to a
-# newer version, run `pre-commit autoupdate` and then replace
-# the newer versions with their commit hash.
-
-default_language_version:
-  python: python3
-
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: 9136088a246768144165fcc3ecc3d31bb686920a # v3.3.0
+    rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       # Replaces or checks mixed line ending
       - id: mixed-line-ending
         args: ['--fix', 'lf']
         exclude: '.*\.(svg)$'
       # Forbid files which have a UTF-8 byte-order marker
@@ -23,17 +14,17 @@
       # Check for files that contain merge conflict strings.
       - id: check-merge-conflict
       # Check for debugger imports and py37+ breakpoint()
       # calls in python source
       - id: debug-statements
       - id: check-yaml
         files: .*\.(yaml|yml)$
-  - repo: local
+  - repo: https://opendev.org/openstack/hacking
+    rev: 6.1.0
     hooks:
-      - id: flake8
-        name: flake8
-        additional_dependencies:
-          - hacking>=6.1.0,<6.2.0
-        language: python
-        entry: flake8
-        files: '^.*\.py$'
+      - id: hacking
+        additional_dependencies: []
         exclude: '^(doc|releasenotes|tools)/.*$'
+  - repo: https://github.com/PyCQA/doc8
+    rev: v1.1.1
+    hooks:
+      - id: doc8
```

### Comparing `tooz-6.1.0/.zuul.yaml` & `tooz-6.2.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/AUTHORS` & `tooz-6.2.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Bob.Haddleton <bob.haddleton@nokia.com>
 Cao Xuan Hoang <hoangcx@vn.fujitsu.com>
 ChangBo Guo(gcb) <eric.guo@easystack.cn>
 Chris Dent <chdent@redhat.com>
 Christian Rohmann <christian.rohmann@inovex.de>
 Corey Bryant <corey.bryant@canonical.com>
 Daniel Bengtsson <dbengt@redhat.com>
+Daniel Porter <dporter@proofpoint.com>
 Davanum Srinivas <davanum@gmail.com>
 Davanum Srinivas <dims@linux.vnet.ibm.com>
 Dina Belova <dbelova@mirantis.com>
 Dirk Mueller <dirk@dmllr.de>
 Dmitriy Rabotjagov <dmitriy.r@sitevalley.com>
 Dmitriy Rabotyagov <dmitriy.rabotyagov@citynetwork.eu>
 Dmitriy Rabotyagov <noonedeadpunk@ya.ru>
```

### Comparing `tooz-6.1.0/CONTRIBUTING.rst` & `tooz-6.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/ChangeLog` & `tooz-6.2.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 CHANGES
 =======
 
+6.2.0
+-----
+
+* Loose lower bound of packaging library version
+* fix: correctly pass ssl\_ca\_certs to sentinel when enabled
+* Remove old excludes
+* pre-commit: Bump version, add doc8
+* Remove unnecessary dependencies
+* Remove use of distutils
+
 6.1.0
 -----
 
 * Make authentication/SSL for redis sentinel optional
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
 
 6.0.1
 -----
 
 * Fix sentinel tests not running
 * Fix broken redis sentinel support
```

### Comparing `tooz-6.1.0/LICENSE` & `tooz-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/PKG-INFO` & `tooz-6.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooz
-Version: 6.1.0
+Version: 6.2.0
 Summary: Coordination library for distributed systems.
 Home-page: https://docs.openstack.org/tooz/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Tooz
         ====
```

### Comparing `tooz-6.1.0/README.rst` & `tooz-6.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/requirements.txt` & `tooz-6.2.0/doc/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-sphinx>=2.0.0,!=2.1.0 # BSD
+sphinx>=2.0.0 # BSD
 openstackdocstheme>=2.2.1 # Apache-2.0
 reno>=3.1.0 # Apache-2.0
 
 # Install dependencies for tooz so that autodoc works.
 ## consul
 python-consul2>=0.0.16 # MIT License
 ## etcd
 requests>=2.10.0 # Apache-2.0
 ## etcd3gw
-etcd3gw!=0.2.6,>=0.1.0 # Apache-2.0
+etcd3gw>=0.1.0 # Apache-2.0
 ## zake
 zake>=0.1.6 # Apache-2.0
 ## redis
 redis>=3.1.0 # MIT
 ## postgresql
 psycopg2>=2.5 # LGPL/ZPL
 ## mysql
 PyMySQL>=0.6.2 # MIT License
 ## zookeeper
 kazoo>=2.2 # Apache-2.0
 ## memcached
-pymemcache!=1.3.0,>=1.2.9 # Apache 2.0 License
+pymemcache>=1.2.9 # Apache 2.0 License
 ## ipc
 sysv-ipc>=0.6.8 # BSD License
```

### Comparing `tooz-6.1.0/doc/source/conf.py` & `tooz-6.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/index.rst` & `tooz-6.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/install/index.rst` & `tooz-6.2.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/reference/index.rst` & `tooz-6.2.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/user/compatibility.rst` & `tooz-6.2.0/doc/source/user/compatibility.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/user/drivers.rst` & `tooz-6.2.0/doc/source/user/drivers.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/user/tutorial/coordinator.rst` & `tooz-6.2.0/doc/source/user/tutorial/coordinator.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/user/tutorial/group_membership.rst` & `tooz-6.2.0/doc/source/user/tutorial/group_membership.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/user/tutorial/leader_election.rst` & `tooz-6.2.0/doc/source/user/tutorial/leader_election.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/doc/source/user/tutorial/lock.rst` & `tooz-6.2.0/doc/source/user/tutorial/lock.rst`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/coordinator.py` & `tooz-6.2.0/examples/coordinator.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/coordinator_heartbeat.py` & `tooz-6.2.0/examples/coordinator_heartbeat.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/group_membership.py` & `tooz-6.2.0/examples/group_membership.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/group_membership_watch.py` & `tooz-6.2.0/examples/group_membership_watch.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/hashring.py` & `tooz-6.2.0/examples/hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/leader_election.py` & `tooz-6.2.0/examples/leader_election.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/lock.py` & `tooz-6.2.0/examples/lock.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/examples/partitioner.py` & `tooz-6.2.0/examples/partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/releasenotes/notes/bug-2056656-f71dca8a61138f95.yaml` & `tooz-6.2.0/releasenotes/notes/bug-2056656-f71dca8a61138f95.yaml`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/releasenotes/notes/etcd3gw-api-version-discovery-3e9943c73fae48d4.yaml` & `tooz-6.2.0/releasenotes/notes/etcd3gw-api-version-discovery-3e9943c73fae48d4.yaml`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml` & `tooz-6.2.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml` & `tooz-6.2.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/releasenotes/source/conf.py` & `tooz-6.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/setup-consul-env.sh` & `tooz-6.2.0/setup-consul-env.sh`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/setup-etcd-env.sh` & `tooz-6.2.0/setup-etcd-env.sh`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/setup.cfg` & `tooz-6.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -45,27 +45,28 @@
 
 [extras]
 consul = 
 	python-consul2>=0.0.16 # MIT License
 etcd = 
 	requests>=2.10.0 # Apache-2.0
 etcd3gw = 
-	etcd3gw!=0.2.6,>=2.3.0 # Apache-2.0
+	etcd3gw>=2.3.0 # Apache-2.0
 zake = 
 	zake>=0.1.6 # Apache-2.0
 redis = 
 	redis>=4.0.0 # MIT
+	packaging>=20.4.0 # Apache-2.0
 postgresql = 
 	psycopg2>=2.5 # LGPL/ZPL
 mysql = 
 	PyMySQL>=0.6.2 # MIT License
 zookeeper = 
 	kazoo>=2.6 # Apache-2.0
 memcached = 
-	pymemcache!=1.3.0,>=1.2.9 # Apache 2.0 License
+	pymemcache>=1.2.9 # Apache 2.0 License
 ipc = 
 	sysv-ipc>=0.6.8 # BSD License
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tooz-6.1.0/setup.py` & `tooz-6.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tools/compat-matrix.py` & `tooz-6.2.0/tools/compat-matrix.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/__init__.py` & `tooz-6.2.0/tooz/__init__.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/_retry.py` & `tooz-6.2.0/tooz/_retry.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/coordination.py` & `tooz-6.2.0/tooz/coordination.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/consul.py` & `tooz-6.2.0/tooz/drivers/consul.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/etcd.py` & `tooz-6.2.0/tooz/drivers/etcd.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/etcd3gw.py` & `tooz-6.2.0/tooz/drivers/etcd3gw.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/file.py` & `tooz-6.2.0/tooz/drivers/file.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/ipc.py` & `tooz-6.2.0/tooz/drivers/ipc.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/memcached.py` & `tooz-6.2.0/tooz/drivers/memcached.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/mysql.py` & `tooz-6.2.0/tooz/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/pgsql.py` & `tooz-6.2.0/tooz/drivers/pgsql.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/redis.py` & `tooz-6.2.0/tooz/drivers/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from distutils import version
 import functools
 import logging
 import re
 import string
 import threading
 
 from oslo_utils import encodeutils
 from oslo_utils import strutils
+from packaging import version
 import redis
 from redis import exceptions
 from redis import sentinel
 
 import tooz
 from tooz import coordination
 from tooz import locking
@@ -215,15 +215,15 @@
         coordination.Characteristics.CAUSAL,
     )
     """
     Tuple of :py:class:`~tooz.coordination.Characteristics` introspectable
     enum member(s) that can be used to interogate how this driver works.
     """
 
-    MIN_VERSION = version.LooseVersion("2.6.0")
+    MIN_VERSION = version.Version("2.6.0")
     """
     The min redis version that this driver requires to operate with...
     """
 
     GROUP_EXISTS = b'__created__'
     """
     Redis deletes dictionaries that have no keys in them, which means the
@@ -391,22 +391,21 @@
         self._acquired_locks = set()
         self._started = False
         self._server_info = {}
         self._scripts = {}
 
     def _check_fetch_redis_version(self, geq_version, not_existent=True):
         if isinstance(geq_version, str):
-            desired_version = version.LooseVersion(geq_version)
-        elif isinstance(geq_version, version.LooseVersion):
+            desired_version = version.Version(geq_version)
+        elif isinstance(geq_version, version.Version):
             desired_version = geq_version
         else:
             raise TypeError("Version check expects a string/version type")
         try:
-            redis_version = version.LooseVersion(
-                self._server_info['redis_version'])
+            redis_version = version.Version(self._server_info['redis_version'])
         except KeyError:
             return (not_existent, None)
         else:
             if redis_version < desired_version:
                 return (False, redis_version)
             else:
                 return (True, redis_version)
@@ -482,15 +481,15 @@
             # NOTE(tkajinam): Copy socket_* options, according to the logic
             # in redis-py
             for key in kwargs:
                 if key.startswith('socket_'):
                     sentinel_kwargs[key] = kwargs[key]
             if kwargs.pop('sentinel_ssl', False):
                 sentinel_kwargs['ssl'] = True
-                for key in ('ssl_certfile', 'ssl_keyfile', 'ssl_cafile'):
+                for key in ('ssl_certfile', 'ssl_keyfile', 'ssl_ca_certs'):
                     if key in kwargs:
                         sentinel_kwargs[key] = kwargs[key]
             for key in ('username', 'password'):
                 if 'sentinel_' + key in kwargs:
                     sentinel_kwargs[key] = kwargs.pop('sentinel_' + key)
             sentinel_server = sentinel.Sentinel(
                 sentinel_hosts,
```

### Comparing `tooz-6.1.0/tooz/drivers/zake.py` & `tooz-6.2.0/tooz/drivers/zake.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/drivers/zookeeper.py` & `tooz-6.2.0/tooz/drivers/zookeeper.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/hashring.py` & `tooz-6.2.0/tooz/hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/locking.py` & `tooz-6.2.0/tooz/locking.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/partitioner.py` & `tooz-6.2.0/tooz/partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/__init__.py` & `tooz-6.2.0/tooz/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/drivers/test_etcd.py` & `tooz-6.2.0/tooz/tests/drivers/test_etcd.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/drivers/test_etcd3gw.py` & `tooz-6.2.0/tooz/tests/drivers/test_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/drivers/test_file.py` & `tooz-6.2.0/tooz/tests/drivers/test_file.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/drivers/test_memcache.py` & `tooz-6.2.0/tooz/tests/drivers/test_memcache.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/drivers/test_mysql.py` & `tooz-6.2.0/tooz/tests/drivers/test_mysql.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/drivers/test_postgresql.py` & `tooz-6.2.0/tooz/tests/drivers/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/test_coordination.py` & `tooz-6.2.0/tooz/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/test_hashring.py` & `tooz-6.2.0/tooz/tests/test_hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/test_partitioner.py` & `tooz-6.2.0/tooz/tests/test_partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/tests/test_utils.py` & `tooz-6.2.0/tooz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz/utils.py` & `tooz-6.2.0/tooz/utils.py`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz.egg-info/PKG-INFO` & `tooz-6.2.0/tooz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooz
-Version: 6.1.0
+Version: 6.2.0
 Summary: Coordination library for distributed systems.
 Home-page: https://docs.openstack.org/tooz/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Tooz
         ====
```

### Comparing `tooz-6.1.0/tooz.egg-info/SOURCES.txt` & `tooz-6.2.0/tooz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tooz.egg-info/entry_points.txt` & `tooz-6.2.0/tooz.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tooz-6.1.0/tox.ini` & `tooz-6.2.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,18 @@
 [testenv:docs]
 setenv = {[testenv]setenv}
     PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python
 deps = -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pep8]
-deps = hacking>=4.0.0,<4.1.0
-      doc8
-      pre-commit>=2.6.0
+deps =
+    pre-commit
 commands =
-    pre-commit run -a
-    doc8 doc/source
+    pre-commit run --all-files --show-diff-on-failure
 
 [flake8]
 exclude=.venv,.git,.tox,dist,*egg,*.egg-info,build,examples,doc
 show-source = True
 
 [testenv:releasenotes]
 deps = -r{toxinidir}/doc/requirements.txt
```

