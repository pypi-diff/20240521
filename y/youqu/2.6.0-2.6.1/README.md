# Comparing `tmp/youqu-2.6.0.tar.gz` & `tmp/youqu-2.6.1.tar.gz`

## Comparing `youqu-2.6.0.tar` & `youqu-2.6.1.tar`

### file list

```diff
@@ -1,228 +1,228 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/CURRENT
--rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/conftest.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/env.sh
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/manage.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/pytest.ini
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/ruff.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/apps/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/__init__.py
--rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/globalconfig.ini
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/globalconfig.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/playbook.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/pmsmark.ini
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/pylintrc.cfg
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/skipif.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/sleepx.ini
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/subcmd.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/ci.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/language.ini
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/${app_name}_assert.py-tpl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/.gitignore-tpl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/__init__.py-tpl
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/config.ini-tpl
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/config.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/conftest.py-tpl
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/control-tpl
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/mycase.csv-tpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/__init__.py-tpl
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/base_case.py-tpl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/case/assert_res/readme
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/__init__.py-tpl
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/base_widget.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/other.ini-tpl
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/other_widget.py-tpl
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/ui.ini-tpl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/case_res/readme
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/setting/template/app_template/widget/pic_res/readme
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/__init__.py
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/assert_common.py
--rw-r--r--   0        0        0    26398 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/button_center.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/calculate.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/cmdctl.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/csvctl.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/custom_exception.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/dbus_utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/desktop.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/dogtail_utils.py
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/filectl.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/filter_image.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/image_utils.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/mouse_key.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/ocr_utils.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pinyin.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/read_csv.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/read_toml.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/recording_screen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/requestx.py
--rw-r--r--   0        0        0    15610 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/shortcut.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/singleton.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/sleepx.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/startapp.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/startproject.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/video_utils.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/wayland_wininfo.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/webui.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/ydotool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/__version__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/cli.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/colors.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/consts.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/py.typed
--rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/3d.json
--rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/block.json
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/chrome.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/grid.json
--rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/huge.json
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/pallet.json
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/shade.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple3d.json
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/simpleBlock.json
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/slick.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/cfonts/fonts/tiny.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/colorama/winterm.py
--rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/COPYING
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/__init__.py
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/config.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/dump.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/errors.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/i18n.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/path.py
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/predicate.py
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/procedural.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/rawinput.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/rawinput_wayland.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/sessions.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/tc.py
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/tree.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/wrapped.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head-48.png
--rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head.svg
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
--rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail.svg
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/LICENSE.txt
--rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_java.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_osx.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_wayland.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_win.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_x11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/__init__.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/generictreemodel.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/meson.build
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/pygtkcompat/pygtkcompat.py
--rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/sniff
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/sniff.desktop
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/sniff.ui
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/button.xpm
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/checkbutton.xpm
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/checkmenuitem.xpm
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/colorselection.xpm
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/combo.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/dialog.xpm
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/image.xpm
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/label.xpm
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/menubar.xpm
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/menuitem.xpm
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/notebook.xpm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/scrolledwindow.xpm
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/spinbutton.xpm
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/statusbar.xpm
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/table.xpm
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/text.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/toolbar.xpm
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/tree.xpm
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/treeitem.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/unknown.xpm
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/viewport.xpm
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/vscrollbar.xpm
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/vseparator.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/sniff/icons/window.xpm
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/CMakeLists.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/README.md
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.cpp
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/install.sh
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/wayland_autotool/main.cpp
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/.editorconfig
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/CMakeLists.txt
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/LICENSE
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_click.c
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_key.c
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_mousemove.c
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_type.c
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.c
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.h
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotool.service.in
--rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotoold.c
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/manpage/CMakeLists.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotool.1.scd
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/_cargo.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/check.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/clone.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/code_statistics.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/git/commit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/__init__.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/allure_report_extend.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/emoji_hooks.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/plugins/mng.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/__init__.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/_base.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/_cargo.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/csv2pms.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/pms2csv.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/send2pms.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/suite.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/pms/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/__init__.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/_base.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/_remote_dogtail_ctl.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/_remote_other_ctl.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/remotectl/remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/__init__.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/_base.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/_cargo.py
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/local_runner.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/playbook.py
--rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/rtk/remote_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/__init__.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/_env_base.sh
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/check_python_source.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/command_complete.sh
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/docs_env.sh
--rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/env_dev.sh
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/env_vir.sh
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/opencv_rpc_server.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/pylint.sh
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sslclone.sh
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_deb.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_depends.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_env_cut.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_remote.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_sources.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/sub_webui.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/src/utils/vnc.sh
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 youqu-2.6.0/youqu/README.md
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 youqu-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/CURRENT
+-rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/conftest.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/env.sh
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/manage.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/pytest.ini
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/ruff.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/apps/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/__init__.py
+-rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/globalconfig.ini
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/globalconfig.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/playbook.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/pmsmark.ini
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/pylintrc.cfg
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/skipif.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/sleepx.ini
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/subcmd.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/ci.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/language.ini
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/${app_name}_assert.py-tpl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/.gitignore-tpl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/config.ini-tpl
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/config.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/conftest.py-tpl
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/control-tpl
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/mycase.csv-tpl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/__init__.py-tpl
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/base_case.py-tpl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/assert_res/readme
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/__init__.py-tpl
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/base_widget.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/other.ini-tpl
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/other_widget.py-tpl
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/ui.ini-tpl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/case_res/readme
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/pic_res/readme
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/__init__.py
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/assert_common.py
+-rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/button_center.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/calculate.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/cmdctl.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/csvctl.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/custom_exception.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/dbus_utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/desktop.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/dogtail_utils.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/filectl.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/filter_image.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/image_utils.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/mouse_key.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/ocr_utils.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pinyin.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/read_csv.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/read_toml.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/recording_screen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/requestx.py
+-rw-r--r--   0        0        0    15610 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/shortcut.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/singleton.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/sleepx.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/startapp.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/startproject.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/video_utils.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/wayland_wininfo.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/webui.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/ydotool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/__version__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/cli.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/colors.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/consts.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/py.typed
+-rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/3d.json
+-rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/block.json
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/chrome.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/grid.json
+-rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/huge.json
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/pallet.json
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/shade.json
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple3d.json
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/simpleBlock.json
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/slick.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/tiny.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/winterm.py
+-rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/COPYING
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/__init__.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/config.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/dump.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/errors.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/i18n.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/path.py
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/predicate.py
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/procedural.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/rawinput.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/rawinput_wayland.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/sessions.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/tc.py
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/tree.py
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/wrapped.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head-48.png
+-rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head.svg
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
+-rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail.svg
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/LICENSE.txt
+-rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_java.py
+-rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_osx.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_wayland.py
+-rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_win.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_x11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/__init__.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/generictreemodel.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/meson.build
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/pygtkcompat.py
+-rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/sniff
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/sniff.desktop
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/sniff.ui
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/button.xpm
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/checkbutton.xpm
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/checkmenuitem.xpm
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/colorselection.xpm
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/combo.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/dialog.xpm
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/image.xpm
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/label.xpm
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/menubar.xpm
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/menuitem.xpm
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/notebook.xpm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/scrolledwindow.xpm
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/spinbutton.xpm
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/statusbar.xpm
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/table.xpm
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/text.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/toolbar.xpm
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/tree.xpm
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/treeitem.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/unknown.xpm
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/viewport.xpm
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/vscrollbar.xpm
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/vseparator.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/window.xpm
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/CMakeLists.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/README.md
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.cpp
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/install.sh
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/main.cpp
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/.editorconfig
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/CMakeLists.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/LICENSE
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_click.c
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_key.c
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_mousemove.c
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_type.c
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.c
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.h
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotool.service.in
+-rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotoold.c
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/manpage/CMakeLists.txt
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotool.1.scd
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/__init__.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/_cargo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/check.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/clone.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/code_statistics.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/commit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/__init__.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/allure_report_extend.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/emoji_hooks.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/mng.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/__init__.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/_base.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/_cargo.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/csv2pms.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/pms2csv.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/send2pms.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/suite.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/__init__.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/_base.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/_remote_dogtail_ctl.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/_remote_other_ctl.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/__init__.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/_base.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/_cargo.py
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/local_runner.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/playbook.py
+-rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/remote_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/__init__.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/_env_base.sh
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/check_python_source.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/command_complete.sh
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/docs_env.sh
+-rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/env_dev.sh
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/env_vir.sh
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/opencv_rpc_server.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/pylint.sh
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sslclone.sh
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_deb.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_depends.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_env_cut.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_remote.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_sources.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_webui.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/vnc.sh
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/README.md
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 youqu-2.6.1/PKG-INFO
```

