# Comparing `tmp/nrtk_explorer-0.2.0.tar.gz` & `tmp/nrtk_explorer-0.2.1.tar.gz`

## Comparing `nrtk_explorer-0.2.0.tar` & `nrtk_explorer-0.2.1.tar`

### file list

```diff
@@ -1,118 +1,119 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.codespellrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.flake8
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/screenshot.png
--rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/usage.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.github/workflows/create_release.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/README.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/create_exe.bat
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/create_linux.sh
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/create_mac.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/requirements.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/run.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/DEPLOY.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/Dockerfile
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/captain-definition
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/build_image.sh
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/build_server.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/run_image.sh
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/run_server.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/setup/apps.yml
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/setup/initialize.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/setup/requirements.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/examples/jupyter/show.ipynb
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/applet.py
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/core.py
--rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/embeddings.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/filtering.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/jupyter.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/main.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/parameters.py
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/quasar.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify2.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify3.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/collapsible_card.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/image_list.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/layout.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/result_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/dataset.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/dimension_reducers.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/embeddings_extractor.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/filtering.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/images_manager.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/ml_models.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/nrtk_transforms.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/object_detector.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/transforms.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/assets/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/assets/imagenet_classes.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/__init__.py
--rw-r--r--   0        0        0   725513 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/serve/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/__init__.py
--rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
--rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
--rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
--rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
--rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
--rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
--rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
--rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
--rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
--rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
--rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
--rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
--rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
--rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
--rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
--rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
--rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/widgets/__init__.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/widgets/nrtk_explorer.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/requirements.txt
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_embeddings.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_filtering.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_import.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_object_detector.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.editorconfig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.eslintrc.cjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.prettierrc.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/env.d.ts
--rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/package-lock.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/tsconfig.app.json
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/tsconfig.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/tsconfig.node.json
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/vite.config.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/public/styles.css
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/main.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/FilterOperatorWidget.vue
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/FilterOptionsWidget.vue
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ImageDetection.vue
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ParamWidget.vue
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ParamsWidget.vue
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ScatterPlot.vue
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/index.js
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/types/index.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/utilities/colors.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/LICENSE
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/hatch_build.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.codespellrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.flake8
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29029 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/MANIFEST.in
+-rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/screenshot.png
+-rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/usage.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/workflows/create_release.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.github/workflows/push_to_release.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/create_exe.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/create_linux.sh
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/create_mac.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/desktop/run.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/DEPLOY.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/Dockerfile
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/captain-definition
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/build_image.sh
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/build_server.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/run_image.sh
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/scripts/run_server.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/setup/apps.yml
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/setup/initialize.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/bundles/docker/setup/requirements.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/examples/jupyter/show.ipynb
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/applet.py
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/core.py
+-rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/embeddings.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/filtering.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/jupyter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/main.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/parameters.py
+-rw-r--r--   0        0        0    16333 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/quasar.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify2.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify3.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/collapsible_card.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/image_list.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/layout.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/result_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/dataset.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/dimension_reducers.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/embeddings_extractor.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/filtering.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/images_manager.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/ml_models.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/nrtk_transforms.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/object_detector.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/transforms.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/assets/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/library/assets/imagenet_classes.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/__init__.py
+-rw-r--r--   0        0        0   725513 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/module/serve/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/__init__.py
+-rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
+-rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
+-rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
+-rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
+-rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
+-rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
+-rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
+-rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
+-rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
+-rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
+-rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
+-rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
+-rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
+-rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
+-rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
+-rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
+-rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/widgets/__init__.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/src/nrtk_explorer/widgets/nrtk_explorer.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/requirements.txt
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_embeddings.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_filtering.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_import.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/tests/test_object_detector.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.editorconfig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.eslintrc.cjs
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/.prettierrc.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/env.d.ts
+-rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/package-lock.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/tsconfig.app.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/tsconfig.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/tsconfig.node.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/vite.config.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/public/styles.css
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/main.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/FilterOperatorWidget.vue
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/FilterOptionsWidget.vue
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ImageDetection.vue
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ParamWidget.vue
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ParamsWidget.vue
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/ScatterPlot.vue
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/components/index.js
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/types/index.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/vue-components/src/utilities/colors.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/hatch_build.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.1/PKG-INFO
```

### Comparing `nrtk_explorer-0.2.0/CHANGELOG.md` & `nrtk_explorer-0.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # CHANGELOG
 
 
 
