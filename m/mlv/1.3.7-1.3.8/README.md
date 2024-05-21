# Comparing `tmp/mlv-1.3.7.tar.gz` & `tmp/mlv-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.3.7.tar", last modified: Sun May 19 03:43:44 2024, max compression
+gzip compressed data, was "mlv-1.3.8.tar", last modified: Tue May 21 01:34:04 2024, max compression
```

## Comparing `mlv-1.3.7.tar` & `mlv-1.3.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.545136 mlv-1.3.7/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.7/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-19 03:43:44.544939 mlv-1.3.7/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.543856 mlv-1.3.7/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.7/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.7/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     9958 2024-05-19 03:27:27.000000 mlv-1.3.7/mlv/drawing.py
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-05-19 01:55:07.000000 mlv-1.3.7/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.7/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.7/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    16708 2024-05-19 01:53:13.000000 mlv-1.3.7/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.7/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.7/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.7/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.7/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.7/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.544731 mlv-1.3.7/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.7/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-19 03:43:44.545178 mlv-1.3.7/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-19 03:42:24.000000 mlv-1.3.7/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.544575 mlv-1.3.7/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.7/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-21 01:34:04.887335 mlv-1.3.8/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.8/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-21 01:34:04.887147 mlv-1.3.8/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-21 01:34:04.885666 mlv-1.3.8/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.8/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.8/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    10115 2024-05-21 01:31:22.000000 mlv-1.3.8/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-05-19 01:55:07.000000 mlv-1.3.8/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.8/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.8/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16708 2024-05-19 01:53:13.000000 mlv-1.3.8/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.8/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.8/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.8/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.8/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.8/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-21 01:34:04.886948 mlv-1.3.8/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-21 01:34:04.000000 mlv-1.3.8/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-21 01:34:04.000000 mlv-1.3.8/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-21 01:34:04.000000 mlv-1.3.8/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-21 01:34:04.000000 mlv-1.3.8/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-21 01:34:04.000000 mlv-1.3.8/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.8/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-21 01:34:04.887377 mlv-1.3.8/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-21 01:33:53.000000 mlv-1.3.8/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-21 01:34:04.886652 mlv-1.3.8/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.8/tests/test_hello.py
```

### Comparing `mlv-1.3.7/mlv/drawing.py` & `mlv-1.3.8/mlv/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,26 +126,29 @@
     pipe.fuse_lora()
 
     generator = torch.Generator()
 
     def infer(
         prompt,
         image,
+        seed=None,
         num_inference_steps=3,
         guidance_scale=2,
         strength=0.9,
         invert_color=True,
         negative_prompt=None,
         mode=None,
     ):
         image = load_image(image)
         image = resize(image)
         if invert_color:
             image = ImageOps.invert(image)
         image = image.convert("L")
+        if seed:
+            generator = generator.manual_seed(seed)
 
         with torch.inference_mode():
             with torch.autocast("cuda") if device == "cuda" else nullcontext():
                 with timer("inference"):
                     return pipe(
                         prompt=prompt,
                         image=image,
@@ -219,37 +222,40 @@
     generator = torch.Generator()
 
     img2img_pipe = StableDiffusionImg2ImgPipeline(**txt2img_pipe.components)
 
     def infer(
         prompt,
         image,
+        seed=None,
         num_inference_steps=5,
         guidance_scale=2,
         strength=0.9,
         negative_prompt=None,
         mode="i2i",
     ):
+        if seed:
+            generator = generator.manual_seed(seed)
         with torch.inference_mode():
             with torch.autocast("cuda") if device == "cuda" else nullcontext():
                 with timer("inference"):
                     if mode == "i2i":
                         return img2img_pipe(
                             prompt=prompt,
                             image=resize(load_image(image)),
-                            generator=generator.manual_seed(int(time.time())),
+                            generator=generator,
                             num_inference_steps=num_inference_steps,
                             guidance_scale=guidance_scale,
                             strength=strength,
                             negative_prompt=negative_prompt,
                         ).images[0]
                     elif mode == "t2i":
                         return txt2img_pipe(
                             prompt=prompt,
-                            generator=generator.manual_seed(int(time.time())),
+                            generator=generator,
                             num_inference_steps=num_inference_steps,
                             guidance_scale=guidance_scale,
                             negative_prompt=negative_prompt,
                         ).images[0]
                     else:
                         raise ValueError("mode not support")
 
@@ -293,13 +299,14 @@
                 image = Image.open(image)
         out_image_path = os.path.join(output_path, "sd_image.jpg")
 
         self.model(
             prompt,
             image,
             mode=mode,
+            seed=args.get("seed", None),
             num_inference_steps=args.get("num_inference_steps", 4),
             guidance_scale=args.get("guidance_scale", 2),
             strength=args.get("strength", 0.9),
             negative_prompt=args.get("negative_prompt", "ugly, disform, bad hand"),
         ).save(out_image_path)
         return {"result": out_image_path}
```

### Comparing `mlv-1.3.7/mlv/mps_workaround.py` & `mlv-1.3.8/mlv/mps_workaround.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/old_http.py` & `mlv-1.3.8/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/old_stable_diffusion.py` & `mlv-1.3.8/mlv/old_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/ollama.py` & `mlv-1.3.8/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/rpc.py` & `mlv-1.3.8/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/segment_anything.py` & `mlv-1.3.8/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/stable_diffusion.py` & `mlv-1.3.8/mlv/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.7/mlv/util.py` & `mlv-1.3.8/mlv/util.py`

 * *Files identical despite different names*

