# Comparing `tmp/akhdefo_functions-2.5.6.tar.gz` & `tmp/akhdefo_functions-2.5.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akhdefo_functions-2.5.6.tar", last modified: Tue May  7 01:51:25 2024, max compression
+gzip compressed data, was "akhdefo_functions-2.5.61.tar", last modified: Tue May 21 01:04:44 2024, max compression
```

## Comparing `akhdefo_functions-2.5.6.tar` & `akhdefo_functions-2.5.61.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 01:51:25.459773 akhdefo_functions-2.5.6/
--rw-rw-rw-   0        0        0     9914 2024-05-07 01:51:25.458773 akhdefo_functions-2.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.6/README.md
--rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.6/README_pypi.md
-drwxrwxrwx   0        0        0        0 2024-05-07 01:51:25.437673 akhdefo_functions-2.5.6/akhdefo_functions/
--rw-rw-rw-   0        0        0    79472 2024-04-26 05:03:44.000000 akhdefo_functions-2.5.6/akhdefo_functions/AkhdefoPlot.py
--rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Classification.py
--rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Coreg.py
--rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_GOI.py
--rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_TS.py
--rw-rw-rw-   0        0        0    82914 2024-05-03 18:38:57.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Tools.py
--rw-rw-rw-   0        0        0   156263 2024-05-07 01:45:01.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Utilities.py
--rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.6/akhdefo_functions/Filter_PreProc.py
--rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.6/akhdefo_functions/Mosaic_Crop.py
--rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.6/akhdefo_functions/OpticalFlow.py
--rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.6/akhdefo_functions/Stacked_Velocity.py
--rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.6/akhdefo_functions/Unzip_CopyFiles.py
--rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.6/akhdefo_functions/Video_Streamer.py
--rw-rw-rw-   0        0        0      718 2024-05-07 01:50:57.000000 akhdefo_functions-2.5.6/akhdefo_functions/__init__.py
--rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.6/akhdefo_functions/backend.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:51:25.457773 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/
--rw-rw-rw-   0        0        0     9914 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 01:51:25.460773 akhdefo_functions-2.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-07 01:51:14.000000 akhdefo_functions-2.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:04:44.440492 akhdefo_functions-2.5.61/
+-rw-rw-rw-   0        0        0     9915 2024-05-21 01:04:44.440492 akhdefo_functions-2.5.61/PKG-INFO
+-rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.61/README.md
+-rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.61/README_pypi.md
+drwxrwxrwx   0        0        0        0 2024-05-21 01:04:44.408837 akhdefo_functions-2.5.61/akhdefo_functions/
+-rw-rw-rw-   0        0        0    79472 2024-04-26 05:03:44.000000 akhdefo_functions-2.5.61/akhdefo_functions/AkhdefoPlot.py
+-rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Classification.py
+-rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Coreg.py
+-rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_GOI.py
+-rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_TS.py
+-rw-rw-rw-   0        0        0    82914 2024-05-03 18:38:57.000000 akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Tools.py
+-rw-rw-rw-   0        0        0   156489 2024-05-21 00:27:37.000000 akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Utilities.py
+-rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.61/akhdefo_functions/Filter_PreProc.py
+-rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.61/akhdefo_functions/Mosaic_Crop.py
+-rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.61/akhdefo_functions/OpticalFlow.py
+-rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.61/akhdefo_functions/Stacked_Velocity.py
+-rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.61/akhdefo_functions/Unzip_CopyFiles.py
+-rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.61/akhdefo_functions/Video_Streamer.py
+-rw-rw-rw-   0        0        0      718 2024-05-07 01:50:57.000000 akhdefo_functions-2.5.61/akhdefo_functions/__init__.py
+-rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.61/akhdefo_functions/backend.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:04:44.440492 akhdefo_functions-2.5.61/akhdefo_functions.egg-info/
+-rw-rw-rw-   0        0        0     9915 2024-05-21 01:04:44.000000 akhdefo_functions-2.5.61/akhdefo_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-05-21 01:04:44.000000 akhdefo_functions-2.5.61/akhdefo_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 01:04:44.000000 akhdefo_functions-2.5.61/akhdefo_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.61/akhdefo_functions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-05-21 01:04:44.000000 akhdefo_functions-2.5.61/akhdefo_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 01:04:44.440492 akhdefo_functions-2.5.61/setup.cfg
+-rw-rw-rw-   0        0        0     1835 2024-05-21 01:03:25.000000 akhdefo_functions-2.5.61/setup.py
```

### Comparing `akhdefo_functions-2.5.6/PKG-INFO` & `akhdefo_functions-2.5.61/akhdefo_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: akhdefo_functions
-Version: 2.5.6
+Name: akhdefo-functions
+Version: 2.5.61
 Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `akhdefo_functions-2.5.6/README.md` & `akhdefo_functions-2.5.61/README.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/README_pypi.md` & `akhdefo_functions-2.5.61/README_pypi.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/AkhdefoPlot.py` & `akhdefo_functions-2.5.61/akhdefo_functions/AkhdefoPlot.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Classification.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Classification.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Coreg.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Coreg.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_GOI.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_GOI.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_TS.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_TS.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Tools.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Tools.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Utilities.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Akhdefo_Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -3166,35 +3166,36 @@
         height_f = int(combined_frame.shape[0] * 1)
         new_dimensions = (1280, 400)
 
       
         imagescreenshot_list.append(combined_frame)
         
         if save_output:
+            if release_flag==True:
         
-            # # Create a temporary file and close it immediately to use its name
-            with tempfile.NamedTemporaryFile(delete=False, suffix='.mp4',  dir='plots/Videos/temp') as temp_file:
-                temp_file_name = temp_file.name
-                
-            fps = 30  # or any other frame rate you want
-            frame_size = (imagescreenshot_list[0].shape[1], imagescreenshot_list[0].shape[0])  # width, height from the first image
-            out_v = cv2.VideoWriter(temp_file_name, fourcc, fps, frame_size)
+                # # Create a temporary file and close it immediately to use its name
+                with tempfile.NamedTemporaryFile(delete=False, suffix='.mp4',  dir='plots/Videos/temp') as temp_file:
+                    temp_file_name = temp_file.name
+                    
+                fps = 30  # or any other frame rate you want
+                frame_size = (imagescreenshot_list[0].shape[1], imagescreenshot_list[0].shape[0])  # width, height from the first image
+                out_v = cv2.VideoWriter(temp_file_name, fourcc, fps, frame_size)
 
-            # temp_count=0 
-            # if release_flag== True : 
+                # temp_count=0 
+                # if release_flag== True : 
+                    
+                for img in imagescreenshot_list:
+                    # Assuming the images are in BGR format, if not, convert them
+                    out_v.write(img)
+                    
+                out_v.release()   
+                # Release everything when done
                 
-            for img in imagescreenshot_list:
-                # Assuming the images are in BGR format, if not, convert them
-                out_v.write(img)
                 
-            out_v.release()   
-            # Release everything when done
-            
-            
-            os.replace(temp_file_name, save_gif_image)
+                os.replace(temp_file_name, save_gif_image)
            
             
             #if current_hour!=last_hour:
                # delete_older_mp4('plots/Videos', 1500)
                 
                 #shutil.move(temp_file_name, save_gif_image)
                 
@@ -3216,36 +3217,36 @@
            
             
         ######
        
        
        # Path to the custom directory
         custom_dir = 'plots/Videos/temp'
-
-        try:
-            # List all files in the directory
-            files = [os.path.join(custom_dir, f) for f in os.listdir(custom_dir) if os.path.isfile(os.path.join(custom_dir, f))]
-            
-            # Sort the files by modification time, most recent last
-            files.sort(key=lambda x: os.path.getmtime(x))
-            
-            # Remove the last file from the list to exclude it from deletion
-            files_to_delete = files[:-5]
-            
-            for file in files_to_delete:
-                try:
-                    os.remove(file)
-                except OSError as e:
-                    # Check if the error is WinError 32
-                    if e.winerror == 32:
-                        continue
-                    else:
-                        raise  # Re-raise the exception if it's not related to the file being in use
-        except Exception as e:
-            print(f"Error processing directory cleanup: {e}")
+        if release_flag==True:
+            try:
+                # List all files in the directory
+                files = [os.path.join(custom_dir, f) for f in os.listdir(custom_dir) if os.path.isfile(os.path.join(custom_dir, f))]
+                
+                # Sort the files by modification time, most recent last
+                files.sort(key=lambda x: os.path.getmtime(x))
+                
+                # Remove the last file from the list to exclude it from deletion
+                files_to_delete = files[:-5]
+                
+                for file in files_to_delete:
+                    try:
+                        os.remove(file)
+                    except OSError as e:
+                        # Check if the error is WinError 32
+                        if e.winerror == 32:
+                            continue
+                        else:
+                            raise  # Re-raise the exception if it's not related to the file being in use
+            except Exception as e:
+                print(f"Error processing directory cleanup: {e}")
             
        
         cv2.imwrite(save_image,combined_frame, [int(cv2.IMWRITE_JPEG_QUALITY), 80] )
        
         
         ######################
```

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Filter_PreProc.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Filter_PreProc.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Mosaic_Crop.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Mosaic_Crop.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/OpticalFlow.py` & `akhdefo_functions-2.5.61/akhdefo_functions/OpticalFlow.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Stacked_Velocity.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Stacked_Velocity.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Unzip_CopyFiles.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Unzip_CopyFiles.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/Video_Streamer.py` & `akhdefo_functions-2.5.61/akhdefo_functions/Video_Streamer.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/__init__.py` & `akhdefo_functions-2.5.61/akhdefo_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions/backend.py` & `akhdefo_functions-2.5.61/akhdefo_functions/backend.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions.egg-info/PKG-INFO` & `akhdefo_functions-2.5.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: akhdefo-functions
-Version: 2.5.6
+Name: akhdefo_functions
+Version: 2.5.61
 Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `akhdefo_functions-2.5.6/akhdefo_functions.egg-info/SOURCES.txt` & `akhdefo_functions-2.5.61/akhdefo_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.6/setup.py` & `akhdefo_functions-2.5.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # Read the long description from the README file
 with open("./README_pypi.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setup configuration
 setup(
     name='akhdefo_functions',
-    version='2.5.6',
+    version='2.5.61',
     description='Land Deformation Monitoring Using Optical and SAR Satellite Imagery',
     url='https://github.com/mahmudsfu/AkhDefo',
     author='Mahmud Mustafa Muhammad',
     author_email='mahmud.muhamm1@gmail.com',
     license='Academic Free License (AFL)',
     packages=['akhdefo_functions'],
     long_description=long_description,
```

