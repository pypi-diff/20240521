# Comparing `tmp/aurum_hikari-0.1.5.tar.gz` & `tmp/aurum_hikari-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.5.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.5.1.tar", max compression
```

## Comparing `aurum_hikari-0.1.5.tar` & `aurum_hikari-0.1.5.1.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0     1080 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/LICENSE
--rw-r--r--   0        0        0     3510 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/README.md
--rw-r--r--   0        0        0      598 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/__init__.py
--rw-r--r--   0        0        0      428 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/_about.py
--rw-r--r--   0        0        0      183 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/client/__init__.py
--rw-r--r--   0        0        0     9241 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/client/client.py
--rw-r--r--   0        0        0      309 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/client/integration.py
--rw-r--r--   0        0        0      366 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     2324 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/message_command.py
--rw-r--r--   0        0        0     5747 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     2594 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/sub_command.py
--rw-r--r--   0        0        0     2402 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/enum/__init__.py
--rw-r--r--   0        0        0      423 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/ext/__init__.py
--rw-r--r--   0        0        0      312 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/ext/plugins/plugin.py
--rw-r--r--   0        0        0     1720 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/ext/plugins/plugin_integration.py
--rw-r--r--   0        0        0     3457 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/ext/plugins/plugin_manager.py
--rw-r--r--   0        0        0      292 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     8344 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/__init__.py
--rw-r--r--   0        0        0      332 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3035 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     5491 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1937 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       75 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      456 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/utils/__init__.py
--rw-r--r--   0        0        0     1148 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/internal/utils/commands.py
--rw-r--r--   0        0        0      401 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/l10n/__init__.py
--rw-r--r--   0        0        0      147 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/l10n/locale.py
--rw-r--r--   0        0        0     1323 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      255 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/l10n/localized.py
--rw-r--r--   0        0        0      529 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/l10n/pass_localization_provider.py
--rw-r--r--   0        0        0      207 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/options/__init__.py
--rw-r--r--   0        0        0      299 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/options/choice.py
--rw-r--r--   0        0        0     1715 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/py.typed
--rw-r--r--   0        0        0      147 2024-05-20 21:34:34.024497 aurum_hikari-0.1.5/aurum/types.py
--rw-r--r--   0        0        0     2045 2024-05-20 21:34:45.320573 aurum_hikari-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4867 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/LICENSE
+-rw-r--r--   0        0        0     3510 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/README.md
+-rw-r--r--   0        0        0      598 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/__init__.py
+-rw-r--r--   0        0        0      430 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/_about.py
+-rw-r--r--   0        0        0      183 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/client/__init__.py
+-rw-r--r--   0        0        0     9241 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/client/client.py
+-rw-r--r--   0        0        0      309 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/client/integration.py
+-rw-r--r--   0        0        0      366 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2324 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     5767 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     2720 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2402 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4226 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     1720 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_integration.py
+-rw-r--r--   0        0        0     3457 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      292 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/includable.py
+-rw-r--r--   0        0        0      220 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     8344 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/__init__.py
+-rw-r--r--   0        0        0      332 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     5565 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1937 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/utils/commands.py
+-rw-r--r--   0        0        0      401 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      479 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/options/choice.py
+-rw-r--r--   0        0        0     1715 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/py.typed
+-rw-r--r--   0        0        0      147 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/types.py
+-rw-r--r--   0        0        0     2047 2024-05-21 12:04:06.217797 aurum_hikari-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.1/PKG-INFO
```

### Comparing `aurum_hikari-0.1.5/LICENSE` & `aurum_hikari-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/README.md` & `aurum_hikari-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/__init__.py` & `aurum_hikari-0.1.5.1/aurum/__init__.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/client/client.py` & `aurum_hikari-0.1.5.1/aurum/client/client.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.5.1/aurum/commands/decorators/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/commands/message_command.py` & `aurum_hikari-0.1.5.1/aurum/commands/message_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/commands/slash_command.py` & `aurum_hikari-0.1.5.1/aurum/commands/slash_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
 from aurum.commands.sub_command import SubCommand
 from aurum.internal.commands.app_command import AppCommand
 from aurum.internal.consts import SUB_COMMANDS_CONTAINER
 from aurum.internal.utils.commands import build_option
