# Comparing `tmp/fineslice-0.0.2.tar.gz` & `tmp/fineslice-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fineslice-0.0.2.tar", last modified: Thu Apr 27 18:19:19 2023, max compression
+gzip compressed data, was "fineslice-0.0.3.tar", max compression
```

## Comparing `fineslice-0.0.2.tar` & `fineslice-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,16 @@
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-27 18:19:19.126114 fineslice-0.0.2/
--rw-rw-r--   0 flo       (1000) flo       (1000)     1538 2022-12-08 10:10:43.000000 fineslice-0.0.2/LICENSE
--rw-rw-r--   0 flo       (1000) flo       (1000)     1142 2023-04-27 18:19:19.126114 fineslice-0.0.2/PKG-INFO
--rw-rw-r--   0 flo       (1000) flo       (1000)      716 2023-04-26 20:11:56.000000 fineslice-0.0.2/README.md
--rw-rw-r--   0 flo       (1000) flo       (1000)      169 2022-12-08 10:10:43.000000 fineslice-0.0.2/pyproject.toml
--rw-rw-r--   0 flo       (1000) flo       (1000)      588 2023-04-27 18:19:19.126114 fineslice-0.0.2/setup.cfg
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-27 18:19:19.122114 fineslice-0.0.2/src/
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-27 18:19:19.126114 fineslice-0.0.2/src/fineslice/
--rw-rw-r--   0 flo       (1000) flo       (1000)      448 2023-04-27 15:28:51.000000 fineslice-0.0.2/src/fineslice/__init__.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     2152 2023-04-25 17:58:59.000000 fineslice-0.0.2/src/fineslice/affine.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     1101 2023-04-26 13:54:19.000000 fineslice-0.0.2/src/fineslice/bounds.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     2255 2023-04-25 20:41:48.000000 fineslice-0.0.2/src/fineslice/cuboid.py
--rw-rw-r--   0 flo       (1000) flo       (1000)      942 2023-04-26 17:48:30.000000 fineslice-0.0.2/src/fineslice/debug_utils.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     2329 2023-04-26 14:29:27.000000 fineslice-0.0.2/src/fineslice/intersect.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     1058 2023-04-27 15:36:39.000000 fineslice-0.0.2/src/fineslice/sampler_0d.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     3653 2023-04-27 14:50:53.000000 fineslice-0.0.2/src/fineslice/sampler_1d.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     4038 2023-04-27 15:29:42.000000 fineslice-0.0.2/src/fineslice/sampler_2d.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     3447 2023-04-27 15:17:43.000000 fineslice-0.0.2/src/fineslice/sampler_3d.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     3302 2023-04-27 18:14:34.000000 fineslice-0.0.2/src/fineslice/types.py
--rw-rw-r--   0 flo       (1000) flo       (1000)      696 2023-04-27 15:36:49.000000 fineslice-0.0.2/src/fineslice/utils.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-27 18:19:19.126114 fineslice-0.0.2/src/fineslice.egg-info/
--rw-rw-r--   0 flo       (1000) flo       (1000)     1142 2023-04-27 18:19:19.000000 fineslice-0.0.2/src/fineslice.egg-info/PKG-INFO
--rw-rw-r--   0 flo       (1000) flo       (1000)      538 2023-04-27 18:19:19.000000 fineslice-0.0.2/src/fineslice.egg-info/SOURCES.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)        1 2023-04-27 18:19:19.000000 fineslice-0.0.2/src/fineslice.egg-info/dependency_links.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)        6 2023-04-27 18:19:19.000000 fineslice-0.0.2/src/fineslice.egg-info/requires.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)       10 2023-04-27 18:19:19.000000 fineslice-0.0.2/src/fineslice.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1538 2024-05-21 18:57:15.765757 fineslice-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1522 2024-05-21 18:57:15.765757 fineslice-0.0.3/README.md
+-rw-r--r--   0        0        0     1551 2024-05-21 18:57:15.765757 fineslice-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      891 2024-05-21 18:57:15.765757 fineslice-0.0.3/src/fineslice/__init__.py
+-rw-r--r--   0        0        0     2564 2024-05-21 18:57:15.765757 fineslice-0.0.3/src/fineslice/affine.py
+-rw-r--r--   0        0        0     1449 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/bounds.py
+-rw-r--r--   0        0        0     2659 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/cuboid.py
+-rw-r--r--   0        0        0     1139 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/debug_utils.py
+-rw-r--r--   0        0        0     2240 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/intersect.py
+-rw-r--r--   0        0        0     1135 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/sampler_0d.py
+-rw-r--r--   0        0        0     3961 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/sampler_1d.py
+-rw-r--r--   0        0        0     3908 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/sampler_2d.py
+-rw-r--r--   0        0        0     3561 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/sampler_3d.py
+-rw-r--r--   0        0        0     4285 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/types.py
+-rw-r--r--   0        0        0      764 2024-05-21 18:57:15.769757 fineslice-0.0.3/src/fineslice/utils.py
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 fineslice-0.0.3/PKG-INFO
```

### Comparing `fineslice-0.0.2/LICENSE` & `fineslice-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fineslice-0.0.2/src/fineslice/cuboid.py` & `fineslice-0.0.3/src/fineslice/cuboid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,116 @@
+"""Cuboid utility functions."""
+
 from typing import Iterable
 
 import numpy as np
 import numpy.typing as npt
 
 from .types import SamplerPoints
 
 
 def cuboid(shape: Iterable, dtype: npt.DTypeLike = None) -> np.ndarray:
