# Comparing `tmp/brplotviz-0.2.3.tar.gz` & `tmp/brplotviz-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brplotviz-0.2.3.tar", last modified: Sat Apr 13 11:40:54 2024, max compression
+gzip compressed data, was "brplotviz-0.3.tar", last modified: Sat Apr 27 14:19:45 2024, max compression
```

## Comparing `brplotviz-0.2.3.tar` & `brplotviz-0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/
--rwxr-xr-x   0 bertram   (1000) bertram   (1000)    35081 2022-08-05 18:57:03.000000 brplotviz-0.2.3/LICENSE
--rw-r--r--   0 bertram   (1000) bertram   (1000)    44928 2024-04-13 11:40:54.279367 brplotviz-0.2.3/PKG-INFO
--rwxr-xr-x   0 bertram   (1000) bertram   (1000)     3345 2024-03-30 13:05:24.000000 brplotviz-0.2.3/README.md
--rw-r--r--   0 bertram   (1000) bertram   (1000)     1194 2024-04-13 11:36:40.000000 brplotviz-0.2.3/pyproject.toml
--rw-r--r--   0 bertram   (1000) bertram   (1000)       38 2024-04-13 11:40:54.279367 brplotviz-0.2.3/setup.cfg
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/brplotviz/
--rw-r--r--   0 bertram   (1000) bertram   (1000)      182 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/__init__.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)    20923 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/plot.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)     1578 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/styleselect.py
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/brplotviz/table/
--rw-r--r--   0 bertram   (1000) bertram   (1000)    22137 2024-04-10 18:41:11.000000 brplotviz-0.2.3/src/brplotviz/table/__init__.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)     7410 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/table/engines.py
--rw-r--r--   0 bertram   (1000) bertram   (1000)     1233 2024-03-17 19:47:01.000000 brplotviz-0.2.3/src/brplotviz/table/rules.py
-drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-13 11:40:54.279367 brplotviz-0.2.3/src/brplotviz.egg-info/
--rw-r--r--   0 bertram   (1000) bertram   (1000)    44928 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/PKG-INFO
--rw-r--r--   0 bertram   (1000) bertram   (1000)      385 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/SOURCES.txt
--rw-r--r--   0 bertram   (1000) bertram   (1000)        1 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/dependency_links.txt
--rw-r--r--   0 bertram   (1000) bertram   (1000)       24 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/requires.txt
--rw-r--r--   0 bertram   (1000) bertram   (1000)       10 2024-04-13 11:40:54.000000 brplotviz-0.2.3/src/brplotviz.egg-info/top_level.txt
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-27 14:19:45.527130 brplotviz-0.3/
+-rwxr-xr-x   0 bertram   (1000) bertram   (1000)    35081 2022-08-05 18:57:03.000000 brplotviz-0.3/LICENSE
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    50622 2024-04-27 14:19:45.527130 brplotviz-0.3/PKG-INFO
+-rwxr-xr-x   0 bertram   (1000) bertram   (1000)     9000 2024-04-27 13:29:46.000000 brplotviz-0.3/README.md
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     1225 2024-04-27 14:08:10.000000 brplotviz-0.3/pyproject.toml
+-rw-r--r--   0 bertram   (1000) bertram   (1000)       38 2024-04-27 14:19:45.527130 brplotviz-0.3/setup.cfg
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-27 14:19:45.523130 brplotviz-0.3/src/
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-27 14:19:45.527130 brplotviz-0.3/src/brplotviz/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)      170 2024-04-27 12:22:42.000000 brplotviz-0.3/src/brplotviz/__init__.py
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-27 14:19:45.527130 brplotviz-0.3/src/brplotviz/plot/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    20876 2024-04-27 14:12:49.000000 brplotviz-0.3/src/brplotviz/plot/__init__.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     1517 2024-04-27 12:23:24.000000 brplotviz-0.3/src/brplotviz/plot/styleselect.py
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-27 14:19:45.527130 brplotviz-0.3/src/brplotviz/table/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    24100 2024-04-27 12:21:42.000000 brplotviz-0.3/src/brplotviz/table/__init__.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     1769 2024-04-24 22:01:41.000000 brplotviz-0.3/src/brplotviz/table/rules.py
+-rw-r--r--   0 bertram   (1000) bertram   (1000)     7803 2024-04-27 14:14:57.000000 brplotviz-0.3/src/brplotviz/table/styles.py
+drwxr-xr-x   0 bertram   (1000) bertram   (1000)        0 2024-04-27 14:19:45.527130 brplotviz-0.3/src/brplotviz.egg-info/
+-rw-r--r--   0 bertram   (1000) bertram   (1000)    50622 2024-04-27 14:19:45.000000 brplotviz-0.3/src/brplotviz.egg-info/PKG-INFO
+-rw-r--r--   0 bertram   (1000) bertram   (1000)      398 2024-04-27 14:19:45.000000 brplotviz-0.3/src/brplotviz.egg-info/SOURCES.txt
+-rw-r--r--   0 bertram   (1000) bertram   (1000)        1 2024-04-27 14:19:45.000000 brplotviz-0.3/src/brplotviz.egg-info/dependency_links.txt
+-rw-r--r--   0 bertram   (1000) bertram   (1000)       24 2024-04-27 14:19:45.000000 brplotviz-0.3/src/brplotviz.egg-info/requires.txt
+-rw-r--r--   0 bertram   (1000) bertram   (1000)       10 2024-04-27 14:19:45.000000 brplotviz-0.3/src/brplotviz.egg-info/top_level.txt
```

### Comparing `brplotviz-0.2.3/LICENSE` & `brplotviz-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brplotviz-0.2.3/PKG-INFO` & `brplotviz-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: brplotviz
-Version: 0.2.3
-Summary: Plot utilities for outputting plots and tables nicely formatted
+Version: 0.3
+Summary: Utilities for nicely formatted tables and plots
 Author-email: Bertram Richter <bertram.richter@tu-dresden.de>
 Maintainer-email: Bertram Richter <bertram.richter@tu-dresden.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -678,123 +678,347 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/bertramrichter/brplotviz
 Project-URL: Bug Reports, https://github.com/bertramrichter/brplotviz/issues
 Project-URL: Source, https://github.com/bertramrichter/brplotviz
-Keywords: plot,table,output
+Keywords: plot,table,pretty-print
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5.0
 Requires-Dist: numpy
 
