# Comparing `tmp/bogrod-0.4.0.tar.gz` & `tmp/bogrod-0.4.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bogrod-0.4.0.tar", last modified: Tue Apr 23 11:42:02 2024, max compression
+gzip compressed data, was "bogrod-0.4.1.dev1.tar", last modified: Sat Apr 27 16:07:45 2024, max compression
```

## Comparing `bogrod-0.4.0.tar` & `bogrod-0.4.1.dev1.tar`

### file list

```diff
@@ -1,22 +1,49 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1080 2024-03-12 07:50:14.000000 bogrod-0.4.0/LICENSE
--rw-r--r--   0 patrick   (1000) patrick   (1000)    12143 2024-04-23 11:42:02.974526 bogrod-0.4.0/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11646 2024-03-12 07:50:15.000000 bogrod-0.4.0/README.md
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/bogrod/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    36873 2024-04-08 19:35:52.000000 bogrod-0.4.0/bogrod/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3306 2024-04-08 19:31:09.000000 bogrod-0.4.0/bogrod/sbom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      110 2024-04-08 19:27:37.000000 bogrod-0.4.0/bogrod/settings.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/bogrod/tests/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2022-12-22 20:02:45.000000 bogrod-0.4.0/bogrod/tests/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1382 2024-04-08 19:35:02.000000 bogrod-0.4.0/bogrod/tests/test_bogrod.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2849 2024-04-08 19:35:02.000000 bogrod-0.4.0/bogrod/util.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      283 2024-04-08 19:31:09.000000 bogrod-0.4.0/bogrod/vexfile.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-23 11:42:02.974526 bogrod-0.4.0/bogrod.egg-info/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    12143 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      347 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       39 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/entry_points.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       74 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2024-04-23 11:42:02.000000 bogrod-0.4.0/bogrod.egg-info/top_level.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2024-04-23 11:42:02.978525 bogrod-0.4.0/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      942 2024-04-08 19:35:02.000000 bogrod-0.4.0/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.294900 bogrod-0.4.1.dev1/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1080 2024-03-12 07:50:14.000000 bogrod-0.4.1.dev1/LICENSE
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      159 2024-04-27 16:07:18.000000 bogrod-0.4.1.dev1/MANIFEST.in
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12454 2024-04-27 16:07:45.294900 bogrod-0.4.1.dev1/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11744 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/README.md
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/bogrod/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       11 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/bogrod/VERSION
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    37347 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/bogrod/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       83 2024-04-23 16:15:44.000000 bogrod-0.4.1.dev1/bogrod/__main__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/bogrod/contrib/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      172 2024-04-08 19:35:56.000000 bogrod-0.4.1.dev1/bogrod/contrib/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3512 2024-04-08 19:36:01.000000 bogrod-0.4.1.dev1/bogrod/contrib/aggregator.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3474 2024-04-23 16:15:44.000000 bogrod-0.4.1.dev1/bogrod/contrib/elementaris.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/bogrod/resources/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    72251 2024-03-12 07:49:41.000000 bogrod-0.4.1.dev1/bogrod/resources/bom-1.4.schema.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)   164754 2024-04-08 19:31:09.000000 bogrod-0.4.1.dev1/bogrod/resources/bom-1.5.schema.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3757 2024-04-08 19:31:09.000000 bogrod-0.4.1.dev1/bogrod/resources/vex-1.0.schema.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3306 2024-04-08 19:31:09.000000 bogrod-0.4.1.dev1/bogrod/sbom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      110 2024-04-08 19:27:37.000000 bogrod-0.4.1.dev1/bogrod/settings.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/bogrod/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       90 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/bogrod/tests/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1711 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/bogrod/tests/test_bogrod.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      798 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/bogrod/tests/test_tui.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/bogrod/tui/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      378 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      466 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/app.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      489 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/editor.tcss
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      471 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/styles.tcss
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7134 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/vexedit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10400 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/vulnlist.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/bogrod/tui/widgets/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/widgets/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      906 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/widgets/modals.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      491 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/tui/widgets/radioslist.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2849 2024-04-08 19:35:02.000000 bogrod-0.4.1.dev1/bogrod/util.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      283 2024-04-08 19:31:09.000000 bogrod-0.4.1.dev1/bogrod/vexfile.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.294900 bogrod-0.4.1.dev1/bogrod.egg-info/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12454 2024-04-27 16:07:45.000000 bogrod-0.4.1.dev1/bogrod.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      907 2024-04-27 16:07:45.000000 bogrod-0.4.1.dev1/bogrod.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2024-04-27 16:07:45.000000 bogrod-0.4.1.dev1/bogrod.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       39 2024-04-27 16:07:45.000000 bogrod-0.4.1.dev1/bogrod.egg-info/entry_points.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      130 2024-04-27 16:07:45.000000 bogrod-0.4.1.dev1/bogrod.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       54 2024-04-27 16:07:45.000000 bogrod-0.4.1.dev1/bogrod.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-04-27 16:07:45.290900 bogrod-0.4.1.dev1/resources/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)   779246 2023-05-30 10:52:29.000000 bogrod-0.4.1.dev1/resources/demo3.jpg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12617 2024-04-23 16:15:44.000000 bogrod-0.4.1.dev1/resources/process.drawio
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    61432 2024-04-23 16:15:44.000000 bogrod-0.4.1.dev1/resources/process.png
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2024-04-27 16:07:45.294900 bogrod-0.4.1.dev1/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1187 2024-04-27 15:36:22.000000 bogrod-0.4.1.dev1/setup.py
```

### Comparing `bogrod-0.4.0/LICENSE` & `bogrod-0.4.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `bogrod-0.4.0/PKG-INFO` & `bogrod-0.4.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bogrod
-Version: 0.4.0
+Version: 0.4.1.dev1
 Summary: Manage SBOM, VEX records and release notes in a single tool
 Home-page: https://github.com/productaize/bogrod
 Author: Patrick Senti
 Author-email: patrick@productaize.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,14 +12,20 @@
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
 Requires-Dist: attrdict
 Requires-Dist: textual
 Requires-Dist: textual-dev
 Requires-Dist: requests
 Requires-Dist: yaspin
+Requires-Dist: keyring
+Provides-Extra: dev
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest-textual-snapshot; extra == "dev"
 
 Bogrod
 ======
 
 Manage vulnerabilities analysis (VEX/SBOM) in cyclonedx format like source code.
 
 Why?
@@ -61,15 +67,15 @@
 ------
 
 Run as a command line utility:
 
     usage: bogrod [-h] [-n NOTES] [-o OUTPUT] [-S] [-s SEVERITIES] [-x] [--vex-file VEX_FILE] [-p SBOM_PROPERTIES] [-m] [-w] [-W] [-g GRYPE] sbom
 
     positional arguments:
-      sbom                  /path/to/cyclonedx-sbom.json
+      sbom                  name of sbom in .bogrod, or /path/to/cyclonedx-sbom.json
     
     optional arguments:
       -h, --help            show this help message and exit
       -n NOTES, --notes NOTES
                             /path/to/notes.yaml
       -o OUTPUT, --output OUTPUT
                             output format [table,json,yaml,raw]
@@ -107,32 +113,33 @@
         $ grype sbom:releasenotes/sbom/jupyter-base-notebook.syft.json --file releasenotes/sbom/jupyter-base-notebook.cdx.json --output embedded-cyclonedx-vex-json
 
 3. Use bogrod to analyze each vulnerability interactively
 
         # -- bogrod automatically uses the .grype report to provide additional information for each vulnerability 
         $ bogrod --work -S releasenotes/sbom/jupyter-base-notebook.cdx.json --vex-file releasenotes/sbom/vex.yaml --update-vex --merge-vex 
 
-Note that bogrod will automatically find the .vex and .grype files corresponding to the .cdx file,
+Note that bogrod will automatically find the .vex and .grype files corresponding to the .cdx file, 
 if these are not specified.
 
 Working with vulnerabilities
 ----------------------------
 
 Bogrod can work interactively with vulnerabilities found in a SBOM by specifying
 the -W command line option. This will present a list of the vulnerabilities found
 so that you can select and analyze each one in turn. 
 
     $ bogrod jupyter -W
 
-![bogrod demo](resources/demo1.jpg)
+![bogrod demo](resources/demo1.png)
 
-    Select 1
-![bogrod demo](resources/demo2.jpg)
+    Press Enter to show the details of the vulnerability
 
-    Save analysis and quit
+![bogrod demo](resources/demo2.png)
+
+    Save analysis and quit by pressing Ctrl-C or Q
 
 ![bogrod demo](resources/demo3.jpg)
 
 
 Working with multiple images
 ----------------------------
```

