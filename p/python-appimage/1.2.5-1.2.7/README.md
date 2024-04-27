# Comparing `tmp/python_appimage-1.2.5-py2.py3-none-any.whl.zip` & `tmp/python_appimage-1.2.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,44 @@
-Zip file size: 73399 bytes, number of entries: 40
--rw-r--r--  2.0 unx      114 b- defN 22-Dec-23 13:07 python_appimage/__init__.py
--rw-r--r--  2.0 unx     4150 b- defN 22-Dec-23 13:07 python_appimage/__main__.py
--rw-r--r--  2.0 unx       81 b- defN 22-Dec-23 13:07 python_appimage/version.py
--rw-r--r--  2.0 unx      275 b- defN 22-Dec-23 13:07 python_appimage/appimage/__init__.py
--rw-r--r--  2.0 unx     1903 b- defN 22-Dec-23 13:07 python_appimage/appimage/build.py
--rw-r--r--  2.0 unx    14241 b- defN 22-Dec-23 13:07 python_appimage/appimage/relocate.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 13:07 python_appimage/commands/__init__.py
--rw-r--r--  2.0 unx      527 b- defN 22-Dec-23 13:07 python_appimage/commands/install.py
--rw-r--r--  2.0 unx      378 b- defN 22-Dec-23 13:07 python_appimage/commands/which.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 13:07 python_appimage/commands/build/__init__.py
--rw-r--r--  2.0 unx    11627 b- defN 22-Dec-23 13:07 python_appimage/commands/build/app.py
--rw-r--r--  2.0 unx     1042 b- defN 22-Dec-23 13:07 python_appimage/commands/build/local.py
--rw-r--r--  2.0 unx     3641 b- defN 22-Dec-23 13:07 python_appimage/commands/build/manylinux.py
--rw-r--r--  2.0 unx     1085 b- defN 22-Dec-23 13:07 python_appimage/data/LICENSE
--rw-r--r--  2.0 unx      491 b- defN 22-Dec-23 13:07 python_appimage/data/_initappimage.py
--rwxr-xr-x  2.0 unx      221 b- defN 22-Dec-23 13:07 python_appimage/data/apprun.sh
--rwxr-xr-x  2.0 unx       49 b- defN 22-Dec-23 13:07 python_appimage/data/entrypoint.sh
--rw-rw-rw-  2.0 unx    10774 b- defN 22-Dec-23 13:07 python_appimage/data/excludelist
--rwxr-xr-x  2.0 unx      445 b- defN 22-Dec-23 13:07 python_appimage/data/python-wrapper.sh
--rw-r--r--  2.0 unx      641 b- defN 22-Dec-23 13:07 python_appimage/data/python.appdata.xml
--rw-r--r--  2.0 unx      170 b- defN 22-Dec-23 13:07 python_appimage/data/python.desktop
--rw-r--r--  2.0 unx    28792 b- defN 22-Dec-23 13:07 python_appimage/data/python.png
--rw-r--r--  2.0 unx     3144 b- defN 22-Dec-23 13:07 python_appimage/data/sitecustomize.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 13:07 python_appimage/utils/__init__.py
--rw-r--r--  2.0 unx      753 b- defN 22-Dec-23 13:07 python_appimage/utils/compat.py
--rw-r--r--  2.0 unx     3024 b- defN 22-Dec-23 13:07 python_appimage/utils/deps.py
--rw-r--r--  2.0 unx     1389 b- defN 22-Dec-23 13:07 python_appimage/utils/docker.py
--rw-r--r--  2.0 unx     2079 b- defN 22-Dec-23 13:07 python_appimage/utils/fs.py
--rw-r--r--  2.0 unx      389 b- defN 22-Dec-23 13:07 python_appimage/utils/log.py
--rw-r--r--  2.0 unx     1621 b- defN 22-Dec-23 13:07 python_appimage/utils/system.py
--rw-r--r--  2.0 unx      898 b- defN 22-Dec-23 13:07 python_appimage/utils/template.py
--rw-r--r--  2.0 unx      496 b- defN 22-Dec-23 13:07 python_appimage/utils/tmp.py
--rw-r--r--  2.0 unx      988 b- defN 22-Dec-23 13:07 python_appimage/utils/url.py
--rw-r--r--  2.0 unx      163 b- defN 22-Dec-23 13:07 python_appimage/utils/version.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Dec-23 13:07 python_appimage-1.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3095 b- defN 22-Dec-23 13:07 python_appimage-1.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-23 13:07 python_appimage-1.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 22-Dec-23 13:07 python_appimage-1.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 22-Dec-23 13:07 python_appimage-1.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3567 b- defN 22-Dec-23 13:07 python_appimage-1.2.5.dist-info/RECORD
-40 files, 137595 bytes uncompressed, 67599 bytes compressed:  50.9%
+Zip file size: 74865 bytes, number of entries: 42
+-rw-r--r--  2.0 unx      114 b- defN 24-Apr-27 08:33 python_appimage/__init__.py
+-rw-r--r--  2.0 unx     4354 b- defN 24-Apr-27 08:33 python_appimage/__main__.py
+-rw-r--r--  2.0 unx       81 b- defN 24-Apr-27 08:33 python_appimage/version.py
+-rw-r--r--  2.0 unx      275 b- defN 24-Apr-27 08:33 python_appimage/appimage/__init__.py
+-rw-r--r--  2.0 unx     1903 b- defN 24-Apr-27 08:33 python_appimage/appimage/build.py
+-rw-r--r--  2.0 unx    14256 b- defN 24-Apr-27 08:33 python_appimage/appimage/relocate.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 08:33 python_appimage/commands/__init__.py
+-rw-r--r--  2.0 unx      527 b- defN 24-Apr-27 08:33 python_appimage/commands/install.py
+-rw-r--r--  2.0 unx     1123 b- defN 24-Apr-27 08:33 python_appimage/commands/list.py
+-rw-r--r--  2.0 unx      378 b- defN 24-Apr-27 08:33 python_appimage/commands/which.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 08:33 python_appimage/commands/build/__init__.py
+-rw-r--r--  2.0 unx    11863 b- defN 24-Apr-27 08:33 python_appimage/commands/build/app.py
+-rw-r--r--  2.0 unx     1042 b- defN 24-Apr-27 08:33 python_appimage/commands/build/local.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-Apr-27 08:33 python_appimage/commands/build/manylinux.py
+-rw-r--r--  2.0 unx     1085 b- defN 24-Apr-27 08:33 python_appimage/data/LICENSE
+-rw-r--r--  2.0 unx      491 b- defN 24-Apr-27 08:33 python_appimage/data/_initappimage.py
+-rwxr-xr-x  2.0 unx      221 b- defN 24-Apr-27 08:33 python_appimage/data/apprun.sh
+-rwxr-xr-x  2.0 unx       49 b- defN 24-Apr-27 08:33 python_appimage/data/entrypoint.sh
+-rw-rw-rw-  2.0 unx    11009 b- defN 24-Apr-27 08:33 python_appimage/data/excludelist
+-rwxr-xr-x  2.0 unx      445 b- defN 24-Apr-27 08:33 python_appimage/data/python-wrapper.sh
+-rw-r--r--  2.0 unx      641 b- defN 24-Apr-27 08:33 python_appimage/data/python.appdata.xml
+-rw-r--r--  2.0 unx      170 b- defN 24-Apr-27 08:33 python_appimage/data/python.desktop
+-rw-r--r--  2.0 unx    28792 b- defN 24-Apr-27 08:33 python_appimage/data/python.png
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-27 08:33 python_appimage/data/sitecustomize.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 08:33 python_appimage/utils/__init__.py
+-rw-r--r--  2.0 unx      753 b- defN 24-Apr-27 08:33 python_appimage/utils/compat.py
+-rw-r--r--  2.0 unx     3024 b- defN 24-Apr-27 08:33 python_appimage/utils/deps.py
+-rw-r--r--  2.0 unx     1601 b- defN 24-Apr-27 08:33 python_appimage/utils/docker.py
+-rw-r--r--  2.0 unx     2079 b- defN 24-Apr-27 08:33 python_appimage/utils/fs.py
+-rw-r--r--  2.0 unx      667 b- defN 24-Apr-27 08:33 python_appimage/utils/log.py
+-rw-r--r--  2.0 unx      386 b- defN 24-Apr-27 08:33 python_appimage/utils/manylinux.py
+-rw-r--r--  2.0 unx     1815 b- defN 24-Apr-27 08:33 python_appimage/utils/system.py
+-rw-r--r--  2.0 unx      898 b- defN 24-Apr-27 08:33 python_appimage/utils/template.py
+-rw-r--r--  2.0 unx      496 b- defN 24-Apr-27 08:33 python_appimage/utils/tmp.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-27 08:33 python_appimage/utils/url.py
+-rw-r--r--  2.0 unx      163 b- defN 24-Apr-27 08:33 python_appimage/utils/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-Apr-27 08:33 python_appimage-1.2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3095 b- defN 24-Apr-27 08:33 python_appimage-1.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-27 08:33 python_appimage-1.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-27 08:33 python_appimage-1.2.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-27 08:33 python_appimage-1.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3746 b- defN 24-Apr-27 08:33 python_appimage-1.2.7.dist-info/RECORD
+42 files, 140641 bytes uncompressed, 68781 bytes compressed:  51.1%
```

## zipnote {}

```diff
@@ -18,14 +18,17 @@
 
 Filename: python_appimage/commands/__init__.py
 Comment: 
 
 Filename: python_appimage/commands/install.py
 Comment: 
 
