# Comparing `tmp/rstms_cloudflare-0.1.2.tar.gz` & `tmp/rstms_cloudflare-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_cloudflare-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_cloudflare-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_cloudflare-0.1.2.tar` & `rstms_cloudflare-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      383 2024-05-03 11:19:08.020962 rstms_cloudflare-0.1.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1338 2024-04-16 03:08:46.809802 rstms_cloudflare-0.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-0.1.2/LICENSE
--rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-0.1.2/Makefile
--rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-0.1.2/README.md
--rw-r--r--   0        0        0        6 2024-05-03 11:19:08.020962 rstms_cloudflare-0.1.2/VERSION
--rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.2/docs/Makefile
--rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.2/docs/cli.rst
--rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.2/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.2/docs/contributing.rst
--rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.2/docs/index.rst
--rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.2/docs/installation.rst
--rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.2/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-0.1.2/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.2/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-0.1.2/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-0.1.2/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.2/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.2/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-0.1.2/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-16 03:08:46.821802 rstms_cloudflare-0.1.2/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-0.1.2/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.2/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.2/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-0.1.2/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.2/make/version.mk
--rw-r--r--   0        0        0     1159 2024-05-03 11:19:08.020962 rstms_cloudflare-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-0.1.2/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-03 11:19:07.776964 rstms_cloudflare-0.1.2/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-03 11:19:07.836964 rstms_cloudflare-0.1.2/requirements-docs.txt
--rw-r--r--   0        0        0       19 2024-05-03 11:19:07.720965 rstms_cloudflare-0.1.2/requirements.txt
--rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-0.1.2/rstms_cloudflare/__init__.py
--rw-r--r--   0        0        0     5813 2024-05-03 11:17:39.421870 rstms_cloudflare-0.1.2/rstms_cloudflare/cli.py
--rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-0.1.2/rstms_cloudflare/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-0.1.2/rstms_cloudflare/shell.py
--rw-r--r--   0        0        0      127 2024-05-03 11:19:08.020962 rstms_cloudflare-0.1.2/rstms_cloudflare/version.py
--rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-0.1.2/tests/test_cli.py
--rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-0.1.2/tox.ini
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      383 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1338 2024-04-16 03:08:46.809802 rstms_cloudflare-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.0.0/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.0.0/Makefile
+-rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.0.0/README.md
+-rw-r--r--   0        0        0        6 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/VERSION
+-rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.0.0/docs/cli.rst
+-rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.0.0/docs/contributing.rst
+-rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/index.rst
+-rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/installation.rst
+-rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.0.0/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.0.0/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.0.0/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.0.0/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.0.0/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.0.0/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.0.0/make/docs.mk
+-rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.0.0/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-1.0.0/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.0.0/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.0.0/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.0.0/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.0.0/make/version.mk
+-rw-r--r--   0        0        0     1159 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.0.0/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-21 01:03:15.065281 rstms_cloudflare-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-21 01:03:15.121280 rstms_cloudflare-1.0.0/requirements-docs.txt
+-rw-r--r--   0        0        0       19 2024-05-21 01:03:15.009281 rstms_cloudflare-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.0.0/rstms_cloudflare/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-21 00:42:18.598476 rstms_cloudflare-1.0.0/rstms_cloudflare/cli.py
+-rw-r--r--   0        0        0     5670 2024-05-21 00:53:29.275442 rstms_cloudflare-1.0.0/rstms_cloudflare/cloudflare.py
+-rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.0.0/rstms_cloudflare/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.0.0/rstms_cloudflare/shell.py
+-rw-r--r--   0        0        0      127 2024-05-21 01:03:15.209279 rstms_cloudflare-1.0.0/rstms_cloudflare/version.py
+-rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.0.0/tox.ini
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-1.0.0/PKG-INFO
```

### Comparing `rstms_cloudflare-0.1.2/.gitignore` & `rstms_cloudflare-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/LICENSE` & `rstms_cloudflare-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/Makefile` & `rstms_cloudflare-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/README.md` & `rstms_cloudflare-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/docs/Makefile` & `rstms_cloudflare-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/docs/conf.py` & `rstms_cloudflare-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/docs/installation.rst` & `rstms_cloudflare-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/docs/make.bat` & `rstms_cloudflare-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/clean.mk` & `rstms_cloudflare-1.0.0/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/common.mk` & `rstms_cloudflare-1.0.0/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/docs.mk` & `rstms_cloudflare-1.0.0/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/publish.mk` & `rstms_cloudflare-1.0.0/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/release.mk` & `rstms_cloudflare-1.0.0/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/test.mk` & `rstms_cloudflare-1.0.0/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/make/version.mk` & `rstms_cloudflare-1.0.0/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/pyproject.toml` & `rstms_cloudflare-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-cloudflare"
-version = "0.1.2"
+version = "1.0.0"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_cloudflare"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_cloudflare-0.1.2/rstms_cloudflare/cli.py` & `rstms_cloudflare-1.0.0/rstms_cloudflare/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,22 @@
 """Console script for rstms_cloudflare."""
 
