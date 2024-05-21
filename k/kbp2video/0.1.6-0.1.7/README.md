# Comparing `tmp/kbp2video-0.1.6.tar.gz` & `tmp/kbp2video-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbp2video-0.1.6.tar", last modified: Mon May 13 03:35:44 2024, max compression
+gzip compressed data, was "kbp2video-0.1.7.tar", last modified: Tue May 21 04:39:19 2024, max compression
```

## Comparing `kbp2video-0.1.6.tar` & `kbp2video-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-13 03:35:44.047607 kbp2video-0.1.6/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-05-13 01:35:06.000000 kbp2video-0.1.6/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-13 03:35:44.047607 kbp2video-0.1.6/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-05-13 01:35:06.000000 kbp2video-0.1.6/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-13 03:35:44.047607 kbp2video-0.1.6/kbp2video/
--rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-13 03:35:28.000000 kbp2video-0.1.6/kbp2video/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-05-13 01:35:06.000000 kbp2video-0.1.6/kbp2video/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-05-13 01:35:06.000000 kbp2video-0.1.6/kbp2video/_ffmpegcolor.py
--rw-r--r--   0 matt      (1000) matt      (1000)    80442 2024-05-13 03:32:45.000000 kbp2video-0.1.6/kbp2video/_gui.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-05-13 01:35:06.000000 kbp2video-0.1.6/kbp2video/advanced_editor.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-05-13 01:35:06.000000 kbp2video-0.1.6/kbp2video/utils.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-13 03:35:44.047607 kbp2video-0.1.6/kbp2video.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-13 03:35:44.000000 kbp2video-0.1.6/kbp2video.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-13 03:35:44.000000 kbp2video-0.1.6/kbp2video.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-13 03:35:44.000000 kbp2video-0.1.6/kbp2video.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-13 03:35:44.000000 kbp2video-0.1.6/kbp2video.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       65 2024-05-13 03:35:44.000000 kbp2video-0.1.6/kbp2video.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-13 03:35:44.000000 kbp2video-0.1.6/kbp2video.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      433 2024-05-13 01:35:06.000000 kbp2video-0.1.6/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-13 03:35:44.047607 kbp2video-0.1.6/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 04:39:19.188326 kbp2video-0.1.7/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-05-13 01:35:06.000000 kbp2video-0.1.7/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-21 04:39:19.184992 kbp2video-0.1.7/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-05-13 01:35:06.000000 kbp2video-0.1.7/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 04:39:19.184992 kbp2video-0.1.7/kbp2video/
+-rw-r--r--   0 matt      (1000) matt      (1000)      312 2024-05-21 04:39:02.000000 kbp2video-0.1.7/kbp2video/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/_ffmpegcolor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    81159 2024-05-21 04:39:02.000000 kbp2video-0.1.7/kbp2video/_gui.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/advanced_editor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-05-13 01:35:06.000000 kbp2video-0.1.7/kbp2video/utils.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-05-21 04:39:19.184992 kbp2video-0.1.7/kbp2video.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      200 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       65 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-05-21 04:39:19.000000 kbp2video-0.1.7/kbp2video.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      433 2024-05-21 04:39:02.000000 kbp2video-0.1.7/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-05-21 04:39:19.188326 kbp2video-0.1.7/setup.cfg
```

### Comparing `kbp2video-0.1.6/LICENSE` & `kbp2video-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.6/kbp2video/_ffmpegcolor.py` & `kbp2video-0.1.7/kbp2video/_ffmpegcolor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.6/kbp2video/_gui.py` & `kbp2video-0.1.7/kbp2video/_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -764,14 +764,18 @@
 
         gridRow += 1
         #self.gridLayout.addWidget(self.bind("transparencyBox", QCheckBox(checkState=Qt.Checked if self.settings.value("subtitle/transparent_bg", type=bool, defaultValue=True) else Qt.Unchecked)), gridRow, 0, alignment=Qt.AlignRight)
         self.gridLayout.addWidget(self.bind("transparencyBox", QCheckBox()), gridRow, 0, alignment=Qt.AlignRight)
         self.gridLayout.addWidget(self.bind("transparencyLabel", ClickLabel(buddy=self.transparencyBox, buddyMethod=QCheckBox.toggle)), gridRow, 1, 1, 2)
 
         gridRow += 1