+Filename: python_appimage/commands/list.py
+Comment: 
+
 Filename: python_appimage/commands/which.py
 Comment: 
 
 Filename: python_appimage/commands/build/__init__.py
 Comment: 
 
 Filename: python_appimage/commands/build/app.py
@@ -81,14 +84,17 @@
 
 Filename: python_appimage/utils/fs.py
 Comment: 
 
 Filename: python_appimage/utils/log.py
 Comment: 
 
+Filename: python_appimage/utils/manylinux.py
+Comment: 
+
 Filename: python_appimage/utils/system.py
 Comment: 
 
 Filename: python_appimage/utils/template.py
 Comment: 
 
 Filename: python_appimage/utils/tmp.py
@@ -96,26 +102,26 @@
 
 Filename: python_appimage/utils/url.py
 Comment: 
 
 Filename: python_appimage/utils/version.py
 Comment: 
 
-Filename: python_appimage-1.2.5.dist-info/LICENSE
+Filename: python_appimage-1.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: python_appimage-1.2.5.dist-info/METADATA
+Filename: python_appimage-1.2.7.dist-info/METADATA
 Comment: 
 
-Filename: python_appimage-1.2.5.dist-info/WHEEL
+Filename: python_appimage-1.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: python_appimage-1.2.5.dist-info/entry_points.txt
+Filename: python_appimage-1.2.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: python_appimage-1.2.5.dist-info/top_level.txt
+Filename: python_appimage-1.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: python_appimage-1.2.5.dist-info/RECORD
+Filename: python_appimage-1.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## python_appimage/__main__.py