-import json
 import sys
+from pathlib import Path
 
 import click
 import click.core
-import CloudFlare
 
+from .cloudflare import API
 from .exception_handler import ExceptionHandler
 from .shell import _shell_completion
 from .version import __timestamp__, __version__
 
 header = f"{__name__.split('.')[0]} v{__version__} {__timestamp__}"
 
-RECORD_TYPES = ["A", "AAAA", "CNAME", "MX", "NS", "SOA", "TXT", "SRV", "LOC"]
-MAX_ZONES = 128
-
-
-def fail(msg):
-    click.echo(msg, err=True)
-    sys.exit(-1)
-
-
-def output(context, result):
-    if context.json:
-        click.echo(json.dumps(result))
-    else:
-        click.echo(result)
-
-
-def parse_name(name, domain):
-    if name == "@":
-        name = domain
-    else:
-        name = ".".join([name, domain])
-    name = name.strip(".")
-    return name
-
-
-def get_zones(context):
-    return context.client.zones.get(params={"per_page": MAX_ZONES})
-
-
-def get_zone_id(context, domain):
-    zones = get_zones(context)
-    for z in zones:
-        if z["name"] == domain:
-            return z["id"]
-    fail(f"domain not found: '{domain}'")
-
-
-def get_zone_records(context, domain):
-    records = {}
-    zone_id = get_zone_id(context, domain)
-    records = context.client.zones.dns_records.get(zone_id, params={"per_page": MAX_ZONES})
-    return records
-
-
-class Context:
-    def __init__(self):
-        pass
-
 
 def _ehandler(ctx, option, debug):
     ctx.obj = dict(ehandler=ExceptionHandler(debug))
     ctx.obj["debug"] = debug
 
 
 @click.group(name="cloudflare")
@@ -74,148 +26,190 @@
     "--shell-completion",
     is_flag=False,
     flag_value="[auto]",
     callback=_shell_completion,
     help="configure shell completion",
 )
 @click.option("-q", "--quiet", is_flag=True)
+@click.option("-v", "--verbose", is_flag=True)
 @click.option("-t", "--token", envvar="CLOUDFLARE_AUTH_TOKEN")
-@click.option("-d", "--domain", envvar="DOMAIN")
-@click.option("-i", "--instance", envvar="INSTANCE")
 @click.option("-j", "--json", is_flag=True)
+@click.option("-o", "--output", type=click.Path(writable=True, dir_okay=False, path_type=Path), help="output file")
 @click.pass_context
-def cli(ctx, debug, shell_completion, token, domain, instance, json, quiet):
-    ctx.obj = Context()
-    ctx.obj.client = CloudFlare.CloudFlare(token=token)
-    ctx.obj.domain = domain
-    ctx.obj.instance = instance
-    ctx.obj.json = json
-    ctx.obj.quiet = quiet
-
-
-def format_dns_record(r, record_id=False):
-    out = ''
-    if record_id:
-        out += f"{r['id']} "
-    out += f"{r['type']} "
-    if r["type"] == "MX":
-        out += f"{r['priority']} "
-    out += f"{r['name']} {r['content']} {r['ttl']}"
-    return out
+def cli(ctx, debug, shell_completion, token, json, quiet, verbose, output):
+    if output:
+        func = output.write_text
+    else:
+        func = click.echo
+    ctx.obj = API(token=token, json=json, quiet=quiet, verbose=verbose, output_function=func)
 
 
 @cli.command
