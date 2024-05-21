# Comparing `tmp/rbinstall-1.1.1.tar.gz` & `tmp/rbinstall-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbinstall-1.1.1.tar", last modified: Mon Feb 19 06:05:42 2024, max compression
+gzip compressed data, was "rbinstall-1.2.tar", last modified: Tue May 21 05:29:56 2024, max compression
```

## Comparing `rbinstall-1.1.1.tar` & `rbinstall-1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-02-19 06:05:42.984166 rbinstall-1.1.1/
--rw-r--r--   0 chipx86    (501) staff       (20)       62 2024-02-19 06:05:20.000000 rbinstall-1.1.1/AUTHORS
--rw-r--r--   0 chipx86    (501) staff       (20)     1058 2024-02-19 06:05:20.000000 rbinstall-1.1.1/COPYING
--rw-r--r--   0 chipx86    (501) staff       (20)     6567 2024-02-19 06:05:42.983978 rbinstall-1.1.1/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     3784 2024-02-19 06:05:20.000000 rbinstall-1.1.1/README.md
--rw-r--r--   0 chipx86    (501) staff       (20)     1743 2024-02-19 06:05:20.000000 rbinstall-1.1.1/pyproject.toml
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-02-19 06:05:42.982741 rbinstall-1.1.1/rbinstall/
--rw-r--r--   0 chipx86    (501) staff       (20)     1950 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    24671 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/distro_info.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2937 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)    14064 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/install_methods.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11142 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/install_steps.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9685 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/main.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5306 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/process.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4954 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/pypi.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12440 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/state.py
--rw-r--r--   0 chipx86    (501) staff       (20)    15534 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/ui.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4474 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/versioning.py
--rw-r--r--   0 chipx86    (501) staff       (20)    21385 2024-02-19 06:05:20.000000 rbinstall-1.1.1/rbinstall/wizard.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-02-19 06:05:42.983743 rbinstall-1.1.1/rbinstall.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     6567 2024-02-19 06:05:42.000000 rbinstall-1.1.1/rbinstall.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)      499 2024-02-19 06:05:42.000000 rbinstall-1.1.1/rbinstall.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2024-02-19 06:05:42.000000 rbinstall-1.1.1/rbinstall.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       50 2024-02-19 06:05:42.000000 rbinstall-1.1.1/rbinstall.egg-info/entry_points.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       65 2024-02-19 06:05:42.000000 rbinstall-1.1.1/rbinstall.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       10 2024-02-19 06:05:42.000000 rbinstall-1.1.1/rbinstall.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       38 2024-02-19 06:05:42.984204 rbinstall-1.1.1/setup.cfg
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-21 05:29:56.479364 rbinstall-1.2/
+-rw-r--r--   0 chipx86    (501) staff       (20)       62 2024-05-21 05:29:35.000000 rbinstall-1.2/AUTHORS
+-rw-r--r--   0 chipx86    (501) staff       (20)     1058 2024-05-21 05:29:35.000000 rbinstall-1.2/COPYING
+-rw-r--r--   0 chipx86    (501) staff       (20)     6565 2024-05-21 05:29:56.479162 rbinstall-1.2/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     3784 2024-05-21 05:29:35.000000 rbinstall-1.2/README.md
+-rw-r--r--   0 chipx86    (501) staff       (20)     1743 2024-05-21 05:29:35.000000 rbinstall-1.2/pyproject.toml
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-21 05:29:56.478031 rbinstall-1.2/rbinstall/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1950 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    24671 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/distro_info.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2937 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    14064 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/install_methods.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11142 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/install_steps.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10165 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/main.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5306 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/process.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5470 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/pypi.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12949 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/state.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    16085 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/ui.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4474 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/versioning.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    21385 2024-05-21 05:29:35.000000 rbinstall-1.2/rbinstall/wizard.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-21 05:29:56.478906 rbinstall-1.2/rbinstall.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     6565 2024-05-21 05:29:56.000000 rbinstall-1.2/rbinstall.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)      499 2024-05-21 05:29:56.000000 rbinstall-1.2/rbinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2024-05-21 05:29:56.000000 rbinstall-1.2/rbinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       50 2024-05-21 05:29:56.000000 rbinstall-1.2/rbinstall.egg-info/entry_points.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       65 2024-05-21 05:29:56.000000 rbinstall-1.2/rbinstall.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       10 2024-05-21 05:29:56.000000 rbinstall-1.2/rbinstall.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       38 2024-05-21 05:29:56.479413 rbinstall-1.2/setup.cfg
```

### Comparing `rbinstall-1.1.1/COPYING` & `rbinstall-1.2/COPYING`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/PKG-INFO` & `rbinstall-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbinstall
-Version: 1.1.1
+Version: 1.2
 Summary: Official installer for Review Board code/document review.
 Author-email: "Beanbag, Inc." <questions@beanbaginc.com>
 License: Copyright (c) 2023  Beanbag, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `rbinstall-1.1.1/README.md` & `rbinstall-1.2/README.md`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/pyproject.toml` & `rbinstall-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/__init__.py` & `rbinstall-1.2/rbinstall/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 #: The version of the Review Board installer.
 #:
 #: This is in the format of:
 #:
 #: (Major, Minor, Micro, Patch, alpha/beta/rc/final, Release Number, Released)
 #:
-VERSION = (1, 1, 1, 0, 'final', 0, True)
+VERSION = (1, 2, 0, 0, 'final', 0, True)
 
 
 def get_version_string() -> str:
     """Return the version as a human-readable string.
 
     Returns:
         str:
```