```diff
@@ -1,10 +1,9 @@
 import argparse
 from importlib import import_module
-import logging
 import os
 import sys
 
 
 __all__ = ['main']
 
 
@@ -20,17 +19,17 @@
         prog='python-appimage',
         description='Bundle a Python installation into an AppImage')
     subparsers = parser.add_subparsers(title='command',
                                        help='Command to execute',
                                        dest='command')
 
     parser.add_argument('-q', '--quiet', help='disable logging',
-        dest='verbosity', action='store_const', const=logging.ERROR)
+        dest='verbosity', action='store_const', const='ERROR')
     parser.add_argument('-v', '--verbose', help='print extra information',
-        dest='verbosity', action='store_const', const=logging.DEBUG)
+        dest='verbosity', action='store_const', const='DEBUG')
 
     install_parser = subparsers.add_parser('install',
         description='Install binary dependencies')
     install_parser.add_argument('binary', nargs='+',
         choices=binaries, help='one or more binary name')
 
     build_parser = subparsers.add_parser('build',
@@ -71,24 +70,30 @@
     build_app_parser.add_argument('-p', '--python-version',
         help='python version (e.g. 3.8)')
     build_app_parser.add_argument('--in-tree-build',
                                   help='force pip in-tree-build',
                                   action='store_true',
                                   default=False)
 
+    list_parser = subparsers.add_parser('list',
+        description='List Python versions installed in a manylinux image')
+    list_parser.add_argument('tag',
+        help='manylinux image tag (e.g. 2010_x86_64)')
+
     which_parser = subparsers.add_parser('which',
         description='Locate a binary dependency')
     which_parser.add_argument('binary', choices=binaries,
         help='name of the binary to locate')
 
     args = parser.parse_args()
 
     # Configure the verbosity
     if args.verbosity:
-        logging.getLogger().setLevel(args.verbosity)
+        from .utils import log
+        log.set_level(args.verbosity)
 
     # check if no arguments are passed
     if args.command is None:
         parser.print_help()
         return
 
     # Call the requested command
```