### Comparing `youqu-2.6.0/youqu/conftest.py` & `youqu-2.6.1/youqu/conftest.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/env.sh` & `youqu-2.6.1/youqu/env.sh`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ps -ef | grep -v grep | grep kwin_x11
     [ $? = 0 ] && DISPLAY_SERVER=x11 || DISPLAY_SERVER=wayland
 fi
 PYTHON_VERSION=$(python3 -c "import sys; print(f'{sys.version_info.major}.{sys.version_info.minor}')")
 whitelist="/usr/share/deepin-elf-verify/whitelist"
 pypi_mirror="https://pypi.tuna.tsinghua.edu.cn/simple"
 
-echo "${PASSWORD}" | sudo -S su
+echo "${PASSWORD}" | sudo -S su > /dev/null 2>&1
 
 if [ ! -f "$HOME/.Xauthority" ]; then
         touch $HOME/.Xauthority
 fi
 
 if [ "${DEV}" = "true" ]; then
     source ./src/utils/env_dev.sh
```

### Comparing `youqu-2.6.0/youqu/manage.py` & `youqu-2.6.1/youqu/manage.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/ruff.toml` & `youqu-2.6.1/youqu/ruff.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/startproject.py` & `youqu-2.6.1/youqu/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/globalconfig.ini` & `youqu-2.6.1/youqu/setting/globalconfig.ini`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/globalconfig.py` & `youqu-2.6.1/youqu/setting/globalconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,21 +188,21 @@
         log_cli.get("CLASS_NAME_CONTAIN", default="ShortCut")
         .replace(" ", "")
         .split(",")
     )
 
     # [git]
     git_cfg = GetCfg(GLOBAL_CONFIG_FILE_PATH, "git")
-    GIT_URL = log_cli.get("GIT_URL", default="")
-    GTI_USER = log_cli.get("GTI_USER", default="")
-    GIT_PASSWORD = log_cli.get("GIT_PASSWORD", default="")
-    BRANCH = log_cli.get("BRANCH", default="")
-    DEPTH = log_cli.get("DEPTH", default="")
-    START_DATE = log_cli.get("STAR_TDATE", default="")
-    END_DATE = log_cli.get("END_DATE", default="")
+    GIT_URL = git_cfg.get("GIT_URL", default="")
+    GIT_USER = git_cfg.get("GTI_USER", default="")
+    GIT_PASSWORD = git_cfg.get("GIT_PASSWORD", default="")
+    BRANCH = git_cfg.get("BRANCH", default="")
+    DEPTH = git_cfg.get("DEPTH", default="")
+    START_DATE = git_cfg.get("START_DATE", default="")
+    END_DATE = git_cfg.get("END_DATE", default="")
 
     # ====================== 动态获取变量 ======================
     VERSION = ""
     if exists("/etc/os-version"):
         version_cfg = GetCfg("/etc/os-version", "Version")
         VERSION = (version_cfg.get("EditionName[zh_CN]") or "") + (
                 version_cfg.get("MinorVersion") or ""
@@ -253,15 +253,15 @@
 
     IS_X11 = DISPLAY_SERVER == DisplayServer.x11
     IS_WAYLAND = DISPLAY_SERVER == DisplayServer.wayland
 
     top_cmd = "top -b -d 3 -w 512"
 
     GITHUB_URL = "https://github.com/linuxdeepin/youqu"
-    DOCS_URL = "https://linuxdeepin.github.io/youqu"
+    DOCS_URL = "https://youqu.uniontech.com/"
     PyPI_URL = "https://pypi.org/project/youqu"
 
     LETMEGO_DEBUG = True
     DTK_DISPLAY = False
 
 
 GlobalConfig = _GlobalConfig()
```

### Comparing `youqu-2.6.0/youqu/setting/playbook.toml` & `youqu-2.6.1/youqu/setting/playbook.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/pylintrc.cfg` & `youqu-2.6.1/youqu/setting/pylintrc.cfg`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/template/app_template/config.py-tpl` & `youqu-2.6.1/youqu/setting/template/app_template/config.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/template/app_template/case/test_mycase_002.py-tpl` & `youqu-2.6.1/youqu/setting/template/app_template/case/test_mycase_002.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/template/app_template/widget/base_widget.py-tpl` & `youqu-2.6.1/youqu/setting/template/app_template/widget/base_widget.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/setting/template/app_template/widget/ui.ini-tpl` & `youqu-2.6.1/youqu/setting/template/app_template/widget/ui.ini-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/__init__.py` & `youqu-2.6.1/youqu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/assert_common.py` & `youqu-2.6.1/youqu/src/assert_common.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/button_center.py` & `youqu-2.6.1/youqu/src/button_center.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,12 +643,12 @@
                 )
                 app_id_list = [int(_id) for _id in app_id if _id]  # to int
                 app_id_list.sort()
                 return app_id_list[-1]
             except Exception as exc:
                 raise ApplicationStartError(f"{app_name, exc}") from exc
         else:
-            info = self.wwininfo.window_info().get(self.app_name)
+            info = WaylandWindowInfo().window_info().get(self.app_name)
             if isinstance(info, dict):
                 return info.get("window_id")
             elif isinstance(info, list):
                 return info[-1].get("window_id")
```

### Comparing `youqu-2.6.0/youqu/src/calculate.py` & `youqu-2.6.1/youqu/src/calculate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/cmdctl.py` & `youqu-2.6.1/youqu/src/cmdctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/csvctl.py` & `youqu-2.6.1/youqu/src/csvctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/custom_exception.py` & `youqu-2.6.1/youqu/src/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/dbus_utils.py` & `youqu-2.6.1/youqu/src/dbus_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/desktop.py` & `youqu-2.6.1/youqu/src/desktop.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/dogtail_utils.py` & `youqu-2.6.1/youqu/src/dogtail_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/filectl.py` & `youqu-2.6.1/youqu/src/filectl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/filter_image.py` & `youqu-2.6.1/youqu/src/filter_image.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/image_utils.py` & `youqu-2.6.1/youqu/src/image_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/mouse_key.py` & `youqu-2.6.1/youqu/src/mouse_key.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/ocr_utils.py` & `youqu-2.6.1/youqu/src/ocr_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,42 +85,42 @@
         cls.result = cls.ocr(*args, **kwargs)
         if isinstance(cls.result, tuple):
             cls.x, cls.y = cls.result
             return cls
         return cls.result
 
     @classmethod
-    def check_xy(cls):
+    def _check_xy(cls):
         if cls.x is None and cls.y is None:
-            raise ValueError("ocr_pro 没有识别到")
+            raise ValueError("ocrx 没有识别到")
 
     @classmethod
     def click(cls):
         from src.mouse_key import MouseKey
-        cls.check_xy()
+        cls._check_xy()
         MouseKey.click(cls.x, cls.y)
         return cls
 
     @classmethod
     def right_click(cls):
         from src.mouse_key import MouseKey
-        cls.check_xy()
+        cls._check_xy()
         MouseKey.right_click(cls.x, cls.y)
         return cls
 
     @classmethod
     def double_click(cls):
         from src.mouse_key import MouseKey
-        cls.check_xy()
+        cls._check_xy()
         MouseKey.double_click(cls.x, cls.y)
         return cls
 
     @classmethod
     def center(cls):
-        cls.check_xy()
+        cls._check_xy()
         return cls.x, cls.y
 
     @classmethod
     def all_result(cls):
         return cls.result
