# Comparing `tmp/fsl_sub_plugin_slurm-1.6.2.tar.gz` & `tmp/fsl_sub_plugin_slurm-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsl_sub_plugin_slurm-1.6.2.tar", last modified: Fri Feb  9 17:58:44 2024, max compression
+gzip compressed data, was "fsl_sub_plugin_slurm-1.6.3.tar", last modified: Tue May 21 11:53:10 2024, max compression
```

## Comparing `fsl_sub_plugin_slurm-1.6.2.tar` & `fsl_sub_plugin_slurm-1.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 17:58:44.124568 fsl_sub_plugin_slurm-1.6.2/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-03-31 13:44:00.000000 fsl_sub_plugin_slurm-1.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14004 2024-02-09 17:58:44.124568 fsl_sub_plugin_slurm-1.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12774 2023-05-23 16:36:45.000000 fsl_sub_plugin_slurm-1.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 17:58:44.106568 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/
--rw-rw-rw-   0 root         (0) root         (0)    42503 2023-07-19 15:29:25.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3495 2023-05-23 16:36:45.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/fsl_sub_slurm.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 17:58:44.107568 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-09 17:58:34.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    64932 2023-06-21 08:15:11.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-19 15:29:25.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-09 17:58:44.106568 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14004 2024-02-09 17:58:43.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2024-02-09 17:58:44.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-09 17:58:43.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-02-09 17:58:43.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-09 17:58:43.000000 fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-09 17:58:44.124568 fsl_sub_plugin_slurm-1.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1921 2023-03-31 13:44:00.000000 fsl_sub_plugin_slurm-1.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 11:53:10.778829 fsl_sub_plugin_slurm-1.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14466 2024-05-21 11:53:10.778829 fsl_sub_plugin_slurm-1.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13120 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 11:53:10.776829 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/
+-rw-rw-rw-   0 root         (0) root         (0)    42758 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/fsl_sub_slurm.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 11:53:10.777829 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    65906 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 11:53:10.777829 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14466 2024-05-21 11:53:10.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-21 11:53:10.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 11:53:10.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-21 11:53:10.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-21 11:53:10.000000 fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 11:53:10.778829 fsl_sub_plugin_slurm-1.6.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-05-21 11:53:00.000000 fsl_sub_plugin_slurm-1.6.3/setup.py
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/LICENSE` & `fsl_sub_plugin_slurm-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fsl_sub_plugin_slurm-1.6.2/PKG-INFO` & `fsl_sub_plugin_slurm-1.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsl_sub_plugin_slurm
-Version: 1.6.2
+Version: 1.6.3
 Summary: FSL Cluster Submission Plugin for Slurm
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
 Author: Duncan Mortimer
 Author-email: duncan.mortimer@ndcn.ox.ac.uk
 License: Apache License Version 2.0
 Project-URL: Documentation, https://fsl.fmrib.ox.ac.uk/fsl/fslwiki
 Project-URL: Source, https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
@@ -14,97 +14,101 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: fsl_sub>=2.8.0
+Requires-Dist: ruamel.yaml>=0.16.7
 
-# fsl_sub_plugin_slurm
+# fsl\_sub\_plugin\_slurm
 
 Job submission to SLURM variant cluster queues.
 
 _Copyright 2018-2023 University of Oxford, Oxford, UK._
 
 ## Introduction
 
 fsl\_sub provides a consistent interface to various cluster backends, with a fall back to running tasks locally where no cluster is available.
 This fsl\_sub plugin provides support for submitting tasks to SLURM clusters.
 
-For installation instructions please see INSTALL.md; for building packages see BUILD.md.
+For installation instructions please see `INSTALL.md`; for building packages see `BUILD.md`.
 
 ## Configuration
 
 Use the command:
 
 > fsl_sub_config slurm > fsl_sub.yml
 
 to generate an example configuration, including queue definitions gleaned from the SLURM software - check these, paying attention to any warnings generated.
 
-Use the fsl_sub.yml file as per the main fsl_sub documentation.
+Use the `fsl_sub.yml` file as per the main fsl\_sub documentation.
 
 The configuration for the SLURM plugin is in the _method\_opts_ section, under the key _slurm_.
 
 ### Method options
 
 | Key | Values (default/recommended in bold) | Description |
 | ----|--------|-------------|
