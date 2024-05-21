# Comparing `tmp/geetools-1.3.0.tar.gz` & `tmp/geetools-1.3.1.tar.gz`

## Comparing `geetools-1.3.0.tar` & `geetools-1.3.1.tar`

### file list

```diff
@@ -1,299 +1,302 @@
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 geetools-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 geetools-1.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 geetools-1.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 geetools-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 geetools-1.3.0/RELEASE.rst
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 geetools-1.3.0/noxfile.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 geetools-1.3.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 geetools-1.3.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 geetools-1.3.0/.github/workflows/unit.yaml
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/conf.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/index.rst
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/_extension/docstring.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/_static/custom.css
--rw-r--r--   0        0        0   467521 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/_static/logo.png
--rw-r--r--   0        0        0   136592 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/_static/switcher.json
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/_static/we-need-you.jpg
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/example/asset.ipynb
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/example/index.rst
--rw-r--r--   0        0        0   405609 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/example/plot_featureCollection.ipynb
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/example/template.ipynb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/author.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/contribute.rst
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/index.rst
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/inspiration.rst
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/install.rst
--rw-r--r--   0        0        0    22128 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/layout.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/license.rst
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/migration.rst
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/pattern.rst
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 geetools-1.3.0/docs/usage/quickstart.rst
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/__init__.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_decision_tree.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_expressions.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_filters.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_indices.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_manager.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_oauth.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_utils.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/_deprecated_visualization.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/accessors.py
--rw-r--r--   0        0        0    30152 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/algorithms.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/bitreader.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/classification.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/composite.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/types.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Array/__init__.py
--rw-r--r--   0        0        0    25711 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Asset/__init__.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Authenticate/__init__.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/ComputedObject/__init__.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Date/__init__.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/DateRange/__init__.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Dictionary/__init__.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Feature/__init__.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/FeatureCollection/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Filter/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Geometry/__init__.py
--rw-r--r--   0        0        0    45287 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Image/__init__.py
--rw-r--r--   0        0        0    30124 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/ImageCollection/__init__.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Initialize/__init__.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Join/__init__.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/List/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/Number/__init__.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/String/__init__.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/batch/__init__.py
--rw-r--r--   0        0        0    14601 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/batch/featurecollection.py
--rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/batch/image.py
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/batch/imagecollection.py
--rw-r--r--   0        0        0    10294 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/batch/utils.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/__init__.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_array.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_collection.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_computedobject.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_date.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_dictionary.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_ee_list.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_element.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_feature.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_featurecollection.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_geometry.py
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_image.py
--rw-r--r--   0        0        0    35843 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_imagecollection.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_number.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 geetools-1.3.0/geetools/tools/_deprecated_string.py
--rw-r--r--   0        0        0     6817 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/algorithms/brdf.ipynb
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/algorithms/distance_to_mask.ipynb
--rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/algorithms/euclidean_distance.ipynb
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/algorithms/harmonize.ipynb
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/algorithms/mask_cover.ipynb
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/algorithms/pansharpen.ipynb
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/batch/ImageCollectionToDrive.ipynb
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/batch/exportByFeat.ipynb
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/batch/exportToGCS.ipynb
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/bitreader/BitReader.ipynb
--rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/cloud_mask/cloud_masking.ipynb
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/collection/joinByProperty.ipynb
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/composite/closest_date.ipynb
--rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/composite/medoid.ipynb
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/composite/medoid_score.ipynb
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/date/dayRangeIntervals.ipynb
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/date/since_epoch.ipynb
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/geometry/getRegion.ipynb
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/addConstantBand.ipynb
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/addSuffix_addPrefix.ipynb
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/bufferMask.ipynb
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/clipToCollection.ipynb
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/distributions.ipynb
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/parametrize.ipynb
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/removeBands.ipynb
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/renameDict.ipynb
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/renamePattern.ipynb
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/image/toGrid.ipynb
--rw-r--r--   0        0        0    45107 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/imagecollection/distributions.ipynb
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/imagecollection/mosaicSameDay.ipynb
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/imagecollection/parametrizeProperty.ipynb
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 geetools-1.3.0/notebooks/visualization/stretching.ipynb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Array.py
--rw-r--r--   0        0        0    13037 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ComputedObect.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Date.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_DateRange.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Dictionary.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Feature.py
--rw-r--r--   0        0        0     9727 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Filter.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Float.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Geometry.py
--rw-r--r--   0        0        0    29556 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Integer.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Join.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Number.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_String.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_deprecated.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset/test_glob.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset/test_iterdir.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset/test_iterdir_recursive.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset/test_parents.yml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset/test_rglob.yml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Asset/test_rmdir_recursive_dry_run.yml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Feature/test_deprecated_to_feature_collection.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Feature/test_remove_properties.yml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Feature/test_to_feature_collection.yml
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_by_features.yml
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_by_features_with_id.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_by_features_with_properties.yml
--rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_by_properties.yml
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_by_properties_with_id.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_by_properties_with_properties.yml
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_deprecated_clean.yml
--rw-r--r--   0        0        0   902233 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_deprecated_merge.yml
--rw-r--r--   0        0        0   902233 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_merge_geometries.yml
--rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_bar.png
--rw-r--r--   0        0        0    21949 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_donut.png
--rw-r--r--   0        0        0    19842 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_pie.png
--rw-r--r--   0        0        0    17139 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_scatter.png
--rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_stacked.png
--rw-r--r--   0        0        0    49664 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_properties_area.png
--rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_properties_bar.png
--rw-r--r--   0        0        0    52424 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_properties_plot.png
--rw-r--r--   0        0        0    13014 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_plot_hist.png
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_FeatureCollection/test_to_polygons.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Geometry/test_deprecated_line.yml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Geometry/test_deprecated_point.yml
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Geometry/test_deprecated_polygon.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Geometry/test_keep_type.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_add_date.csv
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_add_prefix_to_all.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_add_prefix_to_selected.yml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_add_suffix_to_all.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_add_suffix_to_selected.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_clip_on_collection_bands.yml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_clip_on_collection_property.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_clip_on_collection_without_properties_bands.yml
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_clip_on_collection_without_properties_property.yml
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_default_spectral_indices.csv
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_add_multi_band.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_add_prefix.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_add_suffix.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_clip_to_collection_bands.yml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_clip_to_collection_property.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_compute.csv
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_doy_to_date.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_empty.csv
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_empty_copy.csv
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_evi.csv
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_gauss_function.csv
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_get_value.csv
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_linear_function.csv
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_make_date_band.csv
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_mask_island.png
--rw-r--r--   0        0        0    73714 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_method.npz
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_mix_bands.yml
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_nbr.csv
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_nbr2.csv
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_ndfi.csv
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_ndvi.csv
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_parametrize.csv
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_remove_bands.yml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_rename_dict.yml
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_rename_pattern.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_sum_bands.csv
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_tasseled_cap.csv
--rw-r--r--   0        0        0    74199 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_deprecated_to_grid.npz
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_doy_to_date.csv
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_doy_to_date_with_band.csv
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_doy_to_date_with_format.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_full.csv
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_full_like.csv
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_full_like_with_mask.csv
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_full_with_lists.csv
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_full_with_name.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_full_with_value.csv
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_gauss.csv
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_gauss_with_band.csv
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_get_scale_params.yml
--rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_get_stac.yml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_get_values.csv
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_get_values_with_scale.csv
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_histogram_match.csv
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_interpolate_bands.csv
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_islet_mask.png
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_mask_S2_clouds.csv
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_merge.yml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_negative_clip.csv
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_pan_sharpen.csv
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_prefix.yml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_preprocess.csv
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_reduce_bands.csv
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_reduce_bands_with_bands.csv
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_reduce_bands_with_name.csv
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_remove.yml
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_remove_properties.yml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_rename.yml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_scale_and_offset.csv
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_suffix.yml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_tasseled_cap.csv
--rw-r--r--   0        0        0    74199 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Image/test_to_grid.npz
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_append.yml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_closest_s2_sr.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_collection_mask.csv
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_deprecated_add.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_deprecated_get_image.csv
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_deprecated_integral.csv
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_deprecated_mask.csv
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_deprecated_outliers.csv
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_get_citation.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_get_doi.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_get_offset_params.yml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_get_scale_params.yml
--rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_get_stac.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_iloc.csv
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_integral.csv
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_mask_s2.yml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_mask_s2_sr.csv
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_outliers.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_outliers_with_bands.csv
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_outliers_with_drop.csv
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_outliers_with_sigma.csv
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_pan_sharpen.csv
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_preprocess.csv
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_scale_and_offset.csv
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_spectral_indices.csv
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_tasseled_cap.csv
--rw-r--r--   0        0        0    27103 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_ImageCollection/test_to_xarray.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Join/test_by_property.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Join/test_by_property_outer.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_Join/test_deprecated_join.yml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_complement_with_different_type.yml
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_complement_with_same_type.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_delete.yml
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_difference.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_intersection.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_mix.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_remove_index.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_replace_dict.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_to_string.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_deprecated_zip.yml
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_intersection_with_different_type.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_intersection_with_same_type.yml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_product_with_different_type.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_product_with_same_type.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_replace_many.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_to_strings.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_union_with_duplicate.yml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_union_without_dupplicates.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_List/test_zip.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_deprecated/test_deprecated_cast_image.yml
--rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_deprecated/test_merge_geometry.yml
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 geetools-1.3.0/tests/test_deprecated/test_tobands.yml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 geetools-1.3.0/.gitignore
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 geetools-1.3.0/AUTHORS.rst
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 geetools-1.3.0/LICENSE
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 geetools-1.3.0/README.rst
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 geetools-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 geetools-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 geetools-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 geetools-1.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 geetools-1.3.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 geetools-1.3.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 geetools-1.3.1/RELEASE.rst
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 geetools-1.3.1/noxfile.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 geetools-1.3.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 geetools-1.3.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 geetools-1.3.1/.github/workflows/unit.yaml
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/conf.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/index.rst
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_extension/docstring.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_static/custom.css
+-rw-r--r--   0        0        0   467521 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_static/logo.png
+-rw-r--r--   0        0        0   136592 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_static/switcher.json
+-rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_static/we-need-you.jpg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_templates/python/class.rst
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_templates/python/function.rst
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_templates/python/method.rst
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/_templates/python/module.rst
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/example/asset.ipynb
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/example/index.rst
+-rw-r--r--   0        0        0   405629 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/example/plot_featureCollection.ipynb
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/example/template.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/author.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/contribute.rst
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/index.rst
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/inspiration.rst
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/install.rst
+-rw-r--r--   0        0        0    22128 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/layout.rst
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/license.rst
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/migration.rst
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/pattern.rst
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 geetools-1.3.1/docs/usage/quickstart.rst
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/__init__.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_decision_tree.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_expressions.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_filters.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_indices.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_manager.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_oauth.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_utils.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/_deprecated_visualization.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/accessors.py
+-rw-r--r--   0        0        0    30152 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/algorithms.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/bitreader.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/classification.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/composite.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/types.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Array/__init__.py
+-rw-r--r--   0        0        0    26859 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Asset/__init__.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Authenticate/__init__.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/ComputedObject/__init__.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Date/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/DateRange/__init__.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Dictionary/__init__.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Feature/__init__.py
+-rw-r--r--   0        0        0    22165 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/FeatureCollection/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Filter/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Geometry/__init__.py
+-rw-r--r--   0        0        0    47006 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Image/__init__.py
+-rw-r--r--   0        0        0    30124 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/ImageCollection/__init__.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Initialize/__init__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Join/__init__.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/List/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/Number/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/String/__init__.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/batch/__init__.py
+-rw-r--r--   0        0        0    14601 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/batch/featurecollection.py
+-rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/batch/image.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/batch/imagecollection.py
+-rw-r--r--   0        0        0    10294 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/batch/utils.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/__init__.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_array.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_collection.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_computedobject.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_date.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_dictionary.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_ee_list.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_element.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_feature.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_featurecollection.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_geometry.py
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_image.py
+-rw-r--r--   0        0        0    35843 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_imagecollection.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_number.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 geetools-1.3.1/geetools/tools/_deprecated_string.py
+-rw-r--r--   0        0        0     6817 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/algorithms/brdf.ipynb
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/algorithms/distance_to_mask.ipynb
+-rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/algorithms/euclidean_distance.ipynb
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/algorithms/harmonize.ipynb
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/algorithms/mask_cover.ipynb
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/algorithms/pansharpen.ipynb
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/batch/ImageCollectionToDrive.ipynb
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/batch/exportByFeat.ipynb
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/batch/exportToGCS.ipynb
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/bitreader/BitReader.ipynb
+-rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/cloud_mask/cloud_masking.ipynb
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/collection/joinByProperty.ipynb
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/composite/closest_date.ipynb
+-rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/composite/medoid.ipynb
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/composite/medoid_score.ipynb
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/date/dayRangeIntervals.ipynb
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/date/since_epoch.ipynb
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/geometry/getRegion.ipynb
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/addConstantBand.ipynb
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/addSuffix_addPrefix.ipynb
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/bufferMask.ipynb
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/clipToCollection.ipynb
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/distributions.ipynb
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/parametrize.ipynb
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/removeBands.ipynb
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/renameDict.ipynb
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/renamePattern.ipynb
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/image/toGrid.ipynb
+-rw-r--r--   0        0        0    45107 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/imagecollection/distributions.ipynb
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/imagecollection/mosaicSameDay.ipynb
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/imagecollection/parametrizeProperty.ipynb
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 geetools-1.3.1/notebooks/visualization/stretching.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Array.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ComputedObect.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Date.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_DateRange.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Dictionary.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Feature.py
+-rw-r--r--   0        0        0     9727 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Filter.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Float.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Geometry.py
+-rw-r--r--   0        0        0    30011 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Integer.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Join.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Number.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_String.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_deprecated.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset/test_glob.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset/test_iterdir.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset/test_iterdir_recursive.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset/test_parents.yml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset/test_rglob.yml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Asset/test_rmdir_recursive_dry_run.yml
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Feature/test_deprecated_to_feature_collection.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Feature/test_remove_properties.yml
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Feature/test_to_feature_collection.yml
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_by_features.yml
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_by_features_with_id.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_by_features_with_properties.yml
+-rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_by_properties.yml
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_by_properties_with_id.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_by_properties_with_properties.yml
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_deprecated_clean.yml
+-rw-r--r--   0        0        0   902233 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_deprecated_merge.yml
+-rw-r--r--   0        0        0   902233 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_merge_geometries.yml
+-rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_bar.png
+-rw-r--r--   0        0        0    21949 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_donut.png
+-rw-r--r--   0        0        0    19842 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_pie.png
+-rw-r--r--   0        0        0    17139 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_scatter.png
+-rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_stacked.png
+-rw-r--r--   0        0        0    49664 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_properties_area.png
+-rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_properties_bar.png
+-rw-r--r--   0        0        0    52424 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_properties_plot.png
+-rw-r--r--   0        0        0    13014 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_plot_hist.png
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_FeatureCollection/test_to_polygons.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Geometry/test_deprecated_line.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Geometry/test_deprecated_point.yml
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Geometry/test_deprecated_polygon.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Geometry/test_keep_type.yml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_add_date.csv
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_add_date_format.csv
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_add_prefix_to_all.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_add_prefix_to_selected.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_add_suffix_to_all.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_add_suffix_to_selected.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_clip_on_collection_bands.yml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_clip_on_collection_property.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_clip_on_collection_without_properties_bands.yml
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_clip_on_collection_without_properties_property.yml
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_default_spectral_indices.csv
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_add_multi_band.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_add_prefix.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_add_suffix.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_clip_to_collection_bands.yml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_clip_to_collection_property.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_compute.csv
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_doy_to_date.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_empty.csv
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_empty_copy.csv
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_evi.csv
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_gauss_function.csv
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_get_value.csv
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_linear_function.csv
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_make_date_band.csv
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_mask_island.png
+-rw-r--r--   0        0        0    73714 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_method.npz
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_mix_bands.yml
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_nbr.csv
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_nbr2.csv
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_ndfi.csv
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_ndvi.csv
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_parametrize.csv
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_remove_bands.yml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_rename_dict.yml
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_rename_pattern.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_sum_bands.csv
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_tasseled_cap.csv
+-rw-r--r--   0        0        0    74199 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_deprecated_to_grid.npz
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_doy_to_date.csv
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_doy_to_date_with_band.csv
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_doy_to_date_with_format.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_full.csv
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_full_like.csv
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_full_like_with_mask.csv
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_full_with_lists.csv
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_full_with_name.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_full_with_value.csv
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_gauss.csv
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_gauss_with_band.csv
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_get_scale_params.yml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_get_values.csv
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_get_values_with_scale.csv
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_histogram_match.csv
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_interpolate_bands.csv
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_islet_mask.png
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_mask_S2_clouds.csv
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_merge.yml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_negative_clip.csv
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_pan_sharpen.csv
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_prefix.yml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_preprocess.csv
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_reduce_bands.csv
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_reduce_bands_with_bands.csv
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_reduce_bands_with_name.csv
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_remove.yml
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_remove_properties.yml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_rename.yml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_scale_and_offset.csv
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_suffix.yml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_tasseled_cap.csv
+-rw-r--r--   0        0        0    74199 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Image/test_to_grid.npz
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_append.yml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_closest_s2_sr.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_collection_mask.csv
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_deprecated_add.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_deprecated_get_image.csv
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_deprecated_integral.csv
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_deprecated_mask.csv
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_deprecated_outliers.csv
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_get_citation.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_get_doi.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_get_offset_params.yml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_get_scale_params.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_iloc.csv
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_integral.csv
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_mask_s2.yml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_mask_s2_sr.csv
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_outliers.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_outliers_with_bands.csv
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_outliers_with_drop.csv
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_outliers_with_sigma.csv
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_pan_sharpen.csv
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_preprocess.csv
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_scale_and_offset.csv
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_spectral_indices.csv
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_tasseled_cap.csv
+-rw-r--r--   0        0        0    27149 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_ImageCollection/test_to_xarray.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Join/test_by_property.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Join/test_by_property_outer.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_Join/test_deprecated_join.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_complement_with_different_type.yml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_complement_with_same_type.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_delete.yml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_difference.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_intersection.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_mix.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_remove_index.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_replace_dict.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_to_string.yml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_deprecated_zip.yml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_intersection_with_different_type.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_intersection_with_same_type.yml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_product_with_different_type.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_product_with_same_type.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_replace_many.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_to_strings.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_union_with_duplicate.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_union_without_dupplicates.yml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_List/test_zip.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_deprecated/test_deprecated_cast_image.yml
+-rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_deprecated/test_merge_geometry.yml
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 geetools-1.3.1/tests/test_deprecated/test_tobands.yml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 geetools-1.3.1/.gitignore
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 geetools-1.3.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 geetools-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 geetools-1.3.1/README.rst
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 geetools-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 geetools-1.3.1/PKG-INFO
```

