# Comparing `tmp/rstms_cloudflare-1.0.0.tar.gz` & `tmp/rstms_cloudflare-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_cloudflare-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_cloudflare-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_cloudflare-1.0.0.tar` & `rstms_cloudflare-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      383 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1338 2024-04-16 03:08:46.809802 rstms_cloudflare-1.0.0/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.0.0/LICENSE
--rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.0.0/Makefile
--rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.0.0/README.md
--rw-r--r--   0        0        0        6 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/VERSION
--rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/Makefile
--rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.0.0/docs/cli.rst
--rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.0.0/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.0.0/docs/contributing.rst
--rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/index.rst
--rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/installation.rst
--rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.0.0/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.0.0/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.0.0/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.0.0/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.0.0/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.0.0/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.0.0/make/docs.mk
--rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.0.0/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-1.0.0/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.0.0/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.0.0/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.0.0/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.0.0/make/version.mk
--rw-r--r--   0        0        0     1159 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.0.0/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-21 01:03:15.065281 rstms_cloudflare-1.0.0/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-21 01:03:15.121280 rstms_cloudflare-1.0.0/requirements-docs.txt
--rw-r--r--   0        0        0       19 2024-05-21 01:03:15.009281 rstms_cloudflare-1.0.0/requirements.txt
--rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.0.0/rstms_cloudflare/__init__.py
--rw-r--r--   0        0        0     6400 2024-05-21 00:42:18.598476 rstms_cloudflare-1.0.0/rstms_cloudflare/cli.py
--rw-r--r--   0        0        0     5670 2024-05-21 00:53:29.275442 rstms_cloudflare-1.0.0/rstms_cloudflare/cloudflare.py
--rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.0.0/rstms_cloudflare/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.0.0/rstms_cloudflare/shell.py
--rw-r--r--   0        0        0      127 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/rstms_cloudflare/version.py
--rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.0.0/tox.ini
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      383 2024-05-21 01:53:12.418270 rstms_cloudflare-1.1.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.0/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.0/Makefile
+-rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.0/README.md
+-rw-r--r--   0        0        0        6 2024-05-21 01:53:12.418270 rstms_cloudflare-1.1.0/VERSION
+-rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.0/docs/cli.rst
+-rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.0/docs/contributing.rst
+-rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.0/docs/installation.rst
+-rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.0/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.0/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.0/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.1.0/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.0/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.0/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.0/make/docs.mk
+-rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.1.0/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.0/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.0/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.0/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.0/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.0/make/version.mk
+-rw-r--r--   0        0        0     1159 2024-05-21 01:53:12.418270 rstms_cloudflare-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.0/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-21 01:53:12.270271 rstms_cloudflare-1.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-21 01:53:12.326271 rstms_cloudflare-1.1.0/requirements-docs.txt
+-rw-r--r--   0        0        0       19 2024-05-21 01:53:12.210272 rstms_cloudflare-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.0/rstms_cloudflare/__init__.py
+-rw-r--r--   0        0        0     6405 2024-05-21 01:43:15.316489 rstms_cloudflare-1.1.0/rstms_cloudflare/cli.py
+-rw-r--r--   0        0        0     6182 2024-05-21 01:42:56.024690 rstms_cloudflare-1.1.0/rstms_cloudflare/cloudflare.py
+-rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.0/rstms_cloudflare/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.0/rstms_cloudflare/shell.py
+-rw-r--r--   0        0        0      127 2024-05-21 01:53:12.418270 rstms_cloudflare-1.1.0/rstms_cloudflare/version.py
+-rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.0/tox.ini
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.0/PKG-INFO
```

### Comparing `rstms_cloudflare-1.0.0/.gitignore` & `rstms_cloudflare-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -115,7 +115,8 @@
 .black
 .errors
 .flake8
 docker/VERSION
 docker/.build
 docker/*.whl
 postactivate
+notes
```

### Comparing `rstms_cloudflare-1.0.0/LICENSE` & `rstms_cloudflare-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/Makefile` & `rstms_cloudflare-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/README.md` & `rstms_cloudflare-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/docs/Makefile` & `rstms_cloudflare-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/docs/conf.py` & `rstms_cloudflare-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/docs/installation.rst` & `rstms_cloudflare-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/docs/make.bat` & `rstms_cloudflare-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/clean.mk` & `rstms_cloudflare-1.1.0/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/common.mk` & `rstms_cloudflare-1.1.0/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/docs.mk` & `rstms_cloudflare-1.1.0/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/lint.mk` & `rstms_cloudflare-1.1.0/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/publish.mk` & `rstms_cloudflare-1.1.0/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/release.mk` & `rstms_cloudflare-1.1.0/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/test.mk` & `rstms_cloudflare-1.1.0/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/make/version.mk` & `rstms_cloudflare-1.1.0/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/pyproject.toml` & `rstms_cloudflare-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-cloudflare"
-version = "1.0.0"
+version = "1.1.0"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_cloudflare"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_cloudflare-1.0.0/rstms_cloudflare/cli.py` & `rstms_cloudflare-1.1.0/rstms_cloudflare/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,26 @@
     "--shell-completion",
     is_flag=False,
     flag_value="[auto]",
     callback=_shell_completion,
     help="configure shell completion",
 )
 @click.option("-q", "--quiet", is_flag=True)
-@click.option("-v", "--verbose", is_flag=True)
+@click.option("-r", "--raw", is_flag=True)
 @click.option("-t", "--token", envvar="CLOUDFLARE_AUTH_TOKEN")
 @click.option("-j", "--json", is_flag=True)
 @click.option("-o", "--output", type=click.Path(writable=True, dir_okay=False, path_type=Path), help="output file")
+@click.option("-i", "--id", "include_id", is_flag=True, help="include record ID in output")
 @click.pass_context
-def cli(ctx, debug, shell_completion, token, json, quiet, verbose, output):
+def cli(ctx, debug, shell_completion, token, json, quiet, raw, include_id, output):
     if output:
         func = output.write_text
     else:
         func = click.echo
-    ctx.obj = API(token=token, json=json, quiet=quiet, verbose=verbose, output_function=func)
+    ctx.obj = API(token=token, json=json, quiet=quiet, raw=raw, include_id=include_id, output_function=func)
 
 
 @cli.command
 @click.argument("domain", required=False)
 @click.pass_obj
 def dump(api, domain):
     """Output API data for one or all domains"""
@@ -68,15 +69,14 @@
             opt = None
         else:
             raise RuntimeError(f"{name} option conflicts with argument")
     return arg or opt
 
 
 @cli.command
-@click.option("-i", "--id", "output_id", is_flag=True, help="output record ID")
 @click.option("--delete", "delete_records", is_flag=True, help="delete selected records")
 @click.option("--update-content", help="update selected record content")
 @click.option("--update-ttl", help="update selected record TTL")
 @click.option("-t", "--type", "filter_type", type=click.Choice(API.RECORD_TYPES + ["ID"]))
 @click.option("-h", "--host", "filter_host", help="match host or /regex/")
 @click.option("-c", "--content", "filter_content", help="match content or /regex/")
 @click.option("-p", "--priority", type=int, help="filter by MX priority")
@@ -87,15 +87,14 @@
 @click.pass_obj
 def records(
     api,
     domain,
     type,
     host,
     content,
-    output_id,
     filter_type,
     filter_host,
     filter_content,
     delete_records,
     priority,
     update_content,
     update_ttl,
@@ -117,15 +116,15 @@
         for record in records:
             if update_content:
                 record["content"] = update_content
             if update_ttl:
                 record["ttl"] = update_ttl
         records = api.update_records(records)
     else:
-        records = api.format_records(records, output_id)
+        records = api.format_records(records)
 
     api.output(records)
     sys.exit(0 if records else -1)
 
 
 @cli.command
 @click.pass_obj
```

### Comparing `rstms_cloudflare-1.0.0/rstms_cloudflare/cloudflare.py` & `rstms_cloudflare-1.1.0/rstms_cloudflare/cloudflare.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 
 class API:
 
     RECORD_TYPES = ["A", "AAAA", "CNAME", "MX", "NS", "SOA", "TXT", "SRV", "LOC"]
     MAX_ZONES = 128
 
-    def __init__(self, token=None, json=False, quiet=False, verbose=False, output_function=None):
+    def __init__(self, token=None, json=False, quiet=False, raw=False, include_id=False, output_function=None):
         token = token or os.environ["CLOUDFLARE_AUTH_TOKEN"]
         self.client = CloudFlare.CloudFlare(token=token)
         self.json = json
-        self.verbose = verbose
+        self.raw = raw
         self.quiet = quiet
+        self.include_id = include_id
         self.output_function = output_function or print
 
     def output(self, data):
         if self.quiet:
             return
         if self.json:
             data = json.dumps(data, indent=2)
@@ -101,63 +102,75 @@
         ret = self.client.zones.dns_records.patch(zone_id, dns_record_id, data=update)
 
         if self.json:
             return ret
         else:
             return ret["id"]
 
-    def format_record(self, record, with_id=False):
+    def format_host(self, record):
+        domain = record["zone_name"]
+        host = record["name"]
+        if host.endswith(domain):
+            host = host[: -1 - len(domain)]
+        if not host:
+            host = "@"
+        return host
+
+    def format_record(self, record):
         if self.json:
-            if self.verbose:
+            if self.raw:
                 out = record
             else:
                 out = dict(
-                    name=record["name"],
+                    domain=record["zone_name"],
+                    name=self.format_host(record),
                     content=record["content"],
                     type=record["type"],
                     ttl=record["ttl"],
                     priority=record.get("priority", None),
                 )
                 if record["type"] == "MX":
                     out["priority"] = record["priority"]
-                if with_id:
+                if self.include_id:
                     out["id"] = record["id"]
         else:
             out = ""
-            if with_id:
+            if self.include_id:
                 out += f"{record['id']} "
             out += f"{record['type']} "
             if record["type"] == "MX":
                 out += f"{record['priority']} "
             if record["type"] == "TXT":
                 content = '"' + record["content"] + '"'
             else:
-                content = record['content']
+                content = record["content"]
             out += f"{record['name']} {content} {record['ttl']}"
         return out
 
-    def format_records(self, records, with_id=False):
-        formatted = [self.format_record(r, with_id) for r in records]
+    def format_records(self, records):
+        formatted = [self.format_record(r) for r in records]
         if self.json:
+            if self.include_id and not self.raw:
+                formatted = {record["id"]: record for record in formatted}
+                [record.pop("id") for record in formatted.values()]
             return formatted
         else:
             return "\n".join(formatted)
 
-
     def is_selected(self, pattern, text):
         if pattern is None:
             return True
         elif pattern.startswith("/"):
             return bool(re.match(pattern.strip("/"), text))
         else:
             return pattern == text
 
     def select_records(self, domain, type=None, host=None, content=None, priority=None):
 
-        if host and type!='ID' and not host.startswith("/"):
+        if host and type != "ID" and not host.startswith("/"):
             host = self.parse_host(host, domain)
 
         records = self.get_zone_records(domain)
 
         selected = []
 
         if type == "ID":
```

### Comparing `rstms_cloudflare-1.0.0/rstms_cloudflare/exception_handler.py` & `rstms_cloudflare-1.1.0/rstms_cloudflare/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/rstms_cloudflare/shell.py` & `rstms_cloudflare-1.1.0/rstms_cloudflare/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/tests/test_cli.py` & `rstms_cloudflare-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.0.0/PKG-INFO` & `rstms_cloudflare-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-cloudflare
-Version: 1.0.0
+Version: 1.1.0
 Summary: Top-level package for rstms-cloudflare.
 Keywords: rstms_cloudflare
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