-| queues | **True** | Does this method use queues/partitions (should be always be True) |
-| memory\_in\_gb | True/**False** | Whether SLURM reports memory in GB - normally false |
-| copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell
-| has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false
-| script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True.
-| mail\_support | True/**False** | Whether the grid installation is configured to send email on job events.
-| mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited.
-| mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default
-| notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true.
-| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
-| array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1.
-| array\_limit | **True**/False | Enable limiting number of concurrent array tasks.
-| job\_resources | **True**/False | Enable additional job resource specification support.
-| projects | **True**/False | Enable support for projects typically used auditing/charging purposes.
-| preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules.
-| add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True.
-| export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node
-| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`.
-| extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler.
-| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0").
+| queues | **True** | Does this method use queues/partitions (should be always be True). |
+| memory\_in\_gb | True/**False** | Whether SLURM reports memory in GB - normally false. |
+| copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell. |
+| has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false. |
+| script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True. |
+| mail\_support | True/**False** | Whether the grid installation is configured to send email on job events. |
+| mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited. |
+| mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default. |
+| notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true. |
+| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True'). |
+| array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1. |
+| array\_limit | **True**/False | Enable limiting number of concurrent array tasks. |
+| job\_resources | **True**/False | Enable additional job resource specification support. |
+| projects | **True**/False | Enable support for projects typically used auditing/charging purposes. |
+| preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules. |
+| add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True. |
+| export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node. |
+| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`. |
+| extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler. |
+| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0"). |
+| allow_nested_queuing | True/**False** | Whether fsl_sub, when called from within a cluster job, should be able to submit further jobs (True) or run subsequent jobs with the shell plugin. You can override this on a per-job or session basis using the environmet |
 
 ### Coprocessor Configuration
 
 This plugin is not capable of automatically determining all the necessary information to configure your co-processors but will advise of the information it can find and propose queue definitions for these GPU resources.
 
 SLURM typically selects GPU resources with a GRES (Generic RESource) that defines the type and quantity of the co-processor. Where multiple classes of co-processor are available this might be selectable via the GRES or you may need to provide a _constraint_. If you would like to be able to support running on a class and all superior devices you need to be able to use constraints as GRES requests do not support logical combinations. The automatically generated configuration should include useful information about your GRES and constraints, but should you wish to obtain this information yourself use the commands:
 
 * `sinfo -p <partition> -o %G` - This will list all the GRES defined on \<partition>.
 * `sinfo -p <partition> -o %f` - This will list all features selectable by a `--constraint` as a comma-separated list.
 
 Typically CUDA resources will be controlled using GRES or constraints with _gpu_ in the name, so look for these.
 
-For each coprocessor hardware type you need a sub-section given an identifier than will be used to request this type of coprocessor. For CUDA processors this sub-section *must* be called 'cuda' to ensure that FSL tools can auto-detect and use CUDA hardware/queues.
+For each coprocessor hardware type you need a sub-section given an identifier than will be used to request this type of coprocessor. For CUDA processors this sub-section **must** be called 'cuda' to ensure that FSL tools can auto-detect and use CUDA hardware/queues.
 
 | Key | Values (default/recommended in bold) | Description |
 | ----|--------|-------------|
 | resource| String | GRES that, when requested, selects machines with the hardware present, e.g. _gpu_. |
 | classes | True/**False** | Whether more than one type of this co-processor is available |
 | include\_more\_capable | **True**/False | Whether to automatically request all classes that are more capable than the requested class. This requires the _class\_constraints_ option to be set to True and for your SLURM cluster to be set up with GPU features/constraints |
 | class\_types | Configuration dictionary | This contains the definition of the GPU classes... |
 | | _Key_ | |
-| | class selector | This is the letter (or word) that is used to select this class of co-processor from the fsl\_sub commandline. For CUDA devices you may consider using the card name e.g. A100.|
-| | resource | This is the name of the SLURM GRES 'type' or contraint that will be used to select this GPU family.
-| | doc | The description that appears in the fsl\_sub help text about this device.
-| | capability | An integer defining the feature set of the device, your most basic device should be given the value 1 and more capable devices higher values, e.g. GTX = 1, Kelper = 2, Pascal = 3, Volta = 4.
-| default\_class | _Class type key_ | The _class selector_ for the class to assign jobs to where a class has not been specified in the fsl\_sub call. For FSL tools that automatically submit to CUDA queues you should aim to select one that has good double-precision performance (K40|80, P100, V100, A100) and ensure all higher capability devices also have good double-precision.
+| | class selector | This is the letter (or word) that is used to select this class of co-processor from the fsl\_sub commandline. For CUDA devices you may consider using the card name e.g. A100. |
+| | resource | This is the name of the SLURM GRES 'type' or contraint that will be used to select this GPU family. |
+| | doc | The description that appears in the fsl\_sub help text about this device. |
+| | capability | An integer defining the feature set of the device, your most basic device should be given the value 1 and more capable devices higher values, e.g. GTX = 1, Kelper = 2, Pascal = 3, Volta = 4. |
+| default\_class | _Class type key_ | The _class selector_ for the class to assign jobs to where a class has not been specified in the fsl\_sub call. For FSL tools that automatically submit to CUDA queues you should aim to select one that has good double-precision performance (K40\|80, P100, V100, A100) and ensure all higher capability devices also have good double-precision. |
 | class\_constraint | **False**/string | Whether your SLURM cluster is configured to use constraints to select co-processor models/features. If so this should be set to the name of the feature that selects between the models and the co-processor class _resource_ strings set appropriately to match the available values. |
 | presence\_test | _Program path_ (**nvidia-smi** for CUDA) | The name of a program that can be used to look for this coprocessor type, for example nvidia-smi for CUDA devices. Program needs to return non-zero exit status if there are no available coprocessors. |
 
 ### Queue Definitions
 
 Slurm refers to queues as partitions. The example configuration should contain definitions for the automatically discovered partitions but you should review these, in particular any warnings generated.
 To query SLURM for queue information you can use the following SLURM commands.
@@ -115,27 +119,27 @@
 
 Then the details for a queue can be obtained with:
 
 > sinfo -p _partitionname_ -O 'CPUs,MaxCPUsPerNode,Memory,Time,NodeHost'
 
 This will return details for every node within that partition. The queue definition should then be setup as follows:
 
-| Key | Value type | Description
+| Key | Value type | Description |
 |-----|------------|-------------|