### Comparing `bogrod-0.4.0/README.md` & `bogrod-0.4.1.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ------
 
 Run as a command line utility:
 
     usage: bogrod [-h] [-n NOTES] [-o OUTPUT] [-S] [-s SEVERITIES] [-x] [--vex-file VEX_FILE] [-p SBOM_PROPERTIES] [-m] [-w] [-W] [-g GRYPE] sbom
 
     positional arguments:
-      sbom                  /path/to/cyclonedx-sbom.json
+      sbom                  name of sbom in .bogrod, or /path/to/cyclonedx-sbom.json
     
     optional arguments:
       -h, --help            show this help message and exit
       -n NOTES, --notes NOTES
                             /path/to/notes.yaml
       -o OUTPUT, --output OUTPUT
                             output format [table,json,yaml,raw]
@@ -88,32 +88,33 @@
         $ grype sbom:releasenotes/sbom/jupyter-base-notebook.syft.json --file releasenotes/sbom/jupyter-base-notebook.cdx.json --output embedded-cyclonedx-vex-json
 
 3. Use bogrod to analyze each vulnerability interactively
 
         # -- bogrod automatically uses the .grype report to provide additional information for each vulnerability 
         $ bogrod --work -S releasenotes/sbom/jupyter-base-notebook.cdx.json --vex-file releasenotes/sbom/vex.yaml --update-vex --merge-vex 
 
