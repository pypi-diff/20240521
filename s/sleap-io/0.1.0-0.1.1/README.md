# Comparing `tmp/sleap_io-0.1.0.tar.gz` & `tmp/sleap_io-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleap_io-0.1.0.tar", last modified: Sun Apr 14 07:43:00 2024, max compression
+gzip compressed data, was "sleap_io-0.1.1.tar", last modified: Tue May 21 00:40:09 2024, max compression
```

## Comparing `sleap_io-0.1.0.tar` & `sleap_io-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:43:00.764012 sleap_io-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-14 07:42:21.000000 sleap_io-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-14 07:43:00.764012 sleap_io-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-14 07:42:21.000000 sleap_io-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-14 07:42:21.000000 sleap_io-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:43:00.764012 sleap_io-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:43:00.760012 sleap_io-0.1.0/sleap_io/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:43:00.760012 sleap_io-0.1.0/sleap_io/io/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19892 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/jabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/labelstudio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17560 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/nwb.py
--rw-r--r--   0 runner    (1001) docker     (127)    22923 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/slp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25869 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/io/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:43:00.764012 sleap_io-0.1.0/sleap_io/model/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/model/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/model/labeled_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    14125 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/model/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/model/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-14 07:42:21.000000 sleap_io-0.1.0/sleap_io/model/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:43:00.764012 sleap_io-0.1.0/sleap_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-14 07:43:00.000000 sleap_io-0.1.0/sleap_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 07:43:00.000000 sleap_io-0.1.0/sleap_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:43:00.000000 sleap_io-0.1.0/sleap_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-14 07:43:00.000000 sleap_io-0.1.0/sleap_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 07:43:00.000000 sleap_io-0.1.0/sleap_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-21 00:39:11.000000 sleap_io-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-21 00:40:09.551547 sleap_io-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-21 00:39:11.000000 sleap_io-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 00:39:11.000000 sleap_io-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:40:09.551547 sleap_io-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.547547 sleap_io-0.1.1/sleap_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/sleap_io/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19988 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/jabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/labelstudio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/slp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27804 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/sleap_io/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/labeled_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/sleap_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/top_level.txt
```

### Comparing `sleap_io-0.1.0/LICENSE` & `sleap_io-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.0/PKG-INFO` & `sleap_io-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleap-io
-Version: 0.1.0
+Version: 0.1.1
 Summary: Standalone utilities for working with pose data from SLEAP and other tools.
 Author-email: Liezl Maree <lmaree@salk.edu>, David Samy <davidasamy@gmail.com>, Talmo Pereira <talmo@salk.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://sleap.ai
 Project-URL: Repository, https://github.com/talmolab/sleap-io
 Keywords: sleap,pose tracking,pose estimation,behavior
 Classifier: Programming Language :: Python :: 3.7
@@ -30,14 +30,19 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pydocstyle; extra == "dev"
 Requires-Dist: toml; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