### Comparing `geetools-1.3.0/.pre-commit-config.yaml` & `geetools-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/CHANGELOG.rst` & `geetools-1.3.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/CONTRIBUTING.rst` & `geetools-1.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/RELEASE.rst` & `geetools-1.3.1/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/noxfile.py` & `geetools-1.3.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/.github/workflows/release.yaml` & `geetools-1.3.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/.github/workflows/unit.yaml` & `geetools-1.3.1/.github/workflows/unit.yaml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/conf.py` & `geetools-1.3.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # add . to sys to import local extensions
 sys.path.append(str(Path(".").resolve()))
 
 # -- Project information -------------------------------------------------------
 project = "geetools"
 author = "Rodrigo E. Principe"
 copyright = f"2017-{datetime.now().year}, {author}"
-release = "1.3.0"
+release = "1.3.1"
 
 # -- General configuration -----------------------------------------------------
 extensions = [
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosectionlabel",
@@ -94,22 +94,23 @@
 html_css_files = ["custom.css"]
 
 # -- Options for autosummary/autodoc output ------------------------------------
 autodoc_typehints = "description"
 autoapi_dirs = ["../geetools"]
 autoapi_python_class_content = "both"
 autoapi_member_order = "groupwise"
+autoapi_template_dir = "_templates"
 autoapi_options = [
     "members",
     "undoc-members",
     "show-inheritance",
     "show-module-summary",
     "special-members",
 ]
-autoapi_render_in_single_page = ["class", "function", "method"]
+autoapi_own_page_level = "method"
 
 # -- Options for intersphinx output --------------------------------------------
 intersphinx_mapping = {}
 
 # -- options for the autolabel extension ---------------------------------------
 autosectionlabel_prefix_document = True
```

### Comparing `geetools-1.3.0/docs/index.rst` & `geetools-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/_extension/docstring.py` & `geetools-1.3.1/docs/_extension/docstring.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/_static/logo.png` & `geetools-1.3.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/_static/logo.svg` & `geetools-1.3.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/_static/we-need-you.jpg` & `geetools-1.3.1/docs/_static/we-need-you.jpg`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/example/asset.ipynb` & `geetools-1.3.1/docs/example/asset.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/example/index.rst` & `geetools-1.3.1/docs/example/index.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/example/plot_featureCollection.ipynb` & `geetools-1.3.1/docs/example/plot_featureCollection.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986359126984127%*

 * *Differences: {"'cells'": "{1: {'source': "*

 * *            "['[![github](https://img.shields.io/badge/-see%20sources-white?logo=github&labelColor=555)](https://github.com/gee-community/geetools/blob/main/docs/example/plot_featureCollection.ipynb)\\n', "*

 * *            "'[![colab](https://img.shields.io/badge/-open%20in%20colab-blue?logo=googlecolab&labelColor=555)](https://colab.research.google.com/github/gee-community/geetools/blob/main/docs/example/plot_featureCollection.ipynb)']}, "*

 * *            "19: {'source': {insert: [(0, […]*

```diff
@@ -9,16 +9,16 @@
                 "The `geetools` extension contains a set of functions for rendering charts from `ee.FeatureCollection` objects. The choice of function determines the arrangement of data in the chart, i.e., what defines x- and y-axis values and what defines the series. Use the following function descriptions and examples to determine the best function and chart type for your purpose."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "[![github](https://img.shields.io/badge/-see%20sources-white?logo=github&labelColor=555)](https://github.com/gee_community/geetools/blob/main/docs/example/plot_feature.ipynb)\n",
-                "[![colab](https://img.shields.io/badge/-open%20in%20colab-blue?logo=googlecolab&labelColor=555)](https://colab.research.google.com/github/gee_community/geetools/blob/main/docs/example/plot_feature.ipynb)"
+                "[![github](https://img.shields.io/badge/-see%20sources-white?logo=github&labelColor=555)](https://github.com/gee-community/geetools/blob/main/docs/example/plot_featureCollection.ipynb)\n",
+                "[![colab](https://img.shields.io/badge/-open%20in%20colab-blue?logo=googlecolab&labelColor=555)](https://colab.research.google.com/github/gee-community/geetools/blob/main/docs/example/plot_featureCollection.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Set up environment\n",
@@ -307,15 +307,15 @@
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## ee.FEatureCollection.geetools.plot_by_properties\n",
+                "## ee.FeatureCollection.geetools.plot_by_properties\n",
                 "\n",
                 "## Column chart\n",
                 "\n",
                 "Feature properties are plotted along the x-axis, labeled and sorted by a dictionary input; the values of the given properties are plotted along the y-axis. Series are features, represented by columns, labeled by values of a selected property."
             ]
         },
         {
@@ -445,15 +445,15 @@
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## ee.FEatureCollection.geetools.plot_hist\n",
+                "## ee.FeatureCollection.geetools.plot_hist\n",
                 "\n",
                 "The x-axis is defined by value bins for the range of values of a selected property; the y-axis is the number of elements in the given bin."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
```

### Comparing `geetools-1.3.0/docs/example/template.ipynb` & `geetools-1.3.1/docs/example/template.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/index.rst` & `geetools-1.3.1/docs/usage/index.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/inspiration.rst` & `geetools-1.3.1/docs/usage/inspiration.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/install.rst` & `geetools-1.3.1/docs/usage/install.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/layout.rst` & `geetools-1.3.1/docs/usage/layout.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/migration.rst` & `geetools-1.3.1/docs/usage/migration.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/pattern.rst` & `geetools-1.3.1/docs/usage/pattern.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/docs/usage/quickstart.rst` & `geetools-1.3.1/docs/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/__init__.py` & `geetools-1.3.1/geetools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,14 @@
 # from .Array import ArrayAccessor
 # from .DateRange import DateRangeAccessor
 
 
 __title__ = "geetools"
 __summary__ = "A set of useful tools to use with Google Earth Engine Python" "API"
 __uri__ = "http://geetools.readthedocs.io"
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 __author__ = "Rodrigo E. Principe"
 __email__ = "fitoprincipe82@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "2017 Rodrigo E. Principe"
```

### Comparing `geetools-1.3.0/geetools/_deprecated_expressions.py` & `geetools-1.3.1/geetools/_deprecated_expressions.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/_deprecated_indices.py` & `geetools-1.3.1/geetools/_deprecated_indices.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/_deprecated_manager.py` & `geetools-1.3.1/geetools/_deprecated_manager.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/_deprecated_oauth.py` & `geetools-1.3.1/geetools/_deprecated_oauth.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/_deprecated_utils.py` & `geetools-1.3.1/geetools/_deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/_deprecated_visualization.py` & `geetools-1.3.1/geetools/_deprecated_visualization.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/accessors.py` & `geetools-1.3.1/geetools/accessors.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/algorithms.py` & `geetools-1.3.1/geetools/algorithms.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/bitreader.py` & `geetools-1.3.1/geetools/bitreader.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/classification.py` & `geetools-1.3.1/geetools/classification.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/composite.py` & `geetools-1.3.1/geetools/composite.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/types.py` & `geetools-1.3.1/geetools/types.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Array/__init__.py` & `geetools-1.3.1/geetools/Array/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Asset/__init__.py` & `geetools-1.3.1/geetools/Asset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import re
 from pathlib import PurePosixPath
 from typing import Optional
 
 import ee
+from anyascii import anyascii
 
 from geetools.accessors import _register_extention
 from geetools.types import pathlike
 
 
 @_register_extention(ee)
 class Asset:
@@ -489,15 +490,15 @@
         # else raise an error with the 1st parent name
         if len(to_be_created) > 1 and parents is False:
             raise ValueError(f'Parent Asset "{to_be_created[-1]}" does not exist.')
 
         # 2 option either there is 1 single element in the list or all the parents are included
         # we need to walk it in reversed to make sure the parents are build first.
         for p in reversed(to_be_created):
-            ee.data.createAsset({"type": "FOLDER"}, p.as_posix())
+            ee.data.createFolder(p.as_posix())
 
         return self
 
     @property
     def owner(self):
         """Return the asset owner (project name).
 
@@ -706,7 +707,44 @@
         Examples:
             .. code-block:: python
 
                 asset = ee.Asset("projects/ee-geetools/assets/folder")
                 asset.rglob("image_*")
         """
         return [a for a in self.iterdir(recursive=True) if a.match(pattern)]
+
+    def as_description(self) -> str:
+        """Transform the name of the Asset in to a description compatible string for a Task.
+
+        Returns:
+            The formatted description.
+        """
+        return self.format_description(self.name)
+
+    @staticmethod
+    def format_description(description: str) -> str:
+        """Format a name to be accepted as a Task description.
+
+        The rule is:
+        The description must contain only the following characters: a..z, A..Z,
+        0..9, ".", ",", ":", ";", "_" or "-". The description must be at most 100
+        characters long.
+
+        Args:
+            description: The description to format.
+
+        Returns:
+            The formatted description.
+        """
+        replacements = [
+            [[" "], "_"],
+            [["/"], "-"],
+            [["?", "!", "¿", "*"], "."],
+            [["(", ")", "[", "]", "{", "}"], ":"],
+        ]
+
+        desc = anyascii(description)
+        for chars, rep in replacements:
+            pattern = "|".join(re.escape(c) for c in chars)
+            desc = re.sub(pattern, rep, desc)  # type: ignore
+
+        return desc[:100]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geetools-1.3.0/geetools/Authenticate/__init__.py` & `geetools-1.3.1/geetools/Authenticate/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/ComputedObject/__init__.py` & `geetools-1.3.1/geetools/ComputedObject/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Date/__init__.py` & `geetools-1.3.1/geetools/Date/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/DateRange/__init__.py` & `geetools-1.3.1/geetools/DateRange/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Dictionary/__init__.py` & `geetools-1.3.1/geetools/Dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Feature/__init__.py` & `geetools-1.3.1/geetools/Feature/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/FeatureCollection/__init__.py` & `geetools-1.3.1/geetools/FeatureCollection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,15 +359,15 @@
 
         # gather the data from the data variable
         labels = list(data.keys())
         if len(labels) != 1:
             raise ValueError("Pie chart can only be used with one property")
 
         kwargs["rwidth"] = kwargs.get("rwidth", 0.9)
-        kwargs["color"] = color or plt.cm.get_cmap("tab10").colors[0]
+        kwargs["color"] = color or plt.get_cmap("tab10").colors[0]
         ax.hist(list(data[labels[0]].values()), **kwargs)
         ax.set_xlabel(labels[0])
         ax.set_ylabel("frequency")
 
         # customize the layout of the axis
         ax.grid(axis="y")
         ax.set_axisbelow(True)
@@ -413,15 +413,15 @@
         # define the ax if not provided by the user
         if ax is None:
             fig, ax = plt.subplots()
 
         # gather the data from parameters
         labels = list(data.keys())
         props = list(data[labels[0]].keys())
-        colors = colors if colors else plt.cm.get_cmap("tab10").colors
+        colors = colors if colors else plt.get_cmap("tab10").colors
 
         # draw the chart based on the type
         if type == "plot":
             for i, label in enumerate(labels):
                 kwargs["color"] = colors[i]
                 name = props[0] if len(props) == 1 else "Properties values"
                 values = list(data[label].values())
```

### Comparing `geetools-1.3.0/geetools/Filter/__init__.py` & `geetools-1.3.1/geetools/Filter/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Geometry/__init__.py` & `geetools-1.3.1/geetools/Geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Image/__init__.py` & `geetools-1.3.1/geetools/Image/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,22 @@
     """Toolbox for the ``ee.Image`` class."""
 
     def __init__(self, obj: ee.Image):
         """Initialize the Image class."""
         self._obj = obj
 
     # -- band manipulation -----------------------------------------------------
-    def addDate(self) -> ee.Image:
+    def addDate(self, format: ee_str = "") -> ee.Image:
         """Add a band with the date of the image in the provided format.
 
-        The date is stored as a Timestamp in millisecond in a band "date".
+        If no format is provided, the date is stored as a Timestamp in millisecond in a band "date". If format band is provided, the date is store in a int8 band with the date in the provided format. This format needs to be a string that can be converted to a number.
+        If not an error will be thrown.
+
+        Args:
+            format: A date pattern, as described at http://joda-time.sourceforge.net/apidocs/org/joda/time/format/DateTimeFormat.html
 
         Returns:
             The image with the date band added.
 
         Examples:
             .. code-block:: python
 
@@ -47,16 +51,24 @@
                 image = ee.Image('COPERNICUS/S2_SR_HARMONIZED/20200101T100319_20200101T100321_T32TQM')
                 image = image.geetools.addDate()
                 date = image.select('date')
                 buffer = ee.Geometry.Point([12.4534, 41.9033]).buffer(100)
                 value = date.reduceRegion(ee.Reducer.first(), buffer, 10).get("date")
                 ee.Date(value).format('YYYY-MM-dd').getInfo()
         """
-        date = self._obj.date().millis()
-        return self._obj.addBands(ee.Image.constant(date).rename("date"))
+        # parse the inputs
+        isMillis = ee.String(format).equals(ee.String(""))
+        format = ee.String(format) if format else ee.String("YYYYMMdd")
+
+        # extract the date from the object and create a image band from it
+        date = self._obj.date()
+        date = ee.Algorithms.If(isMillis, date.millis(), ee.Number.parse(date.format(format)))
+        dateBand = ee.Image.constant(ee.Number(date)).rename("date")
+
+        return self._obj.addBands(dateBand)
 
     def addSuffix(self, suffix: ee_str, bands: ee_list = []) -> ee.Image:
         """Add a suffix to the image selected band.
 
         Add a suffix to the selected band. If no band is specified, the suffix is added to all bands.
 
         Parameters:
@@ -459,24 +471,26 @@
         return ee.Image.constant(values).rename(names)
 
     def fullLike(
         self,
         fillValue: ee_number,
         copyProperties: ee_int = 0,
         keepMask: ee_int = 0,
+        keepFootprint: ee_int = 1,
     ) -> ee.Image:
         """Create an image with the same band names, projection and scale as the original image.
 
         The projection is computed on the first band, make sure all bands have the same.
         The procduced image can also copy the properties of the original image and keep the mask.
 
         Parameters:
             fillValue: The value to fill the image with.
             copyProperties: If True, the properties of the original image will be copied to the new one.
             keepMask: If True, the mask of the original image will be copied to the new one.
+            keepFootprint: If True, the footprint of the original image will be used to clip the new image.
 
         Returns:
             An image with the same band names, projection and scale as the original image.
 
         Examples:
             .. code-block:: python
 
@@ -484,27 +498,42 @@
 
                 ee.Initialize()
 
                 image = ee.Image('COPERNICUS/S2_SR_HARMONIZED/20200101T100319_20200101T100321_T32TQM')
                 image = image.geetools.fullLike(0)
                 print(image.bandNames().getInfo())
         """
+        # function params as GEE objects
         keepMask, copyProperties = ee.Number(keepMask), ee.Number(copyProperties)
+        keepFootprint = ee.Number(keepFootprint)
+        # get geometry, band names and property names
         footprint, bandNames = self._obj.geometry(), self._obj.bandNames()
+        properties = self._obj.propertyNames().remove(
+            "system:footprint"
+        )  # remove footprint as a "normal" property
+        # list of values to fill the image
         fillValue = ee.List.repeat(fillValue, bandNames.size())
-        image = (
-            self.full(fillValue, bandNames)
-            .reproject(self._obj.select(0).projection())
-            .clip(footprint)
+        # filled image
+        image = self.full(fillValue, bandNames)
+        # handler projection
+        projected_list = bandNames.map(
+            lambda b: image.select([b]).reproject(self._obj.select([b]).projection())
         )
-        withProperties = image.copyProperties(self._obj)
+        image = ee.ImageCollection.fromImages(projected_list).toBands().rename(bandNames)
+        # handle footprint
+        image_footprint = image.clip(footprint)  # sets system:footprint property
+        image = ee.Image(ee.Algorithms.If(keepFootprint, image_footprint, image))
+        # handle properties
+        withProperties = image.copyProperties(self._obj, properties)
         image = ee.Algorithms.If(copyProperties, withProperties, image)
+        # handle mask
         withMask = ee.Image(image).updateMask(self._obj.mask())
-        image = ee.Algorithms.If(keepMask, withMask, image)
-        return ee.Image(image)
+        image = ee.Image(ee.Algorithms.If(keepMask, withMask, image))
+        # handle band types
+        return ee.Image(image.cast(self._obj.bandTypes()))
 
     def reduceBands(
         self,
         reducer: str,
         bands: ee_list = [],
         name: ee_str = "",
     ) -> ee.Image:
```

### Comparing `geetools-1.3.0/geetools/ImageCollection/__init__.py` & `geetools-1.3.1/geetools/ImageCollection/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Initialize/__init__.py` & `geetools-1.3.1/geetools/Initialize/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Join/__init__.py` & `geetools-1.3.1/geetools/Join/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/List/__init__.py` & `geetools-1.3.1/geetools/List/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/Number/__init__.py` & `geetools-1.3.1/geetools/Number/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/String/__init__.py` & `geetools-1.3.1/geetools/String/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/batch/__init__.py` & `geetools-1.3.1/geetools/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/batch/featurecollection.py` & `geetools-1.3.1/geetools/batch/featurecollection.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/batch/image.py` & `geetools-1.3.1/geetools/batch/image.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/batch/imagecollection.py` & `geetools-1.3.1/geetools/batch/imagecollection.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/batch/utils.py` & `geetools-1.3.1/geetools/batch/utils.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/__init__.py` & `geetools-1.3.1/geetools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_array.py` & `geetools-1.3.1/geetools/tools/_deprecated_array.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_collection.py` & `geetools-1.3.1/geetools/tools/_deprecated_collection.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_computedobject.py` & `geetools-1.3.1/geetools/tools/_deprecated_computedobject.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_date.py` & `geetools-1.3.1/geetools/tools/_deprecated_date.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_dictionary.py` & `geetools-1.3.1/geetools/tools/_deprecated_dictionary.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_ee_list.py` & `geetools-1.3.1/geetools/tools/_deprecated_ee_list.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_featurecollection.py` & `geetools-1.3.1/geetools/tools/_deprecated_featurecollection.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_geometry.py` & `geetools-1.3.1/geetools/tools/_deprecated_geometry.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_image.py` & `geetools-1.3.1/geetools/tools/_deprecated_image.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_imagecollection.py` & `geetools-1.3.1/geetools/tools/_deprecated_imagecollection.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/geetools/tools/_deprecated_string.py` & `geetools-1.3.1/geetools/tools/_deprecated_string.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/algorithms/brdf.ipynb` & `geetools-1.3.1/notebooks/algorithms/brdf.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/algorithms/distance_to_mask.ipynb` & `geetools-1.3.1/notebooks/algorithms/distance_to_mask.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/algorithms/euclidean_distance.ipynb` & `geetools-1.3.1/notebooks/algorithms/euclidean_distance.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/algorithms/harmonize.ipynb` & `geetools-1.3.1/notebooks/algorithms/harmonize.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/algorithms/mask_cover.ipynb` & `geetools-1.3.1/notebooks/algorithms/mask_cover.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/algorithms/pansharpen.ipynb` & `geetools-1.3.1/notebooks/algorithms/pansharpen.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/batch/ImageCollectionToDrive.ipynb` & `geetools-1.3.1/notebooks/batch/ImageCollectionToDrive.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/batch/exportByFeat.ipynb` & `geetools-1.3.1/notebooks/batch/exportByFeat.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/batch/exportToGCS.ipynb` & `geetools-1.3.1/notebooks/batch/exportToGCS.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/bitreader/BitReader.ipynb` & `geetools-1.3.1/notebooks/bitreader/BitReader.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/cloud_mask/cloud_masking.ipynb` & `geetools-1.3.1/notebooks/cloud_mask/cloud_masking.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/collection/joinByProperty.ipynb` & `geetools-1.3.1/notebooks/collection/joinByProperty.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/composite/closest_date.ipynb` & `geetools-1.3.1/notebooks/composite/closest_date.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/composite/medoid.ipynb` & `geetools-1.3.1/notebooks/composite/medoid.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/composite/medoid_score.ipynb` & `geetools-1.3.1/notebooks/composite/medoid_score.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/date/dayRangeIntervals.ipynb` & `geetools-1.3.1/notebooks/date/dayRangeIntervals.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/date/since_epoch.ipynb` & `geetools-1.3.1/notebooks/date/since_epoch.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/geometry/getRegion.ipynb` & `geetools-1.3.1/notebooks/geometry/getRegion.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/addConstantBand.ipynb` & `geetools-1.3.1/notebooks/image/addConstantBand.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/addSuffix_addPrefix.ipynb` & `geetools-1.3.1/notebooks/image/addSuffix_addPrefix.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/bufferMask.ipynb` & `geetools-1.3.1/notebooks/image/bufferMask.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/clipToCollection.ipynb` & `geetools-1.3.1/notebooks/image/clipToCollection.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/distributions.ipynb` & `geetools-1.3.1/notebooks/image/distributions.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/parametrize.ipynb` & `geetools-1.3.1/notebooks/image/parametrize.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/removeBands.ipynb` & `geetools-1.3.1/notebooks/image/removeBands.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/renameDict.ipynb` & `geetools-1.3.1/notebooks/image/renameDict.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/renamePattern.ipynb` & `geetools-1.3.1/notebooks/image/renamePattern.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/image/toGrid.ipynb` & `geetools-1.3.1/notebooks/image/toGrid.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/imagecollection/distributions.ipynb` & `geetools-1.3.1/notebooks/imagecollection/distributions.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/imagecollection/mosaicSameDay.ipynb` & `geetools-1.3.1/notebooks/imagecollection/mosaicSameDay.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/imagecollection/parametrizeProperty.ipynb` & `geetools-1.3.1/notebooks/imagecollection/parametrizeProperty.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/notebooks/visualization/stretching.ipynb` & `geetools-1.3.1/notebooks/visualization/stretching.ipynb`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/conftest.py` & `geetools-1.3.1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Pytest session configuration."""
 
 import string
 
 import ee
 import pytest
 import pytest_gee
+import requests
 
 
 def pytest_configure() -> None:
     """Initialize earth engine according to the environment."""
     pytest_gee.init_ee_from_service_account()
 
 
@@ -223,7 +224,14 @@
 
 @pytest.fixture
 def climSamp():
     """Return the climate sample collection."""
     normClim = ee.ImageCollection("OREGONSTATE/PRISM/Norm81m").toBands()
     region = ee.Geometry.Rectangle(-123.41, 40.43, -116.38, 45.14)
     return normClim.sample(region, 5000)
+
+
+@pytest.fixture(scope="session")
+def stac_schema():
+    """Return the STAC collection schema."""
+    url = "https://raw.githubusercontent.com/radiantearth/stac-spec/master/collection-spec/json-schema/collection.json"
+    return requests.get(url).json()
```

### Comparing `geetools-1.3.0/tests/test_Array.py` & `geetools-1.3.1/tests/test_Array.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Asset.py` & `geetools-1.3.1/tests/test_Asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         asset = ee.Asset("projects/bar")
         assert asset.as_posix() == "projects/bar"
 
     def test_as_uri(self):
         asset = ee.Asset("projects/bar")
         assert asset.as_uri() == "https://code.earthengine.google.com/?asset=projects/bar"
 
+    def test_as_description(self):
+        asset = ee.Asset(f"projects/{EARTHENGINE_PROJECT}/assets/a weird name")
+        assert asset.as_description() == "a_weird_name"
+
 
 class TestOperations:
     """Test the operations that can be run on the asset."""
 
     def test_truediv(self):
         asset = ee.Asset("projects/bar")
         assert asset / "foo" == "projects/bar/foo"
```

### Comparing `geetools-1.3.0/tests/test_ComputedObect.py` & `geetools-1.3.1/tests/test_ComputedObect.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Date.py` & `geetools-1.3.1/tests/test_Date.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_DateRange.py` & `geetools-1.3.1/tests/test_DateRange.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Dictionary.py` & `geetools-1.3.1/tests/test_Dictionary.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Feature.py` & `geetools-1.3.1/tests/test_Feature.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection.py` & `geetools-1.3.1/tests/test_FeatureCollection.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Filter.py` & `geetools-1.3.1/tests/test_Filter.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Geometry.py` & `geetools-1.3.1/tests/test_Geometry.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image.py` & `geetools-1.3.1/tests/test_Image.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from urllib.request import urlretrieve
 
 import ee
 import numpy as np
 import pytest
+from jsonschema import validate
 
 import geetools
 
 
 class TestAddDate:
     """Test the ``addDate`` method."""
 
     def test_add_date(self, s2_sr_vatican_2020, vatican_buffer, num_regression):
         image = s2_sr_vatican_2020.geetools.addDate()
         values = image.reduceRegion(ee.Reducer.first(), vatican_buffer, 10)
         num_regression.check({k: np.nan if v is None else v for k, v in values.getInfo().items()})
 
+    def test_add_date_format(self, s2_sr_vatican_2020, vatican_buffer, num_regression):
+        image = s2_sr_vatican_2020.geetools.addDate("yyyyMMdd")
+        values = image.reduceRegion(ee.Reducer.first(), vatican_buffer, 10)
+        num_regression.check({k: np.nan if v is None else v for k, v in values.getInfo().items()})
+
     def test_deprecated_make_date_band(self, s2_sr_vatican_2020, vatican_buffer, num_regression):
         with pytest.deprecated_call():
             image = geetools.tools.date.makeDateBand(s2_sr_vatican_2020)
             values = image.reduceRegion(ee.Reducer.first(), vatican_buffer, 10)
             values = {k: np.nan if v is None else v for k, v in values.getInfo().items()}
             num_regression.check(values)
 
@@ -627,18 +633,21 @@
         values = image.reduceRegion(ee.Reducer.mean(), vatican_buffer, 10)
         num_regression.check(values.getInfo())
 
 
 class TestGetSTAC:
     """Test the ``getSTAC`` method."""
 
-    def test_get_stac(self, s2_sr_vatican_2020, data_regression):
+    def test_get_stac_schema(self, s2_sr_vatican_2020, stac_schema):
+        stac = s2_sr_vatican_2020.geetools.getSTAC()
+        validate(stac, stac_schema)
+
+    def test_get_stac(self, s2_sr_vatican_2020):
         stac = s2_sr_vatican_2020.geetools.getSTAC()
-        stac["extent"].pop("temporal")  # it will change all the time
-        data_regression.check(stac)
+        assert stac["id"] == "COPERNICUS/S2_SR_HARMONIZED"
 
 
 class TestGetDOI:
     """Test the ``getDOI`` method."""
 
     def get_doi(self, s2_sr_vatican_2020, data_regression):
         doi = s2_sr_vatican_2020.geetools.getDOI()
```

### Comparing `geetools-1.3.0/tests/test_ImageCollection.py` & `geetools-1.3.1/tests/test_ImageCollection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test the ImageCollection class."""
 from typing import Optional
 
 import ee
 import numpy as np
 import pytest
+from jsonschema import validate
 
 import geetools
 
 
 def reduce(collection: ee.ImageCollection, geometry: Optional[ee.Geometry] = None) -> ee.Dictionary:
     """Compute the mean reduction on the first image of the imageCollection."""
     first = collection.first()
@@ -72,18 +73,21 @@
         values = {k: np.nan if v is None else v for k, v in reduce(preprocessed).getInfo().items()}
         num_regression.check(values)
 
 
 class TestGetSTAC:
     """Test the ``getSTAC`` method."""
 
-    def test_get_stac(self, s2_sr, data_regression):
+    def test_get_stac(self, s2_sr):
         stac = s2_sr.geetools.getSTAC()
-        stac["extent"].pop("temporal")  # it will change all the time
-        data_regression.check(stac)
+        assert stac["id"] == "COPERNICUS/S2_SR"
+
+    def test_get_stac_schema(self, s2_sr, stac_schema):
+        stac = s2_sr.geetools.getSTAC()
+        validate(stac, stac_schema)
 
 
 class TestGetDOI:
     """Test the ``getDOI`` method."""
 
     def test_get_doi(self, s2_sr, data_regression):
         doi = s2_sr.geetools.getDOI()
@@ -210,8 +214,20 @@
 
 
 class TestToXarray:
     """Test the ``toXarray`` method."""
 
     def test_to_xarray(self, s2_sr, data_regression):
         ds = s2_sr.geetools.to_xarray()
+
+        # drop all the dtype as they are not consistently setup depending on the xarray version
+        def drop_dtype(d=ds):
+            for k, v in ds.items():
+                if isinstance(v, dict):
+                    drop_dtype(v)
+                elif k == "dtype":
+                    del ds[k]
+
+        drop_dtype()
+
+        # ds = ds.astype(np.float64)
         data_regression.check(ds.to_dict(data=False))
```

### Comparing `geetools-1.3.0/tests/test_Join.py` & `geetools-1.3.1/tests/test_Join.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_List.py` & `geetools-1.3.1/tests/test_List.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Number.py` & `geetools-1.3.1/tests/test_Number.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_String.py` & `geetools-1.3.1/tests/test_String.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the String class methods."""
+import ee
 import pytest
 
 import geetools
 
 
 class TestEq:
     """Test the eq method."""
@@ -25,12 +26,17 @@
     """test the format method."""
 
     def test_format_with_dictionary(self, format_string_instance):
         params = {"greeting": "Hello", "name": "bob"}
         formatted_string = format_string_instance.geetools.format(params)
         assert formatted_string.getInfo() == "Hello bob !"
 
+    def test_with_number(self, format_string_instance):
+        params = {"greeting": "Hello", "name": ee.Number(1)}
+        formatted_string = format_string_instance.geetools.format(params)
+        assert formatted_string.getInfo() == "Hello 1 !"
+
     def test_deprecated_format(self, format_string_instance):
         with pytest.deprecated_call():
             params = {"greeting": "Hello", "name": "bob"}
             formatted_string = geetools.string.format(format_string_instance, params)
             assert formatted_string.getInfo() == "Hello bob !"
```

### Comparing `geetools-1.3.0/tests/test_deprecated.py` & `geetools-1.3.1/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_by_features.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_by_features.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_by_features_with_id.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_by_features_with_id.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_by_properties.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_by_properties.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_by_properties_with_id.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_by_properties_with_id.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_deprecated_clean.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_deprecated_clean.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_deprecated_merge.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_deprecated_merge.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_merge_geometries.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_merge_geometries.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_bar.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_bar.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_donut.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_donut.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_pie.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_pie.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_scatter.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_scatter.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_features_stacked.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_features_stacked.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_properties_area.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_properties_area.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_properties_bar.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_properties_bar.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_by_properties_plot.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_by_properties_plot.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_plot_hist.png` & `geetools-1.3.1/tests/test_FeatureCollection/test_plot_hist.png`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_FeatureCollection/test_to_polygons.yml` & `geetools-1.3.1/tests/test_FeatureCollection/test_to_polygons.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Geometry/test_deprecated_polygon.yml` & `geetools-1.3.1/tests/test_Geometry/test_deprecated_polygon.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_clip_on_collection_property.yml` & `geetools-1.3.1/tests/test_Image/test_clip_on_collection_property.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_clip_on_collection_without_properties_property.yml` & `geetools-1.3.1/tests/test_Image/test_clip_on_collection_without_properties_property.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_default_spectral_indices.csv` & `geetools-1.3.1/tests/test_Image/test_default_spectral_indices.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_clip_to_collection_property.yml` & `geetools-1.3.1/tests/test_Image/test_deprecated_clip_to_collection_property.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_compute.csv` & `geetools-1.3.1/tests/test_Image/test_deprecated_compute.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_evi.csv` & `geetools-1.3.1/tests/test_Image/test_deprecated_evi.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_method.npz` & `geetools-1.3.1/tests/test_Image/test_deprecated_method.npz`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_nbr.csv` & `geetools-1.3.1/tests/test_Image/test_deprecated_nbr.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_nbr2.csv` & `geetools-1.3.1/tests/test_Image/test_deprecated_nbr2.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_ndfi.csv` & `geetools-1.3.1/tests/test_Image/test_deprecated_ndfi.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_ndvi.csv` & `geetools-1.3.1/tests/test_Image/test_deprecated_ndvi.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_deprecated_to_grid.npz` & `geetools-1.3.1/tests/test_Image/test_deprecated_to_grid.npz`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_mask_S2_clouds.csv` & `geetools-1.3.1/tests/test_Image/test_mask_S2_clouds.csv`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_merge.yml` & `geetools-1.3.1/tests/test_Image/test_merge.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_Image/test_remove_properties.yml` & `geetools-1.3.1/tests/test_Image/test_remove_properties.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+- MEAN_INCIDENCE_AZIMUTH_ANGLE_B8A
 - CLOUD_SHADOW_PERCENTAGE
 - MEAN_SOLAR_AZIMUTH_ANGLE
 - VEGETATION_PERCENTAGE
 - SOLAR_IRRADIANCE_B12
 - SOLAR_IRRADIANCE_B10
 - SENSOR_QUALITY
 - SOLAR_IRRADIANCE_B11
@@ -68,11 +69,11 @@
 - SOLAR_IRRADIANCE_B4
 - GEOMETRIC_QUALITY
 - SOLAR_IRRADIANCE_B3
 - WATER_PERCENTAGE
 - DATATAKE_IDENTIFIER
 - AOT_RETRIEVAL_ACCURACY
 - SPACECRAFT_NAME
+- system:footprint
 - SATURATED_DEFECTIVE_PIXEL_PERCENTAGE
-- MEAN_INCIDENCE_AZIMUTH_ANGLE_B8A
 - system:bands
 - system:band_names
```

### Comparing `geetools-1.3.0/tests/test_Image/test_to_grid.npz` & `geetools-1.3.1/tests/test_Image/test_to_grid.npz`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_ImageCollection/test_mask_s2.yml` & `geetools-1.3.1/tests/test_ImageCollection/test_mask_s2.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_ImageCollection/test_to_xarray.yml` & `geetools-1.3.1/tests/test_ImageCollection/test_to_xarray.yml`

 * *Files 2% similar despite different names*

```diff
@@ -199,22 +199,22 @@
   visualization_0_min: '0.0'
   visualization_0_name: RGB
 coords:
   lat:
     attrs: {}
     dims:
     - lat
-    dtype: float32
+    dtype: float64
     shape:
     - 180
   lon:
     attrs: {}
     dims:
     - lon
-    dtype: float32
+    dtype: float64
     shape:
     - 360
   time:
     attrs: {}
     dims:
     - time
     dtype: datetime64[ns]
@@ -237,15 +237,15 @@
       - 10980
       - 10980
       id: AOT
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B1:
     attrs:
       crs: EPSG:4326
@@ -262,15 +262,15 @@
       - 1830
       - 1830
       id: B1
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B11:
     attrs:
       crs: EPSG:4326
@@ -287,15 +287,15 @@
       - 5490
       - 5490
       id: B11
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B12:
     attrs:
       crs: EPSG:4326
@@ -312,15 +312,15 @@
       - 5490
       - 5490
       id: B12
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B2:
     attrs:
       crs: EPSG:4326
@@ -337,15 +337,15 @@
       - 10980
       - 10980
       id: B2
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B3:
     attrs:
       crs: EPSG:4326
@@ -362,15 +362,15 @@
       - 10980
       - 10980
       id: B3
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B4:
     attrs:
       crs: EPSG:4326
@@ -387,15 +387,15 @@
       - 10980
       - 10980
       id: B4
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B5:
     attrs:
       crs: EPSG:4326
@@ -412,15 +412,15 @@
       - 5490
       - 5490
       id: B5
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B6:
     attrs:
       crs: EPSG:4326
@@ -437,15 +437,15 @@
       - 5490
       - 5490
       id: B6
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B7:
     attrs:
       crs: EPSG:4326
@@ -462,15 +462,15 @@
       - 5490
       - 5490
       id: B7
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B8:
     attrs:
       crs: EPSG:4326
@@ -487,15 +487,15 @@
       - 10980
       - 10980
       id: B8
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B8A:
     attrs:
       crs: EPSG:4326
@@ -512,15 +512,15 @@
       - 5490
       - 5490
       id: B8A
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   B9:
     attrs:
       crs: EPSG:4326
@@ -537,15 +537,15 @@
       - 1830
       - 1830
       id: B9
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   MSK_CLDPRB:
     attrs:
       crs: EPSG:4326
@@ -562,15 +562,15 @@
       - 5490
       - 5490
       id: MSK_CLDPRB
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   MSK_SNWPRB:
     attrs:
       crs: EPSG:4326
@@ -587,15 +587,15 @@
       - 5490
       - 5490
       id: MSK_SNWPRB
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   QA10:
     attrs:
       crs: EPSG:4326
@@ -612,15 +612,15 @@
       - 10980
       - 10980
       id: QA10
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   QA20:
     attrs:
       crs: EPSG:4326
@@ -637,15 +637,15 @@
       - 5490
       - 5490
       id: QA20
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   QA60:
     attrs:
       crs: EPSG:4326
@@ -662,15 +662,15 @@
       - 1830
       - 1830
       id: QA60
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   SCL:
     attrs:
       crs: EPSG:4326
@@ -687,15 +687,15 @@
       - 5490
       - 5490
       id: SCL
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   TCI_B:
     attrs:
       crs: EPSG:4326
@@ -712,15 +712,15 @@
       - 10980
       - 10980
       id: TCI_B
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   TCI_G:
     attrs:
       crs: EPSG:4326
@@ -737,15 +737,15 @@
       - 10980
       - 10980
       id: TCI_G
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   TCI_R:
     attrs:
       crs: EPSG:4326
@@ -762,15 +762,15 @@
       - 10980
       - 10980
       id: TCI_R
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
   WVP:
     attrs:
       crs: EPSG:4326
@@ -787,15 +787,15 @@
       - 10980
       - 10980
       id: WVP
     dims:
     - time
     - lon
     - lat
-    dtype: int32
+    dtype: float32
     shape:
     - 2449
     - 360
     - 180
 dims:
   lat: 180
   lon: 360
```

#### html2text {}

```diff
@@ -293,91 +293,92 @@
 sentinel-2-msi/product-types/level-2a sample: https://mw1.google.com/ges/dd/
 images/COPERNICUS_S2_SR_sample.png source_tags: - eu - esa - copernicus -
 sentinel tags: - copernicus - esa - eu - msi - reflectance - sentinel - sr
 thumb: https://mw1.google.com/ges/dd/images/COPERNICUS_S2_SR_thumb.png title:
 'Sentinel-2 MSI: MultiSpectral Instrument, Level-2A' type_name: ImageCollection
 visualization_0_bands: B4,B3,B2 visualization_0_max: '3000.0'
 visualization_0_min: '0.0' visualization_0_name: RGB coords: lat: attrs: {}
-dims: - lat dtype: float32 shape: - 180 lon: attrs: {} dims: - lon dtype:
-float32 shape: - 360 time: attrs: {} dims: - time dtype: datetime64[ns] shape:
+dims: - lat dtype: float64 shape: - 180 lon: attrs: {} dims: - lon dtype:
+float64 shape: - 360 time: attrs: {} dims: - time dtype: datetime64[ns] shape:
 - 2449 data_vars: AOT: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 -
 0 - -10 - 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
 ''min'': 0, ''max'': 65535}' dimensions: - 10980 - 10980 id: AOT dims: - time -
-lon - lat dtype: int32 shape: - 2449 - 360 - 180 B1: attrs: crs: EPSG:4326
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 B1: attrs: crs: EPSG:4326
 crs_transform: - 60 - 0 - 699960 - 0 - -60 - 9800020 data_type: '{''type'':
 ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
-- 1830 - 1830 id: B1 dims: - time - lon - lat dtype: int32 shape: - 2449 - 360
-- 180 B11: attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960 - 0 - -20 -
-9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'':
-0, ''max'': 65535}' dimensions: - 5490 - 5490 id: B11 dims: - time - lon - lat
-dtype: int32 shape: - 2449 - 360 - 180 B12: attrs: crs: EPSG:4326
+- 1830 - 1830 id: B1 dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 B11: attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960 - 0 - -20
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 5490 - 5490 id: B11 dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 B12: attrs: crs: EPSG:4326
 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'':
 ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
-- 5490 - 5490 id: B12 dims: - time - lon - lat dtype: int32 shape: - 2449 - 360
-- 180 B2: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10 -
-9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'':
-0, ''max'': 65535}' dimensions: - 10980 - 10980 id: B2 dims: - time - lon - lat
-dtype: int32 shape: - 2449 - 360 - 180 B3: attrs: crs: EPSG:4326 crs_transform:
-- 10 - 0 - 699960 - 0 - -10 - 9800020 data_type: '{''type'': ''PixelType'',
-''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions: - 10980 -
-10980 id: B3 dims: - time - lon - lat dtype: int32 shape: - 2449 - 360 - 180
-B4: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020
-data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0,
-''max'': 65535}' dimensions: - 10980 - 10980 id: B4 dims: - time - lon - lat
-dtype: int32 shape: - 2449 - 360 - 180 B5: attrs: crs: EPSG:4326 crs_transform:
-- 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'': ''PixelType'',
-''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions: - 5490 - 5490
-id: B5 dims: - time - lon - lat dtype: int32 shape: - 2449 - 360 - 180 B6:
-attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020
-data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0,
-''max'': 65535}' dimensions: - 5490 - 5490 id: B6 dims: - time - lon - lat
-dtype: int32 shape: - 2449 - 360 - 180 B7: attrs: crs: EPSG:4326 crs_transform:
-- 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'': ''PixelType'',
-''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions: - 5490 - 5490
-id: B7 dims: - time - lon - lat dtype: int32 shape: - 2449 - 360 - 180 B8:
-attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020
-data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0,
-''max'': 65535}' dimensions: - 10980 - 10980 id: B8 dims: - time - lon - lat
-dtype: int32 shape: - 2449 - 360 - 180 B8A: attrs: crs: EPSG:4326
+- 5490 - 5490 id: B12 dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 B2: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 10980 - 10980 id: B2 dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 B3: attrs: crs: EPSG:4326
+crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020 data_type: '{''type'':
+''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
+- 10980 - 10980 id: B3 dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 B4: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 10980 - 10980 id: B4 dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 B5: attrs: crs: EPSG:4326
 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'':
 ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
-- 5490 - 5490 id: B8A dims: - time - lon - lat dtype: int32 shape: - 2449 - 360
-- 180 B9: attrs: crs: EPSG:4326 crs_transform: - 60 - 0 - 699960 - 0 - -60 -
-9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'':
-0, ''max'': 65535}' dimensions: - 1830 - 1830 id: B9 dims: - time - lon - lat
-dtype: int32 shape: - 2449 - 360 - 180 MSK_CLDPRB: attrs: crs: EPSG:4326
+- 5490 - 5490 id: B5 dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 B6: attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960 - 0 - -20
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 5490 - 5490 id: B6 dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 B7: attrs: crs: EPSG:4326
 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'':
-''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 255}' dimensions: -
-5490 - 5490 id: MSK_CLDPRB dims: - time - lon - lat dtype: int32 shape: - 2449
-- 360 - 180 MSK_SNWPRB: attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960
-- 0 - -20 - 9800020 data_type: '{''type'': ''PixelType'', ''precision'':
-''int'', ''min'': 0, ''max'': 255}' dimensions: - 5490 - 5490 id: MSK_SNWPRB
-dims: - time - lon - lat dtype: int32 shape: - 2449 - 360 - 180 QA10: attrs:
-crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020 data_type:
-'{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}'
-dimensions: - 10980 - 10980 id: QA10 dims: - time - lon - lat dtype: int32
-shape: - 2449 - 360 - 180 QA20: attrs: crs: EPSG:4326 crs_transform: - 20 - 0 -
-699960 - 0 - -20 - 9800020 data_type: '{''type'': ''PixelType'', ''precision'':
-''int'', ''min'': 0, ''max'': 4294967295}' dimensions: - 5490 - 5490 id: QA20
-dims: - time - lon - lat dtype: int32 shape: - 2449 - 360 - 180 QA60: attrs:
-crs: EPSG:4326 crs_transform: - 60 - 0 - 699960 - 0 - -60 - 9800020 data_type:
-'{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}'
-dimensions: - 1830 - 1830 id: QA60 dims: - time - lon - lat dtype: int32 shape:
-- 2449 - 360 - 180 SCL: attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960
-- 0 - -20 - 9800020 data_type: '{''type'': ''PixelType'', ''precision'':
-''int'', ''min'': 0, ''max'': 255}' dimensions: - 5490 - 5490 id: SCL dims: -
-time - lon - lat dtype: int32 shape: - 2449 - 360 - 180 TCI_B: attrs: crs:
-EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020 data_type: '
+''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
+- 5490 - 5490 id: B7 dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 B8: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 10980 - 10980 id: B8 dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 B8A: attrs: crs: EPSG:4326
+crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'':
+''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
+- 5490 - 5490 id: B8A dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 B9: attrs: crs: EPSG:4326 crs_transform: - 60 - 0 - 699960 - 0 - -60
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 1830 - 1830 id: B9 dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 MSK_CLDPRB: attrs: crs:
+EPSG:4326 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '
 {''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 255}'
-dimensions: - 10980 - 10980 id: TCI_B dims: - time - lon - lat dtype: int32
-shape: - 2449 - 360 - 180 TCI_G: attrs: crs: EPSG:4326 crs_transform: - 10 - 0
-- 699960 - 0 - -10 - 9800020 data_type: '{''type'': ''PixelType'',
-''precision'': ''int'', ''min'': 0, ''max'': 255}' dimensions: - 10980 - 10980
-id: TCI_G dims: - time - lon - lat dtype: int32 shape: - 2449 - 360 - 180
-TCI_R: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10 -
-9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'':
-0, ''max'': 255}' dimensions: - 10980 - 10980 id: TCI_R dims: - time - lon -
-lat dtype: int32 shape: - 2449 - 360 - 180 WVP: attrs: crs: EPSG:4326
+dimensions: - 5490 - 5490 id: MSK_CLDPRB dims: - time - lon - lat dtype:
+float32 shape: - 2449 - 360 - 180 MSK_SNWPRB: attrs: crs: EPSG:4326
+crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '{''type'':
+''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 255}' dimensions: -
+5490 - 5490 id: MSK_SNWPRB dims: - time - lon - lat dtype: float32 shape: -
+2449 - 360 - 180 QA10: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 -
+0 - -10 - 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 10980 - 10980 id: QA10 dims: - time
+- lon - lat dtype: float32 shape: - 2449 - 360 - 180 QA20: attrs: crs: EPSG:
+4326 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020 data_type: '
+{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'':
+4294967295}' dimensions: - 5490 - 5490 id: QA20 dims: - time - lon - lat dtype:
+float32 shape: - 2449 - 360 - 180 QA60: attrs: crs: EPSG:4326 crs_transform: -
+60 - 0 - 699960 - 0 - -60 - 9800020 data_type: '{''type'': ''PixelType'',
+''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions: - 1830 - 1830
+id: QA60 dims: - time - lon - lat dtype: float32 shape: - 2449 - 360 - 180 SCL:
+attrs: crs: EPSG:4326 crs_transform: - 20 - 0 - 699960 - 0 - -20 - 9800020
+data_type: '{''type'': ''PixelType'', ''precision'': ''int'', ''min'': 0,
+''max'': 255}' dimensions: - 5490 - 5490 id: SCL dims: - time - lon - lat
+dtype: float32 shape: - 2449 - 360 - 180 TCI_B: attrs: crs: EPSG:4326
 crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020 data_type: '{''type'':
-''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 65535}' dimensions:
-- 10980 - 10980 id: WVP dims: - time - lon - lat dtype: int32 shape: - 2449 -
-360 - 180 dims: lat: 180 lon: 360 time: 2449
+''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 255}' dimensions: -
+10980 - 10980 id: TCI_B dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 TCI_G: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -
+10 - 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 255}' dimensions: - 10980 - 10980 id: TCI_G dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 TCI_R: attrs: crs: EPSG:4326
+crs_transform: - 10 - 0 - 699960 - 0 - -10 - 9800020 data_type: '{''type'':
+''PixelType'', ''precision'': ''int'', ''min'': 0, ''max'': 255}' dimensions: -
+10980 - 10980 id: TCI_R dims: - time - lon - lat dtype: float32 shape: - 2449 -
+360 - 180 WVP: attrs: crs: EPSG:4326 crs_transform: - 10 - 0 - 699960 - 0 - -10
+- 9800020 data_type: '{''type'': ''PixelType'', ''precision'': ''int'',
+''min'': 0, ''max'': 65535}' dimensions: - 10980 - 10980 id: WVP dims: - time -
+lon - lat dtype: float32 shape: - 2449 - 360 - 180 dims: lat: 180 lon: 360
+time: 2449
```

### Comparing `geetools-1.3.0/tests/test_deprecated/test_merge_geometry.yml` & `geetools-1.3.1/tests/test_deprecated/test_merge_geometry.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/tests/test_deprecated/test_tobands.yml` & `geetools-1.3.1/tests/test_deprecated/test_tobands.yml`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/.gitignore` & `geetools-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/AUTHORS.rst` & `geetools-1.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/LICENSE` & `geetools-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/README.rst` & `geetools-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `geetools-1.3.0/pyproject.toml` & `geetools-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geetools"
-version = "1.3.0"
+version = "1.3.1"
 description = "A collection of tools to work with Google Earth Engine Python API"
 keywords = [
   "python",
   "geospatial",
   "remote-sensing",
   "google-earth-engine",
   "earthengine",
@@ -20,23 +20,24 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "earthengine-api",
+    "earthengine-api>=0.1.397", # support for ee.data.createFolder
     "requests",
     "pandas",
     "geopandas",
     "deprecated",
     "ee-extra",
-    "xee",
+    "xee>=0.0.11", # xee change dtype management
     "yamlable",
     "matplotlib",
+    "anyascii",
 ]
 
 [[project.authors]]
 name = "Rodrigo E. Principe"
 email = "fitoprincipe82@gmail.com"
 
 [project.license]
@@ -60,21 +61,22 @@
     "pytest-sugar",
     "pytest-cov",
     "pytest-deadfixtures",
     "httplib2",
     "pytest-regressions",
     "Pillow",
     "pytest-gee",
+    "jsonschema",
 ]
 doc = [
   "sphinx>=6.2.1",
   "pydata-sphinx-theme",
   "sphinx-copybutton",
   "sphinx-design",
-  "sphinx-autoapi",
+  "sphinx-autoapi==3.1.0a3",  # until v3.1 is released with the single page fix
   "ipykernel",
   "httplib2",
   "jupyter-sphinx",
   "nbsphinx",
 ]
 
 [tool.hatch.build.targets.wheel]