-| time | integer in minutes | The _TIMELIMIT_ column reports in days-hours:minutes:seconds, this needs converting to minutes. Provide the maximum value observed, but if there are multiple values you should consider enabling job time notification so that SLURM can select the correct node.||
-| max\_size | integer in GB | This is the maximum permitted memory on a node. This is usually reported by SLURM in MB, so for example 63000 should be configured as 63 (GB). It is equal to the maximum _MEMORY_ value reported. Once again, if there are multiple node types you should turn on RAM nofitication so that nodes can be correctly selected.
-| max\_slots | _CPU_ contains the number of CPUs (threads) available on each node. Set this option to the maximum number reported. |
+| time | integer in minutes | The _TIMELIMIT_ column reports in days-hours:minutes:seconds, this needs converting to minutes. Provide the maximum value observed, but if there are multiple values you should consider enabling job time notification so that SLURM can select the correct node. |
+| max\_size | integer in GB | This is the maximum permitted memory on a node. This is usually reported by SLURM in MB, so for example 63000 should be configured as 63 (GB). It is equal to the maximum _MEMORY_ value reported. Once again, if there are multiple node types you should turn on RAM nofitication so that nodes can be correctly selected. |
+| max\_slots | integer | _CPU_ contains the number of CPUs (threads) available on each node. Set this option to the maximum number reported. |
 | slot\_size | **Null**/integer in GB | This is largely meaningless on SLURM and left at None. If you find that you need to get fsl\_sub to split your job into multiple threads to achieve your memory requirements then set this to the figure provided by your cluster manager. |
 | group | integer | (Optional) All partitions with the same group number will be considered together when scheduling, typically this would be all queues with the same run time but differing memory/core counts. |
 | priority | integer | (Optional) Priority within a group - higher wins. |
 | default | True | Is this the default queue when no time/RAM details provided. |
 | copros | _Co-processor dictionary_ | _Optional_ If this queue has hosts with co-processors (e.g. CUDA devices), then provide this entry, with a key identical to the associated co-processor definition, e.g. _cuda_. |
-| | max\_quantity | An integer representing the maximum number of this coprocessor type available on a single compute node. This can be obtained by looking at the _complexes_ entry of `qconf -se <hostname>` for all of the hosts in this queue. If the complex is _gpu_ then an entry of _gpu=2_ would indicated that this value should be set to 2.
-| | classes | A list of coprocessor classes (as defined in the coprocessor configuration section) that this queue has hardware for.
-| | exclusive | True/**False** | Whether this queue is only used for co-processor requiring tasks. |
+| | max\_quantity | An integer representing the maximum number of this coprocessor type available on a single compute node. This can be obtained by looking at the _complexes_ entry of `qconf -se <hostname>` for all of the hosts in this queue. If the complex is _gpu_ then an entry of _gpu=2_ would indicated that this value should be set to 2. |
+| | classes | A list of coprocessor classes (as defined in the coprocessor configuration section) that this queue has hardware for. |
+| | exclusive | True/**False** - Whether this queue is only used for co-processor requiring tasks. |
 
 Where a partition has obvious GRES or features that define GPUs a proposed GPU configuration will be added as comments to the start of the queue definition. You should review this, create/update the coproc_opts>cuda record with the information in the comments and then this section can be uncommented to enable GPU support.
 
 #### Compound Queues
 
 Some clusters may be configured with multiple variants of the same partition, e.g. short.a, short.b, with each queue having different hardware, perhaps CPU generation or maximum memory or memory available per slot. To maximise scheduling options you can define compound queues which have the configuration of the least capable constituent. To define a compound queue, the queue name (key of the YAML dictionary) should be a comma separated list of queue names (no space).
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/README.md` & `fsl_sub_plugin_slurm-1.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
-# fsl_sub_plugin_slurm
+# fsl\_sub\_plugin\_slurm
 
 Job submission to SLURM variant cluster queues.
 
 _Copyright 2018-2023 University of Oxford, Oxford, UK._
 
 ## Introduction
 
 fsl\_sub provides a consistent interface to various cluster backends, with a fall back to running tasks locally where no cluster is available.
 This fsl\_sub plugin provides support for submitting tasks to SLURM clusters.
 
-For installation instructions please see INSTALL.md; for building packages see BUILD.md.
+For installation instructions please see `INSTALL.md`; for building packages see `BUILD.md`.
 
 ## Configuration
 
 Use the command:
 
 > fsl_sub_config slurm > fsl_sub.yml
 
 to generate an example configuration, including queue definitions gleaned from the SLURM software - check these, paying attention to any warnings generated.
 
-Use the fsl_sub.yml file as per the main fsl_sub documentation.
+Use the `fsl_sub.yml` file as per the main fsl\_sub documentation.
 
 The configuration for the SLURM plugin is in the _method\_opts_ section, under the key _slurm_.
 
 ### Method options
 
 | Key | Values (default/recommended in bold) | Description |
 | ----|--------|-------------|
-| queues | **True** | Does this method use queues/partitions (should be always be True) |
-| memory\_in\_gb | True/**False** | Whether SLURM reports memory in GB - normally false |
-| copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell
-| has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false
-| script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True.
-| mail\_support | True/**False** | Whether the grid installation is configured to send email on job events.
-| mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited.
-| mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default
-| notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true.
-| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
-| array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1.
-| array\_limit | **True**/False | Enable limiting number of concurrent array tasks.
-| job\_resources | **True**/False | Enable additional job resource specification support.
-| projects | **True**/False | Enable support for projects typically used auditing/charging purposes.
-| preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules.
-| add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True.
-| export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node
-| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`.
-| extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler.
-| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0").
+| queues | **True** | Does this method use queues/partitions (should be always be True). |
+| memory\_in\_gb | True/**False** | Whether SLURM reports memory in GB - normally false. |
+| copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell. |
+| has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false. |
+| script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True. |
+| mail\_support | True/**False** | Whether the grid installation is configured to send email on job events. |
+| mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited. |
+| mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default. |
+| notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true. |
+| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True'). |
+| array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1. |
+| array\_limit | **True**/False | Enable limiting number of concurrent array tasks. |
+| job\_resources | **True**/False | Enable additional job resource specification support. |
+| projects | **True**/False | Enable support for projects typically used auditing/charging purposes. |
+| preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules. |
+| add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True. |
+| export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node. |
+| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`. |
+| extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler. |
+| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0"). |
+| allow_nested_queuing | True/**False** | Whether fsl_sub, when called from within a cluster job, should be able to submit further jobs (True) or run subsequent jobs with the shell plugin. You can override this on a per-job or session basis using the environmet |
 
 ### Coprocessor Configuration
 
 This plugin is not capable of automatically determining all the necessary information to configure your co-processors but will advise of the information it can find and propose queue definitions for these GPU resources.
 
 SLURM typically selects GPU resources with a GRES (Generic RESource) that defines the type and quantity of the co-processor. Where multiple classes of co-processor are available this might be selectable via the GRES or you may need to provide a _constraint_. If you would like to be able to support running on a class and all superior devices you need to be able to use constraints as GRES requests do not support logical combinations. The automatically generated configuration should include useful information about your GRES and constraints, but should you wish to obtain this information yourself use the commands:
 
 * `sinfo -p <partition> -o %G` - This will list all the GRES defined on \<partition>.
 * `sinfo -p <partition> -o %f` - This will list all features selectable by a `--constraint` as a comma-separated list.
 
 Typically CUDA resources will be controlled using GRES or constraints with _gpu_ in the name, so look for these.
 
-For each coprocessor hardware type you need a sub-section given an identifier than will be used to request this type of coprocessor. For CUDA processors this sub-section *must* be called 'cuda' to ensure that FSL tools can auto-detect and use CUDA hardware/queues.
+For each coprocessor hardware type you need a sub-section given an identifier than will be used to request this type of coprocessor. For CUDA processors this sub-section **must** be called 'cuda' to ensure that FSL tools can auto-detect and use CUDA hardware/queues.
 
 | Key | Values (default/recommended in bold) | Description |
 | ----|--------|-------------|
 | resource| String | GRES that, when requested, selects machines with the hardware present, e.g. _gpu_. |
 | classes | True/**False** | Whether more than one type of this co-processor is available |
 | include\_more\_capable | **True**/False | Whether to automatically request all classes that are more capable than the requested class. This requires the _class\_constraints_ option to be set to True and for your SLURM cluster to be set up with GPU features/constraints |
 | class\_types | Configuration dictionary | This contains the definition of the GPU classes... |
 | | _Key_ | |
