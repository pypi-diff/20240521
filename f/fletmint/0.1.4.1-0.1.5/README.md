# Comparing `tmp/fletmint-0.1.4.1.tar.gz` & `tmp/fletmint-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fletmint-0.1.4.1.tar", last modified: Tue May 14 14:37:59 2024, max compression
+gzip compressed data, was "fletmint-0.1.5.tar", last modified: Tue May 21 07:42:24 2024, max compression
```

## Comparing `fletmint-0.1.4.1.tar` & `fletmint-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 14:37:59.040021 fletmint-0.1.4.1/
--rw-rw-rw-   0        0        0     1476 2024-05-14 14:37:59.040021 fletmint-0.1.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 14:37:59.007814 fletmint-0.1.4.1/fletmint/
--rw-rw-rw-   0        0        0      618 2024-05-09 08:23:35.000000 fletmint-0.1.4.1/fletmint/__init__.py
--rw-rw-rw-   0        0        0     6402 2024-05-08 07:02:01.000000 fletmint-0.1.4.1/fletmint/audioplayer.py
--rw-rw-rw-   0        0        0     1042 2024-05-08 07:35:28.000000 fletmint-0.1.4.1/fletmint/badge.py
--rw-rw-rw-   0        0        0     5471 2024-05-14 12:43:49.000000 fletmint-0.1.4.1/fletmint/button.py
--rw-rw-rw-   0        0        0     4341 2024-05-08 16:20:00.000000 fletmint-0.1.4.1/fletmint/carousel.py
--rw-rw-rw-   0        0        0     5505 2024-05-07 07:52:05.000000 fletmint-0.1.4.1/fletmint/checkbox.py
--rw-rw-rw-   0        0        0    14078 2024-05-14 12:59:01.000000 fletmint-0.1.4.1/fletmint/datepicker.py
--rw-rw-rw-   0        0        0     7784 2024-05-09 07:55:00.000000 fletmint-0.1.4.1/fletmint/dropdown.py
--rw-rw-rw-   0        0        0     3875 2024-05-07 08:56:00.000000 fletmint-0.1.4.1/fletmint/profile.py
--rw-rw-rw-   0        0        0      408 2024-05-09 07:29:27.000000 fletmint-0.1.4.1/fletmint/radio.py
--rw-rw-rw-   0        0        0     1572 2024-05-07 14:45:09.000000 fletmint-0.1.4.1/fletmint/slider.py
--rw-rw-rw-   0        0        0     4954 2024-05-07 07:52:19.000000 fletmint-0.1.4.1/fletmint/stepper.py
--rw-rw-rw-   0        0        0     3558 2024-05-07 07:52:22.000000 fletmint-0.1.4.1/fletmint/tab_switch.py
--rw-rw-rw-   0        0        0     4007 2024-05-06 20:07:39.000000 fletmint-0.1.4.1/fletmint/table.py
--rw-rw-rw-   0        0        0     3297 2024-05-09 08:25:59.000000 fletmint-0.1.4.1/fletmint/tags_input.py
--rw-rw-rw-   0        0        0     5694 2024-05-07 07:50:29.000000 fletmint-0.1.4.1/fletmint/text_input.py
--rw-rw-rw-   0        0        0     3012 2024-05-07 15:21:55.000000 fletmint-0.1.4.1/fletmint/toggle.py
--rw-rw-rw-   0        0        0     3510 2024-05-07 14:46:28.000000 fletmint-0.1.4.1/fletmint/toggle_switch.py
--rw-rw-rw-   0        0        0     3739 2024-05-08 08:32:44.000000 fletmint-0.1.4.1/fletmint/videoplayer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 14:37:59.040021 fletmint-0.1.4.1/fletmint.egg-info/
--rw-rw-rw-   0        0        0     1476 2024-05-14 14:37:58.000000 fletmint-0.1.4.1/fletmint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-14 14:37:58.000000 fletmint-0.1.4.1/fletmint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 14:37:58.000000 fletmint-0.1.4.1/fletmint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 14:37:58.000000 fletmint-0.1.4.1/fletmint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 14:37:58.000000 fletmint-0.1.4.1/fletmint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 14:37:59.040021 fletmint-0.1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1200 2024-05-14 14:25:47.000000 fletmint-0.1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:42:24.942752 fletmint-0.1.5/
+-rw-rw-rw-   0        0        0     1474 2024-05-21 07:42:24.942752 fletmint-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 07:42:24.827151 fletmint-0.1.5/dev/
+-rw-rw-rw-   0        0        0        0 2024-05-15 12:14:21.000000 fletmint-0.1.5/dev/__init__.py
+-rw-rw-rw-   0        0        0    12450 2024-05-20 18:37:44.000000 fletmint-0.1.5/dev/code.py
+-rw-rw-rw-   0        0        0     4200 2024-05-15 12:08:34.000000 fletmint-0.1.5/dev/duration.py
+-rw-rw-rw-   0        0        0    14596 2024-05-19 12:38:11.000000 fletmint-0.1.5/dev/stht.py
+-rw-rw-rw-   0        0        0     4531 2024-05-15 09:33:05.000000 fletmint-0.1.5/dev/t.py
+-rw-rw-rw-   0        0        0    10666 2024-05-21 07:38:33.000000 fletmint-0.1.5/dev/timepicker.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:42:24.921284 fletmint-0.1.5/fletmint/
+-rw-rw-rw-   0        0        0      655 2024-05-21 07:39:51.000000 fletmint-0.1.5/fletmint/__init__.py
+-rw-rw-rw-   0        0        0     6402 2024-05-08 07:02:01.000000 fletmint-0.1.5/fletmint/audioplayer.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 07:35:28.000000 fletmint-0.1.5/fletmint/badge.py
+-rw-rw-rw-   0        0        0     5618 2024-05-16 06:03:43.000000 fletmint-0.1.5/fletmint/button.py
+-rw-rw-rw-   0        0        0     4341 2024-05-08 16:20:00.000000 fletmint-0.1.5/fletmint/carousel.py
+-rw-rw-rw-   0        0        0     5505 2024-05-07 07:52:05.000000 fletmint-0.1.5/fletmint/checkbox.py
+-rw-rw-rw-   0        0        0    13633 2024-05-21 07:11:05.000000 fletmint-0.1.5/fletmint/code.py
+-rw-rw-rw-   0        0        0    14844 2024-05-21 07:14:38.000000 fletmint-0.1.5/fletmint/datepicker.py
+-rw-rw-rw-   0        0        0     7784 2024-05-15 12:21:06.000000 fletmint-0.1.5/fletmint/dropdown.py
+-rw-rw-rw-   0        0        0     3875 2024-05-07 08:56:00.000000 fletmint-0.1.5/fletmint/profile.py
+-rw-rw-rw-   0        0        0      408 2024-05-09 07:29:27.000000 fletmint-0.1.5/fletmint/radio.py
+-rw-rw-rw-   0        0        0     1572 2024-05-07 14:45:09.000000 fletmint-0.1.5/fletmint/slider.py
+-rw-rw-rw-   0        0        0     4954 2024-05-07 07:52:19.000000 fletmint-0.1.5/fletmint/stepper.py
+-rw-rw-rw-   0        0        0     3847 2024-05-21 06:51:18.000000 fletmint-0.1.5/fletmint/tab_switch.py
+-rw-rw-rw-   0        0        0     4007 2024-05-06 20:07:39.000000 fletmint-0.1.5/fletmint/table.py
+-rw-rw-rw-   0        0        0     3297 2024-05-09 08:25:59.000000 fletmint-0.1.5/fletmint/tags_input.py
+-rw-rw-rw-   0        0        0     5694 2024-05-07 07:50:29.000000 fletmint-0.1.5/fletmint/text_input.py
+-rw-rw-rw-   0        0        0     3012 2024-05-07 15:21:55.000000 fletmint-0.1.5/fletmint/toggle.py
+-rw-rw-rw-   0        0        0     3510 2024-05-07 14:46:28.000000 fletmint-0.1.5/fletmint/toggle_switch.py
+-rw-rw-rw-   0        0        0     3739 2024-05-08 08:32:44.000000 fletmint-0.1.5/fletmint/videoplayer.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:42:24.941753 fletmint-0.1.5/fletmint.egg-info/
+-rw-rw-rw-   0        0        0     1474 2024-05-21 07:42:24.000000 fletmint-0.1.5/fletmint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      668 2024-05-21 07:42:24.000000 fletmint-0.1.5/fletmint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:42:24.000000 fletmint-0.1.5/fletmint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 07:42:24.000000 fletmint-0.1.5/fletmint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 07:42:24.000000 fletmint-0.1.5/fletmint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:42:24.942752 fletmint-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2024-05-21 07:35:55.000000 fletmint-0.1.5/setup.py
```

### Comparing `fletmint-0.1.4.1/PKG-INFO` & `fletmint-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fletmint
-Version: 0.1.4.1
+Version: 0.1.5
 Summary: A sharp and modern components library for Flet
 Author: Edoardo Balducci
 Author-email: edoardoba2004@gmail.com
 Project-URL: support, https://www.patreon.com/edoardobalducci
 Project-URL: repository, https://github.com/Bbalduzz/fletmint
 Project-URL: tracker, https://github.com/Bbalduzz/fletmint/issues
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: fletmint Version: 0.1.4.1 Summary: A sharp and
-modern components library for Flet Author: Edoardo Balducci Author-email:
+Metadata-Version: 2.1 Name: fletmint Version: 0.1.5 Summary: A sharp and modern
+components library for Flet Author: Edoardo Balducci Author-email:
 edoardoba2004@gmail.com Project-URL: support, https://www.patreon.com/
 edoardobalducci Project-URL: repository, https://github.com/Bbalduzz/fletmint
 Project-URL: tracker, https://github.com/Bbalduzz/fletmint/issues Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `fletmint-0.1.4.1/fletmint/__init__.py` & `fletmint-0.1.5/fletmint/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 from .slider import Slider
 from .toggle import Toggle
 from .datepicker import DatePicker
 from .audioplayer import AudioPlayer
 from .videoplayer import VideoPlayer
 from .badge import Badge, BadgeColors
 from .carousel import Carousel
