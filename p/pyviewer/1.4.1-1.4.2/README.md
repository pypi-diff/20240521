# Comparing `tmp/pyviewer-1.4.1.tar.gz` & `tmp/pyviewer-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.4.1.tar", last modified: Sun Apr 28 19:40:40 2024, max compression
+gzip compressed data, was "pyviewer-1.4.2.tar", last modified: Tue May 21 16:38:48 2024, max compression
```

## Comparing `pyviewer-1.4.1.tar` & `pyviewer-1.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.604717 pyviewer-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-04-28 19:40:34.000000 pyviewer-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-28 19:40:40.600717 pyviewer-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-28 19:40:34.000000 pyviewer-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.600717 pyviewer-1.4.1/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (127)  3423528 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/MPLUSRounded1c-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.600717 pyviewer-1.4.1/pyviewer/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/custom_ops/cuda_gl_interop.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    25971 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    71936 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/roboto_mono.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-28 19:40:34.000000 pyviewer-1.4.1/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:40:40.600717 pyviewer-1.4.1/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 19:40:40.000000 pyviewer-1.4.1/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:40:40.604717 pyviewer-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-28 19:40:34.000000 pyviewer-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:38:48.056894 pyviewer-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-05-21 16:38:43.000000 pyviewer-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-21 16:38:48.056894 pyviewer-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-21 16:38:43.000000 pyviewer-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:38:48.056894 pyviewer-1.4.2/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)  3423528 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/MPLUSRounded1c-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:38:48.056894 pyviewer-1.4.2/pyviewer/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/custom_ops/cuda_gl_interop.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26586 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71936 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/roboto_mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20093 2024-05-21 16:38:43.000000 pyviewer-1.4.2/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:38:48.056894 pyviewer-1.4.2/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-21 16:38:48.000000 pyviewer-1.4.2/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-21 16:38:48.000000 pyviewer-1.4.2/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:38:48.000000 pyviewer-1.4.2/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 16:38:48.000000 pyviewer-1.4.2/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 16:38:48.000000 pyviewer-1.4.2/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:38:48.056894 pyviewer-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-21 16:38:43.000000 pyviewer-1.4.2/setup.py
```

### Comparing `pyviewer-1.4.1/LICENSE` & `pyviewer-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/PKG-INFO` & `pyviewer-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.4.1
+Version: 1.4.2
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.4.1/README.md` & `pyviewer-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/MPLUSRounded1c-Medium.ttf` & `pyviewer-1.4.2/pyviewer/MPLUSRounded1c-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/custom_ops/cuda_gl_interop.cpp` & `pyviewer-1.4.2/pyviewer/custom_ops/cuda_gl_interop.cpp`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/custom_ops.py` & `pyviewer-1.4.2/pyviewer/custom_ops.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/gl_viewer.py` & `pyviewer-1.4.2/pyviewer/gl_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,16 @@
     def __init__(self, title, inifile=None, swap_interval=0, hidden=False):
         self.quit = False
 
         self._images = {}
         self._editables = {}
         self.tex_interp_mode = gl.GL_LINEAR
         self.default_font_size = 15
-        
+        self.renderer = None
+
         fname = inifile or "".join(c for c in title.lower() if c.isalnum())
         self._inifile = Path(fname).with_suffix('.ini')
 
         if not glfw.init():
             raise RuntimeError('GLFW init failed')
 
         if not has_pycuda and pt_plugin is None:
@@ -421,14 +422,15 @@
         self.tex_interp_mode = gl.GL_NEAREST
 
     def editable(self, name, **kwargs):
         if name not in self._editables:
             self._editables[name] = _editable(name)
         self._editables[name].run(**kwargs)
 
+    # Includes keyboard (glfw.KEY_A) and mouse (glfw.MOUSE_BUTTON_LEFT)
     def keydown(self, key):
         return key in self._pressed_keys
 
     def keyhit(self, key):
         if key in self._hit_keys:
             self._hit_keys.remove(key)
             return True
@@ -500,47 +502,58 @@
         s.scrollbar_size        = scrollbar
 
         c0 = s.colors[imgui.COLOR_MENUBAR_BACKGROUND]
         c1 = s.colors[imgui.COLOR_FRAME_BACKGROUND]
         s.colors[imgui.COLOR_POPUP_BACKGROUND] = [x * 0.7 + y * 0.3 for x, y in zip(c0, c1)][:3] + [1]
 
     def start(self, loopfunc, workers = (), glfw_init_callback = None):
-        # allow single thread object
-        if not hasattr(workers, '__len__'):
-            workers = (workers,)
-
-        for i in range(len(workers)):
-            workers[i].start()
-        
-        with self.lock():
-            impl = GlfwRenderer(self._window)
-        
         self._pressed_keys = set()
         self._hit_keys = set()
+        
+        with self.lock():
+            self.renderer = GlfwRenderer(self._window)
 
         def on_key(window, key, scan, pressed, mods):
             if pressed:
                 if key not in self._pressed_keys:
                     self._hit_keys.add(key)
                 self._pressed_keys.add(key)
             else:
                 if key in self._pressed_keys:
                     self._pressed_keys.remove(key) # check seems to be needed over RDP sometimes
             if key != glfw.KEY_ESCAPE: # imgui erases text with escape (??)
-                impl.keyboard_callback(window, key, scan, pressed, mods)
+                self.renderer.keyboard_callback(window, key, scan, pressed, mods)
+
+        def on_mouse_button(window, key, action, mods):
+            if action == glfw.PRESS:
+                if key not in self._pressed_keys:
+                    self._hit_keys.add(key)
+                self._pressed_keys.add(key)
+            else:
+                if key in self._pressed_keys:
+                    self._pressed_keys.remove(key)
+            self.renderer.keyboard_callback(window, key, None, action, mods)
 
         glfw.set_key_callback(self._window, on_key)
+        glfw.set_mouse_button_callback(self._window, on_mouse_button)
 
         # For settings custom callbacks etc.
         if glfw_init_callback is not None:
             glfw_init_callback(self._window)
 
+        # allow single thread object
+        if not hasattr(workers, '__len__'):
+            workers = (workers,)
+
+        for i in range(len(workers)):
+            workers[i].start()
+
         while not glfw.window_should_close(self._window):
             glfw.poll_events()
-            impl.process_inputs()
+            self.renderer.process_inputs()
 
             if self.keyhit(glfw.KEY_ESCAPE):
                 glfw.set_window_should_close(self._window, 1)
 
             with self.lock(strict=False) as l:
                 if l == nullcontext:
                     continue
@@ -562,15 +575,15 @@
                 imgui.pop_font()
 
                 imgui.render()
                 
                 gl.glClearColor(0, 0, 0, 1)
                 gl.glClear(gl.GL_COLOR_BUFFER_BIT)
 
-                impl.render(imgui.get_draw_data())
+                self.renderer.render(imgui.get_draw_data())
                 
                 # TODO: compute thread has to wait until sync is done
                 # and lock is released if calling upload_image()?
                 glfw.swap_buffers(self._window)
         
         # Update size and pos
         if not self.fullscreen:
```