## python_appimage/version.py

```diff
@@ -1,3 +1,3 @@
 # This file was generated by setup.py
-version = '1.2.5'
-git_revision = 'db5d91e'
+version = '1.2.7'
+git_revision = '9de84d8'
```

## python_appimage/appimage/relocate.py

```diff
@@ -94,15 +94,15 @@
     else:
         excluded = _excluded_libs
 
     ensure_patchelf()
     rpath = '\'' + system((PATCHELF, '--print-rpath', path)) + '\''
     relpath = os.path.relpath(libdir, os.path.dirname(path))
     relpath = '' if relpath == '.' else '/' + relpath
-    expected = '\'$ORIGIN' + relpath + '\''
+    expected = '\'$ORIGIN' + relpath + ':$ORIGIN/../lib\''
     if rpath != expected:
         system((PATCHELF, '--set-rpath', expected, path))
 
     deps = ldd(path)
     for dep in deps:
         name = os.path.basename(dep)
         if name in excluded:
```

## python_appimage/commands/build/app.py

```diff
@@ -249,14 +249,20 @@
             deprecation = (
                 'DEPRECATION: Python 2.7 reached the end of its life',
                 'DEPRECATION: Python 3.5 reached the end of its life',
                 'DEPRECATION: In-tree builds are now the default',
                 'WARNING: Running pip as'
             )
 
+            git_warnings = (
+                re.compile(r'\s+Running command git (clone|checkout) '),
+                re.compile(r"\s+Branch '.*' set up to track remote"),
+                re.compile(r"\s+Switched to a new branch '.*'"),
+            )
+
             isolation_flag = '-sE' if python_version[0] == '2' else '-I'
             system(('./AppDir/AppRun', isolation_flag, '-m', 'pip', 'install', '-U', in_tree_build,
                    '--no-warn-script-location', 'pip'), exclude=deprecation)
             for requirement in requirements_list:
                 if requirement.startswith('git+'):
                     url, name = os.path.split(requirement)
                     log('BUNDLE', name + ' from ' + url[4:])
@@ -275,15 +281,15 @@
                         destination = 'AppDir/opt/python{0:}/lib/python{0:}/site-packages/{1:}'.format(python_version, name)
                         copy_tree(source, destination)
                     continue
                 else:
                     log('BUNDLE', requirement)
                 system(('./AppDir/AppRun', isolation_flag, '-m', 'pip', 'install', '-U', in_tree_build,
                        '--no-warn-script-location', requirement),
-                       exclude=(deprecation, '  Running command git clone'))
+                       exclude=(deprecation + git_warnings))
 
 
         # Bundle the entry point
         entrypoint_path = glob.glob(appdir + '/entrypoint.*')
         if entrypoint_path:
             entrypoint_path = entrypoint_path[0]
             log('BUNDLE', os.path.basename(entrypoint_path))
```

## python_appimage/commands/build/manylinux.py

