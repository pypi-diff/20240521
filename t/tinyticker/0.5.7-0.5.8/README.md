# Comparing `tmp/tinyticker-0.5.7.tar.gz` & `tmp/tinyticker-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.7.tar", max compression
+gzip compressed data, was "tinyticker-0.5.8.tar", max compression
```

## Comparing `tinyticker-0.5.7.tar` & `tinyticker-0.5.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-21 00:26:08.488720 tinyticker-0.5.7/LICENSE
--rw-r--r--   0        0        0     3858 2024-05-21 00:26:08.488720 tinyticker-0.5.7/README.md
--rw-r--r--   0        0        0      917 2024-05-21 00:26:08.488720 tinyticker-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/__init__.py
--rw-r--r--   0        0        0     6145 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/__main__.py
--rw-r--r--   0        0        0     2470 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/config.py
--rw-r--r--   0        0        0     8857 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/paths.py
--rw-r--r--   0        0        0    15609 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/ticker.py
--rw-r--r--   0        0        0     2391 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     1283 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6643 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    14553 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1573 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1369 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-21 01:55:21.895522 tinyticker-0.5.8/LICENSE
+-rw-r--r--   0        0        0     3858 2024-05-21 01:55:21.895522 tinyticker-0.5.8/README.md
+-rw-r--r--   0        0        0      917 2024-05-21 01:55:21.895522 tinyticker-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6145 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2470 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/config.py
+-rw-r--r--   0        0        0     8857 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/paths.py
+-rw-r--r--   0        0        0    15671 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/ticker.py
+-rw-r--r--   0        0        0     2391 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     1283 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6643 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14553 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1573 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2349 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.8/PKG-INFO
```

### Comparing `tinyticker-0.5.7/LICENSE` & `tinyticker-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/README.md` & `tinyticker-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/pyproject.toml` & `tinyticker-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.7"
+version = "0.5.8"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.5.7/tinyticker/__main__.py` & `tinyticker-0.5.8/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/config.py` & `tinyticker-0.5.8/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/display.py` & `tinyticker-0.5.8/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/ticker.py` & `tinyticker-0.5.8/tinyticker/ticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,14 +430,15 @@
                         (utils.now() - response.historical.index[-1])  # type: ignore
                         > outdated_min_delta
                     ):
                         LOGGER.debug(f"{ticker} response outdated, skipping.")
                         continue
                 all_skipped = False
                 yield (ticker, response)
+                LOGGER.info(f"Sleeping {ticker.wait_time}s.")
                 time.sleep(ticker.wait_time)
 
     def __str__(self):
         return (
             f"Sequence(skip_outdated={self.skip_outdated}, skip_empty={self.skip_empty}): \n"
             + "\n".join([ticker.__str__() for ticker in self.tickers])
         )
```

### Comparing `tinyticker-0.5.7/tinyticker/utils.py` & `tinyticker-0.5.8/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/device.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.8/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/__main__.py` & `tinyticker-0.5.8/tinyticker/web/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 from ..display import Display
 from ..paths import CONFIG_FILE, LOG_DIR
 from ..utils import (
     RawTextArgumentDefaultsHelpFormatter,
     dashboard_qrcode,
     set_verbosity,
 )
-from .app import LOGGER as APP_LOGGER
+from . import logger
 from .app import create_app
 
-LOGGER = logging.getLogger(__name__)
-
 
 def parse_args(args: List[str]) -> argparse.Namespace:
     """Parse the command line arguments.
 
     Args:
         args: The command line arguments.
 
@@ -68,39 +66,40 @@
         default=LOG_DIR,
     )
     return parser.parse_args(args)
 
 
 def main():
     args = parse_args(sys.argv[1:])
+    # this stops the logger from double logging for some reason
+    logger.propagate = False
     if args.verbose > 0:
-        set_verbosity(LOGGER, args.verbose)
-        set_verbosity(APP_LOGGER, args.verbose)
+        set_verbosity(logger, args.verbose)
 
-    LOGGER.debug("Args: %s", args)
+    logger.debug("Args: %s", args)
 
     if not args.log_dir.is_dir():
         args.log_dir.mkdir(parents=True)
 
     if args.show_qrcode:
-        LOGGER.info("Generating qrcode.")
+        logger.info("Generating qrcode.")
         tt_config = TinytickerConfig.from_file(args.config)
         display = Display.from_tinyticker_config(tt_config)
         qrcode = dashboard_qrcode(
             display.epd.width,
             display.epd.height,
             args.port,
         )
-        LOGGER.info("Displaying qrcode.")
+        logger.info("Displaying qrcode.")
         display.show_image(qrcode)
         del display
         sys.exit()
 
-    LOGGER.info("Starting tinyticker-web")
+    logger.info("Starting tinyticker-web")
     app = create_app(config_file=args.config, log_dir=args.log_dir)
     serve(app, port=args.port)
     # app.run(host="0.0.0.0", port=args.port, debug=False, threaded=True)
-    LOGGER.info("Stopping tinyticker-web")
+    logger.info("Stopping tinyticker-web")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tinyticker-0.5.7/tinyticker/web/app.py` & `tinyticker-0.5.8/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/command.py` & `tinyticker-0.5.8/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.8/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.8/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.8/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.8/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/index.html` & `tinyticker-0.5.8/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.8/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.8/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.8/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.7/PKG-INFO` & `tinyticker-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.7
+Version: 0.5.8
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.7 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.8 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