### Comparing `pyviewer-1.4.1/pyviewer/imgui_themes.py` & `pyviewer-1.4.2/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/params.py` & `pyviewer-1.4.2/pyviewer/params.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,28 @@
 class _Range2Param(Param):
     def __init__(self, type, label, default_val, minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
         super().__init__(type, label, default_val, tooltip)
         self.min = minval
         self.max = maxval
         self.overlap = overlap  # allow v2 to go below v1?
 
+class _Range3Param(Param):
+    def __init__(self, type, label, default_val, minval, maxval, tooltip: str = None) -> None:
+        super().__init__(type, label, default_val, tooltip)
+        self.min = minval
+        self.max = maxval
+
 class EnumParam(Param):
-    def __init__(self, label, default_val, valid_vals=(), tooltip: str = None) -> None:
+    def __init__(self, label, default_val, valid_vals=(), to_str: Callable[..., str] = str, tooltip: str = None) -> None:
         super().__init__(type(default_val), label, default_val, tooltip)
         self.opts = list(valid_vals)
+        self.to_str = to_str
 
     def draw_widget(self):
-        return combo_box_vals(self.label, self.opts, self.value)
+        return combo_box_vals(self.label, self.opts, self.value, to_str=self.to_str)
 
 class EnumSliderParam(Param):
     def __init__(self, label, default_val, valid_vals=(), to_str: Callable[..., str] = str, tooltip: str = None) -> None:
         super().__init__(type(default_val), label, default_val, tooltip)
         self.opts = list(valid_vals)
         self.to_str = to_str
 
@@ -85,14 +92,21 @@
         super().__init__(Tuple[int], label, default_val, minval, maxval, overlap, tooltip)
     
     def draw_widget(self):
         if not self.overlap:
             return slider_range_int(*self.value, self.min, self.max, title=self.label)
         else:
             return imgui.slider_int2(self.label, *self.value, self.min, self.max)
+        
+class Int3Param(_Range3Param):
+    def __init__(self, label, default_val: Tuple[int], minval, maxval, tooltip: str = None) -> None:
+        super().__init__(Tuple[int], label, default_val, minval, maxval, tooltip)
+    
+    def draw_widget(self):
+        return imgui.slider_int3(self.label, *self.value, self.min, self.max)
 
 class FloatParam(_RangeParam):
     def __init__(self, label, default_val: float, minval, maxval, tooltip: str = None) -> None:
         super().__init__(float, label, default_val, minval, maxval, tooltip)
     
     def draw_widget(self):
         return imgui.slider_float(self.label, self.value, self.min, self.max)
@@ -102,14 +116,21 @@
         super().__init__(Tuple[float], label, default_val, minval, maxval, overlap, tooltip)
     
     def draw_widget(self):
         if not self.overlap:
             return slider_range_float(*self.value, self.min, self.max, title=self.label)
         else:
             return imgui.slider_float2(self.label, *self.value, self.min, self.max)
+        
+class Float3Param(_Range3Param):
+    def __init__(self, label, default_val: Tuple[float], minval, maxval, tooltip: str = None) -> None:
+        super().__init__(Tuple[float], label, default_val, minval, maxval, tooltip)
+    
+    def draw_widget(self):
+        return imgui.slider_float3(self.label, *self.value, self.min, self.max)
     
 ##########################################
 # Container that exposes raw values
 @strict_dataclass
 class ParamContainer:
     def __iter__(self):
         for attr, _ in self.__dataclass_fields__.items():
@@ -132,8 +153,19 @@
     def __todict__(self):
         ret = {}
         for attr, _ in self.__dataclass_fields__.items():
             ret[attr] = self.__getattribute__(attr)
         return ret
 
     def __str__(self):
-        return str(self.__todict__())
+        return str(self.__todict__())
+    
+def draw_container(cont: ParamContainer, reset_button=False):
+    for _, p in cont:
+        if isinstance(p, Param):
+            p.draw()
+    
+    # Draw below widgets
+    if reset_button and imgui.button('Reset'):
+        for _, p in cont:
+            if isinstance(p, Param):
+                p.reset()
```

### Comparing `pyviewer-1.4.1/pyviewer/roboto_mono.ttf` & `pyviewer-1.4.2/pyviewer/roboto_mono.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/single_image_viewer.py` & `pyviewer-1.4.2/pyviewer/single_image_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.4.1/pyviewer/toolbar_viewer.py` & `pyviewer-1.4.2/pyviewer/toolbar_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 import time
 from pathlib import Path
 from functools import partial
 
 from . import gl_viewer
 from .utils import imgui_item_width, begin_inline, PannableArea
 from .easy_dict import EasyDict
-from .params import ParamContainer, Param
+from .params import ParamContainer, Param, draw_container
 
 #----------------------------------------------------------------------------
 # Helper class for UIs with toolbar on the left and output image on the right
 
-def file_drop_callback_wrapper(window, paths, callback: callable):
-    return callback([Path(p) for p in paths])
+def file_drop_callback_wrapper(window, paths, callback: callable, prev: callable):
+    return callback([Path(p) for p in paths]) or prev(window, paths)
+
+def scroll_callback_wrapper(window, xoffset, yoffset, callback: callable, prev: callable):
+    return callback(xoffset, yoffset) or prev(window, xoffset, yoffset)
 
 class ToolbarViewer:
     def __init__(self, name, pad_bottom=0, hidden=False, batch_mode=False):
         self.output_key = ''.join(random.choices(string.ascii_letters, k=20))
         self._user_pad_bottom = pad_bottom
         self.v = gl_viewer.viewer(name, hidden=hidden or batch_mode, swap_interval=1)
         self.menu_bar_height = self.v.font_size + 2*imgui.get_style().frame_padding.y
@@ -42,29 +45,35 @@
         self.state = EasyDict()
 
         # Support image zoom and pan
         self.pan_handler = PannableArea()
         self.pan_handler.clear_color = (0.101, 0.101, 0.101, 1.00) # match theme_deep_dark
         self.pan_enabled = True
         
-        # User-provided
-        self.setup_state()
-
         # User nearest interpolation for sharpness by default
         self.v.set_interp_nearest()
+
+        # User-provided
+        self.setup_state()
         
         # Batch mode: handle compute loop manually, don't start UI
         if not batch_mode:
             self.start_UI()
 
     def start_UI(self):
         compute_thread = threading.Thread(target=self._compute_loop, args=[])
         def init_callbacks(window):
+            def noop(*args, **kwargs):
+                return False
+            prev = glfw.set_drop_callback(window, None)
             glfw.set_drop_callback(window,
-                partial(file_drop_callback_wrapper, callback=self.drag_and_drop_callback))
+                partial(file_drop_callback_wrapper, callback=self.drag_and_drop_callback, prev=(prev or noop)))
+            prev = glfw.set_scroll_callback(window, None)
+            glfw.set_scroll_callback(window,
+                partial(scroll_callback_wrapper, callback=self.scroll_callback, prev=(prev or noop)))
             self.setup_callbacks(window)
             self.pan_handler.set_callbacks(window)
         self.v.start(self._ui_main, (compute_thread), init_callbacks)
 
     # Extra user content below image
     @property
     def pad_bottom(self):
