# Comparing `tmp/cxxbuild-1.6.2.tar.gz` & `tmp/cxxbuild-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxxbuild-1.6.2.tar", last modified: Mon May 20 03:06:17 2024, max compression
+gzip compressed data, was "cxxbuild-1.6.3.tar", last modified: Tue May 21 14:54:31 2024, max compression
```

## Comparing `cxxbuild-1.6.2.tar` & `cxxbuild-1.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-20 03:06:17.815592 cxxbuild-1.6.2/
--rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14973 2024-05-20 03:06:17.815592 cxxbuild-1.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12912 2024-05-20 03:05:46.000000 cxxbuild-1.6.2/README.md
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-20 03:06:17.811592 cxxbuild-1.6.2/cxxbuild/
--rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.2/cxxbuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51317 2024-05-20 03:05:46.000000 cxxbuild-1.6.2/cxxbuild/cxxbuild.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-20 03:06:17.815592 cxxbuild-1.6.2/cxxbuild.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14973 2024-05-20 03:06:17.000000 cxxbuild-1.6.2/cxxbuild.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2024-05-20 03:06:17.000000 cxxbuild-1.6.2/cxxbuild.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 03:06:17.000000 cxxbuild-1.6.2/cxxbuild.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-20 03:06:17.000000 cxxbuild-1.6.2/cxxbuild.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-20 03:06:17.000000 cxxbuild-1.6.2/cxxbuild.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 03:06:17.000000 cxxbuild-1.6.2/cxxbuild.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      923 2024-05-20 03:05:46.000000 cxxbuild-1.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 03:06:17.815592 cxxbuild-1.6.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      227 2024-05-20 03:05:46.000000 cxxbuild-1.6.2/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:31.137412 cxxbuild-1.6.3/
+-rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14991 2024-05-21 14:54:31.137412 cxxbuild-1.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12930 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/README.md
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:31.129412 cxxbuild-1.6.3/cxxbuild/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.3/cxxbuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54411 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/cxxbuild/cxxbuild.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:31.133412 cxxbuild-1.6.3/cxxbuild.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14991 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      923 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 14:54:31.137412 cxxbuild-1.6.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      227 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/setup.py
```

### Comparing `cxxbuild-1.6.2/LICENSE` & `cxxbuild-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cxxbuild-1.6.2/PKG-INFO` & `cxxbuild-1.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.6.2
+Version: 1.6.3
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.2`
+- Version: `cxxbuild version=1.6.3`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
 
@@ -286,43 +286,46 @@
 
 None of them support dependencies, such as `cxxdeps.txt`, or even build systems such as cmake and bazel.
 
 Hopefully, when this project is fully finished, C++ will be a better place for all of us :)
 
 ### Case of Study
 
-In order to check the capabilities of cxxbuild, it was used to build the C/C++ ccbuild tool.
-Unfortunately, few tweaks were necessary in the generated CMakeLists, due to FLEX dependency, 
-but it was quite easy on general. See [Issue 34 on ccbuild project](https://github.com/bneijt/ccbuild/issues/34)
-
-General instructions:
-- Create `cxxdeps.txt` file:
+A very interesting case of study is the use of cxxbuild to build the C/C++ ccbuild tool.
+It is currently very easy to build it, using the following cxxdeps file:
 
 ```
 bobcat
 gnutls
 fl
 png
+FLEX == * [ ] local * _ false patch_flex.txt
 !std c++20
 !tests test
 !include "src"
 !include "src/sourceScanner"
 !define VERSION="v2.0.7-39-gdf7b35c"
 !extrasrc ${FLEX_SourceScanner_OUTPUTS}
 # apt install flex 
 # apt install libboost-all-dev
 # apt install gnutls-dev
 # apt install libbobcat-dev
 # apt install libpng-dev
 ```
 
-- Use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20` (or just `cxxbuild`, since build options will come directly from *cxxdeps.txt*)
+Also create the following `patch_flex.txt` file:
+
+```
+FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
+```
+
+- One may also use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20` (or just `cxxbuild`, since build options will come directly from *cxxdeps.txt*)
 - This line will be added automatically to CMakeLists: `add_definitions(-DVERSION="v2.0.7-39-gdf7b35c")`
 - This line will be added automatically to SOURCES: `${FLEX_SourceScanner_OUTPUTS}`
-- Add these two lines before the SOURCES:
+- These two lines will be put before the SOURCES:
 
 ```
 find_package(FLEX)
 FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
 ```
 
 And that's it! It builds all avaliable targets and tests for ccbuild.
```

