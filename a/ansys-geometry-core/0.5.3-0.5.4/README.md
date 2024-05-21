# Comparing `tmp/ansys_geometry_core-0.5.3.tar.gz` & `tmp/ansys_geometry_core-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_geometry_core-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_geometry_core-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_geometry_core-0.5.3.tar` & `ansys_geometry_core-0.5.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     1098 2024-04-29 09:44:32.136813 ansys_geometry_core-0.5.3/LICENSE
--rw-r--r--   0        0        0     4966 2024-04-29 09:44:32.136813 ansys_geometry_core-0.5.3/README.rst
--rw-r--r--   0        0        0     4465 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2762 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/__init__.py
--rw-r--r--   0        0        0     2477 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/__init__.py
--rw-r--r--   0        0        0     1618 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/backend.py
--rw-r--r--   0        0        0    12306 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/client.py
--rw-r--r--   0        0        0    18876 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/conversions.py
--rw-r--r--   0        0        0     2483 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/defaults.py
--rw-r--r--   0        0        0    13911 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/docker_instance.py
--rw-r--r--   0        0        0    28217 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/launcher.py
--rw-r--r--   0        0        0      167 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/pim_configuration.json
--rw-r--r--   0        0        0    16343 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/product_instance.py
--rw-r--r--   0        0        0     1776 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/validate.py
--rw-r--r--   0        0        0     1782 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/__init__.py
--rw-r--r--   0        0        0     7898 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/beam.py
--rw-r--r--   0        0        0    46126 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/body.py
--rw-r--r--   0        0        0    52507 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/component.py
--rw-r--r--   0        0        0     6034 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/coordinate_system.py
--rw-r--r--   0        0        0    40126 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/design.py
--rw-r--r--   0        0        0     3697 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/designpoint.py
--rw-r--r--   0        0        0     7750 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/edge.py
--rw-r--r--   0        0        0    15145 2024-04-29 09:44:32.140813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/face.py
--rw-r--r--   0        0        0     5468 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/part.py
--rw-r--r--   0        0        0     4686 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/selection.py
--rw-r--r--   0        0        0     4101 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/errors.py
--rw-r--r--   0        0        0    22524 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/logger.py
--rw-r--r--   0        0        0     1349 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/materials/__init__.py
--rw-r--r--   0        0        0     3268 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/materials/material.py
--rw-r--r--   0        0        0     4107 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/materials/property.py
--rw-r--r--   0        0        0     1883 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/__init__.py
--rw-r--r--   0        0        0     6819 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/bbox.py
--rw-r--r--   0        0        0     3259 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/constants.py
--rw-r--r--   0        0        0     7035 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/frame.py
--rw-r--r--   0        0        0     4823 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/matrix.py
--rw-r--r--   0        0        0     4240 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/plane.py
--rw-r--r--   0        0        0    12120 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/point.py
--rw-r--r--   0        0        0    18024 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/vector.py
--rw-r--r--   0        0        0     2085 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/__init__.py
--rw-r--r--   0        0        0     8033 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/accuracy.py
--rw-r--r--   0        0        0     5215 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/auxiliary.py
--rw-r--r--   0        0        0    12751 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/checks.py
--rw-r--r--   0        0        0     8253 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/measurements.py
--rw-r--r--   0        0        0     2291 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/options.py
--rw-r--r--   0        0        0     3684 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/units.py
--rw-r--r--   0        0        0    17075 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/modeler.py
--rw-r--r--   0        0        0     1417 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/__init__.py
--rw-r--r--   0        0        0    22163 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/plotter.py
--rw-r--r--   0        0        0    15007 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/plotter_helper.py
--rw-r--r--   0        0        0     5826 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/plotting_types.py
--rw-r--r--   0        0        0     4213 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/trame_gui.py
--rw-r--r--   0        0        0     1710 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     3058 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/button.py
--rw-r--r--   0        0        0     4239 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3626 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/measure.py
--rw-r--r--   0        0        0     3700 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/ruler.py
--rw-r--r--   0        0        0     3480 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/show_design_point.py
--rw-r--r--   0        0        0     3348 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/view_button.py
--rw-r--r--   0        0        0     2305 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/widget.py
--rw-r--r--   0        0        0     2176 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/__init__.py
--rw-r--r--   0        0        0     5634 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/box_uv.py
--rw-r--r--   0        0        0     1580 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/__init__.py
--rw-r--r--   0        0        0    11617 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/circle.py
--rw-r--r--   0        0        0     3539 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/curve.py
--rw-r--r--   0        0        0     2767 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
--rw-r--r--   0        0        0    14319 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/ellipse.py
--rw-r--r--   0        0        0     8893 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/line.py
--rw-r--r--   0        0        0     7428 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
--rw-r--r--   0        0        0    13001 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/parameterization.py
--rw-r--r--   0        0        0     1746 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/__init__.py
--rw-r--r--   0        0        0    14274 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/cone.py
--rw-r--r--   0        0        0    14748 2024-04-29 09:44:32.144813 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/cylinder.py
--rw-r--r--   0        0        0     8067 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/plane.py
--rw-r--r--   0        0        0    13257 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/sphere.py
--rw-r--r--   0        0        0     3467 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/surface.py
--rw-r--r--   0        0        0     4281 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
--rw-r--r--   0        0        0    16027 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/torus.py
--rw-r--r--   0        0        0     5694 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
--rw-r--r--   0        0        0     1909 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/__init__.py
--rw-r--r--   0        0        0    11643 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/arc.py
--rw-r--r--   0        0        0     6690 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/box.py
--rw-r--r--   0        0        0     5139 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/circle.py
--rw-r--r--   0        0        0     2991 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/edge.py
--rw-r--r--   0        0        0     7734 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/ellipse.py
--rw-r--r--   0        0        0     3018 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/face.py
--rw-r--r--   0        0        0    19590 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/gears.py
--rw-r--r--   0        0        0     6063 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/polygon.py
--rw-r--r--   0        0        0     6076 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/segment.py
--rw-r--r--   0        0        0    31342 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/sketch.py
--rw-r--r--   0        0        0     6878 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/slot.py
--rw-r--r--   0        0        0     8286 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/trapezoid.py
--rw-r--r--   0        0        0     3847 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/triangle.py
--rw-r--r--   0        0        0     1550 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/__init__.py
--rw-r--r--   0        0        0     3856 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/measurement_tools.py
--rw-r--r--   0        0        0    14367 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/problem_areas.py
--rw-r--r--   0        0        0     2429 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/repair_tool_message.py
--rw-r--r--   0        0        0    10524 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/repair_tools.py
--rw-r--r--   0        0        0     1670 2024-04-29 09:44:32.148814 ansys_geometry_core-0.5.3/src/ansys/geometry/core/typing.py
--rw-r--r--   0        0        0     9183 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-15 14:00:35.516828 ansys_geometry_core-0.5.4/LICENSE
+-rw-r--r--   0        0        0     4966 2024-05-15 14:00:35.516828 ansys_geometry_core-0.5.4/README.rst
+-rw-r--r--   0        0        0     4464 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2762 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/__init__.py
+-rw-r--r--   0        0        0     2477 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/__init__.py
+-rw-r--r--   0        0        0     1618 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/backend.py
+-rw-r--r--   0        0        0    12306 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/client.py
+-rw-r--r--   0        0        0    18876 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/conversions.py
+-rw-r--r--   0        0        0     2483 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/defaults.py
+-rw-r--r--   0        0        0    13911 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/docker_instance.py
+-rw-r--r--   0        0        0    30050 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/launcher.py
+-rw-r--r--   0        0        0      167 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/pim_configuration.json
+-rw-r--r--   0        0        0    16343 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/product_instance.py
+-rw-r--r--   0        0        0     1776 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/validate.py
+-rw-r--r--   0        0        0     1782 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/__init__.py
+-rw-r--r--   0        0        0     7898 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/beam.py
+-rw-r--r--   0        0        0    46126 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/body.py
+-rw-r--r--   0        0        0    52507 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/component.py
+-rw-r--r--   0        0        0     6034 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/coordinate_system.py
+-rw-r--r--   0        0        0    40126 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/design.py
+-rw-r--r--   0        0        0     3697 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/designpoint.py
+-rw-r--r--   0        0        0     7750 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/edge.py
+-rw-r--r--   0        0        0    15145 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/face.py
+-rw-r--r--   0        0        0     5468 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/part.py
+-rw-r--r--   0        0        0     4686 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/selection.py
+-rw-r--r--   0        0        0     4101 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/errors.py
+-rw-r--r--   0        0        0    22524 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/logger.py
+-rw-r--r--   0        0        0     1349 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/materials/__init__.py
+-rw-r--r--   0        0        0     3268 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/materials/material.py
+-rw-r--r--   0        0        0     4107 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/materials/property.py
+-rw-r--r--   0        0        0     1883 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/__init__.py
+-rw-r--r--   0        0        0     6819 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/constants.py
+-rw-r--r--   0        0        0     7035 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/frame.py
+-rw-r--r--   0        0        0     4823 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/matrix.py
+-rw-r--r--   0        0        0     4240 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/plane.py
+-rw-r--r--   0        0        0    12120 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/point.py
+-rw-r--r--   0        0        0    18024 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/vector.py
+-rw-r--r--   0        0        0     2085 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/__init__.py
+-rw-r--r--   0        0        0     8033 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/accuracy.py
+-rw-r--r--   0        0        0     5215 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/auxiliary.py
+-rw-r--r--   0        0        0    12751 2024-05-15 14:00:35.524829 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/checks.py
+-rw-r--r--   0        0        0     8253 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/measurements.py
+-rw-r--r--   0        0        0     2291 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/options.py
+-rw-r--r--   0        0        0     3684 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/units.py
+-rw-r--r--   0        0        0    17075 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/modeler.py
+-rw-r--r--   0        0        0     1417 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/__init__.py
+-rw-r--r--   0        0        0    22163 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/plotter.py
+-rw-r--r--   0        0        0    15007 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/plotter_helper.py
+-rw-r--r--   0        0        0     5826 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/plotting_types.py
+-rw-r--r--   0        0        0     4213 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/trame_gui.py
+-rw-r--r--   0        0        0     1710 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     3058 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/button.py
+-rw-r--r--   0        0        0     4239 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3626 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/measure.py
+-rw-r--r--   0        0        0     3700 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/ruler.py
+-rw-r--r--   0        0        0     3480 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/show_design_point.py
+-rw-r--r--   0        0        0     3348 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/view_button.py
+-rw-r--r--   0        0        0     2305 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/widget.py
+-rw-r--r--   0        0        0     2176 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/__init__.py
+-rw-r--r--   0        0        0     5634 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/box_uv.py
+-rw-r--r--   0        0        0     1580 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/__init__.py
+-rw-r--r--   0        0        0    11617 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/circle.py
+-rw-r--r--   0        0        0     3539 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/curve.py
+-rw-r--r--   0        0        0     2767 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
+-rw-r--r--   0        0        0    14319 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/ellipse.py
+-rw-r--r--   0        0        0     8893 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/line.py
+-rw-r--r--   0        0        0     7428 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
+-rw-r--r--   0        0        0    13001 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/parameterization.py
+-rw-r--r--   0        0        0     1746 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/__init__.py
+-rw-r--r--   0        0        0    14274 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/cone.py
+-rw-r--r--   0        0        0    14748 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/cylinder.py
+-rw-r--r--   0        0        0     8067 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/plane.py
+-rw-r--r--   0        0        0    13257 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/sphere.py
+-rw-r--r--   0        0        0     3467 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/surface.py
+-rw-r--r--   0        0        0     4281 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
+-rw-r--r--   0        0        0    16027 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/torus.py
+-rw-r--r--   0        0        0     5694 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
+-rw-r--r--   0        0        0     1909 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/__init__.py
+-rw-r--r--   0        0        0    11643 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/arc.py
+-rw-r--r--   0        0        0     6690 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/box.py
+-rw-r--r--   0        0        0     5139 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/circle.py
+-rw-r--r--   0        0        0     2991 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/edge.py
+-rw-r--r--   0        0        0     7734 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/ellipse.py
+-rw-r--r--   0        0        0     3018 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/face.py
+-rw-r--r--   0        0        0    19590 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/gears.py
+-rw-r--r--   0        0        0     6063 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/polygon.py
+-rw-r--r--   0        0        0     6076 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/segment.py
+-rw-r--r--   0        0        0    31342 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/sketch.py
+-rw-r--r--   0        0        0     6878 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/slot.py
+-rw-r--r--   0        0        0     8286 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/trapezoid.py
+-rw-r--r--   0        0        0     3847 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/triangle.py
+-rw-r--r--   0        0        0     1550 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/__init__.py
+-rw-r--r--   0        0        0     3856 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/measurement_tools.py
+-rw-r--r--   0        0        0    14367 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/problem_areas.py
+-rw-r--r--   0        0        0     2429 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/repair_tool_message.py
+-rw-r--r--   0        0        0    10524 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/repair_tools.py
+-rw-r--r--   0        0        0     1670 2024-05-15 14:00:35.528828 ansys_geometry_core-0.5.4/src/ansys/geometry/core/typing.py
+-rw-r--r--   0        0        0     9183 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.4/PKG-INFO
```

### Comparing `ansys_geometry_core-0.5.3/LICENSE` & `ansys_geometry_core-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/README.rst` & `ansys_geometry_core-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/pyproject.toml` & `ansys_geometry_core-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-geometry-core"
-version = "0.5.3"
+version = "0.5.4"
 description = "A python wrapper for Ansys Geometry service"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -47,66 +47,66 @@
     "pyvista[jupyter]>=0.38.1,<1",
 ]
 tests = [
     "ansys-platform-instancemanagement==1.1.2",
     "ansys-tools-path==0.5.2",
     "beartype==0.18.5",
     "docker==7.0.0",
-    "grpcio==1.62.2",
+    "grpcio==1.63.0",
     "grpcio-health-checking==1.60.0",
     "numpy==1.26.4",
     "Pint==0.23",
     "protobuf==5.26.1",
-    "pytest==8.1.1",
+    "pytest==8.2.0",
     "pytest-cov==5.0.0",
     "pytest-pyvista==0.1.9",
     "pytest-xvfb==3.0.0",
-    "pyvista[jupyter]==0.43.5",
+    "pyvista[jupyter]==0.43.7",
     "requests==2.31.0",
     "scipy==1.13.0",
     "semver==3.0.2",
     "six==1.16.0",
     "vtk==9.3.0",
 ]
 tests-minimal = [
-    "pytest==8.1.1",
+    "pytest==8.2.0",
     "pytest-cov==5.0.0",
     "pytest-pyvista==0.1.9",
     "pytest-xvfb==3.0.0",
 ]
 doc = [
     "ansys-sphinx-theme[autoapi]==0.15.2",
     "beartype==0.18.5",
     "docker==7.0.0",
     "ipyvtklink==0.2.3",
     "jupyter_sphinx==0.5.3",
-    "jupytext==1.16.1",
-    "myst-parser==2.0.0",
-    "nbconvert==7.16.3",
-    "nbsphinx==0.9.3",
+    "jupytext==1.16.2",
+    "myst-parser==3.0.1",
+    "nbconvert==7.16.4",
+    "nbsphinx==0.9.4",
     "notebook==7.1.3",
     "numpydoc==1.7.0",
-    "panel==1.4.1",
-    "pyvista[jupyter]==0.43.5",
+    "panel==1.4.2",
+    "pyvista[jupyter]==0.43.7",
     "requests==2.31.0",
     "sphinx==7.2.6",
     "sphinx-autodoc-typehints==1.24.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-jinja==2.0.2",
-    "trame-vtk==2.8.6",
+    "trame-vtk==2.8.8",
     "vtk==9.3.0",
 ]
 
 [project.urls]
 Source = "https://github.com/ansys/pyansys-geometry"
 Issues = "https://github.com/ansys/pyansys-geometry/issues"
 Discussions = "https://github.com/ansys/pyansys-geometry/discussions"
 Documentation = "https://geometry.docs.pyansys.com"
 Releases = "https://github.com/ansys/pyansys-geometry/releases"