```diff
@@ -3,62 +3,57 @@
 import platform
 import shutil
 import sys
 
 from ...appimage import build_appimage, relocate_python
 from ...utils.docker import docker_run
 from ...utils.fs import copy_tree
+from ...utils.manylinux import format_appimage_name, format_tag
 from ...utils.tmp import TemporaryDirectory
 
 
 __all__ = ['execute']
 
 
 def _unpack_args(args):
     '''Unpack command line arguments
     '''
     return args.tag, args.abi, args.contained
 
 
-def _manylinux_tag(tag):
-    '''Format Manylinux tag
-    '''
-    if tag.startswith('2_'):
-        return 'manylinux_' + tag
-    else:
-        return 'manylinux' + tag
-
-
 def _get_appimage_name(abi, tag):
     '''Format the Python AppImage name using the ABI and OS tags
     '''
     # Read the Python version from the desktop file
     desktop = glob.glob('AppDir/python*.desktop')[0]
     fullversion = desktop[13:-8]
 
     # Finish building the AppImage on the host. See below.
-    return 'python{:}-{:}-{:}.AppImage'.format(
-        fullversion, abi, _manylinux_tag(tag))
+    return format_appimage_name(abi, fullversion, tag)
 
 
 def execute(tag, abi, contained=False):
     '''Build a Python AppImage using a manylinux docker image
     '''
 
     if not contained:
         # Forward the build to a Docker image
-        image = 'quay.io/pypa/' + _manylinux_tag(tag)
+        image = 'quay.io/pypa/' + format_tag(tag)
         python = '/opt/python/' + abi + '/bin/python'
 
         pwd = os.getcwd()
         dirname = os.path.abspath(os.path.dirname(__file__) + '/../..')
         with TemporaryDirectory() as tmpdir:
             copy_tree(dirname, 'python_appimage')
 
-            argv = ' '.join(sys.argv[1:])
+            argv = sys.argv[1:]
+            if argv:
+                argv = ' '.join(argv)
+            else:
+                argv = 'build manylinux {:} {:}'.format(tag, abi)
             if tag.startswith("1_"):
                 # On manylinux1 tk is not installed
                 script = [
                     'yum --disablerepo="*" --enablerepo=base install -q -y tk']
             else:
                 # tk is already installed on other platforms
                 script = []
```

## python_appimage/data/excludelist

```diff
@@ -79,14 +79,18 @@
 
 libX11.so.6
 # Workaround for:
 # Fedora 23
 # symbol lookup error: ./lib/libX11.so.6: undefined symbol: xcb_wait_for_reply64
 # Uncertain if this is required to be bundled for some distributions - if so we need to write a version check script and use LD_PRELOAD to load the system version if it is newer
 
+libX11-xcb.so.1
+# https://github.com/probonopd/linuxdeployqt/issues/582
+# Uncertain if this is required to be bundled for some distributions - if so, please let us know
+
 # The following libraries need to be privately bundled
 # Workaround for: /lib/x86_64-linux-gnu/libgio-2.0.so.0: undefined symbol: g_module_open_full
 # https://github.com/AppImage/pkg2appimage/pull/500#issuecomment-997183221
 # Workaround for: <AppDir>/usr/lib/x86_64-linux-gnu/libgnutls.so.30: version `GNUTLS_3_6_9' not found (required by /lib64/libglib-2.0.so.0)
 # https://github.com/probonopd/Emacs.AppImage/issues/16
 # NOTE: Privately bundling libglib-2.0.so.0 and libgobject-2.0.so.0 may break https://wiki.gnome.org/Projects/Libsecret,
 # see https://github.com/probonopd/linuxdeployqt/issues/544 for details
@@ -156,15 +160,15 @@
 libICE.so.6
 # libidn.so.11 # Does not come with Solus by default
 # libk5crypto.so.3 # Running AppImage built on Debian 9 or Ubuntu 16.04 on an Archlinux fails otherwise; https://github.com/AppImage/AppImages/issues/301
 # libkeyutils.so.1 # Does not come with Void Linux by default; https://github.com/Subsurface-divelog/subsurface/issues/1971#issuecomment-466606834
 # libkrb5.so.26 # Disputed, seemingly needed by Arch Linux since Kerberos is named differently there. Missing on openSUSE LEAP 42.0
 # libkrb5.so.3 # Disputed, seemingly needed by Arch Linux since Kerberos is named differently there
 # libkrb5support.so.0 # Disputed, seemingly needed by Arch Linux since Kerberos is named differently there