-Note that bogrod will automatically find the .vex and .grype files corresponding to the .cdx file,
+Note that bogrod will automatically find the .vex and .grype files corresponding to the .cdx file, 
 if these are not specified.
 
 Working with vulnerabilities
 ----------------------------
 
 Bogrod can work interactively with vulnerabilities found in a SBOM by specifying
 the -W command line option. This will present a list of the vulnerabilities found
 so that you can select and analyze each one in turn. 
 
     $ bogrod jupyter -W
 
-![bogrod demo](resources/demo1.jpg)
+![bogrod demo](resources/demo1.png)
 
-    Select 1
-![bogrod demo](resources/demo2.jpg)
+    Press Enter to show the details of the vulnerability
 
-    Save analysis and quit
+![bogrod demo](resources/demo2.png)
+
+    Save analysis and quit by pressing Ctrl-C or Q
 
 ![bogrod demo](resources/demo3.jpg)
 
 
 Working with multiple images
 ----------------------------
```

### Comparing `bogrod-0.4.0/bogrod/__init__.py` & `bogrod-0.4.1.dev1/bogrod/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,16 @@
                     if vuln_id not in sbom_vulns:
                         if vuln_id in related:
                             # append the reported vulnerability to the sbom
                             # -- take the first related vulnerability as the origin
                             related_vuln_id = related[vuln_id]['origins'][0]
                             self.add_vulnerability_from(vuln_id, related_vuln_id)
                         else:
-                            self.add_vulnerability(vuln_id, name=None, description=None, severity=reportedSeverity, url=None)
+                            self.add_vulnerability(vuln_id, name=None, description=None, severity=reportedSeverity,
+                                                   url=None)
             return vex_issues
 
     def add_vulnerability(self, vuln_id, name, description, severity, url):
         vuln = {
             'id': vuln_id,
             'bom-ref': uuid4().urn,
             'description': description or '(unknown, reported from bogrod)',
@@ -459,15 +460,15 @@
             }
             record = {k: record[k] for k in columns}
             data.append(record)
         severity_rank = lambda v: self.severities_order.index(v['severity'])
         data = sorted(data, key=severity_rank)
         return data
 
-    def report(self, format='table', stream=None, severities=None, columns=None, summary=False):
+    def report(self, format='table', stream=None, severities=None, columns=None, summary=False, fail_on_issues=False):
         data = self._generate_report_data(severities=severities, columns=columns)
         if summary:
             print("\nbogrod SBOM Summary Report\n")
             data, headers = tabulate_data(data, 'severity', ['state'])
         else:
             print("\nbogrod SBOM Report\n")
             headers = "keys"
@@ -476,14 +477,21 @@
         elif format == 'json':
             print(json.dumps(data), file=stream)
         elif format == 'yaml':
             print(yaml.safe_dump(data), file=stream)
         else:
             for rec in data:
                 print("{id:20} {severity:8} {note}".format(**rec))
