# Comparing `tmp/tinyticker-0.5.6.tar.gz` & `tmp/tinyticker-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.6.tar", max compression
+gzip compressed data, was "tinyticker-0.5.7.tar", max compression
```

## Comparing `tinyticker-0.5.6.tar` & `tinyticker-0.5.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-20 00:08:45.326101 tinyticker-0.5.6/LICENSE
--rw-r--r--   0        0        0     3858 2024-05-20 00:08:45.326101 tinyticker-0.5.6/README.md
--rw-r--r--   0        0        0      917 2024-05-20 00:08:45.326101 tinyticker-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/__init__.py
--rw-r--r--   0        0        0     6196 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/__main__.py
--rw-r--r--   0        0        0     1773 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/config.py
--rw-r--r--   0        0        0     8759 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/paths.py
--rw-r--r--   0        0        0    15609 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/ticker.py
--rw-r--r--   0        0        0     2391 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     1283 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6610 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    14553 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1573 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1369 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-21 00:26:08.488720 tinyticker-0.5.7/LICENSE
+-rw-r--r--   0        0        0     3858 2024-05-21 00:26:08.488720 tinyticker-0.5.7/README.md
+-rw-r--r--   0        0        0      917 2024-05-21 00:26:08.488720 tinyticker-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6145 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2470 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/config.py
+-rw-r--r--   0        0        0     8857 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/paths.py
+-rw-r--r--   0        0        0    15609 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/ticker.py
+-rw-r--r--   0        0        0     2391 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-21 00:26:08.492720 tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     1283 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6643 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14553 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1573 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1369 2024-05-21 00:26:08.496720 tinyticker-0.5.7/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.7/PKG-INFO
```

### Comparing `tinyticker-0.5.6/LICENSE` & `tinyticker-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/README.md` & `tinyticker-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/pyproject.toml` & `tinyticker-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.6"
+version = "0.5.7"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.5.6/tinyticker/__main__.py` & `tinyticker-0.5.7/tinyticker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from time import sleep
 from typing import List
 
 from watchdog.events import FileModifiedEvent, FileSystemEventHandler
 from watchdog.observers import Observer
 
 from . import __version__, logger
-from .config import TinytickerConfig
+from .config import load_config_safe
 from .display import Display
 from .paths import CONFIG_FILE, PID_FILE
 from .ticker import Sequence
 from .utils import RawTextArgumentDefaultsHelpFormatter, set_verbosity
 
 
 def parse_args(args: List[str]) -> argparse.Namespace:
@@ -70,15 +70,15 @@
     """Start ticking.
 
     Args:
         config_file: config file path.
     """
     logger.info("Starting ticker process")
     # Read config values
-    tt_config = TinytickerConfig.from_file(config_file)
+    tt_config = load_config_safe(config_file)
 
     display = Display.from_tinyticker_config(tt_config)
     sequence = Sequence.from_tinyticker_config(tt_config)
     logger.debug(sequence)
 
     try:
         for ticker, resp in sequence.start():
@@ -121,25 +121,24 @@
             show=True,
             weight="bold",
             fontsize="small",
         )
 
 
 def main():
+    logger.info("Tinyticker version: %s", __version__)
     args = parse_args(sys.argv[1:])
     config_file: Path = args.config
 
     if args.verbose > 0:
         set_verbosity(logger, args.verbose)
 
-    # if the config file is not present, write the default values
-    if not config_file.is_file():
-        config_file.parent.mkdir(parents=True)
-        # write defaults to file
-        TinytickerConfig().to_file(config_file)
+    # make sure the config file exists and can be parsed before setting up the file
+    # monitor
+    load_config_safe(config_file)
 
     # write the process pid to file.
     pid = os.getpid()
     logger.info("PID file: %s", PID_FILE)
     logger.info("PID: %s", pid)
     if not PID_FILE.parent.is_dir():
         PID_FILE.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `tinyticker-0.5.6/tinyticker/display.py` & `tinyticker-0.5.7/tinyticker/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Args:
         model: epd model name.
         flip: Flip the display.
     """
 
     @classmethod
     def from_tinyticker_config(cls, tt_config: TinytickerConfig) -> "Display":
+        """Create a `Display` object from a `TinytickerConfig` object."""
         return cls(model=tt_config.epd_model, flip=tt_config.flip)
 
     def __init__(
         self,
         model: str = "EPD_v2",
         flip: bool = False,
     ) -> None:
@@ -148,15 +149,15 @@
                 self.epd.getbuffer(image),
                 self.epd.getbuffer(highlight) if highlight is not None else None,
             )
         else:
             self.epd.display(self.epd.getbuffer(image))
 
     def show_image(self, image: Image.Image) -> None:
-        """Show a `PIL.Image.Image` on the display.
+        """Show a `PIL.Image.Image` on the display and put it to sleep.
 
         Args:
             image: The image to display.
         """
         highlight_image = None
         if self.has_highlight and image.mode == "RGB":
             self._log.info("Computing highlight pixels.")
@@ -193,15 +194,15 @@
         top_string: Optional[str] = None,
         sub_string: Optional[str] = None,
         show: bool = False,
         type: str = "candle",
         volume: bool = False,
         **kwargs,
     ) -> Tuple[Figure, Axes]:
-        """Plot symbol historical data chart.
+        """Plot an asset's historical data chart.
 
         Args:
             historical: API response, `pd.DataFrame` containing the historical
                 price of the symbol.
             top_string: Contents of the top left string, '{}' will be replaced with the current
                 price.
             sub_string: Contents of a smaller text box below `top_string`.
```

### Comparing `tinyticker-0.5.6/tinyticker/ticker.py` & `tinyticker-0.5.7/tinyticker/ticker.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/utils.py` & `tinyticker-0.5.7/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/device.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.7/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/__main__.py` & `tinyticker-0.5.7/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/app.py` & `tinyticker-0.5.7/tinyticker/web/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 import threading
 from pathlib import Path
 from typing import Optional
 
 from flask import Flask, abort, redirect, render_template, request, send_from_directory
 
 from .. import __version__
-from ..config import PLOT_TYPES, SequenceConfig, TickerConfig, TinytickerConfig
+from ..config import (
+    PLOT_TYPES,
+    SequenceConfig,
+    TickerConfig,
+    TinytickerConfig,
+    load_config_safe,
+)
 from ..paths import CONFIG_FILE, LOG_DIR
 from ..ticker import INTERVAL_LOOKBACKS, INTERVAL_TIMEDELTAS, SYMBOL_TYPES
 from ..waveshare_lib.models import MODELS
 from .command import COMMANDS, reboot
 
 LOGGER = logging.getLogger(__name__)
 TEMPLATE_PATH = str(Path(__file__).parent / "templates")
@@ -65,15 +71,15 @@
     @app.after_request
     def add_header(response):
         response.cache_control.max_age = 0
         return response
 
     @app.route("/")
     def index():
-        tt_config = TinytickerConfig.from_file(config_file)
+        tt_config = load_config_safe(config_file)
         return render_template(
             "index.html",
             hostname=hostname,
             commands=commands,
             plot_type_options=PLOT_TYPES,
             symbol_type_options=SYMBOL_TYPES,
             interval_lookbacks=INTERVAL_LOOKBACKS,
```

### Comparing `tinyticker-0.5.6/tinyticker/web/command.py` & `tinyticker-0.5.7/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.7/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.7/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.7/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.7/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/index.html` & `tinyticker-0.5.7/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.7/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.7/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.7/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.7/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.6/PKG-INFO` & `tinyticker-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.6
+Version: 0.5.7
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
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.6 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.7 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