@@ -102,14 +111,15 @@
         return (self.mouse_pos_abs - self.output_pos_tl) / dims
 
     def _ui_main(self, v):
         self._toolbar_wrapper()
         self._draw_output()
 
     def _compute_loop(self):
+        self.compute_thread_init()
         while not self.v.quit:
             img = self.compute()
             
             if img is not None:
                 H, W, C = img.shape
                 self.img_shape = [C, H, W]
                 self.v.upload_image(self.output_key, img)
@@ -218,20 +228,23 @@
         v = self.v
         _, H = glfw.get_window_size(v._window)
         imgui.set_next_window_size(self.toolbar_width, H - self.menu_bar_height)
         imgui.set_next_window_position(0, self.menu_bar_height)
 
         # User callback
         begin_inline('toolbar')
+        self._draw_toolbar_impl()
+        imgui.end()
+
+    def _draw_toolbar_impl(self):
         self.draw_toolbar_autoUI()
         self.draw_toolbar()
-        imgui.end()
 
     # Only used by AutoUIViewer
-    def draw_toolbar_autoUI(self):
+    def draw_toolbar_autoUI(self, containers=None):
         pass
 
     def mouse_over_image(self):
         x, y = self.mouse_pos_img_norm
         return (0 <= x <= 1) and (0 <= y <= 1)
 
     def mouse_over_content(self):
