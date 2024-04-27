# Comparing `tmp/rofi_rbw-1.3.0.tar.gz` & `tmp/rofi_rbw-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofi_rbw-1.3.0.tar", max compression
+gzip compressed data, was "rofi_rbw-1.4.0.tar", max compression
```

## Comparing `rofi_rbw-1.3.0.tar` & `rofi_rbw-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,52 @@
--rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.3.0/LICENSE
--rw-r--r--   0        0        0     7586 2023-12-05 12:54:00.818815 rofi_rbw-1.3.0/README.md
--rw-r--r--   0        0        0     4261 2023-12-07 08:39:52.849036 rofi_rbw-1.3.0/docs/rofi-rbw.1
--rw-r--r--   0        0        0      749 2023-12-07 08:39:40.029144 rofi_rbw-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.3.0/src/rofi_rbw/__init__.py
--rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.3.0/src/rofi_rbw/__main__.py
--rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.3.0/src/rofi_rbw/abstractionhelper.py
--rw-r--r--   0        0        0     1182 2023-12-05 12:35:22.072945 rofi_rbw-1.3.0/src/rofi_rbw/cache.py
--rw-r--r--   0        0        0     3586 2022-12-22 13:31:28.675750 rofi_rbw-1.3.0/src/rofi_rbw/clipboarder.py
--rw-r--r--   0        0        0     1321 2023-12-05 12:41:31.219807 rofi_rbw-1.3.0/src/rofi_rbw/credentials.py
--rw-r--r--   0        0        0      516 2023-12-05 12:35:22.072945 rofi_rbw-1.3.0/src/rofi_rbw/entry.py
--rw-r--r--   0        0        0     1319 2023-11-07 16:48:39.890730 rofi_rbw-1.3.0/src/rofi_rbw/models.py
--rw-r--r--   0        0        0      641 2023-12-05 12:35:22.072945 rofi_rbw-1.3.0/src/rofi_rbw/paths.py
--rw-r--r--   0        0        0     2512 2023-12-05 12:41:31.229807 rofi_rbw-1.3.0/src/rofi_rbw/rbw.py
--rwxr-xr-x   0        0        0     8697 2023-12-05 12:38:44.173820 rofi_rbw-1.3.0/src/rofi_rbw/rofi_rbw.py
--rw-r--r--   0        0        0    10295 2023-12-05 12:41:31.293141 rofi_rbw-1.3.0/src/rofi_rbw/selector.py
--rw-r--r--   0        0        0     3098 2023-05-22 15:58:58.192103 rofi_rbw-1.3.0/src/rofi_rbw/typer.py
--rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 rofi_rbw-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-01-03 08:16:30.965044 rofi_rbw-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8498 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/README.md
+-rw-r--r--   0        0        0     4530 2024-04-27 13:48:57.528553 rofi_rbw-1.4.0/docs/rofi-rbw.1
+-rw-r--r--   0        0        0      748 2024-04-27 13:47:26.175425 rofi_rbw-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      206 2022-12-22 13:31:28.675750 rofi_rbw-1.4.0/src/rofi_rbw/__init__.py
+-rw-r--r--   0        0        0      105 2022-12-22 13:31:28.675750 rofi_rbw-1.4.0/src/rofi_rbw/__main__.py
+-rw-r--r--   0        0        0      197 2022-12-22 13:31:28.675750 rofi_rbw-1.4.0/src/rofi_rbw/abstractionhelper.py
+-rw-r--r--   0        0        0     4890 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/argument_parsing.py
+-rw-r--r--   0        0        0     1182 2023-12-05 12:35:22.072945 rofi_rbw-1.4.0/src/rofi_rbw/cache.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__init__.py
+-rw-r--r--   0        0        0      169 2024-03-06 08:45:01.276552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3213 2024-03-06 08:45:01.276552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/clipboarder.cpython-311.pyc
+-rw-r--r--   0        0        0     1384 2024-03-06 08:45:01.286552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/noop.cpython-311.pyc
+-rw-r--r--   0        0        0     1815 2024-03-06 08:45:01.286552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/wlclip.cpython-311.pyc
+-rw-r--r--   0        0        0     2441 2024-04-01 17:27:58.635344 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/xclip.cpython-311.pyc
+-rw-r--r--   0        0        0     2452 2024-03-06 08:45:01.286552 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/__pycache__/xsel.cpython-311.pyc
+-rw-r--r--   0        0        0     1194 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/clipboarder.py
+-rw-r--r--   0        0        0      440 2024-01-18 18:50:32.079752 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/noop.py
+-rw-r--r--   0        0        0      610 2024-01-18 18:50:37.116248 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/wlclip.py
+-rw-r--r--   0        0        0     1106 2024-03-24 12:11:07.281774 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/xclip.py
+-rw-r--r--   0        0        0     1210 2024-01-18 18:50:37.116248 rofi_rbw-1.4.0/src/rofi_rbw/clipboarder/xsel.py
+-rw-r--r--   0        0        0     1592 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/credentials.py
+-rw-r--r--   0        0        0      516 2023-12-05 12:35:22.072945 rofi_rbw-1.4.0/src/rofi_rbw/entry.py
+-rw-r--r--   0        0        0     1473 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/models.py
+-rw-r--r--   0        0        0      641 2023-12-05 12:35:22.072945 rofi_rbw-1.4.0/src/rofi_rbw/paths.py
+-rw-r--r--   0        0        0     2512 2023-12-05 12:41:31.229807 rofi_rbw-1.4.0/src/rofi_rbw/rbw.py
+-rwxr-xr-x   0        0        0     4465 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/rofi_rbw.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/selector/__init__.py
+-rw-r--r--   0        0        0      166 2024-03-06 08:45:01.279885 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5045 2024-03-06 08:45:01.283219 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/bemenu.cpython-311.pyc
+-rw-r--r--   0        0        0     8086 2024-03-06 08:45:01.283219 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/rofi.cpython-311.pyc
+-rw-r--r--   0        0        0     8762 2024-03-21 18:59:51.620840 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/selector.cpython-311.pyc
+-rw-r--r--   0        0        0     5083 2024-03-06 08:45:01.283219 rofi_rbw-1.4.0/src/rofi_rbw/selector/__pycache__/wofi.cpython-311.pyc
+-rw-r--r--   0        0        0     2506 2024-01-18 18:51:27.594529 rofi_rbw-1.4.0/src/rofi_rbw/selector/bemenu.py
+-rw-r--r--   0        0        0     4627 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/selector/rofi.py
+-rw-r--r--   0        0        0     3967 2024-03-21 18:01:21.271335 rofi_rbw-1.4.0/src/rofi_rbw/selector/selector.py
+-rw-r--r--   0        0        0     2523 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/selector/wofi.py
+-rw-r--r--   0        0        0        0 2024-01-18 18:50:19.810170 rofi_rbw-1.4.0/src/rofi_rbw/typer/__init__.py
+-rw-r--r--   0        0        0      163 2024-03-06 08:45:01.279885 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2171 2024-04-13 19:26:05.823685 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/dotool.cpython-311.pyc
+-rw-r--r--   0        0        0     1576 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/noop.cpython-311.pyc
+-rw-r--r--   0        0        0     3672 2024-04-01 17:27:58.628676 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/typer.cpython-311.pyc
+-rw-r--r--   0        0        0     2141 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/wtype.cpython-311.pyc
+-rw-r--r--   0        0        0     2524 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/xdotool.cpython-311.pyc
+-rw-r--r--   0        0        0     2262 2024-04-01 17:27:58.632010 rofi_rbw-1.4.0/src/rofi_rbw/typer/__pycache__/ydotool.cpython-311.pyc
+-rw-r--r--   0        0        0      838 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/dotool.py
+-rw-r--r--   0        0        0      502 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/noop.py
+-rw-r--r--   0        0        0     1313 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/typer.py
+-rw-r--r--   0        0        0      800 2024-04-19 16:55:25.616396 rofi_rbw-1.4.0/src/rofi_rbw/typer/wtype.py
+-rw-r--r--   0        0        0     1286 2024-04-19 16:55:25.619729 rofi_rbw-1.4.0/src/rofi_rbw/typer/xdotool.py
+-rw-r--r--   0        0        0      861 2024-04-19 16:55:25.619729 rofi_rbw-1.4.0/src/rofi_rbw/typer/ydotool.py
+-rw-r--r--   0        0        0     9240 1970-01-01 00:00:00.000000 rofi_rbw-1.4.0/PKG-INFO
```

### Comparing `rofi_rbw-1.3.0/LICENSE` & `rofi_rbw-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.3.0/README.md` & `rofi_rbw-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ## A rofi frontend for Bitwarden
 
 Based on the alternative [Bitwarden](https://bitwarden.com/) CLI [rbw](https://github.com/doy/rbw/) and inspired by [rofi-pass](https://github.com/carnager/rofi-pass), `rbw-rofi` is a simplistic password typer/copier using [rofi](https://github.com/davatorium/rofi) and [wofi](https://hg.sr.ht/~scoopta/wofi).
 
 ## Features
 - Autotype password or username (`Enter`/`Alt+3` and `Alt+2`, respectively)
 - Autotype username and password (with a `tab` character in between) with `Alt+1` (and copy TOTP to clipboard)
+- Configure autotyping either as a keybinding or by having a `_autotype` field in your credential
 - Copy username, password or TOTP to the clipboard (`Alt+u`, `Alt+p` and `Alt+t`, respectively)
 - Show an autotype menu with all fields
 
 ## Usage
 First, you need to configure `rbw`. See its documentation for that.
 Then, you can start `rofi-rbw`. It is *not* available as a rofi mode.
 
@@ -23,22 +24,25 @@
 | `--action`           | `-a`         | `type` (default), `copy`, `print`                             | Choose what `rofi-rbw` should do.                                                                                                                                                                                                                                           |
 | `--target`           | `-t`         | `username`, `password`, `notes`, `totp` (or any custom field) | Choose which components of the selected entry are interesting. Can be passed multiple times to type/copy/print several components. Default is `username` and `password`.                                                                                                    |
 | `--prompt`           | `-r`         | any string                                                    | Define the text of the prompt.                                                                                                                                                                                                                                              |
 | `--keybindings`      |              |                                                               | Define custom keybindings in the format `<shortcut>:<action>:<target>`, for example `Alt+x:copy:username`. Multiple keybindings can be concatenated with `,`; multiple targets for one shortcut can be concatenated with `:`. Note that `wofi` doesn't support keybindings. |
 | `--menu-keybindings` |              |                                                               | Define custom keybindings for the target menu in the format `<shortcut>:<action>`, similar to `--keybindings`. Note that `wofi` doesn't support keybindings.                                                                                                                |
 | `--no-cache`         |              |                                                               | Disable the automatic frecency cache. It contains sha1-hashes of the selected entries and how often they were used.                                                                                                                                                         |
 | `--clear-after`      |              | integer number >= 0 (default is `0`)                          | Limit the duration in seconds passwords stay in your clipboard (unless overwritten). When set to 0, passwords will be kept indefinitely.                                                                                                                                    |
+| `--typing-key-delay` |              | delay in milliseconds                                         | Set a delay between key presses when typing. `0` by default, but that may result in problems.                                                                                                                                                                               |
 | `--no-help`          |              |                                                               | Don't show the help message about the available shortcuts.                                                                                                                                                                                                                  |
 | `--no-folder`        |              |                                                               | Don't show the entry's folder in the list.                                                                                                                                                                                                                                  |
 | `--selector-args`    |              |                                                               | Define arguments that will be passed through to `rofi` or `wofi`.<br/>Please note that you need to specify it as `--selector-args="<args>"` or `--selector-args " <args>"` because of a [bug in argparse](https://github.com/python/cpython/issues/53580)                   |
 | `--selector`         |              | `rofi`, `wofi`                                                | Show the selection dialog with this application. Chosen automatically by default.                                                                                                                                                                                           |
 | `--clipboarder`      |              | `xsel`, `xclip`, `wl-copy`                                    | Access the clipboard with this application. Chosen automatically by default.                                                                                                                                                                                                |
 | `--typer`            |              | `xdotool`, `wtype`, `ydotool`, `dotool`                       | Type the characters using this application. Chosen automatically by default.                                                                                                                                                                                                |
+## Autotyping
+By default, `Alt+1` will type username and password, separated with a `tab` character. However, you can change this behavior by defining your own keybinding (if your selector supports this). For example, `Alt+1:type:username:enter:delay:password:enter` will type the username, `enter`, wait for a second and then type the password and `enter` again.
 
-
+This sequence can also be defined as a field `_autotype` on each credential.
 
 # Installation
 
 ## From distribution repositories
 [![Packaging status](https://repology.org/badge/vertical-allrepos/rofi-rbw.svg)](https://repology.org/project/rofi-rbw/versions)
 
 ## From PyPI
```

### Comparing `rofi_rbw-1.3.0/docs/rofi-rbw.1` & `rofi_rbw-1.4.0/docs/rofi-rbw.1`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,115 @@
-.\" Automatically generated by Pandoc 3.1.9
+.\" Automatically generated by Pandoc 3.1.12.2
 .\"
-.TH "ROFI-RBW" "1" "Dec 07, 2023" "Version 1.3.0" "Rofi Third-party Add-on Documentation"
+.TH "ROFI\-RBW" "1" "April 27, 2024" "Version 1.4.0" "Rofi Third\-party Add\-on Documentation"
 .SH NAME
-\f[B]rofi-rbw\f[R] - A rofi frontend for the alternative Bitwarden
+\f[B]rofi\-rbw\f[R] \- A rofi frontend for the alternative Bitwarden
 client rbw
 .SH SYNOPSIS
 .PP
-\f[B]rofi-rbw\f[R] [\f[B]-h\f[R]] [\f[B]--version\f[R]]
-[\f[B]--action\f[R] {\f[I]type\f[R],\f[I]copy\f[R],\f[I]print\f[R]}]
-[\f[B]--target\f[R]
+\f[B]rofi\-rbw\f[R] [\f[B]\-h\f[R]] [\f[B]\-\-version\f[R]]
+[\f[B]\-\-action\f[R] {\f[I]type\f[R],\f[I]copy\f[R],\f[I]print\f[R]}]
+[\f[B]\-\-target\f[R]
 {\f[I]username\f[R],\f[I]password\f[R],\f[I]totp\f[R],\f[I]OTHER\f[R]}]
-[\f[B]--prompt\f[R] \f[I]PROMPT\f[R]] [\f[B]--selector-args\f[R]
-\f[I]SELECTOR_ARGS\f[R]] [\f[B]--clipboarder\f[R] \f[I]CLIPBOARDER\f[R]]
-[\f[B]--typer\f[R] \f[I]TYPER\f[R]] [\f[B]--selector\f[R]
-\f[I]SELECTOR\f[R]] [\f[B]--clear-after\f[R] \f[I]NUMBER\f[R]]
-[\f[B]--no-help\f[R]] [\f[B]--no-folder\f[R]] [\f[B]--keybindings\f[R]
-\f[I]KEYBINDINGS\f[R]] [\f[B]--menu-keybindings\f[R]
-\f[I]MENU_KEYBINDINGS\f[R]]
+[\f[B]\-\-prompt\f[R] \f[I]PROMPT\f[R]] [\f[B]\-\-selector\-args\f[R]
+\f[I]SELECTOR_ARGS\f[R]] [\f[B]\-\-clipboarder\f[R]
+\f[I]CLIPBOARDER\f[R]] [\f[B]\-\-typer\f[R] \f[I]TYPER\f[R]]
+[\f[B]\-\-selector\f[R] \f[I]SELECTOR\f[R]] [\f[B]\-\-clear\-after\f[R]
+\f[I]NUMBER\f[R]] [\f[B]\-\-typing\-key\-delay\f[R] \f[I]NUMBER\f[R]]
+[\f[B]\-\-no\-help\f[R]] [\f[B]\-\-no\-folder\f[R]]
+[\f[B]\-\-keybindings\f[R] \f[I]KEYBINDINGS\f[R]]
+[\f[B]\-\-menu\-keybindings\f[R] \f[I]MENU_KEYBINDINGS\f[R]]
 .SH DESCRIPTION
 Type, copy or print your credentials from Bitwarden using rofi.
 .SH OPTIONS
 .TP
--h, --help
+\-h, \-\-help
 Prints brief usage information.
 .TP
---version
+\-\-version
 show program\[cq]s version number and exit
 .TP
---action, -a
+\-\-action, \-a
 Possible values: type, copy, print
 .RS
 .PP
 Choose what to do with the selected characters: Directly type them with
 the \[lq]Typer\[rq], copy them to the clipboard using the
 \[lq]Clipboarder\[rq], or \[lq]print\[rq] them on stdout
 .RE
 .TP
---target, -t
+\-\-target, \-t
 Possible values: username, password, totp, notes, \f[I]CUSTOM FIELD
 NAME\f[R]
 .RS
 .PP
 Choose which component of the selected entry to type/copy/print.
 Can be passed multiple times to use multiple targets.
 .RE
 .TP
---prompt \f[I]PROMPT\f[R], -r \f[I]PROMPT\f[R]
+\-\-prompt \f[I]PROMPT\f[R], \-r \f[I]PROMPT\f[R]
 Set the text for the prompt.
 .TP
---keybindings \f[I]KEYBINDINGS\f[R]
+\-\-keybindings \f[I]KEYBINDINGS\f[R]
 Format: ::.
 .RS
 .PP
 Define your own keybindings.
 Multiple keybindings can be concatenated with \f[CR],\f[R]; multiple
 targets for one shortcut can be concatenated with \f[CR]:\f[R].
 This feature is only available in supported \[dq]selectors\[dq].
 .RE
 .TP
---menu-keybindings \f[I]KEYBINDINGS\f[R]
+\-\-menu\-keybindings \f[I]KEYBINDINGS\f[R]
 Format: :.
 .RS
 .PP
 Define your own keybindings for the target menu.
 Multiple keybindings can be concatenated with \f[CR],\f[R].
 This feature is only available in supported \[dq]selectors\[dq].
 .RE
 .TP
---clear-after \f[I]SECONDS\f[R]
+\-\-clear\-after \f[I]SECONDS\f[R]
 Clear the password from the clipboard after \f[I]SECONDS\f[R] seconds.
 Set to \f[CR]0\f[R] to disable.
 .TP
---no-cache
+\-\-typing\-key\-delay \f[I]MILLISECONDS\f[R]
+Set a small delay between keypresses when typing.
+\f[CR]0\f[R] by default.
+.TP
+\-\-no\-cache
 Disable the automatic frecency cache.
-It contains sha1-hashes of the selected entries and how often they were
+It contains sha1\-hashes of the selected entries and how often they were
 used.
 .TP
---no-help
+\-\-no\-help
 Don\[cq]t show the help message about available keyboard shortcuts.
 .TP
---no-folder
+\-\-no\-folder
 Don\[cq]t show folders in the list of possible entries.
 .TP
---selector-args \f[I]SELECTOR-ARGS\f[R]
+\-\-selector\-args \f[I]SELECTOR\-ARGS\f[R]
 A string of arguments to give to the selector.
 .TP
---selector \f[I]SELECTOR\f[R]
+\-\-selector \f[I]SELECTOR\f[R]
 Possible values: rofi, wofi
 .RS
 .PP
 Choose the selector application manually.
 Usually \f[CR]rofi\f[R], but for Wayland, you may want \f[CR]wofi\f[R].
 .RE
 .TP
---clipboarder \f[I]CLIPBOARDER\f[R]
-Possible values: xsel, xclip, wl-copy
+\-\-clipboarder \f[I]CLIPBOARDER\f[R]
+Possible values: xsel, xclip, wl\-copy
 .RS
 .PP
 Choose the application to access the clipboard with manually.
 .RE
 .TP
---typer \f[I]TYPER\f[R]
+\-\-typer \f[I]TYPER\f[R]
 Possible values: xdotool, wtype, ydotool, dotool
 .RS
 .PP
 Choose the application to type with manually.
 .RE
 .SH DEFAULT KEYBINDINGS
 \f[I]enter\f[R] to use the default action
@@ -125,23 +130,23 @@
 \f[I]alt+2\f[R] to type the username
 .PP
 \f[I]alt+3\f[R] to type the password
 .PP
 Please note that wofi does not support keybindings other than
 \f[I]enter\f[R].
 .SH CONFIGURATION
-Args that start with \[lq]--\[rq] (eg.
---version) can also be set in a config file.
+Args that start with \[lq]\-\-\[rq] (eg.
+\-\-version) can also be set in a config file.
 .PP
 Config file syntax allows: key=value, flag=true, stuff=[a,b,c].
 If an arg is specified in more than one place, then commandline values
 override values from the config file.
 .SH FILES
 .TP
-\f[I]\[ti]/.cache/rofi-rbw.runcache\f[R]
+\f[I]\[ti]/.cache/rofi\-rbw.runcache\f[R]
 Saves the number pf times an entry has been used, so that they can be
 sorted first.
 Entries are hashed with sha1 so as not to leak any secrets.
 .SH WEBSITE
-https://github.com/fdw/rofi-rbw
+https://github.com/fdw/rofi\-rbw
 .SH AUTHORS
 Fabian Winter.
```

### Comparing `rofi_rbw-1.3.0/pyproject.toml` & `rofi_rbw-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rofi-rbw"
-version = "1.3.0"
+version = "1.4.0"
 description = "Rofi frontend for Bitwarden"
 authors = ["Fabian Winter <5821180+fdw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fdw/rofi-rbw"
 repository = "https://github.com/fdw/rofi-rbw"
 packages =[
@@ -18,16 +18,16 @@
 rofi-rbw = 'rofi_rbw.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ConfigArgParse = ">0.15,<2.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-isort = "^5.10.1"
+black = "^24.3.0"
+isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `rofi_rbw-1.3.0/src/rofi_rbw/cache.py` & `rofi_rbw-1.4.0/src/rofi_rbw/cache.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.3.0/src/rofi_rbw/credentials.py` & `rofi_rbw-1.4.0/src/rofi_rbw/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass, field
 from subprocess import run
 from typing import Dict, List, Optional, Union
 
 from .entry import Entry
-from .models import Target, Targets
+from .models import Target, Targets, TypeTarget
 
 
 @dataclass(frozen=True)
 class Credentials(Entry):
     password: Optional[str] = ""
     has_totp: bool = False
     notes: Optional[str] = ""
@@ -35,7 +35,14 @@
 
         command = ["rbw", "code", self.name]
         if self.username:
             command.extend([self.username])
         if self.folder:
             command.extend(["--folder", self.folder])
         return run(command, capture_output=True, encoding="utf-8").stdout.strip()
+
+    @property
+    def autotype_sequence(self) -> Union[List[TypeTarget], None]:
+        if "_autotype" not in self.further:
+            return None
+
+        return [TypeTarget(target_string) for target_string in self.further["_autotype"].strip().split(":")]
```

### Comparing `rofi_rbw-1.3.0/src/rofi_rbw/entry.py` & `rofi_rbw-1.4.0/src/rofi_rbw/entry.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.3.0/src/rofi_rbw/models.py` & `rofi_rbw-1.4.0/src/rofi_rbw/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,20 +43,30 @@
     def raw(self):
         return self.__value
 
     def __eq__(self, other):
         return self.__value == other.__value
 
 
+class TypeTarget(Target):
+    pass
+
+
 class Targets:
     USERNAME = Target("username")
     PASSWORD = Target("password")
     TOTP = Target("totp")
     NOTES = Target("notes")
     MENU = Target("menu")
 
 
+class TypeTargets:
+    DELAY = TypeTarget("delay")
+    ENTER = TypeTarget("enter")
+    TAB = TypeTarget("tab")
+
+
 @dataclass
 class Keybinding:
     shortcut: str
     action: Action
-    targets: Union[List[Target], None]
+    targets: Union[List[TypeTarget], None]
```

### Comparing `rofi_rbw-1.3.0/src/rofi_rbw/paths.py` & `rofi_rbw-1.4.0/src/rofi_rbw/paths.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.3.0/src/rofi_rbw/rbw.py` & `rofi_rbw-1.4.0/src/rofi_rbw/rbw.py`

 * *Files identical despite different names*

### Comparing `rofi_rbw-1.3.0/PKG-INFO` & `rofi_rbw-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofi-rbw
-Version: 1.3.0
+Version: 1.4.0
 Summary: Rofi frontend for Bitwarden
 Home-page: https://github.com/fdw/rofi-rbw
 License: MIT
 Author: Fabian Winter
 Author-email: 5821180+fdw@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,15 @@
 ## A rofi frontend for Bitwarden
 
 Based on the alternative [Bitwarden](https://bitwarden.com/) CLI [rbw](https://github.com/doy/rbw/) and inspired by [rofi-pass](https://github.com/carnager/rofi-pass), `rbw-rofi` is a simplistic password typer/copier using [rofi](https://github.com/davatorium/rofi) and [wofi](https://hg.sr.ht/~scoopta/wofi).
 
 ## Features
 - Autotype password or username (`Enter`/`Alt+3` and `Alt+2`, respectively)
 - Autotype username and password (with a `tab` character in between) with `Alt+1` (and copy TOTP to clipboard)
+- Configure autotyping either as a keybinding or by having a `_autotype` field in your credential
 - Copy username, password or TOTP to the clipboard (`Alt+u`, `Alt+p` and `Alt+t`, respectively)
 - Show an autotype menu with all fields
 
 ## Usage
 First, you need to configure `rbw`. See its documentation for that.
 Then, you can start `rofi-rbw`. It is *not* available as a rofi mode.
 
@@ -43,22 +44,25 @@
 | `--action`           | `-a`         | `type` (default), `copy`, `print`                             | Choose what `rofi-rbw` should do.                                                                                                                                                                                                                                           |
 | `--target`           | `-t`         | `username`, `password`, `notes`, `totp` (or any custom field) | Choose which components of the selected entry are interesting. Can be passed multiple times to type/copy/print several components. Default is `username` and `password`.                                                                                                    |
 | `--prompt`           | `-r`         | any string                                                    | Define the text of the prompt.                                                                                                                                                                                                                                              |
 | `--keybindings`      |              |                                                               | Define custom keybindings in the format `<shortcut>:<action>:<target>`, for example `Alt+x:copy:username`. Multiple keybindings can be concatenated with `,`; multiple targets for one shortcut can be concatenated with `:`. Note that `wofi` doesn't support keybindings. |
 | `--menu-keybindings` |              |                                                               | Define custom keybindings for the target menu in the format `<shortcut>:<action>`, similar to `--keybindings`. Note that `wofi` doesn't support keybindings.                                                                                                                |
 | `--no-cache`         |              |                                                               | Disable the automatic frecency cache. It contains sha1-hashes of the selected entries and how often they were used.                                                                                                                                                         |
 | `--clear-after`      |              | integer number >= 0 (default is `0`)                          | Limit the duration in seconds passwords stay in your clipboard (unless overwritten). When set to 0, passwords will be kept indefinitely.                                                                                                                                    |
+| `--typing-key-delay` |              | delay in milliseconds                                         | Set a delay between key presses when typing. `0` by default, but that may result in problems.                                                                                                                                                                               |
 | `--no-help`          |              |                                                               | Don't show the help message about the available shortcuts.                                                                                                                                                                                                                  |
 | `--no-folder`        |              |                                                               | Don't show the entry's folder in the list.                                                                                                                                                                                                                                  |
 | `--selector-args`    |              |                                                               | Define arguments that will be passed through to `rofi` or `wofi`.<br/>Please note that you need to specify it as `--selector-args="<args>"` or `--selector-args " <args>"` because of a [bug in argparse](https://github.com/python/cpython/issues/53580)                   |
 | `--selector`         |              | `rofi`, `wofi`                                                | Show the selection dialog with this application. Chosen automatically by default.                                                                                                                                                                                           |
 | `--clipboarder`      |              | `xsel`, `xclip`, `wl-copy`                                    | Access the clipboard with this application. Chosen automatically by default.                                                                                                                                                                                                |
 | `--typer`            |              | `xdotool`, `wtype`, `ydotool`, `dotool`                       | Type the characters using this application. Chosen automatically by default.                                                                                                                                                                                                |
+## Autotyping
+By default, `Alt+1` will type username and password, separated with a `tab` character. However, you can change this behavior by defining your own keybinding (if your selector supports this). For example, `Alt+1:type:username:enter:delay:password:enter` will type the username, `enter`, wait for a second and then type the password and `enter` again.
 
-
+This sequence can also be defined as a field `_autotype` on each credential.
 
 # Installation
 
 ## From distribution repositories
 [![Packaging status](https://repology.org/badge/vertical-allrepos/rofi-rbw.svg)](https://repology.org/project/rofi-rbw/versions)
 
 ## From PyPI
```