-    """
-    Get vertices of a cuboid defined by shape
-    :param shape: Cuboid dimensions (x, y, z)
-    :param dtype: Output dtype
-    :return: vertices slicer points array
-    """
-    x, y, z = (i - 1 for i in shape)
-    return np.array([
-        [0, 0, 0, 1],  # 0
-        [x, 0, 0, 1],  # 1
-        [0, y, 0, 1],  # 2
-        [0, 0, z, 1],  # 3
-        [x, y, 0, 1],  # 4
-        [0, y, z, 1],  # 5
-        [x, 0, z, 1],  # 6
-        [x, y, z, 1]  # 7
-    ], dtype=dtype if dtype is not None else np.float64).T
+    """Get vertices of a cuboid defined by shape.
 
+    Args:
+        shape: Cuboid dimensions (x, y, z)
+        dtype: Output dtype
 
-def cuboid_from_bounds(bounds: SamplerPoints, dtype: npt.DTypeLike = None) -> np.ndarray:
+    Returns:
+        vertices slicer points array
     """
-    Get vertices of a cuboid defined by bounds.
+    x, y, z = (i - 1 for i in shape)
+    return np.array(
+        [
+            [0, 0, 0, 1],  # 0
+            [x, 0, 0, 1],  # 1
+            [0, y, 0, 1],  # 2
+            [0, 0, z, 1],  # 3
+            [x, y, 0, 1],  # 4
+            [0, y, z, 1],  # 5
+            [x, 0, z, 1],  # 6
+            [x, y, z, 1],  # 7
+        ],
+        dtype=dtype if dtype is not None else np.float64,
+    ).T
+
+
+def cuboid_from_bounds(
+    bounds: SamplerPoints, dtype: npt.DTypeLike = None
+) -> np.ndarray:
+    """Get vertices of a cuboid defined by bounds.
+
+    Args:
+        bounds: slicer bounds
+        dtype: Output dtype
 
-    :param bounds: slicer bounds
-    :param dtype: Output dtype
-    :return: vertices slicer points array
+    Returns:
+        vertices slicer points array
     """
     x0, y0, z0 = (i - 1 for i in bounds[0:3, 0])
     x1, y1, z1 = (i - 1 for i in bounds[0:3, 1])
-    return np.array([
-        [x0, y0, z0, 1],  # 0
-        [x1, y0, z0, 1],  # 1
-        [x0, y1, x0, 1],  # 2
-        [x0, y0, z1, 1],  # 3
-        [x1, y1, z0, 1],  # 4
-        [x0, y1, z1, 1],  # 5
-        [x1, y0, z1, 1],  # 6
-        [x1, y1, z1, 1]  # 7
-    ], dtype=dtype if dtype is not None else np.float64).T
-
-
-_CUBOID_EDGES = np.array([
-    [0, 1],
-    [0, 2],
-    [0, 3],
-    [1, 4],
-    [1, 6],
-    [2, 4],
-    [2, 5],
-    [3, 5],
-    [3, 6],
-    [4, 7],
-    [5, 7],
-    [6, 7],
-], dtype=int)
+    return np.array(
+        [
+            [x0, y0, z0, 1],  # 0
+            [x1, y0, z0, 1],  # 1
+            [x0, y1, x0, 1],  # 2
+            [x0, y0, z1, 1],  # 3
+            [x1, y1, z0, 1],  # 4
+            [x0, y1, z1, 1],  # 5
+            [x1, y0, z1, 1],  # 6
+            [x1, y1, z1, 1],  # 7
+        ],
+        dtype=dtype if dtype is not None else np.float64,
+    ).T
+
+
+_CUBOID_EDGES = np.array(
+    [
+        [0, 1],
+        [0, 2],
+        [0, 3],
+        [1, 4],
+        [1, 6],
+        [2, 4],
+        [2, 5],
+        [3, 5],
+        [3, 6],
+        [4, 7],
+        [5, 7],
+        [6, 7],
+    ],
+    dtype=int,
+)
 _CUBOID_EDGES.setflags(write=False)  # TODO attempt at making it immutable
 
 
-def cuboid_edges():
-    """
-    Get edges of cube defined by ``cuboid()``.
+def cuboid_edges() -> np.ndarray:
+    """Get edges of cube defined by ``cuboid()``.
 
-    :return: ``[[vertex_from, vertex_to]*]``
+    Returns:
+        ``[[vertex_from, vertex_to]*]``
     """
     return _CUBOID_EDGES
 
 
-def _make_cuboid_edges_axes():
+def _make_cuboid_edges_axes() -> np.ndarray:
+    """Get edges and their axes of cube defined by ``cuboid()``."""
     cube = cuboid((2, 2, 2), dtype=int)
-    return np.array([(v0, v1, np.nonzero(cube.T[v0] - cube.T[v1])[0][0]) for v0, v1 in cuboid_edges()])
+    return np.array(
+        [
+            (v0, v1, np.nonzero(cube.T[v0] - cube.T[v1])[0][0])
+            for v0, v1 in cuboid_edges()
+        ]
+    )
 
 
 _CUBOID_EDGES_AXES = _make_cuboid_edges_axes()
 _CUBOID_EDGES_AXES.setflags(write=False)
 
 
-def cuboid_edges_axes():
-    """
-    Get edges and their axes of cube defined by ``cuboid()``.
+def cuboid_edges_axes() -> np.ndarray:
+    """Get edges and their axes of cube defined by ``cuboid()``.
 
-    :return: ``[[vertex_from, vertex_to, edge_axis]*]``
+    Returns:
+        ``[[vertex_from, vertex_to, edge_axis]*]``
     """
     return _CUBOID_EDGES_AXES
