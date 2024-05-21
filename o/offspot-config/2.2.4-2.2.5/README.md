# Comparing `tmp/offspot_config-2.2.4.tar.gz` & `tmp/offspot_config-2.2.5.tar.gz`

## Comparing `offspot_config-2.2.4.tar` & `offspot_config-2.2.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 offspot_config-2.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/__init__.py
--rw-r--r--   0        0        0    33863 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/builder.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/catalog.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/catalog.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/constants.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/file.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/oci_images.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/packages.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/zim.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/branding/horizontal-logo-light.png
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/branding/square-logo-light.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/base.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/checksum.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/file.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/mainconfig.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/oci.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/output.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/str.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/inputs/ways.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/utils/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/utils/dashboard.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/utils/download.py
--rw-r--r--   0        0        0    12899 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/utils/misc.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/utils/sizes.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_config/utils/yaml.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/__init__.py
--rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/ap.py
--rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/checks.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/configlib.py
--rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/containers.py
--rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/dnsmasqspoof.py
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/ethernet.py
--rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/firmware.py
--rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/fromfile.py
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/hostname.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.2.4/src/offspot_runtime/timezone.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/conftest.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_catalog.py
--rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_checks.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_humanid.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_inputs.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_link.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_reader.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.2.4/tests/test_zim.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.2.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.2.4/LICENSE
--rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.2.4/README.md
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.2.4/pyproject.toml
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.2.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 offspot_config-2.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/__init__.py
+-rw-r--r--   0        0        0    33916 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/builder.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/catalog.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/catalog.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/constants.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/file.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/oci_images.py
+-rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/packages.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/zim.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/branding/horizontal-logo-light.png
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/branding/square-logo-light.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/base.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/checksum.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/file.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/mainconfig.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/oci.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/output.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/str.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/inputs/ways.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/utils/__init__.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/utils/dashboard.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/utils/download.py
+-rw-r--r--   0        0        0    12899 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/utils/misc.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/utils/sizes.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_config/utils/yaml.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/__init__.py
+-rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/ap.py
+-rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/checks.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/configlib.py
+-rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/containers.py
+-rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/dnsmasqspoof.py
+-rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/ethernet.py
+-rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/firmware.py
+-rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/fromfile.py
+-rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/hostname.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.2.5/src/offspot_runtime/timezone.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/conftest.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_catalog.py
+-rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_checks.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_humanid.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_inputs.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_link.py
+-rw-r--r--   0        0        0     7147 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_reader.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.2.5/tests/test_zim.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.2.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.2.5/LICENSE
+-rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.2.5/README.md
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.2.5/PKG-INFO
```

### Comparing `offspot_config-2.2.4/.pre-commit-config.yaml` & `offspot_config-2.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/CHANGELOG.md` & `offspot_config-2.2.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.5] - 2024-05-21
+
+### Added
+
+- [utils.dashboard] New `Reader.to_dashboard_dict()` returning dashboard-transformed download URL
+
+### Fixed
+
+- [builder] Reader download link using local URL
+
 ## [2.2.4] - 2024-05-01
 
 ### Changed
 
 - [builder] Using captive-portal 1.4.3 fixing 2.2.1 regression
 
 ## [2.2.3] - 2024-04-26
```

### Comparing `offspot_config-2.2.4/tasks.py` & `offspot_config-2.2.5/tasks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/builder.py` & `offspot_config-2.2.5/src/offspot_config/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
                 package.to_dashboard_entry(fqdn=self.fqdn, download_fqdn=download_fqdn)
                 for package in self.dashboard_entries
             ],
         }
 
         if self.dashboard_readers:
             payload["readers"] = [
-                reader.to_dict()
+                reader.to_dashboard_dict(download_fqdn=f"{ZIMDL_PREFIX}.{self.fqdn}")
                 for reader in sorted(self.dashboard_readers, key=Reader.sort)
             ]
 
         if self.dashboard_links:
             payload["links"] = [link.to_dict() for link in self.dashboard_links]
             # resolve variables in link (for FQDN mostly)
             for link in payload["links"]:
```

### Comparing `offspot_config-2.2.4/src/offspot_config/catalog.json` & `offspot_config-2.2.5/src/offspot_config/catalog.json`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/catalog.py` & `offspot_config-2.2.5/src/offspot_config/catalog.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/constants.py` & `offspot_config-2.2.5/src/offspot_config/constants.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/file.py` & `offspot_config-2.2.5/src/offspot_config/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/oci_images.py` & `offspot_config-2.2.5/src/offspot_config/oci_images.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/packages.py` & `offspot_config-2.2.5/src/offspot_config/packages.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/zim.py` & `offspot_config-2.2.5/src/offspot_config/zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/branding/horizontal-logo-light.png` & `offspot_config-2.2.5/src/offspot_config/branding/horizontal-logo-light.png`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/branding/square-logo-light.png` & `offspot_config-2.2.5/src/offspot_config/branding/square-logo-light.png`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/inputs/base.py` & `offspot_config-2.2.5/src/offspot_config/inputs/base.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/inputs/checksum.py` & `offspot_config-2.2.5/src/offspot_config/inputs/checksum.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/inputs/file.py` & `offspot_config-2.2.5/src/offspot_config/inputs/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/inputs/mainconfig.py` & `offspot_config-2.2.5/src/offspot_config/inputs/mainconfig.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/inputs/output.py` & `offspot_config-2.2.5/src/offspot_config/inputs/output.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/utils/dashboard.py` & `offspot_config-2.2.5/src/offspot_config/utils/dashboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,19 @@
         def value_or_dict(value):
             if hasattr(value, "to_dict"):
                 return value.to_dict()
             return value
 
         return {field: value_or_dict(getattr(self, field)) for field in self._fields}
 
+    def to_dashboard_dict(self, download_fqdn: str) -> dict[str, str | int]:
+        data = self.to_dict()
+        data["download_url"] = f"//{download_fqdn}/{data['filename']!s}"
+        return data
+
     @property
     def order(self) -> int:
         """sort-usable order based on reader's platform popularity"""
         return {"windows": 0, "android": 1, "macos": 2, "linux": 3}.get(
             self.platform, 4
         )
```