```

### Comparing `youqu-2.6.0/youqu/src/pinyin.py` & `youqu-2.6.1/youqu/src/pinyin.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/read_csv.py` & `youqu-2.6.1/youqu/src/read_csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/recording_screen.py` & `youqu-2.6.1/youqu/src/recording_screen.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/requestx.py` & `youqu-2.6.1/youqu/src/requestx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/shortcut.py` & `youqu-2.6.1/youqu/src/shortcut.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/singleton.py` & `youqu-2.6.1/youqu/src/singleton.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/sleepx.py` & `youqu-2.6.1/youqu/src/sleepx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/startapp.py` & `youqu-2.6.1/youqu/src/startapp.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/startproject.py` & `youqu-2.6.1/youqu/src/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/video_utils.py` & `youqu-2.6.1/youqu/src/video_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/wayland_wininfo.py` & `youqu-2.6.1/youqu/src/wayland_wininfo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/webui.py` & `youqu-2.6.1/youqu/src/webui.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/ydotool.py` & `youqu-2.6.1/youqu/src/ydotool.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/cli.py` & `youqu-2.6.1/youqu/src/depends/cfonts/cli.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/colors.py` & `youqu-2.6.1/youqu/src/depends/cfonts/colors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/consts.py` & `youqu-2.6.1/youqu/src/depends/cfonts/consts.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/core.py` & `youqu-2.6.1/youqu/src/depends/cfonts/core.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/3d.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/block.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/block.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/chrome.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/chrome.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/grid.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/grid.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/huge.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/huge.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/pallet.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/pallet.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/shade.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/shade.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/simple3d.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/simpleBlock.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/simpleBlock.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/slick.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/slick.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/cfonts/fonts/tiny.json` & `youqu-2.6.1/youqu/src/depends/cfonts/fonts/tiny.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/colorama/ansi.py` & `youqu-2.6.1/youqu/src/depends/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/colorama/ansitowin32.py` & `youqu-2.6.1/youqu/src/depends/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/colorama/initialise.py` & `youqu-2.6.1/youqu/src/depends/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/colorama/win32.py` & `youqu-2.6.1/youqu/src/depends/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/colorama/winterm.py` & `youqu-2.6.1/youqu/src/depends/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/COPYING` & `youqu-2.6.1/youqu/src/depends/dogtail/COPYING`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/__init__.py` & `youqu-2.6.1/youqu/src/depends/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/config.py` & `youqu-2.6.1/youqu/src/depends/dogtail/config.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/distro.py` & `youqu-2.6.1/youqu/src/depends/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/dump.py` & `youqu-2.6.1/youqu/src/depends/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/errors.py` & `youqu-2.6.1/youqu/src/depends/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/i18n.py` & `youqu-2.6.1/youqu/src/depends/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/logging.py` & `youqu-2.6.1/youqu/src/depends/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/path.py` & `youqu-2.6.1/youqu/src/depends/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/predicate.py` & `youqu-2.6.1/youqu/src/depends/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/procedural.py` & `youqu-2.6.1/youqu/src/depends/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/rawinput.py` & `youqu-2.6.1/youqu/src/depends/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/rawinput_wayland.py` & `youqu-2.6.1/youqu/src/depends/dogtail/rawinput_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/sessions.py` & `youqu-2.6.1/youqu/src/depends/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/tc.py` & `youqu-2.6.1/youqu/src/depends/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/tree.py` & `youqu-2.6.1/youqu/src/depends/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/utils.py` & `youqu-2.6.1/youqu/src/depends/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/version.py` & `youqu-2.6.1/youqu/src/depends/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/wrapped.py` & `youqu-2.6.1/youqu/src/depends/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head-48.png` & `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-head.svg` & `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail-48.png` & `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/dogtail/icons/dogtail-tail.svg` & `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pyautogui/LICENSE.txt` & `youqu-2.6.1/youqu/src/depends/pyautogui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pyautogui/__init__.py` & `youqu-2.6.1/youqu/src/depends/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_osx.py` & `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_wayland.py` & `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_win.py` & `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pyautogui/_pyautogui_x11.py` & `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pygtkcompat/__init__.py` & `youqu-2.6.1/youqu/src/depends/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pygtkcompat/generictreemodel.py` & `youqu-2.6.1/youqu/src/depends/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/pygtkcompat/pygtkcompat.py` & `youqu-2.6.1/youqu/src/depends/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/sniff` & `youqu-2.6.1/youqu/src/depends/sniff/sniff`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/sniff.ui` & `youqu-2.6.1/youqu/src/depends/sniff/sniff.ui`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/button.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/button.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/checkbutton.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/checkbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/checkmenuitem.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/checkmenuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/colorselection.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/colorselection.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/combo.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/combo.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/dialog.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/dialog.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/image.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/image.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/label.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/label.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/menubar.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/menubar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/menuitem.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/menuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/notebook.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/notebook.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/scrolledwindow.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/scrolledwindow.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/spinbutton.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/spinbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/statusbar.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/statusbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/table.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/table.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/text.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/text.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/toolbar.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/toolbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/tree.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/tree.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/treeitem.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/treeitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/unknown.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/unknown.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/viewport.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/viewport.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/vscrollbar.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/vscrollbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/vseparator.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/vseparator.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/sniff/icons/window.xpm` & `youqu-2.6.1/youqu/src/depends/sniff/icons/window.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/wayland_autotool/CMakeLists.txt` & `youqu-2.6.1/youqu/src/depends/wayland_autotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.cpp` & `youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/wayland_autotool/autotool.h` & `youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/wayland_autotool/main.cpp` & `youqu-2.6.1/youqu/src/depends/wayland_autotool/main.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/CMakeLists.txt` & `youqu-2.6.1/youqu/src/depends/ydotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/LICENSE` & `youqu-2.6.1/youqu/src/depends/ydotool/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_click.c` & `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_click.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_key.c` & `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_key.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_mousemove.c` & `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_mousemove.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Client/tool_type.c` & `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_type.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.c` & `youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Client/ydotool.h` & `youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/Daemon/ydotoold.c` & `youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotoold.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotool.1.scd` & `youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotool.1.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/depends/ydotool/manpage/ydotoold.8.scd` & `youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotoold.8.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/git/_cargo.py` & `youqu-2.6.1/youqu/src/git/_cargo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def git_control(self, parser=None, sub_parser_git=None):
+def git_control(parser=None, sub_parser_git=None):
     sub_parser_git.add_argument(
         "-a",
         "--app",
         default="",
         help="应用名称：apps/autotest_deepin_music 或 autotest_deepin_music",
     )
     sub_parser_git.add_argument("-u", "--user", default="", help="git仓库用户名")
@@ -10,24 +10,25 @@
     sub_parser_git.add_argument("-l", "--url", default="", help="git仓库地址")
     sub_parser_git.add_argument("-b", "--branch_or_tag", default="", help="分支或Tag")
     sub_parser_git.add_argument("-d", "--depth", default="", help="git仓库克隆深度")
     sub_parser_git.add_argument("-s", "--startdate", default="", help="统计开始时间")
     sub_parser_git.add_argument("-e", "--enddate", default="", help="统计结束时间")
     args = parser.parse_args()
     from src.rtk._base import Args
+    from setting import conf
 
     git_kwargs = {
-        Args.app_name.value: args.app or self.default_app,
-        Args.url.value: args.url or self.default_url,
-        Args.user.value: args.user or self.default_git_user,
-        Args.password.value: args.password or self.default_git_password,
-        Args.branch.value: args.branch or self.default_branch,
-        Args.depth.value: args.depth or self.default_depth,
-        Args.startdate.value: args.startdate or self.default_startdate,
-        Args.enddate.value: args.enddate or self.default_enddate,
+        Args.app_name.value: args.app or conf.APP_NAME,
+        Args.url.value: args.url or conf.GIT_URL,
+        Args.user.value: args.user or conf.GIT_USER,
+        Args.password.value: args.password or conf.GIT_PASSWORD,
+        Args.branch.value: args.branch_or_tag or conf.BRANCH,
+        Args.depth.value: args.depth or conf.DEPTH,
+        Args.startdate.value: args.startdate or conf.START_DATE,
+        Args.enddate.value: args.enddate or conf.END_DATE,
     }
     from src.git.check import check_git_installed
 
     if git_kwargs.get(Args.url.value):
         if all(
             [
                 git_kwargs.get(Args.user.value),
@@ -35,17 +36,17 @@
             ]
         ):
             from src.git.clone import sslclone as git_clone
         else:
             from src.git.clone import clone as git_clone
         check_git_installed()
         git_clone(**git_kwargs)
-    if all(
-        [
-            git_kwargs.get(Args.app_name.value),
-            git_kwargs.get(Args.startdate.value),
-        ]
-    ):
-        from src.git.code_statistics import CodeStatistics
+    if git_kwargs.get(Args.app_name.value):
+        if git_kwargs.get(Args.startdate.value):
+            from src.git.code_statistics import CodeStatistics
 
-        check_git_installed()
-        CodeStatistics(**git_kwargs).codex()
+            check_git_installed()
+            CodeStatistics(**git_kwargs).codex()
+        else:
+            print("-s/--startdate 参数未传入")
+    else:
+        print("-a/--app 参数未传入")
```