-libp11-kit.so.0
+# libp11-kit.so.0 # https://github.com/AppImageCommunity/pkg2appimage/issues/547
 # libpcre.so.3 # Missing on Fedora 24, SLED 12 SP1, and openSUSE Leap 42.2
 # libroken.so.18 # Mission on openSUSE LEAP 42.0
 # libsasl2.so.2 # Seemingly needed when running Ubuntu 14.04 binaries on Fedora 23
 libSM.so.6
 libusb-1.0.so.0
 libuuid.so.1
 # libwind.so.0 # Missing on openSUSE LEAP 42.0
```

## python_appimage/utils/docker.py

```diff
@@ -1,18 +1,19 @@
 import os
 import platform
 import stat
 import subprocess
 import sys
 
+from .compat import decode
 from .log import log
 from .system import system
 
 
-def docker_run(image, extra_cmds):
+def docker_run(image, extra_cmds, capture=False):
     '''Execute commands within a docker container
     '''
 
     ARCH = platform.machine()
     if image.endswith(ARCH):
         bash_arg = '/pwd/run.sh'
     elif image.endswith('i686') and ARCH == 'x86_64':
@@ -38,14 +39,20 @@
         f.write(os.linesep.join(script))
     os.chmod('run.sh', stat.S_IRWXU)
 
     cmd = ' '.join(('docker', 'run', '--mount',
                     'type=bind,source={:},target=/pwd'.format(os.getcwd()),
                     image, '/bin/bash', bash_arg))
 
+    if capture:
+        opts = {'stderr': subprocess.PIPE, 'stdout': subprocess.PIPE}
+    else:
+        opts = {}
     log('RUN', image)
-    p = subprocess.Popen(cmd, shell=True)
-    p.communicate()
+    p = subprocess.Popen(cmd, shell=True, **opts)
+    r = p.communicate()
     if p.returncode != 0:
         if p.returncode == 139:
             sys.stderr.write("segmentation fault when running Docker (139)\n")
         sys.exit(p.returncode)
+    if capture:
+        return decode(r[0])
```

## python_appimage/utils/log.py

```diff
@@ -3,21 +3,29 @@
 
 __all__ = ['debug', 'log']
 
 
 # Configure the logger
 logging.basicConfig(
     format='[%(asctime)s] %(message)s',
-    level=logging.INFO
+    level=logging.ERROR
 )
+logging.getLogger('python-appimage').setLevel(logging.INFO)
 
 
 def log(task, fmt, *args):
     '''Log a standard message
     '''
-    logging.info('%-8s ' + fmt, task, *args)
+    logging.getLogger('python-appimage').info('%-8s ' + fmt, task, *args)
 
 
 def debug(task, fmt, *args):
     '''Report some debug information
     '''
-    logging.debug('%-8s ' + fmt, task, *args)
+    logging.getLogger('python-appimage').debug('%-8s ' + fmt, task, *args)
+
+
+def set_level(level):
+    '''Set the threshold for logs
+    '''
+    level = getattr(logging, level)
+    logging.getLogger('python-appimage').setLevel(level)
```

## python_appimage/utils/system.py

```diff
@@ -37,17 +37,24 @@
 
     p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
                          stderr=subprocess.PIPE, stdin=in_arg)
     out, err = p.communicate(input=stdin)
     if err:
         err = decode(err)
         stripped = [line for line in err.split(os.linesep) if line]
+
+        def matches_pattern(line, pattern):
+            if isinstance(pattern, re.Pattern):
+                return bool(pattern.match(line))
+            return line.startswith(pattern)
+
         for pattern in exclude:
             stripped = [line for line in stripped
-                        if not line.startswith(pattern)]
+                        if not matches_pattern(line, pattern)]
+
         if stripped:
             # Tolerate single line warning(s)
             for line in stripped:
                 if (len(line) < 8) or (line[:8].lower() != "warning:"):
                     raise RuntimeError(err)
             else:
                 for line in stripped:
```

## Comparing `python_appimage-1.2.5.dist-info/LICENSE` & `python_appimage-1.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_appimage-1.2.5.dist-info/METADATA` & `python_appimage-1.2.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-appimage
-Version: 1.2.5
+Version: 1.2.7
 Summary: Appimage releases of Python
 Home-page: https://github.com/niess/python-appimage
 Author: Valentin Niess
 Author-email: valentin.niess@gmail.com
 License: GPLv3
 Download-URL: https://pypi.python.org/pypi/python-appimage
 Project-URL: Bug Tracker, https://github.com/niess/python-appimage/issues