### Comparing `offspot_config-2.2.4/src/offspot_config/utils/download.py` & `offspot_config-2.2.5/src/offspot_config/utils/download.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/utils/misc.py` & `offspot_config-2.2.5/src/offspot_config/utils/misc.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/utils/sizes.py` & `offspot_config-2.2.5/src/offspot_config/utils/sizes.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_config/utils/yaml.py` & `offspot_config-2.2.5/src/offspot_config/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/ap.py` & `offspot_config-2.2.5/src/offspot_runtime/ap.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/checks.py` & `offspot_config-2.2.5/src/offspot_runtime/checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/configlib.py` & `offspot_config-2.2.5/src/offspot_runtime/configlib.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/containers.py` & `offspot_config-2.2.5/src/offspot_runtime/containers.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/dnsmasqspoof.py` & `offspot_config-2.2.5/src/offspot_runtime/dnsmasqspoof.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/ethernet.py` & `offspot_config-2.2.5/src/offspot_runtime/ethernet.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/firmware.py` & `offspot_config-2.2.5/src/offspot_runtime/firmware.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/fromfile.py` & `offspot_config-2.2.5/src/offspot_runtime/fromfile.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/hostname.py` & `offspot_config-2.2.5/src/offspot_runtime/hostname.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/src/offspot_runtime/timezone.py` & `offspot_config-2.2.5/src/offspot_runtime/timezone.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/tests/conftest.py` & `offspot_config-2.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/tests/test_checks.py` & `offspot_config-2.2.5/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/tests/test_humanid.py` & `offspot_config-2.2.5/tests/test_humanid.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/tests/test_inputs.py` & `offspot_config-2.2.5/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/tests/test_link.py` & `offspot_config-2.2.5/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/tests/test_reader.py` & `offspot_config-2.2.5/tests/test_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         "https://download.kiwix.org/release/kiwix-desktop/kiwix-desktop_windows_x64_2.3.1-2.zip",
         "kiwix-desktop_windows_x64_2.3.1-2.zip",
         126628211,
         "adf9b64b5c6906427d7a1c8bdfc31546",
     ),
     (
         "macos",
-        "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
-        "kiwix-desktop-macos_3.1.0.dmg",
+        "https://download.kiwix.org/release/kiwix-macos/kiwix-macos_3.1.0.dmg",
+        "kiwix-macos_3.1.0.dmg",
         16051402,
         "747fd0841b56d2d5158e0e65646b1be1",
     ),
 ]
 
 
 @pytest.mark.parametrize(
@@ -43,16 +43,16 @@
             "kiwix-desktop_windows_x64_2.3.1-2.zip",
         ),
         (
             "https://download.kiwix.org/release/kiwix-android/kiwix-3.9.1.apk",
             "kiwix-3.9.1.apk",
         ),
         (
-            "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
-            "kiwix-desktop-macos_3.1.0.dmg",
+            "https://download.kiwix.org/release/kiwix-macos/kiwix-macos_3.1.0.dmg",
+            "kiwix-macos_3.1.0.dmg",
         ),
         (
             "https://download.kiwix.org/release/kiwix-desktop/kiwix-desktop_x86_64_2.3.1-4.appimage",
             "kiwix-desktop_x86_64_2.3.1-4.appimage",
         ),
         ("https://www.freecodecamp.org/news/css-unit-guide/", "css-unit-guide"),
     ],
@@ -197,22 +197,22 @@
                     "value": "adf9b64b5c6906427d7a1c8bdfc31546",
                     "kind": "digest",
                 },
             },
         ),
         (
             "macos",
-            "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
+            "https://download.kiwix.org/release/kiwix-macos/kiwix-macos_3.1.0.dmg",
             None,
             None,
             None,
             {
                 "platform": "macos",
-                "download_url": "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
-                "filename": "kiwix-desktop-macos_3.1.0.dmg",
+                "download_url": "https://download.kiwix.org/release/kiwix-macos/kiwix-macos_3.1.0.dmg",
+                "filename": "kiwix-macos_3.1.0.dmg",
                 "size": 16051402,
                 "checksum": None,
             },
         ),
     ],
 )
 def test_to_dict(platform, download_url, filename, size, md5sum, expected_dict):
```

### Comparing `offspot_config-2.2.4/tests/test_zim.py` & `offspot_config-2.2.5/tests/test_zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/.gitignore` & `offspot_config-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/LICENSE` & `offspot_config-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/README.md` & `offspot_config-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/pyproject.toml` & `offspot_config-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.4/PKG-INFO` & `offspot_config-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: offspot-config
-Version: 2.2.4
+Version: 2.2.5
 Summary: Offspot Config helpers
 Project-URL: Homepage, https://github.com/offspot/offspot-config
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Author-email: Kiwix <dev@kiwix.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offspot
```

