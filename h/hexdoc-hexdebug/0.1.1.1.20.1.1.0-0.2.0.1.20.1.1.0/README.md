# Comparing `tmp/hexdoc_hexdebug-0.1.1.1.20.1.1.0.tar.gz` & `tmp/hexdoc_hexdebug-0.2.0.1.20.1.1.0.tar.gz`

## Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0.tar` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0.tar`

### file list

```diff
@@ -1,64 +1,70 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/gradle.properties
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/__version__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/empty.json
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/full.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/empty.json
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/full.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/empty.json
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/full.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/empty.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/full.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/empty.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/full.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/empty.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/full.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/empty.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/full.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/empty.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/full.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/empty.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/full.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/empty.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/full.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/empty.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/full.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/empty.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/full.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/debug_state/debugging.png
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/debugger.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_templates/__init__.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/LICENSE
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.1.1.1.20.1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/gradle.properties
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/__version__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/empty.json
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/full.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/empty.json
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/full.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/empty.json
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/full.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/empty.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/full.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/empty.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/full.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/empty.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/full.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/empty.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/full.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/empty.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/full.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/empty.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/full.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/empty.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/full.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/empty.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/full.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/empty.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/full.json
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator/default.json
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator/modified.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/evaluator.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/debug_state/debugging.png
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/evaluator/eval_state/modified.png
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/debugger.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/evaluator.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_templates/__init__.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/LICENSE
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.0.1.20.1.1.0/PKG-INFO
```

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6526118259803921%*

 * *Differences: {"'asset_url'": "'https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7'",*

 * * "'book_url'": "'https://hexdebug.hexxy.media/v/0.2.0+1.20.1/1.0/en_us'",*

 * * "'textures'": "{'PNGTexture': {'hexdebug:textures/item/debugger.png': {'url': "*

 * *               "'https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png'}, "*

 * *               "'hexdebug:textures/item/debugger/ […]*

```diff
@@ -1,78 +1,86 @@
 {
-    "asset_url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc",
-    "book_url": "https://hexdebug.hexxy.media/v/0.1.1+1.20.1/1.0/en_us",
+    "asset_url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7",
+    "book_url": "https://hexdebug.hexxy.media/v/0.2.0+1.20.1/1.0/en_us",
     "textures": {
         "PNGTexture": {
             "hexdebug:textures/item/debugger.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
             },
             "hexdebug:textures/item/debugger/debug_state/debugging.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/debug_state/debugging.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/debug_state/debugging.png"
             },
             "hexdebug:textures/item/debugger/has_hex/full.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/has_hex/full.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/has_hex/full.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/continue.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/in.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/out.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/over.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/restart.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/stop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/continue.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/in.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/out.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/over.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/restart.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/stop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png"
+            },
+            "hexdebug:textures/item/evaluator.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png"
+            },
+            "hexdebug:textures/item/evaluator/eval_state/modified.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/evaluator/eval_state/modified.png"
             }
         },
         "SingleItemTexture": {
             "hexdebug:debugger": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/d993c847f25433fc9eaf7ededf0687209b68f4cc/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
                 }
             },
             "hexdebug:debugger/debugging/continue/empty": {
                 "inner": {
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
@@ -210,11 +218,29 @@
                 }
             },
             "hexdebug:debugger/not_debugging/stop/full": {
                 "inner": {
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
+            },
+            "hexdebug:evaluator": {
+                "inner": {
+                    "pixelated": true,
+                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/6bf7276803cba5c483ffc825b4009ca5ccce62e7/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png"
+                }
+            },
+            "hexdebug:evaluator/default": {
+                "inner": {
+                    "pixelated": true,
+                    "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
+                }
+            },
+            "hexdebug:evaluator/modified": {
+                "inner": {
+                    "pixelated": true,
+                    "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
+                }
             }
         }
     }
 }
```

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6944444444444444%*

 * *Differences: {"'hexdebug.category.items.entry.debugging.page.debugger'": "'部分文献中有些不太明确的描述，称古代人会使用一件奇怪的物品协助他们发现复杂$(hex)咒术/$中的问题。我应已成功复刻出了它，定名为$(item)调试杖/$。$(br2)它的工作方式与$(l:items/hexcasting)$(item)造物/$类似。不过，它还能从副手中的物品（比如$(l:items/focus)$(item)核心/$）里直接施放$(hex)咒术/$。$(br2)有些可惜的是，$(item)调试杖/$自身没有太大用处；它似乎需要某种$(l:https://marketplace.visualstudio.com/items?itemName=object-Object.hex-casting)外部工具/$才能正常运作。'",*

 * * "'hexdebug.category.items.entry.debugging.page.evaluator'": "'我又新制造了一种法杖——$(l:items/debugging#evaluator)$(item)运行杖/$，用以补充$ […]*

```diff
@@ -1,29 +1,37 @@
 {
     "hexcasting.action.hexdebug:breakpoint/after": "\u5728\u540e\u65b9\u6dfb\u52a0\u65ad\u70b9",
     "hexcasting.action.hexdebug:breakpoint/before": "\u5728\u524d\u65b9\u6dfb\u52a0\u65ad\u70b9",
     "hexcasting.action.hexdebug:const/debugging": "\u8c03\u8bd5\u6756\u4e4b\u7cbe\u601d",
     "hexcasting.action.hexdebug:craft/debugger": "\u5236\u4f5c\u8c03\u8bd5\u6756",
     "hexdebug.category.items.entry.debugging": "\u8c03\u8bd5\u7269\u54c1",
-    "hexdebug.category.items.entry.debugging.page.1": "\u90e8\u5206\u6587\u732e\u4e2d\u6709\u4e9b\u4e0d\u592a\u660e\u786e\u7684\u63cf\u8ff0\uff0c\u79f0\u53e4\u4ee3\u4eba\u4f1a\u4f7f\u7528\u4e00\u4ef6\u5947\u602a\u7684\u7269\u54c1\u534f\u52a9\u4ed6\u4eec\u53d1\u73b0\u590d\u6742$(hex)\u5492\u672f/$\u4e2d\u7684\u95ee\u9898\u3002\u6211\u5e94\u5df2\u6210\u529f\u590d\u523b\u51fa\u4e86\u5b83\uff0c\u5b9a\u540d\u4e3a$(item)\u8c03\u8bd5\u6756/$\u3002$(br2)\u5b83\u7684\u5de5\u4f5c\u65b9\u5f0f\u4e0e$(l:items/hexcasting)$(item)\u9020\u7269/$\u7c7b\u4f3c\u3002\u4e0d\u8fc7\uff0c\u5b83\u8fd8\u80fd\u4ece\u526f\u624b\u4e2d\u7684\u7269\u54c1\uff08\u6bd4\u5982$(l:items/focus)$(item)\u6838\u5fc3/$\uff09\u91cc\u76f4\u63a5\u65bd\u653e$(hex)\u5492\u672f/$\u3002$(br2)$(item)\u8c03\u8bd5\u6756/$\u81ea\u8eab\u6ca1\u6709\u592a\u5927\u7528\u5904\uff0c\u6709\u4e9b\u53ef\u60dc\uff1b\u5b83\u4f3c\u4e4e\u9700\u8981\u67d0\u79cd$(l:https://marketplace.visualstudio.com/items?itemName=object-Object.hex-casting)\u5916\u90e8\u5de5\u5177/$\u624d\u80fd\u6b63\u5e38\u8fd0\u4f5c\u3002",
+    "hexdebug.category.items.entry.debugging.page.debugger": "\u90e8\u5206\u6587\u732e\u4e2d\u6709\u4e9b\u4e0d\u592a\u660e\u786e\u7684\u63cf\u8ff0\uff0c\u79f0\u53e4\u4ee3\u4eba\u4f1a\u4f7f\u7528\u4e00\u4ef6\u5947\u602a\u7684\u7269\u54c1\u534f\u52a9\u4ed6\u4eec\u53d1\u73b0\u590d\u6742$(hex)\u5492\u672f/$\u4e2d\u7684\u95ee\u9898\u3002\u6211\u5e94\u5df2\u6210\u529f\u590d\u523b\u51fa\u4e86\u5b83\uff0c\u5b9a\u540d\u4e3a$(item)\u8c03\u8bd5\u6756/$\u3002$(br2)\u5b83\u7684\u5de5\u4f5c\u65b9\u5f0f\u4e0e$(l:items/hexcasting)$(item)\u9020\u7269/$\u7c7b\u4f3c\u3002\u4e0d\u8fc7\uff0c\u5b83\u8fd8\u80fd\u4ece\u526f\u624b\u4e2d\u7684\u7269\u54c1\uff08\u6bd4\u5982$(l:items/focus)$(item)\u6838\u5fc3/$\uff09\u91cc\u76f4\u63a5\u65bd\u653e$(hex)\u5492\u672f/$\u3002$(br2)\u6709\u4e9b\u53ef\u60dc\u7684\u662f\uff0c$(item)\u8c03\u8bd5\u6756/$\u81ea\u8eab\u6ca1\u6709\u592a\u5927\u7528\u5904\uff1b\u5b83\u4f3c\u4e4e\u9700\u8981\u67d0\u79cd$(l:https://marketplace.visualstudio.com/items?itemName=object-Object.hex-casting)\u5916\u90e8\u5de5\u5177/$\u624d\u80fd\u6b63\u5e38\u8fd0\u4f5c\u3002",
+    "hexdebug.category.items.entry.debugging.page.evaluator": "\u6211\u53c8\u65b0\u5236\u9020\u4e86\u4e00\u79cd\u6cd5\u6756\u2014\u2014$(l:items/debugging#evaluator)$(item)\u8fd0\u884c\u6756/$\uff0c\u7528\u4ee5\u8865\u5145$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u7684\u529f\u80fd\u3002$(br2)\u8c03\u8bd5$(hex)\u5492\u672f/$\u65f6\uff0c\u6b64\u6cd5\u6756\u7ed8\u5236\u7684\u56fe\u6848\u4f1a\u8fd0\u884c\u4e8e$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u5f53\u524d\u7684\u6808\u548c$(l:patterns/readwrite#hexcasting:local)$(thing)\u6e21\u9e26\u4e4b\u601d/$\u3002$(br2)\u6e05\u7a7a\u5492\u672f\u7f51\u683c\u540e\uff0c$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u4f3c\u4e4e\u4f1a\u56de\u5230$(l:items/debugging#evaluator)$(item)\u8fd0\u884c\u6756/$\u7ed8\u5236\u9996\u4e2a\u56fe\u6848\u524d\u7684\u72b6\u6001\u3002\u5f53\u7136\uff0c\u8fd9\u79cd\u64cd\u4f5c\u65e0\u6cd5\u64a4\u56de\u5df2\u9020\u6210\u5b9e\u9645\u5f71\u54cd\u7684\u6cd5\u672f\u3002",
     "hexdebug.category.items.entry.debugging.page.thwack": "$(italic)\u54d0\u5f53\uff01/$",
+    "hexdebug.category.items.entry.debugging.page.thwonk": "$(italic)\u54d0\u5577\uff01/$",
     "hexdebug.category.patterns.entry.debugging": "\u8c03\u8bd5",
     "hexdebug.category.patterns.entry.debugging.page.breakpoint/after": "\u5728\u8fd0\u884c\u6b64\u56fe\u6848\u540e\uff0c\u4e5f\u5373\u5728\u8fd0\u884c\u4e0b\u4e00\u56fe\u6848\u4e4b\u524d\uff0c\u6682\u505c$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u3002",
     "hexdebug.category.patterns.entry.debugging.page.breakpoint/before": "\u5728\u8fd0\u884c\u6b64\u56fe\u6848\u524d\uff0c\u6682\u505c$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u3002",
     "hexdebug.category.patterns.entry.debugging.page.const/debugging": "\u82e5\u6808\u7531$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u6267\u884c\uff0c\u5219\u8fd4\u56de $(thing)True/$\uff1b\u5426\u5219\u8fd4\u56de $(thing)False/$\u3002",
     "hexdebug.category.patterns.entry.debugging.page.craft/debugger": "\u5236\u4f5c\u4e00\u652f\u80fd\u65bd\u653e$(hex)\u5492\u672f/$\u7684$(l:items/debugging#debugger)$(item)\u8c03\u8bd5\u6756/$\u3002\u8fd9\u4e2a\u56fe\u6848\u548c\u6211\u4e4b\u524d\u7528\u8fc7\u7684$(l:patterns/spells/hexcasting)\u67d0\u4e9b\u56fe\u6848/$\u6709\u4e9b\u76f8\u4f3c\u3002$(br2)\u6d88\u8017\u5927\u7ea6 10 \u4e2a$(l:items/amethyst)$(item)\u5145\u80fd\u7d2b\u6c34\u6676/$\u3002",
     "hexdebug.tooltip.debugger.step_mode": "\u6a21\u5f0f\uff1a%s",
     "hexdebug.tooltip.debugger.step_mode.continue": "\u7ee7\u7eed",
     "hexdebug.tooltip.debugger.step_mode.in": "\u5355\u6b65\u8c03\u8bd5",
     "hexdebug.tooltip.debugger.step_mode.out": "\u5355\u6b65\u8df3\u51fa",
     "hexdebug.tooltip.debugger.step_mode.over": "\u9010\u8fc7\u7a0b",
     "hexdebug.tooltip.debugger.step_mode.restart": "\u91cd\u542f",
     "hexdebug.tooltip.debugger.step_mode.stop": "\u505c\u6b62",
     "item.hexdebug.debugger": "\u8c03\u8bd5\u6756",
-    "itemGroup.hexdebug": "\u5492\u672f\u8c03\u8bd5",
+    "item.hexdebug.evaluator": "\u8fd0\u884c\u6756",
+    "itemGroup.hexdebug": "\u5492\u6cd5\u8c03\u8bd5",
     "text.autoconfig.hexdebug.category.client": "\u5ba2\u6237\u7aef",
     "text.autoconfig.hexdebug.option.client.debugPort": "\u8c03\u8bd5\u7aef\u53e3",
-    "text.autoconfig.hexdebug.title": "\u5492\u672f\u8c03\u8bd5\u914d\u7f6e",
+    "text.autoconfig.hexdebug.option.client.debugPort.@Tooltip": "\u5f00\u653e\u4ee5\u8fde\u63a5\u81f3\u8c03\u8bd5\u5ba2\u6237\u7aef\uff08\u5982VSCode\uff09\u7684\u7aef\u53e3\u53f7\uff081024-65535\uff09\u3002",
+    "text.autoconfig.hexdebug.option.client.openDebugPort": "\u5f00\u653e\u8c03\u8bd5\u7aef\u53e3",
+    "text.autoconfig.hexdebug.option.client.openDebugPort.@Tooltip": "\u662f\u5426\u5f00\u653e\u7aef\u53e3\u3002\u82e5\u8bbe\u4e3afalse\uff0c\u8c03\u8bd5\u6756\u4f1a\u5931\u53bb\u4f5c\u7528\u3002",
+    "text.autoconfig.hexdebug.option.client.smartDebuggerSneakScroll": "\u8c03\u8bd5\u6756\u667a\u80fd\u6f5c\u884c\u6eda\u8f6e",
+    "text.autoconfig.hexdebug.option.client.smartDebuggerSneakScroll.@Tooltip": "\u82e5\u5f53\u524d\u4e3b\u624b\u6301\u6709\u8c03\u8bd5\u6756\uff0c\u4e14\u672a\u5728\u8c03\u8bd5\u5492\u672f\uff0c\u5219\u4f18\u5148\u5904\u7406\u526f\u624b\u4e2d\u6cd5\u672f\u4e66\u4e00\u7c7b\u7269\u54c1\u7684\u201c\u6f5c\u884c\u6eda\u52a8\u6eda\u8f6e\u201d\u64cd\u4f5c\u3002",
+    "text.autoconfig.hexdebug.title": "\u5492\u6cd5\u8c03\u8bd5\u914d\u7f6e",
     "text.hexdebug.connected": "\u8c03\u8bd5\u5ba2\u6237\u7aef\u5df2\u8fde\u63a5\uff01",
     "text.hexdebug.no_client": "\u8c03\u8bd5\u5ba2\u6237\u7aef\u672a\u8fde\u63a5\u3002",
     "text.hexdebug.thwack": "\u54d0\u5f53\uff01"
 }
```

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'parent'": "'minecraft:item/handheld_rod'"}*

```diff
@@ -195,12 +195,12 @@
         {
             "model": "hexdebug:item/debugger",
             "predicate": {
                 "hexdebug:hide_icons": 1.0
             }
         }
     ],
-    "parent": "minecraft:item/generated",
+    "parent": "minecraft:item/handheld_rod",
     "textures": {
         "layer0": "hexdebug:item/debugger"
     }
 }
```

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/.gitignore` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/LICENSE` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/pyproject.toml` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/doc/README.md` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.1.1.1.20.1.1.0/PKG-INFO` & `hexdoc_hexdebug-0.2.0.1.20.1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hexdoc-hexdebug
-Version: 0.1.1.1.20.1.1.0
+Version: 0.2.0.1.20.1.1.0
 Summary: Python web book docgen and hexdoc plugin for HexDebug.
 Project-URL: Homepage, https://hexdebug.hexxy.media
 Project-URL: Source, https://github.com/object-Object/HexDebug
 Author: object-Object
 License-File: LICENSE
 Keywords: hexdoc
 Requires-Python: >=3.11
```

