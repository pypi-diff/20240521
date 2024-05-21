# Comparing `tmp/pyppeteerstealth-0.0.3.tar.gz` & `tmp/pyppeteerstealth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppeteerstealth-0.0.3.tar", max compression
+gzip compressed data, was "pyppeteerstealth-0.0.4.tar", max compression
```

## Comparing `pyppeteerstealth-0.0.3.tar` & `pyppeteerstealth-0.0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1404 2024-02-20 18:34:12.064331 pyppeteerstealth-0.0.3/README.md
--rw-r--r--   0        0        0    34890 2024-02-20 18:34:12.068331 pyppeteerstealth-0.0.3/pyppeteerstealth/__init__.py
--rw-r--r--   0        0        0     1318 2024-02-20 18:34:12.068331 pyppeteerstealth-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pyppeteerstealth-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1666 2024-05-21 09:41:22.259361 pyppeteerstealth-0.0.4/README.md
+-rw-r--r--   0        0        0    34968 2024-05-21 09:41:22.263362 pyppeteerstealth-0.0.4/pyppeteerstealth/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-21 09:41:22.263362 pyppeteerstealth-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 pyppeteerstealth-0.0.4/PKG-INFO
```

### Comparing `pyppeteerstealth-0.0.3/README.md` & `pyppeteerstealth-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # pyppeteerstealth
 
 A bunch of hacks from different websites
 
-**Does not yet pass https://arh.antoinevastel.com/bots/areyouheadless**
+## Note!
+- **Does not yet pass https://arh.antoinevastel.com/bots/areyouheadless** please help!
+- Probably wont help where sites are using https://developer.mozilla.org/en-US/docs/Web/API/User-Agent_Client_Hints_API (`navigator.userAgentData.brands` etc)
 
-If you know what is missing, please make a PR!
+__**If you know what is missing, please make a PR!!!**__
 
 If you compare loading https://arh.antoinevastel.com/bots/ in your application, versus in your browser you might be able
 to see what is required to get the fingerprint closer to a "normal" browser (further away from a "headless" browser)
 
 This is intended to be used with https://github.com/dgtlmoon/pyppeteer-ng and is also part of the 
 https://changedetection.io project.
 
 ```python
 browser = await pyppeteer_instance.connect(browserWSEndpoint="ws://127.0.0.1:3000",
                                            ignoreHTTPSErrors=True
                                            )
 
 self.page = (pages := await browser.pages) and len(pages) or await browser.newPage()
-await self.page.setUserAgent("Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36")
+# Should be set with setUserAgent
+user_agent = next((value for key, value in request_headers.items() if key.lower().strip() == 'user-agent'), DEFAULT_USER_AGENT)
+await self.page.setUserAgent(user_agent)
 
 try:
     from pyppeteerstealth import inject_evasions_into_page
 except ImportError:
     logger.debug("pyppeteerstealth module not available, skipping")
     pass
 else:
```

### Comparing `pyppeteerstealth-0.0.3/pyppeteerstealth/__init__.py` & `pyppeteerstealth-0.0.4/pyppeteerstealth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     #    Will likely need to add:
     #    - navigator.platform
     #    - Different vendor/renderer names (DirectX vs Mesa) for WebGL getParameter
     #    - Different codec support (untested)
     #    - Different avail/inner/outer widths/heights because Windows has a different size taskbar and other things
     #    - Widevine plugin
     #    */
-    await page.setExtraHTTPHeaders({"DNT": "1"});
+
+# Doesn't really help and results in errors from scraping browser providers
+#    await page.setExtraHTTPHeaders({"DNT": "1"});
 
     # Puppeteer defines languages to be "" for some reason
     # https://pptr.dev/api/puppeteer.page.evaluateRawOnNewDocument
     await page.evaluateRawOnNewDocument('''Object.defineProperty(navigator, "languages", {
                   get: function() {
                     return ["en-GB", "en"]
                   }
```

### Comparing `pyppeteerstealth-0.0.3/pyproject.toml` & `pyppeteerstealth-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyppeteerstealth"
-version = "0.0.3"
+version = "0.0.4"
 description = "A general collection of robot-evading tweaks for pyppeteer-ng"
 readme = 'README.md'
 license = "MIT"
 homepage = "https://github.com/dgtlmoon/pyppeteerstealth"
 repository = "https://github.com/dgtlmoon/pyppeteerstealth"
 keywords=['pyppeteer', 'puppeteer', 'chrome', 'chromium', 'pyppeteerstealth', 'stealth', 'robot', 'captcha']
 authors = [
```

### Comparing `pyppeteerstealth-0.0.3/PKG-INFO` & `pyppeteerstealth-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppeteerstealth
-Version: 0.0.3
+Version: 0.0.4
 Summary: A general collection of robot-evading tweaks for pyppeteer-ng
 Home-page: https://github.com/dgtlmoon/pyppeteerstealth
 License: MIT
 Keywords: pyppeteer,puppeteer,chrome,chromium,pyppeteerstealth,stealth,robot,captcha
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,31 +25,35 @@
 Project-URL: Repository, https://github.com/dgtlmoon/pyppeteerstealth
 Description-Content-Type: text/markdown
 
 # pyppeteerstealth
 
 A bunch of hacks from different websites
 
-**Does not yet pass https://arh.antoinevastel.com/bots/areyouheadless**
+## Note!
+- **Does not yet pass https://arh.antoinevastel.com/bots/areyouheadless** please help!
+- Probably wont help where sites are using https://developer.mozilla.org/en-US/docs/Web/API/User-Agent_Client_Hints_API (`navigator.userAgentData.brands` etc)
 
-If you know what is missing, please make a PR!
+__**If you know what is missing, please make a PR!!!**__
 
 If you compare loading https://arh.antoinevastel.com/bots/ in your application, versus in your browser you might be able
 to see what is required to get the fingerprint closer to a "normal" browser (further away from a "headless" browser)
 
 This is intended to be used with https://github.com/dgtlmoon/pyppeteer-ng and is also part of the 
 https://changedetection.io project.
 
 ```python
 browser = await pyppeteer_instance.connect(browserWSEndpoint="ws://127.0.0.1:3000",
                                            ignoreHTTPSErrors=True
                                            )
 
 self.page = (pages := await browser.pages) and len(pages) or await browser.newPage()
-await self.page.setUserAgent("Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36")
+# Should be set with setUserAgent
+user_agent = next((value for key, value in request_headers.items() if key.lower().strip() == 'user-agent'), DEFAULT_USER_AGENT)
+await self.page.setUserAgent(user_agent)
 
 try:
     from pyppeteerstealth import inject_evasions_into_page
 except ImportError:
     logger.debug("pyppeteerstealth module not available, skipping")
     pass
 else:
```

