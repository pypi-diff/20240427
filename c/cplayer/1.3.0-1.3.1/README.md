# Comparing `tmp/cplayer-1.3.0.tar.gz` & `tmp/cplayer-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cplayer-1.3.0.tar", max compression
+gzip compressed data, was "cplayer-1.3.1.tar", max compression
```

## Comparing `cplayer-1.3.0.tar` & `cplayer-1.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1063 2024-03-28 21:12:01.621521 cplayer-1.3.0/LICENSE
--rw-r--r--   0        0        0    10348 2024-03-30 22:56:06.078293 cplayer-1.3.0/README.md
--rw-r--r--   0        0        0       85 2024-03-30 23:52:14.474667 cplayer-1.3.0/cplayer/__init__.py
--rw-r--r--   0        0        0     4704 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/__main__.py
--rw-r--r--   0        0        0     2015 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/documentation/help.md
--rw-r--r--   0        0        0     1592 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/resources/config/default.yaml
--rw-r--r--   0        0        0      696 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/resources/styles/application.css
--rw-r--r--   0        0        0        0 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/__init__.py
--rw-r--r--   0        0        0     2661 2024-03-30 22:34:43.665398 cplayer-1.3.0/cplayer/src/components/file_explorer/__init__.py
--rw-r--r--   0        0        0      142 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/file_explorer/styles.css
--rw-r--r--   0        0        0     1226 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/hidden_widget/__init__.py
--rw-r--r--   0        0        0     2724 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/input_label/__init__.py
--rw-r--r--   0        0        0       87 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/input_label/styles.css
--rw-r--r--   0        0        0     1838 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/notification/__init__.py
--rw-r--r--   0        0        0       54 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/notification/styles.css
--rw-r--r--   0        0        0     5559 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/options_list/__init__.py
--rw-r--r--   0        0        0      145 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/options_list/styles.css
--rw-r--r--   0        0        0     2478 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/progress_bar/__init__.py
--rw-r--r--   0        0        0      146 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/progress_bar/styles.css
--rw-r--r--   0        0        0     1554 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/status_song/__init__.py
--rw-r--r--   0        0        0       50 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/status_song/styles.css
--rw-r--r--   0        0        0    12879 2024-03-30 18:35:33.279799 cplayer-1.3.0/cplayer/src/components/tracklist/__init__.py
--rw-r--r--   0        0        0      235 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/tracklist/styles.css
--rw-r--r--   0        0        0     2238 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/volume_bar/__init__.py
--rw-r--r--   0        0        0      143 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/components/volume_bar/styles.css
--rw-r--r--   0        0        0      228 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/elements/__init__.py
--rw-r--r--   0        0        0     4209 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/elements/config.py
--rw-r--r--   0        0        0     2221 2024-03-30 18:34:26.154239 cplayer-1.3.0/cplayer/src/elements/downloader.py
--rw-r--r--   0        0        0     1674 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/elements/playlist.py
--rw-r--r--   0        0        0        0 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/pages/__init__.py
--rw-r--r--   0        0        0      819 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/pages/base/__init__.py
--rw-r--r--   0        0        0       44 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/pages/base/styles.css
--rw-r--r--   0        0        0     1108 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/pages/help/__init__.py
--rw-r--r--   0        0        0      128 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/pages/help/styles.css
--rw-r--r--   0        0        0    25140 2024-03-30 22:35:49.894262 cplayer-1.3.0/cplayer/src/pages/home/__init__.py
--rw-r--r--   0        0        0       62 2024-03-28 21:12:01.624854 cplayer-1.3.0/cplayer/src/pages/home/styles.css
--rw-r--r--   0        0        0     1708 2024-03-31 00:11:33.519274 cplayer-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    11638 1970-01-01 00:00:00.000000 cplayer-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-26 02:03:51.400567 cplayer-1.3.1/LICENSE
+-rw-r--r--   0        0        0    10461 2024-04-27 14:23:16.363419 cplayer-1.3.1/README.md
+-rw-r--r--   0        0        0       85 2024-04-26 02:03:51.350567 cplayer-1.3.1/cplayer/__init__.py
+-rw-r--r--   0        0        0     4703 2024-04-27 03:08:32.620792 cplayer-1.3.1/cplayer/__main__.py
+-rw-r--r--   0        0        0     2015 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/documentation/help.md
+-rw-r--r--   0        0        0     1592 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/resources/config/default.yaml
+-rw-r--r--   0        0        0      696 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/resources/styles/application.css
+-rw-r--r--   0        0        0       19 2024-04-27 03:09:30.104127 cplayer-1.3.1/cplayer/src/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-27 03:05:32.414118 cplayer-1.3.1/cplayer/src/components/__init__.py
+-rw-r--r--   0        0        0     2776 2024-04-27 14:19:49.060078 cplayer-1.3.1/cplayer/src/components/file_explorer/__init__.py
+-rw-r--r--   0        0        0      142 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/file_explorer/styles.css
+-rw-r--r--   0        0        0     1293 2024-04-27 03:06:33.267454 cplayer-1.3.1/cplayer/src/components/hidden_widget/__init__.py
+-rw-r--r--   0        0        0     2797 2024-04-27 03:04:15.317449 cplayer-1.3.1/cplayer/src/components/input_label/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/input_label/styles.css
+-rw-r--r--   0        0        0     1911 2024-04-27 03:04:30.137449 cplayer-1.3.1/cplayer/src/components/notification/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/notification/styles.css
+-rw-r--r--   0        0        0     5633 2024-04-27 03:07:42.567456 cplayer-1.3.1/cplayer/src/components/options_list/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/options_list/styles.css
+-rw-r--r--   0        0        0     2551 2024-04-27 03:08:03.607457 cplayer-1.3.1/cplayer/src/components/progress_bar/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/progress_bar/styles.css
+-rw-r--r--   0        0        0     1626 2024-04-27 03:03:16.404114 cplayer-1.3.1/cplayer/src/components/status_song/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/status_song/styles.css
+-rw-r--r--   0        0        0    12933 2024-04-26 02:15:38.463925 cplayer-1.3.1/cplayer/src/components/tracklist/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/tracklist/styles.css
+-rw-r--r--   0        0        0     2309 2024-04-27 03:08:45.910792 cplayer-1.3.1/cplayer/src/components/volume_bar/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/volume_bar/styles.css
+-rw-r--r--   0        0        0      253 2024-04-27 03:05:47.750786 cplayer-1.3.1/cplayer/src/elements/__init__.py
+-rw-r--r--   0        0        0     4209 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/elements/config.py
+-rw-r--r--   0        0        0     2221 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/elements/downloader.py
+-rw-r--r--   0        0        0     1674 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/elements/playlist.py
+-rw-r--r--   0        0        0       21 2024-04-27 03:05:00.737450 cplayer-1.3.1/cplayer/src/pages/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-27 03:02:32.087445 cplayer-1.3.1/cplayer/src/pages/base/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/pages/base/styles.css
+-rw-r--r--   0        0        0     1133 2024-04-27 03:02:12.167445 cplayer-1.3.1/cplayer/src/pages/help/__init__.py
+-rw-r--r--   0        0        0      128 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/pages/help/styles.css
+-rw-r--r--   0        0        0    25311 2024-04-26 02:07:08.857241 cplayer-1.3.1/cplayer/src/pages/home/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-26 02:03:51.350567 cplayer-1.3.1/cplayer/src/pages/home/styles.css
+-rw-r--r--   0        0        0     1724 2024-04-27 02:49:25.994084 cplayer-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11751 1970-01-01 00:00:00.000000 cplayer-1.3.1/PKG-INFO
```

### Comparing `cplayer-1.3.0/LICENSE` & `cplayer-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/README.md` & `cplayer-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,24 +152,24 @@
 This project use [tox](https://tox.wiki/en/latest/) and [pytest](https://docs.pytest.org/) to run the library tests.
 
 #### Dependencies
 
 To use development tools you must install the poetry packages:
 
 ```bash
-poetry install
+poetry install --with dev
 ```
 
 #### Set up pre-commit
 
 After cloning the repository run the following command in the repository root, this ensures that library tests are run
 before each commit into the repository to maintain the quality of the project:
 
 ```bash
-poetry run pre-commit install
+git config core.hooksPath .githooks
 ```
 
 #### Basic configuration
 
 Install development python requirements
 
 ```bash
@@ -180,28 +180,28 @@
 
 Simply run "`tox`" to execute all the library tests.
 
 ```bash
 poetry run tox
 ```
 
-to run the tests for a particular Python version, you can do:
+To run the tests for a particular Python version, you can do:
 
 
 ```bash
 poetry run tox -e py38
 ```
 
-to clean the test environment:
+To clean the test environment:
 
 ```bash
 poetry run tox -e clean
 ```
 
-to publish the pypi package:
+To publish the pypi package:
 
 ```bash
 poetry run tox -e publish
 ```
 
 #### Advanced configuration
 
@@ -308,7 +308,10 @@
     * `feat`: Adds compatibility to python 3.10 and 3.12.
     * `fix`: Fixes an error in the size of the layouts.
     * `refactor`: Adds poetry as a dependency and packaging manager.
     * `refactor`: General refactoring on static code analysis tools.
 * 1.3.0:
     * `feat`: Adds support for wav song files.
     * `documentation`: Refactor developers documentation.
+* 1.3.1:
+    * `fix`: Adds file explorer quit action.
+    * `refactor`: Update textual package.
```

### Comparing `cplayer-1.3.0/cplayer/__main__.py` & `cplayer-1.3.1/cplayer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,14 @@
 @click.version_option(version=__version__)
 def main(path: Path | None, url: str | None) -> None:
     """Command Line Python player CLI.
 
     This command line tool plays music files from a specified directory or last used playlist.
 
     Examples:
-
         - Play music from the current directory or the last used playlist if it exists:
 
           $ cplayer
 
         - Play music from a specific directory:
 
           $ cplayer --path /path/to/music_directory
```

### Comparing `cplayer-1.3.0/cplayer/documentation/help.md` & `cplayer-1.3.1/cplayer/documentation/help.md`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/cplayer/resources/config/default.yaml` & `cplayer-1.3.1/cplayer/resources/config/default.yaml`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/cplayer/resources/styles/application.css` & `cplayer-1.3.1/cplayer/resources/styles/application.css`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/cplayer/src/components/file_explorer/__init__.py` & `cplayer-1.3.1/cplayer/src/components/file_explorer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,52 @@
+"""Module that contains the implementation of a file explorer widget."""
+
 import logging
 from collections.abc import Callable, Iterable
 from pathlib import Path
 from typing import ClassVar
 
 from textual.binding import Binding, BindingType
-from textual.widget import Widget
 from textual.widgets import DirectoryTree
 
 from cplayer.src.components.hidden_widget import HiddenWidget
 
 
 class FileExplorerWidget(DirectoryTree, HiddenWidget):  # pylint: disable=too-many-ancestors
     """File explorer widget."""
 
     DEFAULT_CSS = Path(__file__).parent.joinpath('styles.css').read_text(encoding='UTF-8')
 
     BINDINGS: ClassVar[list[BindingType]] = [
+        Binding('escape', 'quit', 'Quit', show=True),
         Binding('enter', 'select', 'Select', show=True),
         Binding('right', 'open', 'Open', show=True),
     ]
 
     def __init__(  # noqa: PLR0913
         self,
-        *children: Widget,
         path: str | Path,
         on_select: Callable[[Path], None],
+        on_quit: Callable[[], None],
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
-        disabled: bool = False,
-        start_hidden: bool = True,
+        disabled: bool = False,  # noqa: FBT002
     ) -> None:
         """Initializes the Widget object.
 
         :param on_select: A function to be called when a file or directory is selected.
         :param *args: Variable length argument list.
         :param **kwargs: Arbitrary keyword arguments.
         """
         DirectoryTree.__init__(self, path=path, name=name, id=id, classes=classes, disabled=disabled)
-        HiddenWidget.__init__(
-            self, *children, name=name, id=id, classes=classes, disabled=disabled, start_hidden=start_hidden
-        )
 
         self.default_path = path
         self.on_select = on_select
+        self.on_quit = on_quit
 
     def on_mount(self) -> None:
         """Handles events on the mounting of the file explorer."""
         super().on_mount()
 
         self.path = self.default_path
 
@@ -64,14 +63,19 @@
             if (not path.name.startswith('.')) and (path.is_dir() or path.suffix in ('.mp3', '.wav'))
         ]
 
     def action_open(self) -> None:
         """Selects the selected cursor."""
         super().action_select_cursor()
 
+    def action_quit(self) -> None:
+        """Perform the action associated with quitting the widget."""
+        self.hide()
+        self.on_quit()
+
     def action_select(self) -> None:
         """Runs the `self.on_select` callback with the selected path."""
         line = self._tree_lines[self.cursor_line]
         node = line.path[-1]
 
         if node.data:
             self.on_select(node.data.path)
```

### Comparing `cplayer-1.3.0/cplayer/src/components/hidden_widget/__init__.py` & `cplayer-1.3.1/cplayer/src/components/hidden_widget/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of a hidden widget."""
+
 from textual.widget import Widget
 
 
 class HiddenWidget(Widget):
     """Hidden widget representation."""
 
     def __init__(  # noqa: PLR0913
```

### Comparing `cplayer-1.3.0/cplayer/src/components/input_label/__init__.py` & `cplayer-1.3.1/cplayer/src/components/input_label/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of an input label widget."""
+
 from collections.abc import Callable, Coroutine
 from pathlib import Path
 from typing import ClassVar
 
 from textual.app import ComposeResult
 from textual.binding import BindingType
 from textual.widget import Widget
```

### Comparing `cplayer-1.3.0/cplayer/src/components/notification/__init__.py` & `cplayer-1.3.1/cplayer/src/components/notification/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of a notification widget."""
+
 from pathlib import Path
 
 from textual.app import ComposeResult
 from textual.widget import Widget
 from textual.widgets import Label
 
 from cplayer.src.components.hidden_widget import HiddenWidget
```

### Comparing `cplayer-1.3.0/cplayer/src/components/options_list/__init__.py` & `cplayer-1.3.1/cplayer/src/components/options_list/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of an options list widget."""
+
 from collections.abc import Callable
 from pathlib import Path
 from typing import Any, ClassVar
 
 from textual.app import ComposeResult
 from textual.binding import Binding, BindingType
 from textual.containers import Middle, VerticalScroll
```

### Comparing `cplayer-1.3.0/cplayer/src/components/progress_bar/__init__.py` & `cplayer-1.3.1/cplayer/src/components/progress_bar/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of a progress bar widget."""
+
 from enum import Enum
 from pathlib import Path
 from typing import cast
 
 from textual.app import ComposeResult
 from textual.containers import Horizontal
 from textual.widget import Widget
```

### Comparing `cplayer-1.3.0/cplayer/src/components/status_song/__init__.py` & `cplayer-1.3.1/cplayer/src/components/status_song/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of a status song widget."""
+
 from pathlib import Path
 
 from textual.app import ComposeResult
 from textual.containers import Horizontal
 from textual.widget import Widget
 from textual.widgets import Label
```

### Comparing `cplayer-1.3.0/cplayer/src/components/tracklist/__init__.py` & `cplayer-1.3.1/cplayer/src/components/tracklist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Package representing a playlist widget."""
+
 import random
 from collections.abc import Callable
 from difflib import SequenceMatcher
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar
 
@@ -169,20 +171,15 @@
     def compose(self) -> ComposeResult:
         """Composes the widget.
 
         :returns: The widget object representing the composed widget.
         """
         yield self.content
 
-    def refresh(
-        self,
-        *regions: Region,
-        repaint: bool = True,
-        layout: bool = False,
-    ) -> Self:
+    def refresh(self, *regions: Region, repaint: bool = True, layout: bool = False, recompose: bool = False) -> Self:
         """Refresh the tracklist widget.
 
         :param *args: Variable length argument list.
         :param **kwargs: Arbitrary keyword arguments.
         """
         new_length = self.console.size.height - self._fixed_size
         if new_length > self.length:
@@ -191,15 +188,15 @@
             self.length = new_length
             self.index += delta
             self.draw()
 
             if self.current_song:
                 self.select(self.current_song.path)
 
-        return super().refresh(*regions, repaint=repaint, layout=layout)
+        return super().refresh(*regions, repaint=repaint, layout=layout, recompose=recompose)
 
     def clean(self) -> None:
         """Cleans seleted song in the tracklist."""
         self.content.update('No data.')
 
     def go_to(self, position: int) -> None:
         """Moves the highlighted position to a specified position.
```

### Comparing `cplayer-1.3.0/cplayer/src/components/volume_bar/__init__.py` & `cplayer-1.3.1/cplayer/src/components/volume_bar/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of a volume bar widget."""
+
 from pathlib import Path
 
 from textual._types import UnusedParameter
 from textual.app import ComposeResult
 from textual.containers import Horizontal
 from textual.widget import Widget
 from textual.widgets import Label, ProgressBar
```

### Comparing `cplayer-1.3.0/cplayer/src/elements/config.py` & `cplayer-1.3.1/cplayer/src/elements/config.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/cplayer/src/elements/downloader.py` & `cplayer-1.3.1/cplayer/src/elements/downloader.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/cplayer/src/elements/playlist.py` & `cplayer-1.3.1/cplayer/src/elements/playlist.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.0/cplayer/src/pages/base/__init__.py` & `cplayer-1.3.1/cplayer/src/pages/base/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module that contains the implementation of a base class for all pages in the application."""
+
 from collections.abc import Callable
 from pathlib import Path
 
 from cplayer.src.components.hidden_widget import HiddenWidget
 
 
 class PageBase(HiddenWidget):
```

### Comparing `cplayer-1.3.0/cplayer/src/pages/help/__init__.py` & `cplayer-1.3.1/cplayer/src/pages/help/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Help Page Module."""
+
 from pathlib import Path
 
 from textual.app import ComposeResult
 from textual.widgets import MarkdownViewer
 
 from cplayer.src.pages.base import PageBase
```

### Comparing `cplayer-1.3.0/cplayer/src/pages/home/__init__.py` & `cplayer-1.3.1/cplayer/src/pages/home/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,19 @@
             on_change_position=self.on_change_position,
             order=next(
                 (order for order in PlaylistOrder if order.value == CONFIG.data.general.playlist.order),
                 PlaylistOrder.ASCENDING,
             ),
             fixed_size=11 if CONFIG.data.appearance.style.footer else 8,
         )
-        self.file_explorer_widget = FileExplorerWidget(path=Path('~').expanduser(), on_select=self.on_select_path)
+        self.file_explorer_widget = FileExplorerWidget(
+            path=Path('~').expanduser(),
+            on_select=self.on_select_path,
+            on_quit=lambda: setattr(self.tracklist_widget, 'display', True),
+        )
 
         self.notification_widget = NotificationWidget('')
 
         self.select_playlist_widget = OptionsListWidget('Select a playlist:', self.on_quit, self.select_playlist)
         self.select_order_widget = OptionsListWidget('Select an order:', self.on_quit, self.select_order)
 
         self.goto_position_widget = InputLabelWidget(
@@ -304,14 +308,17 @@
         self.file_explorer_widget.show()
 
     def on_select_path(self, path: Path) -> None:
         """Handles the selection of a file path.
 
         :param path: The selected file path.
         """
+        if path.is_file():
+            path = path.parent
+
         self._load_directory(path)
 
     def action_load_directory(self) -> None:
         """Opens the input widget to load a directory path."""
         self.status_song_widget.hide()
         self.directory_widget.show()
```

### Comparing `cplayer-1.3.0/pyproject.toml` & `cplayer-1.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cplayer"
-version = "1.3.0"
+version = "1.3.1"
 description = "Minimalist song player implemented with Python"
 authors = ["Erik Ccanto <ccanto.erik@gmail.com>"]
 repository = "https://github.com/eccanto/cplayer"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "cplayer" },
@@ -41,28 +41,29 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 numpy = "^1.26.4"
 pygame = "^2.5.2"
 pydub = "^0.25.1"
-textual = "^0.52.1"
+textual = "^0.58.0"
 pyyaml = "^6.0.1"
 dotmap = "^1.3.30"
 yt-dlp = "^2024.3.10"
 tox = "^4.14.1"
 pip = "^24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 twine = "^5.0.0"
 assertpy = "^1.1"
 pre-commit = "^3.6.2"
 prospector = {extras = ["with-mypy", "with-pyroma"], version = "^1.10.3"}
 types-pyyaml = "^6.0.12.20240311"
+ruff = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `cplayer-1.3.0/PKG-INFO` & `cplayer-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cplayer
-Version: 1.3.0
+Version: 1.3.1
 Summary: Minimalist song player implemented with Python
 Home-page: https://github.com/eccanto/cplayer
 License: MIT
 Keywords: music,songs player,command line
 Author: Erik Ccanto
 Author-email: ccanto.erik@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -22,15 +22,15 @@
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: dotmap (>=1.3.30,<2.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pip (>=24.0,<25.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pygame (>=2.5.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: textual (>=0.52.1,<0.53.0)
+Requires-Dist: textual (>=0.58.0,<0.59.0)
 Requires-Dist: tox (>=4.14.1,<5.0.0)
 Requires-Dist: yt-dlp (>=2024.3.10,<2025.0.0)
 Project-URL: Repository, https://github.com/eccanto/cplayer
 Description-Content-Type: text/markdown
 
 # CPlayer
 
@@ -186,24 +186,24 @@
 This project use [tox](https://tox.wiki/en/latest/) and [pytest](https://docs.pytest.org/) to run the library tests.
 
 #### Dependencies
 
 To use development tools you must install the poetry packages:
 
 ```bash
-poetry install
+poetry install --with dev
 ```
 
 #### Set up pre-commit
 
 After cloning the repository run the following command in the repository root, this ensures that library tests are run
 before each commit into the repository to maintain the quality of the project:
 
 ```bash
-poetry run pre-commit install
+git config core.hooksPath .githooks
 ```
 
 #### Basic configuration
 
 Install development python requirements
 
 ```bash
@@ -214,28 +214,28 @@
 
 Simply run "`tox`" to execute all the library tests.
 
 ```bash
 poetry run tox
 ```
 
-to run the tests for a particular Python version, you can do:
+To run the tests for a particular Python version, you can do:
 
 
 ```bash
 poetry run tox -e py38
 ```
 
-to clean the test environment:
+To clean the test environment:
 
 ```bash
 poetry run tox -e clean
 ```
 
-to publish the pypi package:
+To publish the pypi package:
 
 ```bash
 poetry run tox -e publish
 ```
 
 #### Advanced configuration
 
@@ -342,8 +342,11 @@
     * `feat`: Adds compatibility to python 3.10 and 3.12.
     * `fix`: Fixes an error in the size of the layouts.
     * `refactor`: Adds poetry as a dependency and packaging manager.
     * `refactor`: General refactoring on static code analysis tools.
 * 1.3.0:
     * `feat`: Adds support for wav song files.
     * `documentation`: Refactor developers documentation.
+* 1.3.1:
+    * `fix`: Adds file explorer quit action.
+    * `refactor`: Update textual package.
```