+        if fail_on_issues:
+            is_open = lambda rec: rec.get('state') in ('in_triage', 'exploitable')
+            has_issues = lambda rec: '*' in rec.get('vulnerability', '*')
+            should_fail = any(is_open(rec) or has_issues(rec) for rec in data)
+            if should_fail:
+                print("ERROR: found open issues or unresolved vulnerabilities")
+                sys.exit(1)
 
     def _get_sbom_schema(self):
         # TODO get the actual schema
         schema_path = Path(__file__).parent / 'resources/bom-1.5.schema.json'
         with open(schema_path) as fin:
             schema = json.load(fin)
         return schema
@@ -649,17 +657,20 @@
                 'vuln_id': vuln_id,
                 'change': diff_data['delta'],
                 'description': diff_data['vuln']['affects'][0]
             })
         headers = 'keys'
         print(tabulate(data, headers=headers), file=stream)
 
+    def has_issues(self):
+        return
+
 
 def main(argv=None):
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(prog='bogrod')
     parser.add_argument('sbom',
                         help='/path/to/cyclonedx-sbom.json')
     parser.add_argument('-n', '--notes',
                         help='/path/to/notes.yaml')
     parser.add_argument('-o', '--output', default='table',
                         help='output format [table,json,yaml,raw]')
     parser.add_argument('-S', '--summary', action='store_true',
@@ -676,27 +687,26 @@
                         help='Merge vex data back to sbom')
     parser.add_argument('-w', '--write-notes',
                         action='store_true',
                         help='update notes according to sbom (add new, mark fixed)')
     parser.add_argument('-W', '--work',
                         action='store_true',
                         help='work each vulnerability')
-    parser.add_argument('--tui',
-                        action='store_true',
-                        help='use tui')
     parser.add_argument('-g', '--grype',
                         help='use grype SBOM to match vulnerabilities at /path/to/grype.json')
     parser.add_argument('--diff',
                         help='/path/to/cyclonedx-sbom.json')
     parser.add_argument('--vex-issues',
                         help='/path/to/vex-issues.yaml')
     parser.add_argument('--upload',
                         help='specify target aggregator to upload sbom and get issues report')
     parser.add_argument('--upload-tentative', action='store_true',
                         help='if specified upload sbom as tentative')
+    parser.add_argument('-F', '--fail-on-issues', action='store_true', dest='fail_on_issues',
+                        help='if there are pending issues or unresolved vulnerabilities, exit with error')
     args = parser.parse_args(argv)
 
     def write_vex_merge(vex_file):
         bogrod.write_vex(vex_file)
         if args.merge_vex:
             prop_data = None
             if args.sbom_properties:
@@ -826,21 +836,17 @@
         sbomID, report = aggregator.submit(args.projectpath, args.sbom, tentative=args.upload_tentative)
         with open(args.vex_issues, 'w') as fout:
             yaml.safe_dump(report, fout)
         aggregator.summary(sbomID, report)
         exit(0)
     if args.work:
         vex_file = args.vex_file or args.sbom
-        if sys.argv[0] == '-c' or args.tui:
-            from bogrod.tui.app import BogrodApp
-            bogrod.app = BogrodApp(bogrod=bogrod)
-            bogrod.app.run() if args.tui else None
-        else:
-            bogrod.work()
+        from bogrod.tui.app import BogrodApp
+        bogrod.app = BogrodApp(bogrod=bogrod)
+        bogrod.app.run()
         write_vex_merge(vex_file)
     else:
-        bogrod.report(format=args.output, summary=args.summary)
+        bogrod.report(format=args.output, summary=args.summary, fail_on_issues=args.fail_on_issues)
     return bogrod
 
 
-if __name__ == '__main__':
-    bogrod = main(sys.argv)
+
```

### Comparing `bogrod-0.4.0/bogrod/sbom.py` & `bogrod-0.4.1.dev1/bogrod/sbom.py`

 * *Files identical despite different names*

### Comparing `bogrod-0.4.0/bogrod/tests/test_bogrod.py` & `bogrod-0.4.1.dev1/bogrod/tests/test_bogrod.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,30 @@
+import contextlib
 import unittest
 from io import StringIO
-from pathlib import Path
 from unittest import skip
 
 import bogrod
-
 from bogrod import Bogrod