-Changelog =  "https://github.com/ansys/pyansys-geometry/blob/main/doc/source/changelog.rst"
+Changelog = "https://github.com/ansys/pyansys-geometry/blob/main/doc/source/changelog.rst"
 
 [tool.flit.module]
 name = "ansys.geometry.core"
 
 [tool.black]
 line-length = 100
```

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/backend.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/backend.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/client.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/client.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/conversions.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/conversions.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/defaults.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/docker_instance.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/docker_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/launcher.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,22 @@
         * ``"geometry_service"``: Launches the ``Modeler`` service locally using the
           Ansys Geometry Service.
         * ``"spaceclaim"``: Launches the ``Modeler`` service locally using Ansys SpaceClaim.
         * ``"discovery"``: Launches the ``Modeler`` service locally using Ansys Discovery.
 
     **kwargs : dict, default: None
         Keyword arguments for the launching methods. For allowable keyword arguments, see the
-        :func:`launch_remote_modeler` and :func:`launch_docker_modeler` methods. Some of these
-        keywords might be unused.
+        corresponding methods for each mode:
+
+        * For ``"pypim"`` mode, see the :func:`launch_remote_modeler` method.
+        * For ``"docker"`` mode, see the :func:`launch_docker_modeler` method.
+        * For ``"geometry_service"`` mode, see the
+          :func:`launch_modeler_with_geometry_service` method.
+        * For ``"spaceclaim"`` mode, see the :func:`launch_modeler_with_spaceclaim` method.
+        * For ``"discovery"`` mode, see the :func:`launch_modeler_with_discovery` method.
 
     Returns
     -------
     ansys.geometry.core.modeler.Modeler
         Pythonic interface for geometry modeling.
 
     Examples
@@ -228,17 +234,16 @@
     Parameters
     ----------
     version : str, default: None
         Version of the Geometry service to run in the three-digit format.
         For example, "232". If you do not specify the version, the server
         chooses the version.
     **kwargs : dict, default: None
-        Keyword arguments for the launching methods. For allowable keyword arguments, see the
-        :func:`launch_remote_modeler` and :func:`launch_docker_modeler` methods. Some of these
-        keywords might be unused.
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Returns
     -------
     ansys.geometry.core.modeler.Modeler
         Instance of the Geometry service.
     """
     return _launch_pim_instance(
@@ -282,17 +287,16 @@
         in which case Docker assigns it a random name.
     image : Optional[GeometryContainers], default: None
         The Geometry service Docker image to deploy. The default is ``None``,
         in which case the ``LocalDockerInstance`` class identifies the OS of your
         Docker engine and deploys the latest version of the Geometry service for
         that OS.
     **kwargs : dict, default: None
-        Keyword arguments for the launching methods. For allowable keyword arguments, see the
-        :func:`launch_remote_modeler` and :func:`launch_docker_modeler` methods. Some of these
-        keywords might be unused.
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Returns
     -------
     Modeler
         Instance of the Geometry service.
     """
     from ansys.geometry.core.modeler import Modeler
@@ -309,58 +313,68 @@
         image=image,
     )
 
     # Once the local Docker instance is ready... return the Modeler
     return Modeler(host="localhost", port=port, docker_instance=docker_instance)
 
 
-def launch_modeler_with_discovery_and_pimlight(version: Optional[str] = None) -> "Modeler":
+def launch_modeler_with_discovery_and_pimlight(
+    version: Optional[str] = None, **kwargs: Optional[Dict]
+) -> "Modeler":
     """
     Start Ansys Discovery remotely using the PIM API.
 
     When calling this method, you must ensure that you are in an
     environment where `PyPIM <https://github.com/ansys/pypim>`_ is configured.
     You can use the :func:`pypim.is_configured <ansys.platform.instancemanagement.is_configured>`
     method to check if it is configured.
 
     Parameters
     ----------
     version : str, default: None
         Version of Discovery to run in the three-digit format.
         For example, "232". If you do not specify the version, the server
         chooses the version.