@@ -242,14 +255,18 @@
     # (e.g. in callbacks or from UI thread)
     def update_image(self, img_hwc):
         H, W = img_hwc.shape[0:2]
         C = 1 if img_hwc.ndim == 2 else img_hwc.shape[-1]
         self.img_shape = [C, H, W]
         self.v.upload_image(self.output_key, img_hwc)
     
+    # Includes keyboard (glfw.KEY_A) and mouse (glfw.MOUSE_BUTTON_LEFT)
+    def keydown(self, key):
+        return self.v.keydown(key)
+
     #------------------------
     # User-provided functions
 
     # Draw toolbar, must be implemented
     def draw_toolbar(self):
         pass
 
@@ -267,47 +284,50 @@
     # Draw overlays using main window draw list
     def draw_overlays(self, draw_list):
         pass
 
     def draw_menu(self):
         pass
     
+    # One time compute thread initialization
+    # Usually not needed
+    def compute_thread_init(self):
+        pass
+
     # Perform computation, returning single np/torch image, or None
     def compute(self):
         pass
 
     # Program state init
     def setup_state(self):
         pass
 
     # Manual GLFW callbacks
     # Overrides the ones below
     def setup_callbacks(self, window):
         pass
 
-    def drag_and_drop_callback(self, paths: list[Path]):
+    def drag_and_drop_callback(self, paths: list[Path]) -> bool:
+        pass
+
+    def scroll_callback(self, xoffset: float, yoffset: float) -> bool:
         pass
 
 #----------------------------------------------
 # Version that creates UI widgets automatically
 
 class AutoUIViewer(ToolbarViewer):