+from aurum.l10n.localized import Localized
 
 if typing.TYPE_CHECKING:
     from collections.abc import Callable, Sequence
 
     from hikari.api import SlashCommandBuilder
     from hikari.guilds import PartialGuild
     from hikari.snowflakes import SnowflakeishOr
@@ -132,17 +133,17 @@
     ) -> SlashCommandBuilder:
         description: LocalizedOr[str] = self.description or "No description"
         builder: SlashCommandBuilder = (
             factory(self.name, str(description))
             .set_default_member_permissions(self.default_member_permissions)
             .set_is_dm_enabled(self.is_dm_enabled)
             .set_is_nsfw(self.is_nsfw)
-            .set_description_localizations(l10n.build_localized(description))
         )
         if not self.sub_commands:
-            builder.set_description_localizations(l10n.build_localized(description))
+            if isinstance(description, Localized):
+                builder.set_description_localizations(l10n.build_localized(description))
             for option in self.options:
                 builder.add_option(build_option(option, l10n))
         else:
             for sub_command in self.sub_commands.values():
                 builder.add_option(sub_command.as_option(l10n))
         return builder
```

### Comparing `aurum_hikari-0.1.5/aurum/commands/sub_command.py` & `aurum_hikari-0.1.5.1/aurum/commands/sub_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import typing
 from dataclasses import dataclass, field
 
 from hikari.commands import CommandOption, OptionType
 
 from aurum.internal.utils.commands import build_option
+from aurum.l10n.localized import Localized
 from aurum.options import Option
 
 if typing.TYPE_CHECKING:
     from collections.abc import Awaitable, Callable, Sequence
 
     from aurum.l10n import LocalizationProviderInterface
     from aurum.l10n.types import LocalizedOr
@@ -58,15 +59,17 @@
 
     def as_option(self, l10n: LocalizationProviderInterface) -> CommandOption:
         options: Sequence[CommandOption]
         if not self.sub_commands:
             options = [build_option(option, l10n) for option in self.options]
         else:
             options = [sub_command.as_option(l10n) for sub_command in self.sub_commands.values()]
+        description: LocalizedOr[str] = self.description or "No description"
         return CommandOption(
             type=OptionType.SUB_COMMAND if not self.sub_commands else OptionType.SUB_COMMAND_GROUP,
-            name=str(self.name),
-            name_localizations=l10n.build_localized(self.name),
-            description=str(self.description),
-            description_localizations=l10n.build_localized(self.description or "No description"),
+            name=str(self.name),  # TODO: display name
+            description=str(description),
+            description_localizations=(
+                l10n.build_localized(description) if isinstance(description, Localized) else {}
+            ),
             options=options,
         )
```

### Comparing `aurum_hikari-0.1.5/aurum/commands/user_command.py` & `aurum_hikari-0.1.5.1/aurum/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/ext/plugins/plugin.py` & `aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/ext/plugins/plugin_integration.py` & `aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_integration.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/ext/plugins/plugin_manager.py` & `aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/interactions/interaction_context.py` & `aurum_hikari-0.1.5.1/aurum/interactions/interaction_context.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/internal/commands/app_command.py` & `aurum_hikari-0.1.5.1/aurum/internal/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.5.1/aurum/internal/commands/command_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 import importlib.util
 import inspect
 import typing
 from logging import getLogger
 from pathlib import Path
 
 from hikari.undefined import UNDEFINED