+    **kwargs : dict, default: None
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Returns
     -------
     ansys.geometry.core.modeler.Modeler
         Instance of Modeler.
     """
     return _launch_pim_instance(
         is_pim_light=True,
         product_name="discovery",
         product_version=version,
         backend_type=BackendType.DISCOVERY,
     )
 
 
-def launch_modeler_with_geometry_service_and_pimlight(version: Optional[str] = None) -> "Modeler":
+def launch_modeler_with_geometry_service_and_pimlight(
+    version: Optional[str] = None, **kwargs: Optional[Dict]
+) -> "Modeler":
     """
     Start the Geometry service remotely using the PIM API.
 
     When calling this method, you must ensure that you are in an
     environment where `PyPIM <https://github.com/ansys/pypim>`_ is configured.
     You can use the :func:`pypim.is_configured <ansys.platform.instancemanagement.is_configured>`
     method to check if it is configured.
 
     Parameters
     ----------
     version : str, default: None
         Version of the Geometry service to run in the three-digit format.
         For example, "232". If you do not specify the version, the server
         chooses the version.
+    **kwargs : dict, default: None
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Returns
     -------
     ansys.geometry.core.modeler.Modeler
         Instance of Modeler.
     """
     return _launch_pim_instance(
@@ -397,31 +411,42 @@
         product_name="scdm",
         product_version=version,
         backend_type=BackendType.SPACECLAIM,
     )
 
 
 def launch_modeler_with_geometry_service(
+    product_version: int = None,
     host: str = "localhost",
     port: int = None,
     enable_trace: bool = False,
     log_level: int = 2,
     timeout: int = 60,
     logs_folder: str = None,
+    **kwargs: Optional[Dict],
 ) -> "Modeler":
     """
     Start the Geometry service locally using the ``ProductInstance`` class.
 
     When calling this method, a standalone Geometry service is started.
     By default, if an endpoint is specified (by defining `host` and `port` parameters)
     but the endpoint is not available, the startup will fail. Otherwise, it will try to
     launch its own service.
 
     Parameters
     ----------