@@ -118,15 +120,15 @@
 [tool.coverage.run]
 source = ["geetools"]
 branch = true
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "1.3.0"
+version = "1.3.1"
 version_files = [
     "pyproject.toml:version",
     "geetools/__init__.py:__version__",
     "docs/conf.py:release",
 ]
 
 [tool.codespell]
```

### Comparing `geetools-1.3.0/PKG-INFO` & `geetools-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: geetools
-Version: 1.3.0
+Version: 1.3.1
 Summary: A collection of tools to work with Google Earth Engine Python API
 Project-URL: Homepage, https://github.com/gee-community/geetools
 Author-email: "Rodrigo E. Principe" <fitoprincipe82@gmail.com>
 License: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: earthengine,geospatial,google-earth-engine,python,remote-sensing
@@ -12,39 +12,41 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.9
+Requires-Dist: anyascii
 Requires-Dist: deprecated
-Requires-Dist: earthengine-api
+Requires-Dist: earthengine-api>=0.1.397
 Requires-Dist: ee-extra
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: requests
-Requires-Dist: xee
+Requires-Dist: xee>=0.0.11
 Requires-Dist: yamlable
 Provides-Extra: dev
 Requires-Dist: commitizen; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: httplib2; extra == 'doc'
 Requires-Dist: ipykernel; extra == 'doc'
 Requires-Dist: jupyter-sphinx; extra == 'doc'
 Requires-Dist: nbsphinx; extra == 'doc'
 Requires-Dist: pydata-sphinx-theme; extra == 'doc'
-Requires-Dist: sphinx-autoapi; extra == 'doc'
+Requires-Dist: sphinx-autoapi==3.1.0a3; extra == 'doc'
 Requires-Dist: sphinx-copybutton; extra == 'doc'
 Requires-Dist: sphinx-design; extra == 'doc'
 Requires-Dist: sphinx>=6.2.1; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: httplib2; extra == 'test'
+Requires-Dist: jsonschema; extra == 'test'
 Requires-Dist: pillow; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-deadfixtures; extra == 'test'
 Requires-Dist: pytest-gee; extra == 'test'
 Requires-Dist: pytest-regressions; extra == 'test'
 Requires-Dist: pytest-sugar; extra == 'test'
```

