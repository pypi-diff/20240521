# Comparing `tmp/axoden-1.0.2.tar.gz` & `tmp/axoden-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axoden-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "axoden-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `axoden-1.0.2.tar` & `axoden-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1698 2024-05-13 19:22:12.517159 axoden-1.0.2/.github/workflows/build_executables.yml
--rw-r--r--   0        0        0      764 2024-05-13 19:22:12.517159 axoden-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      338 2024-05-13 19:22:12.517159 axoden-1.0.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      436 2024-05-13 19:22:12.517159 axoden-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1195 2024-05-13 19:22:12.517159 axoden-1.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      494 2024-05-13 19:22:12.517159 axoden-1.0.2/.gitignore
--rw-r--r--   0        0        0      154 2024-05-13 19:22:12.517159 axoden-1.0.2/.streamlit/config.toml
--rw-r--r--   0        0        0    32422 2024-05-13 19:22:12.517159 axoden-1.0.2/LICENSE
--rw-r--r--   0        0        0    10584 2024-05-13 19:22:12.517159 axoden-1.0.2/README.md
--rw-r--r--   0        0        0      599 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/__init__.py
--rw-r--r--   0        0        0      325 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/__init__.py
--rw-r--r--   0        0        0     9998 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/gui_projections_quantification.py
--rw-r--r--   0        0        0     5314 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/1_📊️_Axoden.py
--rw-r--r--   0        0        0        0 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/__init__.py
--rw-r--r--   0        0        0      526 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/__main__.py
--rw-r--r--   0        0        0     7857 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/app_utils.py
--rw-r--r--   0        0        0     8408 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
--rw-r--r--   0        0        0      570 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
--rw-r--r--   0        0        0     2433 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/gui/streamlit_app/pdf_utils.py
--rw-r--r--   0        0        0    29140 2024-05-13 19:22:12.517159 axoden-1.0.2/axoden/volume_projections.py
--rw-r--r--   0        0        0    85110 2024-05-13 19:22:12.517159 axoden-1.0.2/media/control_plots.jpg
--rw-r--r--   0        0        0    29852 2024-05-13 19:22:12.517159 axoden-1.0.2/media/summary_data.pdf
--rw-r--r--   0        0        0   327888 2024-05-13 19:22:12.521159 axoden-1.0.2/media/summary_data_axis.pdf
--rw-r--r--   0        0        0     1396 2024-05-13 19:22:12.521159 axoden-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-13 19:22:12.645160 axoden-1.0.2/tox.ini
--rw-r--r--   0        0        0    11407 1970-01-01 00:00:00.000000 axoden-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1698 2024-05-21 10:33:04.786280 axoden-1.1.0/.github/workflows/build_executables.yml
+-rw-r--r--   0        0        0      764 2024-05-21 10:33:04.786280 axoden-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      338 2024-05-21 10:33:04.786280 axoden-1.1.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      436 2024-05-21 10:33:04.786280 axoden-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1195 2024-05-21 10:33:04.786280 axoden-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      504 2024-05-21 10:33:04.786280 axoden-1.1.0/.gitignore
+-rw-r--r--   0        0        0      154 2024-05-21 10:33:04.786280 axoden-1.1.0/.streamlit/config.toml
+-rw-r--r--   0        0        0    32422 2024-05-21 10:33:04.786280 axoden-1.1.0/LICENSE
+-rw-r--r--   0        0        0    10811 2024-05-21 10:33:04.786280 axoden-1.1.0/README.md
+-rw-r--r--   0        0        0      599 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/__init__.py
+-rw-r--r--   0        0        0     9998 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/gui_projections_quantification.py
+-rw-r--r--   0        0        0     5908 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/1_📊️_Axoden.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/__init__.py
+-rw-r--r--   0        0        0      526 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/__main__.py
+-rw-r--r--   0        0        0     6703 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/app_utils.py
+-rw-r--r--   0        0        0     8500 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
+-rw-r--r--   0        0        0      570 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
+-rw-r--r--   0        0        0     2470 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/gui/streamlit_app/pdf_utils.py
+-rw-r--r--   0        0        0    29148 2024-05-21 10:33:04.786280 axoden-1.1.0/axoden/volume_projections.py
+-rw-r--r--   0        0        0    85110 2024-05-21 10:33:04.786280 axoden-1.1.0/media/control_plots.jpg
+-rw-r--r--   0        0        0   121987 2024-05-21 10:33:04.790280 axoden-1.1.0/media/preprocessing.jpg
+-rw-r--r--   0        0        0    29852 2024-05-21 10:33:04.790280 axoden-1.1.0/media/summary_data.pdf
+-rw-r--r--   0        0        0   327888 2024-05-21 10:33:04.790280 axoden-1.1.0/media/summary_data_axis.pdf
+-rw-r--r--   0        0        0   198888 2024-05-21 10:33:04.790280 axoden-1.1.0/media/workflow.jpg
+-rw-r--r--   0        0        0     1396 2024-05-21 10:33:04.790280 axoden-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-21 10:33:04.914280 axoden-1.1.0/tox.ini
+-rw-r--r--   0        0        0    11634 1970-01-01 00:00:00.000000 axoden-1.1.0/PKG-INFO
```

### Comparing `axoden-1.0.2/.github/workflows/build_executables.yml` & `axoden-1.1.0/.github/workflows/build_executables.yml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/.github/workflows/docs.yml` & `axoden-1.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/.github/workflows/test.yml` & `axoden-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/LICENSE` & `axoden-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/README.md` & `axoden-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [![Test](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml)
 [![Lint](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml)
 [![PyPI](https://img.shields.io/pypi/v/axoden?label=pypi%20package)](https://pypi.org/project/axoden)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/axoden)
+[![Documentation](https://img.shields.io/badge/Documentation-8A2BE2)](https://raqueladaia.github.io/AxoDen/)
 
 # Axoden
 
+<img src="https://github.com/raqueladaia/AxoDen/blob/main/media/workflow.jpg?raw=true)">
+
+
 ## Table of Contents
 
 - [How to use AxoDen](#how-to-use-axoden)
   - [Streamlit App](#streamlit-app)
   - [Standalone GUI](#standalone-gui)
 - [Installation](#installation)
   - [With pip](#pip-install)
   - [Git clone](#clone-from-github)
-- [Contributing](#contributing)
+- [Using AxoDen in your code](#using-axoden-in-your-code)
 
 ## Overview of AxoDen
 
 AxoDen is an open source platform that facilitates and streamlines the quantification of fluorescently labeled axonal projections of a given brain area.
 
 AxoDen accepts .tif images, transforms them into gray scale and uses the Otsu method to set a threshold that distinguishes signal from background. Because it collects the pixel values of any color channel which sum is above zero, users can use any fluorophore and obtain the same quantification accuracy. In addition, given that the input are images of projections, AxoDen can be applied to virtually any animal species.
 
@@ -181,15 +185,15 @@
 This should automatically open a browser window to the app.
 If not, streamlit will post the URL where you can reach the web app,
 usually at http://localhost:8501.
 
 
 This is the same interface as the [Streamlit Web App](https://axoden.streamlit.app).
 
-# Using axoden in your code
+## Using axoden in your code
 Below you find a few examples of how to use axoden.
 You can see the full [documentation here](https://raqueladaia.github.io/AxoDen/).
 
 You can process a single image. This will not save any results or plots.
 ```python
 import axoden
```

### Comparing `axoden-1.0.2/axoden/__init__.py` & `axoden-1.1.0/axoden/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 axoden simplifies the quantification of axonal projections in neuroscience.
 """
 
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 
 from .volume_projections import (  # noqa: F401
     load_table,
     plot_signal_intensity_along_axis,
     plot_summary_data,
     process_folder,
     process_image,
```

### Comparing `axoden-1.0.2/axoden/gui/gui_projections_quantification.py` & `axoden-1.1.0/axoden/gui/gui_projections_quantification.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/axoden/gui/streamlit_app/1_📊️_Axoden.py` & `axoden-1.1.0/axoden/gui/streamlit_app/1_📊️_Axoden.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import logging
 import os
 import sys
 
+import matplotlib.pyplot as plt
 import streamlit as st
 from streamlit_pdf_viewer import pdf_viewer
 
 if os.getcwd() not in sys.path:
     sys.path.append(os.getcwd())
 
+from axoden import __version__ as axoden_version
 from axoden.gui.streamlit_app.app_utils import (
     cached_plot_signal_intensity_along_axis,
     cached_plot_summary_data,
     get_brain_regions,
     get_figure_by_brain_region,
-    init_session_state,
-    invalidate_figure_cache,
     process_images,
 )
-from axoden.gui.streamlit_app.pdf_utils import join_pdfs, pdf2stream
+from axoden.gui.streamlit_app.pdf_utils import join_pdfs
 
-MAX_IMAGES = 200  # TODO: decide on file upload limit
+MAX_IMAGES = 100
+MAX_IMAGE_MB = 200
 DEFAULT_PIXEL_SIZE = 0.75521
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.WARNING)
 
 
 def axo_den_app():
     """Main Streamlit application for AxoDen."""
-    init_session_state()
-
     st.title("AxoDen")
+    st.text(f"Version {axoden_version}")
 
     with st.container(border=True):
         st.write(
             "If you're new to AxoDen, see the tutorial and learn how to use AxoDen:"
         )
         st.page_link(
             "pages/2_❔️_Tutorial_&_How_To.py",
@@ -47,115 +47,133 @@
 
     st.header("Input")
     project_name = st.text_input(label="Project Name", value="AxoDen Analysis")
     pixel_size = st.number_input(
         "Pixel Size (μm):",
         value=DEFAULT_PIXEL_SIZE,
         format="%f",
-        on_change=invalidate_figure_cache,
         key="pixel_size",
     )  # Set the pixel size
     st.text(
         "Note:\nThe default pixel size is for the 20x Objective of the Keyence BZ-810X "
         "series.\n"
         "Please change it according to the objective used.\n\n4x Objective: 3.77396\n"
         "20x Objective: 0.75521\n"
     )
 
     raw_files = st.file_uploader(
-        "Upload image here. You can add more or remove them later.",
+        "Upload image here. You can add more or remove them later. "
+        f"You can upload up to {MAX_IMAGES} images "
+        f"with a total size of {MAX_IMAGE_MB} MB.",
         type=["tif"],
         accept_multiple_files=True,
     )
     if len(raw_files) > MAX_IMAGES:
         st.warning(
             f"This application is limited to using {MAX_IMAGES} images concurrently. "
-            "You uploaded {len(raw_files)}, remaining images will not be used in the "
-            "analysis!"
+            f"You uploaded {len(raw_files)}, remove some to start the analysis. "
+            "If you have more images, either run the analysis in batches "
+            "(e.g. per group or brain area), or use the standalone version of AxoDen, "
+            "which you can find. at https://github.com/raqueladaia/AxoDen/releases"
         )
-        raw_files = raw_files[:MAX_IMAGES]
+        st.stop()
 
     is_masked = st.checkbox(
         "Images are masked (desired brain region are cropped out, "
         "backround fluorescence has values above 0, "
         "areas of the image lacking tissue have value 0)",
         value=True,
-        on_change=invalidate_figure_cache,
         key="is_masked",
     )
 
+    import numpy as np
+
+    total_memory = np.sum([f.size for f in raw_files]) / 1024**2
+    if total_memory > MAX_IMAGE_MB:
+        st.warning(
+            f"We currently limit the uploaded images to {MAX_IMAGE_MB} MB "
+            f"and {MAX_IMAGES} images.\n"
+            f"The memory from your uploaded files is {total_memory} MB!\n"
+            "Please reduce the number of images or the size of the images to continue. "
+            "You can run the analysis in batches (e.g. per group or brain area), "
+            "or use the standalone version of Axoden, "
+            "which you can find. at https://github.com/raqueladaia/AxoDen/releases"
+        )
+        st.stop()
+
     (
-        st.session_state.figures,
-        st.session_state.table_data,
-        st.session_state.table_data_axis,
-    ) = process_images(
-        raw_files, pixel_size, is_masked, cache=st.session_state.figure_cache
-    )
+        ctrl_figures,
+        table_data,
+        table_data_axis,
+    ) = process_images(raw_files, pixel_size, is_masked)
 
     # plot table data results
-    if st.session_state.table_data is not None:
+    if table_data is not None:
         logger.info("Creating data section")
         st.header("Summary Data")
 
         fig, fig_stream = cached_plot_summary_data(
-            st.session_state.table_data, project_name
+            table_data,
+            project_name,
         )
 
         st.pyplot(fig)
+        plt.close(fig)
         st.download_button(
             "Download figure as pdf", fig_stream, "axoden_summary_data.pdf"
         )
-        st.dataframe(st.session_state.table_data)
+        st.dataframe(table_data)
 
     # plot table data by axis results
-    if st.session_state.table_data_axis is not None:
+    if table_data_axis is not None:
         logger.info("Creating data axis section")
         st.header("Summary Data Axis")
 
         fig, fig_stream = cached_plot_signal_intensity_along_axis(
-            project_name, st.session_state.table_data_axis, pixel_size
+            project_name,
+            table_data_axis,
+            pixel_size,
         )
         st.pyplot(fig)
+        plt.close(fig)
 
         st.download_button(
             "Download figure as pdf", fig_stream, "axoden_summary_data_axis.pdf"
         )
-        st.dataframe(st.session_state.table_data_axis)
+        st.dataframe(table_data_axis)
 
     logger.info("Creating control plots pdf")
-    st.session_state.ctrl_plots_pdf = join_pdfs(st.session_state.figures)
+    ctrl_plots_pdf = join_pdfs(ctrl_figures)
 
     brain_regions = get_brain_regions(raw_files)
     if brain_regions:
         logger.info("Creating control plots by brain area")
         st.header("Control Plots by Brain Area")
 
         tabs = st.tabs(brain_regions)
 
-        brain_areas = st.session_state.table_data.brain_area.to_list()
-        figure_dict = get_figure_by_brain_region(st.session_state.figures, brain_areas)
+        brain_areas = table_data.brain_area.to_list()
+        figure_dict = get_figure_by_brain_region(ctrl_figures, brain_areas)
 
         for tab, brain_region in zip(tabs, brain_regions):
             figures = figure_dict[brain_region]
 
             with tab:
                 if len(figures) > 1:
                     indices = [str(x) for x in range(len(figures))]
                     tabs_brain_region = st.tabs(indices)
                     for i, tab_fig_nr in enumerate(tabs_brain_region):
                         with tab_fig_nr:
-                            pdf_figure = pdf2stream(figures[i]).getvalue()
-                            pdf_viewer(pdf_figure, key=f"{brain_region}_{i}")
+                            pdf_viewer(figures[i].getvalue(), key=f"{brain_region}_{i}")
                 else:
-                    pdf_figure = pdf2stream(figures[0]).getvalue()
-                    pdf_viewer(pdf_figure, key=brain_region)
+                    pdf_viewer(figures[0].getvalue(), key=brain_region)
 
         st.download_button(
             "Download plots as pdf",
-            st.session_state.ctrl_plots_pdf,
+            ctrl_plots_pdf,
             "control_plots.pdf",
         )
 
 
 if __name__ == "__main__":
     st.set_page_config(page_title="Axoden App", page_icon="📊️")
     axo_den_app()
```

### Comparing `axoden-1.0.2/axoden/gui/streamlit_app/__main__.py` & `axoden-1.1.0/axoden/gui/streamlit_app/__main__.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/axoden/gui/streamlit_app/app_utils.py` & `axoden-1.1.0/axoden/gui/streamlit_app/app_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,59 +2,34 @@
 from io import BytesIO
 from typing import Dict, Iterable, List, Tuple
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import pypdf
 import streamlit as st
 from matplotlib.figure import Figure
 from PIL import UnidentifiedImageError
 from streamlit.runtime.uploaded_file_manager import UploadedFile
 
-from axoden.gui.streamlit_app.pdf_utils import fig2pdfpage, fig2stream, pages2pdf
+from axoden.gui.streamlit_app.pdf_utils import fig2stream
 from axoden.volume_projections import (
     collect_info_from_filename,
     plot_signal_intensity_along_axis,
     plot_summary_data,
     process_image,
 )
 
 matplotlib.use("Agg")  # fixes hanging tests due to use of tk backend
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.WARNING)
 
 
-def init_session_state():
-    """Initializes the session state variables."""
-    if "figures" not in st.session_state:
-        st.session_state.figures = []
-
-    if "ctrl_plots_pdf" not in st.session_state:
-        st.session_state.ctrl_plots_pdf = None
-
-    if "table_data" not in st.session_state:
-        st.session_state.table_data = None
-
-    if "table_data_axis" not in st.session_state:
-        st.session_state.table_data_axis = None
-
-    if "figure_cache" not in st.session_state:
-        st.session_state.figure_cache = {}
-
-
-def invalidate_figure_cache():
-    """Invalidates the figure cache."""
-    st.session_state.figure_cache = {}
-    logger.info("invalidated figure cache")
-
-
-@st.cache_data
+@st.cache_data(ttl=300)
 def get_brain_regions(raw_files: List[UploadedFile]) -> Iterable[str]:
     """
     Get the brain regions from the uploaded files.
 
     Args:
         raw_files (List[UploadedFile]): The raw uploaded files to process.
 
@@ -97,37 +72,35 @@
     Args:
         project_name (str): The name of the project.
         table_data_axis (pd.DataFrame): The table data containing the signal intensity
             values along the axis.
         pixel_size (float): The size of each pixel.
 
     Returns:
-        Tuple[Figure, BytesIO]: A tuple containing the generated figure and a BytesIO
-            object representing the figure.
-
+        Tuple[Figure, BytesIO]: A tuple containing the generated figure and file stream.
     """
     logger.info("creating signal intensity along axis")
     fig = plot_signal_intensity_along_axis(project_name, table_data_axis, pixel_size)
     fig_stream = fig2stream(fig)
     return fig, fig_stream
 
 
 def get_figure_by_brain_region(
-    figures: List[pypdf.PdfWriter], brain_areas: List[str]
-) -> Dict[str, List[pypdf.PdfWriter]]:
+    figures: List[BytesIO], brain_areas: List[str]
+) -> Dict[str, List[BytesIO]]:
     """
     Group the given figures by brain region.
 
     Args:
-        figures (List[pypdf.PdfWriter]): A list of figures to be grouped.
+        figures (List[BytesIO]): A list of figure streams to be grouped.
         brain_areas (List[str]): A list of brain areas corresponding to each figure.
 
     Returns:
-        Dict[str, List[pypdf.PdfWriter]]: A dictionary where the keys are brain regions
-            and the values are lists of figures belonging to each brain region.
+        Dict[str, List[BytesIO]]: A dictionary where the keys are brain regions
+            and the values are lists of figure streams belonging to each brain region.
     """
     logger.info("get_figure_by_brain_region")
     figures_out = {}
     for fig, brain_area in zip(figures, brain_areas):
         if brain_area not in figures_out:
             figures_out[brain_area] = []
 
@@ -136,29 +109,25 @@
     return figures_out
 
 
 def process_images(
     raw_files: List[UploadedFile],
     pixel_size: float,
     is_masked: bool,
-    cache: Dict[Tuple[str, float, bool], Tuple[pypdf.PdfWriter, dict, dict]] = None,
-) -> Tuple[List[plt.Figure], pd.DataFrame, pd.DataFrame]:
-    """
-    Process a list of raw image files.
+) -> Tuple[List[BytesIO], pd.DataFrame, pd.DataFrame]:
+    """Process a list of raw image files.
 
     Args:
         raw_files (List[UploadedFile]): A list of raw image files.
         pixel_size (float): The pixel size.
         is_masked (bool): A flag indicating whether the images are masked.
-        cache (Dict[(str, float, bool), (pypdf.PdfWriter, dict, dict)], optional):
-            Use st.session_state.figure_cache as an intermediate cache. Defaults to None
 
     Returns:
-        Tuple[List[plt.Figure], pd.DataFrame, pd.DataFrame]: A tuple containing the
-            processed figures, table data, and table data axis.
+        Tuple[List[BytesIO], pd.DataFrame, pd.DataFrame]: A tuple containing the
+            processed figure streams, table data, and table data axis.
     """
 
     if not raw_files:
         return [], None, None
 
     logger.info("process_images")
     table_data = pd.DataFrame()
@@ -169,16 +138,18 @@
     progress_bar = st.progress(0.0, text=f"Processing image {1}/{len(raw_files)}")
     progress_step_size = 1.0 / len(raw_files)
 
     for i, raw_image in enumerate(raw_files):
         progress_bar.progress(
             i * progress_step_size, text=f"Processing image {(i+1)}/{len(raw_files)}"
         )
-        fig, data_row, data_axis_row = process_image_single(
-            raw_image, pixel_size, is_masked, cache=cache
+        fig, data_row, data_axis_row = process_image_single_cached(
+            raw_image,
+            pixel_size,
+            is_masked,
         )
 
         if np.sum(table_data.shape) == 0:
             table_data = pd.DataFrame(columns=data_row.keys())
         table_data.loc[len(table_data)] = data_row
 
         if np.sum(table_data_axis.shape) == 0:
@@ -192,35 +163,34 @@
         table_data["pixels_signal"] / table_data["pixels_total"] * 100
     )
 
     progress_bar.empty()
     return figures, table_data, table_data_axis
 
 
-def process_image_single(raw_image, pixel_size, is_masked, cache={}):
-    """
-    Process a single image.
+def hash_uploaded_file(file: UploadedFile) -> str:
+    """Hash util for an uploaded file."""
+    return file.file_id
+
+
+@st.cache_data(ttl=300, hash_funcs={UploadedFile: hash_uploaded_file}, max_entries=100)
+def process_image_single_cached(
+    raw_image: UploadedFile, pixel_size: float, is_masked: bool
+) -> Tuple[BytesIO, Dict, Dict]:
+    """Process a single image.
 
     Args:
-        raw_image (object): The raw image object.
-        pixel_size (float): The pixel size.
+        raw_image (UploadedFile): The input image object.
+        pixel_size (float): The pixel size in um.
         is_masked (bool): Flag indicating whether the image is masked.
-        cache (dict, optional): The cache dictionary to store processed images.
-            Defaults to None.
 
     Returns:
-        tuple: A tuple containing the processed image, temporary variables,
-            and temporary axis.
+        Tuple[BytesIO, Dict, Dict]: A tuple containing the processed image as a stream
+            and the data and axis data
     """
-
-    cache_key = (raw_image.file_id, pixel_size, is_masked)
-    if cache_key in cache:
-        logger.info(f"process_image_single found cache for {cache_key}")
-        return cache[cache_key]
-
     try:
         animal, brain_area, group = collect_info_from_filename(raw_image.name)
     except ValueError as e:
         logger.error(f"Error: {e}")
         st.warning(f"Error: {e}")
         st.stop()
         return None, None, None
@@ -235,15 +205,14 @@
         )
     except UnidentifiedImageError as e:
         logger.error(f"Error: {e}")
         st.warning(f"Error: {e}")
         st.stop()
         return None, None, None
 
-    pdf_fig = fig2pdfpage(fig)
-    pdf_fig = pages2pdf([pdf_fig])
-    plt.close(fig)
+    # pdf_fig = fig2pdfpage(fig)
+    # pdf_fig = pages2pdf([pdf_fig])
 
-    cache[(raw_image.file_id, pixel_size, is_masked)] = (pdf_fig, _temp_, _temp_axis_)
-    logger.info(f"process_image_single created cache for {cache_key}")
+    pdf_fig = fig2stream(fig)
+    plt.close(fig)
 
     return pdf_fig, _temp_, _temp_axis_
```

### Comparing `axoden-1.0.2/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py` & `axoden-1.1.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 The memory is erased when closing or refreshing the browser.  
 No third party can access the data in memory.  
 The developers of AxoDen have no access to any uploaded nor generated data on the AxoDen web app.  
 Only the user can see, interact and store the data the user has uploaded and generated.  
 """
     )
 
+    st.markdown("## Part 1: Prepare your images")
+    st.image("media/preprocessing.jpg")
+
     st.markdown(
         """
-## Part 1: Prepare your images
 Preparing your images for AxoDen requires the use of 3rd party software.
 
 We recommend using ImageJ or FIJI to modify your images because programs such as Adobe Illustrator
 can redistribute the color information into 3 or more channels when saving the modified image as .tif.
 
 Download ImageJ/FIJI here: [imagej.net](https://imagej.net/)
 
@@ -65,15 +67,17 @@
     7. Save the resulting image following AxoDen naming convention.
 
 > :point_up: :blue[_TIP:_]  
 > _Use the histogram (Analyze > Histogram) to confirm that the background fluorescence in the brain region does not contain zero values._
 """
     )
 
-    st.markdown("""## Part 2: AxoDen analysis""")
+    st.markdown("## Part 2: AxoDen analysis")
+
+    st.image("media/workflow.jpg")
 
     st.markdown(
         """
 If you want to test AxoDen quickly, you can download the test images from
 [the github repository](https://github.com/raqueladaia/AxoDen/tree/main/test_images)
 """
     )
```

### Comparing `axoden-1.0.2/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py` & `axoden-1.1.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/axoden/gui/streamlit_app/pdf_utils.py` & `axoden-1.1.0/axoden/gui/streamlit_app/pdf_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from io import BytesIO
-from typing import List, Union
+from typing import List
 
 from matplotlib.figure import Figure
 from pypdf import PdfReader, PdfWriter
 from pypdf._page import PageObject
 
 
 def fig2pdfpage(fig: Figure) -> PageObject:
@@ -71,28 +71,31 @@
 
     pdf = PdfWriter()
     for page in pages:
         pdf.add_page(page)
     return pdf
 
 
-def join_pdfs(pdfs: List[Union[PdfReader, PdfWriter]]) -> BytesIO:
+def join_pdfs(pdf_streams: List[BytesIO]) -> BytesIO:
     """Joins all first pages of multiple pdfs into a single pdf.
 
     This function only cares about the first page.
     These types of pdfs are used when figures are converted to pdfs containing only one
     page. The output BytesIO stream can be directly used as a download in Streamlit.
 
     Args:
-        pdfs (List[PdfReader | PdfWriter]): list of pdfs
+        pdfs (List[BytesIO]): list of pdfs as streams
 
     Returns:
         BytesIO: BytesIO stream of the joined pdf
 
     """
     pdf = PdfWriter()
-    for p in pdfs:
+    for p_stream in pdf_streams:
+        p = PdfReader(p_stream)
+
         page = p.pages[0]
         pdf.add_page(page)
-    pdf_stream = BytesIO()
-    pdf.write_stream(pdf_stream)
-    return pdf_stream
+
+    out_pdf_stream = BytesIO()
+    pdf.write_stream(out_pdf_stream)
+    return out_pdf_stream
```

### Comparing `axoden-1.0.2/axoden/volume_projections.py` & `axoden-1.1.0/axoden/volume_projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,15 @@
 
         if np.sum(table_data_axis.shape) == 0:
             table_data_axis = pd.DataFrame(columns=_temp_axis_.keys())
         table_data_axis.loc[len(table_data_axis)] = _temp_axis_
 
         # Save control plot
         if save:
-            figure_name = f"{animal}_{brain_area}_control_plot.pdf"
+            figure_name = f"{animal}_{brain_area}_{group}_control_plot.pdf"
             figure_path = os.path.join(control_plot_path, figure_name)
             plt.savefig(figure_path, dpi=300)
         plt.close(fig)
 
     # Compute the percentage of white pixels
     table_data["percent_signal"] = (
         table_data["pixels_signal"] / table_data["pixels_total"] * 100
```

### Comparing `axoden-1.0.2/media/control_plots.jpg` & `axoden-1.1.0/media/control_plots.jpg`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/media/summary_data.pdf` & `axoden-1.1.0/media/summary_data.pdf`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/media/summary_data_axis.pdf` & `axoden-1.1.0/media/summary_data_axis.pdf`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/pyproject.toml` & `axoden-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.2/PKG-INFO` & `axoden-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axoden
-Version: 1.0.2
+Version: 1.1.0
 Summary: axoden simplifies the quantification of axonal projections in neuroscience.
 Author-email: Raquel Adaia Sandoval Ortega <raqueladaia@gmail.com>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: tqdm >= 4.0.0
 Requires-Dist: numpy >= 1.16.0
@@ -19,26 +19,30 @@
 Project-URL: Home, https://github.com/raqueladaia/AxoDen
 Provides-Extra: gui
 
 [![Test](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml)
 [![Lint](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml)
 [![PyPI](https://img.shields.io/pypi/v/axoden?label=pypi%20package)](https://pypi.org/project/axoden)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/axoden)
+[![Documentation](https://img.shields.io/badge/Documentation-8A2BE2)](https://raqueladaia.github.io/AxoDen/)
 
 # Axoden
 
+<img src="https://github.com/raqueladaia/AxoDen/blob/main/media/workflow.jpg?raw=true)">
+
+
 ## Table of Contents
 
 - [How to use AxoDen](#how-to-use-axoden)
   - [Streamlit App](#streamlit-app)
   - [Standalone GUI](#standalone-gui)
 - [Installation](#installation)
   - [With pip](#pip-install)
   - [Git clone](#clone-from-github)
-- [Contributing](#contributing)
+- [Using AxoDen in your code](#using-axoden-in-your-code)
 
 ## Overview of AxoDen
 
 AxoDen is an open source platform that facilitates and streamlines the quantification of fluorescently labeled axonal projections of a given brain area.
 
 AxoDen accepts .tif images, transforms them into gray scale and uses the Otsu method to set a threshold that distinguishes signal from background. Because it collects the pixel values of any color channel which sum is above zero, users can use any fluorophore and obtain the same quantification accuracy. In addition, given that the input are images of projections, AxoDen can be applied to virtually any animal species.
 
@@ -202,15 +206,15 @@
 This should automatically open a browser window to the app.
 If not, streamlit will post the URL where you can reach the web app,
 usually at http://localhost:8501.
 
 
 This is the same interface as the [Streamlit Web App](https://axoden.streamlit.app).
 
-# Using axoden in your code
+## Using axoden in your code
 Below you find a few examples of how to use axoden.
 You can see the full [documentation here](https://raqueladaia.github.io/AxoDen/).
 
 You can process a single image. This will not save any results or plots.
 ```python
 import axoden
```