+    product_version: int, optional
+        The product version to be started. Goes from v23.2.1 to
+        the latest. Default is ``None``.
+        If a specific product version is requested but not installed locally,
+        a SystemError will be raised.
+
+        **Ansys products versions and their corresponding int values:**
+
+        * ``241`` : Ansys 24R1
     host: str, optional
         IP address at which the Geometry service will be deployed. By default,
         its value will be ``localhost``.
     port : int, optional
         Port at which the Geometry service will be deployed. By default, its
         value will be ``None``.
     enable_trace : bool, optional
@@ -436,14 +461,17 @@
         * ``3``: Error
 
         The default is ``2`` (Warning).
     timeout : int, optional
         Timeout for starting the backend startup process. The default is 60.
     logs_folder : sets the backend's logs folder path. If nothing is defined,
         the backend will use its default path.
+    **kwargs : dict, default: None
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Raises
     ------
     ConnectionError
         If the specified endpoint is already in use, a connection
         error will be raised.
     SystemError
@@ -469,16 +497,24 @@
     >>> from ansys.geometry.core import launch_modeler_with_geometry_service
     >>> modeler = launch_modeler_with_geometry_service(host="10.171.22.44",
         port=5001,
         log_level=0,
         enable_trace= True,
         timeout=300)
     """
+    # if api_version is passed, throw a warning saying that it is not used
+    if "api_version" in kwargs:
+        logger.warning(
+            "The 'api_version' parameter is not used in 'launch_modeler_with_geometry_service'. "
+            "Please remove it from the arguments."
+        )
+
     return prepare_and_start_backend(
         BackendType.WINDOWS_SERVICE,
+        product_version=product_version,
         host=host,
         port=port,
         enable_trace=enable_trace,
         log_level=log_level,
         api_version=ApiVersions.LATEST,
         timeout=timeout,
         logs_folder=logs_folder,
@@ -491,14 +527,15 @@
     port: int = None,
     log_level: int = 2,
     api_version: ApiVersions = ApiVersions.LATEST,
     timeout: int = 150,
     manifest_path: str = None,
     logs_folder: str = None,
     hidden: bool = False,
+    **kwargs: Optional[Dict],
 ):
     """
     Start Ansys Discovery locally using the ``ProductInstance`` class.
 
     .. note::
 
        Support for Ansys Discovery is restricted to Ansys 24.1 onward.