```

## Comparing `python_appimage-1.2.5.dist-info/RECORD` & `python_appimage-1.2.7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 python_appimage/__init__.py,sha256=-mpxOEjP18p7V4KREyW_Yte1qHRqFWyTc6Ct9locVMo,114
-python_appimage/__main__.py,sha256=AODo-PyiBVi8DdqJXCM1gBaf3mmB4k8LlzHnF7TKCTA,4150
-python_appimage/version.py,sha256=PNBIzxpDKoeRlGCYj3y06-C6rMjs6QhYiuzKaBY2Gk4,81
+python_appimage/__main__.py,sha256=rvwxzvhjIcYoJ0yBe-FNTI_MSA9TXxVUcEkhDddpRNc,4354
+python_appimage/version.py,sha256=WLd9n6-63SlAd5eP21y-buTKiQ3iUyCqtxr0t0AWuvc,81
 python_appimage/appimage/__init__.py,sha256=eYQOgd83PPrpRt_l_i3gJajysg919DT6ycfq-jJovl8,275
 python_appimage/appimage/build.py,sha256=Lp5zpSBfahN2WYtjztGD7ZGKtFvudF2G-Md2Z2_c2eE,1903
-python_appimage/appimage/relocate.py,sha256=dXFkrUGfzMLLE0YYt3cuEZUZnFMKvkPYjLyl3I3qF1c,14241
+python_appimage/appimage/relocate.py,sha256=3TzFaEVSJ2ldSBB-wAxbBE3CaaPKUbp2Esd4ZMpRI6s,14256
 python_appimage/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_appimage/commands/install.py,sha256=9yFgdhUiHyU6khKPwckgVgRU3EQRiWmeqw4eh0-TGtg,527
+python_appimage/commands/list.py,sha256=W132gDu7ffffpL8471Ay-NPhwqhFkVVX9Ok6tFdoheI,1123
 python_appimage/commands/which.py,sha256=0ZzLuQsEmPQvqFvN5dkvoXHgyGD-ZPVD_1isWeVLsgs,378
 python_appimage/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-python_appimage/commands/build/app.py,sha256=uaRMheeeKDjDEW8l_GzP2PMpTbwjfkAVe6pi8RipS0Y,11627
+python_appimage/commands/build/app.py,sha256=OVI3RzlpNYLWfiKH4xiM_BOvWWBKjfcen6yWcySbeUI,11863
 python_appimage/commands/build/local.py,sha256=PwOXWQIKvvjIHOVyzcMcS9ViX7zJcoNNiO0tTA-Gh0E,1042
-python_appimage/commands/build/manylinux.py,sha256=CnMJsg8qyG70QH_1wsJO_Ry0jJcOWx6TWFnCvqasPbI,3641
+python_appimage/commands/build/manylinux.py,sha256=U9jU_WNWOqqCDAWBD8BECYRYKQNo2118LGfuP041WIc,3625
 python_appimage/data/LICENSE,sha256=DkcLCzOlvZufwJhKFOzkaAsJO-ywsgd53BEQ-yY3jfA,1085
 python_appimage/data/_initappimage.py,sha256=5awuy0agK6CHefb7LSUO2IaX5ZiMN7zne5q8xanSkfA,491
 python_appimage/data/apprun.sh,sha256=V8F-6hg-e6rAUxxPy63leV_pFdV3fXAafa6DI3Y3NDw,221
 python_appimage/data/entrypoint.sh,sha256=xkj-klDl-QJ31IA65WvQrAAdLpU71S_qtErKbNknWBg,49