-    def draw_toolbar_autoUI(self):
-        if not isinstance(self.state, ParamContainer):
-            return
-
-        for _, p in self.state:
-            if isinstance(p, Param):
-                p.draw()
+    def draw_toolbar_autoUI(self, containers=None):
+        if containers is None:
+            containers = [self.state]
         
-        # Draw below widgets
-        if imgui.button('Reset'):
-            for _, p in self.state:
-                if isinstance(p, Param):
-                    p.reset()
+        for cont in containers:
+            if not isinstance(cont, ParamContainer):
+                continue
+            draw_container(cont, reset_button=True)
 
 #--------------
 # Example usage
 
 def main():
     import numpy as np
```

### Comparing `pyviewer-1.4.1/pyviewer/utils.py` & `pyviewer-1.4.2/pyviewer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # and allows mouse pand & zoom controls
 class PannableArea():
     def __init__(self, set_callbacks=False, glfw_window=False) -> None:  # draw_content: callable, 
         self.prev_cbk: callable = lambda : None  # for chaining
         self.output_pos_tl = np.zeros(2, dtype=np.float32)
         self.id = ''.join(random.choices(string.ascii_letters, k=20))
         self.is_panning = False
+        self.zoom_enabled = True
         self.pan = (0, 0)
         self.pan_start = (0, 0)
         self.pan_delta = (0, 0)
         self.zoom: float = 1.0
         self.clear_color = (0, 0, 0, 1) # in [0, 1]
 
         # Canvas onto which resmapled image is drawn
@@ -311,15 +312,15 @@
         return (self.mouse_pos_abs - self.output_pos_tl) / dims
 
     def mouse_hovers_content(self):
         x, y = self.mouse_pos_img_norm
         return (0 <= x <= 1) and (0 <= y <= 1)
     
     def mouse_wheel_callback(self, window, x, y) -> None:
-        if self.mouse_hovers_content():
+        if self.mouse_hovers_content() and self.zoom_enabled:
             self.zoom = max(1e-2, (0.85**np.sign(-y)) * self.zoom)
         else:
             self.prev_cbk(window, x, y) # scroll imgui lists etc.
 
 # Dataclass that enforces type annotation
 # Enables compare-by-value
 def strict_dataclass(cls, *args, **kwargs):
```

### Comparing `pyviewer-1.4.1/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.4.2/pyviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.4.1
+Version: 1.4.2
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.4.1/setup.py` & `pyviewer-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # git push --delete origin tagname
 
 # Test package_data changes by manually starting
 # the publish workflow and checking the "Print whl contents" step,
 # or with: `rm -r build\ && pip wheel . && unzip -l pyviewer-*.whl`
 # (not same environment, but good first step)
 setup(name='pyviewer',
-    version='1.4.1',
+    version='1.4.2',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
```