@@ -542,14 +579,17 @@
     manifest_path : str, optional
         Used to specify a manifest file path for the ApiServerAddin. This way,
         it is possible to run an ApiServerAddin from a version an older product
         version.
     logs_folder : sets the backend's logs folder path. If nothing is defined,
         the backend will use its default path.
     hidden : starts the product hiding its UI. Default is ``False``.
+    **kwargs : dict, default: None
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Raises
     ------
     ConnectionError
         If the specified endpoint is already in use, a connection error will be raised.
     SystemError:
         If there is not an Ansys product 23.2 version or later installed
@@ -601,14 +641,15 @@
     port: int = None,
     log_level: int = 2,
     api_version: ApiVersions = ApiVersions.LATEST,
     timeout: int = 150,
     manifest_path: str = None,
     logs_folder: str = None,
     hidden: bool = False,
+    **kwargs: Optional[Dict],
 ):
     """
     Start Ansys SpaceClaim locally using the ``ProductInstance`` class.
 
     When calling this method, a standalone SpaceClaim session is started.
     By default, if an endpoint is specified (by defining `host` and `port` parameters)
     but the endpoint is not available, the startup will fail. Otherwise, it will try to
@@ -649,14 +690,17 @@
     manifest_path : str, optional
         Used to specify a manifest file path for the ApiServerAddin. This way,
         it is possible to run an ApiServerAddin from a version an older product
         version.
     logs_folder : sets the backend's logs folder path. If nothing is defined,
         the backend will use its default path.
     hidden : starts the product hiding its UI. Default is ``False``.
+    **kwargs : dict, default: None
+        Placeholder to prevent errors when passing additional arguments that
+        are not compatible with this method.
 
     Raises
     ------
     ConnectionError
         If the specified endpoint is already in use, a connection error will be raised.
     SystemError
         If there is not an Ansys product 23.2 version or later installed
```

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/product_instance.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/product_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/connection/validate.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/connection/validate.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/beam.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/beam.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/body.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/body.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/component.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/component.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/coordinate_system.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/design.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/design.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/designpoint.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/designpoint.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/edge.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/face.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/part.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/part.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/designer/selection.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/designer/selection.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/errors.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/logger.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/materials/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/materials/material.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/materials/material.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/materials/property.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/materials/property.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/bbox.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/bbox.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/constants.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/frame.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/frame.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/matrix.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/matrix.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/plane.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/point.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/math/vector.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/math/vector.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/accuracy.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/accuracy.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/auxiliary.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/auxiliary.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/checks.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/checks.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/measurements.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/measurements.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/options.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/options.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/misc/units.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/misc/units.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/modeler.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/modeler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/plotter.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/plotter_helper.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/plotter_helper.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/plotting_types.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/plotting_types.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/trame_gui.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/_images/isometric.png` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/button.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/displace_arrows.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/measure.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/measure.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/ruler.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/ruler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/show_design_point.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/show_design_point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/view_button.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/plotting/widgets/widget.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/plotting/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/box_uv.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/box_uv.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/circle.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/curve.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/curve_evaluation.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/curve_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/ellipse.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/line.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/line.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/curves/trimmed_curve.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/curves/trimmed_curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/parameterization.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/parameterization.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/cone.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/cone.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/cylinder.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/cylinder.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/plane.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/sphere.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/sphere.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/surface.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/torus.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/torus.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/arc.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/arc.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/box.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/box.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/circle.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/edge.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/ellipse.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/face.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/gears.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/gears.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/polygon.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/polygon.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/segment.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/segment.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/sketch.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/sketch.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/slot.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/slot.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/trapezoid.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/trapezoid.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/sketch/triangle.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/sketch/triangle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/__init__.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/measurement_tools.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/measurement_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/problem_areas.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/problem_areas.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/repair_tool_message.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/repair_tool_message.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/tools/repair_tools.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/tools/repair_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/src/ansys/geometry/core/typing.py` & `ansys_geometry_core-0.5.4/src/ansys/geometry/core/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.3/PKG-INFO` & `ansys_geometry_core-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-geometry-core
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python wrapper for Ansys Geometry service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -33,49 +33,49 @@
 Requires-Dist: docker>=6.0.1,<8 ; extra == "all"
 Requires-Dist: pyvista[jupyter]>=0.38.1,<1 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme[autoapi]==0.15.2 ; extra == "doc"
 Requires-Dist: beartype==0.18.5 ; extra == "doc"
 Requires-Dist: docker==7.0.0 ; extra == "doc"
 Requires-Dist: ipyvtklink==0.2.3 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
-Requires-Dist: jupytext==1.16.1 ; extra == "doc"
-Requires-Dist: myst-parser==2.0.0 ; extra == "doc"
-Requires-Dist: nbconvert==7.16.3 ; extra == "doc"
-Requires-Dist: nbsphinx==0.9.3 ; extra == "doc"
+Requires-Dist: jupytext==1.16.2 ; extra == "doc"
+Requires-Dist: myst-parser==3.0.1 ; extra == "doc"
+Requires-Dist: nbconvert==7.16.4 ; extra == "doc"
+Requires-Dist: nbsphinx==0.9.4 ; extra == "doc"
 Requires-Dist: notebook==7.1.3 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
-Requires-Dist: panel==1.4.1 ; extra == "doc"
-Requires-Dist: pyvista[jupyter]==0.43.5 ; extra == "doc"
+Requires-Dist: panel==1.4.2 ; extra == "doc"
+Requires-Dist: pyvista[jupyter]==0.43.7 ; extra == "doc"
 Requires-Dist: requests==2.31.0 ; extra == "doc"
 Requires-Dist: sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.24.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
-Requires-Dist: trame-vtk==2.8.6 ; extra == "doc"
+Requires-Dist: trame-vtk==2.8.8 ; extra == "doc"
 Requires-Dist: vtk==9.3.0 ; extra == "doc"
 Requires-Dist: ansys-platform-instancemanagement==1.1.2 ; extra == "tests"
 Requires-Dist: ansys-tools-path==0.5.2 ; extra == "tests"
 Requires-Dist: beartype==0.18.5 ; extra == "tests"
 Requires-Dist: docker==7.0.0 ; extra == "tests"
-Requires-Dist: grpcio==1.62.2 ; extra == "tests"
+Requires-Dist: grpcio==1.63.0 ; extra == "tests"
 Requires-Dist: grpcio-health-checking==1.60.0 ; extra == "tests"
 Requires-Dist: numpy==1.26.4 ; extra == "tests"
 Requires-Dist: Pint==0.23 ; extra == "tests"
 Requires-Dist: protobuf==5.26.1 ; extra == "tests"
-Requires-Dist: pytest==8.1.1 ; extra == "tests"
+Requires-Dist: pytest==8.2.0 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests"
-Requires-Dist: pyvista[jupyter]==0.43.5 ; extra == "tests"
+Requires-Dist: pyvista[jupyter]==0.43.7 ; extra == "tests"
 Requires-Dist: requests==2.31.0 ; extra == "tests"
 Requires-Dist: scipy==1.13.0 ; extra == "tests"
 Requires-Dist: semver==3.0.2 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
 Requires-Dist: vtk==9.3.0 ; extra == "tests"
-Requires-Dist: pytest==8.1.1 ; extra == "tests-minimal"
+Requires-Dist: pytest==8.2.0 ; extra == "tests-minimal"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests-minimal"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests-minimal"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests-minimal"
 Project-URL: Changelog, https://github.com/ansys/pyansys-geometry/blob/main/doc/source/changelog.rst
 Project-URL: Discussions, https://github.com/ansys/pyansys-geometry/discussions
 Project-URL: Documentation, https://geometry.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyansys-geometry/issues
```