```

### Comparing `fineslice-0.0.2/src/fineslice/intersect.py` & `fineslice-0.0.3/src/fineslice/intersect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+"""Find intersections between geometric objects."""
+
 from typing import Optional
 
 import numpy as np
 
 
 def intersect_line_plane(
-        line_origin: np.ndarray,
-        line_dir: np.ndarray,
-        plane_origin: np.ndarray,
-        plane_normal: np.ndarray,
-        epsilon=1e-6) -> Optional[np.ndarray]:
-    """
-    Find intersection point of a line with a plane.
+    line_origin: np.ndarray,
+    line_dir: np.ndarray,
+    plane_origin: np.ndarray,
+    plane_normal: np.ndarray,
+    epsilon: float = 1e-6,
+) -> Optional[np.ndarray]:
+    """Find intersection point of a line with a plane.
+
     Returns None if there is no intersection.
 
     TODO: Can this be sped up if either plane or line is axis aligned?
     """
     nu = plane_normal.dot(line_dir)
 
     if abs(nu) < epsilon:
@@ -24,32 +27,33 @@
     si = -plane_normal.dot(w) / nu
     psi = w + si * line_dir + plane_origin
 
     return psi
 
 
 def intersect_line_segment_plane(
-        point1: np.ndarray,
-        point2: np.ndarray,
-        plane_origin: np.ndarray,
-        plane_normal: np.ndarray,
-        epsilon=1e-6) -> Optional[np.ndarray]:
-    """
-    Find intersection point of a line segment (between 2 points) with a plane.
+    point1: np.ndarray,
+    point2: np.ndarray,
+    plane_origin: np.ndarray,
+    plane_normal: np.ndarray,
+    epsilon: float = 1e-6,
+) -> Optional[np.ndarray]:
+    """Find intersection point of a line segment (between 2 points) with a plane.
+
     Returns None if there is no intersection.
     """
     direction = point2 - point1
     orig = point1
 
     inter = intersect_line_plane(
         line_origin=orig,
         line_dir=direction,
         plane_origin=plane_origin,
         plane_normal=plane_normal,
-        epsilon=epsilon
+        epsilon=epsilon,
     )
 
     if inter is None:
         return None
 
     between_dist = np.linalg.norm(direction)
     point1_dist = np.linalg.norm(inter - point1)
@@ -58,37 +62,30 @@
     if (between_dist + epsilon) < (point1_dist + point2_dist):
         return None
 
     return inter
 
 
 def intersect_polygon_plane(
-        vertices: np.ndarray,
-        edges: np.ndarray,
-        plane_origin: np.ndarray,
-        plane_normal: np.ndarray
+    vertices: np.ndarray,
+    edges: np.ndarray,
+    plane_origin: np.ndarray,
+    plane_normal: np.ndarray,
 ) -> Optional[np.ndarray]:
-    """
-    Intersect polygon with plane. TODO
-
-    :param vertices:
-    :param edges:
-    :param plane_origin:
-    :param plane_normal:
-    :return:
-    """
+    """Intersect polygon with plane. TODO."""
     inters = []
     for e in edges:
         line = vertices[0:3, e]
 
         inter = intersect_line_segment_plane(
             point1=line[:, 0],
             point2=line[:, 1],
             plane_origin=plane_origin,
-            plane_normal=plane_normal)
+            plane_normal=plane_normal,
+        )
 
         if inter is not None:
             inters.append(inter)
 
     re = np.array(inters, dtype=np.float64).T
     if re.shape[0] == 0:
         return None
```

### Comparing `fineslice-0.0.2/src/fineslice/sampler_0d.py` & `fineslice-0.0.3/src/fineslice/sampler_0d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,41 @@
+"""0D sampler for 3D textures."""
+
 from typing import Any, Optional
 
 import numpy as np
 
-from .types import SamplerResult0D, as_affine, AffineLike, SamplerPointLike, sampler_point_3d, Texture3D, \
-    check_valid_texture_3d
+from .types import (
+    AffineLike,
+    SamplerPointLike,
+    SamplerResult0D,
+    Texture3D,
+    as_affine,
+    check_valid_texture_3d,
+    sampler_point_3d,
+)
 
 
 def sample_0d(
-        texture: Texture3D,
-        affine: AffineLike,
-        out_position: SamplerPointLike,
-        out_default: Any = None
+    texture: Texture3D,
+    affine: AffineLike,
+    out_position: SamplerPointLike,
+    out_default: Any = None,  # noqa: ANN401
 ) -> Optional[SamplerResult0D]:
-    """
-    Sample a single point from a texture.
+    """Sample a single point from a texture.
+
+    Args:
+        texture: Image texture.
+        affine: Affine matrix.
+        out_position: Point to sample. E.g. (1, 2, 3).
+        out_default: Default value that will be returned when sampling
+            outside of texture bounds.
 
-    :param texture: Image texture.
-    :param affine: Affine matrix.
-    :param out_position: Point to sample. E.g. (1, 2, 3).
-    :param out_default: Default value that will be returned when sampling outside of texture bounds.
-    :return: Sampled value (type equals texture array type).
+    Returns:
+        Sampled value (type equals texture array type).
     """
     check_valid_texture_3d(texture)
 
     affine = as_affine(affine)
     affine_inv = np.linalg.inv(affine)
     out_position = sampler_point_3d(out_position)
```

### Comparing `fineslice-0.0.2/src/fineslice/sampler_1d.py` & `fineslice-0.0.3/src/fineslice/sampler_1d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,108 +1,125 @@
-from typing import Any, Optional
+"""1D sampling of 3D textures."""
+
+from typing import List, Optional
 
 import numpy as np
 
 from .intersect import intersect_line_plane
-from .types import as_affine, AffineLike, Texture3D, check_valid_texture_3d, SamplerPointLike, sampler_point_3d, \
-    sampler_point_1d, as_sampler_points, SamplerResultND
+from .types import (
+    AffineLike,
+    SamplerPointLike,
+    SamplerResultND,
+    Texture3D,
+    as_affine,
+    as_sampler_points,
+    check_valid_texture_3d,
+    sampler_point_1d,
+    sampler_point_3d,
+)
 
 
 def sample_1d(
-        texture: Texture3D,
-        affine: AffineLike,
-        out_position: SamplerPointLike,
-        out_axis: int,
-        # out_bounds: Optional[Iterable] = None,
-        out_resolution_scale: float = 1,
-        out_resolution: Optional[int] = None
+    texture: Texture3D,
+    affine: AffineLike,
+    out_position: SamplerPointLike,
+    out_axis: int,
+    # out_bounds: Optional[Iterable] = None,
+    out_resolution_scale: float = 1,
+    out_resolution: Optional[int] = None,
 ) -> Optional[SamplerResultND]:
-    """
-
-    :param texture:
-    :param affine:
-    :param out_position:
-    :param out_axis:
-    :param out_resolution_scale:
-    :param out_resolution:
-    :return:
-    """
+    """Sample a 1D line from a 3D texture."""
     check_valid_texture_3d(texture)
 
     out_position = sampler_point_3d(out_position)
     out_normal = sampler_point_1d(1, axis=out_axis)
 
     affine = as_affine(affine)
     affine_inv = np.linalg.inv(affine)
 
-    vecs = np.vstack([
-        np.vstack((
-            np.zeros(3, dtype=int),  # Origin
-            texture.shape,  # Data limit
-            np.eye(3, dtype=int)  # Axis directions
-
-        )).T, np.ones(5)
-    ])
+    vecs = np.vstack(
+        [
+            np.vstack(
+                (
+                    np.zeros(3, dtype=int),  # Origin
+                    texture.shape,  # Data limit
+                    np.eye(3, dtype=int),  # Axis directions
+                )
+            ).T,
+            np.ones(5),
+        ]
+    )
 
     vecs_trans = np.dot(affine, vecs)
     vecs_trans_origin = vecs_trans[:, 0, np.newaxis]
     vecs_origin = vecs[:, 0, np.newaxis]
     vecs_datalim = vecs[:, 1, np.newaxis]
 
-    unit_vecs = vecs_trans[:, 2:] - vecs_trans_origin  # Absolute directions (from new origin)
+    unit_vecs = (
+        vecs_trans[:, 2:] - vecs_trans_origin
+    )  # Absolute directions (from new origin)
+
+    def _find_intersections() -> np.ndarray:
+        intersects: List[np.ndarray] = []
+        for plane_origin in vecs_trans[:, :2].T:
+            for plane_normal in unit_vecs.T:
+                p = intersect_line_plane(
+                    out_position[:3], out_normal[:3], plane_origin[:3], plane_normal[:3]
+                )
+                if p is not None:
+                    intersects.append(p)
+        return as_sampler_points(intersects)
 
-    intersects = []
-    for plane_origin in vecs_trans[:, :2].T:
-        for plane_normal in unit_vecs.T:
-            p = intersect_line_plane(out_position[:3], out_normal[:3], plane_origin[:3], plane_normal[:3])
-            if p is not None:
-                intersects.append(p)
-    intersects = as_sampler_points(intersects)
+    intersects = _find_intersections()
     intersects_trans = np.dot(affine_inv, intersects)
     intersects_in_bounds = np.all(
-        ((vecs_origin - 1e-6) < intersects_trans) &
-        (intersects_trans < (vecs_datalim + 1e-6)),
-        axis=0
+        ((vecs_origin - 1e-6) < intersects_trans)
+        & (intersects_trans < (vecs_datalim + 1e-6)),
+        axis=0,
     )
 
     intersects_cube = intersects[:, intersects_in_bounds]
     intersects_cube_trans = intersects_trans[:, intersects_in_bounds]
 
     if intersects_cube.shape[0] < 2:  # No intersection
         return None
 
     if intersects_cube.shape[0] > 2:
         # There might be more than 2 intersections
         # (when line directly cuts through edge/corner).
         # Select first and furthest from first:
         diff_idx = [
             0,
-            np.argmax(np.sum(intersects_cube[:, 1:] - intersects_cube[:, 0, np.newaxis], axis=0)) + 1
+            np.argmax(
+                np.sum(
+                    intersects_cube[:, 1:] - intersects_cube[:, 0, np.newaxis], axis=0
+                )
+            )
+            + 1,
         ]
-        intersects_cube = intersects_cube[:, diff_idx]
+        intersects_cube = intersects_cube[:, diff_idx]  # type: ignore
         intersects_cube_trans = intersects_cube_trans[:, diff_idx]
 
     if out_resolution is not None:
         res = out_resolution
     else:
-
         # Find resolution in data space
 
         line_origin = intersects_cube_trans[:, 0]
         line_target = intersects_cube_trans[:, 1]
         line_dir = line_target - line_origin
 
         mag = np.linalg.norm(line_dir)
         res = int(np.ceil(mag * out_resolution_scale)) + 1
 
     lmin = np.min(intersects_cube[out_axis])
     lmax = np.max(intersects_cube[out_axis])
 
     sample_grid = np.repeat(out_position[:, np.newaxis], repeats=res, axis=1)
-    sample_grid[out_axis] = np.mgrid[lmin:lmax:complex(res)]
+    sample_grid[out_axis] = np.mgrid[lmin : lmax : complex(res)]  # type: ignore
 
     # transform sampling grid (and round for nearest neighbour TODO)
     sample_grid_trans = np.dot(affine_inv, sample_grid).astype(int)
 
     # clip sampling grid TODO
     for i in range(3):
         sample_grid_trans[i] = sample_grid_trans[i].clip(0, texture.shape[i] - 1)
```

### Comparing `fineslice-0.0.2/src/fineslice/sampler_2d.py` & `fineslice-0.0.3/src/fineslice/sampler_2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from typing import Tuple, Optional
+"""0D sampler for 3D textures."""
+
+from typing import Optional, Tuple
 
 import numpy as np
 
 from .cuboid import cuboid, cuboid_edges
 from .intersect import intersect_polygon_plane
-from .types import SamplerResultND, Texture3D, AffineLike, as_affine, check_valid_texture_3d, SamplerPointLike, \
-    sampler_point_3d
+from .types import (
+    AffineLike,
+    SamplerPointLike,
+    SamplerResultND,
+    Texture3D,
+    as_affine,
+    check_valid_texture_3d,
+    sampler_point_3d,
+)
 from .utils import eye_1d
 
 
 def sample_2d(
-        texture: Texture3D,
-        affine: AffineLike,
-        out_position: SamplerPointLike,
-        out_axis: int,
-        out_bounds: Optional[np.ndarray] = None,
-        out_resolution_scale: float = 1,
-        out_resolution: Optional[Tuple[float, float]] = None
+    texture: Texture3D,
+    affine: AffineLike,
+    out_position: SamplerPointLike,
+    out_axis: int,
+    out_bounds: Optional[np.ndarray] = None,
+    out_resolution_scale: float = 1,
+    out_resolution: Optional[Tuple[float, float]] = None,
 ) -> Optional[SamplerResultND]:
-    """
-    Sample 2d.
-
-    :param texture:
-    :param affine:
-    :param out_axis:
-    :param out_position:
-    :param out_bounds:
-    :param out_resolution:
-    :return:
-    """
+    """Sample a 2D slice from a 3D texture."""
     check_valid_texture_3d(texture)
     out_position = sampler_point_3d(out_position)
 
     affine = as_affine(affine)
     affine_inv = np.linalg.inv(affine)
 
     corners = cuboid(texture.shape)
     edges = cuboid_edges()
     corners_trans = np.dot(affine, corners)
 
     out_axis_offset = out_position[out_axis]
 
     inters = intersect_polygon_plane(
-        corners_trans, edges,
+        corners_trans,
+        edges,
         plane_origin=out_position[:3],
-        plane_normal=eye_1d(3, out_axis, dtype=np.float64))
+        plane_normal=eye_1d(3, out_axis, dtype=np.float64),
+    )
 
     # data cube does not intersect plane
     if inters is None or inters.shape[1] < 3:
         return None
 
     # select variable dimensions
     var_dims = eye_1d(4, 3, False, True, dtype=bool)
@@ -71,18 +72,17 @@
 
         # todo dont need to do stuff above
         x_min, y_min = np.min(var_bounds, axis=1)
         x_max, y_max = np.max(var_bounds, axis=1)
 
     # sampling rectangle
     rect = np.full((4, 4), fill_value=1, dtype=np.float64)
-    rect[var_dims] = np.array([
-        [x_min, x_max, x_max, x_min],
-        [y_min, y_min, y_max, y_max]
-    ])
+    rect[var_dims] = np.array(
+        [[x_min, x_max, x_max, x_min], [y_min, y_min, y_max, y_max]]
+    )
     rect[out_axis] = out_axis_offset  # equals: inters[sample_axis, 0]
 
     # find minimum needed resolution (by measuring rectangle sides in data-space)
     if out_resolution is None:
         rect_trans = np.dot(affine_inv, rect)
         w1 = np.linalg.norm(rect_trans[:, 1] - rect_trans[:, 0])
         w2 = np.linalg.norm(rect_trans[:, 3] - rect_trans[:, 2])
@@ -90,22 +90,21 @@
         h2 = np.linalg.norm(rect_trans[:, 0] - rect_trans[:, 3])
 
         w = max(w1, w2)
         h = max(h1, h2)
         wn = int(np.ceil(w * out_resolution_scale)) + 1
         hn = int(np.ceil(h * out_resolution_scale)) + 1
     else:
-        hn, wn = out_resolution
+        hn, wn = map(int, out_resolution)
 
     # create sampling grid
     sample_grid = np.full((4, wn * hn), fill_value=1, dtype=np.float64)
     sample_grid[var_dims] = np.mgrid[
-                            x_min:x_max:complex(wn),
-                            y_min:y_max:complex(hn)
-                            ].reshape(2, -1)
+        x_min : x_max : complex(wn), y_min : y_max : complex(hn)  # type: ignore
+    ].reshape(2, -1)
     sample_grid[out_axis] = out_axis_offset  # equals: inters[axis, 0]
 
     # transform sampling grid (and round for nearest neighbour TODO)
     sample_grid_trans = np.dot(affine_inv, sample_grid).astype(int)
 
     # clip sampling grid TODO
     for i in range(3):
```

### Comparing `fineslice-0.0.2/src/fineslice/sampler_3d.py` & `fineslice-0.0.3/src/fineslice/sampler_3d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from typing import Optional, Tuple
+"""3D texture sampler."""
+
+from typing import Optional, Tuple, Union
 
 import numpy as np
 
 from .cuboid import cuboid, cuboid_edges_axes, cuboid_from_bounds
-from .types import Texture3D, check_valid_texture_3d, AffineLike, as_affine, SamplerPoints, SamplerResultND
+from .types import (
+    AffineLike,
+    SamplerPoints,
+    SamplerResultND,
+    Texture3D,
+    as_affine,
+    check_valid_texture_3d,
+)
 
 
-def _minmax_spoints(points: SamplerPoints):
+def _minmax_spoints(points: SamplerPoints) -> np.ndarray:
+    """Get minmax bounds of sampler points."""
     return np.column_stack((np.min(points, axis=1), np.max(points, axis=1)))
 
 
 def sample_3d(
-        texture: Texture3D,
-        affine: AffineLike,
-        out_bounds: Optional[np.ndarray] = None,
-        out_resolution_scale: float = 1,
-        out_resolution: Optional[Tuple[float, float, float]] = None) -> Optional[SamplerResultND]:
-    """
-
-    :param texture:
-    :param affine:
-    :param out_bounds:
-    :param out_resolution_scale:
-    :param out_resolution:
-    :return:
-    """
+    texture: Texture3D,
+    affine: AffineLike,
+    out_bounds: Optional[np.ndarray] = None,
+    out_resolution_scale: float = 1,
+    out_resolution: Optional[Tuple[float, float, float]] = None,
+) -> Optional[SamplerResultND]:
+    """Sample a 3D texture."""
     check_valid_texture_3d(texture)
 
     affine = as_affine(affine)
     affine_inv = np.linalg.inv(affine)
 
     corners_ds = cuboid(texture.shape)
     cube_edges_axes = cuboid_edges_axes()
@@ -40,14 +43,15 @@
         # Minmax bounds after transforming to RS
         sampling_cube_bounds_rs = _minmax_spoints(np.dot(affine, corners_ds))
 
     sampling_cube_rs = cuboid_from_bounds(sampling_cube_bounds_rs)
     sampling_cube_ds = np.dot(affine_inv, sampling_cube_rs).astype(int)  # todo
 
     # Sampling grid dimensions (data space)
+    axis_len: Union[np.ndarray, Tuple[float, float, float]]
     if out_resolution is None:
         axis_len = np.zeros((3,))
         for v0, v1, va in cube_edges_axes:
             edge_len = np.linalg.norm(sampling_cube_ds[:, v0] - sampling_cube_ds[:, v1])
             if edge_len > axis_len[va]:
                 axis_len[va] = edge_len
         axis_len = (axis_len * out_resolution_scale).astype(int)  # todo
@@ -57,36 +61,38 @@
     minmax_data = sampling_cube_bounds_rs
     minmax_data_n = axis_len
     minmax_data_n_total = np.prod(minmax_data_n)
     # print("minmax_data", minmax_data)
     # print("minmax_data_n", minmax_data_n)
     # print("minmax_data_n_total", minmax_data_n_total)
 
-    # print(f'x = from {minmax_data[0, 0]} to {minmax_data[0, 1]} in {minmax_data_n[0]} steps')
-    # print(f'y = from {minmax_data[1, 0]} to {minmax_data[1, 1]} in {minmax_data_n[1]} steps')
-    # print(f'z = from {minmax_data[2, 0]} to {minmax_data[2, 1]} in {minmax_data_n[2]} steps')
+    # print(f'x = from {minmax_data[0, 0]} to {minmax_data[0, 1]} in {minmax_data_n[0]} steps')  # noqa: E501
+    # print(f'y = from {minmax_data[1, 0]} to {minmax_data[1, 1]} in {minmax_data_n[1]} steps')  # noqa: E501
+    # print(f'z = from {minmax_data[2, 0]} to {minmax_data[2, 1]} in {minmax_data_n[2]} steps')  # noqa: E501
 
     # Make sampling grid
-    sample_grid = np.full((4, minmax_data_n_total), fill_value=1, dtype=np.float64)
+    sample_grid = np.full((4, minmax_data_n_total), fill_value=1, dtype=np.float64)  # type: ignore
     sample_grid[0:3] = np.mgrid[
-                       minmax_data[0, 0]:minmax_data[0, 1]:complex(minmax_data_n[0]),
-                       minmax_data[1, 0]:minmax_data[1, 1]:complex(minmax_data_n[1]),
-                       minmax_data[2, 0]:minmax_data[2, 1]:complex(minmax_data_n[2])
-                       ].reshape(3, -1)
+        minmax_data[0, 0] : minmax_data[0, 1] : complex(minmax_data_n[0]),  # type: ignore
+        minmax_data[1, 0] : minmax_data[1, 1] : complex(minmax_data_n[1]),  # type: ignore
+        minmax_data[2, 0] : minmax_data[2, 1] : complex(minmax_data_n[2]),  # type: ignore
+    ].reshape(3, -1)
 
     # print("sampling_grid", sample_grid.shape)
 
     # transform sampling grid (and round for nearest neighbour TODO)
     sample_grid_trans = np.dot(affine_inv, sample_grid).astype(int)
 
     # clip sampling grid TODO
     for i in range(3):
         sample_grid_trans[i] = sample_grid_trans[i].clip(0, texture.shape[i] - 1)
 
-    x = sample_grid_trans[0:3].reshape((3, minmax_data_n[0], minmax_data_n[1], minmax_data_n[2]))
+    x = sample_grid_trans[0:3].reshape(
+        (3, minmax_data_n[0], minmax_data_n[1], minmax_data_n[2])
+    )
 
     rastered = texture[x[0], x[1], x[2]]
 
     # Todo: convert rounded (for nearest neighbour) estimates
     #  back forth to get more accurate axis_lims
     axis_lims = sampling_cube_bounds_rs[0:3]
```

### Comparing `fineslice-0.0.2/src/fineslice/types.py` & `fineslice-0.0.3/src/fineslice/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,167 @@
-from typing import Tuple, Union, Iterable, Protocol, NamedTuple, Any
+"""Type definitions for fineslice module."""
+
+from typing import Any, Iterable, NamedTuple, Protocol, Tuple, Union
 
 import numpy as np
 
 # Affine matrix
 
 Affine = np.ndarray
+"""Affine matrix type."""
 AffineLike = Union[np.ndarray, Iterable]
+"""Objects convertible to Affine type."""
 
 
-def as_affine(affine_like: AffineLike, dtype=np.float64) -> Affine:
+def as_affine(
+    affine_like: AffineLike,
+    dtype=np.float64,  # noqa: ANN001
+) -> Affine:
+    """Converts AffineLike to Affine."""
     a = np.array(affine_like, dtype=dtype)
     if a.shape == (4, 4) and np.allclose(a[3, :], np.array([0, 0, 0, 1], dtype=dtype)):
         return a
-    raise Exception('Affine matrix does not have the correct format')
+    raise Exception("Affine matrix does not have the correct format")
 
 
 # Texture3D
 
-# pylint: too-few-public-methods
+
 class Texture3D(Protocol):
-    ndim: int
+    """3D texture type."""
+
+    @property
+    def ndim(self) -> int:
+        """Number of dimensions."""
+        ...
+
     shape: Tuple[int, ...]
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: Any) -> Any:  # noqa: ANN401
+        """Get item."""
         pass
 
 
 def check_valid_texture_3d(texture_3d_like: Texture3D) -> None:
+    """Check if texture has the correct format."""
     if not texture_3d_like.ndim == 3:
-        raise Exception('Texture does not have the correct format')
+        raise Exception("Texture does not have the correct format")
 
 
 # Sampler point
 
 SamplerPoint = np.ndarray
+"""Sampler point type."""
 SamplerPointLike = Union[np.ndarray, Iterable, int, float]
+"""Objects convertible to SamplerPoint type."""
 
 
-def sampler_point_0d(dtype=np.float64) -> SamplerPoint:
-    """
-    Creates origin sampler point (0,0,0).
+def sampler_point_0d(
+    dtype=np.float64,  # noqa: ANN001
+) -> SamplerPoint:
+    """Creates origin sampler point (0,0,0).
 
-    :param dtype:
-    :return:
+    Args:
+        dtype: Output dtype.
+
+    Returns:
+        Sampler point.
     """
     return np.array([0, 0, 0, 1], dtype=dtype)
 
 