-@click.option("-i", "--id", "record_id", is_flag=True, help='output record ID')
 @click.argument("domain", required=False)
-@click.argument("record_type", type=click.Choice(RECORD_TYPES), required=False)
-@click.argument("name", required=False)
 @click.pass_obj
-def list(context, domain, record_type, name, record_id):
-    if domain is None:
-        domain = context.domain
+def dump(api, domain):
+    """Output API data for one or all domains"""
+    data = {}
+    zones = api.get_zones()
+    for zone in zones:
+        if domain in [None, zone["name"]]:
+            data[zone["name"]] = api.get_zone_records(zone["name"])
+    if domain:
+        if not data:
+            raise ValueError(f"unknown domain: '{domain}'")
+
+    api.json = True
+    api.output(data)
+    sys.exit(0 if data else -1)
+
+
+def process_filter(arg, opt, name):
+    if arg and opt:
+        if arg == opt:
+            opt = None
+        else:
+            raise RuntimeError(f"{name} option conflicts with argument")
+    return arg or opt
+
 
-    zone_records = get_zone_records(context, domain)
+@cli.command
+@click.option("-i", "--id", "output_id", is_flag=True, help="output record ID")
+@click.option("--delete", "delete_records", is_flag=True, help="delete selected records")
+@click.option("--update-content", help="update selected record content")
+@click.option("--update-ttl", help="update selected record TTL")
+@click.option("-t", "--type", "filter_type", type=click.Choice(API.RECORD_TYPES + ["ID"]))
+@click.option("-h", "--host", "filter_host", help="match host or /regex/")
+@click.option("-c", "--content", "filter_content", help="match content or /regex/")
+@click.option("-p", "--priority", type=int, help="filter by MX priority")
+@click.argument("domain")
+@click.argument("type", type=click.Choice(API.RECORD_TYPES + ["ID"]), required=False)
+@click.argument("host", required=False)
+@click.argument("content", required=False)
+@click.pass_obj
+def records(
+    api,
+    domain,
+    type,
+    host,
+    content,
+    output_id,
+    filter_type,
+    filter_host,
+    filter_content,
+    delete_records,
+    priority,
+    update_content,
+    update_ttl,
+):
+    """select domain records"""
 
-    if name is not None:
-        name = ".".join([name, domain])
+    if domain is None:
+        domain = api.domain
 
-    records = []
-    for record in zone_records:
-        if record_type in [None, record["type"]]:
-            if name in [None, record["name"]]:
-                records.append(record)
+    type = process_filter(type, filter_type, "type")
+    host = process_filter(host, filter_host, "host")
+    content = process_filter(content, filter_content, "content")
 
-    if context.json:
-        click.echo(json.dumps(records))
-    else:
+    records = api.select_records(domain, type, host, content, priority)
+
+    if delete_records:
+        records = api.delete_records(records)
+    elif update_content or update_ttl:
         for record in records:
-            click.echo(format_dns_record(record, record_id))
+            if update_content:
+                record["content"] = update_content
+            if update_ttl:
+                record["ttl"] = update_ttl
+        records = api.update_records(records)
+    else:
+        records = api.format_records(records, output_id)
+
+    api.output(records)
+    sys.exit(0 if records else -1)
 
 
 @cli.command
 @click.pass_obj
-def domains(context):
-    zones = get_zones(context)
-    if context.json:
-        output(context, zones)
-    else:
-        for zone in zones:
-            click.echo(zone["name"])
+def domains(api):
+    """output registered domains"""
+    zones = [zone["name"] for zone in api.get_zones()]
+    if not api.json:
+        zones = "\n".join(zones)
+    api.output(zones)
+    sys.exit(0 if zones else -1)
 
 
 @cli.command
-@click.argument("domain", required=False)
+@click.argument("domain")
 @click.pass_obj
-def zone(context, domain):
-    if domain is None:
-        domain = context.domain
-
-    zone_id = get_zone_id(context, domain)
+def zone(api, domain):
+    """output zone file"""
 
-    click.echo(context.client.zones.dns_records.export(zone_id))
+    zone_id = api.get_zone_id(domain)
+    api.json = False
+    api.output(api.client.zones.dns_records.export(zone_id))
+    sys.exit(0)
 
 
 @cli.command
 @click.argument("domain")