### Comparing `rbinstall-1.1.1/rbinstall/distro_info.py` & `rbinstall-1.2/rbinstall/distro_info.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/errors.py` & `rbinstall-1.2/rbinstall/errors.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/install_methods.py` & `rbinstall-1.2/rbinstall/install_methods.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/install_steps.py` & `rbinstall-1.2/rbinstall/install_steps.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/main.py` & `rbinstall-1.2/rbinstall/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import sys
 from gettext import gettext as _
 from typing import Dict, List, Optional, TYPE_CHECKING, Tuple
 
 from rbinstall import get_version_string
 from rbinstall.errors import InstallerError
+from rbinstall.process import debug
 from rbinstall.pypi import get_package_version_info
 from rbinstall.state import get_system_info
 from rbinstall.ui import get_console, init_console
 from rbinstall.wizard import start_wizard
 
 if TYPE_CHECKING:
     from rbinstall.state import InstallState, SystemInfo
@@ -49,40 +50,47 @@
         '--version',
         action='version',
         version='rbinstall %s' % get_version_string(),
         help=_('Show the version of the Review Board installer.'))
     parser.add_argument(
         '--no-color',
         action='store_false',
-        default=True,
+        default=(os.environ.get('RBINSTALL_COLOR') != '0'),
         dest='color',
-        help=_('Disable color output in the terminal'))
+        help=_(
+            'Disable color output in the terminal. You can also set '
+            '$RBINSTALL_COLOR=0.'
+        ))
     parser.add_argument(
         '--noinput',
         action='store_false',
         dest='interactive',
-        default=True,
+        default=(os.environ.get('RBINSTALL_INTERACTIVE') != '0'),
         help=_(
             'Run without prompting for any questions. This allows for '
-            'unattended installs.'
+            'unattended installs. You can also set $RBINSTALL_INTERACTIVE=0.'
         ))
     parser.add_argument(
         '--dry-run',
         action='store_true',
         default=(os.environ.get('RBINSTALL_DRY_RUN') == '1'),
         help=_(
             'Whether to perform a dry-run of the installation. No '
-            'installation commands will actually be run.'
+            'installation commands will actually be run. You can also set '
+            '$RBINSTALL_DRY_RUN=1.'
         ))
     parser.add_argument(
         '--debug',
         action='store_true',
         dest='debug',
         default=(os.environ.get('RBINSTALL_DEBUG') == '1'),
-        help=_('Run with additional debug information.'))
+        help=_(
+            'Run with additional debug information. You can also set '
+            '$RBINSTALL_DEBUG=1.'
+        ))
     parser.add_argument(
         '--install-path',
         metavar='PATH',
         default=os.path.join('/', 'opt', 'reviewboard'),
         help=_('The location for the Review Board install.'))
     parser.add_argument(
         '--create-sitedir',
@@ -211,14 +219,16 @@
                         'package_name': package_name,
                     })
         else:
             version_info = None
 
         package_versions[package_name] = version_info
 
+    debug('All package information has been fetched.')
+
     return package_versions
 
 
 def main(
     argv: List[str] = sys.argv,
 ) -> None:
     """Main entry point for the Review Board installer.
@@ -233,14 +243,16 @@
         argv (list of str, optional):
             The command line arguments to parse.
     """
     options = parse_options(argv[1:])
     console = get_console()
 
     try:
+        debug('Setting up the installer console support.')
+
         init_console(allow_color=options.color,
                      allow_interactive=options.interactive)
 
         if options.interactive and not os.isatty(sys.stdout.fileno()):
             raise InstallerError(_(
                 'To run the Review Board installer without an interactive '
                 'terminal, please run with --noinput. This will run an '
```

### Comparing `rbinstall-1.1.1/rbinstall/process.py` & `rbinstall-1.2/rbinstall/process.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/pypi.py` & `rbinstall-1.2/rbinstall/pypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from packaging.specifiers import SpecifierSet
 from packaging.version import parse as parse_version
 from typing_extensions import TypedDict
 
 from rbinstall import get_package_version
 from rbinstall.errors import InstallerError
+from rbinstall.process import debug
 
 if TYPE_CHECKING:
     from rbinstall.state import SystemInfo
 
 
 USER_AGENT = f'rbinstall/{get_package_version()}'
 
@@ -90,19 +91,24 @@
     """
     url = urljoin(pypi_url, f'pypi/{package_name}/json')
 
     request = Request(url)
     request.add_header('Accept', 'application/json')
     request.add_header('User-Agent', USER_AGENT)
 
+    debug(f'Fetching package information for "{package_name}" from {url}...')
+
     try:
         try:
             with urlopen(request) as fp:
                 rsp = json.load(fp)
         except HTTPError as e:
+            error_data = e.read()
+            debug(f'Received HTTP error {e.code}: {error_data!r}')
+
             if e.code == 404:
                 return None
 
             raise
     except Exception as e:
         raise InstallerError(
             f'Could not fetch information on the {package_name} packages '
@@ -125,14 +131,17 @@
 
         # Find the nearest compatible version of Review Board.
         rsp_releases = sorted(
             rsp['releases'].items(),
             key=lambda pair: parse_version(pair[0]),
             reverse=True)
 
+        debug(f'Found {len(rsp_releases)} possible releases for '
+              f'"{package_name}".')
+
         for rsp_version, rsp_release in rsp_releases:
             if not rsp_release:
                 continue
 
             parsed_rsp_version = parse_version(rsp_version)
 
             if parsed_rsp_version > parsed_target_version:
@@ -144,24 +153,29 @@
                 continue
 
             requires_python = rsp_dist.get('requires_python', '')
 
             if (not requires_python or
                 python_version in SpecifierSet(requires_python)):
                 # This is a compatible version. Return it.
+                debug(f'Found compatible release for "{package_name}": '
+                      f'{parsed_rsp_version}')
+
                 return {
                     'is_latest': parsed_rsp_version == parsed_latest_version,
                     'is_requested':
                         parsed_rsp_version == parsed_target_version,
                     'latest_version': latest_version,
                     'package_name': rsp_info['name'],
                     'requires_python': requires_python,
                     'version': rsp_version,
                 }
 
+        debug(f'Could not find compatible release for "{package_name}".')
+
         return None
     except Exception as e:
         raise InstallerError(
             f'Could not parse information on {package_name} packages '
             f'(at {url}). This may indicate an issue accessing '
             f'https://pypi.org/ or an issue with the requested version of '
             f'Review Board. The error was: {e}'
```

### Comparing `rbinstall-1.1.1/rbinstall/state.py` & `rbinstall-1.2/rbinstall/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,16 @@
         SystemInfo:
         The computed information on the system.
 
     Raises:
         rbinstall.errors.InstallerError:
             There was an error computing system information.
     """
+    debug('Fetching information on the current system...')
+
     system_info: SystemInfo
     system_install_method: Optional[InstallMethodType]
 
     system = os.environ.get('RBINSTALL_FORCE_SYSTEM') or platform.system()
     arch = os.environ.get('RBINSTALL_FORCE_ARCH') or platform.machine()
 
     paths: Dict[str, str] = {}
@@ -198,25 +200,29 @@
     if system == 'Linux':
         # This is a Linux system.
         #
         # We'll be looking for a "os-release" file, which will tell us
         # information about the Linux distribution. From that, we can
         # determine the default method for installation, and what packages
         # we need to install.
+        debug('Found Linux. Fetching distribution information...')
+
         distro_info = get_linux_distro_info()
 
         if not distro_info:
             raise InstallerError(
                 f'Could not determine the distribution of Linux being used. '
                 f'This indicates you may be missing /etc/os-release and '
                 f'/usr/lib/os-release files. You may need to install through '
                 f'another method. See {INSTALLATION_DOCS_URL} for '
                 f'instructions.'
             )
 
+        debug(f'Distribution information = {distro_info!r}')
+
         # Determine the Linux distro families supported by this distro.
         distro_id = distro_info.get('ID')
         id_like = distro_info.get('ID_LIKE')
         families: Set[str] = set()
 
         if distro_id:
             families.add(distro_id)
@@ -225,16 +231,18 @@
             families.update(id_like.split())
 
         families_str = ', '.join(sorted(families))
 
         debug(f'Linux families = {families_str}')
 
         # Determine the install methods enabled for this distro.
+        debug('Determining the default install method...')
         system_install_method = get_default_linux_install_method(
             families=families)
+        debug(f'Install method = {system_install_method!r}')
 
         if not system_install_method:
             raise InstallerError(
                 f"The Review Board installer doesn't support installing on "
                 f"this family of Linux ({families_str}). Please contact "
                 f"support@beanbaginc.com for assistance. You may need to "
                 f"install through another method. See "
@@ -258,14 +266,16 @@
             'system_python_version': system_python_version,
             'version': distro_info.get('VERSION_ID') or '',
         }
     elif system == 'Darwin':
         # This is a macOS system.
         #
         # On macOS, we can use brew to install dependencies.
+        debug('Found macOS. Please note, Brew is required.')
+
         mac_ver = platform.mac_ver()
 
         if not mac_ver[0]:
             raise InstallerError(
                 f'Python reports that this is macOS, but no macOS version was '
                 f'found! This seems to be a Python installation issue. You '
                 f'may need to install through another method. See '
@@ -349,16 +359,21 @@
         os_release_paths = [custom_os_release_file]
     else:
         os_release_paths = [
             '/etc/os-release',
             '/usr/lib/os-release',
         ]
 
+    debug(f'Checking for an os-release file (considering '
+          f'{os_release_paths!r})')
+
     for path in os_release_paths:
         if os.path.exists(path):
+            debug(f'Parsing {path}...')
+
             with open(path, 'r') as fp:
                 for line in fp.readlines():
                     m = line_re.match(line)
 
                     if m:
                         distro_info[m.group('name')] = \
                             unescape_re.sub(r'\1', m.group('value'))
```

### Comparing `rbinstall-1.1.1/rbinstall/ui.py` & `rbinstall-1.2/rbinstall/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,25 +228,37 @@
     Version Added:
         1.0
 
     Returns:
         bool:
         ``True`` if the terminal is in dark mode. ``False`` if in light mode.
     """
+    from rbinstall.process import debug
+
+    debug('Attempting to determine terminal color configuration...')
+
     try:
         fg, *unused, bg = os.getenv('COLORFGBG', '').split(';')
 
+        debug(f'Got COLOFGBG: Foreground = {fg}, Background = {bg}')
+
         # 0=black, 7=light-grey, 15=white.
-        return fg in ('7', '15') and bg == '0'
+        is_dark = fg in ('7', '15') and bg == '0'
+
+        debug(f'Parsed COLORFGBG dark background result: {is_dark}')
+
+        return is_dark
     except Exception:
         pass
 
     # Try an xterm-compatible terminal ANSI command for checking the
     # background color.
+    debug('Querying terminal for background color...')
     xterm_bg_info = query_terminal('\033]11;?\a', terminator='\a')
+    debug(f'Got terminal result = {xterm_bg_info!r}')
 
     if xterm_bg_info:
         # This actually comes in 4-digit R, G, and B values. We're only going
         # to look at the first digit of each. There's maybe a better way of
         # calculating dark vs. light mode here, but we're going with what Vim
         # itself does.
         m = re.search(
@@ -269,17 +281,23 @@
                 for value in (r, g, b)
             )
 
             # Calculate a luma based on the background color.
             luma = 0.2126 * r + 0.7152 * g + 0.0722 * b
             luma_pct = (luma / 255) * 100
 
-            return luma_pct < 50
+            is_dark = luma_pct < 50
+
+            debug(f'Queried dark background result: {is_dark}')
+
+            return is_dark
 
     # Dark backgrounds are a reasonable default.
+    debug('Falling back to assuming terminal background is dark.')
+
     return True
 
 
 def query_terminal(
     ansi_code: str,
     *,
     terminator: str = '\a',
```

### Comparing `rbinstall-1.1.1/rbinstall/versioning.py` & `rbinstall-1.2/rbinstall/versioning.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall/wizard.py` & `rbinstall-1.2/rbinstall/wizard.py`

 * *Files identical despite different names*

### Comparing `rbinstall-1.1.1/rbinstall.egg-info/PKG-INFO` & `rbinstall-1.2/rbinstall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbinstall
-Version: 1.1.1
+Version: 1.2
 Summary: Official installer for Review Board code/document review.
 Author-email: "Beanbag, Inc." <questions@beanbaginc.com>
 License: Copyright (c) 2023  Beanbag, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