-| | class selector | This is the letter (or word) that is used to select this class of co-processor from the fsl\_sub commandline. For CUDA devices you may consider using the card name e.g. A100.|
-| | resource | This is the name of the SLURM GRES 'type' or contraint that will be used to select this GPU family.
-| | doc | The description that appears in the fsl\_sub help text about this device.
-| | capability | An integer defining the feature set of the device, your most basic device should be given the value 1 and more capable devices higher values, e.g. GTX = 1, Kelper = 2, Pascal = 3, Volta = 4.
-| default\_class | _Class type key_ | The _class selector_ for the class to assign jobs to where a class has not been specified in the fsl\_sub call. For FSL tools that automatically submit to CUDA queues you should aim to select one that has good double-precision performance (K40|80, P100, V100, A100) and ensure all higher capability devices also have good double-precision.
+| | class selector | This is the letter (or word) that is used to select this class of co-processor from the fsl\_sub commandline. For CUDA devices you may consider using the card name e.g. A100. |
+| | resource | This is the name of the SLURM GRES 'type' or contraint that will be used to select this GPU family. |
+| | doc | The description that appears in the fsl\_sub help text about this device. |
+| | capability | An integer defining the feature set of the device, your most basic device should be given the value 1 and more capable devices higher values, e.g. GTX = 1, Kelper = 2, Pascal = 3, Volta = 4. |
+| default\_class | _Class type key_ | The _class selector_ for the class to assign jobs to where a class has not been specified in the fsl\_sub call. For FSL tools that automatically submit to CUDA queues you should aim to select one that has good double-precision performance (K40\|80, P100, V100, A100) and ensure all higher capability devices also have good double-precision. |
 | class\_constraint | **False**/string | Whether your SLURM cluster is configured to use constraints to select co-processor models/features. If so this should be set to the name of the feature that selects between the models and the co-processor class _resource_ strings set appropriately to match the available values. |
 | presence\_test | _Program path_ (**nvidia-smi** for CUDA) | The name of a program that can be used to look for this coprocessor type, for example nvidia-smi for CUDA devices. Program needs to return non-zero exit status if there are no available coprocessors. |
 
 ### Queue Definitions
 
 Slurm refers to queues as partitions. The example configuration should contain definitions for the automatically discovered partitions but you should review these, in particular any warnings generated.
 To query SLURM for queue information you can use the following SLURM commands.
@@ -87,27 +88,27 @@
 
 Then the details for a queue can be obtained with:
 
 > sinfo -p _partitionname_ -O 'CPUs,MaxCPUsPerNode,Memory,Time,NodeHost'
 
 This will return details for every node within that partition. The queue definition should then be setup as follows:
 
-| Key | Value type | Description
+| Key | Value type | Description |
 |-----|------------|-------------|