-
-BASE_PATH = Path(bogrod.__file__).parent.parent
+from bogrod.tests import BASE_PATH
 
 
 class BogrodTests(unittest.TestCase):
+    # TODO add more tests
+    def test_main(self):
+        f = StringIO()
+        with contextlib.redirect_stdout(f):
+            bogrod.main(['jupyter'])
+        output = f.getvalue()
+        self.assertIn('bogrod', output)
+
+    def test_contrib_base(self):
+        from bogrod.contrib import aggregators
+        self.assertIn('dummy', aggregators)
+
     @skip('functionality currently not working properly')
     def test_from_file(self):
         notes_file = BASE_PATH / 'releasenotes/notes/rc1-99e6a29d3335a383.yaml'
         notes_file_update = BASE_PATH / 'releasenotes/notes/rc1-99e6a29d3335a383-update.yaml'
         sbom = Bogrod.from_sbom(BASE_PATH / 'releasenotes/sbom/jupyter-base-notebook.json')
         sbom.read_notes(notes_file)
         # check previous release with known security issue present
```

### Comparing `bogrod-0.4.0/bogrod/util.py` & `bogrod-0.4.1.dev1/bogrod/util.py`

 * *Files identical despite different names*

### Comparing `bogrod-0.4.0/bogrod.egg-info/PKG-INFO` & `bogrod-0.4.1.dev1/bogrod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bogrod
-Version: 0.4.0
+Version: 0.4.1.dev1
 Summary: Manage SBOM, VEX records and release notes in a single tool
 Home-page: https://github.com/productaize/bogrod
 Author: Patrick Senti
 Author-email: patrick@productaize.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,14 +12,20 @@
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
 Requires-Dist: attrdict
 Requires-Dist: textual
 Requires-Dist: textual-dev
 Requires-Dist: requests
 Requires-Dist: yaspin
+Requires-Dist: keyring
+Provides-Extra: dev
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest-textual-snapshot; extra == "dev"
 
 Bogrod
 ======
 
 Manage vulnerabilities analysis (VEX/SBOM) in cyclonedx format like source code.
 
 Why?
@@ -61,15 +67,15 @@
 ------
 
 Run as a command line utility:
 
     usage: bogrod [-h] [-n NOTES] [-o OUTPUT] [-S] [-s SEVERITIES] [-x] [--vex-file VEX_FILE] [-p SBOM_PROPERTIES] [-m] [-w] [-W] [-g GRYPE] sbom
 
     positional arguments:
-      sbom                  /path/to/cyclonedx-sbom.json
+      sbom                  name of sbom in .bogrod, or /path/to/cyclonedx-sbom.json
     
     optional arguments:
       -h, --help            show this help message and exit
       -n NOTES, --notes NOTES
                             /path/to/notes.yaml
       -o OUTPUT, --output OUTPUT
                             output format [table,json,yaml,raw]
@@ -107,32 +113,33 @@
         $ grype sbom:releasenotes/sbom/jupyter-base-notebook.syft.json --file releasenotes/sbom/jupyter-base-notebook.cdx.json --output embedded-cyclonedx-vex-json
 
 3. Use bogrod to analyze each vulnerability interactively
 
         # -- bogrod automatically uses the .grype report to provide additional information for each vulnerability 
         $ bogrod --work -S releasenotes/sbom/jupyter-base-notebook.cdx.json --vex-file releasenotes/sbom/vex.yaml --update-vex --merge-vex 
 
-Note that bogrod will automatically find the .vex and .grype files corresponding to the .cdx file,
+Note that bogrod will automatically find the .vex and .grype files corresponding to the .cdx file, 
 if these are not specified.
 
 Working with vulnerabilities
 ----------------------------
 
 Bogrod can work interactively with vulnerabilities found in a SBOM by specifying
 the -W command line option. This will present a list of the vulnerabilities found
 so that you can select and analyze each one in turn. 
 
     $ bogrod jupyter -W
 
-![bogrod demo](resources/demo1.jpg)
+![bogrod demo](resources/demo1.png)
 
-    Select 1
-![bogrod demo](resources/demo2.jpg)
+    Press Enter to show the details of the vulnerability
 
-    Save analysis and quit
+![bogrod demo](resources/demo2.png)
+
+    Save analysis and quit by pressing Ctrl-C or Q
 
 ![bogrod demo](resources/demo3.jpg)
 
 
 Working with multiple images
 ----------------------------
```