-@click.argument("type", type=click.Choice(RECORD_TYPES))
-@click.argument("name")
+@click.argument("type", type=click.Choice(API.RECORD_TYPES))
+@click.argument("host")
 @click.argument("content")
 @click.option("-t", "--ttl", default=60)
 @click.option("-p", "--priority", default=10)
 @click.pass_obj
-def create(context, domain, type, name, content, ttl, priority):
-    zone_id = get_zone_id(context, domain)
-    name = parse_name(name, domain)
-    record = dict(type=type, name=name, content=content, ttl=ttl)
+def add(api, domain, type, host, content, ttl, priority):
+    """add a new record"""
+
     if type in ["A", "CNAME", "TXT"]:
-        pass
+        priority = None
     elif type == "MX":
-        record["priority"] = priority
+        priority = priority or 0
     else:
-        fail(f"Unsupported record type: {type}")
+        raise ValueError(f"Unsupported record type '{type}'")
 
-    ret = context.client.zones.dns_records.post(zone_id, data=record)
-
-    if context.json:
-        click.echo(json.dumps(ret))
-    else:
-        if not context.quiet:
-            click.echo(ret["id"])
+    added = api.add_record(domain, type, host, content, ttl, priority)
+    api.output(added)
+    sys.exit(0)
 
 
 @cli.command
 @click.option("-p", "--priority")
 @click.argument("domain")
-@click.argument("type", type=click.Choice(RECORD_TYPES + ["ID"]))
-@click.argument("name")
+@click.argument("type", type=click.Choice(API.RECORD_TYPES + ["ID"]))
+@click.argument("host")
+@click.argument("content", required=False)
 @click.pass_obj
-def delete(context, domain, type, name, priority):
-    records = get_zone_records(context, domain)
-    hostname = parse_name(name, domain)
-
-    for record in records:
-        if type == "ID":
-            if name != record["id"]:
-                continue
-        elif type == record["type"] and hostname == record["name"]:
-            if priority and (priority != record.get("priority", None)):
-                continue
-        else:
-            continue
-        record_id = record["id"]
-        zone_id = record["zone_id"]
-        ret = context.client.zones.dns_records.delete(zone_id, record_id)
-        if context.json:
-            click.echo(json.dumps(ret))
-        else:
-            if not context.quiet:
-                click.echo(ret["id"])
-        sys.exit(0)
+def delete(api, domain, type, host, content, priority):
+    """delete matching record"""
+    selected = api.select_records(domain, type, host, content, priority)
+    deleted = api.delete_records(selected)
+    api.output(deleted)
+    sys.exit(0 if deleted else -1)
 
-    if not context.quiet:
-        fail("record not found")
 
-    sys.exit(-1)
+@cli.command
+@click.option("-p", "--priority", type=int)
+@click.option("-t", "--ttl", type=int)
+@click.argument("domain")
+@click.argument("type", type=click.Choice(API.RECORD_TYPES + ["ID"]))
+@click.argument("host")
+@click.argument("content", required=False)
+@click.pass_obj
+def update(api, domain, type, host, content, priority, ttl):
+    """update matching record content"""
+    selected = api.select_records(domain, type, host, content, priority)
+    for record in selected:
+        if content:
+            record["content"] = content
+        if priority and record["type"] == "MX":
+            record["priority"] = content
+        if ttl:
+            record["ttl"] = ttl
+    updated = api.update_records(selected)
+    api.output(updated)
+    sys.exit(0 if updated else -1)
 
 
 if __name__ == "__main__":
     sys.exit(cli())
```

### Comparing `rstms_cloudflare-0.1.2/rstms_cloudflare/exception_handler.py` & `rstms_cloudflare-1.0.0/rstms_cloudflare/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/rstms_cloudflare/shell.py` & `rstms_cloudflare-1.0.0/rstms_cloudflare/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/tests/test_cli.py` & `rstms_cloudflare-1.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.2/PKG-INFO` & `rstms_cloudflare-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-cloudflare
-Version: 0.1.2
+Version: 1.0.0
 Summary: Top-level package for rstms-cloudflare.
 Keywords: rstms_cloudflare
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

