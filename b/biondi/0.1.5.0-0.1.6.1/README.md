# Comparing `tmp/biondi-0.1.5.0.tar.gz` & `tmp/biondi-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\biondi-0.1.5.0.tar", last modified: Mon Mar 14 20:55:26 2022, max compression
+gzip compressed data, was "biondi-0.1.6.1.tar", last modified: Mon May 20 23:55:57 2024, max compression
```

## Comparing `biondi-0.1.5.0.tar` & `biondi-0.1.6.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-03-14 20:55:26.000000 biondi-0.1.5.0/
-drwxrwxrwx   0        0        0        0 2022-03-14 20:55:26.000000 biondi-0.1.5.0/biondi/
--rw-rw-rw-   0        0        0   125439 2022-02-25 01:51:32.000000 biondi-0.1.5.0/biondi/dataset.py
-drwxrwxrwx   0        0        0        0 2022-03-14 20:55:26.000000 biondi-0.1.5.0/biondi/misc/
--rw-rw-rw-   0        0        0     5403 2020-05-01 11:45:02.000000 biondi-0.1.5.0/biondi/misc/DCGAN.py
--rw-rw-rw-   0        0        0     7194 2020-04-30 06:34:51.000000 biondi-0.1.5.0/biondi/misc/infogan practice.py
--rw-rw-rw-   0        0        0     5914 2020-10-23 03:49:18.000000 biondi-0.1.5.0/biondi/misc/misc ai code.py
--rw-rw-rw-   0        0        0     2350 2020-05-01 22:47:39.000000 biondi-0.1.5.0/biondi/misc/WSI autoencoder.py
--rw-rw-rw-   0        0        0        0 2020-10-23 08:39:08.000000 biondi-0.1.5.0/biondi/misc/__init__.py
--rw-rw-rw-   0        0        0    44657 2022-02-22 21:33:17.000000 biondi-0.1.5.0/biondi/models.py
--rw-rw-rw-   0        0        0     9091 2022-02-16 23:42:38.000000 biondi-0.1.5.0/biondi/random stuff.py
--rw-rw-rw-   0        0        0    29528 2021-10-20 09:03:28.000000 biondi-0.1.5.0/biondi/statistics.py
--rw-rw-rw-   0        0        0       48 2021-03-04 05:20:26.000000 biondi-0.1.5.0/biondi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-14 20:55:26.000000 biondi-0.1.5.0/biondi.egg-info/
--rw-rw-rw-   0        0        0        1 2022-03-14 20:55:25.000000 biondi-0.1.5.0/biondi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      411 2022-03-14 20:55:25.000000 biondi-0.1.5.0/biondi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2022-03-14 20:55:25.000000 biondi-0.1.5.0/biondi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2022-03-14 20:55:25.000000 biondi-0.1.5.0/biondi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      411 2022-03-14 20:55:26.000000 biondi-0.1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2020-10-23 09:20:46.000000 biondi-0.1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2022-03-14 20:55:26.000000 biondi-0.1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      627 2022-03-14 20:54:07.000000 biondi-0.1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:55:57.622990 biondi-0.1.6.1/
+-rw-rw-rw-   0        0        0    35823 2020-10-23 09:30:39.000000 biondi-0.1.6.1/LICENSE
+-rw-rw-rw-   0        0        0      425 2024-05-20 23:55:57.621968 biondi-0.1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2020-10-23 09:20:46.000000 biondi-0.1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 23:55:57.601048 biondi-0.1.6.1/biondi/
+-rw-rw-rw-   0        0        0       48 2021-03-04 05:20:26.000000 biondi-0.1.6.1/biondi/__init__.py
+-rw-rw-rw-   0        0        0   158429 2024-05-20 22:43:53.000000 biondi-0.1.6.1/biondi/dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:55:57.619002 biondi-0.1.6.1/biondi/misc/
+-rw-rw-rw-   0        0        0     5403 2020-05-01 11:45:02.000000 biondi-0.1.6.1/biondi/misc/DCGAN.py
+-rw-rw-rw-   0        0        0     2350 2020-05-01 22:47:39.000000 biondi-0.1.6.1/biondi/misc/WSI autoencoder.py
+-rw-rw-rw-   0        0        0        0 2020-10-23 08:39:08.000000 biondi-0.1.6.1/biondi/misc/__init__.py
+-rw-rw-rw-   0        0        0     7194 2020-04-30 06:34:51.000000 biondi-0.1.6.1/biondi/misc/infogan practice.py
+-rw-rw-rw-   0        0        0     5914 2020-10-23 03:49:18.000000 biondi-0.1.6.1/biondi/misc/misc ai code.py
+-rw-rw-rw-   0        0        0    44678 2022-07-12 22:52:29.000000 biondi-0.1.6.1/biondi/models.py
+-rw-rw-rw-   0        0        0     6495 2024-05-20 23:40:14.000000 biondi-0.1.6.1/biondi/random delete 2.py
+-rw-rw-rw-   0        0        0    12239 2024-05-20 21:31:59.000000 biondi-0.1.6.1/biondi/random delete.py
+-rw-rw-rw-   0        0        0    27769 2024-04-29 23:59:50.000000 biondi-0.1.6.1/biondi/random stuff.py
+-rw-rw-rw-   0        0        0    29528 2021-10-20 09:03:28.000000 biondi-0.1.6.1/biondi/statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:55:57.609026 biondi-0.1.6.1/biondi.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-20 23:55:56.000000 biondi-0.1.6.1/biondi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2024-05-20 23:55:57.000000 biondi-0.1.6.1/biondi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:55:56.000000 biondi-0.1.6.1/biondi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 23:55:57.000000 biondi-0.1.6.1/biondi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:55:57.622990 biondi-0.1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      627 2024-05-20 23:54:45.000000 biondi-0.1.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `biondi-0.1.5.0/biondi/dataset.py` & `biondi-0.1.6.1/biondi/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 from tensorflow import keras
 from sklearn.neighbors import KDTree
 import h5py
 import pandas as pd
 import biondi.statistics
 import pickle
 import PIL
+from PIL import Image
 import math
-
+import seaborn as sns
+import sqlite3
 
 def load_tif(tif_file):
     # TODO: adjust code to load channels last regardles of skimage or imageio version
     """
     Warning: only use with skimage 0.15.x and imageio 2.6.1, newer versions of imageio load the image incorrectly.
     Returns array of a .tif image.
 
@@ -969,28 +971,29 @@
         column = i % num_of_columns
         row = i // num_of_columns
         # pixel range
         c_start = tile_size * column
         c_stop = c_start + tile_size
         r_start = tile_size * row
         r_stop = r_start + tile_size
-        print(f'Extracting bounding boxes: {i + 1} out of {len(tiles)}',end='      \r', flush=True)
+        print(f'Extracting bounding boxes: {i + 1} out of {len(tiles)}', end='      \r', flush=True)
 
         # ((c_start <= coords[:,0]) & (coords[:,0] < c_stop)) & ((r_start <= coords[:,1]) & (coords[:,1] < r_stop))
-        tile_coords = coords[((c_start <= coords[:,0]) & (coords[:,0] < c_stop)) & ((r_start <= coords[:,1]) & (coords[:,1] < r_stop))]
+        tile_coords = coords[((c_start <= coords[:, 0]) & (coords[:, 0] < c_stop)) & (
+                    (r_start <= coords[:, 1]) & (coords[:, 1] < r_stop))]
         x = int(bbox_size / 2)
         y0 = (tile_coords[:, 1] - r_start) - x
         y1 = (tile_coords[:, 1] - r_start) + x
         x0 = (tile_coords[:, 0] - c_start) - x
         x1 = (tile_coords[:, 0] - c_start) + x
         tile_coords = np.stack([y0, x0, y1, x1], axis=1)
         # (0 <= tile_coords) & (tile_coords < 1024)
         if len(tile_coords) != 0:
             # TODO: need to implement dynamic tile_sizes
-            tile_coords = tile_coords[np.all((0 <= tile_coords) & (tile_coords < 1024),axis=1)]
+            tile_coords = tile_coords[np.all((0 <= tile_coords) & (tile_coords < 1024), axis=1)]
             if len(tile_coords) != 0:
                 anc_params.append(tile_coords)
             else:
                 anc_params.append('None')
         else:
             anc_params.append('None')
     return anc_params
@@ -1153,25 +1156,25 @@
 def convert_anc_to_box_v2_2d(anc_params, boundingbox):
     """
     ***This code is meant for multiple feature maps***
     """
     boxes = {}
     for h in boundingbox.params['inputs_shapes'].keys():
         boxes[h] = []
-    #print('Converting extracted anchors to box parameters.')
+    # print('Converting extracted anchors to box parameters.')
     for i in range(len(anc_params)):
         print(f'Converting extracted anchors to box parameters: {i + 1} out of {len(anc_params)}', end='      \r',
               flush=True)
         box = boundingbox.convert_anc_to_box(anc_params[i], np.ones((anc_params[i].shape[0], 1)))
         for j in box.keys():
             boxes[j].append(box[j])
     for k in boxes.keys():
         # this will provide an array with 4 dims for a 2d image, will not work for 3d!
         boxes[k] = np.concatenate(boxes[k], axis=0)
-        print(k, boxes[k].shape,'                                          ', flush=True)
+        print(k, boxes[k].shape, '                                          ', flush=True)
         print('Finished!', flush=True)
     return boxes
 
 
 def normalized_tiles_and_bbox_params_from_wsi_mosaic_v2(wsi_tiles_filename, mosaic_metadata, coords, boundingbox,
                                                         normalize=False, bbox_size=64, tile_size=1024,
                                                         per_channel=False):
@@ -1200,18 +1203,20 @@
 
 def normalized_tiles_and_bbox_params_from_wsi_tiles_v2(wsi_tiles_filename, coords, boundingbox, normalize=False,
                                                        bbox_size=64, tile_size=1024, per_channel=False, nump=False):
     tiles = np.load(wsi_tiles_filename)
     if tiles.shape[3] == 4:
         tiles = tiles[:, :, :, :-1]
     if nump:
-        anc = anc_params_from_tiles_v2(tiles=tiles, coords=coords, wsi_tiles_filename=wsi_tiles_filename, bbox_size=bbox_size,
+        anc = anc_params_from_tiles_v2(tiles=tiles, coords=coords, wsi_tiles_filename=wsi_tiles_filename,
+                                       bbox_size=bbox_size,
                                        tile_size=tile_size)
     else:
-        anc = anc_params_from_tiles(tiles=tiles, coords=coords, wsi_tiles_filename=wsi_tiles_filename, bbox_size=bbox_size,
+        anc = anc_params_from_tiles(tiles=tiles, coords=coords, wsi_tiles_filename=wsi_tiles_filename,
+                                    bbox_size=bbox_size,
                                     tile_size=tile_size)
     sorted_tiles = []
     sorted_anc = []
     # print('Removing tiles without bounding boxes.')
     print(f'Removing tiles without bounding boxes.', end='                    \r', flush=True)
     for i in range(len(anc)):
         if type(anc[i]) != str:
@@ -2013,31 +2018,46 @@
             global_coords.append([c_start + local_coords[i][j, 0], r_start + local_coords[i][j, 1]])
     if len(global_coords) == 0:
         return None
     else:
         return np.array(global_coords)
 
 
-def cpec_coords_from_anc_v2(anc, num_of_columns, tile_size, half_res=False):
+def cpec_coords_from_anc_v2(anc, num_of_columns, tile_size, downsampled=False, ds_factor=2):
     # anc is a list(2: anchor coords and classes) of a list of arrays (1 array per image tile)
     # anc arrays are local coordinates for the tile
     # convert tile coords to WSI coords
+    """
+    Takes local tile anchor parameters output and converts them to WSI reference frame coordinates.
+    :param anc: list[anchor coords and classes] where anchor coords is list of arrays (1 array per image tile)
+    :type anc: list
+    :param num_of_columns: number of tile sized columns in the WSI. Used to convert local coords to WSI coords
+    :type num_of_columns: int
+    :param tile_size: Size of tile. Should be at the resolution that the AI model uses. Typically 256
+    :type tile_size: int
+    :param downsampled: Whether the coords were obtained from tiles at a downsampled resolution.
+    :type downsampled: bool
+    :param ds_factor: Downsample factor.
+    :type ds_factor: int
+    :return: array of WSI CPEC coords
+    :rtype: ndarray
+    """
     local_coords = []
     for j in range(len(anc[0])):
         if len(anc[0][j]) != 0:
             y_coords = (anc[0][j][:, 2] + anc[0][j][:, 0]) / 2
             x_coords = (anc[0][j][:, 3] + anc[0][j][:, 1]) / 2
             local_coords.append(np.stack([x_coords, y_coords], axis=1))
         else:
             local_coords.append(anc[0][j])
     wsi_coords = local_to_global_coords_retinanet_v2(local_coords, num_of_columns, tile_size)
-    if not half_res:
+    if not downsampled:
         return wsi_coords
-    elif half_res:
-        return (wsi_coords * 2).astype(int)
+    elif downsampled:
+        return (wsi_coords * ds_factor).astype(int)
     else:
         print('half_res parameter must be a boolean!')
         return
 
 
 def retinanet_prediction_output(WSI, model, boundingbox, batch_size=1, im_size=512, half_res=True, normalize=True,
                                 per_channel=False, two_channel=True):
@@ -2126,168 +2146,366 @@
                 normalize=normalize,
                 per_channel=per_channel,
                 two_channel=two_channel),
             iou_nms=iou_nms,
             apply_deltas=True),
         dim[0] // im_size,
         tile_size=tile_size,
-        half_res=half_res
+        downsampled=half_res
     )
     prediction_logits = classifier.predict(wsi_cpec_generator(wsi, coords))
     affected_coords = biondi.statistics.sort_affected_coords_from_aipredictions(
         biondi.statistics.convert_probabilities_to_predictions(prediction_logits),
         coords,
     )
     prevalence = (len(affected_coords) / len(coords)) * 100
     return {'coords': coords, 'af_coords': affected_coords, 'prevalence': prevalence}
 
 
 class PredictionGenerator(keras.utils.Sequence):
-    # TODO: add compatibility with vacuole 40x HE images. such as downscale factor and such
+    # TODO: consider add code to allow use of 40x WSI level for vesicles if the 10x level cannot be read by openslide.
+    # TODO: consider removing old parameter
     def __init__(self,
                  WSI,
-                 boundingbox,
+                 boundingbox=None,
                  batch_size=1,
                  im_size=512,
-                 half_res=True,
+                 downsample=True,
                  normalize=True,
                  per_channel=False,
-                 two_channel=True,
+                 two_channel=False,
                  prediction=False,
                  retinanet=False,
-                 coords=None):
+                 resnet_2D=False,
+                 coords=None,
+                 vesicles=False,
+                 old=False,
+                 low_level=False,):
         if type(WSI) is str:
             self.wsi = openslide.open_slide(WSI)
         else:
             self.wsi = WSI
         self.dim = self.wsi.dimensions
         self.im_size = im_size
         self.retinanet = retinanet
         if self.retinanet:
             self.tile_count = (self.dim[0] // self.im_size) * (self.dim[1] // self.im_size)
+        self.resnet_2D = resnet_2D
         self.column_num = self.dim[0] // self.im_size
-        self.boundingbox = boundingbox
+        if boundingbox != None:
+            self.boundingbox = boundingbox
+        if boundingbox == None and retinanet == True:
+            raise ValueError( 'Must provide boundingbox object for retinanet-based predictions!')
         self.batch_size = batch_size
-        self.half_res = half_res
+        self.downsample = downsample
         self.two_channel = two_channel
-        if self.half_res:
+        self.vesicles = vesicles
+        self.low_level = low_level
+        if self.vesicles:
+            self.dsf = 4
+            self.cpec_im_size = 128
+        else:
+            self.dsf = 2
+            self.cpec_im_size = 64
+        if self.downsample and not self.vesicles:
             if self.two_channel:
-                self.downscale_model = biondi.dataset.half_tile_resolution(self.im_size, channels=2)
+                self.downscale_model = biondi.dataset.downsampling_model(self.im_size, downsample_factor=self.dsf, channels=2)
             else:
-                self.downscale_model = biondi.dataset.half_tile_resolution(self.im_size)
+                self.downscale_model = biondi.dataset.downsampling_model(self.im_size, downsample_factor=self.dsf)
+        if self.vesicles and self.low_level:
+            self.downscale_model = biondi.dataset.downsampling_model(self.im_size, downsample_factor=self.dsf)
         self.normalize = normalize
         self.per_channel = per_channel
         if self.two_channel:
             self.c_idx_start = 1
         else:
             self.c_idx_start = 0
         self.prediction = prediction
         self.coords = coords
+        self.old = old
         self.on_epoch_end()
 
     def __len__(self):
         if self.retinanet:
             return int(np.ceil(self.tile_count / self.batch_size))
         else:
             return int(np.ceil(len(self.coords) / self.batch_size))
 
     def __getitem__(self, index):
         batch = []
         if self.retinanet:
             for idx in self.indexes[index * self.batch_size:(index + 1) * self.batch_size]:
                 r = idx // self.column_num
                 c = idx % self.column_num
-                batch.append(
-                    np.array(self.wsi.read_region((c * self.im_size, r * self.im_size), 0, (self.im_size, self.im_size))
-                             )[..., self.c_idx_start:-1])
+                if self.vesicles:
+                    if self.low_level:
+                        batch.append(
+                            np.array(self.wsi.read_region((c * self.im_size, r * self.im_size), 0, (self.im_size, self.im_size))
+                                     )[..., self.c_idx_start:-1])
+                    else:
+                        batch.append(
+                            np.array(self.wsi.read_region((c * self.im_size, r * self.im_size), 1,
+                                                          (int(self.im_size / self.dsf), int(self.im_size / self.dsf)))
+                                     )[..., self.c_idx_start:-1])
+                else:
+                    batch.append(
+                        np.array(self.wsi.read_region((c * self.im_size, r * self.im_size), 0, (self.im_size, self.im_size))
+                                 )[..., self.c_idx_start:-1])
             batch = np.stack(batch)
         else:
             batch_idx = self.indexes[index * self.batch_size:(index + 1) * self.batch_size]
-            batch = wsi_cell_extraction_from_coords_v3(self.wsi, im_size=64, coords=self.coords[batch_idx], verbose=0)
-        if self.half_res:
-            batch = self.downscale_model(batch.astype('float32'))
+            batch = biondi.dataset.wsi_cell_extraction_from_coords_v3(self.wsi, im_size=self.cpec_im_size, coords=self.coords[batch_idx], verbose=0)
+        if self.downsample and not self.vesicles:
+            batch = self.downscale_model(batch.astype('float32')).numpy()
+        if self.downsample and self.low_level and self.vesicles:
+            batch = self.downscale_model(batch.astype('float32')).numpy()
         if self.normalize:
             batch = biondi.dataset.per_sample_tile_normalization(batch, per_channel=self.per_channel)
         if self.retinanet:
             batch_dict = {'dat': np.expand_dims(batch, axis=1)}
-            # TODO: Need to include cls and reg inputs in dictionary
             for key in self.boundingbox.params['inputs_shapes'].keys():
-                if 'msk' in key:
-                    batch_dict[key] = np.zeros(
-                        shape=(self.batch_size,) + tuple(self.boundingbox.params['inputs_shapes'][key]))
+                batch_dict[key] = np.zeros(
+                    shape=(len(batch_dict['dat']),) + tuple(self.boundingbox.params['inputs_shapes'][key]))
             return batch_dict
         else:
-            return np.expand_dims(batch, axis=1)
+            if self.resnet_2D:
+                return batch
+            else:
+                return np.expand_dims(batch, axis=1)
 
     def on_epoch_end(self):
         if self.retinanet:
             self.indexes = np.arange(self.tile_count)
         else:
             self.indexes = np.arange(len(self.coords))
 
 
-def retinanet_prediction_output_v2(WSI, model, boundingbox):
+def retinanet_prediction_output_v2(WSI, model, boundingbox, downsample, im_size, two_channel, old=False, vesicle=False):
     # want to add path boolean and code load model if model is a filepath
     output = model.predict(
-        PredictionGenerator(WSI, boundingbox, batch_size=8, retinanet=True),
+        PredictionGenerator(WSI, boundingbox, batch_size=32, retinanet=True, downsample=downsample, im_size=im_size,
+                            two_channel=two_channel, old=old, vesicles=vesicle),
         verbose=1,
-        workers=8,
-        max_queue_size=64
+        workers=12,
+        max_queue_size=128
     )
-    # TODO: TF 2.5 seems to output a dictionary and the blow  line of code now just produces a dictionary without any actually data, only string names.
-    output_dic = {name: pred for name, pred in zip(model.output_names, output)}
-    return output_dic
+    return output
 
 
 def biondi_prevalence_and_coords_v2(WSI,
                                     retinanet,
                                     classifier,
                                     boundingbox,
                                     im_size=512,
                                     half_res=True,
                                     iou_nms=0.3,
-                                    return_predictions=False):
+                                    return_predictions=False,
+                                    two_channel=False,
+                                    filter_coords=True,
+                                    filter_threshold=110,
+                                    old=False):
+    """
+    Returns Biondi body prevalence and coords.
+
+    :param WSI: WSI filepath or Openslide object
+    :type WSI: str or openslide object
+    :param retinanet: retinanet CPEC detection model
+    :type retinanet: Keras model
+    :param classifier: resnet CPEC classifier model
+    :type classifier: Keras model
+    :param boundingbox: bounding box from Jarvis package
+    :type boundingbox: boundingbox object
+    :param im_size: Size of image tiles fed into the retinanet model before downsampling. Should be 512 for Biondi bodies.
+    :type im_size: int
+    :param half_res:
+    :type half_res: bool
+    :param iou_nms: non-max suppression threshold
+    :type iou_nms: float
+    :param return_predictions: Whether to return predictions
+    :type return_predictions: bool
+    :param two_channel:
+    :type two_channel: bool
+    :param filter_coords: Whether to filter predicted CPEC coords to remove coords unlike to be CPECs based on proximity
+    of neighboring cells.
+    :type filter_coords: bool
+    :param filter_threshold: Threshold to check for neighboring CPECs for filtering coords. Typically 110 which
+    corresponds roughly to 35.4 microns.
+    :type filter_threshold: int
+    :param old:
+    :type old: bool
+    :return: total coords, affected coords, Biondi body prevalence, and predictions (optional)
+    :rtype: dict
+    """
     if type(WSI) is str:
         wsi = openslide.open_slide(WSI)
     else:
         wsi = WSI
     dim = wsi.dimensions
     if half_res:
         tile_size = im_size // 2
     else:
         tile_size = im_size
     coords = cpec_coords_from_anc_v2(
         boundingbox.convert_box_to_anc(
             retinanet_prediction_output_v2(
                 WSI=wsi,
                 model=retinanet,
-                boundingbox=boundingbox
+                boundingbox=boundingbox,
+                downsample=half_res,
+                im_size=im_size,
+                two_channel=two_channel,
+                old=old,
             ),
             iou_nms=iou_nms,
             apply_deltas=True),
         dim[0] // im_size,
         tile_size=tile_size,
-        half_res=half_res,
+        downsampled=half_res,
+        ds_factor=2,
     )
+    if filter_coords:
+        coords = binary_stats(coords, f_threshold=filter_threshold)
     prediction_logits = classifier.predict(
-        PredictionGenerator(wsi, boundingbox, batch_size=32, half_res=False, retinanet=False, coords=coords),
+        PredictionGenerator(wsi, boundingbox, batch_size=32, downsample=False, retinanet=False, coords=coords),
         verbose=1,
-        workers=8,
-        max_queue_size=64
-    )
-    predictions = biondi.statistics.convert_probabilities_to_predictions(prediction_logits)
-    affected_coords = biondi.statistics.sort_affected_coords_from_aipredictions(
-        predictions,
-        coords,
+        workers=12,
+        max_queue_size=128,
     )
+    predictions = np.argmax(prediction_logits, axis=-1)
+    affected_coords = coords[predictions == 1]
     prevalence = (len(affected_coords) / len(coords)) * 100
     if return_predictions:
-        return {'coords': coords, 'af_coords': affected_coords, 'prevalence': prevalence, 'predictions': predictions, }
+        return {'coords': coords,
+                'af_coords': affected_coords,
+                'prevalence': prevalence,
+                'predictions': predictions, }
+    else:
+        return {'coords': coords,
+                'af_coords': affected_coords,
+                'prevalence': prevalence}
+
+
+def vesicle_prevalence_and_coords(WSI,
+                                     retinanet,
+                                     classifier,
+                                     boundingbox,
+                                     im_size=1024,
+                                     downsample=True,
+                                     iou_nms=0.3,
+                                     return_predictions=False,
+                                     filter_coords=False,
+                                     filter_threshold=258,
+                                     old=False,
+                                     binary_predictions=True,
+                                     secondary_classifier=None):
+    if type(WSI) is str:
+        wsi = openslide.open_slide(WSI)
     else:
-        return {'coords': coords, 'af_coords': affected_coords, 'prevalence': prevalence}
+        wsi = WSI
+    dim = wsi.dimensions
+    tile_size = im_size // 4
+    coords = cpec_coords_from_anc_v2(
+        boundingbox.convert_box_to_anc(
+            retinanet_prediction_output_v2(
+                WSI=wsi,
+                model=retinanet,
+                boundingbox=boundingbox,
+                downsample=downsample,
+                im_size=im_size,
+                two_channel=False,
+                old=old,
+                vesicle=True
+            ),
+            iou_nms=iou_nms,
+            apply_deltas=True),
+        dim[0] // im_size,
+        tile_size=tile_size,
+        downsampled=downsample,
+        ds_factor=4,
+    )
+    if filter_coords:
+        # f_threshold value may need checking/optimization. Number is based off value used for biondi bodies
+        # (35.4 microns) but is adjusted based on the resolution of 40x brightfield images, which is 258.
+        coords = binary_stats(coords, f_threshold=filter_threshold)
+    binary_prediction_logits = classifier.predict(
+        PredictionGenerator(wsi, boundingbox, batch_size=32, downsample=False,
+                            retinanet=False, coords=coords, vesicles=True),
+        verbose=1,
+        workers=12,
+        max_queue_size=128,
+    )
+    # predictions are currently binary
+    binary_prediction = np.argmax(binary_prediction_logits, axis=-1)
+    if not binary_predictions:
+        full_prediction_logits = secondary_classifier.predict(
+            PredictionGenerator(wsi, boundingbox, batch_size=32, downsample=False,
+                                retinanet=False, coords=coords[binary_prediction==1], vesicles=True),
+            verbose=1,
+            workers=12,
+            max_queue_size=128,
+        )
+        full_prediction = np.argmax(full_prediction_logits, axis=-1) + 1
+        coords = np.concatenate([coords[binary_prediction==0],coords[binary_prediction==1]], axis=0)
+        full_predictions = np.concatenate([binary_prediction[binary_prediction==0], full_prediction], axis=0)
+    else:
+        coords = coords
+        full_predictions = binary_prediction
+    # affected_coords = coords[predictions == 1]
+    prevalence = (len(coords[full_predictions>0]) / len(coords)) * 100
+    if return_predictions:
+        return {'coords': coords,
+                'binary prevalence': prevalence,
+                'predictions': full_predictions, }
+    else:
+        return {'coords': coords,
+                'binary prevalence': prevalence}
+
+
+def binary_stats(pred, true=None, threshold=30, f_threshold=110):
+    """
+    Filters predicted CPEC coords to filter out cells unlikely to be CPECs by checking if any other cells are nearby.
+    Will provide some binary statistics if true CPEC coords are given.
+    :param pred: predicted CPEC coords
+    :type pred: ndarray
+    :param true: True CPEC coords (optional)
+    :type true: ndarray
+    :param threshold: Distance threshold to determine if two coordinates are the same cell.
+    :type threshold: int
+    :param f_threshold:Threshold to check for neighboring CPECs for filtering coords. Typically 110 which corresponds
+    roughly to 35.4 microns.
+    :type f_threshold: int
+    :return: returns filtered coords and prints some binary statistics if True coords are also provided
+    :rtype: ndarray
+    """
+    PT = KDTree(pred)
+    #TODO: recode how checking for true parameter handles arrays, current spits errors if an array is passed to true.
+    if not true:
+        distance = PT.query(pred, k=2, return_distance=True)[0][:, 1]
+        return pred[distance < f_threshold]
+    TT = KDTree(true)
+    TP = np.sum(TT.query(pred)[0] < threshold)
+    FP = np.sum(TT.query(pred)[0] > threshold)
+    P = len(true)
+    FN = np.sum(PT.query(true)[0] > threshold)
+    TPR1 = TP / (TP + FN)
+    TPR2 = TP / P
+    PPV = TP / (TP + FP)
+    FNR1 = FN / (FN + TP)
+    FNR2 = FN / P
+    FDR = FP / (FP + TP)
+    print(f'TP = {TP}')
+    print(f'FP = {FP}')
+    print(f'P = {P}')
+    print(f'FN(may be inappropriate) = {FN}')
+    print(f'TPR = {TPR1} (TP/(TP+FN)) or {TPR2} (TP/P)')
+    print(f'PPV = {PPV}')
+    print(f'FNR(may be inappropriate) = {FNR1} (FN/(FN+TP)) or {FNR2} (FN/P)')
+    print(f'FDR = {FDR}')
+    distance = TT.query(pred, k=2, return_distance=True)[0][:, 1]
+    return pred[distance < f_threshold]
 
 
 def random_adjust_brightness(x, b_delta, batch_size):
     return np.clip(
         ((x / 255) + np.random.uniform(-b_delta, b_delta, size=(batch_size, 1, 1, 1, 1))) * 255,
         a_min=0,
         a_max=255
@@ -2300,71 +2518,80 @@
         (((x / 255) - mean) * np.random.uniform(c_factor_min, c_factor_max, size=(batch_size, 1, 1, 1, 1)) +
          mean) * 255,
         a_min=0,
         a_max=255
     )
 
 
+# TODO: update code to use keras augmentation functions
+# TODO: add ability to choose single image channels.
 class TrainingGenerator(keras.utils.Sequence):
     def __init__(self,
                  data,
                  batch_size,
                  labels=None,
                  normalize=True,
                  per_channel=False,
                  two_channel=False,
                  retinanet=False,
+                 resnet_2D=False,
                  validation=False,
-                 augmentation=False,
                  flip=False,
                  rotation=False,
-                 rand_brightness=False,
-                 rand_contrast=False,
-                 simultaneous_aug=False,
-                 b_delta=0.95,
-                 c_factor_min=0.1,
-                 c_factor_max=0.9, ):
+                 contrast=False,
+                 c_factor=0.9,
+                 r_factor=0.4,
+                 prediction=False,
+                 **kwargs):
         self.retinanet = retinanet
         self.batch_size = batch_size
         self.normalize = normalize
         self.per_channel = per_channel
         self.two_channel = two_channel
         self.validation = validation
-        self.augmentation = augmentation
+        self.prediction = prediction
+        self.resnet_2D = resnet_2D
         self.flip = flip
+        if self.flip:
+            # will likely need to update this code when moving to a newer version of TF/Keras
+            self.flipper = keras.layers.experimental.preprocessing.RandomFlip()
         self.rotation = rotation
-        self.rand_brightness = rand_brightness
-        self.rand_contrast = rand_contrast
-        self.simultaneous_aug = simultaneous_aug
-        self.b_delta = b_delta
-        self.c_factor_min = c_factor_min
-        self.c_factor_max = c_factor_max
+        self.r_factor = r_factor
+        if self.rotation:
+            # will likely need to update this code when moving to a newer version of TF/Keras
+            self.rotator = keras.layers.experimental.preprocessing.RandomRotation(self.r_factor)
+        self.contrast = contrast
+        self.c_factor = c_factor
+        if self.contrast:
+            # will likely need to update this code when moving to a newer version of TF/Keras
+            self.contraster = keras.layers.experimental.preprocessing.RandomContrast(self.c_factor)
         if type(data) is str:
             if '.pickle' in data:
                 with open(data, 'rb') as handle:
                     self.data = pickle.load(handle)
             elif '.npy' in data:
                 self.data = np.load(data)
-                if self.data.ndim != 5:
-                    self.data = np.expand_dims(self.data, axis=1)
-                    if self.data.ndim != 5:
+                if self.data.ndim != 4:
+                    self.data = np.squeeze(self.data)
+                    if self.data.ndim != 4:
                         raise ValueError(f"Data ndim is {self.data.ndim}. Data needs to have either 4 or 5 dimensions.")
             else:
                 raise ValueError('Warning: Filetype is not recognized. Only ".pickle" and ".npy" filetypes are supported.')
         else:
             if self.retinanet:
                 self.data = data
             else:
                 if data.ndim == 5:
-                    self.data = data
+                    self.data = np.squeeze(data)
                 else:
-                    self.data = np.expand_dims(data, axis=1)
+                    self.data = data
         if self.retinanet:
             self.sample_number = len(self.data['dat'])
             self.keys = self.data.keys()
+            self.data['dat'] = np.squeeze(self.data['dat'])
         else:
             self.sample_number = len(self.data)
             if labels is not None:
                 if type(labels) is str:
                     self.labels = np.load(labels)
                 else:
                     self.labels = labels
@@ -2383,116 +2610,46 @@
     def __getitem__(self, index):
         batch_idx = self.indexes[index * self.batch_size:(index + 1) * self.batch_size]
         if self.retinanet:
             x_batch = {}
             y_batch = {}
             for key in self.keys:
                 if 'dat' in key:
-                    if self.rand_contrast and self.rand_brightness:
-                        if self.simultaneous_aug:
-                            x_batch[key] = random_adjust_brightness(
-                                self.data[key][batch_idx, ..., self.c_idx_start:],
-                                b_delta=self.b_delta,
-                                batch_size=len(batch_idx)
-                            )
-                            x_batch[key] = random_adjust_contrast(
-                                x_batch[key],
-                                c_factor_min=self.c_factor_min,
-                                c_factor_max=self.c_factor_max,
-                                batch_size=len(batch_idx)
-                            )
-                        else:
-                            rand_bools = np.random.choice([False, True], size=self.batch_size)
-                            x_batch[key] = self.data[key][batch_idx, ..., self.c_idx_start:].astype('float32')
-                            for i, j in enumerate(rand_bools):
-                                if j:
-                                    x_batch[key][i:i + 1] = random_adjust_contrast(
-                                        x_batch[key][i:i + 1],
-                                        c_factor_min=self.c_factor_min,
-                                        c_factor_max=self.c_factor_max,
-                                        batch_size=1
-                                    )
-                                else:
-                                    x_batch[key][i:i + 1] = random_adjust_brightness(
-                                        x_batch[key][i:i + 1],
-                                        b_delta=self.b_delta,
-                                        batch_size=1
-                                    )
-                    elif self.rand_brightness:
-                        x_batch[key] = random_adjust_brightness(
-                            self.data[key][batch_idx, ..., self.c_idx_start:],
-                            b_delta=self.b_delta,
-                            batch_size=len(batch_idx)
-                        )
-                    elif self.rand_contrast:
-                        x_batch[key] = random_adjust_contrast(
-                            self.data[key][batch_idx, ..., self.c_idx_start:],
-                            c_factor_min=self.c_factor_min,
-                            c_factor_max=self.c_factor_max,
-                            batch_size=len(batch_idx)
-                        )
-                    else:
-                        x_batch[key] = self.data[key][batch_idx, ..., self.c_idx_start:]
+                    x_batch[key] = self.data[key][batch_idx, ..., self.c_idx_start:]
+                    if self.contrast and not self.validation:
+                        x_batch[key] = self.contraster(x_batch[key]).numpy()
                     if self.normalize:
-                        x_batch[key] = per_sample_tile_normalization(x_batch[key], per_channel=self.per_channel)
+                        x_batch[key] = biondi.dataset.per_sample_tile_normalization(x_batch[key],
+                                                                                    per_channel=self.per_channel)
+                    x_batch[key] = np.expand_dims(x_batch[key], axis=1)
                 elif 'msk' in key:
                     x_batch[key] = self.data[key][batch_idx]
                 else:
-                    y_batch[key] = self.data[key][batch_idx]
-            return x_batch, y_batch
+                    x_batch[key] = self.data[key][batch_idx]
+            return x_batch
         else:
-            if self.rand_contrast and self.rand_brightness:
-                if self.simultaneous_aug:
-                    x_batch = random_adjust_brightness(
-                        self.data[batch_idx, ..., self.c_idx_start:],
-                        b_delta=self.b_delta,
-                        batch_size=len(batch_idx)
-                    )
-                    x_batch = random_adjust_contrast(
-                        x_batch,
-                        c_factor_min=self.c_factor_min,
-                        c_factor_max=self.c_factor_max,
-                        batch_size=len(batch_idx)
-                    )
-                else:
-                    rand_bools = np.random.choice([False, True], size=self.batch_size)
-                    x_batch = self.data[batch_idx, ..., self.c_idx_start:].astype('float32')
-                    for i, j in enumerate(rand_bools):
-                        if j:
-                            x_batch[i:i + 1] = random_adjust_contrast(
-                                x_batch[i:i + 1],
-                                c_factor_min=self.c_factor_min,
-                                c_factor_max=self.c_factor_max,
-                                batch_size=1
-                            )
-                        else:
-                            x_batch[i:i + 1] = random_adjust_brightness(
-                                x_batch[i:i + 1],
-                                b_delta=self.b_delta,
-                                batch_size=1
-                            )
-            elif self.rand_brightness:
-                x_batch = random_adjust_brightness(
-                    self.data[batch_idx, ..., self.c_idx_start:],
-                    b_delta=self.b_delta,
-                    batch_size=len(batch_idx)
-                )
-            elif self.rand_contrast:
-                x_batch = random_adjust_contrast(
-                    self.data[batch_idx, ..., self.c_idx_start:],
-                    c_factor_min=self.c_factor_min,
-                    c_factor_max=self.c_factor_max,
-                    batch_size=len(batch_idx)
-                )
-            else:
-                x_batch = self.data[batch_idx, ..., self.c_idx_start:]
+            x_batch = self.data[batch_idx, ..., self.c_idx_start:]
+            if self.flip and not self.validation:
+                x_batch = self.flipper(x_batch).numpy()
+            if self.rotation and not self.validation:
+                x_batch = self.rotator(x_batch).numpy()
+            if self.contrast and not self.validation:
+                x_batch = self.contraster(x_batch).numpy()
+
             if self.normalize:
-                x_batch = per_sample_tile_normalization(x_batch, per_channel=self.per_channel)
+                x_batch = biondi.dataset.per_sample_tile_normalization(x_batch, per_channel=self.per_channel)
+            if self.resnet_2D:
+                pass
+            else:
+                x_batch = np.expand_dims(x_batch, axis=1)
             y_batch = self.labels[batch_idx]
-            return x_batch, y_batch
+            if self.prediction:
+                return x_batch
+            else:
+                return x_batch, y_batch
 
     def on_epoch_end(self):
         if self.validation:
             self.indexes = np.arange(self.sample_number)
         else:
             # not necessary since keras shuffles the index it gives __getitem__()
             # self.indexes = np.random.permutation(self.sample_number)
@@ -2532,26 +2689,25 @@
         row = i // grid_width
         # pixel range
         c_start = int(tile_size / downscale_factor) * column
         c_stop = c_start + int(tile_size / downscale_factor)
         r_start = int(tile_size / downscale_factor) * row
         r_stop = r_start + int(tile_size / downscale_factor)
         # TODO: reconsider print output, message rate will likely be too fast
-        print(f'Extracting bounding boxes: {i + 1} out of {max_tiles}',end='      \r', flush=True)
+        print(f'Extracting bounding boxes: {i + 1} out of {max_tiles}', end='      \r', flush=True)
         tile_coords = scaled_coords[((c_start <= scaled_coords[:, 0]) & (scaled_coords[:, 0] < c_stop)) & (
                 (r_start <= scaled_coords[:, 1]) & (scaled_coords[:, 1] < r_stop))]
         x = int((bbox_size / downscale_factor) / 2)
         y0 = (tile_coords[:, 1] - r_start) - x
         y1 = (tile_coords[:, 1] - r_start) + x
         x0 = (tile_coords[:, 0] - c_start) - x
         x1 = (tile_coords[:, 0] - c_start) + x
         tile_coords = np.stack([y0, x0, y1, x1], axis=1)
         if len(tile_coords) != 0:
-            # TODO: Implement dynamic tilesizes for param comparisons
-            tile_coords = tile_coords[np.all((0 <= tile_coords) & (tile_coords < 1024), axis=1)]
+            tile_coords = tile_coords[np.all((0 <= tile_coords) & (tile_coords < tile_size), axis=1)]
             if len(tile_coords) != 0:
                 anc_params.append(tile_coords)
             else:
                 anc_params.append('None')
         else:
             anc_params.append('None')
     return anc_params
@@ -2577,15 +2733,15 @@
         r = i // grid_width
         c = i % grid_width
         # TODO: Double check that level param is correct, consider changing if sampling 10x level
         batch.append(
             np.array(WSI.read_region((c * tile_size, r * tile_size), 0, (tile_size, tile_size)))[..., :-1])
     batch = np.stack(batch)
     if downscale_factor != 1:
-        model = downsample(im_size=tile_size, downsample_factor=downscale_factor)
+        model = downsampling_model(im_size=tile_size, downsample_factor=downscale_factor)
         batch = model.predict(batch)
     if normalize:
         images = per_sample_tile_normalization(batch, per_channel=per_channel)
     else:
         images = batch
     return images, im_boxes
 
@@ -2607,15 +2763,26 @@
     )
     boxes['dat'] = tiles
     for key in boxes.keys():
         boxes[key] = np.expand_dims(boxes[key], axis=1)
     return boxes
 
 
-def downsample(im_size, downsample_factor=2, channels=3):
+def downsampling_model(im_size, downsample_factor=2, channels=3):
+    """
+    Creates a model to utilizing average pooling to downsample an image
+    :param im_size: Size of the original image
+    :type im_size: int
+    :param downsample_factor: Factor by which to downsample image
+    :type downsample_factor: int
+    :param channels: Number of channels in the image. Usually 3, but can vary for fluorescent images.
+    :type channels: int
+    :return: A downsampling model
+    :rtype: Keras model
+    """
     inputs = keras.Input(shape=(im_size, im_size, channels))
     out = keras.layers.AveragePooling2D(pool_size=downsample_factor)(inputs)
     model = keras.Model(inputs=inputs, outputs=out)
     return model
 
 
 def fibrosis_tiles_and_masks_quarterres_v1(wsi_path, papilla, dense, hyalinized, mineralized):
@@ -2657,15 +2824,15 @@
     dense_pts = pd.read_csv(dense).to_numpy()[:, 1:6]
     hyalinized_pts = pd.read_csv(hyalinized).to_numpy()[:, 1:6]
     mineralized_pts = pd.read_csv(mineralized).to_numpy()[:, 1:6]
     real_tile_indices = pd.read_csv(papilla).to_numpy()[:, 5]
     unique_tile_indices = np.unique(real_tile_indices)
     WSI = TileLoaderV2(wsi_path)
     tile_num = len(unique_tile_indices)
-    counter=0
+    counter = 0
     # model = biondi.dataset.half_tile_resolution(4096)
     for i in unique_tile_indices:
         tile_pts = [
             papilla_pts[papilla_pts[:, -1] == i],
             dense_pts[dense_pts[:, -1] == i],
             hyalinized_pts[hyalinized_pts[:, -1] == i],
             mineralized_pts[mineralized_pts[:, -1] == i],
@@ -2702,23 +2869,26 @@
             raise ValueError('Masks list is unexpectedly empty!')
         else:
             masks = np.clip(np.add.reduce(masks, dtype=np.uint8), 0, 1)
             # print(masks.dtype)
             return masks
 
 
-def generate_mask_quarterres_v2(pts):
+def generate_mask_quarterres_v2(pts, cellmask=False):
     if pts.shape[0] == 0:
         return np.zeros(shape=(1024, 1024), dtype=np.uint8)
     else:
         masks = []
         unique_tags = np.unique(pts[:, 2])
         for i in unique_tags:
             img = PIL.Image.new('L', (1024, 1024), 0)
-            PIL.ImageDraw.Draw(img).polygon([tuple(i) for i in (pts[pts[:, 2] == i][:, :2]*1)], outline=1, fill=1)
+            if cellmask:
+                PIL.ImageDraw.Draw(img).polygon([tuple(i) for i in (pts[pts[:, 2] == i][:, :2] / 8)], outline=1, fill=1)
+            else:
+                PIL.ImageDraw.Draw(img).polygon([tuple(i) for i in (pts[pts[:, 2] == i][:, :2] * 1)], outline=1, fill=1)
             masks.append(np.array(img))
         if len(masks) == 1:
             # print(masks[0].dtype)
             return masks[0]
         elif len(masks) == 0:
             raise ValueError('Masks list is unexpectedly empty!')
         else:
@@ -2737,14 +2907,15 @@
         self.exclusion_line_width = 5
 
 
 class TileLoaderV1:
     """
     Tileloader to load tiles as implemented in fibrosis client 1.0.0 adn 1.1.0. Do not use on 1.2.0+ or on 0.2.0.
     """
+
     def __init__(self, file_path, c=CConstants):
         self.C = c
         self.wsi_image = openslide.open_slide(file_path)
         self.width, self.height = self.wsi_image.dimensions
         self.max_tiles = (self.width // self.C.tile_size, self.height // self.C.tile_size)  # (x, y) max tiles
         self.check_excess()
 
@@ -2824,23 +2995,25 @@
         return y
 
 
 class TileLoaderV2:
     """
     Tileloader to load tiles as implemented in fibrosis client 1.2.0.
     """
+
     def __init__(self, file_path, c=CConstants):
         self.C = c
         self.wsi_image = openslide.open_slide(file_path)
         self.width, self.height = self.wsi_image.dimensions
         self.max_tiles = (self.width // self.C.tile_size, self.height // self.C.tile_size)  # (x, y) max tiles
         # self.check_excess()
 
     def check_excess(self):
-        all_tiles = (self.width // (self.C.tile_size // self.C.tile_width), self.height // (self.C.tile_size // self.C.tile_width))
+        all_tiles = (
+        self.width // (self.C.tile_size // self.C.tile_width), self.height // (self.C.tile_size // self.C.tile_width))
         curr_x = self.max_tiles[0]
         curr_y = self.max_tiles[1]
 
         if curr_x * 2 < all_tiles[0]:
             curr_x += 1
         if curr_y * 2 < all_tiles[1]:
             curr_y += 1
@@ -2918,15 +3091,15 @@
                  batch_size,
                  normalize=True,
                  validation=False,
                  flip=False,
                  rotation=False,
                  contrast=False,
                  c_factor=0.9,
-                 r_factor=0.4,):
+                 r_factor=0.4, ):
         self.batch_size = batch_size
         self.normalize = normalize
         self.validation = validation
         self.flip = flip
         if self.flip:
             # will likely need to update this code when moving to a newer version of TF/Keras
             self.flipper = keras.layers.experimental.preprocessing.RandomFlip()
@@ -2968,14 +3141,15 @@
         return x_batch, y_batch
 
 
 class UnetPredictionGenerator(keras.utils.Sequence):
     """
     Currently only works to produce 10X images from 40x WSIs.
     """
+
     def __init__(self,
                  WSI,
                  batch_size=16,
                  im_size=512,
                  wsi_level=1,
                  normalize=True):
         if type(WSI) is str:
@@ -3003,35 +3177,59 @@
 
     def __getitem__(self, index):
         batch = []
         for idx in self.indexes[index * self.batch_size:(index + 1) * self.batch_size]:
             r = idx // self.column_num
             c = idx % self.column_num
             batch.append(
-                np.array(self.wsi.read_region((c * self.im_size*4, r * self.im_size*4), self.wsi_level, (self.im_size, self.im_size))
+                np.array(self.wsi.read_region((c * self.im_size * 4, r * self.im_size * 4), self.wsi_level,
+                                              (self.im_size, self.im_size))
                          )[..., :-1])
         batch = np.stack(batch)
         if self.normalize:
             batch = biondi.dataset.per_sample_tile_normalization(batch, per_channel=False).astype('float32')
         return np.expand_dims(batch, axis=1)
 
 
-def unet_prediction(model, PredictionGenerator, verbose=1):
+def downsampling3D_model(im_size, downsample_factor=2, channels=3):
+    """
+    Creates a model to utilizing average pooling to downsample 2D images represented as 5D tensors/arrays.
+    :param im_size: Size of the original image
+    :type im_size: int
+    :param downsample_factor: Factor by which to downsample image
+    :type downsample_factor: int
+    :param channels: Number of channels in the image. Usually 3, but can vary for fluorescent images.
+    :type channels: int
+    :return: A downsampling model
+    :rtype: Keras model
+    """
+    inputs = keras.Input(shape=(1, im_size, im_size, channels))
+    out = keras.layers.AveragePooling3D(pool_size=(1, downsample_factor, downsample_factor))(inputs)
+    model = keras.Model(inputs=inputs, outputs=out)
+    return model
+
+
+def unet_prediction(model, PredictionGenerator, verbose=1, workers=8, max_queue_size=64):
     tiles = {
         'filename': PredictionGenerator.filename,
         'zones0': [],
         'zones1': [],
         'zones2': [],
         'zones3': [],
     }
+    ds_model = downsampling3D_model(512, channels=2)
+    enqueuer = keras.utils.OrderedEnqueuer(PredictionGenerator)
+    enqueuer.start(workers=workers, max_queue_size=max_queue_size)
+    datas = enqueuer.get()
     progbar = keras.utils.Progbar(PredictionGenerator.__len__(), verbose=verbose)
     for i in range(PredictionGenerator.__len__()):
-        for key, output in model.predict(PredictionGenerator.__getitem__(i)).items():
-            tiles[key].append(np.argmax(biondi.statistics.softmax(output), axis=-1).astype('uint8'))
+        for key, output in model.predict_on_batch(next(datas)).items():
+            tiles[key].append(np.argmax(ds_model.predict(output), axis=-1).astype('uint8'))
         progbar.add(1)
+    enqueuer.stop()
     for key, output in tiles.items():
         if key != 'filename':
             tiles[key] = np.concatenate(output, axis=0)
     return tiles
 
 
 def bulk_unet_prediction(filelist, model, dst_dir, verbose=1, batch_size=8):
@@ -3044,20 +3242,515 @@
 
 
 def generate_wsi_mask(data, mask_key, show_image=False):
     """
     Only works for 10x images.
     """
     dim = openslide.open_slide(data['filename']).dimensions
-    mask = np.zeros(shape=(dim[1]//4, dim[0]//4), dtype=bool)
+    mask = np.zeros(shape=(dim[1] // 8, dim[0] // 8), dtype=bool)
     for i in range(len(data[mask_key])):
-        num_c = dim[0]//(4*512)
-        num_r = dim[1]//(4*512)
-        r_start = (i//num_c)*512
-        c_start = (i% num_c)*512
-        mask[r_start:(r_start+512), c_start:(c_start+512)][data[mask_key][i, 0, ...].astype(bool)] = True
+        num_c = dim[0] // (8 * 256)
+        num_r = dim[1] // (8 * 256)
+        r_start = (i // num_c) * 256
+        c_start = (i % num_c) * 256
+        mask[r_start:(r_start + 256), c_start:(c_start + 256)][data[mask_key][i, 0, ...].astype(bool)] = True
     if show_image:
         plt.figure(figsize=(30, 30))
         plt.show(mask)
         return mask
     else:
         return mask
+
+
+def get_labeled_papilla(data):
+    """
+
+    :return:
+    :rtype:
+    """
+    wsi_data = generate_wsi_mask(data, 'zones0')
+    refined_mask = ndimage.binary_closing(
+        ndimage.binary_opening(
+            ndimage.binary_fill_holes(
+                wsi_data
+            ),
+            iterations=3,
+        ),
+        iterations=3,
+    )
+    refined_mask = skimage.morphology.remove_small_objects(refined_mask, min_size=100, out=refined_mask)
+    distance = ndimage.distance_transform_edt(refined_mask).astype('float32')
+    local_max = skimage.feature.peak_local_max(distance, indices=False, min_distance=20, labels=refined_mask)
+    local_max, num_labels = ndimage.label(local_max)
+    labeled_papilla = skimage.segmentation.watershed(-distance, local_max, mask=refined_mask)
+    return labeled_papilla, num_labels
+
+
+def get_pap_data(pap_mask, feature_mask):
+    coords = np.array(ndimage.center_of_mass(pap_mask, labels=pap_mask, index=np.arange(1, pap_mask.max()+1)))[...,::-1]
+    slices = ndimage.find_objects(pap_mask)
+    pap_labels = []
+    pap_areas = []
+    for i in range(len(slices)):
+        if np.any(feature_mask[slices[i]][pap_mask[slices[i]] == (i + 1)] == True):
+            pap_labels.append(True)
+            pap_areas.append(np.sum(feature_mask[slices[i]][pap_mask[slices[i]] == (i + 1)] == True))
+        else:
+            pap_labels.append(False)
+            pap_areas.append(0)
+    pap_labels = np.array(pap_labels)
+    return coords, pap_labels, np.array(pap_areas)
+
+def fibrosis_heterogeneity(filename, masks_dict, save_dir=None):
+
+    """
+    Code to obtain center of mass coords for papilla
+    :return:
+    :rtype:
+    """
+    masks_dict['zones2'][masks_dict['zones3']==True] = True
+    masks_dict['zones1'][masks_dict['zones2']==True] = True
+    labeled_mask, num_labels = get_labeled_papilla(masks_dict)
+    dense = get_pap_data(labeled_mask, generate_wsi_mask(masks_dict, 'zones1'))
+    hyalinized = get_pap_data(labeled_mask, generate_wsi_mask(masks_dict, 'zones2'))
+    mineralized = get_pap_data(labeled_mask, generate_wsi_mask(masks_dict, 'zones3'))
+    processed_coords = {'coords': dense[0], 'p_a': np.array(
+        [np.sum(labeled_mask[j] == (i + 1)) for i, j in enumerate(ndimage.find_objects(labeled_mask))]),
+                        'd_a': dense[2], 'h_a': hyalinized[2], 'm_a': mineralized[2],
+                        'd_p': np.sum(masks_dict['zones1']) / np.sum(masks_dict['zones0']),
+                        'h_p': np.sum(masks_dict['zones2']) / np.sum(masks_dict['zones0']),
+                        'm_p': np.sum(masks_dict['zones3']) / np.sum(masks_dict['zones0']), 'd_lb': dense[1],
+                        'h_lb': hyalinized[1], 'm_lb': mineralized[1],
+                        'filename': str(os.path.basename(filename))}
+    return processed_coords, labeled_mask
+
+
+def papilla_specific_prevalence(papilla_masks, prevalence_data, show_fig=True, return_processed_fib_data=False,
+                                coord_scaling_factor=8):
+    """
+    Code to calculate prevalence of Biondi bodies or lipid vesicles around different categories of papilla (fibrotic vs
+    non-fibrotic papilla). For now, only works on to look at lipid vesicles and fibrosis.
+    :return:
+    :rtype:
+    """
+    fpout, papmask = fibrosis_heterogeneity(papilla_masks['filename'], papilla_masks)
+    # indices output show coordinates to nearest 0 value. Because papilla in papmask are labeled as 1 - N, papmask==0 is
+    # used to flip 1/0 (True/False)
+    distance, indices = ndimage.distance_transform_edt(papmask == 0, return_indices=True)
+    # TODO: double check factor by which to scale coordinates. For lipid vesicles, it should be 8 if coords are at 1:1
+    #  scale. Depending on which version of vesicle prevalence code use, scaling may be a factor of 4.
+    # create down-scaled CPEC coordinates
+    cpec_coords = prevalence_data['coords']/coord_scaling_factor
+    # get coordinates to nearest papilla mask for every CPEC coordinate.
+    cp_indices = indices[:, cpec_coords[..., 1].astype(int), cpec_coords[..., 0].astype(int)]
+    # get papilla labels using cp_indices on papmask
+    # TODO: Currently cp_labels points to nearest papilla for each CPEC. However, not all CPECs are located in papilla
+    #  and may be incorrect assign to a papilla that is quite far from it. Need to incorporate distance to filter out
+    #  these CPECs.
+    cp_labels = papmask[cp_indices[0], cp_indices[1]]
+    # get pathology prevalence around papilla by using list comprehension to calculate prevalence using only CPECs that
+    # have the same cp_label
+    pap_prev_percent = [np.mean(prevalence_data['predictions'][cp_labels == (i+1)]) for i in range(len(fpout['d_lb']))]
+    # TODO: Need to dynamically specify in dataframe if biondi bodies or lipid vesicles are being looked at.
+    df = pd.DataFrame()
+    df['papilla vesicle percentage'] = np.array(pap_prev_percent)[np.isnan(pap_prev_percent) == False]
+    df['fibrotic?'] = fpout['d_lb'][np.isnan(pap_prev_percent) == False]
+    df['p_a'] = fpout['p_a'][np.isnan(pap_prev_percent) == False]
+    df['d_a'] = fpout['d_a'][np.isnan(pap_prev_percent) == False]
+    df['h_a'] = fpout['h_a'][np.isnan(pap_prev_percent) == False]
+    df['m_a'] = fpout['m_a'][np.isnan(pap_prev_percent) == False]
+    if show_fig:
+        print(papilla_masks['filename'])
+        sns.violinplot(y="papilla vesicle percentage",
+                       x="fibrotic?",
+                       data=df,)
+        plt.show()
+    if return_processed_fib_data:
+        return df, fpout
+    else:
+        return df
+
+
+def biondi_prevalence_and_coords_from_hdf5(
+        hdf5,
+        coords_csv,
+        database,
+        retinanet,
+        classifier,
+        boundingbox,
+        bbox_size=64,
+        im_size=512,
+        half_res=True,
+        iou_nms=0.3,
+        return_predictions=True,
+):
+    if half_res:
+        tile_size = im_size // 2
+    else:
+        tile_size = im_size
+    h5 = h5py.File(hdf5)
+    h5_dict = get_retinanet_training_dictionary_from_hdf52(hdf5, coords_csv, database, boundingbox, bbox_size=bbox_size,
+                                                           tile_size=1024, downscale_factor=2, quartered=True,
+                                                           filter_coords=True,
+                                                           remove_blanks=False, )
+    # TODO: need to modify code to allow specifying channels
+    h5_dict['dat'] = biondi.dataset.per_sample_tile_normalization(h5_dict['dat'])
+    anc = boundingbox.convert_box_to_anc(
+        retinanet.predict(
+            h5_dict,
+            verbose=1,
+            workers=8,
+            max_queue_size=64
+        ),
+        iou_nms=iou_nms,
+        apply_deltas=True)
+    print(len(anc), len(h5_dict['dat']), len(anc[0]))
+    local_coords = []
+    for j in range(len(anc[0])):
+        if len(anc[0][j]) != 0:
+            y_coords = (anc[0][j][:, 2] + anc[0][j][:, 0]) / 2
+            x_coords = (anc[0][j][:, 3] + anc[0][j][:, 1]) / 2
+            local_coords.append(np.stack([x_coords, y_coords], axis=1))
+        else:
+            local_coords.append(anc[0][j] * 2)
+    # local_coords = np.array(local_coords)
+    ims = []
+    for i in range(len(local_coords)):
+        for j in local_coords[i]:
+            print(i, len(local_coords))
+            if np.any(j - 32 < 0) or np.any(j + 32 > 512):
+                continue
+            else:
+                ims.append(h5['images'][i][int(j[1] - 32):int(j[1] + 32), int(j[0] - 32):int(j[0] + 32)])
+    ims = np.array(ims)
+    ims = np.expand_dims(biondi.dataset.per_sample_tile_normalization(ims), axis=1)
+    logits = classifier.predict(ims, verbose=1, workers=8, max_queue_size=64)
+    predictions = biondi.statistics.convert_probabilities_to_predictions(logits)
+    prevalence = np.sum(predictions) / len(ims)
+    if return_predictions:
+        return {'coords': local_coords, 'prevalence': prevalence, 'predictions': predictions, }
+    else:
+        return {'coords': local_coords, 'prevalence': prevalence}
+
+
+def get_retinanet_training_dictionary_from_hdf52(hdf5_filename, coords_csv, database, boundingbox, bbox_size=64,
+                                                tile_size=1024, downscale_factor=2, quartered=True, filter_coords=True,
+                                                remove_blanks=False,):
+    """
+    **RIGHT NOW ONLY WORKS TO MAKE 256 FINAL HALF RES DATA**
+    Code to generate training data for retinanet based models. Currently can only generated 1024x1024 or 512x512 full res data or 512x512 or 256x256 half res data.
+
+    :param hdf5_filename: tile_array.hdf5 file used by the annotation client.
+    :type hdf5_filename: str
+    :param coords_csv: unadjusted-grids csv file generated by the annotation client.
+    :type coords_csv: str
+    :param database: database.db file used by the annotation client.
+    :type database: str
+    :param boundingbox: BoundingBox object generated using Jarvis package.
+    :type boundingbox: object
+    :param normalize: Whether or not to normalize the image.
+    :type normalize: bool
+    :param bbox_size: Size of the desired boundingbox square around each cell. Size should be at the resolution of the HDF5 image.
+    :type bbox_size: int
+    :param tile_size: Size of the image tiles in the HDF5 file.
+    :type tile_size: int
+    :param downscale_factor: Factor by which to downscale the image and coords. Usually 10x output resolution is desired so typical 20x HDF5 images are scaled down by a factor of 2.
+    :type downscale_factor: int
+    :param quartered: Whether or not to divide the processed images into quarters. This is usually done to get a final image size of 256 when the 10x resolution output images are 512.
+    :type quartered: bool
+    :param filter_coords: Whether to filter out coords where the resulting bbox would be outside the image range.
+    :type filter_coords: bool
+    :param remove_blanks: Whether to remove tiles that don't contain annotated cells
+    :type remove_blanks: bool
+    :return: dictionary containing images and box parameters
+    :rtype:dict
+    """
+    con = sqlite3.connect(database)
+    cur = con.cursor()
+    cur.execute("SELECT TILE_ID, FINISHED FROM tile;")
+    completed_tiles = np.array(cur.fetchall())
+    coords = pd.read_csv(coords_csv).to_numpy()[:, 2:]
+    image_file = h5py.File(hdf5_filename, 'r')
+    images = image_file['images'][:]
+    if downscale_factor != 1:
+        ds_model = biondi.dataset.downsampling_model(tile_size, downsample_factor=downscale_factor, channels=3)
+        images = ds_model.predict(images).astype('uint8')
+        coords = np.concatenate([coords[:,:1], (coords[:,1:]/downscale_factor).astype(int)], axis=1)
+    if quartered:
+        #if quartered function is broke change any reference to q_size to 256
+        q_size = tile_size // downscale_factor//2
+    im_out = []
+    bx_out = []
+    for i in range(len(completed_tiles)):
+        if completed_tiles[i,1] == 1:
+            # coords should be x, y where x is the column number and y is the row number
+            tile_coords = coords[coords[:,0]==i, 1:]
+            # TODO: add code to automatically calculate quarter split, currently assuming 512x512 before quartering
+            if remove_blanks:
+                if len(tile_coords) == 0:
+                    continue
+            if quartered:
+                # TODO: implement check for annotated cells in each image after quartering
+                q1_coords = tile_coords[(tile_coords[:,1]<q_size) & (tile_coords[:,0]<q_size)]
+                q2_coords = tile_coords[(tile_coords[:,1]<q_size) & (tile_coords[:,0]>=q_size)]
+                q3_coords = tile_coords[(tile_coords[:,1]>=q_size) & (tile_coords[:,0]<q_size)]
+                q4_coords = tile_coords[(tile_coords[:,1]>=q_size) & (tile_coords[:,0]>=q_size)]
+                # TODO: add code to automatically calculate output_tile_size, currently assuming 256
+                bx_out.append(anc_params(coords=q1_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=0, c_start=0, filter_coords=filter_coords))
+                bx_out.append(anc_params(coords=q2_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=0, c_start=q_size, filter_coords=filter_coords))
+                bx_out.append(anc_params(coords=q3_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=q_size, c_start=0, filter_coords=filter_coords))
+                bx_out.append(anc_params(coords=q4_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=q_size, c_start=q_size, filter_coords=filter_coords))
+                im_out.append(images[i, :q_size, :q_size])
+                im_out.append(images[i, :q_size, q_size:])
+                im_out.append(images[i, q_size:, :q_size])
+                im_out.append(images[i, q_size:, q_size:])
+            else:
+                bx_out.append(anc_params(coords=tile_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=512, r_start=0, c_start=0, filter_coords=filter_coords))
+                im_out.append(images[i])
+    bx_out = biondi.dataset.convert_anc_to_box_v2_2d(anc_params=bx_out, boundingbox=boundingbox)
+    im_out = np.stack(im_out, axis=0)
+    bx_out['dat'] = im_out
+    for key in bx_out.keys():
+        bx_out[key] = np.expand_dims(bx_out[key], axis=1)
+    image_file.close()
+    return bx_out
+
+
+def anc_params(coords, bbox_size, downscale_factor, ouput_tile_size, r_start, c_start, filter_coords=True):
+    x = int((bbox_size / downscale_factor) / 2)
+    y0 = (coords[:, 1] - r_start) - x
+    y1 = (coords[:, 1] - r_start) + x
+    x0 = (coords[:, 0] - c_start) - x
+    x1 = (coords[:, 0] - c_start) + x
+    params = np.stack([y0, x0, y1, x1], axis=1)
+    if filter_coords:
+        if len(params) != 0:
+            params = params[np.all((0 <= params) & (params < ouput_tile_size), axis=1)]
+    return params
+
+# TODO: should this be removed?
+def get_retinanet_training_dictionary_from_wsi_v2(wsi_filename, coords, boundingbox, normalize=False,
+                                               bbox_size=128, tile_size=1024, downscale_factor=1):
+    if type(wsi_filename) is str:
+        WSI = openslide.OpenSlide(wsi_filename)
+    else:
+        WSI = wsi_filename
+    image_file = h5py.File(hdf5_filename, 'r')
+    images = image_file['images'][:]
+    if downscale_factor != 1:
+        ds_model = biondi.dataset.downsampling_model(tile_size, downsample_factor=downscale_factor, channels=3)
+        images = ds_model.predict(images).astype('uint8')
+        coords = np.concatenate([coords[:, :1], (coords[:, 1:] / downscale_factor).astype(int)], axis=1)
+    im_out = []
+    bx_out = []
+    for i in range(len(completed_tiles)):
+        if completed_tiles[i, 1] == 1:
+            # coords should be x, y where x is the column number and y is the row number
+            tile_coords = coords[coords[:, 0] == i, 1:]
+            # TODO: add code to automatically calculate quarter split, currently assuming 512x512 before quartering
+            if remove_blanks:
+                if len(tile_coords) == 0:
+                    continue
+            if quartered:
+                # TODO: implement check for annotated cells in each image after quartering
+                q1_coords = tile_coords[(tile_coords[:, 1] < q_size) & (tile_coords[:, 0] < q_size)]
+                q2_coords = tile_coords[(tile_coords[:, 1] < q_size) & (tile_coords[:, 0] >= q_size)]
+                q3_coords = tile_coords[(tile_coords[:, 1] >= q_size) & (tile_coords[:, 0] < q_size)]
+                q4_coords = tile_coords[(tile_coords[:, 1] >= q_size) & (tile_coords[:, 0] >= q_size)]
+                # TODO: add code to automatically calculate output_tile_size, currently assuming 256
+                bx_out.append(anc_params(coords=q1_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=0, c_start=0, filter_coords=filter_coords))
+                bx_out.append(anc_params(coords=q2_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=0, c_start=q_size,
+                                         filter_coords=filter_coords))
+                bx_out.append(anc_params(coords=q3_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=q_size, c_start=0,
+                                         filter_coords=filter_coords))
+                bx_out.append(anc_params(coords=q4_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=q_size, r_start=q_size, c_start=q_size,
+                                         filter_coords=filter_coords))
+                im_out.append(images[i, :q_size, :q_size])
+                im_out.append(images[i, :q_size, q_size:])
+                im_out.append(images[i, q_size:, :q_size])
+                im_out.append(images[i, q_size:, q_size:])
+            else:
+                bx_out.append(anc_params(coords=tile_coords, bbox_size=bbox_size, downscale_factor=downscale_factor,
+                                         ouput_tile_size=512, r_start=0, c_start=0, filter_coords=filter_coords))
+                im_out.append(images[i])
+    bx_out = biondi.dataset.convert_anc_to_box_v2_2d(anc_params=bx_out, boundingbox=boundingbox)
+    im_out = np.stack(im_out, axis=0)
+    bx_out['dat'] = im_out
+    for key in bx_out.keys():
+        bx_out[key] = np.expand_dims(bx_out[key], axis=1)
+    image_file.close()
+    return bx_out
+
+
+def anc_params_from_wsi_v2(WSI, coords, bbox_size=128, tile_size=1024, downscale_factor=1, verbose=True):
+    anc_params = []
+    dim = WSI.dimensions
+    grid_height = dim[1] // tile_size
+    grid_width = dim[0] // tile_size
+    max_tiles = grid_width * grid_height
+    scaled_coords = (coords / downscale_factor).astype(int)
+    print('Extracting bounding boxes.')
+    for i in range(max_tiles):
+        tile_bbox_param = []
+        # get coords of image
+        column = i % grid_width
+        row = i // grid_width
+        # pixel range
+        c_start = int(tile_size / downscale_factor) * column
+        c_stop = c_start + int(tile_size / downscale_factor)
+        r_start = int(tile_size / downscale_factor) * row
+        r_stop = r_start + int(tile_size / downscale_factor)
+        # TODO: reconsider print output, message rate will likely be too fast
+        print(f'Extracting bounding boxes: {i + 1} out of {max_tiles}', end='      \r', flush=True)
+        tile_coords = scaled_coords[((c_start <= scaled_coords[:, 0]) & (scaled_coords[:, 0] < c_stop)) & (
+                (r_start <= scaled_coords[:, 1]) & (scaled_coords[:, 1] < r_stop))]
+        x = int((bbox_size / downscale_factor) / 2)
+        y0 = (tile_coords[:, 1] - r_start) - x
+        y1 = (tile_coords[:, 1] - r_start) + x
+        x0 = (tile_coords[:, 0] - c_start) - x
+        x1 = (tile_coords[:, 0] - c_start) + x
+        tile_coords = np.stack([y0, x0, y1, x1], axis=1)
+        if len(tile_coords) != 0:
+            tile_coords = tile_coords[np.all((0 <= tile_coords) & (tile_coords < tile_size), axis=1)]
+            if len(tile_coords) != 0:
+                anc_params.append(tile_coords)
+            else:
+                anc_params.append('None')
+        else:
+            anc_params.append('None')
+    return anc_params
+
+
+def cell_segmentation_hdf5_generation(wsi, coords, samplesize=200, imsize=128, upscale_size=1024, save_path=None):
+    """
+    Generates hdf5 files with images of cells for cell segmentation.
+    :param wsi: WSI filename
+    :type wsi: str
+    :param coords: coordinates of cells
+    :type coords: array
+    :param samplesize: # of images to include
+    :type samplesize: int
+    :param imsize: size of images to extract from the WSI
+    :type imsize: int
+    :param upscale_size: output size of upscaled images
+    :type upscale_size: int
+    :param save_path: save folder path
+    :type save_path: str
+    :return:
+    :rtype:
+    """
+    # get case number from WSI filename
+    wsi_name = re.search('(^.*?) ', os.path.basename(wsi)).group(1)
+    filename = wsi_name + '_cell_sample'
+    if save_path:
+        sp = save_path
+    else:
+        sp = ''
+    full_filename = sp + filename + '.hdf5'
+    # make indices for random sample
+    p = np.random.permutation(len(coords))
+    # randomly select coords
+    rand_coords = coords[p[:samplesize]]
+    # extract images
+    images = wsi_cell_extraction_from_coords_v3(wsi, im_size=imsize, coords=rand_coords, verbose=0)
+    # upscale images
+    images = np.stack([Image.fromarray(i).resize([upscale_size, upscale_size], resample=Image.NEAREST) for i in images])
+    f = h5py.File(full_filename, 'w')
+    f['images'] = images
+    f['coords'] = rand_coords
+    f['wsi_path'] = wsi
+    f.close()
+    print('Saved as:', full_filename)
+
+
+def cell_prediction_from_coords(wsi, classifier, coords, return_predictions=True,):
+    # currently only for BB predictions.
+    # TODO: Add support for lipid vesicle predictions
+    if type(wsi) is str:
+        wsi = openslide.open_slide(wsi)
+    else:
+        wsi = wsi
+    prediction_logits = classifier.predict(
+        PredictionGenerator(wsi, batch_size=32, downsample=False, retinanet=False, coords=coords),
+        verbose=1,
+        workers=12,
+        max_queue_size=128,
+    )
+    predictions = np.argmax(prediction_logits, axis=-1)
+    affected_coords = coords[predictions == 1]
+    prevalence = (len(affected_coords) / len(coords)) * 100
+    if return_predictions:
+        return {'coords': coords,
+                'af_coords': affected_coords,
+                'prevalence': prevalence,
+                'predictions': predictions, }
+    else:
+        return {'coords': coords,
+                'af_coords': affected_coords,
+                'prevalence': prevalence}
+
+
+class AffectedImgen(keras.utils.Sequence):
+    """
+    Extracts images of affected cpecs based on af_coords from biondi prevalence ai output.
+    """
+    def __init__(
+            self,
+            wsi_file_list,
+            data_list,
+            wsi_file_prefix,
+    ):
+        self.wfl = wsi_file_list
+        self.datas = data_list
+        self.fnprefix = wsi_file_prefix
+
+    def __len__(self):
+        return int(len(self.wfl))
+
+    def __getitem__(self, index):
+        return biondi.dataset.wsi_cell_extraction_from_coords_v3(self.fnprefix+self.wfl[index], im_size=44, coords=self.datas[index]['af_coords'], verbose=0)
+
+
+def biondi_load_from_coords(wsi_file_list, coord_data_list, file_name_prefix='', return_table=True):
+    sizes = []
+    gen = AffectedImgen(wsi_file_list, coord_data_list, file_name_prefix)
+    enqueuer = keras.utils.OrderedEnqueuer(gen)
+    enqueuer.start(workers=12, max_queue_size=gen.__len__())
+    datas = enqueuer.get()
+    progbar = keras.utils.Progbar(gen.__len__(), verbose=1)
+    for i in range(gen.__len__()):
+        data = next(datas)
+        histogram = skimage.exposure.histogram(data[...,1])
+        threshold = skimage.filters.threshold_multiotsu(hist=histogram, classes=4)
+        sizes.append(np.sum(data[...,1]>threshold[-1], axis=(1,2)))
+        progbar.add(1)
+    enqueuer.stop()
+    total = np.array([len(i['predictions']) for i in coord_data_list])
+    #poscount = np.array([np.sum(i['predictions']) for i in coord_data_list])
+    sumsizes = np.array([np.sum(i) for i in sizes])
+    avg_load_all_cells = sumsizes/total
+    #avg_load_pos_cells = sumsizes/poscount
+
+    if return_table:
+        df = pd.DataFrame()
+        df['case'] = wsi_file_list
+        df['BB_load_all_cells'] = avg_load_all_cells
+        return sizes, df
+    else:
+        return sizes,
+
+
+def biondi_local_load(affected_cpec_coords, biondi_load_data, radius=310.559):
+    ac = KDTree(affected_cpec_coords)
+    queried_coords = ac.query_radius(affected_cpec_coords, r=radius)
+    avg_load = np.array([np.mean(biondi_load_data[queried_coords[i]]) for i in range(len(queried_coords))])
+    return avg_load
+
```