+Requires-Dist: mkdocs-material[imaging]; extra == "dev"
+Requires-Dist: mkdocs-jupyter; extra == "dev"
+Requires-Dist: mkdocstrings[python]>=0.18; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-literate-nav; extra == "dev"
 
 # sleap-io
 
 [![CI](https://github.com/talmolab/sleap-io/actions/workflows/ci.yml/badge.svg)](https://github.com/talmolab/sleap-io/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/talmolab/sleap-io/branch/main/graph/badge.svg?token=Sj8kIFl3pi)](https://codecov.io/gh/talmolab/sleap-io)
 [![Release](https://img.shields.io/github/v/release/talmolab/sleap-io?label=Latest)](https://github.com/talmolab/sleap-io/releases/)
 [![PyPI](https://img.shields.io/pypi/v/sleap-io?label=PyPI)](https://pypi.org/project/sleap-io)
```

### Comparing `sleap_io-0.1.0/README.md` & `sleap_io-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.0/pyproject.toml` & `sleap_io-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -32,26 +32,31 @@
     "imageio",
     "imageio-ffmpeg",
     "av"
 ]
 dynamic = ["version", "readme"]
 
 [tool.setuptools.dynamic]
-version = {attr = "sleap_io.__version__"}
+version = {attr = "sleap_io.version.__version__"}
 readme = {file = ["README.md"], content-type="text/markdown"}
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
     "black",
     "pydocstyle",
     "toml",
     "twine",
-    "build"
+    "build",
+    "mkdocs-material[imaging]",
+    "mkdocs-jupyter",
+    "mkdocstrings[python]>=0.18",
+    "mkdocs-gen-files",
+    "mkdocs-literate-nav"
 ]
 
 [project.urls]
 Homepage = "https://sleap.ai"
 Repository = "https://github.com/talmolab/sleap-io"
 
 [tool.black]
```

### Comparing `sleap_io-0.1.0/sleap_io/__init__.py` & `sleap_io-0.1.1/sleap_io/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """This module exposes all high level APIs for sleap-io."""
 
-# Define package version.
-# This is read dynamically by setuptools in pyproject.toml to determine the release version.
-__version__ = "0.1.0"
-
+from sleap_io.version import __version__
 from sleap_io.model.skeleton import Node, Edge, Skeleton, Symmetry
 from sleap_io.model.video import Video
 from sleap_io.model.instance import (
     Point,
     PredictedPoint,
     Track,
     Instance,
     PredictedInstance,
 )
+from sleap_io.model.suggestions import SuggestionFrame
 from sleap_io.model.labeled_frame import LabeledFrame
 from sleap_io.model.labels import Labels
 from sleap_io.io.main import (
     load_slp,
     save_slp,
     load_nwb,
     save_nwb,
```

### Comparing `sleap_io-0.1.0/sleap_io/io/jabs.py` & `sleap_io-0.1.1/sleap_io/io/jabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,18 @@
     confidence: np.ndarray[np.float32],
     skeleton: Skeleton,
     track: Track = None,
 ) -> Instance:
     """Create an `Instance` from prediction data.
 
     Args:
-        points: keypoint locations
+        data: keypoint locations
         confidence: confidence for keypoints
+        skeleton: `Skeleton` to use for `Instance`
+        track: `Track` to assign to `Instance`
 
     Returns:
         Parsed `Instance`.
     """
     assert (
         len(skeleton.nodes) == data.shape[0]
     ), f"Skeleton ({len(skeleton.nodes)}) does not match number of keypoints ({data.shape[0]})"
```

### Comparing `sleap_io-0.1.0/sleap_io/io/labelstudio.py` & `sleap_io-0.1.1/sleap_io/io/labelstudio.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     return LabeledFrame(video, frame_idx, instances)
 
 
 def filter_and_index(annotations: Iterable[dict], annot_type: str) -> Dict[str, dict]:
     """Filter annotations based on the type field and index them by ID.
 
     Args:
-        annotation: annotations to filter and index
+        annotations: annotations to filter and index
         annot_type: annotation type to filter e.x. 'keypointlabels' or 'rectanglelabels'
 
     Returns:
         Dict of ndexed and filtered annotations. Only annotations of type `annot_type`
         will survive, and annotations are indexed by ID.
     """
     filtered = list(filter(lambda d: d["type"] == annot_type, annotations))
```

### Comparing `sleap_io-0.1.0/sleap_io/io/main.py` & `sleap_io-0.1.1/sleap_io/io/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 def load_labelstudio(
     filename: str, skeleton: Optional[Union[Skeleton, list[str]]] = None
 ) -> Labels:
     """Read Label Studio-style annotations from a file and return a `Labels` object.
 
     Args:
-        labels_path: Path to the label-studio annotation file in JSON format.
+        filename: Path to the label-studio annotation file in JSON format.
         skeleton: An optional `Skeleton` object or list of node names. If not provided
             (the default), skeleton will be inferred from the data. It may be useful to
             provide this so the keypoint label types can be filtered to just the ones in
             the skeleton.
 
     Returns:
         Parsed labels as a `Labels` instance.
```

### Comparing `sleap_io-0.1.0/sleap_io/io/nwb.py` & `sleap_io-0.1.1/sleap_io/io/nwb.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     video: Video,
     pose_estimation_metadata: dict,
 ) -> PoseEstimation:
     """Create a PoseEstimation container for a track.
 
     Args:
         labels_data_df (pd.DataFrame): A pandas object with the data corresponding
-        to the predicted instances associated to this labels object.
+            to the predicted instances associated to this labels object.
         labels (Labels): A general labels object
         track_name (str): The name of the track in labels.tracks
         video (Video): The video to which data belongs to
 
     Returns:
         PoseEstimation: A PoseEstimation multicontainer where the time series
         of all the node trajectories in the track are stored. One time series per
@@ -396,15 +396,15 @@
 def build_track_pose_estimation_list(
     track_data_df: pd.DataFrame, timestamps: ArrayLike
 ) -> List[PoseEstimationSeries]:
     """Build a list of PoseEstimationSeries from tracks.
 
     Args:
         track_data_df (pd.DataFrame): A pandas DataFrame object containing the
-        trajectories for all the nodes associated with a specific track.
+            trajectories for all the nodes associated with a specific track.
 
     Returns:
         List[PoseEstimationSeries]: The list of all the PoseEstimationSeries.
         One for each node.
     """
     name_of_nodes_in_track = track_data_df.columns.get_level_values(
         "node_name"
```

### Comparing `sleap_io-0.1.0/sleap_io/io/slp.py` & `sleap_io-0.1.1/sleap_io/io/slp.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from sleap_io import (
     Video,
     Skeleton,
     Edge,
     Symmetry,
     Node,
     Track,
+    SuggestionFrame,
     Point,
     PredictedPoint,
     Instance,
     PredictedInstance,
     LabeledFrame,
     Labels,
 )
-from sleap_io.io.video import MediaVideo, HDF5Video
+from sleap_io.io.video import ImageVideo, MediaVideo, HDF5Video
 from sleap_io.io.utils import (
     read_hdf5_attrs,
     read_hdf5_dataset,
     write_hdf5_dataset,
     write_hdf5_group,
     write_hdf5_attrs,
 )
@@ -67,24 +68,31 @@
             if video_path_.exists():
                 video_path = video_path_
             else:
                 # TODO (TP): Expand capabilities of path resolution to support more
                 # complex path finding strategies.
                 pass
 
+        video_path = video_path.as_posix()
+
+        if "filenames" in backend:
+            # This is an ImageVideo.
+            # TODO: Path resolution.
+            video_path = backend["filenames"]
+
         try:
             backend = VideoBackend.from_filename(
-                video_path.as_posix(),
+                video_path,
                 dataset=backend.get("dataset", None),
                 grayscale=backend.get("grayscale", None),
                 input_format=backend.get("input_format", None),
             )
         except ValueError:
             backend = None
-        video_objects.append(Video(filename=video_path.as_posix(), backend=backend))
+        video_objects.append(Video(filename=video_path, backend=backend))
     return video_objects
 
 
 def write_videos(labels_path: str, videos: list[Video]):
     """Write video metadata to a SLEAP labels file.
 
     Args:
@@ -114,14 +122,32 @@
                     "input_format": video.backend.input_format,
                     "convert_range": False,
                 }
             }
             # TODO: Handle saving embedded images or restoring source video.
             # Ref: https://github.com/talmolab/sleap/blob/fb61b6ce7a9ac9613d99303111f3daafaffc299b/sleap/io/format/hdf5.py#L246-L273
 
+        elif type(video.backend) == ImageVideo:
+            shape = video.shape
+            if shape is None:
+                height, width, channels = 0, 0, 1
+            else:
+                height, width, channels = shape[1:]
+
+            video_json = {
+                "backend": {
+                    "filename": video.filename[0],
+                    "filenames": video.filename,
+                    "height_": height,
+                    "width_": width,
+                    "channels_": channels,
+                    "grayscale": video.backend.grayscale,
+                }
+            }
+
         else:
             raise NotImplementedError(
                 f"Cannot serialize video backend for video: {video}"
             )
         video_jsons.append(np.string_(json.dumps(video_json, separators=(",", ":"))))
 
     with h5py.File(labels_path, "a") as f:
@@ -157,14 +183,63 @@
         np.string_(json.dumps([SPAWNED_ON, track.name], separators=(",", ":")))
         for track in tracks
     ]
     with h5py.File(labels_path, "a") as f:
         f.create_dataset("tracks_json", data=tracks_json, maxshape=(None,))
 
 
+def read_suggestions(labels_path: str, videos: list[Video]) -> list[SuggestionFrame]:
+    """Read `SuggestionFrame` dataset in a SLEAP labels file.
+
+    Args:
+        labels_path: A string path to the SLEAP labels file.
+        videos: A list of `Video` objects.
+
+    Returns:
+        A list of `SuggestionFrame` objects.
+    """
+    suggestions = [
+        json.loads(x) for x in read_hdf5_dataset(labels_path, "suggestions_json")
+    ]
+    suggestions_objects = []
+    for suggestion in suggestions:
+        suggestions_objects.append(
+            SuggestionFrame(
+                video=videos[int(suggestion["video"])],
+                frame_idx=suggestion["frame_idx"],
+            )
+        )
+    return suggestions_objects
+
+
+def write_suggestions(
+    labels_path: str, suggestions: list[SuggestionFrame], videos: list[Video]
+):
+    """Write track metadata to a SLEAP labels file.
+
+    Args:
+        labels_path: A string path to the SLEAP labels file.
+        suggestions: A list of `SuggestionFrame` objects to store the metadata for.
+        videos: A list of `Video` objects.
+    """
+    GROUP = 0  # TODO: Handle storing extraneous metadata.
+    suggestions_json = []
+    for suggestion in suggestions:
+        suggestion_dict = {
+            "video": str(videos.index(suggestion.video)),
+            "frame_idx": suggestion.frame_idx,
+            "group": GROUP,
+        }
+        suggestion_json = np.string_(json.dumps(suggestion_dict, separators=(",", ":")))
+        suggestions_json.append(suggestion_json)
+
+    with h5py.File(labels_path, "a") as f:
+        f.create_dataset("suggestions_json", data=suggestions_json, maxshape=(None,))
+
+
 def read_metadata(labels_path: str) -> dict:
     """Read metadata from a SLEAP labels file.
 
     Args:
         labels_path: A string path to the SLEAP labels file.
 
     Returns:
@@ -645,14 +720,15 @@
     skeletons = read_skeletons(labels_path)
     points = read_points(labels_path)
     pred_points = read_pred_points(labels_path)
     format_id = read_hdf5_attrs(labels_path, "metadata", "format_id")
     instances = read_instances(
         labels_path, skeletons, tracks, points, pred_points, format_id
     )
+    suggestions = read_suggestions(labels_path, videos)
     metadata = read_metadata(labels_path)
     provenance = metadata.get("provenance", dict())
 
     frames = read_hdf5_dataset(labels_path, "frames")
     labeled_frames = []
     for _, video_id, frame_idx, instance_id_start, instance_id_end in frames:
         labeled_frames.append(
@@ -664,14 +740,15 @@
         )
 
     labels = Labels(
         labeled_frames=labeled_frames,
         videos=videos,
         skeletons=skeletons,
         tracks=tracks,
+        suggestions=suggestions,
         provenance=provenance,
     )
 
     return labels
 
 
 def write_labels(labels_path: str, labels: Labels):
@@ -681,9 +758,10 @@
         labels_path: A string path to the SLEAP labels file to save.
         labels: A `Labels` object to save.
     """
     if Path(labels_path).exists():
         Path(labels_path).unlink()
     write_videos(labels_path, labels.videos)
     write_tracks(labels_path, labels.tracks)
+    write_suggestions(labels_path, labels.suggestions, labels.videos)
     write_metadata(labels_path, labels)
     write_lfs(labels_path, labels)
```

### Comparing `sleap_io-0.1.0/sleap_io/io/utils.py` & `sleap_io-0.1.1/sleap_io/io/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                 )
 
     with h5py.File(filename, "a") as f:  # "a": read/write if exists, create otherwise
         write_group(f, data)
 
 
 def read_hdf5_attrs(
-    filename, dataset: str = "/", attribute: Optional[str] = None
+    filename: str, dataset: str = "/", attribute: Optional[str] = None
 ) -> Union[Any, dict[str, Any]]:
     """Read attributes from an HDF5 dataset.
 
     Args:
         filename: Path to an HDF5 file.
         dataset: Path to a dataset or group from which attributes will be read.
         attribute: If specified, the attribute name to read. If `None` (the default),
```

### Comparing `sleap_io-0.1.0/sleap_io/io/video.py` & `sleap_io-0.1.1/sleap_io/io/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Backends for reading and writing videos."""
 
 from __future__ import annotations
+from pathlib import Path
 
 import simplejson as json
 import sys
 from io import BytesIO
 from typing import Optional, Tuple
 
 import attrs
@@ -38,56 +39,68 @@
 class VideoBackend:
     """Base class for video backends.
 
     This class is not meant to be used directly. Instead, use the `from_filename`
     constructor to create a backend instance.
 
     Attributes:
-        filename: Path to video file.
+        filename: Path to video file(s).
         grayscale: Whether to force grayscale. If None, autodetect on first frame load.
         keep_open: Whether to keep the video reader open between calls to read frames.
             If False, will close the reader after each call. If True (the default), it
             will keep the reader open and cache it for subsequent calls which may
             enhance the performance of reading multiple frames.
     """
 
-    filename: str
+    filename: str | Path | list[str] | list[Path]
     grayscale: Optional[bool] = None
     keep_open: bool = True
     _cached_shape: Optional[Tuple[int, int, int, int]] = None
     _open_reader: Optional[object] = None
 
     @classmethod
     def from_filename(
         cls,
-        filename: str,
+        filename: str | list[str],
         dataset: Optional[str] = None,
         grayscale: Optional[bool] = None,
         keep_open: bool = True,
         **kwargs,
     ) -> VideoBackend:
         """Create a VideoBackend from a filename.
 
         Args:
-            filename: Path to video file.
+            filename: Path to video file(s).
             dataset: Name of dataset in HDF5 file.
             grayscale: Whether to force grayscale. If None, autodetect on first frame
                 load.
             keep_open: Whether to keep the video reader open between calls to read
                 frames. If False, will close the reader after each call. If True (the
                 default), it will keep the reader open and cache it for subsequent calls
                 which may enhance the performance of reading multiple frames.
 
         Returns:
             VideoBackend subclass instance.
         """
-        if type(filename) != str:
-            filename = str(filename)
+        if isinstance(filename, Path):
+            filename = filename.as_posix()
+
+        if type(filename) == str and Path(filename).is_dir():
+            filename = ImageVideo.find_images(filename)
 
-        if filename.endswith(MediaVideo.EXTS):
+        if type(filename) == list:
+            filename = [Path(f).as_posix() for f in filename]
+            return ImageVideo(
+                filename, grayscale=grayscale, **_get_valid_kwargs(ImageVideo, kwargs)
+            )
+        elif filename.endswith(ImageVideo.EXTS):
+            return ImageVideo(
+                [filename], grayscale=grayscale, **_get_valid_kwargs(ImageVideo, kwargs)
+            )
+        elif filename.endswith(MediaVideo.EXTS):
             return MediaVideo(
                 filename,
                 grayscale=grayscale,
                 keep_open=keep_open,
                 **_get_valid_kwargs(MediaVideo, kwargs),
             )
         elif filename.endswith(HDF5Video.EXTS):
@@ -102,16 +115,16 @@
             raise ValueError(f"Unknown video file type: {filename}")
 
     def _read_frame(self, frame_idx: int) -> np.ndarray:
         """Read a single frame from the video. Must be implemented in subclasses."""
         raise NotImplementedError
 
     def _read_frames(self, frame_inds: list) -> np.ndarray:
-        """Read a list of frames from the video. Must be implemented in subclasses."""
-        return np.stack([self._read_frame(i) for i in frame_inds], axis=0)
+        """Read a list of frames from the video."""
+        return np.stack([self.get_frame(i) for i in frame_inds], axis=0)
 
     def read_test_frame(self) -> np.ndarray:
         """Read a single frame from the video to test for grayscale.
 
         Note:
             This reads the frame at index 0. This may not be appropriate if the first
             frame is not available in a given backend.
@@ -142,15 +155,15 @@
     @property
     def num_frames(self) -> int:
         """Number of frames in the video. Must be implemented in subclasses."""
         raise NotImplementedError
 
     @property
     def img_shape(self) -> Tuple[int, int, int]:
-        """Shape of a single frame in the video. Must be implemented in subclasses."""
+        """Shape of a single frame in the video."""
         return self.get_frame(0).shape
 
     @property
     def shape(self) -> Tuple[int, int, int, int]:
         """Shape of the video as a tuple of `(frames, height, width, channels)`.
 
         On first call, this will defer to `num_frames` and `img_shape` to determine the
@@ -664,7 +677,52 @@
         if self.input_format == "channels_first":
             imgs = np.transpose(imgs, (0, 3, 2, 1))
 
         if not self.keep_open:
             f.close()
 
         return imgs
+
+
+@attrs.define
+class ImageVideo(VideoBackend):
+    """Video backend for reading videos stored as image files.
+
+    This backend supports reading videos stored as a list of images.
+
+    Attributes:
+        filename: Path to video files.
+        grayscale: Whether to force grayscale. If None, autodetect on first frame load.
+    """
+
+    EXTS = ("png", "jpg", "jpeg", "tif", "tiff", "bmp")
+
+    @staticmethod
+    def find_images(folder: str) -> list[str]:
+        """Find images in a folder and return a list of filenames."""
+        folder = Path(folder)
+        return sorted(
+            [f.as_posix() for f in folder.glob("*") if f.suffix[1:] in ImageVideo.EXTS]
+        )
+
+    @property
+    def num_frames(self) -> int:
+        """Number of frames in the video."""
+        return len(self.filename)
+
+    def _read_frame(self, frame_idx: int) -> np.ndarray:
+        """Read a single frame from the video.
+
+        Args:
+            frame_idx: Index of frame to read.
+
+        Returns:
+            The frame as a numpy array of shape `(height, width, channels)`.
+
+        Notes:
+            This does not apply grayscale conversion. It is recommended to use the
+            `get_frame` method of the `VideoBackend` class instead.
+        """
+        img = iio.imread(self.filename[frame_idx])
+        if img.ndim == 2:
+            img = np.expand_dims(img, axis=-1)
+        return img
```

### Comparing `sleap_io-0.1.0/sleap_io/model/instance.py` & `sleap_io-0.1.1/sleap_io/model/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,29 @@
     eq_rtol: ClassVar[float] = 0
 
     x: float
     y: float
     visible: bool = True
     complete: bool = False
 
-    def __eq__(self, other: object):
+    def __eq__(self, other: object) -> bool:
         """Compare `self` and `other` for equality.
 
         Precision error between the respective `x` and `y` properties of two
         instances may be allowed or controlled via the `Point.eq_atol` and
         `Point.eq_rtol` class variables. Set to zero to disable their effect.
         Internally, `numpy.isclose()` is used for the comparison:
         https://numpy.org/doc/stable/reference/generated/numpy.isclose.html
 
         Args:
             other: Instance of `Point` to compare to.
 
         Returns:
-            True if all attributes of `self` and `other` are the identical (possibly
-            allowing precision error for `x` and `y` attributes).
+            Returns True if all attributes of `self` and `other` are the identical
+                (possibly allowing precision error for `x` and `y` attributes).
         """
         # Check that other is a Point.
         if type(other) is not type(self):
             return False
 
         # We know that we have some kind of point at this point.
         other = cast(Point, other)
@@ -104,25 +104,25 @@
         """Return the coordinates and score as a numpy array of shape `(3,)`."""
         return (
             np.array([self.x, self.y, self.score])
             if self.visible
             else np.full((3,), np.nan)
         )
 
-    def __eq__(self, other: object):
+    def __eq__(self, other: object) -> bool:
         """Compare `self` and `other` for equality.
 
         See `Point.__eq__()` for important notes about point equality semantics!
 
         Args:
-            self, other: instance of `PredictedPoint` to compare
+            other: Instance of `PredictedPoint` to compare
 
         Returns:
-            True if all attributes of `self` and `other` are the identical (possibly
-            allowing precision error for `x` and `y` attributes).
+            Returns True if all attributes of `self` and `other` are the identical
+                (possibly allowing precision error for `x` and `y` attributes).
         """
         if not super().__eq__(other):
             return False
 
         # we know that we have a point at this point
         other = cast(PredictedPoint, other)
 
@@ -302,15 +302,15 @@
         return pts
 
 
 @define
 class PredictedInstance(Instance):
     """A `PredictedInstance` is an `Instance` that was predicted using a model.
 
-    Args:
+    Attributes:
         skeleton: The `Skeleton` that this `Instance` is associated with.
         points: A dictionary where keys are `Skeleton` nodes and values are `Point`s.
         track: An optional `Track` associated with a unique animal/object across frames
             or videos.
         from_predicted: Not applicable in `PredictedInstance`s (must be set to `None`).
         score: The instance detection or part grouping prediction score. This is a
             scalar that represents the confidence with which this entire instance was
```

### Comparing `sleap_io-0.1.0/sleap_io/model/labeled_frame.py` & `sleap_io-0.1.1/sleap_io/model/labeled_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 
 
 @define(auto_attribs=True)
 class LabeledFrame:
     """Labeled data for a single frame of a video.
 
-    Args:
+    Attributes:
         video: The :class:`Video` associated with this `LabeledFrame`.
         frame_idx: The index of the `LabeledFrame` in the `Video`.
         instances: List of `Instance` objects associated with this `LabeledFrame`.
     """
 
     video: Video
     frame_idx: int
```

### Comparing `sleap_io-0.1.0/sleap_io/model/labels.py` & `sleap_io-0.1.1/sleap_io/model/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 
 It is intended to be the entrypoint for deserialization and main container that should
 be used for serialization. It is designed to support both labeled data (used for
 training models) and predictions (inference results).
 """
 
 from __future__ import annotations
-from sleap_io import LabeledFrame, Instance, PredictedInstance, Video, Track
+from sleap_io import (
+    LabeledFrame,
+    Instance,
+    PredictedInstance,
+    Video,
+    Track,
+    SuggestionFrame,
+)
 from attrs import define, field
 from typing import Union, Optional, Any
 import numpy as np
 
 from sleap_io.model.skeleton import Skeleton
 
 
@@ -28,26 +35,28 @@
         labeled_frames: A list of `LabeledFrame`s that are associated with this dataset.
         videos: A list of `Video`s that are associated with this dataset. Videos do not
             need to have corresponding `LabeledFrame`s if they do not have any
             labels or predictions yet.
         skeletons: A list of `Skeleton`s that are associated with this dataset. This
             should generally only contain a single skeleton.
         tracks: A list of `Track`s that are associated with this dataset.
+        suggestions: A list of `SuggestionFrame`s that are associated with this dataset.
         provenance: Dictionary of arbitrary metadata providing additional information
             about where the dataset came from.
 
     Notes:
         `Video`s in contain `LabeledFrame`s, and `Skeleton`s and `Track`s in contained
         `Instance`s are added to the respective lists automatically.
     """
 
     labeled_frames: list[LabeledFrame] = field(factory=list)
     videos: list[Video] = field(factory=list)
     skeletons: list[Skeleton] = field(factory=list)
     tracks: list[Track] = field(factory=list)
+    suggestions: list[SuggestionFrame] = field(factory=list)
     provenance: dict[str, Any] = field(factory=dict)
 
     def __attrs_post_init__(self):
         """Append videos, skeletons, and tracks seen in `labeled_frames` to `Labels`."""
         for lf in self.labeled_frames:
             if lf.video not in self.videos:
                 self.videos.append(lf.video)
@@ -239,17 +248,17 @@
                 range. If not specific, then we'll return all labeled frames for video.
             return_new: Whether to return singleton of new and empty `LabeledFrame` if
                 none are found in project.
 
         Returns:
             List of `LabeledFrame` objects that match the criteria.
 
-            The list will be empty if no matches found, unless return_new is True,
-            in which case it contains new (empty) `LabeledFrame` objects with `video`
-            and `frame_index` set.
+            The list will be empty if no matches found, unless return_new is True, in
+            which case it contains new (empty) `LabeledFrame` objects with `video` and
+            `frame_index` set.
         """
         results = []
 
         if frame_idx is None:
             for lf in self.labeled_frames:
                 if lf.video == video:
                     results.append(lf)
```

### Comparing `sleap_io-0.1.0/sleap_io/model/skeleton.py` & `sleap_io-0.1.1/sleap_io/model/skeleton.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.0/sleap_io/model/video.py` & `sleap_io-0.1.1/sleap_io/model/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,40 +18,40 @@
 
     This class is used to store information regarding a video and its components.
     It is used to store the video's `filename`, `shape`, and the video's `backend`.
 
     To create a `Video` object, use the `from_filename` method which will select the
     backend appropriately.
 
-    Args:
-        filename: The filename of the video.
+    Attributes:
+        filename: The filename(s) of the video.
         backend: An object that implements the basic methods for reading and
             manipulating frames of a specific video type.
 
     See also: VideoBackend
     """
 
-    filename: str
+    filename: str | list[str]
     backend: Optional[VideoBackend] = None
 
     EXTS = MediaVideo.EXTS + HDF5Video.EXTS
 
     @classmethod
     def from_filename(
         cls,
-        filename: str,
+        filename: str | list[str],
         dataset: Optional[str] = None,
-        grayscale: Optional[str] = None,
+        grayscale: Optional[bool] = None,
         keep_open: bool = True,
         **kwargs,
     ) -> VideoBackend:
         """Create a Video from a filename.
 
         Args:
-            filename: Path to video file.
+            filename: Path to video file(s).
             dataset: Name of dataset in HDF5 file.
             grayscale: Whether to force grayscale. If None, autodetect on first frame
                 load.
             keep_open: Whether to keep the video reader open between calls to read
                 frames. If False, will close the reader after each call. If True (the
                 default), it will keep the reader open and cache it for subsequent calls
                 which may enhance the performance of reading multiple frames.
@@ -115,29 +115,42 @@
         """Informal string representation (for print or format)."""
         return self.__repr__()
 
     def __getitem__(self, inds: int | list[int] | slice) -> np.ndarray:
         """Return the frames of the video at the given indices.
 
         Args:
-            ind: Index or list of indices of frames to read.
+            inds: Index or list of indices of frames to read.
 
         Returns:
             Frame or frames as a numpy array of shape `(height, width, channels)` if a
             scalar index is provided, or `(frames, height, width, channels)` if a list
             of indices is provided.
 
         See also: VideoBackend.get_frame, VideoBackend.get_frames
         """
         if not self.is_open:
             self.open()
         return self.backend[inds]
 
-    def exists(self) -> bool:
-        """Check if the video file exists."""
+    def exists(self, check_all: bool = False) -> bool:
+        """Check if the video file exists.
+
+        Args:
+            check_all: If `True`, check that all filenames in a list exist. If `False`
+                (the default), check that the first filename exists.
+        """
+        if isinstance(self.filename, list):
+            if check_all:
+                for f in self.filename:
+                    if not Path(f).exists():
+                        return False
+                return True
+            else:
+                return Path(self.filename[0]).exists()
         return Path(self.filename).exists()
 
     @property
     def is_open(self) -> bool:
         """Check if the video backend is open."""
         return self.exists() and self.backend is not None
 
@@ -189,25 +202,32 @@
 
     def close(self):
         """Close the video backend."""
         if self.backend is not None:
             del self.backend
             self.backend = None
 
-    def replace_filename(self, new_filename: str | Path, open: bool = True):
+    def replace_filename(
+        self, new_filename: str | Path | list[str] | list[Path], open: bool = True
+    ):
         """Update the filename of the video, optionally opening the backend.
 
         Args:
             new_filename: New filename to set for the video.
             open: If `True` (the default), open the backend with the new filename. If
                 the new filename does not exist, no error is raised.
         """
         if isinstance(new_filename, Path):
             new_filename = str(new_filename)
 
+        if isinstance(new_filename, list):
+            new_filename = [
+                p.as_posix() if isinstance(p, Path) else p for p in new_filename
+            ]
+
         self.filename = new_filename
 
         if open:
             if self.exists():
                 self.open()
             else:
                 self.close()
```

### Comparing `sleap_io-0.1.0/sleap_io.egg-info/PKG-INFO` & `sleap_io-0.1.1/sleap_io.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleap-io
-Version: 0.1.0
+Version: 0.1.1
 Summary: Standalone utilities for working with pose data from SLEAP and other tools.
 Author-email: Liezl Maree <lmaree@salk.edu>, David Samy <davidasamy@gmail.com>, Talmo Pereira <talmo@salk.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://sleap.ai
 Project-URL: Repository, https://github.com/talmolab/sleap-io
 Keywords: sleap,pose tracking,pose estimation,behavior
 Classifier: Programming Language :: Python :: 3.7
@@ -30,14 +30,19 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pydocstyle; extra == "dev"
 Requires-Dist: toml; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
+Requires-Dist: mkdocs-material[imaging]; extra == "dev"
+Requires-Dist: mkdocs-jupyter; extra == "dev"
+Requires-Dist: mkdocstrings[python]>=0.18; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-literate-nav; extra == "dev"
 
 # sleap-io
 
 [![CI](https://github.com/talmolab/sleap-io/actions/workflows/ci.yml/badge.svg)](https://github.com/talmolab/sleap-io/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/talmolab/sleap-io/branch/main/graph/badge.svg?token=Sj8kIFl3pi)](https://codecov.io/gh/talmolab/sleap-io)
 [![Release](https://img.shields.io/github/v/release/talmolab/sleap-io?label=Latest)](https://github.com/talmolab/sleap-io/releases/)
 [![PyPI](https://img.shields.io/pypi/v/sleap-io?label=PyPI)](https://pypi.org/project/sleap-io)
```

### Comparing `sleap_io-0.1.0/sleap_io.egg-info/SOURCES.txt` & `sleap_io-0.1.1/sleap_io.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 sleap_io/__init__.py
+sleap_io/version.py
 sleap_io.egg-info/PKG-INFO
 sleap_io.egg-info/SOURCES.txt
 sleap_io.egg-info/dependency_links.txt
 sleap_io.egg-info/requires.txt
 sleap_io.egg-info/top_level.txt
 sleap_io/io/__init__.py
 sleap_io/io/jabs.py
@@ -16,8 +17,9 @@
 sleap_io/io/utils.py
 sleap_io/io/video.py
 sleap_io/model/__init__.py
 sleap_io/model/instance.py
 sleap_io/model/labeled_frame.py
 sleap_io/model/labels.py
 sleap_io/model/skeleton.py
+sleap_io/model/suggestions.py
 sleap_io/model/video.py
```