+        self.gridLayout.addWidget(self.bind("ktBox", QCheckBox()), gridRow, 0, alignment=Qt.AlignRight)
+        self.gridLayout.addWidget(self.bind("ktLabel", ClickLabel(buddy=self.ktBox, buddyMethod=QCheckBox.toggle)), gridRow, 1, 1, 2)
+
+        gridRow += 1
         self.gridLayout.addWidget(
             self.bind("overflowBox", QComboBox()), gridRow, 1, 1, 2)
         self.gridLayout.addWidget(
             self.bind("overflowLabel", ClickLabel(buddy=self.overflowBox)), gridRow, 0)
         self.overflowBox.addItems(["no wrap","even split","top split","bottom split"])
 
         gridRow += 1
@@ -1065,14 +1069,15 @@
         to_save = {
             "subtitle/aspect_ratio": self.aspectRatioBox.currentText(),
             "subtitle/fade_in": self.fadeIn.value(),
             "subtitle/fade_out": self.fadeOut.value(),
             "subtitle/offset": self.offset.value(),
             "subtitle/override_offset": check2bool(self.overrideOffset),
             "subtitle/transparent_bg": check2bool(self.transparencyBox),
+            "subtitle/allow_kt": check2bool(self.ktBox),
             "subtitle/overflow": self.overflowBox.currentText(),
             "video/background_color": self.colorText.text(),
             "video/output_resolution": self.resolutionBox.currentText(),
             "video/override_bg_resolution": check2bool(self.overrideBGResolution),
             "video/container_format_index": self.containerBox.currentIndex(),
             "video/video_codec_index": self.vcodecBox.currentIndex(),
             "video/lossless": check2bool(self.lossless),
@@ -1104,14 +1109,15 @@
             self.aspectRatioBox.setCurrentText(aspect_text)
 
         self.fadeIn.setValue(self.settings.value("subtitle/fade_in", type=int, defaultValue=50))
         self.fadeOut.setValue(self.settings.value("subtitle/fade_out", type=int, defaultValue=50))
         self.offset.setValue(self.settings.value("subtitle/offset", type=float, defaultValue=0.0))
         self.offset_check_box(setState=bool2check(self.settings.value("subtitle/override_offset", type=bool, defaultValue=False)))
         self.transparencyBox.setCheckState(bool2check(self.settings.value("subtitle/transparent_bg", type=bool, defaultValue=True)))
+        self.ktBox.setCheckState(bool2check(self.settings.value("subtitle/allow_kt", type=bool, defaultValue=False)))
         self.overflowBox.setCurrentText(self.settings.value("subtitle/overflow", type=str, defaultValue="no wrap"))
         self.updateColor(setColor=self.settings.value("video/background_color", type=str, defaultValue="#000000"))
 
         # Restore existing or custom option
         resolution_text = self.settings.value("video/output_resolution", type=str, defaultValue="<NONEXISTENT>")
         if (index := self.resolutionBox.findText(resolution_text)) != -1:
             self.resolutionBox.setCurrentIndex(index)
@@ -1206,15 +1212,14 @@
 
     @Slot(str, str)
     def info(self, title, text):
         QMessageBox.information(self, title, text)
 
     def conversion_runner(self, signals, assOnly = False):
         unsupported_message = False
-        assOptions = ["-f"]
         kbputils_options = {}
         ratio, border = self.get_aspect_ratio()
         if ratio[0] is None or border is None:
             QMetaObject.invokeMethod(
                 self,
                 'info', 
                 Qt.AutoConnection,
@@ -1237,28 +1242,24 @@
             kbputils_options['target_x'] = tmp[0]
             kbputils_options['target_y'] = int(tmp[0] * ratio[1] / ratio[0])
         else:
             kbputils_options['target_y'] = tmp[1]
             kbputils_options['target_x'] = int(tmp[1] * ratio[0] / ratio[1])
         width = round((216 if border else 192) * ratio[0] / ratio[1])
         default_bg = self.colorText.text().strip(" #")
-        if width != 300:
-            assOptions += ["-W", f"{width}"]
         if not border:
-            assOptions += ["--no-b"]
             kbputils_options['border'] = False
-        assOptions += ["-F", f"{self.fadeIn.value()},{self.fadeOut.value()}"]
         kbputils_options['fade_in'] = self.fadeIn.value()
         kbputils_options['fade_out'] = self.fadeOut.value()
         if self.overrideOffset.checkState() == Qt.Checked:
-            assOptions += ["-o", f"{self.offset.value()}"]
             kbputils_options['offset'] = self.offset.value()
         if self.transparencyBox.checkState() != Qt.Checked:
-            assOptions += ["--no-t"]
             kbputils_options['transparency'] = False
+        if self.ktBox.checkState() == Qt.Checked:
+            kbputils_options['allow_kt'] = True
         kbputils_options['overflow'] = kbputils.AssOverflow[self.overflowBox.currentText().replace(" ", "_").upper()]
         conversion_errors = False
         for row in range(self.tableWidget.rowCount()):
             kbp_table_item = self.tableWidget.item(row, TrackTableColumn.KBP_ASS.value)
             kbp_obj = kbp_table_item.data(Qt.UserRole) or kbp_table_item.text()
             kbp = str(kbp_obj)
             audio = self.tableWidget.filename(row, TrackTableColumn.Audio.value)
@@ -1560,14 +1561,18 @@
             "MainWindow", "&Fade In/Out", None))
         self.aspectLabel.setText(QCoreApplication.translate(
             "MainWindow", "A&spect Ratio", None))
         self.transparencyLabel.setText(QCoreApplication.translate(
             "MainWindow", "&Draw BG color transparent", None))
         self.transparencyLabel.setToolTip(QCoreApplication.translate(
             "MainWindow", "When using palette index 0 as a font or border color in KBS, make that color\ntransparent in the resulting .ass file. This improves compatibility with\ndrawing appearing and overlapping text. ", None))