@@ -66,34 +67,35 @@
         ensuring they are up-to-date with the currently stored command builders.
 
         Args:
             debug: A boolean flag that, when set to True, enables more verbose logging
                    of the synchronization process for debugging purposes.
             build: A boolean flag to enable a automatic building of commands.
         """
+        if not self._app:
+            self._app = await self._bot.rest.fetch_application()
+        synchronized: typing.Dict[
+            SnowflakeishOr[PartialGuild] | UndefinedType, Sequence[PartialCommand]
+        ] = {}
         for name, command in self.commands.items():
             self._commands_builders.setdefault(command.guild, {})
             if isinstance(command, SlashCommand):
                 self._commands_builders[command.guild][name] = command.get_builder(
                     self._bot.rest.slash_command_builder,
                     self._l10n,
                 )
             elif isinstance(command, ContextMenuCommand):
                 self._commands_builders[command.guild][name] = command.get_builder(
                     self._bot.rest.context_menu_command_builder,
                     self._l10n,
                 )
-        synchronized: typing.Dict[
-            SnowflakeishOr[PartialGuild] | UndefinedType, Sequence[PartialCommand]
-        ] = {}
-        if not self._app:
-            self._app = await self._bot.rest.fetch_application()
-        synchronized[UNDEFINED] = await self._bot.rest.set_application_commands(
-            self._app, list(self._commands_builders.pop(UNDEFINED).values())
-        )
+        with contextlib.suppress(KeyError):
+            synchronized[UNDEFINED] = await self._bot.rest.set_application_commands(
+                self._app, list(self._commands_builders.pop(UNDEFINED).values())
+            )
         for guild, commands_builders in self._commands_builders.items():
             synchronized[guild] = await self._bot.rest.set_application_commands(
                 self._app, list(commands_builders.values()), guild=guild
             )
         for entity, commands in synchronized.items():
             for partial_command in commands:
                 self.commands[command.name].set_app(partial_command)
```

### Comparing `aurum_hikari-0.1.5/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.5.1/aurum/internal/commands/context_menu_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/aurum/l10n/localization_provider_interface.py` & `aurum_hikari-0.1.5.1/aurum/l10n/localization_provider_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import typing
 
 if typing.TYPE_CHECKING:
     from hikari import CommandInteraction, ComponentInteraction
 
-    from aurum.l10n.locale import Locale
-    from aurum.l10n.types import LocalizedOr
+    from aurum.l10n.localized import Localized
 
 
 class LocalizationProviderInterface(typing.Protocol):
     """Localization provider interface.
 
     It's used to localize commands, components, and provide a locale for interaction.
 
@@ -23,19 +22,18 @@
         """Start the localization provider.
 
         Warning:
             Important function, must be implemented.
         """
         ...
 
-    def build_localized(self, value: LocalizedOr[str]) -> typing.Dict[str, str]:
+    def build_localized(self, value: Localized) -> typing.Dict[str, str]:
         """Build [Localized object][aurum.l10n.localized.Localized] for Discord API.
 
         Warning:
-            - Important function, must be implemented.
-            - When str is passed to value, this function must return empty dictionary.
+            Important function, must be implemented.
         """
         ...
 
-    def get_locale(self, by: str | CommandInteraction | ComponentInteraction) -> Locale | None:
+    def get_locale(self, by: str | CommandInteraction | ComponentInteraction) -> typing.Any:
         """Get locale by name or interaction"""
         ...
```

### Comparing `aurum_hikari-0.1.5/aurum/options/option.py` & `aurum_hikari-0.1.5.1/aurum/options/option.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5/pyproject.toml` & `aurum_hikari-0.1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 
 # Package information
 [tool.poetry]
 packages = [{ include = "aurum" }]
 name = "aurum-hikari"
-version = "v0.1.5"
+version = "v0.1.5.1"
 license = "MIT"
 authors = ["stefanlight <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible framework for handling commands and components with integrations."
 keywords = [
     "discord",
     "hikari",
     "commands",
```

### Comparing `aurum_hikari-0.1.5/PKG-INFO` & `aurum_hikari-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurum-hikari
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: A flexible framework for handling commands and components with integrations.
 License: MIT
 Keywords: discord,hikari,commands,components,command-handler,component-handler,integrations
 Author: stefanlight
 Author-email: 64615032+stefanlight8@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
```