+## v0.2.1 (2024-05-21)
+
+### Ci
+
+* ci: create_release only in release branch ([`d07bdf4`](https://github.com/Kitware/nrtk-explorer/commit/d07bdf4ad712a8a2936782b1fab8a934858cedd3))
+
+### Fix
+
+* fix: gracefully disable nrtk transform if we have import error ([`05efbcc`](https://github.com/Kitware/nrtk-explorer/commit/05efbccf345d43b02aa86bb6ba978a77a1f65135))
+
+### Unknown
+
+* Update create_release.yaml ([`73f6e97`](https://github.com/Kitware/nrtk-explorer/commit/73f6e9784552588e7e36919bfda72f77df10b324))
+
+* Merge main to release ([`511736c`](https://github.com/Kitware/nrtk-explorer/commit/511736c5cdaea66704001f3a327b744fe844adeb))
+
+* Auto-merge release back to main ([`facc6aa`](https://github.com/Kitware/nrtk-explorer/commit/facc6aafee5b1ff17e178ea7151fb46fec407056))
+
+
 ## v0.2.0 (2024-05-16)
 
 ### Ci
 
 * ci: fixture in semantic release script ([`5ce57e5`](https://github.com/Kitware/nrtk-explorer/commit/5ce57e57b18eb0c77677dc61694d6a3f52588c9e))
 
 ### Feature
```

### Comparing `nrtk_explorer-0.2.0/CONTRIBUTING.rst` & `nrtk_explorer-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/screenshot.png` & `nrtk_explorer-0.2.1/screenshot.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/usage.png` & `nrtk_explorer-0.2.1/usage.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/.github/workflows/ci.yml` & `nrtk_explorer-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/bundles/desktop/README.md` & `nrtk_explorer-0.2.1/bundles/desktop/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/bundles/docker/DEPLOY.md` & `nrtk_explorer-0.2.1/bundles/docker/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/bundles/docker/README.md` & `nrtk_explorer-0.2.1/bundles/docker/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/examples/jupyter/show.ipynb` & `nrtk_explorer-0.2.1/examples/jupyter/show.ipynb`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/applet.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/applet.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/core.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/core.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/embeddings.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/filtering.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/jupyter.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/parameters.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/parameters.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/transforms.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,18 +77,20 @@
         self.state.feature_extraction_model = self.state.models[0]
 
         self._transforms: Dict[str, trans.ImageTransform] = {
             "identity": trans.IdentityTransform(),
             "blur": trans.GaussianBlurTransform(),
             "invert": trans.InvertTransform(),
             "downsample": trans.DownSampleTransform(),
-            "nrtk_blur": nrtk_trans.NrtkGaussianBlurTransform(),
-            "nrtk_pybsm": nrtk_trans.NrtkPybsmTransform(),
         }
 
+        if nrtk_trans.nrtk_transforms_available():
+            self._transforms["nrtk_blur"] = nrtk_trans.NrtkGaussianBlurTransform()
+            self._transforms["nrtk_pybsm"] = nrtk_trans.NrtkPybsmTransform()
+
         self._parameters_app._transforms = self._transforms
 
         self.state.annotation_categories = {}
 
         self.state.source_image_ids = []
         self.state.transformed_image_ids = []
         self.state.transforms = [k for k in self._transforms.keys()]
```

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/quasar.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/quasar.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify2.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify2.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify3.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/test/vuetify3.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/collapsible_card.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/collapsible_card.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/image_list.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/image_list.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/layout.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/app/ui/layout.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/dimension_reducers.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/dimension_reducers.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/embeddings_extractor.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/embeddings_extractor.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/filtering.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/images_manager.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/images_manager.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/ml_models.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/ml_models.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/nrtk_transforms.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/nrtk_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,35 @@
-from typing import Any, Optional, Dict, Tuple
+from typing import Any, Dict
 
 import numpy as np
+import logging
 from PIL import Image as ImageModule
 from PIL.Image import Image
-from pybsm.otf import darkCurrentFromDensity
-from nrtk.impls.perturb_image.generic.cv2.blur import GaussianBlurPerturber
-from nrtk.impls.perturb_image.pybsm.perturber import PybsmPerturber, PybsmSensor, PybsmScenario
-
 from nrtk_explorer.library.transforms import ImageTransform, ParameterDescription
 
+ENABLED_NRTK_TRANSFORMS = True
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
+try:
+    from pybsm.otf import darkCurrentFromDensity
+    from nrtk.impls.perturb_image.generic.cv2.blur import GaussianBlurPerturber
+    from nrtk.impls.perturb_image.pybsm.perturber import PybsmPerturber, PybsmSensor, PybsmScenario
+except ImportError:
+    logger.info("Disabling NRTK transforms due to missing library/failing imports")
+    ENABLED_NRTK_TRANSFORMS = False
+
+
+def nrtk_transforms_available():
+    return ENABLED_NRTK_TRANSFORMS
+
 
 class NrtkGaussianBlurTransform(ImageTransform):
-    def __init__(self, perturber: Optional[GaussianBlurPerturber] = None):
+    def __init__(self, perturber=None):
         if perturber is None:
             perturber = GaussianBlurPerturber()
 
         self._perturber: GaussianBlurPerturber = perturber
 
     def get_parameters(self) -> Dict[str, Any]:
         return {
@@ -43,15 +57,15 @@
         output_array = self._perturber.perturb(input_array)
 
         return ImageModule.fromarray(output_array)
 
 
 # Taken from the nrtk package tests
 # https://github.com/Kitware/nrtk/blob/main/tests/impls/perturb_image/pybsm/test_pybsm_pertuber.py#L21
-def createSampleSensorAndScenario() -> Tuple[PybsmSensor, PybsmScenario]:
+def createSampleSensorAndScenario():
 
     name = "L32511x"
 
     # telescope focal length (m)
     f = 4
     # Telescope diameter (m)
     D = 275e-3
@@ -137,15 +151,15 @@
     scenario = PybsmScenario(scenario_name, ihaze, altitude, groundRange)
     scenario.aircraftSpeed = 100.0
 
     return sensor, scenario
 
 
 class NrtkPybsmTransform(ImageTransform):
-    def __init__(self, perturber: Optional[PybsmPerturber] = None):
+    def __init__(self, perturber=None):
         if perturber is None:
             sensor, scenario = createSampleSensorAndScenario()
             perturber = PybsmPerturber(sensor=sensor, scenario=scenario)
 
         self._perturber: PybsmPerturber = perturber
 
     def get_parameters(self) -> dict[str, Any]:
```

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/object_detector.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/transforms.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/library/assets/imagenet_classes.txt` & `nrtk_explorer-0.2.1/src/nrtk_explorer/library/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js` & `nrtk_explorer-0.2.1/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json` & `nrtk_explorer-0.2.1/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/src/nrtk_explorer/widgets/nrtk_explorer.py` & `nrtk_explorer-0.2.1/src/nrtk_explorer/widgets/nrtk_explorer.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/tests/conftest.py` & `nrtk_explorer-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/tests/test_embeddings.py` & `nrtk_explorer-0.2.1/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/tests/test_filtering.py` & `nrtk_explorer-0.2.1/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/tests/test_object_detector.py` & `nrtk_explorer-0.2.1/tests/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/package-lock.json` & `nrtk_explorer-0.2.1/vue-components/package-lock.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/package.json` & `nrtk_explorer-0.2.1/vue-components/package.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/vite.config.ts` & `nrtk_explorer-0.2.1/vue-components/vite.config.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/components/FilterOperatorWidget.vue` & `nrtk_explorer-0.2.1/vue-components/src/components/FilterOperatorWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/components/FilterOptionsWidget.vue` & `nrtk_explorer-0.2.1/vue-components/src/components/FilterOptionsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/components/ImageDetection.vue` & `nrtk_explorer-0.2.1/vue-components/src/components/ImageDetection.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/components/ParamWidget.vue` & `nrtk_explorer-0.2.1/vue-components/src/components/ParamWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/components/ParamsWidget.vue` & `nrtk_explorer-0.2.1/vue-components/src/components/ParamsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/components/ScatterPlot.vue` & `nrtk_explorer-0.2.1/vue-components/src/components/ScatterPlot.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/types/index.ts` & `nrtk_explorer-0.2.1/vue-components/src/types/index.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/vue-components/src/utilities/colors.ts` & `nrtk_explorer-0.2.1/vue-components/src/utilities/colors.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/LICENSE` & `nrtk_explorer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/README.md` & `nrtk_explorer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/hatch_build.py` & `nrtk_explorer-0.2.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.2.0/pyproject.toml` & `nrtk_explorer-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nrtk-explorer"
-version="0.2.0"
+version="0.2.1"
 description="Model Visualizer"
 authors = [
   {name = "Alessandro Genova", email = "alessandro.genova@kitware.com"},
   {name = "Vicente Adolfo Bolea Sanchez", email = "vicente.bolea@kitware.com"},
 ]
 readme = "README.md"
 keywords = [
```

### Comparing `nrtk_explorer-0.2.0/PKG-INFO` & `nrtk_explorer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nrtk-explorer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Model Visualizer
 Author-email: Alessandro Genova <alessandro.genova@kitware.com>, Vicente Adolfo Bolea Sanchez <vicente.bolea@kitware.com>
 License-File: LICENSE
 Keywords: Application,Framework,Interactive,Python,Web
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: Other/Proprietary License
```

