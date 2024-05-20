# Comparing `tmp/rio_ui-0.7.4.tar.gz` & `tmp/rio_ui-0.7.5.tar.gz`

## Comparing `rio_ui-0.7.4.tar` & `rio_ui-0.7.5.tar`

### file list

```diff
@@ -1,382 +1,382 @@
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.prettierrc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.sassrc
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.7.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 rio_ui-0.7.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.7.4/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 rio_ui-0.7.4/changelog.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 rio_ui-0.7.4/debug.log
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.7.4/package.json
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.7.4/vite.config.js
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.github/DISCUSSION_TEMPLATE/feature-requests.yml
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/index.html
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/layouting.ts
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/rippleEffect.ts
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/utils.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/button.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/card.ts
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/codeBlock.ts
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/debuggerConnector.ts
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/html.ts
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/code/components/website.ts
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/css/style.scss
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.7.4/frontend/css/switcheroos.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.7.4/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/__main__.py
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/app.py
--rw-r--r--   0        0        0    32919 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/app_server.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/byte_serving.py
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/color.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cursor_style.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/dataclass.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/errors.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/event.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/global_state.py
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/icon_registry.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/inspection.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/py.typed
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/self_serializing.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/serialization.py
--rw-r--r--   0        0        0    80113 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/session.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/session_attachments.py
--rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/state_properties.py
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/testing.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/text_style.py
--rw-r--r--   0        0        0    28614 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/theme.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/user_settings_module.py
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/utils.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/world_units.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/hosted/README.md
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/project.py
--rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    22822 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/app_root.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/auto_form.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/banner.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/build_failed.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/button.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/card.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/class_container.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/code_block.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/code_explorer.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/color_picker.py
--rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/component.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/component_tree.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/devel_component.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/drawer.py
--rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/dropdown.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/flow_container.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/grid.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/html.py
--rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/icon.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/image.py
--rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/labeled_column.py
--rw-r--r--   0        0        0    10697 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/linear_containers.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/link.py
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/list_items.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/list_view.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/markdown.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/media_player.py
--rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/node_input.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/node_output.py
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/number_input.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/overlay.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/page_view.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/plot.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/popup.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/progress_circle.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/rectangle.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/revealer.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/root_components.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/separator.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/slider.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/slideshow.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/spacer.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/stack.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/switch.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/switcher.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/table.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/text.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/text_input.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/tooltip.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/__init__.py
--rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/component_details.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/deploy_page.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/dev_tools_sidebar.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/docs_page.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/icons_page.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/project_page.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/sample_icons_grid.py
--rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/debug/dev_tools/tree_page.py
--rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/docs/__init__.py
--rw-r--r--   0        0        0   416487 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/generated/index.html
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/README.md
--rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/core-classes.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/debugging-setup.md
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/deployment.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-custom-events.md
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-install.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/persistent-settings.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/project-setup.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/run-project.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos/theming.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/custom-events.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/force-refresh.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/layouting.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/README.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
--rw-r--r--   0        0        0   208005 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/README.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/data_models.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/meta.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/root_init.py
--rw-r--r--   0        0        0   117987 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.7.4/scripts/benchmark.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.7.4/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.7.4/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.7.4/scripts/code_coverage.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.7.4/scripts/publish_new_release.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_app_build.py
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_attribute_bindings.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_custom_components.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_documentation.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_project_templates.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_reconciliation.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_refresh.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_session.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_testing_tools.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_user_settings.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.4/tests/utils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.7.4/.gitignore
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.7.4/LICENSE.txt
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.7.4/README.md
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 rio_ui-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    22714 2020-02-02 00:00:00.000000 rio_ui-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.sassrc
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.7.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 rio_ui-0.7.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.7.5/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 rio_ui-0.7.5/changelog.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 rio_ui-0.7.5/debug.log
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.7.5/package.json
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.7.5/vite.config.js
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.github/DISCUSSION_TEMPLATE/feature-requests.yml
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/index.html
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/codeBlock.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/debuggerConnector.ts
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/code/components/website.ts
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.7.5/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.7.5/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/__main__.py
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/app.py
+-rw-r--r--   0        0        0    33608 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/app_server.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/byte_serving.py
+-rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/color.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cursor_style.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/dataclass.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/errors.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/event.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/global_state.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/inspection.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/py.typed
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/self_serializing.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/serialization.py
+-rw-r--r--   0        0        0    80195 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/session.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/session_attachments.py
+-rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/state_properties.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/testing.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/text_style.py
+-rw-r--r--   0        0        0    28614 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/theme.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/user_settings_module.py
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/utils.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/world_units.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/project.py
+-rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22444 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/app_root.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/banner.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/build_failed.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/button.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/card.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/class_container.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/code_block.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/component.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/drawer.py
+-rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/grid.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/html.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/icon.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/image.py
+-rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/labeled_column.py
+-rw-r--r--   0        0        0    10697 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/link.py
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/list_items.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/list_view.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/markdown.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/media_player.py
+-rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/node_output.py
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/number_input.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/overlay.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/page_view.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/plot.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/popup.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/rectangle.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/revealer.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/root_components.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/separator.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/slider.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/spacer.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/stack.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/switch.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/switcher.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/table.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/text.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/text_input.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/tooltip.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/__init__.py
+-rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/component_details.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/deploy_page.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/dev_tools_sidebar.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/icons_page.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/sample_icons_grid.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/debug/dev_tools/tree_page.py
+-rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/docs/__init__.py
+-rw-r--r--   0        0        0   416604 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/generated/index.html
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/README.md
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/README.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
+-rw-r--r--   0        0        0   208005 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/README.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/data_models.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/meta.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/root_init.py
+-rw-r--r--   0        0        0   117987 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.7.5/scripts/benchmark.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.7.5/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.7.5/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.7.5/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.7.5/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_app_build.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_documentation.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_project_templates.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_refresh.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_session.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_testing_tools.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_user_settings.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.5/tests/utils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.7.5/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.7.5/LICENSE.txt
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.7.5/README.md
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 rio_ui-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 rio_ui-0.7.5/PKG-INFO
```

### Comparing `rio_ui-0.7.4/CODE_OF_CONDUCT.md` & `rio_ui-0.7.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/CONTRIBUTING.md` & `rio_ui-0.7.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/package.json` & `rio_ui-0.7.5/package.json`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/.github/PULL_REQUEST_TEMPLATE.md` & `rio_ui-0.7.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/.github/DISCUSSION_TEMPLATE/feature-requests.yml` & `rio_ui-0.7.5/.github/DISCUSSION_TEMPLATE/feature-requests.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/.github/ISSUE_TEMPLATE/bug_report.yml` & `rio_ui-0.7.5/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/.github/ISSUE_TEMPLATE/config.yml` & `rio_ui-0.7.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/index.html` & `rio_ui-0.7.5/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/app.ts` & `rio_ui-0.7.5/frontend/code/app.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/colorConversion.ts` & `rio_ui-0.7.5/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/componentManagement.ts` & `rio_ui-0.7.5/frontend/code/componentManagement.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/cssUtils.ts` & `rio_ui-0.7.5/frontend/code/cssUtils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/dataModels.ts` & `rio_ui-0.7.5/frontend/code/dataModels.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/designApplication.ts` & `rio_ui-0.7.5/frontend/code/designApplication.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/easeFunctions.ts` & `rio_ui-0.7.5/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/eventHandling.ts` & `rio_ui-0.7.5/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/inputBoxTools.ts` & `rio_ui-0.7.5/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/layoutHelpers.ts` & `rio_ui-0.7.5/frontend/code/layoutHelpers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/layouting.ts` & `rio_ui-0.7.5/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/rippleEffect.ts` & `rio_ui-0.7.5/frontend/code/rippleEffect.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/rpc.ts` & `rio_ui-0.7.5/frontend/code/rpc.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/rpcFunctions.ts` & `rio_ui-0.7.5/frontend/code/rpcFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/utils.ts` & `rio_ui-0.7.5/frontend/code/utils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/align.ts` & `rio_ui-0.7.5/frontend/code/components/align.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/buildFailed.ts` & `rio_ui-0.7.5/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/button.ts` & `rio_ui-0.7.5/frontend/code/components/button.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/card.ts` & `rio_ui-0.7.5/frontend/code/components/card.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/classContainer.ts` & `rio_ui-0.7.5/frontend/code/components/classContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/codeBlock.ts` & `rio_ui-0.7.5/frontend/code/components/codeBlock.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/codeExplorer.ts` & `rio_ui-0.7.5/frontend/code/components/codeExplorer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/colorPicker.ts` & `rio_ui-0.7.5/frontend/code/components/colorPicker.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/componentBase.ts` & `rio_ui-0.7.5/frontend/code/components/componentBase.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/componentTree.ts` & `rio_ui-0.7.5/frontend/code/components/componentTree.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/customListItem.ts` & `rio_ui-0.7.5/frontend/code/components/customListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/debuggerConnector.ts` & `rio_ui-0.7.5/frontend/code/components/debuggerConnector.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/drawer.ts` & `rio_ui-0.7.5/frontend/code/components/drawer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/dropdown.ts` & `rio_ui-0.7.5/frontend/code/components/dropdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/flowContainer.ts` & `rio_ui-0.7.5/frontend/code/components/flowContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.7.5/frontend/code/components/fundamentalRootComponent.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/grid.ts` & `rio_ui-0.7.5/frontend/code/components/grid.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/headingListItem.ts` & `rio_ui-0.7.5/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/html.ts` & `rio_ui-0.7.5/frontend/code/components/html.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/icon.ts` & `rio_ui-0.7.5/frontend/code/components/icon.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/image.ts` & `rio_ui-0.7.5/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/keyEventListener.ts` & `rio_ui-0.7.5/frontend/code/components/keyEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/linearContainers.ts` & `rio_ui-0.7.5/frontend/code/components/linearContainers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/link.ts` & `rio_ui-0.7.5/frontend/code/components/link.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/listView.ts` & `rio_ui-0.7.5/frontend/code/components/listView.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/margin.ts` & `rio_ui-0.7.5/frontend/code/components/margin.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/markdown.ts` & `rio_ui-0.7.5/frontend/code/components/markdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.7.5/frontend/code/components/mediaPlayer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.7.5/frontend/code/components/mouseEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.7.5/frontend/code/components/multiLineTextInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/nodeInput.ts` & `rio_ui-0.7.5/frontend/code/components/nodeInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/nodeOutput.ts` & `rio_ui-0.7.5/frontend/code/components/nodeOutput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/overlay.ts` & `rio_ui-0.7.5/frontend/code/components/overlay.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/placeholder.ts` & `rio_ui-0.7.5/frontend/code/components/placeholder.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/plot.ts` & `rio_ui-0.7.5/frontend/code/components/plot.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/popup.ts` & `rio_ui-0.7.5/frontend/code/components/popup.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/progressBar.ts` & `rio_ui-0.7.5/frontend/code/components/progressBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/progressCircle.ts` & `rio_ui-0.7.5/frontend/code/components/progressCircle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/rectangle.ts` & `rio_ui-0.7.5/frontend/code/components/rectangle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/revealer.ts` & `rio_ui-0.7.5/frontend/code/components/revealer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/scrollContainer.ts` & `rio_ui-0.7.5/frontend/code/components/scrollContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/scrollTarget.ts` & `rio_ui-0.7.5/frontend/code/components/scrollTarget.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/separator.ts` & `rio_ui-0.7.5/frontend/code/components/separator.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/separatorListItem.ts` & `rio_ui-0.7.5/frontend/code/components/separatorListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/singleContainer.ts` & `rio_ui-0.7.5/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/slider.ts` & `rio_ui-0.7.5/frontend/code/components/slider.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/slideshow.ts` & `rio_ui-0.7.5/frontend/code/components/slideshow.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/stack.ts` & `rio_ui-0.7.5/frontend/code/components/stack.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/switch.ts` & `rio_ui-0.7.5/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/switcher.ts` & `rio_ui-0.7.5/frontend/code/components/switcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/switcherBar.ts` & `rio_ui-0.7.5/frontend/code/components/switcherBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/table.ts` & `rio_ui-0.7.5/frontend/code/components/table.ts`

 * *Files 6% similar despite different names*

```diff
@@ -112,23 +112,29 @@
         }
     }
 }
 
 export class TableComponent extends ComponentBase {
     state: TableState;
 
+    // We need a container element for `getElementDimensions`
+    private tableElement: HTMLElement;
+
     private sortOrder = new SortOrder();
 
     private headerCells: HTMLElement[] = [];
     private rowNumberCells: HTMLElement[] = [];
     private dataCells: HTMLElement[] = [];
 
     createElement(): HTMLElement {
         let element = document.createElement('div');
-        element.classList.add('rio-table');
+
+        this.tableElement = document.createElement('div');
+        this.tableElement.classList.add('rio-table');
+        element.appendChild(this.tableElement);
 
         return element;
     }
 
     updateElement(
         deltaState: TableDeltaState,
         latentComponents: Set<ComponentBase>
@@ -156,15 +162,15 @@
             } else {
                 this.hideRowNumbers();
             }
         }
 
         this.makeLayoutDirty();
         [this.naturalWidth, this.naturalHeight] = getElementDimensions(
-            this.element
+            this.tableElement
         );
     }
 
     // Natural size is set in updateElement
     updateNaturalWidth(ctx: LayoutContext): void {}
     updateNaturalHeight(ctx: LayoutContext): void {}
 
@@ -180,15 +186,15 @@
             for (let [rowNr, value] of column.values.entries()) {
                 let cell = document.createElement('span');
                 cell.textContent = `${value}`;
                 cell.style.textAlign = column.alignment;
 
                 cell.style.gridRow = `${rowNr + 2}`;
                 cell.style.gridColumn = `${columnNr}`;
-                this.element.appendChild(cell);
+                this.tableElement.appendChild(cell);
                 this.dataCells.push(cell);
             }
 
             columnNr++;
         }
     }
 
@@ -202,15 +208,15 @@
             let cell = document.createElement('span');
             cell.textContent = `${i + 1}.`;
             cell.style.textAlign = 'right';
             cell.style.opacity = '0.5';
 
             cell.style.gridRow = `${i + 2}`;
             cell.style.gridColumn = '1';
-            this.element.appendChild(cell);
+            this.tableElement.appendChild(cell);
 
             this.rowNumberCells.push(cell);
         }
     }
 
     private hideRowNumbers(): void {
         for (let element of this.rowNumberCells) {
@@ -233,15 +239,15 @@
             cell.addEventListener(
                 'click',
                 this.onHeaderClick.bind(this, column.name)
             );
 
             cell.style.gridRow = '1';
             cell.style.gridColumn = `${i + 2}`;
-            this.element.appendChild(cell);
+            this.tableElement.appendChild(cell);
 
             this.headerCells.push(cell);
         }
     }
 
     private hideColumnHeaders(): void {
         for (let element of this.headerCells) {
```

### Comparing `rio_ui-0.7.4/frontend/code/components/text.ts` & `rio_ui-0.7.5/frontend/code/components/text.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/textInput.ts` & `rio_ui-0.7.5/frontend/code/components/textInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.7.5/frontend/code/components/themeContextSwitcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/tooltip.ts` & `rio_ui-0.7.5/frontend/code/components/tooltip.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/code/components/website.ts` & `rio_ui-0.7.5/frontend/code/components/website.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.7.5/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/css/highlightjs-default-light.css` & `rio_ui-0.7.5/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/css/style.scss` & `rio_ui-0.7.5/frontend/css/style.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/frontend/css/switcheroos.scss` & `rio_ui-0.7.5/frontend/css/switcheroos.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.7.5/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.7.5/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.7.5/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.7.5/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/logo.svg` & `rio_ui-0.7.5/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.7.5/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.7.5/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/color/logo.svg` & `rio_ui-0.7.5/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.7.5/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.7.5/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/rio/fill/logo.svg` & `rio_ui-0.7.5/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.7.5/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.7.5/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.7.5/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.7.5/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/__init__.py` & `rio_ui-0.7.5/rio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 import logging
 
 _logger = logging.getLogger(__name__)
 
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
```

### Comparing `rio_ui-0.7.4/rio/app.py` & `rio_ui-0.7.5/rio/app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/app_server.py` & `rio_ui-0.7.5/rio/app_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,19 @@
 
         self.app = app_
         self.debug_mode = debug_mode
         self.running_in_window = running_in_window
         self.validator_factory = validator_factory
         self.internal_on_app_start = internal_on_app_start
 
+        # While this boolean is True, no new connections will be accepted. This
+        # is used to ensure that no clients (re-)connect while `rio run` is
+        # reloading the app.
+        self._reject_websocket_connections = False
+
         # Initialized lazily, when the favicon is first requested.
         self._icon_as_png_blob: bytes | None = None
 
         # The session tokens for all active sessions. These allow clients to
         # identify themselves, for example to reconnect in case of a lost
         # connection.
         self._active_session_tokens: dict[str, rio.Session] = {}
@@ -645,14 +650,23 @@
             ]
         )
 
         return fastapi.responses.Response(
             status_code=fastapi.status.HTTP_200_OK
         )
 
+    @contextlib.contextmanager
+    def reject_websocket_connections(self):
+        self._reject_websocket_connections = True
+
+        try:
+            yield
+        finally:
+            self._reject_websocket_connections = False
+
     async def _serve_websocket(
         self,
         websocket: fastapi.WebSocket,
         sessionToken: str,
     ):
         """
         Handler for establishing the websocket connection and handling any
@@ -661,14 +675,21 @@
         # Blah, naming conventions
         session_token = sessionToken
         del sessionToken
 
         # Accept the socket
         await websocket.accept()
 
+        if self._reject_websocket_connections:
+            await websocket.close(
+                3001,  # Custom error code
+                "App is currently reloading, try again later",
+            )
+            return
+
         # Look up the session token. If it is valid the session's duration is
         # refreshed so it doesn't expire. If the token is not valid, don't
         # accept the websocket.
         try:
             sess = self._active_session_tokens[session_token]
         except KeyError:
             # Inform the client that its session token is unknown and request a
```

### Comparing `rio_ui-0.7.4/rio/assets.py` & `rio_ui-0.7.5/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/byte_serving.py` & `rio_ui-0.7.5/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/color.py` & `rio_ui-0.7.5/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/dataclass.py` & `rio_ui-0.7.5/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/errors.py` & `rio_ui-0.7.5/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/event.py` & `rio_ui-0.7.5/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/fills.py` & `rio_ui-0.7.5/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/global_state.py` & `rio_ui-0.7.5/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/icon_registry.py` & `rio_ui-0.7.5/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/inspection.py` & `rio_ui-0.7.5/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/maybes.py` & `rio_ui-0.7.5/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/routing.py` & `rio_ui-0.7.5/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/serialization.py` & `rio_ui-0.7.5/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/session.py` & `rio_ui-0.7.5/rio/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import typing
 import weakref
 from collections.abc import Callable, Coroutine, Iterable
 from dataclasses import dataclass
 from datetime import tzinfo
 from typing import Any, Literal, cast, overload
 
-import aiofiles
 import fastapi
 import unicall
 import uniserde
 from uniserde import Jsonable, JsonDoc
 
 import rio
 
@@ -1512,14 +1511,16 @@
         #
         # Keys in this dict can be attributes of the "root" section or names of
         # sections. To prevent name clashes, section names are prefixed with
         # "section:".
         settings_json: dict[str, object]
 
         if self.running_in_window:
+            import aiofiles
+
             try:
                 async with aiofiles.open(
                     self._get_settings_file_path()
                 ) as file:
                     settings_text = await file.read()
 
                 settings_json = json.loads(settings_text)
@@ -1592,14 +1593,16 @@
 
     async def _save_settings_now_in_window(
         self,
         settings_to_save: Iterable[
             tuple[user_settings_module.UserSettings, Iterable[str]]
         ],
     ) -> None:
+        import aiofiles
+
         for settings, dirty_attributes in settings_to_save:
             if settings.section_name:
                 section = cast(
                     dict[str, object],
                     self._settings_json.setdefault(
                         "section:" + settings.section_name, {}
                     ),
@@ -1686,15 +1689,15 @@
         Changes the window title of this session.
 
         ## Parameters
 
         `title`: The new window title.
         """
         if self.running_in_window:
-            import webview.util
+            import webview.util  # type: ignore
 
             window = await self._get_webview_window()
 
             while True:
                 try:
                     window.set_title(title)
                     break
@@ -1816,14 +1819,15 @@
 
         `directory`: The directory where the file dialog should open. This has
             no effect if the user is visiting the app in a browser.
         """
         if self.running_in_window:
             # FIXME: Find (1) a better way to get the active window and (2) a
             # way to open a file dialog without blocking the event loop.
+            import aiofiles
             import webview  # type: ignore
 
             window = await self._get_webview_window()
             destinations = window.create_file_dialog(
                 webview.SAVE_DIALOG,
                 directory="" if directory is None else str(directory),
                 save_filename=file_name,
```

### Comparing `rio_ui-0.7.4/rio/session_attachments.py` & `rio_ui-0.7.5/rio/session_attachments.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/state_properties.py` & `rio_ui-0.7.5/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/testing.py` & `rio_ui-0.7.5/rio/testing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/text_style.py` & `rio_ui-0.7.5/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/theme.py` & `rio_ui-0.7.5/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/user_settings_module.py` & `rio_ui-0.7.5/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/utils.py` & `rio_ui-0.7.5/rio/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/world_units.py` & `rio_ui-0.7.5/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto/LICENSE.txt` & `rio_ui-0.7.5/rio/assets/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.7.5/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.7.5/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.7.5/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.7.5/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.7.5/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.7.5/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/__init__.py` & `rio_ui-0.7.5/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/cli_instance.py` & `rio_ui-0.7.5/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/nice_traceback.py` & `rio_ui-0.7.5/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/project.py` & `rio_ui-0.7.5/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/project_setup.py` & `rio_ui-0.7.5/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/rio_api.py` & `rio_ui-0.7.5/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/rioignore.py` & `rio_ui-0.7.5/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/tomlconfig.py` & `rio_ui-0.7.5/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/run_project/app_loading.py` & `rio_ui-0.7.5/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/run_project/arbiter.py` & `rio_ui-0.7.5/rio/cli/run_project/arbiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -568,62 +568,49 @@
         # Shut down the current app. This happens automatically when the app
         # server shuts down, but since we're just swapping out the app, we have
         # to call it manually.
         #
         # But first, close all open sessions. It's important that
         # `on_session_close` is executed *before* we reload the module. (And
         # before `on_app_close` is called.)
-        await asyncio.gather(
-            *[
-                session._close(close_remote_session=False)
-                for session in app_server._active_session_tokens.values()
-            ]
-        )
-        await app_server._call_on_app_close()
-
-        # Load the user's app again
-        new_app, loading_error = self.try_load_app()
-
-        # Replace the app which is currently hosted by uvicorn
-        self._uvicorn_worker.replace_app(new_app)
-        revel.success("Ready")
-
-        # There is a subtlety here. Sessions which have requested their
-        # index.html, but aren't yet connected to the websocket cannot
-        # receive messages. So `_spawn_traceback_popups` will skip them.
-        # This is fine as long as `self._app_server.app` has already been
-        # assigned, since this ensures that any new websocket connections
-        # will receive the new app anyway.
         #
-        # -> This MUST happen after the new app has already been injected
-        if loading_error is not None:
-            self._spawn_traceback_popups(loading_error)
-
-        # The app has changed, but the uvicorn server is still the same. Because
-        # of this, uvicorn won't call the `on_app_start` function - do it
-        # manually.
-        await app_server._call_on_app_start()
+        # And to makes sure that clients can't reconnect while we're still
+        # shutting down sessions, tell the app server to reject attempted
+        # reconnects.
+        with app_server.reject_websocket_connections():
+            await asyncio.gather(
+                *[
+                    session._close(close_remote_session=False)
+                    for session in app_server._active_session_tokens.values()
+                ]
+            )
+            await app_server._call_on_app_close()
 
-        # Tell all sessions to reconnect, and close old sessions
-        rio.cli._logger.debug("Reloading all sessions")
+            # Load the user's app again
+            new_app, loading_error = self.try_load_app()
 
-        for sess in list(app_server._active_session_tokens.values()):
-            # Tell the session to reload
+            # Replace the app which is currently hosted by uvicorn
+            self._uvicorn_worker.replace_app(new_app)
+            revel.success("Ready")
+
+            # The app has changed, but the uvicorn server is still the same.
+            # Because of this, uvicorn won't call the `on_app_start` function -
+            # do it manually.
+            await app_server._call_on_app_start()
+
+            # There is a subtlety here. Sessions which have requested their
+            # index.html, but aren't yet connected to the websocket cannot
+            # receive messages. So `_spawn_traceback_popups` will skip them.
+            # This is fine as long as `self._app_server.app` has already been
+            # assigned, since this ensures that any new websocket connections
+            # will receive the new app anyway.
             #
-            # TODO: Should there be some waiting period here, so that the
-            # session has time to save settings first and shut down in general?
-            self._evaluate_javascript_in_session_if_connected(
-                sess, "window.location.reload()"
-            )
-
-            # Close it
-            asyncio.create_task(
-                sess._close(close_remote_session=False),
-                name=f'Close session "{sess._session_token}"',
-            )
+            # -> This MUST happen after the new app has already been injected
+            if loading_error is not None:
+                self._spawn_traceback_popups(loading_error)
 
     def _evaluate_javascript_in_session_if_connected(
         self,
         session: rio.Session,
         javascript_source: str,
     ) -> None:
         """
```

### Comparing `rio_ui-0.7.4/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.7.5/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.7.5/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/cli/run_project/webview_worker.py` & `rio_ui-0.7.5/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/__init__.py` & `rio_ui-0.7.5/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/app_root.py` & `rio_ui-0.7.5/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/auto_form.py` & `rio_ui-0.7.5/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/banner.py` & `rio_ui-0.7.5/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/build_failed.py` & `rio_ui-0.7.5/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/button.py` & `rio_ui-0.7.5/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/card.py` & `rio_ui-0.7.5/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/class_container.py` & `rio_ui-0.7.5/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/code_block.py` & `rio_ui-0.7.5/rio/components/code_block.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/color_picker.py` & `rio_ui-0.7.5/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/component.py` & `rio_ui-0.7.5/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/component_tree.py` & `rio_ui-0.7.5/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/container.py` & `rio_ui-0.7.5/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/devel_component.py` & `rio_ui-0.7.5/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/drawer.py` & `rio_ui-0.7.5/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/dropdown.py` & `rio_ui-0.7.5/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/flow_container.py` & `rio_ui-0.7.5/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/fundamental_component.py` & `rio_ui-0.7.5/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/grid.py` & `rio_ui-0.7.5/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/html.py` & `rio_ui-0.7.5/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/icon.py` & `rio_ui-0.7.5/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/image.py` & `rio_ui-0.7.5/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/key_event_listener.py` & `rio_ui-0.7.5/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/labeled_column.py` & `rio_ui-0.7.5/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/linear_containers.py` & `rio_ui-0.7.5/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/link.py` & `rio_ui-0.7.5/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/list_items.py` & `rio_ui-0.7.5/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/list_view.py` & `rio_ui-0.7.5/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/markdown.py` & `rio_ui-0.7.5/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/media_player.py` & `rio_ui-0.7.5/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/mouse_event_listener.py` & `rio_ui-0.7.5/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/multi_line_text_input.py` & `rio_ui-0.7.5/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/node_input.py` & `rio_ui-0.7.5/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/node_output.py` & `rio_ui-0.7.5/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/number_input.py` & `rio_ui-0.7.5/rio/components/number_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/overlay.py` & `rio_ui-0.7.5/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/page_view.py` & `rio_ui-0.7.5/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/plot.py` & `rio_ui-0.7.5/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/popup.py` & `rio_ui-0.7.5/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/progress_bar.py` & `rio_ui-0.7.5/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/progress_circle.py` & `rio_ui-0.7.5/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/rectangle.py` & `rio_ui-0.7.5/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/revealer.py` & `rio_ui-0.7.5/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/root_components.py` & `rio_ui-0.7.5/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/scroll_container.py` & `rio_ui-0.7.5/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/scroll_target.py` & `rio_ui-0.7.5/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/separator.py` & `rio_ui-0.7.5/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/slider.py` & `rio_ui-0.7.5/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/slideshow.py` & `rio_ui-0.7.5/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/spacer.py` & `rio_ui-0.7.5/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/stack.py` & `rio_ui-0.7.5/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/switch.py` & `rio_ui-0.7.5/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/switcher.py` & `rio_ui-0.7.5/rio/components/switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/switcher_bar.py` & `rio_ui-0.7.5/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/table.py` & `rio_ui-0.7.5/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/text.py` & `rio_ui-0.7.5/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/text_input.py` & `rio_ui-0.7.5/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/theme_context_switcher.py` & `rio_ui-0.7.5/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/tooltip.py` & `rio_ui-0.7.5/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/components/website.py` & `rio_ui-0.7.5/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/monkeypatches.py` & `rio_ui-0.7.5/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/typing_utils.py` & `rio_ui-0.7.5/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/validator.py` & `rio_ui-0.7.5/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/component_details.py` & `rio_ui-0.7.5/rio/debug/dev_tools/component_details.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/deploy_page.py` & `rio_ui-0.7.5/rio/debug/dev_tools/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/dev_tools_sidebar.py` & `rio_ui-0.7.5/rio/debug/dev_tools/dev_tools_sidebar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/docs_page.py` & `rio_ui-0.7.5/rio/debug/dev_tools/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/icons_page.py` & `rio_ui-0.7.5/rio/debug/dev_tools/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/layout_preview.py` & `rio_ui-0.7.5/rio/debug/dev_tools/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/project_page.py` & `rio_ui-0.7.5/rio/debug/dev_tools/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/sample_icons_grid.py` & `rio_ui-0.7.5/rio/debug/dev_tools/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/theme_picker_page.py` & `rio_ui-0.7.5/rio/debug/dev_tools/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/debug/dev_tools/tree_page.py` & `rio_ui-0.7.5/rio/debug/dev_tools/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/docs/__init__.py` & `rio_ui-0.7.5/rio/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/generated/index.html` & `rio_ui-0.7.5/rio/generated/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -21495,4537 +21495,4544 @@
 00053f60: 6e65 7720 4175 2c74 6869 732e 6865 6164  new Au,this.head
 00053f70: 6572 4365 6c6c 733d 5b5d 2c74 6869 732e  erCells=[],this.
 00053f80: 726f 774e 756d 6265 7243 656c 6c73 3d5b  rowNumberCells=[
 00053f90: 5d2c 7468 6973 2e64 6174 6143 656c 6c73  ],this.dataCells
 00053fa0: 3d5b 5d7d 6372 6561 7465 456c 656d 656e  =[]}createElemen
 00053fb0: 7428 297b 6c65 7420 653d 646f 6375 6d65  t(){let e=docume
 00053fc0: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
-00053fd0: 2822 6469 7622 293b 7265 7475 726e 2065  ("div");return e
-00053fe0: 2e63 6c61 7373 4c69 7374 2e61 6464 2822  .classList.add("
-00053ff0: 7269 6f2d 7461 626c 6522 292c 657d 7570  rio-table"),e}up
-00054000: 6461 7465 456c 656d 656e 7428 652c 6e29  dateElement(e,n)
-00054010: 7b65 2e64 6174 6121 3d3d 766f 6964 2030  {e.data!==void 0
-00054020: 3f28 7468 6973 2e73 7461 7465 2e64 6174  ?(this.state.dat
-00054030: 613d 5375 2865 2e64 6174 6129 2c74 6869  a=Su(e.data),thi
-00054040: 732e 6469 7370 6c61 7944 6174 6128 292c  s.displayData(),
-00054050: 2865 2e73 686f 775f 726f 775f 6e75 6d62  (e.show_row_numb
-00054060: 6572 733f 3f74 6869 732e 7374 6174 652e  ers??this.state.
-00054070: 7368 6f77 5f72 6f77 5f6e 756d 6265 7273  show_row_numbers
-00054080: 2926 2674 6869 732e 7368 6f77 526f 774e  )&&this.showRowN
-00054090: 756d 6265 7273 2829 2c41 7272 6179 2e69  umbers(),Array.i
-000540a0: 7341 7272 6179 2865 2e64 6174 6129 3f74  sArray(e.data)?t
-000540b0: 6869 732e 6869 6465 436f 6c75 6d6e 4865  his.hideColumnHe
-000540c0: 6164 6572 7328 293a 7468 6973 2e73 686f  aders():this.sho
-000540d0: 7743 6f6c 756d 6e48 6561 6465 7273 2829  wColumnHeaders()
-000540e0: 293a 652e 7368 6f77 5f72 6f77 5f6e 756d  ):e.show_row_num
-000540f0: 6265 7273 213d 3d76 6f69 6420 3026 2665  bers!==void 0&&e
-00054100: 2e73 686f 775f 726f 775f 6e75 6d62 6572  .show_row_number
-00054110: 7321 3d3d 7468 6973 2e73 7461 7465 2e73  s!==this.state.s
-00054120: 686f 775f 726f 775f 6e75 6d62 6572 7326  how_row_numbers&
-00054130: 2628 652e 7368 6f77 5f72 6f77 5f6e 756d  &(e.show_row_num
-00054140: 6265 7273 3f74 6869 732e 7368 6f77 526f  bers?this.showRo
-00054150: 774e 756d 6265 7273 2829 3a74 6869 732e  wNumbers():this.
-00054160: 6869 6465 526f 774e 756d 6265 7273 2829  hideRowNumbers()
-00054170: 292c 7468 6973 2e6d 616b 654c 6179 6f75  ),this.makeLayou
-00054180: 7444 6972 7479 2829 2c5b 7468 6973 2e6e  tDirty(),[this.n
-00054190: 6174 7572 616c 5769 6474 682c 7468 6973  aturalWidth,this
-000541a0: 2e6e 6174 7572 616c 4865 6967 6874 5d3d  .naturalHeight]=
-000541b0: 6174 2874 6869 732e 656c 656d 656e 7429  at(this.element)
-000541c0: 7d75 7064 6174 654e 6174 7572 616c 5769  }updateNaturalWi
-000541d0: 6474 6828 6529 7b7d 7570 6461 7465 4e61  dth(e){}updateNa
-000541e0: 7475 7261 6c48 6569 6768 7428 6529 7b7d  turalHeight(e){}
-000541f0: 6469 7370 6c61 7944 6174 6128 297b 666f  displayData(){fo
-00054200: 7228 6c65 7420 6e20 6f66 2074 6869 732e  r(let n of this.
-00054210: 6461 7461 4365 6c6c 7329 6e2e 7265 6d6f  dataCells)n.remo
-00054220: 7665 2829 3b74 6869 732e 6461 7461 4365  ve();this.dataCe
-00054230: 6c6c 733d 5b5d 3b6c 6574 2065 3d32 3b66  lls=[];let e=2;f
-00054240: 6f72 286c 6574 206e 206f 6620 7468 6973  or(let n of this
-00054250: 2e73 7461 7465 2e64 6174 6129 7b66 6f72  .state.data){for
-00054260: 286c 6574 5b69 2c72 5d6f 6620 6e2e 7661  (let[i,r]of n.va
-00054270: 6c75 6573 2e65 6e74 7269 6573 2829 297b  lues.entries()){
-00054280: 6c65 7420 733d 646f 6375 6d65 6e74 2e63  let s=document.c
-00054290: 7265 6174 6545 6c65 6d65 6e74 2822 7370  reateElement("sp
-000542a0: 616e 2229 3b73 2e74 6578 7443 6f6e 7465  an");s.textConte
-000542b0: 6e74 3d60 247b 727d 602c 732e 7374 796c  nt=`${r}`,s.styl
-000542c0: 652e 7465 7874 416c 6967 6e3d 6e2e 616c  e.textAlign=n.al
-000542d0: 6967 6e6d 656e 742c 732e 7374 796c 652e  ignment,s.style.
-000542e0: 6772 6964 526f 773d 6024 7b69 2b32 7d60  gridRow=`${i+2}`
-000542f0: 2c73 2e73 7479 6c65 2e67 7269 6443 6f6c  ,s.style.gridCol
-00054300: 756d 6e3d 6024 7b65 7d60 2c74 6869 732e  umn=`${e}`,this.
-00054310: 656c 656d 656e 742e 6170 7065 6e64 4368  element.appendCh
-00054320: 696c 6428 7329 2c74 6869 732e 6461 7461  ild(s),this.data
-00054330: 4365 6c6c 732e 7075 7368 2873 297d 652b  Cells.push(s)}e+
-00054340: 2b7d 7d73 686f 7752 6f77 4e75 6d62 6572  +}}showRowNumber
-00054350: 7328 297b 7468 6973 2e68 6964 6552 6f77  s(){this.hideRow
-00054360: 4e75 6d62 6572 7328 293b 6c65 7420 653d  Numbers();let e=
-00054370: 7468 6973 2e73 7461 7465 2e64 6174 612e  this.state.data.
-00054380: 6c65 6e67 7468 3d3d 3d30 3f30 3a74 6869  length===0?0:thi
-00054390: 732e 7374 6174 652e 6461 7461 5b30 5d2e  s.state.data[0].
-000543a0: 7661 6c75 6573 2e6c 656e 6774 683b 666f  values.length;fo
-000543b0: 7228 6c65 7420 6e3d 303b 6e3c 653b 6e2b  r(let n=0;n<e;n+
-000543c0: 2b29 7b6c 6574 2069 3d64 6f63 756d 656e  +){let i=documen
-000543d0: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
-000543e0: 2273 7061 6e22 293b 692e 7465 7874 436f  "span");i.textCo
-000543f0: 6e74 656e 743d 6024 7b6e 2b31 7d2e 602c  ntent=`${n+1}.`,
-00054400: 692e 7374 796c 652e 7465 7874 416c 6967  i.style.textAlig
-00054410: 6e3d 2272 6967 6874 222c 692e 7374 796c  n="right",i.styl
-00054420: 652e 6f70 6163 6974 793d 2230 2e35 222c  e.opacity="0.5",
-00054430: 692e 7374 796c 652e 6772 6964 526f 773d  i.style.gridRow=
-00054440: 6024 7b6e 2b32 7d60 2c69 2e73 7479 6c65  `${n+2}`,i.style
-00054450: 2e67 7269 6443 6f6c 756d 6e3d 2231 222c  .gridColumn="1",
-00054460: 7468 6973 2e65 6c65 6d65 6e74 2e61 7070  this.element.app
-00054470: 656e 6443 6869 6c64 2869 292c 7468 6973  endChild(i),this
-00054480: 2e72 6f77 4e75 6d62 6572 4365 6c6c 732e  .rowNumberCells.
-00054490: 7075 7368 2869 297d 7d68 6964 6552 6f77  push(i)}}hideRow
-000544a0: 4e75 6d62 6572 7328 297b 666f 7228 6c65  Numbers(){for(le
-000544b0: 7420 6520 6f66 2074 6869 732e 726f 774e  t e of this.rowN
-000544c0: 756d 6265 7243 656c 6c73 2965 2e72 656d  umberCells)e.rem
-000544d0: 6f76 6528 293b 7468 6973 2e72 6f77 4e75  ove();this.rowNu
-000544e0: 6d62 6572 4365 6c6c 733d 5b5d 7d73 686f  mberCells=[]}sho
-000544f0: 7743 6f6c 756d 6e48 6561 6465 7273 2829  wColumnHeaders()
-00054500: 7b74 6869 732e 6869 6465 436f 6c75 6d6e  {this.hideColumn
-00054510: 4865 6164 6572 7328 293b 666f 7228 6c65  Headers();for(le
-00054520: 745b 652c 6e5d 6f66 2074 6869 732e 7374  t[e,n]of this.st
-00054530: 6174 652e 6461 7461 2e65 6e74 7269 6573  ate.data.entries
-00054540: 2829 297b 6c65 7420 693d 646f 6375 6d65  ()){let i=docume
-00054550: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
-00054560: 2822 7370 616e 2229 3b69 2e63 6c61 7373  ("span");i.class
-00054570: 4c69 7374 2e61 6464 2822 6865 6164 6572  List.add("header
-00054580: 2229 2c69 2e74 6578 7443 6f6e 7465 6e74  "),i.textContent
-00054590: 3d6e 2e6e 616d 652c 692e 7374 796c 652e  =n.name,i.style.
-000545a0: 7465 7874 416c 6967 6e3d 6e2e 616c 6967  textAlign=n.alig
-000545b0: 6e6d 656e 742c 692e 7374 796c 652e 6f70  nment,i.style.op
-000545c0: 6163 6974 793d 2230 2e35 222c 692e 6164  acity="0.5",i.ad
-000545d0: 6445 7665 6e74 4c69 7374 656e 6572 2822  dEventListener("
-000545e0: 636c 6963 6b22 2c74 6869 732e 6f6e 4865  click",this.onHe
-000545f0: 6164 6572 436c 6963 6b2e 6269 6e64 2874  aderClick.bind(t
-00054600: 6869 732c 6e2e 6e61 6d65 2929 2c69 2e73  his,n.name)),i.s
-00054610: 7479 6c65 2e67 7269 6452 6f77 3d22 3122  tyle.gridRow="1"
-00054620: 2c69 2e73 7479 6c65 2e67 7269 6443 6f6c  ,i.style.gridCol
-00054630: 756d 6e3d 6024 7b65 2b32 7d60 2c74 6869  umn=`${e+2}`,thi
-00054640: 732e 656c 656d 656e 742e 6170 7065 6e64  s.element.append
-00054650: 4368 696c 6428 6929 2c74 6869 732e 6865  Child(i),this.he
-00054660: 6164 6572 4365 6c6c 732e 7075 7368 2869  aderCells.push(i
-00054670: 297d 7d68 6964 6543 6f6c 756d 6e48 6561  )}}hideColumnHea
-00054680: 6465 7273 2829 7b66 6f72 286c 6574 2065  ders(){for(let e
-00054690: 206f 6620 7468 6973 2e68 6561 6465 7243   of this.headerC
-000546a0: 656c 6c73 2965 2e72 656d 6f76 6528 293b  ells)e.remove();
-000546b0: 7468 6973 2e68 6561 6465 7243 656c 6c73  this.headerCells
-000546c0: 3d5b 5d7d 6f6e 4865 6164 6572 436c 6963  =[]}onHeaderClic
-000546d0: 6b28 652c 6e29 7b6c 6574 2069 3d6e 2e74  k(e,n){let i=n.t
-000546e0: 6172 6765 743b 692e 7461 674e 616d 6521  arget;i.tagName!
-000546f0: 3d3d 2253 5041 4e22 2626 2869 3d69 2e70  =="SPAN"&&(i=i.p
-00054700: 6172 656e 7445 6c65 6d65 6e74 293b 6c65  arentElement);le
-00054710: 7420 723d 692e 6461 7461 7365 742e 736f  t r=i.dataset.so
-00054720: 7274 213d 3d22 6173 6365 6e64 696e 6722  rt!=="ascending"
-00054730: 3b66 6f72 286c 6574 2073 206f 6620 7468  ;for(let s of th
-00054740: 6973 2e68 6561 6465 7243 656c 6c73 2964  is.headerCells)d
-00054750: 656c 6574 6520 732e 6461 7461 7365 742e  elete s.dataset.
-00054760: 736f 7274 3b69 2e64 6174 6173 6574 2e73  sort;i.dataset.s
-00054770: 6f72 743d 723f 2261 7363 656e 6469 6e67  ort=r?"ascending
-00054780: 223a 2264 6573 6365 6e64 696e 6722 2c74  ":"descending",t
-00054790: 6869 732e 736f 7274 4f72 6465 722e 6164  his.sortOrder.ad
-000547a0: 6428 652c 7229 2c74 6869 732e 736f 7274  d(e,r),this.sort
-000547b0: 4f72 6465 722e 736f 7274 2874 6869 732e  Order.sort(this.
-000547c0: 7374 6174 652e 6461 7461 292c 7468 6973  state.data),this
-000547d0: 2e64 6973 706c 6179 4461 7461 2829 2c6e  .displayData(),n
-000547e0: 2e73 746f 7050 726f 7061 6761 7469 6f6e  .stopPropagation
-000547f0: 2829 7d7d 636c 6173 7320 5275 2065 7874  ()}}class Ru ext
-00054800: 656e 6473 2055 7b63 7265 6174 6545 6c65  ends U{createEle
-00054810: 6d65 6e74 2829 7b6c 6574 2065 3d64 6f63  ment(){let e=doc
-00054820: 756d 656e 742e 6372 6561 7465 456c 656d  ument.createElem
-00054830: 656e 7428 2264 6976 2229 3b72 6574 7572  ent("div");retur
-00054840: 6e20 652e 636c 6173 734c 6973 742e 6164  n e.classList.ad
-00054850: 6428 2272 696f 2d74 6578 7422 292c 7468  d("rio-text"),th
-00054860: 6973 2e69 6e6e 6572 3d64 6f63 756d 656e  is.inner=documen
-00054870: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
-00054880: 2264 6976 2229 2c65 2e61 7070 656e 6443  "div"),e.appendC
-00054890: 6869 6c64 2874 6869 732e 696e 6e65 7229  hild(this.inner)
-000548a0: 2c65 7d75 7064 6174 6545 6c65 6d65 6e74  ,e}updateElement
-000548b0: 2865 2c6e 297b 7377 6974 6368 2865 2e74  (e,n){switch(e.t
-000548c0: 6578 7421 3d3d 766f 6964 2030 2626 2874  ext!==void 0&&(t
-000548d0: 6869 732e 696e 6e65 722e 7465 7874 436f  his.inner.textCo
-000548e0: 6e74 656e 743d 652e 7465 7874 292c 652e  ntent=e.text),e.
-000548f0: 7772 6170 297b 6361 7365 2131 3a74 6869  wrap){case!1:thi
-00054900: 732e 696e 6e65 722e 7374 796c 652e 7768  s.inner.style.wh
-00054910: 6974 6553 7061 6365 3d22 7072 6522 2c74  iteSpace="pre",t
-00054920: 6869 732e 696e 6e65 722e 7374 796c 652e  his.inner.style.
-00054930: 7465 7874 4f76 6572 666c 6f77 3d22 636c  textOverflow="cl
-00054940: 6970 223b 6272 6561 6b3b 6361 7365 2130  ip";break;case!0
-00054950: 3a74 6869 732e 696e 6e65 722e 7374 796c  :this.inner.styl
-00054960: 652e 7768 6974 6553 7061 6365 3d22 7072  e.whiteSpace="pr
-00054970: 652d 7772 6170 222c 7468 6973 2e69 6e6e  e-wrap",this.inn
-00054980: 6572 2e73 7479 6c65 2e74 6578 744f 7665  er.style.textOve
-00054990: 7266 6c6f 773d 2263 6c69 7022 3b62 7265  rflow="clip";bre
-000549a0: 616b 3b63 6173 6522 656c 6c69 7073 697a  ak;case"ellipsiz
-000549b0: 6522 3a74 6869 732e 696e 6e65 722e 7374  e":this.inner.st
-000549c0: 796c 652e 7768 6974 6553 7061 6365 3d22  yle.whiteSpace="
-000549d0: 7072 6522 2c74 6869 732e 696e 6e65 722e  pre",this.inner.
-000549e0: 7374 796c 652e 7465 7874 4f76 6572 666c  style.textOverfl
-000549f0: 6f77 3d22 656c 6c69 7073 6973 223b 6272  ow="ellipsis";br
-00054a00: 6561 6b7d 652e 7365 6c65 6374 6162 6c65  eak}e.selectable
-00054a10: 213d 3d76 6f69 6420 3026 2628 7468 6973  !==void 0&&(this
-00054a20: 2e69 6e6e 6572 2e73 7479 6c65 2e70 6f69  .inner.style.poi
-00054a30: 6e74 6572 4576 656e 7473 3d65 2e73 656c  nterEvents=e.sel
-00054a40: 6563 7461 626c 653f 2261 7574 6f22 3a22  ectable?"auto":"
-00054a50: 6e6f 6e65 2229 2c65 2e73 7479 6c65 213d  none"),e.style!=
-00054a60: 3d76 6f69 6420 3026 264f 626a 6563 742e  =void 0&&Object.
-00054a70: 6173 7369 676e 2874 6869 732e 696e 6e65  assign(this.inne
-00054a80: 722e 7374 796c 652c 5474 2865 2e73 7479  r.style,Tt(e.sty
-00054a90: 6c65 2929 2c65 2e6a 7573 7469 6679 213d  le)),e.justify!=
-00054aa0: 3d76 6f69 6420 3026 2628 7468 6973 2e69  =void 0&&(this.i
-00054ab0: 6e6e 6572 2e73 7479 6c65 2e74 6578 7441  nner.style.textA
-00054ac0: 6c69 676e 3d65 2e6a 7573 7469 6679 292c  lign=e.justify),
-00054ad0: 2865 2e74 6578 7421 3d3d 766f 6964 2030  (e.text!==void 0
-00054ae0: 7c7c 652e 7772 6170 213d 3d76 6f69 6420  ||e.wrap!==void 
-00054af0: 307c 7c65 2e73 7479 6c65 213d 3d76 6f69  0||e.style!==voi
-00054b00: 6420 3029 2626 2874 6869 732e 6d61 6b65  d 0)&&(this.make
-00054b10: 4c61 796f 7574 4469 7274 7928 292c 7468  LayoutDirty(),th
-00054b20: 6973 2e63 6163 6865 644e 6f57 7261 7044  is.cachedNoWrapD
-00054b30: 696d 656e 7369 6f6e 733d 6b65 2874 6869  imensions=ke(thi
-00054b40: 732e 656c 656d 656e 742e 7465 7874 436f  s.element.textCo
-00054b50: 6e74 656e 742c 7468 6973 2e73 7461 7465  ntent,this.state
-00054b60: 2e73 7479 6c65 2929 7d75 7064 6174 654e  .style))}updateN
-00054b70: 6174 7572 616c 5769 6474 6828 6529 7b74  aturalWidth(e){t
-00054b80: 6869 732e 7374 6174 652e 7772 6170 3d3d  his.state.wrap==
-00054b90: 3d21 313f 7468 6973 2e6e 6174 7572 616c  =!1?this.natural
-00054ba0: 5769 6474 683d 7468 6973 2e63 6163 6865  Width=this.cache
-00054bb0: 644e 6f57 7261 7044 696d 656e 7369 6f6e  dNoWrapDimension
-00054bc0: 735b 305d 3a74 6869 732e 6e61 7475 7261  s[0]:this.natura
-00054bd0: 6c57 6964 7468 3d30 7d75 7064 6174 654e  lWidth=0}updateN
-00054be0: 6174 7572 616c 4865 6967 6874 2865 297b  aturalHeight(e){
-00054bf0: 7468 6973 2e73 7461 7465 2e77 7261 703d  this.state.wrap=
-00054c00: 3d3d 2130 3f74 6869 732e 6e61 7475 7261  ==!0?this.natura
-00054c10: 6c48 6569 6768 743d 6b65 2874 6869 732e  lHeight=ke(this.
-00054c20: 7374 6174 652e 7465 7874 2c74 6869 732e  state.text,this.
-00054c30: 7374 6174 652e 7374 796c 652c 7468 6973  state.style,this
-00054c40: 2e61 6c6c 6f63 6174 6564 5769 6474 6829  .allocatedWidth)
-00054c50: 5b31 5d3a 7468 6973 2e6e 6174 7572 616c  [1]:this.natural
-00054c60: 4865 6967 6874 3d74 6869 732e 6361 6368  Height=this.cach
-00054c70: 6564 4e6f 5772 6170 4469 6d65 6e73 696f  edNoWrapDimensio
-00054c80: 6e73 5b31 5d7d 7d63 6c61 7373 204d 7520  ns[1]}}class Mu 
-00054c90: 6578 7465 6e64 7320 557b 636f 6e73 7472  extends U{constr
-00054ca0: 7563 746f 7228 297b 7375 7065 7228 2e2e  uctor(){super(..
-00054cb0: 2e61 7267 756d 656e 7473 292c 7468 6973  .arguments),this
-00054cc0: 2e70 7265 6669 7854 6578 7457 6964 7468  .prefixTextWidth
-00054cd0: 3d30 2c74 6869 732e 7375 6666 6978 5465  =0,this.suffixTe
-00054ce0: 7874 5769 6474 683d 307d 6372 6561 7465  xtWidth=0}create
-00054cf0: 456c 656d 656e 7428 297b 6c65 7420 653d  Element(){let e=
-00054d00: 646f 6375 6d65 6e74 2e63 7265 6174 6545  document.createE
-00054d10: 6c65 6d65 6e74 2822 6469 7622 293b 7265  lement("div");re
-00054d20: 7475 726e 2065 2e63 6c61 7373 4c69 7374  turn e.classList
-00054d30: 2e61 6464 2822 7269 6f2d 7465 7874 2d69  .add("rio-text-i
-00054d40: 6e70 7574 222c 2272 696f 2d69 6e70 7574  nput","rio-input
-00054d50: 2d62 6f78 2229 2c65 2e69 6e6e 6572 4854  -box"),e.innerHT
-00054d60: 4d4c 3d60 0a20 2020 2020 2020 2020 2020  ML=`.           
-00054d70: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
-00054d80: 7874 2220 7374 796c 653d 226f 7264 6572  xt" style="order
-00054d90: 3a20 3222 2070 6c61 6365 686f 6c64 6572  : 2" placeholder
-00054da0: 3d22 223e 0a20 2020 2020 2020 2020 2020  ="">.           
-00054db0: 203c 6469 7620 636c 6173 733d 2272 696f   <div class="rio
-00054dc0: 2d74 6578 742d 696e 7075 742d 6869 6e74  -text-input-hint
-00054dd0: 2d74 6578 7420 7269 6f2d 7465 7874 2d69  -text rio-text-i
-00054de0: 6e70 7574 2d70 7265 6669 782d 7465 7874  nput-prefix-text
-00054df0: 2220 7374 796c 653d 226f 7264 6572 3a20  " style="order: 
-00054e00: 3122 3e3c 2f64 6976 3e0a 2020 2020 2020  1"></div>.      
-00054e10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00054e20: 3d22 7269 6f2d 7465 7874 2d69 6e70 7574  ="rio-text-input
-00054e30: 2d68 696e 742d 7465 7874 2072 696f 2d74  -hint-text rio-t
-00054e40: 6578 742d 696e 7075 742d 7375 6666 6978  ext-input-suffix
-00054e50: 2d74 6578 7422 2073 7479 6c65 3d22 6f72  -text" style="or
-00054e60: 6465 723a 2033 223e 3c2f 6469 763e 0a20  der: 3"></div>. 
-00054e70: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00054e80: 636c 6173 733d 2272 696f 2d69 6e70 7574  class="rio-input
-00054e90: 2d62 6f78 2d6c 6162 656c 223e 3c2f 6469  -box-label"></di
-00054ea0: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
-00054eb0: 6469 7620 636c 6173 733d 2272 696f 2d69  div class="rio-i
-00054ec0: 6e70 7574 2d62 6f78 2d70 6c61 696e 2d62  nput-box-plain-b
-00054ed0: 6172 223e 3c2f 6469 763e 0a20 2020 2020  ar"></div>.     
-00054ee0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00054ef0: 733d 2272 696f 2d69 6e70 7574 2d62 6f78  s="rio-input-box
-00054f00: 2d63 6f6c 6f72 2d62 6172 223e 3c2f 6469  -color-bar"></di
-00054f10: 763e 0a20 2020 2020 2020 2060 2c74 6869  v>.        `,thi
-00054f20: 732e 6c61 6265 6c45 6c65 6d65 6e74 3d65  s.labelElement=e
-00054f30: 2e71 7565 7279 5365 6c65 6374 6f72 2822  .querySelector("
-00054f40: 2e72 696f 2d69 6e70 7574 2d62 6f78 2d6c  .rio-input-box-l
-00054f50: 6162 656c 2229 2c5b 7468 6973 2e70 7265  abel"),[this.pre
-00054f60: 6669 7854 6578 7445 6c65 6d65 6e74 2c74  fixTextElement,t
-00054f70: 6869 732e 7375 6666 6978 5465 7874 456c  his.suffixTextEl
-00054f80: 656d 656e 745d 3d41 7272 6179 2e66 726f  ement]=Array.fro
-00054f90: 6d28 652e 7175 6572 7953 656c 6563 746f  m(e.querySelecto
-00054fa0: 7241 6c6c 2822 2e72 696f 2d74 6578 742d  rAll(".rio-text-
-00054fb0: 696e 7075 742d 6869 6e74 2d74 6578 7422  input-hint-text"
-00054fc0: 2929 2c74 6869 732e 696e 7075 7445 6c65  )),this.inputEle
-00054fd0: 6d65 6e74 3d65 2e71 7565 7279 5365 6c65  ment=e.querySele
-00054fe0: 6374 6f72 2822 696e 7075 7422 292c 7468  ctor("input"),th
-00054ff0: 6973 2e69 6e70 7574 456c 656d 656e 742e  is.inputElement.
-00055000: 6164 6445 7665 6e74 4c69 7374 656e 6572  addEventListener
-00055010: 2822 626c 7572 222c 2829 3d3e 7b74 6869  ("blur",()=>{thi
-00055020: 732e 7365 7453 7461 7465 416e 644e 6f74  s.setStateAndNot
-00055030: 6966 7942 6163 6b65 6e64 287b 7465 7874  ifyBackend({text
-00055040: 3a74 6869 732e 696e 7075 7445 6c65 6d65  :this.inputEleme
-00055050: 6e74 2e76 616c 7565 7d29 7d29 2c74 6869  nt.value})}),thi
-00055060: 732e 696e 7075 7445 6c65 6d65 6e74 2e61  s.inputElement.a
-00055070: 6464 4576 656e 744c 6973 7465 6e65 7228  ddEventListener(
-00055080: 226b 6579 646f 776e 222c 6e3d 3e7b 6e2e  "keydown",n=>{n.
-00055090: 6b65 793d 3d3d 2245 6e74 6572 2226 2628  key==="Enter"&&(
-000550a0: 7468 6973 2e73 7461 7465 2e74 6578 743d  this.state.text=
-000550b0: 7468 6973 2e69 6e70 7574 456c 656d 656e  this.inputElemen
-000550c0: 742e 7661 6c75 652c 7468 6973 2e73 656e  t.value,this.sen
-000550d0: 644d 6573 7361 6765 546f 4261 636b 656e  dMessageToBacken
-000550e0: 6428 7b74 6578 743a 7468 6973 2e73 7461  d({text:this.sta
-000550f0: 7465 2e74 6578 747d 2929 2c6e 2e73 746f  te.text})),n.sto
-00055100: 7050 726f 7061 6761 7469 6f6e 2829 7d29  pPropagation()})
-00055110: 2c74 6869 732e 7072 6566 6978 5465 7874  ,this.prefixText
-00055120: 456c 656d 656e 742e 6164 6445 7665 6e74  Element.addEvent
-00055130: 4c69 7374 656e 6572 2822 6d6f 7573 6564  Listener("moused
-00055140: 6f77 6e22 2c6e 3d3e 7b6e 2e73 746f 7050  own",n=>{n.stopP
-00055150: 726f 7061 6761 7469 6f6e 2829 7d29 2c74  ropagation()}),t
-00055160: 6869 732e 7375 6666 6978 5465 7874 456c  his.suffixTextEl
-00055170: 656d 656e 742e 6164 6445 7665 6e74 4c69  ement.addEventLi
-00055180: 7374 656e 6572 2822 6d6f 7573 6564 6f77  stener("mousedow
-00055190: 6e22 2c6e 3d3e 7b6e 2e73 746f 7050 726f  n",n=>{n.stopPro
-000551a0: 7061 6761 7469 6f6e 2829 7d29 2c74 6869  pagation()}),thi
-000551b0: 732e 7072 6566 6978 5465 7874 456c 656d  s.prefixTextElem
-000551c0: 656e 742e 6164 6445 7665 6e74 4c69 7374  ent.addEventList
-000551d0: 656e 6572 2822 636c 6963 6b22 2c6e 3d3e  ener("click",n=>
-000551e0: 7b74 6869 732e 696e 7075 7445 6c65 6d65  {this.inputEleme
-000551f0: 6e74 2e66 6f63 7573 2829 2c74 6869 732e  nt.focus(),this.
-00055200: 696e 7075 7445 6c65 6d65 6e74 2e73 6574  inputElement.set
-00055210: 5365 6c65 6374 696f 6e52 616e 6765 2830  SelectionRange(0
-00055220: 2c30 292c 6e2e 7374 6f70 5072 6f70 6167  ,0),n.stopPropag
-00055230: 6174 696f 6e28 297d 292c 7468 6973 2e73  ation()}),this.s
-00055240: 7566 6669 7854 6578 7445 6c65 6d65 6e74  uffixTextElement
-00055250: 2e61 6464 4576 656e 744c 6973 7465 6e65  .addEventListene
-00055260: 7228 2263 6c69 636b 222c 6e3d 3e7b 7468  r("click",n=>{th
-00055270: 6973 2e69 6e70 7574 456c 656d 656e 742e  is.inputElement.
-00055280: 666f 6375 7328 292c 7468 6973 2e69 6e70  focus(),this.inp
-00055290: 7574 456c 656d 656e 742e 7365 7453 656c  utElement.setSel
-000552a0: 6563 7469 6f6e 5261 6e67 6528 7468 6973  ectionRange(this
-000552b0: 2e69 6e70 7574 456c 656d 656e 742e 7661  .inputElement.va
-000552c0: 6c75 652e 6c65 6e67 7468 2c74 6869 732e  lue.length,this.
-000552d0: 696e 7075 7445 6c65 6d65 6e74 2e76 616c  inputElement.val
-000552e0: 7565 2e6c 656e 6774 6829 2c6e 2e73 746f  ue.length),n.sto
-000552f0: 7050 726f 7061 6761 7469 6f6e 2829 7d29  pPropagation()})
-00055300: 2c74 6869 732e 696e 7075 7445 6c65 6d65  ,this.inputEleme
-00055310: 6e74 2e61 6464 4576 656e 744c 6973 7465  nt.addEventListe
-00055320: 6e65 7228 226d 6f75 7365 646f 776e 222c  ner("mousedown",
-00055330: 6e3d 3e7b 6e2e 7374 6f70 5072 6f70 6167  n=>{n.stopPropag
-00055340: 6174 696f 6e28 297d 292c 657d 7570 6461  ation()}),e}upda
-00055350: 7465 456c 656d 656e 7428 652c 6e29 7b65  teElement(e,n){e
-00055360: 2e74 6578 7421 3d3d 766f 6964 2030 2626  .text!==void 0&&
-00055370: 2874 6869 732e 696e 7075 7445 6c65 6d65  (this.inputEleme
-00055380: 6e74 2e76 616c 7565 3d65 2e74 6578 7429  nt.value=e.text)
-00055390: 2c65 2e6c 6162 656c 213d 3d76 6f69 6420  ,e.label!==void 
-000553a0: 3026 2628 7468 6973 2e6c 6162 656c 456c  0&&(this.labelEl
-000553b0: 656d 656e 742e 7465 7874 436f 6e74 656e  ement.textConten
-000553c0: 743d 652e 6c61 6265 6c2c 246e 2874 6869  t=e.label,$n(thi
-000553d0: 732c 652e 6c61 6265 6c2c 3029 292c 652e  s,e.label,0)),e.
-000553e0: 7072 6566 6978 5f74 6578 743d 3d3d 2222  prefix_text===""
-000553f0: 3f28 7468 6973 2e70 7265 6669 7854 6578  ?(this.prefixTex
-00055400: 7445 6c65 6d65 6e74 2e73 7479 6c65 2e64  tElement.style.d
-00055410: 6973 706c 6179 3d22 6e6f 6e65 222c 7468  isplay="none",th
-00055420: 6973 2e70 7265 6669 7854 6578 7457 6964  is.prefixTextWid
-00055430: 7468 3d30 2c74 6869 732e 696e 7075 7445  th=0,this.inputE
-00055440: 6c65 6d65 6e74 2e73 7479 6c65 2e70 6164  lement.style.pad
-00055450: 6469 6e67 4c65 6674 3d60 247b 4f6e 7d72  dingLeft=`${On}r
-00055460: 656d 602c 7468 6973 2e6d 616b 654c 6179  em`,this.makeLay
-00055470: 6f75 7444 6972 7479 2829 293a 652e 7072  outDirty()):e.pr
-00055480: 6566 6978 5f74 6578 7421 3d3d 766f 6964  efix_text!==void
-00055490: 2030 2626 2874 6869 732e 7072 6566 6978   0&&(this.prefix
-000554a0: 5465 7874 456c 656d 656e 742e 7465 7874  TextElement.text
-000554b0: 436f 6e74 656e 743d 652e 7072 6566 6978  Content=e.prefix
-000554c0: 5f74 6578 742c 7468 6973 2e70 7265 6669  _text,this.prefi
-000554d0: 7854 6578 7445 6c65 6d65 6e74 2e73 7479  xTextElement.sty
-000554e0: 6c65 2e72 656d 6f76 6550 726f 7065 7274  le.removePropert
-000554f0: 7928 2264 6973 706c 6179 2229 2c74 6869  y("display"),thi
-00055500: 732e 696e 7075 7445 6c65 6d65 6e74 2e73  s.inputElement.s
-00055510: 7479 6c65 2e72 656d 6f76 6550 726f 7065  tyle.removePrope
-00055520: 7274 7928 2270 6164 6469 6e67 2d6c 6566  rty("padding-lef
-00055530: 7422 292c 7468 6973 2e70 7265 6669 7854  t"),this.prefixT
-00055540: 6578 7457 6964 7468 3d6b 6528 652e 7072  extWidth=ke(e.pr
-00055550: 6566 6978 5f74 6578 742c 2274 6578 7422  efix_text,"text"
-00055560: 295b 305d 2b2e 322c 7468 6973 2e6d 616b  )[0]+.2,this.mak
-00055570: 654c 6179 6f75 7444 6972 7479 2829 292c  eLayoutDirty()),
-00055580: 652e 7375 6666 6978 5f74 6578 743d 3d3d  e.suffix_text===
-00055590: 2222 3f28 7468 6973 2e73 7566 6669 7854  ""?(this.suffixT
-000555a0: 6578 7445 6c65 6d65 6e74 2e73 7479 6c65  extElement.style
-000555b0: 2e64 6973 706c 6179 3d22 6e6f 6e65 222c  .display="none",
-000555c0: 7468 6973 2e73 7566 6669 7854 6578 7457  this.suffixTextW
-000555d0: 6964 7468 3d30 2c74 6869 732e 696e 7075  idth=0,this.inpu
-000555e0: 7445 6c65 6d65 6e74 2e73 7479 6c65 2e70  tElement.style.p
-000555f0: 6164 6469 6e67 5269 6768 743d 6024 7b4f  addingRight=`${O
-00055600: 6e7d 7265 6d60 2c74 6869 732e 6d61 6b65  n}rem`,this.make
-00055610: 4c61 796f 7574 4469 7274 7928 2929 3a65  LayoutDirty()):e
-00055620: 2e73 7566 6669 785f 7465 7874 213d 3d76  .suffix_text!==v
-00055630: 6f69 6420 3026 2628 7468 6973 2e73 7566  oid 0&&(this.suf
-00055640: 6669 7854 6578 7445 6c65 6d65 6e74 2e74  fixTextElement.t
-00055650: 6578 7443 6f6e 7465 6e74 3d65 2e73 7566  extContent=e.suf
-00055660: 6669 785f 7465 7874 2c74 6869 732e 7375  fix_text,this.su
-00055670: 6666 6978 5465 7874 456c 656d 656e 742e  ffixTextElement.
-00055680: 7374 796c 652e 7265 6d6f 7665 5072 6f70  style.removeProp
-00055690: 6572 7479 2822 6469 7370 6c61 7922 292c  erty("display"),
-000556a0: 7468 6973 2e69 6e70 7574 456c 656d 656e  this.inputElemen
-000556b0: 742e 7374 796c 652e 7265 6d6f 7665 5072  t.style.removePr
-000556c0: 6f70 6572 7479 2822 7061 6464 696e 672d  operty("padding-
-000556d0: 7269 6768 7422 292c 7468 6973 2e73 7566  right"),this.suf
-000556e0: 6669 7854 6578 7457 6964 7468 3d6b 6528  fixTextWidth=ke(
-000556f0: 652e 7375 6666 6978 5f74 6578 742c 2274  e.suffix_text,"t
-00055700: 6578 7422 295b 305d 2b2e 322c 7468 6973  ext")[0]+.2,this
-00055710: 2e6d 616b 654c 6179 6f75 7444 6972 7479  .makeLayoutDirty
-00055720: 2829 292c 652e 6973 5f73 6563 7265 7421  ()),e.is_secret!
-00055730: 3d3d 766f 6964 2030 2626 2874 6869 732e  ==void 0&&(this.
-00055740: 696e 7075 7445 6c65 6d65 6e74 2e74 7970  inputElement.typ
-00055750: 653d 652e 6973 5f73 6563 7265 743f 2270  e=e.is_secret?"p
-00055760: 6173 7377 6f72 6422 3a22 7465 7874 2229  assword":"text")
-00055770: 2c65 2e69 735f 7365 6e73 6974 6976 653d  ,e.is_sensitive=
-00055780: 3d3d 2130 3f28 7468 6973 2e69 6e70 7574  ==!0?(this.input
-00055790: 456c 656d 656e 742e 6469 7361 626c 6564  Element.disabled
-000557a0: 3d21 312c 7468 6973 2e65 6c65 6d65 6e74  =!1,this.element
-000557b0: 2e63 6c61 7373 4c69 7374 2e72 656d 6f76  .classList.remov
-000557c0: 6528 2272 696f 2d64 6973 6162 6c65 642d  e("rio-disabled-
-000557d0: 696e 7075 7422 2929 3a65 2e69 735f 7365  input")):e.is_se
-000557e0: 6e73 6974 6976 653d 3d3d 2131 2626 2874  nsitive===!1&&(t
-000557f0: 6869 732e 696e 7075 7445 6c65 6d65 6e74  his.inputElement
-00055800: 2e64 6973 6162 6c65 643d 2130 2c74 6869  .disabled=!0,thi
-00055810: 732e 656c 656d 656e 742e 636c 6173 734c  s.element.classL
-00055820: 6973 742e 6164 6428 2272 696f 2d64 6973  ist.add("rio-dis
-00055830: 6162 6c65 642d 696e 7075 7422 2929 2c65  abled-input")),e
-00055840: 2e69 735f 7661 6c69 643d 3d3d 2131 3f74  .is_valid===!1?t
-00055850: 6869 732e 656c 656d 656e 742e 7374 796c  his.element.styl
-00055860: 652e 7365 7450 726f 7065 7274 7928 222d  e.setProperty("-
-00055870: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
-00055880: 636f 6c6f 7222 2c22 7661 7228 2d2d 7269  color","var(--ri
-00055890: 6f2d 676c 6f62 616c 2d64 616e 6765 722d  o-global-danger-
-000558a0: 6267 2922 293a 652e 6973 5f76 616c 6964  bg)"):e.is_valid
-000558b0: 3d3d 3d21 3026 2674 6869 732e 656c 656d  ===!0&&this.elem
-000558c0: 656e 742e 7374 796c 652e 7265 6d6f 7665  ent.style.remove
-000558d0: 5072 6f70 6572 7479 2822 2d2d 7269 6f2d  Property("--rio-
-000558e0: 6c6f 6361 6c2d 7465 7874 2d63 6f6c 6f72  local-text-color
-000558f0: 2229 7d67 7261 624b 6579 626f 6172 6446  ")}grabKeyboardF
-00055900: 6f63 7573 2829 7b74 6869 732e 696e 7075  ocus(){this.inpu
-00055910: 7445 6c65 6d65 6e74 2e66 6f63 7573 2829  tElement.focus()
-00055920: 7d75 7064 6174 654e 6174 7572 616c 5769  }updateNaturalWi
-00055930: 6474 6828 6529 7b55 6e28 7468 6973 2c74  dth(e){Un(this,t
-00055940: 6869 732e 7072 6566 6978 5465 7874 5769  his.prefixTextWi
-00055950: 6474 682b 7468 6973 2e73 7566 6669 7854  dth+this.suffixT
-00055960: 6578 7457 6964 7468 297d 7570 6461 7465  extWidth)}update
-00055970: 4e61 7475 7261 6c48 6569 6768 7428 6529  NaturalHeight(e)
-00055980: 7b7d 7d63 6c61 7373 2049 7520 6578 7465  {}}class Iu exte
-00055990: 6e64 7320 4965 7b63 7265 6174 6545 6c65  nds Ie{createEle
-000559a0: 6d65 6e74 2829 7b72 6574 7572 6e20 646f  ment(){return do
-000559b0: 6375 6d65 6e74 2e63 7265 6174 6545 6c65  cument.createEle
-000559c0: 6d65 6e74 2822 6469 7622 297d 7570 6461  ment("div")}upda
-000559d0: 7465 456c 656d 656e 7428 652c 6e29 7b74  teElement(e,n){t
-000559e0: 6869 732e 7265 706c 6163 654f 6e6c 7943  his.replaceOnlyC
-000559f0: 6869 6c64 286e 2c65 2e63 6f6e 7465 6e74  hild(n,e.content
-00055a00: 292c 652e 636f 6c6f 7221 3d3d 766f 6964  ),e.color!==void
-00055a10: 2030 2626 2465 2874 6869 732e 656c 656d   0&&$e(this.elem
-00055a20: 656e 742c 652e 636f 6c6f 7229 7d7d 636c  ent,e.color)}}cl
-00055a30: 6173 7320 4c75 2065 7874 656e 6473 2055  ass Lu extends U
-00055a40: 7b63 7265 6174 6545 6c65 6d65 6e74 2829  {createElement()
-00055a50: 7b6c 6574 2065 3d64 6f63 756d 656e 742e  {let e=document.
-00055a60: 6372 6561 7465 456c 656d 656e 7428 2264  createElement("d
-00055a70: 6976 2229 3b72 6574 7572 6e20 652e 636c  iv");return e.cl
-00055a80: 6173 734c 6973 742e 6164 6428 2272 696f  assList.add("rio
-00055a90: 2d74 6f6f 6c74 6970 2229 2c65 2e69 6e6e  -tooltip"),e.inn
-00055aa0: 6572 4854 4d4c 3d60 0a20 2020 2020 2020  erHTML=`.       
-00055ab0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00055ac0: 2272 696f 2d74 6f6f 6c74 6970 2d61 6e63  "rio-tooltip-anc
-00055ad0: 686f 7222 3e3c 2f64 6976 3e0a 2020 2020  hor"></div>.    
-00055ae0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00055af0: 7373 3d22 7269 6f2d 746f 6f6c 7469 702d  ss="rio-tooltip-
-00055b00: 6c61 6265 6c20 7269 6f2d 7377 6974 6368  label rio-switch
-00055b10: 6572 6f6f 2d68 7564 223e 3c2f 6469 763e  eroo-hud"></div>
-00055b20: 0a20 2020 2020 2020 2060 2c74 6869 732e  .        `,this.
-00055b30: 616e 6368 6f72 436f 6e74 6169 6e65 723d  anchorContainer=
-00055b40: 652e 7175 6572 7953 656c 6563 746f 7228  e.querySelector(
-00055b50: 222e 7269 6f2d 746f 6f6c 7469 702d 616e  ".rio-tooltip-an
-00055b60: 6368 6f72 2229 2c74 6869 732e 6c61 6265  chor"),this.labe
-00055b70: 6c45 6c65 6d65 6e74 3d65 2e71 7565 7279  lElement=e.query
-00055b80: 5365 6c65 6374 6f72 2822 2e72 696f 2d74  Selector(".rio-t
-00055b90: 6f6f 6c74 6970 2d6c 6162 656c 2229 2c74  ooltip-label"),t
-00055ba0: 6869 732e 616e 6368 6f72 436f 6e74 6169  his.anchorContai
-00055bb0: 6e65 722e 6164 6445 7665 6e74 4c69 7374  ner.addEventList
-00055bc0: 656e 6572 2822 6d6f 7573 656f 7665 7222  ener("mouseover"
-00055bd0: 2c28 293d 3e7b 7468 6973 2e6c 6162 656c  ,()=>{this.label
-00055be0: 456c 656d 656e 742e 7374 796c 652e 6f70  Element.style.op
-00055bf0: 6163 6974 793d 2231 227d 292c 7468 6973  acity="1"}),this
-00055c00: 2e61 6e63 686f 7243 6f6e 7461 696e 6572  .anchorContainer
-00055c10: 2e61 6464 4576 656e 744c 6973 7465 6e65  .addEventListene
-00055c20: 7228 226d 6f75 7365 6f75 7422 2c28 293d  r("mouseout",()=
-00055c30: 3e7b 7468 6973 2e6c 6162 656c 456c 656d  >{this.labelElem
-00055c40: 656e 742e 7374 796c 652e 6f70 6163 6974  ent.style.opacit
-00055c50: 793d 2230 227d 292c 657d 7570 6461 7465  y="0"}),e}update
-00055c60: 456c 656d 656e 7428 652c 6e29 7b69 6628  Element(e,n){if(
-00055c70: 652e 616e 6368 6f72 213d 3d76 6f69 6420  e.anchor!==void 
-00055c80: 3026 2674 6869 732e 7265 706c 6163 654f  0&&this.replaceO
-00055c90: 6e6c 7943 6869 6c64 286e 2c65 2e61 6e63  nlyChild(n,e.anc
-00055ca0: 686f 722c 7468 6973 2e61 6e63 686f 7243  hor,this.anchorC
-00055cb0: 6f6e 7461 696e 6572 292c 652e 5f74 6970  ontainer),e._tip
-00055cc0: 5f63 6f6d 706f 6e65 6e74 213d 3d76 6f69  _component!==voi
-00055cd0: 6420 3026 2674 6869 732e 7265 706c 6163  d 0&&this.replac
-00055ce0: 654f 6e6c 7943 6869 6c64 286e 2c65 2e5f  eOnlyChild(n,e._
-00055cf0: 7469 705f 636f 6d70 6f6e 656e 742c 7468  tip_component,th
-00055d00: 6973 2e6c 6162 656c 456c 656d 656e 7429  is.labelElement)
-00055d10: 2c65 2e70 6f73 6974 696f 6e21 3d3d 766f  ,e.position!==vo
-00055d20: 6964 2030 297b 6c65 7420 692c 722c 732c  id 0){let i,r,s,
-00055d30: 612c 6f3b 636f 6e73 7420 633d 2263 616c  a,o;const c="cal
-00055d40: 6328 3130 3025 202b 2030 2e35 7265 6d29  c(100% + 0.5rem)
-00055d50: 223b 652e 706f 7369 7469 6f6e 3d3d 3d22  ";e.position==="
-00055d60: 6c65 6674 223f 2869 3d22 756e 7365 7422  left"?(i="unset"
-00055d70: 2c72 3d22 3530 2522 2c73 3d63 2c61 3d22  ,r="50%",s=c,a="
-00055d80: 756e 7365 7422 2c6f 3d22 7472 616e 736c  unset",o="transl
-00055d90: 6174 6559 282d 3530 2529 2229 3a65 2e70  ateY(-50%)"):e.p
-00055da0: 6f73 6974 696f 6e3d 3d3d 2274 6f70 223f  osition==="top"?
-00055db0: 2869 3d22 3530 2522 2c72 3d22 756e 7365  (i="50%",r="unse
-00055dc0: 7422 2c73 3d22 756e 7365 7422 2c61 3d63  t",s="unset",a=c
-00055dd0: 2c6f 3d22 7472 616e 736c 6174 6558 282d  ,o="translateX(-
-00055de0: 3530 2529 2229 3a65 2e70 6f73 6974 696f  50%)"):e.positio
-00055df0: 6e3d 3d3d 2272 6967 6874 223f 2869 3d63  n==="right"?(i=c
-00055e00: 2c72 3d22 3530 2522 2c73 3d22 756e 7365  ,r="50%",s="unse
-00055e10: 7422 2c61 3d22 756e 7365 7422 2c6f 3d22  t",a="unset",o="
-00055e20: 7472 616e 736c 6174 6559 282d 3530 2529  translateY(-50%)
-00055e30: 2229 3a28 693d 2235 3025 222c 723d 632c  "):(i="50%",r=c,
-00055e40: 733d 2275 6e73 6574 222c 613d 2275 6e73  s="unset",a="uns
-00055e50: 6574 222c 6f3d 2274 7261 6e73 6c61 7465  et",o="translate
-00055e60: 5828 2d35 3025 2922 292c 7468 6973 2e6c  X(-50%)"),this.l
-00055e70: 6162 656c 456c 656d 656e 742e 7374 796c  abelElement.styl
-00055e80: 652e 6c65 6674 3d69 2c74 6869 732e 6c61  e.left=i,this.la
-00055e90: 6265 6c45 6c65 6d65 6e74 2e73 7479 6c65  belElement.style
-00055ea0: 2e74 6f70 3d72 2c74 6869 732e 6c61 6265  .top=r,this.labe
-00055eb0: 6c45 6c65 6d65 6e74 2e73 7479 6c65 2e72  lElement.style.r
-00055ec0: 6967 6874 3d73 2c74 6869 732e 6c61 6265  ight=s,this.labe
-00055ed0: 6c45 6c65 6d65 6e74 2e73 7479 6c65 2e62  lElement.style.b
-00055ee0: 6f74 746f 6d3d 612c 7468 6973 2e6c 6162  ottom=a,this.lab
-00055ef0: 656c 456c 656d 656e 742e 7374 796c 652e  elElement.style.
-00055f00: 7472 616e 7366 6f72 6d3d 6f7d 7d75 7064  transform=o}}upd
-00055f10: 6174 654e 6174 7572 616c 5769 6474 6828  ateNaturalWidth(
-00055f20: 6529 7b74 6869 732e 6e61 7475 7261 6c57  e){this.naturalW
-00055f30: 6964 7468 3d43 5b74 6869 732e 7374 6174  idth=C[this.stat
-00055f40: 652e 616e 6368 6f72 5d2e 7265 7175 6573  e.anchor].reques
-00055f50: 7465 6457 6964 7468 7d75 7064 6174 6541  tedWidth}updateA
-00055f60: 6c6c 6f63 6174 6564 5769 6474 6828 6529  llocatedWidth(e)
-00055f70: 7b6c 6574 206e 3d43 5b74 6869 732e 7374  {let n=C[this.st
-00055f80: 6174 652e 616e 6368 6f72 5d2c 693d 435b  ate.anchor],i=C[
-00055f90: 7468 6973 2e73 7461 7465 2e5f 7469 705f  this.state._tip_
-00055fa0: 636f 6d70 6f6e 656e 745d 3b6e 2e61 6c6c  component];n.all
-00055fb0: 6f63 6174 6564 5769 6474 683d 7468 6973  ocatedWidth=this
-00055fc0: 2e61 6c6c 6f63 6174 6564 5769 6474 682c  .allocatedWidth,
-00055fd0: 692e 616c 6c6f 6361 7465 6457 6964 7468  i.allocatedWidth
-00055fe0: 3d69 2e6e 6174 7572 616c 5769 6474 687d  =i.naturalWidth}
-00055ff0: 7570 6461 7465 4e61 7475 7261 6c48 6569  updateNaturalHei
-00056000: 6768 7428 6529 7b74 6869 732e 6e61 7475  ght(e){this.natu
-00056010: 7261 6c48 6569 6768 743d 435b 7468 6973  ralHeight=C[this
-00056020: 2e73 7461 7465 2e61 6e63 686f 725d 2e72  .state.anchor].r
-00056030: 6571 7565 7374 6564 4865 6967 6874 7d75  equestedHeight}u
-00056040: 7064 6174 6541 6c6c 6f63 6174 6564 4865  pdateAllocatedHe
-00056050: 6967 6874 2865 297b 6c65 7420 6e3d 435b  ight(e){let n=C[
-00056060: 7468 6973 2e73 7461 7465 2e61 6e63 686f  this.state.ancho
-00056070: 725d 2c69 3d43 5b74 6869 732e 7374 6174  r],i=C[this.stat
-00056080: 652e 5f74 6970 5f63 6f6d 706f 6e65 6e74  e._tip_component
-00056090: 5d3b 6e2e 616c 6c6f 6361 7465 6448 6569  ];n.allocatedHei
-000560a0: 6768 743d 7468 6973 2e61 6c6c 6f63 6174  ght=this.allocat
-000560b0: 6564 4865 6967 6874 2c69 2e61 6c6c 6f63  edHeight,i.alloc
-000560c0: 6174 6564 4865 6967 6874 3d69 2e6e 6174  atedHeight=i.nat
-000560d0: 7572 616c 4865 6967 6874 2c6e 2e65 6c65  uralHeight,n.ele
-000560e0: 6d65 6e74 2e73 7479 6c65 2e6c 6566 743d  ment.style.left=
-000560f0: 2230 222c 6e2e 656c 656d 656e 742e 7374  "0",n.element.st
-00056100: 796c 652e 746f 703d 2230 222c 692e 656c  yle.top="0",i.el
-00056110: 656d 656e 742e 7374 796c 652e 6c65 6674  ement.style.left
-00056120: 3d22 3022 2c69 2e65 6c65 6d65 6e74 2e73  ="0",i.element.s
-00056130: 7479 6c65 2e74 6f70 3d22 3022 7d7d 636f  tyle.top="0"}}co
-00056140: 6e73 7420 6f73 3d7b 2241 6c69 676e 2d62  nst os={"Align-b
-00056150: 7569 6c74 696e 223a 4f73 2c22 4275 696c  uiltin":Os,"Buil
-00056160: 6446 6169 6c65 642d 6275 696c 7469 6e22  dFailed-builtin"
-00056170: 3a48 732c 2242 7574 746f 6e2d 6275 696c  :Hs,"Button-buil
-00056180: 7469 6e22 3a46 732c 2243 6172 642d 6275  tin":Fs,"Card-bu
-00056190: 696c 7469 6e22 3a57 732c 2243 6c61 7373  iltin":Ws,"Class
-000561a0: 436f 6e74 6169 6e65 722d 6275 696c 7469  Container-builti
-000561b0: 6e22 3a55 732c 2243 6f64 6542 6c6f 636b  n":Us,"CodeBlock
-000561c0: 2d62 7569 6c74 696e 223a 796f 2c22 436f  -builtin":yo,"Co
-000561d0: 6465 4578 706c 6f72 6572 2d62 7569 6c74  deExplorer-built
-000561e0: 696e 223a 766f 2c22 436f 6c6f 7250 6963  in":vo,"ColorPic
-000561f0: 6b65 722d 6275 696c 7469 6e22 3a78 6f2c  ker-builtin":xo,
-00056200: 2243 6f6c 756d 6e2d 6275 696c 7469 6e22  "Column-builtin"
-00056210: 3a47 722c 2243 6f6d 706f 6e65 6e74 5472  :Gr,"ComponentTr
-00056220: 6565 2d62 7569 6c74 696e 223a 6b6f 2c22  ee-builtin":ko,"
-00056230: 4375 7374 6f6d 4c69 7374 4974 656d 2d62  CustomListItem-b
-00056240: 7569 6c74 696e 223a 5672 2c22 4465 6275  uiltin":Vr,"Debu
-00056250: 6767 6572 436f 6e6e 6563 746f 722d 6275  ggerConnector-bu
-00056260: 696c 7469 6e22 3a4e 6f2c 2244 7261 7765  iltin":No,"Drawe
-00056270: 722d 6275 696c 7469 6e22 3a54 6f2c 2244  r-builtin":To,"D
-00056280: 726f 7064 6f77 6e2d 6275 696c 7469 6e22  ropdown-builtin"
-00056290: 3a41 6f2c 2246 6c6f 7743 6f6e 7461 696e  :Ao,"FlowContain
-000562a0: 6572 2d62 7569 6c74 696e 223a 4f6f 2c22  er-builtin":Oo,"
-000562b0: 4675 6e64 616d 656e 7461 6c52 6f6f 7443  FundamentalRootC
-000562c0: 6f6d 706f 6e65 6e74 2d62 7569 6c74 696e  omponent-builtin
-000562d0: 223a 526f 2c22 4772 6964 2d62 7569 6c74  ":Ro,"Grid-built
-000562e0: 696e 223a 4d6f 2c22 4865 6164 696e 674c  in":Mo,"HeadingL
-000562f0: 6973 7449 7465 6d2d 6275 696c 7469 6e22  istItem-builtin"
-00056300: 3a59 722c 2248 746d 6c2d 6275 696c 7469  :Yr,"Html-builti
-00056310: 6e22 3a49 6f2c 2249 636f 6e2d 6275 696c  n":Io,"Icon-buil
-00056320: 7469 6e22 3a44 6f2c 2249 6d61 6765 2d62  tin":Do,"Image-b
-00056330: 7569 6c74 696e 223a 426f 2c22 4b65 7945  uiltin":Bo,"KeyE
-00056340: 7665 6e74 4c69 7374 656e 6572 2d62 7569  ventListener-bui
-00056350: 6c74 696e 223a 576f 2c22 4c69 6e6b 2d62  ltin":Wo,"Link-b
-00056360: 7569 6c74 696e 223a 556f 2c22 4c69 7374  uiltin":Uo,"List
-00056370: 5669 6577 2d62 7569 6c74 696e 223a 246f  View-builtin":$o
-00056380: 2c22 4d61 7267 696e 2d62 7569 6c74 696e  ,"Margin-builtin
-00056390: 223a 7a6f 2c22 4d61 726b 646f 776e 2d62  ":zo,"Markdown-b
-000563a0: 7569 6c74 696e 223a 5163 2c22 4d65 6469  uiltin":Qc,"Medi
-000563b0: 6150 6c61 7965 722d 6275 696c 7469 6e22  aPlayer-builtin"
-000563c0: 3a6a 632c 224d 6f75 7365 4576 656e 744c  :jc,"MouseEventL
-000563d0: 6973 7465 6e65 722d 6275 696c 7469 6e22  istener-builtin"
-000563e0: 3a74 752c 224d 756c 7469 4c69 6e65 5465  :tu,"MultiLineTe
-000563f0: 7874 496e 7075 742d 6275 696c 7469 6e22  xtInput-builtin"
-00056400: 3a6e 752c 224e 6f64 6549 6e70 7574 2d62  :nu,"NodeInput-b
-00056410: 7569 6c74 696e 223a 6975 2c22 4e6f 6465  uiltin":iu,"Node
-00056420: 4f75 7470 7574 2d62 7569 6c74 696e 223a  Output-builtin":
-00056430: 7275 2c22 4f76 6572 6c61 792d 6275 696c  ru,"Overlay-buil
-00056440: 7469 6e22 3a73 752c 2250 6c6f 742d 6275  tin":su,"Plot-bu
-00056450: 696c 7469 6e22 3a6c 752c 2250 6f70 7570  iltin":lu,"Popup
-00056460: 2d62 7569 6c74 696e 223a 6375 2c22 5072  -builtin":cu,"Pr
-00056470: 6f67 7265 7373 4261 722d 6275 696c 7469  ogressBar-builti
-00056480: 6e22 3a75 752c 2250 726f 6772 6573 7343  n":uu,"ProgressC
-00056490: 6972 636c 652d 6275 696c 7469 6e22 3a64  ircle-builtin":d
-000564a0: 752c 2252 6563 7461 6e67 6c65 2d62 7569  u,"Rectangle-bui
-000564b0: 6c74 696e 223a 7075 2c22 5265 7665 616c  ltin":pu,"Reveal
-000564c0: 6572 2d62 7569 6c74 696e 223a 6775 2c22  er-builtin":gu,"
-000564d0: 526f 772d 6275 696c 7469 6e22 3a43 6f2c  Row-builtin":Co,
-000564e0: 2253 6372 6f6c 6c43 6f6e 7461 696e 6572  "ScrollContainer
-000564f0: 2d62 7569 6c74 696e 223a 6675 2c22 5363  -builtin":fu,"Sc
-00056500: 726f 6c6c 5461 7267 6574 2d62 7569 6c74  rollTarget-built
-00056510: 696e 223a 6275 2c22 5365 7061 7261 746f  in":bu,"Separato
-00056520: 722d 6275 696c 7469 6e22 3a45 752c 2253  r-builtin":Eu,"S
-00056530: 6570 6172 6174 6f72 4c69 7374 4974 656d  eparatorListItem
-00056540: 2d62 7569 6c74 696e 223a 5a72 2c22 536c  -builtin":Zr,"Sl
-00056550: 6964 6572 2d62 7569 6c74 696e 223a 5f75  ider-builtin":_u
-00056560: 2c22 536c 6964 6573 686f 772d 6275 696c  ,"Slideshow-buil
-00056570: 7469 6e22 3a76 752c 2253 7461 636b 2d62  tin":vu,"Stack-b
-00056580: 7569 6c74 696e 223a 7775 2c22 5377 6974  uiltin":wu,"Swit
-00056590: 6368 2d62 7569 6c74 696e 223a 7875 2c22  ch-builtin":xu,"
-000565a0: 5377 6974 6368 6572 2d62 7569 6c74 696e  Switcher-builtin
-000565b0: 223a 5475 2c22 5377 6974 6368 6572 4261  ":Tu,"SwitcherBa
-000565c0: 722d 6275 696c 7469 6e22 3a6b 752c 2254  r-builtin":ku,"T
-000565d0: 6162 6c65 2d62 7569 6c74 696e 223a 4f75  able-builtin":Ou
-000565e0: 2c22 5465 7874 2d62 7569 6c74 696e 223a  ,"Text-builtin":
-000565f0: 5275 2c22 5465 7874 496e 7075 742d 6275  Ru,"TextInput-bu
-00056600: 696c 7469 6e22 3a4d 752c 2254 6865 6d65  iltin":Mu,"Theme
-00056610: 436f 6e74 6578 7453 7769 7463 6865 722d  ContextSwitcher-
-00056620: 6275 696c 7469 6e22 3a49 752c 2254 6f6f  builtin":Iu,"Too
-00056630: 6c74 6970 2d62 7569 6c74 696e 223a 4c75  ltip-builtin":Lu
-00056640: 2c50 6c61 6365 686f 6c64 6572 3a61 757d  ,Placeholder:au}
-00056650: 3b67 6c6f 6261 6c54 6869 732e 434f 4d50  ;globalThis.COMP
-00056660: 4f4e 454e 545f 434c 4153 5345 533d 6f73  ONENT_CLASSES=os
-00056670: 3b63 6f6e 7374 2043 3d7b 7d2c 5665 3d6e  ;const C={},Ve=n
-00056680: 6577 204d 6170 3b66 756e 6374 696f 6e20  ew Map;function 
-00056690: 6474 2829 7b6c 6574 2074 3d64 6f63 756d  dt(){let t=docum
-000566a0: 656e 742e 626f 6479 2e71 7565 7279 5365  ent.body.querySe
-000566b0: 6c65 6374 6f72 2822 2e72 696f 2d66 756e  lector(".rio-fun
-000566c0: 6461 6d65 6e74 616c 2d72 6f6f 742d 636f  damental-root-co
-000566d0: 6d70 6f6e 656e 7422 293b 7265 7475 726e  mponent");return
-000566e0: 2063 6f6e 736f 6c65 2e61 7373 6572 7428   console.assert(
-000566f0: 7421 3d3d 6e75 6c6c 2c22 436f 756c 646e  t!==null,"Couldn
-00056700: 2774 2066 696e 6420 7468 6520 726f 6f74  't find the root
-00056710: 2063 6f6d 706f 6e65 6e74 2069 6e20 7468   component in th
-00056720: 6520 646f 6375 6d65 6e74 2062 6f64 7922  e document body"
-00056730: 292c 5665 2e67 6574 2874 297d 6675 6e63  ),Ve.get(t)}func
-00056740: 7469 6f6e 206c 7328 297b 6c65 7420 743d  tion ls(){let t=
-00056750: 6474 2829 3b72 6574 7572 6e20 435b 742e  dt();return C[t.
-00056760: 7374 6174 652e 636f 6e74 656e 745d 7d67  state.content]}g
-00056770: 6c6f 6261 6c54 6869 732e 6765 7452 6f6f  lobalThis.getRoo
-00056780: 7453 6372 6f6c 6c65 723d 6c73 3b66 756e  tScroller=ls;fun
-00056790: 6374 696f 6e20 4b65 2874 297b 6c65 7420  ction Ke(t){let 
-000567a0: 653d 4374 2874 293b 6966 2865 3d3d 3d6e  e=Ct(t);if(e===n
-000567b0: 756c 6c29 7b6c 6574 206e 3d74 2e70 6172  ull){let n=t.par
-000567c0: 656e 7445 6c65 6d65 6e74 3b66 6f72 283b  entElement;for(;
-000567d0: 6e3b 297b 6966 2865 3d43 7428 6e29 2c65  n;){if(e=Ct(n),e
-000567e0: 213d 3d6e 756c 6c29 7468 726f 7760 456c  !==null)throw`El
-000567f0: 656d 656e 7420 247b 516e 2874 297d 2064  ement ${Qn(t)} d
-00056800: 6f65 7320 6e6f 7420 636f 7272 6573 706f  oes not correspo
-00056810: 6e64 2074 6f20 6120 636f 6d70 6f6e 656e  nd to a componen
-00056820: 742e 2049 7420 6973 2061 2063 6869 6c64  t. It is a child
-00056830: 2065 6c65 6d65 6e74 206f 6620 247b 652e   element of ${e.
-00056840: 746f 5374 7269 6e67 2829 7d60 3b6e 3d6e  toString()}`;n=n
-00056850: 2e70 6172 656e 7445 6c65 6d65 6e74 7d74  .parentElement}t
-00056860: 6872 6f77 6045 6c65 6d65 6e74 2024 7b51  hrow`Element ${Q
-00056870: 6e28 7429 7d20 646f 6573 206e 6f74 2063  n(t)} does not c
-00056880: 6f72 7265 7370 6f6e 6420 746f 2061 2063  orrespond to a c
-00056890: 6f6d 706f 6e65 6e74 2028 616e 6420 6e6f  omponent (and no
-000568a0: 6e65 206f 6620 6974 7320 7061 7265 6e74  ne of its parent
-000568b0: 2065 6c65 6d65 6e74 7320 636f 7272 6573   elements corres
-000568c0: 706f 6e64 2074 6f20 6120 636f 6d70 6f6e  pond to a compon
-000568d0: 656e 742c 2065 6974 6865 7229 607d 7265  ent, either)`}re
-000568e0: 7475 726e 2065 7d67 6c6f 6261 6c54 6869  turn e}globalThi
-000568f0: 732e 636f 6d70 6f6e 656e 7473 4279 4964  s.componentsById
-00056900: 3d43 3b67 6c6f 6261 6c54 6869 732e 6765  =C;globalThis.ge
-00056910: 7449 6e73 7461 6e63 6542 7945 6c65 6d65  tInstanceByEleme
-00056920: 6e74 3d4b 653b 6675 6e63 7469 6f6e 2043  nt=Ke;function C
-00056930: 7428 7429 7b72 6574 7572 6e20 5665 2e67  t(t){return Ve.g
-00056940: 6574 2874 293f 3f6e 756c 6c7d 6675 6e63  et(t)??null}func
-00056950: 7469 6f6e 2044 7528 7429 7b72 6574 7572  tion Du(t){retur
-00056960: 6e20 5665 2e68 6173 2874 297d 6675 6e63  n Ve.has(t)}func
-00056970: 7469 6f6e 2050 7528 742c 6529 7b6c 6574  tion Pu(t,e){let
-00056980: 206e 3d43 5b74 5d3b 7265 7475 726e 206e   n=C[t];return n
-00056990: 3d3d 3d76 6f69 6420 303f 653a 7b2e 2e2e  ===void 0?e:{...
-000569a0: 6e2e 7374 6174 652c 2e2e 2e65 7d7d 6675  n.state,...e}}fu
-000569b0: 6e63 7469 6f6e 2066 7228 742c 6529 7b6c  nction fr(t,e){l
-000569c0: 6574 206e 3d65 5b74 5d7c 7c7b 7d2c 693d  et n=e[t]||{},i=
-000569d0: 5075 2874 2c6e 292c 723d 742c 733d 692e  Pu(t,n),r=t,s=i.
-000569e0: 5f6d 6172 6769 6e5f 3b69 6628 733d 3d3d  _margin_;if(s===
-000569f0: 766f 6964 2030 2626 636f 6e73 6f6c 652e  void 0&&console.
-00056a00: 6572 726f 7228 6047 6f74 2069 6e63 6f6d  error(`Got incom
-00056a10: 706c 6574 6520 7374 6174 6520 666f 7220  plete state for 
-00056a20: 636f 6d70 6f6e 656e 7420 247b 747d 6029  component ${t}`)
-00056a30: 2c73 5b30 5d21 3d3d 307c 7c73 5b31 5d21  ,s[0]!==0||s[1]!
-00056a40: 3d3d 307c 7c73 5b32 5d21 3d3d 307c 7c73  ==0||s[2]!==0||s
-00056a50: 5b33 5d21 3d3d 3029 7b6c 6574 206f 3d74  [3]!==0){let o=t
-00056a60: 2a2d 3130 3b65 5b6f 5d3d 7b5f 7479 7065  *-10;e[o]={_type
-00056a70: 5f3a 224d 6172 6769 6e2d 6275 696c 7469  _:"Margin-builti
-00056a80: 6e22 2c5f 7079 7468 6f6e 5f74 7970 655f  n",_python_type_
-00056a90: 3a22 4d61 7267 696e 2028 696e 6a65 6374  :"Margin (inject
-00056aa0: 6564 2922 2c5f 6b65 795f 3a6e 756c 6c2c  ed)",_key_:null,
-00056ab0: 5f6d 6172 6769 6e5f 3a5b 302c 302c 302c  _margin_:[0,0,0,
-00056ac0: 305d 2c5f 7369 7a65 5f3a 5b30 2c30 5d2c  0],_size_:[0,0],
-00056ad0: 5f67 726f 775f 3a69 2e5f 6772 6f77 5f2c  _grow_:i._grow_,
-00056ae0: 5f72 696f 5f69 6e74 6572 6e61 6c5f 3a21  _rio_internal_:!
-00056af0: 302c 636f 6e74 656e 743a 722c 6d61 7267  0,content:r,marg
-00056b00: 696e 5f6c 6566 743a 735b 305d 2c6d 6172  in_left:s[0],mar
-00056b10: 6769 6e5f 746f 703a 735b 315d 2c6d 6172  gin_top:s[1],mar
-00056b20: 6769 6e5f 7269 6768 743a 735b 325d 2c6d  gin_right:s[2],m
-00056b30: 6172 6769 6e5f 626f 7474 6f6d 3a73 5b33  argin_bottom:s[3
-00056b40: 5d7d 2c72 3d6f 7d6c 6574 2061 3d69 2e5f  ]},r=o}let a=i._
-00056b50: 616c 6967 6e5f 3b69 6628 613d 3d3d 766f  align_;if(a===vo
-00056b60: 6964 2030 2626 636f 6e73 6f6c 652e 6572  id 0&&console.er
-00056b70: 726f 7228 6047 6f74 2069 6e63 6f6d 706c  ror(`Got incompl
-00056b80: 6574 6520 7374 6174 6520 666f 7220 636f  ete state for co
-00056b90: 6d70 6f6e 656e 7420 247b 747d 6029 2c61  mponent ${t}`),a
-00056ba0: 5b30 5d21 3d3d 6e75 6c6c 7c7c 615b 315d  [0]!==null||a[1]
-00056bb0: 213d 3d6e 756c 6c29 7b6c 6574 206f 3d74  !==null){let o=t
-00056bc0: 2a2d 3130 2d31 3b65 5b6f 5d3d 7b5f 7479  *-10-1;e[o]={_ty
-00056bd0: 7065 5f3a 2241 6c69 676e 2d62 7569 6c74  pe_:"Align-built
-00056be0: 696e 222c 5f70 7974 686f 6e5f 7479 7065  in",_python_type
-00056bf0: 5f3a 2241 6c69 676e 2028 696e 6a65 6374  _:"Align (inject
-00056c00: 6564 2922 2c5f 6b65 795f 3a6e 756c 6c2c  ed)",_key_:null,
-00056c10: 5f6d 6172 6769 6e5f 3a5b 302c 302c 302c  _margin_:[0,0,0,
-00056c20: 305d 2c5f 7369 7a65 5f3a 5b30 2c30 5d2c  0],_size_:[0,0],
-00056c30: 5f67 726f 775f 3a69 2e5f 6772 6f77 5f2c  _grow_:i._grow_,
-00056c40: 5f72 696f 5f69 6e74 6572 6e61 6c5f 3a21  _rio_internal_:!
-00056c50: 302c 636f 6e74 656e 743a 722c 616c 6967  0,content:r,alig
-00056c60: 6e5f 783a 615b 305d 2c61 6c69 676e 5f79  n_x:a[0],align_y
-00056c70: 3a61 5b31 5d7d 2c72 3d6f 7d72 6574 7572  :a[1]},r=o}retur
-00056c80: 6e20 727d 6675 6e63 7469 6f6e 2062 7228  n r}function br(
-00056c90: 742c 652c 6e29 7b6c 6574 2069 3d67 6c6f  t,e,n){let i=glo
-00056ca0: 6261 6c54 6869 732e 4348 494c 445f 4154  balThis.CHILD_AT
-00056cb0: 5452 4942 5554 455f 4e41 4d45 535b 742e  TRIBUTE_NAMES[t.
-00056cc0: 5f74 7970 655f 5d7c 7c5b 5d3b 6675 6e63  _type_]||[];func
-00056cd0: 7469 6f6e 2072 2873 297b 7265 7475 726e  tion r(s){return
-00056ce0: 2073 3e3d 303f 733a 4d61 7468 2e66 6c6f   s>=0?s:Math.flo
-00056cf0: 6f72 2873 2f2d 3130 297d 666f 7228 6c65  or(s/-10)}for(le
-00056d00: 7420 7320 6f66 2069 297b 6c65 7420 613d  t s of i){let a=
-00056d10: 745b 735d 3b69 6628 4172 7261 792e 6973  t[s];if(Array.is
-00056d20: 4172 7261 7928 6129 2974 5b73 5d3d 612e  Array(a))t[s]=a.
-00056d30: 6d61 7028 6f3d 3e28 6f3d 7228 6f29 2c65  map(o=>(o=r(o),e
-00056d40: 2e61 6464 286f 292c 6672 286f 2c6e 2929  .add(o),fr(o,n))
-00056d50: 293b 656c 7365 2069 6628 6121 3d6e 756c  );else if(a!=nul
-00056d60: 6c29 7b6c 6574 206f 3d72 2861 293b 745b  l){let o=r(a);t[
-00056d70: 735d 3d66 7228 6f2c 6e29 2c65 2e61 6464  s]=fr(o,n),e.add
-00056d80: 286f 297d 7d7d 6675 6e63 7469 6f6e 2042  (o)}}}function B
-00056d90: 7528 7429 7b6c 6574 2065 3d4f 626a 6563  u(t){let e=Objec
-00056da0: 742e 6b65 7973 2874 292e 6d61 7028 693d  t.keys(t).map(i=
-00056db0: 3e70 6172 7365 496e 7428 6929 292c 6e3d  >parseInt(i)),n=
-00056dc0: 6e65 7720 5365 743b 666f 7228 6c65 7420  new Set;for(let 
-00056dd0: 6920 6f66 2065 2962 7228 745b 695d 2c6e  i of e)br(t[i],n
-00056de0: 2c74 293b 666f 7228 6c65 7420 6920 6f66  ,t);for(let i of
-00056df0: 2065 297b 6966 286e 2e68 6173 2869 2929   e){if(n.has(i))
-00056e00: 636f 6e74 696e 7565 3b6c 6574 2072 3d43  continue;let r=C
-00056e10: 5b69 5d3b 6966 2872 3d3d 3d76 6f69 6420  [i];if(r===void 
-00056e20: 3029 636f 6e74 696e 7565 3b6c 6574 2073  0)continue;let s
-00056e30: 3d72 2e67 6574 5061 7265 6e74 4578 636c  =r.getParentExcl
-00056e40: 7564 696e 6749 6e6a 6563 7465 6428 293b  udingInjected();
-00056e50: 6966 2873 3d3d 3d6e 756c 6c29 636f 6e74  if(s===null)cont
-00056e60: 696e 7565 3b6c 6574 2061 3d7b 2e2e 2e73  inue;let a={...s
-00056e70: 2e73 7461 7465 7d3b 6272 2861 2c6e 2c74  .state};br(a,n,t
-00056e80: 292c 745b 732e 6964 5d3d 617d 7d66 756e  ),t[s.id]=a}}fun
-00056e90: 6374 696f 6e20 4875 2874 2c65 297b 4275  ction Hu(t,e){Bu
-00056ea0: 2874 293b 6c65 7420 6e3d 646f 6375 6d65  (t);let n=docume
-00056eb0: 6e74 2e61 6374 6976 6545 6c65 6d65 6e74  nt.activeElement
-00056ec0: 3b66 6f72 283b 6e21 3d3d 6e75 6c6c 2626  ;for(;n!==null&&
-00056ed0: 2144 7528 6e29 3b29 6e3d 6e2e 7061 7265  !Du(n);)n=n.pare
-00056ee0: 6e74 456c 656d 656e 743b 6c65 7420 693d  ntElement;let i=
-00056ef0: 6e3d 3d3d 6e75 6c6c 3f6e 756c 6c3a 4b65  n===null?null:Ke
-00056f00: 286e 292c 723d 6e65 7720 5365 743b 666f  (n),r=new Set;fo
-00056f10: 7228 6c65 7420 7320 696e 2074 297b 6c65  r(let s in t){le
-00056f20: 7420 613d 745b 735d 3b69 6628 435b 735d  t a=t[s];if(C[s]
-00056f30: 2963 6f6e 7469 6e75 653b 636f 6e73 7420  )continue;const 
-00056f40: 633d 6f73 5b61 2e5f 7479 7065 5f5d 3b69  c=os[a._type_];i
-00056f50: 6628 2163 2974 6872 6f77 6045 6e63 6f75  f(!c)throw`Encou
-00056f60: 6e74 6572 6564 2075 6e6b 6e6f 776e 2063  ntered unknown c
-00056f70: 6f6d 706f 6e65 6e74 2074 7970 653a 2024  omponent type: $
-00056f80: 7b61 2e5f 7479 7065 5f7d 603b 6c65 7420  {a._type_}`;let 
-00056f90: 6c3d 6e65 7720 6328 7061 7273 6549 6e74  l=new c(parseInt
-00056fa0: 2873 292c 6129 3b43 5b73 5d3d 6c2c 5665  (s),a);C[s]=l,Ve
-00056fb0: 2e73 6574 286c 2e65 6c65 6d65 6e74 2c6c  .set(l.element,l
-00056fc0: 292c 6c2e 656c 656d 656e 742e 7365 7441  ),l.element.setA
-00056fd0: 7474 7269 6275 7465 2822 6462 672d 7079  ttribute("dbg-py
-00056fe0: 2d63 6c61 7373 222c 612e 5f70 7974 686f  -class",a._pytho
-00056ff0: 6e5f 7479 7065 5f29 2c6c 2e65 6c65 6d65  n_type_),l.eleme
-00057000: 6e74 2e73 6574 4174 7472 6962 7574 6528  nt.setAttribute(
-00057010: 2264 6267 2d69 6422 2c73 293b 6c65 7420  "dbg-id",s);let 
-00057020: 753d 612e 6b65 793b 7521 3d3d 766f 6964  u=a.key;u!==void
-00057030: 2030 2626 6c2e 656c 656d 656e 742e 7365   0&&l.element.se
-00057040: 7441 7474 7269 6275 7465 2822 6462 672d  tAttribute("dbg-
-00057050: 6b65 7922 2c60 247b 757d 6029 7d66 6f72  key",`${u}`)}for
-00057060: 286c 6574 2073 2069 6e20 7429 7b6c 6574  (let s in t){let
-00057070: 2061 3d74 5b73 5d2c 6f3d 435b 735d 3b6f   a=t[s],o=C[s];o
-00057080: 2e75 7064 6174 6545 6c65 6d65 6e74 2861  .updateElement(a
-00057090: 2c72 293b 6c65 7420 633d 4d61 7468 2e61  ,r);let c=Math.a
-000570a0: 6273 2861 2e5f 7369 7a65 5f5b 305d 2d6f  bs(a._size_[0]-o
-000570b0: 2e73 7461 7465 2e5f 7369 7a65 5f5b 305d  .state._size_[0]
-000570c0: 293e 3165 2d36 2c6c 3d4d 6174 682e 6162  )>1e-6,l=Math.ab
-000570d0: 7328 612e 5f73 697a 655f 5b31 5d2d 6f2e  s(a._size_[1]-o.
-000570e0: 7374 6174 652e 5f73 697a 655f 5b31 5d29  state._size_[1])
-000570f0: 3e31 652d 363b 2863 7c7c 6c29 2626 2863  >1e-6;(c||l)&&(c
-00057100: 6f6e 736f 6c65 2e6c 6f67 2860 5472 6967  onsole.log(`Trig
-00057110: 6765 7269 6e67 2072 652d 6c61 796f 7574  gering re-layout
-00057120: 2062 6563 6175 7365 2063 6f6d 706f 6e65   because compone
-00057130: 6e74 2023 247b 737d 2063 6861 6e67 6564  nt #${s} changed
-00057140: 2073 697a 653a 2024 7b6f 2e73 7461 7465   size: ${o.state
-00057150: 2e5f 7369 7a65 5f7d 202d 3e20 247b 612e  ._size_} -> ${a.
-00057160: 5f73 697a 655f 7d60 292c 6f2e 6d61 6b65  _size_}`),o.make
-00057170: 4c61 796f 7574 4469 7274 7928 2929 2c6f  LayoutDirty()),o
-00057180: 2e73 7461 7465 3d7b 2e2e 2e6f 2e73 7461  .state={...o.sta
-00057190: 7465 2c2e 2e2e 617d 7d69 6628 6521 3d3d  te,...a}}if(e!==
-000571a0: 6e75 6c6c 297b 6c65 7420 733d 435b 655d  null){let s=C[e]
-000571b0: 2e65 6c65 6d65 6e74 3b64 6f63 756d 656e  .element;documen
-000571c0: 742e 626f 6479 2e61 7070 656e 6443 6869  t.body.appendChi
-000571d0: 6c64 2873 297d 6921 3d3d 6e75 6c6c 2626  ld(s)}i!==null&&
-000571e0: 5775 2869 2c72 293b 666f 7228 6c65 7420  Wu(i,r);for(let 
-000571f0: 7320 6f66 2072 297b 6c65 7420 613d 5b73  s of r){let a=[s
-00057200: 5d3b 666f 7228 6c65 7420 6f20 6f66 2061  ];for(let o of a
-00057210: 2961 2e70 7573 6828 2e2e 2e6f 2e63 6869  )a.push(...o.chi
-00057220: 6c64 7265 6e29 2c6f 2e6f 6e44 6573 7472  ldren),o.onDestr
-00057230: 7563 7469 6f6e 2829 2c64 656c 6574 6520  uction(),delete 
-00057240: 435b 6f2e 6964 5d2c 5665 2e64 656c 6574  C[o.id],Ve.delet
-00057250: 6528 6f2e 656c 656d 656e 7429 7d75 7428  e(o.element)}ut(
-00057260: 292c 6521 3d3d 6e75 6c6c 2626 5f72 2829  ),e!==null&&_r()
-00057270: 7d66 756e 6374 696f 6e20 4675 2874 297b  }function Fu(t){
-00057280: 7265 7475 726e 2074 7970 656f 6620 742e  return typeof t.
-00057290: 6772 6162 4b65 7962 6f61 7264 466f 6375  grabKeyboardFocu
-000572a0: 733d 3d22 6675 6e63 7469 6f6e 227d 6675  s=="function"}fu
-000572b0: 6e63 7469 6f6e 2057 7528 742c 6529 7b6c  nction Wu(t,e){l
-000572c0: 6574 206e 3d64 7428 292c 693d 742c 723d  et n=dt(),i=t,r=
-000572d0: 6e75 6c6c 3b66 6f72 283b 6921 3d3d 6e3b  null;for(;i!==n;
-000572e0: 2965 2e68 6173 2869 293f 723d 6e75 6c6c  )e.has(i)?r=null
-000572f0: 3a72 3d3d 3d6e 756c 6c26 2646 7528 6929  :r===null&&Fu(i)
-00057300: 2626 2872 3d69 292c 693d 692e 7061 7265  &&(r=i),i=i.pare
-00057310: 6e74 3b72 213d 3d6e 756c 6c26 2672 2e67  nt;r!==null&&r.g
-00057320: 7261 624b 6579 626f 6172 6446 6f63 7573  rabKeyboardFocus
-00057330: 2829 7d67 6c6f 6261 6c54 6869 732e 5345  ()}globalThis.SE
-00057340: 5353 494f 4e5f 544f 4b45 4e3d 227b 7365  SSION_TOKEN="{se
-00057350: 7373 696f 6e5f 746f 6b65 6e7d 223b 676c  ssion_token}";gl
-00057360: 6f62 616c 5468 6973 2e50 494e 475f 504f  obalThis.PING_PO
-00057370: 4e47 5f49 4e54 4552 5641 4c5f 5345 434f  NG_INTERVAL_SECO
-00057380: 4e44 533d 227b 7069 6e67 5f70 6f6e 675f  NDS="{ping_pong_
-00057390: 696e 7465 7276 616c 7d22 3b67 6c6f 6261  interval}";globa
-000573a0: 6c54 6869 732e 5249 4f5f 4445 4255 475f  lThis.RIO_DEBUG_
-000573b0: 4d4f 4445 3d22 7b64 6562 7567 5f6d 6f64  MODE="{debug_mod
-000573c0: 657d 223b 676c 6f62 616c 5468 6973 2e43  e}";globalThis.C
-000573d0: 4849 4c44 5f41 5454 5249 4255 5445 5f4e  HILD_ATTRIBUTE_N
-000573e0: 414d 4553 3d22 7b63 6869 6c64 5f61 7474  AMES="{child_att
-000573f0: 7269 6275 7465 5f6e 616d 6573 7d22 3b67  ribute_names}";g
-00057400: 6c6f 6261 6c54 6869 732e 5255 4e4e 494e  lobalThis.RUNNIN
-00057410: 475f 494e 5f57 494e 444f 573d 227b 7275  G_IN_WINDOW="{ru
-00057420: 6e6e 696e 675f 696e 5f77 696e 646f 777d  nning_in_window}
-00057430: 223b 676c 6f62 616c 5468 6973 2e52 494f  ";globalThis.RIO
-00057440: 5f44 4542 5547 4745 523d 6e75 6c6c 3b6c  _DEBUGGER=null;l
-00057450: 6574 2047 6e3d 2131 3b66 756e 6374 696f  et Gn=!1;functio
-00057460: 6e20 5575 2829 7b6c 6574 2074 3d64 6f63  n Uu(){let t=doc
-00057470: 756d 656e 742e 6372 6561 7465 456c 656d  ument.createElem
-00057480: 656e 7428 2264 6976 2229 3b74 2e73 7479  ent("div");t.sty
-00057490: 6c65 2e70 6f73 6974 696f 6e3d 2261 6273  le.position="abs
-000574a0: 6f6c 7574 6522 2c74 2e73 7479 6c65 2e74  olute",t.style.t
-000574b0: 6f70 3d22 3070 7822 2c74 2e73 7479 6c65  op="0px",t.style
-000574c0: 2e6c 6566 743d 2230 7078 222c 742e 7374  .left="0px",t.st
-000574d0: 796c 652e 7669 7369 6269 6c69 7479 3d22  yle.visibility="
-000574e0: 6869 6464 656e 222c 742e 7374 796c 652e  hidden",t.style.
-000574f0: 7769 6474 683d 2232 3030 7078 222c 742e  width="200px",t.
-00057500: 7374 796c 652e 6865 6967 6874 3d22 3135  style.height="15
-00057510: 3070 7822 2c74 2e73 7479 6c65 2e6f 7665  0px",t.style.ove
-00057520: 7266 6c6f 773d 2268 6964 6465 6e22 3b6c  rflow="hidden";l
-00057530: 6574 2065 3d64 6f63 756d 656e 742e 6372  et e=document.cr
-00057540: 6561 7465 456c 656d 656e 7428 2270 2229  eateElement("p")
-00057550: 3b65 2e73 7479 6c65 2e77 6964 7468 3d22  ;e.style.width="
-00057560: 3130 3025 222c 652e 7374 796c 652e 6865  100%",e.style.he
-00057570: 6967 6874 3d22 3230 3070 7822 2c74 2e61  ight="200px",t.a
-00057580: 7070 656e 6443 6869 6c64 2865 292c 646f  ppendChild(e),do
-00057590: 6375 6d65 6e74 2e62 6f64 792e 6170 7065  cument.body.appe
-000575a0: 6e64 4368 696c 6428 7429 3b6c 6574 206e  ndChild(t);let n
-000575b0: 3d65 2e6f 6666 7365 7457 6964 7468 3b74  =e.offsetWidth;t
-000575c0: 2e73 7479 6c65 2e6f 7665 7266 6c6f 773d  .style.overflow=
-000575d0: 2273 6372 6f6c 6c22 3b6c 6574 2069 3d65  "scroll";let i=e
-000575e0: 2e6f 6666 7365 7457 6964 7468 3b72 6574  .offsetWidth;ret
-000575f0: 7572 6e20 6e3d 3d69 2626 2869 3d74 2e63  urn n==i&&(i=t.c
-00057600: 6c69 656e 7457 6964 7468 292c 646f 6375  lientWidth),docu
-00057610: 6d65 6e74 2e62 6f64 792e 7265 6d6f 7665  ment.body.remove
-00057620: 4368 696c 6428 7429 2c6e 2d69 7d63 6f6e  Child(t),n-i}con
-00057630: 7374 2063 733d 5575 2829 3b6c 6574 2059  st cs=Uu();let Y
-00057640: 3d31 362c 5765 3d63 732f 593b 6675 6e63  =16,We=cs/Y;func
-00057650: 7469 6f6e 2024 7528 297b 6966 2874 7970  tion $u(){if(typ
-00057660: 656f 6620 676c 6f62 616c 5468 6973 2e50  eof globalThis.P
-00057670: 494e 475f 504f 4e47 5f49 4e54 4552 5641  ING_PONG_INTERVA
-00057680: 4c5f 5345 434f 4e44 5321 3d22 6e75 6d62  L_SECONDS!="numb
-00057690: 6572 2229 7b63 6f6e 736f 6c65 2e65 7272  er"){console.err
-000576a0: 6f72 2860 5265 6365 6976 6564 2065 7272  or(`Received err
-000576b0: 6f6e 656f 7573 2048 544d 4c20 6672 6f6d  oneous HTML from
-000576c0: 2074 6865 2073 6572 7665 723a 2054 6865   the server: The
-000576d0: 2070 696e 6720 706f 6e67 2069 6e74 6572   ping pong inter
-000576e0: 7661 6c20 6973 2024 7b67 6c6f 6261 6c54  val is ${globalT
-000576f0: 6869 732e 5049 4e47 5f50 4f4e 475f 494e  his.PING_PONG_IN
-00057700: 5445 5256 414c 5f53 4543 4f4e 4453 7d20  TERVAL_SECONDS} 
-00057710: 696e 7374 6561 6420 6f66 2061 206e 756d  instead of a num
-00057720: 6265 7260 293b 7265 7475 726e 7d67 6c6f  ber`);return}glo
-00057730: 6261 6c54 6869 732e 5249 4f5f 4445 4255  balThis.RIO_DEBU
-00057740: 475f 4d4f 4445 2626 636f 6e73 6f6c 652e  G_MODE&&console.
-00057750: 7761 726e 2860 5269 6f20 6973 2072 756e  warn(`Rio is run
-00057760: 6e69 6e67 2069 6e20 4445 4255 4720 6d6f  ning in DEBUG mo
-00057770: 6465 2e0a 4465 6275 6720 6d6f 6465 2069  de..Debug mode i
-00057780: 6e63 6c75 6465 7320 6865 6c70 6675 6c20  ncludes helpful 
-00057790: 746f 6f6c 7320 666f 7220 6465 7665 6c6f  tools for develo
-000577a0: 706d 656e 742c 2062 7574 2069 7320 736c  pment, but is sl
-000577b0: 6f77 6572 2061 6e64 2064 6973 6162 6c65  ower and disable
-000577c0: 7320 736f 6d65 2073 6166 6574 7920 6368  s some safety ch
-000577d0: 6563 6b73 2e20 4e65 7665 7220 7573 6520  ecks. Never use 
-000577e0: 6974 2069 6e20 7072 6f64 7563 7469 6f6e  it in production
-000577f0: 2160 293b 7661 7220 743d 646f 6375 6d65  !`);var t=docume
-00057800: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
-00057810: 2822 6469 7622 293b 742e 7374 796c 652e  ("div");t.style.
-00057820: 6865 6967 6874 3d22 3130 7265 6d22 2c64  height="10rem",d
-00057830: 6f63 756d 656e 742e 626f 6479 2e61 7070  ocument.body.app
-00057840: 656e 6443 6869 6c64 2874 292c 593d 742e  endChild(t),Y=t.
-00057850: 6f66 6673 6574 4865 6967 6874 2f31 302c  offsetHeight/10,
-00057860: 646f 6375 6d65 6e74 2e62 6f64 792e 7265  document.body.re
-00057870: 6d6f 7665 4368 696c 6428 7429 2c57 653d  moveChild(t),We=
-00057880: 6373 2f59 2c67 6c6f 6261 6c54 6869 732e  cs/Y,globalThis.
-00057890: 7069 7865 6c73 5065 7252 656d 3d59 2c67  pixelsPerRem=Y,g
-000578a0: 6c6f 6261 6c54 6869 732e 7363 726f 6c6c  lobalThis.scroll
-000578b0: 4261 7253 697a 653d 5765 2c77 696e 646f  BarSize=We,windo
-000578c0: 772e 6164 6445 7665 6e74 4c69 7374 656e  w.addEventListen
-000578d0: 6572 2822 6265 666f 7265 756e 6c6f 6164  er("beforeunload
-000578e0: 222c 2829 3d3e 7b47 6e3d 2130 7d29 2c77  ",()=>{Gn=!0}),w
-000578f0: 696e 646f 772e 6164 6445 7665 6e74 4c69  indow.addEventLi
-00057900: 7374 656e 6572 2822 706f 7073 7461 7465  stener("popstate
-00057910: 222c 653d 3e7b 636f 6e73 6f6c 652e 6c6f  ",e=>{console.lo
-00057920: 6728 6055 524c 2063 6861 6e67 6564 2074  g(`URL changed t
-00057930: 6f20 247b 7769 6e64 6f77 2e6c 6f63 6174  o ${window.locat
-00057940: 696f 6e2e 6872 6566 7d60 292c 6e74 2822  ion.href}`),nt("
-00057950: 6f6e 5572 6c43 6861 6e67 6522 2c7b 6e65  onUrlChange",{ne
-00057960: 7755 726c 3a77 696e 646f 772e 6c6f 6361  wUrl:window.loca
-00057970: 7469 6f6e 2e68 7265 662e 746f 5374 7269  tion.href.toStri
-00057980: 6e67 2829 7d29 7d29 2c77 696e 646f 772e  ng()})}),window.
-00057990: 6164 6445 7665 6e74 4c69 7374 656e 6572  addEventListener
-000579a0: 2822 7265 7369 7a65 222c 653d 3e7b 7472  ("resize",e=>{tr
-000579b0: 797b 6e74 2822 6f6e 5769 6e64 6f77 5265  y{nt("onWindowRe
-000579c0: 7369 7a65 222c 7b6e 6577 5769 6474 683a  size",{newWidth:
-000579d0: 7769 6e64 6f77 2e69 6e6e 6572 5769 6474  window.innerWidt
-000579e0: 682f 592c 6e65 7748 6569 6768 743a 7769  h/Y,newHeight:wi
-000579f0: 6e64 6f77 2e69 6e6e 6572 4865 6967 6874  ndow.innerHeight
-00057a00: 2f59 7d29 7d63 6174 6368 2869 297b 636f  /Y})}catch(i){co
-00057a10: 6e73 6f6c 652e 7761 726e 2860 436f 756c  nsole.warn(`Coul
-00057a20: 646e 2774 206e 6f74 6966 7920 6261 636b  dn't notify back
-00057a30: 656e 6420 6f66 2077 696e 646f 7720 7265  end of window re
-00057a40: 7369 7a65 3a20 247b 697d 6029 7d6c 6574  size: ${i}`)}let
-00057a50: 206e 3d64 6f63 756d 656e 742e 626f 6479   n=document.body
-00057a60: 2e71 7565 7279 5365 6c65 6374 6f72 2822  .querySelector("
-00057a70: 2e72 696f 2d66 756e 6461 6d65 6e74 616c  .rio-fundamental
-00057a80: 2d72 6f6f 742d 636f 6d70 6f6e 656e 7422  -root-component"
-00057a90: 293b 6e21 3d3d 6e75 6c6c 2626 284b 6528  );n!==null&&(Ke(
-00057aa0: 6e29 2e6d 616b 654c 6179 6f75 7444 6972  n).makeLayoutDir
-00057ab0: 7479 2829 2c75 7428 2929 7d29 2c77 696e  ty(),ut())}),win
-00057ac0: 646f 772e 6164 6445 7665 6e74 4c69 7374  dow.addEventList
-00057ad0: 656e 6572 2822 6861 7368 6368 616e 6765  ener("hashchange
-00057ae0: 222c 5f72 292c 7673 2829 7d24 7528 293b  ",_r),vs()}$u();
-00057af0: 0a0a 3c2f 7363 7269 7074 3e0a 2020 2020  ..</script>.    
-00057b00: 2020 3c73 7479 6c65 3e0a 4063 6861 7273    <style>.@chars
-00057b10: 6574 2022 5554 462d 3822 3b2e 7269 6f2d  et "UTF-8";.rio-
-00057b20: 7377 6974 6368 6572 6f6f 2d62 6163 6b67  switcheroo-backg
-00057b30: 726f 756e 647b 2d2d 7269 6f2d 6c6f 6361  round{--rio-loca
-00057b40: 6c2d 6267 3a20 7661 7228 2d2d 7269 6f2d  l-bg: var(--rio-
-00057b50: 676c 6f62 616c 2d62 6163 6b67 726f 756e  global-backgroun
-00057b60: 642d 6267 293b 2d2d 7269 6f2d 6c6f 6361  d-bg);--rio-loca
-00057b70: 6c2d 6267 2d76 6172 6961 6e74 3a20 7661  l-bg-variant: va
-00057b80: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d62  r(--rio-global-b
-00057b90: 6163 6b67 726f 756e 642d 6267 2d76 6172  ackground-bg-var
-00057ba0: 6961 6e74 293b 2d2d 7269 6f2d 6c6f 6361  iant);--rio-loca
-00057bb0: 6c2d 6267 2d61 6374 6976 653a 2076 6172  l-bg-active: var
-00057bc0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6261  (--rio-global-ba
-00057bd0: 636b 6772 6f75 6e64 2d62 672d 6163 7469  ckground-bg-acti
-00057be0: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
-00057bf0: 6667 3a20 7661 7228 2d2d 7269 6f2d 676c  fg: var(--rio-gl
-00057c00: 6f62 616c 2d62 6163 6b67 726f 756e 642d  obal-background-
-00057c10: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-00057c20: 6c65 7665 6c2d 322d 6267 3a20 7661 7228  level-2-bg: var(
-00057c30: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
-00057c40: 6f6e 6461 7279 2d62 6729 3b2d 2d72 696f  ondary-bg);--rio
-00057c50: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
-00057c60: 672d 7661 7269 616e 743a 2076 6172 282d  g-variant: var(-
-00057c70: 2d72 696f 2d67 6c6f 6261 6c2d 7365 636f  -rio-global-seco
-00057c80: 6e64 6172 792d 6267 2d76 6172 6961 6e74  ndary-bg-variant
-00057c90: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
-00057ca0: 7665 6c2d 322d 6267 2d61 6374 6976 653a  vel-2-bg-active:
-00057cb0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-00057cc0: 6c2d 7365 636f 6e64 6172 792d 6267 2d61  l-secondary-bg-a
-00057cd0: 6374 6976 6529 3b2d 2d72 696f 2d6c 6f63  ctive);--rio-loc
-00057ce0: 616c 2d6c 6576 656c 2d32 2d66 673a 2076  al-level-2-fg: v
-00057cf0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00057d00: 7365 636f 6e64 6172 792d 6667 293b 2d2d  secondary-fg);--
-00057d10: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-00057d20: 332d 6267 3a20 7661 7228 2d2d 7269 6f2d  3-bg: var(--rio-
-00057d30: 676c 6f62 616c 2d70 7269 6d61 7279 2d62  global-primary-b
-00057d40: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
-00057d50: 6576 656c 2d33 2d62 672d 7661 7269 616e  evel-3-bg-varian
-00057d60: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
-00057d70: 6261 6c2d 7072 696d 6172 792d 6267 2d76  bal-primary-bg-v
-00057d80: 6172 6961 6e74 293b 2d2d 7269 6f2d 6c6f  ariant);--rio-lo
-00057d90: 6361 6c2d 6c65 7665 6c2d 332d 6267 2d61  cal-level-3-bg-a
-00057da0: 6374 6976 653a 2076 6172 282d 2d72 696f  ctive: var(--rio
-00057db0: 2d67 6c6f 6261 6c2d 7072 696d 6172 792d  -global-primary-
-00057dc0: 6267 2d61 6374 6976 6529 3b2d 2d72 696f  bg-active);--rio
-00057dd0: 2d6c 6f63 616c 2d6c 6576 656c 2d33 2d66  -local-level-3-f
-00057de0: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
-00057df0: 6261 6c2d 7072 696d 6172 792d 6667 293b  bal-primary-fg);
-00057e00: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-00057e10: 696e 6731 2d63 6f6c 6f72 3a20 7661 7228  ing1-color: var(
-00057e20: 2d2d 7269 6f2d 676c 6f62 616c 2d68 6561  --rio-global-hea
-00057e30: 6469 6e67 312d 636f 6c6f 7229 3b2d 2d72  ding1-color);--r
-00057e40: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-00057e50: 312d 6261 636b 6772 6f75 6e64 3a20 7661  1-background: va
-00057e60: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
-00057e70: 6561 6469 6e67 312d 6261 636b 6772 6f75  eading1-backgrou
-00057e80: 6e64 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nd);--rio-local-
-00057e90: 6865 6164 696e 6731 2d62 6163 6b67 726f  heading1-backgro
-00057ea0: 756e 642d 636c 6970 3a20 7661 7228 202d  und-clip: var( -
-00057eb0: 2d72 696f 2d67 6c6f 6261 6c2d 6865 6164  -rio-global-head
-00057ec0: 696e 6731 2d62 6163 6b67 726f 756e 642d  ing1-background-
-00057ed0: 636c 6970 2029 3b2d 2d72 696f 2d6c 6f63  clip );--rio-loc
-00057ee0: 616c 2d68 6561 6469 6e67 312d 6669 6c6c  al-heading1-fill
-00057ef0: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
-00057f00: 6f2d 676c 6f62 616c 2d68 6561 6469 6e67  o-global-heading
-00057f10: 312d 6669 6c6c 2d63 6f6c 6f72 293b 2d2d  1-fill-color);--
-00057f20: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-00057f30: 6731 2d66 6f6e 742d 7765 6967 6874 3a20  g1-font-weight: 
-00057f40: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00057f50: 2d68 6561 6469 6e67 312d 666f 6e74 2d77  -heading1-font-w
-00057f60: 6569 6768 7429 3b2d 2d72 696f 2d6c 6f63  eight);--rio-loc
-00057f70: 616c 2d68 6561 6469 6e67 322d 636f 6c6f  al-heading2-colo
-00057f80: 723a 2076 6172 282d 2d72 696f 2d67 6c6f  r: var(--rio-glo
-00057f90: 6261 6c2d 6865 6164 696e 6732 2d63 6f6c  bal-heading2-col
-00057fa0: 6f72 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  or);--rio-local-
-00057fb0: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
-00057fc0: 756e 643a 2076 6172 282d 2d72 696f 2d67  und: var(--rio-g
-00057fd0: 6c6f 6261 6c2d 6865 6164 696e 6732 2d62  lobal-heading2-b
-00057fe0: 6163 6b67 726f 756e 6429 3b2d 2d72 696f  ackground);--rio
-00057ff0: 2d6c 6f63 616c 2d68 6561 6469 6e67 322d  -local-heading2-
-00058000: 6261 636b 6772 6f75 6e64 2d63 6c69 703a  background-clip:
-00058010: 2076 6172 2820 2d2d 7269 6f2d 676c 6f62   var( --rio-glob
-00058020: 616c 2d68 6561 6469 6e67 322d 6261 636b  al-heading2-back
-00058030: 6772 6f75 6e64 2d63 6c69 7020 293b 2d2d  ground-clip );--
-00058040: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-00058050: 6732 2d66 696c 6c2d 636f 6c6f 723a 2076  g2-fill-color: v
-00058060: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00058070: 6865 6164 696e 6732 2d66 696c 6c2d 636f  heading2-fill-co
-00058080: 6c6f 7229 3b2d 2d72 696f 2d6c 6f63 616c  lor);--rio-local
-00058090: 2d68 6561 6469 6e67 322d 666f 6e74 2d77  -heading2-font-w
-000580a0: 6569 6768 743a 2076 6172 282d 2d72 696f  eight: var(--rio
-000580b0: 2d67 6c6f 6261 6c2d 6865 6164 696e 6732  -global-heading2
-000580c0: 2d66 6f6e 742d 7765 6967 6874 293b 2d2d  -font-weight);--
-000580d0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-000580e0: 6733 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g3-color: var(--
-000580f0: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
-00058100: 6e67 332d 636f 6c6f 7229 3b2d 2d72 696f  ng3-color);--rio
-00058110: 2d6c 6f63 616c 2d68 6561 6469 6e67 332d  -local-heading3-
-00058120: 6261 636b 6772 6f75 6e64 3a20 7661 7228  background: var(
-00058130: 2d2d 7269 6f2d 676c 6f62 616c 2d68 6561  --rio-global-hea
-00058140: 6469 6e67 332d 6261 636b 6772 6f75 6e64  ding3-background
-00058150: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
-00058160: 6164 696e 6733 2d62 6163 6b67 726f 756e  ading3-backgroun
-00058170: 642d 636c 6970 3a20 7661 7228 202d 2d72  d-clip: var( --r
-00058180: 696f 2d67 6c6f 6261 6c2d 6865 6164 696e  io-global-headin
-00058190: 6733 2d62 6163 6b67 726f 756e 642d 636c  g3-background-cl
-000581a0: 6970 2029 3b2d 2d72 696f 2d6c 6f63 616c  ip );--rio-local
-000581b0: 2d68 6561 6469 6e67 332d 6669 6c6c 2d63  -heading3-fill-c
-000581c0: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
-000581d0: 676c 6f62 616c 2d68 6561 6469 6e67 332d  global-heading3-
-000581e0: 6669 6c6c 2d63 6f6c 6f72 293b 2d2d 7269  fill-color);--ri
-000581f0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
-00058200: 2d66 6f6e 742d 7765 6967 6874 3a20 7661  -font-weight: va
-00058210: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
-00058220: 6561 6469 6e67 332d 666f 6e74 2d77 6569  eading3-font-wei
-00058230: 6768 7429 3b2d 2d72 696f 2d6c 6f63 616c  ght);--rio-local
-00058240: 2d74 6578 742d 636f 6c6f 723a 2076 6172  -text-color: var
-00058250: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7465  (--rio-global-te
-00058260: 7874 2d63 6f6c 6f72 293b 2d2d 7269 6f2d  xt-color);--rio-
-00058270: 6c6f 6361 6c2d 7465 7874 2d62 6163 6b67  local-text-backg
-00058280: 726f 756e 643a 2076 6172 282d 2d72 696f  round: var(--rio
-00058290: 2d67 6c6f 6261 6c2d 7465 7874 2d62 6163  -global-text-bac
-000582a0: 6b67 726f 756e 6429 3b2d 2d72 696f 2d6c  kground);--rio-l
-000582b0: 6f63 616c 2d74 6578 742d 6261 636b 6772  ocal-text-backgr
-000582c0: 6f75 6e64 2d63 6c69 703a 2076 6172 282d  ound-clip: var(-
-000582d0: 2d72 696f 2d67 6c6f 6261 6c2d 7465 7874  -rio-global-text
-000582e0: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
-000582f0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  );--rio-local-te
-00058300: 7874 2d66 696c 6c2d 636f 6c6f 723a 2076  xt-fill-color: v
-00058310: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00058320: 7465 7874 2d66 696c 6c2d 636f 6c6f 7229  text-fill-color)
-00058330: 3b2d 2d72 696f 2d6c 6f63 616c 2d74 6578  ;--rio-local-tex
-00058340: 742d 666f 6e74 2d77 6569 6768 743a 2076  t-font-weight: v
-00058350: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00058360: 7465 7874 2d66 6f6e 742d 7765 6967 6874  text-font-weight
-00058370: 293b 636f 6c6f 723a 7661 7228 2d2d 7269  );color:var(--ri
-00058380: 6f2d 6c6f 6361 6c2d 6667 297d 2e72 696f  o-local-fg)}.rio
-00058390: 2d73 7769 7463 6865 726f 6f2d 6e65 7574  -switcheroo-neut
-000583a0: 7261 6c7b 2d2d 7269 6f2d 6c6f 6361 6c2d  ral{--rio-local-
-000583b0: 6267 3a20 7661 7228 2d2d 7269 6f2d 676c  bg: var(--rio-gl
-000583c0: 6f62 616c 2d6e 6575 7472 616c 2d62 6729  obal-neutral-bg)
-000583d0: 3b2d 2d72 696f 2d6c 6f63 616c 2d62 672d  ;--rio-local-bg-
-000583e0: 7661 7269 616e 743a 2076 6172 282d 2d72  variant: var(--r
-000583f0: 696f 2d67 6c6f 6261 6c2d 6e65 7574 7261  io-global-neutra
-00058400: 6c2d 6267 2d76 6172 6961 6e74 293b 2d2d  l-bg-variant);--
-00058410: 7269 6f2d 6c6f 6361 6c2d 6267 2d61 6374  rio-local-bg-act
-00058420: 6976 653a 2076 6172 282d 2d72 696f 2d67  ive: var(--rio-g
-00058430: 6c6f 6261 6c2d 6e65 7574 7261 6c2d 6267  lobal-neutral-bg
-00058440: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
-00058450: 6f63 616c 2d66 673a 2076 6172 282d 2d72  ocal-fg: var(--r
-00058460: 696f 2d67 6c6f 6261 6c2d 6e65 7574 7261  io-global-neutra
-00058470: 6c2d 6667 293b 2d2d 7269 6f2d 6c6f 6361  l-fg);--rio-loca
-00058480: 6c2d 6c65 7665 6c2d 322d 6267 3a20 7661  l-level-2-bg: va
-00058490: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-000584a0: 6563 6f6e 6461 7279 2d62 6729 3b2d 2d72  econdary-bg);--r
-000584b0: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d32  io-local-level-2
-000584c0: 2d62 672d 7661 7269 616e 743a 2076 6172  -bg-variant: var
-000584d0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
-000584e0: 636f 6e64 6172 792d 6267 2d76 6172 6961  condary-bg-varia
-000584f0: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
-00058500: 6c65 7665 6c2d 322d 6267 2d61 6374 6976  level-2-bg-activ
-00058510: 653a 2076 6172 282d 2d72 696f 2d67 6c6f  e: var(--rio-glo
-00058520: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
-00058530: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
-00058540: 6f63 616c 2d6c 6576 656c 2d32 2d66 673a  ocal-level-2-fg:
-00058550: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-00058560: 6c2d 7365 636f 6e64 6172 792d 6667 293b  l-secondary-fg);
-00058570: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-00058580: 6c2d 332d 6267 3a20 7661 7228 2d2d 7269  l-3-bg: var(--ri
-00058590: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
-000585a0: 2d62 6729 3b2d 2d72 696f 2d6c 6f63 616c  -bg);--rio-local
-000585b0: 2d6c 6576 656c 2d33 2d62 672d 7661 7269  -level-3-bg-vari
-000585c0: 616e 743a 2076 6172 282d 2d72 696f 2d67  ant: var(--rio-g
-000585d0: 6c6f 6261 6c2d 7072 696d 6172 792d 6267  lobal-primary-bg
-000585e0: 2d76 6172 6961 6e74 293b 2d2d 7269 6f2d  -variant);--rio-
-000585f0: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
-00058600: 2d61 6374 6976 653a 2076 6172 282d 2d72  -active: var(--r
-00058610: 696f 2d67 6c6f 6261 6c2d 7072 696d 6172  io-global-primar
-00058620: 792d 6267 2d61 6374 6976 6529 3b2d 2d72  y-bg-active);--r
-00058630: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
-00058640: 2d66 673a 2076 6172 282d 2d72 696f 2d67  -fg: var(--rio-g
-00058650: 6c6f 6261 6c2d 7072 696d 6172 792d 6667  lobal-primary-fg
-00058660: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
-00058670: 6164 696e 6731 2d63 6f6c 6f72 3a20 7661  ading1-color: va
-00058680: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
-00058690: 6561 6469 6e67 312d 636f 6c6f 7229 3b2d  eading1-color);-
-000586a0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-000586b0: 6e67 312d 6261 636b 6772 6f75 6e64 3a20  ng1-background: 
-000586c0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-000586d0: 2d68 6561 6469 6e67 312d 6261 636b 6772  -heading1-backgr
-000586e0: 6f75 6e64 293b 2d2d 7269 6f2d 6c6f 6361  ound);--rio-loca
-000586f0: 6c2d 6865 6164 696e 6731 2d62 6163 6b67  l-heading1-backg
-00058700: 726f 756e 642d 636c 6970 3a20 7661 7228  round-clip: var(
-00058710: 202d 2d72 696f 2d67 6c6f 6261 6c2d 6865   --rio-global-he
-00058720: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
-00058730: 642d 636c 6970 2029 3b2d 2d72 696f 2d6c  d-clip );--rio-l
-00058740: 6f63 616c 2d68 6561 6469 6e67 312d 6669  ocal-heading1-fi
-00058750: 6c6c 2d63 6f6c 6f72 3a20 7661 7228 2d2d  ll-color: var(--
-00058760: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
-00058770: 6e67 312d 6669 6c6c 2d63 6f6c 6f72 293b  ng1-fill-color);
-00058780: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-00058790: 696e 6731 2d66 6f6e 742d 7765 6967 6874  ing1-font-weight
-000587a0: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
-000587b0: 616c 2d68 6561 6469 6e67 312d 666f 6e74  al-heading1-font
-000587c0: 2d77 6569 6768 7429 3b2d 2d72 696f 2d6c  -weight);--rio-l
-000587d0: 6f63 616c 2d68 6561 6469 6e67 322d 636f  ocal-heading2-co
-000587e0: 6c6f 723a 2076 6172 282d 2d72 696f 2d67  lor: var(--rio-g
-000587f0: 6c6f 6261 6c2d 6865 6164 696e 6732 2d63  lobal-heading2-c
-00058800: 6f6c 6f72 293b 2d2d 7269 6f2d 6c6f 6361  olor);--rio-loca
-00058810: 6c2d 6865 6164 696e 6732 2d62 6163 6b67  l-heading2-backg
-00058820: 726f 756e 643a 2076 6172 282d 2d72 696f  round: var(--rio
-00058830: 2d67 6c6f 6261 6c2d 6865 6164 696e 6732  -global-heading2
-00058840: 2d62 6163 6b67 726f 756e 6429 3b2d 2d72  -background);--r
-00058850: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-00058860: 322d 6261 636b 6772 6f75 6e64 2d63 6c69  2-background-cli
-00058870: 703a 2076 6172 2820 2d2d 7269 6f2d 676c  p: var( --rio-gl
-00058880: 6f62 616c 2d68 6561 6469 6e67 322d 6261  obal-heading2-ba
-00058890: 636b 6772 6f75 6e64 2d63 6c69 7020 293b  ckground-clip );
-000588a0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-000588b0: 696e 6732 2d66 696c 6c2d 636f 6c6f 723a  ing2-fill-color:
-000588c0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-000588d0: 6c2d 6865 6164 696e 6732 2d66 696c 6c2d  l-heading2-fill-
-000588e0: 636f 6c6f 7229 3b2d 2d72 696f 2d6c 6f63  color);--rio-loc
-000588f0: 616c 2d68 6561 6469 6e67 322d 666f 6e74  al-heading2-font
-00058900: 2d77 6569 6768 743a 2076 6172 282d 2d72  -weight: var(--r
-00058910: 696f 2d67 6c6f 6261 6c2d 6865 6164 696e  io-global-headin
-00058920: 6732 2d66 6f6e 742d 7765 6967 6874 293b  g2-font-weight);
-00058930: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-00058940: 696e 6733 2d63 6f6c 6f72 3a20 7661 7228  ing3-color: var(
-00058950: 2d2d 7269 6f2d 676c 6f62 616c 2d68 6561  --rio-global-hea
-00058960: 6469 6e67 332d 636f 6c6f 7229 3b2d 2d72  ding3-color);--r
-00058970: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-00058980: 332d 6261 636b 6772 6f75 6e64 3a20 7661  3-background: va
-00058990: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
-000589a0: 6561 6469 6e67 332d 6261 636b 6772 6f75  eading3-backgrou
-000589b0: 6e64 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nd);--rio-local-
-000589c0: 6865 6164 696e 6733 2d62 6163 6b67 726f  heading3-backgro
-000589d0: 756e 642d 636c 6970 3a20 7661 7228 202d  und-clip: var( -
-000589e0: 2d72 696f 2d67 6c6f 6261 6c2d 6865 6164  -rio-global-head
-000589f0: 696e 6733 2d62 6163 6b67 726f 756e 642d  ing3-background-
-00058a00: 636c 6970 2029 3b2d 2d72 696f 2d6c 6f63  clip );--rio-loc
-00058a10: 616c 2d68 6561 6469 6e67 332d 6669 6c6c  al-heading3-fill
-00058a20: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
-00058a30: 6f2d 676c 6f62 616c 2d68 6561 6469 6e67  o-global-heading
-00058a40: 332d 6669 6c6c 2d63 6f6c 6f72 293b 2d2d  3-fill-color);--
-00058a50: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-00058a60: 6733 2d66 6f6e 742d 7765 6967 6874 3a20  g3-font-weight: 
-00058a70: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00058a80: 2d68 6561 6469 6e67 332d 666f 6e74 2d77  -heading3-font-w
-00058a90: 6569 6768 7429 3b2d 2d72 696f 2d6c 6f63  eight);--rio-loc
-00058aa0: 616c 2d74 6578 742d 636f 6c6f 723a 2076  al-text-color: v
-00058ab0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00058ac0: 7465 7874 2d63 6f6c 6f72 293b 2d2d 7269  text-color);--ri
-00058ad0: 6f2d 6c6f 6361 6c2d 7465 7874 2d62 6163  o-local-text-bac
-00058ae0: 6b67 726f 756e 643a 2076 6172 282d 2d72  kground: var(--r
-00058af0: 696f 2d67 6c6f 6261 6c2d 7465 7874 2d62  io-global-text-b
-00058b00: 6163 6b67 726f 756e 6429 3b2d 2d72 696f  ackground);--rio
-00058b10: 2d6c 6f63 616c 2d74 6578 742d 6261 636b  -local-text-back
-00058b20: 6772 6f75 6e64 2d63 6c69 703a 2076 6172  ground-clip: var
-00058b30: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7465  (--rio-global-te
-00058b40: 7874 2d62 6163 6b67 726f 756e 642d 636c  xt-background-cl
-00058b50: 6970 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ip);--rio-local-
-00058b60: 7465 7874 2d66 696c 6c2d 636f 6c6f 723a  text-fill-color:
-00058b70: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-00058b80: 6c2d 7465 7874 2d66 696c 6c2d 636f 6c6f  l-text-fill-colo
-00058b90: 7229 3b2d 2d72 696f 2d6c 6f63 616c 2d74  r);--rio-local-t
-00058ba0: 6578 742d 666f 6e74 2d77 6569 6768 743a  ext-font-weight:
-00058bb0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-00058bc0: 6c2d 7465 7874 2d66 6f6e 742d 7765 6967  l-text-font-weig
-00058bd0: 6874 293b 636f 6c6f 723a 7661 7228 2d2d  ht);color:var(--
-00058be0: 7269 6f2d 6c6f 6361 6c2d 6667 297d 2e72  rio-local-fg)}.r
-00058bf0: 696f 2d73 7769 7463 6865 726f 6f2d 6875  io-switcheroo-hu
-00058c00: 647b 2d2d 7269 6f2d 6c6f 6361 6c2d 6267  d{--rio-local-bg
-00058c10: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
-00058c20: 616c 2d68 7564 2d62 6729 3b2d 2d72 696f  al-hud-bg);--rio
-00058c30: 2d6c 6f63 616c 2d62 672d 7661 7269 616e  -local-bg-varian
-00058c40: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
-00058c50: 6261 6c2d 6875 642d 6267 2d76 6172 6961  bal-hud-bg-varia
-00058c60: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
-00058c70: 6267 2d61 6374 6976 653a 2076 6172 282d  bg-active: var(-
-00058c80: 2d72 696f 2d67 6c6f 6261 6c2d 6875 642d  -rio-global-hud-
-00058c90: 6267 2d61 6374 6976 6529 3b2d 2d72 696f  bg-active);--rio
-00058ca0: 2d6c 6f63 616c 2d66 673a 2076 6172 282d  -local-fg: var(-
-00058cb0: 2d72 696f 2d67 6c6f 6261 6c2d 6875 642d  -rio-global-hud-
-00058cc0: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-00058cd0: 6c65 7665 6c2d 322d 6267 3a20 7661 7228  level-2-bg: var(
-00058ce0: 2d2d 7269 6f2d 676c 6f62 616c 2d70 7269  --rio-global-pri
-00058cf0: 6d61 7279 2d62 6729 3b2d 2d72 696f 2d6c  mary-bg);--rio-l
-00058d00: 6f63 616c 2d6c 6576 656c 2d32 2d62 672d  ocal-level-2-bg-
-00058d10: 7661 7269 616e 743a 2076 6172 282d 2d72  variant: var(--r
-00058d20: 696f 2d67 6c6f 6261 6c2d 7072 696d 6172  io-global-primar
-00058d30: 792d 6267 2d76 6172 6961 6e74 293b 2d2d  y-bg-variant);--
-00058d40: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-00058d50: 322d 6267 2d61 6374 6976 653a 2076 6172  2-bg-active: var
-00058d60: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7072  (--rio-global-pr
-00058d70: 696d 6172 792d 6267 2d61 6374 6976 6529  imary-bg-active)
-00058d80: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
-00058d90: 656c 2d32 2d66 673a 2076 6172 282d 2d72  el-2-fg: var(--r
-00058da0: 696f 2d67 6c6f 6261 6c2d 7072 696d 6172  io-global-primar
-00058db0: 792d 6667 293b 2d2d 7269 6f2d 6c6f 6361  y-fg);--rio-loca
-00058dc0: 6c2d 6c65 7665 6c2d 332d 6267 3a20 7661  l-level-3-bg: va
-00058dd0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-00058de0: 6563 6f6e 6461 7279 2d62 6729 3b2d 2d72  econdary-bg);--r
-00058df0: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
-00058e00: 2d62 672d 7661 7269 616e 743a 2076 6172  -bg-variant: var
-00058e10: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
-00058e20: 636f 6e64 6172 792d 6267 2d76 6172 6961  condary-bg-varia
-00058e30: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
-00058e40: 6c65 7665 6c2d 332d 6267 2d61 6374 6976  level-3-bg-activ
-00058e50: 653a 2076 6172 282d 2d72 696f 2d67 6c6f  e: var(--rio-glo
-00058e60: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
-00058e70: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
-00058e80: 6f63 616c 2d6c 6576 656c 2d33 2d66 673a  ocal-level-3-fg:
-00058e90: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-00058ea0: 6c2d 7365 636f 6e64 6172 792d 6667 293b  l-secondary-fg);
-00058eb0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-00058ec0: 696e 6731 2d63 6f6c 6f72 3a20 7661 7228  ing1-color: var(
-00058ed0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6667 293b  --rio-local-fg);
-00058ee0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-00058ef0: 696e 6731 2d62 6163 6b67 726f 756e 643a  ing1-background:
-00058f00: 2022 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f   "none";--rio-lo
-00058f10: 6361 6c2d 6865 6164 696e 6731 2d62 6163  cal-heading1-bac
-00058f20: 6b67 726f 756e 642d 636c 6970 3a20 2262  kground-clip: "b
-00058f30: 6f72 6465 722d 626f 7822 3b2d 2d72 696f  order-box";--rio
-00058f40: 2d6c 6f63 616c 2d68 6561 6469 6e67 312d  -local-heading1-
-00058f50: 6669 6c6c 2d63 6f6c 6f72 3a20 2274 7261  fill-color: "tra
-00058f60: 6e73 7061 7265 6e74 223b 2d2d 7269 6f2d  nsparent";--rio-
-00058f70: 6c6f 6361 6c2d 6865 6164 696e 6732 2d63  local-heading2-c
-00058f80: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
-00058f90: 6c6f 6361 6c2d 6667 293b 2d2d 7269 6f2d  local-fg);--rio-
-00058fa0: 6c6f 6361 6c2d 6865 6164 696e 6732 2d62  local-heading2-b
-00058fb0: 6163 6b67 726f 756e 643a 2022 6e6f 6e65  ackground: "none
-00058fc0: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
-00058fd0: 6164 696e 6732 2d62 6163 6b67 726f 756e  ading2-backgroun
-00058fe0: 642d 636c 6970 3a20 2262 6f72 6465 722d  d-clip: "border-
-00058ff0: 626f 7822 3b2d 2d72 696f 2d6c 6f63 616c  box";--rio-local
-00059000: 2d68 6561 6469 6e67 322d 6669 6c6c 2d63  -heading2-fill-c
-00059010: 6f6c 6f72 3a20 2274 7261 6e73 7061 7265  olor: "transpare
-00059020: 6e74 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt";--rio-local-
-00059030: 6865 6164 696e 6733 2d63 6f6c 6f72 3a20  heading3-color: 
-00059040: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00059050: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-00059060: 6865 6164 696e 6733 2d62 6163 6b67 726f  heading3-backgro
-00059070: 756e 643a 2022 6e6f 6e65 223b 2d2d 7269  und: "none";--ri
-00059080: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
-00059090: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
-000590a0: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
-000590b0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-000590c0: 6e67 332d 6669 6c6c 2d63 6f6c 6f72 3a20  ng3-fill-color: 
-000590d0: 2274 7261 6e73 7061 7265 6e74 223b 2d2d  "transparent";--
-000590e0: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d63  rio-local-text-c
-000590f0: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
-00059100: 6c6f 6361 6c2d 6667 293b 2d2d 7269 6f2d  local-fg);--rio-
-00059110: 6c6f 6361 6c2d 7465 7874 2d62 6163 6b67  local-text-backg
-00059120: 726f 756e 643a 2022 6e6f 6e65 223b 2d2d  round: "none";--
-00059130: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d62  rio-local-text-b
-00059140: 6163 6b67 726f 756e 642d 636c 6970 3a20  ackground-clip: 
-00059150: 2262 6f72 6465 722d 626f 7822 3b2d 2d72  "border-box";--r
-00059160: 696f 2d6c 6f63 616c 2d74 6578 742d 6669  io-local-text-fi
-00059170: 6c6c 2d63 6f6c 6f72 3a20 2274 7261 6e73  ll-color: "trans
-00059180: 7061 7265 6e74 223b 636f 6c6f 723a 7661  parent";color:va
-00059190: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  r(--rio-local-fg
-000591a0: 297d 2e72 696f 2d73 7769 7463 6865 726f  )}.rio-switchero
-000591b0: 6f2d 7072 696d 6172 797b 2d2d 7269 6f2d  o-primary{--rio-
-000591c0: 6c6f 6361 6c2d 6267 3a20 7661 7228 2d2d  local-bg: var(--
-000591d0: 7269 6f2d 676c 6f62 616c 2d70 7269 6d61  rio-global-prima
-000591e0: 7279 2d62 6729 3b2d 2d72 696f 2d6c 6f63  ry-bg);--rio-loc
-000591f0: 616c 2d62 672d 7661 7269 616e 743a 2076  al-bg-variant: v
-00059200: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00059210: 7072 696d 6172 792d 6267 2d76 6172 6961  primary-bg-varia
-00059220: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
-00059230: 6267 2d61 6374 6976 653a 2076 6172 282d  bg-active: var(-
-00059240: 2d72 696f 2d67 6c6f 6261 6c2d 7072 696d  -rio-global-prim
-00059250: 6172 792d 6267 2d61 6374 6976 6529 3b2d  ary-bg-active);-
-00059260: 2d72 696f 2d6c 6f63 616c 2d66 673a 2076  -rio-local-fg: v
-00059270: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00059280: 7072 696d 6172 792d 6667 293b 2d2d 7269  primary-fg);--ri
-00059290: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 322d  o-local-level-2-
-000592a0: 6267 3a20 7661 7228 2d2d 7269 6f2d 676c  bg: var(--rio-gl
-000592b0: 6f62 616c 2d73 6563 6f6e 6461 7279 2d62  obal-secondary-b
-000592c0: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
-000592d0: 6576 656c 2d32 2d62 672d 7661 7269 616e  evel-2-bg-varian
-000592e0: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
-000592f0: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
-00059300: 2d76 6172 6961 6e74 293b 2d2d 7269 6f2d  -variant);--rio-
-00059310: 6c6f 6361 6c2d 6c65 7665 6c2d 322d 6267  local-level-2-bg
-00059320: 2d61 6374 6976 653a 2076 6172 282d 2d72  -active: var(--r
-00059330: 696f 2d67 6c6f 6261 6c2d 7365 636f 6e64  io-global-second
-00059340: 6172 792d 6267 2d61 6374 6976 6529 3b2d  ary-bg-active);-
-00059350: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
-00059360: 2d32 2d66 673a 2076 6172 282d 2d72 696f  -2-fg: var(--rio
-00059370: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
-00059380: 792d 6667 293b 2d2d 7269 6f2d 6c6f 6361  y-fg);--rio-loca
-00059390: 6c2d 6c65 7665 6c2d 332d 6267 3a20 7661  l-level-3-bg: va
-000593a0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d70  r(--rio-global-p
-000593b0: 7269 6d61 7279 2d62 6729 3b2d 2d72 696f  rimary-bg);--rio
-000593c0: 2d6c 6f63 616c 2d6c 6576 656c 2d33 2d62  -local-level-3-b
-000593d0: 672d 7661 7269 616e 743a 2076 6172 282d  g-variant: var(-
-000593e0: 2d72 696f 2d67 6c6f 6261 6c2d 7072 696d  -rio-global-prim
-000593f0: 6172 792d 6267 2d76 6172 6961 6e74 293b  ary-bg-variant);
-00059400: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-00059410: 6c2d 332d 6267 2d61 6374 6976 653a 2076  l-3-bg-active: v
-00059420: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00059430: 7072 696d 6172 792d 6267 2d61 6374 6976  primary-bg-activ
-00059440: 6529 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  e);--rio-local-l
-00059450: 6576 656c 2d33 2d66 673a 2076 6172 282d  evel-3-fg: var(-
-00059460: 2d72 696f 2d67 6c6f 6261 6c2d 7072 696d  -rio-global-prim
-00059470: 6172 792d 6667 293b 2d2d 7269 6f2d 6c6f  ary-fg);--rio-lo
-00059480: 6361 6c2d 6865 6164 696e 6731 2d63 6f6c  cal-heading1-col
-00059490: 6f72 3a20 7661 7228 2d2d 7269 6f2d 6c6f  or: var(--rio-lo
-000594a0: 6361 6c2d 6667 293b 2d2d 7269 6f2d 6c6f  cal-fg);--rio-lo
-000594b0: 6361 6c2d 6865 6164 696e 6731 2d62 6163  cal-heading1-bac
-000594c0: 6b67 726f 756e 643a 2022 6e6f 6e65 223b  kground: "none";
-000594d0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-000594e0: 696e 6731 2d62 6163 6b67 726f 756e 642d  ing1-background-
-000594f0: 636c 6970 3a20 2262 6f72 6465 722d 626f  clip: "border-bo
-00059500: 7822 3b2d 2d72 696f 2d6c 6f63 616c 2d68  x";--rio-local-h
-00059510: 6561 6469 6e67 312d 6669 6c6c 2d63 6f6c  eading1-fill-col
-00059520: 6f72 3a20 2274 7261 6e73 7061 7265 6e74  or: "transparent
-00059530: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
-00059540: 6164 696e 6732 2d63 6f6c 6f72 3a20 7661  ading2-color: va
-00059550: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  r(--rio-local-fg
-00059560: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
-00059570: 6164 696e 6732 2d62 6163 6b67 726f 756e  ading2-backgroun
-00059580: 643a 2022 6e6f 6e65 223b 2d2d 7269 6f2d  d: "none";--rio-
-00059590: 6c6f 6361 6c2d 6865 6164 696e 6732 2d62  local-heading2-b
-000595a0: 6163 6b67 726f 756e 642d 636c 6970 3a20  ackground-clip: 
-000595b0: 2262 6f72 6465 722d 626f 7822 3b2d 2d72  "border-box";--r
-000595c0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-000595d0: 322d 6669 6c6c 2d63 6f6c 6f72 3a20 2274  2-fill-color: "t
-000595e0: 7261 6e73 7061 7265 6e74 223b 2d2d 7269  ransparent";--ri
-000595f0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
-00059600: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
-00059610: 6f2d 6c6f 6361 6c2d 6667 293b 2d2d 7269  o-local-fg);--ri
-00059620: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
-00059630: 2d62 6163 6b67 726f 756e 643a 2022 6e6f  -background: "no
-00059640: 6e65 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ne";--rio-local-
-00059650: 6865 6164 696e 6733 2d62 6163 6b67 726f  heading3-backgro
-00059660: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
-00059670: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
-00059680: 616c 2d68 6561 6469 6e67 332d 6669 6c6c  al-heading3-fill
-00059690: 2d63 6f6c 6f72 3a20 2274 7261 6e73 7061  -color: "transpa
-000596a0: 7265 6e74 223b 2d2d 7269 6f2d 6c6f 6361  rent";--rio-loca
-000596b0: 6c2d 7465 7874 2d63 6f6c 6f72 3a20 7661  l-text-color: va
-000596c0: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  r(--rio-local-fg
-000596d0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  );--rio-local-te
-000596e0: 7874 2d62 6163 6b67 726f 756e 643a 2022  xt-background: "
-000596f0: 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f 6361  none";--rio-loca
-00059700: 6c2d 7465 7874 2d62 6163 6b67 726f 756e  l-text-backgroun
-00059710: 642d 636c 6970 3a20 2262 6f72 6465 722d  d-clip: "border-
-00059720: 626f 7822 3b2d 2d72 696f 2d6c 6f63 616c  box";--rio-local
-00059730: 2d74 6578 742d 6669 6c6c 2d63 6f6c 6f72  -text-fill-color
-00059740: 3a20 2274 7261 6e73 7061 7265 6e74 223b  : "transparent";
-00059750: 636f 6c6f 723a 7661 7228 2d2d 7269 6f2d  color:var(--rio-
-00059760: 6c6f 6361 6c2d 6667 297d 2e72 696f 2d73  local-fg)}.rio-s
-00059770: 7769 7463 6865 726f 6f2d 7365 636f 6e64  witcheroo-second
-00059780: 6172 797b 2d2d 7269 6f2d 6c6f 6361 6c2d  ary{--rio-local-
-00059790: 6267 3a20 7661 7228 2d2d 7269 6f2d 676c  bg: var(--rio-gl
-000597a0: 6f62 616c 2d73 6563 6f6e 6461 7279 2d62  obal-secondary-b
-000597b0: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d62  g);--rio-local-b
-000597c0: 672d 7661 7269 616e 743a 2076 6172 282d  g-variant: var(-
-000597d0: 2d72 696f 2d67 6c6f 6261 6c2d 7365 636f  -rio-global-seco
-000597e0: 6e64 6172 792d 6267 2d76 6172 6961 6e74  ndary-bg-variant
-000597f0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6267  );--rio-local-bg
-00059800: 2d61 6374 6976 653a 2076 6172 282d 2d72  -active: var(--r
+00053fd0: 2822 6469 7622 293b 7265 7475 726e 2074  ("div");return t
+00053fe0: 6869 732e 7461 626c 6545 6c65 6d65 6e74  his.tableElement
+00053ff0: 3d64 6f63 756d 656e 742e 6372 6561 7465  =document.create
+00054000: 456c 656d 656e 7428 2264 6976 2229 2c74  Element("div"),t
+00054010: 6869 732e 7461 626c 6545 6c65 6d65 6e74  his.tableElement
+00054020: 2e63 6c61 7373 4c69 7374 2e61 6464 2822  .classList.add("
+00054030: 7269 6f2d 7461 626c 6522 292c 652e 6170  rio-table"),e.ap
+00054040: 7065 6e64 4368 696c 6428 7468 6973 2e74  pendChild(this.t
+00054050: 6162 6c65 456c 656d 656e 7429 2c65 7d75  ableElement),e}u
+00054060: 7064 6174 6545 6c65 6d65 6e74 2865 2c6e  pdateElement(e,n
+00054070: 297b 652e 6461 7461 213d 3d76 6f69 6420  ){e.data!==void 
+00054080: 303f 2874 6869 732e 7374 6174 652e 6461  0?(this.state.da
+00054090: 7461 3d53 7528 652e 6461 7461 292c 7468  ta=Su(e.data),th
+000540a0: 6973 2e64 6973 706c 6179 4461 7461 2829  is.displayData()
+000540b0: 2c28 652e 7368 6f77 5f72 6f77 5f6e 756d  ,(e.show_row_num
+000540c0: 6265 7273 3f3f 7468 6973 2e73 7461 7465  bers??this.state
+000540d0: 2e73 686f 775f 726f 775f 6e75 6d62 6572  .show_row_number
+000540e0: 7329 2626 7468 6973 2e73 686f 7752 6f77  s)&&this.showRow
+000540f0: 4e75 6d62 6572 7328 292c 4172 7261 792e  Numbers(),Array.
+00054100: 6973 4172 7261 7928 652e 6461 7461 293f  isArray(e.data)?
+00054110: 7468 6973 2e68 6964 6543 6f6c 756d 6e48  this.hideColumnH
+00054120: 6561 6465 7273 2829 3a74 6869 732e 7368  eaders():this.sh
+00054130: 6f77 436f 6c75 6d6e 4865 6164 6572 7328  owColumnHeaders(
+00054140: 2929 3a65 2e73 686f 775f 726f 775f 6e75  )):e.show_row_nu
+00054150: 6d62 6572 7321 3d3d 766f 6964 2030 2626  mbers!==void 0&&
+00054160: 652e 7368 6f77 5f72 6f77 5f6e 756d 6265  e.show_row_numbe
+00054170: 7273 213d 3d74 6869 732e 7374 6174 652e  rs!==this.state.
+00054180: 7368 6f77 5f72 6f77 5f6e 756d 6265 7273  show_row_numbers
+00054190: 2626 2865 2e73 686f 775f 726f 775f 6e75  &&(e.show_row_nu
+000541a0: 6d62 6572 733f 7468 6973 2e73 686f 7752  mbers?this.showR
+000541b0: 6f77 4e75 6d62 6572 7328 293a 7468 6973  owNumbers():this
+000541c0: 2e68 6964 6552 6f77 4e75 6d62 6572 7328  .hideRowNumbers(
+000541d0: 2929 2c74 6869 732e 6d61 6b65 4c61 796f  )),this.makeLayo
+000541e0: 7574 4469 7274 7928 292c 5b74 6869 732e  utDirty(),[this.
+000541f0: 6e61 7475 7261 6c57 6964 7468 2c74 6869  naturalWidth,thi
+00054200: 732e 6e61 7475 7261 6c48 6569 6768 745d  s.naturalHeight]
+00054210: 3d61 7428 7468 6973 2e74 6162 6c65 456c  =at(this.tableEl
+00054220: 656d 656e 7429 7d75 7064 6174 654e 6174  ement)}updateNat
+00054230: 7572 616c 5769 6474 6828 6529 7b7d 7570  uralWidth(e){}up
+00054240: 6461 7465 4e61 7475 7261 6c48 6569 6768  dateNaturalHeigh
+00054250: 7428 6529 7b7d 6469 7370 6c61 7944 6174  t(e){}displayDat
+00054260: 6128 297b 666f 7228 6c65 7420 6e20 6f66  a(){for(let n of
+00054270: 2074 6869 732e 6461 7461 4365 6c6c 7329   this.dataCells)
+00054280: 6e2e 7265 6d6f 7665 2829 3b74 6869 732e  n.remove();this.
+00054290: 6461 7461 4365 6c6c 733d 5b5d 3b6c 6574  dataCells=[];let
+000542a0: 2065 3d32 3b66 6f72 286c 6574 206e 206f   e=2;for(let n o
+000542b0: 6620 7468 6973 2e73 7461 7465 2e64 6174  f this.state.dat
+000542c0: 6129 7b66 6f72 286c 6574 5b69 2c72 5d6f  a){for(let[i,r]o
+000542d0: 6620 6e2e 7661 6c75 6573 2e65 6e74 7269  f n.values.entri
+000542e0: 6573 2829 297b 6c65 7420 733d 646f 6375  es()){let s=docu
+000542f0: 6d65 6e74 2e63 7265 6174 6545 6c65 6d65  ment.createEleme
+00054300: 6e74 2822 7370 616e 2229 3b73 2e74 6578  nt("span");s.tex
+00054310: 7443 6f6e 7465 6e74 3d60 247b 727d 602c  tContent=`${r}`,
+00054320: 732e 7374 796c 652e 7465 7874 416c 6967  s.style.textAlig
+00054330: 6e3d 6e2e 616c 6967 6e6d 656e 742c 732e  n=n.alignment,s.
+00054340: 7374 796c 652e 6772 6964 526f 773d 6024  style.gridRow=`$
+00054350: 7b69 2b32 7d60 2c73 2e73 7479 6c65 2e67  {i+2}`,s.style.g
+00054360: 7269 6443 6f6c 756d 6e3d 6024 7b65 7d60  ridColumn=`${e}`
+00054370: 2c74 6869 732e 7461 626c 6545 6c65 6d65  ,this.tableEleme
+00054380: 6e74 2e61 7070 656e 6443 6869 6c64 2873  nt.appendChild(s
+00054390: 292c 7468 6973 2e64 6174 6143 656c 6c73  ),this.dataCells
+000543a0: 2e70 7573 6828 7329 7d65 2b2b 7d7d 7368  .push(s)}e++}}sh
+000543b0: 6f77 526f 774e 756d 6265 7273 2829 7b74  owRowNumbers(){t
+000543c0: 6869 732e 6869 6465 526f 774e 756d 6265  his.hideRowNumbe
+000543d0: 7273 2829 3b6c 6574 2065 3d74 6869 732e  rs();let e=this.
+000543e0: 7374 6174 652e 6461 7461 2e6c 656e 6774  state.data.lengt
+000543f0: 683d 3d3d 303f 303a 7468 6973 2e73 7461  h===0?0:this.sta
+00054400: 7465 2e64 6174 615b 305d 2e76 616c 7565  te.data[0].value
+00054410: 732e 6c65 6e67 7468 3b66 6f72 286c 6574  s.length;for(let
+00054420: 206e 3d30 3b6e 3c65 3b6e 2b2b 297b 6c65   n=0;n<e;n++){le
+00054430: 7420 693d 646f 6375 6d65 6e74 2e63 7265  t i=document.cre
+00054440: 6174 6545 6c65 6d65 6e74 2822 7370 616e  ateElement("span
+00054450: 2229 3b69 2e74 6578 7443 6f6e 7465 6e74  ");i.textContent
+00054460: 3d60 247b 6e2b 317d 2e60 2c69 2e73 7479  =`${n+1}.`,i.sty
+00054470: 6c65 2e74 6578 7441 6c69 676e 3d22 7269  le.textAlign="ri
+00054480: 6768 7422 2c69 2e73 7479 6c65 2e6f 7061  ght",i.style.opa
+00054490: 6369 7479 3d22 302e 3522 2c69 2e73 7479  city="0.5",i.sty
+000544a0: 6c65 2e67 7269 6452 6f77 3d60 247b 6e2b  le.gridRow=`${n+
+000544b0: 327d 602c 692e 7374 796c 652e 6772 6964  2}`,i.style.grid
+000544c0: 436f 6c75 6d6e 3d22 3122 2c74 6869 732e  Column="1",this.
+000544d0: 7461 626c 6545 6c65 6d65 6e74 2e61 7070  tableElement.app
+000544e0: 656e 6443 6869 6c64 2869 292c 7468 6973  endChild(i),this
+000544f0: 2e72 6f77 4e75 6d62 6572 4365 6c6c 732e  .rowNumberCells.
+00054500: 7075 7368 2869 297d 7d68 6964 6552 6f77  push(i)}}hideRow
+00054510: 4e75 6d62 6572 7328 297b 666f 7228 6c65  Numbers(){for(le
+00054520: 7420 6520 6f66 2074 6869 732e 726f 774e  t e of this.rowN
+00054530: 756d 6265 7243 656c 6c73 2965 2e72 656d  umberCells)e.rem
+00054540: 6f76 6528 293b 7468 6973 2e72 6f77 4e75  ove();this.rowNu
+00054550: 6d62 6572 4365 6c6c 733d 5b5d 7d73 686f  mberCells=[]}sho
+00054560: 7743 6f6c 756d 6e48 6561 6465 7273 2829  wColumnHeaders()
+00054570: 7b74 6869 732e 6869 6465 436f 6c75 6d6e  {this.hideColumn
+00054580: 4865 6164 6572 7328 293b 666f 7228 6c65  Headers();for(le
+00054590: 745b 652c 6e5d 6f66 2074 6869 732e 7374  t[e,n]of this.st
+000545a0: 6174 652e 6461 7461 2e65 6e74 7269 6573  ate.data.entries
+000545b0: 2829 297b 6c65 7420 693d 646f 6375 6d65  ()){let i=docume
+000545c0: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
+000545d0: 2822 7370 616e 2229 3b69 2e63 6c61 7373  ("span");i.class
+000545e0: 4c69 7374 2e61 6464 2822 6865 6164 6572  List.add("header
+000545f0: 2229 2c69 2e74 6578 7443 6f6e 7465 6e74  "),i.textContent
+00054600: 3d6e 2e6e 616d 652c 692e 7374 796c 652e  =n.name,i.style.
+00054610: 7465 7874 416c 6967 6e3d 6e2e 616c 6967  textAlign=n.alig
+00054620: 6e6d 656e 742c 692e 7374 796c 652e 6f70  nment,i.style.op
+00054630: 6163 6974 793d 2230 2e35 222c 692e 6164  acity="0.5",i.ad
+00054640: 6445 7665 6e74 4c69 7374 656e 6572 2822  dEventListener("
+00054650: 636c 6963 6b22 2c74 6869 732e 6f6e 4865  click",this.onHe
+00054660: 6164 6572 436c 6963 6b2e 6269 6e64 2874  aderClick.bind(t
+00054670: 6869 732c 6e2e 6e61 6d65 2929 2c69 2e73  his,n.name)),i.s
+00054680: 7479 6c65 2e67 7269 6452 6f77 3d22 3122  tyle.gridRow="1"
+00054690: 2c69 2e73 7479 6c65 2e67 7269 6443 6f6c  ,i.style.gridCol
+000546a0: 756d 6e3d 6024 7b65 2b32 7d60 2c74 6869  umn=`${e+2}`,thi
+000546b0: 732e 7461 626c 6545 6c65 6d65 6e74 2e61  s.tableElement.a
+000546c0: 7070 656e 6443 6869 6c64 2869 292c 7468  ppendChild(i),th
+000546d0: 6973 2e68 6561 6465 7243 656c 6c73 2e70  is.headerCells.p
+000546e0: 7573 6828 6929 7d7d 6869 6465 436f 6c75  ush(i)}}hideColu
+000546f0: 6d6e 4865 6164 6572 7328 297b 666f 7228  mnHeaders(){for(
+00054700: 6c65 7420 6520 6f66 2074 6869 732e 6865  let e of this.he
+00054710: 6164 6572 4365 6c6c 7329 652e 7265 6d6f  aderCells)e.remo
+00054720: 7665 2829 3b74 6869 732e 6865 6164 6572  ve();this.header
+00054730: 4365 6c6c 733d 5b5d 7d6f 6e48 6561 6465  Cells=[]}onHeade
+00054740: 7243 6c69 636b 2865 2c6e 297b 6c65 7420  rClick(e,n){let 
+00054750: 693d 6e2e 7461 7267 6574 3b69 2e74 6167  i=n.target;i.tag
+00054760: 4e61 6d65 213d 3d22 5350 414e 2226 2628  Name!=="SPAN"&&(
+00054770: 693d 692e 7061 7265 6e74 456c 656d 656e  i=i.parentElemen
+00054780: 7429 3b6c 6574 2072 3d69 2e64 6174 6173  t);let r=i.datas
+00054790: 6574 2e73 6f72 7421 3d3d 2261 7363 656e  et.sort!=="ascen
+000547a0: 6469 6e67 223b 666f 7228 6c65 7420 7320  ding";for(let s 
+000547b0: 6f66 2074 6869 732e 6865 6164 6572 4365  of this.headerCe
+000547c0: 6c6c 7329 6465 6c65 7465 2073 2e64 6174  lls)delete s.dat
+000547d0: 6173 6574 2e73 6f72 743b 692e 6461 7461  aset.sort;i.data
+000547e0: 7365 742e 736f 7274 3d72 3f22 6173 6365  set.sort=r?"asce
+000547f0: 6e64 696e 6722 3a22 6465 7363 656e 6469  nding":"descendi
+00054800: 6e67 222c 7468 6973 2e73 6f72 744f 7264  ng",this.sortOrd
+00054810: 6572 2e61 6464 2865 2c72 292c 7468 6973  er.add(e,r),this
+00054820: 2e73 6f72 744f 7264 6572 2e73 6f72 7428  .sortOrder.sort(
+00054830: 7468 6973 2e73 7461 7465 2e64 6174 6129  this.state.data)
+00054840: 2c74 6869 732e 6469 7370 6c61 7944 6174  ,this.displayDat
+00054850: 6128 292c 6e2e 7374 6f70 5072 6f70 6167  a(),n.stopPropag
+00054860: 6174 696f 6e28 297d 7d63 6c61 7373 2052  ation()}}class R
+00054870: 7520 6578 7465 6e64 7320 557b 6372 6561  u extends U{crea
+00054880: 7465 456c 656d 656e 7428 297b 6c65 7420  teElement(){let 
+00054890: 653d 646f 6375 6d65 6e74 2e63 7265 6174  e=document.creat
+000548a0: 6545 6c65 6d65 6e74 2822 6469 7622 293b  eElement("div");
+000548b0: 7265 7475 726e 2065 2e63 6c61 7373 4c69  return e.classLi
+000548c0: 7374 2e61 6464 2822 7269 6f2d 7465 7874  st.add("rio-text
+000548d0: 2229 2c74 6869 732e 696e 6e65 723d 646f  "),this.inner=do
+000548e0: 6375 6d65 6e74 2e63 7265 6174 6545 6c65  cument.createEle
+000548f0: 6d65 6e74 2822 6469 7622 292c 652e 6170  ment("div"),e.ap
+00054900: 7065 6e64 4368 696c 6428 7468 6973 2e69  pendChild(this.i
+00054910: 6e6e 6572 292c 657d 7570 6461 7465 456c  nner),e}updateEl
+00054920: 656d 656e 7428 652c 6e29 7b73 7769 7463  ement(e,n){switc
+00054930: 6828 652e 7465 7874 213d 3d76 6f69 6420  h(e.text!==void 
+00054940: 3026 2628 7468 6973 2e69 6e6e 6572 2e74  0&&(this.inner.t
+00054950: 6578 7443 6f6e 7465 6e74 3d65 2e74 6578  extContent=e.tex
+00054960: 7429 2c65 2e77 7261 7029 7b63 6173 6521  t),e.wrap){case!
+00054970: 313a 7468 6973 2e69 6e6e 6572 2e73 7479  1:this.inner.sty
+00054980: 6c65 2e77 6869 7465 5370 6163 653d 2270  le.whiteSpace="p
+00054990: 7265 222c 7468 6973 2e69 6e6e 6572 2e73  re",this.inner.s
+000549a0: 7479 6c65 2e74 6578 744f 7665 7266 6c6f  tyle.textOverflo
+000549b0: 773d 2263 6c69 7022 3b62 7265 616b 3b63  w="clip";break;c
+000549c0: 6173 6521 303a 7468 6973 2e69 6e6e 6572  ase!0:this.inner
+000549d0: 2e73 7479 6c65 2e77 6869 7465 5370 6163  .style.whiteSpac
+000549e0: 653d 2270 7265 2d77 7261 7022 2c74 6869  e="pre-wrap",thi
+000549f0: 732e 696e 6e65 722e 7374 796c 652e 7465  s.inner.style.te
+00054a00: 7874 4f76 6572 666c 6f77 3d22 636c 6970  xtOverflow="clip
+00054a10: 223b 6272 6561 6b3b 6361 7365 2265 6c6c  ";break;case"ell
+00054a20: 6970 7369 7a65 223a 7468 6973 2e69 6e6e  ipsize":this.inn
+00054a30: 6572 2e73 7479 6c65 2e77 6869 7465 5370  er.style.whiteSp
+00054a40: 6163 653d 2270 7265 222c 7468 6973 2e69  ace="pre",this.i
+00054a50: 6e6e 6572 2e73 7479 6c65 2e74 6578 744f  nner.style.textO
+00054a60: 7665 7266 6c6f 773d 2265 6c6c 6970 7369  verflow="ellipsi
+00054a70: 7322 3b62 7265 616b 7d65 2e73 656c 6563  s";break}e.selec
+00054a80: 7461 626c 6521 3d3d 766f 6964 2030 2626  table!==void 0&&
+00054a90: 2874 6869 732e 696e 6e65 722e 7374 796c  (this.inner.styl
+00054aa0: 652e 706f 696e 7465 7245 7665 6e74 733d  e.pointerEvents=
+00054ab0: 652e 7365 6c65 6374 6162 6c65 3f22 6175  e.selectable?"au
+00054ac0: 746f 223a 226e 6f6e 6522 292c 652e 7374  to":"none"),e.st
+00054ad0: 796c 6521 3d3d 766f 6964 2030 2626 4f62  yle!==void 0&&Ob
+00054ae0: 6a65 6374 2e61 7373 6967 6e28 7468 6973  ject.assign(this
+00054af0: 2e69 6e6e 6572 2e73 7479 6c65 2c54 7428  .inner.style,Tt(
+00054b00: 652e 7374 796c 6529 292c 652e 6a75 7374  e.style)),e.just
+00054b10: 6966 7921 3d3d 766f 6964 2030 2626 2874  ify!==void 0&&(t
+00054b20: 6869 732e 696e 6e65 722e 7374 796c 652e  his.inner.style.
+00054b30: 7465 7874 416c 6967 6e3d 652e 6a75 7374  textAlign=e.just
+00054b40: 6966 7929 2c28 652e 7465 7874 213d 3d76  ify),(e.text!==v
+00054b50: 6f69 6420 307c 7c65 2e77 7261 7021 3d3d  oid 0||e.wrap!==
+00054b60: 766f 6964 2030 7c7c 652e 7374 796c 6521  void 0||e.style!
+00054b70: 3d3d 766f 6964 2030 2926 2628 7468 6973  ==void 0)&&(this
+00054b80: 2e6d 616b 654c 6179 6f75 7444 6972 7479  .makeLayoutDirty
+00054b90: 2829 2c74 6869 732e 6361 6368 6564 4e6f  (),this.cachedNo
+00054ba0: 5772 6170 4469 6d65 6e73 696f 6e73 3d6b  WrapDimensions=k
+00054bb0: 6528 7468 6973 2e65 6c65 6d65 6e74 2e74  e(this.element.t
+00054bc0: 6578 7443 6f6e 7465 6e74 2c74 6869 732e  extContent,this.
+00054bd0: 7374 6174 652e 7374 796c 6529 297d 7570  state.style))}up
+00054be0: 6461 7465 4e61 7475 7261 6c57 6964 7468  dateNaturalWidth
+00054bf0: 2865 297b 7468 6973 2e73 7461 7465 2e77  (e){this.state.w
+00054c00: 7261 703d 3d3d 2131 3f74 6869 732e 6e61  rap===!1?this.na
+00054c10: 7475 7261 6c57 6964 7468 3d74 6869 732e  turalWidth=this.
+00054c20: 6361 6368 6564 4e6f 5772 6170 4469 6d65  cachedNoWrapDime
+00054c30: 6e73 696f 6e73 5b30 5d3a 7468 6973 2e6e  nsions[0]:this.n
+00054c40: 6174 7572 616c 5769 6474 683d 307d 7570  aturalWidth=0}up
+00054c50: 6461 7465 4e61 7475 7261 6c48 6569 6768  dateNaturalHeigh
+00054c60: 7428 6529 7b74 6869 732e 7374 6174 652e  t(e){this.state.
+00054c70: 7772 6170 3d3d 3d21 303f 7468 6973 2e6e  wrap===!0?this.n
+00054c80: 6174 7572 616c 4865 6967 6874 3d6b 6528  aturalHeight=ke(
+00054c90: 7468 6973 2e73 7461 7465 2e74 6578 742c  this.state.text,
+00054ca0: 7468 6973 2e73 7461 7465 2e73 7479 6c65  this.state.style
+00054cb0: 2c74 6869 732e 616c 6c6f 6361 7465 6457  ,this.allocatedW
+00054cc0: 6964 7468 295b 315d 3a74 6869 732e 6e61  idth)[1]:this.na
+00054cd0: 7475 7261 6c48 6569 6768 743d 7468 6973  turalHeight=this
+00054ce0: 2e63 6163 6865 644e 6f57 7261 7044 696d  .cachedNoWrapDim
+00054cf0: 656e 7369 6f6e 735b 315d 7d7d 636c 6173  ensions[1]}}clas
+00054d00: 7320 4d75 2065 7874 656e 6473 2055 7b63  s Mu extends U{c
+00054d10: 6f6e 7374 7275 6374 6f72 2829 7b73 7570  onstructor(){sup
+00054d20: 6572 282e 2e2e 6172 6775 6d65 6e74 7329  er(...arguments)
+00054d30: 2c74 6869 732e 7072 6566 6978 5465 7874  ,this.prefixText
+00054d40: 5769 6474 683d 302c 7468 6973 2e73 7566  Width=0,this.suf
+00054d50: 6669 7854 6578 7457 6964 7468 3d30 7d63  fixTextWidth=0}c
+00054d60: 7265 6174 6545 6c65 6d65 6e74 2829 7b6c  reateElement(){l
+00054d70: 6574 2065 3d64 6f63 756d 656e 742e 6372  et e=document.cr
+00054d80: 6561 7465 456c 656d 656e 7428 2264 6976  eateElement("div
+00054d90: 2229 3b72 6574 7572 6e20 652e 636c 6173  ");return e.clas
+00054da0: 734c 6973 742e 6164 6428 2272 696f 2d74  sList.add("rio-t
+00054db0: 6578 742d 696e 7075 7422 2c22 7269 6f2d  ext-input","rio-
+00054dc0: 696e 7075 742d 626f 7822 292c 652e 696e  input-box"),e.in
+00054dd0: 6e65 7248 544d 4c3d 600a 2020 2020 2020  nerHTML=`.      
+00054de0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
+00054df0: 653d 2274 6578 7422 2073 7479 6c65 3d22  e="text" style="
+00054e00: 6f72 6465 723a 2032 2220 706c 6163 6568  order: 2" placeh
+00054e10: 6f6c 6465 723d 2222 3e0a 2020 2020 2020  older="">.      
+00054e20: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00054e30: 3d22 7269 6f2d 7465 7874 2d69 6e70 7574  ="rio-text-input
+00054e40: 2d68 696e 742d 7465 7874 2072 696f 2d74  -hint-text rio-t
+00054e50: 6578 742d 696e 7075 742d 7072 6566 6978  ext-input-prefix
+00054e60: 2d74 6578 7422 2073 7479 6c65 3d22 6f72  -text" style="or
+00054e70: 6465 723a 2031 223e 3c2f 6469 763e 0a20  der: 1"></div>. 
+00054e80: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00054e90: 636c 6173 733d 2272 696f 2d74 6578 742d  class="rio-text-
+00054ea0: 696e 7075 742d 6869 6e74 2d74 6578 7420  input-hint-text 
+00054eb0: 7269 6f2d 7465 7874 2d69 6e70 7574 2d73  rio-text-input-s
+00054ec0: 7566 6669 782d 7465 7874 2220 7374 796c  uffix-text" styl
+00054ed0: 653d 226f 7264 6572 3a20 3322 3e3c 2f64  e="order: 3"></d
+00054ee0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00054ef0: 3c64 6976 2063 6c61 7373 3d22 7269 6f2d  <div class="rio-
+00054f00: 696e 7075 742d 626f 782d 6c61 6265 6c22  input-box-label"
+00054f10: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
+00054f20: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00054f30: 7269 6f2d 696e 7075 742d 626f 782d 706c  rio-input-box-pl
+00054f40: 6169 6e2d 6261 7222 3e3c 2f64 6976 3e0a  ain-bar"></div>.
+00054f50: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00054f60: 2063 6c61 7373 3d22 7269 6f2d 696e 7075   class="rio-inpu
+00054f70: 742d 626f 782d 636f 6c6f 722d 6261 7222  t-box-color-bar"
+00054f80: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
+00054f90: 602c 7468 6973 2e6c 6162 656c 456c 656d  `,this.labelElem
+00054fa0: 656e 743d 652e 7175 6572 7953 656c 6563  ent=e.querySelec
+00054fb0: 746f 7228 222e 7269 6f2d 696e 7075 742d  tor(".rio-input-
+00054fc0: 626f 782d 6c61 6265 6c22 292c 5b74 6869  box-label"),[thi
+00054fd0: 732e 7072 6566 6978 5465 7874 456c 656d  s.prefixTextElem
+00054fe0: 656e 742c 7468 6973 2e73 7566 6669 7854  ent,this.suffixT
+00054ff0: 6578 7445 6c65 6d65 6e74 5d3d 4172 7261  extElement]=Arra
+00055000: 792e 6672 6f6d 2865 2e71 7565 7279 5365  y.from(e.querySe
+00055010: 6c65 6374 6f72 416c 6c28 222e 7269 6f2d  lectorAll(".rio-
+00055020: 7465 7874 2d69 6e70 7574 2d68 696e 742d  text-input-hint-
+00055030: 7465 7874 2229 292c 7468 6973 2e69 6e70  text")),this.inp
+00055040: 7574 456c 656d 656e 743d 652e 7175 6572  utElement=e.quer
+00055050: 7953 656c 6563 746f 7228 2269 6e70 7574  ySelector("input
+00055060: 2229 2c74 6869 732e 696e 7075 7445 6c65  "),this.inputEle
+00055070: 6d65 6e74 2e61 6464 4576 656e 744c 6973  ment.addEventLis
+00055080: 7465 6e65 7228 2262 6c75 7222 2c28 293d  tener("blur",()=
+00055090: 3e7b 7468 6973 2e73 6574 5374 6174 6541  >{this.setStateA
+000550a0: 6e64 4e6f 7469 6679 4261 636b 656e 6428  ndNotifyBackend(
+000550b0: 7b74 6578 743a 7468 6973 2e69 6e70 7574  {text:this.input
+000550c0: 456c 656d 656e 742e 7661 6c75 657d 297d  Element.value})}
+000550d0: 292c 7468 6973 2e69 6e70 7574 456c 656d  ),this.inputElem
+000550e0: 656e 742e 6164 6445 7665 6e74 4c69 7374  ent.addEventList
+000550f0: 656e 6572 2822 6b65 7964 6f77 6e22 2c6e  ener("keydown",n
+00055100: 3d3e 7b6e 2e6b 6579 3d3d 3d22 456e 7465  =>{n.key==="Ente
+00055110: 7222 2626 2874 6869 732e 7374 6174 652e  r"&&(this.state.
+00055120: 7465 7874 3d74 6869 732e 696e 7075 7445  text=this.inputE
+00055130: 6c65 6d65 6e74 2e76 616c 7565 2c74 6869  lement.value,thi
+00055140: 732e 7365 6e64 4d65 7373 6167 6554 6f42  s.sendMessageToB
+00055150: 6163 6b65 6e64 287b 7465 7874 3a74 6869  ackend({text:thi
+00055160: 732e 7374 6174 652e 7465 7874 7d29 292c  s.state.text})),
+00055170: 6e2e 7374 6f70 5072 6f70 6167 6174 696f  n.stopPropagatio
+00055180: 6e28 297d 292c 7468 6973 2e70 7265 6669  n()}),this.prefi
+00055190: 7854 6578 7445 6c65 6d65 6e74 2e61 6464  xTextElement.add
+000551a0: 4576 656e 744c 6973 7465 6e65 7228 226d  EventListener("m
+000551b0: 6f75 7365 646f 776e 222c 6e3d 3e7b 6e2e  ousedown",n=>{n.
+000551c0: 7374 6f70 5072 6f70 6167 6174 696f 6e28  stopPropagation(
+000551d0: 297d 292c 7468 6973 2e73 7566 6669 7854  )}),this.suffixT
+000551e0: 6578 7445 6c65 6d65 6e74 2e61 6464 4576  extElement.addEv
+000551f0: 656e 744c 6973 7465 6e65 7228 226d 6f75  entListener("mou
+00055200: 7365 646f 776e 222c 6e3d 3e7b 6e2e 7374  sedown",n=>{n.st
+00055210: 6f70 5072 6f70 6167 6174 696f 6e28 297d  opPropagation()}
+00055220: 292c 7468 6973 2e70 7265 6669 7854 6578  ),this.prefixTex
+00055230: 7445 6c65 6d65 6e74 2e61 6464 4576 656e  tElement.addEven
+00055240: 744c 6973 7465 6e65 7228 2263 6c69 636b  tListener("click
+00055250: 222c 6e3d 3e7b 7468 6973 2e69 6e70 7574  ",n=>{this.input
+00055260: 456c 656d 656e 742e 666f 6375 7328 292c  Element.focus(),
+00055270: 7468 6973 2e69 6e70 7574 456c 656d 656e  this.inputElemen
+00055280: 742e 7365 7453 656c 6563 7469 6f6e 5261  t.setSelectionRa
+00055290: 6e67 6528 302c 3029 2c6e 2e73 746f 7050  nge(0,0),n.stopP
+000552a0: 726f 7061 6761 7469 6f6e 2829 7d29 2c74  ropagation()}),t
+000552b0: 6869 732e 7375 6666 6978 5465 7874 456c  his.suffixTextEl
+000552c0: 656d 656e 742e 6164 6445 7665 6e74 4c69  ement.addEventLi
+000552d0: 7374 656e 6572 2822 636c 6963 6b22 2c6e  stener("click",n
+000552e0: 3d3e 7b74 6869 732e 696e 7075 7445 6c65  =>{this.inputEle
+000552f0: 6d65 6e74 2e66 6f63 7573 2829 2c74 6869  ment.focus(),thi
+00055300: 732e 696e 7075 7445 6c65 6d65 6e74 2e73  s.inputElement.s
+00055310: 6574 5365 6c65 6374 696f 6e52 616e 6765  etSelectionRange
+00055320: 2874 6869 732e 696e 7075 7445 6c65 6d65  (this.inputEleme
+00055330: 6e74 2e76 616c 7565 2e6c 656e 6774 682c  nt.value.length,
+00055340: 7468 6973 2e69 6e70 7574 456c 656d 656e  this.inputElemen
+00055350: 742e 7661 6c75 652e 6c65 6e67 7468 292c  t.value.length),
+00055360: 6e2e 7374 6f70 5072 6f70 6167 6174 696f  n.stopPropagatio
+00055370: 6e28 297d 292c 7468 6973 2e69 6e70 7574  n()}),this.input
+00055380: 456c 656d 656e 742e 6164 6445 7665 6e74  Element.addEvent
+00055390: 4c69 7374 656e 6572 2822 6d6f 7573 6564  Listener("moused
+000553a0: 6f77 6e22 2c6e 3d3e 7b6e 2e73 746f 7050  own",n=>{n.stopP
+000553b0: 726f 7061 6761 7469 6f6e 2829 7d29 2c65  ropagation()}),e
+000553c0: 7d75 7064 6174 6545 6c65 6d65 6e74 2865  }updateElement(e
+000553d0: 2c6e 297b 652e 7465 7874 213d 3d76 6f69  ,n){e.text!==voi
+000553e0: 6420 3026 2628 7468 6973 2e69 6e70 7574  d 0&&(this.input
+000553f0: 456c 656d 656e 742e 7661 6c75 653d 652e  Element.value=e.
+00055400: 7465 7874 292c 652e 6c61 6265 6c21 3d3d  text),e.label!==
+00055410: 766f 6964 2030 2626 2874 6869 732e 6c61  void 0&&(this.la
+00055420: 6265 6c45 6c65 6d65 6e74 2e74 6578 7443  belElement.textC
+00055430: 6f6e 7465 6e74 3d65 2e6c 6162 656c 2c24  ontent=e.label,$
+00055440: 6e28 7468 6973 2c65 2e6c 6162 656c 2c30  n(this,e.label,0
+00055450: 2929 2c65 2e70 7265 6669 785f 7465 7874  )),e.prefix_text
+00055460: 3d3d 3d22 223f 2874 6869 732e 7072 6566  ===""?(this.pref
+00055470: 6978 5465 7874 456c 656d 656e 742e 7374  ixTextElement.st
+00055480: 796c 652e 6469 7370 6c61 793d 226e 6f6e  yle.display="non
+00055490: 6522 2c74 6869 732e 7072 6566 6978 5465  e",this.prefixTe
+000554a0: 7874 5769 6474 683d 302c 7468 6973 2e69  xtWidth=0,this.i
+000554b0: 6e70 7574 456c 656d 656e 742e 7374 796c  nputElement.styl
+000554c0: 652e 7061 6464 696e 674c 6566 743d 6024  e.paddingLeft=`$
+000554d0: 7b4f 6e7d 7265 6d60 2c74 6869 732e 6d61  {On}rem`,this.ma
+000554e0: 6b65 4c61 796f 7574 4469 7274 7928 2929  keLayoutDirty())
+000554f0: 3a65 2e70 7265 6669 785f 7465 7874 213d  :e.prefix_text!=
+00055500: 3d76 6f69 6420 3026 2628 7468 6973 2e70  =void 0&&(this.p
+00055510: 7265 6669 7854 6578 7445 6c65 6d65 6e74  refixTextElement
+00055520: 2e74 6578 7443 6f6e 7465 6e74 3d65 2e70  .textContent=e.p
+00055530: 7265 6669 785f 7465 7874 2c74 6869 732e  refix_text,this.
+00055540: 7072 6566 6978 5465 7874 456c 656d 656e  prefixTextElemen
+00055550: 742e 7374 796c 652e 7265 6d6f 7665 5072  t.style.removePr
+00055560: 6f70 6572 7479 2822 6469 7370 6c61 7922  operty("display"
+00055570: 292c 7468 6973 2e69 6e70 7574 456c 656d  ),this.inputElem
+00055580: 656e 742e 7374 796c 652e 7265 6d6f 7665  ent.style.remove
+00055590: 5072 6f70 6572 7479 2822 7061 6464 696e  Property("paddin
+000555a0: 672d 6c65 6674 2229 2c74 6869 732e 7072  g-left"),this.pr
+000555b0: 6566 6978 5465 7874 5769 6474 683d 6b65  efixTextWidth=ke
+000555c0: 2865 2e70 7265 6669 785f 7465 7874 2c22  (e.prefix_text,"
+000555d0: 7465 7874 2229 5b30 5d2b 2e32 2c74 6869  text")[0]+.2,thi
+000555e0: 732e 6d61 6b65 4c61 796f 7574 4469 7274  s.makeLayoutDirt
+000555f0: 7928 2929 2c65 2e73 7566 6669 785f 7465  y()),e.suffix_te
+00055600: 7874 3d3d 3d22 223f 2874 6869 732e 7375  xt===""?(this.su
+00055610: 6666 6978 5465 7874 456c 656d 656e 742e  ffixTextElement.
+00055620: 7374 796c 652e 6469 7370 6c61 793d 226e  style.display="n
+00055630: 6f6e 6522 2c74 6869 732e 7375 6666 6978  one",this.suffix
+00055640: 5465 7874 5769 6474 683d 302c 7468 6973  TextWidth=0,this
+00055650: 2e69 6e70 7574 456c 656d 656e 742e 7374  .inputElement.st
+00055660: 796c 652e 7061 6464 696e 6752 6967 6874  yle.paddingRight
+00055670: 3d60 247b 4f6e 7d72 656d 602c 7468 6973  =`${On}rem`,this
+00055680: 2e6d 616b 654c 6179 6f75 7444 6972 7479  .makeLayoutDirty
+00055690: 2829 293a 652e 7375 6666 6978 5f74 6578  ()):e.suffix_tex
+000556a0: 7421 3d3d 766f 6964 2030 2626 2874 6869  t!==void 0&&(thi
+000556b0: 732e 7375 6666 6978 5465 7874 456c 656d  s.suffixTextElem
+000556c0: 656e 742e 7465 7874 436f 6e74 656e 743d  ent.textContent=
+000556d0: 652e 7375 6666 6978 5f74 6578 742c 7468  e.suffix_text,th
+000556e0: 6973 2e73 7566 6669 7854 6578 7445 6c65  is.suffixTextEle
+000556f0: 6d65 6e74 2e73 7479 6c65 2e72 656d 6f76  ment.style.remov
+00055700: 6550 726f 7065 7274 7928 2264 6973 706c  eProperty("displ
+00055710: 6179 2229 2c74 6869 732e 696e 7075 7445  ay"),this.inputE
+00055720: 6c65 6d65 6e74 2e73 7479 6c65 2e72 656d  lement.style.rem
+00055730: 6f76 6550 726f 7065 7274 7928 2270 6164  oveProperty("pad
+00055740: 6469 6e67 2d72 6967 6874 2229 2c74 6869  ding-right"),thi
+00055750: 732e 7375 6666 6978 5465 7874 5769 6474  s.suffixTextWidt
+00055760: 683d 6b65 2865 2e73 7566 6669 785f 7465  h=ke(e.suffix_te
+00055770: 7874 2c22 7465 7874 2229 5b30 5d2b 2e32  xt,"text")[0]+.2
+00055780: 2c74 6869 732e 6d61 6b65 4c61 796f 7574  ,this.makeLayout
+00055790: 4469 7274 7928 2929 2c65 2e69 735f 7365  Dirty()),e.is_se
+000557a0: 6372 6574 213d 3d76 6f69 6420 3026 2628  cret!==void 0&&(
+000557b0: 7468 6973 2e69 6e70 7574 456c 656d 656e  this.inputElemen
+000557c0: 742e 7479 7065 3d65 2e69 735f 7365 6372  t.type=e.is_secr
+000557d0: 6574 3f22 7061 7373 776f 7264 223a 2274  et?"password":"t
+000557e0: 6578 7422 292c 652e 6973 5f73 656e 7369  ext"),e.is_sensi
+000557f0: 7469 7665 3d3d 3d21 303f 2874 6869 732e  tive===!0?(this.
+00055800: 696e 7075 7445 6c65 6d65 6e74 2e64 6973  inputElement.dis
+00055810: 6162 6c65 643d 2131 2c74 6869 732e 656c  abled=!1,this.el
+00055820: 656d 656e 742e 636c 6173 734c 6973 742e  ement.classList.
+00055830: 7265 6d6f 7665 2822 7269 6f2d 6469 7361  remove("rio-disa
+00055840: 626c 6564 2d69 6e70 7574 2229 293a 652e  bled-input")):e.
+00055850: 6973 5f73 656e 7369 7469 7665 3d3d 3d21  is_sensitive===!
+00055860: 3126 2628 7468 6973 2e69 6e70 7574 456c  1&&(this.inputEl
+00055870: 656d 656e 742e 6469 7361 626c 6564 3d21  ement.disabled=!
+00055880: 302c 7468 6973 2e65 6c65 6d65 6e74 2e63  0,this.element.c
+00055890: 6c61 7373 4c69 7374 2e61 6464 2822 7269  lassList.add("ri
+000558a0: 6f2d 6469 7361 626c 6564 2d69 6e70 7574  o-disabled-input
+000558b0: 2229 292c 652e 6973 5f76 616c 6964 3d3d  ")),e.is_valid==
+000558c0: 3d21 313f 7468 6973 2e65 6c65 6d65 6e74  =!1?this.element
+000558d0: 2e73 7479 6c65 2e73 6574 5072 6f70 6572  .style.setProper
+000558e0: 7479 2822 2d2d 7269 6f2d 6c6f 6361 6c2d  ty("--rio-local-
+000558f0: 7465 7874 2d63 6f6c 6f72 222c 2276 6172  text-color","var
+00055900: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6461  (--rio-global-da
+00055910: 6e67 6572 2d62 6729 2229 3a65 2e69 735f  nger-bg)"):e.is_
+00055920: 7661 6c69 643d 3d3d 2130 2626 7468 6973  valid===!0&&this
+00055930: 2e65 6c65 6d65 6e74 2e73 7479 6c65 2e72  .element.style.r
+00055940: 656d 6f76 6550 726f 7065 7274 7928 222d  emoveProperty("-
+00055950: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
+00055960: 636f 6c6f 7222 297d 6772 6162 4b65 7962  color")}grabKeyb
+00055970: 6f61 7264 466f 6375 7328 297b 7468 6973  oardFocus(){this
+00055980: 2e69 6e70 7574 456c 656d 656e 742e 666f  .inputElement.fo
+00055990: 6375 7328 297d 7570 6461 7465 4e61 7475  cus()}updateNatu
+000559a0: 7261 6c57 6964 7468 2865 297b 556e 2874  ralWidth(e){Un(t
+000559b0: 6869 732c 7468 6973 2e70 7265 6669 7854  his,this.prefixT
+000559c0: 6578 7457 6964 7468 2b74 6869 732e 7375  extWidth+this.su
+000559d0: 6666 6978 5465 7874 5769 6474 6829 7d75  ffixTextWidth)}u
+000559e0: 7064 6174 654e 6174 7572 616c 4865 6967  pdateNaturalHeig
+000559f0: 6874 2865 297b 7d7d 636c 6173 7320 4975  ht(e){}}class Iu
+00055a00: 2065 7874 656e 6473 2049 657b 6372 6561   extends Ie{crea
+00055a10: 7465 456c 656d 656e 7428 297b 7265 7475  teElement(){retu
+00055a20: 726e 2064 6f63 756d 656e 742e 6372 6561  rn document.crea
+00055a30: 7465 456c 656d 656e 7428 2264 6976 2229  teElement("div")
+00055a40: 7d75 7064 6174 6545 6c65 6d65 6e74 2865  }updateElement(e
+00055a50: 2c6e 297b 7468 6973 2e72 6570 6c61 6365  ,n){this.replace
+00055a60: 4f6e 6c79 4368 696c 6428 6e2c 652e 636f  OnlyChild(n,e.co
+00055a70: 6e74 656e 7429 2c65 2e63 6f6c 6f72 213d  ntent),e.color!=
+00055a80: 3d76 6f69 6420 3026 2624 6528 7468 6973  =void 0&&$e(this
+00055a90: 2e65 6c65 6d65 6e74 2c65 2e63 6f6c 6f72  .element,e.color
+00055aa0: 297d 7d63 6c61 7373 204c 7520 6578 7465  )}}class Lu exte
+00055ab0: 6e64 7320 557b 6372 6561 7465 456c 656d  nds U{createElem
+00055ac0: 656e 7428 297b 6c65 7420 653d 646f 6375  ent(){let e=docu
+00055ad0: 6d65 6e74 2e63 7265 6174 6545 6c65 6d65  ment.createEleme
+00055ae0: 6e74 2822 6469 7622 293b 7265 7475 726e  nt("div");return
+00055af0: 2065 2e63 6c61 7373 4c69 7374 2e61 6464   e.classList.add
+00055b00: 2822 7269 6f2d 746f 6f6c 7469 7022 292c  ("rio-tooltip"),
+00055b10: 652e 696e 6e65 7248 544d 4c3d 600a 2020  e.innerHTML=`.  
+00055b20: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00055b30: 6c61 7373 3d22 7269 6f2d 746f 6f6c 7469  lass="rio-toolti
+00055b40: 702d 616e 6368 6f72 223e 3c2f 6469 763e  p-anchor"></div>
+00055b50: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00055b60: 7620 636c 6173 733d 2272 696f 2d74 6f6f  v class="rio-too
+00055b70: 6c74 6970 2d6c 6162 656c 2072 696f 2d73  ltip-label rio-s
+00055b80: 7769 7463 6865 726f 6f2d 6875 6422 3e3c  witcheroo-hud"><
+00055b90: 2f64 6976 3e0a 2020 2020 2020 2020 602c  /div>.        `,
+00055ba0: 7468 6973 2e61 6e63 686f 7243 6f6e 7461  this.anchorConta
+00055bb0: 696e 6572 3d65 2e71 7565 7279 5365 6c65  iner=e.querySele
+00055bc0: 6374 6f72 2822 2e72 696f 2d74 6f6f 6c74  ctor(".rio-toolt
+00055bd0: 6970 2d61 6e63 686f 7222 292c 7468 6973  ip-anchor"),this
+00055be0: 2e6c 6162 656c 456c 656d 656e 743d 652e  .labelElement=e.
+00055bf0: 7175 6572 7953 656c 6563 746f 7228 222e  querySelector(".
+00055c00: 7269 6f2d 746f 6f6c 7469 702d 6c61 6265  rio-tooltip-labe
+00055c10: 6c22 292c 7468 6973 2e61 6e63 686f 7243  l"),this.anchorC
+00055c20: 6f6e 7461 696e 6572 2e61 6464 4576 656e  ontainer.addEven
+00055c30: 744c 6973 7465 6e65 7228 226d 6f75 7365  tListener("mouse
+00055c40: 6f76 6572 222c 2829 3d3e 7b74 6869 732e  over",()=>{this.
+00055c50: 6c61 6265 6c45 6c65 6d65 6e74 2e73 7479  labelElement.sty
+00055c60: 6c65 2e6f 7061 6369 7479 3d22 3122 7d29  le.opacity="1"})
+00055c70: 2c74 6869 732e 616e 6368 6f72 436f 6e74  ,this.anchorCont
+00055c80: 6169 6e65 722e 6164 6445 7665 6e74 4c69  ainer.addEventLi
+00055c90: 7374 656e 6572 2822 6d6f 7573 656f 7574  stener("mouseout
+00055ca0: 222c 2829 3d3e 7b74 6869 732e 6c61 6265  ",()=>{this.labe
+00055cb0: 6c45 6c65 6d65 6e74 2e73 7479 6c65 2e6f  lElement.style.o
+00055cc0: 7061 6369 7479 3d22 3022 7d29 2c65 7d75  pacity="0"}),e}u
+00055cd0: 7064 6174 6545 6c65 6d65 6e74 2865 2c6e  pdateElement(e,n
+00055ce0: 297b 6966 2865 2e61 6e63 686f 7221 3d3d  ){if(e.anchor!==
+00055cf0: 766f 6964 2030 2626 7468 6973 2e72 6570  void 0&&this.rep
+00055d00: 6c61 6365 4f6e 6c79 4368 696c 6428 6e2c  laceOnlyChild(n,
+00055d10: 652e 616e 6368 6f72 2c74 6869 732e 616e  e.anchor,this.an
+00055d20: 6368 6f72 436f 6e74 6169 6e65 7229 2c65  chorContainer),e
+00055d30: 2e5f 7469 705f 636f 6d70 6f6e 656e 7421  ._tip_component!
+00055d40: 3d3d 766f 6964 2030 2626 7468 6973 2e72  ==void 0&&this.r
+00055d50: 6570 6c61 6365 4f6e 6c79 4368 696c 6428  eplaceOnlyChild(
+00055d60: 6e2c 652e 5f74 6970 5f63 6f6d 706f 6e65  n,e._tip_compone
+00055d70: 6e74 2c74 6869 732e 6c61 6265 6c45 6c65  nt,this.labelEle
+00055d80: 6d65 6e74 292c 652e 706f 7369 7469 6f6e  ment),e.position
+00055d90: 213d 3d76 6f69 6420 3029 7b6c 6574 2069  !==void 0){let i
+00055da0: 2c72 2c73 2c61 2c6f 3b63 6f6e 7374 2063  ,r,s,a,o;const c
+00055db0: 3d22 6361 6c63 2831 3030 2520 2b20 302e  ="calc(100% + 0.
+00055dc0: 3572 656d 2922 3b65 2e70 6f73 6974 696f  5rem)";e.positio
+00055dd0: 6e3d 3d3d 226c 6566 7422 3f28 693d 2275  n==="left"?(i="u
+00055de0: 6e73 6574 222c 723d 2235 3025 222c 733d  nset",r="50%",s=
+00055df0: 632c 613d 2275 6e73 6574 222c 6f3d 2274  c,a="unset",o="t
+00055e00: 7261 6e73 6c61 7465 5928 2d35 3025 2922  ranslateY(-50%)"
+00055e10: 293a 652e 706f 7369 7469 6f6e 3d3d 3d22  ):e.position==="
+00055e20: 746f 7022 3f28 693d 2235 3025 222c 723d  top"?(i="50%",r=
+00055e30: 2275 6e73 6574 222c 733d 2275 6e73 6574  "unset",s="unset
+00055e40: 222c 613d 632c 6f3d 2274 7261 6e73 6c61  ",a=c,o="transla
+00055e50: 7465 5828 2d35 3025 2922 293a 652e 706f  teX(-50%)"):e.po
+00055e60: 7369 7469 6f6e 3d3d 3d22 7269 6768 7422  sition==="right"
+00055e70: 3f28 693d 632c 723d 2235 3025 222c 733d  ?(i=c,r="50%",s=
+00055e80: 2275 6e73 6574 222c 613d 2275 6e73 6574  "unset",a="unset
+00055e90: 222c 6f3d 2274 7261 6e73 6c61 7465 5928  ",o="translateY(
+00055ea0: 2d35 3025 2922 293a 2869 3d22 3530 2522  -50%)"):(i="50%"
+00055eb0: 2c72 3d63 2c73 3d22 756e 7365 7422 2c61  ,r=c,s="unset",a
+00055ec0: 3d22 756e 7365 7422 2c6f 3d22 7472 616e  ="unset",o="tran
+00055ed0: 736c 6174 6558 282d 3530 2529 2229 2c74  slateX(-50%)"),t
+00055ee0: 6869 732e 6c61 6265 6c45 6c65 6d65 6e74  his.labelElement
+00055ef0: 2e73 7479 6c65 2e6c 6566 743d 692c 7468  .style.left=i,th
+00055f00: 6973 2e6c 6162 656c 456c 656d 656e 742e  is.labelElement.
+00055f10: 7374 796c 652e 746f 703d 722c 7468 6973  style.top=r,this
+00055f20: 2e6c 6162 656c 456c 656d 656e 742e 7374  .labelElement.st
+00055f30: 796c 652e 7269 6768 743d 732c 7468 6973  yle.right=s,this
+00055f40: 2e6c 6162 656c 456c 656d 656e 742e 7374  .labelElement.st
+00055f50: 796c 652e 626f 7474 6f6d 3d61 2c74 6869  yle.bottom=a,thi
+00055f60: 732e 6c61 6265 6c45 6c65 6d65 6e74 2e73  s.labelElement.s
+00055f70: 7479 6c65 2e74 7261 6e73 666f 726d 3d6f  tyle.transform=o
+00055f80: 7d7d 7570 6461 7465 4e61 7475 7261 6c57  }}updateNaturalW
+00055f90: 6964 7468 2865 297b 7468 6973 2e6e 6174  idth(e){this.nat
+00055fa0: 7572 616c 5769 6474 683d 435b 7468 6973  uralWidth=C[this
+00055fb0: 2e73 7461 7465 2e61 6e63 686f 725d 2e72  .state.anchor].r
+00055fc0: 6571 7565 7374 6564 5769 6474 687d 7570  equestedWidth}up
+00055fd0: 6461 7465 416c 6c6f 6361 7465 6457 6964  dateAllocatedWid
+00055fe0: 7468 2865 297b 6c65 7420 6e3d 435b 7468  th(e){let n=C[th
+00055ff0: 6973 2e73 7461 7465 2e61 6e63 686f 725d  is.state.anchor]
+00056000: 2c69 3d43 5b74 6869 732e 7374 6174 652e  ,i=C[this.state.
+00056010: 5f74 6970 5f63 6f6d 706f 6e65 6e74 5d3b  _tip_component];
+00056020: 6e2e 616c 6c6f 6361 7465 6457 6964 7468  n.allocatedWidth
+00056030: 3d74 6869 732e 616c 6c6f 6361 7465 6457  =this.allocatedW
+00056040: 6964 7468 2c69 2e61 6c6c 6f63 6174 6564  idth,i.allocated
+00056050: 5769 6474 683d 692e 6e61 7475 7261 6c57  Width=i.naturalW
+00056060: 6964 7468 7d75 7064 6174 654e 6174 7572  idth}updateNatur
+00056070: 616c 4865 6967 6874 2865 297b 7468 6973  alHeight(e){this
+00056080: 2e6e 6174 7572 616c 4865 6967 6874 3d43  .naturalHeight=C
+00056090: 5b74 6869 732e 7374 6174 652e 616e 6368  [this.state.anch
+000560a0: 6f72 5d2e 7265 7175 6573 7465 6448 6569  or].requestedHei
+000560b0: 6768 747d 7570 6461 7465 416c 6c6f 6361  ght}updateAlloca
+000560c0: 7465 6448 6569 6768 7428 6529 7b6c 6574  tedHeight(e){let
+000560d0: 206e 3d43 5b74 6869 732e 7374 6174 652e   n=C[this.state.
+000560e0: 616e 6368 6f72 5d2c 693d 435b 7468 6973  anchor],i=C[this
+000560f0: 2e73 7461 7465 2e5f 7469 705f 636f 6d70  .state._tip_comp
+00056100: 6f6e 656e 745d 3b6e 2e61 6c6c 6f63 6174  onent];n.allocat
+00056110: 6564 4865 6967 6874 3d74 6869 732e 616c  edHeight=this.al
+00056120: 6c6f 6361 7465 6448 6569 6768 742c 692e  locatedHeight,i.
+00056130: 616c 6c6f 6361 7465 6448 6569 6768 743d  allocatedHeight=
+00056140: 692e 6e61 7475 7261 6c48 6569 6768 742c  i.naturalHeight,
+00056150: 6e2e 656c 656d 656e 742e 7374 796c 652e  n.element.style.
+00056160: 6c65 6674 3d22 3022 2c6e 2e65 6c65 6d65  left="0",n.eleme
+00056170: 6e74 2e73 7479 6c65 2e74 6f70 3d22 3022  nt.style.top="0"
+00056180: 2c69 2e65 6c65 6d65 6e74 2e73 7479 6c65  ,i.element.style
+00056190: 2e6c 6566 743d 2230 222c 692e 656c 656d  .left="0",i.elem
+000561a0: 656e 742e 7374 796c 652e 746f 703d 2230  ent.style.top="0
+000561b0: 227d 7d63 6f6e 7374 206f 733d 7b22 416c  "}}const os={"Al
+000561c0: 6967 6e2d 6275 696c 7469 6e22 3a4f 732c  ign-builtin":Os,
+000561d0: 2242 7569 6c64 4661 696c 6564 2d62 7569  "BuildFailed-bui
+000561e0: 6c74 696e 223a 4873 2c22 4275 7474 6f6e  ltin":Hs,"Button
+000561f0: 2d62 7569 6c74 696e 223a 4673 2c22 4361  -builtin":Fs,"Ca
+00056200: 7264 2d62 7569 6c74 696e 223a 5773 2c22  rd-builtin":Ws,"
+00056210: 436c 6173 7343 6f6e 7461 696e 6572 2d62  ClassContainer-b
+00056220: 7569 6c74 696e 223a 5573 2c22 436f 6465  uiltin":Us,"Code
+00056230: 426c 6f63 6b2d 6275 696c 7469 6e22 3a79  Block-builtin":y
+00056240: 6f2c 2243 6f64 6545 7870 6c6f 7265 722d  o,"CodeExplorer-
+00056250: 6275 696c 7469 6e22 3a76 6f2c 2243 6f6c  builtin":vo,"Col
+00056260: 6f72 5069 636b 6572 2d62 7569 6c74 696e  orPicker-builtin
+00056270: 223a 786f 2c22 436f 6c75 6d6e 2d62 7569  ":xo,"Column-bui
+00056280: 6c74 696e 223a 4772 2c22 436f 6d70 6f6e  ltin":Gr,"Compon
+00056290: 656e 7454 7265 652d 6275 696c 7469 6e22  entTree-builtin"
+000562a0: 3a6b 6f2c 2243 7573 746f 6d4c 6973 7449  :ko,"CustomListI
+000562b0: 7465 6d2d 6275 696c 7469 6e22 3a56 722c  tem-builtin":Vr,
+000562c0: 2244 6562 7567 6765 7243 6f6e 6e65 6374  "DebuggerConnect
+000562d0: 6f72 2d62 7569 6c74 696e 223a 4e6f 2c22  or-builtin":No,"
+000562e0: 4472 6177 6572 2d62 7569 6c74 696e 223a  Drawer-builtin":
+000562f0: 546f 2c22 4472 6f70 646f 776e 2d62 7569  To,"Dropdown-bui
+00056300: 6c74 696e 223a 416f 2c22 466c 6f77 436f  ltin":Ao,"FlowCo
+00056310: 6e74 6169 6e65 722d 6275 696c 7469 6e22  ntainer-builtin"
+00056320: 3a4f 6f2c 2246 756e 6461 6d65 6e74 616c  :Oo,"Fundamental
+00056330: 526f 6f74 436f 6d70 6f6e 656e 742d 6275  RootComponent-bu
+00056340: 696c 7469 6e22 3a52 6f2c 2247 7269 642d  iltin":Ro,"Grid-
+00056350: 6275 696c 7469 6e22 3a4d 6f2c 2248 6561  builtin":Mo,"Hea
+00056360: 6469 6e67 4c69 7374 4974 656d 2d62 7569  dingListItem-bui
+00056370: 6c74 696e 223a 5972 2c22 4874 6d6c 2d62  ltin":Yr,"Html-b
+00056380: 7569 6c74 696e 223a 496f 2c22 4963 6f6e  uiltin":Io,"Icon
+00056390: 2d62 7569 6c74 696e 223a 446f 2c22 496d  -builtin":Do,"Im
+000563a0: 6167 652d 6275 696c 7469 6e22 3a42 6f2c  age-builtin":Bo,
+000563b0: 224b 6579 4576 656e 744c 6973 7465 6e65  "KeyEventListene
+000563c0: 722d 6275 696c 7469 6e22 3a57 6f2c 224c  r-builtin":Wo,"L
+000563d0: 696e 6b2d 6275 696c 7469 6e22 3a55 6f2c  ink-builtin":Uo,
+000563e0: 224c 6973 7456 6965 772d 6275 696c 7469  "ListView-builti
+000563f0: 6e22 3a24 6f2c 224d 6172 6769 6e2d 6275  n":$o,"Margin-bu
+00056400: 696c 7469 6e22 3a7a 6f2c 224d 6172 6b64  iltin":zo,"Markd
+00056410: 6f77 6e2d 6275 696c 7469 6e22 3a51 632c  own-builtin":Qc,
+00056420: 224d 6564 6961 506c 6179 6572 2d62 7569  "MediaPlayer-bui
+00056430: 6c74 696e 223a 6a63 2c22 4d6f 7573 6545  ltin":jc,"MouseE
+00056440: 7665 6e74 4c69 7374 656e 6572 2d62 7569  ventListener-bui
+00056450: 6c74 696e 223a 7475 2c22 4d75 6c74 694c  ltin":tu,"MultiL
+00056460: 696e 6554 6578 7449 6e70 7574 2d62 7569  ineTextInput-bui
+00056470: 6c74 696e 223a 6e75 2c22 4e6f 6465 496e  ltin":nu,"NodeIn
+00056480: 7075 742d 6275 696c 7469 6e22 3a69 752c  put-builtin":iu,
+00056490: 224e 6f64 654f 7574 7075 742d 6275 696c  "NodeOutput-buil
+000564a0: 7469 6e22 3a72 752c 224f 7665 726c 6179  tin":ru,"Overlay
+000564b0: 2d62 7569 6c74 696e 223a 7375 2c22 506c  -builtin":su,"Pl
+000564c0: 6f74 2d62 7569 6c74 696e 223a 6c75 2c22  ot-builtin":lu,"
+000564d0: 506f 7075 702d 6275 696c 7469 6e22 3a63  Popup-builtin":c
+000564e0: 752c 2250 726f 6772 6573 7342 6172 2d62  u,"ProgressBar-b
+000564f0: 7569 6c74 696e 223a 7575 2c22 5072 6f67  uiltin":uu,"Prog
+00056500: 7265 7373 4369 7263 6c65 2d62 7569 6c74  ressCircle-built
+00056510: 696e 223a 6475 2c22 5265 6374 616e 676c  in":du,"Rectangl
+00056520: 652d 6275 696c 7469 6e22 3a70 752c 2252  e-builtin":pu,"R
+00056530: 6576 6561 6c65 722d 6275 696c 7469 6e22  evealer-builtin"
+00056540: 3a67 752c 2252 6f77 2d62 7569 6c74 696e  :gu,"Row-builtin
+00056550: 223a 436f 2c22 5363 726f 6c6c 436f 6e74  ":Co,"ScrollCont
+00056560: 6169 6e65 722d 6275 696c 7469 6e22 3a66  ainer-builtin":f
+00056570: 752c 2253 6372 6f6c 6c54 6172 6765 742d  u,"ScrollTarget-
+00056580: 6275 696c 7469 6e22 3a62 752c 2253 6570  builtin":bu,"Sep
+00056590: 6172 6174 6f72 2d62 7569 6c74 696e 223a  arator-builtin":
+000565a0: 4575 2c22 5365 7061 7261 746f 724c 6973  Eu,"SeparatorLis
+000565b0: 7449 7465 6d2d 6275 696c 7469 6e22 3a5a  tItem-builtin":Z
+000565c0: 722c 2253 6c69 6465 722d 6275 696c 7469  r,"Slider-builti
+000565d0: 6e22 3a5f 752c 2253 6c69 6465 7368 6f77  n":_u,"Slideshow
+000565e0: 2d62 7569 6c74 696e 223a 7675 2c22 5374  -builtin":vu,"St
+000565f0: 6163 6b2d 6275 696c 7469 6e22 3a77 752c  ack-builtin":wu,
+00056600: 2253 7769 7463 682d 6275 696c 7469 6e22  "Switch-builtin"
+00056610: 3a78 752c 2253 7769 7463 6865 722d 6275  :xu,"Switcher-bu
+00056620: 696c 7469 6e22 3a54 752c 2253 7769 7463  iltin":Tu,"Switc
+00056630: 6865 7242 6172 2d62 7569 6c74 696e 223a  herBar-builtin":
+00056640: 6b75 2c22 5461 626c 652d 6275 696c 7469  ku,"Table-builti
+00056650: 6e22 3a4f 752c 2254 6578 742d 6275 696c  n":Ou,"Text-buil
+00056660: 7469 6e22 3a52 752c 2254 6578 7449 6e70  tin":Ru,"TextInp
+00056670: 7574 2d62 7569 6c74 696e 223a 4d75 2c22  ut-builtin":Mu,"
+00056680: 5468 656d 6543 6f6e 7465 7874 5377 6974  ThemeContextSwit
+00056690: 6368 6572 2d62 7569 6c74 696e 223a 4975  cher-builtin":Iu
+000566a0: 2c22 546f 6f6c 7469 702d 6275 696c 7469  ,"Tooltip-builti
+000566b0: 6e22 3a4c 752c 506c 6163 6568 6f6c 6465  n":Lu,Placeholde
+000566c0: 723a 6175 7d3b 676c 6f62 616c 5468 6973  r:au};globalThis
+000566d0: 2e43 4f4d 504f 4e45 4e54 5f43 4c41 5353  .COMPONENT_CLASS
+000566e0: 4553 3d6f 733b 636f 6e73 7420 433d 7b7d  ES=os;const C={}
+000566f0: 2c56 653d 6e65 7720 4d61 703b 6675 6e63  ,Ve=new Map;func
+00056700: 7469 6f6e 2064 7428 297b 6c65 7420 743d  tion dt(){let t=
+00056710: 646f 6375 6d65 6e74 2e62 6f64 792e 7175  document.body.qu
+00056720: 6572 7953 656c 6563 746f 7228 222e 7269  erySelector(".ri
+00056730: 6f2d 6675 6e64 616d 656e 7461 6c2d 726f  o-fundamental-ro
+00056740: 6f74 2d63 6f6d 706f 6e65 6e74 2229 3b72  ot-component");r
+00056750: 6574 7572 6e20 636f 6e73 6f6c 652e 6173  eturn console.as
+00056760: 7365 7274 2874 213d 3d6e 756c 6c2c 2243  sert(t!==null,"C
+00056770: 6f75 6c64 6e27 7420 6669 6e64 2074 6865  ouldn't find the
+00056780: 2072 6f6f 7420 636f 6d70 6f6e 656e 7420   root component 
+00056790: 696e 2074 6865 2064 6f63 756d 656e 7420  in the document 
+000567a0: 626f 6479 2229 2c56 652e 6765 7428 7429  body"),Ve.get(t)
+000567b0: 7d66 756e 6374 696f 6e20 6c73 2829 7b6c  }function ls(){l
+000567c0: 6574 2074 3d64 7428 293b 7265 7475 726e  et t=dt();return
+000567d0: 2043 5b74 2e73 7461 7465 2e63 6f6e 7465   C[t.state.conte
+000567e0: 6e74 5d7d 676c 6f62 616c 5468 6973 2e67  nt]}globalThis.g
+000567f0: 6574 526f 6f74 5363 726f 6c6c 6572 3d6c  etRootScroller=l
+00056800: 733b 6675 6e63 7469 6f6e 204b 6528 7429  s;function Ke(t)
+00056810: 7b6c 6574 2065 3d43 7428 7429 3b69 6628  {let e=Ct(t);if(
+00056820: 653d 3d3d 6e75 6c6c 297b 6c65 7420 6e3d  e===null){let n=
+00056830: 742e 7061 7265 6e74 456c 656d 656e 743b  t.parentElement;
+00056840: 666f 7228 3b6e 3b29 7b69 6628 653d 4374  for(;n;){if(e=Ct
+00056850: 286e 292c 6521 3d3d 6e75 6c6c 2974 6872  (n),e!==null)thr
+00056860: 6f77 6045 6c65 6d65 6e74 2024 7b51 6e28  ow`Element ${Qn(
+00056870: 7429 7d20 646f 6573 206e 6f74 2063 6f72  t)} does not cor
+00056880: 7265 7370 6f6e 6420 746f 2061 2063 6f6d  respond to a com
+00056890: 706f 6e65 6e74 2e20 4974 2069 7320 6120  ponent. It is a 
+000568a0: 6368 696c 6420 656c 656d 656e 7420 6f66  child element of
+000568b0: 2024 7b65 2e74 6f53 7472 696e 6728 297d   ${e.toString()}
+000568c0: 603b 6e3d 6e2e 7061 7265 6e74 456c 656d  `;n=n.parentElem
+000568d0: 656e 747d 7468 726f 7760 456c 656d 656e  ent}throw`Elemen
+000568e0: 7420 247b 516e 2874 297d 2064 6f65 7320  t ${Qn(t)} does 
+000568f0: 6e6f 7420 636f 7272 6573 706f 6e64 2074  not correspond t
+00056900: 6f20 6120 636f 6d70 6f6e 656e 7420 2861  o a component (a
+00056910: 6e64 206e 6f6e 6520 6f66 2069 7473 2070  nd none of its p
+00056920: 6172 656e 7420 656c 656d 656e 7473 2063  arent elements c
+00056930: 6f72 7265 7370 6f6e 6420 746f 2061 2063  orrespond to a c
+00056940: 6f6d 706f 6e65 6e74 2c20 6569 7468 6572  omponent, either
+00056950: 2960 7d72 6574 7572 6e20 657d 676c 6f62  )`}return e}glob
+00056960: 616c 5468 6973 2e63 6f6d 706f 6e65 6e74  alThis.component
+00056970: 7342 7949 643d 433b 676c 6f62 616c 5468  sById=C;globalTh
+00056980: 6973 2e67 6574 496e 7374 616e 6365 4279  is.getInstanceBy
+00056990: 456c 656d 656e 743d 4b65 3b66 756e 6374  Element=Ke;funct
+000569a0: 696f 6e20 4374 2874 297b 7265 7475 726e  ion Ct(t){return
+000569b0: 2056 652e 6765 7428 7429 3f3f 6e75 6c6c   Ve.get(t)??null
+000569c0: 7d66 756e 6374 696f 6e20 4475 2874 297b  }function Du(t){
+000569d0: 7265 7475 726e 2056 652e 6861 7328 7429  return Ve.has(t)
+000569e0: 7d66 756e 6374 696f 6e20 5075 2874 2c65  }function Pu(t,e
+000569f0: 297b 6c65 7420 6e3d 435b 745d 3b72 6574  ){let n=C[t];ret
+00056a00: 7572 6e20 6e3d 3d3d 766f 6964 2030 3f65  urn n===void 0?e
+00056a10: 3a7b 2e2e 2e6e 2e73 7461 7465 2c2e 2e2e  :{...n.state,...
+00056a20: 657d 7d66 756e 6374 696f 6e20 6672 2874  e}}function fr(t
+00056a30: 2c65 297b 6c65 7420 6e3d 655b 745d 7c7c  ,e){let n=e[t]||
+00056a40: 7b7d 2c69 3d50 7528 742c 6e29 2c72 3d74  {},i=Pu(t,n),r=t
+00056a50: 2c73 3d69 2e5f 6d61 7267 696e 5f3b 6966  ,s=i._margin_;if
+00056a60: 2873 3d3d 3d76 6f69 6420 3026 2663 6f6e  (s===void 0&&con
+00056a70: 736f 6c65 2e65 7272 6f72 2860 476f 7420  sole.error(`Got 
+00056a80: 696e 636f 6d70 6c65 7465 2073 7461 7465  incomplete state
+00056a90: 2066 6f72 2063 6f6d 706f 6e65 6e74 2024   for component $
+00056aa0: 7b74 7d60 292c 735b 305d 213d 3d30 7c7c  {t}`),s[0]!==0||
+00056ab0: 735b 315d 213d 3d30 7c7c 735b 325d 213d  s[1]!==0||s[2]!=
+00056ac0: 3d30 7c7c 735b 335d 213d 3d30 297b 6c65  =0||s[3]!==0){le
+00056ad0: 7420 6f3d 742a 2d31 303b 655b 6f5d 3d7b  t o=t*-10;e[o]={
+00056ae0: 5f74 7970 655f 3a22 4d61 7267 696e 2d62  _type_:"Margin-b
+00056af0: 7569 6c74 696e 222c 5f70 7974 686f 6e5f  uiltin",_python_
+00056b00: 7479 7065 5f3a 224d 6172 6769 6e20 2869  type_:"Margin (i
+00056b10: 6e6a 6563 7465 6429 222c 5f6b 6579 5f3a  njected)",_key_:
+00056b20: 6e75 6c6c 2c5f 6d61 7267 696e 5f3a 5b30  null,_margin_:[0
+00056b30: 2c30 2c30 2c30 5d2c 5f73 697a 655f 3a5b  ,0,0,0],_size_:[
+00056b40: 302c 305d 2c5f 6772 6f77 5f3a 692e 5f67  0,0],_grow_:i._g
+00056b50: 726f 775f 2c5f 7269 6f5f 696e 7465 726e  row_,_rio_intern
+00056b60: 616c 5f3a 2130 2c63 6f6e 7465 6e74 3a72  al_:!0,content:r
+00056b70: 2c6d 6172 6769 6e5f 6c65 6674 3a73 5b30  ,margin_left:s[0
+00056b80: 5d2c 6d61 7267 696e 5f74 6f70 3a73 5b31  ],margin_top:s[1
+00056b90: 5d2c 6d61 7267 696e 5f72 6967 6874 3a73  ],margin_right:s
+00056ba0: 5b32 5d2c 6d61 7267 696e 5f62 6f74 746f  [2],margin_botto
+00056bb0: 6d3a 735b 335d 7d2c 723d 6f7d 6c65 7420  m:s[3]},r=o}let 
+00056bc0: 613d 692e 5f61 6c69 676e 5f3b 6966 2861  a=i._align_;if(a
+00056bd0: 3d3d 3d76 6f69 6420 3026 2663 6f6e 736f  ===void 0&&conso
+00056be0: 6c65 2e65 7272 6f72 2860 476f 7420 696e  le.error(`Got in
+00056bf0: 636f 6d70 6c65 7465 2073 7461 7465 2066  complete state f
+00056c00: 6f72 2063 6f6d 706f 6e65 6e74 2024 7b74  or component ${t
+00056c10: 7d60 292c 615b 305d 213d 3d6e 756c 6c7c  }`),a[0]!==null|
+00056c20: 7c61 5b31 5d21 3d3d 6e75 6c6c 297b 6c65  |a[1]!==null){le
+00056c30: 7420 6f3d 742a 2d31 302d 313b 655b 6f5d  t o=t*-10-1;e[o]
+00056c40: 3d7b 5f74 7970 655f 3a22 416c 6967 6e2d  ={_type_:"Align-
+00056c50: 6275 696c 7469 6e22 2c5f 7079 7468 6f6e  builtin",_python
+00056c60: 5f74 7970 655f 3a22 416c 6967 6e20 2869  _type_:"Align (i
+00056c70: 6e6a 6563 7465 6429 222c 5f6b 6579 5f3a  njected)",_key_:
+00056c80: 6e75 6c6c 2c5f 6d61 7267 696e 5f3a 5b30  null,_margin_:[0
+00056c90: 2c30 2c30 2c30 5d2c 5f73 697a 655f 3a5b  ,0,0,0],_size_:[
+00056ca0: 302c 305d 2c5f 6772 6f77 5f3a 692e 5f67  0,0],_grow_:i._g
+00056cb0: 726f 775f 2c5f 7269 6f5f 696e 7465 726e  row_,_rio_intern
+00056cc0: 616c 5f3a 2130 2c63 6f6e 7465 6e74 3a72  al_:!0,content:r
+00056cd0: 2c61 6c69 676e 5f78 3a61 5b30 5d2c 616c  ,align_x:a[0],al
+00056ce0: 6967 6e5f 793a 615b 315d 7d2c 723d 6f7d  ign_y:a[1]},r=o}
+00056cf0: 7265 7475 726e 2072 7d66 756e 6374 696f  return r}functio
+00056d00: 6e20 6272 2874 2c65 2c6e 297b 6c65 7420  n br(t,e,n){let 
+00056d10: 693d 676c 6f62 616c 5468 6973 2e43 4849  i=globalThis.CHI
+00056d20: 4c44 5f41 5454 5249 4255 5445 5f4e 414d  LD_ATTRIBUTE_NAM
+00056d30: 4553 5b74 2e5f 7479 7065 5f5d 7c7c 5b5d  ES[t._type_]||[]
+00056d40: 3b66 756e 6374 696f 6e20 7228 7329 7b72  ;function r(s){r
+00056d50: 6574 7572 6e20 733e 3d30 3f73 3a4d 6174  eturn s>=0?s:Mat
+00056d60: 682e 666c 6f6f 7228 732f 2d31 3029 7d66  h.floor(s/-10)}f
+00056d70: 6f72 286c 6574 2073 206f 6620 6929 7b6c  or(let s of i){l
+00056d80: 6574 2061 3d74 5b73 5d3b 6966 2841 7272  et a=t[s];if(Arr
+00056d90: 6179 2e69 7341 7272 6179 2861 2929 745b  ay.isArray(a))t[
+00056da0: 735d 3d61 2e6d 6170 286f 3d3e 286f 3d72  s]=a.map(o=>(o=r
+00056db0: 286f 292c 652e 6164 6428 6f29 2c66 7228  (o),e.add(o),fr(
+00056dc0: 6f2c 6e29 2929 3b65 6c73 6520 6966 2861  o,n)));else if(a
+00056dd0: 213d 6e75 6c6c 297b 6c65 7420 6f3d 7228  !=null){let o=r(
+00056de0: 6129 3b74 5b73 5d3d 6672 286f 2c6e 292c  a);t[s]=fr(o,n),
+00056df0: 652e 6164 6428 6f29 7d7d 7d66 756e 6374  e.add(o)}}}funct
+00056e00: 696f 6e20 4275 2874 297b 6c65 7420 653d  ion Bu(t){let e=
+00056e10: 4f62 6a65 6374 2e6b 6579 7328 7429 2e6d  Object.keys(t).m
+00056e20: 6170 2869 3d3e 7061 7273 6549 6e74 2869  ap(i=>parseInt(i
+00056e30: 2929 2c6e 3d6e 6577 2053 6574 3b66 6f72  )),n=new Set;for
+00056e40: 286c 6574 2069 206f 6620 6529 6272 2874  (let i of e)br(t
+00056e50: 5b69 5d2c 6e2c 7429 3b66 6f72 286c 6574  [i],n,t);for(let
+00056e60: 2069 206f 6620 6529 7b69 6628 6e2e 6861   i of e){if(n.ha
+00056e70: 7328 6929 2963 6f6e 7469 6e75 653b 6c65  s(i))continue;le
+00056e80: 7420 723d 435b 695d 3b69 6628 723d 3d3d  t r=C[i];if(r===
+00056e90: 766f 6964 2030 2963 6f6e 7469 6e75 653b  void 0)continue;
+00056ea0: 6c65 7420 733d 722e 6765 7450 6172 656e  let s=r.getParen
+00056eb0: 7445 7863 6c75 6469 6e67 496e 6a65 6374  tExcludingInject
+00056ec0: 6564 2829 3b69 6628 733d 3d3d 6e75 6c6c  ed();if(s===null
+00056ed0: 2963 6f6e 7469 6e75 653b 6c65 7420 613d  )continue;let a=
+00056ee0: 7b2e 2e2e 732e 7374 6174 657d 3b62 7228  {...s.state};br(
+00056ef0: 612c 6e2c 7429 2c74 5b73 2e69 645d 3d61  a,n,t),t[s.id]=a
+00056f00: 7d7d 6675 6e63 7469 6f6e 2048 7528 742c  }}function Hu(t,
+00056f10: 6529 7b42 7528 7429 3b6c 6574 206e 3d64  e){Bu(t);let n=d
+00056f20: 6f63 756d 656e 742e 6163 7469 7665 456c  ocument.activeEl
+00056f30: 656d 656e 743b 666f 7228 3b6e 213d 3d6e  ement;for(;n!==n
+00056f40: 756c 6c26 2621 4475 286e 293b 296e 3d6e  ull&&!Du(n);)n=n
+00056f50: 2e70 6172 656e 7445 6c65 6d65 6e74 3b6c  .parentElement;l
+00056f60: 6574 2069 3d6e 3d3d 3d6e 756c 6c3f 6e75  et i=n===null?nu
+00056f70: 6c6c 3a4b 6528 6e29 2c72 3d6e 6577 2053  ll:Ke(n),r=new S
+00056f80: 6574 3b66 6f72 286c 6574 2073 2069 6e20  et;for(let s in 
+00056f90: 7429 7b6c 6574 2061 3d74 5b73 5d3b 6966  t){let a=t[s];if
+00056fa0: 2843 5b73 5d29 636f 6e74 696e 7565 3b63  (C[s])continue;c
+00056fb0: 6f6e 7374 2063 3d6f 735b 612e 5f74 7970  onst c=os[a._typ
+00056fc0: 655f 5d3b 6966 2821 6329 7468 726f 7760  e_];if(!c)throw`
+00056fd0: 456e 636f 756e 7465 7265 6420 756e 6b6e  Encountered unkn
+00056fe0: 6f77 6e20 636f 6d70 6f6e 656e 7420 7479  own component ty
+00056ff0: 7065 3a20 247b 612e 5f74 7970 655f 7d60  pe: ${a._type_}`
+00057000: 3b6c 6574 206c 3d6e 6577 2063 2870 6172  ;let l=new c(par
+00057010: 7365 496e 7428 7329 2c61 293b 435b 735d  seInt(s),a);C[s]
+00057020: 3d6c 2c56 652e 7365 7428 6c2e 656c 656d  =l,Ve.set(l.elem
+00057030: 656e 742c 6c29 2c6c 2e65 6c65 6d65 6e74  ent,l),l.element
+00057040: 2e73 6574 4174 7472 6962 7574 6528 2264  .setAttribute("d
+00057050: 6267 2d70 792d 636c 6173 7322 2c61 2e5f  bg-py-class",a._
+00057060: 7079 7468 6f6e 5f74 7970 655f 292c 6c2e  python_type_),l.
+00057070: 656c 656d 656e 742e 7365 7441 7474 7269  element.setAttri
+00057080: 6275 7465 2822 6462 672d 6964 222c 7329  bute("dbg-id",s)
+00057090: 3b6c 6574 2075 3d61 2e6b 6579 3b75 213d  ;let u=a.key;u!=
+000570a0: 3d76 6f69 6420 3026 266c 2e65 6c65 6d65  =void 0&&l.eleme
+000570b0: 6e74 2e73 6574 4174 7472 6962 7574 6528  nt.setAttribute(
+000570c0: 2264 6267 2d6b 6579 222c 6024 7b75 7d60  "dbg-key",`${u}`
+000570d0: 297d 666f 7228 6c65 7420 7320 696e 2074  )}for(let s in t
+000570e0: 297b 6c65 7420 613d 745b 735d 2c6f 3d43  ){let a=t[s],o=C
+000570f0: 5b73 5d3b 6f2e 7570 6461 7465 456c 656d  [s];o.updateElem
+00057100: 656e 7428 612c 7229 3b6c 6574 2063 3d4d  ent(a,r);let c=M
+00057110: 6174 682e 6162 7328 612e 5f73 697a 655f  ath.abs(a._size_
+00057120: 5b30 5d2d 6f2e 7374 6174 652e 5f73 697a  [0]-o.state._siz
+00057130: 655f 5b30 5d29 3e31 652d 362c 6c3d 4d61  e_[0])>1e-6,l=Ma
+00057140: 7468 2e61 6273 2861 2e5f 7369 7a65 5f5b  th.abs(a._size_[
+00057150: 315d 2d6f 2e73 7461 7465 2e5f 7369 7a65  1]-o.state._size
+00057160: 5f5b 315d 293e 3165 2d36 3b28 637c 7c6c  _[1])>1e-6;(c||l
+00057170: 2926 2628 636f 6e73 6f6c 652e 6c6f 6728  )&&(console.log(
+00057180: 6054 7269 6767 6572 696e 6720 7265 2d6c  `Triggering re-l
+00057190: 6179 6f75 7420 6265 6361 7573 6520 636f  ayout because co
+000571a0: 6d70 6f6e 656e 7420 2324 7b73 7d20 6368  mponent #${s} ch
+000571b0: 616e 6765 6420 7369 7a65 3a20 247b 6f2e  anged size: ${o.
+000571c0: 7374 6174 652e 5f73 697a 655f 7d20 2d3e  state._size_} ->
+000571d0: 2024 7b61 2e5f 7369 7a65 5f7d 6029 2c6f   ${a._size_}`),o
+000571e0: 2e6d 616b 654c 6179 6f75 7444 6972 7479  .makeLayoutDirty
+000571f0: 2829 292c 6f2e 7374 6174 653d 7b2e 2e2e  ()),o.state={...
+00057200: 6f2e 7374 6174 652c 2e2e 2e61 7d7d 6966  o.state,...a}}if
+00057210: 2865 213d 3d6e 756c 6c29 7b6c 6574 2073  (e!==null){let s
+00057220: 3d43 5b65 5d2e 656c 656d 656e 743b 646f  =C[e].element;do
+00057230: 6375 6d65 6e74 2e62 6f64 792e 6170 7065  cument.body.appe
+00057240: 6e64 4368 696c 6428 7329 7d69 213d 3d6e  ndChild(s)}i!==n
+00057250: 756c 6c26 2657 7528 692c 7229 3b66 6f72  ull&&Wu(i,r);for
+00057260: 286c 6574 2073 206f 6620 7229 7b6c 6574  (let s of r){let
+00057270: 2061 3d5b 735d 3b66 6f72 286c 6574 206f   a=[s];for(let o
+00057280: 206f 6620 6129 612e 7075 7368 282e 2e2e   of a)a.push(...
+00057290: 6f2e 6368 696c 6472 656e 292c 6f2e 6f6e  o.children),o.on
+000572a0: 4465 7374 7275 6374 696f 6e28 292c 6465  Destruction(),de
+000572b0: 6c65 7465 2043 5b6f 2e69 645d 2c56 652e  lete C[o.id],Ve.
+000572c0: 6465 6c65 7465 286f 2e65 6c65 6d65 6e74  delete(o.element
+000572d0: 297d 7574 2829 2c65 213d 3d6e 756c 6c26  )}ut(),e!==null&
+000572e0: 265f 7228 297d 6675 6e63 7469 6f6e 2046  &_r()}function F
+000572f0: 7528 7429 7b72 6574 7572 6e20 7479 7065  u(t){return type
+00057300: 6f66 2074 2e67 7261 624b 6579 626f 6172  of t.grabKeyboar
+00057310: 6446 6f63 7573 3d3d 2266 756e 6374 696f  dFocus=="functio
+00057320: 6e22 7d66 756e 6374 696f 6e20 5775 2874  n"}function Wu(t
+00057330: 2c65 297b 6c65 7420 6e3d 6474 2829 2c69  ,e){let n=dt(),i
+00057340: 3d74 2c72 3d6e 756c 6c3b 666f 7228 3b69  =t,r=null;for(;i
+00057350: 213d 3d6e 3b29 652e 6861 7328 6929 3f72  !==n;)e.has(i)?r
+00057360: 3d6e 756c 6c3a 723d 3d3d 6e75 6c6c 2626  =null:r===null&&
+00057370: 4675 2869 2926 2628 723d 6929 2c69 3d69  Fu(i)&&(r=i),i=i
+00057380: 2e70 6172 656e 743b 7221 3d3d 6e75 6c6c  .parent;r!==null
+00057390: 2626 722e 6772 6162 4b65 7962 6f61 7264  &&r.grabKeyboard
+000573a0: 466f 6375 7328 297d 676c 6f62 616c 5468  Focus()}globalTh
+000573b0: 6973 2e53 4553 5349 4f4e 5f54 4f4b 454e  is.SESSION_TOKEN
+000573c0: 3d22 7b73 6573 7369 6f6e 5f74 6f6b 656e  ="{session_token
+000573d0: 7d22 3b67 6c6f 6261 6c54 6869 732e 5049  }";globalThis.PI
+000573e0: 4e47 5f50 4f4e 475f 494e 5445 5256 414c  NG_PONG_INTERVAL
+000573f0: 5f53 4543 4f4e 4453 3d22 7b70 696e 675f  _SECONDS="{ping_
+00057400: 706f 6e67 5f69 6e74 6572 7661 6c7d 223b  pong_interval}";
+00057410: 676c 6f62 616c 5468 6973 2e52 494f 5f44  globalThis.RIO_D
+00057420: 4542 5547 5f4d 4f44 453d 227b 6465 6275  EBUG_MODE="{debu
+00057430: 675f 6d6f 6465 7d22 3b67 6c6f 6261 6c54  g_mode}";globalT
+00057440: 6869 732e 4348 494c 445f 4154 5452 4942  his.CHILD_ATTRIB
+00057450: 5554 455f 4e41 4d45 533d 227b 6368 696c  UTE_NAMES="{chil
+00057460: 645f 6174 7472 6962 7574 655f 6e61 6d65  d_attribute_name
+00057470: 737d 223b 676c 6f62 616c 5468 6973 2e52  s}";globalThis.R
+00057480: 554e 4e49 4e47 5f49 4e5f 5749 4e44 4f57  UNNING_IN_WINDOW
+00057490: 3d22 7b72 756e 6e69 6e67 5f69 6e5f 7769  ="{running_in_wi
+000574a0: 6e64 6f77 7d22 3b67 6c6f 6261 6c54 6869  ndow}";globalThi
+000574b0: 732e 5249 4f5f 4445 4255 4747 4552 3d6e  s.RIO_DEBUGGER=n
+000574c0: 756c 6c3b 6c65 7420 476e 3d21 313b 6675  ull;let Gn=!1;fu
+000574d0: 6e63 7469 6f6e 2055 7528 297b 6c65 7420  nction Uu(){let 
+000574e0: 743d 646f 6375 6d65 6e74 2e63 7265 6174  t=document.creat
+000574f0: 6545 6c65 6d65 6e74 2822 6469 7622 293b  eElement("div");
+00057500: 742e 7374 796c 652e 706f 7369 7469 6f6e  t.style.position
+00057510: 3d22 6162 736f 6c75 7465 222c 742e 7374  ="absolute",t.st
+00057520: 796c 652e 746f 703d 2230 7078 222c 742e  yle.top="0px",t.
+00057530: 7374 796c 652e 6c65 6674 3d22 3070 7822  style.left="0px"
+00057540: 2c74 2e73 7479 6c65 2e76 6973 6962 696c  ,t.style.visibil
+00057550: 6974 793d 2268 6964 6465 6e22 2c74 2e73  ity="hidden",t.s
+00057560: 7479 6c65 2e77 6964 7468 3d22 3230 3070  tyle.width="200p
+00057570: 7822 2c74 2e73 7479 6c65 2e68 6569 6768  x",t.style.heigh
+00057580: 743d 2231 3530 7078 222c 742e 7374 796c  t="150px",t.styl
+00057590: 652e 6f76 6572 666c 6f77 3d22 6869 6464  e.overflow="hidd
+000575a0: 656e 223b 6c65 7420 653d 646f 6375 6d65  en";let e=docume
+000575b0: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
+000575c0: 2822 7022 293b 652e 7374 796c 652e 7769  ("p");e.style.wi
+000575d0: 6474 683d 2231 3030 2522 2c65 2e73 7479  dth="100%",e.sty
+000575e0: 6c65 2e68 6569 6768 743d 2232 3030 7078  le.height="200px
+000575f0: 222c 742e 6170 7065 6e64 4368 696c 6428  ",t.appendChild(
+00057600: 6529 2c64 6f63 756d 656e 742e 626f 6479  e),document.body
+00057610: 2e61 7070 656e 6443 6869 6c64 2874 293b  .appendChild(t);
+00057620: 6c65 7420 6e3d 652e 6f66 6673 6574 5769  let n=e.offsetWi
+00057630: 6474 683b 742e 7374 796c 652e 6f76 6572  dth;t.style.over
+00057640: 666c 6f77 3d22 7363 726f 6c6c 223b 6c65  flow="scroll";le
+00057650: 7420 693d 652e 6f66 6673 6574 5769 6474  t i=e.offsetWidt
+00057660: 683b 7265 7475 726e 206e 3d3d 6926 2628  h;return n==i&&(
+00057670: 693d 742e 636c 6965 6e74 5769 6474 6829  i=t.clientWidth)
+00057680: 2c64 6f63 756d 656e 742e 626f 6479 2e72  ,document.body.r
+00057690: 656d 6f76 6543 6869 6c64 2874 292c 6e2d  emoveChild(t),n-
+000576a0: 697d 636f 6e73 7420 6373 3d55 7528 293b  i}const cs=Uu();
+000576b0: 6c65 7420 593d 3136 2c57 653d 6373 2f59  let Y=16,We=cs/Y
+000576c0: 3b66 756e 6374 696f 6e20 2475 2829 7b69  ;function $u(){i
+000576d0: 6628 7479 7065 6f66 2067 6c6f 6261 6c54  f(typeof globalT
+000576e0: 6869 732e 5049 4e47 5f50 4f4e 475f 494e  his.PING_PONG_IN
+000576f0: 5445 5256 414c 5f53 4543 4f4e 4453 213d  TERVAL_SECONDS!=
+00057700: 226e 756d 6265 7222 297b 636f 6e73 6f6c  "number"){consol
+00057710: 652e 6572 726f 7228 6052 6563 6569 7665  e.error(`Receive
+00057720: 6420 6572 726f 6e65 6f75 7320 4854 4d4c  d erroneous HTML
+00057730: 2066 726f 6d20 7468 6520 7365 7276 6572   from the server
+00057740: 3a20 5468 6520 7069 6e67 2070 6f6e 6720  : The ping pong 
+00057750: 696e 7465 7276 616c 2069 7320 247b 676c  interval is ${gl
+00057760: 6f62 616c 5468 6973 2e50 494e 475f 504f  obalThis.PING_PO
+00057770: 4e47 5f49 4e54 4552 5641 4c5f 5345 434f  NG_INTERVAL_SECO
+00057780: 4e44 537d 2069 6e73 7465 6164 206f 6620  NDS} instead of 
+00057790: 6120 6e75 6d62 6572 6029 3b72 6574 7572  a number`);retur
+000577a0: 6e7d 676c 6f62 616c 5468 6973 2e52 494f  n}globalThis.RIO
+000577b0: 5f44 4542 5547 5f4d 4f44 4526 2663 6f6e  _DEBUG_MODE&&con
+000577c0: 736f 6c65 2e77 6172 6e28 6052 696f 2069  sole.warn(`Rio i
+000577d0: 7320 7275 6e6e 696e 6720 696e 2044 4542  s running in DEB
+000577e0: 5547 206d 6f64 652e 0a44 6562 7567 206d  UG mode..Debug m
+000577f0: 6f64 6520 696e 636c 7564 6573 2068 656c  ode includes hel
+00057800: 7066 756c 2074 6f6f 6c73 2066 6f72 2064  pful tools for d
+00057810: 6576 656c 6f70 6d65 6e74 2c20 6275 7420  evelopment, but 
+00057820: 6973 2073 6c6f 7765 7220 616e 6420 6469  is slower and di
+00057830: 7361 626c 6573 2073 6f6d 6520 7361 6665  sables some safe
+00057840: 7479 2063 6865 636b 732e 204e 6576 6572  ty checks. Never
+00057850: 2075 7365 2069 7420 696e 2070 726f 6475   use it in produ
+00057860: 6374 696f 6e21 6029 3b76 6172 2074 3d64  ction!`);var t=d
+00057870: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
+00057880: 656d 656e 7428 2264 6976 2229 3b74 2e73  ement("div");t.s
+00057890: 7479 6c65 2e68 6569 6768 743d 2231 3072  tyle.height="10r
+000578a0: 656d 222c 646f 6375 6d65 6e74 2e62 6f64  em",document.bod
+000578b0: 792e 6170 7065 6e64 4368 696c 6428 7429  y.appendChild(t)
+000578c0: 2c59 3d74 2e6f 6666 7365 7448 6569 6768  ,Y=t.offsetHeigh
+000578d0: 742f 3130 2c64 6f63 756d 656e 742e 626f  t/10,document.bo
+000578e0: 6479 2e72 656d 6f76 6543 6869 6c64 2874  dy.removeChild(t
+000578f0: 292c 5765 3d63 732f 592c 676c 6f62 616c  ),We=cs/Y,global
+00057900: 5468 6973 2e70 6978 656c 7350 6572 5265  This.pixelsPerRe
+00057910: 6d3d 592c 676c 6f62 616c 5468 6973 2e73  m=Y,globalThis.s
+00057920: 6372 6f6c 6c42 6172 5369 7a65 3d57 652c  crollBarSize=We,
+00057930: 7769 6e64 6f77 2e61 6464 4576 656e 744c  window.addEventL
+00057940: 6973 7465 6e65 7228 2262 6566 6f72 6575  istener("beforeu
+00057950: 6e6c 6f61 6422 2c28 293d 3e7b 476e 3d21  nload",()=>{Gn=!
+00057960: 307d 292c 7769 6e64 6f77 2e61 6464 4576  0}),window.addEv
+00057970: 656e 744c 6973 7465 6e65 7228 2270 6f70  entListener("pop
+00057980: 7374 6174 6522 2c65 3d3e 7b63 6f6e 736f  state",e=>{conso
+00057990: 6c65 2e6c 6f67 2860 5552 4c20 6368 616e  le.log(`URL chan
+000579a0: 6765 6420 746f 2024 7b77 696e 646f 772e  ged to ${window.
+000579b0: 6c6f 6361 7469 6f6e 2e68 7265 667d 6029  location.href}`)
+000579c0: 2c6e 7428 226f 6e55 726c 4368 616e 6765  ,nt("onUrlChange
+000579d0: 222c 7b6e 6577 5572 6c3a 7769 6e64 6f77  ",{newUrl:window
+000579e0: 2e6c 6f63 6174 696f 6e2e 6872 6566 2e74  .location.href.t
+000579f0: 6f53 7472 696e 6728 297d 297d 292c 7769  oString()})}),wi
+00057a00: 6e64 6f77 2e61 6464 4576 656e 744c 6973  ndow.addEventLis
+00057a10: 7465 6e65 7228 2272 6573 697a 6522 2c65  tener("resize",e
+00057a20: 3d3e 7b74 7279 7b6e 7428 226f 6e57 696e  =>{try{nt("onWin
+00057a30: 646f 7752 6573 697a 6522 2c7b 6e65 7757  dowResize",{newW
+00057a40: 6964 7468 3a77 696e 646f 772e 696e 6e65  idth:window.inne
+00057a50: 7257 6964 7468 2f59 2c6e 6577 4865 6967  rWidth/Y,newHeig
+00057a60: 6874 3a77 696e 646f 772e 696e 6e65 7248  ht:window.innerH
+00057a70: 6569 6768 742f 597d 297d 6361 7463 6828  eight/Y})}catch(
+00057a80: 6929 7b63 6f6e 736f 6c65 2e77 6172 6e28  i){console.warn(
+00057a90: 6043 6f75 6c64 6e27 7420 6e6f 7469 6679  `Couldn't notify
+00057aa0: 2062 6163 6b65 6e64 206f 6620 7769 6e64   backend of wind
+00057ab0: 6f77 2072 6573 697a 653a 2024 7b69 7d60  ow resize: ${i}`
+00057ac0: 297d 6c65 7420 6e3d 646f 6375 6d65 6e74  )}let n=document
+00057ad0: 2e62 6f64 792e 7175 6572 7953 656c 6563  .body.querySelec
+00057ae0: 746f 7228 222e 7269 6f2d 6675 6e64 616d  tor(".rio-fundam
+00057af0: 656e 7461 6c2d 726f 6f74 2d63 6f6d 706f  ental-root-compo
+00057b00: 6e65 6e74 2229 3b6e 213d 3d6e 756c 6c26  nent");n!==null&
+00057b10: 2628 4b65 286e 292e 6d61 6b65 4c61 796f  &(Ke(n).makeLayo
+00057b20: 7574 4469 7274 7928 292c 7574 2829 297d  utDirty(),ut())}
+00057b30: 292c 7769 6e64 6f77 2e61 6464 4576 656e  ),window.addEven
+00057b40: 744c 6973 7465 6e65 7228 2268 6173 6863  tListener("hashc
+00057b50: 6861 6e67 6522 2c5f 7229 2c76 7328 297d  hange",_r),vs()}
+00057b60: 2475 2829 3b0a 0a3c 2f73 6372 6970 743e  $u();..</script>
+00057b70: 0a20 2020 2020 203c 7374 796c 653e 0a40  .      <style>.@
+00057b80: 6368 6172 7365 7420 2255 5446 2d38 223b  charset "UTF-8";
+00057b90: 2e72 696f 2d73 7769 7463 6865 726f 6f2d  .rio-switcheroo-
+00057ba0: 6261 636b 6772 6f75 6e64 7b2d 2d72 696f  background{--rio
+00057bb0: 2d6c 6f63 616c 2d62 673a 2076 6172 282d  -local-bg: var(-
+00057bc0: 2d72 696f 2d67 6c6f 6261 6c2d 6261 636b  -rio-global-back
+00057bd0: 6772 6f75 6e64 2d62 6729 3b2d 2d72 696f  ground-bg);--rio
+00057be0: 2d6c 6f63 616c 2d62 672d 7661 7269 616e  -local-bg-varian
+00057bf0: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
+00057c00: 6261 6c2d 6261 636b 6772 6f75 6e64 2d62  bal-background-b
+00057c10: 672d 7661 7269 616e 7429 3b2d 2d72 696f  g-variant);--rio
+00057c20: 2d6c 6f63 616c 2d62 672d 6163 7469 7665  -local-bg-active
+00057c30: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00057c40: 616c 2d62 6163 6b67 726f 756e 642d 6267  al-background-bg
+00057c50: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
+00057c60: 6f63 616c 2d66 673a 2076 6172 282d 2d72  ocal-fg: var(--r
+00057c70: 696f 2d67 6c6f 6261 6c2d 6261 636b 6772  io-global-backgr
+00057c80: 6f75 6e64 2d66 6729 3b2d 2d72 696f 2d6c  ound-fg);--rio-l
+00057c90: 6f63 616c 2d6c 6576 656c 2d32 2d62 673a  ocal-level-2-bg:
+00057ca0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+00057cb0: 6c2d 7365 636f 6e64 6172 792d 6267 293b  l-secondary-bg);
+00057cc0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+00057cd0: 6c2d 322d 6267 2d76 6172 6961 6e74 3a20  l-2-bg-variant: 
+00057ce0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00057cf0: 2d73 6563 6f6e 6461 7279 2d62 672d 7661  -secondary-bg-va
+00057d00: 7269 616e 7429 3b2d 2d72 696f 2d6c 6f63  riant);--rio-loc
+00057d10: 616c 2d6c 6576 656c 2d32 2d62 672d 6163  al-level-2-bg-ac
+00057d20: 7469 7665 3a20 7661 7228 2d2d 7269 6f2d  tive: var(--rio-
+00057d30: 676c 6f62 616c 2d73 6563 6f6e 6461 7279  global-secondary
+00057d40: 2d62 672d 6163 7469 7665 293b 2d2d 7269  -bg-active);--ri
+00057d50: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 322d  o-local-level-2-
+00057d60: 6667 3a20 7661 7228 2d2d 7269 6f2d 676c  fg: var(--rio-gl
+00057d70: 6f62 616c 2d73 6563 6f6e 6461 7279 2d66  obal-secondary-f
+00057d80: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
+00057d90: 6576 656c 2d33 2d62 673a 2076 6172 282d  evel-3-bg: var(-
+00057da0: 2d72 696f 2d67 6c6f 6261 6c2d 7072 696d  -rio-global-prim
+00057db0: 6172 792d 6267 293b 2d2d 7269 6f2d 6c6f  ary-bg);--rio-lo
+00057dc0: 6361 6c2d 6c65 7665 6c2d 332d 6267 2d76  cal-level-3-bg-v
+00057dd0: 6172 6961 6e74 3a20 7661 7228 2d2d 7269  ariant: var(--ri
+00057de0: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
+00057df0: 2d62 672d 7661 7269 616e 7429 3b2d 2d72  -bg-variant);--r
+00057e00: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
+00057e10: 2d62 672d 6163 7469 7665 3a20 7661 7228  -bg-active: var(
+00057e20: 2d2d 7269 6f2d 676c 6f62 616c 2d70 7269  --rio-global-pri
+00057e30: 6d61 7279 2d62 672d 6163 7469 7665 293b  mary-bg-active);
+00057e40: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+00057e50: 6c2d 332d 6667 3a20 7661 7228 2d2d 7269  l-3-fg: var(--ri
+00057e60: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
+00057e70: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
+00057e80: 2d68 6561 6469 6e67 312d 636f 6c6f 723a  -heading1-color:
+00057e90: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+00057ea0: 6c2d 6865 6164 696e 6731 2d63 6f6c 6f72  l-heading1-color
+00057eb0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
+00057ec0: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
+00057ed0: 643a 2076 6172 282d 2d72 696f 2d67 6c6f  d: var(--rio-glo
+00057ee0: 6261 6c2d 6865 6164 696e 6731 2d62 6163  bal-heading1-bac
+00057ef0: 6b67 726f 756e 6429 3b2d 2d72 696f 2d6c  kground);--rio-l
+00057f00: 6f63 616c 2d68 6561 6469 6e67 312d 6261  ocal-heading1-ba
+00057f10: 636b 6772 6f75 6e64 2d63 6c69 703a 2076  ckground-clip: v
+00057f20: 6172 2820 2d2d 7269 6f2d 676c 6f62 616c  ar( --rio-global
+00057f30: 2d68 6561 6469 6e67 312d 6261 636b 6772  -heading1-backgr
+00057f40: 6f75 6e64 2d63 6c69 7020 293b 2d2d 7269  ound-clip );--ri
+00057f50: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6731  o-local-heading1
+00057f60: 2d66 696c 6c2d 636f 6c6f 723a 2076 6172  -fill-color: var
+00057f70: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6865  (--rio-global-he
+00057f80: 6164 696e 6731 2d66 696c 6c2d 636f 6c6f  ading1-fill-colo
+00057f90: 7229 3b2d 2d72 696f 2d6c 6f63 616c 2d68  r);--rio-local-h
+00057fa0: 6561 6469 6e67 312d 666f 6e74 2d77 6569  eading1-font-wei
+00057fb0: 6768 743a 2076 6172 282d 2d72 696f 2d67  ght: var(--rio-g
+00057fc0: 6c6f 6261 6c2d 6865 6164 696e 6731 2d66  lobal-heading1-f
+00057fd0: 6f6e 742d 7765 6967 6874 293b 2d2d 7269  ont-weight);--ri
+00057fe0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
+00057ff0: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
+00058000: 6f2d 676c 6f62 616c 2d68 6561 6469 6e67  o-global-heading
+00058010: 322d 636f 6c6f 7229 3b2d 2d72 696f 2d6c  2-color);--rio-l
+00058020: 6f63 616c 2d68 6561 6469 6e67 322d 6261  ocal-heading2-ba
+00058030: 636b 6772 6f75 6e64 3a20 7661 7228 2d2d  ckground: var(--
+00058040: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
+00058050: 6e67 322d 6261 636b 6772 6f75 6e64 293b  ng2-background);
+00058060: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
+00058070: 696e 6732 2d62 6163 6b67 726f 756e 642d  ing2-background-
+00058080: 636c 6970 3a20 7661 7228 202d 2d72 696f  clip: var( --rio
+00058090: 2d67 6c6f 6261 6c2d 6865 6164 696e 6732  -global-heading2
+000580a0: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
+000580b0: 2029 3b2d 2d72 696f 2d6c 6f63 616c 2d68   );--rio-local-h
+000580c0: 6561 6469 6e67 322d 6669 6c6c 2d63 6f6c  eading2-fill-col
+000580d0: 6f72 3a20 7661 7228 2d2d 7269 6f2d 676c  or: var(--rio-gl
+000580e0: 6f62 616c 2d68 6561 6469 6e67 322d 6669  obal-heading2-fi
+000580f0: 6c6c 2d63 6f6c 6f72 293b 2d2d 7269 6f2d  ll-color);--rio-
+00058100: 6c6f 6361 6c2d 6865 6164 696e 6732 2d66  local-heading2-f
+00058110: 6f6e 742d 7765 6967 6874 3a20 7661 7228  ont-weight: var(
+00058120: 2d2d 7269 6f2d 676c 6f62 616c 2d68 6561  --rio-global-hea
+00058130: 6469 6e67 322d 666f 6e74 2d77 6569 6768  ding2-font-weigh
+00058140: 7429 3b2d 2d72 696f 2d6c 6f63 616c 2d68  t);--rio-local-h
+00058150: 6561 6469 6e67 332d 636f 6c6f 723a 2076  eading3-color: v
+00058160: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00058170: 6865 6164 696e 6733 2d63 6f6c 6f72 293b  heading3-color);
+00058180: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
+00058190: 696e 6733 2d62 6163 6b67 726f 756e 643a  ing3-background:
+000581a0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+000581b0: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
+000581c0: 726f 756e 6429 3b2d 2d72 696f 2d6c 6f63  round);--rio-loc
+000581d0: 616c 2d68 6561 6469 6e67 332d 6261 636b  al-heading3-back
+000581e0: 6772 6f75 6e64 2d63 6c69 703a 2076 6172  ground-clip: var
+000581f0: 2820 2d2d 7269 6f2d 676c 6f62 616c 2d68  ( --rio-global-h
+00058200: 6561 6469 6e67 332d 6261 636b 6772 6f75  eading3-backgrou
+00058210: 6e64 2d63 6c69 7020 293b 2d2d 7269 6f2d  nd-clip );--rio-
+00058220: 6c6f 6361 6c2d 6865 6164 696e 6733 2d66  local-heading3-f
+00058230: 696c 6c2d 636f 6c6f 723a 2076 6172 282d  ill-color: var(-
+00058240: 2d72 696f 2d67 6c6f 6261 6c2d 6865 6164  -rio-global-head
+00058250: 696e 6733 2d66 696c 6c2d 636f 6c6f 7229  ing3-fill-color)
+00058260: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+00058270: 6469 6e67 332d 666f 6e74 2d77 6569 6768  ding3-font-weigh
+00058280: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
+00058290: 6261 6c2d 6865 6164 696e 6733 2d66 6f6e  bal-heading3-fon
+000582a0: 742d 7765 6967 6874 293b 2d2d 7269 6f2d  t-weight);--rio-
+000582b0: 6c6f 6361 6c2d 7465 7874 2d63 6f6c 6f72  local-text-color
+000582c0: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+000582d0: 616c 2d74 6578 742d 636f 6c6f 7229 3b2d  al-text-color);-
+000582e0: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
+000582f0: 6261 636b 6772 6f75 6e64 3a20 7661 7228  background: var(
+00058300: 2d2d 7269 6f2d 676c 6f62 616c 2d74 6578  --rio-global-tex
+00058310: 742d 6261 636b 6772 6f75 6e64 293b 2d2d  t-background);--
+00058320: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d62  rio-local-text-b
+00058330: 6163 6b67 726f 756e 642d 636c 6970 3a20  ackground-clip: 
+00058340: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00058350: 2d74 6578 742d 6261 636b 6772 6f75 6e64  -text-background
+00058360: 2d63 6c69 7029 3b2d 2d72 696f 2d6c 6f63  -clip);--rio-loc
+00058370: 616c 2d74 6578 742d 6669 6c6c 2d63 6f6c  al-text-fill-col
+00058380: 6f72 3a20 7661 7228 2d2d 7269 6f2d 676c  or: var(--rio-gl
+00058390: 6f62 616c 2d74 6578 742d 6669 6c6c 2d63  obal-text-fill-c
+000583a0: 6f6c 6f72 293b 2d2d 7269 6f2d 6c6f 6361  olor);--rio-loca
+000583b0: 6c2d 7465 7874 2d66 6f6e 742d 7765 6967  l-text-font-weig
+000583c0: 6874 3a20 7661 7228 2d2d 7269 6f2d 676c  ht: var(--rio-gl
+000583d0: 6f62 616c 2d74 6578 742d 666f 6e74 2d77  obal-text-font-w
+000583e0: 6569 6768 7429 3b63 6f6c 6f72 3a76 6172  eight);color:var
+000583f0: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+00058400: 7d2e 7269 6f2d 7377 6974 6368 6572 6f6f  }.rio-switcheroo
+00058410: 2d6e 6575 7472 616c 7b2d 2d72 696f 2d6c  -neutral{--rio-l
+00058420: 6f63 616c 2d62 673a 2076 6172 282d 2d72  ocal-bg: var(--r
+00058430: 696f 2d67 6c6f 6261 6c2d 6e65 7574 7261  io-global-neutra
+00058440: 6c2d 6267 293b 2d2d 7269 6f2d 6c6f 6361  l-bg);--rio-loca
+00058450: 6c2d 6267 2d76 6172 6961 6e74 3a20 7661  l-bg-variant: va
+00058460: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d6e  r(--rio-global-n
+00058470: 6575 7472 616c 2d62 672d 7661 7269 616e  eutral-bg-varian
+00058480: 7429 3b2d 2d72 696f 2d6c 6f63 616c 2d62  t);--rio-local-b
+00058490: 672d 6163 7469 7665 3a20 7661 7228 2d2d  g-active: var(--
+000584a0: 7269 6f2d 676c 6f62 616c 2d6e 6575 7472  rio-global-neutr
+000584b0: 616c 2d62 672d 6163 7469 7665 293b 2d2d  al-bg-active);--
+000584c0: 7269 6f2d 6c6f 6361 6c2d 6667 3a20 7661  rio-local-fg: va
+000584d0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d6e  r(--rio-global-n
+000584e0: 6575 7472 616c 2d66 6729 3b2d 2d72 696f  eutral-fg);--rio
+000584f0: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
+00058500: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
+00058510: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
+00058520: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+00058530: 7665 6c2d 322d 6267 2d76 6172 6961 6e74  vel-2-bg-variant
+00058540: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00058550: 616c 2d73 6563 6f6e 6461 7279 2d62 672d  al-secondary-bg-
+00058560: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
+00058570: 6f63 616c 2d6c 6576 656c 2d32 2d62 672d  ocal-level-2-bg-
+00058580: 6163 7469 7665 3a20 7661 7228 2d2d 7269  active: var(--ri
+00058590: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
+000585a0: 7279 2d62 672d 6163 7469 7665 293b 2d2d  ry-bg-active);--
+000585b0: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
+000585c0: 322d 6667 3a20 7661 7228 2d2d 7269 6f2d  2-fg: var(--rio-
+000585d0: 676c 6f62 616c 2d73 6563 6f6e 6461 7279  global-secondary
+000585e0: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
+000585f0: 2d6c 6576 656c 2d33 2d62 673a 2076 6172  -level-3-bg: var
+00058600: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7072  (--rio-global-pr
+00058610: 696d 6172 792d 6267 293b 2d2d 7269 6f2d  imary-bg);--rio-
+00058620: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
+00058630: 2d76 6172 6961 6e74 3a20 7661 7228 2d2d  -variant: var(--
+00058640: 7269 6f2d 676c 6f62 616c 2d70 7269 6d61  rio-global-prima
+00058650: 7279 2d62 672d 7661 7269 616e 7429 3b2d  ry-bg-variant);-
+00058660: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
+00058670: 2d33 2d62 672d 6163 7469 7665 3a20 7661  -3-bg-active: va
+00058680: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d70  r(--rio-global-p
+00058690: 7269 6d61 7279 2d62 672d 6163 7469 7665  rimary-bg-active
+000586a0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+000586b0: 7665 6c2d 332d 6667 3a20 7661 7228 2d2d  vel-3-fg: var(--
+000586c0: 7269 6f2d 676c 6f62 616c 2d70 7269 6d61  rio-global-prima
+000586d0: 7279 2d66 6729 3b2d 2d72 696f 2d6c 6f63  ry-fg);--rio-loc
+000586e0: 616c 2d68 6561 6469 6e67 312d 636f 6c6f  al-heading1-colo
+000586f0: 723a 2076 6172 282d 2d72 696f 2d67 6c6f  r: var(--rio-glo
+00058700: 6261 6c2d 6865 6164 696e 6731 2d63 6f6c  bal-heading1-col
+00058710: 6f72 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  or);--rio-local-
+00058720: 6865 6164 696e 6731 2d62 6163 6b67 726f  heading1-backgro
+00058730: 756e 643a 2076 6172 282d 2d72 696f 2d67  und: var(--rio-g
+00058740: 6c6f 6261 6c2d 6865 6164 696e 6731 2d62  lobal-heading1-b
+00058750: 6163 6b67 726f 756e 6429 3b2d 2d72 696f  ackground);--rio
+00058760: 2d6c 6f63 616c 2d68 6561 6469 6e67 312d  -local-heading1-
+00058770: 6261 636b 6772 6f75 6e64 2d63 6c69 703a  background-clip:
+00058780: 2076 6172 2820 2d2d 7269 6f2d 676c 6f62   var( --rio-glob
+00058790: 616c 2d68 6561 6469 6e67 312d 6261 636b  al-heading1-back
+000587a0: 6772 6f75 6e64 2d63 6c69 7020 293b 2d2d  ground-clip );--
+000587b0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+000587c0: 6731 2d66 696c 6c2d 636f 6c6f 723a 2076  g1-fill-color: v
+000587d0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+000587e0: 6865 6164 696e 6731 2d66 696c 6c2d 636f  heading1-fill-co
+000587f0: 6c6f 7229 3b2d 2d72 696f 2d6c 6f63 616c  lor);--rio-local
+00058800: 2d68 6561 6469 6e67 312d 666f 6e74 2d77  -heading1-font-w
+00058810: 6569 6768 743a 2076 6172 282d 2d72 696f  eight: var(--rio
+00058820: 2d67 6c6f 6261 6c2d 6865 6164 696e 6731  -global-heading1
+00058830: 2d66 6f6e 742d 7765 6967 6874 293b 2d2d  -font-weight);--
+00058840: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+00058850: 6732 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g2-color: var(--
+00058860: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
+00058870: 6e67 322d 636f 6c6f 7229 3b2d 2d72 696f  ng2-color);--rio
+00058880: 2d6c 6f63 616c 2d68 6561 6469 6e67 322d  -local-heading2-
+00058890: 6261 636b 6772 6f75 6e64 3a20 7661 7228  background: var(
+000588a0: 2d2d 7269 6f2d 676c 6f62 616c 2d68 6561  --rio-global-hea
+000588b0: 6469 6e67 322d 6261 636b 6772 6f75 6e64  ding2-background
+000588c0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
+000588d0: 6164 696e 6732 2d62 6163 6b67 726f 756e  ading2-backgroun
+000588e0: 642d 636c 6970 3a20 7661 7228 202d 2d72  d-clip: var( --r
+000588f0: 696f 2d67 6c6f 6261 6c2d 6865 6164 696e  io-global-headin
+00058900: 6732 2d62 6163 6b67 726f 756e 642d 636c  g2-background-cl
+00058910: 6970 2029 3b2d 2d72 696f 2d6c 6f63 616c  ip );--rio-local
+00058920: 2d68 6561 6469 6e67 322d 6669 6c6c 2d63  -heading2-fill-c
+00058930: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
+00058940: 676c 6f62 616c 2d68 6561 6469 6e67 322d  global-heading2-
+00058950: 6669 6c6c 2d63 6f6c 6f72 293b 2d2d 7269  fill-color);--ri
+00058960: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
+00058970: 2d66 6f6e 742d 7765 6967 6874 3a20 7661  -font-weight: va
+00058980: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
+00058990: 6561 6469 6e67 322d 666f 6e74 2d77 6569  eading2-font-wei
+000589a0: 6768 7429 3b2d 2d72 696f 2d6c 6f63 616c  ght);--rio-local
+000589b0: 2d68 6561 6469 6e67 332d 636f 6c6f 723a  -heading3-color:
+000589c0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+000589d0: 6c2d 6865 6164 696e 6733 2d63 6f6c 6f72  l-heading3-color
+000589e0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
+000589f0: 6164 696e 6733 2d62 6163 6b67 726f 756e  ading3-backgroun
+00058a00: 643a 2076 6172 282d 2d72 696f 2d67 6c6f  d: var(--rio-glo
+00058a10: 6261 6c2d 6865 6164 696e 6733 2d62 6163  bal-heading3-bac
+00058a20: 6b67 726f 756e 6429 3b2d 2d72 696f 2d6c  kground);--rio-l
+00058a30: 6f63 616c 2d68 6561 6469 6e67 332d 6261  ocal-heading3-ba
+00058a40: 636b 6772 6f75 6e64 2d63 6c69 703a 2076  ckground-clip: v
+00058a50: 6172 2820 2d2d 7269 6f2d 676c 6f62 616c  ar( --rio-global
+00058a60: 2d68 6561 6469 6e67 332d 6261 636b 6772  -heading3-backgr
+00058a70: 6f75 6e64 2d63 6c69 7020 293b 2d2d 7269  ound-clip );--ri
+00058a80: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
+00058a90: 2d66 696c 6c2d 636f 6c6f 723a 2076 6172  -fill-color: var
+00058aa0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6865  (--rio-global-he
+00058ab0: 6164 696e 6733 2d66 696c 6c2d 636f 6c6f  ading3-fill-colo
+00058ac0: 7229 3b2d 2d72 696f 2d6c 6f63 616c 2d68  r);--rio-local-h
+00058ad0: 6561 6469 6e67 332d 666f 6e74 2d77 6569  eading3-font-wei
+00058ae0: 6768 743a 2076 6172 282d 2d72 696f 2d67  ght: var(--rio-g
+00058af0: 6c6f 6261 6c2d 6865 6164 696e 6733 2d66  lobal-heading3-f
+00058b00: 6f6e 742d 7765 6967 6874 293b 2d2d 7269  ont-weight);--ri
+00058b10: 6f2d 6c6f 6361 6c2d 7465 7874 2d63 6f6c  o-local-text-col
+00058b20: 6f72 3a20 7661 7228 2d2d 7269 6f2d 676c  or: var(--rio-gl
+00058b30: 6f62 616c 2d74 6578 742d 636f 6c6f 7229  obal-text-color)
+00058b40: 3b2d 2d72 696f 2d6c 6f63 616c 2d74 6578  ;--rio-local-tex
+00058b50: 742d 6261 636b 6772 6f75 6e64 3a20 7661  t-background: va
+00058b60: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d74  r(--rio-global-t
+00058b70: 6578 742d 6261 636b 6772 6f75 6e64 293b  ext-background);
+00058b80: 2d2d 7269 6f2d 6c6f 6361 6c2d 7465 7874  --rio-local-text
+00058b90: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
+00058ba0: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00058bb0: 616c 2d74 6578 742d 6261 636b 6772 6f75  al-text-backgrou
+00058bc0: 6e64 2d63 6c69 7029 3b2d 2d72 696f 2d6c  nd-clip);--rio-l
+00058bd0: 6f63 616c 2d74 6578 742d 6669 6c6c 2d63  ocal-text-fill-c
+00058be0: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
+00058bf0: 676c 6f62 616c 2d74 6578 742d 6669 6c6c  global-text-fill
+00058c00: 2d63 6f6c 6f72 293b 2d2d 7269 6f2d 6c6f  -color);--rio-lo
+00058c10: 6361 6c2d 7465 7874 2d66 6f6e 742d 7765  cal-text-font-we
+00058c20: 6967 6874 3a20 7661 7228 2d2d 7269 6f2d  ight: var(--rio-
+00058c30: 676c 6f62 616c 2d74 6578 742d 666f 6e74  global-text-font
+00058c40: 2d77 6569 6768 7429 3b63 6f6c 6f72 3a76  -weight);color:v
+00058c50: 6172 282d 2d72 696f 2d6c 6f63 616c 2d66  ar(--rio-local-f
+00058c60: 6729 7d2e 7269 6f2d 7377 6974 6368 6572  g)}.rio-switcher
+00058c70: 6f6f 2d68 7564 7b2d 2d72 696f 2d6c 6f63  oo-hud{--rio-loc
+00058c80: 616c 2d62 673a 2076 6172 282d 2d72 696f  al-bg: var(--rio
+00058c90: 2d67 6c6f 6261 6c2d 6875 642d 6267 293b  -global-hud-bg);
+00058ca0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6267 2d76  --rio-local-bg-v
+00058cb0: 6172 6961 6e74 3a20 7661 7228 2d2d 7269  ariant: var(--ri
+00058cc0: 6f2d 676c 6f62 616c 2d68 7564 2d62 672d  o-global-hud-bg-
+00058cd0: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
+00058ce0: 6f63 616c 2d62 672d 6163 7469 7665 3a20  ocal-bg-active: 
+00058cf0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00058d00: 2d68 7564 2d62 672d 6163 7469 7665 293b  -hud-bg-active);
+00058d10: 2d2d 7269 6f2d 6c6f 6361 6c2d 6667 3a20  --rio-local-fg: 
+00058d20: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00058d30: 2d68 7564 2d66 6729 3b2d 2d72 696f 2d6c  -hud-fg);--rio-l
+00058d40: 6f63 616c 2d6c 6576 656c 2d32 2d62 673a  ocal-level-2-bg:
+00058d50: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+00058d60: 6c2d 7072 696d 6172 792d 6267 293b 2d2d  l-primary-bg);--
+00058d70: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
+00058d80: 322d 6267 2d76 6172 6961 6e74 3a20 7661  2-bg-variant: va
+00058d90: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d70  r(--rio-global-p
+00058da0: 7269 6d61 7279 2d62 672d 7661 7269 616e  rimary-bg-varian
+00058db0: 7429 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  t);--rio-local-l
+00058dc0: 6576 656c 2d32 2d62 672d 6163 7469 7665  evel-2-bg-active
+00058dd0: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00058de0: 616c 2d70 7269 6d61 7279 2d62 672d 6163  al-primary-bg-ac
+00058df0: 7469 7665 293b 2d2d 7269 6f2d 6c6f 6361  tive);--rio-loca
+00058e00: 6c2d 6c65 7665 6c2d 322d 6667 3a20 7661  l-level-2-fg: va
+00058e10: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d70  r(--rio-global-p
+00058e20: 7269 6d61 7279 2d66 6729 3b2d 2d72 696f  rimary-fg);--rio
+00058e30: 2d6c 6f63 616c 2d6c 6576 656c 2d33 2d62  -local-level-3-b
+00058e40: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
+00058e50: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
+00058e60: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+00058e70: 7665 6c2d 332d 6267 2d76 6172 6961 6e74  vel-3-bg-variant
+00058e80: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00058e90: 616c 2d73 6563 6f6e 6461 7279 2d62 672d  al-secondary-bg-
+00058ea0: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
+00058eb0: 6f63 616c 2d6c 6576 656c 2d33 2d62 672d  ocal-level-3-bg-
+00058ec0: 6163 7469 7665 3a20 7661 7228 2d2d 7269  active: var(--ri
+00058ed0: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
+00058ee0: 7279 2d62 672d 6163 7469 7665 293b 2d2d  ry-bg-active);--
+00058ef0: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
+00058f00: 332d 6667 3a20 7661 7228 2d2d 7269 6f2d  3-fg: var(--rio-
+00058f10: 676c 6f62 616c 2d73 6563 6f6e 6461 7279  global-secondary
+00058f20: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
+00058f30: 2d68 6561 6469 6e67 312d 636f 6c6f 723a  -heading1-color:
+00058f40: 2076 6172 282d 2d72 696f 2d6c 6f63 616c   var(--rio-local
+00058f50: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
+00058f60: 2d68 6561 6469 6e67 312d 6261 636b 6772  -heading1-backgr
+00058f70: 6f75 6e64 3a20 226e 6f6e 6522 3b2d 2d72  ound: "none";--r
+00058f80: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
+00058f90: 312d 6261 636b 6772 6f75 6e64 2d63 6c69  1-background-cli
+00058fa0: 703a 2022 626f 7264 6572 2d62 6f78 223b  p: "border-box";
+00058fb0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
+00058fc0: 696e 6731 2d66 696c 6c2d 636f 6c6f 723a  ing1-fill-color:
+00058fd0: 2022 7472 616e 7370 6172 656e 7422 3b2d   "transparent";-
+00058fe0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+00058ff0: 6e67 322d 636f 6c6f 723a 2076 6172 282d  ng2-color: var(-
+00059000: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
+00059010: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+00059020: 6e67 322d 6261 636b 6772 6f75 6e64 3a20  ng2-background: 
+00059030: 226e 6f6e 6522 3b2d 2d72 696f 2d6c 6f63  "none";--rio-loc
+00059040: 616c 2d68 6561 6469 6e67 322d 6261 636b  al-heading2-back
+00059050: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
+00059060: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
+00059070: 6c6f 6361 6c2d 6865 6164 696e 6732 2d66  local-heading2-f
+00059080: 696c 6c2d 636f 6c6f 723a 2022 7472 616e  ill-color: "tran
+00059090: 7370 6172 656e 7422 3b2d 2d72 696f 2d6c  sparent";--rio-l
+000590a0: 6f63 616c 2d68 6561 6469 6e67 332d 636f  ocal-heading3-co
+000590b0: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+000590c0: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+000590d0: 6f63 616c 2d68 6561 6469 6e67 332d 6261  ocal-heading3-ba
+000590e0: 636b 6772 6f75 6e64 3a20 226e 6f6e 6522  ckground: "none"
+000590f0: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+00059100: 6469 6e67 332d 6261 636b 6772 6f75 6e64  ding3-background
+00059110: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
+00059120: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
+00059130: 6865 6164 696e 6733 2d66 696c 6c2d 636f  heading3-fill-co
+00059140: 6c6f 723a 2022 7472 616e 7370 6172 656e  lor: "transparen
+00059150: 7422 3b2d 2d72 696f 2d6c 6f63 616c 2d74  t";--rio-local-t
+00059160: 6578 742d 636f 6c6f 723a 2076 6172 282d  ext-color: var(-
+00059170: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
+00059180: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
+00059190: 6261 636b 6772 6f75 6e64 3a20 226e 6f6e  background: "non
+000591a0: 6522 3b2d 2d72 696f 2d6c 6f63 616c 2d74  e";--rio-local-t
+000591b0: 6578 742d 6261 636b 6772 6f75 6e64 2d63  ext-background-c
+000591c0: 6c69 703a 2022 626f 7264 6572 2d62 6f78  lip: "border-box
+000591d0: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  ";--rio-local-te
+000591e0: 7874 2d66 696c 6c2d 636f 6c6f 723a 2022  xt-fill-color: "
+000591f0: 7472 616e 7370 6172 656e 7422 3b63 6f6c  transparent";col
+00059200: 6f72 3a76 6172 282d 2d72 696f 2d6c 6f63  or:var(--rio-loc
+00059210: 616c 2d66 6729 7d2e 7269 6f2d 7377 6974  al-fg)}.rio-swit
+00059220: 6368 6572 6f6f 2d70 7269 6d61 7279 7b2d  cheroo-primary{-
+00059230: 2d72 696f 2d6c 6f63 616c 2d62 673a 2076  -rio-local-bg: v
+00059240: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00059250: 7072 696d 6172 792d 6267 293b 2d2d 7269  primary-bg);--ri
+00059260: 6f2d 6c6f 6361 6c2d 6267 2d76 6172 6961  o-local-bg-varia
+00059270: 6e74 3a20 7661 7228 2d2d 7269 6f2d 676c  nt: var(--rio-gl
+00059280: 6f62 616c 2d70 7269 6d61 7279 2d62 672d  obal-primary-bg-
+00059290: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
+000592a0: 6f63 616c 2d62 672d 6163 7469 7665 3a20  ocal-bg-active: 
+000592b0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+000592c0: 2d70 7269 6d61 7279 2d62 672d 6163 7469  -primary-bg-acti
+000592d0: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
+000592e0: 6667 3a20 7661 7228 2d2d 7269 6f2d 676c  fg: var(--rio-gl
+000592f0: 6f62 616c 2d70 7269 6d61 7279 2d66 6729  obal-primary-fg)
+00059300: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
+00059310: 656c 2d32 2d62 673a 2076 6172 282d 2d72  el-2-bg: var(--r
+00059320: 696f 2d67 6c6f 6261 6c2d 7365 636f 6e64  io-global-second
+00059330: 6172 792d 6267 293b 2d2d 7269 6f2d 6c6f  ary-bg);--rio-lo
+00059340: 6361 6c2d 6c65 7665 6c2d 322d 6267 2d76  cal-level-2-bg-v
+00059350: 6172 6961 6e74 3a20 7661 7228 2d2d 7269  ariant: var(--ri
+00059360: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
+00059370: 7279 2d62 672d 7661 7269 616e 7429 3b2d  ry-bg-variant);-
+00059380: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
+00059390: 2d32 2d62 672d 6163 7469 7665 3a20 7661  -2-bg-active: va
+000593a0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
+000593b0: 6563 6f6e 6461 7279 2d62 672d 6163 7469  econdary-bg-acti
+000593c0: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
+000593d0: 6c65 7665 6c2d 322d 6667 3a20 7661 7228  level-2-fg: var(
+000593e0: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
+000593f0: 6f6e 6461 7279 2d66 6729 3b2d 2d72 696f  ondary-fg);--rio
+00059400: 2d6c 6f63 616c 2d6c 6576 656c 2d33 2d62  -local-level-3-b
+00059410: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
+00059420: 6261 6c2d 7072 696d 6172 792d 6267 293b  bal-primary-bg);
+00059430: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+00059440: 6c2d 332d 6267 2d76 6172 6961 6e74 3a20  l-3-bg-variant: 
+00059450: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00059460: 2d70 7269 6d61 7279 2d62 672d 7661 7269  -primary-bg-vari
+00059470: 616e 7429 3b2d 2d72 696f 2d6c 6f63 616c  ant);--rio-local
+00059480: 2d6c 6576 656c 2d33 2d62 672d 6163 7469  -level-3-bg-acti
+00059490: 7665 3a20 7661 7228 2d2d 7269 6f2d 676c  ve: var(--rio-gl
+000594a0: 6f62 616c 2d70 7269 6d61 7279 2d62 672d  obal-primary-bg-
+000594b0: 6163 7469 7665 293b 2d2d 7269 6f2d 6c6f  active);--rio-lo
+000594c0: 6361 6c2d 6c65 7665 6c2d 332d 6667 3a20  cal-level-3-fg: 
+000594d0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+000594e0: 2d70 7269 6d61 7279 2d66 6729 3b2d 2d72  -primary-fg);--r
+000594f0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
+00059500: 312d 636f 6c6f 723a 2076 6172 282d 2d72  1-color: var(--r
+00059510: 696f 2d6c 6f63 616c 2d66 6729 3b2d 2d72  io-local-fg);--r
+00059520: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
+00059530: 312d 6261 636b 6772 6f75 6e64 3a20 226e  1-background: "n
+00059540: 6f6e 6522 3b2d 2d72 696f 2d6c 6f63 616c  one";--rio-local
+00059550: 2d68 6561 6469 6e67 312d 6261 636b 6772  -heading1-backgr
+00059560: 6f75 6e64 2d63 6c69 703a 2022 626f 7264  ound-clip: "bord
+00059570: 6572 2d62 6f78 223b 2d2d 7269 6f2d 6c6f  er-box";--rio-lo
+00059580: 6361 6c2d 6865 6164 696e 6731 2d66 696c  cal-heading1-fil
+00059590: 6c2d 636f 6c6f 723a 2022 7472 616e 7370  l-color: "transp
+000595a0: 6172 656e 7422 3b2d 2d72 696f 2d6c 6f63  arent";--rio-loc
+000595b0: 616c 2d68 6561 6469 6e67 322d 636f 6c6f  al-heading2-colo
+000595c0: 723a 2076 6172 282d 2d72 696f 2d6c 6f63  r: var(--rio-loc
+000595d0: 616c 2d66 6729 3b2d 2d72 696f 2d6c 6f63  al-fg);--rio-loc
+000595e0: 616c 2d68 6561 6469 6e67 322d 6261 636b  al-heading2-back
+000595f0: 6772 6f75 6e64 3a20 226e 6f6e 6522 3b2d  ground: "none";-
+00059600: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+00059610: 6e67 322d 6261 636b 6772 6f75 6e64 2d63  ng2-background-c
+00059620: 6c69 703a 2022 626f 7264 6572 2d62 6f78  lip: "border-box
+00059630: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
+00059640: 6164 696e 6732 2d66 696c 6c2d 636f 6c6f  ading2-fill-colo
+00059650: 723a 2022 7472 616e 7370 6172 656e 7422  r: "transparent"
+00059660: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+00059670: 6469 6e67 332d 636f 6c6f 723a 2076 6172  ding3-color: var
+00059680: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+00059690: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+000596a0: 6469 6e67 332d 6261 636b 6772 6f75 6e64  ding3-background
+000596b0: 3a20 226e 6f6e 6522 3b2d 2d72 696f 2d6c  : "none";--rio-l
+000596c0: 6f63 616c 2d68 6561 6469 6e67 332d 6261  ocal-heading3-ba
+000596d0: 636b 6772 6f75 6e64 2d63 6c69 703a 2022  ckground-clip: "
+000596e0: 626f 7264 6572 2d62 6f78 223b 2d2d 7269  border-box";--ri
+000596f0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
+00059700: 2d66 696c 6c2d 636f 6c6f 723a 2022 7472  -fill-color: "tr
+00059710: 616e 7370 6172 656e 7422 3b2d 2d72 696f  ansparent";--rio
+00059720: 2d6c 6f63 616c 2d74 6578 742d 636f 6c6f  -local-text-colo
+00059730: 723a 2076 6172 282d 2d72 696f 2d6c 6f63  r: var(--rio-loc
+00059740: 616c 2d66 6729 3b2d 2d72 696f 2d6c 6f63  al-fg);--rio-loc
+00059750: 616c 2d74 6578 742d 6261 636b 6772 6f75  al-text-backgrou
+00059760: 6e64 3a20 226e 6f6e 6522 3b2d 2d72 696f  nd: "none";--rio
+00059770: 2d6c 6f63 616c 2d74 6578 742d 6261 636b  -local-text-back
+00059780: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
+00059790: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
+000597a0: 6c6f 6361 6c2d 7465 7874 2d66 696c 6c2d  local-text-fill-
+000597b0: 636f 6c6f 723a 2022 7472 616e 7370 6172  color: "transpar
+000597c0: 656e 7422 3b63 6f6c 6f72 3a76 6172 282d  ent";color:var(-
+000597d0: 2d72 696f 2d6c 6f63 616c 2d66 6729 7d2e  -rio-local-fg)}.
+000597e0: 7269 6f2d 7377 6974 6368 6572 6f6f 2d73  rio-switcheroo-s
+000597f0: 6563 6f6e 6461 7279 7b2d 2d72 696f 2d6c  econdary{--rio-l
+00059800: 6f63 616c 2d62 673a 2076 6172 282d 2d72  ocal-bg: var(--r
 00059810: 696f 2d67 6c6f 6261 6c2d 7365 636f 6e64  io-global-second
-00059820: 6172 792d 6267 2d61 6374 6976 6529 3b2d  ary-bg-active);-
-00059830: 2d72 696f 2d6c 6f63 616c 2d66 673a 2076  -rio-local-fg: v
-00059840: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00059850: 7365 636f 6e64 6172 792d 6667 293b 2d2d  secondary-fg);--
-00059860: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-00059870: 322d 6267 3a20 7661 7228 2d2d 7269 6f2d  2-bg: var(--rio-
-00059880: 676c 6f62 616c 2d70 7269 6d61 7279 2d62  global-primary-b
-00059890: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
-000598a0: 6576 656c 2d32 2d62 672d 7661 7269 616e  evel-2-bg-varian
-000598b0: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
-000598c0: 6261 6c2d 7072 696d 6172 792d 6267 2d76  bal-primary-bg-v
-000598d0: 6172 6961 6e74 293b 2d2d 7269 6f2d 6c6f  ariant);--rio-lo
-000598e0: 6361 6c2d 6c65 7665 6c2d 322d 6267 2d61  cal-level-2-bg-a
-000598f0: 6374 6976 653a 2076 6172 282d 2d72 696f  ctive: var(--rio
-00059900: 2d67 6c6f 6261 6c2d 7072 696d 6172 792d  -global-primary-
-00059910: 6267 2d61 6374 6976 6529 3b2d 2d72 696f  bg-active);--rio
-00059920: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d66  -local-level-2-f
-00059930: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
-00059940: 6261 6c2d 7072 696d 6172 792d 6667 293b  bal-primary-fg);
-00059950: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-00059960: 6c2d 332d 6267 3a20 7661 7228 2d2d 7269  l-3-bg: var(--ri
-00059970: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
-00059980: 7279 2d62 6729 3b2d 2d72 696f 2d6c 6f63  ry-bg);--rio-loc
-00059990: 616c 2d6c 6576 656c 2d33 2d62 672d 7661  al-level-3-bg-va
-000599a0: 7269 616e 743a 2076 6172 282d 2d72 696f  riant: var(--rio
-000599b0: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
-000599c0: 792d 6267 2d76 6172 6961 6e74 293b 2d2d  y-bg-variant);--
-000599d0: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-000599e0: 332d 6267 2d61 6374 6976 653a 2076 6172  3-bg-active: var
-000599f0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
-00059a00: 636f 6e64 6172 792d 6267 2d61 6374 6976  condary-bg-activ
-00059a10: 6529 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  e);--rio-local-l
-00059a20: 6576 656c 2d33 2d66 673a 2076 6172 282d  evel-3-fg: var(-
-00059a30: 2d72 696f 2d67 6c6f 6261 6c2d 7365 636f  -rio-global-seco
-00059a40: 6e64 6172 792d 6667 293b 2d2d 7269 6f2d  ndary-fg);--rio-
-00059a50: 6c6f 6361 6c2d 6865 6164 696e 6731 2d63  local-heading1-c
-00059a60: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
-00059a70: 6c6f 6361 6c2d 6667 293b 2d2d 7269 6f2d  local-fg);--rio-
-00059a80: 6c6f 6361 6c2d 6865 6164 696e 6731 2d62  local-heading1-b
-00059a90: 6163 6b67 726f 756e 643a 2022 6e6f 6e65  ackground: "none
-00059aa0: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
-00059ab0: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
-00059ac0: 642d 636c 6970 3a20 2262 6f72 6465 722d  d-clip: "border-
-00059ad0: 626f 7822 3b2d 2d72 696f 2d6c 6f63 616c  box";--rio-local
-00059ae0: 2d68 6561 6469 6e67 312d 6669 6c6c 2d63  -heading1-fill-c
-00059af0: 6f6c 6f72 3a20 2274 7261 6e73 7061 7265  olor: "transpare
-00059b00: 6e74 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt";--rio-local-
-00059b10: 6865 6164 696e 6732 2d63 6f6c 6f72 3a20  heading2-color: 
-00059b20: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00059b30: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-00059b40: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
-00059b50: 756e 643a 2022 6e6f 6e65 223b 2d2d 7269  und: "none";--ri
-00059b60: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
-00059b70: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
-00059b80: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
-00059b90: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-00059ba0: 6e67 322d 6669 6c6c 2d63 6f6c 6f72 3a20  ng2-fill-color: 
-00059bb0: 2274 7261 6e73 7061 7265 6e74 223b 2d2d  "transparent";--
-00059bc0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-00059bd0: 6733 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g3-color: var(--
-00059be0: 7269 6f2d 6c6f 6361 6c2d 6667 293b 2d2d  rio-local-fg);--
-00059bf0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-00059c00: 6733 2d62 6163 6b67 726f 756e 643a 2022  g3-background: "
-00059c10: 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f 6361  none";--rio-loca
-00059c20: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
-00059c30: 726f 756e 642d 636c 6970 3a20 2262 6f72  round-clip: "bor
-00059c40: 6465 722d 626f 7822 3b2d 2d72 696f 2d6c  der-box";--rio-l
-00059c50: 6f63 616c 2d68 6561 6469 6e67 332d 6669  ocal-heading3-fi
-00059c60: 6c6c 2d63 6f6c 6f72 3a20 2274 7261 6e73  ll-color: "trans
-00059c70: 7061 7265 6e74 223b 2d2d 7269 6f2d 6c6f  parent";--rio-lo
-00059c80: 6361 6c2d 7465 7874 2d63 6f6c 6f72 3a20  cal-text-color: 
-00059c90: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00059ca0: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-00059cb0: 7465 7874 2d62 6163 6b67 726f 756e 643a  text-background:
-00059cc0: 2022 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f   "none";--rio-lo
-00059cd0: 6361 6c2d 7465 7874 2d62 6163 6b67 726f  cal-text-backgro
-00059ce0: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
-00059cf0: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
-00059d00: 616c 2d74 6578 742d 6669 6c6c 2d63 6f6c  al-text-fill-col
-00059d10: 6f72 3a20 2274 7261 6e73 7061 7265 6e74  or: "transparent
-00059d20: 223b 636f 6c6f 723a 7661 7228 2d2d 7269  ";color:var(--ri
-00059d30: 6f2d 6c6f 6361 6c2d 6667 297d 2e72 696f  o-local-fg)}.rio
-00059d40: 2d73 7769 7463 6865 726f 6f2d 7375 6363  -switcheroo-succ
-00059d50: 6573 737b 2d2d 7269 6f2d 6c6f 6361 6c2d  ess{--rio-local-
-00059d60: 6267 3a20 7661 7228 2d2d 7269 6f2d 676c  bg: var(--rio-gl
-00059d70: 6f62 616c 2d73 7563 6365 7373 2d62 6729  obal-success-bg)
-00059d80: 3b2d 2d72 696f 2d6c 6f63 616c 2d62 672d  ;--rio-local-bg-
-00059d90: 7661 7269 616e 743a 2076 6172 282d 2d72  variant: var(--r
-00059da0: 696f 2d67 6c6f 6261 6c2d 7375 6363 6573  io-global-succes
-00059db0: 732d 6267 2d76 6172 6961 6e74 293b 2d2d  s-bg-variant);--
-00059dc0: 7269 6f2d 6c6f 6361 6c2d 6267 2d61 6374  rio-local-bg-act
-00059dd0: 6976 653a 2076 6172 282d 2d72 696f 2d67  ive: var(--rio-g
-00059de0: 6c6f 6261 6c2d 7375 6363 6573 732d 6267  lobal-success-bg
-00059df0: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
-00059e00: 6f63 616c 2d66 673a 2076 6172 282d 2d72  ocal-fg: var(--r
-00059e10: 696f 2d67 6c6f 6261 6c2d 7375 6363 6573  io-global-succes
-00059e20: 732d 6667 293b 2d2d 7269 6f2d 6c6f 6361  s-fg);--rio-loca
-00059e30: 6c2d 6c65 7665 6c2d 322d 6267 3a20 7661  l-level-2-bg: va
-00059e40: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-00059e50: 6563 6f6e 6461 7279 2d62 6729 3b2d 2d72  econdary-bg);--r
-00059e60: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d32  io-local-level-2
-00059e70: 2d62 672d 7661 7269 616e 743a 2076 6172  -bg-variant: var
-00059e80: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
-00059e90: 636f 6e64 6172 792d 6267 2d76 6172 6961  condary-bg-varia
-00059ea0: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
-00059eb0: 6c65 7665 6c2d 322d 6267 2d61 6374 6976  level-2-bg-activ
-00059ec0: 653a 2076 6172 282d 2d72 696f 2d67 6c6f  e: var(--rio-glo
-00059ed0: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
-00059ee0: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
-00059ef0: 6f63 616c 2d6c 6576 656c 2d32 2d66 673a  ocal-level-2-fg:
-00059f00: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-00059f10: 6c2d 7365 636f 6e64 6172 792d 6667 293b  l-secondary-fg);
-00059f20: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-00059f30: 6c2d 332d 6267 3a20 7661 7228 2d2d 7269  l-3-bg: var(--ri
-00059f40: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
-00059f50: 2d62 6729 3b2d 2d72 696f 2d6c 6f63 616c  -bg);--rio-local
-00059f60: 2d6c 6576 656c 2d33 2d62 672d 7661 7269  -level-3-bg-vari
-00059f70: 616e 743a 2076 6172 282d 2d72 696f 2d67  ant: var(--rio-g
-00059f80: 6c6f 6261 6c2d 7072 696d 6172 792d 6267  lobal-primary-bg
-00059f90: 2d76 6172 6961 6e74 293b 2d2d 7269 6f2d  -variant);--rio-
-00059fa0: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
-00059fb0: 2d61 6374 6976 653a 2076 6172 282d 2d72  -active: var(--r
-00059fc0: 696f 2d67 6c6f 6261 6c2d 7072 696d 6172  io-global-primar
-00059fd0: 792d 6267 2d61 6374 6976 6529 3b2d 2d72  y-bg-active);--r
-00059fe0: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
-00059ff0: 2d66 673a 2076 6172 282d 2d72 696f 2d67  -fg: var(--rio-g
-0005a000: 6c6f 6261 6c2d 7072 696d 6172 792d 6667  lobal-primary-fg
-0005a010: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
-0005a020: 6164 696e 6731 2d63 6f6c 6f72 3a20 7661  ading1-color: va
-0005a030: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  r(--rio-local-fg
-0005a040: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
-0005a050: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
-0005a060: 643a 2022 6e6f 6e65 223b 2d2d 7269 6f2d  d: "none";--rio-
-0005a070: 6c6f 6361 6c2d 6865 6164 696e 6731 2d62  local-heading1-b
-0005a080: 6163 6b67 726f 756e 642d 636c 6970 3a20  ackground-clip: 
-0005a090: 2262 6f72 6465 722d 626f 7822 3b2d 2d72  "border-box";--r
-0005a0a0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-0005a0b0: 312d 6669 6c6c 2d63 6f6c 6f72 3a20 2274  1-fill-color: "t
-0005a0c0: 7261 6e73 7061 7265 6e74 223b 2d2d 7269  ransparent";--ri
-0005a0d0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
-0005a0e0: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
-0005a0f0: 6f2d 6c6f 6361 6c2d 6667 293b 2d2d 7269  o-local-fg);--ri
-0005a100: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
-0005a110: 2d62 6163 6b67 726f 756e 643a 2022 6e6f  -background: "no
-0005a120: 6e65 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ne";--rio-local-
-0005a130: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
-0005a140: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
-0005a150: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
-0005a160: 616c 2d68 6561 6469 6e67 322d 6669 6c6c  al-heading2-fill
-0005a170: 2d63 6f6c 6f72 3a20 2274 7261 6e73 7061  -color: "transpa
-0005a180: 7265 6e74 223b 2d2d 7269 6f2d 6c6f 6361  rent";--rio-loca
-0005a190: 6c2d 6865 6164 696e 6733 2d63 6f6c 6f72  l-heading3-color
-0005a1a0: 3a20 7661 7228 2d2d 7269 6f2d 6c6f 6361  : var(--rio-loca
-0005a1b0: 6c2d 6667 293b 2d2d 7269 6f2d 6c6f 6361  l-fg);--rio-loca
-0005a1c0: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
-0005a1d0: 726f 756e 643a 2022 6e6f 6e65 223b 2d2d  round: "none";--
-0005a1e0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-0005a1f0: 6733 2d62 6163 6b67 726f 756e 642d 636c  g3-background-cl
-0005a200: 6970 3a20 2262 6f72 6465 722d 626f 7822  ip: "border-box"
-0005a210: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
-0005a220: 6469 6e67 332d 6669 6c6c 2d63 6f6c 6f72  ding3-fill-color
-0005a230: 3a20 2274 7261 6e73 7061 7265 6e74 223b  : "transparent";
-0005a240: 2d2d 7269 6f2d 6c6f 6361 6c2d 7465 7874  --rio-local-text
-0005a250: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
-0005a260: 6f2d 6c6f 6361 6c2d 6667 293b 2d2d 7269  o-local-fg);--ri
-0005a270: 6f2d 6c6f 6361 6c2d 7465 7874 2d62 6163  o-local-text-bac
-0005a280: 6b67 726f 756e 643a 2022 6e6f 6e65 223b  kground: "none";
-0005a290: 2d2d 7269 6f2d 6c6f 6361 6c2d 7465 7874  --rio-local-text
-0005a2a0: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
-0005a2b0: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
-0005a2c0: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
-0005a2d0: 6669 6c6c 2d63 6f6c 6f72 3a20 2274 7261  fill-color: "tra
-0005a2e0: 6e73 7061 7265 6e74 223b 636f 6c6f 723a  nsparent";color:
-0005a2f0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005a300: 6667 297d 2e72 696f 2d73 7769 7463 6865  fg)}.rio-switche
-0005a310: 726f 6f2d 7761 726e 696e 677b 2d2d 7269  roo-warning{--ri
-0005a320: 6f2d 6c6f 6361 6c2d 6267 3a20 7661 7228  o-local-bg: var(
-0005a330: 2d2d 7269 6f2d 676c 6f62 616c 2d77 6172  --rio-global-war
-0005a340: 6e69 6e67 2d62 6729 3b2d 2d72 696f 2d6c  ning-bg);--rio-l
-0005a350: 6f63 616c 2d62 672d 7661 7269 616e 743a  ocal-bg-variant:
-0005a360: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-0005a370: 6c2d 7761 726e 696e 672d 6267 2d76 6172  l-warning-bg-var
-0005a380: 6961 6e74 293b 2d2d 7269 6f2d 6c6f 6361  iant);--rio-loca
-0005a390: 6c2d 6267 2d61 6374 6976 653a 2076 6172  l-bg-active: var
-0005a3a0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7761  (--rio-global-wa
-0005a3b0: 726e 696e 672d 6267 2d61 6374 6976 6529  rning-bg-active)
-0005a3c0: 3b2d 2d72 696f 2d6c 6f63 616c 2d66 673a  ;--rio-local-fg:
-0005a3d0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-0005a3e0: 6c2d 7761 726e 696e 672d 6667 293b 2d2d  l-warning-fg);--
-0005a3f0: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-0005a400: 322d 6267 3a20 7661 7228 2d2d 7269 6f2d  2-bg: var(--rio-
-0005a410: 676c 6f62 616c 2d73 6563 6f6e 6461 7279  global-secondary
-0005a420: 2d62 6729 3b2d 2d72 696f 2d6c 6f63 616c  -bg);--rio-local
-0005a430: 2d6c 6576 656c 2d32 2d62 672d 7661 7269  -level-2-bg-vari
-0005a440: 616e 743a 2076 6172 282d 2d72 696f 2d67  ant: var(--rio-g
-0005a450: 6c6f 6261 6c2d 7365 636f 6e64 6172 792d  lobal-secondary-
-0005a460: 6267 2d76 6172 6961 6e74 293b 2d2d 7269  bg-variant);--ri
-0005a470: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 322d  o-local-level-2-
-0005a480: 6267 2d61 6374 6976 653a 2076 6172 282d  bg-active: var(-
-0005a490: 2d72 696f 2d67 6c6f 6261 6c2d 7365 636f  -rio-global-seco
-0005a4a0: 6e64 6172 792d 6267 2d61 6374 6976 6529  ndary-bg-active)
-0005a4b0: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
-0005a4c0: 656c 2d32 2d66 673a 2076 6172 282d 2d72  el-2-fg: var(--r
-0005a4d0: 696f 2d67 6c6f 6261 6c2d 7365 636f 6e64  io-global-second
-0005a4e0: 6172 792d 6667 293b 2d2d 7269 6f2d 6c6f  ary-fg);--rio-lo
-0005a4f0: 6361 6c2d 6c65 7665 6c2d 332d 6267 3a20  cal-level-3-bg: 
+00059820: 6172 792d 6267 293b 2d2d 7269 6f2d 6c6f  ary-bg);--rio-lo
+00059830: 6361 6c2d 6267 2d76 6172 6961 6e74 3a20  cal-bg-variant: 
+00059840: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00059850: 2d73 6563 6f6e 6461 7279 2d62 672d 7661  -secondary-bg-va
+00059860: 7269 616e 7429 3b2d 2d72 696f 2d6c 6f63  riant);--rio-loc
+00059870: 616c 2d62 672d 6163 7469 7665 3a20 7661  al-bg-active: va
+00059880: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
+00059890: 6563 6f6e 6461 7279 2d62 672d 6163 7469  econdary-bg-acti
+000598a0: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
+000598b0: 6667 3a20 7661 7228 2d2d 7269 6f2d 676c  fg: var(--rio-gl
+000598c0: 6f62 616c 2d73 6563 6f6e 6461 7279 2d66  obal-secondary-f
+000598d0: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
+000598e0: 6576 656c 2d32 2d62 673a 2076 6172 282d  evel-2-bg: var(-
+000598f0: 2d72 696f 2d67 6c6f 6261 6c2d 7072 696d  -rio-global-prim
+00059900: 6172 792d 6267 293b 2d2d 7269 6f2d 6c6f  ary-bg);--rio-lo
+00059910: 6361 6c2d 6c65 7665 6c2d 322d 6267 2d76  cal-level-2-bg-v
+00059920: 6172 6961 6e74 3a20 7661 7228 2d2d 7269  ariant: var(--ri
+00059930: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
+00059940: 2d62 672d 7661 7269 616e 7429 3b2d 2d72  -bg-variant);--r
+00059950: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d32  io-local-level-2
+00059960: 2d62 672d 6163 7469 7665 3a20 7661 7228  -bg-active: var(
+00059970: 2d2d 7269 6f2d 676c 6f62 616c 2d70 7269  --rio-global-pri
+00059980: 6d61 7279 2d62 672d 6163 7469 7665 293b  mary-bg-active);
+00059990: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+000599a0: 6c2d 322d 6667 3a20 7661 7228 2d2d 7269  l-2-fg: var(--ri
+000599b0: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
+000599c0: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
+000599d0: 2d6c 6576 656c 2d33 2d62 673a 2076 6172  -level-3-bg: var
+000599e0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
+000599f0: 636f 6e64 6172 792d 6267 293b 2d2d 7269  condary-bg);--ri
+00059a00: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 332d  o-local-level-3-
+00059a10: 6267 2d76 6172 6961 6e74 3a20 7661 7228  bg-variant: var(
+00059a20: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
+00059a30: 6f6e 6461 7279 2d62 672d 7661 7269 616e  ondary-bg-varian
+00059a40: 7429 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  t);--rio-local-l
+00059a50: 6576 656c 2d33 2d62 672d 6163 7469 7665  evel-3-bg-active
+00059a60: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00059a70: 616c 2d73 6563 6f6e 6461 7279 2d62 672d  al-secondary-bg-
+00059a80: 6163 7469 7665 293b 2d2d 7269 6f2d 6c6f  active);--rio-lo
+00059a90: 6361 6c2d 6c65 7665 6c2d 332d 6667 3a20  cal-level-3-fg: 
+00059aa0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00059ab0: 2d73 6563 6f6e 6461 7279 2d66 6729 3b2d  -secondary-fg);-
+00059ac0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+00059ad0: 6e67 312d 636f 6c6f 723a 2076 6172 282d  ng1-color: var(-
+00059ae0: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
+00059af0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+00059b00: 6e67 312d 6261 636b 6772 6f75 6e64 3a20  ng1-background: 
+00059b10: 226e 6f6e 6522 3b2d 2d72 696f 2d6c 6f63  "none";--rio-loc
+00059b20: 616c 2d68 6561 6469 6e67 312d 6261 636b  al-heading1-back
+00059b30: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
+00059b40: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
+00059b50: 6c6f 6361 6c2d 6865 6164 696e 6731 2d66  local-heading1-f
+00059b60: 696c 6c2d 636f 6c6f 723a 2022 7472 616e  ill-color: "tran
+00059b70: 7370 6172 656e 7422 3b2d 2d72 696f 2d6c  sparent";--rio-l
+00059b80: 6f63 616c 2d68 6561 6469 6e67 322d 636f  ocal-heading2-co
+00059b90: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+00059ba0: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+00059bb0: 6f63 616c 2d68 6561 6469 6e67 322d 6261  ocal-heading2-ba
+00059bc0: 636b 6772 6f75 6e64 3a20 226e 6f6e 6522  ckground: "none"
+00059bd0: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+00059be0: 6469 6e67 322d 6261 636b 6772 6f75 6e64  ding2-background
+00059bf0: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
+00059c00: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
+00059c10: 6865 6164 696e 6732 2d66 696c 6c2d 636f  heading2-fill-co
+00059c20: 6c6f 723a 2022 7472 616e 7370 6172 656e  lor: "transparen
+00059c30: 7422 3b2d 2d72 696f 2d6c 6f63 616c 2d68  t";--rio-local-h
+00059c40: 6561 6469 6e67 332d 636f 6c6f 723a 2076  eading3-color: v
+00059c50: 6172 282d 2d72 696f 2d6c 6f63 616c 2d66  ar(--rio-local-f
+00059c60: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d68  g);--rio-local-h
+00059c70: 6561 6469 6e67 332d 6261 636b 6772 6f75  eading3-backgrou
+00059c80: 6e64 3a20 226e 6f6e 6522 3b2d 2d72 696f  nd: "none";--rio
+00059c90: 2d6c 6f63 616c 2d68 6561 6469 6e67 332d  -local-heading3-
+00059ca0: 6261 636b 6772 6f75 6e64 2d63 6c69 703a  background-clip:
+00059cb0: 2022 626f 7264 6572 2d62 6f78 223b 2d2d   "border-box";--
+00059cc0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+00059cd0: 6733 2d66 696c 6c2d 636f 6c6f 723a 2022  g3-fill-color: "
+00059ce0: 7472 616e 7370 6172 656e 7422 3b2d 2d72  transparent";--r
+00059cf0: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
+00059d00: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+00059d10: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+00059d20: 6f63 616c 2d74 6578 742d 6261 636b 6772  ocal-text-backgr
+00059d30: 6f75 6e64 3a20 226e 6f6e 6522 3b2d 2d72  ound: "none";--r
+00059d40: 696f 2d6c 6f63 616c 2d74 6578 742d 6261  io-local-text-ba
+00059d50: 636b 6772 6f75 6e64 2d63 6c69 703a 2022  ckground-clip: "
+00059d60: 626f 7264 6572 2d62 6f78 223b 2d2d 7269  border-box";--ri
+00059d70: 6f2d 6c6f 6361 6c2d 7465 7874 2d66 696c  o-local-text-fil
+00059d80: 6c2d 636f 6c6f 723a 2022 7472 616e 7370  l-color: "transp
+00059d90: 6172 656e 7422 3b63 6f6c 6f72 3a76 6172  arent";color:var
+00059da0: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+00059db0: 7d2e 7269 6f2d 7377 6974 6368 6572 6f6f  }.rio-switcheroo
+00059dc0: 2d73 7563 6365 7373 7b2d 2d72 696f 2d6c  -success{--rio-l
+00059dd0: 6f63 616c 2d62 673a 2076 6172 282d 2d72  ocal-bg: var(--r
+00059de0: 696f 2d67 6c6f 6261 6c2d 7375 6363 6573  io-global-succes
+00059df0: 732d 6267 293b 2d2d 7269 6f2d 6c6f 6361  s-bg);--rio-loca
+00059e00: 6c2d 6267 2d76 6172 6961 6e74 3a20 7661  l-bg-variant: va
+00059e10: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
+00059e20: 7563 6365 7373 2d62 672d 7661 7269 616e  uccess-bg-varian
+00059e30: 7429 3b2d 2d72 696f 2d6c 6f63 616c 2d62  t);--rio-local-b
+00059e40: 672d 6163 7469 7665 3a20 7661 7228 2d2d  g-active: var(--
+00059e50: 7269 6f2d 676c 6f62 616c 2d73 7563 6365  rio-global-succe
+00059e60: 7373 2d62 672d 6163 7469 7665 293b 2d2d  ss-bg-active);--
+00059e70: 7269 6f2d 6c6f 6361 6c2d 6667 3a20 7661  rio-local-fg: va
+00059e80: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
+00059e90: 7563 6365 7373 2d66 6729 3b2d 2d72 696f  uccess-fg);--rio
+00059ea0: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
+00059eb0: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
+00059ec0: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
+00059ed0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+00059ee0: 7665 6c2d 322d 6267 2d76 6172 6961 6e74  vel-2-bg-variant
+00059ef0: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+00059f00: 616c 2d73 6563 6f6e 6461 7279 2d62 672d  al-secondary-bg-
+00059f10: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
+00059f20: 6f63 616c 2d6c 6576 656c 2d32 2d62 672d  ocal-level-2-bg-
+00059f30: 6163 7469 7665 3a20 7661 7228 2d2d 7269  active: var(--ri
+00059f40: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
+00059f50: 7279 2d62 672d 6163 7469 7665 293b 2d2d  ry-bg-active);--
+00059f60: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
+00059f70: 322d 6667 3a20 7661 7228 2d2d 7269 6f2d  2-fg: var(--rio-
+00059f80: 676c 6f62 616c 2d73 6563 6f6e 6461 7279  global-secondary
+00059f90: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
+00059fa0: 2d6c 6576 656c 2d33 2d62 673a 2076 6172  -level-3-bg: var
+00059fb0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7072  (--rio-global-pr
+00059fc0: 696d 6172 792d 6267 293b 2d2d 7269 6f2d  imary-bg);--rio-
+00059fd0: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
+00059fe0: 2d76 6172 6961 6e74 3a20 7661 7228 2d2d  -variant: var(--
+00059ff0: 7269 6f2d 676c 6f62 616c 2d70 7269 6d61  rio-global-prima
+0005a000: 7279 2d62 672d 7661 7269 616e 7429 3b2d  ry-bg-variant);-
+0005a010: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
+0005a020: 2d33 2d62 672d 6163 7469 7665 3a20 7661  -3-bg-active: va
+0005a030: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d70  r(--rio-global-p
+0005a040: 7269 6d61 7279 2d62 672d 6163 7469 7665  rimary-bg-active
+0005a050: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+0005a060: 7665 6c2d 332d 6667 3a20 7661 7228 2d2d  vel-3-fg: var(--
+0005a070: 7269 6f2d 676c 6f62 616c 2d70 7269 6d61  rio-global-prima
+0005a080: 7279 2d66 6729 3b2d 2d72 696f 2d6c 6f63  ry-fg);--rio-loc
+0005a090: 616c 2d68 6561 6469 6e67 312d 636f 6c6f  al-heading1-colo
+0005a0a0: 723a 2076 6172 282d 2d72 696f 2d6c 6f63  r: var(--rio-loc
+0005a0b0: 616c 2d66 6729 3b2d 2d72 696f 2d6c 6f63  al-fg);--rio-loc
+0005a0c0: 616c 2d68 6561 6469 6e67 312d 6261 636b  al-heading1-back
+0005a0d0: 6772 6f75 6e64 3a20 226e 6f6e 6522 3b2d  ground: "none";-
+0005a0e0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+0005a0f0: 6e67 312d 6261 636b 6772 6f75 6e64 2d63  ng1-background-c
+0005a100: 6c69 703a 2022 626f 7264 6572 2d62 6f78  lip: "border-box
+0005a110: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
+0005a120: 6164 696e 6731 2d66 696c 6c2d 636f 6c6f  ading1-fill-colo
+0005a130: 723a 2022 7472 616e 7370 6172 656e 7422  r: "transparent"
+0005a140: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+0005a150: 6469 6e67 322d 636f 6c6f 723a 2076 6172  ding2-color: var
+0005a160: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+0005a170: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+0005a180: 6469 6e67 322d 6261 636b 6772 6f75 6e64  ding2-background
+0005a190: 3a20 226e 6f6e 6522 3b2d 2d72 696f 2d6c  : "none";--rio-l
+0005a1a0: 6f63 616c 2d68 6561 6469 6e67 322d 6261  ocal-heading2-ba
+0005a1b0: 636b 6772 6f75 6e64 2d63 6c69 703a 2022  ckground-clip: "
+0005a1c0: 626f 7264 6572 2d62 6f78 223b 2d2d 7269  border-box";--ri
+0005a1d0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
+0005a1e0: 2d66 696c 6c2d 636f 6c6f 723a 2022 7472  -fill-color: "tr
+0005a1f0: 616e 7370 6172 656e 7422 3b2d 2d72 696f  ansparent";--rio
+0005a200: 2d6c 6f63 616c 2d68 6561 6469 6e67 332d  -local-heading3-
+0005a210: 636f 6c6f 723a 2076 6172 282d 2d72 696f  color: var(--rio
+0005a220: 2d6c 6f63 616c 2d66 6729 3b2d 2d72 696f  -local-fg);--rio
+0005a230: 2d6c 6f63 616c 2d68 6561 6469 6e67 332d  -local-heading3-
+0005a240: 6261 636b 6772 6f75 6e64 3a20 226e 6f6e  background: "non
+0005a250: 6522 3b2d 2d72 696f 2d6c 6f63 616c 2d68  e";--rio-local-h
+0005a260: 6561 6469 6e67 332d 6261 636b 6772 6f75  eading3-backgrou
+0005a270: 6e64 2d63 6c69 703a 2022 626f 7264 6572  nd-clip: "border
+0005a280: 2d62 6f78 223b 2d2d 7269 6f2d 6c6f 6361  -box";--rio-loca
+0005a290: 6c2d 6865 6164 696e 6733 2d66 696c 6c2d  l-heading3-fill-
+0005a2a0: 636f 6c6f 723a 2022 7472 616e 7370 6172  color: "transpar
+0005a2b0: 656e 7422 3b2d 2d72 696f 2d6c 6f63 616c  ent";--rio-local
+0005a2c0: 2d74 6578 742d 636f 6c6f 723a 2076 6172  -text-color: var
+0005a2d0: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+0005a2e0: 3b2d 2d72 696f 2d6c 6f63 616c 2d74 6578  ;--rio-local-tex
+0005a2f0: 742d 6261 636b 6772 6f75 6e64 3a20 226e  t-background: "n
+0005a300: 6f6e 6522 3b2d 2d72 696f 2d6c 6f63 616c  one";--rio-local
+0005a310: 2d74 6578 742d 6261 636b 6772 6f75 6e64  -text-background
+0005a320: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
+0005a330: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
+0005a340: 7465 7874 2d66 696c 6c2d 636f 6c6f 723a  text-fill-color:
+0005a350: 2022 7472 616e 7370 6172 656e 7422 3b63   "transparent";c
+0005a360: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
+0005a370: 6f63 616c 2d66 6729 7d2e 7269 6f2d 7377  ocal-fg)}.rio-sw
+0005a380: 6974 6368 6572 6f6f 2d77 6172 6e69 6e67  itcheroo-warning
+0005a390: 7b2d 2d72 696f 2d6c 6f63 616c 2d62 673a  {--rio-local-bg:
+0005a3a0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+0005a3b0: 6c2d 7761 726e 696e 672d 6267 293b 2d2d  l-warning-bg);--
+0005a3c0: 7269 6f2d 6c6f 6361 6c2d 6267 2d76 6172  rio-local-bg-var
+0005a3d0: 6961 6e74 3a20 7661 7228 2d2d 7269 6f2d  iant: var(--rio-
+0005a3e0: 676c 6f62 616c 2d77 6172 6e69 6e67 2d62  global-warning-b
+0005a3f0: 672d 7661 7269 616e 7429 3b2d 2d72 696f  g-variant);--rio
+0005a400: 2d6c 6f63 616c 2d62 672d 6163 7469 7665  -local-bg-active
+0005a410: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+0005a420: 616c 2d77 6172 6e69 6e67 2d62 672d 6163  al-warning-bg-ac
+0005a430: 7469 7665 293b 2d2d 7269 6f2d 6c6f 6361  tive);--rio-loca
+0005a440: 6c2d 6667 3a20 7661 7228 2d2d 7269 6f2d  l-fg: var(--rio-
+0005a450: 676c 6f62 616c 2d77 6172 6e69 6e67 2d66  global-warning-f
+0005a460: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
+0005a470: 6576 656c 2d32 2d62 673a 2076 6172 282d  evel-2-bg: var(-
+0005a480: 2d72 696f 2d67 6c6f 6261 6c2d 7365 636f  -rio-global-seco
+0005a490: 6e64 6172 792d 6267 293b 2d2d 7269 6f2d  ndary-bg);--rio-
+0005a4a0: 6c6f 6361 6c2d 6c65 7665 6c2d 322d 6267  local-level-2-bg
+0005a4b0: 2d76 6172 6961 6e74 3a20 7661 7228 2d2d  -variant: var(--
+0005a4c0: 7269 6f2d 676c 6f62 616c 2d73 6563 6f6e  rio-global-secon
+0005a4d0: 6461 7279 2d62 672d 7661 7269 616e 7429  dary-bg-variant)
+0005a4e0: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
+0005a4f0: 656c 2d32 2d62 672d 6163 7469 7665 3a20  el-2-bg-active: 
 0005a500: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005a510: 2d70 7269 6d61 7279 2d62 6729 3b2d 2d72  -primary-bg);--r
-0005a520: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
-0005a530: 2d62 672d 7661 7269 616e 743a 2076 6172  -bg-variant: var
-0005a540: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7072  (--rio-global-pr
-0005a550: 696d 6172 792d 6267 2d76 6172 6961 6e74  imary-bg-variant
-0005a560: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
-0005a570: 7665 6c2d 332d 6267 2d61 6374 6976 653a  vel-3-bg-active:
-0005a580: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
-0005a590: 6c2d 7072 696d 6172 792d 6267 2d61 6374  l-primary-bg-act
-0005a5a0: 6976 6529 3b2d 2d72 696f 2d6c 6f63 616c  ive);--rio-local
-0005a5b0: 2d6c 6576 656c 2d33 2d66 673a 2076 6172  -level-3-fg: var
-0005a5c0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7072  (--rio-global-pr
-0005a5d0: 696d 6172 792d 6667 293b 2d2d 7269 6f2d  imary-fg);--rio-
-0005a5e0: 6c6f 6361 6c2d 6865 6164 696e 6731 2d63  local-heading1-c
-0005a5f0: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
-0005a600: 6c6f 6361 6c2d 6667 293b 2d2d 7269 6f2d  local-fg);--rio-
-0005a610: 6c6f 6361 6c2d 6865 6164 696e 6731 2d62  local-heading1-b
-0005a620: 6163 6b67 726f 756e 643a 2022 6e6f 6e65  ackground: "none
-0005a630: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
-0005a640: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
-0005a650: 642d 636c 6970 3a20 2262 6f72 6465 722d  d-clip: "border-
-0005a660: 626f 7822 3b2d 2d72 696f 2d6c 6f63 616c  box";--rio-local
-0005a670: 2d68 6561 6469 6e67 312d 6669 6c6c 2d63  -heading1-fill-c
-0005a680: 6f6c 6f72 3a20 2274 7261 6e73 7061 7265  olor: "transpare
-0005a690: 6e74 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt";--rio-local-
-0005a6a0: 6865 6164 696e 6732 2d63 6f6c 6f72 3a20  heading2-color: 
-0005a6b0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005a6c0: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-0005a6d0: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
-0005a6e0: 756e 643a 2022 6e6f 6e65 223b 2d2d 7269  und: "none";--ri
-0005a6f0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
-0005a700: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
-0005a710: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
-0005a720: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-0005a730: 6e67 322d 6669 6c6c 2d63 6f6c 6f72 3a20  ng2-fill-color: 
-0005a740: 2274 7261 6e73 7061 7265 6e74 223b 2d2d  "transparent";--
-0005a750: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-0005a760: 6733 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g3-color: var(--
-0005a770: 7269 6f2d 6c6f 6361 6c2d 6667 293b 2d2d  rio-local-fg);--
-0005a780: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-0005a790: 6733 2d62 6163 6b67 726f 756e 643a 2022  g3-background: "
-0005a7a0: 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f 6361  none";--rio-loca
-0005a7b0: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
-0005a7c0: 726f 756e 642d 636c 6970 3a20 2262 6f72  round-clip: "bor
-0005a7d0: 6465 722d 626f 7822 3b2d 2d72 696f 2d6c  der-box";--rio-l
-0005a7e0: 6f63 616c 2d68 6561 6469 6e67 332d 6669  ocal-heading3-fi
-0005a7f0: 6c6c 2d63 6f6c 6f72 3a20 2274 7261 6e73  ll-color: "trans
-0005a800: 7061 7265 6e74 223b 2d2d 7269 6f2d 6c6f  parent";--rio-lo
-0005a810: 6361 6c2d 7465 7874 2d63 6f6c 6f72 3a20  cal-text-color: 
-0005a820: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005a830: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-0005a840: 7465 7874 2d62 6163 6b67 726f 756e 643a  text-background:
-0005a850: 2022 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f   "none";--rio-lo
-0005a860: 6361 6c2d 7465 7874 2d62 6163 6b67 726f  cal-text-backgro
-0005a870: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
-0005a880: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
-0005a890: 616c 2d74 6578 742d 6669 6c6c 2d63 6f6c  al-text-fill-col
-0005a8a0: 6f72 3a20 2274 7261 6e73 7061 7265 6e74  or: "transparent
-0005a8b0: 223b 636f 6c6f 723a 7661 7228 2d2d 7269  ";color:var(--ri
-0005a8c0: 6f2d 6c6f 6361 6c2d 6667 297d 2e72 696f  o-local-fg)}.rio
-0005a8d0: 2d73 7769 7463 6865 726f 6f2d 6461 6e67  -switcheroo-dang
-0005a8e0: 6572 7b2d 2d72 696f 2d6c 6f63 616c 2d62  er{--rio-local-b
-0005a8f0: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
-0005a900: 6261 6c2d 6461 6e67 6572 2d62 6729 3b2d  bal-danger-bg);-
-0005a910: 2d72 696f 2d6c 6f63 616c 2d62 672d 7661  -rio-local-bg-va
-0005a920: 7269 616e 743a 2076 6172 282d 2d72 696f  riant: var(--rio
-0005a930: 2d67 6c6f 6261 6c2d 6461 6e67 6572 2d62  -global-danger-b
-0005a940: 672d 7661 7269 616e 7429 3b2d 2d72 696f  g-variant);--rio
-0005a950: 2d6c 6f63 616c 2d62 672d 6163 7469 7665  -local-bg-active
-0005a960: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
-0005a970: 616c 2d64 616e 6765 722d 6267 2d61 6374  al-danger-bg-act
-0005a980: 6976 6529 3b2d 2d72 696f 2d6c 6f63 616c  ive);--rio-local
-0005a990: 2d66 673a 2076 6172 282d 2d72 696f 2d67  -fg: var(--rio-g
-0005a9a0: 6c6f 6261 6c2d 6461 6e67 6572 2d66 6729  lobal-danger-fg)
-0005a9b0: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
-0005a9c0: 656c 2d32 2d62 673a 2076 6172 282d 2d72  el-2-bg: var(--r
-0005a9d0: 696f 2d67 6c6f 6261 6c2d 7365 636f 6e64  io-global-second
-0005a9e0: 6172 792d 6267 293b 2d2d 7269 6f2d 6c6f  ary-bg);--rio-lo
-0005a9f0: 6361 6c2d 6c65 7665 6c2d 322d 6267 2d76  cal-level-2-bg-v
-0005aa00: 6172 6961 6e74 3a20 7661 7228 2d2d 7269  ariant: var(--ri
-0005aa10: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
-0005aa20: 7279 2d62 672d 7661 7269 616e 7429 3b2d  ry-bg-variant);-
-0005aa30: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
-0005aa40: 2d32 2d62 672d 6163 7469 7665 3a20 7661  -2-bg-active: va
-0005aa50: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-0005aa60: 6563 6f6e 6461 7279 2d62 672d 6163 7469  econdary-bg-acti
-0005aa70: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
-0005aa80: 6c65 7665 6c2d 322d 6667 3a20 7661 7228  level-2-fg: var(
-0005aa90: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
-0005aaa0: 6f6e 6461 7279 2d66 6729 3b2d 2d72 696f  ondary-fg);--rio
-0005aab0: 2d6c 6f63 616c 2d6c 6576 656c 2d33 2d62  -local-level-3-b
-0005aac0: 673a 2076 6172 282d 2d72 696f 2d67 6c6f  g: var(--rio-glo
-0005aad0: 6261 6c2d 7072 696d 6172 792d 6267 293b  bal-primary-bg);
-0005aae0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005aaf0: 6c2d 332d 6267 2d76 6172 6961 6e74 3a20  l-3-bg-variant: 
-0005ab00: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005ab10: 2d70 7269 6d61 7279 2d62 672d 7661 7269  -primary-bg-vari
-0005ab20: 616e 7429 3b2d 2d72 696f 2d6c 6f63 616c  ant);--rio-local
-0005ab30: 2d6c 6576 656c 2d33 2d62 672d 6163 7469  -level-3-bg-acti
-0005ab40: 7665 3a20 7661 7228 2d2d 7269 6f2d 676c  ve: var(--rio-gl
-0005ab50: 6f62 616c 2d70 7269 6d61 7279 2d62 672d  obal-primary-bg-
-0005ab60: 6163 7469 7665 293b 2d2d 7269 6f2d 6c6f  active);--rio-lo
-0005ab70: 6361 6c2d 6c65 7665 6c2d 332d 6667 3a20  cal-level-3-fg: 
-0005ab80: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005ab90: 2d70 7269 6d61 7279 2d66 6729 3b2d 2d72  -primary-fg);--r
-0005aba0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-0005abb0: 312d 636f 6c6f 723a 2076 6172 282d 2d72  1-color: var(--r
-0005abc0: 696f 2d6c 6f63 616c 2d66 6729 3b2d 2d72  io-local-fg);--r
-0005abd0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-0005abe0: 312d 6261 636b 6772 6f75 6e64 3a20 226e  1-background: "n
-0005abf0: 6f6e 6522 3b2d 2d72 696f 2d6c 6f63 616c  one";--rio-local
-0005ac00: 2d68 6561 6469 6e67 312d 6261 636b 6772  -heading1-backgr
-0005ac10: 6f75 6e64 2d63 6c69 703a 2022 626f 7264  ound-clip: "bord
-0005ac20: 6572 2d62 6f78 223b 2d2d 7269 6f2d 6c6f  er-box";--rio-lo
-0005ac30: 6361 6c2d 6865 6164 696e 6731 2d66 696c  cal-heading1-fil
-0005ac40: 6c2d 636f 6c6f 723a 2022 7472 616e 7370  l-color: "transp
-0005ac50: 6172 656e 7422 3b2d 2d72 696f 2d6c 6f63  arent";--rio-loc
-0005ac60: 616c 2d68 6561 6469 6e67 322d 636f 6c6f  al-heading2-colo
-0005ac70: 723a 2076 6172 282d 2d72 696f 2d6c 6f63  r: var(--rio-loc
-0005ac80: 616c 2d66 6729 3b2d 2d72 696f 2d6c 6f63  al-fg);--rio-loc
-0005ac90: 616c 2d68 6561 6469 6e67 322d 6261 636b  al-heading2-back
-0005aca0: 6772 6f75 6e64 3a20 226e 6f6e 6522 3b2d  ground: "none";-
-0005acb0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-0005acc0: 6e67 322d 6261 636b 6772 6f75 6e64 2d63  ng2-background-c
-0005acd0: 6c69 703a 2022 626f 7264 6572 2d62 6f78  lip: "border-box
-0005ace0: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
-0005acf0: 6164 696e 6732 2d66 696c 6c2d 636f 6c6f  ading2-fill-colo
-0005ad00: 723a 2022 7472 616e 7370 6172 656e 7422  r: "transparent"
-0005ad10: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
-0005ad20: 6469 6e67 332d 636f 6c6f 723a 2076 6172  ding3-color: var
-0005ad30: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
-0005ad40: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
-0005ad50: 6469 6e67 332d 6261 636b 6772 6f75 6e64  ding3-background
-0005ad60: 3a20 226e 6f6e 6522 3b2d 2d72 696f 2d6c  : "none";--rio-l
-0005ad70: 6f63 616c 2d68 6561 6469 6e67 332d 6261  ocal-heading3-ba
-0005ad80: 636b 6772 6f75 6e64 2d63 6c69 703a 2022  ckground-clip: "
-0005ad90: 626f 7264 6572 2d62 6f78 223b 2d2d 7269  border-box";--ri
-0005ada0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6733  o-local-heading3
-0005adb0: 2d66 696c 6c2d 636f 6c6f 723a 2022 7472  -fill-color: "tr
-0005adc0: 616e 7370 6172 656e 7422 3b2d 2d72 696f  ansparent";--rio
-0005add0: 2d6c 6f63 616c 2d74 6578 742d 636f 6c6f  -local-text-colo
-0005ade0: 723a 2076 6172 282d 2d72 696f 2d6c 6f63  r: var(--rio-loc
-0005adf0: 616c 2d66 6729 3b2d 2d72 696f 2d6c 6f63  al-fg);--rio-loc
-0005ae00: 616c 2d74 6578 742d 6261 636b 6772 6f75  al-text-backgrou
-0005ae10: 6e64 3a20 226e 6f6e 6522 3b2d 2d72 696f  nd: "none";--rio
-0005ae20: 2d6c 6f63 616c 2d74 6578 742d 6261 636b  -local-text-back
-0005ae30: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
-0005ae40: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
-0005ae50: 6c6f 6361 6c2d 7465 7874 2d66 696c 6c2d  local-text-fill-
-0005ae60: 636f 6c6f 723a 2022 7472 616e 7370 6172  color: "transpar
-0005ae70: 656e 7422 3b63 6f6c 6f72 3a76 6172 282d  ent";color:var(-
-0005ae80: 2d72 696f 2d6c 6f63 616c 2d66 6729 7d2e  -rio-local-fg)}.
-0005ae90: 7269 6f2d 7377 6974 6368 6572 6f6f 2d64  rio-switcheroo-d
-0005aea0: 6973 6162 6c65 647b 2d2d 7269 6f2d 6c6f  isabled{--rio-lo
-0005aeb0: 6361 6c2d 6267 3a20 7661 7228 2d2d 7269  cal-bg: var(--ri
-0005aec0: 6f2d 676c 6f62 616c 2d64 6973 6162 6c65  o-global-disable
-0005aed0: 642d 6267 293b 2d2d 7269 6f2d 6c6f 6361  d-bg);--rio-loca
-0005aee0: 6c2d 6267 2d76 6172 6961 6e74 3a20 7661  l-bg-variant: va
-0005aef0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d64  r(--rio-global-d
-0005af00: 6973 6162 6c65 642d 6267 2d76 6172 6961  isabled-bg-varia
-0005af10: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
-0005af20: 6267 2d61 6374 6976 653a 2076 6172 282d  bg-active: var(-
-0005af30: 2d72 696f 2d67 6c6f 6261 6c2d 6469 7361  -rio-global-disa
-0005af40: 626c 6564 2d62 672d 6163 7469 7665 293b  bled-bg-active);
-0005af50: 2d2d 7269 6f2d 6c6f 6361 6c2d 6667 3a20  --rio-local-fg: 
-0005af60: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005af70: 2d64 6973 6162 6c65 642d 6667 293b 2d2d  -disabled-fg);--
-0005af80: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-0005af90: 322d 6267 3a20 7661 7228 2d2d 7269 6f2d  2-bg: var(--rio-
-0005afa0: 676c 6f62 616c 2d64 6973 6162 6c65 642d  global-disabled-
-0005afb0: 6267 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  bg);--rio-local-
-0005afc0: 6c65 7665 6c2d 322d 6267 2d76 6172 6961  level-2-bg-varia
-0005afd0: 6e74 3a20 7661 7228 2d2d 7269 6f2d 676c  nt: var(--rio-gl
-0005afe0: 6f62 616c 2d64 6973 6162 6c65 642d 6267  obal-disabled-bg
-0005aff0: 2d76 6172 6961 6e74 293b 2d2d 7269 6f2d  -variant);--rio-
-0005b000: 6c6f 6361 6c2d 6c65 7665 6c2d 322d 6267  local-level-2-bg
-0005b010: 2d61 6374 6976 653a 2076 6172 282d 2d72  -active: var(--r
-0005b020: 696f 2d67 6c6f 6261 6c2d 6469 7361 626c  io-global-disabl
-0005b030: 6564 2d62 672d 6163 7469 7665 293b 2d2d  ed-bg-active);--
-0005b040: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-0005b050: 322d 6667 3a20 7661 7228 2d2d 7269 6f2d  2-fg: var(--rio-
-0005b060: 676c 6f62 616c 2d64 6973 6162 6c65 642d  global-disabled-
-0005b070: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-0005b080: 6c65 7665 6c2d 332d 6267 3a20 7661 7228  level-3-bg: var(
-0005b090: 2d2d 7269 6f2d 676c 6f62 616c 2d64 6973  --rio-global-dis
-0005b0a0: 6162 6c65 642d 6267 293b 2d2d 7269 6f2d  abled-bg);--rio-
-0005b0b0: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
-0005b0c0: 2d76 6172 6961 6e74 3a20 7661 7228 2d2d  -variant: var(--
-0005b0d0: 7269 6f2d 676c 6f62 616c 2d64 6973 6162  rio-global-disab
-0005b0e0: 6c65 642d 6267 2d76 6172 6961 6e74 293b  led-bg-variant);
-0005b0f0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005b100: 6c2d 332d 6267 2d61 6374 6976 653a 2076  l-3-bg-active: v
-0005b110: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-0005b120: 6469 7361 626c 6564 2d62 672d 6163 7469  disabled-bg-acti
-0005b130: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
-0005b140: 6c65 7665 6c2d 332d 6667 3a20 7661 7228  level-3-fg: var(
-0005b150: 2d2d 7269 6f2d 676c 6f62 616c 2d64 6973  --rio-global-dis
-0005b160: 6162 6c65 642d 6667 293b 2d2d 7269 6f2d  abled-fg);--rio-
-0005b170: 6c6f 6361 6c2d 6865 6164 696e 6731 2d63  local-heading1-c
-0005b180: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
-0005b190: 6c6f 6361 6c2d 6667 293b 2d2d 7269 6f2d  local-fg);--rio-
-0005b1a0: 6c6f 6361 6c2d 6865 6164 696e 6731 2d62  local-heading1-b
-0005b1b0: 6163 6b67 726f 756e 643a 2022 6e6f 6e65  ackground: "none
-0005b1c0: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
-0005b1d0: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
-0005b1e0: 642d 636c 6970 3a20 2262 6f72 6465 722d  d-clip: "border-
-0005b1f0: 626f 7822 3b2d 2d72 696f 2d6c 6f63 616c  box";--rio-local
-0005b200: 2d68 6561 6469 6e67 312d 6669 6c6c 2d63  -heading1-fill-c
-0005b210: 6f6c 6f72 3a20 2274 7261 6e73 7061 7265  olor: "transpare
-0005b220: 6e74 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt";--rio-local-
-0005b230: 6865 6164 696e 6732 2d63 6f6c 6f72 3a20  heading2-color: 
-0005b240: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005b250: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-0005b260: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
-0005b270: 756e 643a 2022 6e6f 6e65 223b 2d2d 7269  und: "none";--ri
-0005b280: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
-0005b290: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
-0005b2a0: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
-0005b2b0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-0005b2c0: 6e67 322d 6669 6c6c 2d63 6f6c 6f72 3a20  ng2-fill-color: 
-0005b2d0: 2274 7261 6e73 7061 7265 6e74 223b 2d2d  "transparent";--
-0005b2e0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-0005b2f0: 6733 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g3-color: var(--
-0005b300: 7269 6f2d 6c6f 6361 6c2d 6667 293b 2d2d  rio-local-fg);--
-0005b310: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-0005b320: 6733 2d62 6163 6b67 726f 756e 643a 2022  g3-background: "
-0005b330: 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f 6361  none";--rio-loca
-0005b340: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
-0005b350: 726f 756e 642d 636c 6970 3a20 2262 6f72  round-clip: "bor
-0005b360: 6465 722d 626f 7822 3b2d 2d72 696f 2d6c  der-box";--rio-l
-0005b370: 6f63 616c 2d68 6561 6469 6e67 332d 6669  ocal-heading3-fi
-0005b380: 6c6c 2d63 6f6c 6f72 3a20 2274 7261 6e73  ll-color: "trans
-0005b390: 7061 7265 6e74 223b 2d2d 7269 6f2d 6c6f  parent";--rio-lo
-0005b3a0: 6361 6c2d 7465 7874 2d63 6f6c 6f72 3a20  cal-text-color: 
-0005b3b0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005b3c0: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
-0005b3d0: 7465 7874 2d62 6163 6b67 726f 756e 643a  text-background:
-0005b3e0: 2022 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f   "none";--rio-lo
-0005b3f0: 6361 6c2d 7465 7874 2d62 6163 6b67 726f  cal-text-backgro
-0005b400: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
-0005b410: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
-0005b420: 616c 2d74 6578 742d 6669 6c6c 2d63 6f6c  al-text-fill-col
-0005b430: 6f72 3a20 2274 7261 6e73 7061 7265 6e74  or: "transparent
-0005b440: 223b 636f 6c6f 723a 7661 7228 2d2d 7269  ";color:var(--ri
-0005b450: 6f2d 6c6f 6361 6c2d 6667 297d 2e72 696f  o-local-fg)}.rio
-0005b460: 2d73 7769 7463 6865 726f 6f2d 6375 7374  -switcheroo-cust
-0005b470: 6f6d 7b2d 2d72 696f 2d6c 6f63 616c 2d62  om{--rio-local-b
-0005b480: 673a 2076 6172 282d 2d72 696f 2d63 7573  g: var(--rio-cus
-0005b490: 746f 6d2d 6c6f 6361 6c2d 6267 293b 2d2d  tom-local-bg);--
-0005b4a0: 7269 6f2d 6c6f 6361 6c2d 6267 2d76 6172  rio-local-bg-var
-0005b4b0: 6961 6e74 3a20 7661 7228 2d2d 7269 6f2d  iant: var(--rio-
-0005b4c0: 6375 7374 6f6d 2d6c 6f63 616c 2d62 672d  custom-local-bg-
-0005b4d0: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
-0005b4e0: 6f63 616c 2d62 672d 6163 7469 7665 3a20  ocal-bg-active: 
-0005b4f0: 7661 7228 2d2d 7269 6f2d 6375 7374 6f6d  var(--rio-custom
-0005b500: 2d6c 6f63 616c 2d62 672d 6163 7469 7665  -local-bg-active
-0005b510: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  );--rio-local-fg
-0005b520: 3a20 7661 7228 2d2d 7269 6f2d 6375 7374  : var(--rio-cust
-0005b530: 6f6d 2d6c 6f63 616c 2d66 6729 3b2d 2d72  om-local-fg);--r
-0005b540: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d32  io-local-level-2
-0005b550: 2d62 673a 2076 6172 282d 2d72 696f 2d67  -bg: var(--rio-g
-0005b560: 6c6f 6261 6c2d 7365 636f 6e64 6172 792d  lobal-secondary-
-0005b570: 6267 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  bg);--rio-local-
-0005b580: 6c65 7665 6c2d 322d 6267 2d76 6172 6961  level-2-bg-varia
-0005b590: 6e74 3a20 7661 7228 2d2d 7269 6f2d 676c  nt: var(--rio-gl
-0005b5a0: 6f62 616c 2d73 6563 6f6e 6461 7279 2d62  obal-secondary-b
-0005b5b0: 672d 7661 7269 616e 7429 3b2d 2d72 696f  g-variant);--rio
-0005b5c0: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
-0005b5d0: 672d 6163 7469 7665 3a20 7661 7228 2d2d  g-active: var(--
-0005b5e0: 7269 6f2d 676c 6f62 616c 2d73 6563 6f6e  rio-global-secon
-0005b5f0: 6461 7279 2d62 672d 6163 7469 7665 293b  dary-bg-active);
-0005b600: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005b610: 6c2d 322d 6667 3a20 7661 7228 2d2d 7269  l-2-fg: var(--ri
-0005b620: 6f2d 676c 6f62 616c 2d73 6563 6f6e 6461  o-global-seconda
-0005b630: 7279 2d66 6729 3b2d 2d72 696f 2d6c 6f63  ry-fg);--rio-loc
-0005b640: 616c 2d6c 6576 656c 2d33 2d62 673a 2076  al-level-3-bg: v
+0005a510: 2d73 6563 6f6e 6461 7279 2d62 672d 6163  -secondary-bg-ac
+0005a520: 7469 7665 293b 2d2d 7269 6f2d 6c6f 6361  tive);--rio-loca
+0005a530: 6c2d 6c65 7665 6c2d 322d 6667 3a20 7661  l-level-2-fg: va
+0005a540: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
+0005a550: 6563 6f6e 6461 7279 2d66 6729 3b2d 2d72  econdary-fg);--r
+0005a560: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
+0005a570: 2d62 673a 2076 6172 282d 2d72 696f 2d67  -bg: var(--rio-g
+0005a580: 6c6f 6261 6c2d 7072 696d 6172 792d 6267  lobal-primary-bg
+0005a590: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+0005a5a0: 7665 6c2d 332d 6267 2d76 6172 6961 6e74  vel-3-bg-variant
+0005a5b0: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+0005a5c0: 616c 2d70 7269 6d61 7279 2d62 672d 7661  al-primary-bg-va
+0005a5d0: 7269 616e 7429 3b2d 2d72 696f 2d6c 6f63  riant);--rio-loc
+0005a5e0: 616c 2d6c 6576 656c 2d33 2d62 672d 6163  al-level-3-bg-ac
+0005a5f0: 7469 7665 3a20 7661 7228 2d2d 7269 6f2d  tive: var(--rio-
+0005a600: 676c 6f62 616c 2d70 7269 6d61 7279 2d62  global-primary-b
+0005a610: 672d 6163 7469 7665 293b 2d2d 7269 6f2d  g-active);--rio-
+0005a620: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6667  local-level-3-fg
+0005a630: 3a20 7661 7228 2d2d 7269 6f2d 676c 6f62  : var(--rio-glob
+0005a640: 616c 2d70 7269 6d61 7279 2d66 6729 3b2d  al-primary-fg);-
+0005a650: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+0005a660: 6e67 312d 636f 6c6f 723a 2076 6172 282d  ng1-color: var(-
+0005a670: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
+0005a680: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+0005a690: 6e67 312d 6261 636b 6772 6f75 6e64 3a20  ng1-background: 
+0005a6a0: 226e 6f6e 6522 3b2d 2d72 696f 2d6c 6f63  "none";--rio-loc
+0005a6b0: 616c 2d68 6561 6469 6e67 312d 6261 636b  al-heading1-back
+0005a6c0: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
+0005a6d0: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
+0005a6e0: 6c6f 6361 6c2d 6865 6164 696e 6731 2d66  local-heading1-f
+0005a6f0: 696c 6c2d 636f 6c6f 723a 2022 7472 616e  ill-color: "tran
+0005a700: 7370 6172 656e 7422 3b2d 2d72 696f 2d6c  sparent";--rio-l
+0005a710: 6f63 616c 2d68 6561 6469 6e67 322d 636f  ocal-heading2-co
+0005a720: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+0005a730: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+0005a740: 6f63 616c 2d68 6561 6469 6e67 322d 6261  ocal-heading2-ba
+0005a750: 636b 6772 6f75 6e64 3a20 226e 6f6e 6522  ckground: "none"
+0005a760: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+0005a770: 6469 6e67 322d 6261 636b 6772 6f75 6e64  ding2-background
+0005a780: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
+0005a790: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
+0005a7a0: 6865 6164 696e 6732 2d66 696c 6c2d 636f  heading2-fill-co
+0005a7b0: 6c6f 723a 2022 7472 616e 7370 6172 656e  lor: "transparen
+0005a7c0: 7422 3b2d 2d72 696f 2d6c 6f63 616c 2d68  t";--rio-local-h
+0005a7d0: 6561 6469 6e67 332d 636f 6c6f 723a 2076  eading3-color: v
+0005a7e0: 6172 282d 2d72 696f 2d6c 6f63 616c 2d66  ar(--rio-local-f
+0005a7f0: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d68  g);--rio-local-h
+0005a800: 6561 6469 6e67 332d 6261 636b 6772 6f75  eading3-backgrou
+0005a810: 6e64 3a20 226e 6f6e 6522 3b2d 2d72 696f  nd: "none";--rio
+0005a820: 2d6c 6f63 616c 2d68 6561 6469 6e67 332d  -local-heading3-
+0005a830: 6261 636b 6772 6f75 6e64 2d63 6c69 703a  background-clip:
+0005a840: 2022 626f 7264 6572 2d62 6f78 223b 2d2d   "border-box";--
+0005a850: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005a860: 6733 2d66 696c 6c2d 636f 6c6f 723a 2022  g3-fill-color: "
+0005a870: 7472 616e 7370 6172 656e 7422 3b2d 2d72  transparent";--r
+0005a880: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
+0005a890: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+0005a8a0: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+0005a8b0: 6f63 616c 2d74 6578 742d 6261 636b 6772  ocal-text-backgr
+0005a8c0: 6f75 6e64 3a20 226e 6f6e 6522 3b2d 2d72  ound: "none";--r
+0005a8d0: 696f 2d6c 6f63 616c 2d74 6578 742d 6261  io-local-text-ba
+0005a8e0: 636b 6772 6f75 6e64 2d63 6c69 703a 2022  ckground-clip: "
+0005a8f0: 626f 7264 6572 2d62 6f78 223b 2d2d 7269  border-box";--ri
+0005a900: 6f2d 6c6f 6361 6c2d 7465 7874 2d66 696c  o-local-text-fil
+0005a910: 6c2d 636f 6c6f 723a 2022 7472 616e 7370  l-color: "transp
+0005a920: 6172 656e 7422 3b63 6f6c 6f72 3a76 6172  arent";color:var
+0005a930: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+0005a940: 7d2e 7269 6f2d 7377 6974 6368 6572 6f6f  }.rio-switcheroo
+0005a950: 2d64 616e 6765 727b 2d2d 7269 6f2d 6c6f  -danger{--rio-lo
+0005a960: 6361 6c2d 6267 3a20 7661 7228 2d2d 7269  cal-bg: var(--ri
+0005a970: 6f2d 676c 6f62 616c 2d64 616e 6765 722d  o-global-danger-
+0005a980: 6267 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  bg);--rio-local-
+0005a990: 6267 2d76 6172 6961 6e74 3a20 7661 7228  bg-variant: var(
+0005a9a0: 2d2d 7269 6f2d 676c 6f62 616c 2d64 616e  --rio-global-dan
+0005a9b0: 6765 722d 6267 2d76 6172 6961 6e74 293b  ger-bg-variant);
+0005a9c0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6267 2d61  --rio-local-bg-a
+0005a9d0: 6374 6976 653a 2076 6172 282d 2d72 696f  ctive: var(--rio
+0005a9e0: 2d67 6c6f 6261 6c2d 6461 6e67 6572 2d62  -global-danger-b
+0005a9f0: 672d 6163 7469 7665 293b 2d2d 7269 6f2d  g-active);--rio-
+0005aa00: 6c6f 6361 6c2d 6667 3a20 7661 7228 2d2d  local-fg: var(--
+0005aa10: 7269 6f2d 676c 6f62 616c 2d64 616e 6765  rio-global-dange
+0005aa20: 722d 6667 293b 2d2d 7269 6f2d 6c6f 6361  r-fg);--rio-loca
+0005aa30: 6c2d 6c65 7665 6c2d 322d 6267 3a20 7661  l-level-2-bg: va
+0005aa40: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
+0005aa50: 6563 6f6e 6461 7279 2d62 6729 3b2d 2d72  econdary-bg);--r
+0005aa60: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d32  io-local-level-2
+0005aa70: 2d62 672d 7661 7269 616e 743a 2076 6172  -bg-variant: var
+0005aa80: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
+0005aa90: 636f 6e64 6172 792d 6267 2d76 6172 6961  condary-bg-varia
+0005aaa0: 6e74 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt);--rio-local-
+0005aab0: 6c65 7665 6c2d 322d 6267 2d61 6374 6976  level-2-bg-activ
+0005aac0: 653a 2076 6172 282d 2d72 696f 2d67 6c6f  e: var(--rio-glo
+0005aad0: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
+0005aae0: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
+0005aaf0: 6f63 616c 2d6c 6576 656c 2d32 2d66 673a  ocal-level-2-fg:
+0005ab00: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+0005ab10: 6c2d 7365 636f 6e64 6172 792d 6667 293b  l-secondary-fg);
+0005ab20: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+0005ab30: 6c2d 332d 6267 3a20 7661 7228 2d2d 7269  l-3-bg: var(--ri
+0005ab40: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
+0005ab50: 2d62 6729 3b2d 2d72 696f 2d6c 6f63 616c  -bg);--rio-local
+0005ab60: 2d6c 6576 656c 2d33 2d62 672d 7661 7269  -level-3-bg-vari
+0005ab70: 616e 743a 2076 6172 282d 2d72 696f 2d67  ant: var(--rio-g
+0005ab80: 6c6f 6261 6c2d 7072 696d 6172 792d 6267  lobal-primary-bg
+0005ab90: 2d76 6172 6961 6e74 293b 2d2d 7269 6f2d  -variant);--rio-
+0005aba0: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
+0005abb0: 2d61 6374 6976 653a 2076 6172 282d 2d72  -active: var(--r
+0005abc0: 696f 2d67 6c6f 6261 6c2d 7072 696d 6172  io-global-primar
+0005abd0: 792d 6267 2d61 6374 6976 6529 3b2d 2d72  y-bg-active);--r
+0005abe0: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
+0005abf0: 2d66 673a 2076 6172 282d 2d72 696f 2d67  -fg: var(--rio-g
+0005ac00: 6c6f 6261 6c2d 7072 696d 6172 792d 6667  lobal-primary-fg
+0005ac10: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
+0005ac20: 6164 696e 6731 2d63 6f6c 6f72 3a20 7661  ading1-color: va
+0005ac30: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  r(--rio-local-fg
+0005ac40: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
+0005ac50: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
+0005ac60: 643a 2022 6e6f 6e65 223b 2d2d 7269 6f2d  d: "none";--rio-
+0005ac70: 6c6f 6361 6c2d 6865 6164 696e 6731 2d62  local-heading1-b
+0005ac80: 6163 6b67 726f 756e 642d 636c 6970 3a20  ackground-clip: 
+0005ac90: 2262 6f72 6465 722d 626f 7822 3b2d 2d72  "border-box";--r
+0005aca0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
+0005acb0: 312d 6669 6c6c 2d63 6f6c 6f72 3a20 2274  1-fill-color: "t
+0005acc0: 7261 6e73 7061 7265 6e74 223b 2d2d 7269  ransparent";--ri
+0005acd0: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
+0005ace0: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
+0005acf0: 6f2d 6c6f 6361 6c2d 6667 293b 2d2d 7269  o-local-fg);--ri
+0005ad00: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
+0005ad10: 2d62 6163 6b67 726f 756e 643a 2022 6e6f  -background: "no
+0005ad20: 6e65 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ne";--rio-local-
+0005ad30: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
+0005ad40: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
+0005ad50: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
+0005ad60: 616c 2d68 6561 6469 6e67 322d 6669 6c6c  al-heading2-fill
+0005ad70: 2d63 6f6c 6f72 3a20 2274 7261 6e73 7061  -color: "transpa
+0005ad80: 7265 6e74 223b 2d2d 7269 6f2d 6c6f 6361  rent";--rio-loca
+0005ad90: 6c2d 6865 6164 696e 6733 2d63 6f6c 6f72  l-heading3-color
+0005ada0: 3a20 7661 7228 2d2d 7269 6f2d 6c6f 6361  : var(--rio-loca
+0005adb0: 6c2d 6667 293b 2d2d 7269 6f2d 6c6f 6361  l-fg);--rio-loca
+0005adc0: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
+0005add0: 726f 756e 643a 2022 6e6f 6e65 223b 2d2d  round: "none";--
+0005ade0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005adf0: 6733 2d62 6163 6b67 726f 756e 642d 636c  g3-background-cl
+0005ae00: 6970 3a20 2262 6f72 6465 722d 626f 7822  ip: "border-box"
+0005ae10: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+0005ae20: 6469 6e67 332d 6669 6c6c 2d63 6f6c 6f72  ding3-fill-color
+0005ae30: 3a20 2274 7261 6e73 7061 7265 6e74 223b  : "transparent";
+0005ae40: 2d2d 7269 6f2d 6c6f 6361 6c2d 7465 7874  --rio-local-text
+0005ae50: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 7269  -color: var(--ri
+0005ae60: 6f2d 6c6f 6361 6c2d 6667 293b 2d2d 7269  o-local-fg);--ri
+0005ae70: 6f2d 6c6f 6361 6c2d 7465 7874 2d62 6163  o-local-text-bac
+0005ae80: 6b67 726f 756e 643a 2022 6e6f 6e65 223b  kground: "none";
+0005ae90: 2d2d 7269 6f2d 6c6f 6361 6c2d 7465 7874  --rio-local-text
+0005aea0: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
+0005aeb0: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
+0005aec0: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
+0005aed0: 6669 6c6c 2d63 6f6c 6f72 3a20 2274 7261  fill-color: "tra
+0005aee0: 6e73 7061 7265 6e74 223b 636f 6c6f 723a  nsparent";color:
+0005aef0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+0005af00: 6667 297d 2e72 696f 2d73 7769 7463 6865  fg)}.rio-switche
+0005af10: 726f 6f2d 6469 7361 626c 6564 7b2d 2d72  roo-disabled{--r
+0005af20: 696f 2d6c 6f63 616c 2d62 673a 2076 6172  io-local-bg: var
+0005af30: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6469  (--rio-global-di
+0005af40: 7361 626c 6564 2d62 6729 3b2d 2d72 696f  sabled-bg);--rio
+0005af50: 2d6c 6f63 616c 2d62 672d 7661 7269 616e  -local-bg-varian
+0005af60: 743a 2076 6172 282d 2d72 696f 2d67 6c6f  t: var(--rio-glo
+0005af70: 6261 6c2d 6469 7361 626c 6564 2d62 672d  bal-disabled-bg-
+0005af80: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
+0005af90: 6f63 616c 2d62 672d 6163 7469 7665 3a20  ocal-bg-active: 
+0005afa0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+0005afb0: 2d64 6973 6162 6c65 642d 6267 2d61 6374  -disabled-bg-act
+0005afc0: 6976 6529 3b2d 2d72 696f 2d6c 6f63 616c  ive);--rio-local
+0005afd0: 2d66 673a 2076 6172 282d 2d72 696f 2d67  -fg: var(--rio-g
+0005afe0: 6c6f 6261 6c2d 6469 7361 626c 6564 2d66  lobal-disabled-f
+0005aff0: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
+0005b000: 6576 656c 2d32 2d62 673a 2076 6172 282d  evel-2-bg: var(-
+0005b010: 2d72 696f 2d67 6c6f 6261 6c2d 6469 7361  -rio-global-disa
+0005b020: 626c 6564 2d62 6729 3b2d 2d72 696f 2d6c  bled-bg);--rio-l
+0005b030: 6f63 616c 2d6c 6576 656c 2d32 2d62 672d  ocal-level-2-bg-
+0005b040: 7661 7269 616e 743a 2076 6172 282d 2d72  variant: var(--r
+0005b050: 696f 2d67 6c6f 6261 6c2d 6469 7361 626c  io-global-disabl
+0005b060: 6564 2d62 672d 7661 7269 616e 7429 3b2d  ed-bg-variant);-
+0005b070: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
+0005b080: 2d32 2d62 672d 6163 7469 7665 3a20 7661  -2-bg-active: va
+0005b090: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d64  r(--rio-global-d
+0005b0a0: 6973 6162 6c65 642d 6267 2d61 6374 6976  isabled-bg-activ
+0005b0b0: 6529 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  e);--rio-local-l
+0005b0c0: 6576 656c 2d32 2d66 673a 2076 6172 282d  evel-2-fg: var(-
+0005b0d0: 2d72 696f 2d67 6c6f 6261 6c2d 6469 7361  -rio-global-disa
+0005b0e0: 626c 6564 2d66 6729 3b2d 2d72 696f 2d6c  bled-fg);--rio-l
+0005b0f0: 6f63 616c 2d6c 6576 656c 2d33 2d62 673a  ocal-level-3-bg:
+0005b100: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+0005b110: 6c2d 6469 7361 626c 6564 2d62 6729 3b2d  l-disabled-bg);-
+0005b120: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
+0005b130: 2d33 2d62 672d 7661 7269 616e 743a 2076  -3-bg-variant: v
+0005b140: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+0005b150: 6469 7361 626c 6564 2d62 672d 7661 7269  disabled-bg-vari
+0005b160: 616e 7429 3b2d 2d72 696f 2d6c 6f63 616c  ant);--rio-local
+0005b170: 2d6c 6576 656c 2d33 2d62 672d 6163 7469  -level-3-bg-acti
+0005b180: 7665 3a20 7661 7228 2d2d 7269 6f2d 676c  ve: var(--rio-gl
+0005b190: 6f62 616c 2d64 6973 6162 6c65 642d 6267  obal-disabled-bg
+0005b1a0: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
+0005b1b0: 6f63 616c 2d6c 6576 656c 2d33 2d66 673a  ocal-level-3-fg:
+0005b1c0: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+0005b1d0: 6c2d 6469 7361 626c 6564 2d66 6729 3b2d  l-disabled-fg);-
+0005b1e0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+0005b1f0: 6e67 312d 636f 6c6f 723a 2076 6172 282d  ng1-color: var(-
+0005b200: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
+0005b210: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+0005b220: 6e67 312d 6261 636b 6772 6f75 6e64 3a20  ng1-background: 
+0005b230: 226e 6f6e 6522 3b2d 2d72 696f 2d6c 6f63  "none";--rio-loc
+0005b240: 616c 2d68 6561 6469 6e67 312d 6261 636b  al-heading1-back
+0005b250: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
+0005b260: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
+0005b270: 6c6f 6361 6c2d 6865 6164 696e 6731 2d66  local-heading1-f
+0005b280: 696c 6c2d 636f 6c6f 723a 2022 7472 616e  ill-color: "tran
+0005b290: 7370 6172 656e 7422 3b2d 2d72 696f 2d6c  sparent";--rio-l
+0005b2a0: 6f63 616c 2d68 6561 6469 6e67 322d 636f  ocal-heading2-co
+0005b2b0: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+0005b2c0: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+0005b2d0: 6f63 616c 2d68 6561 6469 6e67 322d 6261  ocal-heading2-ba
+0005b2e0: 636b 6772 6f75 6e64 3a20 226e 6f6e 6522  ckground: "none"
+0005b2f0: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
+0005b300: 6469 6e67 322d 6261 636b 6772 6f75 6e64  ding2-background
+0005b310: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
+0005b320: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
+0005b330: 6865 6164 696e 6732 2d66 696c 6c2d 636f  heading2-fill-co
+0005b340: 6c6f 723a 2022 7472 616e 7370 6172 656e  lor: "transparen
+0005b350: 7422 3b2d 2d72 696f 2d6c 6f63 616c 2d68  t";--rio-local-h
+0005b360: 6561 6469 6e67 332d 636f 6c6f 723a 2076  eading3-color: v
+0005b370: 6172 282d 2d72 696f 2d6c 6f63 616c 2d66  ar(--rio-local-f
+0005b380: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d68  g);--rio-local-h
+0005b390: 6561 6469 6e67 332d 6261 636b 6772 6f75  eading3-backgrou
+0005b3a0: 6e64 3a20 226e 6f6e 6522 3b2d 2d72 696f  nd: "none";--rio
+0005b3b0: 2d6c 6f63 616c 2d68 6561 6469 6e67 332d  -local-heading3-
+0005b3c0: 6261 636b 6772 6f75 6e64 2d63 6c69 703a  background-clip:
+0005b3d0: 2022 626f 7264 6572 2d62 6f78 223b 2d2d   "border-box";--
+0005b3e0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005b3f0: 6733 2d66 696c 6c2d 636f 6c6f 723a 2022  g3-fill-color: "
+0005b400: 7472 616e 7370 6172 656e 7422 3b2d 2d72  transparent";--r
+0005b410: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
+0005b420: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
+0005b430: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
+0005b440: 6f63 616c 2d74 6578 742d 6261 636b 6772  ocal-text-backgr
+0005b450: 6f75 6e64 3a20 226e 6f6e 6522 3b2d 2d72  ound: "none";--r
+0005b460: 696f 2d6c 6f63 616c 2d74 6578 742d 6261  io-local-text-ba
+0005b470: 636b 6772 6f75 6e64 2d63 6c69 703a 2022  ckground-clip: "
+0005b480: 626f 7264 6572 2d62 6f78 223b 2d2d 7269  border-box";--ri
+0005b490: 6f2d 6c6f 6361 6c2d 7465 7874 2d66 696c  o-local-text-fil
+0005b4a0: 6c2d 636f 6c6f 723a 2022 7472 616e 7370  l-color: "transp
+0005b4b0: 6172 656e 7422 3b63 6f6c 6f72 3a76 6172  arent";color:var
+0005b4c0: 282d 2d72 696f 2d6c 6f63 616c 2d66 6729  (--rio-local-fg)
+0005b4d0: 7d2e 7269 6f2d 7377 6974 6368 6572 6f6f  }.rio-switcheroo
+0005b4e0: 2d63 7573 746f 6d7b 2d2d 7269 6f2d 6c6f  -custom{--rio-lo
+0005b4f0: 6361 6c2d 6267 3a20 7661 7228 2d2d 7269  cal-bg: var(--ri
+0005b500: 6f2d 6375 7374 6f6d 2d6c 6f63 616c 2d62  o-custom-local-b
+0005b510: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d62  g);--rio-local-b
+0005b520: 672d 7661 7269 616e 743a 2076 6172 282d  g-variant: var(-
+0005b530: 2d72 696f 2d63 7573 746f 6d2d 6c6f 6361  -rio-custom-loca
+0005b540: 6c2d 6267 2d76 6172 6961 6e74 293b 2d2d  l-bg-variant);--
+0005b550: 7269 6f2d 6c6f 6361 6c2d 6267 2d61 6374  rio-local-bg-act
+0005b560: 6976 653a 2076 6172 282d 2d72 696f 2d63  ive: var(--rio-c
+0005b570: 7573 746f 6d2d 6c6f 6361 6c2d 6267 2d61  ustom-local-bg-a
+0005b580: 6374 6976 6529 3b2d 2d72 696f 2d6c 6f63  ctive);--rio-loc
+0005b590: 616c 2d66 673a 2076 6172 282d 2d72 696f  al-fg: var(--rio
+0005b5a0: 2d63 7573 746f 6d2d 6c6f 6361 6c2d 6667  -custom-local-fg
+0005b5b0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+0005b5c0: 7665 6c2d 322d 6267 3a20 7661 7228 2d2d  vel-2-bg: var(--
+0005b5d0: 7269 6f2d 676c 6f62 616c 2d73 6563 6f6e  rio-global-secon
+0005b5e0: 6461 7279 2d62 6729 3b2d 2d72 696f 2d6c  dary-bg);--rio-l
+0005b5f0: 6f63 616c 2d6c 6576 656c 2d32 2d62 672d  ocal-level-2-bg-
+0005b600: 7661 7269 616e 743a 2076 6172 282d 2d72  variant: var(--r
+0005b610: 696f 2d67 6c6f 6261 6c2d 7365 636f 6e64  io-global-second
+0005b620: 6172 792d 6267 2d76 6172 6961 6e74 293b  ary-bg-variant);
+0005b630: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+0005b640: 6c2d 322d 6267 2d61 6374 6976 653a 2076  l-2-bg-active: v
 0005b650: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-0005b660: 7072 696d 6172 792d 6267 293b 2d2d 7269  primary-bg);--ri
-0005b670: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 332d  o-local-level-3-
-0005b680: 6267 2d76 6172 6961 6e74 3a20 7661 7228  bg-variant: var(
-0005b690: 2d2d 7269 6f2d 676c 6f62 616c 2d70 7269  --rio-global-pri
-0005b6a0: 6d61 7279 2d62 672d 7661 7269 616e 7429  mary-bg-variant)
-0005b6b0: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
-0005b6c0: 656c 2d33 2d62 672d 6163 7469 7665 3a20  el-3-bg-active: 
-0005b6d0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005b6e0: 2d70 7269 6d61 7279 2d62 672d 6163 7469  -primary-bg-acti
-0005b6f0: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
-0005b700: 6c65 7665 6c2d 332d 6667 3a20 7661 7228  level-3-fg: var(
-0005b710: 2d2d 7269 6f2d 676c 6f62 616c 2d70 7269  --rio-global-pri
-0005b720: 6d61 7279 2d66 6729 3b2d 2d72 696f 2d6c  mary-fg);--rio-l
-0005b730: 6f63 616c 2d68 6561 6469 6e67 312d 636f  ocal-heading1-co
-0005b740: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
-0005b750: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
-0005b760: 6f63 616c 2d68 6561 6469 6e67 312d 6261  ocal-heading1-ba
-0005b770: 636b 6772 6f75 6e64 3a20 226e 6f6e 6522  ckground: "none"
-0005b780: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
-0005b790: 6469 6e67 312d 6261 636b 6772 6f75 6e64  ding1-background
-0005b7a0: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
-0005b7b0: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
-0005b7c0: 6865 6164 696e 6731 2d66 696c 6c2d 636f  heading1-fill-co
-0005b7d0: 6c6f 723a 2022 7472 616e 7370 6172 656e  lor: "transparen
-0005b7e0: 7422 3b2d 2d72 696f 2d6c 6f63 616c 2d68  t";--rio-local-h
-0005b7f0: 6561 6469 6e67 322d 636f 6c6f 723a 2076  eading2-color: v
-0005b800: 6172 282d 2d72 696f 2d6c 6f63 616c 2d66  ar(--rio-local-f
-0005b810: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d68  g);--rio-local-h
-0005b820: 6561 6469 6e67 322d 6261 636b 6772 6f75  eading2-backgrou
-0005b830: 6e64 3a20 226e 6f6e 6522 3b2d 2d72 696f  nd: "none";--rio
-0005b840: 2d6c 6f63 616c 2d68 6561 6469 6e67 322d  -local-heading2-
-0005b850: 6261 636b 6772 6f75 6e64 2d63 6c69 703a  background-clip:
-0005b860: 2022 626f 7264 6572 2d62 6f78 223b 2d2d   "border-box";--
-0005b870: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
-0005b880: 6732 2d66 696c 6c2d 636f 6c6f 723a 2022  g2-fill-color: "
-0005b890: 7472 616e 7370 6172 656e 7422 3b2d 2d72  transparent";--r
-0005b8a0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-0005b8b0: 332d 636f 6c6f 723a 2076 6172 282d 2d72  3-color: var(--r
-0005b8c0: 696f 2d6c 6f63 616c 2d66 6729 3b2d 2d72  io-local-fg);--r
-0005b8d0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-0005b8e0: 332d 6261 636b 6772 6f75 6e64 3a20 226e  3-background: "n
-0005b8f0: 6f6e 6522 3b2d 2d72 696f 2d6c 6f63 616c  one";--rio-local
-0005b900: 2d68 6561 6469 6e67 332d 6261 636b 6772  -heading3-backgr
-0005b910: 6f75 6e64 2d63 6c69 703a 2022 626f 7264  ound-clip: "bord
-0005b920: 6572 2d62 6f78 223b 2d2d 7269 6f2d 6c6f  er-box";--rio-lo
-0005b930: 6361 6c2d 6865 6164 696e 6733 2d66 696c  cal-heading3-fil
-0005b940: 6c2d 636f 6c6f 723a 2022 7472 616e 7370  l-color: "transp
-0005b950: 6172 656e 7422 3b2d 2d72 696f 2d6c 6f63  arent";--rio-loc
-0005b960: 616c 2d74 6578 742d 636f 6c6f 723a 2076  al-text-color: v
-0005b970: 6172 282d 2d72 696f 2d6c 6f63 616c 2d66  ar(--rio-local-f
-0005b980: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d74  g);--rio-local-t
-0005b990: 6578 742d 6261 636b 6772 6f75 6e64 3a20  ext-background: 
-0005b9a0: 226e 6f6e 6522 3b2d 2d72 696f 2d6c 6f63  "none";--rio-loc
-0005b9b0: 616c 2d74 6578 742d 6261 636b 6772 6f75  al-text-backgrou
-0005b9c0: 6e64 2d63 6c69 703a 2022 626f 7264 6572  nd-clip: "border
-0005b9d0: 2d62 6f78 223b 2d2d 7269 6f2d 6c6f 6361  -box";--rio-loca
-0005b9e0: 6c2d 7465 7874 2d66 696c 6c2d 636f 6c6f  l-text-fill-colo
-0005b9f0: 723a 2022 7472 616e 7370 6172 656e 7422  r: "transparent"
-0005ba00: 3b63 6f6c 6f72 3a76 6172 282d 2d72 696f  ;color:var(--rio
-0005ba10: 2d6c 6f63 616c 2d66 6729 7d2e 7269 6f2d  -local-fg)}.rio-
-0005ba20: 7377 6974 6368 6572 6f6f 2d62 6163 6b67  switcheroo-backg
-0005ba30: 726f 756e 643e 2a2c 2e72 696f 2d73 7769  round>*,.rio-swi
-0005ba40: 7463 6865 726f 6f2d 6e65 7574 7261 6c3e  tcheroo-neutral>
-0005ba50: 2a2c 2e72 696f 2d73 7769 7463 6865 726f  *,.rio-switchero
-0005ba60: 6f2d 6875 643e 2a2c 2e72 696f 2d73 7769  o-hud>*,.rio-swi
-0005ba70: 7463 6865 726f 6f2d 7072 696d 6172 793e  tcheroo-primary>
-0005ba80: 2a2c 2e72 696f 2d73 7769 7463 6865 726f  *,.rio-switchero
-0005ba90: 6f2d 7365 636f 6e64 6172 793e 2a2c 2e72  o-secondary>*,.r
-0005baa0: 696f 2d73 7769 7463 6865 726f 6f2d 7375  io-switcheroo-su
-0005bab0: 6363 6573 733e 2a2c 2e72 696f 2d73 7769  ccess>*,.rio-swi
-0005bac0: 7463 6865 726f 6f2d 7761 726e 696e 673e  tcheroo-warning>
-0005bad0: 2a2c 2e72 696f 2d73 7769 7463 6865 726f  *,.rio-switchero
-0005bae0: 6f2d 6461 6e67 6572 3e2a 2c2e 7269 6f2d  o-danger>*,.rio-
-0005baf0: 7377 6974 6368 6572 6f6f 2d64 6973 6162  switcheroo-disab
-0005bb00: 6c65 643e 2a2c 2e72 696f 2d73 7769 7463  led>*,.rio-switc
-0005bb10: 6865 726f 6f2d 6375 7374 6f6d 3e2a 2c2e  heroo-custom>*,.
-0005bb20: 7269 6f2d 7377 6974 6368 6572 6f6f 2d62  rio-switcheroo-b
-0005bb30: 756d 703e 2a7b 2d2d 7269 6f2d 6275 6666  ump>*{--rio-buff
-0005bb40: 6572 2d6c 6576 656c 2d32 2d62 673a 2076  er-level-2-bg: v
-0005bb50: 6172 282d 2d72 696f 2d6c 6f63 616c 2d6c  ar(--rio-local-l
-0005bb60: 6576 656c 2d32 2d62 6729 3b2d 2d72 696f  evel-2-bg);--rio
-0005bb70: 2d62 7566 6665 722d 6c65 7665 6c2d 322d  -buffer-level-2-
-0005bb80: 6267 2d76 6172 6961 6e74 3a20 7661 7228  bg-variant: var(
-0005bb90: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005bba0: 6c2d 322d 6267 2d76 6172 6961 6e74 293b  l-2-bg-variant);
-0005bbb0: 2d2d 7269 6f2d 6275 6666 6572 2d6c 6576  --rio-buffer-lev
-0005bbc0: 656c 2d32 2d62 672d 6163 7469 7665 3a20  el-2-bg-active: 
-0005bbd0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005bbe0: 6c65 7665 6c2d 322d 6267 2d61 6374 6976  level-2-bg-activ
-0005bbf0: 6529 3b2d 2d72 696f 2d62 7566 6665 722d  e);--rio-buffer-
-0005bc00: 6c65 7665 6c2d 322d 6667 3a20 7661 7228  level-2-fg: var(
-0005bc10: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005bc20: 6c2d 322d 6667 293b 2d2d 7269 6f2d 6275  l-2-fg);--rio-bu
-0005bc30: 6666 6572 2d6c 6576 656c 2d33 2d62 673a  ffer-level-3-bg:
-0005bc40: 2076 6172 282d 2d72 696f 2d6c 6f63 616c   var(--rio-local
-0005bc50: 2d6c 6576 656c 2d33 2d62 6729 3b2d 2d72  -level-3-bg);--r
-0005bc60: 696f 2d62 7566 6665 722d 6c65 7665 6c2d  io-buffer-level-
-0005bc70: 332d 6267 2d76 6172 6961 6e74 3a20 7661  3-bg-variant: va
-0005bc80: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  r(--rio-local-le
-0005bc90: 7665 6c2d 332d 6267 2d76 6172 6961 6e74  vel-3-bg-variant
-0005bca0: 293b 2d2d 7269 6f2d 6275 6666 6572 2d6c  );--rio-buffer-l
-0005bcb0: 6576 656c 2d33 2d62 672d 6163 7469 7665  evel-3-bg-active
-0005bcc0: 3a20 7661 7228 2d2d 7269 6f2d 6c6f 6361  : var(--rio-loca
-0005bcd0: 6c2d 6c65 7665 6c2d 332d 6267 2d61 6374  l-level-3-bg-act
-0005bce0: 6976 6529 3b2d 2d72 696f 2d62 7566 6665  ive);--rio-buffe
-0005bcf0: 722d 6c65 7665 6c2d 332d 6667 3a20 7661  r-level-3-fg: va
-0005bd00: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  r(--rio-local-le
-0005bd10: 7665 6c2d 332d 6667 297d 2e72 696f 2d73  vel-3-fg)}.rio-s
-0005bd20: 7769 7463 6865 726f 6f2d 6275 6d70 7b2d  witcheroo-bump{-
-0005bd30: 2d72 696f 2d6c 6f63 616c 2d62 673a 2076  -rio-local-bg: v
-0005bd40: 6172 282d 2d72 696f 2d62 7566 6665 722d  ar(--rio-buffer-
-0005bd50: 6c65 7665 6c2d 322d 6267 293b 2d2d 7269  level-2-bg);--ri
-0005bd60: 6f2d 6c6f 6361 6c2d 6267 2d76 6172 6961  o-local-bg-varia
-0005bd70: 6e74 3a20 7661 7228 2d2d 7269 6f2d 6275  nt: var(--rio-bu
-0005bd80: 6666 6572 2d6c 6576 656c 2d32 2d62 672d  ffer-level-2-bg-
-0005bd90: 7661 7269 616e 7429 3b2d 2d72 696f 2d6c  variant);--rio-l
-0005bda0: 6f63 616c 2d62 672d 6163 7469 7665 3a20  ocal-bg-active: 
-0005bdb0: 7661 7228 2d2d 7269 6f2d 6275 6666 6572  var(--rio-buffer
-0005bdc0: 2d6c 6576 656c 2d32 2d62 672d 6163 7469  -level-2-bg-acti
-0005bdd0: 7665 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  ve);--rio-local-
-0005bde0: 6667 3a20 7661 7228 2d2d 7269 6f2d 6275  fg: var(--rio-bu
-0005bdf0: 6666 6572 2d6c 6576 656c 2d32 2d66 6729  ffer-level-2-fg)
-0005be00: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
-0005be10: 656c 2d32 2d62 673a 2076 6172 282d 2d72  el-2-bg: var(--r
-0005be20: 696f 2d62 7566 6665 722d 6c65 7665 6c2d  io-buffer-level-
-0005be30: 332d 6267 293b 2d2d 7269 6f2d 6c6f 6361  3-bg);--rio-loca
-0005be40: 6c2d 6c65 7665 6c2d 322d 6267 2d76 6172  l-level-2-bg-var
-0005be50: 6961 6e74 3a20 7661 7228 2d2d 7269 6f2d  iant: var(--rio-
-0005be60: 6275 6666 6572 2d6c 6576 656c 2d33 2d62  buffer-level-3-b
-0005be70: 672d 7661 7269 616e 7429 3b2d 2d72 696f  g-variant);--rio
-0005be80: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
-0005be90: 672d 6163 7469 7665 3a20 7661 7228 2d2d  g-active: var(--
-0005bea0: 7269 6f2d 6275 6666 6572 2d6c 6576 656c  rio-buffer-level
-0005beb0: 2d33 2d62 672d 6163 7469 7665 293b 2d2d  -3-bg-active);--
-0005bec0: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-0005bed0: 322d 6667 3a20 7661 7228 2d2d 7269 6f2d  2-fg: var(--rio-
-0005bee0: 6275 6666 6572 2d6c 6576 656c 2d33 2d66  buffer-level-3-f
-0005bef0: 6729 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  g);--rio-local-l
-0005bf00: 6576 656c 2d33 2d62 673a 2076 6172 282d  evel-3-bg: var(-
-0005bf10: 2d72 696f 2d62 7566 6665 722d 6c65 7665  -rio-buffer-leve
-0005bf20: 6c2d 322d 6267 293b 2d2d 7269 6f2d 6c6f  l-2-bg);--rio-lo
-0005bf30: 6361 6c2d 6c65 7665 6c2d 332d 6267 2d76  cal-level-3-bg-v
-0005bf40: 6172 6961 6e74 3a20 7661 7228 2d2d 7269  ariant: var(--ri
-0005bf50: 6f2d 6275 6666 6572 2d6c 6576 656c 2d32  o-buffer-level-2
-0005bf60: 2d62 672d 7661 7269 616e 7429 3b2d 2d72  -bg-variant);--r
-0005bf70: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
-0005bf80: 2d62 672d 6163 7469 7665 3a20 7661 7228  -bg-active: var(
-0005bf90: 2d2d 7269 6f2d 6275 6666 6572 2d6c 6576  --rio-buffer-lev
-0005bfa0: 656c 2d32 2d62 672d 6163 7469 7665 293b  el-2-bg-active);
-0005bfb0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005bfc0: 6c2d 332d 6667 3a20 7661 7228 2d2d 7269  l-3-fg: var(--ri
-0005bfd0: 6f2d 6275 6666 6572 2d6c 6576 656c 2d32  o-buffer-level-2
-0005bfe0: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
-0005bff0: 2d68 6561 6469 6e67 312d 636f 6c6f 723a  -heading1-color:
-0005c000: 2076 6172 282d 2d72 696f 2d6c 6f63 616c   var(--rio-local
-0005c010: 2d66 6729 3b2d 2d72 696f 2d6c 6f63 616c  -fg);--rio-local
-0005c020: 2d68 6561 6469 6e67 312d 6261 636b 6772  -heading1-backgr
-0005c030: 6f75 6e64 3a20 226e 6f6e 6522 3b2d 2d72  ound: "none";--r
-0005c040: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
-0005c050: 312d 6261 636b 6772 6f75 6e64 2d63 6c69  1-background-cli
-0005c060: 703a 2022 626f 7264 6572 2d62 6f78 223b  p: "border-box";
-0005c070: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-0005c080: 696e 6731 2d66 696c 6c2d 636f 6c6f 723a  ing1-fill-color:
-0005c090: 2022 7472 616e 7370 6172 656e 7422 3b2d   "transparent";-
-0005c0a0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-0005c0b0: 6e67 322d 636f 6c6f 723a 2076 6172 282d  ng2-color: var(-
-0005c0c0: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
-0005c0d0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-0005c0e0: 6e67 322d 6261 636b 6772 6f75 6e64 3a20  ng2-background: 
-0005c0f0: 226e 6f6e 6522 3b2d 2d72 696f 2d6c 6f63  "none";--rio-loc
-0005c100: 616c 2d68 6561 6469 6e67 322d 6261 636b  al-heading2-back
-0005c110: 6772 6f75 6e64 2d63 6c69 703a 2022 626f  ground-clip: "bo
-0005c120: 7264 6572 2d62 6f78 223b 2d2d 7269 6f2d  rder-box";--rio-
-0005c130: 6c6f 6361 6c2d 6865 6164 696e 6732 2d66  local-heading2-f
-0005c140: 696c 6c2d 636f 6c6f 723a 2022 7472 616e  ill-color: "tran
-0005c150: 7370 6172 656e 7422 3b2d 2d72 696f 2d6c  sparent";--rio-l
-0005c160: 6f63 616c 2d68 6561 6469 6e67 332d 636f  ocal-heading3-co
-0005c170: 6c6f 723a 2076 6172 282d 2d72 696f 2d6c  lor: var(--rio-l
-0005c180: 6f63 616c 2d66 6729 3b2d 2d72 696f 2d6c  ocal-fg);--rio-l
-0005c190: 6f63 616c 2d68 6561 6469 6e67 332d 6261  ocal-heading3-ba
-0005c1a0: 636b 6772 6f75 6e64 3a20 226e 6f6e 6522  ckground: "none"
-0005c1b0: 3b2d 2d72 696f 2d6c 6f63 616c 2d68 6561  ;--rio-local-hea
-0005c1c0: 6469 6e67 332d 6261 636b 6772 6f75 6e64  ding3-background
-0005c1d0: 2d63 6c69 703a 2022 626f 7264 6572 2d62  -clip: "border-b
-0005c1e0: 6f78 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  ox";--rio-local-
-0005c1f0: 6865 6164 696e 6733 2d66 696c 6c2d 636f  heading3-fill-co
-0005c200: 6c6f 723a 2022 7472 616e 7370 6172 656e  lor: "transparen
-0005c210: 7422 3b2d 2d72 696f 2d6c 6f63 616c 2d74  t";--rio-local-t
-0005c220: 6578 742d 636f 6c6f 723a 2076 6172 282d  ext-color: var(-
-0005c230: 2d72 696f 2d6c 6f63 616c 2d66 6729 3b2d  -rio-local-fg);-
-0005c240: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
-0005c250: 6261 636b 6772 6f75 6e64 3a20 226e 6f6e  background: "non
-0005c260: 6522 3b2d 2d72 696f 2d6c 6f63 616c 2d74  e";--rio-local-t
-0005c270: 6578 742d 6261 636b 6772 6f75 6e64 2d63  ext-background-c
-0005c280: 6c69 703a 2022 626f 7264 6572 2d62 6f78  lip: "border-box
-0005c290: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  ";--rio-local-te
-0005c2a0: 7874 2d66 696c 6c2d 636f 6c6f 723a 2022  xt-fill-color: "
-0005c2b0: 7472 616e 7370 6172 656e 7422 3b63 6f6c  transparent";col
-0005c2c0: 6f72 3a76 6172 282d 2d72 696f 2d6c 6f63  or:var(--rio-loc
-0005c2d0: 616c 2d66 6729 7d68 746d 6c5b 6461 7461  al-fg)}html[data
-0005c2e0: 2d74 6865 6d65 3d6c 6967 6874 5d20 7072  -theme=light] pr
-0005c2f0: 6520 636f 6465 2e68 6c6a 737b 6469 7370  e code.hljs{disp
-0005c300: 6c61 793a 626c 6f63 6b3b 6f76 6572 666c  lay:block;overfl
-0005c310: 6f77 2d78 3a61 7574 6f3b 7061 6464 696e  ow-x:auto;paddin
-0005c320: 673a 3172 656d 7d68 746d 6c5b 6461 7461  g:1rem}html[data
-0005c330: 2d74 6865 6d65 3d6c 6967 6874 5d20 636f  -theme=light] co
-0005c340: 6465 2e68 6c6a 737b 7061 6464 696e 673a  de.hljs{padding:
-0005c350: 3370 7820 3570 787d 6874 6d6c 5b64 6174  3px 5px}html[dat
-0005c360: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
-0005c370: 686c 6a73 7b62 6163 6b67 726f 756e 643a  hljs{background:
-0005c380: 2366 3366 3366 333b 636f 6c6f 723a 2334  #f3f3f3;color:#4
-0005c390: 3434 7d68 746d 6c5b 6461 7461 2d74 6865  44}html[data-the
-0005c3a0: 6d65 3d6c 6967 6874 5d20 2e68 6c6a 732d  me=light] .hljs-
-0005c3b0: 636f 6d6d 656e 747b 636f 6c6f 723a 2336  comment{color:#6
-0005c3c0: 3937 3037 307d 6874 6d6c 5b64 6174 612d  97070}html[data-
-0005c3d0: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c3e0: 6a73 2d70 756e 6374 7561 7469 6f6e 2c68  js-punctuation,h
-0005c3f0: 746d 6c5b 6461 7461 2d74 6865 6d65 3d6c  tml[data-theme=l
-0005c400: 6967 6874 5d20 2e68 6c6a 732d 7461 677b  ight] .hljs-tag{
-0005c410: 636f 6c6f 723a 2334 3434 617d 6874 6d6c  color:#444a}html
-0005c420: 5b64 6174 612d 7468 656d 653d 6c69 6768  [data-theme=ligh
-0005c430: 745d 202e 686c 6a73 2d74 6167 202e 686c  t] .hljs-tag .hl
-0005c440: 6a73 2d61 7474 722c 6874 6d6c 5b64 6174  js-attr,html[dat
-0005c450: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
-0005c460: 686c 6a73 2d74 6167 202e 686c 6a73 2d6e  hljs-tag .hljs-n
-0005c470: 616d 657b 636f 6c6f 723a 2334 3434 7d68  ame{color:#444}h
-0005c480: 746d 6c5b 6461 7461 2d74 6865 6d65 3d6c  tml[data-theme=l
-0005c490: 6967 6874 5d20 2e68 6c6a 732d 6174 7472  ight] .hljs-attr
-0005c4a0: 6962 7574 652c 6874 6d6c 5b64 6174 612d  ibute,html[data-
-0005c4b0: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c4c0: 6a73 2d64 6f63 7461 672c 6874 6d6c 5b64  js-doctag,html[d
-0005c4d0: 6174 612d 7468 656d 653d 6c69 6768 745d  ata-theme=light]
-0005c4e0: 202e 686c 6a73 2d6b 6579 776f 7264 2c68   .hljs-keyword,h
-0005c4f0: 746d 6c5b 6461 7461 2d74 6865 6d65 3d6c  tml[data-theme=l
-0005c500: 6967 6874 5d20 2e68 6c6a 732d 6d65 7461  ight] .hljs-meta
-0005c510: 202e 686c 6a73 2d6b 6579 776f 7264 2c68   .hljs-keyword,h
-0005c520: 746d 6c5b 6461 7461 2d74 6865 6d65 3d6c  tml[data-theme=l
-0005c530: 6967 6874 5d20 2e68 6c6a 732d 6e61 6d65  ight] .hljs-name
-0005c540: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
-0005c550: 3d6c 6967 6874 5d20 2e68 6c6a 732d 7365  =light] .hljs-se
-0005c560: 6c65 6374 6f72 2d74 6167 7b66 6f6e 742d  lector-tag{font-
-0005c570: 7765 6967 6874 3a37 3030 7d68 746d 6c5b  weight:700}html[
-0005c580: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
-0005c590: 5d20 2e68 6c6a 732d 6465 6c65 7469 6f6e  ] .hljs-deletion
-0005c5a0: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
-0005c5b0: 3d6c 6967 6874 5d20 2e68 6c6a 732d 6e75  =light] .hljs-nu
-0005c5c0: 6d62 6572 2c68 746d 6c5b 6461 7461 2d74  mber,html[data-t
-0005c5d0: 6865 6d65 3d6c 6967 6874 5d20 2e68 6c6a  heme=light] .hlj
-0005c5e0: 732d 7175 6f74 652c 6874 6d6c 5b64 6174  s-quote,html[dat
-0005c5f0: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
-0005c600: 686c 6a73 2d73 656c 6563 746f 722d 636c  hljs-selector-cl
-0005c610: 6173 732c 6874 6d6c 5b64 6174 612d 7468  ass,html[data-th
-0005c620: 656d 653d 6c69 6768 745d 202e 686c 6a73  eme=light] .hljs
-0005c630: 2d73 656c 6563 746f 722d 6964 2c68 746d  -selector-id,htm
-0005c640: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
-0005c650: 6874 5d20 2e68 6c6a 732d 7374 7269 6e67  ht] .hljs-string
-0005c660: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
-0005c670: 3d6c 6967 6874 5d20 2e68 6c6a 732d 7465  =light] .hljs-te
-0005c680: 6d70 6c61 7465 2d74 6167 2c68 746d 6c5b  mplate-tag,html[
-0005c690: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
-0005c6a0: 5d20 2e68 6c6a 732d 7479 7065 7b63 6f6c  ] .hljs-type{col
-0005c6b0: 6f72 3a23 3830 307d 6874 6d6c 5b64 6174  or:#800}html[dat
-0005c6c0: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
-0005c6d0: 686c 6a73 2d73 6563 7469 6f6e 2c68 746d  hljs-section,htm
-0005c6e0: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
-0005c6f0: 6874 5d20 2e68 6c6a 732d 7469 746c 657b  ht] .hljs-title{
-0005c700: 636f 6c6f 723a 2338 3030 3b66 6f6e 742d  color:#800;font-
-0005c710: 7765 6967 6874 3a37 3030 7d68 746d 6c5b  weight:700}html[
-0005c720: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
-0005c730: 5d20 2e68 6c6a 732d 6c69 6e6b 2c68 746d  ] .hljs-link,htm
-0005c740: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
-0005c750: 6874 5d20 2e68 6c6a 732d 6f70 6572 6174  ht] .hljs-operat
-0005c760: 6f72 2c68 746d 6c5b 6461 7461 2d74 6865  or,html[data-the
-0005c770: 6d65 3d6c 6967 6874 5d20 2e68 6c6a 732d  me=light] .hljs-
-0005c780: 7265 6765 7870 2c68 746d 6c5b 6461 7461  regexp,html[data
-0005c790: 2d74 6865 6d65 3d6c 6967 6874 5d20 2e68  -theme=light] .h
-0005c7a0: 6c6a 732d 7365 6c65 6374 6f72 2d61 7474  ljs-selector-att
-0005c7b0: 722c 6874 6d6c 5b64 6174 612d 7468 656d  r,html[data-them
-0005c7c0: 653d 6c69 6768 745d 202e 686c 6a73 2d73  e=light] .hljs-s
-0005c7d0: 656c 6563 746f 722d 7073 6575 646f 2c68  elector-pseudo,h
-0005c7e0: 746d 6c5b 6461 7461 2d74 6865 6d65 3d6c  tml[data-theme=l
-0005c7f0: 6967 6874 5d20 2e68 6c6a 732d 7379 6d62  ight] .hljs-symb
-0005c800: 6f6c 2c68 746d 6c5b 6461 7461 2d74 6865  ol,html[data-the
-0005c810: 6d65 3d6c 6967 6874 5d20 2e68 6c6a 732d  me=light] .hljs-
-0005c820: 7465 6d70 6c61 7465 2d76 6172 6961 626c  template-variabl
-0005c830: 652c 6874 6d6c 5b64 6174 612d 7468 656d  e,html[data-them
-0005c840: 653d 6c69 6768 745d 202e 686c 6a73 2d76  e=light] .hljs-v
-0005c850: 6172 6961 626c 657b 636f 6c6f 723a 2361  ariable{color:#a
-0005c860: 6235 3635 367d 6874 6d6c 5b64 6174 612d  b5656}html[data-
-0005c870: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c880: 6a73 2d6c 6974 6572 616c 7b63 6f6c 6f72  js-literal{color
-0005c890: 3a23 3639 357d 6874 6d6c 5b64 6174 612d  :#695}html[data-
-0005c8a0: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c8b0: 6a73 2d61 6464 6974 696f 6e2c 6874 6d6c  js-addition,html
-0005c8c0: 5b64 6174 612d 7468 656d 653d 6c69 6768  [data-theme=ligh
-0005c8d0: 745d 202e 686c 6a73 2d62 7569 6c74 5f69  t] .hljs-built_i
-0005c8e0: 6e2c 6874 6d6c 5b64 6174 612d 7468 656d  n,html[data-them
-0005c8f0: 653d 6c69 6768 745d 202e 686c 6a73 2d62  e=light] .hljs-b
-0005c900: 756c 6c65 742c 6874 6d6c 5b64 6174 612d  ullet,html[data-
-0005c910: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c920: 6a73 2d63 6f64 657b 636f 6c6f 723a 2333  js-code{color:#3
-0005c930: 3937 3330 307d 6874 6d6c 5b64 6174 612d  97300}html[data-
-0005c940: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c950: 6a73 2d6d 6574 617b 636f 6c6f 723a 2331  js-meta{color:#1
-0005c960: 6637 3139 397d 6874 6d6c 5b64 6174 612d  f7199}html[data-
-0005c970: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
-0005c980: 6a73 2d6d 6574 6120 2e68 6c6a 732d 7374  js-meta .hljs-st
-0005c990: 7269 6e67 7b63 6f6c 6f72 3a23 3338 617d  ring{color:#38a}
-0005c9a0: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
-0005c9b0: 6c69 6768 745d 202e 686c 6a73 2d65 6d70  light] .hljs-emp
-0005c9c0: 6861 7369 737b 666f 6e74 2d73 7479 6c65  hasis{font-style
-0005c9d0: 3a69 7461 6c69 637d 6874 6d6c 5b64 6174  :italic}html[dat
-0005c9e0: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
-0005c9f0: 686c 6a73 2d73 7472 6f6e 677b 666f 6e74  hljs-strong{font
-0005ca00: 2d77 6569 6768 743a 3730 307d 6874 6d6c  -weight:700}html
-0005ca10: 5b64 6174 612d 7468 656d 653d 6461 726b  [data-theme=dark
-0005ca20: 5d20 2e68 6c6a 737b 636f 6c6f 723a 2364  ] .hljs{color:#d
-0005ca30: 6464 3b62 6163 6b67 726f 756e 643a 2333  dd;background:#3
-0005ca40: 3033 3033 307d 6874 6d6c 5b64 6174 612d  03030}html[data-
-0005ca50: 7468 656d 653d 6461 726b 5d20 2e68 6c6a  theme=dark] .hlj
-0005ca60: 732d 6b65 7977 6f72 642c 6874 6d6c 5b64  s-keyword,html[d
-0005ca70: 6174 612d 7468 656d 653d 6461 726b 5d20  ata-theme=dark] 
-0005ca80: 2e68 6c6a 732d 7365 6c65 6374 6f72 2d74  .hljs-selector-t
-0005ca90: 6167 2c68 746d 6c5b 6461 7461 2d74 6865  ag,html[data-the
-0005caa0: 6d65 3d64 6172 6b5d 202e 686c 6a73 2d6c  me=dark] .hljs-l
-0005cab0: 6974 6572 616c 2c68 746d 6c5b 6461 7461  iteral,html[data
-0005cac0: 2d74 6865 6d65 3d64 6172 6b5d 202e 686c  -theme=dark] .hl
-0005cad0: 6a73 2d73 6563 7469 6f6e 2c68 746d 6c5b  js-section,html[
-0005cae0: 6461 7461 2d74 6865 6d65 3d64 6172 6b5d  data-theme=dark]
-0005caf0: 202e 686c 6a73 2d6c 696e 6b7b 636f 6c6f   .hljs-link{colo
-0005cb00: 723a 2366 6666 7d68 746d 6c5b 6461 7461  r:#fff}html[data
-0005cb10: 2d74 6865 6d65 3d64 6172 6b5d 202e 686c  -theme=dark] .hl
-0005cb20: 6a73 2d73 7472 696e 672c 6874 6d6c 5b64  js-string,html[d
-0005cb30: 6174 612d 7468 656d 653d 6461 726b 5d20  ata-theme=dark] 
-0005cb40: 2e68 6c6a 732d 7469 746c 652c 6874 6d6c  .hljs-title,html
-0005cb50: 5b64 6174 612d 7468 656d 653d 6461 726b  [data-theme=dark
-0005cb60: 5d20 2e68 6c6a 732d 6e61 6d65 2c68 746d  ] .hljs-name,htm
-0005cb70: 6c5b 6461 7461 2d74 6865 6d65 3d64 6172  l[data-theme=dar
-0005cb80: 6b5d 202e 686c 6a73 2d74 7970 652c 6874  k] .hljs-type,ht
-0005cb90: 6d6c 5b64 6174 612d 7468 656d 653d 6461  ml[data-theme=da
-0005cba0: 726b 5d20 2e68 6c6a 732d 6174 7472 6962  rk] .hljs-attrib
-0005cbb0: 7574 652c 6874 6d6c 5b64 6174 612d 7468  ute,html[data-th
-0005cbc0: 656d 653d 6461 726b 5d20 2e68 6c6a 732d  eme=dark] .hljs-
-0005cbd0: 7379 6d62 6f6c 2c68 746d 6c5b 6461 7461  symbol,html[data
-0005cbe0: 2d74 6865 6d65 3d64 6172 6b5d 202e 686c  -theme=dark] .hl
-0005cbf0: 6a73 2d62 756c 6c65 742c 6874 6d6c 5b64  js-bullet,html[d
-0005cc00: 6174 612d 7468 656d 653d 6461 726b 5d20  ata-theme=dark] 
-0005cc10: 2e68 6c6a 732d 6275 696c 745f 696e 2c68  .hljs-built_in,h
-0005cc20: 746d 6c5b 6461 7461 2d74 6865 6d65 3d64  tml[data-theme=d
-0005cc30: 6172 6b5d 202e 686c 6a73 2d61 6464 6974  ark] .hljs-addit
-0005cc40: 696f 6e2c 6874 6d6c 5b64 6174 612d 7468  ion,html[data-th
-0005cc50: 656d 653d 6461 726b 5d20 2e68 6c6a 732d  eme=dark] .hljs-
-0005cc60: 7661 7269 6162 6c65 2c68 746d 6c5b 6461  variable,html[da
-0005cc70: 7461 2d74 6865 6d65 3d64 6172 6b5d 202e  ta-theme=dark] .
-0005cc80: 686c 6a73 2d74 656d 706c 6174 652d 7461  hljs-template-ta
-0005cc90: 672c 6874 6d6c 5b64 6174 612d 7468 656d  g,html[data-them
-0005cca0: 653d 6461 726b 5d20 2e68 6c6a 732d 7465  e=dark] .hljs-te
-0005ccb0: 6d70 6c61 7465 2d76 6172 6961 626c 657b  mplate-variable{
-0005ccc0: 636f 6c6f 723a 2364 3838 7d68 746d 6c5b  color:#d88}html[
-0005ccd0: 6461 7461 2d74 6865 6d65 3d64 6172 6b5d  data-theme=dark]
-0005cce0: 202e 686c 6a73 2d63 6f6d 6d65 6e74 2c68   .hljs-comment,h
-0005ccf0: 746d 6c5b 6461 7461 2d74 6865 6d65 3d64  tml[data-theme=d
-0005cd00: 6172 6b5d 202e 686c 6a73 2d71 756f 7465  ark] .hljs-quote
-0005cd10: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
-0005cd20: 3d64 6172 6b5d 202e 686c 6a73 2d64 656c  =dark] .hljs-del
-0005cd30: 6574 696f 6e2c 6874 6d6c 5b64 6174 612d  etion,html[data-
-0005cd40: 7468 656d 653d 6461 726b 5d20 2e68 6c6a  theme=dark] .hlj
-0005cd50: 732d 6d65 7461 7b63 6f6c 6f72 3a23 3937  s-meta{color:#97
-0005cd60: 3937 3937 7d68 746d 6c5b 6461 7461 2d74  9797}html[data-t
-0005cd70: 6865 6d65 3d64 6172 6b5d 202e 686c 6a73  heme=dark] .hljs
-0005cd80: 2d6b 6579 776f 7264 2c68 746d 6c5b 6461  -keyword,html[da
-0005cd90: 7461 2d74 6865 6d65 3d64 6172 6b5d 202e  ta-theme=dark] .
-0005cda0: 686c 6a73 2d73 656c 6563 746f 722d 7461  hljs-selector-ta
-0005cdb0: 672c 6874 6d6c 5b64 6174 612d 7468 656d  g,html[data-them
-0005cdc0: 653d 6461 726b 5d20 2e68 6c6a 732d 6c69  e=dark] .hljs-li
-0005cdd0: 7465 7261 6c2c 6874 6d6c 5b64 6174 612d  teral,html[data-
-0005cde0: 7468 656d 653d 6461 726b 5d20 2e68 6c6a  theme=dark] .hlj
-0005cdf0: 732d 7469 746c 652c 6874 6d6c 5b64 6174  s-title,html[dat
-0005ce00: 612d 7468 656d 653d 6461 726b 5d20 2e68  a-theme=dark] .h
-0005ce10: 6c6a 732d 7365 6374 696f 6e2c 6874 6d6c  ljs-section,html
-0005ce20: 5b64 6174 612d 7468 656d 653d 6461 726b  [data-theme=dark
-0005ce30: 5d20 2e68 6c6a 732d 646f 6374 6167 2c68  ] .hljs-doctag,h
-0005ce40: 746d 6c5b 6461 7461 2d74 6865 6d65 3d64  tml[data-theme=d
-0005ce50: 6172 6b5d 202e 686c 6a73 2d74 7970 652c  ark] .hljs-type,
-0005ce60: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
-0005ce70: 6461 726b 5d20 2e68 6c6a 732d 6e61 6d65  dark] .hljs-name
-0005ce80: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
-0005ce90: 3d64 6172 6b5d 202e 686c 6a73 2d73 7472  =dark] .hljs-str
-0005cea0: 6f6e 677b 666f 6e74 2d77 6569 6768 743a  ong{font-weight:
-0005ceb0: 3730 307d 6874 6d6c 5b64 6174 612d 7468  700}html[data-th
+0005b660: 7365 636f 6e64 6172 792d 6267 2d61 6374  secondary-bg-act
+0005b670: 6976 6529 3b2d 2d72 696f 2d6c 6f63 616c  ive);--rio-local
+0005b680: 2d6c 6576 656c 2d32 2d66 673a 2076 6172  -level-2-fg: var
+0005b690: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
+0005b6a0: 636f 6e64 6172 792d 6667 293b 2d2d 7269  condary-fg);--ri
+0005b6b0: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 332d  o-local-level-3-
+0005b6c0: 6267 3a20 7661 7228 2d2d 7269 6f2d 676c  bg: var(--rio-gl
+0005b6d0: 6f62 616c 2d70 7269 6d61 7279 2d62 6729  obal-primary-bg)
+0005b6e0: 3b2d 2d72 696f 2d6c 6f63 616c 2d6c 6576  ;--rio-local-lev
+0005b6f0: 656c 2d33 2d62 672d 7661 7269 616e 743a  el-3-bg-variant:
+0005b700: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+0005b710: 6c2d 7072 696d 6172 792d 6267 2d76 6172  l-primary-bg-var
+0005b720: 6961 6e74 293b 2d2d 7269 6f2d 6c6f 6361  iant);--rio-loca
+0005b730: 6c2d 6c65 7665 6c2d 332d 6267 2d61 6374  l-level-3-bg-act
+0005b740: 6976 653a 2076 6172 282d 2d72 696f 2d67  ive: var(--rio-g
+0005b750: 6c6f 6261 6c2d 7072 696d 6172 792d 6267  lobal-primary-bg
+0005b760: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
+0005b770: 6f63 616c 2d6c 6576 656c 2d33 2d66 673a  ocal-level-3-fg:
+0005b780: 2076 6172 282d 2d72 696f 2d67 6c6f 6261   var(--rio-globa
+0005b790: 6c2d 7072 696d 6172 792d 6667 293b 2d2d  l-primary-fg);--
+0005b7a0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005b7b0: 6731 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g1-color: var(--
+0005b7c0: 7269 6f2d 6c6f 6361 6c2d 6667 293b 2d2d  rio-local-fg);--
+0005b7d0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005b7e0: 6731 2d62 6163 6b67 726f 756e 643a 2022  g1-background: "
+0005b7f0: 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f 6361  none";--rio-loca
+0005b800: 6c2d 6865 6164 696e 6731 2d62 6163 6b67  l-heading1-backg
+0005b810: 726f 756e 642d 636c 6970 3a20 2262 6f72  round-clip: "bor
+0005b820: 6465 722d 626f 7822 3b2d 2d72 696f 2d6c  der-box";--rio-l
+0005b830: 6f63 616c 2d68 6561 6469 6e67 312d 6669  ocal-heading1-fi
+0005b840: 6c6c 2d63 6f6c 6f72 3a20 2274 7261 6e73  ll-color: "trans
+0005b850: 7061 7265 6e74 223b 2d2d 7269 6f2d 6c6f  parent";--rio-lo
+0005b860: 6361 6c2d 6865 6164 696e 6732 2d63 6f6c  cal-heading2-col
+0005b870: 6f72 3a20 7661 7228 2d2d 7269 6f2d 6c6f  or: var(--rio-lo
+0005b880: 6361 6c2d 6667 293b 2d2d 7269 6f2d 6c6f  cal-fg);--rio-lo
+0005b890: 6361 6c2d 6865 6164 696e 6732 2d62 6163  cal-heading2-bac
+0005b8a0: 6b67 726f 756e 643a 2022 6e6f 6e65 223b  kground: "none";
+0005b8b0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
+0005b8c0: 696e 6732 2d62 6163 6b67 726f 756e 642d  ing2-background-
+0005b8d0: 636c 6970 3a20 2262 6f72 6465 722d 626f  clip: "border-bo
+0005b8e0: 7822 3b2d 2d72 696f 2d6c 6f63 616c 2d68  x";--rio-local-h
+0005b8f0: 6561 6469 6e67 322d 6669 6c6c 2d63 6f6c  eading2-fill-col
+0005b900: 6f72 3a20 2274 7261 6e73 7061 7265 6e74  or: "transparent
+0005b910: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
+0005b920: 6164 696e 6733 2d63 6f6c 6f72 3a20 7661  ading3-color: va
+0005b930: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6667  r(--rio-local-fg
+0005b940: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  );--rio-local-he
+0005b950: 6164 696e 6733 2d62 6163 6b67 726f 756e  ading3-backgroun
+0005b960: 643a 2022 6e6f 6e65 223b 2d2d 7269 6f2d  d: "none";--rio-
+0005b970: 6c6f 6361 6c2d 6865 6164 696e 6733 2d62  local-heading3-b
+0005b980: 6163 6b67 726f 756e 642d 636c 6970 3a20  ackground-clip: 
+0005b990: 2262 6f72 6465 722d 626f 7822 3b2d 2d72  "border-box";--r
+0005b9a0: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
+0005b9b0: 332d 6669 6c6c 2d63 6f6c 6f72 3a20 2274  3-fill-color: "t
+0005b9c0: 7261 6e73 7061 7265 6e74 223b 2d2d 7269  ransparent";--ri
+0005b9d0: 6f2d 6c6f 6361 6c2d 7465 7874 2d63 6f6c  o-local-text-col
+0005b9e0: 6f72 3a20 7661 7228 2d2d 7269 6f2d 6c6f  or: var(--rio-lo
+0005b9f0: 6361 6c2d 6667 293b 2d2d 7269 6f2d 6c6f  cal-fg);--rio-lo
+0005ba00: 6361 6c2d 7465 7874 2d62 6163 6b67 726f  cal-text-backgro
+0005ba10: 756e 643a 2022 6e6f 6e65 223b 2d2d 7269  und: "none";--ri
+0005ba20: 6f2d 6c6f 6361 6c2d 7465 7874 2d62 6163  o-local-text-bac
+0005ba30: 6b67 726f 756e 642d 636c 6970 3a20 2262  kground-clip: "b
+0005ba40: 6f72 6465 722d 626f 7822 3b2d 2d72 696f  order-box";--rio
+0005ba50: 2d6c 6f63 616c 2d74 6578 742d 6669 6c6c  -local-text-fill
+0005ba60: 2d63 6f6c 6f72 3a20 2274 7261 6e73 7061  -color: "transpa
+0005ba70: 7265 6e74 223b 636f 6c6f 723a 7661 7228  rent";color:var(
+0005ba80: 2d2d 7269 6f2d 6c6f 6361 6c2d 6667 297d  --rio-local-fg)}
+0005ba90: 2e72 696f 2d73 7769 7463 6865 726f 6f2d  .rio-switcheroo-
+0005baa0: 6261 636b 6772 6f75 6e64 3e2a 2c2e 7269  background>*,.ri
+0005bab0: 6f2d 7377 6974 6368 6572 6f6f 2d6e 6575  o-switcheroo-neu
+0005bac0: 7472 616c 3e2a 2c2e 7269 6f2d 7377 6974  tral>*,.rio-swit
+0005bad0: 6368 6572 6f6f 2d68 7564 3e2a 2c2e 7269  cheroo-hud>*,.ri
+0005bae0: 6f2d 7377 6974 6368 6572 6f6f 2d70 7269  o-switcheroo-pri
+0005baf0: 6d61 7279 3e2a 2c2e 7269 6f2d 7377 6974  mary>*,.rio-swit
+0005bb00: 6368 6572 6f6f 2d73 6563 6f6e 6461 7279  cheroo-secondary
+0005bb10: 3e2a 2c2e 7269 6f2d 7377 6974 6368 6572  >*,.rio-switcher
+0005bb20: 6f6f 2d73 7563 6365 7373 3e2a 2c2e 7269  oo-success>*,.ri
+0005bb30: 6f2d 7377 6974 6368 6572 6f6f 2d77 6172  o-switcheroo-war
+0005bb40: 6e69 6e67 3e2a 2c2e 7269 6f2d 7377 6974  ning>*,.rio-swit
+0005bb50: 6368 6572 6f6f 2d64 616e 6765 723e 2a2c  cheroo-danger>*,
+0005bb60: 2e72 696f 2d73 7769 7463 6865 726f 6f2d  .rio-switcheroo-
+0005bb70: 6469 7361 626c 6564 3e2a 2c2e 7269 6f2d  disabled>*,.rio-
+0005bb80: 7377 6974 6368 6572 6f6f 2d63 7573 746f  switcheroo-custo
+0005bb90: 6d3e 2a2c 2e72 696f 2d73 7769 7463 6865  m>*,.rio-switche
+0005bba0: 726f 6f2d 6275 6d70 3e2a 7b2d 2d72 696f  roo-bump>*{--rio
+0005bbb0: 2d62 7566 6665 722d 6c65 7665 6c2d 322d  -buffer-level-2-
+0005bbc0: 6267 3a20 7661 7228 2d2d 7269 6f2d 6c6f  bg: var(--rio-lo
+0005bbd0: 6361 6c2d 6c65 7665 6c2d 322d 6267 293b  cal-level-2-bg);
+0005bbe0: 2d2d 7269 6f2d 6275 6666 6572 2d6c 6576  --rio-buffer-lev
+0005bbf0: 656c 2d32 2d62 672d 7661 7269 616e 743a  el-2-bg-variant:
+0005bc00: 2076 6172 282d 2d72 696f 2d6c 6f63 616c   var(--rio-local
+0005bc10: 2d6c 6576 656c 2d32 2d62 672d 7661 7269  -level-2-bg-vari
+0005bc20: 616e 7429 3b2d 2d72 696f 2d62 7566 6665  ant);--rio-buffe
+0005bc30: 722d 6c65 7665 6c2d 322d 6267 2d61 6374  r-level-2-bg-act
+0005bc40: 6976 653a 2076 6172 282d 2d72 696f 2d6c  ive: var(--rio-l
+0005bc50: 6f63 616c 2d6c 6576 656c 2d32 2d62 672d  ocal-level-2-bg-
+0005bc60: 6163 7469 7665 293b 2d2d 7269 6f2d 6275  active);--rio-bu
+0005bc70: 6666 6572 2d6c 6576 656c 2d32 2d66 673a  ffer-level-2-fg:
+0005bc80: 2076 6172 282d 2d72 696f 2d6c 6f63 616c   var(--rio-local
+0005bc90: 2d6c 6576 656c 2d32 2d66 6729 3b2d 2d72  -level-2-fg);--r
+0005bca0: 696f 2d62 7566 6665 722d 6c65 7665 6c2d  io-buffer-level-
+0005bcb0: 332d 6267 3a20 7661 7228 2d2d 7269 6f2d  3-bg: var(--rio-
+0005bcc0: 6c6f 6361 6c2d 6c65 7665 6c2d 332d 6267  local-level-3-bg
+0005bcd0: 293b 2d2d 7269 6f2d 6275 6666 6572 2d6c  );--rio-buffer-l
+0005bce0: 6576 656c 2d33 2d62 672d 7661 7269 616e  evel-3-bg-varian
+0005bcf0: 743a 2076 6172 282d 2d72 696f 2d6c 6f63  t: var(--rio-loc
+0005bd00: 616c 2d6c 6576 656c 2d33 2d62 672d 7661  al-level-3-bg-va
+0005bd10: 7269 616e 7429 3b2d 2d72 696f 2d62 7566  riant);--rio-buf
+0005bd20: 6665 722d 6c65 7665 6c2d 332d 6267 2d61  fer-level-3-bg-a
+0005bd30: 6374 6976 653a 2076 6172 282d 2d72 696f  ctive: var(--rio
+0005bd40: 2d6c 6f63 616c 2d6c 6576 656c 2d33 2d62  -local-level-3-b
+0005bd50: 672d 6163 7469 7665 293b 2d2d 7269 6f2d  g-active);--rio-
+0005bd60: 6275 6666 6572 2d6c 6576 656c 2d33 2d66  buffer-level-3-f
+0005bd70: 673a 2076 6172 282d 2d72 696f 2d6c 6f63  g: var(--rio-loc
+0005bd80: 616c 2d6c 6576 656c 2d33 2d66 6729 7d2e  al-level-3-fg)}.
+0005bd90: 7269 6f2d 7377 6974 6368 6572 6f6f 2d62  rio-switcheroo-b
+0005bda0: 756d 707b 2d2d 7269 6f2d 6c6f 6361 6c2d  ump{--rio-local-
+0005bdb0: 6267 3a20 7661 7228 2d2d 7269 6f2d 6275  bg: var(--rio-bu
+0005bdc0: 6666 6572 2d6c 6576 656c 2d32 2d62 6729  ffer-level-2-bg)
+0005bdd0: 3b2d 2d72 696f 2d6c 6f63 616c 2d62 672d  ;--rio-local-bg-
+0005bde0: 7661 7269 616e 743a 2076 6172 282d 2d72  variant: var(--r
+0005bdf0: 696f 2d62 7566 6665 722d 6c65 7665 6c2d  io-buffer-level-
+0005be00: 322d 6267 2d76 6172 6961 6e74 293b 2d2d  2-bg-variant);--
+0005be10: 7269 6f2d 6c6f 6361 6c2d 6267 2d61 6374  rio-local-bg-act
+0005be20: 6976 653a 2076 6172 282d 2d72 696f 2d62  ive: var(--rio-b
+0005be30: 7566 6665 722d 6c65 7665 6c2d 322d 6267  uffer-level-2-bg
+0005be40: 2d61 6374 6976 6529 3b2d 2d72 696f 2d6c  -active);--rio-l
+0005be50: 6f63 616c 2d66 673a 2076 6172 282d 2d72  ocal-fg: var(--r
+0005be60: 696f 2d62 7566 6665 722d 6c65 7665 6c2d  io-buffer-level-
+0005be70: 322d 6667 293b 2d2d 7269 6f2d 6c6f 6361  2-fg);--rio-loca
+0005be80: 6c2d 6c65 7665 6c2d 322d 6267 3a20 7661  l-level-2-bg: va
+0005be90: 7228 2d2d 7269 6f2d 6275 6666 6572 2d6c  r(--rio-buffer-l
+0005bea0: 6576 656c 2d33 2d62 6729 3b2d 2d72 696f  evel-3-bg);--rio
+0005beb0: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
+0005bec0: 672d 7661 7269 616e 743a 2076 6172 282d  g-variant: var(-
+0005bed0: 2d72 696f 2d62 7566 6665 722d 6c65 7665  -rio-buffer-leve
+0005bee0: 6c2d 332d 6267 2d76 6172 6961 6e74 293b  l-3-bg-variant);
+0005bef0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+0005bf00: 6c2d 322d 6267 2d61 6374 6976 653a 2076  l-2-bg-active: v
+0005bf10: 6172 282d 2d72 696f 2d62 7566 6665 722d  ar(--rio-buffer-
+0005bf20: 6c65 7665 6c2d 332d 6267 2d61 6374 6976  level-3-bg-activ
+0005bf30: 6529 3b2d 2d72 696f 2d6c 6f63 616c 2d6c  e);--rio-local-l
+0005bf40: 6576 656c 2d32 2d66 673a 2076 6172 282d  evel-2-fg: var(-
+0005bf50: 2d72 696f 2d62 7566 6665 722d 6c65 7665  -rio-buffer-leve
+0005bf60: 6c2d 332d 6667 293b 2d2d 7269 6f2d 6c6f  l-3-fg);--rio-lo
+0005bf70: 6361 6c2d 6c65 7665 6c2d 332d 6267 3a20  cal-level-3-bg: 
+0005bf80: 7661 7228 2d2d 7269 6f2d 6275 6666 6572  var(--rio-buffer
+0005bf90: 2d6c 6576 656c 2d32 2d62 6729 3b2d 2d72  -level-2-bg);--r
+0005bfa0: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d33  io-local-level-3
+0005bfb0: 2d62 672d 7661 7269 616e 743a 2076 6172  -bg-variant: var
+0005bfc0: 282d 2d72 696f 2d62 7566 6665 722d 6c65  (--rio-buffer-le
+0005bfd0: 7665 6c2d 322d 6267 2d76 6172 6961 6e74  vel-2-bg-variant
+0005bfe0: 293b 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  );--rio-local-le
+0005bff0: 7665 6c2d 332d 6267 2d61 6374 6976 653a  vel-3-bg-active:
+0005c000: 2076 6172 282d 2d72 696f 2d62 7566 6665   var(--rio-buffe
+0005c010: 722d 6c65 7665 6c2d 322d 6267 2d61 6374  r-level-2-bg-act
+0005c020: 6976 6529 3b2d 2d72 696f 2d6c 6f63 616c  ive);--rio-local
+0005c030: 2d6c 6576 656c 2d33 2d66 673a 2076 6172  -level-3-fg: var
+0005c040: 282d 2d72 696f 2d62 7566 6665 722d 6c65  (--rio-buffer-le
+0005c050: 7665 6c2d 322d 6667 293b 2d2d 7269 6f2d  vel-2-fg);--rio-
+0005c060: 6c6f 6361 6c2d 6865 6164 696e 6731 2d63  local-heading1-c
+0005c070: 6f6c 6f72 3a20 7661 7228 2d2d 7269 6f2d  olor: var(--rio-
+0005c080: 6c6f 6361 6c2d 6667 293b 2d2d 7269 6f2d  local-fg);--rio-
+0005c090: 6c6f 6361 6c2d 6865 6164 696e 6731 2d62  local-heading1-b
+0005c0a0: 6163 6b67 726f 756e 643a 2022 6e6f 6e65  ackground: "none
+0005c0b0: 223b 2d2d 7269 6f2d 6c6f 6361 6c2d 6865  ";--rio-local-he
+0005c0c0: 6164 696e 6731 2d62 6163 6b67 726f 756e  ading1-backgroun
+0005c0d0: 642d 636c 6970 3a20 2262 6f72 6465 722d  d-clip: "border-
+0005c0e0: 626f 7822 3b2d 2d72 696f 2d6c 6f63 616c  box";--rio-local
+0005c0f0: 2d68 6561 6469 6e67 312d 6669 6c6c 2d63  -heading1-fill-c
+0005c100: 6f6c 6f72 3a20 2274 7261 6e73 7061 7265  olor: "transpare
+0005c110: 6e74 223b 2d2d 7269 6f2d 6c6f 6361 6c2d  nt";--rio-local-
+0005c120: 6865 6164 696e 6732 2d63 6f6c 6f72 3a20  heading2-color: 
+0005c130: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+0005c140: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
+0005c150: 6865 6164 696e 6732 2d62 6163 6b67 726f  heading2-backgro
+0005c160: 756e 643a 2022 6e6f 6e65 223b 2d2d 7269  und: "none";--ri
+0005c170: 6f2d 6c6f 6361 6c2d 6865 6164 696e 6732  o-local-heading2
+0005c180: 2d62 6163 6b67 726f 756e 642d 636c 6970  -background-clip
+0005c190: 3a20 2262 6f72 6465 722d 626f 7822 3b2d  : "border-box";-
+0005c1a0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
+0005c1b0: 6e67 322d 6669 6c6c 2d63 6f6c 6f72 3a20  ng2-fill-color: 
+0005c1c0: 2274 7261 6e73 7061 7265 6e74 223b 2d2d  "transparent";--
+0005c1d0: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005c1e0: 6733 2d63 6f6c 6f72 3a20 7661 7228 2d2d  g3-color: var(--
+0005c1f0: 7269 6f2d 6c6f 6361 6c2d 6667 293b 2d2d  rio-local-fg);--
+0005c200: 7269 6f2d 6c6f 6361 6c2d 6865 6164 696e  rio-local-headin
+0005c210: 6733 2d62 6163 6b67 726f 756e 643a 2022  g3-background: "
+0005c220: 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f 6361  none";--rio-loca
+0005c230: 6c2d 6865 6164 696e 6733 2d62 6163 6b67  l-heading3-backg
+0005c240: 726f 756e 642d 636c 6970 3a20 2262 6f72  round-clip: "bor
+0005c250: 6465 722d 626f 7822 3b2d 2d72 696f 2d6c  der-box";--rio-l
+0005c260: 6f63 616c 2d68 6561 6469 6e67 332d 6669  ocal-heading3-fi
+0005c270: 6c6c 2d63 6f6c 6f72 3a20 2274 7261 6e73  ll-color: "trans
+0005c280: 7061 7265 6e74 223b 2d2d 7269 6f2d 6c6f  parent";--rio-lo
+0005c290: 6361 6c2d 7465 7874 2d63 6f6c 6f72 3a20  cal-text-color: 
+0005c2a0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+0005c2b0: 6667 293b 2d2d 7269 6f2d 6c6f 6361 6c2d  fg);--rio-local-
+0005c2c0: 7465 7874 2d62 6163 6b67 726f 756e 643a  text-background:
+0005c2d0: 2022 6e6f 6e65 223b 2d2d 7269 6f2d 6c6f   "none";--rio-lo
+0005c2e0: 6361 6c2d 7465 7874 2d62 6163 6b67 726f  cal-text-backgro
+0005c2f0: 756e 642d 636c 6970 3a20 2262 6f72 6465  und-clip: "borde
+0005c300: 722d 626f 7822 3b2d 2d72 696f 2d6c 6f63  r-box";--rio-loc
+0005c310: 616c 2d74 6578 742d 6669 6c6c 2d63 6f6c  al-text-fill-col
+0005c320: 6f72 3a20 2274 7261 6e73 7061 7265 6e74  or: "transparent
+0005c330: 223b 636f 6c6f 723a 7661 7228 2d2d 7269  ";color:var(--ri
+0005c340: 6f2d 6c6f 6361 6c2d 6667 297d 6874 6d6c  o-local-fg)}html
+0005c350: 5b64 6174 612d 7468 656d 653d 6c69 6768  [data-theme=ligh
+0005c360: 745d 2070 7265 2063 6f64 652e 686c 6a73  t] pre code.hljs
+0005c370: 7b64 6973 706c 6179 3a62 6c6f 636b 3b6f  {display:block;o
+0005c380: 7665 7266 6c6f 772d 783a 6175 746f 3b70  verflow-x:auto;p
+0005c390: 6164 6469 6e67 3a31 7265 6d7d 6874 6d6c  adding:1rem}html
+0005c3a0: 5b64 6174 612d 7468 656d 653d 6c69 6768  [data-theme=ligh
+0005c3b0: 745d 2063 6f64 652e 686c 6a73 7b70 6164  t] code.hljs{pad
+0005c3c0: 6469 6e67 3a33 7078 2035 7078 7d68 746d  ding:3px 5px}htm
+0005c3d0: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
+0005c3e0: 6874 5d20 2e68 6c6a 737b 6261 636b 6772  ht] .hljs{backgr
+0005c3f0: 6f75 6e64 3a23 6633 6633 6633 3b63 6f6c  ound:#f3f3f3;col
+0005c400: 6f72 3a23 3434 347d 6874 6d6c 5b64 6174  or:#444}html[dat
+0005c410: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
+0005c420: 686c 6a73 2d63 6f6d 6d65 6e74 7b63 6f6c  hljs-comment{col
+0005c430: 6f72 3a23 3639 3730 3730 7d68 746d 6c5b  or:#697070}html[
+0005c440: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c450: 5d20 2e68 6c6a 732d 7075 6e63 7475 6174  ] .hljs-punctuat
+0005c460: 696f 6e2c 6874 6d6c 5b64 6174 612d 7468  ion,html[data-th
+0005c470: 656d 653d 6c69 6768 745d 202e 686c 6a73  eme=light] .hljs
+0005c480: 2d74 6167 7b63 6f6c 6f72 3a23 3434 3461  -tag{color:#444a
+0005c490: 7d68 746d 6c5b 6461 7461 2d74 6865 6d65  }html[data-theme
+0005c4a0: 3d6c 6967 6874 5d20 2e68 6c6a 732d 7461  =light] .hljs-ta
+0005c4b0: 6720 2e68 6c6a 732d 6174 7472 2c68 746d  g .hljs-attr,htm
+0005c4c0: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
+0005c4d0: 6874 5d20 2e68 6c6a 732d 7461 6720 2e68  ht] .hljs-tag .h
+0005c4e0: 6c6a 732d 6e61 6d65 7b63 6f6c 6f72 3a23  ljs-name{color:#
+0005c4f0: 3434 347d 6874 6d6c 5b64 6174 612d 7468  444}html[data-th
+0005c500: 656d 653d 6c69 6768 745d 202e 686c 6a73  eme=light] .hljs
+0005c510: 2d61 7474 7269 6275 7465 2c68 746d 6c5b  -attribute,html[
+0005c520: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c530: 5d20 2e68 6c6a 732d 646f 6374 6167 2c68  ] .hljs-doctag,h
+0005c540: 746d 6c5b 6461 7461 2d74 6865 6d65 3d6c  tml[data-theme=l
+0005c550: 6967 6874 5d20 2e68 6c6a 732d 6b65 7977  ight] .hljs-keyw
+0005c560: 6f72 642c 6874 6d6c 5b64 6174 612d 7468  ord,html[data-th
+0005c570: 656d 653d 6c69 6768 745d 202e 686c 6a73  eme=light] .hljs
+0005c580: 2d6d 6574 6120 2e68 6c6a 732d 6b65 7977  -meta .hljs-keyw
+0005c590: 6f72 642c 6874 6d6c 5b64 6174 612d 7468  ord,html[data-th
+0005c5a0: 656d 653d 6c69 6768 745d 202e 686c 6a73  eme=light] .hljs
+0005c5b0: 2d6e 616d 652c 6874 6d6c 5b64 6174 612d  -name,html[data-
+0005c5c0: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
+0005c5d0: 6a73 2d73 656c 6563 746f 722d 7461 677b  js-selector-tag{
+0005c5e0: 666f 6e74 2d77 6569 6768 743a 3730 307d  font-weight:700}
+0005c5f0: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
+0005c600: 6c69 6768 745d 202e 686c 6a73 2d64 656c  light] .hljs-del
+0005c610: 6574 696f 6e2c 6874 6d6c 5b64 6174 612d  etion,html[data-
+0005c620: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
+0005c630: 6a73 2d6e 756d 6265 722c 6874 6d6c 5b64  js-number,html[d
+0005c640: 6174 612d 7468 656d 653d 6c69 6768 745d  ata-theme=light]
+0005c650: 202e 686c 6a73 2d71 756f 7465 2c68 746d   .hljs-quote,htm
+0005c660: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
+0005c670: 6874 5d20 2e68 6c6a 732d 7365 6c65 6374  ht] .hljs-select
+0005c680: 6f72 2d63 6c61 7373 2c68 746d 6c5b 6461  or-class,html[da
+0005c690: 7461 2d74 6865 6d65 3d6c 6967 6874 5d20  ta-theme=light] 
+0005c6a0: 2e68 6c6a 732d 7365 6c65 6374 6f72 2d69  .hljs-selector-i
+0005c6b0: 642c 6874 6d6c 5b64 6174 612d 7468 656d  d,html[data-them
+0005c6c0: 653d 6c69 6768 745d 202e 686c 6a73 2d73  e=light] .hljs-s
+0005c6d0: 7472 696e 672c 6874 6d6c 5b64 6174 612d  tring,html[data-
+0005c6e0: 7468 656d 653d 6c69 6768 745d 202e 686c  theme=light] .hl
+0005c6f0: 6a73 2d74 656d 706c 6174 652d 7461 672c  js-template-tag,
+0005c700: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
+0005c710: 6c69 6768 745d 202e 686c 6a73 2d74 7970  light] .hljs-typ
+0005c720: 657b 636f 6c6f 723a 2338 3030 7d68 746d  e{color:#800}htm
+0005c730: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
+0005c740: 6874 5d20 2e68 6c6a 732d 7365 6374 696f  ht] .hljs-sectio
+0005c750: 6e2c 6874 6d6c 5b64 6174 612d 7468 656d  n,html[data-them
+0005c760: 653d 6c69 6768 745d 202e 686c 6a73 2d74  e=light] .hljs-t
+0005c770: 6974 6c65 7b63 6f6c 6f72 3a23 3830 303b  itle{color:#800;
+0005c780: 666f 6e74 2d77 6569 6768 743a 3730 307d  font-weight:700}
+0005c790: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
+0005c7a0: 6c69 6768 745d 202e 686c 6a73 2d6c 696e  light] .hljs-lin
+0005c7b0: 6b2c 6874 6d6c 5b64 6174 612d 7468 656d  k,html[data-them
+0005c7c0: 653d 6c69 6768 745d 202e 686c 6a73 2d6f  e=light] .hljs-o
+0005c7d0: 7065 7261 746f 722c 6874 6d6c 5b64 6174  perator,html[dat
+0005c7e0: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
+0005c7f0: 686c 6a73 2d72 6567 6578 702c 6874 6d6c  hljs-regexp,html
+0005c800: 5b64 6174 612d 7468 656d 653d 6c69 6768  [data-theme=ligh
+0005c810: 745d 202e 686c 6a73 2d73 656c 6563 746f  t] .hljs-selecto
+0005c820: 722d 6174 7472 2c68 746d 6c5b 6461 7461  r-attr,html[data
+0005c830: 2d74 6865 6d65 3d6c 6967 6874 5d20 2e68  -theme=light] .h
+0005c840: 6c6a 732d 7365 6c65 6374 6f72 2d70 7365  ljs-selector-pse
+0005c850: 7564 6f2c 6874 6d6c 5b64 6174 612d 7468  udo,html[data-th
+0005c860: 656d 653d 6c69 6768 745d 202e 686c 6a73  eme=light] .hljs
+0005c870: 2d73 796d 626f 6c2c 6874 6d6c 5b64 6174  -symbol,html[dat
+0005c880: 612d 7468 656d 653d 6c69 6768 745d 202e  a-theme=light] .
+0005c890: 686c 6a73 2d74 656d 706c 6174 652d 7661  hljs-template-va
+0005c8a0: 7269 6162 6c65 2c68 746d 6c5b 6461 7461  riable,html[data
+0005c8b0: 2d74 6865 6d65 3d6c 6967 6874 5d20 2e68  -theme=light] .h
+0005c8c0: 6c6a 732d 7661 7269 6162 6c65 7b63 6f6c  ljs-variable{col
+0005c8d0: 6f72 3a23 6162 3536 3536 7d68 746d 6c5b  or:#ab5656}html[
+0005c8e0: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c8f0: 5d20 2e68 6c6a 732d 6c69 7465 7261 6c7b  ] .hljs-literal{
+0005c900: 636f 6c6f 723a 2336 3935 7d68 746d 6c5b  color:#695}html[
+0005c910: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c920: 5d20 2e68 6c6a 732d 6164 6469 7469 6f6e  ] .hljs-addition
+0005c930: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
+0005c940: 3d6c 6967 6874 5d20 2e68 6c6a 732d 6275  =light] .hljs-bu
+0005c950: 696c 745f 696e 2c68 746d 6c5b 6461 7461  ilt_in,html[data
+0005c960: 2d74 6865 6d65 3d6c 6967 6874 5d20 2e68  -theme=light] .h
+0005c970: 6c6a 732d 6275 6c6c 6574 2c68 746d 6c5b  ljs-bullet,html[
+0005c980: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c990: 5d20 2e68 6c6a 732d 636f 6465 7b63 6f6c  ] .hljs-code{col
+0005c9a0: 6f72 3a23 3339 3733 3030 7d68 746d 6c5b  or:#397300}html[
+0005c9b0: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c9c0: 5d20 2e68 6c6a 732d 6d65 7461 7b63 6f6c  ] .hljs-meta{col
+0005c9d0: 6f72 3a23 3166 3731 3939 7d68 746d 6c5b  or:#1f7199}html[
+0005c9e0: 6461 7461 2d74 6865 6d65 3d6c 6967 6874  data-theme=light
+0005c9f0: 5d20 2e68 6c6a 732d 6d65 7461 202e 686c  ] .hljs-meta .hl
+0005ca00: 6a73 2d73 7472 696e 677b 636f 6c6f 723a  js-string{color:
+0005ca10: 2333 3861 7d68 746d 6c5b 6461 7461 2d74  #38a}html[data-t
+0005ca20: 6865 6d65 3d6c 6967 6874 5d20 2e68 6c6a  heme=light] .hlj
+0005ca30: 732d 656d 7068 6173 6973 7b66 6f6e 742d  s-emphasis{font-
+0005ca40: 7374 796c 653a 6974 616c 6963 7d68 746d  style:italic}htm
+0005ca50: 6c5b 6461 7461 2d74 6865 6d65 3d6c 6967  l[data-theme=lig
+0005ca60: 6874 5d20 2e68 6c6a 732d 7374 726f 6e67  ht] .hljs-strong
+0005ca70: 7b66 6f6e 742d 7765 6967 6874 3a37 3030  {font-weight:700
+0005ca80: 7d68 746d 6c5b 6461 7461 2d74 6865 6d65  }html[data-theme
+0005ca90: 3d64 6172 6b5d 202e 686c 6a73 7b63 6f6c  =dark] .hljs{col
+0005caa0: 6f72 3a23 6464 643b 6261 636b 6772 6f75  or:#ddd;backgrou
+0005cab0: 6e64 3a23 3330 3330 3330 7d68 746d 6c5b  nd:#303030}html[
+0005cac0: 6461 7461 2d74 6865 6d65 3d64 6172 6b5d  data-theme=dark]
+0005cad0: 202e 686c 6a73 2d6b 6579 776f 7264 2c68   .hljs-keyword,h
+0005cae0: 746d 6c5b 6461 7461 2d74 6865 6d65 3d64  tml[data-theme=d
+0005caf0: 6172 6b5d 202e 686c 6a73 2d73 656c 6563  ark] .hljs-selec
+0005cb00: 746f 722d 7461 672c 6874 6d6c 5b64 6174  tor-tag,html[dat
+0005cb10: 612d 7468 656d 653d 6461 726b 5d20 2e68  a-theme=dark] .h
+0005cb20: 6c6a 732d 6c69 7465 7261 6c2c 6874 6d6c  ljs-literal,html
+0005cb30: 5b64 6174 612d 7468 656d 653d 6461 726b  [data-theme=dark
+0005cb40: 5d20 2e68 6c6a 732d 7365 6374 696f 6e2c  ] .hljs-section,
+0005cb50: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
+0005cb60: 6461 726b 5d20 2e68 6c6a 732d 6c69 6e6b  dark] .hljs-link
+0005cb70: 7b63 6f6c 6f72 3a23 6666 667d 6874 6d6c  {color:#fff}html
+0005cb80: 5b64 6174 612d 7468 656d 653d 6461 726b  [data-theme=dark
+0005cb90: 5d20 2e68 6c6a 732d 7374 7269 6e67 2c68  ] .hljs-string,h
+0005cba0: 746d 6c5b 6461 7461 2d74 6865 6d65 3d64  tml[data-theme=d
+0005cbb0: 6172 6b5d 202e 686c 6a73 2d74 6974 6c65  ark] .hljs-title
+0005cbc0: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
+0005cbd0: 3d64 6172 6b5d 202e 686c 6a73 2d6e 616d  =dark] .hljs-nam
+0005cbe0: 652c 6874 6d6c 5b64 6174 612d 7468 656d  e,html[data-them
+0005cbf0: 653d 6461 726b 5d20 2e68 6c6a 732d 7479  e=dark] .hljs-ty
+0005cc00: 7065 2c68 746d 6c5b 6461 7461 2d74 6865  pe,html[data-the
+0005cc10: 6d65 3d64 6172 6b5d 202e 686c 6a73 2d61  me=dark] .hljs-a
+0005cc20: 7474 7269 6275 7465 2c68 746d 6c5b 6461  ttribute,html[da
+0005cc30: 7461 2d74 6865 6d65 3d64 6172 6b5d 202e  ta-theme=dark] .
+0005cc40: 686c 6a73 2d73 796d 626f 6c2c 6874 6d6c  hljs-symbol,html
+0005cc50: 5b64 6174 612d 7468 656d 653d 6461 726b  [data-theme=dark
+0005cc60: 5d20 2e68 6c6a 732d 6275 6c6c 6574 2c68  ] .hljs-bullet,h
+0005cc70: 746d 6c5b 6461 7461 2d74 6865 6d65 3d64  tml[data-theme=d
+0005cc80: 6172 6b5d 202e 686c 6a73 2d62 7569 6c74  ark] .hljs-built
+0005cc90: 5f69 6e2c 6874 6d6c 5b64 6174 612d 7468  _in,html[data-th
+0005cca0: 656d 653d 6461 726b 5d20 2e68 6c6a 732d  eme=dark] .hljs-
+0005ccb0: 6164 6469 7469 6f6e 2c68 746d 6c5b 6461  addition,html[da
+0005ccc0: 7461 2d74 6865 6d65 3d64 6172 6b5d 202e  ta-theme=dark] .
+0005ccd0: 686c 6a73 2d76 6172 6961 626c 652c 6874  hljs-variable,ht
+0005cce0: 6d6c 5b64 6174 612d 7468 656d 653d 6461  ml[data-theme=da
+0005ccf0: 726b 5d20 2e68 6c6a 732d 7465 6d70 6c61  rk] .hljs-templa
+0005cd00: 7465 2d74 6167 2c68 746d 6c5b 6461 7461  te-tag,html[data
+0005cd10: 2d74 6865 6d65 3d64 6172 6b5d 202e 686c  -theme=dark] .hl
+0005cd20: 6a73 2d74 656d 706c 6174 652d 7661 7269  js-template-vari
+0005cd30: 6162 6c65 7b63 6f6c 6f72 3a23 6438 387d  able{color:#d88}
+0005cd40: 6874 6d6c 5b64 6174 612d 7468 656d 653d  html[data-theme=
+0005cd50: 6461 726b 5d20 2e68 6c6a 732d 636f 6d6d  dark] .hljs-comm
+0005cd60: 656e 742c 6874 6d6c 5b64 6174 612d 7468  ent,html[data-th
+0005cd70: 656d 653d 6461 726b 5d20 2e68 6c6a 732d  eme=dark] .hljs-
+0005cd80: 7175 6f74 652c 6874 6d6c 5b64 6174 612d  quote,html[data-
+0005cd90: 7468 656d 653d 6461 726b 5d20 2e68 6c6a  theme=dark] .hlj
+0005cda0: 732d 6465 6c65 7469 6f6e 2c68 746d 6c5b  s-deletion,html[
+0005cdb0: 6461 7461 2d74 6865 6d65 3d64 6172 6b5d  data-theme=dark]
+0005cdc0: 202e 686c 6a73 2d6d 6574 617b 636f 6c6f   .hljs-meta{colo
+0005cdd0: 723a 2339 3739 3739 377d 6874 6d6c 5b64  r:#979797}html[d
+0005cde0: 6174 612d 7468 656d 653d 6461 726b 5d20  ata-theme=dark] 
+0005cdf0: 2e68 6c6a 732d 6b65 7977 6f72 642c 6874  .hljs-keyword,ht
+0005ce00: 6d6c 5b64 6174 612d 7468 656d 653d 6461  ml[data-theme=da
+0005ce10: 726b 5d20 2e68 6c6a 732d 7365 6c65 6374  rk] .hljs-select
+0005ce20: 6f72 2d74 6167 2c68 746d 6c5b 6461 7461  or-tag,html[data
+0005ce30: 2d74 6865 6d65 3d64 6172 6b5d 202e 686c  -theme=dark] .hl
+0005ce40: 6a73 2d6c 6974 6572 616c 2c68 746d 6c5b  js-literal,html[
+0005ce50: 6461 7461 2d74 6865 6d65 3d64 6172 6b5d  data-theme=dark]
+0005ce60: 202e 686c 6a73 2d74 6974 6c65 2c68 746d   .hljs-title,htm
+0005ce70: 6c5b 6461 7461 2d74 6865 6d65 3d64 6172  l[data-theme=dar
+0005ce80: 6b5d 202e 686c 6a73 2d73 6563 7469 6f6e  k] .hljs-section
+0005ce90: 2c68 746d 6c5b 6461 7461 2d74 6865 6d65  ,html[data-theme
+0005cea0: 3d64 6172 6b5d 202e 686c 6a73 2d64 6f63  =dark] .hljs-doc
+0005ceb0: 7461 672c 6874 6d6c 5b64 6174 612d 7468  tag,html[data-th
 0005cec0: 656d 653d 6461 726b 5d20 2e68 6c6a 732d  eme=dark] .hljs-
-0005ced0: 656d 7068 6173 6973 7b66 6f6e 742d 7374  emphasis{font-st
-0005cee0: 796c 653a 6974 616c 6963 7d40 6b65 7966  yle:italic}@keyf
-0005cef0: 7261 6d65 7320 636f 6e74 656e 742d 6c6f  rames content-lo
-0005cf00: 6164 696e 677b 3025 7b62 6163 6b67 726f  ading{0%{backgro
-0005cf10: 756e 642d 706f 7369 7469 6f6e 3a2d 3130  und-position:-10
-0005cf20: 3072 656d 2030 7d74 6f7b 6261 636b 6772  0rem 0}to{backgr
-0005cf30: 6f75 6e64 2d70 6f73 6974 696f 6e3a 3020  ound-position:0 
-0005cf40: 307d 7d2e 7269 6f2d 636f 6e74 656e 742d  0}}.rio-content-
-0005cf50: 6c6f 6164 696e 677b 6261 636b 6772 6f75  loading{backgrou
-0005cf60: 6e64 2d69 6d61 6765 3a6c 696e 6561 722d  nd-image:linear-
-0005cf70: 6772 6164 6965 6e74 2874 6f20 7269 6768  gradient(to righ
-0005cf80: 742c 7472 616e 7370 6172 656e 7420 3130  t,transparent 10
-0005cf90: 252c 7661 7228 2d2d 7269 6f2d 6c6f 6361  %,var(--rio-loca
-0005cfa0: 6c2d 6c65 7665 6c2d 322d 6267 2920 3132  l-level-2-bg) 12
-0005cfb0: 252c 7472 616e 7370 6172 656e 7420 3134  %,transparent 14
-0005cfc0: 2529 3b62 6163 6b67 726f 756e 642d 7369  %);background-si
-0005cfd0: 7a65 3a31 3030 7265 6d20 3572 656d 3b61  ze:100rem 5rem;a
-0005cfe0: 6e69 6d61 7469 6f6e 3a63 6f6e 7465 6e74  nimation:content
-0005cff0: 2d6c 6f61 6469 6e67 2033 7320 6c69 6e65  -loading 3s line
-0005d000: 6172 2069 6e66 696e 6974 657d 406b 6579  ar infinite}@key
-0005d010: 6672 616d 6573 2062 6172 6265 722d 706f  frames barber-po
-0005d020: 6c65 7b30 257b 6261 636b 6772 6f75 6e64  le{0%{background
-0005d030: 2d70 6f73 6974 696f 6e3a 3020 307d 746f  -position:0 0}to
-0005d040: 7b62 6163 6b67 726f 756e 642d 706f 7369  {background-posi
-0005d050: 7469 6f6e 3a33 7265 6d20 3072 656d 7d7d  tion:3rem 0rem}}
-0005d060: 617b 636f 6c6f 723a 7661 7228 2d2d 7269  a{color:var(--ri
-0005d070: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 322d  o-local-level-2-
-0005d080: 6267 297d 613a 686f 7665 727b 636f 6c6f  bg)}a:hover{colo
-0005d090: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
-0005d0a0: 6c2d 6c65 7665 6c2d 322d 6267 2d61 6374  l-level-2-bg-act
-0005d0b0: 6976 6529 7d63 6f64 657b 666f 6e74 2d66  ive)}code{font-f
-0005d0c0: 616d 696c 793a 7661 7228 2d2d 7269 6f2d  amily:var(--rio-
-0005d0d0: 676c 6f62 616c 2d6d 6f6e 6f73 7061 6365  global-monospace
-0005d0e0: 2d66 6f6e 7429 2c6d 6f6e 6f73 7061 6365  -font),monospace
-0005d0f0: 7d68 746d 6c7b 6261 636b 6772 6f75 6e64  }html{background
-0005d100: 3a76 6172 282d 2d72 696f 2d67 6c6f 6261  :var(--rio-globa
-0005d110: 6c2d 6261 636b 6772 6f75 6e64 2d62 6729  l-background-bg)
-0005d120: 3b6f 7665 7266 6c6f 773a 6869 6464 656e  ;overflow:hidden
-0005d130: 7d62 6f64 797b 6d61 7267 696e 3a30 3b70  }body{margin:0;p
-0005d140: 6164 6469 6e67 3a30 3b66 6f6e 742d 6661  adding:0;font-fa
-0005d150: 6d69 6c79 3a76 6172 282d 2d72 696f 2d67  mily:var(--rio-g
-0005d160: 6c6f 6261 6c2d 666f 6e74 2c20 7361 6e73  lobal-font, sans
-0005d170: 2d73 6572 6966 297d 696e 7075 742c 7465  -serif)}input,te
-0005d180: 7874 6172 6561 2c73 656c 6563 747b 666f  xtarea,select{fo
-0005d190: 6e74 2d66 616d 696c 793a 696e 6865 7269  nt-family:inheri
-0005d1a0: 743b 666f 6e74 2d73 697a 653a 3172 656d  t;font-size:1rem
-0005d1b0: 7d2e 7269 6f2d 636f 6d70 6f6e 656e 747b  }.rio-component{
-0005d1c0: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
-0005d1d0: 657d 2e72 696f 2d66 756e 6461 6d65 6e74  e}.rio-fundament
-0005d1e0: 616c 2d72 6f6f 742d 636f 6d70 6f6e 656e  al-root-componen
-0005d1f0: 747b 706f 7369 7469 6f6e 3a72 656c 6174  t{position:relat
-0005d200: 6976 6521 696d 706f 7274 616e 743b 7769  ive!important;wi
-0005d210: 6474 683a 3130 3076 773b 6865 6967 6874  dth:100vw;height
-0005d220: 3a31 3030 7668 7d2e 7269 6f2d 6c69 6e65  :100vh}.rio-line
-0005d230: 6172 2d63 6869 6c64 2d63 6f6e 7461 696e  ar-child-contain
-0005d240: 6572 7b70 6f69 6e74 6572 2d65 7665 6e74  er{pointer-event
-0005d250: 733a 6e6f 6e65 3b64 6973 706c 6179 3a66  s:none;display:f
-0005d260: 6c65 783b 616c 6967 6e2d 6974 656d 733a  lex;align-items:
-0005d270: 7374 7265 7463 687d 2e72 696f 2d6c 696e  stretch}.rio-lin
-0005d280: 6561 722d 6368 696c 642d 636f 6e74 6169  ear-child-contai
-0005d290: 6e65 723e 2a7b 706f 7369 7469 6f6e 3a72  ner>*{position:r
-0005d2a0: 656c 6174 6976 6521 696d 706f 7274 616e  elative!importan
-0005d2b0: 747d 2e72 696f 2d6c 6973 742d 7669 6577  t}.rio-list-view
-0005d2c0: 3e64 6976 3e2a 3a66 6972 7374 2d63 6869  >div>*:first-chi
-0005d2d0: 6c64 7b70 6f73 6974 696f 6e3a 7265 6c61  ld{position:rela
-0005d2e0: 7469 7665 2169 6d70 6f72 7461 6e74 7d2e  tive!important}.
-0005d2f0: 7269 6f2d 636f 6c75 6d6e 7b66 6c65 782d  rio-column{flex-
-0005d300: 6469 7265 6374 696f 6e3a 636f 6c75 6d6e  direction:column
-0005d310: 7d2e 7269 6f2d 6772 6964 7b70 6f69 6e74  }.rio-grid{point
-0005d320: 6572 2d65 7665 6e74 733a 6e6f 6e65 3b64  er-events:none;d
-0005d330: 6973 706c 6179 3a67 7269 647d 2e72 696f  isplay:grid}.rio
-0005d340: 2d74 6578 747b 706f 696e 7465 722d 6576  -text{pointer-ev
-0005d350: 656e 7473 3a61 7574 6f3b 6469 7370 6c61  ents:auto;displa
-0005d360: 793a 666c 6578 3b61 6c69 676e 2d69 7465  y:flex;align-ite
-0005d370: 6d73 3a63 656e 7465 723b 636f 6c6f 723a  ms:center;color:
-0005d380: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005d390: 7465 7874 2d63 6f6c 6f72 297d 2e72 696f  text-color)}.rio
-0005d3a0: 2d74 6578 743e 6469 767b 666c 6578 2d67  -text>div{flex-g
-0005d3b0: 726f 773a 313b 6f76 6572 666c 6f77 3a68  row:1;overflow:h
-0005d3c0: 6964 6465 6e7d 2e72 696f 2d72 6563 7461  idden}.rio-recta
-0005d3d0: 6e67 6c65 7b70 6f69 6e74 6572 2d65 7665  ngle{pointer-eve
-0005d3e0: 6e74 733a 6175 746f 3b62 6f72 6465 722d  nts:auto;border-
-0005d3f0: 7374 796c 653a 736f 6c69 643b 7472 616e  style:solid;tran
-0005d400: 7369 7469 6f6e 2d70 726f 7065 7274 793a  sition-property:
-0005d410: 6261 636b 6772 6f75 6e64 2c73 7472 6f6b  background,strok
-0005d420: 652d 636f 6c6f 722c 7374 726f 6b65 2d77  e-color,stroke-w
-0005d430: 6964 7468 2c62 6f72 6465 722d 7261 6469  idth,border-radi
-0005d440: 7573 2c73 6861 646f 772d 636f 6c6f 722c  us,shadow-color,
-0005d450: 7368 6164 6f77 2d72 6164 6975 732c 7368  shadow-radius,sh
-0005d460: 6164 6f77 2d6f 6666 7365 743b 7472 616e  adow-offset;tran
-0005d470: 7369 7469 6f6e 2d74 696d 696e 672d 6675  sition-timing-fu
-0005d480: 6e63 7469 6f6e 3a65 6173 653b 6261 636b  nction:ease;back
-0005d490: 6772 6f75 6e64 3a76 6172 282d 2d72 696f  ground:var(--rio
-0005d4a0: 2d72 6563 7461 6e67 6c65 2d66 696c 6c29  -rectangle-fill)
-0005d4b0: 3b62 6f72 6465 722d 636f 6c6f 723a 7661  ;border-color:va
-0005d4c0: 7228 2d2d 7269 6f2d 7265 6374 616e 676c  r(--rio-rectangl
-0005d4d0: 652d 7374 726f 6b65 5f63 6f6c 6f72 293b  e-stroke_color);
-0005d4e0: 626f 7264 6572 2d77 6964 7468 3a76 6172  border-width:var
-0005d4f0: 282d 2d72 696f 2d72 6563 7461 6e67 6c65  (--rio-rectangle
-0005d500: 2d73 7472 6f6b 655f 7769 6474 6829 3b62  -stroke_width);b
-0005d510: 6f72 6465 722d 7261 6469 7573 3a76 6172  order-radius:var
-0005d520: 282d 2d72 696f 2d72 6563 7461 6e67 6c65  (--rio-rectangle
-0005d530: 2d63 6f72 6e65 725f 7261 6469 7573 293b  -corner_radius);
-0005d540: 626f 782d 7368 6164 6f77 3a76 6172 282d  box-shadow:var(-
-0005d550: 2d72 696f 2d72 6563 7461 6e67 6c65 2d73  -rio-rectangle-s
-0005d560: 6861 646f 775f 6f66 6673 6574 5f78 2920  hadow_offset_x) 
-0005d570: 7661 7228 2d2d 7269 6f2d 7265 6374 616e  var(--rio-rectan
-0005d580: 676c 652d 7368 6164 6f77 5f6f 6666 7365  gle-shadow_offse
-0005d590: 745f 7929 2076 6172 282d 2d72 696f 2d72  t_y) var(--rio-r
-0005d5a0: 6563 7461 6e67 6c65 2d73 6861 646f 775f  ectangle-shadow_
-0005d5b0: 7261 6469 7573 2920 7661 7228 2d2d 7269  radius) var(--ri
-0005d5c0: 6f2d 7265 6374 616e 676c 652d 7368 6164  o-rectangle-shad
-0005d5d0: 6f77 5f63 6f6c 6f72 297d 2e72 696f 2d72  ow_color)}.rio-r
-0005d5e0: 6563 7461 6e67 6c65 3a68 6f76 6572 7b62  ectangle:hover{b
-0005d5f0: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
-0005d600: 7269 6f2d 7265 6374 616e 676c 652d 686f  rio-rectangle-ho
-0005d610: 7665 722d 6669 6c6c 293b 626f 7264 6572  ver-fill);border
-0005d620: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
-0005d630: 2d72 6563 7461 6e67 6c65 2d68 6f76 6572  -rectangle-hover
-0005d640: 2d73 7472 6f6b 655f 636f 6c6f 7229 3b62  -stroke_color);b
-0005d650: 6f72 6465 722d 7769 6474 683a 7661 7228  order-width:var(
-0005d660: 2d2d 7269 6f2d 7265 6374 616e 676c 652d  --rio-rectangle-
-0005d670: 686f 7665 722d 7374 726f 6b65 5f77 6964  hover-stroke_wid
-0005d680: 7468 293b 626f 7264 6572 2d72 6164 6975  th);border-radiu
-0005d690: 733a 7661 7228 2d2d 7269 6f2d 7265 6374  s:var(--rio-rect
-0005d6a0: 616e 676c 652d 686f 7665 722d 636f 726e  angle-hover-corn
-0005d6b0: 6572 5f72 6164 6975 7329 3b62 6f78 2d73  er_radius);box-s
-0005d6c0: 6861 646f 773a 7661 7228 2d2d 7269 6f2d  hadow:var(--rio-
-0005d6d0: 7265 6374 616e 676c 652d 686f 7665 722d  rectangle-hover-
-0005d6e0: 7368 6164 6f77 5f6f 6666 7365 745f 7829  shadow_offset_x)
-0005d6f0: 2076 6172 282d 2d72 696f 2d72 6563 7461   var(--rio-recta
-0005d700: 6e67 6c65 2d68 6f76 6572 2d73 6861 646f  ngle-hover-shado
-0005d710: 775f 6f66 6673 6574 5f79 2920 7661 7228  w_offset_y) var(
-0005d720: 2d2d 7269 6f2d 7265 6374 616e 676c 652d  --rio-rectangle-
-0005d730: 686f 7665 722d 7368 6164 6f77 5f72 6164  hover-shadow_rad
-0005d740: 6975 7329 2076 6172 282d 2d72 696f 2d72  ius) var(--rio-r
-0005d750: 6563 7461 6e67 6c65 2d68 6f76 6572 2d73  ectangle-hover-s
-0005d760: 6861 646f 775f 636f 6c6f 7229 7d2e 7269  hadow_color)}.ri
-0005d770: 6f2d 7265 6374 616e 676c 652d 7269 7070  o-rectangle-ripp
-0005d780: 6c65 7b6f 7665 7266 6c6f 773a 6869 6464  le{overflow:hidd
-0005d790: 656e 7d2e 7269 6f2d 7465 7874 2d69 6e70  en}.rio-text-inp
-0005d7a0: 7574 7b63 7572 736f 723a 7465 7874 7d2e  ut{cursor:text}.
-0005d7b0: 7269 6f2d 7465 7874 2d69 6e70 7574 2d68  rio-text-input-h
-0005d7c0: 696e 742d 7465 7874 7b64 6973 706c 6179  int-text{display
-0005d7d0: 3a66 6c65 783b 616c 6967 6e2d 6974 656d  :flex;align-item
-0005d7e0: 733a 656e 643b 2d77 6562 6b69 742d 7573  s:end;-webkit-us
-0005d7f0: 6572 2d73 656c 6563 743a 6e6f 6e65 3b75  er-select:none;u
-0005d800: 7365 722d 7365 6c65 6374 3a6e 6f6e 653b  ser-select:none;
-0005d810: 7061 6464 696e 672d 626f 7474 6f6d 3a2e  padding-bottom:.
-0005d820: 3672 656d 3b63 6f6c 6f72 3a76 6172 282d  6rem;color:var(-
-0005d830: 2d72 696f 2d6c 6f63 616c 2d74 6578 742d  -rio-local-text-
-0005d840: 636f 6c6f 7229 3b6f 7061 6369 7479 3a30  color);opacity:0
-0005d850: 3b74 7261 6e73 6974 696f 6e3a 616c 6c20  ;transition:all 
-0005d860: 2e31 3373 206c 696e 6561 727d 2e72 696f  .13s linear}.rio
-0005d870: 2d74 6578 742d 696e 7075 742d 7072 6566  -text-input-pref
-0005d880: 6978 2d74 6578 747b 7061 6464 696e 672d  ix-text{padding-
-0005d890: 6c65 6674 3a2e 3872 656d 3b6d 6172 6769  left:.8rem;margi
-0005d8a0: 6e2d 7269 6768 743a 2e32 7265 6d7d 2e72  n-right:.2rem}.r
-0005d8b0: 696f 2d74 6578 742d 696e 7075 742d 7375  io-text-input-su
-0005d8c0: 6666 6978 2d74 6578 747b 7061 6464 696e  ffix-text{paddin
-0005d8d0: 672d 7269 6768 743a 2e38 7265 6d3b 6d61  g-right:.8rem;ma
-0005d8e0: 7267 696e 2d6c 6566 743a 2e32 7265 6d7d  rgin-left:.2rem}
-0005d8f0: 696e 7075 743a 6e6f 7428 3a70 6c61 6365  input:not(:place
-0005d900: 686f 6c64 6572 2d73 686f 776e 297e 2e72  holder-shown)~.r
-0005d910: 696f 2d74 6578 742d 696e 7075 742d 6869  io-text-input-hi
-0005d920: 6e74 2d74 6578 742c 2e72 696f 2d69 6e70  nt-text,.rio-inp
-0005d930: 7574 2d62 6f78 3a66 6f63 7573 2d77 6974  ut-box:focus-wit
-0005d940: 6869 6e3e 2e72 696f 2d74 6578 742d 696e  hin>.rio-text-in
-0005d950: 7075 742d 6869 6e74 2d74 6578 742c 2e72  put-hint-text,.r
-0005d960: 696f 2d69 6e70 7574 2d62 6f78 2d66 6f63  io-input-box-foc
-0005d970: 7573 6564 3e2e 7269 6f2d 7465 7874 2d69  used>.rio-text-i
-0005d980: 6e70 7574 2d68 696e 742d 7465 7874 7b6f  nput-hint-text{o
-0005d990: 7061 6369 7479 3a2e 357d 2e72 696f 2d74  pacity:.5}.rio-t
-0005d9a0: 6578 742d 696e 7075 742e 7269 6f2d 696e  ext-input.rio-in
-0005d9b0: 7075 742d 626f 787b 7061 6464 696e 672d  put-box{padding-
-0005d9c0: 6c65 6674 3a30 2169 6d70 6f72 7461 6e74  left:0!important
-0005d9d0: 3b70 6164 6469 6e67 2d72 6967 6874 3a30  ;padding-right:0
-0005d9e0: 2169 6d70 6f72 7461 6e74 7d2e 7269 6f2d  !important}.rio-
-0005d9f0: 696e 7075 742d 626f 787b 706f 696e 7465  input-box{pointe
-0005da00: 722d 6576 656e 7473 3a61 7574 6f3b 6469  r-events:auto;di
-0005da10: 7370 6c61 793a 666c 6578 3b66 6c65 782d  splay:flex;flex-
-0005da20: 6469 7265 6374 696f 6e3a 726f 773b 616c  direction:row;al
-0005da30: 6967 6e2d 6974 656d 733a 7374 7265 7463  ign-items:stretc
-0005da40: 683b 7061 6464 696e 672d 6c65 6674 3a2e  h;padding-left:.
-0005da50: 3872 656d 3b70 6164 6469 6e67 2d72 6967  8rem;padding-rig
-0005da60: 6874 3a2e 3872 656d 3b62 6f78 2d73 697a  ht:.8rem;box-siz
-0005da70: 696e 673a 626f 7264 6572 2d62 6f78 3b62  ing:border-box;b
-0005da80: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-0005da90: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-0005daa0: 6267 2d76 6172 6961 6e74 293b 626f 7264  bg-variant);bord
-0005dab0: 6572 2d72 6164 6975 733a 7661 7228 2d2d  er-radius:var(--
-0005dac0: 7269 6f2d 676c 6f62 616c 2d63 6f72 6e65  rio-global-corne
-0005dad0: 722d 7261 6469 7573 2d73 6d61 6c6c 2920  r-radius-small) 
-0005dae0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005daf0: 2d63 6f72 6e65 722d 7261 6469 7573 2d73  -corner-radius-s
-0005db00: 6d61 6c6c 2920 3020 307d 2e72 696f 2d69  mall) 0 0}.rio-i
-0005db10: 6e70 7574 2d62 6f78 3a6e 6f74 282e 7269  nput-box:not(.ri
-0005db20: 6f2d 6469 7361 626c 6564 2d69 6e70 7574  o-disabled-input
-0005db30: 297b 6f76 6572 666c 6f77 3a68 6964 6465  ){overflow:hidde
-0005db40: 6e7d 2e72 696f 2d69 6e70 7574 2d62 6f78  n}.rio-input-box
-0005db50: 3a66 6f63 7573 2d77 6974 6869 6e2c 2e72  :focus-within,.r
-0005db60: 696f 2d69 6e70 7574 2d62 6f78 2e72 696f  io-input-box.rio
-0005db70: 2d69 6e70 7574 2d62 6f78 2d66 6f63 7573  -input-box-focus
-0005db80: 6564 7b6f 7574 6c69 6e65 3a6e 6f6e 653b  ed{outline:none;
-0005db90: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-0005dba0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
-0005dbb0: 2d62 672d 6163 7469 7665 297d 2e72 696f  -bg-active)}.rio
-0005dbc0: 2d69 6e70 7574 2d62 6f78 3e69 6e70 7574  -input-box>input
-0005dbd0: 2c2e 7269 6f2d 696e 7075 742d 626f 783e  ,.rio-input-box>
-0005dbe0: 7465 7874 6172 6561 7b66 6c65 782d 6772  textarea{flex-gr
-0005dbf0: 6f77 3a31 3b6d 696e 2d77 6964 7468 3a30  ow:1;min-width:0
-0005dc00: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-0005dc10: 723a 7472 616e 7370 6172 656e 743b 636f  r:transparent;co
-0005dc20: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
-0005dc30: 6361 6c2d 7465 7874 2d63 6f6c 6f72 293b  cal-text-color);
-0005dc40: 6361 7265 742d 636f 6c6f 723a 7661 7228  caret-color:var(
-0005dc50: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-0005dc60: 6c2d 322d 6267 293b 626f 7264 6572 3a6e  l-2-bg);border:n
-0005dc70: 6f6e 657d 2e72 696f 2d69 6e70 7574 2d62  one}.rio-input-b
-0005dc80: 6f78 3e69 6e70 7574 7b68 6569 6768 743a  ox>input{height:
-0005dc90: 6361 6c63 2832 3030 2520 2d20 322e 3338  calc(200% - 2.38
-0005dca0: 7265 6d29 7d2e 7269 6f2d 696e 7075 742d  rem)}.rio-input-
-0005dcb0: 626f 783e 7465 7874 6172 6561 7b6d 6172  box>textarea{mar
-0005dcc0: 6769 6e2d 746f 703a 312e 3572 656d 3b77  gin-top:1.5rem;w
-0005dcd0: 6964 7468 3a31 3030 253b 7265 7369 7a65  idth:100%;resize
-0005dce0: 3a6e 6f6e 653b 7061 6464 696e 673a 3020  :none;padding:0 
-0005dcf0: 2e38 7265 6d7d 2e72 696f 2d69 6e70 7574  .8rem}.rio-input
-0005dd00: 2d62 6f78 3e69 6e70 7574 3a61 6374 6976  -box>input:activ
-0005dd10: 652c 2e72 696f 2d69 6e70 7574 2d62 6f78  e,.rio-input-box
-0005dd20: 3e74 6578 7461 7265 613a 6163 7469 7665  >textarea:active
-0005dd30: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
-0005dd40: 723a 7472 616e 7370 6172 656e 747d 2e72  r:transparent}.r
-0005dd50: 696f 2d69 6e70 7574 2d62 6f78 3e69 6e70  io-input-box>inp
-0005dd60: 7574 3a66 6f63 7573 2d76 6973 6962 6c65  ut:focus-visible
-0005dd70: 2c2e 7269 6f2d 696e 7075 742d 626f 783e  ,.rio-input-box>
-0005dd80: 7465 7874 6172 6561 3a66 6f63 7573 2d76  textarea:focus-v
-0005dd90: 6973 6962 6c65 7b6f 7574 6c69 6e65 3a6e  isible{outline:n
-0005dda0: 6f6e 657d 2e72 696f 2d69 6e70 7574 2d62  one}.rio-input-b
-0005ddb0: 6f78 2d6c 6162 656c 7b70 6f69 6e74 6572  ox-label{pointer
-0005ddc0: 2d65 7665 6e74 733a 6e6f 6e65 3b70 6f73  -events:none;pos
-0005ddd0: 6974 696f 6e3a 6162 736f 6c75 7465 3b6c  ition:absolute;l
-0005dde0: 6566 743a 2e38 7265 6d3b 746f 703a 6361  eft:.8rem;top:ca
-0005ddf0: 6c63 2835 3025 202d 202e 3572 656d 293b  lc(50% - .5rem);
-0005de00: 666f 6e74 2d73 697a 653a 3172 656d 3b63  font-size:1rem;c
-0005de10: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
-0005de20: 6f63 616c 2d74 6578 742d 636f 6c6f 7229  ocal-text-color)
-0005de30: 3b6f 7061 6369 7479 3a2e 353b 7472 616e  ;opacity:.5;tran
-0005de40: 7369 7469 6f6e 3a61 6c6c 202e 3133 7320  sition:all .13s 
-0005de50: 6c69 6e65 6172 7d69 6e70 7574 3a6e 6f74  linear}input:not
-0005de60: 283a 706c 6163 6568 6f6c 6465 722d 7368  (:placeholder-sh
-0005de70: 6f77 6e29 7e2e 7269 6f2d 696e 7075 742d  own)~.rio-input-
-0005de80: 626f 782d 6c61 6265 6c2c 7465 7874 6172  box-label,textar
-0005de90: 6561 3a6e 6f74 283a 706c 6163 6568 6f6c  ea:not(:placehol
-0005dea0: 6465 722d 7368 6f77 6e29 7e2e 7269 6f2d  der-shown)~.rio-
-0005deb0: 696e 7075 742d 626f 782d 6c61 6265 6c2c  input-box-label,
-0005dec0: 2e72 696f 2d69 6e70 7574 2d62 6f78 3a66  .rio-input-box:f
-0005ded0: 6f63 7573 2d77 6974 6869 6e3e 2e72 696f  ocus-within>.rio
-0005dee0: 2d69 6e70 7574 2d62 6f78 2d6c 6162 656c  -input-box-label
-0005def0: 2c2e 7269 6f2d 696e 7075 742d 626f 782d  ,.rio-input-box-
-0005df00: 666f 6375 7365 643e 2e72 696f 2d69 6e70  focused>.rio-inp
-0005df10: 7574 2d62 6f78 2d6c 6162 656c 7b6f 7061  ut-box-label{opa
-0005df20: 6369 7479 3a31 3b74 6f70 3a2e 3472 656d  city:1;top:.4rem
-0005df30: 3b62 6f74 746f 6d3a 756e 7365 743b 666f  ;bottom:unset;fo
-0005df40: 6e74 2d73 697a 653a 2e38 7265 6d7d 2e72  nt-size:.8rem}.r
-0005df50: 696f 2d69 6e70 7574 2d62 6f78 3a66 6f63  io-input-box:foc
-0005df60: 7573 2d77 6974 6869 6e3e 2e72 696f 2d69  us-within>.rio-i
-0005df70: 6e70 7574 2d62 6f78 2d6c 6162 656c 2c2e  nput-box-label,.
-0005df80: 7269 6f2d 696e 7075 742d 626f 782d 666f  rio-input-box-fo
-0005df90: 6375 7365 643e 2e72 696f 2d69 6e70 7574  cused>.rio-input
-0005dfa0: 2d62 6f78 2d6c 6162 656c 7b63 6f6c 6f72  -box-label{color
-0005dfb0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
-0005dfc0: 2d6c 6576 656c 2d32 2d62 6729 7d2e 7269  -level-2-bg)}.ri
-0005dfd0: 6f2d 696e 7075 742d 626f 782d 706c 6169  o-input-box-plai
-0005dfe0: 6e2d 6261 722c 2e72 696f 2d69 6e70 7574  n-bar,.rio-input
-0005dff0: 2d62 6f78 2d63 6f6c 6f72 2d62 6172 7b70  -box-color-bar{p
-0005e000: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
-0005e010: 3b62 6f74 746f 6d3a 303b 6865 6967 6874  ;bottom:0;height
-0005e020: 3a2e 3132 7265 6d7d 2e72 696f 2d69 6e70  :.12rem}.rio-inp
-0005e030: 7574 2d62 6f78 2d70 6c61 696e 2d62 6172  ut-box-plain-bar
-0005e040: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
-0005e050: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
-0005e060: 6c2d 7465 7874 2d63 6f6c 6f72 293b 6c65  l-text-color);le
-0005e070: 6674 3a30 3b72 6967 6874 3a30 3b6f 7061  ft:0;right:0;opa
-0005e080: 6369 7479 3a2e 3135 7d2e 7269 6f2d 696e  city:.15}.rio-in
-0005e090: 7075 742d 626f 782d 636f 6c6f 722d 6261  put-box-color-ba
-0005e0a0: 727b 6261 636b 6772 6f75 6e64 2d63 6f6c  r{background-col
-0005e0b0: 6f72 3a76 6172 282d 2d72 696f 2d6c 6f63  or:var(--rio-loc
-0005e0c0: 616c 2d6c 6576 656c 2d32 2d62 6729 3b6c  al-level-2-bg);l
-0005e0d0: 6566 743a 3430 253b 7269 6768 743a 3430  eft:40%;right:40
-0005e0e0: 253b 6f70 6163 6974 793a 303b 7472 616e  %;opacity:0;tran
-0005e0f0: 7369 7469 6f6e 3a61 6c6c 202e 3273 2065  sition:all .2s e
-0005e100: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
-0005e110: 696e 7075 742d 626f 783a 666f 6375 732d  input-box:focus-
-0005e120: 7769 7468 696e 202e 7269 6f2d 696e 7075  within .rio-inpu
-0005e130: 742d 626f 782d 636f 6c6f 722d 6261 722c  t-box-color-bar,
-0005e140: 2e72 696f 2d69 6e70 7574 2d62 6f78 2d66  .rio-input-box-f
-0005e150: 6f63 7573 6564 202e 7269 6f2d 696e 7075  ocused .rio-inpu
-0005e160: 742d 626f 782d 636f 6c6f 722d 6261 727b  t-box-color-bar{
-0005e170: 6c65 6674 3a30 3b72 6967 6874 3a30 3b6f  left:0;right:0;o
-0005e180: 7061 6369 7479 3a31 7d2e 7269 6f2d 7374  pacity:1}.rio-st
-0005e190: 6163 6b7b 706f 696e 7465 722d 6576 656e  ack{pointer-even
-0005e1a0: 7473 3a6e 6f6e 653b 6469 7370 6c61 793a  ts:none;display:
-0005e1b0: 696e 6c69 6e65 2d67 7269 647d 2e72 696f  inline-grid}.rio
-0005e1c0: 2d73 7461 636b 3e2a 7b67 7269 642d 636f  -stack>*{grid-co
-0005e1d0: 6c75 6d6e 2d73 7461 7274 3a31 3b67 7269  lumn-start:1;gri
-0005e1e0: 642d 726f 772d 7374 6172 743a 317d 2e72  d-row-start:1}.r
-0005e1f0: 696f 2d73 7769 7463 687b 6469 7370 6c61  io-switch{displa
-0005e200: 793a 666c 6578 7d2e 7269 6f2d 7377 6974  y:flex}.rio-swit
-0005e210: 6368 3e2a 7b70 6f69 6e74 6572 2d65 7665  ch>*{pointer-eve
-0005e220: 6e74 733a 6175 746f 3b70 6f73 6974 696f  nts:auto;positio
-0005e230: 6e3a 7265 6c61 7469 7665 3b77 6964 7468  n:relative;width
-0005e240: 3a33 2e31 3872 656d 3b68 6569 6768 743a  :3.18rem;height:
-0005e250: 312e 3534 7265 6d3b 6d61 7267 696e 3a61  1.54rem;margin:a
-0005e260: 7574 6f3b 626f 7264 6572 2d72 6164 6975  uto;border-radiu
-0005e270: 733a 342e 3372 656d 3b62 6163 6b67 726f  s:4.3rem;backgro
-0005e280: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-0005e290: 7269 6f2d 676c 6f62 616c 2d64 6973 6162  rio-global-disab
-0005e2a0: 6c65 642d 6267 2d76 6172 6961 6e74 293b  led-bg-variant);
-0005e2b0: 7472 616e 7369 7469 6f6e 3a2e 3373 2065  transition:.3s e
-0005e2c0: 6173 6520 616c 6c3b 7a2d 696e 6465 783a  ase all;z-index:
-0005e2d0: 317d 2e72 696f 2d73 7769 7463 682e 6973  1}.rio-switch.is
-0005e2e0: 2d6f 6e3e 2a7b 6261 636b 6772 6f75 6e64  -on>*{background
-0005e2f0: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
-0005e300: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
-0005e310: 6729 7d2e 7269 6f2d 7377 6974 6368 2069  g)}.rio-switch i
-0005e320: 6e70 7574 7b70 6f73 6974 696f 6e3a 7265  nput{position:re
-0005e330: 6c61 7469 7665 3b77 6964 7468 3a31 3030  lative;width:100
-0005e340: 253b 6865 6967 6874 3a31 3030 253b 7061  %;height:100%;pa
-0005e350: 6464 696e 673a 303b 6d61 7267 696e 3a30  dding:0;margin:0
-0005e360: 3b6f 7061 6369 7479 3a30 3b63 7572 736f  ;opacity:0;curso
-0005e370: 723a 706f 696e 7465 723b 7a2d 696e 6465  r:pointer;z-inde
-0005e380: 783a 337d 2e72 696f 2d73 7769 7463 6820  x:3}.rio-switch 
-0005e390: 2e6b 6e6f 627b 7a2d 696e 6465 783a 323b  .knob{z-index:2;
-0005e3a0: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
-0005e3b0: 653b 746f 703a 2e31 3772 656d 3b6c 6566  e;top:.17rem;lef
-0005e3c0: 743a 2e31 3772 656d 3b77 6964 7468 3a2e  t:.17rem;width:.
-0005e3d0: 3836 7265 6d3b 6865 6967 6874 3a2e 3433  86rem;height:.43
-0005e3e0: 7265 6d3b 7061 6464 696e 673a 2e33 3972  rem;padding:.39r
-0005e3f0: 656d 202e 3137 7265 6d3b 6261 636b 6772  em .17rem;backgr
-0005e400: 6f75 6e64 2d63 6f6c 6f72 3a76 6172 282d  ound-color:var(-
-0005e410: 2d72 696f 2d67 6c6f 6261 6c2d 6469 7361  -rio-global-disa
-0005e420: 626c 6564 2d62 6729 3b62 6f72 6465 722d  bled-bg);border-
-0005e430: 7261 6469 7573 3a35 3025 3b74 7261 6e73  radius:50%;trans
-0005e440: 6974 696f 6e3a 2e33 7320 6561 7365 2061  ition:.3s ease a
-0005e450: 6c6c 2c6c 6566 7420 2e33 7320 6375 6269  ll,left .3s cubi
-0005e460: 632d 6265 7a69 6572 282e 3138 2c2e 3839  c-bezier(.18,.89
-0005e470: 2c2e 3335 2c31 2e31 3529 7d2e 7269 6f2d  ,.35,1.15)}.rio-
-0005e480: 7377 6974 6368 2069 6e70 7574 3a61 6374  switch input:act
-0005e490: 6976 652b 2e6b 6e6f 627b 7769 6474 683a  ive+.knob{width:
-0005e4a0: 312e 3938 7265 6d3b 626f 7264 6572 2d72  1.98rem;border-r
-0005e4b0: 6164 6975 733a 342e 3372 656d 7d2e 7269  adius:4.3rem}.ri
-0005e4c0: 6f2d 7377 6974 6368 2e69 732d 6f6e 2069  o-switch.is-on i
-0005e4d0: 6e70 7574 3a61 6374 6976 652b 2e6b 6e6f  nput:active+.kno
-0005e4e0: 627b 6d61 7267 696e 2d6c 6566 743a 2d31  b{margin-left:-1
-0005e4f0: 2e31 3272 656d 7d2e 7269 6f2d 7377 6974  .12rem}.rio-swit
-0005e500: 6368 2e69 732d 6f6e 2069 6e70 7574 2b2e  ch.is-on input+.
-0005e510: 6b6e 6f62 7b6c 6566 743a 312e 3872 656d  knob{left:1.8rem
-0005e520: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-0005e530: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
-0005e540: 6c2d 6267 297d 2e72 696f 2d64 726f 7064  l-bg)}.rio-dropd
-0005e550: 6f77 6e7b 706f 696e 7465 722d 6576 656e  own{pointer-even
-0005e560: 7473 3a61 7574 6f7d 2e72 696f 2d64 726f  ts:auto}.rio-dro
-0005e570: 7064 6f77 6e2c 2e72 696f 2d64 726f 7064  pdown,.rio-dropd
-0005e580: 6f77 6e3e 696e 7075 747b 6375 7273 6f72  own>input{cursor
-0005e590: 3a70 6f69 6e74 6572 7d2e 7269 6f2d 6472  :pointer}.rio-dr
-0005e5a0: 6f70 646f 776e 2d70 6f70 7570 7b70 6f73  opdown-popup{pos
-0005e5b0: 6974 696f 6e3a 6162 736f 6c75 7465 3b7a  ition:absolute;z
-0005e5c0: 2d69 6e64 6578 3a31 3030 3033 3b68 6569  -index:10003;hei
-0005e5d0: 6768 743a 303b 6d61 782d 6865 6967 6874  ght:0;max-height
-0005e5e0: 3a31 3030 7668 3b62 6163 6b67 726f 756e  :100vh;backgroun
-0005e5f0: 642d 636f 6c6f 723a 7661 7228 2d2d 7269  d-color:var(--ri
-0005e600: 6f2d 676c 6f62 616c 2d62 6163 6b67 726f  o-global-backgro
-0005e610: 756e 642d 6267 293b 636f 6c6f 723a 7661  und-bg);color:va
-0005e620: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d74  r(--rio-global-t
-0005e630: 6578 742d 636f 6c6f 7229 3b62 6f72 6465  ext-color);borde
-0005e640: 722d 7261 6469 7573 3a30 2030 2076 6172  r-radius:0 0 var
-0005e650: 282d 2d72 696f 2d67 6c6f 6261 6c2d 636f  (--rio-global-co
-0005e660: 726e 6572 2d72 6164 6975 732d 736d 616c  rner-radius-smal
-0005e670: 6c29 2076 6172 282d 2d72 696f 2d67 6c6f  l) var(--rio-glo
-0005e680: 6261 6c2d 636f 726e 6572 2d72 6164 6975  bal-corner-radiu
-0005e690: 732d 736d 616c 6c29 3b62 6f78 2d73 6861  s-small);box-sha
-0005e6a0: 646f 773a 3020 3020 2e38 7265 6d20 7661  dow:0 0 .8rem va
-0005e6b0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-0005e6c0: 6861 646f 772d 636f 6c6f 7229 3b74 7261  hadow-color);tra
-0005e6d0: 6e73 6974 696f 6e3a 6865 6967 6874 202e  nsition:height .
-0005e6e0: 3273 2065 6173 652d 696e 2d6f 7574 7d2e  2s ease-in-out}.
-0005e6f0: 7269 6f2d 6472 6f70 646f 776e 2d70 6f70  rio-dropdown-pop
-0005e700: 7570 2d61 626f 7665 7b62 6f72 6465 722d  up-above{border-
-0005e710: 7261 6469 7573 3a76 6172 282d 2d72 696f  radius:var(--rio
-0005e720: 2d67 6c6f 6261 6c2d 636f 726e 6572 2d72  -global-corner-r
-0005e730: 6164 6975 732d 736d 616c 6c29 2169 6d70  adius-small)!imp
-0005e740: 6f72 7461 6e74 7d2e 7269 6f2d 6472 6f70  ortant}.rio-drop
-0005e750: 646f 776e 2e72 696f 2d69 6e70 7574 2d62  down.rio-input-b
-0005e760: 6f78 3e2e 7269 6f2d 6472 6f70 646f 776e  ox>.rio-dropdown
-0005e770: 2d61 7272 6f77 7b70 6f69 6e74 6572 2d65  -arrow{pointer-e
-0005e780: 7665 6e74 733a 6e6f 6e65 3b6f 7264 6572  vents:none;order
-0005e790: 3a32 3b64 6973 706c 6179 3a66 6c65 783b  :2;display:flex;
-0005e7a0: 616c 6967 6e2d 6974 656d 733a 6365 6e74  align-items:cent
-0005e7b0: 6572 7d2e 7269 6f2d 6472 6f70 646f 776e  er}.rio-dropdown
-0005e7c0: 2e72 696f 2d69 6e70 7574 2d62 6f78 3e2e  .rio-input-box>.
-0005e7d0: 7269 6f2d 6472 6f70 646f 776e 2d61 7272  rio-dropdown-arr
-0005e7e0: 6f77 2073 7667 7b77 6964 7468 3a31 2e33  ow svg{width:1.3
-0005e7f0: 7265 6d3b 6865 6967 6874 3a31 2e33 7265  rem;height:1.3re
-0005e800: 6d7d 2e72 696f 2d64 726f 7064 6f77 6e2d  m}.rio-dropdown-
-0005e810: 6f70 7469 6f6e 2d68 6967 686c 6967 6874  option-highlight
-0005e820: 7b66 6f6e 742d 7765 6967 6874 3a37 3030  {font-weight:700
-0005e830: 3b63 6f6c 6f72 3a76 6172 282d 2d72 696f  ;color:var(--rio
-0005e840: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
-0005e850: 6729 7d2e 7269 6f2d 6472 6f70 646f 776e  g)}.rio-dropdown
-0005e860: 2d6f 7074 696f 6e73 7b70 6f73 6974 696f  -options{positio
-0005e870: 6e3a 7265 6c61 7469 7665 3b64 6973 706c  n:relative;displ
-0005e880: 6179 3a66 6c65 783b 666c 6578 2d64 6972  ay:flex;flex-dir
-0005e890: 6563 7469 6f6e 3a63 6f6c 756d 6e3b 616c  ection:column;al
-0005e8a0: 6967 6e2d 6974 656d 733a 7374 7265 7463  ign-items:stretc
-0005e8b0: 683b 6375 7273 6f72 3a70 6f69 6e74 6572  h;cursor:pointer
-0005e8c0: 7d2e 7269 6f2d 6472 6f70 646f 776e 2d6f  }.rio-dropdown-o
-0005e8d0: 7074 696f 6e73 3e64 6976 7b70 6f73 6974  ptions>div{posit
-0005e8e0: 696f 6e3a 7265 6c61 7469 7665 7d2e 7269  ion:relative}.ri
-0005e8f0: 6f2d 6472 6f70 646f 776e 2d6f 7074 696f  o-dropdown-optio
-0005e900: 6e73 3e73 7667 7b70 6f73 6974 696f 6e3a  ns>svg{position:
-0005e910: 7265 6c61 7469 7665 3b77 6964 7468 3a34  relative;width:4
-0005e920: 7265 6d3b 6865 6967 6874 3a34 7265 6d3b  rem;height:4rem;
-0005e930: 6d61 7267 696e 3a31 2e35 7265 6d20 6175  margin:1.5rem au
-0005e940: 746f 3b6f 7061 6369 7479 3a2e 327d 2e72  to;opacity:.2}.r
-0005e950: 696f 2d64 726f 7064 6f77 6e2d 6f70 7469  io-dropdown-opti
-0005e960: 6f6e 3a61 6674 6572 7b63 6f6e 7465 6e74  on:after{content
-0005e970: 3a22 223b 706f 696e 7465 722d 6576 656e  :"";pointer-even
-0005e980: 7473 3a6e 6f6e 653b 706f 7369 7469 6f6e  ts:none;position
-0005e990: 3a61 6273 6f6c 7574 653b 746f 703a 303b  :absolute;top:0;
-0005e9a0: 6c65 6674 3a30 3b72 6967 6874 3a30 3b62  left:0;right:0;b
-0005e9b0: 6f74 746f 6d3a 303b 6261 636b 6772 6f75  ottom:0;backgrou
-0005e9c0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
-0005e9d0: 696f 2d67 6c6f 6261 6c2d 7072 696d 6172  io-global-primar
-0005e9e0: 792d 6267 293b 6f70 6163 6974 793a 303b  y-bg);opacity:0;
-0005e9f0: 7472 616e 7369 7469 6f6e 3a6f 7061 6369  transition:opaci
-0005ea00: 7479 202e 3173 2065 6173 652d 696e 2d6f  ty .1s ease-in-o
-0005ea10: 7574 7d2e 7269 6f2d 6472 6f70 646f 776e  ut}.rio-dropdown
-0005ea20: 2d6f 7074 696f 6e2d 6869 6768 6c69 6768  -option-highligh
-0005ea30: 7465 643a 6166 7465 727b 6f70 6163 6974  ted:after{opacit
-0005ea40: 793a 2e32 7d2e 7269 6f2d 7072 6f67 7265  y:.2}.rio-progre
-0005ea50: 7373 6261 727b 706f 696e 7465 722d 6576  ssbar{pointer-ev
-0005ea60: 656e 7473 3a6e 6f6e 653b 6f76 6572 666c  ents:none;overfl
-0005ea70: 6f77 3a68 6964 6465 6e7d 2e72 696f 2d70  ow:hidden}.rio-p
-0005ea80: 726f 6772 6573 7362 6172 2d74 7261 636b  rogressbar-track
-0005ea90: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
-0005eaa0: 7465 3b77 6964 7468 3a31 3030 253b 6865  te;width:100%;he
-0005eab0: 6967 6874 3a31 3030 253b 6261 636b 6772  ight:100%;backgr
-0005eac0: 6f75 6e64 3a76 6172 282d 2d72 696f 2d6c  ound:var(--rio-l
-0005ead0: 6f63 616c 2d74 6578 742d 636f 6c6f 7229  ocal-text-color)
-0005eae0: 3b6f 7061 6369 7479 3a2e 337d 2e72 696f  ;opacity:.3}.rio
-0005eaf0: 2d70 726f 6772 6573 7362 6172 2d66 696c  -progressbar-fil
-0005eb00: 6c7b 706f 7369 7469 6f6e 3a61 6273 6f6c  l{position:absol
-0005eb10: 7574 653b 6865 6967 6874 3a31 3030 253b  ute;height:100%;
-0005eb20: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-0005eb30: 2d72 696f 2d6c 6f63 616c 2d6c 6576 656c  -rio-local-level
-0005eb40: 2d32 2d62 6729 7d40 6b65 7966 7261 6d65  -2-bg)}@keyframe
-0005eb50: 7320 7269 6f2d 7072 6f67 7265 7373 6261  s rio-progressba
-0005eb60: 722d 616e 696d 6174 696f 6e2d 696e 6465  r-animation-inde
-0005eb70: 7465 726d 696e 6174 657b 3025 7b6c 6566  terminate{0%{lef
-0005eb80: 743a 2d32 3025 3b77 6964 7468 3a36 257d  t:-20%;width:6%}
-0005eb90: 3530 257b 7769 6474 683a 3330 257d 746f  50%{width:30%}to
-0005eba0: 7b6c 6566 743a 3132 3025 3b77 6964 7468  {left:120%;width
-0005ebb0: 3a36 257d 7d2e 7269 6f2d 7072 6f67 7265  :6%}}.rio-progre
-0005ebc0: 7373 6261 722d 696e 6465 7465 726d 696e  ssbar-indetermin
-0005ebd0: 6174 6520 2e72 696f 2d70 726f 6772 6573  ate .rio-progres
-0005ebe0: 7362 6172 2d66 696c 6c7b 7472 616e 7366  sbar-fill{transf
-0005ebf0: 6f72 6d3a 7472 616e 736c 6174 6528 2d35  orm:translate(-5
-0005ec00: 3025 293b 616e 696d 6174 696f 6e3a 7269  0%);animation:ri
-0005ec10: 6f2d 7072 6f67 7265 7373 6261 722d 616e  o-progressbar-an
-0005ec20: 696d 6174 696f 6e2d 696e 6465 7465 726d  imation-indeterm
-0005ec30: 696e 6174 6520 312e 3573 2065 6173 652d  inate 1.5s ease-
-0005ec40: 696e 2d6f 7574 2069 6e66 696e 6974 657d  in-out infinite}
-0005ec50: 2e72 696f 2d70 726f 6772 6573 7362 6172  .rio-progressbar
-0005ec60: 3a6e 6f74 282e 7269 6f2d 7072 6f67 7265  :not(.rio-progre
-0005ec70: 7373 6261 722d 696e 6465 7465 726d 696e  ssbar-indetermin
-0005ec80: 6174 6529 202e 7269 6f2d 7072 6f67 7265  ate) .rio-progre
-0005ec90: 7373 6261 722d 6669 6c6c 7b6c 6566 743a  ssbar-fill{left:
-0005eca0: 303b 7769 6474 683a 7661 7228 2d2d 7269  0;width:var(--ri
-0005ecb0: 6f2d 7072 6f67 7265 7373 6261 722d 6672  o-progressbar-fr
-0005ecc0: 6163 7469 6f6e 293b 7472 616e 7369 7469  action);transiti
-0005ecd0: 6f6e 3a77 6964 7468 202e 3373 2065 6173  on:width .3s eas
-0005ece0: 652d 696e 2d6f 7574 7d2e 7269 6f2d 7072  e-in-out}.rio-pr
-0005ecf0: 6f67 7265 7373 2d63 6972 636c 657b 706f  ogress-circle{po
-0005ed00: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
-0005ed10: 6f3b 7374 726f 6b65 3a76 6172 282d 2d72  o;stroke:var(--r
-0005ed20: 696f 2d6c 6f63 616c 2d62 6729 3b64 6973  io-local-bg);dis
-0005ed30: 706c 6179 3a66 6c65 783b 6a75 7374 6966  play:flex;justif
-0005ed40: 792d 636f 6e74 656e 743a 6365 6e74 6572  y-content:center
-0005ed50: 3b6f 7665 7266 6c6f 773a 6869 6464 656e  ;overflow:hidden
-0005ed60: 7d2e 7269 6f2d 7072 6f67 7265 7373 2d63  }.rio-progress-c
-0005ed70: 6972 636c 6520 6369 7263 6c65 7b66 696c  ircle circle{fil
-0005ed80: 6c3a 6e6f 6e65 3b73 7472 6f6b 652d 7769  l:none;stroke-wi
-0005ed90: 6474 683a 332e 353b 636f 6c6f 723a 7661  dth:3.5;color:va
-0005eda0: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65  r(--rio-local-le
-0005edb0: 7665 6c2d 322d 6267 297d 2e73 7069 6e6e  vel-2-bg)}.spinn
-0005edc0: 696e 6720 7376 677b 7472 616e 7366 6f72  ing svg{transfor
-0005edd0: 6d2d 6f72 6967 696e 3a63 656e 7465 723b  m-origin:center;
-0005ede0: 616e 696d 6174 696f 6e3a 726f 7461 7465  animation:rotate
-0005edf0: 2032 7320 6c69 6e65 6172 2069 6e66 696e   2s linear infin
-0005ee00: 6974 657d 2e73 7069 6e6e 696e 6720 2e70  ite}.spinning .p
-0005ee10: 726f 6772 6573 737b 7374 726f 6b65 2d64  rogress{stroke-d
-0005ee20: 6173 6861 7272 6179 3a31 2c32 3030 3b73  asharray:1,200;s
-0005ee30: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0005ee40: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
-0005ee50: 703a 726f 756e 643b 616e 696d 6174 696f  p:round;animatio
-0005ee60: 6e3a 6461 7368 2031 2e35 7320 6561 7365  n:dash 1.5s ease
-0005ee70: 2d69 6e2d 6f75 7420 696e 6669 6e69 7465  -in-out infinite
-0005ee80: 7d2e 7269 6f2d 7072 6f67 7265 7373 2d63  }.rio-progress-c
-0005ee90: 6972 636c 653a 6e6f 7428 2e73 7069 6e6e  ircle:not(.spinn
-0005eea0: 696e 6729 202e 7072 6f67 7265 7373 7b73  ing) .progress{s
-0005eeb0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0005eec0: 3a2d 3934 2e32 353b 7374 726f 6b65 2d64  :-94.25;stroke-d
-0005eed0: 6173 6861 7272 6179 3a76 6172 282d 2d64  asharray:var(--d
-0005eee0: 6173 6861 7272 6179 293b 7472 616e 7369  asharray);transi
-0005eef0: 7469 6f6e 3a73 7472 6f6b 652d 6461 7368  tion:stroke-dash
-0005ef00: 6172 7261 7920 2e35 7320 6561 7365 7d40  array .5s ease}@
-0005ef10: 6b65 7966 7261 6d65 7320 726f 7461 7465  keyframes rotate
-0005ef20: 7b74 6f7b 7472 616e 7366 6f72 6d3a 726f  {to{transform:ro
-0005ef30: 7461 7465 2833 3630 6465 6729 7d7d 406b  tate(360deg)}}@k
-0005ef40: 6579 6672 616d 6573 2064 6173 687b 3025  eyframes dash{0%
-0005ef50: 7b73 7472 6f6b 652d 6461 7368 6172 7261  {stroke-dasharra
-0005ef60: 793a 312c 3230 303b 7374 726f 6b65 2d64  y:1,200;stroke-d
-0005ef70: 6173 686f 6666 7365 743a 307d 3530 257b  ashoffset:0}50%{
-0005ef80: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0005ef90: 3a39 302c 3230 303b 7374 726f 6b65 2d64  :90,200;stroke-d
-0005efa0: 6173 686f 6666 7365 743a 2d33 3570 787d  ashoffset:-35px}
-0005efb0: 746f 7b73 7472 6f6b 652d 6461 7368 6f66  to{stroke-dashof
-0005efc0: 6673 6574 3a2d 3132 3570 787d 7d2e 7269  fset:-125px}}.ri
-0005efd0: 6f2d 6275 7474 6f6e 7b2d 2d6f 7574 6572  o-button{--outer
-0005efe0: 2d74 6578 742d 636f 6c6f 723a 2076 6172  -text-color: var
-0005eff0: 282d 2d72 696f 2d6c 6f63 616c 2d74 6578  (--rio-local-tex
-0005f000: 742d 636f 6c6f 7229 7d2e 7269 6f2d 6275  t-color)}.rio-bu
-0005f010: 7474 6f6e 3e2a 7b70 6f69 6e74 6572 2d65  tton>*{pointer-e
-0005f020: 7665 6e74 733a 6175 746f 3b70 6f73 6974  vents:auto;posit
-0005f030: 696f 6e3a 7265 6c61 7469 7665 3b77 6964  ion:relative;wid
-0005f040: 7468 3a31 3030 253b 6865 6967 6874 3a31  th:100%;height:1
-0005f050: 3030 253b 6f76 6572 666c 6f77 3a68 6964  00%;overflow:hid
-0005f060: 6465 6e3b 7472 616e 7369 7469 6f6e 3a63  den;transition:c
-0005f070: 6f6c 6f72 202e 3173 2065 6173 652d 696e  olor .1s ease-in
-0005f080: 2d6f 7574 2c62 6f72 6465 722d 636f 6c6f  -out,border-colo
-0005f090: 7220 2e31 7320 6561 7365 2d69 6e2d 6f75  r .1s ease-in-ou
-0005f0a0: 747d 2e72 696f 2d62 7574 746f 6e73 7479  t}.rio-buttonsty
-0005f0b0: 6c65 2d6d 616a 6f72 7b62 6163 6b67 726f  le-major{backgro
-0005f0c0: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-0005f0d0: 7269 6f2d 6c6f 6361 6c2d 6267 293b 626f  rio-local-bg);bo
-0005f0e0: 782d 7368 6164 6f77 3a30 2030 2030 2074  x-shadow:0 0 0 t
-0005f0f0: 7261 6e73 7061 7265 6e74 3b74 7261 6e73  ransparent;trans
-0005f100: 6974 696f 6e3a 6261 636b 6772 6f75 6e64  ition:background
-0005f110: 2d63 6f6c 6f72 202e 3173 2065 6173 652d  -color .1s ease-
-0005f120: 696e 2d6f 7574 2c62 6f78 2d73 6861 646f  in-out,box-shado
-0005f130: 7720 2e32 7320 6561 7365 2d69 6e2d 6f75  w .2s ease-in-ou
-0005f140: 747d 2e72 696f 2d62 7574 746f 6e73 7479  t}.rio-buttonsty
-0005f150: 6c65 2d6d 616a 6f72 3a68 6f76 6572 3a6e  le-major:hover:n
-0005f160: 6f74 282e 7269 6f2d 7377 6974 6368 6572  ot(.rio-switcher
-0005f170: 6f6f 2d64 6973 6162 6c65 6429 7b62 6163  oo-disabled){bac
-0005f180: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
-0005f190: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6267  r(--rio-local-bg
-0005f1a0: 2d61 6374 6976 6529 3b63 7572 736f 723a  -active);cursor:
-0005f1b0: 706f 696e 7465 723b 626f 782d 7368 6164  pointer;box-shad
-0005f1c0: 6f77 3a30 202e 3172 656d 202e 3232 7265  ow:0 .1rem .22re
-0005f1d0: 6d20 2330 3030 3030 3035 397d 2e72 696f  m #00000059}.rio
-0005f1e0: 2d62 7574 746f 6e73 7479 6c65 2d6d 696e  -buttonstyle-min
-0005f1f0: 6f72 3a6e 6f74 283a 686f 7665 7229 7b6f  or:not(:hover){o
-0005f200: 7574 6c69 6e65 3a2e 3172 656d 2073 6f6c  utline:.1rem sol
-0005f210: 6964 2076 6172 282d 2d72 696f 2d6c 6f63  id var(--rio-loc
-0005f220: 616c 2d62 6729 3b2d 2d72 696f 2d6c 6f63  al-bg);--rio-loc
-0005f230: 616c 2d74 6578 742d 636f 6c6f 723a 2076  al-text-color: v
-0005f240: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
-0005f250: 6729 7d2e 7269 6f2d 6275 7474 6f6e 7374  g)}.rio-buttonst
-0005f260: 796c 652d 6d69 6e6f 723a 686f 7665 723a  yle-minor:hover:
-0005f270: 6e6f 7428 2e72 696f 2d73 7769 7463 6865  not(.rio-switche
-0005f280: 726f 6f2d 6469 7361 626c 6564 297b 6261  roo-disabled){ba
-0005f290: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-0005f2a0: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
-0005f2b0: 6729 3b63 7572 736f 723a 706f 696e 7465  g);cursor:pointe
-0005f2c0: 727d 2e72 696f 2d62 7574 746f 6e73 7479  r}.rio-buttonsty
-0005f2d0: 6c65 2d70 6c61 696e 7b2d 2d72 696f 2d6c  le-plain{--rio-l
-0005f2e0: 6f63 616c 2d74 6578 742d 636f 6c6f 723a  ocal-text-color:
-0005f2f0: 2076 6172 282d 2d6f 7574 6572 2d74 6578   var(--outer-tex
-0005f300: 742d 636f 6c6f 7229 7d2e 7269 6f2d 6275  t-color)}.rio-bu
-0005f310: 7474 6f6e 7374 796c 652d 706c 6169 6e3a  ttonstyle-plain:
-0005f320: 686f 7665 723a 6e6f 7428 2e72 696f 2d73  hover:not(.rio-s
-0005f330: 7769 7463 6865 726f 6f2d 6469 7361 626c  witcheroo-disabl
-0005f340: 6564 297b 6375 7273 6f72 3a70 6f69 6e74  ed){cursor:point
-0005f350: 6572 3b2d 2d72 696f 2d6c 6f63 616c 2d74  er;--rio-local-t
-0005f360: 6578 742d 636f 6c6f 723a 2076 6172 282d  ext-color: var(-
-0005f370: 2d72 696f 2d6c 6f63 616c 2d62 6729 7d2e  -rio-local-bg)}.
-0005f380: 7269 6f2d 7368 6170 652d 7069 6c6c 7b62  rio-shape-pill{b
-0005f390: 6f72 6465 722d 7261 6469 7573 3a39 3939  order-radius:999
-0005f3a0: 3939 7078 7d2e 7269 6f2d 7368 6170 652d  99px}.rio-shape-
-0005f3b0: 726f 756e 6465 647b 626f 7264 6572 2d72  rounded{border-r
-0005f3c0: 6164 6975 733a 7661 7228 2d2d 7269 6f2d  adius:var(--rio-
-0005f3d0: 676c 6f62 616c 2d63 6f72 6e65 722d 7261  global-corner-ra
-0005f3e0: 6469 7573 2d73 6d61 6c6c 297d 2e72 696f  dius-small)}.rio
-0005f3f0: 2d73 6861 7065 2d72 6563 7461 6e67 6c65  -shape-rectangle
-0005f400: 7b62 6f72 6465 722d 7261 6469 7573 3a30  {border-radius:0
-0005f410: 7d2e 7269 6f2d 7368 6170 652d 6369 7263  }.rio-shape-circ
-0005f420: 6c65 7b62 6f72 6465 722d 7261 6469 7573  le{border-radius
-0005f430: 3a35 3025 7d2e 7269 6f2d 7265 7665 616c  :50%}.rio-reveal
-0005f440: 6572 7b64 6973 706c 6179 3a66 6c65 783b  er{display:flex;
-0005f450: 666c 6578 2d64 6972 6563 7469 6f6e 3a63  flex-direction:c
-0005f460: 6f6c 756d 6e3b 616c 6967 6e2d 6974 656d  olumn;align-item
-0005f470: 733a 7374 7265 7463 683b 6a75 7374 6966  s:stretch;justif
-0005f480: 792d 636f 6e74 656e 743a 7374 7265 7463  y-content:stretc
-0005f490: 683b 626f 7264 6572 2d72 6164 6975 733a  h;border-radius:
-0005f4a0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-0005f4b0: 2d63 6f72 6e65 722d 7261 6469 7573 2d73  -corner-radius-s
-0005f4c0: 6d61 6c6c 293b 7472 616e 7369 7469 6f6e  mall);transition
-0005f4d0: 3a62 6163 6b67 726f 756e 642d 636f 6c6f  :background-colo
-0005f4e0: 7220 2e31 3573 2065 6173 652d 6f75 743b  r .15s ease-out;
-0005f4f0: 6f76 6572 666c 6f77 3a68 6964 6465 6e7d  overflow:hidden}
-0005f500: 2e72 696f 2d72 6576 6561 6c65 722d 6865  .rio-revealer-he
-0005f510: 6164 6572 7b70 6f69 6e74 6572 2d65 7665  ader{pointer-eve
-0005f520: 6e74 733a 6175 746f 3b63 7572 736f 723a  nts:auto;cursor:
-0005f530: 706f 696e 7465 723b 6469 7370 6c61 793a  pointer;display:
-0005f540: 666c 6578 3b61 6c69 676e 2d69 7465 6d73  flex;align-items
-0005f550: 3a63 656e 7465 723b 6a75 7374 6966 792d  :center;justify-
-0005f560: 636f 6e74 656e 743a 7370 6163 652d 6265  content:space-be
-0005f570: 7477 6565 6e3b 636f 6c6f 723a 7661 7228  tween;color:var(
-0005f580: 2d2d 7269 6f2d 6c6f 6361 6c2d 7465 7874  --rio-local-text
-0005f590: 2d63 6f6c 6f72 297d 2e72 696f 2d72 6576  -color)}.rio-rev
-0005f5a0: 6561 6c65 722d 6c61 6265 6c7b 666c 6578  ealer-label{flex
-0005f5b0: 2d67 726f 773a 317d 2e72 696f 2d72 6576  -grow:1}.rio-rev
-0005f5c0: 6561 6c65 722d 6172 726f 777b 7472 616e  ealer-arrow{tran
-0005f5d0: 7366 6f72 6d3a 726f 7461 7465 2839 3064  sform:rotate(90d
-0005f5e0: 6567 293b 7472 616e 7369 7469 6f6e 3a74  eg);transition:t
-0005f5f0: 7261 6e73 666f 726d 202e 3235 7320 6561  ransform .25s ea
-0005f600: 7365 2d69 6e2d 6f75 747d 2e72 696f 2d72  se-in-out}.rio-r
-0005f610: 6576 6561 6c65 722d 6f70 656e 202e 7269  evealer-open .ri
-0005f620: 6f2d 7265 7665 616c 6572 2d61 7272 6f77  o-revealer-arrow
-0005f630: 7b74 7261 6e73 666f 726d 3a72 6f74 6174  {transform:rotat
-0005f640: 6528 3029 7d2e 7269 6f2d 7265 7665 616c  e(0)}.rio-reveal
-0005f650: 6572 2d63 6f6e 7465 6e74 2d6f 7574 6572  er-content-outer
-0005f660: 7b66 6c65 782d 6772 6f77 3a31 3b70 6f73  {flex-grow:1;pos
-0005f670: 6974 696f 6e3a 7265 6c61 7469 7665 3b6f  ition:relative;o
-0005f680: 7665 7266 6c6f 773a 6869 6464 656e 7d2e  verflow:hidden}.
-0005f690: 7269 6f2d 7265 7665 616c 6572 2d63 6f6e  rio-revealer-con
-0005f6a0: 7465 6e74 2d69 6e6e 6572 7b70 6f73 6974  tent-inner{posit
-0005f6b0: 696f 6e3a 6162 736f 6c75 7465 3b62 6f74  ion:absolute;bot
-0005f6c0: 746f 6d3a 303b 6f70 6163 6974 793a 303b  tom:0;opacity:0;
-0005f6d0: 7472 616e 7366 6f72 6d3a 7472 616e 736c  transform:transl
-0005f6e0: 6174 6559 282d 3530 2529 3b74 7261 6e73  ateY(-50%);trans
-0005f6f0: 6974 696f 6e3a 6f70 6163 6974 7920 2e34  ition:opacity .4
-0005f700: 3573 2065 6173 652d 696e 2d6f 7574 2c74  5s ease-in-out,t
-0005f710: 7261 6e73 666f 726d 202e 3335 7320 6561  ransform .35s ea
-0005f720: 7365 7d2e 7269 6f2d 7265 7665 616c 6572  se}.rio-revealer
-0005f730: 2d6f 7065 6e20 2e72 696f 2d72 6576 6561  -open .rio-revea
-0005f740: 6c65 722d 636f 6e74 656e 742d 696e 6e65  ler-content-inne
-0005f750: 727b 6f70 6163 6974 793a 313b 7472 616e  r{opacity:1;tran
-0005f760: 7366 6f72 6d3a 7472 616e 736c 6174 6559  sform:translateY
-0005f770: 2830 297d 2e72 696f 2d72 6576 6561 6c65  (0)}.rio-reveale
-0005f780: 722d 636f 6e74 656e 742d 696e 6e65 723e  r-content-inner>
-0005f790: 2a7b 706f 7369 7469 6f6e 3a72 656c 6174  *{position:relat
-0005f7a0: 6976 6521 696d 706f 7274 616e 747d 2e72  ive!important}.r
-0005f7b0: 696f 2d70 6c6f 747b 6469 7370 6c61 793a  io-plot{display:
-0005f7c0: 696e 6c69 6e65 2d62 6c6f 636b 3b64 6973  inline-block;dis
-0005f7d0: 706c 6179 3a66 6c65 783b 6a75 7374 6966  play:flex;justif
-0005f7e0: 792d 636f 6e74 656e 743a 6365 6e74 6572  y-content:center
-0005f7f0: 3b61 6c69 676e 2d69 7465 6d73 3a63 656e  ;align-items:cen
-0005f800: 7465 723b 6f76 6572 666c 6f77 3a68 6964  ter;overflow:hid
-0005f810: 6465 6e7d 2e72 696f 2d69 636f 6e7b 706f  den}.rio-icon{po
-0005f820: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
-0005f830: 6f3b 6469 7370 6c61 793a 666c 6578 3b6a  o;display:flex;j
-0005f840: 7573 7469 6679 2d63 6f6e 7465 6e74 3a63  ustify-content:c
-0005f850: 656e 7465 723b 616c 6967 6e2d 6974 656d  enter;align-item
-0005f860: 733a 6365 6e74 6572 7d2e 7269 6f2d 736c  s:center}.rio-sl
-0005f870: 6964 6572 7b70 6f69 6e74 6572 2d65 7665  ider{pointer-eve
-0005f880: 6e74 733a 6175 746f 3b2d 2d72 696f 2d73  nts:auto;--rio-s
-0005f890: 6c69 6465 722d 706f 7369 7469 6f6e 2d74  lider-position-t
-0005f8a0: 7261 6e73 6974 696f 6e2d 7469 6d65 3a20  ransition-time: 
-0005f8b0: 2e33 737d 2e72 696f 2d73 6c69 6465 723a  .3s}.rio-slider:
-0005f8c0: 6e6f 7428 2e72 696f 2d73 7769 7463 6865  not(.rio-switche
-0005f8d0: 726f 6f2d 6469 7361 626c 6564 297b 6375  roo-disabled){cu
-0005f8e0: 7273 6f72 3a70 6f69 6e74 6572 7d2e 7269  rsor:pointer}.ri
-0005f8f0: 6f2d 736c 6964 6572 2d69 6e6e 6572 7b70  o-slider-inner{p
-0005f900: 6f69 6e74 6572 2d65 7665 6e74 733a 6e6f  ointer-events:no
-0005f910: 6e65 3b70 6f73 6974 696f 6e3a 6162 736f  ne;position:abso
-0005f920: 6c75 7465 3b6c 6566 743a 2e36 7265 6d3b  lute;left:.6rem;
-0005f930: 7269 6768 743a 2e36 7265 6d3b 6865 6967  right:.6rem;heig
-0005f940: 6874 3a2e 3235 7265 6d3b 746f 703a 3530  ht:.25rem;top:50
-0005f950: 253b 7472 616e 7366 6f72 6d3a 7472 616e  %;transform:tran
-0005f960: 736c 6174 6559 282d 3530 2529 7d2e 7269  slateY(-50%)}.ri
-0005f970: 6f2d 736c 6964 6572 2d74 7261 636b 7b70  o-slider-track{p
-0005f980: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
-0005f990: 3b77 6964 7468 3a31 3030 253b 6865 6967  ;width:100%;heig
-0005f9a0: 6874 3a31 3030 253b 6f70 6163 6974 793a  ht:100%;opacity:
-0005f9b0: 2e33 3b62 6163 6b67 726f 756e 643a 7661  .3;background:va
-0005f9c0: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  r(--rio-local-te
-0005f9d0: 7874 2d63 6f6c 6f72 293b 626f 7264 6572  xt-color);border
-0005f9e0: 2d72 6164 6975 733a 3939 3939 3970 787d  -radius:99999px}
-0005f9f0: 2e72 696f 2d73 6c69 6465 722d 6669 6c6c  .rio-slider-fill
-0005fa00: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
-0005fa10: 7465 3b6c 6566 743a 303b 7769 6474 683a  te;left:0;width:
-0005fa20: 7661 7228 2d2d 7269 6f2d 736c 6964 6572  var(--rio-slider
-0005fa30: 2d66 7261 6374 696f 6e29 3b68 6569 6768  -fraction);heigh
-0005fa40: 743a 3130 3025 3b62 6163 6b67 726f 756e  t:100%;backgroun
-0005fa50: 643a 7661 7228 2d2d 7269 6f2d 6c6f 6361  d:var(--rio-loca
-0005fa60: 6c2d 6c65 7665 6c2d 322d 6267 293b 626f  l-level-2-bg);bo
-0005fa70: 7264 6572 2d72 6164 6975 733a 3939 3939  rder-radius:9999
-0005fa80: 3970 783b 7472 616e 7369 7469 6f6e 3a77  9px;transition:w
-0005fa90: 6964 7468 2076 6172 282d 2d72 696f 2d73  idth var(--rio-s
-0005faa0: 6c69 6465 722d 706f 7369 7469 6f6e 2d74  lider-position-t
-0005fab0: 7261 6e73 6974 696f 6e2d 7469 6d65 2920  ransition-time) 
-0005fac0: 6561 7365 2d69 6e2d 6f75 747d 2e72 696f  ease-in-out}.rio
-0005fad0: 2d73 6c69 6465 722d 676c 6f77 7b70 6f73  -slider-glow{pos
-0005fae0: 6974 696f 6e3a 6162 736f 6c75 7465 3b6c  ition:absolute;l
-0005faf0: 6566 743a 7661 7228 2d2d 7269 6f2d 736c  eft:var(--rio-sl
-0005fb00: 6964 6572 2d66 7261 6374 696f 6e29 3b74  ider-fraction);t
-0005fb10: 6f70 3a35 3025 3b77 6964 7468 3a31 2e31  op:50%;width:1.1
-0005fb20: 7265 6d3b 6865 6967 6874 3a31 2e31 7265  rem;height:1.1re
-0005fb30: 6d3b 7472 616e 7366 6f72 6d3a 7472 616e  m;transform:tran
-0005fb40: 736c 6174 6528 2d35 3025 2c2d 3530 2529  slate(-50%,-50%)
-0005fb50: 3b62 6f72 6465 722d 7261 6469 7573 3a35  ;border-radius:5
-0005fb60: 3025 3b62 6163 6b67 726f 756e 642d 636f  0%;background-co
-0005fb70: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
-0005fb80: 6361 6c2d 6c65 7665 6c2d 322d 6267 293b  cal-level-2-bg);
-0005fb90: 6f70 6163 6974 793a 3025 3b74 7261 6e73  opacity:0%;trans
-0005fba0: 6974 696f 6e3a 6c65 6674 2076 6172 282d  ition:left var(-
-0005fbb0: 2d72 696f 2d73 6c69 6465 722d 706f 7369  -rio-slider-posi
-0005fbc0: 7469 6f6e 2d74 7261 6e73 6974 696f 6e2d  tion-transition-
-0005fbd0: 7469 6d65 2920 6561 7365 2d69 6e2d 6f75  time) ease-in-ou
-0005fbe0: 742c 7769 6474 6820 2e31 3573 2065 6173  t,width .15s eas
-0005fbf0: 652d 696e 2d6f 7574 2c68 6569 6768 7420  e-in-out,height 
-0005fc00: 2e31 3573 2065 6173 652d 696e 2d6f 7574  .15s ease-in-out
-0005fc10: 2c6f 7061 6369 7479 202e 3135 7320 6561  ,opacity .15s ea
-0005fc20: 7365 2d69 6e2d 6f75 747d 2e72 696f 2d73  se-in-out}.rio-s
-0005fc30: 6c69 6465 723a 686f 7665 723a 6e6f 7428  lider:hover:not(
-0005fc40: 2e72 696f 2d73 7769 7463 6865 726f 6f2d  .rio-switcheroo-
-0005fc50: 6469 7361 626c 6564 2920 2e72 696f 2d73  disabled) .rio-s
-0005fc60: 6c69 6465 722d 676c 6f77 7b77 6964 7468  lider-glow{width
-0005fc70: 3a32 2e38 7265 6d3b 6865 6967 6874 3a32  :2.8rem;height:2
-0005fc80: 2e38 7265 6d3b 6f70 6163 6974 793a 3230  .8rem;opacity:20
-0005fc90: 257d 2e72 696f 2d73 6c69 6465 722d 6b6e  %}.rio-slider-kn
-0005fca0: 6f62 7b70 6f73 6974 696f 6e3a 6162 736f  ob{position:abso
-0005fcb0: 6c75 7465 3b6c 6566 743a 7661 7228 2d2d  lute;left:var(--
-0005fcc0: 7269 6f2d 736c 6964 6572 2d66 7261 6374  rio-slider-fract
-0005fcd0: 696f 6e29 3b74 6f70 3a35 3025 3b77 6964  ion);top:50%;wid
-0005fce0: 7468 3a31 2e32 7265 6d3b 6865 6967 6874  th:1.2rem;height
-0005fcf0: 3a31 2e32 7265 6d3b 7472 616e 7366 6f72  :1.2rem;transfor
-0005fd00: 6d3a 7472 616e 736c 6174 6528 2d35 3025  m:translate(-50%
-0005fd10: 2c2d 3530 2529 3b62 6f72 6465 722d 7261  ,-50%);border-ra
-0005fd20: 6469 7573 3a35 3025 3b62 6163 6b67 726f  dius:50%;backgro
-0005fd30: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-0005fd40: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-0005fd50: 322d 6267 293b 626f 782d 7368 6164 6f77  2-bg);box-shadow
-0005fd60: 3a30 202e 3172 656d 202e 3272 656d 2076  :0 .1rem .2rem v
-0005fd70: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-0005fd80: 7368 6164 6f77 2d63 6f6c 6f72 293b 7472  shadow-color);tr
-0005fd90: 616e 7369 7469 6f6e 3a6c 6566 7420 7661  ansition:left va
-0005fda0: 7228 2d2d 7269 6f2d 736c 6964 6572 2d70  r(--rio-slider-p
-0005fdb0: 6f73 6974 696f 6e2d 7472 616e 7369 7469  osition-transiti
-0005fdc0: 6f6e 2d74 696d 6529 2065 6173 652d 696e  on-time) ease-in
-0005fdd0: 2d6f 7574 2c62 6163 6b67 726f 756e 642d  -out,background-
-0005fde0: 636f 6c6f 7220 2e31 7320 6561 7365 2d69  color .1s ease-i
-0005fdf0: 6e2d 6f75 747d 2e72 696f 2d73 6c69 6465  n-out}.rio-slide
-0005fe00: 7368 6f77 7b70 6f69 6e74 6572 2d65 7665  show{pointer-eve
-0005fe10: 6e74 733a 6175 746f 3b6f 7665 7266 6c6f  nts:auto;overflo
-0005fe20: 773a 6869 6464 656e 7d2e 736c 6964 6573  w:hidden}.slides
-0005fe30: 686f 772d 6368 696c 642d 636f 6e74 6169  how-child-contai
-0005fe40: 6e65 727b 706f 7369 7469 6f6e 3a72 656c  ner{position:rel
-0005fe50: 6174 6976 653b 6469 7370 6c61 793a 6772  ative;display:gr
-0005fe60: 6964 3b77 6964 7468 3a31 3030 253b 6865  id;width:100%;he
-0005fe70: 6967 6874 3a31 3030 257d 2e73 6c69 6465  ight:100%}.slide
-0005fe80: 7368 6f77 2d63 6869 6c64 2d63 6f6e 7461  show-child-conta
-0005fe90: 696e 6572 3e64 6976 7b67 7269 642d 636f  iner>div{grid-co
-0005fea0: 6c75 6d6e 2d73 7461 7274 3a31 3b67 7269  lumn-start:1;gri
-0005feb0: 642d 726f 772d 7374 6172 743a 313b 7769  d-row-start:1;wi
-0005fec0: 6474 683a 3130 3025 3b68 6569 6768 743a  dth:100%;height:
-0005fed0: 3130 3025 7d2e 736c 6964 6573 686f 772d  100%}.slideshow-
-0005fee0: 6368 696c 642d 636f 6e74 6169 6e65 723e  child-container>
-0005fef0: 6469 763e 2a7b 6772 6964 2d63 6f6c 756d  div>*{grid-colum
-0005ff00: 6e2d 7374 6172 743a 313b 6772 6964 2d72  n-start:1;grid-r
-0005ff10: 6f77 2d73 7461 7274 3a31 3b77 6964 7468  ow-start:1;width
-0005ff20: 3a31 3030 253b 6865 6967 6874 3a31 3030  :100%;height:100
-0005ff30: 257d 2e73 6c69 6465 7368 6f77 2d70 726f  %}.slideshow-pro
-0005ff40: 6772 6573 737b 706f 7369 7469 6f6e 3a61  gress{position:a
-0005ff50: 6273 6f6c 7574 653b 626f 7474 6f6d 3a30  bsolute;bottom:0
-0005ff60: 3b77 6964 7468 3a31 3030 253b 6865 6967  ;width:100%;heig
-0005ff70: 6874 3a2e 3372 656d 3b62 6163 6b67 726f  ht:.3rem;backgro
-0005ff80: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-0005ff90: 7269 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d  rio-local-level-
-0005ffa0: 322d 6267 297d 2e72 696f 2d6f 7665 726c  2-bg)}.rio-overl
-0005ffb0: 6179 7b70 6f69 6e74 6572 2d65 7665 6e74  ay{pointer-event
-0005ffc0: 733a 6e6f 6e65 3b70 6f73 6974 696f 6e3a  s:none;position:
-0005ffd0: 6669 7865 6421 696d 706f 7274 616e 743b  fixed!important;
-0005ffe0: 746f 703a 3021 696d 706f 7274 616e 743b  top:0!important;
-0005fff0: 6c65 6674 3a30 2169 6d70 6f72 7461 6e74  left:0!important
-00060000: 3b77 6964 7468 3a75 6e73 6574 2169 6d70  ;width:unset!imp
-00060010: 6f72 7461 6e74 3b68 6569 6768 743a 756e  ortant;height:un
-00060020: 7365 7421 696d 706f 7274 616e 743b 7a2d  set!important;z-
-00060030: 696e 6465 783a 3130 3030 307d 2e72 696f  index:10000}.rio
-00060040: 2d73 7061 6365 727b 706f 696e 7465 722d  -spacer{pointer-
-00060050: 6576 656e 7473 3a6e 6f6e 657d 2e72 696f  events:none}.rio
-00060060: 2d6d 6564 6961 2d70 6c61 7965 727b 706f  -media-player{po
-00060070: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
-00060080: 6f7d 2e72 696f 2d6d 6564 6961 2d70 6c61  o}.rio-media-pla
-00060090: 7965 7220 7669 6465 6f7b 706f 696e 7465  yer video{pointe
-000600a0: 722d 6576 656e 7473 3a6e 6f6e 653b 7769  r-events:none;wi
-000600b0: 6474 683a 3130 3025 3b68 6569 6768 743a  dth:100%;height:
-000600c0: 3130 3025 3b6f 626a 6563 742d 6669 743a  100%;object-fit:
-000600d0: 636f 6e74 6169 6e7d 2e72 696f 2d6d 6564  contain}.rio-med
-000600e0: 6961 2d70 6c61 7965 722d 616c 742d 6469  ia-player-alt-di
-000600f0: 7370 6c61 797b 706f 696e 7465 722d 6576  splay{pointer-ev
-00060100: 656e 7473 3a6e 6f6e 653b 706f 7369 7469  ents:none;positi
-00060110: 6f6e 3a61 6273 6f6c 7574 653b 6c65 6674  on:absolute;left
-00060120: 3a35 3025 3b74 6f70 3a35 3025 3b77 6964  :50%;top:50%;wid
-00060130: 7468 3a35 3025 3b68 6569 6768 743a 3530  th:50%;height:50
-00060140: 253b 6d61 782d 7769 6474 683a 3230 7265  %;max-width:20re
-00060150: 6d3b 6d61 782d 6865 6967 6874 3a32 3072  m;max-height:20r
-00060160: 656d 3b61 7370 6563 742d 7261 7469 6f3a  em;aspect-ratio:
-00060170: 313b 6f70 6163 6974 793a 2e35 3b74 7261  1;opacity:.5;tra
-00060180: 6e73 666f 726d 3a74 7261 6e73 6c61 7465  nsform:translate
-00060190: 282d 3530 252c 2d35 3025 297d 2e72 696f  (-50%,-50%)}.rio
-000601a0: 2d6d 6564 6961 2d70 6c61 7965 722d 636f  -media-player-co
-000601b0: 6e74 726f 6c73 7b70 6f73 6974 696f 6e3a  ntrols{position:
-000601c0: 6162 736f 6c75 7465 3b6c 6566 743a 303b  absolute;left:0;
-000601d0: 626f 7474 6f6d 3a30 3b72 6967 6874 3a30  bottom:0;right:0
-000601e0: 3b62 6163 6b67 726f 756e 643a 6c69 6e65  ;background:line
-000601f0: 6172 2d67 7261 6469 656e 7428 7267 6261  ar-gradient(rgba
-00060200: 2830 2c30 2c30 2c30 292c 7267 6261 2830  (0,0,0,0),rgba(0
-00060210: 2c30 2c30 2c2e 3629 293b 7061 6464 696e  ,0,0,.6));paddin
-00060220: 672d 746f 703a 322e 3572 656d 3b64 6973  g-top:2.5rem;dis
-00060230: 706c 6179 3a66 6c65 783b 666c 6578 2d64  play:flex;flex-d
-00060240: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
-00060250: 6761 703a 3072 656d 3b61 6c69 676e 2d69  gap:0rem;align-i
-00060260: 7465 6d73 3a73 7472 6574 6368 3b74 7261  tems:stretch;tra
-00060270: 6e73 6974 696f 6e3a 6f70 6163 6974 7920  nsition:opacity 
-00060280: 2e34 7320 6561 7365 2d69 6e2d 6f75 747d  .4s ease-in-out}
-00060290: 2e72 696f 2d6d 6564 6961 2d70 6c61 7965  .rio-media-playe
-000602a0: 722d 7469 6d65 6c69 6e65 7b70 6f69 6e74  r-timeline{point
-000602b0: 6572 2d65 7665 6e74 733a 6175 746f 3b63  er-events:auto;c
-000602c0: 7572 736f 723a 706f 696e 7465 723b 706f  ursor:pointer;po
-000602d0: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
-000602e0: 6865 6967 6874 3a32 7265 6d3b 6d61 7267  height:2rem;marg
-000602f0: 696e 3a30 202e 3572 656d 7d2e 7269 6f2d  in:0 .5rem}.rio-
-00060300: 6d65 6469 612d 706c 6179 6572 2d74 696d  media-player-tim
-00060310: 656c 696e 653e 6469 767b 706f 696e 7465  eline>div{pointe
-00060320: 722d 6576 656e 7473 3a6e 6f6e 653b 706f  r-events:none;po
-00060330: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
-00060340: 746f 703a 3530 253b 6865 6967 6874 3a2e  top:50%;height:.
-00060350: 3272 656d 3b74 7261 6e73 666f 726d 3a74  2rem;transform:t
-00060360: 7261 6e73 6c61 7465 5928 2d35 3025 293b  ranslateY(-50%);
-00060370: 7472 616e 7369 7469 6f6e 3a68 6569 6768  transition:heigh
-00060380: 7420 2e32 7320 6561 7365 2d69 6e2d 6f75  t .2s ease-in-ou
-00060390: 747d 2e72 696f 2d6d 6564 6961 2d70 6c61  t}.rio-media-pla
-000603a0: 7965 722d 7469 6d65 6c69 6e65 3a68 6f76  yer-timeline:hov
-000603b0: 6572 3e64 6976 7b68 6569 6768 743a 2e34  er>div{height:.4
-000603c0: 7265 6d7d 2e72 696f 2d6d 6564 6961 2d70  rem}.rio-media-p
-000603d0: 6c61 7965 722d 7469 6d65 6c69 6e65 2d6b  layer-timeline-k
-000603e0: 6e6f 627b 706f 7369 7469 6f6e 3a61 6273  nob{position:abs
-000603f0: 6f6c 7574 653b 7769 6474 683a 3072 656d  olute;width:0rem
-00060400: 3b68 6569 6768 743a 3072 656d 3b6c 6566  ;height:0rem;lef
-00060410: 743a 3130 3025 3b74 6f70 3a35 3025 3b62  t:100%;top:50%;b
-00060420: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00060430: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00060440: 2d70 7269 6d61 7279 2d62 6729 3b62 6f72  -primary-bg);bor
-00060450: 6465 722d 7261 6469 7573 3a35 3025 3b74  der-radius:50%;t
-00060460: 7261 6e73 666f 726d 3a74 7261 6e73 6c61  ransform:transla
-00060470: 7465 282d 3530 252c 2d35 3025 293b 7472  te(-50%,-50%);tr
-00060480: 616e 7369 7469 6f6e 3a77 6964 7468 202e  ansition:width .
-00060490: 3273 2065 6173 652d 696e 2d6f 7574 2c68  2s ease-in-out,h
-000604a0: 6569 6768 7420 2e32 7320 6561 7365 2d69  eight .2s ease-i
-000604b0: 6e2d 6f75 747d 2e72 696f 2d6d 6564 6961  n-out}.rio-media
-000604c0: 2d70 6c61 7965 722d 7469 6d65 6c69 6e65  -player-timeline
-000604d0: 3a68 6f76 6572 202e 7269 6f2d 6d65 6469  :hover .rio-medi
-000604e0: 612d 706c 6179 6572 2d74 696d 656c 696e  a-player-timelin
-000604f0: 652d 6b6e 6f62 7b77 6964 7468 3a2e 3972  e-knob{width:.9r
-00060500: 656d 3b68 6569 6768 743a 2e39 7265 6d7d  em;height:.9rem}
-00060510: 2e72 696f 2d6d 6564 6961 2d70 6c61 7965  .rio-media-playe
-00060520: 722d 7469 6d65 6c69 6e65 2d62 6163 6b67  r-timeline-backg
-00060530: 726f 756e 642c 2e72 696f 2d6d 6564 6961  round,.rio-media
-00060540: 2d70 6c61 7965 722d 7469 6d65 6c69 6e65  -player-timeline
-00060550: 2d6c 6f61 6465 642c 2e72 696f 2d6d 6564  -loaded,.rio-med
-00060560: 6961 2d70 6c61 7965 722d 7469 6d65 6c69  ia-player-timeli
-00060570: 6e65 2d68 6f76 6572 2c2e 7269 6f2d 6d65  ne-hover,.rio-me
-00060580: 6469 612d 706c 6179 6572 2d74 696d 656c  dia-player-timel
-00060590: 696e 652d 706c 6179 6564 7b70 6f73 6974  ine-played{posit
-000605a0: 696f 6e3a 6162 736f 6c75 7465 3b77 6964  ion:absolute;wid
-000605b0: 7468 3a30 253b 6865 6967 6874 3a31 3030  th:0%;height:100
-000605c0: 253b 6261 636b 6772 6f75 6e64 2d63 6f6c  %;background-col
-000605d0: 6f72 3a23 6666 663b 626f 7264 6572 2d72  or:#fff;border-r
-000605e0: 6164 6975 733a 3939 3939 3970 787d 2e72  adius:99999px}.r
+0005ced0: 7479 7065 2c68 746d 6c5b 6461 7461 2d74  type,html[data-t
+0005cee0: 6865 6d65 3d64 6172 6b5d 202e 686c 6a73  heme=dark] .hljs
+0005cef0: 2d6e 616d 652c 6874 6d6c 5b64 6174 612d  -name,html[data-
+0005cf00: 7468 656d 653d 6461 726b 5d20 2e68 6c6a  theme=dark] .hlj
+0005cf10: 732d 7374 726f 6e67 7b66 6f6e 742d 7765  s-strong{font-we
+0005cf20: 6967 6874 3a37 3030 7d68 746d 6c5b 6461  ight:700}html[da
+0005cf30: 7461 2d74 6865 6d65 3d64 6172 6b5d 202e  ta-theme=dark] .
+0005cf40: 686c 6a73 2d65 6d70 6861 7369 737b 666f  hljs-emphasis{fo
+0005cf50: 6e74 2d73 7479 6c65 3a69 7461 6c69 637d  nt-style:italic}
+0005cf60: 406b 6579 6672 616d 6573 2063 6f6e 7465  @keyframes conte
+0005cf70: 6e74 2d6c 6f61 6469 6e67 7b30 257b 6261  nt-loading{0%{ba
+0005cf80: 636b 6772 6f75 6e64 2d70 6f73 6974 696f  ckground-positio
+0005cf90: 6e3a 2d31 3030 7265 6d20 307d 746f 7b62  n:-100rem 0}to{b
+0005cfa0: 6163 6b67 726f 756e 642d 706f 7369 7469  ackground-positi
+0005cfb0: 6f6e 3a30 2030 7d7d 2e72 696f 2d63 6f6e  on:0 0}}.rio-con
+0005cfc0: 7465 6e74 2d6c 6f61 6469 6e67 7b62 6163  tent-loading{bac
+0005cfd0: 6b67 726f 756e 642d 696d 6167 653a 6c69  kground-image:li
+0005cfe0: 6e65 6172 2d67 7261 6469 656e 7428 746f  near-gradient(to
+0005cff0: 2072 6967 6874 2c74 7261 6e73 7061 7265   right,transpare
+0005d000: 6e74 2031 3025 2c76 6172 282d 2d72 696f  nt 10%,var(--rio
+0005d010: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
+0005d020: 6729 2031 3225 2c74 7261 6e73 7061 7265  g) 12%,transpare
+0005d030: 6e74 2031 3425 293b 6261 636b 6772 6f75  nt 14%);backgrou
+0005d040: 6e64 2d73 697a 653a 3130 3072 656d 2035  nd-size:100rem 5
+0005d050: 7265 6d3b 616e 696d 6174 696f 6e3a 636f  rem;animation:co
+0005d060: 6e74 656e 742d 6c6f 6164 696e 6720 3373  ntent-loading 3s
+0005d070: 206c 696e 6561 7220 696e 6669 6e69 7465   linear infinite
+0005d080: 7d40 6b65 7966 7261 6d65 7320 6261 7262  }@keyframes barb
+0005d090: 6572 2d70 6f6c 657b 3025 7b62 6163 6b67  er-pole{0%{backg
+0005d0a0: 726f 756e 642d 706f 7369 7469 6f6e 3a30  round-position:0
+0005d0b0: 2030 7d74 6f7b 6261 636b 6772 6f75 6e64   0}to{background
+0005d0c0: 2d70 6f73 6974 696f 6e3a 3372 656d 2030  -position:3rem 0
+0005d0d0: 7265 6d7d 7d61 7b63 6f6c 6f72 3a76 6172  rem}}a{color:var
+0005d0e0: 282d 2d72 696f 2d6c 6f63 616c 2d6c 6576  (--rio-local-lev
+0005d0f0: 656c 2d32 2d62 6729 7d61 3a68 6f76 6572  el-2-bg)}a:hover
+0005d100: 7b63 6f6c 6f72 3a76 6172 282d 2d72 696f  {color:var(--rio
+0005d110: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
+0005d120: 672d 6163 7469 7665 297d 636f 6465 7b66  g-active)}code{f
+0005d130: 6f6e 742d 6661 6d69 6c79 3a76 6172 282d  ont-family:var(-
+0005d140: 2d72 696f 2d67 6c6f 6261 6c2d 6d6f 6e6f  -rio-global-mono
+0005d150: 7370 6163 652d 666f 6e74 292c 6d6f 6e6f  space-font),mono
+0005d160: 7370 6163 657d 6874 6d6c 7b62 6163 6b67  space}html{backg
+0005d170: 726f 756e 643a 7661 7228 2d2d 7269 6f2d  round:var(--rio-
+0005d180: 676c 6f62 616c 2d62 6163 6b67 726f 756e  global-backgroun
+0005d190: 642d 6267 293b 6f76 6572 666c 6f77 3a68  d-bg);overflow:h
+0005d1a0: 6964 6465 6e7d 626f 6479 7b6d 6172 6769  idden}body{margi
+0005d1b0: 6e3a 303b 7061 6464 696e 673a 303b 666f  n:0;padding:0;fo
+0005d1c0: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
+0005d1d0: 7269 6f2d 676c 6f62 616c 2d66 6f6e 742c  rio-global-font,
+0005d1e0: 2073 616e 732d 7365 7269 6629 7d69 6e70   sans-serif)}inp
+0005d1f0: 7574 2c74 6578 7461 7265 612c 7365 6c65  ut,textarea,sele
+0005d200: 6374 7b66 6f6e 742d 6661 6d69 6c79 3a69  ct{font-family:i
+0005d210: 6e68 6572 6974 3b66 6f6e 742d 7369 7a65  nherit;font-size
+0005d220: 3a31 7265 6d7d 2e72 696f 2d63 6f6d 706f  :1rem}.rio-compo
+0005d230: 6e65 6e74 7b70 6f73 6974 696f 6e3a 6162  nent{position:ab
+0005d240: 736f 6c75 7465 7d2e 7269 6f2d 6675 6e64  solute}.rio-fund
+0005d250: 616d 656e 7461 6c2d 726f 6f74 2d63 6f6d  amental-root-com
+0005d260: 706f 6e65 6e74 7b70 6f73 6974 696f 6e3a  ponent{position:
+0005d270: 7265 6c61 7469 7665 2169 6d70 6f72 7461  relative!importa
+0005d280: 6e74 3b77 6964 7468 3a31 3030 7677 3b68  nt;width:100vw;h
+0005d290: 6569 6768 743a 3130 3076 687d 2e72 696f  eight:100vh}.rio
+0005d2a0: 2d6c 696e 6561 722d 6368 696c 642d 636f  -linear-child-co
+0005d2b0: 6e74 6169 6e65 727b 706f 696e 7465 722d  ntainer{pointer-
+0005d2c0: 6576 656e 7473 3a6e 6f6e 653b 6469 7370  events:none;disp
+0005d2d0: 6c61 793a 666c 6578 3b61 6c69 676e 2d69  lay:flex;align-i
+0005d2e0: 7465 6d73 3a73 7472 6574 6368 7d2e 7269  tems:stretch}.ri
+0005d2f0: 6f2d 6c69 6e65 6172 2d63 6869 6c64 2d63  o-linear-child-c
+0005d300: 6f6e 7461 696e 6572 3e2a 7b70 6f73 6974  ontainer>*{posit
+0005d310: 696f 6e3a 7265 6c61 7469 7665 2169 6d70  ion:relative!imp
+0005d320: 6f72 7461 6e74 7d2e 7269 6f2d 6c69 7374  ortant}.rio-list
+0005d330: 2d76 6965 773e 6469 763e 2a3a 6669 7273  -view>div>*:firs
+0005d340: 742d 6368 696c 647b 706f 7369 7469 6f6e  t-child{position
+0005d350: 3a72 656c 6174 6976 6521 696d 706f 7274  :relative!import
+0005d360: 616e 747d 2e72 696f 2d63 6f6c 756d 6e7b  ant}.rio-column{
+0005d370: 666c 6578 2d64 6972 6563 7469 6f6e 3a63  flex-direction:c
+0005d380: 6f6c 756d 6e7d 2e72 696f 2d67 7269 647b  olumn}.rio-grid{
+0005d390: 706f 696e 7465 722d 6576 656e 7473 3a6e  pointer-events:n
+0005d3a0: 6f6e 653b 6469 7370 6c61 793a 6772 6964  one;display:grid
+0005d3b0: 7d2e 7269 6f2d 7465 7874 7b70 6f69 6e74  }.rio-text{point
+0005d3c0: 6572 2d65 7665 6e74 733a 6175 746f 3b64  er-events:auto;d
+0005d3d0: 6973 706c 6179 3a66 6c65 783b 616c 6967  isplay:flex;alig
+0005d3e0: 6e2d 6974 656d 733a 6365 6e74 6572 3b63  n-items:center;c
+0005d3f0: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
+0005d400: 6f63 616c 2d74 6578 742d 636f 6c6f 7229  ocal-text-color)
+0005d410: 7d2e 7269 6f2d 7465 7874 3e64 6976 7b66  }.rio-text>div{f
+0005d420: 6c65 782d 6772 6f77 3a31 3b6f 7665 7266  lex-grow:1;overf
+0005d430: 6c6f 773a 6869 6464 656e 7d2e 7269 6f2d  low:hidden}.rio-
+0005d440: 7265 6374 616e 676c 657b 706f 696e 7465  rectangle{pointe
+0005d450: 722d 6576 656e 7473 3a61 7574 6f3b 626f  r-events:auto;bo
+0005d460: 7264 6572 2d73 7479 6c65 3a73 6f6c 6964  rder-style:solid
+0005d470: 3b74 7261 6e73 6974 696f 6e2d 7072 6f70  ;transition-prop
+0005d480: 6572 7479 3a62 6163 6b67 726f 756e 642c  erty:background,
+0005d490: 7374 726f 6b65 2d63 6f6c 6f72 2c73 7472  stroke-color,str
+0005d4a0: 6f6b 652d 7769 6474 682c 626f 7264 6572  oke-width,border
+0005d4b0: 2d72 6164 6975 732c 7368 6164 6f77 2d63  -radius,shadow-c
+0005d4c0: 6f6c 6f72 2c73 6861 646f 772d 7261 6469  olor,shadow-radi
+0005d4d0: 7573 2c73 6861 646f 772d 6f66 6673 6574  us,shadow-offset
+0005d4e0: 3b74 7261 6e73 6974 696f 6e2d 7469 6d69  ;transition-timi
+0005d4f0: 6e67 2d66 756e 6374 696f 6e3a 6561 7365  ng-function:ease
+0005d500: 3b62 6163 6b67 726f 756e 643a 7661 7228  ;background:var(
+0005d510: 2d2d 7269 6f2d 7265 6374 616e 676c 652d  --rio-rectangle-
+0005d520: 6669 6c6c 293b 626f 7264 6572 2d63 6f6c  fill);border-col
+0005d530: 6f72 3a76 6172 282d 2d72 696f 2d72 6563  or:var(--rio-rec
+0005d540: 7461 6e67 6c65 2d73 7472 6f6b 655f 636f  tangle-stroke_co
+0005d550: 6c6f 7229 3b62 6f72 6465 722d 7769 6474  lor);border-widt
+0005d560: 683a 7661 7228 2d2d 7269 6f2d 7265 6374  h:var(--rio-rect
+0005d570: 616e 676c 652d 7374 726f 6b65 5f77 6964  angle-stroke_wid
+0005d580: 7468 293b 626f 7264 6572 2d72 6164 6975  th);border-radiu
+0005d590: 733a 7661 7228 2d2d 7269 6f2d 7265 6374  s:var(--rio-rect
+0005d5a0: 616e 676c 652d 636f 726e 6572 5f72 6164  angle-corner_rad
+0005d5b0: 6975 7329 3b62 6f78 2d73 6861 646f 773a  ius);box-shadow:
+0005d5c0: 7661 7228 2d2d 7269 6f2d 7265 6374 616e  var(--rio-rectan
+0005d5d0: 676c 652d 7368 6164 6f77 5f6f 6666 7365  gle-shadow_offse
+0005d5e0: 745f 7829 2076 6172 282d 2d72 696f 2d72  t_x) var(--rio-r
+0005d5f0: 6563 7461 6e67 6c65 2d73 6861 646f 775f  ectangle-shadow_
+0005d600: 6f66 6673 6574 5f79 2920 7661 7228 2d2d  offset_y) var(--
+0005d610: 7269 6f2d 7265 6374 616e 676c 652d 7368  rio-rectangle-sh
+0005d620: 6164 6f77 5f72 6164 6975 7329 2076 6172  adow_radius) var
+0005d630: 282d 2d72 696f 2d72 6563 7461 6e67 6c65  (--rio-rectangle
+0005d640: 2d73 6861 646f 775f 636f 6c6f 7229 7d2e  -shadow_color)}.
+0005d650: 7269 6f2d 7265 6374 616e 676c 653a 686f  rio-rectangle:ho
+0005d660: 7665 727b 6261 636b 6772 6f75 6e64 3a76  ver{background:v
+0005d670: 6172 282d 2d72 696f 2d72 6563 7461 6e67  ar(--rio-rectang
+0005d680: 6c65 2d68 6f76 6572 2d66 696c 6c29 3b62  le-hover-fill);b
+0005d690: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+0005d6a0: 2d2d 7269 6f2d 7265 6374 616e 676c 652d  --rio-rectangle-
+0005d6b0: 686f 7665 722d 7374 726f 6b65 5f63 6f6c  hover-stroke_col
+0005d6c0: 6f72 293b 626f 7264 6572 2d77 6964 7468  or);border-width
+0005d6d0: 3a76 6172 282d 2d72 696f 2d72 6563 7461  :var(--rio-recta
+0005d6e0: 6e67 6c65 2d68 6f76 6572 2d73 7472 6f6b  ngle-hover-strok
+0005d6f0: 655f 7769 6474 6829 3b62 6f72 6465 722d  e_width);border-
+0005d700: 7261 6469 7573 3a76 6172 282d 2d72 696f  radius:var(--rio
+0005d710: 2d72 6563 7461 6e67 6c65 2d68 6f76 6572  -rectangle-hover
+0005d720: 2d63 6f72 6e65 725f 7261 6469 7573 293b  -corner_radius);
+0005d730: 626f 782d 7368 6164 6f77 3a76 6172 282d  box-shadow:var(-
+0005d740: 2d72 696f 2d72 6563 7461 6e67 6c65 2d68  -rio-rectangle-h
+0005d750: 6f76 6572 2d73 6861 646f 775f 6f66 6673  over-shadow_offs
+0005d760: 6574 5f78 2920 7661 7228 2d2d 7269 6f2d  et_x) var(--rio-
+0005d770: 7265 6374 616e 676c 652d 686f 7665 722d  rectangle-hover-
+0005d780: 7368 6164 6f77 5f6f 6666 7365 745f 7929  shadow_offset_y)
+0005d790: 2076 6172 282d 2d72 696f 2d72 6563 7461   var(--rio-recta
+0005d7a0: 6e67 6c65 2d68 6f76 6572 2d73 6861 646f  ngle-hover-shado
+0005d7b0: 775f 7261 6469 7573 2920 7661 7228 2d2d  w_radius) var(--
+0005d7c0: 7269 6f2d 7265 6374 616e 676c 652d 686f  rio-rectangle-ho
+0005d7d0: 7665 722d 7368 6164 6f77 5f63 6f6c 6f72  ver-shadow_color
+0005d7e0: 297d 2e72 696f 2d72 6563 7461 6e67 6c65  )}.rio-rectangle
+0005d7f0: 2d72 6970 706c 657b 6f76 6572 666c 6f77  -ripple{overflow
+0005d800: 3a68 6964 6465 6e7d 2e72 696f 2d74 6578  :hidden}.rio-tex
+0005d810: 742d 696e 7075 747b 6375 7273 6f72 3a74  t-input{cursor:t
+0005d820: 6578 747d 2e72 696f 2d74 6578 742d 696e  ext}.rio-text-in
+0005d830: 7075 742d 6869 6e74 2d74 6578 747b 6469  put-hint-text{di
+0005d840: 7370 6c61 793a 666c 6578 3b61 6c69 676e  splay:flex;align
+0005d850: 2d69 7465 6d73 3a65 6e64 3b2d 7765 626b  -items:end;-webk
+0005d860: 6974 2d75 7365 722d 7365 6c65 6374 3a6e  it-user-select:n
+0005d870: 6f6e 653b 7573 6572 2d73 656c 6563 743a  one;user-select:
+0005d880: 6e6f 6e65 3b70 6164 6469 6e67 2d62 6f74  none;padding-bot
+0005d890: 746f 6d3a 2e36 7265 6d3b 636f 6c6f 723a  tom:.6rem;color:
+0005d8a0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+0005d8b0: 7465 7874 2d63 6f6c 6f72 293b 6f70 6163  text-color);opac
+0005d8c0: 6974 793a 303b 7472 616e 7369 7469 6f6e  ity:0;transition
+0005d8d0: 3a61 6c6c 202e 3133 7320 6c69 6e65 6172  :all .13s linear
+0005d8e0: 7d2e 7269 6f2d 7465 7874 2d69 6e70 7574  }.rio-text-input
+0005d8f0: 2d70 7265 6669 782d 7465 7874 7b70 6164  -prefix-text{pad
+0005d900: 6469 6e67 2d6c 6566 743a 2e38 7265 6d3b  ding-left:.8rem;
+0005d910: 6d61 7267 696e 2d72 6967 6874 3a2e 3272  margin-right:.2r
+0005d920: 656d 7d2e 7269 6f2d 7465 7874 2d69 6e70  em}.rio-text-inp
+0005d930: 7574 2d73 7566 6669 782d 7465 7874 7b70  ut-suffix-text{p
+0005d940: 6164 6469 6e67 2d72 6967 6874 3a2e 3872  adding-right:.8r
+0005d950: 656d 3b6d 6172 6769 6e2d 6c65 6674 3a2e  em;margin-left:.
+0005d960: 3272 656d 7d69 6e70 7574 3a6e 6f74 283a  2rem}input:not(:
+0005d970: 706c 6163 6568 6f6c 6465 722d 7368 6f77  placeholder-show
+0005d980: 6e29 7e2e 7269 6f2d 7465 7874 2d69 6e70  n)~.rio-text-inp
+0005d990: 7574 2d68 696e 742d 7465 7874 2c2e 7269  ut-hint-text,.ri
+0005d9a0: 6f2d 696e 7075 742d 626f 783a 666f 6375  o-input-box:focu
+0005d9b0: 732d 7769 7468 696e 3e2e 7269 6f2d 7465  s-within>.rio-te
+0005d9c0: 7874 2d69 6e70 7574 2d68 696e 742d 7465  xt-input-hint-te
+0005d9d0: 7874 2c2e 7269 6f2d 696e 7075 742d 626f  xt,.rio-input-bo
+0005d9e0: 782d 666f 6375 7365 643e 2e72 696f 2d74  x-focused>.rio-t
+0005d9f0: 6578 742d 696e 7075 742d 6869 6e74 2d74  ext-input-hint-t
+0005da00: 6578 747b 6f70 6163 6974 793a 2e35 7d2e  ext{opacity:.5}.
+0005da10: 7269 6f2d 7465 7874 2d69 6e70 7574 2e72  rio-text-input.r
+0005da20: 696f 2d69 6e70 7574 2d62 6f78 7b70 6164  io-input-box{pad
+0005da30: 6469 6e67 2d6c 6566 743a 3021 696d 706f  ding-left:0!impo
+0005da40: 7274 616e 743b 7061 6464 696e 672d 7269  rtant;padding-ri
+0005da50: 6768 743a 3021 696d 706f 7274 616e 747d  ght:0!important}
+0005da60: 2e72 696f 2d69 6e70 7574 2d62 6f78 7b70  .rio-input-box{p
+0005da70: 6f69 6e74 6572 2d65 7665 6e74 733a 6175  ointer-events:au
+0005da80: 746f 3b64 6973 706c 6179 3a66 6c65 783b  to;display:flex;
+0005da90: 666c 6578 2d64 6972 6563 7469 6f6e 3a72  flex-direction:r
+0005daa0: 6f77 3b61 6c69 676e 2d69 7465 6d73 3a73  ow;align-items:s
+0005dab0: 7472 6574 6368 3b70 6164 6469 6e67 2d6c  tretch;padding-l
+0005dac0: 6566 743a 2e38 7265 6d3b 7061 6464 696e  eft:.8rem;paddin
+0005dad0: 672d 7269 6768 743a 2e38 7265 6d3b 626f  g-right:.8rem;bo
+0005dae0: 782d 7369 7a69 6e67 3a62 6f72 6465 722d  x-sizing:border-
+0005daf0: 626f 783b 6261 636b 6772 6f75 6e64 2d63  box;background-c
+0005db00: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
+0005db10: 6f63 616c 2d62 672d 7661 7269 616e 7429  ocal-bg-variant)
+0005db20: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
+0005db30: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+0005db40: 636f 726e 6572 2d72 6164 6975 732d 736d  corner-radius-sm
+0005db50: 616c 6c29 2076 6172 282d 2d72 696f 2d67  all) var(--rio-g
+0005db60: 6c6f 6261 6c2d 636f 726e 6572 2d72 6164  lobal-corner-rad
+0005db70: 6975 732d 736d 616c 6c29 2030 2030 7d2e  ius-small) 0 0}.
+0005db80: 7269 6f2d 696e 7075 742d 626f 783a 6e6f  rio-input-box:no
+0005db90: 7428 2e72 696f 2d64 6973 6162 6c65 642d  t(.rio-disabled-
+0005dba0: 696e 7075 7429 7b6f 7665 7266 6c6f 773a  input){overflow:
+0005dbb0: 6869 6464 656e 7d2e 7269 6f2d 696e 7075  hidden}.rio-inpu
+0005dbc0: 742d 626f 783a 666f 6375 732d 7769 7468  t-box:focus-with
+0005dbd0: 696e 2c2e 7269 6f2d 696e 7075 742d 626f  in,.rio-input-bo
+0005dbe0: 782e 7269 6f2d 696e 7075 742d 626f 782d  x.rio-input-box-
+0005dbf0: 666f 6375 7365 647b 6f75 746c 696e 653a  focused{outline:
+0005dc00: 6e6f 6e65 3b62 6163 6b67 726f 756e 642d  none;background-
+0005dc10: 636f 6c6f 723a 7661 7228 2d2d 7269 6f2d  color:var(--rio-
+0005dc20: 6c6f 6361 6c2d 6267 2d61 6374 6976 6529  local-bg-active)
+0005dc30: 7d2e 7269 6f2d 696e 7075 742d 626f 783e  }.rio-input-box>
+0005dc40: 696e 7075 742c 2e72 696f 2d69 6e70 7574  input,.rio-input
+0005dc50: 2d62 6f78 3e74 6578 7461 7265 617b 666c  -box>textarea{fl
+0005dc60: 6578 2d67 726f 773a 313b 6d69 6e2d 7769  ex-grow:1;min-wi
+0005dc70: 6474 683a 303b 6261 636b 6772 6f75 6e64  dth:0;background
+0005dc80: 2d63 6f6c 6f72 3a74 7261 6e73 7061 7265  -color:transpare
+0005dc90: 6e74 3b63 6f6c 6f72 3a76 6172 282d 2d72  nt;color:var(--r
+0005dca0: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
+0005dcb0: 6c6f 7229 3b63 6172 6574 2d63 6f6c 6f72  lor);caret-color
+0005dcc0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
+0005dcd0: 2d6c 6576 656c 2d32 2d62 6729 3b62 6f72  -level-2-bg);bor
+0005dce0: 6465 723a 6e6f 6e65 7d2e 7269 6f2d 696e  der:none}.rio-in
+0005dcf0: 7075 742d 626f 783e 696e 7075 747b 6865  put-box>input{he
+0005dd00: 6967 6874 3a63 616c 6328 3230 3025 202d  ight:calc(200% -
+0005dd10: 2032 2e33 3872 656d 297d 2e72 696f 2d69   2.38rem)}.rio-i
+0005dd20: 6e70 7574 2d62 6f78 3e74 6578 7461 7265  nput-box>textare
+0005dd30: 617b 6d61 7267 696e 2d74 6f70 3a31 2e35  a{margin-top:1.5
+0005dd40: 7265 6d3b 7769 6474 683a 3130 3025 3b72  rem;width:100%;r
+0005dd50: 6573 697a 653a 6e6f 6e65 3b70 6164 6469  esize:none;paddi
+0005dd60: 6e67 3a30 202e 3872 656d 7d2e 7269 6f2d  ng:0 .8rem}.rio-
+0005dd70: 696e 7075 742d 626f 783e 696e 7075 743a  input-box>input:
+0005dd80: 6163 7469 7665 2c2e 7269 6f2d 696e 7075  active,.rio-inpu
+0005dd90: 742d 626f 783e 7465 7874 6172 6561 3a61  t-box>textarea:a
+0005dda0: 6374 6976 657b 6261 636b 6772 6f75 6e64  ctive{background
+0005ddb0: 2d63 6f6c 6f72 3a74 7261 6e73 7061 7265  -color:transpare
+0005ddc0: 6e74 7d2e 7269 6f2d 696e 7075 742d 626f  nt}.rio-input-bo
+0005ddd0: 783e 696e 7075 743a 666f 6375 732d 7669  x>input:focus-vi
+0005dde0: 7369 626c 652c 2e72 696f 2d69 6e70 7574  sible,.rio-input
+0005ddf0: 2d62 6f78 3e74 6578 7461 7265 613a 666f  -box>textarea:fo
+0005de00: 6375 732d 7669 7369 626c 657b 6f75 746c  cus-visible{outl
+0005de10: 696e 653a 6e6f 6e65 7d2e 7269 6f2d 696e  ine:none}.rio-in
+0005de20: 7075 742d 626f 782d 6c61 6265 6c7b 706f  put-box-label{po
+0005de30: 696e 7465 722d 6576 656e 7473 3a6e 6f6e  inter-events:non
+0005de40: 653b 706f 7369 7469 6f6e 3a61 6273 6f6c  e;position:absol
+0005de50: 7574 653b 6c65 6674 3a2e 3872 656d 3b74  ute;left:.8rem;t
+0005de60: 6f70 3a63 616c 6328 3530 2520 2d20 2e35  op:calc(50% - .5
+0005de70: 7265 6d29 3b66 6f6e 742d 7369 7a65 3a31  rem);font-size:1
+0005de80: 7265 6d3b 636f 6c6f 723a 7661 7228 2d2d  rem;color:var(--
+0005de90: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d63  rio-local-text-c
+0005dea0: 6f6c 6f72 293b 6f70 6163 6974 793a 2e35  olor);opacity:.5
+0005deb0: 3b74 7261 6e73 6974 696f 6e3a 616c 6c20  ;transition:all 
+0005dec0: 2e31 3373 206c 696e 6561 727d 696e 7075  .13s linear}inpu
+0005ded0: 743a 6e6f 7428 3a70 6c61 6365 686f 6c64  t:not(:placehold
+0005dee0: 6572 2d73 686f 776e 297e 2e72 696f 2d69  er-shown)~.rio-i
+0005def0: 6e70 7574 2d62 6f78 2d6c 6162 656c 2c74  nput-box-label,t
+0005df00: 6578 7461 7265 613a 6e6f 7428 3a70 6c61  extarea:not(:pla
+0005df10: 6365 686f 6c64 6572 2d73 686f 776e 297e  ceholder-shown)~
+0005df20: 2e72 696f 2d69 6e70 7574 2d62 6f78 2d6c  .rio-input-box-l
+0005df30: 6162 656c 2c2e 7269 6f2d 696e 7075 742d  abel,.rio-input-
+0005df40: 626f 783a 666f 6375 732d 7769 7468 696e  box:focus-within
+0005df50: 3e2e 7269 6f2d 696e 7075 742d 626f 782d  >.rio-input-box-
+0005df60: 6c61 6265 6c2c 2e72 696f 2d69 6e70 7574  label,.rio-input
+0005df70: 2d62 6f78 2d66 6f63 7573 6564 3e2e 7269  -box-focused>.ri
+0005df80: 6f2d 696e 7075 742d 626f 782d 6c61 6265  o-input-box-labe
+0005df90: 6c7b 6f70 6163 6974 793a 313b 746f 703a  l{opacity:1;top:
+0005dfa0: 2e34 7265 6d3b 626f 7474 6f6d 3a75 6e73  .4rem;bottom:uns
+0005dfb0: 6574 3b66 6f6e 742d 7369 7a65 3a2e 3872  et;font-size:.8r
+0005dfc0: 656d 7d2e 7269 6f2d 696e 7075 742d 626f  em}.rio-input-bo
+0005dfd0: 783a 666f 6375 732d 7769 7468 696e 3e2e  x:focus-within>.
+0005dfe0: 7269 6f2d 696e 7075 742d 626f 782d 6c61  rio-input-box-la
+0005dff0: 6265 6c2c 2e72 696f 2d69 6e70 7574 2d62  bel,.rio-input-b
+0005e000: 6f78 2d66 6f63 7573 6564 3e2e 7269 6f2d  ox-focused>.rio-
+0005e010: 696e 7075 742d 626f 782d 6c61 6265 6c7b  input-box-label{
+0005e020: 636f 6c6f 723a 7661 7228 2d2d 7269 6f2d  color:var(--rio-
+0005e030: 6c6f 6361 6c2d 6c65 7665 6c2d 322d 6267  local-level-2-bg
+0005e040: 297d 2e72 696f 2d69 6e70 7574 2d62 6f78  )}.rio-input-box
+0005e050: 2d70 6c61 696e 2d62 6172 2c2e 7269 6f2d  -plain-bar,.rio-
+0005e060: 696e 7075 742d 626f 782d 636f 6c6f 722d  input-box-color-
+0005e070: 6261 727b 706f 7369 7469 6f6e 3a61 6273  bar{position:abs
+0005e080: 6f6c 7574 653b 626f 7474 6f6d 3a30 3b68  olute;bottom:0;h
+0005e090: 6569 6768 743a 2e31 3272 656d 7d2e 7269  eight:.12rem}.ri
+0005e0a0: 6f2d 696e 7075 742d 626f 782d 706c 6169  o-input-box-plai
+0005e0b0: 6e2d 6261 727b 6261 636b 6772 6f75 6e64  n-bar{background
+0005e0c0: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
+0005e0d0: 2d6c 6f63 616c 2d74 6578 742d 636f 6c6f  -local-text-colo
+0005e0e0: 7229 3b6c 6566 743a 303b 7269 6768 743a  r);left:0;right:
+0005e0f0: 303b 6f70 6163 6974 793a 2e31 357d 2e72  0;opacity:.15}.r
+0005e100: 696f 2d69 6e70 7574 2d62 6f78 2d63 6f6c  io-input-box-col
+0005e110: 6f72 2d62 6172 7b62 6163 6b67 726f 756e  or-bar{backgroun
+0005e120: 642d 636f 6c6f 723a 7661 7228 2d2d 7269  d-color:var(--ri
+0005e130: 6f2d 6c6f 6361 6c2d 6c65 7665 6c2d 322d  o-local-level-2-
+0005e140: 6267 293b 6c65 6674 3a34 3025 3b72 6967  bg);left:40%;rig
+0005e150: 6874 3a34 3025 3b6f 7061 6369 7479 3a30  ht:40%;opacity:0
+0005e160: 3b74 7261 6e73 6974 696f 6e3a 616c 6c20  ;transition:all 
+0005e170: 2e32 7320 6561 7365 2d69 6e2d 6f75 747d  .2s ease-in-out}
+0005e180: 2e72 696f 2d69 6e70 7574 2d62 6f78 3a66  .rio-input-box:f
+0005e190: 6f63 7573 2d77 6974 6869 6e20 2e72 696f  ocus-within .rio
+0005e1a0: 2d69 6e70 7574 2d62 6f78 2d63 6f6c 6f72  -input-box-color
+0005e1b0: 2d62 6172 2c2e 7269 6f2d 696e 7075 742d  -bar,.rio-input-
+0005e1c0: 626f 782d 666f 6375 7365 6420 2e72 696f  box-focused .rio
+0005e1d0: 2d69 6e70 7574 2d62 6f78 2d63 6f6c 6f72  -input-box-color
+0005e1e0: 2d62 6172 7b6c 6566 743a 303b 7269 6768  -bar{left:0;righ
+0005e1f0: 743a 303b 6f70 6163 6974 793a 317d 2e72  t:0;opacity:1}.r
+0005e200: 696f 2d73 7461 636b 7b70 6f69 6e74 6572  io-stack{pointer
+0005e210: 2d65 7665 6e74 733a 6e6f 6e65 3b64 6973  -events:none;dis
+0005e220: 706c 6179 3a69 6e6c 696e 652d 6772 6964  play:inline-grid
+0005e230: 7d2e 7269 6f2d 7374 6163 6b3e 2a7b 6772  }.rio-stack>*{gr
+0005e240: 6964 2d63 6f6c 756d 6e2d 7374 6172 743a  id-column-start:
+0005e250: 313b 6772 6964 2d72 6f77 2d73 7461 7274  1;grid-row-start
+0005e260: 3a31 7d2e 7269 6f2d 7377 6974 6368 7b64  :1}.rio-switch{d
+0005e270: 6973 706c 6179 3a66 6c65 787d 2e72 696f  isplay:flex}.rio
+0005e280: 2d73 7769 7463 683e 2a7b 706f 696e 7465  -switch>*{pointe
+0005e290: 722d 6576 656e 7473 3a61 7574 6f3b 706f  r-events:auto;po
+0005e2a0: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
+0005e2b0: 7769 6474 683a 332e 3138 7265 6d3b 6865  width:3.18rem;he
+0005e2c0: 6967 6874 3a31 2e35 3472 656d 3b6d 6172  ight:1.54rem;mar
+0005e2d0: 6769 6e3a 6175 746f 3b62 6f72 6465 722d  gin:auto;border-
+0005e2e0: 7261 6469 7573 3a34 2e33 7265 6d3b 6261  radius:4.3rem;ba
+0005e2f0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+0005e300: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+0005e310: 6469 7361 626c 6564 2d62 672d 7661 7269  disabled-bg-vari
+0005e320: 616e 7429 3b74 7261 6e73 6974 696f 6e3a  ant);transition:
+0005e330: 2e33 7320 6561 7365 2061 6c6c 3b7a 2d69  .3s ease all;z-i
+0005e340: 6e64 6578 3a31 7d2e 7269 6f2d 7377 6974  ndex:1}.rio-swit
+0005e350: 6368 2e69 732d 6f6e 3e2a 7b62 6163 6b67  ch.is-on>*{backg
+0005e360: 726f 756e 642d 636f 6c6f 723a 7661 7228  round-color:var(
+0005e370: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+0005e380: 6c2d 322d 6267 297d 2e72 696f 2d73 7769  l-2-bg)}.rio-swi
+0005e390: 7463 6820 696e 7075 747b 706f 7369 7469  tch input{positi
+0005e3a0: 6f6e 3a72 656c 6174 6976 653b 7769 6474  on:relative;widt
+0005e3b0: 683a 3130 3025 3b68 6569 6768 743a 3130  h:100%;height:10
+0005e3c0: 3025 3b70 6164 6469 6e67 3a30 3b6d 6172  0%;padding:0;mar
+0005e3d0: 6769 6e3a 303b 6f70 6163 6974 793a 303b  gin:0;opacity:0;
+0005e3e0: 6375 7273 6f72 3a70 6f69 6e74 6572 3b7a  cursor:pointer;z
+0005e3f0: 2d69 6e64 6578 3a33 7d2e 7269 6f2d 7377  -index:3}.rio-sw
+0005e400: 6974 6368 202e 6b6e 6f62 7b7a 2d69 6e64  itch .knob{z-ind
+0005e410: 6578 3a32 3b70 6f73 6974 696f 6e3a 6162  ex:2;position:ab
+0005e420: 736f 6c75 7465 3b74 6f70 3a2e 3137 7265  solute;top:.17re
+0005e430: 6d3b 6c65 6674 3a2e 3137 7265 6d3b 7769  m;left:.17rem;wi
+0005e440: 6474 683a 2e38 3672 656d 3b68 6569 6768  dth:.86rem;heigh
+0005e450: 743a 2e34 3372 656d 3b70 6164 6469 6e67  t:.43rem;padding
+0005e460: 3a2e 3339 7265 6d20 2e31 3772 656d 3b62  :.39rem .17rem;b
+0005e470: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+0005e480: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+0005e490: 2d64 6973 6162 6c65 642d 6267 293b 626f  -disabled-bg);bo
+0005e4a0: 7264 6572 2d72 6164 6975 733a 3530 253b  rder-radius:50%;
+0005e4b0: 7472 616e 7369 7469 6f6e 3a2e 3373 2065  transition:.3s e
+0005e4c0: 6173 6520 616c 6c2c 6c65 6674 202e 3373  ase all,left .3s
+0005e4d0: 2063 7562 6963 2d62 657a 6965 7228 2e31   cubic-bezier(.1
+0005e4e0: 382c 2e38 392c 2e33 352c 312e 3135 297d  8,.89,.35,1.15)}
+0005e4f0: 2e72 696f 2d73 7769 7463 6820 696e 7075  .rio-switch inpu
+0005e500: 743a 6163 7469 7665 2b2e 6b6e 6f62 7b77  t:active+.knob{w
+0005e510: 6964 7468 3a31 2e39 3872 656d 3b62 6f72  idth:1.98rem;bor
+0005e520: 6465 722d 7261 6469 7573 3a34 2e33 7265  der-radius:4.3re
+0005e530: 6d7d 2e72 696f 2d73 7769 7463 682e 6973  m}.rio-switch.is
+0005e540: 2d6f 6e20 696e 7075 743a 6163 7469 7665  -on input:active
+0005e550: 2b2e 6b6e 6f62 7b6d 6172 6769 6e2d 6c65  +.knob{margin-le
+0005e560: 6674 3a2d 312e 3132 7265 6d7d 2e72 696f  ft:-1.12rem}.rio
+0005e570: 2d73 7769 7463 682e 6973 2d6f 6e20 696e  -switch.is-on in
+0005e580: 7075 742b 2e6b 6e6f 627b 6c65 6674 3a31  put+.knob{left:1
+0005e590: 2e38 7265 6d3b 6261 636b 6772 6f75 6e64  .8rem;background
+0005e5a0: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
+0005e5b0: 2d6c 6f63 616c 2d62 6729 7d2e 7269 6f2d  -local-bg)}.rio-
+0005e5c0: 6472 6f70 646f 776e 7b70 6f69 6e74 6572  dropdown{pointer
+0005e5d0: 2d65 7665 6e74 733a 6175 746f 7d2e 7269  -events:auto}.ri
+0005e5e0: 6f2d 6472 6f70 646f 776e 2c2e 7269 6f2d  o-dropdown,.rio-
+0005e5f0: 6472 6f70 646f 776e 3e69 6e70 7574 7b63  dropdown>input{c
+0005e600: 7572 736f 723a 706f 696e 7465 727d 2e72  ursor:pointer}.r
+0005e610: 696f 2d64 726f 7064 6f77 6e2d 706f 7075  io-dropdown-popu
+0005e620: 707b 706f 7369 7469 6f6e 3a61 6273 6f6c  p{position:absol
+0005e630: 7574 653b 7a2d 696e 6465 783a 3130 3030  ute;z-index:1000
+0005e640: 333b 6865 6967 6874 3a30 3b6d 6178 2d68  3;height:0;max-h
+0005e650: 6569 6768 743a 3130 3076 683b 6261 636b  eight:100vh;back
+0005e660: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+0005e670: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6261  (--rio-global-ba
+0005e680: 636b 6772 6f75 6e64 2d62 6729 3b63 6f6c  ckground-bg);col
+0005e690: 6f72 3a76 6172 282d 2d72 696f 2d67 6c6f  or:var(--rio-glo
+0005e6a0: 6261 6c2d 7465 7874 2d63 6f6c 6f72 293b  bal-text-color);
+0005e6b0: 626f 7264 6572 2d72 6164 6975 733a 3020  border-radius:0 
+0005e6c0: 3020 7661 7228 2d2d 7269 6f2d 676c 6f62  0 var(--rio-glob
+0005e6d0: 616c 2d63 6f72 6e65 722d 7261 6469 7573  al-corner-radius
+0005e6e0: 2d73 6d61 6c6c 2920 7661 7228 2d2d 7269  -small) var(--ri
+0005e6f0: 6f2d 676c 6f62 616c 2d63 6f72 6e65 722d  o-global-corner-
+0005e700: 7261 6469 7573 2d73 6d61 6c6c 293b 626f  radius-small);bo
+0005e710: 782d 7368 6164 6f77 3a30 2030 202e 3872  x-shadow:0 0 .8r
+0005e720: 656d 2076 6172 282d 2d72 696f 2d67 6c6f  em var(--rio-glo
+0005e730: 6261 6c2d 7368 6164 6f77 2d63 6f6c 6f72  bal-shadow-color
+0005e740: 293b 7472 616e 7369 7469 6f6e 3a68 6569  );transition:hei
+0005e750: 6768 7420 2e32 7320 6561 7365 2d69 6e2d  ght .2s ease-in-
+0005e760: 6f75 747d 2e72 696f 2d64 726f 7064 6f77  out}.rio-dropdow
+0005e770: 6e2d 706f 7075 702d 6162 6f76 657b 626f  n-popup-above{bo
+0005e780: 7264 6572 2d72 6164 6975 733a 7661 7228  rder-radius:var(
+0005e790: 2d2d 7269 6f2d 676c 6f62 616c 2d63 6f72  --rio-global-cor
+0005e7a0: 6e65 722d 7261 6469 7573 2d73 6d61 6c6c  ner-radius-small
+0005e7b0: 2921 696d 706f 7274 616e 747d 2e72 696f  )!important}.rio
+0005e7c0: 2d64 726f 7064 6f77 6e2e 7269 6f2d 696e  -dropdown.rio-in
+0005e7d0: 7075 742d 626f 783e 2e72 696f 2d64 726f  put-box>.rio-dro
+0005e7e0: 7064 6f77 6e2d 6172 726f 777b 706f 696e  pdown-arrow{poin
+0005e7f0: 7465 722d 6576 656e 7473 3a6e 6f6e 653b  ter-events:none;
+0005e800: 6f72 6465 723a 323b 6469 7370 6c61 793a  order:2;display:
+0005e810: 666c 6578 3b61 6c69 676e 2d69 7465 6d73  flex;align-items
+0005e820: 3a63 656e 7465 727d 2e72 696f 2d64 726f  :center}.rio-dro
+0005e830: 7064 6f77 6e2e 7269 6f2d 696e 7075 742d  pdown.rio-input-
+0005e840: 626f 783e 2e72 696f 2d64 726f 7064 6f77  box>.rio-dropdow
+0005e850: 6e2d 6172 726f 7720 7376 677b 7769 6474  n-arrow svg{widt
+0005e860: 683a 312e 3372 656d 3b68 6569 6768 743a  h:1.3rem;height:
+0005e870: 312e 3372 656d 7d2e 7269 6f2d 6472 6f70  1.3rem}.rio-drop
+0005e880: 646f 776e 2d6f 7074 696f 6e2d 6869 6768  down-option-high
+0005e890: 6c69 6768 747b 666f 6e74 2d77 6569 6768  light{font-weigh
+0005e8a0: 743a 3730 303b 636f 6c6f 723a 7661 7228  t:700;color:var(
+0005e8b0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
+0005e8c0: 6c2d 322d 6267 297d 2e72 696f 2d64 726f  l-2-bg)}.rio-dro
+0005e8d0: 7064 6f77 6e2d 6f70 7469 6f6e 737b 706f  pdown-options{po
+0005e8e0: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
+0005e8f0: 6469 7370 6c61 793a 666c 6578 3b66 6c65  display:flex;fle
+0005e900: 782d 6469 7265 6374 696f 6e3a 636f 6c75  x-direction:colu
+0005e910: 6d6e 3b61 6c69 676e 2d69 7465 6d73 3a73  mn;align-items:s
+0005e920: 7472 6574 6368 3b63 7572 736f 723a 706f  tretch;cursor:po
+0005e930: 696e 7465 727d 2e72 696f 2d64 726f 7064  inter}.rio-dropd
+0005e940: 6f77 6e2d 6f70 7469 6f6e 733e 6469 767b  own-options>div{
+0005e950: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+0005e960: 657d 2e72 696f 2d64 726f 7064 6f77 6e2d  e}.rio-dropdown-
+0005e970: 6f70 7469 6f6e 733e 7376 677b 706f 7369  options>svg{posi
+0005e980: 7469 6f6e 3a72 656c 6174 6976 653b 7769  tion:relative;wi
+0005e990: 6474 683a 3472 656d 3b68 6569 6768 743a  dth:4rem;height:
+0005e9a0: 3472 656d 3b6d 6172 6769 6e3a 312e 3572  4rem;margin:1.5r
+0005e9b0: 656d 2061 7574 6f3b 6f70 6163 6974 793a  em auto;opacity:
+0005e9c0: 2e32 7d2e 7269 6f2d 6472 6f70 646f 776e  .2}.rio-dropdown
+0005e9d0: 2d6f 7074 696f 6e3a 6166 7465 727b 636f  -option:after{co
+0005e9e0: 6e74 656e 743a 2222 3b70 6f69 6e74 6572  ntent:"";pointer
+0005e9f0: 2d65 7665 6e74 733a 6e6f 6e65 3b70 6f73  -events:none;pos
+0005ea00: 6974 696f 6e3a 6162 736f 6c75 7465 3b74  ition:absolute;t
+0005ea10: 6f70 3a30 3b6c 6566 743a 303b 7269 6768  op:0;left:0;righ
+0005ea20: 743a 303b 626f 7474 6f6d 3a30 3b62 6163  t:0;bottom:0;bac
+0005ea30: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
+0005ea40: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d70  r(--rio-global-p
+0005ea50: 7269 6d61 7279 2d62 6729 3b6f 7061 6369  rimary-bg);opaci
+0005ea60: 7479 3a30 3b74 7261 6e73 6974 696f 6e3a  ty:0;transition:
+0005ea70: 6f70 6163 6974 7920 2e31 7320 6561 7365  opacity .1s ease
+0005ea80: 2d69 6e2d 6f75 747d 2e72 696f 2d64 726f  -in-out}.rio-dro
+0005ea90: 7064 6f77 6e2d 6f70 7469 6f6e 2d68 6967  pdown-option-hig
+0005eaa0: 686c 6967 6874 6564 3a61 6674 6572 7b6f  hlighted:after{o
+0005eab0: 7061 6369 7479 3a2e 327d 2e72 696f 2d70  pacity:.2}.rio-p
+0005eac0: 726f 6772 6573 7362 6172 7b70 6f69 6e74  rogressbar{point
+0005ead0: 6572 2d65 7665 6e74 733a 6e6f 6e65 3b6f  er-events:none;o
+0005eae0: 7665 7266 6c6f 773a 6869 6464 656e 7d2e  verflow:hidden}.
+0005eaf0: 7269 6f2d 7072 6f67 7265 7373 6261 722d  rio-progressbar-
+0005eb00: 7472 6163 6b7b 706f 7369 7469 6f6e 3a61  track{position:a
+0005eb10: 6273 6f6c 7574 653b 7769 6474 683a 3130  bsolute;width:10
+0005eb20: 3025 3b68 6569 6768 743a 3130 3025 3b62  0%;height:100%;b
+0005eb30: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
+0005eb40: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d63  rio-local-text-c
+0005eb50: 6f6c 6f72 293b 6f70 6163 6974 793a 2e33  olor);opacity:.3
+0005eb60: 7d2e 7269 6f2d 7072 6f67 7265 7373 6261  }.rio-progressba
+0005eb70: 722d 6669 6c6c 7b70 6f73 6974 696f 6e3a  r-fill{position:
+0005eb80: 6162 736f 6c75 7465 3b68 6569 6768 743a  absolute;height:
+0005eb90: 3130 3025 3b62 6163 6b67 726f 756e 643a  100%;background:
+0005eba0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+0005ebb0: 6c65 7665 6c2d 322d 6267 297d 406b 6579  level-2-bg)}@key
+0005ebc0: 6672 616d 6573 2072 696f 2d70 726f 6772  frames rio-progr
+0005ebd0: 6573 7362 6172 2d61 6e69 6d61 7469 6f6e  essbar-animation
+0005ebe0: 2d69 6e64 6574 6572 6d69 6e61 7465 7b30  -indeterminate{0
+0005ebf0: 257b 6c65 6674 3a2d 3230 253b 7769 6474  %{left:-20%;widt
+0005ec00: 683a 3625 7d35 3025 7b77 6964 7468 3a33  h:6%}50%{width:3
+0005ec10: 3025 7d74 6f7b 6c65 6674 3a31 3230 253b  0%}to{left:120%;
+0005ec20: 7769 6474 683a 3625 7d7d 2e72 696f 2d70  width:6%}}.rio-p
+0005ec30: 726f 6772 6573 7362 6172 2d69 6e64 6574  rogressbar-indet
+0005ec40: 6572 6d69 6e61 7465 202e 7269 6f2d 7072  erminate .rio-pr
+0005ec50: 6f67 7265 7373 6261 722d 6669 6c6c 7b74  ogressbar-fill{t
+0005ec60: 7261 6e73 666f 726d 3a74 7261 6e73 6c61  ransform:transla
+0005ec70: 7465 282d 3530 2529 3b61 6e69 6d61 7469  te(-50%);animati
+0005ec80: 6f6e 3a72 696f 2d70 726f 6772 6573 7362  on:rio-progressb
+0005ec90: 6172 2d61 6e69 6d61 7469 6f6e 2d69 6e64  ar-animation-ind
+0005eca0: 6574 6572 6d69 6e61 7465 2031 2e35 7320  eterminate 1.5s 
+0005ecb0: 6561 7365 2d69 6e2d 6f75 7420 696e 6669  ease-in-out infi
+0005ecc0: 6e69 7465 7d2e 7269 6f2d 7072 6f67 7265  nite}.rio-progre
+0005ecd0: 7373 6261 723a 6e6f 7428 2e72 696f 2d70  ssbar:not(.rio-p
+0005ece0: 726f 6772 6573 7362 6172 2d69 6e64 6574  rogressbar-indet
+0005ecf0: 6572 6d69 6e61 7465 2920 2e72 696f 2d70  erminate) .rio-p
+0005ed00: 726f 6772 6573 7362 6172 2d66 696c 6c7b  rogressbar-fill{
+0005ed10: 6c65 6674 3a30 3b77 6964 7468 3a76 6172  left:0;width:var
+0005ed20: 282d 2d72 696f 2d70 726f 6772 6573 7362  (--rio-progressb
+0005ed30: 6172 2d66 7261 6374 696f 6e29 3b74 7261  ar-fraction);tra
+0005ed40: 6e73 6974 696f 6e3a 7769 6474 6820 2e33  nsition:width .3
+0005ed50: 7320 6561 7365 2d69 6e2d 6f75 747d 2e72  s ease-in-out}.r
+0005ed60: 696f 2d70 726f 6772 6573 732d 6369 7263  io-progress-circ
+0005ed70: 6c65 7b70 6f69 6e74 6572 2d65 7665 6e74  le{pointer-event
+0005ed80: 733a 6175 746f 3b73 7472 6f6b 653a 7661  s:auto;stroke:va
+0005ed90: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6267  r(--rio-local-bg
+0005eda0: 293b 6469 7370 6c61 793a 666c 6578 3b6a  );display:flex;j
+0005edb0: 7573 7469 6679 2d63 6f6e 7465 6e74 3a63  ustify-content:c
+0005edc0: 656e 7465 723b 6f76 6572 666c 6f77 3a68  enter;overflow:h
+0005edd0: 6964 6465 6e7d 2e72 696f 2d70 726f 6772  idden}.rio-progr
+0005ede0: 6573 732d 6369 7263 6c65 2063 6972 636c  ess-circle circl
+0005edf0: 657b 6669 6c6c 3a6e 6f6e 653b 7374 726f  e{fill:none;stro
+0005ee00: 6b65 2d77 6964 7468 3a33 2e35 3b63 6f6c  ke-width:3.5;col
+0005ee10: 6f72 3a76 6172 282d 2d72 696f 2d6c 6f63  or:var(--rio-loc
+0005ee20: 616c 2d6c 6576 656c 2d32 2d62 6729 7d2e  al-level-2-bg)}.
+0005ee30: 7370 696e 6e69 6e67 2073 7667 7b74 7261  spinning svg{tra
+0005ee40: 6e73 666f 726d 2d6f 7269 6769 6e3a 6365  nsform-origin:ce
+0005ee50: 6e74 6572 3b61 6e69 6d61 7469 6f6e 3a72  nter;animation:r
+0005ee60: 6f74 6174 6520 3273 206c 696e 6561 7220  otate 2s linear 
+0005ee70: 696e 6669 6e69 7465 7d2e 7370 696e 6e69  infinite}.spinni
+0005ee80: 6e67 202e 7072 6f67 7265 7373 7b73 7472  ng .progress{str
+0005ee90: 6f6b 652d 6461 7368 6172 7261 793a 312c  oke-dasharray:1,
+0005eea0: 3230 303b 7374 726f 6b65 2d64 6173 686f  200;stroke-dasho
+0005eeb0: 6666 7365 743a 303b 7374 726f 6b65 2d6c  ffset:0;stroke-l
+0005eec0: 696e 6563 6170 3a72 6f75 6e64 3b61 6e69  inecap:round;ani
+0005eed0: 6d61 7469 6f6e 3a64 6173 6820 312e 3573  mation:dash 1.5s
+0005eee0: 2065 6173 652d 696e 2d6f 7574 2069 6e66   ease-in-out inf
+0005eef0: 696e 6974 657d 2e72 696f 2d70 726f 6772  inite}.rio-progr
+0005ef00: 6573 732d 6369 7263 6c65 3a6e 6f74 282e  ess-circle:not(.
+0005ef10: 7370 696e 6e69 6e67 2920 2e70 726f 6772  spinning) .progr
+0005ef20: 6573 737b 7374 726f 6b65 2d64 6173 686f  ess{stroke-dasho
+0005ef30: 6666 7365 743a 2d39 342e 3235 3b73 7472  ffset:-94.25;str
+0005ef40: 6f6b 652d 6461 7368 6172 7261 793a 7661  oke-dasharray:va
+0005ef50: 7228 2d2d 6461 7368 6172 7261 7929 3b74  r(--dasharray);t
+0005ef60: 7261 6e73 6974 696f 6e3a 7374 726f 6b65  ransition:stroke
+0005ef70: 2d64 6173 6861 7272 6179 202e 3573 2065  -dasharray .5s e
+0005ef80: 6173 657d 406b 6579 6672 616d 6573 2072  ase}@keyframes r
+0005ef90: 6f74 6174 657b 746f 7b74 7261 6e73 666f  otate{to{transfo
+0005efa0: 726d 3a72 6f74 6174 6528 3336 3064 6567  rm:rotate(360deg
+0005efb0: 297d 7d40 6b65 7966 7261 6d65 7320 6461  )}}@keyframes da
+0005efc0: 7368 7b30 257b 7374 726f 6b65 2d64 6173  sh{0%{stroke-das
+0005efd0: 6861 7272 6179 3a31 2c32 3030 3b73 7472  harray:1,200;str
+0005efe0: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+0005eff0: 7d35 3025 7b73 7472 6f6b 652d 6461 7368  }50%{stroke-dash
+0005f000: 6172 7261 793a 3930 2c32 3030 3b73 7472  array:90,200;str
+0005f010: 6f6b 652d 6461 7368 6f66 6673 6574 3a2d  oke-dashoffset:-
+0005f020: 3335 7078 7d74 6f7b 7374 726f 6b65 2d64  35px}to{stroke-d
+0005f030: 6173 686f 6666 7365 743a 2d31 3235 7078  ashoffset:-125px
+0005f040: 7d7d 2e72 696f 2d62 7574 746f 6e7b 2d2d  }}.rio-button{--
+0005f050: 6f75 7465 722d 7465 7874 2d63 6f6c 6f72  outer-text-color
+0005f060: 3a20 7661 7228 2d2d 7269 6f2d 6c6f 6361  : var(--rio-loca
+0005f070: 6c2d 7465 7874 2d63 6f6c 6f72 297d 2e72  l-text-color)}.r
+0005f080: 696f 2d62 7574 746f 6e3e 2a7b 706f 696e  io-button>*{poin
+0005f090: 7465 722d 6576 656e 7473 3a61 7574 6f3b  ter-events:auto;
+0005f0a0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+0005f0b0: 653b 7769 6474 683a 3130 3025 3b68 6569  e;width:100%;hei
+0005f0c0: 6768 743a 3130 3025 3b6f 7665 7266 6c6f  ght:100%;overflo
+0005f0d0: 773a 6869 6464 656e 3b74 7261 6e73 6974  w:hidden;transit
+0005f0e0: 696f 6e3a 636f 6c6f 7220 2e31 7320 6561  ion:color .1s ea
+0005f0f0: 7365 2d69 6e2d 6f75 742c 626f 7264 6572  se-in-out,border
+0005f100: 2d63 6f6c 6f72 202e 3173 2065 6173 652d  -color .1s ease-
+0005f110: 696e 2d6f 7574 7d2e 7269 6f2d 6275 7474  in-out}.rio-butt
+0005f120: 6f6e 7374 796c 652d 6d61 6a6f 727b 6261  onstyle-major{ba
+0005f130: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+0005f140: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
+0005f150: 6729 3b62 6f78 2d73 6861 646f 773a 3020  g);box-shadow:0 
+0005f160: 3020 3020 7472 616e 7370 6172 656e 743b  0 0 transparent;
+0005f170: 7472 616e 7369 7469 6f6e 3a62 6163 6b67  transition:backg
+0005f180: 726f 756e 642d 636f 6c6f 7220 2e31 7320  round-color .1s 
+0005f190: 6561 7365 2d69 6e2d 6f75 742c 626f 782d  ease-in-out,box-
+0005f1a0: 7368 6164 6f77 202e 3273 2065 6173 652d  shadow .2s ease-
+0005f1b0: 696e 2d6f 7574 7d2e 7269 6f2d 6275 7474  in-out}.rio-butt
+0005f1c0: 6f6e 7374 796c 652d 6d61 6a6f 723a 686f  onstyle-major:ho
+0005f1d0: 7665 723a 6e6f 7428 2e72 696f 2d73 7769  ver:not(.rio-swi
+0005f1e0: 7463 6865 726f 6f2d 6469 7361 626c 6564  tcheroo-disabled
+0005f1f0: 297b 6261 636b 6772 6f75 6e64 2d63 6f6c  ){background-col
+0005f200: 6f72 3a76 6172 282d 2d72 696f 2d6c 6f63  or:var(--rio-loc
+0005f210: 616c 2d62 672d 6163 7469 7665 293b 6375  al-bg-active);cu
+0005f220: 7273 6f72 3a70 6f69 6e74 6572 3b62 6f78  rsor:pointer;box
+0005f230: 2d73 6861 646f 773a 3020 2e31 7265 6d20  -shadow:0 .1rem 
+0005f240: 2e32 3272 656d 2023 3030 3030 3030 3539  .22rem #00000059
+0005f250: 7d2e 7269 6f2d 6275 7474 6f6e 7374 796c  }.rio-buttonstyl
+0005f260: 652d 6d69 6e6f 723a 6e6f 7428 3a68 6f76  e-minor:not(:hov
+0005f270: 6572 297b 6f75 746c 696e 653a 2e31 7265  er){outline:.1re
+0005f280: 6d20 736f 6c69 6420 7661 7228 2d2d 7269  m solid var(--ri
+0005f290: 6f2d 6c6f 6361 6c2d 6267 293b 2d2d 7269  o-local-bg);--ri
+0005f2a0: 6f2d 6c6f 6361 6c2d 7465 7874 2d63 6f6c  o-local-text-col
+0005f2b0: 6f72 3a20 7661 7228 2d2d 7269 6f2d 6c6f  or: var(--rio-lo
+0005f2c0: 6361 6c2d 6267 297d 2e72 696f 2d62 7574  cal-bg)}.rio-but
+0005f2d0: 746f 6e73 7479 6c65 2d6d 696e 6f72 3a68  tonstyle-minor:h
+0005f2e0: 6f76 6572 3a6e 6f74 282e 7269 6f2d 7377  over:not(.rio-sw
+0005f2f0: 6974 6368 6572 6f6f 2d64 6973 6162 6c65  itcheroo-disable
+0005f300: 6429 7b62 6163 6b67 726f 756e 642d 636f  d){background-co
+0005f310: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
+0005f320: 6361 6c2d 6267 293b 6375 7273 6f72 3a70  cal-bg);cursor:p
+0005f330: 6f69 6e74 6572 7d2e 7269 6f2d 6275 7474  ointer}.rio-butt
+0005f340: 6f6e 7374 796c 652d 706c 6169 6e7b 2d2d  onstyle-plain{--
+0005f350: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d63  rio-local-text-c
+0005f360: 6f6c 6f72 3a20 7661 7228 2d2d 6f75 7465  olor: var(--oute
+0005f370: 722d 7465 7874 2d63 6f6c 6f72 297d 2e72  r-text-color)}.r
+0005f380: 696f 2d62 7574 746f 6e73 7479 6c65 2d70  io-buttonstyle-p
+0005f390: 6c61 696e 3a68 6f76 6572 3a6e 6f74 282e  lain:hover:not(.
+0005f3a0: 7269 6f2d 7377 6974 6368 6572 6f6f 2d64  rio-switcheroo-d
+0005f3b0: 6973 6162 6c65 6429 7b63 7572 736f 723a  isabled){cursor:
+0005f3c0: 706f 696e 7465 723b 2d2d 7269 6f2d 6c6f  pointer;--rio-lo
+0005f3d0: 6361 6c2d 7465 7874 2d63 6f6c 6f72 3a20  cal-text-color: 
+0005f3e0: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+0005f3f0: 6267 297d 2e72 696f 2d73 6861 7065 2d70  bg)}.rio-shape-p
+0005f400: 696c 6c7b 626f 7264 6572 2d72 6164 6975  ill{border-radiu
+0005f410: 733a 3939 3939 3970 787d 2e72 696f 2d73  s:99999px}.rio-s
+0005f420: 6861 7065 2d72 6f75 6e64 6564 7b62 6f72  hape-rounded{bor
+0005f430: 6465 722d 7261 6469 7573 3a76 6172 282d  der-radius:var(-
+0005f440: 2d72 696f 2d67 6c6f 6261 6c2d 636f 726e  -rio-global-corn
+0005f450: 6572 2d72 6164 6975 732d 736d 616c 6c29  er-radius-small)
+0005f460: 7d2e 7269 6f2d 7368 6170 652d 7265 6374  }.rio-shape-rect
+0005f470: 616e 676c 657b 626f 7264 6572 2d72 6164  angle{border-rad
+0005f480: 6975 733a 307d 2e72 696f 2d73 6861 7065  ius:0}.rio-shape
+0005f490: 2d63 6972 636c 657b 626f 7264 6572 2d72  -circle{border-r
+0005f4a0: 6164 6975 733a 3530 257d 2e72 696f 2d72  adius:50%}.rio-r
+0005f4b0: 6576 6561 6c65 727b 6469 7370 6c61 793a  evealer{display:
+0005f4c0: 666c 6578 3b66 6c65 782d 6469 7265 6374  flex;flex-direct
+0005f4d0: 696f 6e3a 636f 6c75 6d6e 3b61 6c69 676e  ion:column;align
+0005f4e0: 2d69 7465 6d73 3a73 7472 6574 6368 3b6a  -items:stretch;j
+0005f4f0: 7573 7469 6679 2d63 6f6e 7465 6e74 3a73  ustify-content:s
+0005f500: 7472 6574 6368 3b62 6f72 6465 722d 7261  tretch;border-ra
+0005f510: 6469 7573 3a76 6172 282d 2d72 696f 2d67  dius:var(--rio-g
+0005f520: 6c6f 6261 6c2d 636f 726e 6572 2d72 6164  lobal-corner-rad
+0005f530: 6975 732d 736d 616c 6c29 3b74 7261 6e73  ius-small);trans
+0005f540: 6974 696f 6e3a 6261 636b 6772 6f75 6e64  ition:background
+0005f550: 2d63 6f6c 6f72 202e 3135 7320 6561 7365  -color .15s ease
+0005f560: 2d6f 7574 3b6f 7665 7266 6c6f 773a 6869  -out;overflow:hi
+0005f570: 6464 656e 7d2e 7269 6f2d 7265 7665 616c  dden}.rio-reveal
+0005f580: 6572 2d68 6561 6465 727b 706f 696e 7465  er-header{pointe
+0005f590: 722d 6576 656e 7473 3a61 7574 6f3b 6375  r-events:auto;cu
+0005f5a0: 7273 6f72 3a70 6f69 6e74 6572 3b64 6973  rsor:pointer;dis
+0005f5b0: 706c 6179 3a66 6c65 783b 616c 6967 6e2d  play:flex;align-
+0005f5c0: 6974 656d 733a 6365 6e74 6572 3b6a 7573  items:center;jus
+0005f5d0: 7469 6679 2d63 6f6e 7465 6e74 3a73 7061  tify-content:spa
+0005f5e0: 6365 2d62 6574 7765 656e 3b63 6f6c 6f72  ce-between;color
+0005f5f0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
+0005f600: 2d74 6578 742d 636f 6c6f 7229 7d2e 7269  -text-color)}.ri
+0005f610: 6f2d 7265 7665 616c 6572 2d6c 6162 656c  o-revealer-label
+0005f620: 7b66 6c65 782d 6772 6f77 3a31 7d2e 7269  {flex-grow:1}.ri
+0005f630: 6f2d 7265 7665 616c 6572 2d61 7272 6f77  o-revealer-arrow
+0005f640: 7b74 7261 6e73 666f 726d 3a72 6f74 6174  {transform:rotat
+0005f650: 6528 3930 6465 6729 3b74 7261 6e73 6974  e(90deg);transit
+0005f660: 696f 6e3a 7472 616e 7366 6f72 6d20 2e32  ion:transform .2
+0005f670: 3573 2065 6173 652d 696e 2d6f 7574 7d2e  5s ease-in-out}.
+0005f680: 7269 6f2d 7265 7665 616c 6572 2d6f 7065  rio-revealer-ope
+0005f690: 6e20 2e72 696f 2d72 6576 6561 6c65 722d  n .rio-revealer-
+0005f6a0: 6172 726f 777b 7472 616e 7366 6f72 6d3a  arrow{transform:
+0005f6b0: 726f 7461 7465 2830 297d 2e72 696f 2d72  rotate(0)}.rio-r
+0005f6c0: 6576 6561 6c65 722d 636f 6e74 656e 742d  evealer-content-
+0005f6d0: 6f75 7465 727b 666c 6578 2d67 726f 773a  outer{flex-grow:
+0005f6e0: 313b 706f 7369 7469 6f6e 3a72 656c 6174  1;position:relat
+0005f6f0: 6976 653b 6f76 6572 666c 6f77 3a68 6964  ive;overflow:hid
+0005f700: 6465 6e7d 2e72 696f 2d72 6576 6561 6c65  den}.rio-reveale
+0005f710: 722d 636f 6e74 656e 742d 696e 6e65 727b  r-content-inner{
+0005f720: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
+0005f730: 653b 626f 7474 6f6d 3a30 3b6f 7061 6369  e;bottom:0;opaci
+0005f740: 7479 3a30 3b74 7261 6e73 666f 726d 3a74  ty:0;transform:t
+0005f750: 7261 6e73 6c61 7465 5928 2d35 3025 293b  ranslateY(-50%);
+0005f760: 7472 616e 7369 7469 6f6e 3a6f 7061 6369  transition:opaci
+0005f770: 7479 202e 3435 7320 6561 7365 2d69 6e2d  ty .45s ease-in-
+0005f780: 6f75 742c 7472 616e 7366 6f72 6d20 2e33  out,transform .3
+0005f790: 3573 2065 6173 657d 2e72 696f 2d72 6576  5s ease}.rio-rev
+0005f7a0: 6561 6c65 722d 6f70 656e 202e 7269 6f2d  ealer-open .rio-
+0005f7b0: 7265 7665 616c 6572 2d63 6f6e 7465 6e74  revealer-content
+0005f7c0: 2d69 6e6e 6572 7b6f 7061 6369 7479 3a31  -inner{opacity:1
+0005f7d0: 3b74 7261 6e73 666f 726d 3a74 7261 6e73  ;transform:trans
+0005f7e0: 6c61 7465 5928 3029 7d2e 7269 6f2d 7265  lateY(0)}.rio-re
+0005f7f0: 7665 616c 6572 2d63 6f6e 7465 6e74 2d69  vealer-content-i
+0005f800: 6e6e 6572 3e2a 7b70 6f73 6974 696f 6e3a  nner>*{position:
+0005f810: 7265 6c61 7469 7665 2169 6d70 6f72 7461  relative!importa
+0005f820: 6e74 7d2e 7269 6f2d 706c 6f74 7b64 6973  nt}.rio-plot{dis
+0005f830: 706c 6179 3a69 6e6c 696e 652d 626c 6f63  play:inline-bloc
+0005f840: 6b3b 6469 7370 6c61 793a 666c 6578 3b6a  k;display:flex;j
+0005f850: 7573 7469 6679 2d63 6f6e 7465 6e74 3a63  ustify-content:c
+0005f860: 656e 7465 723b 616c 6967 6e2d 6974 656d  enter;align-item
+0005f870: 733a 6365 6e74 6572 3b6f 7665 7266 6c6f  s:center;overflo
+0005f880: 773a 6869 6464 656e 7d2e 7269 6f2d 6963  w:hidden}.rio-ic
+0005f890: 6f6e 7b70 6f69 6e74 6572 2d65 7665 6e74  on{pointer-event
+0005f8a0: 733a 6175 746f 3b64 6973 706c 6179 3a66  s:auto;display:f
+0005f8b0: 6c65 783b 6a75 7374 6966 792d 636f 6e74  lex;justify-cont
+0005f8c0: 656e 743a 6365 6e74 6572 3b61 6c69 676e  ent:center;align
+0005f8d0: 2d69 7465 6d73 3a63 656e 7465 727d 2e72  -items:center}.r
+0005f8e0: 696f 2d73 6c69 6465 727b 706f 696e 7465  io-slider{pointe
+0005f8f0: 722d 6576 656e 7473 3a61 7574 6f3b 2d2d  r-events:auto;--
+0005f900: 7269 6f2d 736c 6964 6572 2d70 6f73 6974  rio-slider-posit
+0005f910: 696f 6e2d 7472 616e 7369 7469 6f6e 2d74  ion-transition-t
+0005f920: 696d 653a 202e 3373 7d2e 7269 6f2d 736c  ime: .3s}.rio-sl
+0005f930: 6964 6572 3a6e 6f74 282e 7269 6f2d 7377  ider:not(.rio-sw
+0005f940: 6974 6368 6572 6f6f 2d64 6973 6162 6c65  itcheroo-disable
+0005f950: 6429 7b63 7572 736f 723a 706f 696e 7465  d){cursor:pointe
+0005f960: 727d 2e72 696f 2d73 6c69 6465 722d 696e  r}.rio-slider-in
+0005f970: 6e65 727b 706f 696e 7465 722d 6576 656e  ner{pointer-even
+0005f980: 7473 3a6e 6f6e 653b 706f 7369 7469 6f6e  ts:none;position
+0005f990: 3a61 6273 6f6c 7574 653b 6c65 6674 3a2e  :absolute;left:.
+0005f9a0: 3672 656d 3b72 6967 6874 3a2e 3672 656d  6rem;right:.6rem
+0005f9b0: 3b68 6569 6768 743a 2e32 3572 656d 3b74  ;height:.25rem;t
+0005f9c0: 6f70 3a35 3025 3b74 7261 6e73 666f 726d  op:50%;transform
+0005f9d0: 3a74 7261 6e73 6c61 7465 5928 2d35 3025  :translateY(-50%
+0005f9e0: 297d 2e72 696f 2d73 6c69 6465 722d 7472  )}.rio-slider-tr
+0005f9f0: 6163 6b7b 706f 7369 7469 6f6e 3a61 6273  ack{position:abs
+0005fa00: 6f6c 7574 653b 7769 6474 683a 3130 3025  olute;width:100%
+0005fa10: 3b68 6569 6768 743a 3130 3025 3b6f 7061  ;height:100%;opa
+0005fa20: 6369 7479 3a2e 333b 6261 636b 6772 6f75  city:.3;backgrou
+0005fa30: 6e64 3a76 6172 282d 2d72 696f 2d6c 6f63  nd:var(--rio-loc
+0005fa40: 616c 2d74 6578 742d 636f 6c6f 7229 3b62  al-text-color);b
+0005fa50: 6f72 6465 722d 7261 6469 7573 3a39 3939  order-radius:999
+0005fa60: 3939 7078 7d2e 7269 6f2d 736c 6964 6572  99px}.rio-slider
+0005fa70: 2d66 696c 6c7b 706f 7369 7469 6f6e 3a61  -fill{position:a
+0005fa80: 6273 6f6c 7574 653b 6c65 6674 3a30 3b77  bsolute;left:0;w
+0005fa90: 6964 7468 3a76 6172 282d 2d72 696f 2d73  idth:var(--rio-s
+0005faa0: 6c69 6465 722d 6672 6163 7469 6f6e 293b  lider-fraction);
+0005fab0: 6865 6967 6874 3a31 3030 253b 6261 636b  height:100%;back
+0005fac0: 6772 6f75 6e64 3a76 6172 282d 2d72 696f  ground:var(--rio
+0005fad0: 2d6c 6f63 616c 2d6c 6576 656c 2d32 2d62  -local-level-2-b
+0005fae0: 6729 3b62 6f72 6465 722d 7261 6469 7573  g);border-radius
+0005faf0: 3a39 3939 3939 7078 3b74 7261 6e73 6974  :99999px;transit
+0005fb00: 696f 6e3a 7769 6474 6820 7661 7228 2d2d  ion:width var(--
+0005fb10: 7269 6f2d 736c 6964 6572 2d70 6f73 6974  rio-slider-posit
+0005fb20: 696f 6e2d 7472 616e 7369 7469 6f6e 2d74  ion-transition-t
+0005fb30: 696d 6529 2065 6173 652d 696e 2d6f 7574  ime) ease-in-out
+0005fb40: 7d2e 7269 6f2d 736c 6964 6572 2d67 6c6f  }.rio-slider-glo
+0005fb50: 777b 706f 7369 7469 6f6e 3a61 6273 6f6c  w{position:absol
+0005fb60: 7574 653b 6c65 6674 3a76 6172 282d 2d72  ute;left:var(--r
+0005fb70: 696f 2d73 6c69 6465 722d 6672 6163 7469  io-slider-fracti
+0005fb80: 6f6e 293b 746f 703a 3530 253b 7769 6474  on);top:50%;widt
+0005fb90: 683a 312e 3172 656d 3b68 6569 6768 743a  h:1.1rem;height:
+0005fba0: 312e 3172 656d 3b74 7261 6e73 666f 726d  1.1rem;transform
+0005fbb0: 3a74 7261 6e73 6c61 7465 282d 3530 252c  :translate(-50%,
+0005fbc0: 2d35 3025 293b 626f 7264 6572 2d72 6164  -50%);border-rad
+0005fbd0: 6975 733a 3530 253b 6261 636b 6772 6f75  ius:50%;backgrou
+0005fbe0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
+0005fbf0: 696f 2d6c 6f63 616c 2d6c 6576 656c 2d32  io-local-level-2
+0005fc00: 2d62 6729 3b6f 7061 6369 7479 3a30 253b  -bg);opacity:0%;
+0005fc10: 7472 616e 7369 7469 6f6e 3a6c 6566 7420  transition:left 
+0005fc20: 7661 7228 2d2d 7269 6f2d 736c 6964 6572  var(--rio-slider
+0005fc30: 2d70 6f73 6974 696f 6e2d 7472 616e 7369  -position-transi
+0005fc40: 7469 6f6e 2d74 696d 6529 2065 6173 652d  tion-time) ease-
+0005fc50: 696e 2d6f 7574 2c77 6964 7468 202e 3135  in-out,width .15
+0005fc60: 7320 6561 7365 2d69 6e2d 6f75 742c 6865  s ease-in-out,he
+0005fc70: 6967 6874 202e 3135 7320 6561 7365 2d69  ight .15s ease-i
+0005fc80: 6e2d 6f75 742c 6f70 6163 6974 7920 2e31  n-out,opacity .1
+0005fc90: 3573 2065 6173 652d 696e 2d6f 7574 7d2e  5s ease-in-out}.
+0005fca0: 7269 6f2d 736c 6964 6572 3a68 6f76 6572  rio-slider:hover
+0005fcb0: 3a6e 6f74 282e 7269 6f2d 7377 6974 6368  :not(.rio-switch
+0005fcc0: 6572 6f6f 2d64 6973 6162 6c65 6429 202e  eroo-disabled) .
+0005fcd0: 7269 6f2d 736c 6964 6572 2d67 6c6f 777b  rio-slider-glow{
+0005fce0: 7769 6474 683a 322e 3872 656d 3b68 6569  width:2.8rem;hei
+0005fcf0: 6768 743a 322e 3872 656d 3b6f 7061 6369  ght:2.8rem;opaci
+0005fd00: 7479 3a32 3025 7d2e 7269 6f2d 736c 6964  ty:20%}.rio-slid
+0005fd10: 6572 2d6b 6e6f 627b 706f 7369 7469 6f6e  er-knob{position
+0005fd20: 3a61 6273 6f6c 7574 653b 6c65 6674 3a76  :absolute;left:v
+0005fd30: 6172 282d 2d72 696f 2d73 6c69 6465 722d  ar(--rio-slider-
+0005fd40: 6672 6163 7469 6f6e 293b 746f 703a 3530  fraction);top:50
+0005fd50: 253b 7769 6474 683a 312e 3272 656d 3b68  %;width:1.2rem;h
+0005fd60: 6569 6768 743a 312e 3272 656d 3b74 7261  eight:1.2rem;tra
+0005fd70: 6e73 666f 726d 3a74 7261 6e73 6c61 7465  nsform:translate
+0005fd80: 282d 3530 252c 2d35 3025 293b 626f 7264  (-50%,-50%);bord
+0005fd90: 6572 2d72 6164 6975 733a 3530 253b 6261  er-radius:50%;ba
+0005fda0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+0005fdb0: 6172 282d 2d72 696f 2d6c 6f63 616c 2d6c  ar(--rio-local-l
+0005fdc0: 6576 656c 2d32 2d62 6729 3b62 6f78 2d73  evel-2-bg);box-s
+0005fdd0: 6861 646f 773a 3020 2e31 7265 6d20 2e32  hadow:0 .1rem .2
+0005fde0: 7265 6d20 7661 7228 2d2d 7269 6f2d 676c  rem var(--rio-gl
+0005fdf0: 6f62 616c 2d73 6861 646f 772d 636f 6c6f  obal-shadow-colo
+0005fe00: 7229 3b74 7261 6e73 6974 696f 6e3a 6c65  r);transition:le
+0005fe10: 6674 2076 6172 282d 2d72 696f 2d73 6c69  ft var(--rio-sli
+0005fe20: 6465 722d 706f 7369 7469 6f6e 2d74 7261  der-position-tra
+0005fe30: 6e73 6974 696f 6e2d 7469 6d65 2920 6561  nsition-time) ea
+0005fe40: 7365 2d69 6e2d 6f75 742c 6261 636b 6772  se-in-out,backgr
+0005fe50: 6f75 6e64 2d63 6f6c 6f72 202e 3173 2065  ound-color .1s e
+0005fe60: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
+0005fe70: 736c 6964 6573 686f 777b 706f 696e 7465  slideshow{pointe
+0005fe80: 722d 6576 656e 7473 3a61 7574 6f3b 6f76  r-events:auto;ov
+0005fe90: 6572 666c 6f77 3a68 6964 6465 6e7d 2e73  erflow:hidden}.s
+0005fea0: 6c69 6465 7368 6f77 2d63 6869 6c64 2d63  lideshow-child-c
+0005feb0: 6f6e 7461 696e 6572 7b70 6f73 6974 696f  ontainer{positio
+0005fec0: 6e3a 7265 6c61 7469 7665 3b64 6973 706c  n:relative;displ
+0005fed0: 6179 3a67 7269 643b 7769 6474 683a 3130  ay:grid;width:10
+0005fee0: 3025 3b68 6569 6768 743a 3130 3025 7d2e  0%;height:100%}.
+0005fef0: 736c 6964 6573 686f 772d 6368 696c 642d  slideshow-child-
+0005ff00: 636f 6e74 6169 6e65 723e 6469 767b 6772  container>div{gr
+0005ff10: 6964 2d63 6f6c 756d 6e2d 7374 6172 743a  id-column-start:
+0005ff20: 313b 6772 6964 2d72 6f77 2d73 7461 7274  1;grid-row-start
+0005ff30: 3a31 3b77 6964 7468 3a31 3030 253b 6865  :1;width:100%;he
+0005ff40: 6967 6874 3a31 3030 257d 2e73 6c69 6465  ight:100%}.slide
+0005ff50: 7368 6f77 2d63 6869 6c64 2d63 6f6e 7461  show-child-conta
+0005ff60: 696e 6572 3e64 6976 3e2a 7b67 7269 642d  iner>div>*{grid-
+0005ff70: 636f 6c75 6d6e 2d73 7461 7274 3a31 3b67  column-start:1;g
+0005ff80: 7269 642d 726f 772d 7374 6172 743a 313b  rid-row-start:1;
+0005ff90: 7769 6474 683a 3130 3025 3b68 6569 6768  width:100%;heigh
+0005ffa0: 743a 3130 3025 7d2e 736c 6964 6573 686f  t:100%}.slidesho
+0005ffb0: 772d 7072 6f67 7265 7373 7b70 6f73 6974  w-progress{posit
+0005ffc0: 696f 6e3a 6162 736f 6c75 7465 3b62 6f74  ion:absolute;bot
+0005ffd0: 746f 6d3a 303b 7769 6474 683a 3130 3025  tom:0;width:100%
+0005ffe0: 3b68 6569 6768 743a 2e33 7265 6d3b 6261  ;height:.3rem;ba
+0005fff0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+00060000: 6172 282d 2d72 696f 2d6c 6f63 616c 2d6c  ar(--rio-local-l
+00060010: 6576 656c 2d32 2d62 6729 7d2e 7269 6f2d  evel-2-bg)}.rio-
+00060020: 6f76 6572 6c61 797b 706f 696e 7465 722d  overlay{pointer-
+00060030: 6576 656e 7473 3a6e 6f6e 653b 706f 7369  events:none;posi
+00060040: 7469 6f6e 3a66 6978 6564 2169 6d70 6f72  tion:fixed!impor
+00060050: 7461 6e74 3b74 6f70 3a30 2169 6d70 6f72  tant;top:0!impor
+00060060: 7461 6e74 3b6c 6566 743a 3021 696d 706f  tant;left:0!impo
+00060070: 7274 616e 743b 7769 6474 683a 756e 7365  rtant;width:unse
+00060080: 7421 696d 706f 7274 616e 743b 6865 6967  t!important;heig
+00060090: 6874 3a75 6e73 6574 2169 6d70 6f72 7461  ht:unset!importa
+000600a0: 6e74 3b7a 2d69 6e64 6578 3a31 3030 3030  nt;z-index:10000
+000600b0: 7d2e 7269 6f2d 7370 6163 6572 7b70 6f69  }.rio-spacer{poi
+000600c0: 6e74 6572 2d65 7665 6e74 733a 6e6f 6e65  nter-events:none
+000600d0: 7d2e 7269 6f2d 6d65 6469 612d 706c 6179  }.rio-media-play
+000600e0: 6572 7b70 6f69 6e74 6572 2d65 7665 6e74  er{pointer-event
+000600f0: 733a 6175 746f 7d2e 7269 6f2d 6d65 6469  s:auto}.rio-medi
+00060100: 612d 706c 6179 6572 2076 6964 656f 7b70  a-player video{p
+00060110: 6f69 6e74 6572 2d65 7665 6e74 733a 6e6f  ointer-events:no
+00060120: 6e65 3b77 6964 7468 3a31 3030 253b 6865  ne;width:100%;he
+00060130: 6967 6874 3a31 3030 253b 6f62 6a65 6374  ight:100%;object
+00060140: 2d66 6974 3a63 6f6e 7461 696e 7d2e 7269  -fit:contain}.ri
+00060150: 6f2d 6d65 6469 612d 706c 6179 6572 2d61  o-media-player-a
+00060160: 6c74 2d64 6973 706c 6179 7b70 6f69 6e74  lt-display{point
+00060170: 6572 2d65 7665 6e74 733a 6e6f 6e65 3b70  er-events:none;p
+00060180: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
+00060190: 3b6c 6566 743a 3530 253b 746f 703a 3530  ;left:50%;top:50
+000601a0: 253b 7769 6474 683a 3530 253b 6865 6967  %;width:50%;heig
+000601b0: 6874 3a35 3025 3b6d 6178 2d77 6964 7468  ht:50%;max-width
+000601c0: 3a32 3072 656d 3b6d 6178 2d68 6569 6768  :20rem;max-heigh
+000601d0: 743a 3230 7265 6d3b 6173 7065 6374 2d72  t:20rem;aspect-r
+000601e0: 6174 696f 3a31 3b6f 7061 6369 7479 3a2e  atio:1;opacity:.
+000601f0: 353b 7472 616e 7366 6f72 6d3a 7472 616e  5;transform:tran
+00060200: 736c 6174 6528 2d35 3025 2c2d 3530 2529  slate(-50%,-50%)
+00060210: 7d2e 7269 6f2d 6d65 6469 612d 706c 6179  }.rio-media-play
+00060220: 6572 2d63 6f6e 7472 6f6c 737b 706f 7369  er-controls{posi
+00060230: 7469 6f6e 3a61 6273 6f6c 7574 653b 6c65  tion:absolute;le
+00060240: 6674 3a30 3b62 6f74 746f 6d3a 303b 7269  ft:0;bottom:0;ri
+00060250: 6768 743a 303b 6261 636b 6772 6f75 6e64  ght:0;background
+00060260: 3a6c 696e 6561 722d 6772 6164 6965 6e74  :linear-gradient
+00060270: 2872 6762 6128 302c 302c 302c 3029 2c72  (rgba(0,0,0,0),r
+00060280: 6762 6128 302c 302c 302c 2e36 2929 3b70  gba(0,0,0,.6));p
+00060290: 6164 6469 6e67 2d74 6f70 3a32 2e35 7265  adding-top:2.5re
+000602a0: 6d3b 6469 7370 6c61 793a 666c 6578 3b66  m;display:flex;f
+000602b0: 6c65 782d 6469 7265 6374 696f 6e3a 636f  lex-direction:co
+000602c0: 6c75 6d6e 3b67 6170 3a30 7265 6d3b 616c  lumn;gap:0rem;al
+000602d0: 6967 6e2d 6974 656d 733a 7374 7265 7463  ign-items:stretc
+000602e0: 683b 7472 616e 7369 7469 6f6e 3a6f 7061  h;transition:opa
+000602f0: 6369 7479 202e 3473 2065 6173 652d 696e  city .4s ease-in
+00060300: 2d6f 7574 7d2e 7269 6f2d 6d65 6469 612d  -out}.rio-media-
+00060310: 706c 6179 6572 2d74 696d 656c 696e 657b  player-timeline{
+00060320: 706f 696e 7465 722d 6576 656e 7473 3a61  pointer-events:a
+00060330: 7574 6f3b 6375 7273 6f72 3a70 6f69 6e74  uto;cursor:point
+00060340: 6572 3b70 6f73 6974 696f 6e3a 7265 6c61  er;position:rela
+00060350: 7469 7665 3b68 6569 6768 743a 3272 656d  tive;height:2rem
+00060360: 3b6d 6172 6769 6e3a 3020 2e35 7265 6d7d  ;margin:0 .5rem}
+00060370: 2e72 696f 2d6d 6564 6961 2d70 6c61 7965  .rio-media-playe
+00060380: 722d 7469 6d65 6c69 6e65 3e64 6976 7b70  r-timeline>div{p
+00060390: 6f69 6e74 6572 2d65 7665 6e74 733a 6e6f  ointer-events:no
+000603a0: 6e65 3b70 6f73 6974 696f 6e3a 7265 6c61  ne;position:rela
+000603b0: 7469 7665 3b74 6f70 3a35 3025 3b68 6569  tive;top:50%;hei
+000603c0: 6768 743a 2e32 7265 6d3b 7472 616e 7366  ght:.2rem;transf
+000603d0: 6f72 6d3a 7472 616e 736c 6174 6559 282d  orm:translateY(-
+000603e0: 3530 2529 3b74 7261 6e73 6974 696f 6e3a  50%);transition:
+000603f0: 6865 6967 6874 202e 3273 2065 6173 652d  height .2s ease-
+00060400: 696e 2d6f 7574 7d2e 7269 6f2d 6d65 6469  in-out}.rio-medi
+00060410: 612d 706c 6179 6572 2d74 696d 656c 696e  a-player-timelin
+00060420: 653a 686f 7665 723e 6469 767b 6865 6967  e:hover>div{heig
+00060430: 6874 3a2e 3472 656d 7d2e 7269 6f2d 6d65  ht:.4rem}.rio-me
+00060440: 6469 612d 706c 6179 6572 2d74 696d 656c  dia-player-timel
+00060450: 696e 652d 6b6e 6f62 7b70 6f73 6974 696f  ine-knob{positio
+00060460: 6e3a 6162 736f 6c75 7465 3b77 6964 7468  n:absolute;width
+00060470: 3a30 7265 6d3b 6865 6967 6874 3a30 7265  :0rem;height:0re
+00060480: 6d3b 6c65 6674 3a31 3030 253b 746f 703a  m;left:100%;top:
+00060490: 3530 253b 6261 636b 6772 6f75 6e64 2d63  50%;background-c
+000604a0: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d67  olor:var(--rio-g
+000604b0: 6c6f 6261 6c2d 7072 696d 6172 792d 6267  lobal-primary-bg
+000604c0: 293b 626f 7264 6572 2d72 6164 6975 733a  );border-radius:
+000604d0: 3530 253b 7472 616e 7366 6f72 6d3a 7472  50%;transform:tr
+000604e0: 616e 736c 6174 6528 2d35 3025 2c2d 3530  anslate(-50%,-50
+000604f0: 2529 3b74 7261 6e73 6974 696f 6e3a 7769  %);transition:wi
+00060500: 6474 6820 2e32 7320 6561 7365 2d69 6e2d  dth .2s ease-in-
+00060510: 6f75 742c 6865 6967 6874 202e 3273 2065  out,height .2s e
+00060520: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
+00060530: 6d65 6469 612d 706c 6179 6572 2d74 696d  media-player-tim
+00060540: 656c 696e 653a 686f 7665 7220 2e72 696f  eline:hover .rio
+00060550: 2d6d 6564 6961 2d70 6c61 7965 722d 7469  -media-player-ti
+00060560: 6d65 6c69 6e65 2d6b 6e6f 627b 7769 6474  meline-knob{widt
+00060570: 683a 2e39 7265 6d3b 6865 6967 6874 3a2e  h:.9rem;height:.
+00060580: 3972 656d 7d2e 7269 6f2d 6d65 6469 612d  9rem}.rio-media-
+00060590: 706c 6179 6572 2d74 696d 656c 696e 652d  player-timeline-
+000605a0: 6261 636b 6772 6f75 6e64 2c2e 7269 6f2d  background,.rio-
+000605b0: 6d65 6469 612d 706c 6179 6572 2d74 696d  media-player-tim
+000605c0: 656c 696e 652d 6c6f 6164 6564 2c2e 7269  eline-loaded,.ri
+000605d0: 6f2d 6d65 6469 612d 706c 6179 6572 2d74  o-media-player-t
+000605e0: 696d 656c 696e 652d 686f 7665 722c 2e72  imeline-hover,.r
 000605f0: 696f 2d6d 6564 6961 2d70 6c61 7965 722d  io-media-player-
-00060600: 7469 6d65 6c69 6e65 2d62 6163 6b67 726f  timeline-backgro
-00060610: 756e 647b 7769 6474 683a 3130 3025 3b6f  und{width:100%;o
-00060620: 7061 6369 7479 3a2e 327d 2e72 696f 2d6d  pacity:.2}.rio-m
-00060630: 6564 6961 2d70 6c61 7965 722d 7469 6d65  edia-player-time
-00060640: 6c69 6e65 2d6c 6f61 6465 647b 6f70 6163  line-loaded{opac
-00060650: 6974 793a 2e33 7d2e 7269 6f2d 6d65 6469  ity:.3}.rio-medi
-00060660: 612d 706c 6179 6572 2d74 696d 656c 696e  a-player-timelin
-00060670: 652d 686f 7665 727b 6f70 6163 6974 793a  e-hover{opacity:
-00060680: 303b 7472 616e 7369 7469 6f6e 3a6f 7061  0;transition:opa
-00060690: 6369 7479 202e 3273 2065 6173 652d 696e  city .2s ease-in
-000606a0: 2d6f 7574 7d2e 7269 6f2d 6d65 6469 612d  -out}.rio-media-
-000606b0: 706c 6179 6572 2d74 696d 656c 696e 652d  player-timeline-
-000606c0: 706c 6179 6564 7b62 6163 6b67 726f 756e  played{backgroun
-000606d0: 642d 636f 6c6f 723a 7661 7228 2d2d 7269  d-color:var(--ri
-000606e0: 6f2d 676c 6f62 616c 2d70 7269 6d61 7279  o-global-primary
-000606f0: 2d62 6729 7d2e 7269 6f2d 6d65 6469 612d  -bg)}.rio-media-
-00060700: 706c 6179 6572 2d63 6f6e 7472 6f6c 732d  player-controls-
-00060710: 726f 777b 6469 7370 6c61 793a 666c 6578  row{display:flex
-00060720: 3b67 6170 3a31 2e32 7265 6d3b 616c 6967  ;gap:1.2rem;alig
-00060730: 6e2d 6974 656d 733a 6365 6e74 6572 3b70  n-items:center;p
-00060740: 6164 6469 6e67 3a2e 3572 656d 3b70 6164  adding:.5rem;pad
-00060750: 6469 6e67 2d74 6f70 3a30 7d2e 7269 6f2d  ding-top:0}.rio-
-00060760: 6d65 6469 612d 706c 6179 6572 2d62 7574  media-player-but
-00060770: 746f 6e7b 706f 696e 7465 722d 6576 656e  ton{pointer-even
-00060780: 7473 3a61 7574 6f3b 6375 7273 6f72 3a70  ts:auto;cursor:p
-00060790: 6f69 6e74 6572 3b77 6964 7468 3a32 7265  ointer;width:2re
-000607a0: 6d3b 6865 6967 6874 3a32 7265 6d7d 2e72  m;height:2rem}.r
-000607b0: 696f 2d6d 6564 6961 2d70 6c61 7965 722d  io-media-player-
-000607c0: 6275 7474 6f6e 3e69 6d67 7b77 6964 7468  button>img{width
-000607d0: 3a31 3030 253b 6865 6967 6874 3a31 3030  :100%;height:100
-000607e0: 257d 2e72 696f 2d6d 6564 6961 2d70 6c61  %}.rio-media-pla
-000607f0: 7965 722d 766f 6c75 6d65 7b70 6f69 6e74  yer-volume{point
-00060800: 6572 2d65 7665 6e74 733a 6175 746f 3b63  er-events:auto;c
-00060810: 7572 736f 723a 706f 696e 7465 723b 706f  ursor:pointer;po
-00060820: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
-00060830: 7769 6474 683a 3572 656d 3b68 6569 6768  width:5rem;heigh
-00060840: 743a 312e 3572 656d 7d2e 7269 6f2d 6d65  t:1.5rem}.rio-me
-00060850: 6469 612d 706c 6179 6572 2d76 6f6c 756d  dia-player-volum
-00060860: 653e 6469 767b 706f 696e 7465 722d 6576  e>div{pointer-ev
-00060870: 656e 7473 3a6e 6f6e 653b 706f 7369 7469  ents:none;positi
-00060880: 6f6e 3a72 656c 6174 6976 653b 746f 703a  on:relative;top:
-00060890: 3530 253b 6865 6967 6874 3a2e 3272 656d  50%;height:.2rem
-000608a0: 3b74 7261 6e73 666f 726d 3a74 7261 6e73  ;transform:trans
-000608b0: 6c61 7465 5928 2d35 3025 297d 2e72 696f  lateY(-50%)}.rio
-000608c0: 2d6d 6564 6961 2d70 6c61 7965 722d 766f  -media-player-vo
-000608d0: 6c75 6d65 2d62 6163 6b67 726f 756e 642c  lume-background,
-000608e0: 2e72 696f 2d6d 6564 6961 2d70 6c61 7965  .rio-media-playe
-000608f0: 722d 766f 6c75 6d65 2d63 7572 7265 6e74  r-volume-current
-00060900: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
-00060910: 7465 3b77 6964 7468 3a31 3030 253b 6865  te;width:100%;he
-00060920: 6967 6874 3a31 3030 253b 626f 7264 6572  ight:100%;border
-00060930: 2d72 6164 6975 733a 3939 3939 3970 783b  -radius:99999px;
-00060940: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00060950: 3a23 6666 667d 2e72 696f 2d6d 6564 6961  :#fff}.rio-media
-00060960: 2d70 6c61 7965 722d 766f 6c75 6d65 2d62  -player-volume-b
-00060970: 6163 6b67 726f 756e 647b 6f70 6163 6974  ackground{opacit
-00060980: 793a 2e32 7d2e 7269 6f2d 6d65 6469 612d  y:.2}.rio-media-
-00060990: 706c 6179 6572 2d76 6f6c 756d 652d 6b6e  player-volume-kn
-000609a0: 6f62 7b70 6f73 6974 696f 6e3a 6162 736f  ob{position:abso
-000609b0: 6c75 7465 3b77 6964 7468 3a2e 3972 656d  lute;width:.9rem
-000609c0: 3b68 6569 6768 743a 2e39 7265 6d3b 6c65  ;height:.9rem;le
-000609d0: 6674 3a31 3030 253b 746f 703a 3530 253b  ft:100%;top:50%;
-000609e0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-000609f0: 3a23 6666 663b 626f 7264 6572 2d72 6164  :#fff;border-rad
-00060a00: 6975 733a 3530 253b 7472 616e 7366 6f72  ius:50%;transfor
-00060a10: 6d3a 7472 616e 736c 6174 6528 2d35 3025  m:translate(-50%
-00060a20: 2c2d 3530 2529 7d2e 7269 6f2d 6d65 6469  ,-50%)}.rio-medi
-00060a30: 612d 706c 6179 6572 2d76 6f6c 756d 653e  a-player-volume>
-00060a40: 6469 767b 706f 7369 7469 6f6e 3a72 656c  div{position:rel
-00060a50: 6174 6976 653b 746f 703a 3530 253b 6865  ative;top:50%;he
-00060a60: 6967 6874 3a2e 3272 656d 3b74 7261 6e73  ight:.2rem;trans
-00060a70: 666f 726d 3a74 7261 6e73 6c61 7465 5928  form:translateY(
-00060a80: 2d35 3025 297d 2e72 696f 2d6d 6564 6961  -50%)}.rio-media
-00060a90: 2d70 6c61 7965 722d 706c 6179 7469 6d65  -player-playtime
-00060aa0: 2d6c 6162 656c 7b63 6f6c 6f72 3a23 6666  -label{color:#ff
-00060ab0: 663b 6f70 6163 6974 793a 2e36 7d2e 7269  f;opacity:.6}.ri
-00060ac0: 6f2d 6d61 726b 646f 776e 7b70 6f69 6e74  o-markdown{point
-00060ad0: 6572 2d65 7665 6e74 733a 6175 746f 3b63  er-events:auto;c
-00060ae0: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
-00060af0: 6f63 616c 2d74 6578 742d 636f 6c6f 7229  ocal-text-color)
-00060b00: 7d2e 7269 6f2d 6d61 726b 646f 776e 3e2a  }.rio-markdown>*
-00060b10: 2c2e 7269 6f2d 6d61 726b 646f 776e 206c  ,.rio-markdown l
-00060b20: 693e 2a7b 6d61 7267 696e 2d74 6f70 3a30  i>*{margin-top:0
-00060b30: 3b6d 6172 6769 6e2d 626f 7474 6f6d 3a30  ;margin-bottom:0
-00060b40: 7d2e 7269 6f2d 6d61 726b 646f 776e 3e2a  }.rio-markdown>*
-00060b50: 2b2a 2c2e 7269 6f2d 6d61 726b 646f 776e  +*,.rio-markdown
-00060b60: 206c 693e 2a2b 2a7b 6d61 7267 696e 2d74   li>*+*{margin-t
-00060b70: 6f70 3a2e 3872 656d 7d2e 7269 6f2d 6d61  op:.8rem}.rio-ma
-00060b80: 726b 646f 776e 2075 6c7b 7061 6464 696e  rkdown ul{paddin
-00060b90: 672d 6c65 6674 3a31 7265 6d3b 6c69 7374  g-left:1rem;list
-00060ba0: 2d73 7479 6c65 2d74 7970 653a 6e6f 6e65  -style-type:none
-00060bb0: 7d2e 7269 6f2d 6d61 726b 646f 776e 2075  }.rio-markdown u
-00060bc0: 6c3e 6c69 3a62 6566 6f72 657b 636f 6e74  l>li:before{cont
-00060bd0: 656e 743a 222d 223b 666f 6e74 2d77 6569  ent:"-";font-wei
-00060be0: 6768 743a 3730 303b 706f 7369 7469 6f6e  ght:700;position
-00060bf0: 3a61 6273 6f6c 7574 653b 7472 616e 7366  :absolute;transf
-00060c00: 6f72 6d3a 7472 616e 736c 6174 6528 2d2e  orm:translate(-.
-00060c10: 3672 656d 297d 2e72 696f 2d6d 6172 6b64  6rem)}.rio-markd
-00060c20: 6f77 6e20 6c69 2b6c 697b 6d61 7267 696e  own li+li{margin
-00060c30: 2d74 6f70 3a2e 3272 656d 7d2e 7269 6f2d  -top:.2rem}.rio-
-00060c40: 6d61 726b 646f 776e 2063 6f64 657b 666f  markdown code{fo
-00060c50: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
-00060c60: 7269 6f2d 676c 6f62 616c 2d6d 6f6e 6f73  rio-global-monos
-00060c70: 7061 6365 2d66 6f6e 7429 2c6d 6f6e 6f73  pace-font),monos
-00060c80: 7061 6365 3b62 6163 6b67 726f 756e 643a  pace;background:
-00060c90: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00060ca0: 6267 2d76 6172 6961 6e74 293b 626f 7264  bg-variant);bord
-00060cb0: 6572 2d72 6164 6975 733a 7661 7228 2d2d  er-radius:var(--
-00060cc0: 7269 6f2d 676c 6f62 616c 2d63 6f72 6e65  rio-global-corne
-00060cd0: 722d 7261 6469 7573 2d73 6d61 6c6c 293b  r-radius-small);
-00060ce0: 7061 6464 696e 673a 2e31 7265 6d20 2e33  padding:.1rem .3
-00060cf0: 7265 6d7d 2e72 696f 2d6d 6172 6b64 6f77  rem}.rio-markdow
-00060d00: 6e20 6831 7b66 6f6e 742d 6661 6d69 6c79  n h1{font-family
-00060d10: 3a76 6172 282d 2d72 696f 2d67 6c6f 6261  :var(--rio-globa
-00060d20: 6c2d 6865 6164 696e 6731 2d66 6f6e 742d  l-heading1-font-
-00060d30: 6e61 6d65 293b 636f 6c6f 723a 7661 7228  name);color:var(
-00060d40: 2d2d 7269 6f2d 6c6f 6361 6c2d 6865 6164  --rio-local-head
-00060d50: 696e 6731 2d63 6f6c 6f72 293b 666f 6e74  ing1-color);font
-00060d60: 2d73 697a 653a 7661 7228 2d2d 7269 6f2d  -size:var(--rio-
-00060d70: 676c 6f62 616c 2d68 6561 6469 6e67 312d  global-heading1-
-00060d80: 666f 6e74 2d73 697a 6529 3b66 6f6e 742d  font-size);font-
-00060d90: 7374 796c 653a 7661 7228 2d2d 7269 6f2d  style:var(--rio-
-00060da0: 676c 6f62 616c 2d68 6561 6469 6e67 312d  global-heading1-
-00060db0: 6974 616c 6963 293b 666f 6e74 2d77 6569  italic);font-wei
-00060dc0: 6768 743a 7661 7228 2d2d 7269 6f2d 676c  ght:var(--rio-gl
-00060dd0: 6f62 616c 2d68 6561 6469 6e67 312d 666f  obal-heading1-fo
-00060de0: 6e74 2d77 6569 6768 7429 3b74 6578 742d  nt-weight);text-
-00060df0: 6465 636f 7261 7469 6f6e 3a76 6172 282d  decoration:var(-
-00060e00: 2d72 696f 2d67 6c6f 6261 6c2d 6865 6164  -rio-global-head
-00060e10: 696e 6731 2d75 6e64 6572 6c69 6e65 6429  ing1-underlined)
-00060e20: 3b74 6578 742d 7472 616e 7366 6f72 6d3a  ;text-transform:
-00060e30: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00060e40: 2d68 6561 6469 6e67 312d 616c 6c2d 6361  -heading1-all-ca
-00060e50: 7073 297d 2e72 696f 2d6d 6172 6b64 6f77  ps)}.rio-markdow
-00060e60: 6e20 6831 3a6e 6f74 283a 6669 7273 742d  n h1:not(:first-
-00060e70: 6368 696c 6429 7b6d 6172 6769 6e2d 746f  child){margin-to
-00060e80: 703a 3272 656d 7d2e 7269 6f2d 6d61 726b  p:2rem}.rio-mark
-00060e90: 646f 776e 2068 313a 6e6f 7428 3a6c 6173  down h1:not(:las
-00060ea0: 742d 6368 696c 6429 7b6d 6172 6769 6e2d  t-child){margin-
-00060eb0: 626f 7474 6f6d 3a31 7265 6d7d 2e72 696f  bottom:1rem}.rio
-00060ec0: 2d6d 6172 6b64 6f77 6e20 6832 7b66 6f6e  -markdown h2{fon
-00060ed0: 742d 6661 6d69 6c79 3a76 6172 282d 2d72  t-family:var(--r
-00060ee0: 696f 2d67 6c6f 6261 6c2d 6865 6164 696e  io-global-headin
-00060ef0: 6732 2d66 6f6e 742d 6e61 6d65 293b 636f  g2-font-name);co
-00060f00: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
-00060f10: 6361 6c2d 6865 6164 696e 6732 2d63 6f6c  cal-heading2-col
-00060f20: 6f72 293b 666f 6e74 2d73 697a 653a 7661  or);font-size:va
-00060f30: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
-00060f40: 6561 6469 6e67 322d 666f 6e74 2d73 697a  eading2-font-siz
-00060f50: 6529 3b66 6f6e 742d 7374 796c 653a 7661  e);font-style:va
-00060f60: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
-00060f70: 6561 6469 6e67 322d 6974 616c 6963 293b  eading2-italic);
-00060f80: 666f 6e74 2d77 6569 6768 743a 7661 7228  font-weight:var(
-00060f90: 2d2d 7269 6f2d 676c 6f62 616c 2d68 6561  --rio-global-hea
-00060fa0: 6469 6e67 322d 666f 6e74 2d77 6569 6768  ding2-font-weigh
-00060fb0: 7429 3b74 6578 742d 6465 636f 7261 7469  t);text-decorati
-00060fc0: 6f6e 3a76 6172 282d 2d72 696f 2d67 6c6f  on:var(--rio-glo
-00060fd0: 6261 6c2d 6865 6164 696e 6732 2d75 6e64  bal-heading2-und
-00060fe0: 6572 6c69 6e65 6429 3b74 6578 742d 7472  erlined);text-tr
-00060ff0: 616e 7366 6f72 6d3a 7661 7228 2d2d 7269  ansform:var(--ri
-00061000: 6f2d 676c 6f62 616c 2d68 6561 6469 6e67  o-global-heading
-00061010: 322d 616c 6c2d 6361 7073 293b 6d61 7267  2-all-caps);marg
-00061020: 696e 2d74 6f70 3a30 7d2e 7269 6f2d 6d61  in-top:0}.rio-ma
-00061030: 726b 646f 776e 2068 323a 6e6f 7428 3a66  rkdown h2:not(:f
-00061040: 6972 7374 2d63 6869 6c64 297b 6d61 7267  irst-child){marg
-00061050: 696e 2d74 6f70 3a31 2e35 7265 6d7d 2e72  in-top:1.5rem}.r
-00061060: 696f 2d6d 6172 6b64 6f77 6e20 6832 3a6e  io-markdown h2:n
-00061070: 6f74 283a 6c61 7374 2d63 6869 6c64 297b  ot(:last-child){
-00061080: 6d61 7267 696e 2d62 6f74 746f 6d3a 3172  margin-bottom:1r
-00061090: 656d 7d2e 7269 6f2d 6d61 726b 646f 776e  em}.rio-markdown
-000610a0: 2068 337b 666f 6e74 2d66 616d 696c 793a   h3{font-family:
-000610b0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-000610c0: 2d68 6561 6469 6e67 332d 666f 6e74 2d6e  -heading3-font-n
-000610d0: 616d 6529 3b63 6f6c 6f72 3a76 6172 282d  ame);color:var(-
-000610e0: 2d72 696f 2d6c 6f63 616c 2d68 6561 6469  -rio-local-headi
-000610f0: 6e67 332d 636f 6c6f 7229 3b66 6f6e 742d  ng3-color);font-
-00061100: 7369 7a65 3a76 6172 282d 2d72 696f 2d67  size:var(--rio-g
-00061110: 6c6f 6261 6c2d 6865 6164 696e 6733 2d66  lobal-heading3-f
-00061120: 6f6e 742d 7369 7a65 293b 666f 6e74 2d73  ont-size);font-s
-00061130: 7479 6c65 3a76 6172 282d 2d72 696f 2d67  tyle:var(--rio-g
-00061140: 6c6f 6261 6c2d 6865 6164 696e 6733 2d69  lobal-heading3-i
-00061150: 7461 6c69 6329 3b66 6f6e 742d 7765 6967  talic);font-weig
-00061160: 6874 3a76 6172 282d 2d72 696f 2d67 6c6f  ht:var(--rio-glo
-00061170: 6261 6c2d 6865 6164 696e 6733 2d66 6f6e  bal-heading3-fon
-00061180: 742d 7765 6967 6874 293b 7465 7874 2d64  t-weight);text-d
-00061190: 6563 6f72 6174 696f 6e3a 7661 7228 2d2d  ecoration:var(--
-000611a0: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
-000611b0: 6e67 332d 756e 6465 726c 696e 6564 293b  ng3-underlined);
-000611c0: 7465 7874 2d74 7261 6e73 666f 726d 3a76  text-transform:v
-000611d0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-000611e0: 6865 6164 696e 6733 2d61 6c6c 2d63 6170  heading3-all-cap
-000611f0: 7329 3b6d 6172 6769 6e2d 746f 703a 307d  s);margin-top:0}
-00061200: 2e72 696f 2d6d 6172 6b64 6f77 6e20 6833  .rio-markdown h3
-00061210: 3a6e 6f74 283a 6669 7273 742d 6368 696c  :not(:first-chil
-00061220: 6429 7b6d 6172 6769 6e2d 746f 703a 3172  d){margin-top:1r
-00061230: 656d 7d2e 7269 6f2d 6d61 726b 646f 776e  em}.rio-markdown
-00061240: 2068 333a 6e6f 7428 3a6c 6173 742d 6368   h3:not(:last-ch
-00061250: 696c 6429 7b6d 6172 6769 6e2d 626f 7474  ild){margin-bott
-00061260: 6f6d 3a2e 3572 656d 7d2e 7269 6f2d 6d61  om:.5rem}.rio-ma
-00061270: 726b 646f 776e 2070 7b66 6f6e 742d 6661  rkdown p{font-fa
-00061280: 6d69 6c79 3a76 6172 282d 2d72 696f 2d67  mily:var(--rio-g
-00061290: 6c6f 6261 6c2d 666f 6e74 293b 636f 6c6f  lobal-font);colo
-000612a0: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
-000612b0: 6c2d 7465 7874 2d63 6f6c 6f72 293b 666f  l-text-color);fo
-000612c0: 6e74 2d73 697a 653a 7661 7228 2d2d 7269  nt-size:var(--ri
-000612d0: 6f2d 676c 6f62 616c 2d74 6578 742d 666f  o-global-text-fo
-000612e0: 6e74 2d73 697a 6529 3b66 6f6e 742d 7374  nt-size);font-st
-000612f0: 796c 653a 7661 7228 2d2d 7269 6f2d 676c  yle:var(--rio-gl
-00061300: 6f62 616c 2d74 6578 742d 6974 616c 6963  obal-text-italic
-00061310: 293b 666f 6e74 2d77 6569 6768 743a 7661  );font-weight:va
-00061320: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d74  r(--rio-global-t
-00061330: 6578 742d 666f 6e74 2d77 6569 6768 7429  ext-font-weight)
-00061340: 3b74 6578 742d 6465 636f 7261 7469 6f6e  ;text-decoration
-00061350: 3a76 6172 282d 2d72 696f 2d67 6c6f 6261  :var(--rio-globa
-00061360: 6c2d 7465 7874 2d75 6e64 6572 6c69 6e65  l-text-underline
-00061370: 6429 3b74 6578 742d 7472 616e 7366 6f72  d);text-transfor
-00061380: 6d3a 7661 7228 2d2d 7269 6f2d 676c 6f62  m:var(--rio-glob
-00061390: 616c 2d74 6578 742d 616c 6c2d 6361 7073  al-text-all-caps
-000613a0: 297d 2e72 696f 2d63 6f64 652d 626c 6f63  )}.rio-code-bloc
-000613b0: 6b7b 706f 696e 7465 722d 6576 656e 7473  k{pointer-events
-000613c0: 3a61 7574 6f3b 6469 7370 6c61 793a 666c  :auto;display:fl
-000613d0: 6578 3b66 6c65 782d 6469 7265 6374 696f  ex;flex-directio
-000613e0: 6e3a 636f 6c75 6d6e 3b61 6c69 676e 2d69  n:column;align-i
-000613f0: 7465 6d73 3a73 7472 6574 6368 3b67 6170  tems:stretch;gap
-00061400: 3a2e 3572 656d 3b70 6164 6469 6e67 3a2e  :.5rem;padding:.
-00061410: 3572 656d 3b62 6163 6b67 726f 756e 643a  5rem;background:
-00061420: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00061430: 6267 2d76 6172 6961 6e74 293b 626f 7264  bg-variant);bord
-00061440: 6572 2d72 6164 6975 733a 7661 7228 2d2d  er-radius:var(--
-00061450: 7269 6f2d 676c 6f62 616c 2d63 6f72 6e65  rio-global-corne
-00061460: 722d 7261 6469 7573 2d73 6d61 6c6c 293b  r-radius-small);
-00061470: 626f 782d 7369 7a69 6e67 3a62 6f72 6465  box-sizing:borde
-00061480: 722d 626f 787d 2e72 696f 2d63 6f64 652d  r-box}.rio-code-
-00061490: 626c 6f63 6b2d 6865 6164 6572 7b64 6973  block-header{dis
-000614a0: 706c 6179 3a66 6c65 783b 666c 6578 2d64  play:flex;flex-d
-000614b0: 6972 6563 7469 6f6e 3a72 6f77 3b61 6c69  irection:row;ali
-000614c0: 676e 2d69 7465 6d73 3a63 656e 7465 723b  gn-items:center;
-000614d0: 6a75 7374 6966 792d 636f 6e74 656e 743a  justify-content:
-000614e0: 7370 6163 652d 6265 7477 6565 6e3b 6761  space-between;ga
-000614f0: 703a 3172 656d 3b63 6f6c 6f72 3a76 6172  p:1rem;color:var
-00061500: 282d 2d72 696f 2d6c 6f63 616c 2d74 6578  (--rio-local-tex
-00061510: 742d 636f 6c6f 7229 3b66 6f6e 742d 7369  t-color);font-si
-00061520: 7a65 3a2e 3872 656d 7d2e 7269 6f2d 636f  ze:.8rem}.rio-co
-00061530: 6465 2d62 6c6f 636b 2d6c 616e 6775 6167  de-block-languag
-00061540: 657b 666f 6e74 2d77 6569 6768 743a 3730  e{font-weight:70
-00061550: 303b 6f70 6163 6974 793a 2e34 7d2e 7269  0;opacity:.4}.ri
-00061560: 6f2d 636f 6465 2d62 6c6f 636b 2d63 6f70  o-code-block-cop
-00061570: 792d 6275 7474 6f6e 7b77 6964 7468 3a31  y-button{width:1
-00061580: 2e33 7265 6d3b 6865 6967 6874 3a31 2e33  .3rem;height:1.3
-00061590: 7265 6d3b 6375 7273 6f72 3a70 6f69 6e74  rem;cursor:point
-000615a0: 6572 3b62 6f72 6465 723a 6e6f 6e65 3b62  er;border:none;b
-000615b0: 6163 6b67 726f 756e 643a 6e6f 6e65 3b62  ackground:none;b
-000615c0: 6f72 6465 722d 7261 6469 7573 3a76 6172  order-radius:var
-000615d0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 636f  (--rio-global-co
-000615e0: 726e 6572 2d72 6164 6975 732d 736d 616c  rner-radius-smal
-000615f0: 6c29 3b6d 6172 6769 6e3a 303b 7061 6464  l);margin:0;padd
-00061600: 696e 673a 303b 6f70 6163 6974 793a 2e34  ing:0;opacity:.4
-00061610: 3b74 7261 6e73 6974 696f 6e3a 6f70 6163  ;transition:opac
-00061620: 6974 7920 2e32 7320 6561 7365 2d69 6e2d  ity .2s ease-in-
-00061630: 6f75 747d 2e72 696f 2d63 6f64 652d 626c  out}.rio-code-bl
-00061640: 6f63 6b2d 636f 7079 2d62 7574 746f 6e3a  ock-copy-button:
-00061650: 686f 7665 727b 636f 6c6f 723a 7661 7228  hover{color:var(
-00061660: 2d2d 7269 6f2d 6c6f 6361 6c2d 6c65 7665  --rio-local-leve
-00061670: 6c2d 322d 6267 293b 6f70 6163 6974 793a  l-2-bg);opacity:
-00061680: 317d 2e72 696f 2d63 6f64 652d 626c 6f63  1}.rio-code-bloc
-00061690: 6b3e 7072 657b 6d61 7267 696e 3a30 3b66  k>pre{margin:0;f
-000616a0: 6f6e 742d 7369 7a65 3a76 6172 282d 2d72  ont-size:var(--r
-000616b0: 696f 2d67 6c6f 6261 6c2d 7465 7874 2d66  io-global-text-f
-000616c0: 6f6e 742d 7369 7a65 293b 666f 6e74 2d66  ont-size);font-f
-000616d0: 616d 696c 793a 7661 7228 2d2d 7269 6f2d  amily:var(--rio-
-000616e0: 676c 6f62 616c 2d6d 6f6e 6f73 7061 6365  global-monospace
-000616f0: 2d66 6f6e 7429 2c6d 6f6e 6f73 7061 6365  -font),monospace
-00061700: 3b64 6973 706c 6179 3a62 6c6f 636b 7d2e  ;display:block}.
-00061710: 7269 6f2d 6c69 6e6b 7b70 6f69 6e74 6572  rio-link{pointer
-00061720: 2d65 7665 6e74 733a 6175 746f 3b63 7572  -events:auto;cur
-00061730: 736f 723a 706f 696e 7465 723b 6469 7370  sor:pointer;disp
-00061740: 6c61 793a 626c 6f63 6b7d 2e72 696f 2d74  lay:block}.rio-t
-00061750: 6578 742d 6c69 6e6b 7b63 6f6c 6f72 3a76  ext-link{color:v
-00061760: 6172 282d 2d72 696f 2d6c 6f63 616c 2d6c  ar(--rio-local-l
-00061770: 6576 656c 2d32 2d62 6729 3b64 6973 706c  evel-2-bg);displ
-00061780: 6179 3a66 6c65 783b 616c 6967 6e2d 6974  ay:flex;align-it
-00061790: 656d 733a 6365 6e74 6572 3b6a 7573 7469  ems:center;justi
-000617a0: 6679 2d63 6f6e 7465 6e74 3a63 656e 7465  fy-content:cente
-000617b0: 727d 2e72 696f 2d73 6372 6f6c 6c2d 636f  r}.rio-scroll-co
-000617c0: 6e74 6169 6e65 722c 2e72 696f 2d73 6372  ntainer,.rio-scr
-000617d0: 6f6c 6c2d 7461 7267 6574 7b70 6f69 6e74  oll-target{point
-000617e0: 6572 2d65 7665 6e74 733a 6175 746f 7d2e  er-events:auto}.
-000617f0: 7269 6f2d 7363 726f 6c6c 2d74 6172 6765  rio-scroll-targe
-00061800: 743e 2e72 696f 2d73 6372 6f6c 6c2d 7461  t>.rio-scroll-ta
-00061810: 7267 6574 2d75 726c 2d63 6f70 792d 6275  rget-url-copy-bu
-00061820: 7474 6f6e 7b64 6973 706c 6179 3a6e 6f6e  tton{display:non
-00061830: 657d 2e72 696f 2d73 6372 6f6c 6c2d 7461  e}.rio-scroll-ta
-00061840: 7267 6574 3e2e 7269 6f2d 7363 726f 6c6c  rget>.rio-scroll
-00061850: 2d74 6172 6765 742d 7572 6c2d 636f 7079  -target-url-copy
-00061860: 2d62 7574 746f 6e3e 2a7b 706f 7369 7469  -button>*{positi
-00061870: 6f6e 3a61 6273 6f6c 7574 653b 6375 7273  on:absolute;curs
-00061880: 6f72 3a70 6f69 6e74 6572 7d2e 7269 6f2d  or:pointer}.rio-
-00061890: 7363 726f 6c6c 2d74 6172 6765 743a 686f  scroll-target:ho
-000618a0: 7665 723e 2e72 696f 2d73 6372 6f6c 6c2d  ver>.rio-scroll-
-000618b0: 7461 7267 6574 2d75 726c 2d63 6f70 792d  target-url-copy-
-000618c0: 6275 7474 6f6e 7b64 6973 706c 6179 3a62  button{display:b
-000618d0: 6c6f 636b 7d2e 7269 6f2d 636f 6c6f 722d  lock}.rio-color-
-000618e0: 7069 636b 6572 7b70 6f69 6e74 6572 2d65  picker{pointer-e
-000618f0: 7665 6e74 733a 6e6f 6e65 3b64 6973 706c  vents:none;displ
-00061900: 6179 3a66 6c65 783b 666c 6578 2d64 6972  ay:flex;flex-dir
-00061910: 6563 7469 6f6e 3a63 6f6c 756d 6e3b 616c  ection:column;al
-00061920: 6967 6e2d 6974 656d 733a 7374 7265 7463  ign-items:stretc
-00061930: 687d 2e72 696f 2d63 6f6c 6f72 2d70 6963  h}.rio-color-pic
-00061940: 6b65 722d 636f 6c6f 722d 7371 7561 7265  ker-color-square
-00061950: 7b70 6f69 6e74 6572 2d65 7665 6e74 733a  {pointer-events:
-00061960: 6175 746f 3b70 6f73 6974 696f 6e3a 7265  auto;position:re
-00061970: 6c61 7469 7665 3b6d 696e 2d68 6569 6768  lative;min-heigh
-00061980: 743a 3672 656d 3b63 7572 736f 723a 6372  t:6rem;cursor:cr
-00061990: 6f73 7368 6169 723b 6d61 7267 696e 2d62  osshair;margin-b
-000619a0: 6f74 746f 6d3a 2e37 7265 6d3b 626f 7264  ottom:.7rem;bord
-000619b0: 6572 2d72 6164 6975 733a 7661 7228 2d2d  er-radius:var(--
-000619c0: 7269 6f2d 676c 6f62 616c 2d63 6f72 6e65  rio-global-corne
-000619d0: 722d 7261 6469 7573 2d73 6d61 6c6c 293b  r-radius-small);
-000619e0: 666c 6578 2d67 726f 773a 317d 2e72 696f  flex-grow:1}.rio
-000619f0: 2d63 6f6c 6f72 2d70 6963 6b65 722d 736c  -color-picker-sl
-00061a00: 6964 6572 2d6f 7574 6572 7b70 6f69 6e74  ider-outer{point
-00061a10: 6572 2d65 7665 6e74 733a 6175 746f 3b70  er-events:auto;p
-00061a20: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
-00061a30: 3b70 6164 6469 6e67 3a2e 3772 656d 2030  ;padding:.7rem 0
-00061a40: 7d2e 7269 6f2d 636f 6c6f 722d 736c 6964  }.rio-color-slid
-00061a50: 6572 2d69 6e6e 6572 7b68 6569 6768 743a  er-inner{height:
-00061a60: 2e39 7265 6d3b 6375 7273 6f72 3a63 726f  .9rem;cursor:cro
-00061a70: 7373 6861 6972 3b62 6f72 6465 722d 7261  sshair;border-ra
-00061a80: 6469 7573 3a39 3939 3939 7078 7d2e 7269  dius:99999px}.ri
-00061a90: 6f2d 636f 6c6f 722d 7069 636b 6572 2d6b  o-color-picker-k
-00061aa0: 6e6f 627b 706f 696e 7465 722d 6576 656e  nob{pointer-even
-00061ab0: 7473 3a6e 6f6e 653b 6375 7273 6f72 3a63  ts:none;cursor:c
-00061ac0: 726f 7373 6861 6972 3b77 6964 7468 3a31  rosshair;width:1
-00061ad0: 2e34 7265 6d3b 6865 6967 6874 3a31 2e34  .4rem;height:1.4
-00061ae0: 7265 6d3b 626f 7264 6572 2d72 6164 6975  rem;border-radiu
-00061af0: 733a 3530 253b 626f 7264 6572 3a2e 3272  s:50%;border:.2r
-00061b00: 656d 2073 6f6c 6964 2076 6172 282d 2d72  em solid var(--r
-00061b10: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
-00061b20: 6c6f 7229 3b70 6f73 6974 696f 6e3a 6162  lor);position:ab
-00061b30: 736f 6c75 7465 3b74 7261 6e73 666f 726d  solute;transform
-00061b40: 3a74 7261 6e73 6c61 7465 282d 3530 252c  :translate(-50%,
-00061b50: 2d35 3025 293b 626f 782d 7369 7a69 6e67  -50%);box-sizing
-00061b60: 3a62 6f72 6465 722d 626f 783b 6261 636b  :border-box;back
-00061b70: 6772 6f75 6e64 3a76 6172 282d 2d63 686f  ground:var(--cho
-00061b80: 7365 6e2d 636f 6c6f 722d 6f70 6171 7565  sen-color-opaque
-00061b90: 297d 2e72 696f 2d63 6f6c 6f72 2d70 6963  )}.rio-color-pic
-00061ba0: 6b65 722d 736c 6964 6572 2d6f 7574 6572  ker-slider-outer
-00061bb0: 3e2e 7269 6f2d 636f 6c6f 722d 7069 636b  >.rio-color-pick
-00061bc0: 6572 2d6b 6e6f 627b 746f 703a 3530 257d  er-knob{top:50%}
-00061bd0: 2e63 6f6c 6f72 2d73 6c69 6465 722d 6368  .color-slider-ch
-00061be0: 6563 6b65 7273 7b62 6f72 6465 722d 7261  eckers{border-ra
-00061bf0: 6469 7573 3a39 3939 3939 7078 7d2e 7269  dius:99999px}.ri
-00061c00: 6f2d 636f 6c6f 722d 7069 636b 6572 2d68  o-color-picker-h
-00061c10: 7565 2d62 6172 3e2e 7269 6f2d 636f 6c6f  ue-bar>.rio-colo
-00061c20: 722d 736c 6964 6572 2d69 6e6e 6572 7b62  r-slider-inner{b
-00061c30: 6163 6b67 726f 756e 643a 6c69 6e65 6172  ackground:linear
-00061c40: 2d67 7261 6469 656e 7428 746f 2072 6967  -gradient(to rig
-00061c50: 6874 2c72 6564 2c79 656c 6c6f 772c 6c69  ht,red,yellow,li
-00061c60: 6d65 2c61 7175 612c 626c 7565 2c6d 6167  me,aqua,blue,mag
-00061c70: 656e 7461 2c72 6564 297d 2e72 696f 2d63  enta,red)}.rio-c
-00061c80: 6f6c 6f72 2d70 6963 6b65 722d 6f70 6163  olor-picker-opac
-00061c90: 6974 792d 6261 723e 2e72 696f 2d63 6f6c  ity-bar>.rio-col
-00061ca0: 6f72 2d73 6c69 6465 722d 696e 6e65 723a  or-slider-inner:
-00061cb0: 6e6f 7428 2e72 696f 2d63 6865 636b 6572  not(.rio-checker
-00061cc0: 6564 297b 706f 7369 7469 6f6e 3a61 6273  ed){position:abs
-00061cd0: 6f6c 7574 653b 746f 703a 2e37 7265 6d3b  olute;top:.7rem;
-00061ce0: 6c65 6674 3a30 3b72 6967 6874 3a30 3b62  left:0;right:0;b
-00061cf0: 6f74 746f 6d3a 2e37 7265 6d3b 6261 636b  ottom:.7rem;back
-00061d00: 6772 6f75 6e64 3a6c 696e 6561 722d 6772  ground:linear-gr
-00061d10: 6164 6965 6e74 2874 6f20 7269 6768 742c  adient(to right,
-00061d20: 7472 616e 7370 6172 656e 742c 7661 7228  transparent,var(
-00061d30: 2d2d 6368 6f73 656e 2d63 6f6c 6f72 2d6f  --chosen-color-o
-00061d40: 7061 7175 6529 297d 2e72 696f 2d63 6f6c  paque))}.rio-col
-00061d50: 6f72 2d70 6963 6b65 722d 7265 7375 6c74  or-picker-result
-00061d60: 2d63 6f6e 7461 696e 6572 7b6d 6172 6769  -container{margi
-00061d70: 6e2d 746f 703a 2e35 7265 6d3b 6d61 7267  n-top:.5rem;marg
-00061d80: 696e 2d6c 6566 743a 6175 746f 3b6d 6172  in-left:auto;mar
-00061d90: 6769 6e2d 7269 6768 743a 6175 746f 3b64  gin-right:auto;d
-00061da0: 6973 706c 6179 3a66 6c65 783b 616c 6967  isplay:flex;alig
-00061db0: 6e2d 6974 656d 733a 6365 6e74 6572 3b67  n-items:center;g
-00061dc0: 6170 3a2e 3872 656d 7d2e 7269 6f2d 636f  ap:.8rem}.rio-co
-00061dd0: 6c6f 722d 7069 636b 6572 2d73 656c 6563  lor-picker-selec
-00061de0: 7465 642d 636f 6c6f 722d 6369 7263 6c65  ted-color-circle
-00061df0: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
-00061e00: 7665 3b77 6964 7468 3a32 2e35 7265 6d3b  ve;width:2.5rem;
-00061e10: 6865 6967 6874 3a32 2e35 7265 6d7d 2e72  height:2.5rem}.r
-00061e20: 696f 2d63 6f6c 6f72 2d70 6963 6b65 722d  io-color-picker-
-00061e30: 7365 6c65 6374 6564 2d63 6f6c 6f72 2d63  selected-color-c
-00061e40: 6972 636c 653e 2a7b 7769 6474 683a 3130  ircle>*{width:10
-00061e50: 3025 3b68 6569 6768 743a 3130 3025 3b62  0%;height:100%;b
-00061e60: 6f72 6465 722d 7261 6469 7573 3a35 3025  order-radius:50%
-00061e70: 3b62 6f78 2d73 697a 696e 673a 626f 7264  ;box-sizing:bord
-00061e80: 6572 2d62 6f78 3b62 6f72 6465 723a 2e32  er-box;border:.2
-00061e90: 7265 6d20 736f 6c69 6420 7661 7228 2d2d  rem solid var(--
-00061ea0: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d63  rio-local-text-c
-00061eb0: 6f6c 6f72 297d 2e72 696f 2d63 6f6c 6f72  olor)}.rio-color
-00061ec0: 2d70 6963 6b65 722d 7365 6c65 6374 6564  -picker-selected
-00061ed0: 2d63 6f6c 6f72 2d63 6972 636c 653e 6469  -color-circle>di
-00061ee0: 763a 6669 7273 742d 6368 696c 647b 706f  v:first-child{po
-00061ef0: 7369 7469 6f6e 3a61 6273 6f6c 7574 653b  sition:absolute;
-00061f00: 746f 703a 303b 6c65 6674 3a30 3b72 6967  top:0;left:0;rig
-00061f10: 6874 3a30 3b62 6f74 746f 6d3a 303b 6261  ht:0;bottom:0;ba
-00061f20: 636b 6772 6f75 6e64 3a76 6172 282d 2d63  ckground:var(--c
-00061f30: 686f 7365 6e2d 636f 6c6f 722d 7472 616e  hosen-color-tran
-00061f40: 7370 6172 656e 7429 7d2e 7269 6f2d 636f  sparent)}.rio-co
-00061f50: 6c6f 722d 7069 636b 6572 2d73 656c 6563  lor-picker-selec
-00061f60: 7465 642d 636f 6c6f 722d 6369 7263 6c65  ted-color-circle
-00061f70: 2d63 6f6c 6f72 7b62 6163 6b67 726f 756e  -color{backgroun
-00061f80: 643a 7661 7228 2d2d 6368 6f73 656e 2d63  d:var(--chosen-c
-00061f90: 6f6c 6f72 2d74 7261 6e73 7061 7265 6e74  olor-transparent
-00061fa0: 297d 2e72 696f 2d63 6f6c 6f72 2d70 6963  )}.rio-color-pic
-00061fb0: 6b65 722d 7365 6c65 6374 6564 2d63 6f6c  ker-selected-col
-00061fc0: 6f72 2d6c 6162 656c 7b70 6f69 6e74 6572  or-label{pointer
-00061fd0: 2d65 7665 6e74 733a 6175 746f 3b6f 7061  -events:auto;opa
-00061fe0: 6369 7479 3a2e 353b 7769 6474 683a 3572  city:.5;width:5r
-00061ff0: 656d 3b63 6f6c 6f72 3a76 6172 282d 2d72  em;color:var(--r
-00062000: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
-00062010: 6c6f 7229 3b66 6f6e 742d 7369 7a65 3a2e  lor);font-size:.
-00062020: 3972 656d 3b74 6578 742d 616c 6967 6e3a  9rem;text-align:
-00062030: 6365 6e74 6572 3b66 6f6e 742d 7765 6967  center;font-weig
-00062040: 6874 3a37 3030 3b62 6163 6b67 726f 756e  ht:700;backgroun
-00062050: 643a 7472 616e 7370 6172 656e 743b 626f  d:transparent;bo
-00062060: 7264 6572 3a6e 6f6e 653b 7061 6464 696e  rder:none;paddin
-00062070: 673a 2e33 7265 6d3b 626f 7264 6572 2d72  g:.3rem;border-r
-00062080: 6164 6975 733a 2e35 7265 6d3b 7472 616e  adius:.5rem;tran
-00062090: 7369 7469 6f6e 3a6f 7061 6369 7479 202e  sition:opacity .
-000620a0: 3173 2065 6173 652d 696e 2d6f 7574 2c63  1s ease-in-out,c
-000620b0: 6f6c 6f72 202e 3173 2065 6173 652d 696e  olor .1s ease-in
-000620c0: 2d6f 7574 2c62 6163 6b67 726f 756e 642d  -out,background-
-000620d0: 636f 6c6f 7220 2e31 7320 6561 7365 2d69  color .1s ease-i
-000620e0: 6e2d 6f75 747d 2e72 696f 2d63 6f6c 6f72  n-out}.rio-color
-000620f0: 2d70 6963 6b65 722d 7365 6c65 6374 6564  -picker-selected
-00062100: 2d63 6f6c 6f72 2d6c 6162 656c 3a66 6f63  -color-label:foc
-00062110: 7573 7b6f 7574 6c69 6e65 3a6e 6f6e 653b  us{outline:none;
-00062120: 6f70 6163 6974 793a 313b 636f 6c6f 723a  opacity:1;color:
-00062130: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00062140: 6c65 7665 6c2d 322d 6267 293b 6261 636b  level-2-bg);back
-00062150: 6772 6f75 6e64 3a76 6172 282d 2d72 696f  ground:var(--rio
-00062160: 2d6c 6f63 616c 2d62 672d 7661 7269 616e  -local-bg-varian
-00062170: 7429 7d2e 7269 6f2d 6368 6563 6b65 7265  t)}.rio-checkere
-00062180: 647b 2d2d 6368 6563 6b65 722d 636f 6c6f  d{--checker-colo
-00062190: 723a 2023 3838 383b 2d2d 6368 6563 6b65  r: #888;--checke
-000621a0: 722d 7369 7a65 3a20 2e39 7265 6d3b 6261  r-size: .9rem;ba
-000621b0: 636b 6772 6f75 6e64 2d69 6d61 6765 3a6c  ckground-image:l
-000621c0: 696e 6561 722d 6772 6164 6965 6e74 2834  inear-gradient(4
-000621d0: 3564 6567 2c76 6172 282d 2d63 6865 636b  5deg,var(--check
-000621e0: 6572 2d63 6f6c 6f72 2920 3235 252c 7472  er-color) 25%,tr
-000621f0: 616e 7370 6172 656e 7420 3235 2529 2c6c  ansparent 25%),l
-00062200: 696e 6561 722d 6772 6164 6965 6e74 2834  inear-gradient(4
-00062210: 3564 6567 2c74 7261 6e73 7061 7265 6e74  5deg,transparent
-00062220: 2037 3525 2c76 6172 282d 2d63 6865 636b   75%,var(--check
-00062230: 6572 2d63 6f6c 6f72 2920 3735 2529 2c6c  er-color) 75%),l
-00062240: 696e 6561 722d 6772 6164 6965 6e74 2834  inear-gradient(4
-00062250: 3564 6567 2c74 7261 6e73 7061 7265 6e74  5deg,transparent
-00062260: 2037 3525 2c76 6172 282d 2d63 6865 636b   75%,var(--check
-00062270: 6572 2d63 6f6c 6f72 2920 3735 2529 2c6c  er-color) 75%),l
-00062280: 696e 6561 722d 6772 6164 6965 6e74 2834  inear-gradient(4
-00062290: 3564 6567 2c76 6172 282d 2d63 6865 636b  5deg,var(--check
-000622a0: 6572 2d63 6f6c 6f72 2920 3235 252c 7472  er-color) 25%,tr
-000622b0: 616e 7370 6172 656e 7420 3235 2529 3b62  ansparent 25%);b
-000622c0: 6163 6b67 726f 756e 642d 7369 7a65 3a76  ackground-size:v
-000622d0: 6172 282d 2d63 6865 636b 6572 2d73 697a  ar(--checker-siz
-000622e0: 6529 2076 6172 282d 2d63 6865 636b 6572  e) var(--checker
-000622f0: 2d73 697a 6529 3b62 6163 6b67 726f 756e  -size);backgroun
-00062300: 642d 706f 7369 7469 6f6e 3a30 2030 2c30  d-position:0 0,0
-00062310: 2030 2c63 616c 6328 7661 7228 2d2d 6368   0,calc(var(--ch
-00062320: 6563 6b65 722d 7369 7a65 2920 2a20 2d2e  ecker-size) * -.
-00062330: 3529 2063 616c 6328 7661 7228 2d2d 6368  5) calc(var(--ch
-00062340: 6563 6b65 722d 7369 7a65 2920 2a20 2d2e  ecker-size) * -.
-00062350: 3529 2c63 616c 6328 7661 7228 2d2d 6368  5),calc(var(--ch
-00062360: 6563 6b65 722d 7369 7a65 2920 2a20 2e35  ecker-size) * .5
-00062370: 2920 6361 6c63 2876 6172 282d 2d63 6865  ) calc(var(--che
-00062380: 636b 6572 2d73 697a 6529 202a 202e 3529  cker-size) * .5)
-00062390: 7d2e 7269 6f2d 6472 6177 6572 7b70 6f69  }.rio-drawer{poi
-000623a0: 6e74 6572 2d65 7665 6e74 733a 6175 746f  nter-events:auto
-000623b0: 3b6f 7665 7266 6c6f 773a 6869 6464 656e  ;overflow:hidden
-000623c0: 3b64 6973 706c 6179 3a66 6c65 783b 616c  ;display:flex;al
-000623d0: 6967 6e2d 6974 656d 733a 7374 7265 7463  ign-items:stretc
-000623e0: 687d 2e72 696f 2d64 7261 7765 722d 7368  h}.rio-drawer-sh
-000623f0: 6164 657b 706f 696e 7465 722d 6576 656e  ade{pointer-even
-00062400: 7473 3a6e 6f6e 653b 706f 7369 7469 6f6e  ts:none;position
-00062410: 3a61 6273 6f6c 7574 653b 6c65 6674 3a30  :absolute;left:0
-00062420: 3b74 6f70 3a30 3b72 6967 6874 3a30 3b62  ;top:0;right:0;b
-00062430: 6f74 746f 6d3a 303b 7472 616e 7369 7469  ottom:0;transiti
-00062440: 6f6e 3a62 6163 6b67 726f 756e 642d 636f  on:background-co
-00062450: 6c6f 7220 2e35 7320 6561 7365 2d69 6e2d  lor .5s ease-in-
-00062460: 6f75 747d 2e72 696f 2d64 7261 7765 722d  out}.rio-drawer-
-00062470: 616e 6368 6f72 7b70 6f69 6e74 6572 2d65  anchor{pointer-e
-00062480: 7665 6e74 733a 6e6f 6e65 3b66 6c65 782d  vents:none;flex-
-00062490: 6772 6f77 3a31 7d2e 7269 6f2d 6472 6177  grow:1}.rio-draw
-000624a0: 6572 2d63 6f6e 7465 6e74 2d6f 7574 6572  er-content-outer
-000624b0: 7b70 6f69 6e74 6572 2d65 7665 6e74 733a  {pointer-events:
-000624c0: 6175 746f 3b64 6973 706c 6179 3a66 6c65  auto;display:fle
-000624d0: 783b 706f 7369 7469 6f6e 3a61 6273 6f6c  x;position:absol
-000624e0: 7574 653b 6261 636b 6772 6f75 6e64 2d63  ute;background-c
-000624f0: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d67  olor:var(--rio-g
-00062500: 6c6f 6261 6c2d 6e65 7574 7261 6c2d 6267  lobal-neutral-bg
-00062510: 293b 626f 782d 7368 6164 6f77 3a30 2030  );box-shadow:0 0
-00062520: 2031 7265 6d20 7661 7228 2d2d 7269 6f2d   1rem var(--rio-
-00062530: 676c 6f62 616c 2d73 6861 646f 772d 636f  global-shadow-co
-00062540: 6c6f 7229 3b74 7261 6e73 6974 696f 6e3a  lor);transition:
-00062550: 7472 616e 7366 6f72 6d20 2e35 7320 6561  transform .5s ea
-00062560: 7365 2d6f 7574 7d2e 7269 6f2d 6472 6177  se-out}.rio-draw
-00062570: 6572 2d63 6f6e 7465 6e74 2d69 6e6e 6572  er-content-inner
-00062580: 7b6f 7264 6572 3a31 7d2e 7269 6f2d 6472  {order:1}.rio-dr
-00062590: 6177 6572 2d63 6f6e 7465 6e74 2d69 6e6e  awer-content-inn
-000625a0: 6572 3e2a 7b70 6f73 6974 696f 6e3a 7265  er>*{position:re
-000625b0: 6c61 7469 7665 2169 6d70 6f72 7461 6e74  lative!important
-000625c0: 7d2e 7269 6f2d 6472 6177 6572 2d6b 6e6f  }.rio-drawer-kno
-000625d0: 627b 616c 6967 6e2d 7365 6c66 3a63 656e  b{align-self:cen
-000625e0: 7465 723b 6d61 7267 696e 3a2e 3572 656d  ter;margin:.5rem
-000625f0: 3b62 6f72 6465 722d 7261 6469 7573 3a39  ;border-radius:9
-00062600: 3939 3939 7078 3b62 6163 6b67 726f 756e  9999px;backgroun
-00062610: 643a 7661 7228 2d2d 7269 6f2d 6c6f 6361  d:var(--rio-loca
-00062620: 6c2d 7465 7874 2d63 6f6c 6f72 293b 6f70  l-text-color);op
-00062630: 6163 6974 793a 2e31 357d 2e72 696f 2d64  acity:.15}.rio-d
-00062640: 7261 7765 722d 6c65 6674 202e 7269 6f2d  rawer-left .rio-
-00062650: 6472 6177 6572 2d6b 6e6f 622c 2e72 696f  drawer-knob,.rio
-00062660: 2d64 7261 7765 722d 7269 6768 7420 2e72  -drawer-right .r
-00062670: 696f 2d64 7261 7765 722d 6b6e 6f62 7b77  io-drawer-knob{w
-00062680: 6964 7468 3a2e 3472 656d 3b68 6569 6768  idth:.4rem;heigh
-00062690: 743a 3472 656d 7d2e 7269 6f2d 6472 6177  t:4rem}.rio-draw
-000626a0: 6572 2d74 6f70 202e 7269 6f2d 6472 6177  er-top .rio-draw
-000626b0: 6572 2d6b 6e6f 622c 2e72 696f 2d64 7261  er-knob,.rio-dra
-000626c0: 7765 722d 626f 7474 6f6d 202e 7269 6f2d  wer-bottom .rio-
-000626d0: 6472 6177 6572 2d6b 6e6f 627b 7769 6474  drawer-knob{widt
-000626e0: 683a 3472 656d 3b68 6569 6768 743a 2e34  h:4rem;height:.4
-000626f0: 7265 6d7d 2e72 696f 2d64 7261 7765 722d  rem}.rio-drawer-
-00062700: 746f 7020 2e72 696f 2d64 7261 7765 722d  top .rio-drawer-
-00062710: 636f 6e74 656e 742d 6f75 7465 722c 2e72  content-outer,.r
-00062720: 696f 2d64 7261 7765 722d 626f 7474 6f6d  io-drawer-bottom
-00062730: 202e 7269 6f2d 6472 6177 6572 2d63 6f6e   .rio-drawer-con
-00062740: 7465 6e74 2d6f 7574 6572 7b66 6c65 782d  tent-outer{flex-
-00062750: 6469 7265 6374 696f 6e3a 636f 6c75 6d6e  direction:column
-00062760: 7d2e 7269 6f2d 6472 6177 6572 2d6c 6566  }.rio-drawer-lef
-00062770: 7420 2e72 696f 2d64 7261 7765 722d 6b6e  t .rio-drawer-kn
-00062780: 6f62 2c2e 7269 6f2d 6472 6177 6572 2d74  ob,.rio-drawer-t
-00062790: 6f70 202e 7269 6f2d 6472 6177 6572 2d6b  op .rio-drawer-k
-000627a0: 6e6f 627b 6f72 6465 723a 327d 2e72 696f  nob{order:2}.rio
-000627b0: 2d64 7261 7765 722d 7269 6768 7420 2e72  -drawer-right .r
-000627c0: 696f 2d64 7261 7765 722d 6b6e 6f62 2c2e  io-drawer-knob,.
-000627d0: 7269 6f2d 6472 6177 6572 2d62 6f74 746f  rio-drawer-botto
-000627e0: 6d20 2e72 696f 2d64 7261 7765 722d 6b6e  m .rio-drawer-kn
-000627f0: 6f62 7b6f 7264 6572 3a30 7d2e 7269 6f2d  ob{order:0}.rio-
-00062800: 6472 6177 6572 2d6c 6566 743e 2e72 696f  drawer-left>.rio
-00062810: 2d64 7261 7765 722d 636f 6e74 656e 742d  -drawer-content-
-00062820: 6f75 7465 727b 746f 703a 303b 6c65 6674  outer{top:0;left
-00062830: 3a30 3b62 6f74 746f 6d3a 303b 7769 6474  :0;bottom:0;widt
-00062840: 683a 6669 742d 636f 6e74 656e 743b 626f  h:fit-content;bo
-00062850: 7264 6572 2d72 6164 6975 733a 3020 7661  rder-radius:0 va
-00062860: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d63  r(--rio-global-c
-00062870: 6f72 6e65 722d 7261 6469 7573 2d6c 6172  orner-radius-lar
-00062880: 6765 2920 7661 7228 2d2d 7269 6f2d 676c  ge) var(--rio-gl
-00062890: 6f62 616c 2d63 6f72 6e65 722d 7261 6469  obal-corner-radi
-000628a0: 7573 2d6c 6172 6765 2920 307d 2e72 696f  us-large) 0}.rio
-000628b0: 2d64 7261 7765 722d 7269 6768 743e 2e72  -drawer-right>.r
-000628c0: 696f 2d64 7261 7765 722d 636f 6e74 656e  io-drawer-conten
-000628d0: 742d 6f75 7465 727b 746f 703a 303b 7269  t-outer{top:0;ri
-000628e0: 6768 743a 303b 626f 7474 6f6d 3a30 3b77  ght:0;bottom:0;w
-000628f0: 6964 7468 3a66 6974 2d63 6f6e 7465 6e74  idth:fit-content
-00062900: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
-00062910: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00062920: 636f 726e 6572 2d72 6164 6975 732d 6c61  corner-radius-la
-00062930: 7267 6529 2030 2030 2076 6172 282d 2d72  rge) 0 0 var(--r
-00062940: 696f 2d67 6c6f 6261 6c2d 636f 726e 6572  io-global-corner
-00062950: 2d72 6164 6975 732d 6c61 7267 6529 7d2e  -radius-large)}.
-00062960: 7269 6f2d 6472 6177 6572 2d74 6f70 3e2e  rio-drawer-top>.
-00062970: 7269 6f2d 6472 6177 6572 2d63 6f6e 7465  rio-drawer-conte
-00062980: 6e74 2d6f 7574 6572 7b6c 6566 743a 303b  nt-outer{left:0;
-00062990: 746f 703a 303b 7269 6768 743a 303b 6865  top:0;right:0;he
-000629a0: 6967 6874 3a66 6974 2d63 6f6e 7465 6e74  ight:fit-content
-000629b0: 3b62 6f72 6465 722d 7261 6469 7573 3a30  ;border-radius:0
-000629c0: 2030 2076 6172 282d 2d72 696f 2d67 6c6f   0 var(--rio-glo
-000629d0: 6261 6c2d 636f 726e 6572 2d72 6164 6975  bal-corner-radiu
-000629e0: 732d 6c61 7267 6529 2076 6172 282d 2d72  s-large) var(--r
-000629f0: 696f 2d67 6c6f 6261 6c2d 636f 726e 6572  io-global-corner
-00062a00: 2d72 6164 6975 732d 6c61 7267 6529 7d2e  -radius-large)}.
-00062a10: 7269 6f2d 6472 6177 6572 2d62 6f74 746f  rio-drawer-botto
-00062a20: 6d3e 2e72 696f 2d64 7261 7765 722d 636f  m>.rio-drawer-co
-00062a30: 6e74 656e 742d 6f75 7465 727b 6c65 6674  ntent-outer{left
-00062a40: 3a30 3b62 6f74 746f 6d3a 303b 7269 6768  :0;bottom:0;righ
-00062a50: 743a 303b 6865 6967 6874 3a66 6974 2d63  t:0;height:fit-c
-00062a60: 6f6e 7465 6e74 3b62 6f72 6465 722d 7261  ontent;border-ra
-00062a70: 6469 7573 3a76 6172 282d 2d72 696f 2d67  dius:var(--rio-g
-00062a80: 6c6f 6261 6c2d 636f 726e 6572 2d72 6164  lobal-corner-rad
-00062a90: 6975 732d 6c61 7267 6529 2076 6172 282d  ius-large) var(-
-00062aa0: 2d72 696f 2d67 6c6f 6261 6c2d 636f 726e  -rio-global-corn
-00062ab0: 6572 2d72 6164 6975 732d 6c61 7267 6529  er-radius-large)
-00062ac0: 2030 2030 7d2e 7269 6f2d 6472 6177 6572   0 0}.rio-drawer
-00062ad0: 2d6e 6f2d 7472 616e 7369 7469 6f6e 7b74  -no-transition{t
-00062ae0: 7261 6e73 6974 696f 6e3a 6e6f 6e65 2169  ransition:none!i
-00062af0: 6d70 6f72 7461 6e74 7d2e 7269 6f2d 6472  mportant}.rio-dr
-00062b00: 6177 6572 2d6e 6f2d 7472 616e 7369 7469  awer-no-transiti
-00062b10: 6f6e 3e2a 7b74 7261 6e73 6974 696f 6e3a  on>*{transition:
-00062b20: 6e6f 6e65 2169 6d70 6f72 7461 6e74 7d2e  none!important}.
-00062b30: 7269 6f2d 706f 7075 707b 7a2d 696e 6465  rio-popup{z-inde
-00062b40: 783a 3130 3030 337d 2e72 696f 2d70 6f70  x:10003}.rio-pop
-00062b50: 7570 2d61 6e63 686f 723e 2a2c 2e72 696f  up-anchor>*,.rio
-00062b60: 2d70 6f70 7570 2d63 6f6e 7465 6e74 3e2a  -popup-content>*
-00062b70: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
-00062b80: 7665 2169 6d70 6f72 7461 6e74 7d2e 7269  ve!important}.ri
-00062b90: 6f2d 706f 7075 702d 636f 6e74 656e 747b  o-popup-content{
-00062ba0: 706f 7369 7469 6f6e 3a66 6978 6564 3b77  position:fixed;w
-00062bb0: 6964 7468 3a6d 696e 2d63 6f6e 7465 6e74  idth:min-content
-00062bc0: 3b68 6569 6768 743a 6d69 6e2d 636f 6e74  ;height:min-cont
-00062bd0: 656e 743b 6261 636b 6772 6f75 6e64 2d63  ent;background-c
-00062be0: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
-00062bf0: 6f63 616c 2d62 6729 3b62 6f72 6465 722d  ocal-bg);border-
-00062c00: 7261 6469 7573 3a76 6172 282d 2d72 696f  radius:var(--rio
-00062c10: 2d67 6c6f 6261 6c2d 636f 726e 6572 2d72  -global-corner-r
-00062c20: 6164 6975 732d 6d65 6469 756d 293b 626f  adius-medium);bo
-00062c30: 782d 7368 6164 6f77 3a30 2030 2031 7265  x-shadow:0 0 1re
-00062c40: 6d20 7661 7228 2d2d 7269 6f2d 676c 6f62  m var(--rio-glob
-00062c50: 616c 2d73 6861 646f 772d 636f 6c6f 7229  al-shadow-color)
-00062c60: 3b74 7261 6e73 666f 726d 3a73 6361 6c65  ;transform:scale
-00062c70: 2830 293b 6f70 6163 6974 793a 303b 7472  (0);opacity:0;tr
-00062c80: 616e 7369 7469 6f6e 3a74 7261 6e73 666f  ansition:transfo
-00062c90: 726d 202e 3273 206c 696e 6561 722c 6f70  rm .2s linear,op
-00062ca0: 6163 6974 7920 2e31 7320 6561 7365 2d69  acity .1s ease-i
-00062cb0: 6e2d 6f75 747d 2e72 696f 2d70 6f70 7570  n-out}.rio-popup
-00062cc0: 2d6f 7065 6e3e 2e72 696f 2d70 6f70 7570  -open>.rio-popup
-00062cd0: 2d63 6f6e 7465 6e74 7b74 7261 6e73 666f  -content{transfo
-00062ce0: 726d 3a73 6361 6c65 2831 293b 6f70 6163  rm:scale(1);opac
-00062cf0: 6974 793a 313b 7472 616e 7369 7469 6f6e  ity:1;transition
-00062d00: 3a74 7261 6e73 666f 726d 202e 3273 2063  :transform .2s c
-00062d10: 7562 6963 2d62 657a 6965 7228 2e35 2c2e  ubic-bezier(.5,.
-00062d20: 352c 2e32 2c31 2e31 3429 2c6f 7061 6369  5,.2,1.14),opaci
-00062d30: 7479 202e 3173 2065 6173 652d 696e 2d6f  ty .1s ease-in-o
-00062d40: 7574 7d2e 7269 6f2d 696d 6167 657b 706f  ut}.rio-image{po
-00062d50: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
-00062d60: 6f3b 6469 7370 6c61 793a 666c 6578 3b6a  o;display:flex;j
-00062d70: 7573 7469 6679 2d63 6f6e 7465 6e74 3a63  ustify-content:c
-00062d80: 656e 7465 723b 616c 6967 6e2d 6974 656d  enter;align-item
-00062d90: 733a 6365 6e74 6572 7d2e 7269 6f2d 696d  s:center}.rio-im
-00062da0: 6167 6520 696d 677b 7769 6474 683a 3130  age img{width:10
-00062db0: 3025 3b68 6569 6768 743a 3130 3025 3b6f  0%;height:100%;o
-00062dc0: 626a 6563 742d 6669 743a 636f 6e74 6169  bject-fit:contai
-00062dd0: 6e7d 2e72 696f 2d69 6d61 6765 2073 7667  n}.rio-image svg
-00062de0: 7b6d 6178 2d77 6964 7468 3a33 7265 6d7d  {max-width:3rem}
-00062df0: 2e72 696f 2d63 6172 647b 706f 696e 7465  .rio-card{pointe
-00062e00: 722d 6576 656e 7473 3a61 7574 6f3b 6261  r-events:auto;ba
-00062e10: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-00062e20: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
-00062e30: 6729 3b62 6f78 2d73 6861 646f 773a 3020  g);box-shadow:0 
-00062e40: 3020 3020 7661 7228 2d2d 7269 6f2d 676c  0 0 var(--rio-gl
-00062e50: 6f62 616c 2d73 6861 646f 772d 636f 6c6f  obal-shadow-colo
-00062e60: 7229 3b74 7261 6e73 6974 696f 6e3a 626f  r);transition:bo
-00062e70: 782d 7368 6164 6f77 202e 3135 7320 6561  x-shadow .15s ea
-00062e80: 7365 2d6f 7574 2c62 6163 6b67 726f 756e  se-out,backgroun
-00062e90: 642d 636f 6c6f 7220 2e31 7320 6561 7365  d-color .1s ease
-00062ea0: 2d6f 7574 7d2e 7269 6f2d 6361 7264 2d65  -out}.rio-card-e
-00062eb0: 6c65 7661 7465 2d6f 6e2d 686f 7665 723a  levate-on-hover:
-00062ec0: 686f 7665 727b 626f 782d 7368 6164 6f77  hover{box-shadow
-00062ed0: 3a30 202e 3135 7265 6d20 2e33 7265 6d20  :0 .15rem .3rem 
-00062ee0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00062ef0: 2d73 6861 646f 772d 636f 6c6f 7229 7d2e  -shadow-color)}.
-00062f00: 7269 6f2d 6361 7264 2d63 6f6c 6f72 697a  rio-card-coloriz
-00062f10: 652d 6f6e 2d68 6f76 6572 3a68 6f76 6572  e-on-hover:hover
-00062f20: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
-00062f30: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
-00062f40: 6c2d 6267 2d61 6374 6976 6529 7d2e 7269  l-bg-active)}.ri
-00062f50: 6f2d 6361 7264 2d72 6970 706c 657b 6f76  o-card-ripple{ov
-00062f60: 6572 666c 6f77 3a68 6964 6465 6e7d 2e72  erflow:hidden}.r
-00062f70: 696f 2d73 7769 7463 6865 722d 6261 727b  io-switcher-bar{
-00062f80: 6469 7370 6c61 793a 666c 6578 3b61 6c69  display:flex;ali
-00062f90: 676e 2d69 7465 6d73 3a63 656e 7465 727d  gn-items:center}
-00062fa0: 2e72 696f 2d73 7769 7463 6865 722d 6261  .rio-switcher-ba
-00062fb0: 723e 6469 767b 706f 7369 7469 6f6e 3a72  r>div{position:r
-00062fc0: 656c 6174 6976 657d 2e72 696f 2d73 7769  elative}.rio-swi
-00062fd0: 7463 6865 722d 6261 723e 6469 763e 2e72  tcher-bar>div>.r
-00062fe0: 696f 2d73 7769 7463 6865 722d 6261 722d  io-switcher-bar-
-00062ff0: 6f70 7469 6f6e 737b 706f 7369 7469 6f6e  options{position
-00063000: 3a72 656c 6174 6976 6521 696d 706f 7274  :relative!import
-00063010: 616e 747d 2e72 696f 2d73 7769 7463 6865  ant}.rio-switche
-00063020: 722d 6261 722d 6f70 7469 6f6e 737b 706f  r-bar-options{po
-00063030: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
-00063040: 6f3b 706f 7369 7469 6f6e 3a61 6273 6f6c  o;position:absol
-00063050: 7574 653b 6469 7370 6c61 793a 666c 6578  ute;display:flex
-00063060: 3b61 6c69 676e 2d69 7465 6d73 3a73 7472  ;align-items:str
-00063070: 6574 6368 3b6a 7573 7469 6679 2d63 6f6e  etch;justify-con
-00063080: 7465 6e74 3a73 7061 6365 2d62 6574 7765  tent:space-betwe
-00063090: 656e 7d2e 7269 6f2d 7377 6974 6368 6572  en}.rio-switcher
-000630a0: 2d62 6172 2d6f 7074 696f 6e7b 6469 7370  -bar-option{disp
-000630b0: 6c61 793a 666c 6578 3b66 6c65 782d 6469  lay:flex;flex-di
-000630c0: 7265 6374 696f 6e3a 636f 6c75 6d6e 3b61  rection:column;a
-000630d0: 6c69 676e 2d69 7465 6d73 3a63 656e 7465  lign-items:cente
-000630e0: 723b 6a75 7374 6966 792d 636f 6e74 656e  r;justify-conten
-000630f0: 743a 7370 6163 652d 6265 7477 6565 6e3b  t:space-between;
-00063100: 6375 7273 6f72 3a70 6f69 6e74 6572 3b62  cursor:pointer;b
-00063110: 6f72 6465 722d 7261 6469 7573 3a76 6172  order-radius:var
-00063120: 282d 2d72 696f 2d67 6c6f 6261 6c2d 636f  (--rio-global-co
-00063130: 726e 6572 2d72 6164 6975 732d 6c61 7267  rner-radius-larg
-00063140: 6529 3b63 6f6c 6f72 3a76 6172 282d 2d72  e);color:var(--r
-00063150: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
-00063160: 6c6f 7229 3b74 7261 6e73 6974 696f 6e3a  lor);transition:
-00063170: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00063180: 202e 3173 2065 6173 652d 6f75 747d 2e72   .1s ease-out}.r
-00063190: 696f 2d73 7769 7463 6865 722d 6261 722d  io-switcher-bar-
-000631a0: 6f70 7469 6f6e 3a68 6f76 6572 7b62 6163  option:hover{bac
-000631b0: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
-000631c0: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6267  r(--rio-local-bg
-000631d0: 2d61 6374 6976 6529 7d2e 7269 6f2d 7377  -active)}.rio-sw
-000631e0: 6974 6368 6572 2d62 6172 2d6d 6172 6b65  itcher-bar-marke
-000631f0: 723e 2e72 696f 2d73 7769 7463 6865 722d  r>.rio-switcher-
-00063200: 6261 722d 6f70 7469 6f6e 733e 2e72 696f  bar-options>.rio
-00063210: 2d73 7769 7463 6865 722d 6261 722d 6f70  -switcher-bar-op
-00063220: 7469 6f6e 7b62 6163 6b67 726f 756e 642d  tion{background-
-00063230: 636f 6c6f 723a 756e 7365 7421 696d 706f  color:unset!impo
-00063240: 7274 616e 747d 2e72 696f 2d73 7769 7463  rtant}.rio-switc
-00063250: 6865 722d 6261 722d 6f70 7469 6f6e 3e64  her-bar-option>d
-00063260: 6976 7b6d 6172 6769 6e2d 6c65 6674 3a61  iv{margin-left:a
-00063270: 7574 6f3b 6d61 7267 696e 2d72 6967 6874  uto;margin-right
-00063280: 3a61 7574 6f3b 7768 6974 652d 7370 6163  :auto;white-spac
-00063290: 653a 6e6f 7772 6170 7d2e 7269 6f2d 7377  e:nowrap}.rio-sw
-000632a0: 6974 6368 6572 2d62 6172 2d6d 6172 6b65  itcher-bar-marke
-000632b0: 727b 706f 696e 7465 722d 6576 656e 7473  r{pointer-events
-000632c0: 3a6e 6f6e 653b 6261 636b 6772 6f75 6e64  :none;background
-000632d0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
-000632e0: 2d62 6729 3b6f 7665 7266 6c6f 773a 6869  -bg);overflow:hi
-000632f0: 6464 656e 3b70 6f73 6974 696f 6e3a 6162  dden;position:ab
-00063300: 736f 6c75 7465 3b6c 6566 743a 303b 746f  solute;left:0;to
-00063310: 703a 303b 626f 7264 6572 2d72 6164 6975  p:0;border-radiu
-00063320: 733a 7661 7228 2d2d 7269 6f2d 676c 6f62  s:var(--rio-glob
-00063330: 616c 2d63 6f72 6e65 722d 7261 6469 7573  al-corner-radius
-00063340: 2d6c 6172 6765 297d 2e72 696f 2d74 6162  -large)}.rio-tab
-00063350: 6c65 7b70 6f69 6e74 6572 2d65 7665 6e74  le{pointer-event
-00063360: 733a 6175 746f 3b64 6973 706c 6179 3a67  s:auto;display:g
-00063370: 7269 647d 2e72 696f 2d74 6162 6c65 3e2a  rid}.rio-table>*
-00063380: 7b70 6164 6469 6e67 3a2e 3572 656d 202e  {padding:.5rem .
-00063390: 3872 656d 7d2e 7269 6f2d 7461 626c 6520  8rem}.rio-table 
-000633a0: 2e68 6561 6465 727b 6469 7370 6c61 793a  .header{display:
-000633b0: 666c 6578 3b63 7572 736f 723a 706f 696e  flex;cursor:poin
-000633c0: 7465 727d 2e72 696f 2d74 6162 6c65 202e  ter}.rio-table .
-000633d0: 6865 6164 6572 3a61 6674 6572 7b63 6f6e  header:after{con
-000633e0: 7465 6e74 3a22 e296 b422 3b64 6973 706c  tent:"...";displ
-000633f0: 6179 3a69 6e6c 696e 652d 626c 6f63 6b3b  ay:inline-block;
-00063400: 6d61 7267 696e 2d6c 6566 743a 2e33 7265  margin-left:.3re
-00063410: 6d3b 6f70 6163 6974 793a 307d 2e72 696f  m;opacity:0}.rio
-00063420: 2d74 6162 6c65 202e 6865 6164 6572 5b64  -table .header[d
-00063430: 6174 612d 736f 7274 3d61 7363 656e 6469  ata-sort=ascendi
-00063440: 6e67 5d3a 6166 7465 727b 636f 6e74 656e  ng]:after{conten
-00063450: 743a 22e2 96b4 223b 6f70 6163 6974 793a  t:"...";opacity:
-00063460: 317d 2e72 696f 2d74 6162 6c65 202e 6865  1}.rio-table .he
-00063470: 6164 6572 5b64 6174 612d 736f 7274 3d64  ader[data-sort=d
-00063480: 6573 6365 6e64 696e 675d 3a61 6674 6572  escending]:after
-00063490: 7b63 6f6e 7465 6e74 3a22 e296 be22 3b6f  {content:"...";o
-000634a0: 7061 6369 7479 3a31 7d2e 7269 6f2d 6c69  pacity:1}.rio-li
-000634b0: 7374 2d76 6965 777b 706f 696e 7465 722d  st-view{pointer-
-000634c0: 6576 656e 7473 3a6e 6f6e 653b 6469 7370  events:none;disp
-000634d0: 6c61 793a 666c 6578 3b66 6c65 782d 6469  lay:flex;flex-di
-000634e0: 7265 6374 696f 6e3a 636f 6c75 6d6e 3b61  rection:column;a
-000634f0: 6c69 676e 2d69 7465 6d73 3a73 7472 6574  lign-items:stret
-00063500: 6368 7d2e 7269 6f2d 6865 6164 696e 672d  ch}.rio-heading-
-00063510: 6c69 7374 2d69 7465 6d7b 706f 696e 7465  list-item{pointe
-00063520: 722d 6576 656e 7473 3a6e 6f6e 653b 626f  r-events:none;bo
-00063530: 782d 7369 7a69 6e67 3a62 6f72 6465 722d  x-sizing:border-
-00063540: 626f 787d 2e72 696f 2d6c 6973 7476 6965  box}.rio-listvie
-00063550: 772d 6772 6f75 7065 647b 706f 696e 7465  w-grouped{pointe
-00063560: 722d 6576 656e 7473 3a61 7574 6f3b 6261  r-events:auto;ba
-00063570: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-00063580: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
-00063590: 672d 7661 7269 616e 7429 3b74 7261 6e73  g-variant);trans
-000635a0: 6974 696f 6e3a 6261 636b 6772 6f75 6e64  ition:background
-000635b0: 2d63 6f6c 6f72 202e 3173 2065 6173 652d  -color .1s ease-
-000635c0: 6f75 747d 2e72 696f 2d6c 6973 7476 6965  out}.rio-listvie
-000635d0: 772d 6772 6f75 7065 642b 2e72 696f 2d6c  w-grouped+.rio-l
-000635e0: 6973 7476 6965 772d 6772 6f75 7065 643a  istview-grouped:
-000635f0: 6166 7465 727b 636f 6e74 656e 743a 2222  after{content:""
-00063600: 3b70 6f73 6974 696f 6e3a 6162 736f 6c75  ;position:absolu
-00063610: 7465 3b74 6f70 3a30 3b6c 6566 743a 303b  te;top:0;left:0;
-00063620: 7269 6768 743a 303b 6865 6967 6874 3a31  right:0;height:1
-00063630: 7078 3b62 6163 6b67 726f 756e 642d 636f  px;background-co
-00063640: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
-00063650: 6361 6c2d 7465 7874 2d63 6f6c 6f72 293b  cal-text-color);
-00063660: 6f70 6163 6974 793a 2e32 7d2e 7269 6f2d  opacity:.2}.rio-
-00063670: 6c69 7374 2d69 7465 6d2d 7269 7070 6c65  list-item-ripple
-00063680: 7b6f 7665 7266 6c6f 773a 6869 6464 656e  {overflow:hidden
-00063690: 7d2e 7269 6f2d 6c69 7374 2d69 7465 6d2d  }.rio-list-item-
-000636a0: 7269 7070 6c65 3a68 6f76 6572 7b62 6163  ripple:hover{bac
-000636b0: 6b67 726f 756e 643a 7661 7228 2d2d 7269  kground:var(--ri
-000636c0: 6f2d 6c6f 6361 6c2d 6267 2d61 6374 6976  o-local-bg-activ
-000636d0: 6529 7d2e 7269 6f2d 666c 6f77 2d63 6f6e  e)}.rio-flow-con
-000636e0: 7461 696e 6572 7b64 6973 706c 6179 3a66  tainer{display:f
-000636f0: 6c65 783b 666c 6578 2d77 7261 703a 7772  lex;flex-wrap:wr
-00063700: 6170 7d2e 7269 6f2d 666c 6f77 2d63 6f6e  ap}.rio-flow-con
-00063710: 7461 696e 6572 3e2a 7b74 7261 6e73 6974  tainer>*{transit
-00063720: 696f 6e3a 6c65 6674 202e 3273 2065 6173  ion:left .2s eas
-00063730: 652d 6f75 742c 746f 7020 2e32 7320 6561  e-out,top .2s ea
-00063740: 7365 2d6f 7574 7d2e 7269 6f2d 636f 6e6e  se-out}.rio-conn
-00063750: 6563 7469 6f6e 2d6c 6f73 742d 706f 7075  ection-lost-popu
-00063760: 707b 706f 696e 7465 722d 6576 656e 7473  p{pointer-events
-00063770: 3a6e 6f6e 653b 706f 7369 7469 6f6e 3a66  :none;position:f
-00063780: 6978 6564 3b6c 6566 743a 303b 746f 703a  ixed;left:0;top:
-00063790: 303b 7769 6474 683a 3130 3076 773b 6865  0;width:100vw;he
-000637a0: 6967 6874 3a31 3030 7668 3b7a 2d69 6e64  ight:100vh;z-ind
-000637b0: 6578 3a31 3030 3034 3b62 6163 6b67 726f  ex:10004;backgro
-000637c0: 756e 642d 636f 6c6f 723a 7472 616e 7370  und-color:transp
-000637d0: 6172 656e 743b 7472 616e 7369 7469 6f6e  arent;transition
-000637e0: 3a62 6163 6b67 726f 756e 642d 636f 6c6f  :background-colo
-000637f0: 7220 3173 2065 6173 652d 696e 2d6f 7574  r 1s ease-in-out
-00063800: 7d2e 7269 6f2d 636f 6e6e 6563 7469 6f6e  }.rio-connection
-00063810: 2d6c 6f73 742d 706f 7075 702e 7269 6f2d  -lost-popup.rio-
-00063820: 636f 6e6e 6563 7469 6f6e 2d6c 6f73 742d  connection-lost-
-00063830: 706f 7075 702d 7669 7369 626c 657b 6469  popup-visible{di
-00063840: 7370 6c61 793a 666c 6578 3b61 6c69 676e  splay:flex;align
-00063850: 2d69 7465 6d73 3a73 7472 6574 6368 3b62  -items:stretch;b
-00063860: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00063870: 2330 3030 3030 3038 307d 2e72 696f 2d63  #00000080}.rio-c
-00063880: 6f6e 6e65 6374 696f 6e2d 6c6f 7374 2d70  onnection-lost-p
-00063890: 6f70 7570 3e2a 7b70 6f73 6974 696f 6e3a  opup>*{position:
-000638a0: 6162 736f 6c75 7465 3b66 6c65 782d 6772  absolute;flex-gr
-000638b0: 6f77 3a31 3b6c 6566 743a 303b 746f 703a  ow:1;left:0;top:
-000638c0: 303b 7769 6474 683a 3130 3025 3b68 6569  0;width:100%;hei
-000638d0: 6768 743a 3130 3025 3b6f 7061 6369 7479  ght:100%;opacity
-000638e0: 3a30 3b74 7261 6e73 666f 726d 3a74 7261  :0;transform:tra
-000638f0: 6e73 6c61 7465 5928 2d35 7265 6d29 3b74  nslateY(-5rem);t
-00063900: 7261 6e73 6974 696f 6e3a 6f70 6163 6974  ransition:opacit
-00063910: 7920 2e33 7320 6561 7365 2d69 6e2d 6f75  y .3s ease-in-ou
-00063920: 742c 7472 616e 7366 6f72 6d20 2e33 7320  t,transform .3s 
-00063930: 6375 6269 632d 6265 7a69 6572 282e 352c  cubic-bezier(.5,
-00063940: 2e35 2c2e 322c 312e 3134 297d 2e72 696f  .5,.2,1.14)}.rio
-00063950: 2d63 6f6e 6e65 6374 696f 6e2d 6c6f 7374  -connection-lost
-00063960: 2d70 6f70 7570 2e72 696f 2d63 6f6e 6e65  -popup.rio-conne
-00063970: 6374 696f 6e2d 6c6f 7374 2d70 6f70 7570  ction-lost-popup
-00063980: 2d76 6973 6962 6c65 3e2a 7b6f 7061 6369  -visible>*{opaci
-00063990: 7479 3a31 3b74 7261 6e73 666f 726d 3a74  ty:1;transform:t
-000639a0: 7261 6e73 6c61 7465 5928 3029 7d2e 7269  ranslateY(0)}.ri
-000639b0: 6f2d 7472 6163 6562 6163 6b7b 706f 696e  o-traceback{poin
-000639c0: 7465 722d 6576 656e 7473 3a61 7574 6f3b  ter-events:auto;
-000639d0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
-000639e0: 653b 6c65 6674 3a35 3025 3b74 6f70 3a35  e;left:50%;top:5
-000639f0: 7265 6d3b 7769 6474 683a 6669 742d 636f  rem;width:fit-co
-00063a00: 6e74 656e 743b 6d61 782d 7769 6474 683a  ntent;max-width:
-00063a10: 3530 7265 6d3b 7061 6464 696e 673a 322e  50rem;padding:2.
-00063a20: 3272 656d 3b6f 7665 7266 6c6f 773a 6869  2rem;overflow:hi
-00063a30: 6464 656e 3b64 6973 706c 6179 3a66 6c65  dden;display:fle
-00063a40: 783b 666c 6578 2d64 6972 6563 7469 6f6e  x;flex-direction
-00063a50: 3a63 6f6c 756d 6e3b 616c 6967 6e2d 6974  :column;align-it
-00063a60: 656d 733a 7374 7265 7463 683b 6761 703a  ems:stretch;gap:
-00063a70: 312e 3572 656d 3b62 6f72 6465 722d 7261  1.5rem;border-ra
-00063a80: 6469 7573 3a76 6172 282d 2d72 696f 2d67  dius:var(--rio-g
-00063a90: 6c6f 6261 6c2d 636f 726e 6572 2d72 6164  lobal-corner-rad
-00063aa0: 6975 732d 6c61 7267 6529 3b62 6f78 2d73  ius-large);box-s
-00063ab0: 6861 646f 773a 3020 2e34 7265 6d20 3172  hadow:0 .4rem 1r
-00063ac0: 656d 2076 6172 282d 2d72 696f 2d67 6c6f  em var(--rio-glo
-00063ad0: 6261 6c2d 7368 6164 6f77 2d63 6f6c 6f72  bal-shadow-color
-00063ae0: 293b 7472 616e 7366 6f72 6d3a 7472 616e  );transform:tran
-00063af0: 736c 6174 6528 2d35 3025 297d 2e72 696f  slate(-50%)}.rio
-00063b00: 2d74 7261 6365 6261 636b 2d68 6561 6465  -traceback-heade
-00063b10: 727b 6469 7370 6c61 793a 666c 6578 3b61  r{display:flex;a
-00063b20: 6c69 676e 2d69 7465 6d73 3a63 656e 7465  lign-items:cente
-00063b30: 723b 6761 703a 2e36 7265 6d7d 2e72 696f  r;gap:.6rem}.rio
-00063b40: 2d74 7261 6365 6261 636b 2d68 6561 6465  -traceback-heade
-00063b50: 723e 7376 677b 7769 6474 683a 322e 3572  r>svg{width:2.5r
-00063b60: 656d 3b68 6569 6768 743a 322e 3572 656d  em;height:2.5rem
-00063b70: 3b66 696c 6c3a 7661 7228 2d2d 7269 6f2d  ;fill:var(--rio-
-00063b80: 676c 6f62 616c 2d64 616e 6765 722d 6267  global-danger-bg
-00063b90: 297d 2e72 696f 2d74 7261 6365 6261 636b  )}.rio-traceback
-00063ba0: 2d68 6561 6465 723e 6469 767b 666c 6578  -header>div{flex
-00063bb0: 2d67 726f 773a 313b 7465 7874 2d61 6c69  -grow:1;text-ali
-00063bc0: 676e 3a6c 6566 743b 666f 6e74 2d73 697a  gn:left;font-siz
-00063bd0: 653a 312e 3872 656d 3b63 6f6c 6f72 3a76  e:1.8rem;color:v
-00063be0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00063bf0: 6461 6e67 6572 2d62 6729 7d2e 7269 6f2d  danger-bg)}.rio-
-00063c00: 7472 6163 6562 6163 6b2d 7472 6163 6562  traceback-traceb
-00063c10: 6163 6b7b 666f 6e74 2d66 616d 696c 793a  ack{font-family:
-00063c20: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00063c30: 2d6d 6f6e 6f73 7061 6365 2d66 6f6e 7429  -monospace-font)
-00063c40: 2c6d 6f6e 6f73 7061 6365 3b66 6f6e 742d  ,monospace;font-
-00063c50: 7369 7a65 3a2e 3972 656d 3b77 6869 7465  size:.9rem;white
-00063c60: 2d73 7061 6365 3a70 7265 2d77 7261 703b  -space:pre-wrap;
-00063c70: 6f76 6572 666c 6f77 2d77 7261 703a 6272  overflow-wrap:br
-00063c80: 6561 6b2d 776f 7264 3b70 6164 6469 6e67  eak-word;padding
-00063c90: 3a2e 3572 656d 2031 7265 6d3b 6261 636b  :.5rem 1rem;back
-00063ca0: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-00063cb0: 282d 2d72 696f 2d6c 6f63 616c 2d62 672d  (--rio-local-bg-
-00063cc0: 7661 7269 616e 7429 3b62 6f72 6465 722d  variant);border-
-00063cd0: 7261 6469 7573 3a76 6172 282d 2d72 696f  radius:var(--rio
-00063ce0: 2d67 6c6f 6261 6c2d 636f 726e 6572 2d72  -global-corner-r
-00063cf0: 6164 6975 732d 736d 616c 6c29 7d2e 7269  adius-small)}.ri
-00063d00: 6f2d 7472 6163 6562 6163 6b2d 666f 6f74  o-traceback-foot
-00063d10: 6572 7b64 6973 706c 6179 3a66 6c65 783b  er{display:flex;
-00063d20: 666c 6578 2d64 6972 6563 7469 6f6e 3a63  flex-direction:c
-00063d30: 6f6c 756d 6e3b 6761 703a 2e35 7265 6d7d  olumn;gap:.5rem}
-00063d40: 2e72 696f 2d74 7261 6365 6261 636b 2d66  .rio-traceback-f
-00063d50: 6f6f 7465 722d 6c69 6e6b 737b 6469 7370  ooter-links{disp
-00063d60: 6c61 793a 666c 6578 3b66 6c65 782d 6469  lay:flex;flex-di
-00063d70: 7265 6374 696f 6e3a 726f 773b 6761 703a  rection:row;gap:
-00063d80: 2e35 7265 6d3b 6a75 7374 6966 792d 636f  .5rem;justify-co
-00063d90: 6e74 656e 743a 7370 6163 652d 6265 7477  ntent:space-betw
-00063da0: 6565 6e7d 2e72 696f 2d74 7261 6365 6261  een}.rio-traceba
-00063db0: 636b 2d66 6f6f 7465 723e 617b 666c 6578  ck-footer>a{flex
-00063dc0: 3a31 7d2e 7269 6f2d 7472 6163 6562 6163  :1}.rio-tracebac
-00063dd0: 6b2d 626f 6c64 7b66 6f6e 742d 7765 6967  k-bold{font-weig
-00063de0: 6874 3a37 3030 7d2e 7269 6f2d 7472 6163  ht:700}.rio-trac
-00063df0: 6562 6163 6b2d 6469 6d7b 6f70 6163 6974  eback-dim{opacit
-00063e00: 793a 2e35 7d2e 7269 6f2d 7472 6163 6562  y:.5}.rio-traceb
-00063e10: 6163 6b2d 7265 647b 636f 6c6f 723a 7661  ack-red{color:va
-00063e20: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d64  r(--rio-global-d
-00063e30: 616e 6765 722d 6267 297d 2e72 696f 2d74  anger-bg)}.rio-t
-00063e40: 7261 6365 6261 636b 2d79 656c 6c6f 777b  raceback-yellow{
-00063e50: 636f 6c6f 723a 7661 7228 2d2d 7269 6f2d  color:var(--rio-
-00063e60: 676c 6f62 616c 2d77 6172 6e69 6e67 2d62  global-warning-b
-00063e70: 6729 7d2e 7269 6f2d 6465 6275 6767 6572  g)}.rio-debugger
-00063e80: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
-00063e90: 2d2d 7269 6f2d 676c 6f62 616c 2d62 6163  --rio-global-bac
-00063ea0: 6b67 726f 756e 642d 6267 293b 7a2d 696e  kground-bg);z-in
-00063eb0: 6465 783a 3130 3030 327d 2e72 696f 2d64  dex:10002}.rio-d
-00063ec0: 6562 7567 6765 722d 6e61 7669 6761 7469  ebugger-navigati
-00063ed0: 6f6e 2d72 696f 2d6c 6f67 6f7b 706f 696e  on-rio-logo{poin
-00063ee0: 7465 722d 6576 656e 7473 3a61 7574 6f3b  ter-events:auto;
-00063ef0: 6469 7370 6c61 793a 666c 6578 3b66 6c65  display:flex;fle
-00063f00: 782d 6469 7265 6374 696f 6e3a 636f 6c75  x-direction:colu
-00063f10: 6d6e 3b61 6c69 676e 2d69 7465 6d73 3a63  mn;align-items:c
-00063f20: 656e 7465 723b 6a75 7374 6966 792d 636f  enter;justify-co
-00063f30: 6e74 656e 743a 656e 643b 6761 703a 2e33  ntent:end;gap:.3
-00063f40: 3572 656d 3b7a 2d69 6e64 6578 3a32 3b74  5rem;z-index:2;t
-00063f50: 6578 742d 6465 636f 7261 7469 6f6e 3a6e  ext-decoration:n
-00063f60: 6f6e 657d 2e72 696f 2d64 6562 7567 6765  one}.rio-debugge
-00063f70: 722d 6e61 7669 6761 7469 6f6e 2d72 696f  r-navigation-rio
-00063f80: 2d6c 6f67 6f20 696d 677b 7769 6474 683a  -logo img{width:
-00063f90: 322e 3572 656d 3b68 6569 6768 743a 322e  2.5rem;height:2.
-00063fa0: 3572 656d 3b6f 626a 6563 742d 6669 743a  5rem;object-fit:
-00063fb0: 636f 6e74 6169 6e7d 2e72 696f 2d64 6562  contain}.rio-deb
-00063fc0: 7567 6765 722d 6e61 7669 6761 7469 6f6e  ugger-navigation
-00063fd0: 2d72 696f 2d6c 6f67 6f20 6469 767b 6d61  -rio-logo div{ma
-00063fe0: 7267 696e 2d62 6f74 746f 6d3a 3172 656d  rgin-bottom:1rem
-00063ff0: 3b66 6f6e 742d 7369 7a65 3a31 2e32 7265  ;font-size:1.2re
-00064000: 6d3b 636f 6c6f 723a 7661 7228 2d2d 7269  m;color:var(--ri
-00064010: 6f2d 6c6f 6361 6c2d 7465 7874 2d63 6f6c  o-local-text-col
-00064020: 6f72 293b 7472 616e 7369 7469 6f6e 3a63  or);transition:c
-00064030: 6f6c 6f72 2031 7320 6561 7365 2d69 6e2d  olor 1s ease-in-
-00064040: 6f75 747d 2e72 696f 2d64 6562 7567 6765  out}.rio-debugge
-00064050: 722d 6e61 7669 6761 7469 6f6e 2d72 696f  r-navigation-rio
-00064060: 2d6c 6f67 6f3a 686f 7665 7220 6469 767b  -logo:hover div{
-00064070: 636f 6c6f 723a 7661 7228 2d2d 7269 6f2d  color:var(--rio-
-00064080: 676c 6f62 616c 2d73 6563 6f6e 6461 7279  global-secondary
-00064090: 2d66 6729 3b74 7261 6e73 6974 696f 6e3a  -fg);transition:
-000640a0: 636f 6c6f 7220 2e31 7320 6561 7365 2d69  color .1s ease-i
-000640b0: 6e2d 6f75 747d 2e72 696f 2d64 6562 7567  n-out}.rio-debug
-000640c0: 6765 722d 6e61 7669 6761 7469 6f6e 2d72  ger-navigation-r
-000640d0: 696f 2d6c 6f67 6f3a 6265 666f 7265 7b63  io-logo:before{c
-000640e0: 6f6e 7465 6e74 3a22 223b 706f 7369 7469  ontent:"";positi
-000640f0: 6f6e 3a61 6273 6f6c 7574 653b 746f 703a  on:absolute;top:
-00064100: 303b 7269 6768 743a 303b 626f 7474 6f6d  0;right:0;bottom
-00064110: 3a30 3b6c 6566 743a 303b 7a2d 696e 6465  :0;left:0;z-inde
-00064120: 783a 2d31 3b62 6163 6b67 726f 756e 643a  x:-1;background:
-00064130: 6c69 6e65 6172 2d67 7261 6469 656e 7428  linear-gradient(
-00064140: 746f 2074 6f70 2c76 6172 282d 2d72 696f  to top,var(--rio
-00064150: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
-00064160: 792d 6267 292c 7472 616e 7370 6172 656e  y-bg),transparen
-00064170: 7429 3b6f 7061 6369 7479 3a30 3b74 7261  t);opacity:0;tra
-00064180: 6e73 6974 696f 6e3a 6f70 6163 6974 7920  nsition:opacity 
-00064190: 3173 2065 6173 652d 6f75 747d 2e72 696f  1s ease-out}.rio
-000641a0: 2d64 6562 7567 6765 722d 6e61 7669 6761  -debugger-naviga
-000641b0: 7469 6f6e 2d72 696f 2d6c 6f67 6f3a 686f  tion-rio-logo:ho
-000641c0: 7665 723a 6265 666f 7265 7b6f 7061 6369  ver:before{opaci
-000641d0: 7479 3a31 3b74 7261 6e73 6974 696f 6e3a  ty:1;transition:
-000641e0: 6f70 6163 6974 7920 2e31 7320 6561 7365  opacity .1s ease
-000641f0: 2d6f 7574 7d2e 7269 6f2d 6465 6275 6767  -out}.rio-debugg
-00064200: 6572 2d74 7265 652d 636f 6d70 6f6e 656e  er-tree-componen
-00064210: 742d 7472 6565 7b6f 7665 7266 6c6f 773a  t-tree{overflow:
-00064220: 6175 746f 7d2e 7269 6f2d 6465 6275 6767  auto}.rio-debugg
-00064230: 6572 2d74 7265 652d 636f 6d70 6f6e 656e  er-tree-componen
-00064240: 742d 7472 6565 3e2a 7b70 6f73 6974 696f  t-tree>*{positio
-00064250: 6e3a 6162 736f 6c75 7465 3b77 6964 7468  n:absolute;width
-00064260: 3a31 3030 253b 6865 6967 6874 3a31 3030  :100%;height:100
-00064270: 253b 6f76 6572 666c 6f77 2d78 3a68 6964  %;overflow-x:hid
-00064280: 6465 6e3b 6f76 6572 666c 6f77 2d79 3a61  den;overflow-y:a
-00064290: 7574 6f7d 2e72 696f 2d64 6562 7567 6765  uto}.rio-debugge
-000642a0: 722d 636f 6d70 6f6e 656e 742d 7472 6565  r-component-tree
-000642b0: 2d69 7465 6d7b 6469 7370 6c61 793a 666c  -item{display:fl
-000642c0: 6578 3b66 6c65 782d 6469 7265 6374 696f  ex;flex-directio
-000642d0: 6e3a 636f 6c75 6d6e 3b67 6170 3a2e 3272  n:column;gap:.2r
-000642e0: 656d 7d40 6b65 7966 7261 6d65 7320 666c  em}@keyframes fl
-000642f0: 6173 682d 7465 7874 7b30 257b 636f 6c6f  ash-text{0%{colo
-00064300: 723a 696e 6974 6961 6c7d 3230 257b 636f  r:initial}20%{co
-00064310: 6c6f 723a 7661 7228 2d2d 7269 6f2d 676c  lor:var(--rio-gl
-00064320: 6f62 616c 2d77 6172 6e69 6e67 2d62 6729  obal-warning-bg)
-00064330: 7d74 6f7b 636f 6c6f 723a 696e 6974 6961  }to{color:initia
-00064340: 6c7d 7d2e 7269 6f2d 6465 6275 6767 6572  l}}.rio-debugger
-00064350: 2d63 6f6d 706f 6e65 6e74 2d74 7265 652d  -component-tree-
-00064360: 666c 6173 687b 616e 696d 6174 696f 6e3a  flash{animation:
-00064370: 666c 6173 682d 7465 7874 2033 7320 6c69  flash-text 3s li
-00064380: 6e65 6172 7d2e 7269 6f2d 6465 6275 6767  near}.rio-debugg
-00064390: 6572 2d63 6f6d 706f 6e65 6e74 2d74 7265  er-component-tre
-000643a0: 652d 6974 656d 2d68 6561 6465 727b 706f  e-item-header{po
-000643b0: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
-000643c0: 6f3b 6375 7273 6f72 3a70 6f69 6e74 6572  o;cursor:pointer
-000643d0: 3b7a 2d69 6e64 6578 3a31 3b70 6f73 6974  ;z-index:1;posit
-000643e0: 696f 6e3a 7265 6c61 7469 7665 3b70 6164  ion:relative;pad
-000643f0: 6469 6e67 3a2e 3372 656d 202e 3672 656d  ding:.3rem .6rem
-00064400: 3b64 6973 706c 6179 3a66 6c65 783b 666c  ;display:flex;fl
-00064410: 6578 2d64 6972 6563 7469 6f6e 3a72 6f77  ex-direction:row
-00064420: 3b61 6c69 676e 2d69 7465 6d73 3a63 656e  ;align-items:cen
-00064430: 7465 723b 6761 703a 2e35 7265 6d7d 2e72  ter;gap:.5rem}.r
-00064440: 696f 2d64 6562 7567 6765 722d 636f 6d70  io-debugger-comp
-00064450: 6f6e 656e 742d 7472 6565 2d69 7465 6d3e  onent-tree-item>
-00064460: 2e72 696f 2d64 6562 7567 6765 722d 636f  .rio-debugger-co
-00064470: 6d70 6f6e 656e 742d 7472 6565 2d69 7465  mponent-tree-ite
-00064480: 6d2d 6865 6164 6572 3e64 6976 3a66 6972  m-header>div:fir
-00064490: 7374 2d63 6869 6c64 7b77 6964 7468 3a31  st-child{width:1
-000644a0: 7265 6d3b 6865 6967 6874 3a31 7265 6d3b  rem;height:1rem;
-000644b0: 7472 616e 7369 7469 6f6e 3a74 7261 6e73  transition:trans
-000644c0: 666f 726d 202e 3173 2065 6173 652d 696e  form .1s ease-in
-000644d0: 2d6f 7574 7d2e 7269 6f2d 6465 6275 6767  -out}.rio-debugg
+00060600: 7469 6d65 6c69 6e65 2d70 6c61 7965 647b  timeline-played{
+00060610: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
+00060620: 653b 7769 6474 683a 3025 3b68 6569 6768  e;width:0%;heigh
+00060630: 743a 3130 3025 3b62 6163 6b67 726f 756e  t:100%;backgroun
+00060640: 642d 636f 6c6f 723a 2366 6666 3b62 6f72  d-color:#fff;bor
+00060650: 6465 722d 7261 6469 7573 3a39 3939 3939  der-radius:99999
+00060660: 7078 7d2e 7269 6f2d 6d65 6469 612d 706c  px}.rio-media-pl
+00060670: 6179 6572 2d74 696d 656c 696e 652d 6261  ayer-timeline-ba
+00060680: 636b 6772 6f75 6e64 7b77 6964 7468 3a31  ckground{width:1
+00060690: 3030 253b 6f70 6163 6974 793a 2e32 7d2e  00%;opacity:.2}.
+000606a0: 7269 6f2d 6d65 6469 612d 706c 6179 6572  rio-media-player
+000606b0: 2d74 696d 656c 696e 652d 6c6f 6164 6564  -timeline-loaded
+000606c0: 7b6f 7061 6369 7479 3a2e 337d 2e72 696f  {opacity:.3}.rio
+000606d0: 2d6d 6564 6961 2d70 6c61 7965 722d 7469  -media-player-ti
+000606e0: 6d65 6c69 6e65 2d68 6f76 6572 7b6f 7061  meline-hover{opa
+000606f0: 6369 7479 3a30 3b74 7261 6e73 6974 696f  city:0;transitio
+00060700: 6e3a 6f70 6163 6974 7920 2e32 7320 6561  n:opacity .2s ea
+00060710: 7365 2d69 6e2d 6f75 747d 2e72 696f 2d6d  se-in-out}.rio-m
+00060720: 6564 6961 2d70 6c61 7965 722d 7469 6d65  edia-player-time
+00060730: 6c69 6e65 2d70 6c61 7965 647b 6261 636b  line-played{back
+00060740: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+00060750: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7072  (--rio-global-pr
+00060760: 696d 6172 792d 6267 297d 2e72 696f 2d6d  imary-bg)}.rio-m
+00060770: 6564 6961 2d70 6c61 7965 722d 636f 6e74  edia-player-cont
+00060780: 726f 6c73 2d72 6f77 7b64 6973 706c 6179  rols-row{display
+00060790: 3a66 6c65 783b 6761 703a 312e 3272 656d  :flex;gap:1.2rem
+000607a0: 3b61 6c69 676e 2d69 7465 6d73 3a63 656e  ;align-items:cen
+000607b0: 7465 723b 7061 6464 696e 673a 2e35 7265  ter;padding:.5re
+000607c0: 6d3b 7061 6464 696e 672d 746f 703a 307d  m;padding-top:0}
+000607d0: 2e72 696f 2d6d 6564 6961 2d70 6c61 7965  .rio-media-playe
+000607e0: 722d 6275 7474 6f6e 7b70 6f69 6e74 6572  r-button{pointer
+000607f0: 2d65 7665 6e74 733a 6175 746f 3b63 7572  -events:auto;cur
+00060800: 736f 723a 706f 696e 7465 723b 7769 6474  sor:pointer;widt
+00060810: 683a 3272 656d 3b68 6569 6768 743a 3272  h:2rem;height:2r
+00060820: 656d 7d2e 7269 6f2d 6d65 6469 612d 706c  em}.rio-media-pl
+00060830: 6179 6572 2d62 7574 746f 6e3e 696d 677b  ayer-button>img{
+00060840: 7769 6474 683a 3130 3025 3b68 6569 6768  width:100%;heigh
+00060850: 743a 3130 3025 7d2e 7269 6f2d 6d65 6469  t:100%}.rio-medi
+00060860: 612d 706c 6179 6572 2d76 6f6c 756d 657b  a-player-volume{
+00060870: 706f 696e 7465 722d 6576 656e 7473 3a61  pointer-events:a
+00060880: 7574 6f3b 6375 7273 6f72 3a70 6f69 6e74  uto;cursor:point
+00060890: 6572 3b70 6f73 6974 696f 6e3a 7265 6c61  er;position:rela
+000608a0: 7469 7665 3b77 6964 7468 3a35 7265 6d3b  tive;width:5rem;
+000608b0: 6865 6967 6874 3a31 2e35 7265 6d7d 2e72  height:1.5rem}.r
+000608c0: 696f 2d6d 6564 6961 2d70 6c61 7965 722d  io-media-player-
+000608d0: 766f 6c75 6d65 3e64 6976 7b70 6f69 6e74  volume>div{point
+000608e0: 6572 2d65 7665 6e74 733a 6e6f 6e65 3b70  er-events:none;p
+000608f0: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
+00060900: 3b74 6f70 3a35 3025 3b68 6569 6768 743a  ;top:50%;height:
+00060910: 2e32 7265 6d3b 7472 616e 7366 6f72 6d3a  .2rem;transform:
+00060920: 7472 616e 736c 6174 6559 282d 3530 2529  translateY(-50%)
+00060930: 7d2e 7269 6f2d 6d65 6469 612d 706c 6179  }.rio-media-play
+00060940: 6572 2d76 6f6c 756d 652d 6261 636b 6772  er-volume-backgr
+00060950: 6f75 6e64 2c2e 7269 6f2d 6d65 6469 612d  ound,.rio-media-
+00060960: 706c 6179 6572 2d76 6f6c 756d 652d 6375  player-volume-cu
+00060970: 7272 656e 747b 706f 7369 7469 6f6e 3a61  rrent{position:a
+00060980: 6273 6f6c 7574 653b 7769 6474 683a 3130  bsolute;width:10
+00060990: 3025 3b68 6569 6768 743a 3130 3025 3b62  0%;height:100%;b
+000609a0: 6f72 6465 722d 7261 6469 7573 3a39 3939  order-radius:999
+000609b0: 3939 7078 3b62 6163 6b67 726f 756e 642d  99px;background-
+000609c0: 636f 6c6f 723a 2366 6666 7d2e 7269 6f2d  color:#fff}.rio-
+000609d0: 6d65 6469 612d 706c 6179 6572 2d76 6f6c  media-player-vol
+000609e0: 756d 652d 6261 636b 6772 6f75 6e64 7b6f  ume-background{o
+000609f0: 7061 6369 7479 3a2e 327d 2e72 696f 2d6d  pacity:.2}.rio-m
+00060a00: 6564 6961 2d70 6c61 7965 722d 766f 6c75  edia-player-volu
+00060a10: 6d65 2d6b 6e6f 627b 706f 7369 7469 6f6e  me-knob{position
+00060a20: 3a61 6273 6f6c 7574 653b 7769 6474 683a  :absolute;width:
+00060a30: 2e39 7265 6d3b 6865 6967 6874 3a2e 3972  .9rem;height:.9r
+00060a40: 656d 3b6c 6566 743a 3130 3025 3b74 6f70  em;left:100%;top
+00060a50: 3a35 3025 3b62 6163 6b67 726f 756e 642d  :50%;background-
+00060a60: 636f 6c6f 723a 2366 6666 3b62 6f72 6465  color:#fff;borde
+00060a70: 722d 7261 6469 7573 3a35 3025 3b74 7261  r-radius:50%;tra
+00060a80: 6e73 666f 726d 3a74 7261 6e73 6c61 7465  nsform:translate
+00060a90: 282d 3530 252c 2d35 3025 297d 2e72 696f  (-50%,-50%)}.rio
+00060aa0: 2d6d 6564 6961 2d70 6c61 7965 722d 766f  -media-player-vo
+00060ab0: 6c75 6d65 3e64 6976 7b70 6f73 6974 696f  lume>div{positio
+00060ac0: 6e3a 7265 6c61 7469 7665 3b74 6f70 3a35  n:relative;top:5
+00060ad0: 3025 3b68 6569 6768 743a 2e32 7265 6d3b  0%;height:.2rem;
+00060ae0: 7472 616e 7366 6f72 6d3a 7472 616e 736c  transform:transl
+00060af0: 6174 6559 282d 3530 2529 7d2e 7269 6f2d  ateY(-50%)}.rio-
+00060b00: 6d65 6469 612d 706c 6179 6572 2d70 6c61  media-player-pla
+00060b10: 7974 696d 652d 6c61 6265 6c7b 636f 6c6f  ytime-label{colo
+00060b20: 723a 2366 6666 3b6f 7061 6369 7479 3a2e  r:#fff;opacity:.
+00060b30: 367d 2e72 696f 2d6d 6172 6b64 6f77 6e7b  6}.rio-markdown{
+00060b40: 706f 696e 7465 722d 6576 656e 7473 3a61  pointer-events:a
+00060b50: 7574 6f3b 636f 6c6f 723a 7661 7228 2d2d  uto;color:var(--
+00060b60: 7269 6f2d 6c6f 6361 6c2d 7465 7874 2d63  rio-local-text-c
+00060b70: 6f6c 6f72 297d 2e72 696f 2d6d 6172 6b64  olor)}.rio-markd
+00060b80: 6f77 6e3e 2a2c 2e72 696f 2d6d 6172 6b64  own>*,.rio-markd
+00060b90: 6f77 6e20 6c69 3e2a 7b6d 6172 6769 6e2d  own li>*{margin-
+00060ba0: 746f 703a 303b 6d61 7267 696e 2d62 6f74  top:0;margin-bot
+00060bb0: 746f 6d3a 307d 2e72 696f 2d6d 6172 6b64  tom:0}.rio-markd
+00060bc0: 6f77 6e3e 2a2b 2a2c 2e72 696f 2d6d 6172  own>*+*,.rio-mar
+00060bd0: 6b64 6f77 6e20 6c69 3e2a 2b2a 7b6d 6172  kdown li>*+*{mar
+00060be0: 6769 6e2d 746f 703a 2e38 7265 6d7d 2e72  gin-top:.8rem}.r
+00060bf0: 696f 2d6d 6172 6b64 6f77 6e20 756c 7b70  io-markdown ul{p
+00060c00: 6164 6469 6e67 2d6c 6566 743a 3172 656d  adding-left:1rem
+00060c10: 3b6c 6973 742d 7374 796c 652d 7479 7065  ;list-style-type
+00060c20: 3a6e 6f6e 657d 2e72 696f 2d6d 6172 6b64  :none}.rio-markd
+00060c30: 6f77 6e20 756c 3e6c 693a 6265 666f 7265  own ul>li:before
+00060c40: 7b63 6f6e 7465 6e74 3a22 2d22 3b66 6f6e  {content:"-";fon
+00060c50: 742d 7765 6967 6874 3a37 3030 3b70 6f73  t-weight:700;pos
+00060c60: 6974 696f 6e3a 6162 736f 6c75 7465 3b74  ition:absolute;t
+00060c70: 7261 6e73 666f 726d 3a74 7261 6e73 6c61  ransform:transla
+00060c80: 7465 282d 2e36 7265 6d29 7d2e 7269 6f2d  te(-.6rem)}.rio-
+00060c90: 6d61 726b 646f 776e 206c 692b 6c69 7b6d  markdown li+li{m
+00060ca0: 6172 6769 6e2d 746f 703a 2e32 7265 6d7d  argin-top:.2rem}
+00060cb0: 2e72 696f 2d6d 6172 6b64 6f77 6e20 636f  .rio-markdown co
+00060cc0: 6465 7b66 6f6e 742d 6661 6d69 6c79 3a76  de{font-family:v
+00060cd0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00060ce0: 6d6f 6e6f 7370 6163 652d 666f 6e74 292c  monospace-font),
+00060cf0: 6d6f 6e6f 7370 6163 653b 6261 636b 6772  monospace;backgr
+00060d00: 6f75 6e64 3a76 6172 282d 2d72 696f 2d6c  ound:var(--rio-l
+00060d10: 6f63 616c 2d62 672d 7661 7269 616e 7429  ocal-bg-variant)
+00060d20: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
+00060d30: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00060d40: 636f 726e 6572 2d72 6164 6975 732d 736d  corner-radius-sm
+00060d50: 616c 6c29 3b70 6164 6469 6e67 3a2e 3172  all);padding:.1r
+00060d60: 656d 202e 3372 656d 7d2e 7269 6f2d 6d61  em .3rem}.rio-ma
+00060d70: 726b 646f 776e 2068 317b 666f 6e74 2d66  rkdown h1{font-f
+00060d80: 616d 696c 793a 7661 7228 2d2d 7269 6f2d  amily:var(--rio-
+00060d90: 676c 6f62 616c 2d68 6561 6469 6e67 312d  global-heading1-
+00060da0: 666f 6e74 2d6e 616d 6529 3b63 6f6c 6f72  font-name);color
+00060db0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
+00060dc0: 2d68 6561 6469 6e67 312d 636f 6c6f 7229  -heading1-color)
+00060dd0: 3b66 6f6e 742d 7369 7a65 3a76 6172 282d  ;font-size:var(-
+00060de0: 2d72 696f 2d67 6c6f 6261 6c2d 6865 6164  -rio-global-head
+00060df0: 696e 6731 2d66 6f6e 742d 7369 7a65 293b  ing1-font-size);
+00060e00: 666f 6e74 2d73 7479 6c65 3a76 6172 282d  font-style:var(-
+00060e10: 2d72 696f 2d67 6c6f 6261 6c2d 6865 6164  -rio-global-head
+00060e20: 696e 6731 2d69 7461 6c69 6329 3b66 6f6e  ing1-italic);fon
+00060e30: 742d 7765 6967 6874 3a76 6172 282d 2d72  t-weight:var(--r
+00060e40: 696f 2d67 6c6f 6261 6c2d 6865 6164 696e  io-global-headin
+00060e50: 6731 2d66 6f6e 742d 7765 6967 6874 293b  g1-font-weight);
+00060e60: 7465 7874 2d64 6563 6f72 6174 696f 6e3a  text-decoration:
+00060e70: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00060e80: 2d68 6561 6469 6e67 312d 756e 6465 726c  -heading1-underl
+00060e90: 696e 6564 293b 7465 7874 2d74 7261 6e73  ined);text-trans
+00060ea0: 666f 726d 3a76 6172 282d 2d72 696f 2d67  form:var(--rio-g
+00060eb0: 6c6f 6261 6c2d 6865 6164 696e 6731 2d61  lobal-heading1-a
+00060ec0: 6c6c 2d63 6170 7329 7d2e 7269 6f2d 6d61  ll-caps)}.rio-ma
+00060ed0: 726b 646f 776e 2068 313a 6e6f 7428 3a66  rkdown h1:not(:f
+00060ee0: 6972 7374 2d63 6869 6c64 297b 6d61 7267  irst-child){marg
+00060ef0: 696e 2d74 6f70 3a32 7265 6d7d 2e72 696f  in-top:2rem}.rio
+00060f00: 2d6d 6172 6b64 6f77 6e20 6831 3a6e 6f74  -markdown h1:not
+00060f10: 283a 6c61 7374 2d63 6869 6c64 297b 6d61  (:last-child){ma
+00060f20: 7267 696e 2d62 6f74 746f 6d3a 3172 656d  rgin-bottom:1rem
+00060f30: 7d2e 7269 6f2d 6d61 726b 646f 776e 2068  }.rio-markdown h
+00060f40: 327b 666f 6e74 2d66 616d 696c 793a 7661  2{font-family:va
+00060f50: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d68  r(--rio-global-h
+00060f60: 6561 6469 6e67 322d 666f 6e74 2d6e 616d  eading2-font-nam
+00060f70: 6529 3b63 6f6c 6f72 3a76 6172 282d 2d72  e);color:var(--r
+00060f80: 696f 2d6c 6f63 616c 2d68 6561 6469 6e67  io-local-heading
+00060f90: 322d 636f 6c6f 7229 3b66 6f6e 742d 7369  2-color);font-si
+00060fa0: 7a65 3a76 6172 282d 2d72 696f 2d67 6c6f  ze:var(--rio-glo
+00060fb0: 6261 6c2d 6865 6164 696e 6732 2d66 6f6e  bal-heading2-fon
+00060fc0: 742d 7369 7a65 293b 666f 6e74 2d73 7479  t-size);font-sty
+00060fd0: 6c65 3a76 6172 282d 2d72 696f 2d67 6c6f  le:var(--rio-glo
+00060fe0: 6261 6c2d 6865 6164 696e 6732 2d69 7461  bal-heading2-ita
+00060ff0: 6c69 6329 3b66 6f6e 742d 7765 6967 6874  lic);font-weight
+00061000: 3a76 6172 282d 2d72 696f 2d67 6c6f 6261  :var(--rio-globa
+00061010: 6c2d 6865 6164 696e 6732 2d66 6f6e 742d  l-heading2-font-
+00061020: 7765 6967 6874 293b 7465 7874 2d64 6563  weight);text-dec
+00061030: 6f72 6174 696f 6e3a 7661 7228 2d2d 7269  oration:var(--ri
+00061040: 6f2d 676c 6f62 616c 2d68 6561 6469 6e67  o-global-heading
+00061050: 322d 756e 6465 726c 696e 6564 293b 7465  2-underlined);te
+00061060: 7874 2d74 7261 6e73 666f 726d 3a76 6172  xt-transform:var
+00061070: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6865  (--rio-global-he
+00061080: 6164 696e 6732 2d61 6c6c 2d63 6170 7329  ading2-all-caps)
+00061090: 3b6d 6172 6769 6e2d 746f 703a 307d 2e72  ;margin-top:0}.r
+000610a0: 696f 2d6d 6172 6b64 6f77 6e20 6832 3a6e  io-markdown h2:n
+000610b0: 6f74 283a 6669 7273 742d 6368 696c 6429  ot(:first-child)
+000610c0: 7b6d 6172 6769 6e2d 746f 703a 312e 3572  {margin-top:1.5r
+000610d0: 656d 7d2e 7269 6f2d 6d61 726b 646f 776e  em}.rio-markdown
+000610e0: 2068 323a 6e6f 7428 3a6c 6173 742d 6368   h2:not(:last-ch
+000610f0: 696c 6429 7b6d 6172 6769 6e2d 626f 7474  ild){margin-bott
+00061100: 6f6d 3a31 7265 6d7d 2e72 696f 2d6d 6172  om:1rem}.rio-mar
+00061110: 6b64 6f77 6e20 6833 7b66 6f6e 742d 6661  kdown h3{font-fa
+00061120: 6d69 6c79 3a76 6172 282d 2d72 696f 2d67  mily:var(--rio-g
+00061130: 6c6f 6261 6c2d 6865 6164 696e 6733 2d66  lobal-heading3-f
+00061140: 6f6e 742d 6e61 6d65 293b 636f 6c6f 723a  ont-name);color:
+00061150: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
+00061160: 6865 6164 696e 6733 2d63 6f6c 6f72 293b  heading3-color);
+00061170: 666f 6e74 2d73 697a 653a 7661 7228 2d2d  font-size:var(--
+00061180: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
+00061190: 6e67 332d 666f 6e74 2d73 697a 6529 3b66  ng3-font-size);f
+000611a0: 6f6e 742d 7374 796c 653a 7661 7228 2d2d  ont-style:var(--
+000611b0: 7269 6f2d 676c 6f62 616c 2d68 6561 6469  rio-global-headi
+000611c0: 6e67 332d 6974 616c 6963 293b 666f 6e74  ng3-italic);font
+000611d0: 2d77 6569 6768 743a 7661 7228 2d2d 7269  -weight:var(--ri
+000611e0: 6f2d 676c 6f62 616c 2d68 6561 6469 6e67  o-global-heading
+000611f0: 332d 666f 6e74 2d77 6569 6768 7429 3b74  3-font-weight);t
+00061200: 6578 742d 6465 636f 7261 7469 6f6e 3a76  ext-decoration:v
+00061210: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00061220: 6865 6164 696e 6733 2d75 6e64 6572 6c69  heading3-underli
+00061230: 6e65 6429 3b74 6578 742d 7472 616e 7366  ned);text-transf
+00061240: 6f72 6d3a 7661 7228 2d2d 7269 6f2d 676c  orm:var(--rio-gl
+00061250: 6f62 616c 2d68 6561 6469 6e67 332d 616c  obal-heading3-al
+00061260: 6c2d 6361 7073 293b 6d61 7267 696e 2d74  l-caps);margin-t
+00061270: 6f70 3a30 7d2e 7269 6f2d 6d61 726b 646f  op:0}.rio-markdo
+00061280: 776e 2068 333a 6e6f 7428 3a66 6972 7374  wn h3:not(:first
+00061290: 2d63 6869 6c64 297b 6d61 7267 696e 2d74  -child){margin-t
+000612a0: 6f70 3a31 7265 6d7d 2e72 696f 2d6d 6172  op:1rem}.rio-mar
+000612b0: 6b64 6f77 6e20 6833 3a6e 6f74 283a 6c61  kdown h3:not(:la
+000612c0: 7374 2d63 6869 6c64 297b 6d61 7267 696e  st-child){margin
+000612d0: 2d62 6f74 746f 6d3a 2e35 7265 6d7d 2e72  -bottom:.5rem}.r
+000612e0: 696f 2d6d 6172 6b64 6f77 6e20 707b 666f  io-markdown p{fo
+000612f0: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
+00061300: 7269 6f2d 676c 6f62 616c 2d66 6f6e 7429  rio-global-font)
+00061310: 3b63 6f6c 6f72 3a76 6172 282d 2d72 696f  ;color:var(--rio
+00061320: 2d6c 6f63 616c 2d74 6578 742d 636f 6c6f  -local-text-colo
+00061330: 7229 3b66 6f6e 742d 7369 7a65 3a76 6172  r);font-size:var
+00061340: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7465  (--rio-global-te
+00061350: 7874 2d66 6f6e 742d 7369 7a65 293b 666f  xt-font-size);fo
+00061360: 6e74 2d73 7479 6c65 3a76 6172 282d 2d72  nt-style:var(--r
+00061370: 696f 2d67 6c6f 6261 6c2d 7465 7874 2d69  io-global-text-i
+00061380: 7461 6c69 6329 3b66 6f6e 742d 7765 6967  talic);font-weig
+00061390: 6874 3a76 6172 282d 2d72 696f 2d67 6c6f  ht:var(--rio-glo
+000613a0: 6261 6c2d 7465 7874 2d66 6f6e 742d 7765  bal-text-font-we
+000613b0: 6967 6874 293b 7465 7874 2d64 6563 6f72  ight);text-decor
+000613c0: 6174 696f 6e3a 7661 7228 2d2d 7269 6f2d  ation:var(--rio-
+000613d0: 676c 6f62 616c 2d74 6578 742d 756e 6465  global-text-unde
+000613e0: 726c 696e 6564 293b 7465 7874 2d74 7261  rlined);text-tra
+000613f0: 6e73 666f 726d 3a76 6172 282d 2d72 696f  nsform:var(--rio
+00061400: 2d67 6c6f 6261 6c2d 7465 7874 2d61 6c6c  -global-text-all
+00061410: 2d63 6170 7329 7d2e 7269 6f2d 636f 6465  -caps)}.rio-code
+00061420: 2d62 6c6f 636b 7b70 6f69 6e74 6572 2d65  -block{pointer-e
+00061430: 7665 6e74 733a 6175 746f 3b64 6973 706c  vents:auto;displ
+00061440: 6179 3a66 6c65 783b 666c 6578 2d64 6972  ay:flex;flex-dir
+00061450: 6563 7469 6f6e 3a63 6f6c 756d 6e3b 616c  ection:column;al
+00061460: 6967 6e2d 6974 656d 733a 7374 7265 7463  ign-items:stretc
+00061470: 683b 6761 703a 2e35 7265 6d3b 7061 6464  h;gap:.5rem;padd
+00061480: 696e 673a 2e35 7265 6d3b 6261 636b 6772  ing:.5rem;backgr
+00061490: 6f75 6e64 3a76 6172 282d 2d72 696f 2d6c  ound:var(--rio-l
+000614a0: 6f63 616c 2d62 672d 7661 7269 616e 7429  ocal-bg-variant)
+000614b0: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
+000614c0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+000614d0: 636f 726e 6572 2d72 6164 6975 732d 736d  corner-radius-sm
+000614e0: 616c 6c29 3b62 6f78 2d73 697a 696e 673a  all);box-sizing:
+000614f0: 626f 7264 6572 2d62 6f78 7d2e 7269 6f2d  border-box}.rio-
+00061500: 636f 6465 2d62 6c6f 636b 2d68 6561 6465  code-block-heade
+00061510: 727b 6469 7370 6c61 793a 666c 6578 3b66  r{display:flex;f
+00061520: 6c65 782d 6469 7265 6374 696f 6e3a 726f  lex-direction:ro
+00061530: 773b 616c 6967 6e2d 6974 656d 733a 6365  w;align-items:ce
+00061540: 6e74 6572 3b6a 7573 7469 6679 2d63 6f6e  nter;justify-con
+00061550: 7465 6e74 3a73 7061 6365 2d62 6574 7765  tent:space-betwe
+00061560: 656e 3b67 6170 3a31 7265 6d3b 636f 6c6f  en;gap:1rem;colo
+00061570: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
+00061580: 6c2d 7465 7874 2d63 6f6c 6f72 293b 666f  l-text-color);fo
+00061590: 6e74 2d73 697a 653a 2e38 7265 6d7d 2e72  nt-size:.8rem}.r
+000615a0: 696f 2d63 6f64 652d 626c 6f63 6b2d 6c61  io-code-block-la
+000615b0: 6e67 7561 6765 7b66 6f6e 742d 7765 6967  nguage{font-weig
+000615c0: 6874 3a37 3030 3b6f 7061 6369 7479 3a2e  ht:700;opacity:.
+000615d0: 347d 2e72 696f 2d63 6f64 652d 626c 6f63  4}.rio-code-bloc
+000615e0: 6b2d 636f 7079 2d62 7574 746f 6e7b 7769  k-copy-button{wi
+000615f0: 6474 683a 312e 3372 656d 3b68 6569 6768  dth:1.3rem;heigh
+00061600: 743a 312e 3372 656d 3b63 7572 736f 723a  t:1.3rem;cursor:
+00061610: 706f 696e 7465 723b 626f 7264 6572 3a6e  pointer;border:n
+00061620: 6f6e 653b 6261 636b 6772 6f75 6e64 3a6e  one;background:n
+00061630: 6f6e 653b 626f 7264 6572 2d72 6164 6975  one;border-radiu
+00061640: 733a 7661 7228 2d2d 7269 6f2d 676c 6f62  s:var(--rio-glob
+00061650: 616c 2d63 6f72 6e65 722d 7261 6469 7573  al-corner-radius
+00061660: 2d73 6d61 6c6c 293b 6d61 7267 696e 3a30  -small);margin:0
+00061670: 3b70 6164 6469 6e67 3a30 3b6f 7061 6369  ;padding:0;opaci
+00061680: 7479 3a2e 343b 7472 616e 7369 7469 6f6e  ty:.4;transition
+00061690: 3a6f 7061 6369 7479 202e 3273 2065 6173  :opacity .2s eas
+000616a0: 652d 696e 2d6f 7574 7d2e 7269 6f2d 636f  e-in-out}.rio-co
+000616b0: 6465 2d62 6c6f 636b 2d63 6f70 792d 6275  de-block-copy-bu
+000616c0: 7474 6f6e 3a68 6f76 6572 7b63 6f6c 6f72  tton:hover{color
+000616d0: 3a76 6172 282d 2d72 696f 2d6c 6f63 616c  :var(--rio-local
+000616e0: 2d6c 6576 656c 2d32 2d62 6729 3b6f 7061  -level-2-bg);opa
+000616f0: 6369 7479 3a31 7d2e 7269 6f2d 636f 6465  city:1}.rio-code
+00061700: 2d62 6c6f 636b 3e70 7265 7b6d 6172 6769  -block>pre{margi
+00061710: 6e3a 303b 666f 6e74 2d73 697a 653a 7661  n:0;font-size:va
+00061720: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d74  r(--rio-global-t
+00061730: 6578 742d 666f 6e74 2d73 697a 6529 3b66  ext-font-size);f
+00061740: 6f6e 742d 6661 6d69 6c79 3a76 6172 282d  ont-family:var(-
+00061750: 2d72 696f 2d67 6c6f 6261 6c2d 6d6f 6e6f  -rio-global-mono
+00061760: 7370 6163 652d 666f 6e74 292c 6d6f 6e6f  space-font),mono
+00061770: 7370 6163 653b 6469 7370 6c61 793a 626c  space;display:bl
+00061780: 6f63 6b7d 2e72 696f 2d6c 696e 6b7b 706f  ock}.rio-link{po
+00061790: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
+000617a0: 6f3b 6375 7273 6f72 3a70 6f69 6e74 6572  o;cursor:pointer
+000617b0: 3b64 6973 706c 6179 3a62 6c6f 636b 7d2e  ;display:block}.
+000617c0: 7269 6f2d 7465 7874 2d6c 696e 6b7b 636f  rio-text-link{co
+000617d0: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
+000617e0: 6361 6c2d 6c65 7665 6c2d 322d 6267 293b  cal-level-2-bg);
+000617f0: 6469 7370 6c61 793a 666c 6578 3b61 6c69  display:flex;ali
+00061800: 676e 2d69 7465 6d73 3a63 656e 7465 723b  gn-items:center;
+00061810: 6a75 7374 6966 792d 636f 6e74 656e 743a  justify-content:
+00061820: 6365 6e74 6572 7d2e 7269 6f2d 7363 726f  center}.rio-scro
+00061830: 6c6c 2d63 6f6e 7461 696e 6572 2c2e 7269  ll-container,.ri
+00061840: 6f2d 7363 726f 6c6c 2d74 6172 6765 747b  o-scroll-target{
+00061850: 706f 696e 7465 722d 6576 656e 7473 3a61  pointer-events:a
+00061860: 7574 6f7d 2e72 696f 2d73 6372 6f6c 6c2d  uto}.rio-scroll-
+00061870: 7461 7267 6574 3e2e 7269 6f2d 7363 726f  target>.rio-scro
+00061880: 6c6c 2d74 6172 6765 742d 7572 6c2d 636f  ll-target-url-co
+00061890: 7079 2d62 7574 746f 6e7b 6469 7370 6c61  py-button{displa
+000618a0: 793a 6e6f 6e65 7d2e 7269 6f2d 7363 726f  y:none}.rio-scro
+000618b0: 6c6c 2d74 6172 6765 743e 2e72 696f 2d73  ll-target>.rio-s
+000618c0: 6372 6f6c 6c2d 7461 7267 6574 2d75 726c  croll-target-url
+000618d0: 2d63 6f70 792d 6275 7474 6f6e 3e2a 7b70  -copy-button>*{p
+000618e0: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
+000618f0: 3b63 7572 736f 723a 706f 696e 7465 727d  ;cursor:pointer}
+00061900: 2e72 696f 2d73 6372 6f6c 6c2d 7461 7267  .rio-scroll-targ
+00061910: 6574 3a68 6f76 6572 3e2e 7269 6f2d 7363  et:hover>.rio-sc
+00061920: 726f 6c6c 2d74 6172 6765 742d 7572 6c2d  roll-target-url-
+00061930: 636f 7079 2d62 7574 746f 6e7b 6469 7370  copy-button{disp
+00061940: 6c61 793a 626c 6f63 6b7d 2e72 696f 2d63  lay:block}.rio-c
+00061950: 6f6c 6f72 2d70 6963 6b65 727b 706f 696e  olor-picker{poin
+00061960: 7465 722d 6576 656e 7473 3a6e 6f6e 653b  ter-events:none;
+00061970: 6469 7370 6c61 793a 666c 6578 3b66 6c65  display:flex;fle
+00061980: 782d 6469 7265 6374 696f 6e3a 636f 6c75  x-direction:colu
+00061990: 6d6e 3b61 6c69 676e 2d69 7465 6d73 3a73  mn;align-items:s
+000619a0: 7472 6574 6368 7d2e 7269 6f2d 636f 6c6f  tretch}.rio-colo
+000619b0: 722d 7069 636b 6572 2d63 6f6c 6f72 2d73  r-picker-color-s
+000619c0: 7175 6172 657b 706f 696e 7465 722d 6576  quare{pointer-ev
+000619d0: 656e 7473 3a61 7574 6f3b 706f 7369 7469  ents:auto;positi
+000619e0: 6f6e 3a72 656c 6174 6976 653b 6d69 6e2d  on:relative;min-
+000619f0: 6865 6967 6874 3a36 7265 6d3b 6375 7273  height:6rem;curs
+00061a00: 6f72 3a63 726f 7373 6861 6972 3b6d 6172  or:crosshair;mar
+00061a10: 6769 6e2d 626f 7474 6f6d 3a2e 3772 656d  gin-bottom:.7rem
+00061a20: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
+00061a30: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00061a40: 636f 726e 6572 2d72 6164 6975 732d 736d  corner-radius-sm
+00061a50: 616c 6c29 3b66 6c65 782d 6772 6f77 3a31  all);flex-grow:1
+00061a60: 7d2e 7269 6f2d 636f 6c6f 722d 7069 636b  }.rio-color-pick
+00061a70: 6572 2d73 6c69 6465 722d 6f75 7465 727b  er-slider-outer{
+00061a80: 706f 696e 7465 722d 6576 656e 7473 3a61  pointer-events:a
+00061a90: 7574 6f3b 706f 7369 7469 6f6e 3a72 656c  uto;position:rel
+00061aa0: 6174 6976 653b 7061 6464 696e 673a 2e37  ative;padding:.7
+00061ab0: 7265 6d20 307d 2e72 696f 2d63 6f6c 6f72  rem 0}.rio-color
+00061ac0: 2d73 6c69 6465 722d 696e 6e65 727b 6865  -slider-inner{he
+00061ad0: 6967 6874 3a2e 3972 656d 3b63 7572 736f  ight:.9rem;curso
+00061ae0: 723a 6372 6f73 7368 6169 723b 626f 7264  r:crosshair;bord
+00061af0: 6572 2d72 6164 6975 733a 3939 3939 3970  er-radius:99999p
+00061b00: 787d 2e72 696f 2d63 6f6c 6f72 2d70 6963  x}.rio-color-pic
+00061b10: 6b65 722d 6b6e 6f62 7b70 6f69 6e74 6572  ker-knob{pointer
+00061b20: 2d65 7665 6e74 733a 6e6f 6e65 3b63 7572  -events:none;cur
+00061b30: 736f 723a 6372 6f73 7368 6169 723b 7769  sor:crosshair;wi
+00061b40: 6474 683a 312e 3472 656d 3b68 6569 6768  dth:1.4rem;heigh
+00061b50: 743a 312e 3472 656d 3b62 6f72 6465 722d  t:1.4rem;border-
+00061b60: 7261 6469 7573 3a35 3025 3b62 6f72 6465  radius:50%;borde
+00061b70: 723a 2e32 7265 6d20 736f 6c69 6420 7661  r:.2rem solid va
+00061b80: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  r(--rio-local-te
+00061b90: 7874 2d63 6f6c 6f72 293b 706f 7369 7469  xt-color);positi
+00061ba0: 6f6e 3a61 6273 6f6c 7574 653b 7472 616e  on:absolute;tran
+00061bb0: 7366 6f72 6d3a 7472 616e 736c 6174 6528  sform:translate(
+00061bc0: 2d35 3025 2c2d 3530 2529 3b62 6f78 2d73  -50%,-50%);box-s
+00061bd0: 697a 696e 673a 626f 7264 6572 2d62 6f78  izing:border-box
+00061be0: 3b62 6163 6b67 726f 756e 643a 7661 7228  ;background:var(
+00061bf0: 2d2d 6368 6f73 656e 2d63 6f6c 6f72 2d6f  --chosen-color-o
+00061c00: 7061 7175 6529 7d2e 7269 6f2d 636f 6c6f  paque)}.rio-colo
+00061c10: 722d 7069 636b 6572 2d73 6c69 6465 722d  r-picker-slider-
+00061c20: 6f75 7465 723e 2e72 696f 2d63 6f6c 6f72  outer>.rio-color
+00061c30: 2d70 6963 6b65 722d 6b6e 6f62 7b74 6f70  -picker-knob{top
+00061c40: 3a35 3025 7d2e 636f 6c6f 722d 736c 6964  :50%}.color-slid
+00061c50: 6572 2d63 6865 636b 6572 737b 626f 7264  er-checkers{bord
+00061c60: 6572 2d72 6164 6975 733a 3939 3939 3970  er-radius:99999p
+00061c70: 787d 2e72 696f 2d63 6f6c 6f72 2d70 6963  x}.rio-color-pic
+00061c80: 6b65 722d 6875 652d 6261 723e 2e72 696f  ker-hue-bar>.rio
+00061c90: 2d63 6f6c 6f72 2d73 6c69 6465 722d 696e  -color-slider-in
+00061ca0: 6e65 727b 6261 636b 6772 6f75 6e64 3a6c  ner{background:l
+00061cb0: 696e 6561 722d 6772 6164 6965 6e74 2874  inear-gradient(t
+00061cc0: 6f20 7269 6768 742c 7265 642c 7965 6c6c  o right,red,yell
+00061cd0: 6f77 2c6c 696d 652c 6171 7561 2c62 6c75  ow,lime,aqua,blu
+00061ce0: 652c 6d61 6765 6e74 612c 7265 6429 7d2e  e,magenta,red)}.
+00061cf0: 7269 6f2d 636f 6c6f 722d 7069 636b 6572  rio-color-picker
+00061d00: 2d6f 7061 6369 7479 2d62 6172 3e2e 7269  -opacity-bar>.ri
+00061d10: 6f2d 636f 6c6f 722d 736c 6964 6572 2d69  o-color-slider-i
+00061d20: 6e6e 6572 3a6e 6f74 282e 7269 6f2d 6368  nner:not(.rio-ch
+00061d30: 6563 6b65 7265 6429 7b70 6f73 6974 696f  eckered){positio
+00061d40: 6e3a 6162 736f 6c75 7465 3b74 6f70 3a2e  n:absolute;top:.
+00061d50: 3772 656d 3b6c 6566 743a 303b 7269 6768  7rem;left:0;righ
+00061d60: 743a 303b 626f 7474 6f6d 3a2e 3772 656d  t:0;bottom:.7rem
+00061d70: 3b62 6163 6b67 726f 756e 643a 6c69 6e65  ;background:line
+00061d80: 6172 2d67 7261 6469 656e 7428 746f 2072  ar-gradient(to r
+00061d90: 6967 6874 2c74 7261 6e73 7061 7265 6e74  ight,transparent
+00061da0: 2c76 6172 282d 2d63 686f 7365 6e2d 636f  ,var(--chosen-co
+00061db0: 6c6f 722d 6f70 6171 7565 2929 7d2e 7269  lor-opaque))}.ri
+00061dc0: 6f2d 636f 6c6f 722d 7069 636b 6572 2d72  o-color-picker-r
+00061dd0: 6573 756c 742d 636f 6e74 6169 6e65 727b  esult-container{
+00061de0: 6d61 7267 696e 2d74 6f70 3a2e 3572 656d  margin-top:.5rem
+00061df0: 3b6d 6172 6769 6e2d 6c65 6674 3a61 7574  ;margin-left:aut
+00061e00: 6f3b 6d61 7267 696e 2d72 6967 6874 3a61  o;margin-right:a
+00061e10: 7574 6f3b 6469 7370 6c61 793a 666c 6578  uto;display:flex
+00061e20: 3b61 6c69 676e 2d69 7465 6d73 3a63 656e  ;align-items:cen
+00061e30: 7465 723b 6761 703a 2e38 7265 6d7d 2e72  ter;gap:.8rem}.r
+00061e40: 696f 2d63 6f6c 6f72 2d70 6963 6b65 722d  io-color-picker-
+00061e50: 7365 6c65 6374 6564 2d63 6f6c 6f72 2d63  selected-color-c
+00061e60: 6972 636c 657b 706f 7369 7469 6f6e 3a72  ircle{position:r
+00061e70: 656c 6174 6976 653b 7769 6474 683a 322e  elative;width:2.
+00061e80: 3572 656d 3b68 6569 6768 743a 322e 3572  5rem;height:2.5r
+00061e90: 656d 7d2e 7269 6f2d 636f 6c6f 722d 7069  em}.rio-color-pi
+00061ea0: 636b 6572 2d73 656c 6563 7465 642d 636f  cker-selected-co
+00061eb0: 6c6f 722d 6369 7263 6c65 3e2a 7b77 6964  lor-circle>*{wid
+00061ec0: 7468 3a31 3030 253b 6865 6967 6874 3a31  th:100%;height:1
+00061ed0: 3030 253b 626f 7264 6572 2d72 6164 6975  00%;border-radiu
+00061ee0: 733a 3530 253b 626f 782d 7369 7a69 6e67  s:50%;box-sizing
+00061ef0: 3a62 6f72 6465 722d 626f 783b 626f 7264  :border-box;bord
+00061f00: 6572 3a2e 3272 656d 2073 6f6c 6964 2076  er:.2rem solid v
+00061f10: 6172 282d 2d72 696f 2d6c 6f63 616c 2d74  ar(--rio-local-t
+00061f20: 6578 742d 636f 6c6f 7229 7d2e 7269 6f2d  ext-color)}.rio-
+00061f30: 636f 6c6f 722d 7069 636b 6572 2d73 656c  color-picker-sel
+00061f40: 6563 7465 642d 636f 6c6f 722d 6369 7263  ected-color-circ
+00061f50: 6c65 3e64 6976 3a66 6972 7374 2d63 6869  le>div:first-chi
+00061f60: 6c64 7b70 6f73 6974 696f 6e3a 6162 736f  ld{position:abso
+00061f70: 6c75 7465 3b74 6f70 3a30 3b6c 6566 743a  lute;top:0;left:
+00061f80: 303b 7269 6768 743a 303b 626f 7474 6f6d  0;right:0;bottom
+00061f90: 3a30 3b62 6163 6b67 726f 756e 643a 7661  :0;background:va
+00061fa0: 7228 2d2d 6368 6f73 656e 2d63 6f6c 6f72  r(--chosen-color
+00061fb0: 2d74 7261 6e73 7061 7265 6e74 297d 2e72  -transparent)}.r
+00061fc0: 696f 2d63 6f6c 6f72 2d70 6963 6b65 722d  io-color-picker-
+00061fd0: 7365 6c65 6374 6564 2d63 6f6c 6f72 2d63  selected-color-c
+00061fe0: 6972 636c 652d 636f 6c6f 727b 6261 636b  ircle-color{back
+00061ff0: 6772 6f75 6e64 3a76 6172 282d 2d63 686f  ground:var(--cho
+00062000: 7365 6e2d 636f 6c6f 722d 7472 616e 7370  sen-color-transp
+00062010: 6172 656e 7429 7d2e 7269 6f2d 636f 6c6f  arent)}.rio-colo
+00062020: 722d 7069 636b 6572 2d73 656c 6563 7465  r-picker-selecte
+00062030: 642d 636f 6c6f 722d 6c61 6265 6c7b 706f  d-color-label{po
+00062040: 696e 7465 722d 6576 656e 7473 3a61 7574  inter-events:aut
+00062050: 6f3b 6f70 6163 6974 793a 2e35 3b77 6964  o;opacity:.5;wid
+00062060: 7468 3a35 7265 6d3b 636f 6c6f 723a 7661  th:5rem;color:va
+00062070: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  r(--rio-local-te
+00062080: 7874 2d63 6f6c 6f72 293b 666f 6e74 2d73  xt-color);font-s
+00062090: 697a 653a 2e39 7265 6d3b 7465 7874 2d61  ize:.9rem;text-a
+000620a0: 6c69 676e 3a63 656e 7465 723b 666f 6e74  lign:center;font
+000620b0: 2d77 6569 6768 743a 3730 303b 6261 636b  -weight:700;back
+000620c0: 6772 6f75 6e64 3a74 7261 6e73 7061 7265  ground:transpare
+000620d0: 6e74 3b62 6f72 6465 723a 6e6f 6e65 3b70  nt;border:none;p
+000620e0: 6164 6469 6e67 3a2e 3372 656d 3b62 6f72  adding:.3rem;bor
+000620f0: 6465 722d 7261 6469 7573 3a2e 3572 656d  der-radius:.5rem
+00062100: 3b74 7261 6e73 6974 696f 6e3a 6f70 6163  ;transition:opac
+00062110: 6974 7920 2e31 7320 6561 7365 2d69 6e2d  ity .1s ease-in-
+00062120: 6f75 742c 636f 6c6f 7220 2e31 7320 6561  out,color .1s ea
+00062130: 7365 2d69 6e2d 6f75 742c 6261 636b 6772  se-in-out,backgr
+00062140: 6f75 6e64 2d63 6f6c 6f72 202e 3173 2065  ound-color .1s e
+00062150: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
+00062160: 636f 6c6f 722d 7069 636b 6572 2d73 656c  color-picker-sel
+00062170: 6563 7465 642d 636f 6c6f 722d 6c61 6265  ected-color-labe
+00062180: 6c3a 666f 6375 737b 6f75 746c 696e 653a  l:focus{outline:
+00062190: 6e6f 6e65 3b6f 7061 6369 7479 3a31 3b63  none;opacity:1;c
+000621a0: 6f6c 6f72 3a76 6172 282d 2d72 696f 2d6c  olor:var(--rio-l
+000621b0: 6f63 616c 2d6c 6576 656c 2d32 2d62 6729  ocal-level-2-bg)
+000621c0: 3b62 6163 6b67 726f 756e 643a 7661 7228  ;background:var(
+000621d0: 2d2d 7269 6f2d 6c6f 6361 6c2d 6267 2d76  --rio-local-bg-v
+000621e0: 6172 6961 6e74 297d 2e72 696f 2d63 6865  ariant)}.rio-che
+000621f0: 636b 6572 6564 7b2d 2d63 6865 636b 6572  ckered{--checker
+00062200: 2d63 6f6c 6f72 3a20 2338 3838 3b2d 2d63  -color: #888;--c
+00062210: 6865 636b 6572 2d73 697a 653a 202e 3972  hecker-size: .9r
+00062220: 656d 3b62 6163 6b67 726f 756e 642d 696d  em;background-im
+00062230: 6167 653a 6c69 6e65 6172 2d67 7261 6469  age:linear-gradi
+00062240: 656e 7428 3435 6465 672c 7661 7228 2d2d  ent(45deg,var(--
+00062250: 6368 6563 6b65 722d 636f 6c6f 7229 2032  checker-color) 2
+00062260: 3525 2c74 7261 6e73 7061 7265 6e74 2032  5%,transparent 2
+00062270: 3525 292c 6c69 6e65 6172 2d67 7261 6469  5%),linear-gradi
+00062280: 656e 7428 3435 6465 672c 7472 616e 7370  ent(45deg,transp
+00062290: 6172 656e 7420 3735 252c 7661 7228 2d2d  arent 75%,var(--
+000622a0: 6368 6563 6b65 722d 636f 6c6f 7229 2037  checker-color) 7
+000622b0: 3525 292c 6c69 6e65 6172 2d67 7261 6469  5%),linear-gradi
+000622c0: 656e 7428 3435 6465 672c 7472 616e 7370  ent(45deg,transp
+000622d0: 6172 656e 7420 3735 252c 7661 7228 2d2d  arent 75%,var(--
+000622e0: 6368 6563 6b65 722d 636f 6c6f 7229 2037  checker-color) 7
+000622f0: 3525 292c 6c69 6e65 6172 2d67 7261 6469  5%),linear-gradi
+00062300: 656e 7428 3435 6465 672c 7661 7228 2d2d  ent(45deg,var(--
+00062310: 6368 6563 6b65 722d 636f 6c6f 7229 2032  checker-color) 2
+00062320: 3525 2c74 7261 6e73 7061 7265 6e74 2032  5%,transparent 2
+00062330: 3525 293b 6261 636b 6772 6f75 6e64 2d73  5%);background-s
+00062340: 697a 653a 7661 7228 2d2d 6368 6563 6b65  ize:var(--checke
+00062350: 722d 7369 7a65 2920 7661 7228 2d2d 6368  r-size) var(--ch
+00062360: 6563 6b65 722d 7369 7a65 293b 6261 636b  ecker-size);back
+00062370: 6772 6f75 6e64 2d70 6f73 6974 696f 6e3a  ground-position:
+00062380: 3020 302c 3020 302c 6361 6c63 2876 6172  0 0,0 0,calc(var
+00062390: 282d 2d63 6865 636b 6572 2d73 697a 6529  (--checker-size)
+000623a0: 202a 202d 2e35 2920 6361 6c63 2876 6172   * -.5) calc(var
+000623b0: 282d 2d63 6865 636b 6572 2d73 697a 6529  (--checker-size)
+000623c0: 202a 202d 2e35 292c 6361 6c63 2876 6172   * -.5),calc(var
+000623d0: 282d 2d63 6865 636b 6572 2d73 697a 6529  (--checker-size)
+000623e0: 202a 202e 3529 2063 616c 6328 7661 7228   * .5) calc(var(
+000623f0: 2d2d 6368 6563 6b65 722d 7369 7a65 2920  --checker-size) 
+00062400: 2a20 2e35 297d 2e72 696f 2d64 7261 7765  * .5)}.rio-drawe
+00062410: 727b 706f 696e 7465 722d 6576 656e 7473  r{pointer-events
+00062420: 3a61 7574 6f3b 6f76 6572 666c 6f77 3a68  :auto;overflow:h
+00062430: 6964 6465 6e3b 6469 7370 6c61 793a 666c  idden;display:fl
+00062440: 6578 3b61 6c69 676e 2d69 7465 6d73 3a73  ex;align-items:s
+00062450: 7472 6574 6368 7d2e 7269 6f2d 6472 6177  tretch}.rio-draw
+00062460: 6572 2d73 6861 6465 7b70 6f69 6e74 6572  er-shade{pointer
+00062470: 2d65 7665 6e74 733a 6e6f 6e65 3b70 6f73  -events:none;pos
+00062480: 6974 696f 6e3a 6162 736f 6c75 7465 3b6c  ition:absolute;l
+00062490: 6566 743a 303b 746f 703a 303b 7269 6768  eft:0;top:0;righ
+000624a0: 743a 303b 626f 7474 6f6d 3a30 3b74 7261  t:0;bottom:0;tra
+000624b0: 6e73 6974 696f 6e3a 6261 636b 6772 6f75  nsition:backgrou
+000624c0: 6e64 2d63 6f6c 6f72 202e 3573 2065 6173  nd-color .5s eas
+000624d0: 652d 696e 2d6f 7574 7d2e 7269 6f2d 6472  e-in-out}.rio-dr
+000624e0: 6177 6572 2d61 6e63 686f 727b 706f 696e  awer-anchor{poin
+000624f0: 7465 722d 6576 656e 7473 3a6e 6f6e 653b  ter-events:none;
+00062500: 666c 6578 2d67 726f 773a 317d 2e72 696f  flex-grow:1}.rio
+00062510: 2d64 7261 7765 722d 636f 6e74 656e 742d  -drawer-content-
+00062520: 6f75 7465 727b 706f 696e 7465 722d 6576  outer{pointer-ev
+00062530: 656e 7473 3a61 7574 6f3b 6469 7370 6c61  ents:auto;displa
+00062540: 793a 666c 6578 3b70 6f73 6974 696f 6e3a  y:flex;position:
+00062550: 6162 736f 6c75 7465 3b62 6163 6b67 726f  absolute;backgro
+00062560: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
+00062570: 7269 6f2d 676c 6f62 616c 2d6e 6575 7472  rio-global-neutr
+00062580: 616c 2d62 6729 3b62 6f78 2d73 6861 646f  al-bg);box-shado
+00062590: 773a 3020 3020 3172 656d 2076 6172 282d  w:0 0 1rem var(-
+000625a0: 2d72 696f 2d67 6c6f 6261 6c2d 7368 6164  -rio-global-shad
+000625b0: 6f77 2d63 6f6c 6f72 293b 7472 616e 7369  ow-color);transi
+000625c0: 7469 6f6e 3a74 7261 6e73 666f 726d 202e  tion:transform .
+000625d0: 3573 2065 6173 652d 6f75 747d 2e72 696f  5s ease-out}.rio
+000625e0: 2d64 7261 7765 722d 636f 6e74 656e 742d  -drawer-content-
+000625f0: 696e 6e65 727b 6f72 6465 723a 317d 2e72  inner{order:1}.r
+00062600: 696f 2d64 7261 7765 722d 636f 6e74 656e  io-drawer-conten
+00062610: 742d 696e 6e65 723e 2a7b 706f 7369 7469  t-inner>*{positi
+00062620: 6f6e 3a72 656c 6174 6976 6521 696d 706f  on:relative!impo
+00062630: 7274 616e 747d 2e72 696f 2d64 7261 7765  rtant}.rio-drawe
+00062640: 722d 6b6e 6f62 7b61 6c69 676e 2d73 656c  r-knob{align-sel
+00062650: 663a 6365 6e74 6572 3b6d 6172 6769 6e3a  f:center;margin:
+00062660: 2e35 7265 6d3b 626f 7264 6572 2d72 6164  .5rem;border-rad
+00062670: 6975 733a 3939 3939 3970 783b 6261 636b  ius:99999px;back
+00062680: 6772 6f75 6e64 3a76 6172 282d 2d72 696f  ground:var(--rio
+00062690: 2d6c 6f63 616c 2d74 6578 742d 636f 6c6f  -local-text-colo
+000626a0: 7229 3b6f 7061 6369 7479 3a2e 3135 7d2e  r);opacity:.15}.
+000626b0: 7269 6f2d 6472 6177 6572 2d6c 6566 7420  rio-drawer-left 
+000626c0: 2e72 696f 2d64 7261 7765 722d 6b6e 6f62  .rio-drawer-knob
+000626d0: 2c2e 7269 6f2d 6472 6177 6572 2d72 6967  ,.rio-drawer-rig
+000626e0: 6874 202e 7269 6f2d 6472 6177 6572 2d6b  ht .rio-drawer-k
+000626f0: 6e6f 627b 7769 6474 683a 2e34 7265 6d3b  nob{width:.4rem;
+00062700: 6865 6967 6874 3a34 7265 6d7d 2e72 696f  height:4rem}.rio
+00062710: 2d64 7261 7765 722d 746f 7020 2e72 696f  -drawer-top .rio
+00062720: 2d64 7261 7765 722d 6b6e 6f62 2c2e 7269  -drawer-knob,.ri
+00062730: 6f2d 6472 6177 6572 2d62 6f74 746f 6d20  o-drawer-bottom 
+00062740: 2e72 696f 2d64 7261 7765 722d 6b6e 6f62  .rio-drawer-knob
+00062750: 7b77 6964 7468 3a34 7265 6d3b 6865 6967  {width:4rem;heig
+00062760: 6874 3a2e 3472 656d 7d2e 7269 6f2d 6472  ht:.4rem}.rio-dr
+00062770: 6177 6572 2d74 6f70 202e 7269 6f2d 6472  awer-top .rio-dr
+00062780: 6177 6572 2d63 6f6e 7465 6e74 2d6f 7574  awer-content-out
+00062790: 6572 2c2e 7269 6f2d 6472 6177 6572 2d62  er,.rio-drawer-b
+000627a0: 6f74 746f 6d20 2e72 696f 2d64 7261 7765  ottom .rio-drawe
+000627b0: 722d 636f 6e74 656e 742d 6f75 7465 727b  r-content-outer{
+000627c0: 666c 6578 2d64 6972 6563 7469 6f6e 3a63  flex-direction:c
+000627d0: 6f6c 756d 6e7d 2e72 696f 2d64 7261 7765  olumn}.rio-drawe
+000627e0: 722d 6c65 6674 202e 7269 6f2d 6472 6177  r-left .rio-draw
+000627f0: 6572 2d6b 6e6f 622c 2e72 696f 2d64 7261  er-knob,.rio-dra
+00062800: 7765 722d 746f 7020 2e72 696f 2d64 7261  wer-top .rio-dra
+00062810: 7765 722d 6b6e 6f62 7b6f 7264 6572 3a32  wer-knob{order:2
+00062820: 7d2e 7269 6f2d 6472 6177 6572 2d72 6967  }.rio-drawer-rig
+00062830: 6874 202e 7269 6f2d 6472 6177 6572 2d6b  ht .rio-drawer-k
+00062840: 6e6f 622c 2e72 696f 2d64 7261 7765 722d  nob,.rio-drawer-
+00062850: 626f 7474 6f6d 202e 7269 6f2d 6472 6177  bottom .rio-draw
+00062860: 6572 2d6b 6e6f 627b 6f72 6465 723a 307d  er-knob{order:0}
+00062870: 2e72 696f 2d64 7261 7765 722d 6c65 6674  .rio-drawer-left
+00062880: 3e2e 7269 6f2d 6472 6177 6572 2d63 6f6e  >.rio-drawer-con
+00062890: 7465 6e74 2d6f 7574 6572 7b74 6f70 3a30  tent-outer{top:0
+000628a0: 3b6c 6566 743a 303b 626f 7474 6f6d 3a30  ;left:0;bottom:0
+000628b0: 3b77 6964 7468 3a66 6974 2d63 6f6e 7465  ;width:fit-conte
+000628c0: 6e74 3b62 6f72 6465 722d 7261 6469 7573  nt;border-radius
+000628d0: 3a30 2076 6172 282d 2d72 696f 2d67 6c6f  :0 var(--rio-glo
+000628e0: 6261 6c2d 636f 726e 6572 2d72 6164 6975  bal-corner-radiu
+000628f0: 732d 6c61 7267 6529 2076 6172 282d 2d72  s-large) var(--r
+00062900: 696f 2d67 6c6f 6261 6c2d 636f 726e 6572  io-global-corner
+00062910: 2d72 6164 6975 732d 6c61 7267 6529 2030  -radius-large) 0
+00062920: 7d2e 7269 6f2d 6472 6177 6572 2d72 6967  }.rio-drawer-rig
+00062930: 6874 3e2e 7269 6f2d 6472 6177 6572 2d63  ht>.rio-drawer-c
+00062940: 6f6e 7465 6e74 2d6f 7574 6572 7b74 6f70  ontent-outer{top
+00062950: 3a30 3b72 6967 6874 3a30 3b62 6f74 746f  :0;right:0;botto
+00062960: 6d3a 303b 7769 6474 683a 6669 742d 636f  m:0;width:fit-co
+00062970: 6e74 656e 743b 626f 7264 6572 2d72 6164  ntent;border-rad
+00062980: 6975 733a 7661 7228 2d2d 7269 6f2d 676c  ius:var(--rio-gl
+00062990: 6f62 616c 2d63 6f72 6e65 722d 7261 6469  obal-corner-radi
+000629a0: 7573 2d6c 6172 6765 2920 3020 3020 7661  us-large) 0 0 va
+000629b0: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d63  r(--rio-global-c
+000629c0: 6f72 6e65 722d 7261 6469 7573 2d6c 6172  orner-radius-lar
+000629d0: 6765 297d 2e72 696f 2d64 7261 7765 722d  ge)}.rio-drawer-
+000629e0: 746f 703e 2e72 696f 2d64 7261 7765 722d  top>.rio-drawer-
+000629f0: 636f 6e74 656e 742d 6f75 7465 727b 6c65  content-outer{le
+00062a00: 6674 3a30 3b74 6f70 3a30 3b72 6967 6874  ft:0;top:0;right
+00062a10: 3a30 3b68 6569 6768 743a 6669 742d 636f  :0;height:fit-co
+00062a20: 6e74 656e 743b 626f 7264 6572 2d72 6164  ntent;border-rad
+00062a30: 6975 733a 3020 3020 7661 7228 2d2d 7269  ius:0 0 var(--ri
+00062a40: 6f2d 676c 6f62 616c 2d63 6f72 6e65 722d  o-global-corner-
+00062a50: 7261 6469 7573 2d6c 6172 6765 2920 7661  radius-large) va
+00062a60: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d63  r(--rio-global-c
+00062a70: 6f72 6e65 722d 7261 6469 7573 2d6c 6172  orner-radius-lar
+00062a80: 6765 297d 2e72 696f 2d64 7261 7765 722d  ge)}.rio-drawer-
+00062a90: 626f 7474 6f6d 3e2e 7269 6f2d 6472 6177  bottom>.rio-draw
+00062aa0: 6572 2d63 6f6e 7465 6e74 2d6f 7574 6572  er-content-outer
+00062ab0: 7b6c 6566 743a 303b 626f 7474 6f6d 3a30  {left:0;bottom:0
+00062ac0: 3b72 6967 6874 3a30 3b68 6569 6768 743a  ;right:0;height:
+00062ad0: 6669 742d 636f 6e74 656e 743b 626f 7264  fit-content;bord
+00062ae0: 6572 2d72 6164 6975 733a 7661 7228 2d2d  er-radius:var(--
+00062af0: 7269 6f2d 676c 6f62 616c 2d63 6f72 6e65  rio-global-corne
+00062b00: 722d 7261 6469 7573 2d6c 6172 6765 2920  r-radius-large) 
+00062b10: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00062b20: 2d63 6f72 6e65 722d 7261 6469 7573 2d6c  -corner-radius-l
+00062b30: 6172 6765 2920 3020 307d 2e72 696f 2d64  arge) 0 0}.rio-d
+00062b40: 7261 7765 722d 6e6f 2d74 7261 6e73 6974  rawer-no-transit
+00062b50: 696f 6e7b 7472 616e 7369 7469 6f6e 3a6e  ion{transition:n
+00062b60: 6f6e 6521 696d 706f 7274 616e 747d 2e72  one!important}.r
+00062b70: 696f 2d64 7261 7765 722d 6e6f 2d74 7261  io-drawer-no-tra
+00062b80: 6e73 6974 696f 6e3e 2a7b 7472 616e 7369  nsition>*{transi
+00062b90: 7469 6f6e 3a6e 6f6e 6521 696d 706f 7274  tion:none!import
+00062ba0: 616e 747d 2e72 696f 2d70 6f70 7570 7b7a  ant}.rio-popup{z
+00062bb0: 2d69 6e64 6578 3a31 3030 3033 7d2e 7269  -index:10003}.ri
+00062bc0: 6f2d 706f 7075 702d 616e 6368 6f72 3e2a  o-popup-anchor>*
+00062bd0: 2c2e 7269 6f2d 706f 7075 702d 636f 6e74  ,.rio-popup-cont
+00062be0: 656e 743e 2a7b 706f 7369 7469 6f6e 3a72  ent>*{position:r
+00062bf0: 656c 6174 6976 6521 696d 706f 7274 616e  elative!importan
+00062c00: 747d 2e72 696f 2d70 6f70 7570 2d63 6f6e  t}.rio-popup-con
+00062c10: 7465 6e74 7b70 6f73 6974 696f 6e3a 6669  tent{position:fi
+00062c20: 7865 643b 7769 6474 683a 6d69 6e2d 636f  xed;width:min-co
+00062c30: 6e74 656e 743b 6865 6967 6874 3a6d 696e  ntent;height:min
+00062c40: 2d63 6f6e 7465 6e74 3b62 6163 6b67 726f  -content;backgro
+00062c50: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
+00062c60: 7269 6f2d 6c6f 6361 6c2d 6267 293b 626f  rio-local-bg);bo
+00062c70: 7264 6572 2d72 6164 6975 733a 7661 7228  rder-radius:var(
+00062c80: 2d2d 7269 6f2d 676c 6f62 616c 2d63 6f72  --rio-global-cor
+00062c90: 6e65 722d 7261 6469 7573 2d6d 6564 6975  ner-radius-mediu
+00062ca0: 6d29 3b62 6f78 2d73 6861 646f 773a 3020  m);box-shadow:0 
+00062cb0: 3020 3172 656d 2076 6172 282d 2d72 696f  0 1rem var(--rio
+00062cc0: 2d67 6c6f 6261 6c2d 7368 6164 6f77 2d63  -global-shadow-c
+00062cd0: 6f6c 6f72 293b 7472 616e 7366 6f72 6d3a  olor);transform:
+00062ce0: 7363 616c 6528 3029 3b6f 7061 6369 7479  scale(0);opacity
+00062cf0: 3a30 3b74 7261 6e73 6974 696f 6e3a 7472  :0;transition:tr
+00062d00: 616e 7366 6f72 6d20 2e32 7320 6c69 6e65  ansform .2s line
+00062d10: 6172 2c6f 7061 6369 7479 202e 3173 2065  ar,opacity .1s e
+00062d20: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
+00062d30: 706f 7075 702d 6f70 656e 3e2e 7269 6f2d  popup-open>.rio-
+00062d40: 706f 7075 702d 636f 6e74 656e 747b 7472  popup-content{tr
+00062d50: 616e 7366 6f72 6d3a 7363 616c 6528 3129  ansform:scale(1)
+00062d60: 3b6f 7061 6369 7479 3a31 3b74 7261 6e73  ;opacity:1;trans
+00062d70: 6974 696f 6e3a 7472 616e 7366 6f72 6d20  ition:transform 
+00062d80: 2e32 7320 6375 6269 632d 6265 7a69 6572  .2s cubic-bezier
+00062d90: 282e 352c 2e35 2c2e 322c 312e 3134 292c  (.5,.5,.2,1.14),
+00062da0: 6f70 6163 6974 7920 2e31 7320 6561 7365  opacity .1s ease
+00062db0: 2d69 6e2d 6f75 747d 2e72 696f 2d69 6d61  -in-out}.rio-ima
+00062dc0: 6765 7b70 6f69 6e74 6572 2d65 7665 6e74  ge{pointer-event
+00062dd0: 733a 6175 746f 3b64 6973 706c 6179 3a66  s:auto;display:f
+00062de0: 6c65 783b 6a75 7374 6966 792d 636f 6e74  lex;justify-cont
+00062df0: 656e 743a 6365 6e74 6572 3b61 6c69 676e  ent:center;align
+00062e00: 2d69 7465 6d73 3a63 656e 7465 727d 2e72  -items:center}.r
+00062e10: 696f 2d69 6d61 6765 2069 6d67 7b77 6964  io-image img{wid
+00062e20: 7468 3a31 3030 253b 6865 6967 6874 3a31  th:100%;height:1
+00062e30: 3030 253b 6f62 6a65 6374 2d66 6974 3a63  00%;object-fit:c
+00062e40: 6f6e 7461 696e 7d2e 7269 6f2d 696d 6167  ontain}.rio-imag
+00062e50: 6520 7376 677b 6d61 782d 7769 6474 683a  e svg{max-width:
+00062e60: 3372 656d 7d2e 7269 6f2d 6361 7264 7b70  3rem}.rio-card{p
+00062e70: 6f69 6e74 6572 2d65 7665 6e74 733a 6175  ointer-events:au
+00062e80: 746f 3b62 6163 6b67 726f 756e 642d 636f  to;background-co
+00062e90: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
+00062ea0: 6361 6c2d 6267 293b 626f 782d 7368 6164  cal-bg);box-shad
+00062eb0: 6f77 3a30 2030 2030 2076 6172 282d 2d72  ow:0 0 0 var(--r
+00062ec0: 696f 2d67 6c6f 6261 6c2d 7368 6164 6f77  io-global-shadow
+00062ed0: 2d63 6f6c 6f72 293b 7472 616e 7369 7469  -color);transiti
+00062ee0: 6f6e 3a62 6f78 2d73 6861 646f 7720 2e31  on:box-shadow .1
+00062ef0: 3573 2065 6173 652d 6f75 742c 6261 636b  5s ease-out,back
+00062f00: 6772 6f75 6e64 2d63 6f6c 6f72 202e 3173  ground-color .1s
+00062f10: 2065 6173 652d 6f75 747d 2e72 696f 2d63   ease-out}.rio-c
+00062f20: 6172 642d 656c 6576 6174 652d 6f6e 2d68  ard-elevate-on-h
+00062f30: 6f76 6572 3a68 6f76 6572 7b62 6f78 2d73  over:hover{box-s
+00062f40: 6861 646f 773a 3020 2e31 3572 656d 202e  hadow:0 .15rem .
+00062f50: 3372 656d 2076 6172 282d 2d72 696f 2d67  3rem var(--rio-g
+00062f60: 6c6f 6261 6c2d 7368 6164 6f77 2d63 6f6c  lobal-shadow-col
+00062f70: 6f72 297d 2e72 696f 2d63 6172 642d 636f  or)}.rio-card-co
+00062f80: 6c6f 7269 7a65 2d6f 6e2d 686f 7665 723a  lorize-on-hover:
+00062f90: 686f 7665 727b 6261 636b 6772 6f75 6e64  hover{background
+00062fa0: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
+00062fb0: 2d6c 6f63 616c 2d62 672d 6163 7469 7665  -local-bg-active
+00062fc0: 297d 2e72 696f 2d63 6172 642d 7269 7070  )}.rio-card-ripp
+00062fd0: 6c65 7b6f 7665 7266 6c6f 773a 6869 6464  le{overflow:hidd
+00062fe0: 656e 7d2e 7269 6f2d 7377 6974 6368 6572  en}.rio-switcher
+00062ff0: 2d62 6172 7b64 6973 706c 6179 3a66 6c65  -bar{display:fle
+00063000: 783b 616c 6967 6e2d 6974 656d 733a 6365  x;align-items:ce
+00063010: 6e74 6572 7d2e 7269 6f2d 7377 6974 6368  nter}.rio-switch
+00063020: 6572 2d62 6172 3e64 6976 7b70 6f73 6974  er-bar>div{posit
+00063030: 696f 6e3a 7265 6c61 7469 7665 7d2e 7269  ion:relative}.ri
+00063040: 6f2d 7377 6974 6368 6572 2d62 6172 3e64  o-switcher-bar>d
+00063050: 6976 3e2e 7269 6f2d 7377 6974 6368 6572  iv>.rio-switcher
+00063060: 2d62 6172 2d6f 7074 696f 6e73 7b70 6f73  -bar-options{pos
+00063070: 6974 696f 6e3a 7265 6c61 7469 7665 2169  ition:relative!i
+00063080: 6d70 6f72 7461 6e74 7d2e 7269 6f2d 7377  mportant}.rio-sw
+00063090: 6974 6368 6572 2d62 6172 2d6f 7074 696f  itcher-bar-optio
+000630a0: 6e73 7b70 6f69 6e74 6572 2d65 7665 6e74  ns{pointer-event
+000630b0: 733a 6175 746f 3b70 6f73 6974 696f 6e3a  s:auto;position:
+000630c0: 6162 736f 6c75 7465 3b64 6973 706c 6179  absolute;display
+000630d0: 3a66 6c65 783b 616c 6967 6e2d 6974 656d  :flex;align-item
+000630e0: 733a 7374 7265 7463 683b 6a75 7374 6966  s:stretch;justif
+000630f0: 792d 636f 6e74 656e 743a 7370 6163 652d  y-content:space-
+00063100: 6265 7477 6565 6e7d 2e72 696f 2d73 7769  between}.rio-swi
+00063110: 7463 6865 722d 6261 722d 6f70 7469 6f6e  tcher-bar-option
+00063120: 7b64 6973 706c 6179 3a66 6c65 783b 666c  {display:flex;fl
+00063130: 6578 2d64 6972 6563 7469 6f6e 3a63 6f6c  ex-direction:col
+00063140: 756d 6e3b 616c 6967 6e2d 6974 656d 733a  umn;align-items:
+00063150: 6365 6e74 6572 3b6a 7573 7469 6679 2d63  center;justify-c
+00063160: 6f6e 7465 6e74 3a73 7061 6365 2d62 6574  ontent:space-bet
+00063170: 7765 656e 3b63 7572 736f 723a 706f 696e  ween;cursor:poin
+00063180: 7465 723b 626f 7264 6572 2d72 6164 6975  ter;border-radiu
+00063190: 733a 7661 7228 2d2d 7269 6f2d 676c 6f62  s:var(--rio-glob
+000631a0: 616c 2d63 6f72 6e65 722d 7261 6469 7573  al-corner-radius
+000631b0: 2d6c 6172 6765 293b 636f 6c6f 723a 7661  -large);color:va
+000631c0: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 7465  r(--rio-local-te
+000631d0: 7874 2d63 6f6c 6f72 293b 7472 616e 7369  xt-color);transi
+000631e0: 7469 6f6e 3a62 6163 6b67 726f 756e 642d  tion:background-
+000631f0: 636f 6c6f 7220 2e31 7320 6561 7365 2d6f  color .1s ease-o
+00063200: 7574 7d2e 7269 6f2d 7377 6974 6368 6572  ut}.rio-switcher
+00063210: 2d62 6172 2d6f 7074 696f 6e3a 686f 7665  -bar-option:hove
+00063220: 727b 6261 636b 6772 6f75 6e64 2d63 6f6c  r{background-col
+00063230: 6f72 3a76 6172 282d 2d72 696f 2d6c 6f63  or:var(--rio-loc
+00063240: 616c 2d62 672d 6163 7469 7665 297d 2e72  al-bg-active)}.r
+00063250: 696f 2d73 7769 7463 6865 722d 6261 722d  io-switcher-bar-
+00063260: 6d61 726b 6572 3e2e 7269 6f2d 7377 6974  marker>.rio-swit
+00063270: 6368 6572 2d62 6172 2d6f 7074 696f 6e73  cher-bar-options
+00063280: 3e2e 7269 6f2d 7377 6974 6368 6572 2d62  >.rio-switcher-b
+00063290: 6172 2d6f 7074 696f 6e7b 6261 636b 6772  ar-option{backgr
+000632a0: 6f75 6e64 2d63 6f6c 6f72 3a75 6e73 6574  ound-color:unset
+000632b0: 2169 6d70 6f72 7461 6e74 7d2e 7269 6f2d  !important}.rio-
+000632c0: 7377 6974 6368 6572 2d62 6172 2d6f 7074  switcher-bar-opt
+000632d0: 696f 6e3e 6469 767b 6d61 7267 696e 2d6c  ion>div{margin-l
+000632e0: 6566 743a 6175 746f 3b6d 6172 6769 6e2d  eft:auto;margin-
+000632f0: 7269 6768 743a 6175 746f 3b77 6869 7465  right:auto;white
+00063300: 2d73 7061 6365 3a6e 6f77 7261 707d 2e72  -space:nowrap}.r
+00063310: 696f 2d73 7769 7463 6865 722d 6261 722d  io-switcher-bar-
+00063320: 6d61 726b 6572 7b70 6f69 6e74 6572 2d65  marker{pointer-e
+00063330: 7665 6e74 733a 6e6f 6e65 3b62 6163 6b67  vents:none;backg
+00063340: 726f 756e 643a 7661 7228 2d2d 7269 6f2d  round:var(--rio-
+00063350: 6c6f 6361 6c2d 6267 293b 6f76 6572 666c  local-bg);overfl
+00063360: 6f77 3a68 6964 6465 6e3b 706f 7369 7469  ow:hidden;positi
+00063370: 6f6e 3a61 6273 6f6c 7574 653b 6c65 6674  on:absolute;left
+00063380: 3a30 3b74 6f70 3a30 3b62 6f72 6465 722d  :0;top:0;border-
+00063390: 7261 6469 7573 3a76 6172 282d 2d72 696f  radius:var(--rio
+000633a0: 2d67 6c6f 6261 6c2d 636f 726e 6572 2d72  -global-corner-r
+000633b0: 6164 6975 732d 6c61 7267 6529 7d2e 7269  adius-large)}.ri
+000633c0: 6f2d 7461 626c 657b 706f 696e 7465 722d  o-table{pointer-
+000633d0: 6576 656e 7473 3a61 7574 6f3b 6469 7370  events:auto;disp
+000633e0: 6c61 793a 6772 6964 7d2e 7269 6f2d 7461  lay:grid}.rio-ta
+000633f0: 626c 653e 2a7b 7061 6464 696e 673a 2e35  ble>*{padding:.5
+00063400: 7265 6d20 2e38 7265 6d7d 2e72 696f 2d74  rem .8rem}.rio-t
+00063410: 6162 6c65 202e 6865 6164 6572 7b64 6973  able .header{dis
+00063420: 706c 6179 3a66 6c65 783b 6375 7273 6f72  play:flex;cursor
+00063430: 3a70 6f69 6e74 6572 7d2e 7269 6f2d 7461  :pointer}.rio-ta
+00063440: 626c 6520 2e68 6561 6465 723a 6166 7465  ble .header:afte
+00063450: 727b 636f 6e74 656e 743a 22e2 96b4 223b  r{content:"...";
+00063460: 6469 7370 6c61 793a 696e 6c69 6e65 2d62  display:inline-b
+00063470: 6c6f 636b 3b6d 6172 6769 6e2d 6c65 6674  lock;margin-left
+00063480: 3a2e 3372 656d 3b6f 7061 6369 7479 3a30  :.3rem;opacity:0
+00063490: 7d2e 7269 6f2d 7461 626c 6520 2e68 6561  }.rio-table .hea
+000634a0: 6465 725b 6461 7461 2d73 6f72 743d 6173  der[data-sort=as
+000634b0: 6365 6e64 696e 675d 3a61 6674 6572 7b63  cending]:after{c
+000634c0: 6f6e 7465 6e74 3a22 e296 b422 3b6f 7061  ontent:"...";opa
+000634d0: 6369 7479 3a31 7d2e 7269 6f2d 7461 626c  city:1}.rio-tabl
+000634e0: 6520 2e68 6561 6465 725b 6461 7461 2d73  e .header[data-s
+000634f0: 6f72 743d 6465 7363 656e 6469 6e67 5d3a  ort=descending]:
+00063500: 6166 7465 727b 636f 6e74 656e 743a 22e2  after{content:".
+00063510: 96be 223b 6f70 6163 6974 793a 317d 2e72  ..";opacity:1}.r
+00063520: 696f 2d6c 6973 742d 7669 6577 7b70 6f69  io-list-view{poi
+00063530: 6e74 6572 2d65 7665 6e74 733a 6e6f 6e65  nter-events:none
+00063540: 3b64 6973 706c 6179 3a66 6c65 783b 666c  ;display:flex;fl
+00063550: 6578 2d64 6972 6563 7469 6f6e 3a63 6f6c  ex-direction:col
+00063560: 756d 6e3b 616c 6967 6e2d 6974 656d 733a  umn;align-items:
+00063570: 7374 7265 7463 687d 2e72 696f 2d68 6561  stretch}.rio-hea
+00063580: 6469 6e67 2d6c 6973 742d 6974 656d 7b70  ding-list-item{p
+00063590: 6f69 6e74 6572 2d65 7665 6e74 733a 6e6f  ointer-events:no
+000635a0: 6e65 3b62 6f78 2d73 697a 696e 673a 626f  ne;box-sizing:bo
+000635b0: 7264 6572 2d62 6f78 7d2e 7269 6f2d 6c69  rder-box}.rio-li
+000635c0: 7374 7669 6577 2d67 726f 7570 6564 7b70  stview-grouped{p
+000635d0: 6f69 6e74 6572 2d65 7665 6e74 733a 6175  ointer-events:au
+000635e0: 746f 3b62 6163 6b67 726f 756e 642d 636f  to;background-co
+000635f0: 6c6f 723a 7661 7228 2d2d 7269 6f2d 6c6f  lor:var(--rio-lo
+00063600: 6361 6c2d 6267 2d76 6172 6961 6e74 293b  cal-bg-variant);
+00063610: 7472 616e 7369 7469 6f6e 3a62 6163 6b67  transition:backg
+00063620: 726f 756e 642d 636f 6c6f 7220 2e31 7320  round-color .1s 
+00063630: 6561 7365 2d6f 7574 7d2e 7269 6f2d 6c69  ease-out}.rio-li
+00063640: 7374 7669 6577 2d67 726f 7570 6564 2b2e  stview-grouped+.
+00063650: 7269 6f2d 6c69 7374 7669 6577 2d67 726f  rio-listview-gro
+00063660: 7570 6564 3a61 6674 6572 7b63 6f6e 7465  uped:after{conte
+00063670: 6e74 3a22 223b 706f 7369 7469 6f6e 3a61  nt:"";position:a
+00063680: 6273 6f6c 7574 653b 746f 703a 303b 6c65  bsolute;top:0;le
+00063690: 6674 3a30 3b72 6967 6874 3a30 3b68 6569  ft:0;right:0;hei
+000636a0: 6768 743a 3170 783b 6261 636b 6772 6f75  ght:1px;backgrou
+000636b0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
+000636c0: 696f 2d6c 6f63 616c 2d74 6578 742d 636f  io-local-text-co
+000636d0: 6c6f 7229 3b6f 7061 6369 7479 3a2e 327d  lor);opacity:.2}
+000636e0: 2e72 696f 2d6c 6973 742d 6974 656d 2d72  .rio-list-item-r
+000636f0: 6970 706c 657b 6f76 6572 666c 6f77 3a68  ipple{overflow:h
+00063700: 6964 6465 6e7d 2e72 696f 2d6c 6973 742d  idden}.rio-list-
+00063710: 6974 656d 2d72 6970 706c 653a 686f 7665  item-ripple:hove
+00063720: 727b 6261 636b 6772 6f75 6e64 3a76 6172  r{background:var
+00063730: 282d 2d72 696f 2d6c 6f63 616c 2d62 672d  (--rio-local-bg-
+00063740: 6163 7469 7665 297d 2e72 696f 2d66 6c6f  active)}.rio-flo
+00063750: 772d 636f 6e74 6169 6e65 727b 6469 7370  w-container{disp
+00063760: 6c61 793a 666c 6578 3b66 6c65 782d 7772  lay:flex;flex-wr
+00063770: 6170 3a77 7261 707d 2e72 696f 2d66 6c6f  ap:wrap}.rio-flo
+00063780: 772d 636f 6e74 6169 6e65 723e 2a7b 7472  w-container>*{tr
+00063790: 616e 7369 7469 6f6e 3a6c 6566 7420 2e32  ansition:left .2
+000637a0: 7320 6561 7365 2d6f 7574 2c74 6f70 202e  s ease-out,top .
+000637b0: 3273 2065 6173 652d 6f75 747d 2e72 696f  2s ease-out}.rio
+000637c0: 2d63 6f6e 6e65 6374 696f 6e2d 6c6f 7374  -connection-lost
+000637d0: 2d70 6f70 7570 7b70 6f69 6e74 6572 2d65  -popup{pointer-e
+000637e0: 7665 6e74 733a 6e6f 6e65 3b70 6f73 6974  vents:none;posit
+000637f0: 696f 6e3a 6669 7865 643b 6c65 6674 3a30  ion:fixed;left:0
+00063800: 3b74 6f70 3a30 3b77 6964 7468 3a31 3030  ;top:0;width:100
+00063810: 7677 3b68 6569 6768 743a 3130 3076 683b  vw;height:100vh;
+00063820: 7a2d 696e 6465 783a 3130 3030 343b 6261  z-index:10004;ba
+00063830: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a74  ckground-color:t
+00063840: 7261 6e73 7061 7265 6e74 3b74 7261 6e73  ransparent;trans
+00063850: 6974 696f 6e3a 6261 636b 6772 6f75 6e64  ition:background
+00063860: 2d63 6f6c 6f72 2031 7320 6561 7365 2d69  -color 1s ease-i
+00063870: 6e2d 6f75 747d 2e72 696f 2d63 6f6e 6e65  n-out}.rio-conne
+00063880: 6374 696f 6e2d 6c6f 7374 2d70 6f70 7570  ction-lost-popup
+00063890: 2e72 696f 2d63 6f6e 6e65 6374 696f 6e2d  .rio-connection-
+000638a0: 6c6f 7374 2d70 6f70 7570 2d76 6973 6962  lost-popup-visib
+000638b0: 6c65 7b64 6973 706c 6179 3a66 6c65 783b  le{display:flex;
+000638c0: 616c 6967 6e2d 6974 656d 733a 7374 7265  align-items:stre
+000638d0: 7463 683b 6261 636b 6772 6f75 6e64 2d63  tch;background-c
+000638e0: 6f6c 6f72 3a23 3030 3030 3030 3830 7d2e  olor:#00000080}.
+000638f0: 7269 6f2d 636f 6e6e 6563 7469 6f6e 2d6c  rio-connection-l
+00063900: 6f73 742d 706f 7075 703e 2a7b 706f 7369  ost-popup>*{posi
+00063910: 7469 6f6e 3a61 6273 6f6c 7574 653b 666c  tion:absolute;fl
+00063920: 6578 2d67 726f 773a 313b 6c65 6674 3a30  ex-grow:1;left:0
+00063930: 3b74 6f70 3a30 3b77 6964 7468 3a31 3030  ;top:0;width:100
+00063940: 253b 6865 6967 6874 3a31 3030 253b 6f70  %;height:100%;op
+00063950: 6163 6974 793a 303b 7472 616e 7366 6f72  acity:0;transfor
+00063960: 6d3a 7472 616e 736c 6174 6559 282d 3572  m:translateY(-5r
+00063970: 656d 293b 7472 616e 7369 7469 6f6e 3a6f  em);transition:o
+00063980: 7061 6369 7479 202e 3373 2065 6173 652d  pacity .3s ease-
+00063990: 696e 2d6f 7574 2c74 7261 6e73 666f 726d  in-out,transform
+000639a0: 202e 3373 2063 7562 6963 2d62 657a 6965   .3s cubic-bezie
+000639b0: 7228 2e35 2c2e 352c 2e32 2c31 2e31 3429  r(.5,.5,.2,1.14)
+000639c0: 7d2e 7269 6f2d 636f 6e6e 6563 7469 6f6e  }.rio-connection
+000639d0: 2d6c 6f73 742d 706f 7075 702e 7269 6f2d  -lost-popup.rio-
+000639e0: 636f 6e6e 6563 7469 6f6e 2d6c 6f73 742d  connection-lost-
+000639f0: 706f 7075 702d 7669 7369 626c 653e 2a7b  popup-visible>*{
+00063a00: 6f70 6163 6974 793a 313b 7472 616e 7366  opacity:1;transf
+00063a10: 6f72 6d3a 7472 616e 736c 6174 6559 2830  orm:translateY(0
+00063a20: 297d 2e72 696f 2d74 7261 6365 6261 636b  )}.rio-traceback
+00063a30: 7b70 6f69 6e74 6572 2d65 7665 6e74 733a  {pointer-events:
+00063a40: 6175 746f 3b70 6f73 6974 696f 6e3a 7265  auto;position:re
+00063a50: 6c61 7469 7665 3b6c 6566 743a 3530 253b  lative;left:50%;
+00063a60: 746f 703a 3572 656d 3b77 6964 7468 3a66  top:5rem;width:f
+00063a70: 6974 2d63 6f6e 7465 6e74 3b6d 6178 2d77  it-content;max-w
+00063a80: 6964 7468 3a35 3072 656d 3b70 6164 6469  idth:50rem;paddi
+00063a90: 6e67 3a32 2e32 7265 6d3b 6f76 6572 666c  ng:2.2rem;overfl
+00063aa0: 6f77 3a68 6964 6465 6e3b 6469 7370 6c61  ow:hidden;displa
+00063ab0: 793a 666c 6578 3b66 6c65 782d 6469 7265  y:flex;flex-dire
+00063ac0: 6374 696f 6e3a 636f 6c75 6d6e 3b61 6c69  ction:column;ali
+00063ad0: 676e 2d69 7465 6d73 3a73 7472 6574 6368  gn-items:stretch
+00063ae0: 3b67 6170 3a31 2e35 7265 6d3b 626f 7264  ;gap:1.5rem;bord
+00063af0: 6572 2d72 6164 6975 733a 7661 7228 2d2d  er-radius:var(--
+00063b00: 7269 6f2d 676c 6f62 616c 2d63 6f72 6e65  rio-global-corne
+00063b10: 722d 7261 6469 7573 2d6c 6172 6765 293b  r-radius-large);
+00063b20: 626f 782d 7368 6164 6f77 3a30 202e 3472  box-shadow:0 .4r
+00063b30: 656d 2031 7265 6d20 7661 7228 2d2d 7269  em 1rem var(--ri
+00063b40: 6f2d 676c 6f62 616c 2d73 6861 646f 772d  o-global-shadow-
+00063b50: 636f 6c6f 7229 3b74 7261 6e73 666f 726d  color);transform
+00063b60: 3a74 7261 6e73 6c61 7465 282d 3530 2529  :translate(-50%)
+00063b70: 7d2e 7269 6f2d 7472 6163 6562 6163 6b2d  }.rio-traceback-
+00063b80: 6865 6164 6572 7b64 6973 706c 6179 3a66  header{display:f
+00063b90: 6c65 783b 616c 6967 6e2d 6974 656d 733a  lex;align-items:
+00063ba0: 6365 6e74 6572 3b67 6170 3a2e 3672 656d  center;gap:.6rem
+00063bb0: 7d2e 7269 6f2d 7472 6163 6562 6163 6b2d  }.rio-traceback-
+00063bc0: 6865 6164 6572 3e73 7667 7b77 6964 7468  header>svg{width
+00063bd0: 3a32 2e35 7265 6d3b 6865 6967 6874 3a32  :2.5rem;height:2
+00063be0: 2e35 7265 6d3b 6669 6c6c 3a76 6172 282d  .5rem;fill:var(-
+00063bf0: 2d72 696f 2d67 6c6f 6261 6c2d 6461 6e67  -rio-global-dang
+00063c00: 6572 2d62 6729 7d2e 7269 6f2d 7472 6163  er-bg)}.rio-trac
+00063c10: 6562 6163 6b2d 6865 6164 6572 3e64 6976  eback-header>div
+00063c20: 7b66 6c65 782d 6772 6f77 3a31 3b74 6578  {flex-grow:1;tex
+00063c30: 742d 616c 6967 6e3a 6c65 6674 3b66 6f6e  t-align:left;fon
+00063c40: 742d 7369 7a65 3a31 2e38 7265 6d3b 636f  t-size:1.8rem;co
+00063c50: 6c6f 723a 7661 7228 2d2d 7269 6f2d 676c  lor:var(--rio-gl
+00063c60: 6f62 616c 2d64 616e 6765 722d 6267 297d  obal-danger-bg)}
+00063c70: 2e72 696f 2d74 7261 6365 6261 636b 2d74  .rio-traceback-t
+00063c80: 7261 6365 6261 636b 7b66 6f6e 742d 6661  raceback{font-fa
+00063c90: 6d69 6c79 3a76 6172 282d 2d72 696f 2d67  mily:var(--rio-g
+00063ca0: 6c6f 6261 6c2d 6d6f 6e6f 7370 6163 652d  lobal-monospace-
+00063cb0: 666f 6e74 292c 6d6f 6e6f 7370 6163 653b  font),monospace;
+00063cc0: 666f 6e74 2d73 697a 653a 2e39 7265 6d3b  font-size:.9rem;
+00063cd0: 7768 6974 652d 7370 6163 653a 7072 652d  white-space:pre-
+00063ce0: 7772 6170 3b6f 7665 7266 6c6f 772d 7772  wrap;overflow-wr
+00063cf0: 6170 3a62 7265 616b 2d77 6f72 643b 7061  ap:break-word;pa
+00063d00: 6464 696e 673a 2e35 7265 6d20 3172 656d  dding:.5rem 1rem
+00063d10: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
+00063d20: 723a 7661 7228 2d2d 7269 6f2d 6c6f 6361  r:var(--rio-loca
+00063d30: 6c2d 6267 2d76 6172 6961 6e74 293b 626f  l-bg-variant);bo
+00063d40: 7264 6572 2d72 6164 6975 733a 7661 7228  rder-radius:var(
+00063d50: 2d2d 7269 6f2d 676c 6f62 616c 2d63 6f72  --rio-global-cor
+00063d60: 6e65 722d 7261 6469 7573 2d73 6d61 6c6c  ner-radius-small
+00063d70: 297d 2e72 696f 2d74 7261 6365 6261 636b  )}.rio-traceback
+00063d80: 2d66 6f6f 7465 727b 6469 7370 6c61 793a  -footer{display:
+00063d90: 666c 6578 3b66 6c65 782d 6469 7265 6374  flex;flex-direct
+00063da0: 696f 6e3a 636f 6c75 6d6e 3b67 6170 3a2e  ion:column;gap:.
+00063db0: 3572 656d 7d2e 7269 6f2d 7472 6163 6562  5rem}.rio-traceb
+00063dc0: 6163 6b2d 666f 6f74 6572 2d6c 696e 6b73  ack-footer-links
+00063dd0: 7b64 6973 706c 6179 3a66 6c65 783b 666c  {display:flex;fl
+00063de0: 6578 2d64 6972 6563 7469 6f6e 3a72 6f77  ex-direction:row
+00063df0: 3b67 6170 3a2e 3572 656d 3b6a 7573 7469  ;gap:.5rem;justi
+00063e00: 6679 2d63 6f6e 7465 6e74 3a73 7061 6365  fy-content:space
+00063e10: 2d62 6574 7765 656e 7d2e 7269 6f2d 7472  -between}.rio-tr
+00063e20: 6163 6562 6163 6b2d 666f 6f74 6572 3e61  aceback-footer>a
+00063e30: 7b66 6c65 783a 317d 2e72 696f 2d74 7261  {flex:1}.rio-tra
+00063e40: 6365 6261 636b 2d62 6f6c 647b 666f 6e74  ceback-bold{font
+00063e50: 2d77 6569 6768 743a 3730 307d 2e72 696f  -weight:700}.rio
+00063e60: 2d74 7261 6365 6261 636b 2d64 696d 7b6f  -traceback-dim{o
+00063e70: 7061 6369 7479 3a2e 357d 2e72 696f 2d74  pacity:.5}.rio-t
+00063e80: 7261 6365 6261 636b 2d72 6564 7b63 6f6c  raceback-red{col
+00063e90: 6f72 3a76 6172 282d 2d72 696f 2d67 6c6f  or:var(--rio-glo
+00063ea0: 6261 6c2d 6461 6e67 6572 2d62 6729 7d2e  bal-danger-bg)}.
+00063eb0: 7269 6f2d 7472 6163 6562 6163 6b2d 7965  rio-traceback-ye
+00063ec0: 6c6c 6f77 7b63 6f6c 6f72 3a76 6172 282d  llow{color:var(-
+00063ed0: 2d72 696f 2d67 6c6f 6261 6c2d 7761 726e  -rio-global-warn
+00063ee0: 696e 672d 6267 297d 2e72 696f 2d64 6562  ing-bg)}.rio-deb
+00063ef0: 7567 6765 727b 6261 636b 6772 6f75 6e64  ugger{background
+00063f00: 3a76 6172 282d 2d72 696f 2d67 6c6f 6261  :var(--rio-globa
+00063f10: 6c2d 6261 636b 6772 6f75 6e64 2d62 6729  l-background-bg)
+00063f20: 3b7a 2d69 6e64 6578 3a31 3030 3032 7d2e  ;z-index:10002}.
+00063f30: 7269 6f2d 6465 6275 6767 6572 2d6e 6176  rio-debugger-nav
+00063f40: 6967 6174 696f 6e2d 7269 6f2d 6c6f 676f  igation-rio-logo
+00063f50: 7b70 6f69 6e74 6572 2d65 7665 6e74 733a  {pointer-events:
+00063f60: 6175 746f 3b64 6973 706c 6179 3a66 6c65  auto;display:fle
+00063f70: 783b 666c 6578 2d64 6972 6563 7469 6f6e  x;flex-direction
+00063f80: 3a63 6f6c 756d 6e3b 616c 6967 6e2d 6974  :column;align-it
+00063f90: 656d 733a 6365 6e74 6572 3b6a 7573 7469  ems:center;justi
+00063fa0: 6679 2d63 6f6e 7465 6e74 3a65 6e64 3b67  fy-content:end;g
+00063fb0: 6170 3a2e 3335 7265 6d3b 7a2d 696e 6465  ap:.35rem;z-inde
+00063fc0: 783a 323b 7465 7874 2d64 6563 6f72 6174  x:2;text-decorat
+00063fd0: 696f 6e3a 6e6f 6e65 7d2e 7269 6f2d 6465  ion:none}.rio-de
+00063fe0: 6275 6767 6572 2d6e 6176 6967 6174 696f  bugger-navigatio
+00063ff0: 6e2d 7269 6f2d 6c6f 676f 2069 6d67 7b77  n-rio-logo img{w
+00064000: 6964 7468 3a32 2e35 7265 6d3b 6865 6967  idth:2.5rem;heig
+00064010: 6874 3a32 2e35 7265 6d3b 6f62 6a65 6374  ht:2.5rem;object
+00064020: 2d66 6974 3a63 6f6e 7461 696e 7d2e 7269  -fit:contain}.ri
+00064030: 6f2d 6465 6275 6767 6572 2d6e 6176 6967  o-debugger-navig
+00064040: 6174 696f 6e2d 7269 6f2d 6c6f 676f 2064  ation-rio-logo d
+00064050: 6976 7b6d 6172 6769 6e2d 626f 7474 6f6d  iv{margin-bottom
+00064060: 3a31 7265 6d3b 666f 6e74 2d73 697a 653a  :1rem;font-size:
+00064070: 312e 3272 656d 3b63 6f6c 6f72 3a76 6172  1.2rem;color:var
+00064080: 282d 2d72 696f 2d6c 6f63 616c 2d74 6578  (--rio-local-tex
+00064090: 742d 636f 6c6f 7229 3b74 7261 6e73 6974  t-color);transit
+000640a0: 696f 6e3a 636f 6c6f 7220 3173 2065 6173  ion:color 1s eas
+000640b0: 652d 696e 2d6f 7574 7d2e 7269 6f2d 6465  e-in-out}.rio-de
+000640c0: 6275 6767 6572 2d6e 6176 6967 6174 696f  bugger-navigatio
+000640d0: 6e2d 7269 6f2d 6c6f 676f 3a68 6f76 6572  n-rio-logo:hover
+000640e0: 2064 6976 7b63 6f6c 6f72 3a76 6172 282d   div{color:var(-
+000640f0: 2d72 696f 2d67 6c6f 6261 6c2d 7365 636f  -rio-global-seco
+00064100: 6e64 6172 792d 6667 293b 7472 616e 7369  ndary-fg);transi
+00064110: 7469 6f6e 3a63 6f6c 6f72 202e 3173 2065  tion:color .1s e
+00064120: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
+00064130: 6465 6275 6767 6572 2d6e 6176 6967 6174  debugger-navigat
+00064140: 696f 6e2d 7269 6f2d 6c6f 676f 3a62 6566  ion-rio-logo:bef
+00064150: 6f72 657b 636f 6e74 656e 743a 2222 3b70  ore{content:"";p
+00064160: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
+00064170: 3b74 6f70 3a30 3b72 6967 6874 3a30 3b62  ;top:0;right:0;b
+00064180: 6f74 746f 6d3a 303b 6c65 6674 3a30 3b7a  ottom:0;left:0;z
+00064190: 2d69 6e64 6578 3a2d 313b 6261 636b 6772  -index:-1;backgr
+000641a0: 6f75 6e64 3a6c 696e 6561 722d 6772 6164  ound:linear-grad
+000641b0: 6965 6e74 2874 6f20 746f 702c 7661 7228  ient(to top,var(
+000641c0: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
+000641d0: 6f6e 6461 7279 2d62 6729 2c74 7261 6e73  ondary-bg),trans
+000641e0: 7061 7265 6e74 293b 6f70 6163 6974 793a  parent);opacity:
+000641f0: 303b 7472 616e 7369 7469 6f6e 3a6f 7061  0;transition:opa
+00064200: 6369 7479 2031 7320 6561 7365 2d6f 7574  city 1s ease-out
+00064210: 7d2e 7269 6f2d 6465 6275 6767 6572 2d6e  }.rio-debugger-n
+00064220: 6176 6967 6174 696f 6e2d 7269 6f2d 6c6f  avigation-rio-lo
+00064230: 676f 3a68 6f76 6572 3a62 6566 6f72 657b  go:hover:before{
+00064240: 6f70 6163 6974 793a 313b 7472 616e 7369  opacity:1;transi
+00064250: 7469 6f6e 3a6f 7061 6369 7479 202e 3173  tion:opacity .1s
+00064260: 2065 6173 652d 6f75 747d 2e72 696f 2d64   ease-out}.rio-d
+00064270: 6562 7567 6765 722d 7472 6565 2d63 6f6d  ebugger-tree-com
+00064280: 706f 6e65 6e74 2d74 7265 657b 6f76 6572  ponent-tree{over
+00064290: 666c 6f77 3a61 7574 6f7d 2e72 696f 2d64  flow:auto}.rio-d
+000642a0: 6562 7567 6765 722d 7472 6565 2d63 6f6d  ebugger-tree-com
+000642b0: 706f 6e65 6e74 2d74 7265 653e 2a7b 706f  ponent-tree>*{po
+000642c0: 7369 7469 6f6e 3a61 6273 6f6c 7574 653b  sition:absolute;
+000642d0: 7769 6474 683a 3130 3025 3b68 6569 6768  width:100%;heigh
+000642e0: 743a 3130 3025 3b6f 7665 7266 6c6f 772d  t:100%;overflow-
+000642f0: 783a 6869 6464 656e 3b6f 7665 7266 6c6f  x:hidden;overflo
+00064300: 772d 793a 6175 746f 7d2e 7269 6f2d 6465  w-y:auto}.rio-de
+00064310: 6275 6767 6572 2d63 6f6d 706f 6e65 6e74  bugger-component
+00064320: 2d74 7265 652d 6974 656d 7b64 6973 706c  -tree-item{displ
+00064330: 6179 3a66 6c65 783b 666c 6578 2d64 6972  ay:flex;flex-dir
+00064340: 6563 7469 6f6e 3a63 6f6c 756d 6e3b 6761  ection:column;ga
+00064350: 703a 2e32 7265 6d7d 406b 6579 6672 616d  p:.2rem}@keyfram
+00064360: 6573 2066 6c61 7368 2d74 6578 747b 3025  es flash-text{0%
+00064370: 7b63 6f6c 6f72 3a69 6e69 7469 616c 7d32  {color:initial}2
+00064380: 3025 7b63 6f6c 6f72 3a76 6172 282d 2d72  0%{color:var(--r
+00064390: 696f 2d67 6c6f 6261 6c2d 7761 726e 696e  io-global-warnin
+000643a0: 672d 6267 297d 746f 7b63 6f6c 6f72 3a69  g-bg)}to{color:i
+000643b0: 6e69 7469 616c 7d7d 2e72 696f 2d64 6562  nitial}}.rio-deb
+000643c0: 7567 6765 722d 636f 6d70 6f6e 656e 742d  ugger-component-
+000643d0: 7472 6565 2d66 6c61 7368 7b61 6e69 6d61  tree-flash{anima
+000643e0: 7469 6f6e 3a66 6c61 7368 2d74 6578 7420  tion:flash-text 
+000643f0: 3373 206c 696e 6561 727d 2e72 696f 2d64  3s linear}.rio-d
+00064400: 6562 7567 6765 722d 636f 6d70 6f6e 656e  ebugger-componen
+00064410: 742d 7472 6565 2d69 7465 6d2d 6865 6164  t-tree-item-head
+00064420: 6572 7b70 6f69 6e74 6572 2d65 7665 6e74  er{pointer-event
+00064430: 733a 6175 746f 3b63 7572 736f 723a 706f  s:auto;cursor:po
+00064440: 696e 7465 723b 7a2d 696e 6465 783a 313b  inter;z-index:1;
+00064450: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+00064460: 653b 7061 6464 696e 673a 2e33 7265 6d20  e;padding:.3rem 
+00064470: 2e36 7265 6d3b 6469 7370 6c61 793a 666c  .6rem;display:fl
+00064480: 6578 3b66 6c65 782d 6469 7265 6374 696f  ex;flex-directio
+00064490: 6e3a 726f 773b 616c 6967 6e2d 6974 656d  n:row;align-item
+000644a0: 733a 6365 6e74 6572 3b67 6170 3a2e 3572  s:center;gap:.5r
+000644b0: 656d 7d2e 7269 6f2d 6465 6275 6767 6572  em}.rio-debugger
+000644c0: 2d63 6f6d 706f 6e65 6e74 2d74 7265 652d  -component-tree-
+000644d0: 6974 656d 3e2e 7269 6f2d 6465 6275 6767  item>.rio-debugg
 000644e0: 6572 2d63 6f6d 706f 6e65 6e74 2d74 7265  er-component-tre
-000644f0: 652d 6974 656d 5b64 6174 612d 6578 7061  e-item[data-expa
-00064500: 6e64 6564 3d74 7275 655d 3e2e 7269 6f2d  nded=true]>.rio-
-00064510: 6465 6275 6767 6572 2d63 6f6d 706f 6e65  debugger-compone
-00064520: 6e74 2d74 7265 652d 6974 656d 2d68 6561  nt-tree-item-hea
-00064530: 6465 723e 6469 763a 6669 7273 742d 6368  der>div:first-ch
-00064540: 696c 647b 7472 616e 7366 6f72 6d3a 726f  ild{transform:ro
-00064550: 7461 7465 2839 3064 6567 297d 2e72 696f  tate(90deg)}.rio
-00064560: 2d64 6562 7567 6765 722d 636f 6d70 6f6e  -debugger-compon
-00064570: 656e 742d 7472 6565 2d69 7465 6d2d 6865  ent-tree-item-he
-00064580: 6164 6572 3a61 6674 6572 7b70 6f69 6e74  ader:after{point
-00064590: 6572 2d65 7665 6e74 733a 6e6f 6e65 3b63  er-events:none;c
-000645a0: 6f6e 7465 6e74 3a22 223b 6469 7370 6c61  ontent:"";displa
-000645b0: 793a 626c 6f63 6b3b 7a2d 696e 6465 783a  y:block;z-index:
-000645c0: 2d31 3b70 6f73 6974 696f 6e3a 6162 736f  -1;position:abso
-000645d0: 6c75 7465 3b6c 6566 743a 303b 746f 703a  lute;left:0;top:
-000645e0: 303b 7269 6768 743a 303b 626f 7474 6f6d  0;right:0;bottom
-000645f0: 3a30 3b62 6163 6b67 726f 756e 643a 7661  :0;background:va
-00064600: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-00064610: 6563 6f6e 6461 7279 2d62 6729 3b62 6f72  econdary-bg);bor
-00064620: 6465 722d 7261 6469 7573 3a39 3939 3939  der-radius:99999
-00064630: 7078 3b6f 7061 6369 7479 3a30 3b74 7261  px;opacity:0;tra
-00064640: 6e73 6974 696f 6e3a 6f70 6163 6974 7920  nsition:opacity 
-00064650: 2e31 7320 6561 7365 2d69 6e2d 6f75 747d  .1s ease-in-out}
-00064660: 2e72 696f 2d64 6562 7567 6765 722d 636f  .rio-debugger-co
-00064670: 6d70 6f6e 656e 742d 7472 6565 2d69 7465  mponent-tree-ite
-00064680: 6d2d 6865 6164 6572 3e64 6976 3e73 7667  m-header>div>svg
-00064690: 7b77 6964 7468 3a31 7265 6d3b 6865 6967  {width:1rem;heig
-000646a0: 6874 3a31 7265 6d7d 2e72 696f 2d64 6562  ht:1rem}.rio-deb
-000646b0: 7567 6765 722d 636f 6d70 6f6e 656e 742d  ugger-component-
-000646c0: 7472 6565 2d69 7465 6d2d 6865 6164 6572  tree-item-header
-000646d0: 2d77 6561 6b6c 792d 7365 6c65 6374 6564  -weakly-selected
-000646e0: 7b66 6f6e 742d 7765 6967 6874 3a37 3030  {font-weight:700
-000646f0: 7d2e 7269 6f2d 6465 6275 6767 6572 2d63  }.rio-debugger-c
-00064700: 6f6d 706f 6e65 6e74 2d74 7265 652d 6974  omponent-tree-it
-00064710: 656d 2d68 6561 6465 722d 7374 726f 6e67  em-header-strong
-00064720: 6c79 2d73 656c 6563 7465 647b 666f 6e74  ly-selected{font
-00064730: 2d77 6569 6768 743a 3730 303b 636f 6c6f  -weight:700;colo
-00064740: 723a 7661 7228 2d2d 7269 6f2d 676c 6f62  r:var(--rio-glob
-00064750: 616c 2d73 6563 6f6e 6461 7279 2d66 6729  al-secondary-fg)
-00064760: 7d2e 7269 6f2d 6465 6275 6767 6572 2d63  }.rio-debugger-c
-00064770: 6f6d 706f 6e65 6e74 2d74 7265 652d 6974  omponent-tree-it
-00064780: 656d 2d68 6561 6465 723a 686f 7665 723a  em-header:hover:
-00064790: 6166 7465 727b 6f70 6163 6974 793a 2e34  after{opacity:.4
-000647a0: 7d2e 7269 6f2d 6465 6275 6767 6572 2d63  }.rio-debugger-c
-000647b0: 6f6d 706f 6e65 6e74 2d74 7265 652d 6974  omponent-tree-it
-000647c0: 656d 2d68 6561 6465 722d 7765 616b 6c79  em-header-weakly
-000647d0: 2d73 656c 6563 7465 643a 6166 7465 727b  -selected:after{
-000647e0: 6f70 6163 6974 793a 2e31 357d 2e72 696f  opacity:.15}.rio
-000647f0: 2d64 6562 7567 6765 722d 636f 6d70 6f6e  -debugger-compon
-00064800: 656e 742d 7472 6565 2d69 7465 6d2d 6865  ent-tree-item-he
-00064810: 6164 6572 2d73 7472 6f6e 676c 792d 7365  ader-strongly-se
-00064820: 6c65 6374 6564 3a61 6674 6572 7b6f 7061  lected:after{opa
-00064830: 6369 7479 3a2e 367d 2e72 696f 2d64 6562  city:.6}.rio-deb
-00064840: 7567 6765 722d 636f 6d70 6f6e 656e 742d  ugger-component-
-00064850: 7472 6565 2d69 7465 6d2d 6865 6164 6572  tree-item-header
-00064860: 2d73 7472 6f6e 676c 792d 7365 6c65 6374  -strongly-select
-00064870: 6564 3a68 6f76 6572 3a61 6674 6572 7b6f  ed:hover:after{o
-00064880: 7061 6369 7479 3a2e 387d 2e72 696f 2d64  pacity:.8}.rio-d
-00064890: 6562 7567 6765 722d 636f 6d70 6f6e 656e  ebugger-componen
-000648a0: 742d 7472 6565 2d69 7465 6d2d 6368 696c  t-tree-item-chil
-000648b0: 6472 656e 7b6d 6172 6769 6e2d 6c65 6674  dren{margin-left
-000648c0: 3a2e 3772 656d 3b64 6973 706c 6179 3a6e  :.7rem;display:n
-000648d0: 6f6e 653b 666c 6578 2d64 6972 6563 7469  one;flex-directi
-000648e0: 6f6e 3a63 6f6c 756d 6e3b 6761 703a 2e32  on:column;gap:.2
-000648f0: 7265 6d7d 2e72 696f 2d64 6562 7567 6765  rem}.rio-debugge
-00064900: 722d 636f 6d70 6f6e 656e 742d 7472 6565  r-component-tree
-00064910: 2d69 7465 6d5b 6461 7461 2d68 6173 2d63  -item[data-has-c
-00064920: 6869 6c64 7265 6e3d 7472 7565 5d5b 6461  hildren=true][da
-00064930: 7461 2d65 7870 616e 6465 643d 7472 7565  ta-expanded=true
-00064940: 5d3e 2e72 696f 2d64 6562 7567 6765 722d  ]>.rio-debugger-
-00064950: 636f 6d70 6f6e 656e 742d 7472 6565 2d69  component-tree-i
-00064960: 7465 6d2d 6368 696c 6472 656e 7b64 6973  tem-children{dis
-00064970: 706c 6179 3a66 6c65 787d 2e72 696f 2d64  play:flex}.rio-d
-00064980: 6562 7567 6765 722d 636f 6d70 6f6e 656e  ebugger-componen
-00064990: 742d 6869 6768 6c69 6768 7465 727b 706f  t-highlighter{po
-000649a0: 696e 7465 722d 6576 656e 7473 3a6e 6f6e  inter-events:non
-000649b0: 653b 706f 7369 7469 6f6e 3a66 6978 6564  e;position:fixed
-000649c0: 3b7a 2d69 6e64 6578 3a31 3030 3031 3b74  ;z-index:10001;t
-000649d0: 7261 6e73 6974 696f 6e3a 6c65 6674 202e  ransition:left .
-000649e0: 3373 2065 6173 652d 696e 2d6f 7574 2c74  3s ease-in-out,t
-000649f0: 6f70 202e 3373 2065 6173 652d 696e 2d6f  op .3s ease-in-o
-00064a00: 7574 2c77 6964 7468 202e 3373 2065 6173  ut,width .3s eas
-00064a10: 652d 696e 2d6f 7574 2c68 6569 6768 7420  e-in-out,height 
-00064a20: 2e33 7320 6561 7365 2d69 6e2d 6f75 747d  .3s ease-in-out}
-00064a30: 406b 6579 6672 616d 6573 2070 756c 7365  @keyframes pulse
-00064a40: 7b30 257b 6c65 6674 3a2d 2e33 7265 6d3b  {0%{left:-.3rem;
-00064a50: 746f 703a 2d2e 3372 656d 3b72 6967 6874  top:-.3rem;right
-00064a60: 3a2d 2e33 7265 6d3b 626f 7474 6f6d 3a2d  :-.3rem;bottom:-
-00064a70: 2e33 7265 6d3b 626f 7264 6572 2d77 6964  .3rem;border-wid
-00064a80: 7468 3a2e 3472 656d 7d35 3025 7b6c 6566  th:.4rem}50%{lef
-00064a90: 743a 2d2e 3772 656d 3b74 6f70 3a2d 2e37  t:-.7rem;top:-.7
-00064aa0: 7265 6d3b 7269 6768 743a 2d2e 3772 656d  rem;right:-.7rem
-00064ab0: 3b62 6f74 746f 6d3a 2d2e 3772 656d 3b62  ;bottom:-.7rem;b
-00064ac0: 6f72 6465 722d 7769 6474 683a 2e33 7265  order-width:.3re
-00064ad0: 6d7d 746f 7b6c 6566 743a 2d2e 3372 656d  m}to{left:-.3rem
-00064ae0: 3b74 6f70 3a2d 2e33 7265 6d3b 7269 6768  ;top:-.3rem;righ
-00064af0: 743a 2d2e 3372 656d 3b62 6f74 746f 6d3a  t:-.3rem;bottom:
-00064b00: 2d2e 3372 656d 3b62 6f72 6465 722d 7769  -.3rem;border-wi
-00064b10: 6474 683a 2e34 7265 6d7d 7d2e 7269 6f2d  dth:.4rem}}.rio-
-00064b20: 6465 6275 6767 6572 2d63 6f6d 706f 6e65  debugger-compone
-00064b30: 6e74 2d68 6967 686c 6967 6874 6572 3a61  nt-highlighter:a
-00064b40: 6674 6572 7b63 6f6e 7465 6e74 3a22 223b  fter{content:"";
-00064b50: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
-00064b60: 653b 6469 7370 6c61 793a 626c 6f63 6b3b  e;display:block;
-00064b70: 626f 7264 6572 2d72 6164 6975 733a 3172  border-radius:1r
-00064b80: 656d 3b62 6f78 2d73 6861 646f 773a 3020  em;box-shadow:0 
-00064b90: 3020 3020 3939 3939 7265 6d20 2330 3030  0 0 9999rem #000
-00064ba0: 393b 626f 7264 6572 2d73 7479 6c65 3a73  9;border-style:s
-00064bb0: 6f6c 6964 3b62 6f72 6465 722d 636f 6c6f  olid;border-colo
-00064bc0: 723a 7661 7228 2d2d 7269 6f2d 676c 6f62  r:var(--rio-glob
-00064bd0: 616c 2d73 6563 6f6e 6461 7279 2d62 6729  al-secondary-bg)
-00064be0: 3b61 6e69 6d61 7469 6f6e 3a70 756c 7365  ;animation:pulse
-00064bf0: 2031 2e34 7320 696e 6669 6e69 7465 7d2e   1.4s infinite}.
-00064c00: 7269 6f2d 6465 6275 6767 6572 2d62 6163  rio-debugger-bac
-00064c10: 6b67 726f 756e 647b 7a2d 696e 6465 783a  kground{z-index:
-00064c20: 2d31 3b70 6f73 6974 696f 6e3a 7265 6c61  -1;position:rela
-00064c30: 7469 7665 3b62 6163 6b67 726f 756e 643a  tive;background:
-00064c40: 7661 7228 2d2d 7269 6f2d 6c6f 6361 6c2d  var(--rio-local-
-00064c50: 6267 297d 2e72 696f 2d64 6562 7567 6765  bg)}.rio-debugge
-00064c60: 722d 6261 636b 6772 6f75 6e64 3a61 6674  r-background:aft
-00064c70: 6572 7b63 6f6e 7465 6e74 3a22 223b 706f  er{content:"";po
-00064c80: 7369 7469 6f6e 3a61 6273 6f6c 7574 653b  sition:absolute;
-00064c90: 6469 7370 6c61 793a 626c 6f63 6b3b 7a2d  display:block;z-
-00064ca0: 696e 6465 783a 2d31 3b6c 6566 743a 303b  index:-1;left:0;
-00064cb0: 746f 703a 303b 626f 7474 6f6d 3a30 3b72  top:0;bottom:0;r
-00064cc0: 6967 6874 3a30 3b62 6163 6b67 726f 756e  ight:0;backgroun
-00064cd0: 642d 696d 6167 653a 6c69 6e65 6172 2d67  d-image:linear-g
-00064ce0: 7261 6469 656e 7428 2d34 3564 6567 2c76  radient(-45deg,v
-00064cf0: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
-00064d00: 6729 2032 3525 2c76 6172 282d 2d72 696f  g) 25%,var(--rio
-00064d10: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
-00064d20: 792d 6267 2920 3235 252c 7661 7228 2d2d  y-bg) 25%,var(--
-00064d30: 7269 6f2d 676c 6f62 616c 2d73 6563 6f6e  rio-global-secon
-00064d40: 6461 7279 2d62 6729 2035 3025 2c76 6172  dary-bg) 50%,var
-00064d50: 282d 2d72 696f 2d6c 6f63 616c 2d62 6729  (--rio-local-bg)
-00064d60: 2035 3025 2c76 6172 282d 2d72 696f 2d6c   50%,var(--rio-l
-00064d70: 6f63 616c 2d62 6729 2037 3525 2c76 6172  ocal-bg) 75%,var
-00064d80: 282d 2d72 696f 2d67 6c6f 6261 6c2d 7365  (--rio-global-se
-00064d90: 636f 6e64 6172 792d 6267 2920 3735 252c  condary-bg) 75%,
-00064da0: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00064db0: 2d73 6563 6f6e 6461 7279 2d62 6729 293b  -secondary-bg));
-00064dc0: 6261 636b 6772 6f75 6e64 2d73 697a 653a  background-size:
-00064dd0: 3372 656d 2033 7265 6d3b 6f70 6163 6974  3rem 3rem;opacit
-00064de0: 793a 2e30 337d 2e72 696f 2d73 7769 7463  y:.03}.rio-switc
-00064df0: 6865 727b 6f76 6572 666c 6f77 3a68 6964  her{overflow:hid
-00064e00: 6465 6e7d 2e72 696f 2d74 6f6f 6c74 6970  den}.rio-tooltip
-00064e10: 7b70 6f69 6e74 6572 2d65 7665 6e74 733a  {pointer-events:
-00064e20: 6e6f 6e65 3b70 6f73 6974 696f 6e3a 7265  none;position:re
-00064e30: 6c61 7469 7665 7d2e 7269 6f2d 746f 6f6c  lative}.rio-tool
-00064e40: 7469 702d 616e 6368 6f72 7b70 6f69 6e74  tip-anchor{point
-00064e50: 6572 2d65 7665 6e74 733a 6175 746f 3b70  er-events:auto;p
-00064e60: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
-00064e70: 7d2e 7269 6f2d 746f 6f6c 7469 702d 616e  }.rio-tooltip-an
-00064e80: 6368 6f72 3e2a 2c2e 7269 6f2d 746f 6f6c  chor>*,.rio-tool
-00064e90: 7469 702d 6c61 6265 6c3e 2a7b 706f 7369  tip-label>*{posi
-00064ea0: 7469 6f6e 3a72 656c 6174 6976 6521 696d  tion:relative!im
-00064eb0: 706f 7274 616e 747d 2e72 696f 2d74 6f6f  portant}.rio-too
-00064ec0: 6c74 6970 2d6c 6162 656c 7b70 6f73 6974  ltip-label{posit
-00064ed0: 696f 6e3a 6162 736f 6c75 7465 3b77 6964  ion:absolute;wid
-00064ee0: 7468 3a6d 6178 2d63 6f6e 7465 6e74 3b70  th:max-content;p
-00064ef0: 6164 6469 6e67 3a2e 3572 656d 3b62 6f72  adding:.5rem;bor
-00064f00: 6465 722d 7261 6469 7573 3a76 6172 282d  der-radius:var(-
-00064f10: 2d72 696f 2d67 6c6f 6261 6c2d 636f 726e  -rio-global-corn
-00064f20: 6572 2d72 6164 6975 732d 736d 616c 6c29  er-radius-small)
-00064f30: 3b62 6163 6b67 726f 756e 643a 7661 7228  ;background:var(
-00064f40: 2d2d 7269 6f2d 676c 6f62 616c 2d68 7564  --rio-global-hud
-00064f50: 2d62 6729 3b62 6f78 2d73 6861 646f 773a  -bg);box-shadow:
-00064f60: 3020 2e31 7265 6d20 2e32 7265 6d20 7661  0 .1rem .2rem va
-00064f70: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d73  r(--rio-global-s
-00064f80: 6861 646f 772d 636f 6c6f 7229 3b6f 7061  hadow-color);opa
-00064f90: 6369 7479 3a30 3b74 7261 6e73 6974 696f  city:0;transitio
-00064fa0: 6e3a 6f70 6163 6974 7920 2e31 3573 2065  n:opacity .15s e
-00064fb0: 6173 652d 696e 2d6f 7574 7d2e 7269 6f2d  ase-in-out}.rio-
-00064fc0: 6275 696c 642d 6661 696c 6564 7b70 6f69  build-failed{poi
-00064fd0: 6e74 6572 2d65 7665 6e74 733a 6175 746f  nter-events:auto
-00064fe0: 3b63 6f6c 6f72 3a76 6172 282d 2d72 696f  ;color:var(--rio
-00064ff0: 2d67 6c6f 6261 6c2d 6461 6e67 6572 2d66  -global-danger-f
-00065000: 6729 3b64 6973 706c 6179 3a66 6c65 783b  g);display:flex;
-00065010: 666c 6578 2d64 6972 6563 7469 6f6e 3a63  flex-direction:c
-00065020: 6f6c 756d 6e3b 616c 6967 6e2d 6974 656d  olumn;align-item
-00065030: 733a 7374 7265 7463 683b 6261 636b 6772  s:stretch;backgr
-00065040: 6f75 6e64 3a76 6172 282d 2d72 696f 2d67  ound:var(--rio-g
-00065050: 6c6f 6261 6c2d 6461 6e67 6572 2d62 6729  lobal-danger-bg)
-00065060: 3b62 6f72 6465 722d 7261 6469 7573 3a76  ;border-radius:v
-00065070: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00065080: 636f 726e 6572 2d72 6164 6975 732d 736d  corner-radius-sm
-00065090: 616c 6c29 3b6f 7665 7266 6c6f 773a 6869  all);overflow:hi
-000650a0: 6464 656e 3b62 6163 6b67 726f 756e 642d  dden;background-
-000650b0: 696d 6167 653a 6c69 6e65 6172 2d67 7261  image:linear-gra
-000650c0: 6469 656e 7428 2d34 3564 6567 2c76 6172  dient(-45deg,var
-000650d0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6461  (--rio-global-da
-000650e0: 6e67 6572 2d62 672d 7661 7269 616e 7429  nger-bg-variant)
-000650f0: 2031 3525 2c74 7261 6e73 7061 7265 6e74   15%,transparent
-00065100: 2031 3525 2c74 7261 6e73 7061 7265 6e74   15%,transparent
-00065110: 2035 3025 2c76 6172 282d 2d72 696f 2d67   50%,var(--rio-g
-00065120: 6c6f 6261 6c2d 6461 6e67 6572 2d62 672d  lobal-danger-bg-
-00065130: 7661 7269 616e 7429 2035 3025 2c76 6172  variant) 50%,var
-00065140: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6461  (--rio-global-da
-00065150: 6e67 6572 2d62 672d 7661 7269 616e 7429  nger-bg-variant)
-00065160: 2036 3525 2c74 7261 6e73 7061 7265 6e74   65%,transparent
-00065170: 2036 3525 293b 6261 636b 6772 6f75 6e64   65%);background
-00065180: 2d73 697a 653a 3372 656d 2033 7265 6d3b  -size:3rem 3rem;
-00065190: 616e 696d 6174 696f 6e3a 6261 7262 6572  animation:barber
-000651a0: 2d70 6f6c 6520 3173 206c 696e 6561 7220  -pole 1s linear 
-000651b0: 696e 6669 6e69 7465 7d2e 7269 6f2d 6275  infinite}.rio-bu
-000651c0: 696c 642d 6661 696c 6564 2d74 6f70 2c2e  ild-failed-top,.
-000651d0: 7269 6f2d 6275 696c 642d 6661 696c 6564  rio-build-failed
-000651e0: 2d62 6f74 746f 6d7b 666c 6578 2d67 726f  -bottom{flex-gro
-000651f0: 773a 317d 2e72 696f 2d62 7569 6c64 2d66  w:1}.rio-build-f
-00065200: 6169 6c65 642d 746f 707b 6261 636b 6772  ailed-top{backgr
-00065210: 6f75 6e64 3a6c 696e 6561 722d 6772 6164  ound:linear-grad
-00065220: 6965 6e74 2874 6f20 746f 702c 7661 7228  ient(to top,var(
-00065230: 2d2d 7269 6f2d 676c 6f62 616c 2d64 616e  --rio-global-dan
-00065240: 6765 722d 6267 292c 7661 7228 2d2d 7269  ger-bg),var(--ri
-00065250: 6f2d 676c 6f62 616c 2d64 616e 6765 722d  o-global-danger-
-00065260: 6267 2920 3330 252c 7472 616e 7370 6172  bg) 30%,transpar
-00065270: 656e 7429 7d2e 7269 6f2d 6275 696c 642d  ent)}.rio-build-
-00065280: 6661 696c 6564 2d62 6f74 746f 6d7b 6261  failed-bottom{ba
-00065290: 636b 6772 6f75 6e64 3a6c 696e 6561 722d  ckground:linear-
-000652a0: 6772 6164 6965 6e74 2874 6f20 626f 7474  gradient(to bott
-000652b0: 6f6d 2c76 6172 282d 2d72 696f 2d67 6c6f  om,var(--rio-glo
-000652c0: 6261 6c2d 6461 6e67 6572 2d62 6729 2c76  bal-danger-bg),v
-000652d0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-000652e0: 6461 6e67 6572 2d62 6729 2033 3025 2c74  danger-bg) 30%,t
-000652f0: 7261 6e73 7061 7265 6e74 297d 2e72 696f  ransparent)}.rio
-00065300: 2d62 7569 6c64 2d66 6169 6c65 642d 636f  -build-failed-co
-00065310: 6e74 656e 747b 7061 6464 696e 673a 3172  ntent{padding:1r
-00065320: 656d 3b64 6973 706c 6179 3a66 6c65 783b  em;display:flex;
-00065330: 666c 6578 2d64 6972 6563 7469 6f6e 3a63  flex-direction:c
-00065340: 6f6c 756d 6e3b 616c 6967 6e2d 6974 656d  olumn;align-item
-00065350: 733a 7374 7265 7463 683b 6761 703a 3172  s:stretch;gap:1r
-00065360: 656d 3b62 6163 6b67 726f 756e 643a 7661  em;background:va
-00065370: 7228 2d2d 7269 6f2d 676c 6f62 616c 2d64  r(--rio-global-d
-00065380: 616e 6765 722d 6267 297d 2e72 696f 2d62  anger-bg)}.rio-b
-00065390: 7569 6c64 2d66 6169 6c65 642d 6865 6164  uild-failed-head
-000653a0: 6572 7b61 6c69 676e 2d73 656c 663a 6365  er{align-self:ce
-000653b0: 6e74 6572 3b64 6973 706c 6179 3a66 6c65  nter;display:fle
-000653c0: 783b 616c 6967 6e2d 6974 656d 733a 6365  x;align-items:ce
-000653d0: 6e74 6572 3b67 6170 3a2e 3572 656d 7d2e  nter;gap:.5rem}.
-000653e0: 7269 6f2d 6275 696c 642d 6661 696c 6564  rio-build-failed
-000653f0: 2d69 636f 6e7b 7769 6474 683a 3272 656d  -icon{width:2rem
-00065400: 3b68 6569 6768 743a 3272 656d 7d2e 7269  ;height:2rem}.ri
-00065410: 6f2d 6275 696c 642d 6661 696c 6564 2d73  o-build-failed-s
-00065420: 756d 6d61 7279 7b66 6f6e 742d 7765 6967  ummary{font-weig
-00065430: 6874 3a37 3030 7d2e 7269 6f2d 6275 696c  ht:700}.rio-buil
-00065440: 642d 6661 696c 6564 2d64 6574 6169 6c73  d-failed-details
-00065450: 7b61 6c69 676e 2d73 656c 663a 6365 6e74  {align-self:cent
-00065460: 6572 7d2e 7269 6f2d 636f 6465 2d65 7870  er}.rio-code-exp
-00065470: 6c6f 7265 727b 706f 696e 7465 722d 6576  lorer{pointer-ev
-00065480: 656e 7473 3a6e 6f6e 653b 6469 7370 6c61  ents:none;displa
-00065490: 793a 666c 6578 3b61 6c69 676e 2d69 7465  y:flex;align-ite
-000654a0: 6d73 3a63 656e 7465 723b 6a75 7374 6966  ms:center;justif
-000654b0: 792d 636f 6e74 656e 743a 7370 6163 652d  y-content:space-
-000654c0: 6265 7477 6565 6e7d 2e72 696f 2d63 6f64  between}.rio-cod
-000654d0: 652d 6578 706c 6f72 6572 2d73 6f75 7263  e-explorer-sourc
-000654e0: 652d 636f 6465 7b70 6f69 6e74 6572 2d65  e-code{pointer-e
-000654f0: 7665 6e74 733a 6175 746f 3b64 6973 706c  vents:auto;displ
-00065500: 6179 3a62 6c6f 636b 3b63 7572 736f 723a  ay:block;cursor:
-00065510: 7465 7874 3b77 6869 7465 2d73 7061 6365  text;white-space
-00065520: 3a70 7265 3b66 6f6e 742d 7369 7a65 3a31  :pre;font-size:1
-00065530: 7265 6d3b 666f 6e74 2d66 616d 696c 793a  rem;font-family:
-00065540: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
-00065550: 2d6d 6f6e 6f73 7061 6365 2d66 6f6e 7429  -monospace-font)
-00065560: 2c6d 6f6e 6f73 7061 6365 3b70 6f73 6974  ,monospace;posit
-00065570: 696f 6e3a 7265 6c61 7469 7665 3b6d 696e  ion:relative;min
-00065580: 2d77 6964 7468 3a32 3572 656d 3b77 6964  -width:25rem;wid
-00065590: 7468 3a6d 696e 2d63 6f6e 7465 6e74 3b62  th:min-content;b
-000655a0: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
-000655b0: 7269 6f2d 6c6f 6361 6c2d 6267 2d76 6172  rio-local-bg-var
-000655c0: 6961 6e74 293b 626f 7264 6572 2d72 6164  iant);border-rad
-000655d0: 6975 733a 7661 7228 2d2d 7269 6f2d 676c  ius:var(--rio-gl
-000655e0: 6f62 616c 2d63 6f72 6e65 722d 7261 6469  obal-corner-radi
-000655f0: 7573 2d6d 6564 6975 6d29 7d2e 7269 6f2d  us-medium)}.rio-
-00065600: 636f 6465 2d65 7870 6c6f 7265 722d 6275  code-explorer-bu
-00065610: 696c 642d 7265 7375 6c74 7b70 6f73 6974  ild-result{posit
-00065620: 696f 6e3a 7265 6c61 7469 7665 7d2e 7269  ion:relative}.ri
-00065630: 6f2d 636f 6465 2d65 7870 6c6f 7265 722d  o-code-explorer-
-00065640: 6275 696c 642d 7265 7375 6c74 3e2a 3a6e  build-result>*:n
-00065650: 6f74 282e 7269 6f2d 636f 6465 2d65 7870  ot(.rio-code-exp
-00065660: 6c6f 7265 722d 6869 6768 6c69 6768 7465  lorer-highlighte
-00065670: 7229 7b70 6f73 6974 696f 6e3a 7265 6c61  r){position:rela
-00065680: 7469 7665 2169 6d70 6f72 7461 6e74 7d2e  tive!important}.
-00065690: 7269 6f2d 636f 6465 2d65 7870 6c6f 7265  rio-code-explore
-000656a0: 722d 6869 6768 6c69 6768 7465 727b 706f  r-highlighter{po
-000656b0: 696e 7465 722d 6576 656e 7473 3a6e 6f6e  inter-events:non
-000656c0: 653b 706f 7369 7469 6f6e 3a61 6273 6f6c  e;position:absol
-000656d0: 7574 653b 6f70 6163 6974 793a 303b 7472  ute;opacity:0;tr
-000656e0: 616e 7369 7469 6f6e 3a6f 7061 6369 7479  ansition:opacity
-000656f0: 202e 3373 2065 6173 652d 696e 2d6f 7574   .3s ease-in-out
-00065700: 2c6c 6566 7420 2e33 7320 6561 7365 2d69  ,left .3s ease-i
-00065710: 6e2d 6f75 742c 746f 7020 2e33 7320 6561  n-out,top .3s ea
-00065720: 7365 2d69 6e2d 6f75 742c 7769 6474 6820  se-in-out,width 
-00065730: 2e33 7320 6561 7365 2d69 6e2d 6f75 742c  .3s ease-in-out,
-00065740: 6865 6967 6874 202e 3373 2065 6173 652d  height .3s ease-
-00065750: 696e 2d6f 7574 7d2e 7269 6f2d 636f 6465  in-out}.rio-code
-00065760: 2d65 7870 6c6f 7265 722d 6869 6768 6c69  -explorer-highli
-00065770: 6768 7465 723a 6166 7465 727b 636f 6e74  ghter:after{cont
-00065780: 656e 743a 2222 3b7a 2d69 6e64 6578 3a31  ent:"";z-index:1
-00065790: 3030 3031 3b70 6f73 6974 696f 6e3a 6162  0001;position:ab
-000657a0: 736f 6c75 7465 3b62 6f72 6465 722d 7261  solute;border-ra
-000657b0: 6469 7573 3a31 7265 6d3b 626f 7264 6572  dius:1rem;border
-000657c0: 2d73 7479 6c65 3a73 6f6c 6964 3b62 6f72  -style:solid;bor
-000657d0: 6465 722d 7769 6474 683a 2e32 7265 6d21  der-width:.2rem!
-000657e0: 696d 706f 7274 616e 743b 626f 7264 6572  important;border
-000657f0: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
-00065800: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
-00065810: 792d 6267 293b 626f 782d 7368 6164 6f77  y-bg);box-shadow
-00065820: 3a30 2030 2034 7265 6d20 3172 656d 2076  :0 0 4rem 1rem v
-00065830: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
-00065840: 7365 636f 6e64 6172 792d 6267 293b 6f70  secondary-bg);op
-00065850: 6163 6974 793a 2e34 3b61 6e69 6d61 7469  acity:.4;animati
-00065860: 6f6e 3a70 756c 7365 2031 2e34 7320 696e  on:pulse 1.4s in
-00065870: 6669 6e69 7465 7d2e 7269 6f2d 7365 7061  finite}.rio-sepa
-00065880: 7261 746f 727b 706f 7369 7469 6f6e 3a72  rator{position:r
-00065890: 656c 6174 6976 653b 6261 636b 6772 6f75  elative;backgrou
-000658a0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
-000658b0: 696f 2d6c 6f63 616c 2d62 6729 7d2e 7269  io-local-bg)}.ri
-000658c0: 6f2d 7365 7061 7261 746f 723a 6166 7465  o-separator:afte
-000658d0: 727b 636f 6e74 656e 743a 2222 3b70 6f73  r{content:"";pos
-000658e0: 6974 696f 6e3a 6162 736f 6c75 7465 3b6c  ition:absolute;l
-000658f0: 6566 743a 303b 746f 703a 303b 7269 6768  eft:0;top:0;righ
-00065900: 743a 303b 626f 7474 6f6d 3a30 3b62 6163  t:0;bottom:0;bac
+000644f0: 652d 6974 656d 2d68 6561 6465 723e 6469  e-item-header>di
+00064500: 763a 6669 7273 742d 6368 696c 647b 7769  v:first-child{wi
+00064510: 6474 683a 3172 656d 3b68 6569 6768 743a  dth:1rem;height:
+00064520: 3172 656d 3b74 7261 6e73 6974 696f 6e3a  1rem;transition:
+00064530: 7472 616e 7366 6f72 6d20 2e31 7320 6561  transform .1s ea
+00064540: 7365 2d69 6e2d 6f75 747d 2e72 696f 2d64  se-in-out}.rio-d
+00064550: 6562 7567 6765 722d 636f 6d70 6f6e 656e  ebugger-componen
+00064560: 742d 7472 6565 2d69 7465 6d5b 6461 7461  t-tree-item[data
+00064570: 2d65 7870 616e 6465 643d 7472 7565 5d3e  -expanded=true]>
+00064580: 2e72 696f 2d64 6562 7567 6765 722d 636f  .rio-debugger-co
+00064590: 6d70 6f6e 656e 742d 7472 6565 2d69 7465  mponent-tree-ite
+000645a0: 6d2d 6865 6164 6572 3e64 6976 3a66 6972  m-header>div:fir
+000645b0: 7374 2d63 6869 6c64 7b74 7261 6e73 666f  st-child{transfo
+000645c0: 726d 3a72 6f74 6174 6528 3930 6465 6729  rm:rotate(90deg)
+000645d0: 7d2e 7269 6f2d 6465 6275 6767 6572 2d63  }.rio-debugger-c
+000645e0: 6f6d 706f 6e65 6e74 2d74 7265 652d 6974  omponent-tree-it
+000645f0: 656d 2d68 6561 6465 723a 6166 7465 727b  em-header:after{
+00064600: 706f 696e 7465 722d 6576 656e 7473 3a6e  pointer-events:n
+00064610: 6f6e 653b 636f 6e74 656e 743a 2222 3b64  one;content:"";d
+00064620: 6973 706c 6179 3a62 6c6f 636b 3b7a 2d69  isplay:block;z-i
+00064630: 6e64 6578 3a2d 313b 706f 7369 7469 6f6e  ndex:-1;position
+00064640: 3a61 6273 6f6c 7574 653b 6c65 6674 3a30  :absolute;left:0
+00064650: 3b74 6f70 3a30 3b72 6967 6874 3a30 3b62  ;top:0;right:0;b
+00064660: 6f74 746f 6d3a 303b 6261 636b 6772 6f75  ottom:0;backgrou
+00064670: 6e64 3a76 6172 282d 2d72 696f 2d67 6c6f  nd:var(--rio-glo
+00064680: 6261 6c2d 7365 636f 6e64 6172 792d 6267  bal-secondary-bg
+00064690: 293b 626f 7264 6572 2d72 6164 6975 733a  );border-radius:
+000646a0: 3939 3939 3970 783b 6f70 6163 6974 793a  99999px;opacity:
+000646b0: 303b 7472 616e 7369 7469 6f6e 3a6f 7061  0;transition:opa
+000646c0: 6369 7479 202e 3173 2065 6173 652d 696e  city .1s ease-in
+000646d0: 2d6f 7574 7d2e 7269 6f2d 6465 6275 6767  -out}.rio-debugg
+000646e0: 6572 2d63 6f6d 706f 6e65 6e74 2d74 7265  er-component-tre
+000646f0: 652d 6974 656d 2d68 6561 6465 723e 6469  e-item-header>di
+00064700: 763e 7376 677b 7769 6474 683a 3172 656d  v>svg{width:1rem
+00064710: 3b68 6569 6768 743a 3172 656d 7d2e 7269  ;height:1rem}.ri
+00064720: 6f2d 6465 6275 6767 6572 2d63 6f6d 706f  o-debugger-compo
+00064730: 6e65 6e74 2d74 7265 652d 6974 656d 2d68  nent-tree-item-h
+00064740: 6561 6465 722d 7765 616b 6c79 2d73 656c  eader-weakly-sel
+00064750: 6563 7465 647b 666f 6e74 2d77 6569 6768  ected{font-weigh
+00064760: 743a 3730 307d 2e72 696f 2d64 6562 7567  t:700}.rio-debug
+00064770: 6765 722d 636f 6d70 6f6e 656e 742d 7472  ger-component-tr
+00064780: 6565 2d69 7465 6d2d 6865 6164 6572 2d73  ee-item-header-s
+00064790: 7472 6f6e 676c 792d 7365 6c65 6374 6564  trongly-selected
+000647a0: 7b66 6f6e 742d 7765 6967 6874 3a37 3030  {font-weight:700
+000647b0: 3b63 6f6c 6f72 3a76 6172 282d 2d72 696f  ;color:var(--rio
+000647c0: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
+000647d0: 792d 6667 297d 2e72 696f 2d64 6562 7567  y-fg)}.rio-debug
+000647e0: 6765 722d 636f 6d70 6f6e 656e 742d 7472  ger-component-tr
+000647f0: 6565 2d69 7465 6d2d 6865 6164 6572 3a68  ee-item-header:h
+00064800: 6f76 6572 3a61 6674 6572 7b6f 7061 6369  over:after{opaci
+00064810: 7479 3a2e 347d 2e72 696f 2d64 6562 7567  ty:.4}.rio-debug
+00064820: 6765 722d 636f 6d70 6f6e 656e 742d 7472  ger-component-tr
+00064830: 6565 2d69 7465 6d2d 6865 6164 6572 2d77  ee-item-header-w
+00064840: 6561 6b6c 792d 7365 6c65 6374 6564 3a61  eakly-selected:a
+00064850: 6674 6572 7b6f 7061 6369 7479 3a2e 3135  fter{opacity:.15
+00064860: 7d2e 7269 6f2d 6465 6275 6767 6572 2d63  }.rio-debugger-c
+00064870: 6f6d 706f 6e65 6e74 2d74 7265 652d 6974  omponent-tree-it
+00064880: 656d 2d68 6561 6465 722d 7374 726f 6e67  em-header-strong
+00064890: 6c79 2d73 656c 6563 7465 643a 6166 7465  ly-selected:afte
+000648a0: 727b 6f70 6163 6974 793a 2e36 7d2e 7269  r{opacity:.6}.ri
+000648b0: 6f2d 6465 6275 6767 6572 2d63 6f6d 706f  o-debugger-compo
+000648c0: 6e65 6e74 2d74 7265 652d 6974 656d 2d68  nent-tree-item-h
+000648d0: 6561 6465 722d 7374 726f 6e67 6c79 2d73  eader-strongly-s
+000648e0: 656c 6563 7465 643a 686f 7665 723a 6166  elected:hover:af
+000648f0: 7465 727b 6f70 6163 6974 793a 2e38 7d2e  ter{opacity:.8}.
+00064900: 7269 6f2d 6465 6275 6767 6572 2d63 6f6d  rio-debugger-com
+00064910: 706f 6e65 6e74 2d74 7265 652d 6974 656d  ponent-tree-item
+00064920: 2d63 6869 6c64 7265 6e7b 6d61 7267 696e  -children{margin
+00064930: 2d6c 6566 743a 2e37 7265 6d3b 6469 7370  -left:.7rem;disp
+00064940: 6c61 793a 6e6f 6e65 3b66 6c65 782d 6469  lay:none;flex-di
+00064950: 7265 6374 696f 6e3a 636f 6c75 6d6e 3b67  rection:column;g
+00064960: 6170 3a2e 3272 656d 7d2e 7269 6f2d 6465  ap:.2rem}.rio-de
+00064970: 6275 6767 6572 2d63 6f6d 706f 6e65 6e74  bugger-component
+00064980: 2d74 7265 652d 6974 656d 5b64 6174 612d  -tree-item[data-
+00064990: 6861 732d 6368 696c 6472 656e 3d74 7275  has-children=tru
+000649a0: 655d 5b64 6174 612d 6578 7061 6e64 6564  e][data-expanded
+000649b0: 3d74 7275 655d 3e2e 7269 6f2d 6465 6275  =true]>.rio-debu
+000649c0: 6767 6572 2d63 6f6d 706f 6e65 6e74 2d74  gger-component-t
+000649d0: 7265 652d 6974 656d 2d63 6869 6c64 7265  ree-item-childre
+000649e0: 6e7b 6469 7370 6c61 793a 666c 6578 7d2e  n{display:flex}.
+000649f0: 7269 6f2d 6465 6275 6767 6572 2d63 6f6d  rio-debugger-com
+00064a00: 706f 6e65 6e74 2d68 6967 686c 6967 6874  ponent-highlight
+00064a10: 6572 7b70 6f69 6e74 6572 2d65 7665 6e74  er{pointer-event
+00064a20: 733a 6e6f 6e65 3b70 6f73 6974 696f 6e3a  s:none;position:
+00064a30: 6669 7865 643b 7a2d 696e 6465 783a 3130  fixed;z-index:10
+00064a40: 3030 313b 7472 616e 7369 7469 6f6e 3a6c  001;transition:l
+00064a50: 6566 7420 2e33 7320 6561 7365 2d69 6e2d  eft .3s ease-in-
+00064a60: 6f75 742c 746f 7020 2e33 7320 6561 7365  out,top .3s ease
+00064a70: 2d69 6e2d 6f75 742c 7769 6474 6820 2e33  -in-out,width .3
+00064a80: 7320 6561 7365 2d69 6e2d 6f75 742c 6865  s ease-in-out,he
+00064a90: 6967 6874 202e 3373 2065 6173 652d 696e  ight .3s ease-in
+00064aa0: 2d6f 7574 7d40 6b65 7966 7261 6d65 7320  -out}@keyframes 
+00064ab0: 7075 6c73 657b 3025 7b6c 6566 743a 2d2e  pulse{0%{left:-.
+00064ac0: 3372 656d 3b74 6f70 3a2d 2e33 7265 6d3b  3rem;top:-.3rem;
+00064ad0: 7269 6768 743a 2d2e 3372 656d 3b62 6f74  right:-.3rem;bot
+00064ae0: 746f 6d3a 2d2e 3372 656d 3b62 6f72 6465  tom:-.3rem;borde
+00064af0: 722d 7769 6474 683a 2e34 7265 6d7d 3530  r-width:.4rem}50
+00064b00: 257b 6c65 6674 3a2d 2e37 7265 6d3b 746f  %{left:-.7rem;to
+00064b10: 703a 2d2e 3772 656d 3b72 6967 6874 3a2d  p:-.7rem;right:-
+00064b20: 2e37 7265 6d3b 626f 7474 6f6d 3a2d 2e37  .7rem;bottom:-.7
+00064b30: 7265 6d3b 626f 7264 6572 2d77 6964 7468  rem;border-width
+00064b40: 3a2e 3372 656d 7d74 6f7b 6c65 6674 3a2d  :.3rem}to{left:-
+00064b50: 2e33 7265 6d3b 746f 703a 2d2e 3372 656d  .3rem;top:-.3rem
+00064b60: 3b72 6967 6874 3a2d 2e33 7265 6d3b 626f  ;right:-.3rem;bo
+00064b70: 7474 6f6d 3a2d 2e33 7265 6d3b 626f 7264  ttom:-.3rem;bord
+00064b80: 6572 2d77 6964 7468 3a2e 3472 656d 7d7d  er-width:.4rem}}
+00064b90: 2e72 696f 2d64 6562 7567 6765 722d 636f  .rio-debugger-co
+00064ba0: 6d70 6f6e 656e 742d 6869 6768 6c69 6768  mponent-highligh
+00064bb0: 7465 723a 6166 7465 727b 636f 6e74 656e  ter:after{conten
+00064bc0: 743a 2222 3b70 6f73 6974 696f 6e3a 6162  t:"";position:ab
+00064bd0: 736f 6c75 7465 3b64 6973 706c 6179 3a62  solute;display:b
+00064be0: 6c6f 636b 3b62 6f72 6465 722d 7261 6469  lock;border-radi
+00064bf0: 7573 3a31 7265 6d3b 626f 782d 7368 6164  us:1rem;box-shad
+00064c00: 6f77 3a30 2030 2030 2039 3939 3972 656d  ow:0 0 0 9999rem
+00064c10: 2023 3030 3039 3b62 6f72 6465 722d 7374   #0009;border-st
+00064c20: 796c 653a 736f 6c69 643b 626f 7264 6572  yle:solid;border
+00064c30: 2d63 6f6c 6f72 3a76 6172 282d 2d72 696f  -color:var(--rio
+00064c40: 2d67 6c6f 6261 6c2d 7365 636f 6e64 6172  -global-secondar
+00064c50: 792d 6267 293b 616e 696d 6174 696f 6e3a  y-bg);animation:
+00064c60: 7075 6c73 6520 312e 3473 2069 6e66 696e  pulse 1.4s infin
+00064c70: 6974 657d 2e72 696f 2d64 6562 7567 6765  ite}.rio-debugge
+00064c80: 722d 6261 636b 6772 6f75 6e64 7b7a 2d69  r-background{z-i
+00064c90: 6e64 6578 3a2d 313b 706f 7369 7469 6f6e  ndex:-1;position
+00064ca0: 3a72 656c 6174 6976 653b 6261 636b 6772  :relative;backgr
+00064cb0: 6f75 6e64 3a76 6172 282d 2d72 696f 2d6c  ound:var(--rio-l
+00064cc0: 6f63 616c 2d62 6729 7d2e 7269 6f2d 6465  ocal-bg)}.rio-de
+00064cd0: 6275 6767 6572 2d62 6163 6b67 726f 756e  bugger-backgroun
+00064ce0: 643a 6166 7465 727b 636f 6e74 656e 743a  d:after{content:
+00064cf0: 2222 3b70 6f73 6974 696f 6e3a 6162 736f  "";position:abso
+00064d00: 6c75 7465 3b64 6973 706c 6179 3a62 6c6f  lute;display:blo
+00064d10: 636b 3b7a 2d69 6e64 6578 3a2d 313b 6c65  ck;z-index:-1;le
+00064d20: 6674 3a30 3b74 6f70 3a30 3b62 6f74 746f  ft:0;top:0;botto
+00064d30: 6d3a 303b 7269 6768 743a 303b 6261 636b  m:0;right:0;back
+00064d40: 6772 6f75 6e64 2d69 6d61 6765 3a6c 696e  ground-image:lin
+00064d50: 6561 722d 6772 6164 6965 6e74 282d 3435  ear-gradient(-45
+00064d60: 6465 672c 7661 7228 2d2d 7269 6f2d 6c6f  deg,var(--rio-lo
+00064d70: 6361 6c2d 6267 2920 3235 252c 7661 7228  cal-bg) 25%,var(
+00064d80: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
+00064d90: 6f6e 6461 7279 2d62 6729 2032 3525 2c76  ondary-bg) 25%,v
+00064da0: 6172 282d 2d72 696f 2d67 6c6f 6261 6c2d  ar(--rio-global-
+00064db0: 7365 636f 6e64 6172 792d 6267 2920 3530  secondary-bg) 50
+00064dc0: 252c 7661 7228 2d2d 7269 6f2d 6c6f 6361  %,var(--rio-loca
+00064dd0: 6c2d 6267 2920 3530 252c 7661 7228 2d2d  l-bg) 50%,var(--
+00064de0: 7269 6f2d 6c6f 6361 6c2d 6267 2920 3735  rio-local-bg) 75
+00064df0: 252c 7661 7228 2d2d 7269 6f2d 676c 6f62  %,var(--rio-glob
+00064e00: 616c 2d73 6563 6f6e 6461 7279 2d62 6729  al-secondary-bg)
+00064e10: 2037 3525 2c76 6172 282d 2d72 696f 2d67   75%,var(--rio-g
+00064e20: 6c6f 6261 6c2d 7365 636f 6e64 6172 792d  lobal-secondary-
+00064e30: 6267 2929 3b62 6163 6b67 726f 756e 642d  bg));background-
+00064e40: 7369 7a65 3a33 7265 6d20 3372 656d 3b6f  size:3rem 3rem;o
+00064e50: 7061 6369 7479 3a2e 3033 7d2e 7269 6f2d  pacity:.03}.rio-
+00064e60: 7377 6974 6368 6572 7b6f 7665 7266 6c6f  switcher{overflo
+00064e70: 773a 6869 6464 656e 7d2e 7269 6f2d 746f  w:hidden}.rio-to
+00064e80: 6f6c 7469 707b 706f 696e 7465 722d 6576  oltip{pointer-ev
+00064e90: 656e 7473 3a6e 6f6e 653b 706f 7369 7469  ents:none;positi
+00064ea0: 6f6e 3a72 656c 6174 6976 657d 2e72 696f  on:relative}.rio
+00064eb0: 2d74 6f6f 6c74 6970 2d61 6e63 686f 727b  -tooltip-anchor{
+00064ec0: 706f 696e 7465 722d 6576 656e 7473 3a61  pointer-events:a
+00064ed0: 7574 6f3b 706f 7369 7469 6f6e 3a72 656c  uto;position:rel
+00064ee0: 6174 6976 657d 2e72 696f 2d74 6f6f 6c74  ative}.rio-toolt
+00064ef0: 6970 2d61 6e63 686f 723e 2a2c 2e72 696f  ip-anchor>*,.rio
+00064f00: 2d74 6f6f 6c74 6970 2d6c 6162 656c 3e2a  -tooltip-label>*
+00064f10: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
+00064f20: 7665 2169 6d70 6f72 7461 6e74 7d2e 7269  ve!important}.ri
+00064f30: 6f2d 746f 6f6c 7469 702d 6c61 6265 6c7b  o-tooltip-label{
+00064f40: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
+00064f50: 653b 7769 6474 683a 6d61 782d 636f 6e74  e;width:max-cont
+00064f60: 656e 743b 7061 6464 696e 673a 2e35 7265  ent;padding:.5re
+00064f70: 6d3b 626f 7264 6572 2d72 6164 6975 733a  m;border-radius:
+00064f80: 7661 7228 2d2d 7269 6f2d 676c 6f62 616c  var(--rio-global
+00064f90: 2d63 6f72 6e65 722d 7261 6469 7573 2d73  -corner-radius-s
+00064fa0: 6d61 6c6c 293b 6261 636b 6772 6f75 6e64  mall);background
+00064fb0: 3a76 6172 282d 2d72 696f 2d67 6c6f 6261  :var(--rio-globa
+00064fc0: 6c2d 6875 642d 6267 293b 626f 782d 7368  l-hud-bg);box-sh
+00064fd0: 6164 6f77 3a30 202e 3172 656d 202e 3272  adow:0 .1rem .2r
+00064fe0: 656d 2076 6172 282d 2d72 696f 2d67 6c6f  em var(--rio-glo
+00064ff0: 6261 6c2d 7368 6164 6f77 2d63 6f6c 6f72  bal-shadow-color
+00065000: 293b 6f70 6163 6974 793a 303b 7472 616e  );opacity:0;tran
+00065010: 7369 7469 6f6e 3a6f 7061 6369 7479 202e  sition:opacity .
+00065020: 3135 7320 6561 7365 2d69 6e2d 6f75 747d  15s ease-in-out}
+00065030: 2e72 696f 2d62 7569 6c64 2d66 6169 6c65  .rio-build-faile
+00065040: 647b 706f 696e 7465 722d 6576 656e 7473  d{pointer-events
+00065050: 3a61 7574 6f3b 636f 6c6f 723a 7661 7228  :auto;color:var(
+00065060: 2d2d 7269 6f2d 676c 6f62 616c 2d64 616e  --rio-global-dan
+00065070: 6765 722d 6667 293b 6469 7370 6c61 793a  ger-fg);display:
+00065080: 666c 6578 3b66 6c65 782d 6469 7265 6374  flex;flex-direct
+00065090: 696f 6e3a 636f 6c75 6d6e 3b61 6c69 676e  ion:column;align
+000650a0: 2d69 7465 6d73 3a73 7472 6574 6368 3b62  -items:stretch;b
+000650b0: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
+000650c0: 7269 6f2d 676c 6f62 616c 2d64 616e 6765  rio-global-dange
+000650d0: 722d 6267 293b 626f 7264 6572 2d72 6164  r-bg);border-rad
+000650e0: 6975 733a 7661 7228 2d2d 7269 6f2d 676c  ius:var(--rio-gl
+000650f0: 6f62 616c 2d63 6f72 6e65 722d 7261 6469  obal-corner-radi
+00065100: 7573 2d73 6d61 6c6c 293b 6f76 6572 666c  us-small);overfl
+00065110: 6f77 3a68 6964 6465 6e3b 6261 636b 6772  ow:hidden;backgr
+00065120: 6f75 6e64 2d69 6d61 6765 3a6c 696e 6561  ound-image:linea
+00065130: 722d 6772 6164 6965 6e74 282d 3435 6465  r-gradient(-45de
+00065140: 672c 7661 7228 2d2d 7269 6f2d 676c 6f62  g,var(--rio-glob
+00065150: 616c 2d64 616e 6765 722d 6267 2d76 6172  al-danger-bg-var
+00065160: 6961 6e74 2920 3135 252c 7472 616e 7370  iant) 15%,transp
+00065170: 6172 656e 7420 3135 252c 7472 616e 7370  arent 15%,transp
+00065180: 6172 656e 7420 3530 252c 7661 7228 2d2d  arent 50%,var(--
+00065190: 7269 6f2d 676c 6f62 616c 2d64 616e 6765  rio-global-dange
+000651a0: 722d 6267 2d76 6172 6961 6e74 2920 3530  r-bg-variant) 50
+000651b0: 252c 7661 7228 2d2d 7269 6f2d 676c 6f62  %,var(--rio-glob
+000651c0: 616c 2d64 616e 6765 722d 6267 2d76 6172  al-danger-bg-var
+000651d0: 6961 6e74 2920 3635 252c 7472 616e 7370  iant) 65%,transp
+000651e0: 6172 656e 7420 3635 2529 3b62 6163 6b67  arent 65%);backg
+000651f0: 726f 756e 642d 7369 7a65 3a33 7265 6d20  round-size:3rem 
+00065200: 3372 656d 3b61 6e69 6d61 7469 6f6e 3a62  3rem;animation:b
+00065210: 6172 6265 722d 706f 6c65 2031 7320 6c69  arber-pole 1s li
+00065220: 6e65 6172 2069 6e66 696e 6974 657d 2e72  near infinite}.r
+00065230: 696f 2d62 7569 6c64 2d66 6169 6c65 642d  io-build-failed-
+00065240: 746f 702c 2e72 696f 2d62 7569 6c64 2d66  top,.rio-build-f
+00065250: 6169 6c65 642d 626f 7474 6f6d 7b66 6c65  ailed-bottom{fle
+00065260: 782d 6772 6f77 3a31 7d2e 7269 6f2d 6275  x-grow:1}.rio-bu
+00065270: 696c 642d 6661 696c 6564 2d74 6f70 7b62  ild-failed-top{b
+00065280: 6163 6b67 726f 756e 643a 6c69 6e65 6172  ackground:linear
+00065290: 2d67 7261 6469 656e 7428 746f 2074 6f70  -gradient(to top
+000652a0: 2c76 6172 282d 2d72 696f 2d67 6c6f 6261  ,var(--rio-globa
+000652b0: 6c2d 6461 6e67 6572 2d62 6729 2c76 6172  l-danger-bg),var
+000652c0: 282d 2d72 696f 2d67 6c6f 6261 6c2d 6461  (--rio-global-da
+000652d0: 6e67 6572 2d62 6729 2033 3025 2c74 7261  nger-bg) 30%,tra
+000652e0: 6e73 7061 7265 6e74 297d 2e72 696f 2d62  nsparent)}.rio-b
+000652f0: 7569 6c64 2d66 6169 6c65 642d 626f 7474  uild-failed-bott
+00065300: 6f6d 7b62 6163 6b67 726f 756e 643a 6c69  om{background:li
+00065310: 6e65 6172 2d67 7261 6469 656e 7428 746f  near-gradient(to
+00065320: 2062 6f74 746f 6d2c 7661 7228 2d2d 7269   bottom,var(--ri
+00065330: 6f2d 676c 6f62 616c 2d64 616e 6765 722d  o-global-danger-
+00065340: 6267 292c 7661 7228 2d2d 7269 6f2d 676c  bg),var(--rio-gl
+00065350: 6f62 616c 2d64 616e 6765 722d 6267 2920  obal-danger-bg) 
+00065360: 3330 252c 7472 616e 7370 6172 656e 7429  30%,transparent)
+00065370: 7d2e 7269 6f2d 6275 696c 642d 6661 696c  }.rio-build-fail
+00065380: 6564 2d63 6f6e 7465 6e74 7b70 6164 6469  ed-content{paddi
+00065390: 6e67 3a31 7265 6d3b 6469 7370 6c61 793a  ng:1rem;display:
+000653a0: 666c 6578 3b66 6c65 782d 6469 7265 6374  flex;flex-direct
+000653b0: 696f 6e3a 636f 6c75 6d6e 3b61 6c69 676e  ion:column;align
+000653c0: 2d69 7465 6d73 3a73 7472 6574 6368 3b67  -items:stretch;g
+000653d0: 6170 3a31 7265 6d3b 6261 636b 6772 6f75  ap:1rem;backgrou
+000653e0: 6e64 3a76 6172 282d 2d72 696f 2d67 6c6f  nd:var(--rio-glo
+000653f0: 6261 6c2d 6461 6e67 6572 2d62 6729 7d2e  bal-danger-bg)}.
+00065400: 7269 6f2d 6275 696c 642d 6661 696c 6564  rio-build-failed
+00065410: 2d68 6561 6465 727b 616c 6967 6e2d 7365  -header{align-se
+00065420: 6c66 3a63 656e 7465 723b 6469 7370 6c61  lf:center;displa
+00065430: 793a 666c 6578 3b61 6c69 676e 2d69 7465  y:flex;align-ite
+00065440: 6d73 3a63 656e 7465 723b 6761 703a 2e35  ms:center;gap:.5
+00065450: 7265 6d7d 2e72 696f 2d62 7569 6c64 2d66  rem}.rio-build-f
+00065460: 6169 6c65 642d 6963 6f6e 7b77 6964 7468  ailed-icon{width
+00065470: 3a32 7265 6d3b 6865 6967 6874 3a32 7265  :2rem;height:2re
+00065480: 6d7d 2e72 696f 2d62 7569 6c64 2d66 6169  m}.rio-build-fai
+00065490: 6c65 642d 7375 6d6d 6172 797b 666f 6e74  led-summary{font
+000654a0: 2d77 6569 6768 743a 3730 307d 2e72 696f  -weight:700}.rio
+000654b0: 2d62 7569 6c64 2d66 6169 6c65 642d 6465  -build-failed-de
+000654c0: 7461 696c 737b 616c 6967 6e2d 7365 6c66  tails{align-self
+000654d0: 3a63 656e 7465 727d 2e72 696f 2d63 6f64  :center}.rio-cod
+000654e0: 652d 6578 706c 6f72 6572 7b70 6f69 6e74  e-explorer{point
+000654f0: 6572 2d65 7665 6e74 733a 6e6f 6e65 3b64  er-events:none;d
+00065500: 6973 706c 6179 3a66 6c65 783b 616c 6967  isplay:flex;alig
+00065510: 6e2d 6974 656d 733a 6365 6e74 6572 3b6a  n-items:center;j
+00065520: 7573 7469 6679 2d63 6f6e 7465 6e74 3a73  ustify-content:s
+00065530: 7061 6365 2d62 6574 7765 656e 7d2e 7269  pace-between}.ri
+00065540: 6f2d 636f 6465 2d65 7870 6c6f 7265 722d  o-code-explorer-
+00065550: 736f 7572 6365 2d63 6f64 657b 706f 696e  source-code{poin
+00065560: 7465 722d 6576 656e 7473 3a61 7574 6f3b  ter-events:auto;
+00065570: 6469 7370 6c61 793a 626c 6f63 6b3b 6375  display:block;cu
+00065580: 7273 6f72 3a74 6578 743b 7768 6974 652d  rsor:text;white-
+00065590: 7370 6163 653a 7072 653b 666f 6e74 2d73  space:pre;font-s
+000655a0: 697a 653a 3172 656d 3b66 6f6e 742d 6661  ize:1rem;font-fa
+000655b0: 6d69 6c79 3a76 6172 282d 2d72 696f 2d67  mily:var(--rio-g
+000655c0: 6c6f 6261 6c2d 6d6f 6e6f 7370 6163 652d  lobal-monospace-
+000655d0: 666f 6e74 292c 6d6f 6e6f 7370 6163 653b  font),monospace;
+000655e0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+000655f0: 653b 6d69 6e2d 7769 6474 683a 3235 7265  e;min-width:25re
+00065600: 6d3b 7769 6474 683a 6d69 6e2d 636f 6e74  m;width:min-cont
+00065610: 656e 743b 6261 636b 6772 6f75 6e64 3a76  ent;background:v
+00065620: 6172 282d 2d72 696f 2d6c 6f63 616c 2d62  ar(--rio-local-b
+00065630: 672d 7661 7269 616e 7429 3b62 6f72 6465  g-variant);borde
+00065640: 722d 7261 6469 7573 3a76 6172 282d 2d72  r-radius:var(--r
+00065650: 696f 2d67 6c6f 6261 6c2d 636f 726e 6572  io-global-corner
+00065660: 2d72 6164 6975 732d 6d65 6469 756d 297d  -radius-medium)}
+00065670: 2e72 696f 2d63 6f64 652d 6578 706c 6f72  .rio-code-explor
+00065680: 6572 2d62 7569 6c64 2d72 6573 756c 747b  er-build-result{
+00065690: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+000656a0: 657d 2e72 696f 2d63 6f64 652d 6578 706c  e}.rio-code-expl
+000656b0: 6f72 6572 2d62 7569 6c64 2d72 6573 756c  orer-build-resul
+000656c0: 743e 2a3a 6e6f 7428 2e72 696f 2d63 6f64  t>*:not(.rio-cod
+000656d0: 652d 6578 706c 6f72 6572 2d68 6967 686c  e-explorer-highl
+000656e0: 6967 6874 6572 297b 706f 7369 7469 6f6e  ighter){position
+000656f0: 3a72 656c 6174 6976 6521 696d 706f 7274  :relative!import
+00065700: 616e 747d 2e72 696f 2d63 6f64 652d 6578  ant}.rio-code-ex
+00065710: 706c 6f72 6572 2d68 6967 686c 6967 6874  plorer-highlight
+00065720: 6572 7b70 6f69 6e74 6572 2d65 7665 6e74  er{pointer-event
+00065730: 733a 6e6f 6e65 3b70 6f73 6974 696f 6e3a  s:none;position:
+00065740: 6162 736f 6c75 7465 3b6f 7061 6369 7479  absolute;opacity
+00065750: 3a30 3b74 7261 6e73 6974 696f 6e3a 6f70  :0;transition:op
+00065760: 6163 6974 7920 2e33 7320 6561 7365 2d69  acity .3s ease-i
+00065770: 6e2d 6f75 742c 6c65 6674 202e 3373 2065  n-out,left .3s e
+00065780: 6173 652d 696e 2d6f 7574 2c74 6f70 202e  ase-in-out,top .
+00065790: 3373 2065 6173 652d 696e 2d6f 7574 2c77  3s ease-in-out,w
+000657a0: 6964 7468 202e 3373 2065 6173 652d 696e  idth .3s ease-in
+000657b0: 2d6f 7574 2c68 6569 6768 7420 2e33 7320  -out,height .3s 
+000657c0: 6561 7365 2d69 6e2d 6f75 747d 2e72 696f  ease-in-out}.rio
+000657d0: 2d63 6f64 652d 6578 706c 6f72 6572 2d68  -code-explorer-h
+000657e0: 6967 686c 6967 6874 6572 3a61 6674 6572  ighlighter:after
+000657f0: 7b63 6f6e 7465 6e74 3a22 223b 7a2d 696e  {content:"";z-in
+00065800: 6465 783a 3130 3030 313b 706f 7369 7469  dex:10001;positi
+00065810: 6f6e 3a61 6273 6f6c 7574 653b 626f 7264  on:absolute;bord
+00065820: 6572 2d72 6164 6975 733a 3172 656d 3b62  er-radius:1rem;b
+00065830: 6f72 6465 722d 7374 796c 653a 736f 6c69  order-style:soli
+00065840: 643b 626f 7264 6572 2d77 6964 7468 3a2e  d;border-width:.
+00065850: 3272 656d 2169 6d70 6f72 7461 6e74 3b62  2rem!important;b
+00065860: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+00065870: 2d2d 7269 6f2d 676c 6f62 616c 2d73 6563  --rio-global-sec
+00065880: 6f6e 6461 7279 2d62 6729 3b62 6f78 2d73  ondary-bg);box-s
+00065890: 6861 646f 773a 3020 3020 3472 656d 2031  hadow:0 0 4rem 1
+000658a0: 7265 6d20 7661 7228 2d2d 7269 6f2d 676c  rem var(--rio-gl
+000658b0: 6f62 616c 2d73 6563 6f6e 6461 7279 2d62  obal-secondary-b
+000658c0: 6729 3b6f 7061 6369 7479 3a2e 343b 616e  g);opacity:.4;an
+000658d0: 696d 6174 696f 6e3a 7075 6c73 6520 312e  imation:pulse 1.
+000658e0: 3473 2069 6e66 696e 6974 657d 2e72 696f  4s infinite}.rio
+000658f0: 2d73 6570 6172 6174 6f72 7b70 6f73 6974  -separator{posit
+00065900: 696f 6e3a 7265 6c61 7469 7665 3b62 6163  ion:relative;bac
 00065910: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
-00065920: 7228 2d2d 7365 7061 7261 746f 722d 636f  r(--separator-co
-00065930: 6c6f 7229 3b6f 7061 6369 7479 3a76 6172  lor);opacity:var
-00065940: 282d 2d73 6570 6172 6174 6f72 2d6f 7061  (--separator-opa
-00065950: 6369 7479 297d 2e72 696f 2d72 6970 706c  city)}.rio-rippl
-00065960: 652d 6566 6665 6374 7b70 6f69 6e74 6572  e-effect{pointer
-00065970: 2d65 7665 6e74 733a 6e6f 6e65 3b70 6f73  -events:none;pos
-00065980: 6974 696f 6e3a 6162 736f 6c75 7465 3b62  ition:absolute;b
-00065990: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
-000659a0: 7269 6f2d 7269 7070 6c65 2d63 6f6c 6f72  rio-ripple-color
-000659b0: 293b 626f 7264 6572 2d72 6164 6975 733a  );border-radius:
-000659c0: 3530 253b 7472 616e 7366 6f72 6d3a 7472  50%;transform:tr
-000659d0: 616e 736c 6174 6528 2d35 3025 2c2d 3530  anslate(-50%,-50
-000659e0: 2529 3b74 7261 6e73 6974 696f 6e3a 746f  %);transition:to
-000659f0: 7020 7661 7228 2d2d 7269 6f2d 7269 7070  p var(--rio-ripp
-00065a00: 6c65 2d64 7572 6174 696f 6e29 2c6c 6566  le-duration),lef
-00065a10: 7420 7661 7228 2d2d 7269 6f2d 7269 7070  t var(--rio-ripp
-00065a20: 6c65 2d64 7572 6174 696f 6e29 2c77 6964  le-duration),wid
-00065a30: 7468 2076 6172 282d 2d72 696f 2d72 6970  th var(--rio-rip
-00065a40: 706c 652d 6475 7261 7469 6f6e 292c 6865  ple-duration),he
-00065a50: 6967 6874 2076 6172 282d 2d72 696f 2d72  ight var(--rio-r
-00065a60: 6970 706c 652d 6475 7261 7469 6f6e 292c  ipple-duration),
-00065a70: 6f70 6163 6974 7920 7661 7228 2d2d 7269  opacity var(--ri
-00065a80: 6f2d 7269 7070 6c65 2d64 7572 6174 696f  o-ripple-duratio
-00065a90: 6e29 7d0a 0a3c 2f73 7479 6c65 3e0a 2020  n)}..</style>.  
-00065aa0: 2020 3c2f 6865 6164 3e0a 0a20 2020 203c    </head>..    <
-00065ab0: 626f 6479 2063 6c61 7373 3d22 7269 6f2d  body class="rio-
-00065ac0: 7377 6974 6368 6572 6f6f 2d62 6163 6b67  switcheroo-backg
-00065ad0: 726f 756e 6422 3e3c 2f62 6f64 793e 0a3c  round"></body>.<
-00065ae0: 2f68 746d 6c3e 0a                        /html>.
+00065920: 7228 2d2d 7269 6f2d 6c6f 6361 6c2d 6267  r(--rio-local-bg
+00065930: 297d 2e72 696f 2d73 6570 6172 6174 6f72  )}.rio-separator
+00065940: 3a61 6674 6572 7b63 6f6e 7465 6e74 3a22  :after{content:"
+00065950: 223b 706f 7369 7469 6f6e 3a61 6273 6f6c  ";position:absol
+00065960: 7574 653b 6c65 6674 3a30 3b74 6f70 3a30  ute;left:0;top:0
+00065970: 3b72 6967 6874 3a30 3b62 6f74 746f 6d3a  ;right:0;bottom:
+00065980: 303b 6261 636b 6772 6f75 6e64 2d63 6f6c  0;background-col
+00065990: 6f72 3a76 6172 282d 2d73 6570 6172 6174  or:var(--separat
+000659a0: 6f72 2d63 6f6c 6f72 293b 6f70 6163 6974  or-color);opacit
+000659b0: 793a 7661 7228 2d2d 7365 7061 7261 746f  y:var(--separato
+000659c0: 722d 6f70 6163 6974 7929 7d2e 7269 6f2d  r-opacity)}.rio-
+000659d0: 7269 7070 6c65 2d65 6666 6563 747b 706f  ripple-effect{po
+000659e0: 696e 7465 722d 6576 656e 7473 3a6e 6f6e  inter-events:non
+000659f0: 653b 706f 7369 7469 6f6e 3a61 6273 6f6c  e;position:absol
+00065a00: 7574 653b 6261 636b 6772 6f75 6e64 3a76  ute;background:v
+00065a10: 6172 282d 2d72 696f 2d72 6970 706c 652d  ar(--rio-ripple-
+00065a20: 636f 6c6f 7229 3b62 6f72 6465 722d 7261  color);border-ra
+00065a30: 6469 7573 3a35 3025 3b74 7261 6e73 666f  dius:50%;transfo
+00065a40: 726d 3a74 7261 6e73 6c61 7465 282d 3530  rm:translate(-50
+00065a50: 252c 2d35 3025 293b 7472 616e 7369 7469  %,-50%);transiti
+00065a60: 6f6e 3a74 6f70 2076 6172 282d 2d72 696f  on:top var(--rio
+00065a70: 2d72 6970 706c 652d 6475 7261 7469 6f6e  -ripple-duration
+00065a80: 292c 6c65 6674 2076 6172 282d 2d72 696f  ),left var(--rio
+00065a90: 2d72 6970 706c 652d 6475 7261 7469 6f6e  -ripple-duration
+00065aa0: 292c 7769 6474 6820 7661 7228 2d2d 7269  ),width var(--ri
+00065ab0: 6f2d 7269 7070 6c65 2d64 7572 6174 696f  o-ripple-duratio
+00065ac0: 6e29 2c68 6569 6768 7420 7661 7228 2d2d  n),height var(--
+00065ad0: 7269 6f2d 7269 7070 6c65 2d64 7572 6174  rio-ripple-durat
+00065ae0: 696f 6e29 2c6f 7061 6369 7479 2076 6172  ion),opacity var
+00065af0: 282d 2d72 696f 2d72 6970 706c 652d 6475  (--rio-ripple-du
+00065b00: 7261 7469 6f6e 297d 0a0a 3c2f 7374 796c  ration)}..</styl
+00065b10: 653e 0a20 2020 203c 2f68 6561 643e 0a0a  e>.    </head>..
+00065b20: 2020 2020 3c62 6f64 7920 636c 6173 733d      <body class=
+00065b30: 2272 696f 2d73 7769 7463 6865 726f 6f2d  "rio-switcheroo-
+00065b40: 6261 636b 6772 6f75 6e64 223e 3c2f 626f  background"></bo
+00065b50: 6479 3e0a 3c2f 6874 6d6c 3e0a            dy>.</html>.
```

### Comparing `rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.7.5/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/README.md` & `rio_ui-0.7.5/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/__init__.py` & `rio_ui-0.7.5/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/core-classes.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/core-classes.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/debugging-setup.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/debugging-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/deployment.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/deployment.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-custom-events.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-custom-events.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-install.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-install.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/persistent-settings.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/persistent-settings.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/project-setup.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/project-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/run-project.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/run-project.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/howtos/theming.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/howtos/theming.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/README.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/README.md` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.7.5/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/scripts/benchmark.py` & `rio_ui-0.7.5/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/scripts/build_material_icon_set.py` & `rio_ui-0.7.5/scripts/build_material_icon_set.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/scripts/code_coverage.py` & `rio_ui-0.7.5/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/scripts/publish_new_release.py` & `rio_ui-0.7.5/scripts/publish_new_release.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_attribute_bindings.py` & `rio_ui-0.7.5/tests/test_attribute_bindings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_custom_components.py` & `rio_ui-0.7.5/tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_docstring_code_blocks.py` & `rio_ui-0.7.5/tests/test_docstring_code_blocks.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_documentation.py` & `rio_ui-0.7.5/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_events.py` & `rio_ui-0.7.5/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_project_templates.py` & `rio_ui-0.7.5/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_reconciliation.py` & `rio_ui-0.7.5/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_refresh.py` & `rio_ui-0.7.5/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_session.py` & `rio_ui-0.7.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_testing_tools.py` & `rio_ui-0.7.5/tests/test_testing_tools.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_user_settings.py` & `rio_ui-0.7.5/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/test_zzz_guardrails.py` & `rio_ui-0.7.5/tests/test_zzz_guardrails.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/tests/utils.py` & `rio_ui-0.7.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/LICENSE.txt` & `rio_ui-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/README.md` & `rio_ui-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.4/pyproject.toml` & `rio_ui-0.7.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,36 @@
 description = "Build modern Websites and Apps just with Python"
 dynamic = ["version"]
 authors = [
     { name = "Jakob Pinterits", email = "jakob.pinterits@gmail.com" },
     { name = "Paul Pinterits", email = "rawing7@gmail.com" },
 ]
 dependencies = [
-    "aiofiles~=23.2.1",
     "fastapi~=0.110",
-    "fuzzywuzzy~=0.18.0",
+    "fuzzywuzzy~=0.18",
     "gitignore-parser~=0.1.9",
-    "httpx~=0.25.1",
+    "httpx~=0.25",
     "imy~=0.3.2",
     "introspection~=1.8",
-    "isort~=5.13.2",
-    "keyring~=24.3.0",
-    "matplotlib>=3.8.4",
-    "pillow~=10.2.0",
-    "pytest~=7.3.1",
-    "python-levenshtein~=0.23.0",
+    "isort~=5.13",
+    "keyring~=24.3",
+    "matplotlib>=3.8",
+    "pillow~=10.2",
+    "python-levenshtein~=0.23",
     "python-multipart~=0.0.6",
     "pytz~=2024.1",
     "revel~=0.9.1",
-    "timer-dict~=1.0.0",
-    "tomlkit~=0.12.3",
-    "typing-extensions>=4.5.0",
+    "timer-dict~=1.0",
+    "tomlkit~=0.12",
+    "typing-extensions>=4.5",
     "unicall~=0.1.5",
     "uniserde~=0.3.13",
     "uvicorn[standard]~=0.29.0",
-    "watchfiles~=0.21.0",
-    "yarl>=1.9.4",
+    "watchfiles~=0.21",
+    "yarl>=1.9",
 ]
 requires-python = ">= 3.10"
 readme = "README.md"
 license.file = "LICENSE.txt"
 keywords = [
     "web-development",
     "web-framework",
@@ -65,18 +63,19 @@
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.optional-dependencies]
 window = [
-    "platformdirs~=3.11.0",
-    "pywebview~=4.2.2",
+    "aiofiles~=23.2",
+    "platformdirs~=3.11",
+    "pywebview~=4.2",
     "cefpython3~=66.1 ; sys_platform == 'win32'",
-    "pygobject~=3.44.1 ; sys_platform == 'linux'",
+    "pygobject~=3.44 ; sys_platform == 'linux'",
 ]
 
 [project.urls]
 homepage = "https://rio.dev"
 documentation = "https://rio.dev/docs"
 
 [project.scripts]
@@ -84,26 +83,26 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 dev-dependencies = [
+    "aiofiles>=23.2.1",
     "alt-pytest-asyncio~=0.7.2",
-    "black~=24.4.0",
-    "coverage~=7.2.2",
-    "plotly>=5.22.0",
-    "pre-commit~=3.1.1",
-    "pytest~=7.3.1",
+    "black~=24.4",
+    "coverage~=7.2",
+    "pandas>=2.2",
+    "plotly>=5.22",
+    "polars>=0.20",
+    "pre-commit~=3.1",
     "pyright~=1.1.350",
+    "pytest~=7.3",
     "requests~=2.31",
-    "ruff~=0.4.1",
-    "pandas>=2.2.2",
-    "polars>=0.20.23",
-    "pywebview",
+    "ruff~=0.4",
 ]
 managed = true
 
 [tool.rye.scripts]
 build = "npm run build"
 dev-build = "npm run dev-build"
 publish = { call = "scripts.publish_new_release:main" }
```

### Comparing `rio_ui-0.7.4/PKG-INFO` & `rio_ui-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.7.4
+Version: 0.7.5
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: documentation, https://rio.dev/docs
 Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -217,43 +217,42 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
-Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: fastapi~=0.110
-Requires-Dist: fuzzywuzzy~=0.18.0
+Requires-Dist: fuzzywuzzy~=0.18
 Requires-Dist: gitignore-parser~=0.1.9
-Requires-Dist: httpx~=0.25.1
+Requires-Dist: httpx~=0.25
 Requires-Dist: imy~=0.3.2
 Requires-Dist: introspection~=1.8
-Requires-Dist: isort~=5.13.2
-Requires-Dist: keyring~=24.3.0
-Requires-Dist: matplotlib>=3.8.4
-Requires-Dist: pillow~=10.2.0
-Requires-Dist: pytest~=7.3.1
-Requires-Dist: python-levenshtein~=0.23.0
+Requires-Dist: isort~=5.13
+Requires-Dist: keyring~=24.3
+Requires-Dist: matplotlib>=3.8
+Requires-Dist: pillow~=10.2
+Requires-Dist: python-levenshtein~=0.23
 Requires-Dist: python-multipart~=0.0.6
 Requires-Dist: pytz~=2024.1
 Requires-Dist: revel~=0.9.1
-Requires-Dist: timer-dict~=1.0.0
-Requires-Dist: tomlkit~=0.12.3
-Requires-Dist: typing-extensions>=4.5.0
+Requires-Dist: timer-dict~=1.0
+Requires-Dist: tomlkit~=0.12
+Requires-Dist: typing-extensions>=4.5
 Requires-Dist: unicall~=0.1.5
 Requires-Dist: uniserde~=0.3.13
 Requires-Dist: uvicorn[standard]~=0.29.0
-Requires-Dist: watchfiles~=0.21.0
-Requires-Dist: yarl>=1.9.4
+Requires-Dist: watchfiles~=0.21
+Requires-Dist: yarl>=1.9
 Provides-Extra: window
+Requires-Dist: aiofiles~=23.2; extra == 'window'
 Requires-Dist: cefpython3~=66.1; (sys_platform == 'win32') and extra == 'window'
-Requires-Dist: platformdirs~=3.11.0; extra == 'window'
-Requires-Dist: pygobject~=3.44.1; (sys_platform == 'linux') and extra == 'window'
-Requires-Dist: pywebview~=4.2.2; extra == 'window'
+Requires-Dist: platformdirs~=3.11; extra == 'window'
+Requires-Dist: pygobject~=3.44; (sys_platform == 'linux') and extra == 'window'
+Requires-Dist: pywebview~=4.2; extra == 'window'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem; height: 8.8rem"/>
 </p>
 
 <p align="center">
```

