# Comparing `tmp/alibuild-1.9.8.tar.gz` & `tmp/alibuild-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alibuild-1.9.8.tar", last modified: Mon Dec  6 11:51:23 2021, max compression
+gzip compressed data, was "alibuild-1.9.9.tar", last modified: Wed Jan 19 15:44:10 2022, max compression
```

## Comparing `alibuild-1.9.8.tar` & `alibuild-1.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 11:51:23.912217 alibuild-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2021-12-06 11:51:21.000000 alibuild-1.9.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-06 11:51:21.000000 alibuild-1.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2021-12-06 11:51:23.912217 alibuild-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      682 2021-12-06 11:51:21.000000 alibuild-1.9.8/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4422 2021-12-06 11:51:21.000000 alibuild-1.9.8/aliBuild
--rwxr-xr-x   0 runner    (1001) docker     (121)      232 2021-12-06 11:51:21.000000 alibuild-1.9.8/aliDeps
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2021-12-06 11:51:21.000000 alibuild-1.9.8/aliDoctor
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 11:51:23.908217 alibuild-1.9.8/alibuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2021-12-06 11:51:23.000000 alibuild-1.9.8/alibuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-12-06 11:51:23.000000 alibuild-1.9.8/alibuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-06 11:51:23.000000 alibuild-1.9.8/alibuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-12-06 11:51:23.000000 alibuild-1.9.8/alibuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-06 11:51:23.000000 alibuild-1.9.8/alibuild.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 11:51:23.912217 alibuild-1.9.8/alibuild_helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-12-06 11:51:22.000000 alibuild-1.9.8/alibuild_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4659 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)    25968 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/args.py
--rw-r--r--   0 runner    (1001) docker     (121)    51176 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/build.py
--rw-r--r--   0 runner    (1001) docker     (121)    11775 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/build_template.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     3357 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4514 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/deps.py
--rw-r--r--   0 runner    (1001) docker     (121)     8869 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/doctor.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     5525 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    23558 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    17229 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2021-12-06 11:51:21.000000 alibuild-1.9.8/alibuild_helpers/workarea.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11320 2021-12-06 11:51:21.000000 alibuild-1.9.8/alienv
--rwxr-xr-x   0 runner    (1001) docker     (121)      224 2021-12-06 11:51:21.000000 alibuild-1.9.8/pb
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-06 11:51:23.912217 alibuild-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2021-12-06 11:51:21.000000 alibuild-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 15:44:10.646007 alibuild-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-01-19 15:44:09.000000 alibuild-1.9.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-19 15:44:09.000000 alibuild-1.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-01-19 15:44:10.646007 alibuild-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-01-19 15:44:09.000000 alibuild-1.9.9/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4422 2022-01-19 15:44:09.000000 alibuild-1.9.9/aliBuild
+-rwxr-xr-x   0 runner    (1001) docker     (121)      232 2022-01-19 15:44:09.000000 alibuild-1.9.9/aliDeps
+-rwxr-xr-x   0 runner    (1001) docker     (121)      234 2022-01-19 15:44:09.000000 alibuild-1.9.9/aliDoctor
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 15:44:10.646007 alibuild-1.9.9/alibuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-01-19 15:44:10.000000 alibuild-1.9.9/alibuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-01-19 15:44:10.000000 alibuild-1.9.9/alibuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-19 15:44:10.000000 alibuild-1.9.9/alibuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-19 15:44:10.000000 alibuild-1.9.9/alibuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-19 15:44:10.000000 alibuild-1.9.9/alibuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 15:44:10.646007 alibuild-1.9.9/alibuild_helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-01-19 15:44:10.000000 alibuild-1.9.9/alibuild_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25968 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/args.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51176 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12130 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/build_template.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3357 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4514 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5525 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23558 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17229 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-01-19 15:44:09.000000 alibuild-1.9.9/alibuild_helpers/workarea.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11320 2022-01-19 15:44:09.000000 alibuild-1.9.9/alienv
+-rwxr-xr-x   0 runner    (1001) docker     (121)      224 2022-01-19 15:44:09.000000 alibuild-1.9.9/pb
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-19 15:44:10.646007 alibuild-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3617 2022-01-19 15:44:09.000000 alibuild-1.9.9/setup.py
```

### Comparing `alibuild-1.9.8/LICENSE.md` & `alibuild-1.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/PKG-INFO` & `alibuild-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibuild
-Version: 1.9.8
+Version: 1.9.9
 Summary: ALICE Build Tool
 Home-page: https://alisw.github.io/alibuild
 Author: Giulio Eulisse
 Author-email: giulio.eulisse@cern.ch
 License: GPL
 Keywords: HEP ALICE
 Platform: UNKNOWN