-python_appimage/data/excludelist,sha256=ID3t5ciogcO_od7rzkrxHJ0co1rIhr3l3-ZhW9Zs2Qk,10774
+python_appimage/data/excludelist,sha256=ZG7B70iDUewSssGrUqoOhG5Nf8DTrSLo75nxKGBPKT8,11009
 python_appimage/data/python-wrapper.sh,sha256=TI9OM2thdjd7OYXG8c_Mqv7UDBSum_Q_KintU7cWRsk,445
 python_appimage/data/python.appdata.xml,sha256=L7e9JGfgYuGCXYOx4_13W_Q1sH-lr5fbmtO8krjIGPE,641
 python_appimage/data/python.desktop,sha256=VXR6YRl9NWtcm-IybZ3QEN4_3FeBVmtxQLyDjWNgVcQ,170
 python_appimage/data/python.png,sha256=iqeZCDnfTLTlPBDozNW1Fq9RcOmrAGLUw0ycnudcKSE,28792
 python_appimage/data/sitecustomize.py,sha256=eapSqK3cexwZ_2rjbeiHJL9DEdc_i5RI03TiWQBXO_M,3144
 python_appimage/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_appimage/utils/compat.py,sha256=MNTgk6q86dqcq3PzVuV7qGyinUJfGTu-uezerhsJ3v8,753
 python_appimage/utils/deps.py,sha256=wR7SdN9XiirHhicQYENoy9ckP84eUt980_xG4ZX7pGM,3024
-python_appimage/utils/docker.py,sha256=OC0kv-QEe9MWsza7e8N3C4kH4SDoVparE_OdITdLwFA,1389
+python_appimage/utils/docker.py,sha256=_68a72Fvtv7qXZK3CW15U1xITjSjzbcmKnuMDh5M9iQ,1601
 python_appimage/utils/fs.py,sha256=PYhv0AiS9-0lk1YkM9VBrkIKJbBOcz9hZlN_VWi4PWc,2079
-python_appimage/utils/log.py,sha256=BenSToCxQuXpXK9ZmUPLg5NhhJ_Bixrd99NdbdQhAPw,389
-python_appimage/utils/system.py,sha256=VxYRDXCAykETD61LFiaJ7OS91fkaAX2RR4sXu4_ykNQ,1621
+python_appimage/utils/log.py,sha256=6uAHlzkzA1ZtahilUj5akv92Ifql6PqkG8Bf5HIOkKY,667
+python_appimage/utils/manylinux.py,sha256=-CLV9-DfZ7A-Ba9vw086VRUpUNA5rP0qHkZPxvpUJ5M,386
+python_appimage/utils/system.py,sha256=3edpCXIEaP_QUf1zdcKM9SDG_Z9TUaYW9GLQbHmfAZU,1815
 python_appimage/utils/template.py,sha256=gHrxosfWb3FM9VTgxYvhigUO43fLlXzKNXsJWcvkWYY,898
 python_appimage/utils/tmp.py,sha256=d4jEuUOaCToXURMaBoyAHsBOWnJHcPHx44k9mOpCVkM,496
 python_appimage/utils/url.py,sha256=8DV81ZeDuTqfOzeBA1Ttj6WFLS-PrEnGYIYgALo_Fn0,988
 python_appimage/utils/version.py,sha256=rtE1IjlLFWGhHz2wU0vZMsw__76NSdBumD5Om8rJwu0,163
-python_appimage-1.2.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-python_appimage-1.2.5.dist-info/METADATA,sha256=82j7H7seYARfTakaSutJ5G2ojzp95gCZGk2RkxK7POE,3095
-python_appimage-1.2.5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-python_appimage-1.2.5.dist-info/entry_points.txt,sha256=0LVp6HaezXAMdgfEaLEPCBjilsPw99SbYC6_0TKvW0M,67
-python_appimage-1.2.5.dist-info/top_level.txt,sha256=gn_q7GGWej5oftHlH08RUQvAVVx8Eyy9RvZKgPApJCg,16
-python_appimage-1.2.5.dist-info/RECORD,,
+python_appimage-1.2.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+python_appimage-1.2.7.dist-info/METADATA,sha256=2Qk46zp5MksfIKwc4EbbutFnMloGHfShA2t8Es-_-SM,3095
+python_appimage-1.2.7.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+python_appimage-1.2.7.dist-info/entry_points.txt,sha256=0LVp6HaezXAMdgfEaLEPCBjilsPw99SbYC6_0TKvW0M,67
+python_appimage-1.2.7.dist-info/top_level.txt,sha256=gn_q7GGWej5oftHlH08RUQvAVVx8Eyy9RvZKgPApJCg,16
+python_appimage-1.2.7.dist-info/RECORD,,
```