-| time | integer in minutes | The _TIMELIMIT_ column reports in days-hours:minutes:seconds, this needs converting to minutes. Provide the maximum value observed, but if there are multiple values you should consider enabling job time notification so that SLURM can select the correct node.||
-| max\_size | integer in GB | This is the maximum permitted memory on a node. This is usually reported by SLURM in MB, so for example 63000 should be configured as 63 (GB). It is equal to the maximum _MEMORY_ value reported. Once again, if there are multiple node types you should turn on RAM nofitication so that nodes can be correctly selected.
-| max\_slots | _CPU_ contains the number of CPUs (threads) available on each node. Set this option to the maximum number reported. |
+| time | integer in minutes | The _TIMELIMIT_ column reports in days-hours:minutes:seconds, this needs converting to minutes. Provide the maximum value observed, but if there are multiple values you should consider enabling job time notification so that SLURM can select the correct node. |
+| max\_size | integer in GB | This is the maximum permitted memory on a node. This is usually reported by SLURM in MB, so for example 63000 should be configured as 63 (GB). It is equal to the maximum _MEMORY_ value reported. Once again, if there are multiple node types you should turn on RAM nofitication so that nodes can be correctly selected. |
+| max\_slots | integer | _CPU_ contains the number of CPUs (threads) available on each node. Set this option to the maximum number reported. |
 | slot\_size | **Null**/integer in GB | This is largely meaningless on SLURM and left at None. If you find that you need to get fsl\_sub to split your job into multiple threads to achieve your memory requirements then set this to the figure provided by your cluster manager. |
 | group | integer | (Optional) All partitions with the same group number will be considered together when scheduling, typically this would be all queues with the same run time but differing memory/core counts. |
 | priority | integer | (Optional) Priority within a group - higher wins. |
 | default | True | Is this the default queue when no time/RAM details provided. |
 | copros | _Co-processor dictionary_ | _Optional_ If this queue has hosts with co-processors (e.g. CUDA devices), then provide this entry, with a key identical to the associated co-processor definition, e.g. _cuda_. |