-`brplotviz` are plot utilities for outputting plots using `matplotlib` and nicely formatted tables according to the personal taste of Bertram Richter.
+`brplotviz` – utilities for nicely formatted tables and plots
+
+# Installation and Building documentation
+
+Install this package via `pip install -U brplotviz`.
+To build the documentation, download the source code and unpack it.
+Then, run `doxygen` in `brplotviz`'s root directory (this one).
+How to install `doxygen`, see on their website ([doxygen.nl](https://doxygen.nl)).
+The documentation will be assing it to the directory `./Documentation`
 
 # Getting started
-This package provides functions to simplify the output of nicely fomatted graphs.
-The main focus is to enable consistent graphical style suited for printing.
+
+`brplotviz` consists of two packages, `table` and `plot`.
+
+## Table
+
+`brplotviz.plot.table` provides functions to format and output tabular data.
+This tabular data is expected to be a sequence of sequences (list of lists ect.).
+When a row (or column) is shorter than the others the missing cells are added as empty ones.
+Multi-line cells (containing newline characters) are supported,
+additional lines are inserted in the output plain text table a required.
+
+### Styles
+
+`brplotviz.table` comes with a few table styles.
+To showcase the different styles, the script is used, where only the
+`<style>` is replaced with the following options.
+
+Some finer, advanced tuning of the style can be done with the `style_kwargs` dictionary.
+For example, padding of the cells on the left or right side is possible.
+
+```py
+table_data = [
+	["a",123.456, 12],
+	["bc\nde", 23.34, 345],
+	["and f", 45.],
+	]
+
+table.print_table(
+	table=table_data,
+	style=<style>,
+	)
+```
+
+`"csv"` is a simple character-separated value style.
+The separator character is configurable, but defaults to the comma (`","`).
+
+```
+a    ,123.456,12 
+bc   ,23.34  ,345
+de   ,       ,   
+and f,45.0   ,   
+```
+
+`"tsv"` is a special case of `csv` with tab (`"\t"`) as separator charater.
+
+```
+a    	123.456	12 
+bc   	23.34  	345
+de   	       	   
+and f	45.0   	   
+```
+
+`"latex"`
+A table using the LaTeX markup with `booktabs` rules.
+This only sets the content that goes into the body of a `tabular` environment.
+
+```
+\toprule
+a    &123.456&12 \\
+\midrule
+bc   &23.34  &345\\
+de   &       &   \\
+and f&45.0   &   \\
+\bottomrule
+```
+
+A complete LaTeX environment is output the wrapper function `brplotviz.table.print_table_LaTeX()`.
+This function accepts the same (and some more) arguments than `brplotviz.table.print_table()`
+
+```py
+brplotviz.table.print_table_LaTeX(
+	table=table,
+	caption="This is the caption",
+	LaTeX_label="example",
+	)
+```
+
+The result is the following LaTeX code.
+Note, that `brplotviz` will try to fill in the column alignment based on `align`.
+TO overwrite the default, use the argument `LaTeX_format`.
+`LaTeX_format` works analougously to `align`.
+
+```
+\begin{table}[!htbp]
+\centering
+\caption{This is the caption}
+\label{tab:example}
+\begin{tabular}{@{}
+*{3}{l}
+@{}}
+\toprule
+a    &123.456&12 \\
+\midrule
+bc   &23.34  &345\\
+de   &       &   \\
+and f&45.0   &   \\
+\bottomrule
+\end{tabular}
+\end{table}
+```
+
+"markdown"`outputs a Markdown table.
+
+```
+|a    |123.456|12  |
+|:----|:------|:---|
+|bc   |23.34  |345 |
+|de   |       |    |
+|and f|45.0   |    |
+```
+
+`"test"` is for testing purposes.
+
+```
+---TopRule---
+^> a     <||> 123.456 <|> 12  <$
+---HeadRule---
+^> bc    <||> 23.34   <|> 345 <$
+---NoRule---
+^> de    <||>         <|>     <$
+---MidRule---
+^> and f <||> 45.0    <|>     <$
+---BotRule---
+```
+
+Custom styles are possible by sub-classing `brplotviz.tables.styles.Style`.
+
+### Headers
+
+`brplotviz.table` provides the option to add headers, to both columns and rows.
+The `example_table`, that we plotted could be only the body of the table.
+
+```py
+head_row = ["Col 1", "Col 2", "Col 3"]
+head_col = ["Row 1", "Row 2", "Row 3"]
+top_left = "Top left"
+align = ["l", "c", "r", "r"]
+
+table.print_table(
+	table=table_data,
+	style="markdown",
+	head_col=head_col,
+	head_row=head_row,
+	top_left=top_left,
+	)
+```
+
+Note, that both the header row `head_row` and header column `head_col`
+can be set independently of each other.
+
+```
+|Top left|Col 1|Col 2  |Col 3|
+|:-------|:----|:------|:----|
+|Row 1   |a    |123.456|12   |
+|Row 2   |bc   |23.34  |345  |
+|        |de   |       |     |
+|Row 3   |and f|45.0   |     |
+```
+
+Table rows are numbered automatically when setting `head_col="enumerate"`.
+The numbering starts after the header row.
+Note, that rows with multiline cells are taken into account.
+
+```
+|Top left|Col 1|Col 2  |Col 3|
+|:-------|:----|:------|:----|
+|1       |a    |123.456|12   |
+|2       |bc   |23.34  |345  |
+|        |de   |       |     |
+|3       |and f|45.0   |     |
+```
+
+### Formatting
+
+The formatting of the table's cells can be set table-global, column-wise or for each cell individually.
+If the `formatter` is a string, this formatter is applied to all cells of the table.
+If the `formatter` is a list of strings, the formatting is applied column-wise (without the `head_col`).
+If the `formatter` is a list of list strings, the formatting is applied for each cell individually.
+The `formatter` is expected in the [Format Specification Mini-Language](https://docs.python.org/3/library/string.html#formatspec).
+Here, it is shown for a column-wise formatting:
+
+```py
+table.print_table(
+	table=table_data,
+	style="markdown",
+	formatter=["", ":.2f", ":.1f"],
+	)
+```
+
+```
+|Top left|Col 1|Col 2 |Col 3|
+|:-------|:----|:-----|:----|
+|1       |a    |123.46|12.0 |
+|2       |bc   |23.34 |345.0|
+|        |de   |      |     |
+|3       |and f|45.00 |     |
+```
+
+### Alignment
+
+Columns are alined by adding whitespace to make all cells in a column to the same width.
+By default, all cells are printed left-aligned.
+Similar to the formatting, the alignment can be set for all columns or for each column separately.
+Alignment can be turned off by setting `align=None`.
+
+```py
+table.print_table(
+	table=table_data,
+	style="markdown",
+	align=["l", "c", "r", "r"],
+	)
+```
+
+```
+|Top left|Col 1| Col 2 |Col 3|
+|:-------|:---:|------:|----:|
+|1       |  a  |123.456|   12|
+|2       | bc  |  23.34|  345|
+|        | de  |       |     |
+|3       |and f|   45.0|     |
+```
+
+
+### Rules
+
+The horizontal lines in the table ar ecalled rules.
+To add an extra rule include a `brplotviz.table.rules.ExtraRule` in the `table`.
+Note, that not all styles support `ExtraLines`.
+The rule separating the header column from the body can be suppressed by `omit_head_rule=True`.
+
+### Additional options for table output
+
+To transpose the `table` (switch columns with rows), use `transpose=True`.
+Note, that this will not switch `head_col` and `head_row`.
+
+With `replacement`, a dictionary can be passed to replace cell content.
+If a cell's content is found in the replacement`'s keys, the content is replaced with the associated value.
+Note, that the replacement takes place after formatting.
+
+By default `brplotviz.table.print_table()`, prints the typeset table and returns nothing (`None`).
+To return the lines, set `return_lines=True`.
+Set `show=False` to turn off the printing.
+
+## Plot
+
+`brplotviz.plot` provides functions to simplify the output of nicely formatted graphs.
+The focus is on a graphical style suited for printing.
 Thus, a monochrome (black-white) style is used.
 
 Let's start plotting.
 First, we need some data:
 
-```
+```py
 import numpy as np
 import brplotviz
 x_list = np.linspace(0, 2, 17)
 y_list_sin = np.sin(x_list)
 y_list_cos = np.cos(x_list)
 x_table = [x_list, x_list]
 y_table = [y_list_sin, y_list_cos]
 record_names = ["sine", "cosine"]
 ```
 
 Plotting a single line-graph and a scatter plot is as simple as:
+Each one is shown on separately.
 
-```
+```py
 brplotviz.plot.single_line(x_list, y_list_sin)
 brplotviz.plot.single_scatter(x_list, y_list_sin)
 ```
 
 Plotting several line plots or mutliple scatter plots is:
 
-```
+```py
 brplotviz.plot.multi_line(x_table, y_table, record_names)
 brplotviz.plot.multi_scatter(x_table, y_table, record_names)
 
 ```
 
 To mix line and scatter plot we need to construct a list of data record tuples first:
 
-```
+```py
 record_list = [(x_list, y_list_sin, "scatter", {"label": "sine"}), (x_list, y_list_cos, "line", {"label": "cosine"})]
 brplotviz.plot.mixed_graphs(record_list)
 ```
 
 Finally, let's plot a bar chart first with one data record, then with multiple records:
 
-```
+```py
 brplotviz.plot.bar_categories([y_list_sin], category_names=x_list)
 brplotviz.plot.bar_categories(y_table, category_names=x_list)
 ```
 
-Plotting graphs is not the only thing, which can be done with `brplotviz`.
-Presenting data in tabular form is also supported.
-The killer feature here are the possibilities to format the entries either alltogether or each one separately.
+## Output
 
-```
-brplotviz.table.print_table(
-	table=y_table,
-	engine="csv",
-	head_row=x_list,
-	head_col=record_names,
-	top_left="Values",
-	caption="Sine and cosine Values",
-	formatter=":.2f",
-	)
-```
+By default, plots are shown on screen and tables are printed to the standard output.
+Plots and tables can be written to disk with the keyword argument `file=<file path here>`.
+If `file` is set, the nothing shown (neither plots or tables), unless `show=True` is set explicitely.
 
-We can put out the table formatted as a LaTeX table as well.
-After copying into a `.tex` file and compiling it with LaTeX, it is typeset with professional quality.
-For this to work, follow the additional steps as described in \ref brplotviz.table.print_table_LaTeX().
-
-```
-brplotviz.table.print_table_LaTeX(
-	table=y_table,
-	head_row=x_list,
-	head_col=record_names,
-	top_left="Values",
-	formatter=":.2f",
-	caption="Sine and cosine Values",
-	LaTeX_label="sinecosine",
-	)
-```
-
-The content can be written to disk, if the keyword argument `file=<file path here>` is passed, which works for all presented functions.
-Warning: the file is overwritten without further questions.
-
-All of the presented functions are compiled in \ref example.py ready to run.
-
-# Installation and Building documentation
-Install this package via `pip install -U brplotviz`.
-To build the documentation, run `doxygen` in this directory to generate it to the directory `./Documentation`
+**Warning**: the file is overwritten without further questions.
 
 # Licence and Copyright
+
 **Author:** Bertram Richter  
 **Copyright:** Copyright by the author, 2024.  
 **License:** This software is released under GPLv3, see [LICENSE](./LICENSE) for details
 
 # Dependencies
+
 - `Python >=3.?` (Developed under Python 3.9)
 - `matplotlib >=3.5.0` for plotting and drawing graphs. See [matplotlib.org](https://matplotlib.org) for the documentation.
 - `numpy` for array operations. See [numpy.org](https://numpy.org) for the documentation.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `brplotviz-0.2.3/pyproject.toml` & `brplotviz-0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "brplotviz"
 
-version = "0.2.3"
+version = "0.3"
 
-description = "Plot utilities for outputting plots and tables nicely formatted"
+description = "Utilities for nicely formatted tables and plots"
 
 readme = "README.md"
 
 requires-python = ">=3.7"
 
 license = {file = "LICENSE"}
 
-keywords = ["plot", "table", "output"]
+keywords = ["plot", "table", "pretty-print"]
 
 authors = [
 	{name = "Bertram Richter", email = "bertram.richter@tu-dresden.de" }
 ]
 
 maintainers = [
 	{name = "Bertram Richter", email = "bertram.richter@tu-dresden.de" }
@@ -28,14 +28,15 @@
 
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
+	"Programming Language :: Python :: 3.12",
 	"Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
 	"matplotlib >= 3.5.0",
 	"numpy",
 ]
```

### Comparing `brplotviz-0.2.3/src/brplotviz/plot.py` & `brplotviz-0.3/src/brplotviz/plot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 r"""
-\file
 Contains functions for plotting.
 \author Bertram Richter
-\date 2022
-\package brplotviz.plot \copydoc plot.py
+\date 2024
 """
 
 import os
 import warnings
 
 from matplotlib import pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
```

### Comparing `brplotviz-0.2.3/src/brplotviz/styleselect.py` & `brplotviz-0.3/src/brplotviz/plot/styleselect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 r"""
-\file
 Contains functions for setting the plot style.
 \author Bertram Richter
 \date 2022
-\package brplotviz.styleselect \copydoc styleselect.py
 """
 
 from cycler import cycler, concat
 from matplotlib import pyplot as plt
 
 def set_plot_style_fig(**pltrcParams):
 	r"""
```

### Comparing `brplotviz-0.2.3/src/brplotviz/table/__init__.py` & `brplotviz-0.3/src/brplotviz/table/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,66 +7,76 @@
 """
 
 import codecs
 import copy
 import itertools
 import os
 
-from . import engines
-from .engines import *
+from . import styles
+from .styles import *
 from . import rules
-from .rules import *
 
-def get_engine(
-		engine,
+def get_style(
+		style,
 		**kwargs: dict,
-		) -> engines.Engine:
+		) -> styles.Style:
 	r"""
-	Return the engine or retrieve an engine object by its class name.
-	\param engine
-	This can be either an instance of the a subclass of \ref engines.Engine or a `str`.
-	If `engine` is an instance of a subclass, it is returned unchanged.
-	If `engine` is a string it is assumed to be a class name, and an
+	Return the style or retrieve an style object by its class name.
+	\param style
+	This can be either an instance of the a subclass of \ref styles.Style or a `str`.
+	If `style` is an instance of a subclass, it is returned unchanged.
+	If `style` is a string it is assumed to be a class name, and an
 	instance of that class with default settings is returned.
 	Note that the class name is case-insensitive.
-	\param kwargs Keyword arguments, passed to the constructor of the engine.
+	\param kwargs Keyword arguments, passed to the constructor of the style.
 	"""
-	if isinstance(engine, Engine):
-		return engine
-	elif isinstance(engine, type) and issubclass(engine, Engine):
-		return engine(**kwargs)
-	elif isinstance(engine, str):
+	if isinstance(style, Style):
+		return style
+	elif isinstance(style, type) and issubclass(style, Style):
+		return style(**kwargs)
+	elif isinstance(style, str):
 		try: 
-			return getattr(engines, engine.lower())(**kwargs)
+			return getattr(styles, style.lower())(**kwargs)
 		except:
-			raise RuntimeError("Unknown table layout engine: {}".format(engine))
+			raise RuntimeError("Unknown table layout style: {}".format(style))
 
 def print_table(table: list,
-		engine = "csv",
+		style = "csv",
 		head_col: list = None,
 		head_row: list = None,
 		top_left: str = "",
 		align = "l",
 		caption: str = None,
 		file: str = None,
 		formatter = None,
+		omit_headrule: bool = False,
 		replacement: dict = None,
 		show: bool = None,
 		transpose_data: bool = False,
 		return_lines: bool = False,
-		engine_kwargs: dict = None,
+		style_kwargs: dict = None,
 		*args, **kwargs):
 	r"""
 	Prints the table in a nice format.
 	\param table List of lists (array-like, but can have different data types).
-	\param engine This is the engine specifying the table's style.
-		Defaults to `"csv"`, see \ref engines for available options.
-	\param head_col List of row heads, printed as a column infront of rest of the columns, if not left `None` (default).
+	\param style This is the style specifying the table's style.
+		Defaults to `"csv"`, see \ref styles for available options.
+	\param head_col Row heads printed as a column infront of rest of the columns.
+		Following options are available:
+		- `None` (default): The table is not prepended with an extra column.
+		- `list`: A list, each entry is a cell.
+		- `"enumerate"`: the rows of the table body are enumerated.
+			The counting starts at 1 after the `head_row` (if present).
 	\param head_row List of column heads, printed as a line before the rest of the rows, if not left `None` (default).
 	\param top_left This is put in the top-left cell, if both `head_row` and `head_col` are provided. Defaults to `""`.
+	\param omit_headrule Switch to turn off the style-specific \ref rules.HeadRule.
+		Defaults to `False` (show the rule, if the style support that).
+		If the style does not show \ref rules.HeadRule, this setting has no effect.
+		Keep in mind, that this could can invalidate the table format
+		(e.g., Markdown).
 	\param align Specifies the alignment options of the columns.
 		Available options:
 		- `"l"` (default): All columns are left-aligned.
 		- `"c"`: All columns are centered.
 		- `"r"`: All columns are right-aligned.
 		- `None`: No alignment of columns is done.
 		- List of afforementioned options: Each column can have it's own alignment.
@@ -89,17 +99,17 @@
 		If you want to replace (raw) content before the formatting, use \ref replace() before passing the table to \ref print_table().
 	\param show Switch, whether the formatted table should be printed to the default output.
 		If set to `None` (default), it is shown, if `file is None`.
 	\param transpose_data If set to `True`, the content of `table` will be transposed before typesetting.
 		Defaults to `False`.
 		Note, that `head_row` and `head_col` will not be swapped.
 	\param return_lines Switch, whether the list of formatted lines should be returned. Defaults to `False`.
-	\param engine_kwargs Keyword arguments, passed to the constructor of the engine.
+	\param style_kwargs Keyword arguments, passed to the constructor of the style.
 		This can be used to influence some aspects of the table.
-		See \ref engines.Engine.__init__() for more details.
+		See \ref styles.Style.__init__() for more details.
 	\param *args Additional positional arguments, will be ignored.
 	\param **kwargs Additional keyword arguments, will be ignored.
 	
 	The layout with both `head_row` and `head_col` specified will be:
 	| `top_left`	| `head_row 0`	| `head_row 1`	|
 	|:---			| :---:			| :---:			|
 	| `head_col 0`	| `0,0`			| `0,1`			|
@@ -113,85 +123,88 @@
 	
 	Without `head_row`:
 	|				|		|		|
 	| :---			| :---:	| :---:	|
 	| `head_col 0`	| `0,0`	| `0,1`	|
 	| `head_col 1`	| `1,0`	| `1,1`	|
 	"""
-	engine_kwargs = engine_kwargs if engine_kwargs is not None else {}
-	engine = get_engine(engine, **engine_kwargs)
-	# Convert the table to a list of lists (e.g., from numpy arrays) and
-	# extract extra rules
-	clean_table = []
-	rule_dict = {}
-	for i, row in enumerate(copy.deepcopy(table)):
-		if isinstance(row, Rule):
-			rule_dict[i] = row
-		elif isinstance(row, type) and issubclass(row, Rule):
-			rule_dict[i] = row()
-		else:
-			try:
-				clean_table.append(list(row))
-			except:
-				raise ValueError("Cannot convert {}th entry to list: {}".format(i, row))
-	table = clean_table
+	style_kwargs = style_kwargs if style_kwargs is not None else {}
+	style = get_style(style, **style_kwargs)
 	# Transpose the body data, if requested
 	if transpose_data:
+		table, _ = _clean_table(table)
 		table = _transpose(table)
 	# Convert to table of str
+	clean_table, _ = _clean_table(table)
 	table = _apply_format(table, formatter)
-	# Convert the entries of the top_left, head column and head row to str.
-	# This will result in a new list, so the original data is not modified.
 	top_left = "{}".format(top_left)
+	# Enumerate tabele body lines, if requested
+	if isinstance(head_col, str) and head_col.lower() == "enumerate":
+		head_col = list(range(1, len(clean_table)+1))
+	# Add the head_col to the table
+	if head_col is not None:
+		head_col = _apply_format([head_col], formatter=None)[0]
+		head_col_iter = iter(head_col)
+		for line in table:
+			if not _rule_check(line):
+				line.insert(0, next(head_col_iter))
+	# Add the head_row to the table
 	if head_row is not None:
 		head_row = _apply_format([head_row], formatter=None)[0]
+		if head_col is not None:
+			head_row.insert(0, top_left)
 		table.insert(0, head_row)
-	if head_row is not None and head_col is not None:
-		head_col = _apply_format([head_col], formatter=None)[0]
-		head_col.insert(0, top_left)
+	if not omit_headrule:
+		table.insert(1, rules.HeadRule())
+	# New line treatment
+	table_lines = []
+	for i, row in enumerate(table):
+		rule = _rule_check(row)
+		if rule:
+			# Check if the previous rule must be overwritten, the rule
+			# with the lower priority value wins.
+			if i > 0 and _rule_check(table_lines[-1]):
+				last = table_lines.pop()
+				rule = rule if rule.priority < last.priority else last
+			table_lines.append(rule)
+		else:
+			row = _newline_split(row)
+			table_lines.extend(row)
+			table_lines.append(rules.MidRule())
+	table_lines.pop()
+	# Temporarily remove rules to prepare for columnwise operation
+	table, rule_dict = _clean_table(table_lines)
 	# Transpose and operate column wise
 	table = _transpose(table)
-	# Add header column
-	if head_col is not None:
-		table.insert(0, head_col)
 	if replacement is not None:
 		table = replace(table, replacement)
 	col_widths = _find_col_width(table)
 	alignments = _get_alignments(table, align)
-	col_widths = engine.modify_col_widths(col_widths, alignments)
+	col_widths = style.modify_col_widths(col_widths, alignments)
 	table =_align(table, alignments, col_widths)
-	# Transpose again
+	# Transpose again operate row wise again
 	table = _transpose(table)
 	# Insert extra rules again
-	if not transpose_data:
-		# but only if the data was now extra transposed
-		for i, rule in rule_dict.items():
-			if head_row is None:
-				table.insert(i, rule)
-			else:
-				table.insert(i+1, rule)
+	for i, rule in rule_dict.items():
+		table.insert(i, rule)
 	# Compose table as lines of text
 	formatted_lines = []
 	if caption is not None:
 		formatted_lines.append(caption)
-	_rule(formatted_lines, TopRule(), engine, col_widths, alignments)
-	formatted_lines.append(engine.row(table[0]))
-	_rule(formatted_lines, HeadRule(), engine, col_widths, alignments)
-	row_count = len(table)
-	for row_nr, row in enumerate(table[1::]):
-		if not isinstance(row, Rule):
-			formatted_lines.append(engine.row(row))
-			rule = engine.rule(col_widths, alignments, MidRule)
+	rule = style.rule(col_widths, alignments, rules.TopRule())
+	if rule is not None:
+		formatted_lines.append(rule)
+	for row in table:
+		if not isinstance(row, rules.Rule):
+			formatted_lines.append(style.row(row))
+		else:
+			rule = style.rule(col_widths, alignments, row)
 			if rule is not None:
 				formatted_lines.append(rule)
-			if not row_nr == row_count-1:
-				_rule(formatted_lines, MidRule(), engine, col_widths, alignments)
-		else:
-			_rule(formatted_lines, row, engine, col_widths, alignments)
-	rule = engine.rule(col_widths, alignments, BotRule())
+	rule = style.rule(col_widths, alignments, rules.BotRule())
 	if rule is not None:
 		formatted_lines.append(rule)
 	# Output
 	_output_table(formatted_lines, file, show)
 	if return_lines:
 		return formatted_lines
 
@@ -201,25 +214,31 @@
 		top_left: str = "",
 		align = "l",
 		caption: str = None,
 		file: str = None,
 		formatter = None,
 		LaTeX_label: str = None,
 		LaTeX_format: str = "l",
-		show: bool = None,
+		omit_headrule: bool = False,
 		replacement: dict = None,
+		show: bool = None,
 		table_head: str = None,
 		transpose_data: bool = False,
 		return_lines: bool = False,
 		*args, **kwargs):
 	r"""
 	Prints the table in a LaTeX format, and it can be copied or input directly into a TeX file.
 	This is a convenience wrapper around \ref print_table().
 	\param table List of lists (array-like, but can have different data types).
-	\param head_col List of row heads, printed as a column infront of rest of the columns, if not left `None` (default).
+	\param head_col Row heads printed as a column infront of rest of the columns.
+		Following options are available:
+		- `None` (default): The table is not prepended with an extra column.
+		- `list`: A list, each entry is a cell.
+		- `"enumerate"`: the rows of the table body are enumerated.
+			The counting starts at 1 after the `head_row` (if present).
 	\param head_row List of column heads, printed as a line before the rest of the rows, if not left `None` (default).
 	\param top_left This is put in the top-left cell, if both `head_row` and `head_col` are provided.
 		Defaults to `""`.
 	\param align Specifies the alignment options of the columns.
 		Missing entries are filled up with left-alignment (`"l"`).
 		Available options:
 		- `"l"` (default): All columns are left-aligned.
@@ -244,14 +263,16 @@
 		If given `None`, the `file` is used as fallback.
 	\param LaTeX_format Column format specification according to the LaTeX specification.
 		This is flexible with the following options:
 		- String: The format is applied to all data columns.
 			By default, all data columns will be left-aligned, which is equivalent to `"l"`.
 		- List of strings: I is assumed, that each data column has an individual format.
 			Make sure, the number of rows is in sync with the data to avoid compilation errors.
+	\param omit_headrule Switch to turn off the style-specific \ref rules.HeadRule.
+		Defaults to `False`, show the rule.
 	\param replacement  This dictionary contains the source values (to replace) as keys and the target values (to be replaced by) as values.
 		Example: to replace all `NaN` (not a number) by em-dashes and all 0 by `"nothing"`: `{"nan": "---", 0: "nothing"}`
 		Defaults to `None` (no replacement is attempted).
 		If activated, the replacement in carried out after converting the cells to `str`, but before alignment.
 		If you want to replace (raw) content before the formatting, use \ref replace() before passing the table to \ref print_table().
 	\param show Switch, whether the formatted table should be printed to the default output.
 		If set to `None` (default), it is shown, if `file is None`.
@@ -267,69 +288,64 @@
 	To use the generated table, add the following code to your preamble:
 	```
 	\newcommand{\thfl}[1]{\multicolumn{1}{@{}l}{#1}}	% table head format, left most column
 	\newcommand{\thfm}[1]{\multicolumn{1}{c}{#1}}		% table head format, middle column
 	\newcommand{\thfr}[1]{\multicolumn{1}{c@{}}{#1}}	% table head format, right most column
 	```
 	If specifies the formatting of the cells in the header row for the whole document.
-	To actually print the table, use the following code snippet:
-	```
-	\begin{table}[hbtp]
-	\centering
-	% <copy table content here> or \input{<filename>}
-	\end{table}
-	```
+	Then, you can copy the table into your TeX file or use `\input{<filename>}`.
 	"""
 	# Preparation
 	LaTeX_label = LaTeX_label if LaTeX_label is not None else file
-	if head_row is not None:
-		top_left = r"\thfl{"+"{}".format(top_left)+r"}"
+	top_left = r"\thfl{"+"{}".format(top_left)+r"}"
+	if head_row is not None and len(head_row):
 		head_row_format = [r"\thfm{"+"{}".format(entry)+r"}" for entry in head_row]
 		if head_col is None:
 			head_row_format[0] = r"\thfl{"+"{}".format(head_row[0])+r"}"
 		head_row_format[-1] = r"\thfr{"+"{}".format(head_row[-1])+r"}"
 		head_row = head_row_format
 	# Preamble
-	formatted_lines = []
+	formatted_lines = [r"\begin{table}[!htbp]", r"\centering"]
 	formatted_lines.append(r"\caption{" + "{}".format(caption) + r"}")
 	formatted_lines.append(r"\label{tab:" + "{}".format(LaTeX_label) + r"}")
 	formatted_lines.append(r"\begin{tabular}{@{}")
 	if head_col is not None:
 		formatted_lines.append(r"*{1}{l}")
 	if isinstance(LaTeX_format, str):
 		formatted_lines.append(r"*{" + "{}".format(len(table[0])) + "}{" + "{}".format(LaTeX_format) + "}")
 	elif isinstance(LaTeX_format, (list, tuple)):
 		for col in LaTeX_format:
 			formatted_lines.append(r"*{1}{" + "{}".format(col) + "}")
 	else:
 		raise ValueError("LaTeX-format needs to be a str or iterable, not {}".format(type(LaTeX_format)))
 	formatted_lines.append(r"@{}}")
-	formatted_lines.append(r"\toprule")
 	# Add optional head
 	if table_head is not None:
 		formatted_lines.append(table_head)
 	# Table content
 	content = print_table(table=table,
-			engine="latex",
+			style="latex",
 			align=align,
 			head_row=head_row,
 			head_col=head_col,
 			top_left=top_left,
 			caption=None,
 			formatter=formatter,
 			file=None,
+			omit_headrule=omit_headrule,
 			replacement=replacement,
 			show=False,
 			transpose_data=transpose_data,
 			return_lines=True,
+			*args, **kwargs
 			)
 	formatted_lines.extend(content)
 	# Postamble
-	formatted_lines.append(r"\bottomrule")
 	formatted_lines.append(r"\end{tabular}")
+	formatted_lines.append(r"\end{table}")
 	# Output
 	_output_table(formatted_lines, file, show)
 	if return_lines:
 		return formatted_lines
 
 def replace(table: list, replacement: dict) -> list:
 	r"""
@@ -337,15 +353,15 @@
 	\param table Table, for which the content of all cells should be replaced, if they contain something in `source`.
 	\param replacement This dictionary contains the source values (to replace) as keys and the target values (to be replaced by) as values.
 		Example: to replace all `NaN` (not a number) by em-dashes and all `0` by `"nothing"`: `{"nan": "---", 0: "nothing"}`
 	"""
 	if replacement is None:
 		return table
 	for row in table:
-		if not isinstance(row, Rule):
+		if not isinstance(row, rules.Rule):
 			for i, entry in enumerate(row):
 				row[i] = replacement[entry] if entry in replacement else entry
 	return table
 
 def _apply_format(table: list, formatter) -> list:
 	r"""
 	Converts the entries of the given table into `str`.
@@ -355,15 +371,15 @@
 	"""
 	if formatter is None:
 		formatter = ""
 	if isinstance(formatter, str):
 		formatter = itertools.repeat(formatter)
 	str_table = []
 	for row in table:
-		if not isinstance(row, Rule):
+		if not _rule_check(row):
 			str_row = []
 			for format_entry, entry in zip(formatter, row):
 				try:
 					str_row.append("{}".format("{"+format_entry+"}").format(entry))
 				except:
 					str_row.append(str(entry))
 			str_table.append(str_row)
@@ -385,14 +401,28 @@
 	align_code = [align_dict.get(a, "") for a in alignments]
 	aligned = []
 	for align, col, width in zip(align_code, table, col_widths):
 		aligned_col = [("{:" + align + str(width) + "}").format(str(entry)) for entry in col]
 		aligned.append(aligned_col)
 	return aligned
 
+def _clean_table(table):
+	clean_table = []
+	rule_dict = {}
+	for i, row in enumerate(copy.deepcopy(table)):
+		rule = _rule_check(row)
+		if rule:
+			rule_dict[i] = row
+		else:
+			try:
+				clean_table.append(list(row))
+			except:
+				raise ValueError("Cannot convert {}th entry to list: {}".format(i, row))
+	return clean_table, rule_dict
+
 def _find_col_width(table: list) -> list:
 	r"""
 	For each column in the table, the width of the column is determined
 	by the widest cell in the respective column.
 	\param table Table for which the column widths should be determined.
 		It is assumed, that:
 		- the original table is transposed (each entry is a column) and
@@ -457,24 +487,48 @@
 	\param head_row First row, of the table, which holds the column names.
 	\param head_col First column, of the table, which holds the row names.
 	\param top_left Content of the cell, which appears in the top left corner of the table, when both `head_row` and `head_col` is added.
 	"""
 	if head_col is not None:
 		head_col_gen = iter(copy.deepcopy(head_col))
 		for row in table:
-			if not isinstance(row, Rule):
+			if not isinstance(row, rules.Rule):
 				row.insert(0, str(next(head_col_gen)))
 	
 	if head_row is not None:
 		if head_col is not None:
 			table.insert(0, [str(top_left)] + [str(entry) for entry in head_row])
 		else:
 			table.insert(0, [str(entry) for entry in head_row])
 	return table
 
+def _newline_split(row):
+	max_new_lines = 0
+	extra_lines = [[""]*len(row)]
+	for col_number, cell in enumerate(row):
+		if "\n" not in cell:
+			extra_lines[0][col_number] = cell
+			continue
+		# A newline was found
+		cell_lines = cell.split("\n")
+		max_new_lines = max(len(extra_lines), len(cell_lines))
+		for i in range(len(extra_lines), max_new_lines):
+			extra_lines.append([""]*len(row))
+		for extra_line_number, sub_cell in enumerate(cell_lines):
+			extra_lines[extra_line_number][col_number] = sub_cell
+	extra_lines_rules = []
+	for line in extra_lines:
+		if _rule_check(line):
+			extra_lines_rules.append(line)
+		else:
+			extra_lines_rules.append(line)
+			extra_lines_rules.append(rules.NoRule())
+	extra_lines_rules.pop()
+	return extra_lines_rules
+
 def _output_table(formatted_lines: list, file: str, show: bool):
 	r"""
 	Depending on the options, the list of lines is either written to a file on disk or printed on the screen (or neither).
 	\param formatted_lines List of table lines to be outputted.
 	\param file Path to the file in which the table is written to.
 		Defaults to `None`, which means the table is printed on screen instead of saved to disk.
 		If a valid path is given, the table is written to this file.
@@ -493,37 +547,32 @@
 					f.write(line + "\n")
 		except:
 			print('Failed to save table to file "{}"'.format(file))
 	if show:
 		for line in formatted_lines:
 			print(line)
 
-def _rule(
-		formatted_lines: list,
-		rule: rules.Rule,
-		engine: engines.Engine,
-		col_widths: list,
-		alignments: list
-		):
-	r"""
-	Add a rule.
-	\param formatted_lines The alread fully typeset lines of the table.
-	\param rule A \ref rules.Rule, for which the engine is requested to
-		draw a rule.
-	\param engine The engine to draw a rule.
-	\param col_widths A list of the columns' widths.
-	\param alignments A full aligment list (see \ref _get_alignments()).
+def _rule_check(rule):
 	"""
-	rule = engine.rule(col_widths, alignments, rule)
-	if rule is not None:
-		formatted_lines.append(rule)
+	Returns an instance of the \ref rules.Rule objects, of `rule`'s (sub)class.
+	If `rule` is not a \ref rules.Rule object, `None` is returned.
+	Apart from conversion to instances, this can be used to check whether
+	`rule` is a \ref rules.Rule object, because \ref rules.Rule objects, when typecast
+	boolean to result in `True`, but `None` typecast to boolean gives `False`. 
+	"""
+	if isinstance(rule, rules.Rule):
+		return rule
+	elif isinstance(rule, type) and issubclass(rule, rules.Rule):
+		return rule()
+	else:
+		return None
 
 def _transpose(table: list) -> list:
 	r"""
 	Transposes the given table, columns become rows and rows become columns.
 	Missing cells (if a row has fewer entries than other rows) will be
 	fill up with empty strings (`""`).
-	"""	
+	"""
 	return list(map(list, itertools.zip_longest(*table, fillvalue="")))
 
 if __name__ == "__main__":
 	pass
```

### Comparing `brplotviz-0.2.3/src/brplotviz/table/engines.py` & `brplotviz-0.3/src/brplotviz/table/styles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 
 r"""
-This module contains the class definitions for table engines, each of
+This module contains the class definitions for table styles, each of
 which in turn define the look of the table.
 
-See \ref doc/engine_overview.md for an overview of all available styles.
-
 \author Bertram Richter
 \date 2024
 """
 
 import itertools
-from .rules import *
+from . import rules
+#from .rules import *
 
-class Engine():
+class Style():
 	r"""
-	Base class for a table engine.
-	An engine simply stores the style and look of the table, that is the
+	Base class for a table style.
+	A style simply stores the style and look of the table, that is the
 	how the rows and columns are separated and how the frame around the
 	tabular data looks like.
 	For defining a custom table look, implement it as subclass to this one.
 	"""
 	def __init__(self,
 			linestart: str,
 			firstsep: str,
 			itemsep: str,
 			lineend: str,
 			pad_left: str = "",
 			pad_right: str = "",
 			*args, **kwargs):
 		r"""
-		Construct the engine object.
+		Construct the Style object.
 		\param linestart \copydoc linestart
 		\param firstsep \copydoc firstsep
 		\param itemsep \copydoc itemsep
 		\param lineend \copydoc lineend
 		\param pad_left \copydoc pad_left
 		\param pad_right \copydoc pad_right
 		\param *args Additional positional arguments, ignored.
@@ -47,15 +46,15 @@
 		self.itemsep = itemsep
 		## This is appended to the end of each line.
 		self.lineend = lineend
 		## This in each cell put between the content and the \ref itemsep to the left. 
 		self.pad_left = pad_left
 		## This in each cell put between the content and the \ref itemsep to the right. 
 		self.pad_right = pad_right
-	def rule(self, widths: list, align: list, rule_type: Rule) -> str:
+	def rule(self, widths: list, align: list, rule_type: rules.Rule) -> str:
 		r"""
 		Return a `str` looking like the table rule, based on the type (\ref rules).
 		`None` is returned if no rule should be drawn. 
 		\param widths List of `int` containing the column widths.
 		\param align List of `str` containing the column alignments.
 		\param rule_type \ref rules.Rule object which indicates, which rule is used.
 		"""
@@ -72,155 +71,157 @@
 			+ self.pad_left + self.firstsep + self.pad_right \
 			+ (self.pad_left + self.itemsep + self.pad_right).join(row[1::]) \
 			+ self.pad_left + self.lineend
 		return line
 	def modify_col_widths(self, col_widths: list, align: list) -> list:
 		r"""
 		This method is used to modify the determined column widths, as
-		some engines require a minimum column width (e.g., \ref markdown).
-		But most engines will just return the list of column widths.
+		some styles require a minimum column width (e.g., \ref markdown).
+		But most styles will just return the list of column widths.
 		\param col_widths List of `int`, which are the column widths in charaters.
 		\param align List of `str`, specifying the aligment of each column.
 		"""
 		return col_widths
 
-class csv(Engine):
+class csv(Style):
 	r"""
 	Character separated table, defaulting to the comma (`","`).
 	
-	This engine has no built table rules.
+	This style has no table rules.
 	The \ref rules.ExtraRule is used to insert a blank line.
 	
 	Start th 
 	"""
 	def __init__(self, itemsep: str = ",", **kwargs):
 		r"""
-		Construct the csv engine.
+		Construct the csv style.
 		\param itemsep \copydoc itemsep
 			This defaults to the comma (`","`).
 		\param kwargs Additional keyword arguments, passed to the
 			superclass' constructor.
 		"""
 		super().__init__(
 			linestart = "",
 			firstsep = itemsep,
 			itemsep = itemsep,
 			lineend = "",
 			**kwargs)
-	def rule(self, widths: list, align: str, rule_type: str) -> str:
+	def rule(self, widths: list, align: str, rule_type: rules.Rule) -> str:
 		r"""
-		\copydoc Engine.rule()
+		\copydoc Style.rule()
 		
-		This engine has no built table rules.
+		This style has no built table rules.
 		The \ref rules.ExtraRule is used to insert a blank line. 
 		"""
-		if isinstance(rule_type, ExtraRule):
+		if isinstance(rule_type, rules.ExtraRule):
 			return ""
 		else:
 			return None
 
 class tsv(csv):
 	r"""
 	A variation of \ref csv, but with tab (`"\t"`) as column separator.
 	
 	\copydetails csv
 	"""
 	def __init__(self, itemsep: str = "\t", **kwargs):
 		r"""
-		Construct the tsv engine.
+		Construct the tsv style.
 		\param itemsep \copydoc itemsep
 			This defaults to the tab (`"\t"`).
 		\param kwargs Additional keyword arguments, passed to the
 			superclass' constructor.
 		"""
 		super().__init__(itemsep, **kwargs)
 
-class latex(Engine):
+class latex(Style):
 	r"""
 	A LaTeX table, columns are separated by the ampersand (`"&"`) and the
 	the lines are ended with double backslash (`"\\"`).
 	
 	The table rules use the rules provided by [booktabs](https://ctan.org/pkg/booktabs/).
 	Before the tabular part, the table is started with `"\topule"`, the
 	header line is separated by `"\midrule"` and the tabular part is
 	closed with `"\bottomrule"`.
 	The \ref rules.ExtraRule is translated into `"\addlinespace"`, which
 	results in a small vertical space between two rows.
 	"""
 	def __init__(self, **kwargs):
 		r"""
-		Construct the LaTeX engine.
+		Construct the LaTeX style.
 		"""
 		super().__init__(linestart="",
 			firstsep="&",
 			itemsep="&",
 			lineend=r"\\",
 			**kwargs)
-	def rule(self, widths: list, align: list, rule_type: str) -> str:
+	def rule(self, widths: list, align: list, rule_type: rules.Rule) -> str:
 		r"""
-		\copydoc Engine.rule()
+		\copydoc Style.rule()
 		
 		The table rules use the rules provided by[booktabs](https://ctan.org/pkg/booktabs/).
 		Before the tabular part, the table is started with `"\topule"`,
 		the header line is separated by `"\midrule"` and the tabular part
 		is closed with `"\bottomrule"`.
 		The \ref rules.ExtraRule is translated into `"\addlinespace"`,
 		which results in a small vertical space between two rows.
 		"""
-		if isinstance(rule_type, TopRule):
+		if isinstance(rule_type, rules.TopRule):
 			return r"\toprule"
-		elif isinstance(rule_type, HeadRule):
+		elif isinstance(rule_type, rules.HeadRule):
 			return r"\midrule"
-		elif isinstance(rule_type, BotRule):
+		elif isinstance(rule_type, rules.BotRule):
 			return r"\bottomrule"
-		elif isinstance(rule_type, ExtraRule):
+		elif isinstance(rule_type, rules.ExtraRule):
 			return r"\addlinespace"
 		else:
 			return None
 
-class markdown(Engine):
+class markdown(Style):
 	r"""
 	A Markdown table.
 	"""
 	def __init__(self, **kwargs):
 		r"""
-		Construct the Markdown engine.
+		Construct the Markdown style.
 		"""
 		super().__init__(
 			linestart = "|",
 			firstsep = "|",
 			itemsep = "|",
 			lineend = "|",
 			**kwargs
 			)
 		self.rulestart = "|",
 		self.firstrulesep = "|",
 		self.rulesep = "|",
 		self.ruleend = "|",
-	def rule(self, widths: list, align: str, rule_type: str) -> str:
+	def rule(self, widths: list, align: str, rule_type: rules.Rule) -> str:
 		r"""
 		Markdown only draws the \ref rules.HeadRule.
 		"""
-		if isinstance(rule_type, HeadRule):
+		if isinstance(rule_type, rules.HeadRule):
 			if align is None or isinstance(align, str):
 				align = [align] * len(widths)
 			rule = []
 			for w, alignment in itertools.zip_longest(widths, align, fillvalue=""):
 				if alignment is None or alignment == "":
 					rule.append("-"*max(3, w))
 				if alignment == "l": 
 					rule.append(":" + "-"*max(3, w-1))
 				elif alignment == "c": 
 					rule.append(":" + "-"*max(3, w-2) + ":")
 				elif alignment == "r": 
 					rule.append("-"*max(3, w-1) + ":")
 			return self.row(rule)
+		else:
+			return None
 	def modify_col_widths(self, col_widths: list, align: list) -> list:
 		r"""
-		\copydoc Engine.modify_col_widths()
+		\copydoc Style.modify_col_widths()
 		
 		Markdown requires following column widths:
 		
 		| Alignment | Width |
 		|:----------|:-----:|
 		| left      |   4   |
 		| centered  |   5   |
@@ -234,7 +235,23 @@
 			if alignment is None:
 				new_col_widths.append(max(3, w))
 			elif alignment == "c": 
 				new_col_widths.append(max(5, w))
 			else: 
 				new_col_widths.append(max(4, w))
 		return new_col_widths
+
+class test(Style):
+	def __init__(self, **kwargs):
+		r"""
+		Construct the Test style.
+		This is only useful for easier debugging.
+		"""
+		super().__init__(linestart="^",
+			firstsep="||",
+			itemsep="|",
+			lineend="$",
+			pad_left=" <",
+			pad_right="> ",
+			)
+	def rule(self, widths: list, align: str, rule_type: str) -> str:
+		return str("---{}---".format(type(rule_type).__name__))
```

### Comparing `brplotviz-0.2.3/src/brplotviz.egg-info/PKG-INFO` & `brplotviz-0.3/src/brplotviz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: brplotviz
-Version: 0.2.3
-Summary: Plot utilities for outputting plots and tables nicely formatted
+Version: 0.3
+Summary: Utilities for nicely formatted tables and plots
 Author-email: Bertram Richter <bertram.richter@tu-dresden.de>
 Maintainer-email: Bertram Richter <bertram.richter@tu-dresden.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -678,123 +678,347 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/bertramrichter/brplotviz
 Project-URL: Bug Reports, https://github.com/bertramrichter/brplotviz/issues
 Project-URL: Source, https://github.com/bertramrichter/brplotviz
-Keywords: plot,table,output
+Keywords: plot,table,pretty-print
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5.0
 Requires-Dist: numpy
 
-`brplotviz` are plot utilities for outputting plots using `matplotlib` and nicely formatted tables according to the personal taste of Bertram Richter.
+`brplotviz` – utilities for nicely formatted tables and plots
+
+# Installation and Building documentation
+
+Install this package via `pip install -U brplotviz`.
+To build the documentation, download the source code and unpack it.
+Then, run `doxygen` in `brplotviz`'s root directory (this one).
+How to install `doxygen`, see on their website ([doxygen.nl](https://doxygen.nl)).
+The documentation will be assing it to the directory `./Documentation`
 
 # Getting started
-This package provides functions to simplify the output of nicely fomatted graphs.
-The main focus is to enable consistent graphical style suited for printing.
+
+`brplotviz` consists of two packages, `table` and `plot`.
+
+## Table
+
+`brplotviz.plot.table` provides functions to format and output tabular data.
+This tabular data is expected to be a sequence of sequences (list of lists ect.).
+When a row (or column) is shorter than the others the missing cells are added as empty ones.
+Multi-line cells (containing newline characters) are supported,
+additional lines are inserted in the output plain text table a required.
+
+### Styles
+
+`brplotviz.table` comes with a few table styles.
+To showcase the different styles, the script is used, where only the
+`<style>` is replaced with the following options.
+
+Some finer, advanced tuning of the style can be done with the `style_kwargs` dictionary.
+For example, padding of the cells on the left or right side is possible.
+
+```py
+table_data = [
+	["a",123.456, 12],
+	["bc\nde", 23.34, 345],
+	["and f", 45.],
+	]
+
+table.print_table(
+	table=table_data,
+	style=<style>,
+	)
+```
+
+`"csv"` is a simple character-separated value style.
+The separator character is configurable, but defaults to the comma (`","`).
+
+```
+a    ,123.456,12 
+bc   ,23.34  ,345
+de   ,       ,   
+and f,45.0   ,   
+```
+
+`"tsv"` is a special case of `csv` with tab (`"\t"`) as separator charater.
+
+```
+a    	123.456	12 
+bc   	23.34  	345
+de   	       	   
+and f	45.0   	   
+```
+
+`"latex"`
+A table using the LaTeX markup with `booktabs` rules.
+This only sets the content that goes into the body of a `tabular` environment.
+
+```
+\toprule
+a    &123.456&12 \\
+\midrule
+bc   &23.34  &345\\
+de   &       &   \\
+and f&45.0   &   \\
+\bottomrule
+```
+
+A complete LaTeX environment is output the wrapper function `brplotviz.table.print_table_LaTeX()`.
+This function accepts the same (and some more) arguments than `brplotviz.table.print_table()`
+
+```py
+brplotviz.table.print_table_LaTeX(
+	table=table,
+	caption="This is the caption",
+	LaTeX_label="example",
+	)
+```
+
+The result is the following LaTeX code.
+Note, that `brplotviz` will try to fill in the column alignment based on `align`.
+TO overwrite the default, use the argument `LaTeX_format`.
+`LaTeX_format` works analougously to `align`.
+
+```
+\begin{table}[!htbp]
+\centering
+\caption{This is the caption}
+\label{tab:example}
+\begin{tabular}{@{}
+*{3}{l}
+@{}}
+\toprule
+a    &123.456&12 \\
+\midrule
+bc   &23.34  &345\\
+de   &       &   \\
+and f&45.0   &   \\
+\bottomrule
+\end{tabular}
+\end{table}
+```
+
+"markdown"`outputs a Markdown table.
+
+```
+|a    |123.456|12  |
+|:----|:------|:---|
+|bc   |23.34  |345 |
+|de   |       |    |
+|and f|45.0   |    |
+```
+
+`"test"` is for testing purposes.
+
+```
+---TopRule---
+^> a     <||> 123.456 <|> 12  <$
+---HeadRule---
+^> bc    <||> 23.34   <|> 345 <$
+---NoRule---
+^> de    <||>         <|>     <$
+---MidRule---
+^> and f <||> 45.0    <|>     <$
+---BotRule---
+```
+
+Custom styles are possible by sub-classing `brplotviz.tables.styles.Style`.
+
+### Headers
+
+`brplotviz.table` provides the option to add headers, to both columns and rows.
+The `example_table`, that we plotted could be only the body of the table.
+
+```py
+head_row = ["Col 1", "Col 2", "Col 3"]
+head_col = ["Row 1", "Row 2", "Row 3"]
+top_left = "Top left"
+align = ["l", "c", "r", "r"]
+
+table.print_table(
+	table=table_data,
+	style="markdown",
+	head_col=head_col,
+	head_row=head_row,
+	top_left=top_left,
+	)
+```
+
+Note, that both the header row `head_row` and header column `head_col`
+can be set independently of each other.
+
+```
+|Top left|Col 1|Col 2  |Col 3|
+|:-------|:----|:------|:----|
+|Row 1   |a    |123.456|12   |
+|Row 2   |bc   |23.34  |345  |
+|        |de   |       |     |
+|Row 3   |and f|45.0   |     |
+```
+
+Table rows are numbered automatically when setting `head_col="enumerate"`.
+The numbering starts after the header row.
+Note, that rows with multiline cells are taken into account.
+
+```
+|Top left|Col 1|Col 2  |Col 3|
+|:-------|:----|:------|:----|
+|1       |a    |123.456|12   |
+|2       |bc   |23.34  |345  |
+|        |de   |       |     |
+|3       |and f|45.0   |     |
+```
+
+### Formatting
+
+The formatting of the table's cells can be set table-global, column-wise or for each cell individually.
+If the `formatter` is a string, this formatter is applied to all cells of the table.
+If the `formatter` is a list of strings, the formatting is applied column-wise (without the `head_col`).
+If the `formatter` is a list of list strings, the formatting is applied for each cell individually.
+The `formatter` is expected in the [Format Specification Mini-Language](https://docs.python.org/3/library/string.html#formatspec).
+Here, it is shown for a column-wise formatting:
+
+```py
+table.print_table(
+	table=table_data,
+	style="markdown",
+	formatter=["", ":.2f", ":.1f"],
+	)
+```
+
+```
+|Top left|Col 1|Col 2 |Col 3|
+|:-------|:----|:-----|:----|
+|1       |a    |123.46|12.0 |
+|2       |bc   |23.34 |345.0|
+|        |de   |      |     |
+|3       |and f|45.00 |     |
+```
+
+### Alignment
+
+Columns are alined by adding whitespace to make all cells in a column to the same width.
+By default, all cells are printed left-aligned.
+Similar to the formatting, the alignment can be set for all columns or for each column separately.
+Alignment can be turned off by setting `align=None`.
+
+```py
+table.print_table(
+	table=table_data,
+	style="markdown",
+	align=["l", "c", "r", "r"],
+	)
+```
+
+```
+|Top left|Col 1| Col 2 |Col 3|
+|:-------|:---:|------:|----:|
+|1       |  a  |123.456|   12|
+|2       | bc  |  23.34|  345|
+|        | de  |       |     |
+|3       |and f|   45.0|     |
+```
+
+
+### Rules
+
+The horizontal lines in the table ar ecalled rules.
+To add an extra rule include a `brplotviz.table.rules.ExtraRule` in the `table`.
+Note, that not all styles support `ExtraLines`.
+The rule separating the header column from the body can be suppressed by `omit_head_rule=True`.
+
+### Additional options for table output
+
+To transpose the `table` (switch columns with rows), use `transpose=True`.
+Note, that this will not switch `head_col` and `head_row`.
+
+With `replacement`, a dictionary can be passed to replace cell content.
+If a cell's content is found in the replacement`'s keys, the content is replaced with the associated value.
+Note, that the replacement takes place after formatting.
+
+By default `brplotviz.table.print_table()`, prints the typeset table and returns nothing (`None`).
+To return the lines, set `return_lines=True`.
+Set `show=False` to turn off the printing.
+
+## Plot
+
+`brplotviz.plot` provides functions to simplify the output of nicely formatted graphs.
+The focus is on a graphical style suited for printing.
 Thus, a monochrome (black-white) style is used.
 
 Let's start plotting.
 First, we need some data:
 
-```
+```py
 import numpy as np
 import brplotviz
 x_list = np.linspace(0, 2, 17)
 y_list_sin = np.sin(x_list)
 y_list_cos = np.cos(x_list)
 x_table = [x_list, x_list]
 y_table = [y_list_sin, y_list_cos]
 record_names = ["sine", "cosine"]
 ```
 
 Plotting a single line-graph and a scatter plot is as simple as:
+Each one is shown on separately.
 
-```
+```py
 brplotviz.plot.single_line(x_list, y_list_sin)
 brplotviz.plot.single_scatter(x_list, y_list_sin)
 ```
 
 Plotting several line plots or mutliple scatter plots is:
 
-```
+```py
 brplotviz.plot.multi_line(x_table, y_table, record_names)
 brplotviz.plot.multi_scatter(x_table, y_table, record_names)
 
 ```
 
 To mix line and scatter plot we need to construct a list of data record tuples first:
 
-```
+```py
 record_list = [(x_list, y_list_sin, "scatter", {"label": "sine"}), (x_list, y_list_cos, "line", {"label": "cosine"})]
 brplotviz.plot.mixed_graphs(record_list)
 ```
 
 Finally, let's plot a bar chart first with one data record, then with multiple records:
 
-```
+```py
 brplotviz.plot.bar_categories([y_list_sin], category_names=x_list)
 brplotviz.plot.bar_categories(y_table, category_names=x_list)
 ```
 
-Plotting graphs is not the only thing, which can be done with `brplotviz`.
-Presenting data in tabular form is also supported.
-The killer feature here are the possibilities to format the entries either alltogether or each one separately.
+## Output
 
-```
-brplotviz.table.print_table(
-	table=y_table,
-	engine="csv",
-	head_row=x_list,
-	head_col=record_names,
-	top_left="Values",
-	caption="Sine and cosine Values",
-	formatter=":.2f",
-	)
-```
+By default, plots are shown on screen and tables are printed to the standard output.
+Plots and tables can be written to disk with the keyword argument `file=<file path here>`.
+If `file` is set, the nothing shown (neither plots or tables), unless `show=True` is set explicitely.
 
-We can put out the table formatted as a LaTeX table as well.
-After copying into a `.tex` file and compiling it with LaTeX, it is typeset with professional quality.
-For this to work, follow the additional steps as described in \ref brplotviz.table.print_table_LaTeX().
-
-```
-brplotviz.table.print_table_LaTeX(
-	table=y_table,
-	head_row=x_list,
-	head_col=record_names,
-	top_left="Values",
-	formatter=":.2f",
-	caption="Sine and cosine Values",
-	LaTeX_label="sinecosine",
-	)
-```
-
-The content can be written to disk, if the keyword argument `file=<file path here>` is passed, which works for all presented functions.
-Warning: the file is overwritten without further questions.
-
-All of the presented functions are compiled in \ref example.py ready to run.
-
-# Installation and Building documentation
-Install this package via `pip install -U brplotviz`.
-To build the documentation, run `doxygen` in this directory to generate it to the directory `./Documentation`
+**Warning**: the file is overwritten without further questions.
 
 # Licence and Copyright
+
 **Author:** Bertram Richter  
 **Copyright:** Copyright by the author, 2024.  
 **License:** This software is released under GPLv3, see [LICENSE](./LICENSE) for details
 
 # Dependencies
+
 - `Python >=3.?` (Developed under Python 3.9)
 - `matplotlib >=3.5.0` for plotting and drawing graphs. See [matplotlib.org](https://matplotlib.org) for the documentation.
 - `numpy` for array operations. See [numpy.org](https://numpy.org) for the documentation.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