-def sampler_point_1d(value: any, axis: int, dtype=np.float64) -> SamplerPoint:
-    """
-    Creates sampler point at (a, b, c) so that one axis is set to value and the other exes are 0.
+def sampler_point_1d(
+    value: Any,  # noqa: ANN401
+    axis: int,
+    dtype=np.float64,  # noqa: ANN001
+) -> SamplerPoint:
+    """Create sampler point on a 1D line.
+
+    Creates sampler point at (a, b, c) so that one axis
+    is set to value and the other exes are 0.
+
+    Args:
+        value: Position on the axis.
+        axis: Axis.
+        dtype: Output dtype.
 
-    :param value:
-    :param axis:
-    :param dtype: Output dtype.
-    :return:
+    Returns:
+        Sampler point
     """
     if axis > 2:
-        raise Exception('Axis must be < 3.')
+        raise Exception("Axis must be < 3.")
     arr = np.array([0, 0, 0, 1], dtype=dtype)
     arr[axis] = value
     return arr
 
 
-def sampler_point_2d(value: Union[np.ndarray, Iterable, int, float], zero_axis: int,
-                     dtype=np.float64) -> SamplerPoint:
-    """
-    Creates sampler point at (a, b, c) so that one axis is set to 0 and the other exes are broadcast from value.
+def sampler_point_2d(
+    value: Union[np.ndarray, Iterable, int, float],
+    zero_axis: int,
+    dtype=np.float64,  # noqa: ANN001
+) -> SamplerPoint:
+    """Creates sampler point on a 2D plane.
+
+    Creates sampler point at (a, b, c) so that one axis is
+    set to 0 and the other exes are broadcast from value.
+
+    Args:
+        value: Position on the plane.
+        zero_axis: Axis that will be set to 0.
+        dtype: Output dtype.
 
-    :param value:
-    :param zero_axis:
-    :param dtype: Output dtype.
-    :return:
+    Returns:
+        Sampler point.
     """
     if zero_axis > 2:
-        raise Exception('Axis must be < 3.')
+        raise Exception("Axis must be < 3.")
     values = np.asanyarray(value)
     arr = np.array([0, 0, 0, 1], dtype=dtype)
     var_axes = np.full((4,), True)
     var_axes[zero_axis] = False
     var_axes[3] = False
     arr[var_axes] = values
     return arr
 
 
-def sampler_point_3d(sampler_point_like: SamplerPointLike, dtype=np.float64) -> SamplerPoint:
-    """
-    Create sampler point from any array or scalar value.
+def sampler_point_3d(
+    sampler_point_like: SamplerPointLike,
+    dtype=np.float64,  # noqa: ANN001
+) -> SamplerPoint:
+    """Create sampler point from any array or scalar value.
+
+    Args:
+        sampler_point_like: Sampler point like.
+        dtype: Output dtype.
 
-    :param sampler_point_like:
-    :param dtype: Output dtype.
-    :return:
+    Returns:
+        Sampler point.
     """
-    values = np.ravel(sampler_point_like)
+    values: np.ndarray = np.ravel(sampler_point_like)  # type: ignore
     arr = np.array([0, 0, 0, 1], dtype=dtype)
     var_axes = np.full((4,), True)
     var_axes[3] = False
     arr[var_axes] = values[:3]
     return arr
 
 
 # Sampler points
 
 SamplerPoints = np.ndarray
+"""Collection of sampler points."""
 SamplerPointsLike = Union[np.ndarray, Iterable]
+"""Objects convertible to SamplerPoints type."""
 
 
 def as_sampler_points(sampler_points_like: SamplerPointsLike) -> SamplerPoints:
+    """Converts SamplerPointsLike to SamplerPoints."""
     ps = np.array(sampler_points_like, dtype=np.float64).T
     if ps.shape[0] != 3:
-        raise Exception('Sampler points does not have the correct format')
-    return np.vstack([
-        ps, np.ones(ps.shape[1])
-    ])
+        raise Exception("Sampler points does not have the correct format")
+    return np.vstack([ps, np.ones(ps.shape[1])])
 
 
 # Result
 
 SamplerResult0D = Any
 """Return sampled point values directly."""
```

### Comparing `fineslice-0.0.2/src/fineslice/utils.py` & `fineslice-0.0.3/src/fineslice/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from typing import Union, Optional
+"""Utility functions."""
+
+from typing import Any, Union
 
 import numpy as np
 
 
 def eye_1d(
-        n: int,
-        eye_index: int,
-        eye_value: Union[int, float, complex, np.ndarray] = 1,
-        fill_value: Union[int, float, complex, np.ndarray] = 0,
-        dtype: Optional[object] = None
-):
-    """
-    Similar to ``np.full`` but a single index is changed.
+    n: int,
+    eye_index: int,
+    eye_value: Union[int, float, complex, np.ndarray] = 1,
+    fill_value: Union[int, float, complex, np.ndarray] = 0,
+    dtype: Any = None,  # noqa: ANN401
+) -> np.ndarray:
+    """Similar to ``np.full`` but a single index is changed.
+
+    Args:
+        n: Vector length.
+        eye_index: Index.
+        eye_value: Index value.
+        fill_value: Fill value.
+        dtype: The desired data-type for the array The default, None,
+            means ``np.array(f).dtype``.
 
-    :param n: Vector length.
-    :param eye_index: Index.
-    :param eye_value: Index value.
-    :param fill_value: Fill value.
-    :param dtype: The desired data-type for the array The default, None, means ``np.array(f).dtype``.
-    :return:
+    Returns:
+        1D array with a single index changed.
     """
     a = np.full((n,), fill_value=fill_value, dtype=dtype)
     a[eye_index] = eye_value
     return a
```