-| | max\_quantity | An integer representing the maximum number of this coprocessor type available on a single compute node. This can be obtained by looking at the _complexes_ entry of `qconf -se <hostname>` for all of the hosts in this queue. If the complex is _gpu_ then an entry of _gpu=2_ would indicated that this value should be set to 2.
-| | classes | A list of coprocessor classes (as defined in the coprocessor configuration section) that this queue has hardware for.
-| | exclusive | True/**False** | Whether this queue is only used for co-processor requiring tasks. |
+| | max\_quantity | An integer representing the maximum number of this coprocessor type available on a single compute node. This can be obtained by looking at the _complexes_ entry of `qconf -se <hostname>` for all of the hosts in this queue. If the complex is _gpu_ then an entry of _gpu=2_ would indicated that this value should be set to 2. |
+| | classes | A list of coprocessor classes (as defined in the coprocessor configuration section) that this queue has hardware for. |
+| | exclusive | True/**False** - Whether this queue is only used for co-processor requiring tasks. |
 
 Where a partition has obvious GRES or features that define GPUs a proposed GPU configuration will be added as comments to the start of the queue definition. You should review this, create/update the coproc_opts>cuda record with the information in the comments and then this section can be uncommented to enable GPU support.
 
 #### Compound Queues
 
 Some clusters may be configured with multiple variants of the same partition, e.g. short.a, short.b, with each queue having different hardware, perhaps CPU generation or maximum memory or memory available per slot. To maximise scheduling options you can define compound queues which have the configuration of the least capable constituent. To define a compound queue, the queue name (key of the YAML dictionary) should be a comma separated list of queue names (no space).
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/__init__.py` & `fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,23 @@
         return True
     else:
         return False
 
 
 def already_queued():
     '''Is this a running SLURM job?'''
-    return ('SLURM_JOB_ID' in os.environ.keys() or 'SLURM_JOBID' in os.environ.keys())
+    mconfig = method_config(METHOD_NAME)
+    allow_nested = True if os.getenv('FSLSUB_NESTED', '0') == '1' else False
+    if allow_nested:
+        return False
+    if mconfig.get('allow_nested_queuing', False):
+        return False
+    return (
+        'SLURM_JOB_ID' in os.environ.keys()
+        or 'SLURM_JOBID' in os.environ.keys())
 
 
 def qdel(job_id):
     '''Deletes a job - returns a tuple, output, return code'''
     scancel = which('scancel')
     if scancel is None:
         raise BadSubmission("Cannot find Slurm software")
@@ -265,15 +273,15 @@
     if command is None:
         raise BadSubmission(
             "Must provide command line or array task file name")
     if not isinstance(command, list):
         raise BadSubmission(
             "Internal error: command argument must be a list"
         )
-    if extra_args is not None and type(extra_args) != list:
+    if extra_args is not None and extra_args is not list:
         raise BadSubmission(
             "Internal error: extra_args should be a list"
         )
 
     # Can't just have export_vars=[] in function definition as the list is mutable so subsequent calls
     # will return the updated list!
     if export_vars is None:
@@ -307,20 +315,20 @@
                 "Command should be a grid submission script (no arguments)")
         keep_jobscript = False
     else:
         if queue is None:
             raise BadSubmission("Queue not specified")
         if job_name is None:
             job_name = command[0]
-        if type(queue) == str:
+        if isinstance(queue, str):
             if ',' in queue:
                 queues = queue.split(',')
             else:
                 queues = [queue, ]
-        elif type(queue) == list:
+        elif isinstance(queue, list):
             queues = queue
         pure_queues = [q.split('@')[0] for q in queues]
 
         gres = []
 
         if not keep_jobscript:
             keep_jobscript = mconf.get('keep_jobscript', False)
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/fsl_sub_slurm.yml` & `fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/fsl_sub_slurm.yml`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,15 @@
     # If your system uses shell modules to configure environment variables then enable
     # this.
     add_module_paths: [] # If preserve_modules is set and you need to add additional
     # folders to the MODULESPATH environment variable in the job's environment then
     # add these paths to this list
     strict_dependencies: False # Do you want to allow subsequent jobs in a pipeline to run even
     # if an earlier job fails - equivalent environment variable FSLSUB_STRICTDEPS (0=False)
+    allow_nested_queuing: False # Do you want fsl_sub to be able to submit to a cluster when already
+    # running in a batch job. See also FSLSUB_NESTED environment variable.
 coproc_opts:
   cuda:
     class_constraint: False # Does the SURLM cluster use constraints to specify GPU types rather than
     # adding it to the GRES? If your cluster instructions say use --constraint (or -C) <class> then set this
     # to true.
     # If you are told to use --gres gpu:<class>:<qty> then set this to false.
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py` & `fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm/tests/test_fsl_sub_plugin_slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         mail_mode: a
         set_time_limit: False
         array_holds: True
         array_limit: True
         preserve_modules: True
         add_module_paths: []
         keep_jobscript: False
+        allow_nested_queuing: False
 copro_opts:
     cuda:
         resource: gpu
         classes: True
         class_resource: gputype
         class_types:
             K:
@@ -72,14 +73,34 @@
 queues:
     a.q:
 ''')
 mconf_dict = conf_dict['method_opts']['slurm']
 
 
 class TestSlurmUtils(unittest.TestCase):
+    @patch(
+        'fsl_sub_plugin_slurm.method_config',
+        return_value=conf_dict['method_opts']['slurm'])
+    def test_already_queued(self, mock_mc):
+
+        with patch.dict(os.environ, {'SLURM_JOB_ID': '1234'}, clear=True):
+            self.assertTrue(fsl_sub_plugin_slurm.already_queued())
+        with patch.dict(os.environ, {'SLURM_JOBID': '1234'}, clear=True):
+            self.assertTrue(fsl_sub_plugin_slurm.already_queued())
+
+        with patch.dict(os.environ, {
+                "FSLSUB_NESTED": "1",
+                "SLURM_JOB_ID": "1234"}, clear=True):
+            self.assertFalse(fsl_sub_plugin_slurm.already_queued())
+        test_cd = copy.deepcopy(conf_dict['method_opts']['slurm'])
+        test_cd['allow_nested_queuing'] = True
+        mock_mc.return_value = test_cd
+        with patch.dict(os.environ, {"SLURM_JOB_ID": "1234"}, clear=True):
+            self.assertFalse(fsl_sub_plugin_slurm.already_queued())
+
     def test__sacct_datetimestamp(self):
         self.assertEqual(
             fsl_sub_plugin_slurm._sacct_datetimestamp('2018-06-04T10:30:30'),
             datetime.datetime(2018, 6, 4, 10, 30, 30)
         )
 
     def test__sacct_timstamp_seconds(self):
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/fsl_sub_plugin_slurm.egg-info/PKG-INFO` & `fsl_sub_plugin_slurm-1.6.3/fsl_sub_plugin_slurm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fsl-sub-plugin-slurm
-Version: 1.6.2
+Name: fsl_sub_plugin_slurm
+Version: 1.6.3
 Summary: FSL Cluster Submission Plugin for Slurm
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
 Author: Duncan Mortimer
 Author-email: duncan.mortimer@ndcn.ox.ac.uk
 License: Apache License Version 2.0
 Project-URL: Documentation, https://fsl.fmrib.ox.ac.uk/fsl/fslwiki
 Project-URL: Source, https://git.fmrib.ox.ac.uk/fsl/fsl_sub_plugin_slurm
@@ -14,97 +14,101 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: fsl_sub>=2.8.0
+Requires-Dist: ruamel.yaml>=0.16.7
 
-# fsl_sub_plugin_slurm
+# fsl\_sub\_plugin\_slurm
 
 Job submission to SLURM variant cluster queues.
 
 _Copyright 2018-2023 University of Oxford, Oxford, UK._
 
 ## Introduction
 
 fsl\_sub provides a consistent interface to various cluster backends, with a fall back to running tasks locally where no cluster is available.
 This fsl\_sub plugin provides support for submitting tasks to SLURM clusters.
 
-For installation instructions please see INSTALL.md; for building packages see BUILD.md.
+For installation instructions please see `INSTALL.md`; for building packages see `BUILD.md`.
 
 ## Configuration
 
 Use the command:
 
 > fsl_sub_config slurm > fsl_sub.yml
 
 to generate an example configuration, including queue definitions gleaned from the SLURM software - check these, paying attention to any warnings generated.
 
-Use the fsl_sub.yml file as per the main fsl_sub documentation.
+Use the `fsl_sub.yml` file as per the main fsl\_sub documentation.
 
 The configuration for the SLURM plugin is in the _method\_opts_ section, under the key _slurm_.
 
 ### Method options
 
 | Key | Values (default/recommended in bold) | Description |
 | ----|--------|-------------|
-| queues | **True** | Does this method use queues/partitions (should be always be True) |
-| memory\_in\_gb | True/**False** | Whether SLURM reports memory in GB - normally false |
-| copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell
-| has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false
-| script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True.
-| mail\_support | True/**False** | Whether the grid installation is configured to send email on job events.
-| mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited.
-| mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default
-| notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true.
-| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True').
-| array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1.
-| array\_limit | **True**/False | Enable limiting number of concurrent array tasks.
-| job\_resources | **True**/False | Enable additional job resource specification support.
-| projects | **True**/False | Enable support for projects typically used auditing/charging purposes.
-| preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules.
-| add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True.
-| export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node
-| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`.
-| extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler.
-| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0").
+| queues | **True** | Does this method use queues/partitions (should be always be True). |
+| memory\_in\_gb | True/**False** | Whether SLURM reports memory in GB - normally false. |
+| copy\_environment | **True**/False | Whether to replicate the environment variables in the shell that called fsl_sub into the job's shell. |
+| has\_parallel_envs | **False**/True | SLURM does not provide parallel environments so this should always be false. |
+| script\_conf | **True**/False | Whether _--usesscript_ option to fsl_sub is available via this method. This option allows you to define the grid options as comments in a shell script and then provide this to the cluster for running. Should be set to True. |
+| mail\_support | True/**False** | Whether the grid installation is configured to send email on job events. |
+| mail\_modes | Dictionary of option lists | If the grid has email notifications turned on, this option configures the submission options for different verbosity levels, 'b' = job start, 'e' = job end, 'a' = job abort, 'f' = all events, 'n' = no mail. Each event type should then have a list of submission mail arguments that will be applied to the submitted job. Typically, these should not be edited. |
+| mail\_mode | b/e/a/f/**n** | Which of the above mail_modes to use by default. |
+| notify\_ram\_usage | **True**/False | Whether to notify SLURM of the RAM you have requested. SLURM is typically configured to give jobs a small RAM allocation so you will invariably need this set to true. |
+| set\_time\_limit | True/**False** | Whether to notify SLURM of the expected **maximum** run-time of your job. This helps the scheduler fill in reserved slots (for e.g. parallel environment jobs), however, this time limit will be enforced, resulting in a job being killed if it is exceeded, even if this is less than the queue run-time limit. This can be disabled on a per-job basis by setting the environment variable FSLSUB_NOTIMELIMIT to '1' (or 'True'). |
+| array\_holds | **True**/False | Enable support array holds, e.g. sub-task 1 waits for parent sub-task 1. |
+| array\_limit | **True**/False | Enable limiting number of concurrent array tasks. |
+| job\_resources | **True**/False | Enable additional job resource specification support. |
+| projects | **True**/False | Enable support for projects typically used auditing/charging purposes. |
+| preseve\_modules | True/**False** | Whether to re-load shell modules on the compute node. Required if you have multiple CPU generations and per-generation optimised libraries configured with modules. |
+| add_module_paths | **[]**/ a list | List of file system paths to search for modules in addition to the system defined ones. Useful if you have your own shell modules directory but need to allow the compute node to auto-set it's MODULEPATH environment variable (e.g. to a architecture specific folder). Only used when preserve_modules is True. |
+| export\_vars | **[]**/List | List of environment variables that should transfered with the job to the compute node. |
+| keep\_jobscript | True/**False** | Whether to preserve the generated wrapper in a file `wrapper_<jobid>.sh`. This file contains sufficient information to resubmit this job in the future. If the job fails to submit, this will be preserved in the file `wrapper_failed_<DD>-<MMM>-<YYYY>_<HH><MM><SS>.sh`. |
+| extra\_args | **[]**/List | List of additional SLURM arguments to pass through to the sheduler. |
+| strict_dependencies | True/**False** | Whether to use 'afterok' (True) or 'afterany' (False) when specifying simple job dependencies. This can also be controlled by the environment variable `FSLSUB_STRICTDEPS` (True="1", False="0"). |
+| allow_nested_queuing | True/**False** | Whether fsl_sub, when called from within a cluster job, should be able to submit further jobs (True) or run subsequent jobs with the shell plugin. You can override this on a per-job or session basis using the environmet |
 
 ### Coprocessor Configuration
 
 This plugin is not capable of automatically determining all the necessary information to configure your co-processors but will advise of the information it can find and propose queue definitions for these GPU resources.
 
 SLURM typically selects GPU resources with a GRES (Generic RESource) that defines the type and quantity of the co-processor. Where multiple classes of co-processor are available this might be selectable via the GRES or you may need to provide a _constraint_. If you would like to be able to support running on a class and all superior devices you need to be able to use constraints as GRES requests do not support logical combinations. The automatically generated configuration should include useful information about your GRES and constraints, but should you wish to obtain this information yourself use the commands:
 
 * `sinfo -p <partition> -o %G` - This will list all the GRES defined on \<partition>.
 * `sinfo -p <partition> -o %f` - This will list all features selectable by a `--constraint` as a comma-separated list.
 
 Typically CUDA resources will be controlled using GRES or constraints with _gpu_ in the name, so look for these.
 
-For each coprocessor hardware type you need a sub-section given an identifier than will be used to request this type of coprocessor. For CUDA processors this sub-section *must* be called 'cuda' to ensure that FSL tools can auto-detect and use CUDA hardware/queues.
+For each coprocessor hardware type you need a sub-section given an identifier than will be used to request this type of coprocessor. For CUDA processors this sub-section **must** be called 'cuda' to ensure that FSL tools can auto-detect and use CUDA hardware/queues.
 
 | Key | Values (default/recommended in bold) | Description |
 | ----|--------|-------------|
 | resource| String | GRES that, when requested, selects machines with the hardware present, e.g. _gpu_. |
 | classes | True/**False** | Whether more than one type of this co-processor is available |
 | include\_more\_capable | **True**/False | Whether to automatically request all classes that are more capable than the requested class. This requires the _class\_constraints_ option to be set to True and for your SLURM cluster to be set up with GPU features/constraints |
 | class\_types | Configuration dictionary | This contains the definition of the GPU classes... |
 | | _Key_ | |
-| | class selector | This is the letter (or word) that is used to select this class of co-processor from the fsl\_sub commandline. For CUDA devices you may consider using the card name e.g. A100.|
-| | resource | This is the name of the SLURM GRES 'type' or contraint that will be used to select this GPU family.
-| | doc | The description that appears in the fsl\_sub help text about this device.
-| | capability | An integer defining the feature set of the device, your most basic device should be given the value 1 and more capable devices higher values, e.g. GTX = 1, Kelper = 2, Pascal = 3, Volta = 4.
-| default\_class | _Class type key_ | The _class selector_ for the class to assign jobs to where a class has not been specified in the fsl\_sub call. For FSL tools that automatically submit to CUDA queues you should aim to select one that has good double-precision performance (K40|80, P100, V100, A100) and ensure all higher capability devices also have good double-precision.
+| | class selector | This is the letter (or word) that is used to select this class of co-processor from the fsl\_sub commandline. For CUDA devices you may consider using the card name e.g. A100. |
+| | resource | This is the name of the SLURM GRES 'type' or contraint that will be used to select this GPU family. |
+| | doc | The description that appears in the fsl\_sub help text about this device. |
+| | capability | An integer defining the feature set of the device, your most basic device should be given the value 1 and more capable devices higher values, e.g. GTX = 1, Kelper = 2, Pascal = 3, Volta = 4. |
+| default\_class | _Class type key_ | The _class selector_ for the class to assign jobs to where a class has not been specified in the fsl\_sub call. For FSL tools that automatically submit to CUDA queues you should aim to select one that has good double-precision performance (K40\|80, P100, V100, A100) and ensure all higher capability devices also have good double-precision. |
 | class\_constraint | **False**/string | Whether your SLURM cluster is configured to use constraints to select co-processor models/features. If so this should be set to the name of the feature that selects between the models and the co-processor class _resource_ strings set appropriately to match the available values. |
 | presence\_test | _Program path_ (**nvidia-smi** for CUDA) | The name of a program that can be used to look for this coprocessor type, for example nvidia-smi for CUDA devices. Program needs to return non-zero exit status if there are no available coprocessors. |
 
 ### Queue Definitions
 
 Slurm refers to queues as partitions. The example configuration should contain definitions for the automatically discovered partitions but you should review these, in particular any warnings generated.
 To query SLURM for queue information you can use the following SLURM commands.
@@ -115,27 +119,27 @@
 
 Then the details for a queue can be obtained with:
 
 > sinfo -p _partitionname_ -O 'CPUs,MaxCPUsPerNode,Memory,Time,NodeHost'
 
 This will return details for every node within that partition. The queue definition should then be setup as follows:
 
-| Key | Value type | Description
+| Key | Value type | Description |
 |-----|------------|-------------|
-| time | integer in minutes | The _TIMELIMIT_ column reports in days-hours:minutes:seconds, this needs converting to minutes. Provide the maximum value observed, but if there are multiple values you should consider enabling job time notification so that SLURM can select the correct node.||
-| max\_size | integer in GB | This is the maximum permitted memory on a node. This is usually reported by SLURM in MB, so for example 63000 should be configured as 63 (GB). It is equal to the maximum _MEMORY_ value reported. Once again, if there are multiple node types you should turn on RAM nofitication so that nodes can be correctly selected.
-| max\_slots | _CPU_ contains the number of CPUs (threads) available on each node. Set this option to the maximum number reported. |
+| time | integer in minutes | The _TIMELIMIT_ column reports in days-hours:minutes:seconds, this needs converting to minutes. Provide the maximum value observed, but if there are multiple values you should consider enabling job time notification so that SLURM can select the correct node. |
+| max\_size | integer in GB | This is the maximum permitted memory on a node. This is usually reported by SLURM in MB, so for example 63000 should be configured as 63 (GB). It is equal to the maximum _MEMORY_ value reported. Once again, if there are multiple node types you should turn on RAM nofitication so that nodes can be correctly selected. |
+| max\_slots | integer | _CPU_ contains the number of CPUs (threads) available on each node. Set this option to the maximum number reported. |
 | slot\_size | **Null**/integer in GB | This is largely meaningless on SLURM and left at None. If you find that you need to get fsl\_sub to split your job into multiple threads to achieve your memory requirements then set this to the figure provided by your cluster manager. |
 | group | integer | (Optional) All partitions with the same group number will be considered together when scheduling, typically this would be all queues with the same run time but differing memory/core counts. |
 | priority | integer | (Optional) Priority within a group - higher wins. |
 | default | True | Is this the default queue when no time/RAM details provided. |
 | copros | _Co-processor dictionary_ | _Optional_ If this queue has hosts with co-processors (e.g. CUDA devices), then provide this entry, with a key identical to the associated co-processor definition, e.g. _cuda_. |
-| | max\_quantity | An integer representing the maximum number of this coprocessor type available on a single compute node. This can be obtained by looking at the _complexes_ entry of `qconf -se <hostname>` for all of the hosts in this queue. If the complex is _gpu_ then an entry of _gpu=2_ would indicated that this value should be set to 2.
-| | classes | A list of coprocessor classes (as defined in the coprocessor configuration section) that this queue has hardware for.
-| | exclusive | True/**False** | Whether this queue is only used for co-processor requiring tasks. |
+| | max\_quantity | An integer representing the maximum number of this coprocessor type available on a single compute node. This can be obtained by looking at the _complexes_ entry of `qconf -se <hostname>` for all of the hosts in this queue. If the complex is _gpu_ then an entry of _gpu=2_ would indicated that this value should be set to 2. |
+| | classes | A list of coprocessor classes (as defined in the coprocessor configuration section) that this queue has hardware for. |
+| | exclusive | True/**False** - Whether this queue is only used for co-processor requiring tasks. |
 
 Where a partition has obvious GRES or features that define GPUs a proposed GPU configuration will be added as comments to the start of the queue definition. You should review this, create/update the coproc_opts>cuda record with the information in the comments and then this section can be uncommented to enable GPU support.
 
 #### Compound Queues
 
 Some clusters may be configured with multiple variants of the same partition, e.g. short.a, short.b, with each queue having different hardware, perhaps CPU generation or maximum memory or memory available per slot. To maximise scheduling options you can define compound queues which have the configuration of the least capable constituent. To define a compound queue, the queue name (key of the YAML dictionary) should be a comma separated list of queue names (no space).
```

### Comparing `fsl_sub_plugin_slurm-1.6.2/setup.py` & `fsl_sub_plugin_slurm-1.6.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Natural Language :: English',
         'Environment :: Console',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
     ],
     keywords='FSL fsl Neuroimaging neuroimaging cluster'
              ' grid slurm',
```