### Comparing `cxxbuild-1.6.2/README.md` & `cxxbuild-1.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.2`
+- Version: `cxxbuild version=1.6.3`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
 
@@ -242,43 +242,46 @@
 
 None of them support dependencies, such as `cxxdeps.txt`, or even build systems such as cmake and bazel.
 
 Hopefully, when this project is fully finished, C++ will be a better place for all of us :)
 
 ### Case of Study
 
-In order to check the capabilities of cxxbuild, it was used to build the C/C++ ccbuild tool.
-Unfortunately, few tweaks were necessary in the generated CMakeLists, due to FLEX dependency, 
-but it was quite easy on general. See [Issue 34 on ccbuild project](https://github.com/bneijt/ccbuild/issues/34)
-
-General instructions:
-- Create `cxxdeps.txt` file:
+A very interesting case of study is the use of cxxbuild to build the C/C++ ccbuild tool.
+It is currently very easy to build it, using the following cxxdeps file:
 
 ```
 bobcat
 gnutls
 fl
 png
+FLEX == * [ ] local * _ false patch_flex.txt
 !std c++20
 !tests test
 !include "src"
 !include "src/sourceScanner"
 !define VERSION="v2.0.7-39-gdf7b35c"
 !extrasrc ${FLEX_SourceScanner_OUTPUTS}
 # apt install flex 
 # apt install libboost-all-dev
 # apt install gnutls-dev
 # apt install libbobcat-dev
 # apt install libpng-dev
 ```
 
-- Use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20` (or just `cxxbuild`, since build options will come directly from *cxxdeps.txt*)
+Also create the following `patch_flex.txt` file:
+
+```
+FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
+```
+
+- One may also use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20` (or just `cxxbuild`, since build options will come directly from *cxxdeps.txt*)
 - This line will be added automatically to CMakeLists: `add_definitions(-DVERSION="v2.0.7-39-gdf7b35c")`
 - This line will be added automatically to SOURCES: `${FLEX_SourceScanner_OUTPUTS}`
-- Add these two lines before the SOURCES:
+- These two lines will be put before the SOURCES:
 
 ```
 find_package(FLEX)
 FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
 ```
 
 And that's it! It builds all avaliable targets and tests for ccbuild.
```

### Comparing `cxxbuild-1.6.2/cxxbuild/cxxbuild.py` & `cxxbuild-1.6.3/cxxbuild/cxxbuild.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import platform
 import sys
 import json
 import subprocess
 
 def version():
-    v = "cxxbuild=1.6.2"
+    v = "cxxbuild=1.6.3"
     return v
 
 def usage():
     u=version()+"""
 Usage:
     cxxbuild [build] [ROOT_PATH] 
       builds with cxxbuild, examples: 
@@ -143,49 +143,90 @@
                                 for l in libs:
                                     cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+project_name+")")    
                         # end-if test
                         if triplet != "":
                             cmakelists.append("ENDIF()")
                         continue
                     #end-if system
-                    if pkg_manager == 'git' or pkg_manager == 'cmake+git':
+                    elif pkg_manager == 'git' or pkg_manager == 'cmake+git':
                         git_url = fields[k]
                         k=k+1
-                    cmakelists.append("FetchContent_Declare("+project_name+" GIT_REPOSITORY "+git_url+" GIT_TAG "+version_number+")")
-                    cmakelists.append("FetchContent_MakeAvailable("+project_name+")")
-                    # attach it to libraries, binaries and test binaries, if mode is *
-                    if mode == '*':
-                        for i in range(len(INCLUDE_DIRS)):
-                            for l in libs:
-                                cmakelists.append("target_link_libraries(my_headers"+str(i)+" INTERFACE "+l+")")
-                        for filepath, app_name in src_main.items():
-                            for l in libs:
-                                cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+l+")")    
-                        for filepath, app_name in src_test_main.items():
-                            for l in libs:
-                                cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+l+")")    
-                    # attach it to test binaries, if mode is 'test'
-                    if mode == 'test':
-                        for filepath, app_name in src_test_main.items():
-                            for l in libs:
-                                cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+l+")")    
-                    # read special, if exists
-                    print("k=",k)
-                    if k < len(fields):
-                        special = fields[k]
-                        k = k+1
-                        print("special=",special)
-                        # IGNORING THE special part for now... or forever, I hope!!!
-                        if special == '_special_catch_cmake_extras':
-                            cmakelists.append("list(APPEND CMAKE_MODULE_PATH ${catch2_SOURCE_DIR}/extras)")    
-                            cmakelists.append("include(CTest)")
-                            cmakelists.append("include(Catch)")
+                        cmakelists.append("FetchContent_Declare("+project_name+" GIT_REPOSITORY "+git_url+" GIT_TAG "+version_number+")")
+                        cmakelists.append("FetchContent_MakeAvailable("+project_name+")")
+                        # attach it to libraries, binaries and test binaries, if mode is *
+                        if mode == '*':
+                            for i in range(len(INCLUDE_DIRS)):
+                                for l in libs:
+                                    cmakelists.append("target_link_libraries(my_headers"+str(i)+" INTERFACE "+l+")")
+                            for filepath, app_name in src_main.items():
+                                for l in libs:
+                                    cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+l+")")    
                             for filepath, app_name in src_test_main.items():
-                                cmakelists.append("catch_discover_tests("+app_name[1]+")")    
-                    # end special
+                                for l in libs:
+                                    cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+l+")")    
+                        # attach it to test binaries, if mode is 'test'
+                        if mode == 'test':
+                            for filepath, app_name in src_test_main.items():
+                                for l in libs:
+                                    cmakelists.append("target_link_libraries("+app_name[1]+" PRIVATE "+l+")")    
+                        # read special, if exists
+                        print("k=",k)
+                        if k < len(fields):
+                            special = fields[k]
+                            k = k+1
+                            print("special=",special)
+                            # IGNORING THE special part for now... or forever, I hope!!!
+                            if special == '_special_catch_cmake_extras':
+                                cmakelists.append("list(APPEND CMAKE_MODULE_PATH ${catch2_SOURCE_DIR}/extras)")    
+                                cmakelists.append("include(CTest)")
+                                cmakelists.append("include(Catch)")
+                                for filepath, app_name in src_test_main.items():
+                                    cmakelists.append("catch_discover_tests("+app_name[1]+")")    
+                        # end special
+                        continue
+                    # end if git
+                    elif pkg_manager == 'local' or pkg_manager == 'cmake+local':
+                        # on cmake, this is resolved using find_package module
+                        local_path = fields[k]
+                        # check if local path is empty
+                        if local_path == "_":
+                            local_path = ""
+                        k=k+1
+                        # check if including libraries and special fix/patch
+                        add_inc_lib = True
+                        special = ""
+                        if k < len(fields):
+                            add_inc_lib = fields[k]
+                            if add_inc_lib == "true" or add_inc_lib == "True":
+                                add_inc_lib = True
+                            else:
+                                add_inc_lib = False
+                            k = k+1
+                            if k < len(fields):
+                                special = fields[k]
+                                k = k+1
+                        # begin construction of FindPackage
+                        if local_path != "":
+                            cmakelists.append("set("+project_name+"_DIR \"${CMAKE_SOURCE_DIR}/"+local_path+"\")")
+                        # ignoring 'version_number', for now!
+                        cmakelists.append("find_package("+project_name+" REQUIRED)")
+                        if add_inc_lib:
+                            cmakelists.append("include_directories(\"${"+project_name+"_INCLUDE_DIRS}\")")
+                            # todo: check libraries as well
+                        # todo: attach it to libraries, binaries and test binaries, if mode is *
+                        if special != "":
+                            # load patch file and append it
+                            with open(root_path+'/'+special, 'r') as fdx:
+                                patches=fdx.readlines()
+                                for p_line in patches:
+                                    cmakelists.append(p_line)
+                        continue
+                    # end if local
+                    print("cxxdeps error: build type '"+pkg_manager+"' unknown or not supported!")
+                    exit(1)
                 # end if not comment
             # end for line
         # end cxxdeps
 
     except FileNotFoundError:
         print("File cxxdeps.txt does not exist... ignoring it!")
 
@@ -487,45 +528,29 @@
     cmakelists.append("set (CMAKE_CXX_EXTENSIONS OFF)")
     cmakelists.append("set (CMAKE_EXPORT_COMPILE_COMMANDS ON)")
     cmakelists.append("Include(FetchContent)")
     # add definitions!
     for d in DEFINITIONS:
         # TODO: check definition type! type1: JUST_DEF   type2: DEF="value"
         cmakelists.append("add_definitions(-D"+d+")")
-    # add sources!
-    cmakelists.append("set(SOURCES")
-    # add extra sources!
-    for esrc in EXTRA_SOURCES:
-        cmakelists.append(esrc)
-    # get all sources not in main() list (no duplicates exist)
-    clean_list = []
-    clean_list_main = []
-    for f in src_list:
-        clean_list.append(f.replace("\\", "/"))
-    #clean_list = list(set(clean_list)) # do not do this!
-    for filepath, app_name in src_main.items():
-        clean_list_main.append(filepath.replace("\\", "/"))
-    #clean_list_main = list(set(clean_list_main))  # do not do this!
-    clean_list = [x for x in clean_list if x not in clean_list_main]
-    for f in clean_list:
-        cmakelists.append("\t"+f)
-    cmakelists.append(")")
+    #
+    cmakelists.append("# add all executables")
     COUNT_APP_ID=1
     all_apps = []
     # add_executable for binaries
     for filepath, app_name in src_main.items():
-        cmakelists.append("add_executable("+app_name[1]+" "+filepath.replace("\\", "/")+" ${SOURCES})")
+        cmakelists.append("add_executable("+app_name[1]+" "+filepath.replace("\\", "/")+" )")
     # add_executable for test binaries
     print("finding test executables!")
     # if no main is found, then each test is assumed to be independent!
     if len(src_test_main.items()) == 0:
         print("WARNING: no main() is found for tests... using main-less strategy!")
         src_test_main = src_test_nomain
     for filepath, app_name in src_test_main.items():
-        cmakelists.append("add_executable("+app_name[1]+" "+filepath.replace("\\", "/")+" ${SOURCES})")
+        cmakelists.append("add_executable("+app_name[1]+" "+filepath.replace("\\", "/")+" )")
 
 
     # INCLUDE_DIRS will act as header-only libraries
     #  => DO NOT ADD SOURCE FILES INTO include FOLDERS!!!
     for i in range(len(INCLUDE_DIRS)):
         cmakelists.append("add_library(my_headers"+str(i)+" INTERFACE)")
         cmakelists.append("target_include_directories(my_headers"+str(i)+" INTERFACE "+INCLUDE_DIRS[i]+")")
@@ -536,14 +561,38 @@
     #
     #print(cmakelists)
     generate_txt_from_toml(root_path)
 
     # cxxdeps.txt
     cmakelists = get_cmakelists_from_cxxdeps(root_path, cmakelists, INCLUDE_DIRS, src_main, src_test_main)
 
+    # ======== begin add sources ========
+    cmakelists.append("# finally, add all sources")
+    cmakelists.append("set(SOURCES")
+    # add extra sources!
+    for esrc in EXTRA_SOURCES:
+        cmakelists.append("\t"+esrc)
+    # get all sources not in main() list (no duplicates exist)
+    clean_list = []
+    clean_list_main = []
+    for f in src_list:
+        clean_list.append(f.replace("\\", "/"))
+    #clean_list = list(set(clean_list)) # do not do this!
+    for filepath, app_name in src_main.items():
+        clean_list_main.append(filepath.replace("\\", "/"))
+    #clean_list_main = list(set(clean_list_main))  # do not do this!
+    clean_list = [x for x in clean_list if x not in clean_list_main]
+    for f in clean_list:
+        cmakelists.append("\t"+f)
+    cmakelists.append(")")
+    # ======== end add sources ========
+    for filepath, app_name in src_main.items():
+        cmakelists.append("target_sources("+app_name[1]+" PRIVATE ${SOURCES})")
+    for filepath, app_name in src_test_main.items():
+        cmakelists.append("target_sources("+app_name[1]+" PRIVATE ${SOURCES})")
 
 
     # Generate CMakeLists.txt (or look for other option, such as 'bazel')
     # Assuming CMake and Ninja for now (TODO: must detect and warn to install!)
 
     # TODO: check if some CMakeLists.txt exists before overwriting it!
     # TODO: make backup of CMakeLists.txt only if content is different...
@@ -1083,16 +1132,20 @@
                     with open(root_path+"/"+file_path, 'r') as fd:
                         # TODO: add other formats for main... such as "int main()", etc...
                         # ANYWAY, these limitations are acceptable! 
                         # other options are: " main(" and "\nmain("
                         # If someone has a function "xxxmain(" it can currently break.
                         entrypoint = "main("
                         print("checking entrypoint:", entrypoint)
-                        if entrypoint in fd.read():
-                            src_main[file_path] = (root, file_name)
+                        all_lines=fd.readlines()
+                        for l in all_lines:
+                            # avoid commented lines (small improvement)
+                            l2 = l.strip()
+                            if entrypoint in l2 and l2[0] != "/" and l2[1] != "/":
+                                src_main[file_path] = (root, file_name)
         # end-for src_path
     # end-for src_paths
 
     print("src_main:", src_main)
     print("src_list:", src_list)
 
     # finding tests...
```

### Comparing `cxxbuild-1.6.2/cxxbuild.egg-info/PKG-INFO` & `cxxbuild-1.6.3/cxxbuild.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.6.2
+Version: 1.6.3
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.2`
+- Version: `cxxbuild version=1.6.3`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
 
@@ -286,43 +286,46 @@
 
 None of them support dependencies, such as `cxxdeps.txt`, or even build systems such as cmake and bazel.
 
 Hopefully, when this project is fully finished, C++ will be a better place for all of us :)
 
 ### Case of Study
 
-In order to check the capabilities of cxxbuild, it was used to build the C/C++ ccbuild tool.
-Unfortunately, few tweaks were necessary in the generated CMakeLists, due to FLEX dependency, 
-but it was quite easy on general. See [Issue 34 on ccbuild project](https://github.com/bneijt/ccbuild/issues/34)
-
-General instructions:
-- Create `cxxdeps.txt` file:
+A very interesting case of study is the use of cxxbuild to build the C/C++ ccbuild tool.
+It is currently very easy to build it, using the following cxxdeps file:
 
 ```
 bobcat
 gnutls
 fl
 png
+FLEX == * [ ] local * _ false patch_flex.txt
 !std c++20
 !tests test
 !include "src"
 !include "src/sourceScanner"
 !define VERSION="v2.0.7-39-gdf7b35c"
 !extrasrc ${FLEX_SourceScanner_OUTPUTS}
 # apt install flex 
 # apt install libboost-all-dev
 # apt install gnutls-dev
 # apt install libbobcat-dev
 # apt install libpng-dev
 ```
 
-- Use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20` (or just `cxxbuild`, since build options will come directly from *cxxdeps.txt*)
+Also create the following `patch_flex.txt` file:
+
+```
+FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
+```
+
+- One may also use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20` (or just `cxxbuild`, since build options will come directly from *cxxdeps.txt*)
 - This line will be added automatically to CMakeLists: `add_definitions(-DVERSION="v2.0.7-39-gdf7b35c")`
 - This line will be added automatically to SOURCES: `${FLEX_SourceScanner_OUTPUTS}`
-- Add these two lines before the SOURCES:
+- These two lines will be put before the SOURCES:
 
 ```
 find_package(FLEX)
 FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
 ```
 
 And that's it! It builds all avaliable targets and tests for ccbuild.
```

### Comparing `cxxbuild-1.6.2/pyproject.toml` & `cxxbuild-1.6.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires=["setuptools", "wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name="cxxbuild"
-version="1.6.2"
+version="1.6.3"
 description="CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!"
 readme="README.md"
 authors=[{ name="Igor Machado Coelho", email="igormcoelho@proton.me" }]
 license={ file="LICENSE" }
 classifiers=[
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