### Comparing `biondi-0.1.5.0/biondi/misc/DCGAN.py` & `biondi-0.1.6.1/biondi/misc/DCGAN.py`

 * *Files identical despite different names*

### Comparing `biondi-0.1.5.0/biondi/misc/infogan practice.py` & `biondi-0.1.6.1/biondi/misc/infogan practice.py`

 * *Files identical despite different names*

### Comparing `biondi-0.1.5.0/biondi/misc/misc ai code.py` & `biondi-0.1.6.1/biondi/misc/misc ai code.py`

 * *Files identical despite different names*

### Comparing `biondi-0.1.5.0/biondi/misc/WSI autoencoder.py` & `biondi-0.1.6.1/biondi/misc/WSI autoencoder.py`

 * *Files identical despite different names*

### Comparing `biondi-0.1.5.0/biondi/models.py` & `biondi-0.1.6.1/biondi/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                                    filter_ratio=filter_ratio,
                                    shared_weights=shared_weights)
     model = Model(inputs=inputs, outputs=logits)
     return model
 
 
 def retinanet_resnet50_3d(inputs, K, A, filter_ratio=1, n=2, include_fc_layer=False, shared_weights=False, tahn=False,
-                          lr=2e-4, feature_maps=('c3', 'c4', 'c5')):
+                          lr=2e-4, feature_maps=('c3')):
     """Generates retinanet with resnet backbone. Can specify if classification and regression networks share weights"""
     r_model = resnet50_3d(inputs=inputs['dat'],
                           filter_ratio=filter_ratio,
                           n=n,
                           include_fc_layer=include_fc_layer,
                           kernal1=(1, 1, 1),
                           kernal3=(1, 3, 3),
@@ -50,15 +50,15 @@
     model = Model(inputs=inputs, outputs=preds)
     model.compile(
         optimizer=optimizers.Adam(learning_rate=lr),
         experimental_run_tf_function=False,
     )
     return model
 
-
+# TODO: add model compilation to function
 def resnet50_3d(inputs, filter_ratio=1, n=2, include_fc_layer=False, logits=True, kernal1=(1, 1, 1), kernal3=(1, 3, 3),
                 kernal7=(1, 7, 7), num_layers=None):
     """
 
     :param inputs: Keras Input object with desire shape
     :type inputs:
     :param filter_ratio:
@@ -827,16 +827,16 @@
     for j in reversed(range(num_layers - 1)):  # 4,3,2,1,0
         if j == num_layers - 2:
             expanding_layers.append(tran2(int(8 * filter_ratio) * j, contracting_layers[j + 1]))
         else:
             expanding_layers.append(e_layer(int(8 * filter_ratio) * j if j != 0 else int(4 * filter_ratio),
                                             int(8 * filter_ratio) * (j + 1),
                                             expanding_layers[-1] + contracting_layers[j + 1]))
-        last_layer = conv1(int(4 * filter_ratio),
-                           conv1(int(4 * filter_ratio), expanding_layers[-1] + contracting_layers[0]))
+    last_layer = conv1(int(4 * filter_ratio),
+                       conv1(int(4 * filter_ratio), expanding_layers[-1] + contracting_layers[0]))
 
     # --- Create logits
     logits = {}
     for k in range(class_num):
         logits[f'zones{k}'] = layers.Conv3D(filters=logits_num, name=f'zones{k}', **kwargs)(last_layer)
 
     # --- Create model
```

### Comparing `biondi-0.1.5.0/biondi/statistics.py` & `biondi-0.1.6.1/biondi/statistics.py`

 * *Files identical despite different names*

### Comparing `biondi-0.1.5.0/setup.py` & `biondi-0.1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='biondi',
-    version='0.1.5.0',
+    version='0.1.6.1',
     author='Michael Neel',
     author_email='neelm@uci.edu',
     description='Machine learning code and resources for analyzing choroid plexus pathology',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mjneel/Biondi',
     license='GNU GPLv3',
```