### Comparing `youqu-2.6.0/youqu/src/git/clone.py` & `youqu-2.6.1/youqu/src/git/clone.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/git/code_statistics.py` & `youqu-2.6.1/youqu/src/git/code_statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
-import os
 import json
+import os
 from copy import deepcopy
 from datetime import datetime
 
 from setting import conf
-from src.rtk._base import transform_app_name
-from src.git.commit import Commit
 from src.depends.colorama import Fore
+from src.git.commit import Commit
+from src.rtk._base import transform_app_name
+from src import logger
 
 
 class CodeStatistics(Commit):
     __author__ = "mikigo<huangmingqiang@uniontech.com>"
 
     def __init__(
-        self,
-        app_name: str,
-        branch: str,
-        startdate: str = None,
-        enddate: str = None,
-        **kwargs,
+            self,
+            app_name: str,
+            branch: str,
+            startdate: str = None,
+            enddate: str = None,
+            **kwargs,
     ):
         self.app_name = transform_app_name(app_name or conf.APP_NAME)
         self.repo_path = f"{conf.APPS_PATH}/{self.app_name}"
         self.branch = branch or conf.BRANCH
         self.startdate = startdate or conf.START_DATE
 
         if startdate:
             super().__init__(app_name, branch=branch, startdate=startdate, enddate=enddate)
-        self.ignore_txt = ["from", "import"]
+        self.ignore_txt = ["from", "import", '"""', '    """', "class", "#", "@"]
 
         for i in range(100):
             self.ignore_txt.append(" " * i + "#")
 
     def get_git_files(self, commit_id, max_width=10000):
         git_files = []
         _files = os.popen(f"cd {self.repo_path};git show --stat={max_width} {commit_id}").read()
@@ -56,17 +57,17 @@
         fix_test_case_num = 0
         new_method_num = 0
         del_method_num = 0
         fix_method_num = 0
         git_files = self.get_git_files(commit_id=commit_id)
         for filepath in git_files:
             filename = filepath.split("/")[-1]
-            dif_texts = os.popen(f"cd {self.repo_path}/;git show {commit_id} {filepath}").read()
-            print(Fore.GREEN, "=" * 100, Fore.RESET)
-            print(filepath, "\n", dif_texts)
+            dif_texts = os.popen(f"cd {self.repo_path}/;git show {commit_id} -- {filepath}").read()
+            logger.info(Fore.GREEN + ("=" * 100) + Fore.RESET)
+            logger.info(filepath + "\n" + dif_texts)
             dif_lines = dif_texts.splitlines()
             # case
             if filename.startswith("test_"):
                 for line in dif_lines:
                     if line.startswith("--- /dev/null"):
                         new_test_case_num += 1
                         break
@@ -97,15 +98,19 @@
                     method_name = method.get("name")
                     method_content = method.get("method_content")
 
                     if method_name is None:
                         if method_content:
                             for content in method_content:
                                 if content.startswith(("-", "+")):
-                                    if content[1:].startswith(tuple(self.ignore_txt)):
+                                    if any([
+                                        content[1:].startswith(tuple(self.ignore_txt)),
+                                        content[1:] == "",
+                                        content[1:].endswith(('"""', "@staticmethod", "@classmethod"))
+                                    ]):
                                         continue
                                     _fix_debug.append(method)
                                     fix_method_num += 1
                                     break
 
                     # 正常出现的方法
                     # 方法名称是+开头，直接视为新增方法
@@ -115,14 +120,19 @@
                     # 方法名称是-开头，直接视为删除方法
                     elif method_name.startswith("-"):
                         del_method_num += 1
                     else:
                         if method_content:
                             for content in method_content:
                                 if content.startswith(("-", "+")):
+                                    if any([
+                                        content[1:] == "",
+                                        content[1:].endswith(('"""', "@staticmethod", "@classmethod"))
+                                    ]):
+                                        continue
                                     _fix_debug.append(method)
                                     fix_method_num += 1
                                     break
 
         res = {
             "commit_id": commit_id,
             "author": author,
@@ -144,16 +154,16 @@
             conf.REPORT_PATH,
             f"{self.app_name}_git_commit_result{f'_detail' if detail else ''}.json",
         )
         with open(result_file, "w", encoding="utf-8") as f:
             f.write(json.dumps(res, ensure_ascii=False, indent=4, default=None))
 
         with open(result_file, "r", encoding="utf-8") as f:
-            print(f.read())
-        print(f"{Fore.GREEN}数据结果{'详细' if detail else '汇总'}报告：{result_file}{Fore.RESET}")
+            logger.info(f.read())
+        logger.info(f"{Fore.GREEN}数据结果{'详细' if detail else '汇总'}报告：{result_file}{Fore.RESET}")
 
     def codex(self):
         results = None
         results_detail = []
         if self.startdate:
             commit_id_pairs = self.commit_id()
             results = {}
@@ -180,15 +190,15 @@
                     results[author]["删除方法"] += del_method_num
                     results[author]["修改方法"] += fix_method_num
                     results[author]["commit_id"] = commit_id
                     results[author]["git_dt_end"] = _git_dt
 
         if results is None:
             raise ValueError()
-        print(Fore.GREEN, "=" * 100, Fore.RESET)
+        logger.info(Fore.GREEN +  ("=" * 100) + Fore.RESET)
         self.write_result(results)
         if results_detail:
             self.write_result(results_detail, detail=True)
 
 
 if __name__ == "__main__":
     app_name = "apps/autotest_deepin_kwin_UI"
```

### Comparing `youqu-2.6.0/youqu/src/git/commit.py` & `youqu-2.6.1/youqu/src/git/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     __author__ = "mikigo<huangmingqiang@uniontech.com>"
 
     def __init__(self, app_name: str, branch: str, startdate: str, enddate: str = None):
         self.app_name = transform_app_name(app_name)
         self.startdate = datetime.strptime(startdate, "%Y-%m-%d")
         self.enddate = (
             self.now_dt
-            if enddate is None
+            if enddate == ""
             else datetime.strptime(enddate, "%Y-%m-%d") + timedelta(days=1)
         )
         self.branch = branch
         if self.branch is None:
             raise ValueError("branch 参数必传")
 
     @property
```

### Comparing `youqu-2.6.0/youqu/src/plugins/allure_report_extend.py` & `youqu-2.6.1/youqu/src/plugins/allure_report_extend.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/plugins/emoji_hooks.py` & `youqu-2.6.1/youqu/src/plugins/emoji_hooks.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/plugins/mng.py` & `youqu-2.6.1/youqu/src/plugins/mng.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/_base.py` & `youqu-2.6.1/youqu/src/pms/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/_cargo.py` & `youqu-2.6.1/youqu/src/pms/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/csv2pms.py` & `youqu-2.6.1/youqu/src/pms/csv2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/pms2csv.py` & `youqu-2.6.1/youqu/src/pms/pms2csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/send2pms.py` & `youqu-2.6.1/youqu/src/pms/send2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/suite.py` & `youqu-2.6.1/youqu/src/pms/suite.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/pms/task.py` & `youqu-2.6.1/youqu/src/pms/task.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/remotectl/_base.py` & `youqu-2.6.1/youqu/src/remotectl/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/remotectl/_remote_dogtail_ctl.py` & `youqu-2.6.1/youqu/src/remotectl/_remote_dogtail_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/remotectl/_remote_other_ctl.py` & `youqu-2.6.1/youqu/src/remotectl/_remote_other_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/remotectl/remote.py` & `youqu-2.6.1/youqu/src/remotectl/remote.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/rtk/_base.py` & `youqu-2.6.1/youqu/src/rtk/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,19 +81,20 @@
         if dir_name == app_name:
             return app_name
     raise NotADirectoryError(f"{app_name} 目录不存在")
 
 
 def collect_result(results):
     res = Counter([results.get(i).get("result") for i in results])
-    total = sum(res.values())
+    _total = sum(res.values())
     skiped = res.get("skip", 0)