+        self.ktLabel.setText(QCoreApplication.translate(
+            "MainWindow", "Use \\&kt to allow overlapping wipes", None))
+        self.ktLabel.setToolTip(QCoreApplication.translate(
+            "MainWindow", "When wipes overlap on the same line, handle it by adding \\kt tags\nto show the wipes at their chosen times. Note that\n1) This is different from KBS that just tries to wipe it fast after the previous wipe\n2) It's not supported by some ASS tools, including Aegisub.", None))
         self.overflowLabel.setText(QCoreApplication.translate(
             "MainWindow", "Word Wrappin&g", None))
         self.overflowBox.setToolTip(QCoreApplication.translate(
             "MainWindow", "When a line is too wide for the screen, use this strategy to wrap words\n  no wrap: Allow text to go off screen\n  even split: Wrap words in a way that makes the following line(s) about the same size\n  top split: Keep the first line long, only wrap at the word that causes it to go offscreen\n  bottom split: Make the bottom line long when wrapping", None))
         self.overrideOffsetLabel.setText(QCoreApplication.translate(
             "MainWindow", "Overr&ide Timestamp Offset", None))
         self.overrideOffsetLabel.setToolTip(QCoreApplication.translate(
```

### Comparing `kbp2video-0.1.6/kbp2video/advanced_editor.py` & `kbp2video-0.1.7/kbp2video/advanced_editor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.6/kbp2video/utils.py` & `kbp2video-0.1.7/kbp2video/utils.py`

 * *Files identical despite different names*