+
+from .code import Code, CodeTheme
```

### Comparing `fletmint-0.1.4.1/fletmint/audioplayer.py` & `fletmint-0.1.5/fletmint/audioplayer.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/badge.py` & `fletmint-0.1.5/fletmint/badge.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/button.py` & `fletmint-0.1.5/fletmint/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,41 +22,45 @@
 class Button(TextButton):
     def __init__(
         self,
         width=200,
         height=50,
         on_click=None,
         disabled=False,
+        style=None,
         label="Button",
         icon=None,
     ):
         if icon:
             button_content = Icon(
                 icon, size=13, color=ButtonColors.button_content_color
             )
         else:
             button_content = Text(
                 label, size=13, color=ButtonColors.button_content_color
             )
 
-        self.style = ButtonStyle(
-            color={
-                "": ButtonColors.button_disabled_content_color
-                if disabled
-                else ButtonColors.button_content_color,  # MaterialState.DEFAULT
-            },
-            bgcolor={
-                "": ButtonColors.button_backgound_color
-                if not disabled
-                else ButtonColors.button_disabled_background_color,
-                "disabled": ButtonColors.button_disabled_background_color,
-            },
-            padding=18,
-            shape=ContinuousRectangleBorder(radius=20),
-        )
+        if not style:
+            self.style = ButtonStyle(
+                color={
+                    "": ButtonColors.button_disabled_content_color
+                    if disabled
+                    else ButtonColors.button_content_color,  # MaterialState.DEFAULT
+                },
+                bgcolor={
+                    "": ButtonColors.button_backgound_color
+                    if not disabled
+                    else ButtonColors.button_disabled_background_color,
+                    "disabled": ButtonColors.button_disabled_background_color,
+                },
+                padding=18,
+                shape=ContinuousRectangleBorder(radius=20),
+            )
+        else:
+            self.style = style
 
         super().__init__(
             content=Container(content=button_content),
             width=width,
             height=height,
             on_click=None if disabled else on_click,
             disabled=disabled,
```

### Comparing `fletmint-0.1.4.1/fletmint/carousel.py` & `fletmint-0.1.5/fletmint/carousel.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/checkbox.py` & `fletmint-0.1.5/fletmint/checkbox.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/datepicker.py` & `fletmint-0.1.5/fletmint/datepicker.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,41 +7,47 @@
 
 
 @dataclass
 class DatePickerColors:
     container_background_color: str
     container_border_color: str
     weekday_color: str
+    selected_date_background_color: str
+    today_button_border_color: str
     today_button_background_color: str
     default_day_background_color: str
     today_text_color: str
     filler_day_text_color: str
     default_day_text_color: str
     dropdown_starter_icon_color: str
 
     @staticmethod
     def dark():
         return DatePickerColors(
             container_background_color="#323741",
             container_border_color="#3d424d",
             weekday_color="#4a505b",
-            today_button_background_color="#1f5eff",
+            selected_date_background_color="#1f5eff",
+            today_button_border_color="#325de3",
+            today_button_background_color="#314276",
             default_day_background_color="#3c414a",
             today_text_color="#ffffff",
             filler_day_text_color="#4a505b",
             default_day_text_color="#b0b8cc",
             dropdown_starter_icon_color="#ffffff",
         )
 
     @staticmethod
     def light():
         return DatePickerColors(
             container_background_color="#ffffff",
             container_border_color="#e0e4ed",
             weekday_color="#EBEBEB",
+            selected_date_background_color="#1f5eff",
+            today_button_border_color="#1f5eff",
             today_button_background_color="#1f5eff",
             default_day_background_color="#EBF1FF",
             today_text_color="#ffffff",
             filler_day_text_color="#EBEBEB",
             default_day_text_color="#A8B1C7",
             dropdown_starter_icon_color="#7e879e",
         )
@@ -51,28 +57,30 @@
     def __init__(
         self,
         tz_info=timezone.utc,
         left_content=None,
         max_width=300,
         is_dropdown=True,
         multi_select_mode=True,
+        show_today=True,
         on_date_choosen=None,
         on_cancel=None,
         theme: ft.ThemeMode | str = ft.ThemeMode.DARK,
         drodown_icons=[
             ft.icons.ARROW_DROP_DOWN_ROUNDED,
             ft.icons.ARROW_DROP_UP_ROUNDED,
         ],
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.tz_info = tz_info
         self.left_content = left_content
         self.max_width = max_width
         self.is_dropdown = is_dropdown
+        self.show_today = show_today
         self.on_date_choosen = on_date_choosen
         self.on_cancel = on_cancel
         self.multi_select_mode = multi_select_mode
         self.dropdown_icons = drodown_icons
         self.selected_dates = set()
         self.current_month = datetime.now(self.tz_info).month
         self.current_year = datetime.now(self.tz_info).year
@@ -162,19 +170,22 @@
         filler_days = (start_day_of_week + 7) % 7
         for i in range(filler_days):
             day = (start_of_month - timedelta(days=filler_days - i)).day
             grid.controls.append(self.create_day_button(str(day), is_filler=True))
 
         for i in range(1, days_in_month + 1):
             day = datetime(self.current_year, self.current_month, i)
-            is_today = (
-                self.current_month == self.today.month
-                and self.current_year == self.today.year
-                and i == self.today.day
-            )
+            if not self.show_today:
+                is_today = False
+            else:
+                is_today = (
+                    self.current_month == self.today.month
+                    and self.current_year == self.today.year
+                    and i == self.today.day
+                )
             button = self.create_day_button(str(i), is_today=is_today, day_date=day)
             grid.controls.append(button)
 
         next_month_day_count = (7 - (end_of_month.weekday() + 1)) % 7
         for i in range(1, next_month_day_count + 1):
             grid.controls.append(self.create_day_button(str(i), is_filler=True))
 
@@ -184,22 +195,30 @@
         bgcolor = (
             self.colors.today_button_background_color
             if is_today
             else ""
             if is_filler
             else self.colors.default_day_background_color
         )
+        bordercolor = (
+            self.colors.today_button_border_color
+            if is_today
+            else ft.colors.with_opacity(0, "white")
+            if is_filler
+            else self.colors.default_day_background_color
+        )
         button = ft.TextButton(
             text=text,
             width=50,
             height=50,
             data=day_date,
             on_click=self.select_day,
             style=ft.ButtonStyle(
                 bgcolor=bgcolor,
+                side=ft.BorderSide(1, bordercolor),
                 color=self.colors.today_text_color
                 if is_today
                 else self.colors.filler_day_text_color
                 if is_filler
                 else self.colors.default_day_text_color,
                 shape=ft.ContinuousRectangleBorder(radius=12),
                 padding=2,
@@ -218,29 +237,29 @@
         if self.multi_select_mode:
             if day_date in self.selected_dates:
                 self.selected_dates.remove(day_date)
                 day_button.style.bgcolor = self.colors.default_day_background_color
                 day_button.style.color = self.colors.default_day_text_color
             else:
                 self.selected_dates.add(day_date)
-                day_button.style.bgcolor = self.colors.today_button_background_color
+                day_button.style.bgcolor = self.colors.selected_date_background_color
                 day_button.style.color = self.colors.today_text_color
         else:
             for button in self.calendarpicker.content.controls[1].controls:
                 if (
                     isinstance(button, ft.TextButton)
                     and button.data in self.selected_dates
                 ):
                     button.style.bgcolor = self.colors.default_day_background_color
                     button.style.color = self.colors.default_day_text_color
                     button.update()
 
             self.selected_dates.clear()
             self.selected_dates.add(day_date)
-            day_button.style.bgcolor = self.colors.today_button_background_color
+            day_button.style.bgcolor = self.colors.selected_date_background_color
             day_button.style.color = self.colors.today_text_color
 
         day_button.update()
 
     def build_calendarpicker(self):
         def on_control_click(e):
             print(e.control)
```

### Comparing `fletmint-0.1.4.1/fletmint/dropdown.py` & `fletmint-0.1.5/fletmint/dropdown.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/profile.py` & `fletmint-0.1.5/fletmint/profile.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/slider.py` & `fletmint-0.1.5/fletmint/slider.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/stepper.py` & `fletmint-0.1.5/fletmint/stepper.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/tab_switch.py` & `fletmint-0.1.5/fletmint/tab_switch.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,31 +84,36 @@
             border_radius=5,
             alignment=ft.alignment.center,
             padding=ft.padding.all(5),
             on_click=self.toggle_switch,
         )
 
     def toggle_switch(self, e):
-        """Switch to the tab that was clicked."""
-        clicked_tab_index = self.content.controls.index(e.control)
-        self.value = clicked_tab_index
+        """Switch to the tab that was clicked and update its appearance."""
+        new_active_index = self.content.controls.index(e.control)
+        if new_active_index != self.value:
+            self.update_tab(self.tabs[self.value], False)
+            self.update_tab(self.tabs[new_active_index], True)
+            self.value = new_active_index
+            if self.on_switch:
+                self.on_switch(self.value)
 
-        # Update the tabs to reflect the active state
-        self.content.controls = [
-            self.get_container(label, index == self.value)
-            for index, label in enumerate(self.tab_labels)
-        ]
-
-        self.update()
-        if self.on_switch:
-            self.on_switch(self.value)
-
-    def get_value(self):
-        """Return the current active tab index."""
-        return self.value
+    def update_tab(self, tab, active):
+        """Update the visual state of a tab."""
+        tab.bgcolor = (
+            self.colors.active_tab_background_color
+            if active
+            else self.colors.container_background_color
+        )
+        tab.content.color = (
+            self.colors.label_text_color
+            if active
+            else self.colors.unfocused_label_text_color
+        )
+        tab.update()
 
     def did_mount(self):
         self.colors = (
             TabSwitchColors.dark()
             if self.page.theme_mode == ft.ThemeMode.DARK
             else TabSwitchColors.light()
         )
```

### Comparing `fletmint-0.1.4.1/fletmint/table.py` & `fletmint-0.1.5/fletmint/table.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/tags_input.py` & `fletmint-0.1.5/fletmint/tags_input.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/text_input.py` & `fletmint-0.1.5/fletmint/text_input.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/toggle.py` & `fletmint-0.1.5/fletmint/toggle.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/toggle_switch.py` & `fletmint-0.1.5/fletmint/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint/videoplayer.py` & `fletmint-0.1.5/fletmint/videoplayer.py`

 * *Files identical despite different names*

### Comparing `fletmint-0.1.4.1/fletmint.egg-info/PKG-INFO` & `fletmint-0.1.5/fletmint.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fletmint
-Version: 0.1.4.1
+Version: 0.1.5
 Summary: A sharp and modern components library for Flet
 Author: Edoardo Balducci
 Author-email: edoardoba2004@gmail.com
 Project-URL: support, https://www.patreon.com/edoardobalducci
 Project-URL: repository, https://github.com/Bbalduzz/fletmint
 Project-URL: tracker, https://github.com/Bbalduzz/fletmint/issues
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: fletmint Version: 0.1.4.1 Summary: A sharp and
-modern components library for Flet Author: Edoardo Balducci Author-email:
+Metadata-Version: 2.1 Name: fletmint Version: 0.1.5 Summary: A sharp and modern
+components library for Flet Author: Edoardo Balducci Author-email:
 edoardoba2004@gmail.com Project-URL: support, https://www.patreon.com/
 edoardobalducci Project-URL: repository, https://github.com/Bbalduzz/fletmint
 Project-URL: tracker, https://github.com/Bbalduzz/fletmint/issues Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `fletmint-0.1.4.1/fletmint.egg-info/SOURCES.txt` & `fletmint-0.1.5/fletmint.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 setup.py
+dev/__init__.py
+dev/code.py
+dev/duration.py
+dev/stht.py
+dev/t.py
+dev/timepicker.py
 fletmint/__init__.py
 fletmint/audioplayer.py
 fletmint/badge.py
 fletmint/button.py
 fletmint/carousel.py
 fletmint/checkbox.py
+fletmint/code.py
 fletmint/datepicker.py
 fletmint/dropdown.py
 fletmint/profile.py
 fletmint/radio.py
 fletmint/slider.py
 fletmint/stepper.py
 fletmint/tab_switch.py
```

### Comparing `fletmint-0.1.4.1/setup.py` & `fletmint-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import path
 
 with open(path.join(path.dirname(__file__), "description.md"), "r") as file:
     description = file.read()
 
 setup(
     name="fletmint",
-    version="0.1.4.1",
+    version="0.1.5",
     author="Edoardo Balducci",
     author_email="edoardoba2004@gmail.com",
     description="A sharp and modern components library for Flet",
     long_description=description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["flet"],
```