+    total = _total - skiped
     passed = res.get("pass", 0)
-    failed = total - skiped - passed
-    pass_rate = f"{round((passed / (total - skiped)) * 100, 2)}%" if passed else "0%"
+    failed = total - passed
+    pass_rate = f"{round((passed / total) * 100, 2)}%" if passed else "0%"
     return total, failed, passed, skiped, pass_rate
 
 
 def get_result(ci_result):
     with open(ci_result, "r", encoding="utf-8") as _f:
         results_dict = json.load(_f)
     return collect_result(results_dict)
@@ -121,9 +122,10 @@
         results["pass_rate"],
     ) = get_result(ci_result_path)
 
     json_res_path = f"{GlobalConfig.ROOT_DIR}/{project_name}_at.json"
     with open(json_res_path, "w+", encoding="utf-8") as _f:
         _f.write(json.dumps(results, indent=2, ensure_ascii=False))
     sleep(1)
+    from src import logger
     with open(json_res_path, "r", encoding="utf-8") as _f:
-        print("CICD数据结果:\n", _f.read())
+        logger.info("CICD数据结果:\n", _f.read())
```

### Comparing `youqu-2.6.0/youqu/src/rtk/_cargo.py` & `youqu-2.6.1/youqu/src/rtk/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/rtk/local_runner.py` & `youqu-2.6.1/youqu/src/rtk/local_runner.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/rtk/playbook.py` & `youqu-2.6.1/youqu/src/rtk/playbook.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/rtk/remote_runner.py` & `youqu-2.6.1/youqu/src/rtk/remote_runner.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/_env_base.sh` & `youqu-2.6.1/youqu/src/utils/_env_base.sh`

 * *Files 2% similar despite different names*

```diff
@@ -61,21 +61,21 @@
 
 system_env(){
     echo "${PASSWORD}" | sudo -S su  > /dev/null 2>&1
     sudo sed -i "s/#PubkeyAuthentication yes/PubkeyAuthentication yes/g" /etc/ssh/sshd_config > /dev/null 2>&1
     sudo sed -i "s/#   StrictHostKeyChecking ask/   StrictHostKeyChecking no/g" /etc/ssh/ssh_config  > /dev/null 2>&1
     cat $HOME/.bashrc | grep 'export DISPLAY=":0"' > /dev/null 2>&1
     if [ $? -ne 0 ]; then
+         echo 'export PIPENV_VERBOSITY=-1' >> $HOME/.bashrc
          echo 'export DISPLAY=":0"' >> $HOME/.bashrc
          echo 'export QT_QPA_PLATFORM=' >> $HOME/.bashrc
          echo 'export QT_ACCESSIBILITY=1' >> $HOME/.bashrc
          echo 'export QT_LINUX_ACCESSIBILITY_ALWAYS_ON=1' >> $HOME/.bashrc
     fi
     source $HOME/.bashrc
-    sudo rm -rf /usr/local/lib/python${PYTHON_VERSION}/dist-packages/*.pth
     echo "cd ${ROOT_DIR}/src/depends/sniff/;python3 sniff" | sudo tee /usr/bin/sniff > /dev/null 2>&1
     sudo chmod +x /usr/bin/sniff
 
     gsettings set org.gnome.desktop.interface toolkit-accessibility true  > /dev/null 2>&1
     sudo systemctl enable ssh  > /dev/null 2>&1
     sudo systemctl start ssh  > /dev/null 2>&1
 }
```

### Comparing `youqu-2.6.0/youqu/src/utils/check_python_source.py` & `youqu-2.6.1/youqu/src/utils/check_python_source.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/docs_env.sh` & `youqu-2.6.1/youqu/src/utils/docs_env.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/env_dev.sh` & `youqu-2.6.1/youqu/src/utils/env_dev.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/env_vir.sh` & `youqu-2.6.1/youqu/src/utils/env_vir.sh`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,14 @@
 system_env
 
 echo 'pipenv run python "$@"' | sudo tee /usr/bin/youqu > /dev/null 2>&1
 echo "pipenv shell" | sudo tee /usr/bin/youqu-shell > /dev/null 2>&1
 echo "pipenv --rm" | sudo tee /usr/bin/youqu-rm > /dev/null 2>&1
 sudo chmod +x /usr/bin/youqu
 sudo chmod +x /usr/bin/youqu-shell
-sudo chmod +x /usr/bin/youqu-shell-rm
+sudo chmod +x /usr/bin/youqu-rm
 
 #cp --force ${ROOT_DIR}/src/utils/command_complete.sh ${HOME}/.config/
 #echo "source ${HOME}/.config/command_complete.sh" >> $HOME/.bashrc
 #source $HOME/.bashrc
 
 cd ${ROOT_DIR};youqu manage.py -h
```

### Comparing `youqu-2.6.0/youqu/src/utils/opencv_rpc_server.py` & `youqu-2.6.1/youqu/src/utils/opencv_rpc_server.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/pylint.sh` & `youqu-2.6.1/youqu/src/utils/pylint.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/sslclone.sh` & `youqu-2.6.1/youqu/src/utils/sslclone.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/sub_deb.py` & `youqu-2.6.1/youqu/src/utils/sub_deb.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/youqu/src/utils/vnc.sh` & `youqu-2.6.1/youqu/src/utils/vnc.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.0/pyproject.toml` & `youqu-2.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "youqu"
-version = "2.6.0"
+version = "2.6.1"
 authors = [
     { name = "mikigo", email = "huangmingqiang@uniontech.com" },
 ]
 
 description = "youqu"
 readme = "youqu/README.md"
 requires-python = ">=3.7"
```

### Comparing `youqu-2.6.0/youqu/README.md` & `youqu-2.6.1/youqu/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -15,140 +15,165 @@
 ![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431)
 
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
 [![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
-<a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
+**深度社区：<a href="https://github.com/linuxdeepin/youqu" target="_blank">linuxdeepin</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">deepin-community</a>**
 
-<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
+**欧拉社区：<a href="https://gitee.com/src-openeuler/youqu" target="_blank">src-openeuler</a>**
+
+**官方文档：<a href="https://youqu.uniontech.com" target="_blank">https://youqu.uniontech.com</a>**
+
+**欢迎加入 [YouQu官方兴趣小组](https://youqu.uniontech.com/SIG.html)**
 
 ---
 
-YouQu(有趣)是统信公司(Deepin/UOS)开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
+YouQu（有趣）是统信公司（Deepin/UOS）开源的一个 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
 
-## YouQu（有趣）能做什么
+## [YouQu（有趣）能做什么]()
 
 - [x] 💻 Linux 桌面应用 UI 自动化测试
 - [x] 🌏 Web UI 自动化测试
 - [x] 🚌 Linux DBus 接口自动化测试
 - [x] 🚀 命令行自动化测试
 - [x] 🕷️ HTTP 接口自动化测试
 - [ ] ⏲️ Linux 桌面应用性能自动化测试
 - [ ]    💥 Fuzzy Desktop 桌面模糊测试
 
-## 安装
+## [安装]()
 
 从 PyPI 安装:
 
 
 ```shell
 $ sudo pip3 install youqu
 ```
 
 <details> 
-<summary>不加 sudo ?</summary> 
-<pre>
-其实不加 sudo 也是可以的：<br>
-  pip3 install youqu<br>
-但某些情况下可能出现 youqu-startproject 命令无法使用，这是因为不加 sudo 时，安装包路径是在 $HOME/.local/lib/pythonX.X/site-packages，而此路径可能不在环境变量（PATH）中，您可以通过添加环境变量的方式使用 youqu-startproject 命令：<br>
-  export PATH=$PATH:$HOME/.local/lib/pythonX.X/site-packages<br>
-</pre>
+    <summary><b>不加 sudo ?</b></summary> 
+
+-----------------------
+
+不加 sudo 也可以：
+
+```shell
+pip3 install youqu
+```
+
+但可能出现 `youqu-startproject` 命令无法使用；
+
+这是因为不加 `sudo` 时，`youqu-startproject` 命令会生成在 `$HOME/.local/bin` 下，
+
+而此路径可能不在环境变量（`PATH`）中，因此您需要添加环境变量：
+
+```shell
+export PATH=$PATH:$HOME/.local/lib
+```
+
+-----------------------
+
 </details>
 
-## 创建项目
+
+## [创建项目]()
 
 您可以在任意目录下，使用 `youqu-startproject` 命令创建一个项目：
 
 ```shell
 $ youqu-startproject my_project
 ```
 
+注意：所有命令不要以 `root` 用户执行！
+
 如果 `youqu-startproject` 后面不加参数，默认的项目名称为：`youqu` ；
 
 ![](./docs/assets/install.gif)
 
-## 安装依赖
+## [安装依赖]()
 
 安装部署 YouQu 执行所需环境： 
 
 ```shell
 $ cd my_project
 $ bash env.sh
+# 使用的默认密码是 1；
+# 您可以使用 -p 选项传入密码：bash env.sh -p ${my_password}；
+# 也可以修改配置文件 setting/globalconfig.ini 里面的 PASSWORD 配置项；
 ```
 
-## 创建 APP 工程
+## [创建 APP 工程]()
 
 使用 `startapp` 命令自动创建 APP 工程：
 
 ```shell
 $ youqu manage.py startapp autotest_deepin_some
 ```
 
 自动创建的 APP 工程遵循完整的 PO 设计模式，让你可以专注于用例和方法的编写维护。
 
 在 `apps` 目录下会自动创建一个 APP 工程：`autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
 my_project
 ├── apps
-│   ├── autotest_deepin_some  # <-- APP 工程
+│   ├── autotest_deepin_some  # <-- APP工程
 ...     ├── ...
 ```
 
-在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。
+**在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。**
 
 `autotest_deepin_some` 是你的  APP 工程名称，在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
 
 `apps` 目录下可以存在任意多个 APP 工程。
 
-运行
+[运行]()
 -------
 
-### 1. 执行管理器
+### [1. 执行管理器]()
 
 在项目根目录下有一个 `manage.py` ，它是一个执行器入口，提供了本地执行、远程执行等的功能。
 
-### 2. 本地执行
+### [2. 本地执行]()
 
 
 ```shell
 $ youqu manage.py run
 ```
 
-#### 2.1. 命令行参数
+#### [2.1. 命令行参数]()
 
 在一些 CI 环境下使用命令行参数会更加方便：
 
 
 ```shell
 $ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
 ```
 
 更多用法可以使用 `-h` 或 `--help` 查看。
 
-#### 2.2. 配置文件
+#### [2.2. 配置文件]()
 
 通过配置文件配置参数
 
 在配置文件 [setting/globalconfig.ini](https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)  里面支持配置对执行的一些参数进行配置。
 
-### 3. 远程执行
+### [3. 远程执行]()
 
 远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同。
 
 使用 `remote` 命令：
 
 
 ```shell
 $ youqu manage.py remote
 ```
 
-## 贡献
+## [贡献]()
 
-[贡献文档](https://github.com/linuxdeepin/youqu/blob/master/CONTRIBUTING.md) 
+[贡献文档](https://youqu.uniontech.com/CONTRIBUTING.html) 
 
 
-## 开源许可证
+## [开源许可证]()
 
 YouQu 在 [GPL-2.0](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
```

#### html2text {}

```diff
@@ -5,60 +5,62 @@
 (https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
 (https://pypi.org/project/youqu/) ![Static Badge](https://img.shields.io/badge/
 UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431) [!
 [Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/
 youqu) [![Hits](https://hits.sh/github.com/linuxdeepin/
 youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/
-linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --- YouQu
-(æè¶£)æ¯ç»ä¿¡å¬å¸(Deepin/UOS)å¼æºçä¸ä¸ªç¨äº Linux
+linuxdeepin/youqu) --- **æ·±åº¦ç¤¾åºï¼_l_i_n_u_x_d_e_e_p_i_n | _d_e_e_p_i_n_-_c_o_m_m_u_n_i_t_y**
+**æ¬§æç¤¾åºï¼_s_r_c_-_o_p_e_n_e_u_l_e_r** **å®æ¹ææ¡£ï¼_h_t_t_p_s_:_/_/_y_o_u_q_u_._u_n_i_o_n_t_e_c_h_._c_o_m**
+**æ¬¢è¿å å¥ [YouQuå®æ¹å´è¶£å°ç»](https://youqu.uniontech.com/
+SIG.html)** --- YouQuï¼æè¶£ï¼æ¯ç»ä¿¡å¬å¸ï¼Deepin/UOSï¼å¼æºçä¸ä¸ª
+Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
 X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æãð¥ ##
-YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] ð» Linux æ¡é¢åºç¨ UI èªå¨åæµè¯
-- [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus æ¥å£èªå¨åæµè¯ -
-[x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP æ¥å£èªå¨åæµè¯ -
-[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ - [ ] ð¥ Fuzzy Desktop
-æ¡é¢æ¨¡ç³æµè¯ ## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install
-youqu ``` ä¸å  sudo ?
-å¶å®ä¸å  sudo ä¹æ¯å¯ä»¥çï¼
-
-  pip3 install youqu
-
-ä½æäºæåµä¸å¯è½åºç° youqu-startproject
-å½ä»¤æ æ³ä½¿ç¨ï¼è¿æ¯å ä¸ºä¸å  sudo æ¶ï¼å®è£åè·¯å¾æ¯å¨
-$HOME/.local/lib/pythonX.X/site-
-packagesï¼èæ­¤è·¯å¾å¯è½ä¸å¨ç¯å¢åéï¼PATHï¼ä¸­ï¼æ¨å¯ä»¥éè¿æ·»å ç¯å¢åéçæ¹å¼ä½¿ç¨
-youqu-startproject å½ä»¤ï¼
-
-  export PATH=$PATH:$HOME/.local/lib/pythonX.X/site-packages
-## åå»ºé¡¹ç® æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
-å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ``` å¦æ
-`youqu-startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu`
-ï¼ ![](./docs/assets/install.gif) ## å®è£ä¾èµ å®è£é¨ç½² YouQu
-æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
-å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
-manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
-å·¥ç¨éµå¾ªå®æ´ç PO
+[YouQuï¼æè¶£ï¼è½åä»ä¹]() - [x] ð» Linux æ¡é¢åºç¨ UI
+èªå¨åæµè¯ - [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus
+æ¥å£èªå¨åæµè¯ - [x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP
+æ¥å£èªå¨åæµè¯ - [ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ -
+[ ] ð¥ Fuzzy Desktop æ¡é¢æ¨¡ç³æµè¯ ## [å®è£]() ä» PyPI å®è£:
+```shell $ sudo pip3 install youqu ``` ?ä?¸??å??  ssuuddoo ?? ----------------------
+- ä¸å  sudo ä¹å¯ä»¥ï¼ ```shell pip3 install youqu ``` ä½å¯è½åºç°
+`youqu-startproject` å½ä»¤æ æ³ä½¿ç¨ï¼ è¿æ¯å ä¸ºä¸å  `sudo`
+æ¶ï¼`youqu-startproject` å½ä»¤ä¼çæå¨ `$HOME/.local/bin` ä¸ï¼
+èæ­¤è·¯å¾å¯è½ä¸å¨ç¯å¢åéï¼`PATH`ï¼ä¸­ï¼å æ­¤æ¨éè¦æ·»å ç¯å¢åéï¼
+```shell export PATH=$PATH:$HOME/.local/lib ``` ----------------------- ##
+[åå»ºé¡¹ç®]() æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
+å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ```
+æ³¨æï¼ææå½ä»¤ä¸è¦ä»¥ `root` ç¨æ·æ§è¡ï¼ å¦æ `youqu-
+startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu` ï¼ ![]
+(./docs/assets/install.gif) ## [å®è£ä¾èµ]() å®è£é¨ç½² YouQu
+æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh #
+ä½¿ç¨çé»è®¤å¯ç æ¯ 1ï¼ # æ¨å¯ä»¥ä½¿ç¨ -p éé¡¹ä¼ å¥å¯ç ï¼bash
+env.sh -p ${my_password}ï¼ # ä¹å¯ä»¥ä¿®æ¹éç½®æä»¶ setting/
+globalconfig.ini éé¢ç PASSWORD éç½®é¡¹ï¼ ``` ## [åå»º APP å·¥ç¨]()
+ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu manage.py
+startapp autotest_deepin_some ``` èªå¨åå»ºç APP å·¥ç¨éµå¾ªå®æ´ç PO
 è®¾è®¡æ¨¡å¼ï¼è®©ä½ å¯ä»¥ä¸æ³¨äºç¨ä¾åæ¹æ³çç¼åç»´æ¤ã å¨
 `apps` ç®å½ä¸ä¼èªå¨åå»ºä¸ä¸ª APP
 å·¥ç¨ï¼`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
-```shell my_project âââ apps â âââ autotest_deepin_some # <-- APP
-å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
-ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã
+```shell my_project âââ apps â âââ autotest_deepin_some # <-
+- APPå·¥ç¨ ... Â Â  âââ ... ``` **å¨ä½ çè¿ç¨ Git
+ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã**
 `autotest_deepin_some` æ¯ä½ ç APP
 å·¥ç¨åç§°ï¼å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
 é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã `apps`
-ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã è¿è¡ ------- ### 1.
-æ§è¡ç®¡çå¨ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
+ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã [è¿è¡]() ------- ### [1.
+æ§è¡ç®¡çå¨]() å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
-### 2. æ¬å°æ§è¡ ```shell $ youqu manage.py run ``` #### 2.1.
-å½ä»¤è¡åæ° å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼
-```shell $ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
-``` æ´å¤ç¨æ³å¯ä»¥ä½¿ç¨ `-h` æ `--help` æ¥çã #### 2.2. éç½®æä»¶
+### [2. æ¬å°æ§è¡]() ```shell $ youqu manage.py run ``` #### [2.1.
+å½ä»¤è¡åæ°]() å¨ä¸äº CI
+ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼ ```shell $ youqu manage.py run
+-a apps/autotest_deepin_some -k "xxx" -t "yyy" ``` æ´å¤ç¨æ³å¯ä»¥ä½¿ç¨ `-
+h` æ `--help` æ¥çã #### [2.2. éç½®æä»¶]()
 éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ [setting/globalconfig.ini]
 (https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)
-éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ã ### 3. è¿ç¨æ§è¡
+éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ã ### [3. è¿ç¨æ§è¡]
+()
 è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åã
-ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ## è´¡ç®
-[è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
-CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ YouQu å¨ [GPL-2.0](https://github.com/
-linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã
+ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ## [è´¡ç®]()
+[è´¡ç®ææ¡£](https://youqu.uniontech.com/CONTRIBUTING.html) ##
+[å¼æºè®¸å¯è¯]() YouQu å¨ [GPL-2.0](https://github.com/linuxdeepin/youqu/
+blob/master/LICENSE) ä¸åå¸ã
```

### Comparing `youqu-2.6.0/PKG-INFO` & `youqu-2.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youqu
-Version: 2.6.0
+Version: 2.6.1
 Summary: youqu
 Project-URL: Source, https://github.com/linuxdeepin/youqu
 Project-URL: Documentation, https://linuxdeepin.github.io/youqu
 Author-email: mikigo <huangmingqiang@uniontech.com>
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -28,140 +28,165 @@
 ![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431)
 
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
 [![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
-<a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
+**深度社区：<a href="https://github.com/linuxdeepin/youqu" target="_blank">linuxdeepin</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">deepin-community</a>**
 
-<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
+**欧拉社区：<a href="https://gitee.com/src-openeuler/youqu" target="_blank">src-openeuler</a>**
+
+**官方文档：<a href="https://youqu.uniontech.com" target="_blank">https://youqu.uniontech.com</a>**
+
+**欢迎加入 [YouQu官方兴趣小组](https://youqu.uniontech.com/SIG.html)**
 
 ---
 
-YouQu(有趣)是统信公司(Deepin/UOS)开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
+YouQu（有趣）是统信公司（Deepin/UOS）开源的一个 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
 
-## YouQu（有趣）能做什么
+## [YouQu（有趣）能做什么]()
 
 - [x] 💻 Linux 桌面应用 UI 自动化测试
 - [x] 🌏 Web UI 自动化测试
 - [x] 🚌 Linux DBus 接口自动化测试
 - [x] 🚀 命令行自动化测试
 - [x] 🕷️ HTTP 接口自动化测试
 - [ ] ⏲️ Linux 桌面应用性能自动化测试
 - [ ]    💥 Fuzzy Desktop 桌面模糊测试
 
-## 安装
+## [安装]()
 
 从 PyPI 安装:
 
 
 ```shell
 $ sudo pip3 install youqu
 ```
 
 <details> 
-<summary>不加 sudo ?</summary> 
-<pre>
-其实不加 sudo 也是可以的：<br>
-  pip3 install youqu<br>
-但某些情况下可能出现 youqu-startproject 命令无法使用，这是因为不加 sudo 时，安装包路径是在 $HOME/.local/lib/pythonX.X/site-packages，而此路径可能不在环境变量（PATH）中，您可以通过添加环境变量的方式使用 youqu-startproject 命令：<br>
-  export PATH=$PATH:$HOME/.local/lib/pythonX.X/site-packages<br>
-</pre>
+    <summary><b>不加 sudo ?</b></summary> 
+
+-----------------------
+
+不加 sudo 也可以：
+
+```shell
+pip3 install youqu
+```
+
+但可能出现 `youqu-startproject` 命令无法使用；
+
+这是因为不加 `sudo` 时，`youqu-startproject` 命令会生成在 `$HOME/.local/bin` 下，
+
+而此路径可能不在环境变量（`PATH`）中，因此您需要添加环境变量：
+
+```shell
+export PATH=$PATH:$HOME/.local/lib
+```
+
+-----------------------
+
 </details>
 
-## 创建项目
+
+## [创建项目]()
 
 您可以在任意目录下，使用 `youqu-startproject` 命令创建一个项目：
 
 ```shell
 $ youqu-startproject my_project
 ```
 
+注意：所有命令不要以 `root` 用户执行！
+
 如果 `youqu-startproject` 后面不加参数，默认的项目名称为：`youqu` ；
 
 ![](./docs/assets/install.gif)
 
-## 安装依赖
+## [安装依赖]()
 
 安装部署 YouQu 执行所需环境： 
 
 ```shell
 $ cd my_project
 $ bash env.sh
+# 使用的默认密码是 1；
+# 您可以使用 -p 选项传入密码：bash env.sh -p ${my_password}；
+# 也可以修改配置文件 setting/globalconfig.ini 里面的 PASSWORD 配置项；
 ```
 
-## 创建 APP 工程
+## [创建 APP 工程]()
 
 使用 `startapp` 命令自动创建 APP 工程：
 
 ```shell
 $ youqu manage.py startapp autotest_deepin_some
 ```
 
 自动创建的 APP 工程遵循完整的 PO 设计模式，让你可以专注于用例和方法的编写维护。
 
 在 `apps` 目录下会自动创建一个 APP 工程：`autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
 my_project
 ├── apps
-│   ├── autotest_deepin_some  # <-- APP 工程
+│   ├── autotest_deepin_some  # <-- APP工程
 ...     ├── ...
 ```
 
-在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。
+**在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。**
 
 `autotest_deepin_some` 是你的  APP 工程名称，在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
 
 `apps` 目录下可以存在任意多个 APP 工程。
 
-运行
+[运行]()
 -------
 
-### 1. 执行管理器
+### [1. 执行管理器]()
 
 在项目根目录下有一个 `manage.py` ，它是一个执行器入口，提供了本地执行、远程执行等的功能。
 
-### 2. 本地执行
+### [2. 本地执行]()
 
 
 ```shell
 $ youqu manage.py run
 ```
 
-#### 2.1. 命令行参数
+#### [2.1. 命令行参数]()
 
 在一些 CI 环境下使用命令行参数会更加方便：
 
 
 ```shell
 $ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
 ```
 
 更多用法可以使用 `-h` 或 `--help` 查看。
 
-#### 2.2. 配置文件
+#### [2.2. 配置文件]()
 
 通过配置文件配置参数
 
 在配置文件 [setting/globalconfig.ini](https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)  里面支持配置对执行的一些参数进行配置。
 
-### 3. 远程执行
+### [3. 远程执行]()
 
 远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同。
 
 使用 `remote` 命令：
 
 
 ```shell
 $ youqu manage.py remote
 ```
 
-## 贡献
+## [贡献]()
 
-[贡献文档](https://github.com/linuxdeepin/youqu/blob/master/CONTRIBUTING.md) 
+[贡献文档](https://youqu.uniontech.com/CONTRIBUTING.html) 
 
 
-## 开源许可证
+## [开源许可证]()
 
 YouQu 在 [GPL-2.0](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: youqu Version: 2.6.0 Summary: youqu Project-URL:
+Metadata-Version: 2.1 Name: youqu Version: 2.6.1 Summary: youqu Project-URL:
 Source, https://github.com/linuxdeepin/youqu Project-URL: Documentation, https:
 //linuxdeepin.github.io/youqu Author-email: mikigo
 uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
@@ -12,60 +12,62 @@
 (https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
 (https://pypi.org/project/youqu/) ![Static Badge](https://img.shields.io/badge/
 UOS%2FDeepin/openEuler-Platform?style=flat&label=OS&color=%23F79431) [!
 [Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/
 youqu) [![Hits](https://hits.sh/github.com/linuxdeepin/
 youqu.svg?style=flat&label=visitors&color=blue)](https://github.com/
-linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --- YouQu
-(æè¶£)æ¯ç»ä¿¡å¬å¸(Deepin/UOS)å¼æºçä¸ä¸ªç¨äº Linux
+linuxdeepin/youqu) --- **æ·±åº¦ç¤¾åºï¼_l_i_n_u_x_d_e_e_p_i_n | _d_e_e_p_i_n_-_c_o_m_m_u_n_i_t_y**
+**æ¬§æç¤¾åºï¼_s_r_c_-_o_p_e_n_e_u_l_e_r** **å®æ¹ææ¡£ï¼_h_t_t_p_s_:_/_/_y_o_u_q_u_._u_n_i_o_n_t_e_c_h_._c_o_m**
+**æ¬¢è¿å å¥ [YouQuå®æ¹å´è¶£å°ç»](https://youqu.uniontech.com/
+SIG.html)** --- YouQuï¼æè¶£ï¼æ¯ç»ä¿¡å¬å¸ï¼Deepin/UOSï¼å¼æºçä¸ä¸ª
+Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
 X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æãð¥ ##
-YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] ð» Linux æ¡é¢åºç¨ UI èªå¨åæµè¯
-- [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus æ¥å£èªå¨åæµè¯ -
-[x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP æ¥å£èªå¨åæµè¯ -
-[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ - [ ] ð¥ Fuzzy Desktop
-æ¡é¢æ¨¡ç³æµè¯ ## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install
-youqu ``` ä¸å  sudo ?
-å¶å®ä¸å  sudo ä¹æ¯å¯ä»¥çï¼
-
-  pip3 install youqu
-
-ä½æäºæåµä¸å¯è½åºç° youqu-startproject
-å½ä»¤æ æ³ä½¿ç¨ï¼è¿æ¯å ä¸ºä¸å  sudo æ¶ï¼å®è£åè·¯å¾æ¯å¨
-$HOME/.local/lib/pythonX.X/site-
-packagesï¼èæ­¤è·¯å¾å¯è½ä¸å¨ç¯å¢åéï¼PATHï¼ä¸­ï¼æ¨å¯ä»¥éè¿æ·»å ç¯å¢åéçæ¹å¼ä½¿ç¨
-youqu-startproject å½ä»¤ï¼
-
-  export PATH=$PATH:$HOME/.local/lib/pythonX.X/site-packages
-## åå»ºé¡¹ç® æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
-å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ``` å¦æ
-`youqu-startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu`
-ï¼ ![](./docs/assets/install.gif) ## å®è£ä¾èµ å®è£é¨ç½² YouQu
-æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
-å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
-manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
-å·¥ç¨éµå¾ªå®æ´ç PO
+[YouQuï¼æè¶£ï¼è½åä»ä¹]() - [x] ð» Linux æ¡é¢åºç¨ UI
+èªå¨åæµè¯ - [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus
+æ¥å£èªå¨åæµè¯ - [x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP
+æ¥å£èªå¨åæµè¯ - [ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ -
+[ ] ð¥ Fuzzy Desktop æ¡é¢æ¨¡ç³æµè¯ ## [å®è£]() ä» PyPI å®è£:
+```shell $ sudo pip3 install youqu ``` ?ä?¸??å??  ssuuddoo ?? ----------------------
+- ä¸å  sudo ä¹å¯ä»¥ï¼ ```shell pip3 install youqu ``` ä½å¯è½åºç°
+`youqu-startproject` å½ä»¤æ æ³ä½¿ç¨ï¼ è¿æ¯å ä¸ºä¸å  `sudo`
+æ¶ï¼`youqu-startproject` å½ä»¤ä¼çæå¨ `$HOME/.local/bin` ä¸ï¼
+èæ­¤è·¯å¾å¯è½ä¸å¨ç¯å¢åéï¼`PATH`ï¼ä¸­ï¼å æ­¤æ¨éè¦æ·»å ç¯å¢åéï¼
+```shell export PATH=$PATH:$HOME/.local/lib ``` ----------------------- ##
+[åå»ºé¡¹ç®]() æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
+å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ```
+æ³¨æï¼ææå½ä»¤ä¸è¦ä»¥ `root` ç¨æ·æ§è¡ï¼ å¦æ `youqu-
+startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu` ï¼ ![]
+(./docs/assets/install.gif) ## [å®è£ä¾èµ]() å®è£é¨ç½² YouQu
+æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh #
+ä½¿ç¨çé»è®¤å¯ç æ¯ 1ï¼ # æ¨å¯ä»¥ä½¿ç¨ -p éé¡¹ä¼ å¥å¯ç ï¼bash
+env.sh -p ${my_password}ï¼ # ä¹å¯ä»¥ä¿®æ¹éç½®æä»¶ setting/
+globalconfig.ini éé¢ç PASSWORD éç½®é¡¹ï¼ ``` ## [åå»º APP å·¥ç¨]()
+ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu manage.py
+startapp autotest_deepin_some ``` èªå¨åå»ºç APP å·¥ç¨éµå¾ªå®æ´ç PO
 è®¾è®¡æ¨¡å¼ï¼è®©ä½ å¯ä»¥ä¸æ³¨äºç¨ä¾åæ¹æ³çç¼åç»´æ¤ã å¨
 `apps` ç®å½ä¸ä¼èªå¨åå»ºä¸ä¸ª APP
 å·¥ç¨ï¼`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
-```shell my_project âââ apps â âââ autotest_deepin_some # <-- APP
-å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
-ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã
+```shell my_project âââ apps â âââ autotest_deepin_some # <-
+- APPå·¥ç¨ ... Â Â  âââ ... ``` **å¨ä½ çè¿ç¨ Git
+ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã**
 `autotest_deepin_some` æ¯ä½ ç APP
 å·¥ç¨åç§°ï¼å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
 é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã `apps`
-ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã è¿è¡ ------- ### 1.
-æ§è¡ç®¡çå¨ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
+ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã [è¿è¡]() ------- ### [1.
+æ§è¡ç®¡çå¨]() å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
-### 2. æ¬å°æ§è¡ ```shell $ youqu manage.py run ``` #### 2.1.
-å½ä»¤è¡åæ° å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼
-```shell $ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
-``` æ´å¤ç¨æ³å¯ä»¥ä½¿ç¨ `-h` æ `--help` æ¥çã #### 2.2. éç½®æä»¶
+### [2. æ¬å°æ§è¡]() ```shell $ youqu manage.py run ``` #### [2.1.
+å½ä»¤è¡åæ°]() å¨ä¸äº CI
+ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼ ```shell $ youqu manage.py run
+-a apps/autotest_deepin_some -k "xxx" -t "yyy" ``` æ´å¤ç¨æ³å¯ä»¥ä½¿ç¨ `-
+h` æ `--help` æ¥çã #### [2.2. éç½®æä»¶]()
 éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ [setting/globalconfig.ini]
 (https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)
-éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ã ### 3. è¿ç¨æ§è¡
+éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ã ### [3. è¿ç¨æ§è¡]
+()
 è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åã
-ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ## è´¡ç®
-[è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
-CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ YouQu å¨ [GPL-2.0](https://github.com/
-linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã
+ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ## [è´¡ç®]()
+[è´¡ç®ææ¡£](https://youqu.uniontech.com/CONTRIBUTING.html) ##
+[å¼æºè®¸å¯è¯]() YouQu å¨ [GPL-2.0](https://github.com/linuxdeepin/youqu/
+blob/master/LICENSE) ä¸åå¸ã
```