```

### Comparing `alibuild-1.9.8/README.rst` & `alibuild-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/aliBuild` & `alibuild-1.9.9/aliBuild`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild.egg-info/PKG-INFO` & `alibuild-1.9.9/alibuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibuild
-Version: 1.9.8
+Version: 1.9.9
 Summary: ALICE Build Tool
 Home-page: https://alisw.github.io/alibuild
 Author: Giulio Eulisse
 Author-email: giulio.eulisse@cern.ch
 License: GPL
 Keywords: HEP ALICE
 Platform: UNKNOWN
```

### Comparing `alibuild-1.9.8/alibuild.egg-info/SOURCES.txt` & `alibuild-1.9.9/alibuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/analytics.py` & `alibuild-1.9.9/alibuild_helpers/analytics.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/args.py` & `alibuild-1.9.9/alibuild_helpers/args.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/build.py` & `alibuild-1.9.9/alibuild_helpers/build.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/build_template.sh` & `alibuild-1.9.9/alibuild_helpers/build_template.sh`

 * *Files 6% similar despite different names*

```diff
@@ -208,58 +208,61 @@
 # Always relocate the modulefile (if present) so that it works also in devel mode.
 if [[ ! -s "$INSTALLROOT/.original-unrelocated" && -f "$INSTALLROOT/etc/modulefiles/$PKGNAME" ]]; then
   echo "mv -f \$PP/etc/modulefiles/$PKGNAME \$PP/etc/modulefiles/${PKGNAME}.forced-relocation && sed -e \"s|[@][@]PKGREVISION[@]\$PH[@][@]|$PKGREVISION|g\" \$PP/etc/modulefiles/${PKGNAME}.forced-relocation > \$PP/etc/modulefiles/$PKGNAME" >> "$INSTALLROOT/relocate-me.sh"
 fi
 
 # Find libraries and executables needing relocation on macOS
 if [[ ${ARCHITECTURE:0:3} == "osx" ]]; then
+  otool_arch=$(echo "${ARCHITECTURE#osx_}" | tr - _)  # otool knows x86_64, not x86-64
 
-  /usr/bin/find ${RELOCATE_PATHS:-bin lib lib64} -type f -not -name '*.py' -not -name '*.pyc' -not -name '*.h' -not -name '*.js' -not -name '*.txt' -not -name '*.dat' -not -name '*.sav' -not -name '*.wav' -not -name '*.png' -not -name '*.css' -not -name '*.cc' | \
-  while read BIN; do
-    MACHOTYPE=$(set +o pipefail; otool -h "$PWD/$BIN" 2> /dev/null | grep filetype -A1 | awk 'END{print $5}')
-
-    # See mach-o/loader.h from XNU sources: 2 == executable, 6 == dylib, 8 == bundle
-    if [[ $MACHOTYPE == 6 || $MACHOTYPE == 8 ]]; then
-      # Only dylibs: relocate LC_ID_DYLIB
-      if otool -D "$PWD/$BIN" 2> /dev/null | tail -n1 | grep -q $PKGHASH; then
-        cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
-install_name_tool -id \$(otool -D "\$PP/$BIN" | tail -n1 | sed -e "s|/[^ ]*INSTALLROOT/\$PH/\$OP|\$WORK_DIR/\$PP|g") "\$PP/$BIN"
+  /usr/bin/find ${RELOCATE_PATHS:-bin lib lib64} -type f \
+                -not -name '*.py' -not -name '*.pyc' -not -name '*.h' -not -name '*.js' \
+                -not -name '*.txt' -not -name '*.dat' -not -name '*.sav' -not -name '*.wav' \
+                -not -name '*.png' -not -name '*.css' -not -name '*.cc' |
+    while read -r BIN; do
+      MACHOTYPE=$(set +o pipefail; otool -arch "$otool_arch" -h "$PWD/$BIN" 2> /dev/null | grep filetype -A1 | awk 'END{print $5}')
+
+      # See mach-o/loader.h from XNU sources: 2 == executable, 6 == dylib, 8 == bundle
+      if [[ $MACHOTYPE == 6 || $MACHOTYPE == 8 ]]; then
+        # Only dylibs: relocate LC_ID_DYLIB
+        if otool -arch "$otool_arch" -D "$PWD/$BIN" 2> /dev/null | tail -n1 | grep -q "$PKGHASH"; then
+          cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
+install_name_tool -id "\$(otool -arch $otool_arch -D "\$PP/$BIN" | tail -n1 | sed -e "s|/[^ ]*INSTALLROOT/\$PH/\$OP|\$WORK_DIR/\$PP|g")" "\$PP/$BIN"
 EOF
-      elif otool -D "$PWD/$BIN" 2> /dev/null | tail -n1 | grep -vq /; then
-        cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
+        elif otool -arch "$otool_arch" -D "$PWD/$BIN" 2> /dev/null | tail -n1 | grep -vq /; then
+          cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
 install_name_tool -id "\$WORK_DIR/\$PP/$BIN" "\$PP/$BIN"
 EOF
+        fi
       fi
-    fi
 
-    if [[ $MACHOTYPE == 2 || $MACHOTYPE == 6 || $MACHOTYPE == 8 ]]; then
-      # Both libs and binaries: relocate LC_RPATH
-      if otool -l "$PWD/$BIN" 2> /dev/null | grep -A2 LC_RPATH | grep path | grep -q $PKGHASH; then
-        cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
-OLD_RPATHS=\$(otool -l \$PP/$BIN | grep -A2 LC_RPATH | grep path | grep \$PH | sed -e 's|^.*path ||' -e 's| .*$||' | sort -u)
+      if [[ $MACHOTYPE == 2 || $MACHOTYPE == 6 || $MACHOTYPE == 8 ]]; then
+        # Both libs and binaries: relocate LC_RPATH
+        if otool -arch "$otool_arch" -l "$PWD/$BIN" 2> /dev/null | grep -A2 LC_RPATH | grep path | grep -q "$PKGHASH"; then
+          cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
+OLD_RPATHS=\$(otool -arch $otool_arch -l "\$PP/$BIN" | grep -A2 LC_RPATH | grep path | grep "\$PH" | sed -e 's|^.*path ||' -e 's| .*$||' | sort -u)
 for OLD_RPATH in \$OLD_RPATHS; do
   NEW_RPATH=\${OLD_RPATH/#*INSTALLROOT\/\$PH\/\$OP/\$WORK_DIR/\$PP}
   install_name_tool -rpath "\$OLD_RPATH" "\$NEW_RPATH" "\$PP/$BIN"
 done
 EOF
-      fi
+        fi
 
-      # Both libs and binaries: relocate LC_LOAD_DYLIB
-      if otool -l "$PWD/$BIN" 2> /dev/null | grep -A2 LC_LOAD_DYLIB | grep name | grep -q $PKGHASH; then
-        cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
-OLD_LOAD_DYLIBS=\$(otool -l \$PP/$BIN | grep -A2 LC_LOAD_DYLIB | grep name | grep \$PH | sed -e 's|^.*name ||' -e 's| .*$||' | sort -u)
+        # Both libs and binaries: relocate LC_LOAD_DYLIB
+        if otool -arch "$otool_arch" -l "$PWD/$BIN" 2> /dev/null | grep -A2 LC_LOAD_DYLIB | grep name | grep -q $PKGHASH; then
+          cat <<EOF >> "$INSTALLROOT/relocate-me.sh"
+OLD_LOAD_DYLIBS=\$(otool -arch $otool_arch -l "\$PP/$BIN" | grep -A2 LC_LOAD_DYLIB | grep name | grep "\$PH" | sed -e 's|^.*name ||' -e 's| .*$||' | sort -u)
 for OLD_LOAD_DYLIB in \$OLD_LOAD_DYLIBS; do
   NEW_LOAD_DYLIB=\${OLD_LOAD_DYLIB/#*INSTALLROOT\/\$PH\/\$OP/\$WORK_DIR/\$PP}
   install_name_tool -change "\$OLD_LOAD_DYLIB" "\$NEW_LOAD_DYLIB" "\$PP/$BIN"
 done
 EOF
+        fi
       fi
-    fi
-done || true
-
+    done || true
 fi
 
 cat "$INSTALLROOT/relocate-me.sh"
 cat "$INSTALLROOT/.original-unrelocated" | xargs -n1 -I{} cp '{}' '{}'.unrelocated
 cd "$WORK_DIR/INSTALLROOT/$PKGHASH"
 
 # Archive creation
```

### Comparing `alibuild-1.9.8/alibuild_helpers/clean.py` & `alibuild-1.9.9/alibuild_helpers/clean.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/cmd.py` & `alibuild-1.9.9/alibuild_helpers/cmd.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/deps.py` & `alibuild-1.9.9/alibuild_helpers/deps.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/doctor.py` & `alibuild-1.9.9/alibuild_helpers/doctor.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/init.py` & `alibuild-1.9.9/alibuild_helpers/init.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/log.py` & `alibuild-1.9.9/alibuild_helpers/log.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/sync.py` & `alibuild-1.9.9/alibuild_helpers/sync.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/utilities.py` & `alibuild-1.9.9/alibuild_helpers/utilities.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alibuild_helpers/workarea.py` & `alibuild-1.9.9/alibuild_helpers/workarea.py`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/alienv` & `alibuild-1.9.9/alienv`

 * *Files identical despite different names*

### Comparing `alibuild-1.9.8/setup.py` & `alibuild-1.9.9/setup.py`

 * *Files identical despite different names*

