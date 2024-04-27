# Comparing `tmp/xl2roefact-0.6.tar.gz` & `tmp/xl2roefact-0.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2roefact-0.6.tar", last modified: Sat Apr 27 02:50:14 2024, max compression
+gzip compressed data, was "xl2roefact-0.6rc0.tar", last modified: Sat Apr 20 01:23:45 2024, max compression
```

## Comparing `xl2roefact-0.6.tar` & `xl2roefact-0.6rc0.tar`

### file list

```diff
@@ -1,14 +1,27 @@
--rw-r--r--   0        0        0    35149 2024-04-27 02:49:49.223353 xl2roefact-0.6/LICENSE
--rw-r--r--   0        0        0    18839 2024-04-27 02:49:49.223353 xl2roefact-0.6/README.md
--rw-r--r--   0        0        0     3333 2024-04-27 02:50:14.076239 xl2roefact-0.6/pyproject.toml
--rw-r--r--   0        0        0     1808 2024-04-27 02:49:49.675370 xl2roefact-0.6/src/data/README_app_config_rules.md
--rw-r--r--   0        0        0        1 2024-04-27 02:49:49.675370 xl2roefact-0.6/src/data/__init__.py
--rw-r--r--   0        0        0     7134 2024-04-27 02:49:49.675370 xl2roefact-0.6/src/data/app_settings.yml
--rw-r--r--   0        0        0        1 2024-04-27 02:49:49.675370 xl2roefact-0.6/tests/.gitkeep
--rw-r--r--   0        0        0    21688 2024-04-27 02:49:49.675370 xl2roefact-0.6/tests/Fact_Petrom_11017969.json
--rw-r--r--   0        0        0   268862 2024-04-27 02:49:49.679370 xl2roefact-0.6/tests/Fact_Petrom_11017969.xlsx
--rw-r--r--   0        0        0    15740 2024-04-27 02:49:49.679370 xl2roefact-0.6/tests/Fact_Petrom_11017969.xml
--rw-r--r--   0        0        0      986 2024-04-27 02:49:49.679370 xl2roefact-0.6/tests/_test_results.txt
--rw-r--r--   0        0        0    24150 2024-04-27 02:49:49.679370 xl2roefact-0.6/tests/fact_RENF1004.json
--rw-r--r--   0        0        0    16332 2024-04-27 02:49:49.679370 xl2roefact-0.6/tests/fact_RENF1004.xlsx
--rw-r--r--   0        0        0    61434 1970-01-01 00:00:00.000000 xl2roefact-0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-20 01:23:19.951218 xl2roefact-0.6rc0/LICENSE
+-rw-r--r--   0        0        0    18602 2024-04-20 01:23:19.951218 xl2roefact-0.6rc0/README.md
+-rw-r--r--   0        0        0     3364 2024-04-20 01:23:45.699419 xl2roefact-0.6rc0/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/.gitkeep
+-rw-r--r--   0        0        0    21622 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.json
+-rw-r--r--   0        0        0   268862 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xlsx
+-rw-r--r--   0        0        0    15740 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xml
+-rw-r--r--   0        0        0      986 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/_test_results.txt
+-rw-r--r--   0        0        0    24084 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/fact_RENF1004.json
+-rw-r--r--   0        0        0    16332 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/fact_RENF1004.xlsx
+-rw-r--r--   0        0        0     1531 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/todosXML.md
+-rw-r--r--   0        0        0      567 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__main__.py
+-rw-r--r--   0        0        0     1500 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__version__.py
+-rw-r--r--   0        0        0     7913 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/app_cli.py
+-rw-r--r--   0        0        0      727 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/chkisld.py
+-rw-r--r--   0        0        0      584 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/chkxml.py
+-rw-r--r--   0        0        0     8915 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/config_settings.py
+-rw-r--r--   0        0        0     1808 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/README_app_config_rules.md
+-rw-r--r--   0        0        0        1 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/__init__.py
+-rw-r--r--   0        0        0     7134 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/app_settings.yml
+-rw-r--r--   0        0        0      600 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/ldxml.py
+-rw-r--r--   0        0        0    10480 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/libutils.py
+-rw-r--r--   0        0        0    71476 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/rdinv.py
+-rw-r--r--   0        0        0     1319 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/sys_settings.py
+-rw-r--r--   0        0        0      612 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/wrxml.py
+-rw-r--r--   0        0        0    61200 1970-01-01 00:00:00.000000 xl2roefact-0.6rc0/PKG-INFO
```

### Comparing `xl2roefact-0.6/LICENSE` & `xl2roefact-0.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/README.md` & `xl2roefact-0.6rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![Static Badge](https://img.shields.io/badge/version-{{ xl2roefact_version }}-blue)
 
 Legaturi externe utile:
 
 * [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
 * [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
 * [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
-* [Referinta *dezvoltare software - biblioteca Python*](https://invoicetoroefact.renware.eu/xl2roefact/doc/README_xl2roefact_library.html)
+* [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
 * [Referinta *API*](https://invoicetoroefact.renware.eu/xl2roefact/doc/wrapper_810.05a-xl2roefact_DLD_specs.html)
 <!--Refrence to source doc. If used like that, then must be resolved with an external tool before generating a complete README.html doc. The `mkdoxs` is able to do that but in `PyPi` published version will be unusable
 (./doc/810.05a-xl2roefact_DLD_specs.md)
 -->
 
 
 ## Facilitati
@@ -199,15 +199,15 @@
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
 <!--#NOTE: next section generate application commands in same style as obtained using `--help` CLI options -->
 ::: mkdocs-typer
-    :module: xl2roefact.src.app_cli
+    :module: xl2roefact.app_cli
     :command: app_cli
     :prog_name: xl2roefact
     :depth: 2
 
 
 
 
@@ -223,15 +223,15 @@
 >
 >* una este valoarea introdusa intr-o celula (de ex cu 3 zecimale) si
 >* alta este valoarea afisata (cu 2 zecimale) - aceasta din urma trebuie obtinuta prin formatarea celulei respective de a afisa 2 zecimale prin rotunjire insa valoarea efectiva trebuie sa fie cea originala cu 3 zecimale, lucru (diferenta) care se poate vedea la editarea continutului celulei.
 
 
 ### Reguli recomamdate in configurarea aplicatiei pe specificul Excel al facturilor dumneavoastra
 
-{% include './src/data/README_app_config_rules.md' %}
+{% include './xl2roefact/data/README_app_config_rules.md' %}
 
 
 
 
 ## Tutorial utilizare aplicatie
 
 
@@ -307,41 +307,36 @@
 * **`Invoice`** - datele efective ale facturii
 * **`meta_info`**
     * informatii referitoare la procesarea facturii si mapa de conversie a cheii `Invoice` din formatul `JSON` in formatul `XML` cerut de sistemul *RO E-Fact*
     * harta de ajutor in conversia formatului JSON in formatul XML acceptat de sistemul RO E-Fact (cheie `meta_info.map_JSONkeys_XMLtags`) si definititiile XML aferente (cheie `meta_info.invoice_XML_schemes`)
     * alte informatii despre fisierul Excel prelucrat (numele, worksheet cu factura, data si ora procesarii, CRC pentru verificare, etc)
 * **`excel_original_data`** - informatiile originale din fisierul Excel, asa cum au fost ele identificate si gasite precum si locatia (adresele celulelor). Aceste informatii sunt utile in cazul in care exista neclaritati in urma procesuluicde conversie pentru "a intelege" de unde si cum arata informatiile originale din fisierul Excel
 
-Detalii suplimentare despre formatul JSON se gasesc in documentaţia *[Referinta dezvoltare software](./doc/README_xl2roefact_library.md)*.
+<small markdown="1">Pentru detalii suplimentare despre formatul JSON trebyie consultata componenta referitoare la ***[biblioteca `xl2roefact` destinata dezvoltarii software](./doc/README_xl2roefact_library.md)***.</small>
 
 
 
 
 ## Descarcare (download) aplicatie xl2roefact CLI
 
 * [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
 * [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
 * [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
 * [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
 
 
 
 
-## Referinta dezvoltare software
-
-Documentatia **["Referinta dezvoltare software"](./doc/README_xl2roefact_library.md)** ofera detail necesare pentru utilizarea bibliotecii sursa in dezvoltari specifice, extindere si integrare cu alte sisteme.
-
-
 
 
 ## Date identificare
 
 * part number (p/n): `0000-0095-xl2roefact`
-* producator si copyright: RENWare Software Systems (referinte detalii tehnice: Petre Iordanescu, *petre.iordanescu@gmail.com*)
-
+* producator si copyright: RENWare Software Systems
+* author: Petre Iordanescu (petre.iordanescu@gmail.com)
 
 
 
 ## [License](./LICENSE "download")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xl2roefact-0.6/pyproject.toml` & `xl2roefact-0.6rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,40 +51,40 @@
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
 ]
-version = "0.6"
+version = "0.6rc0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://invoicetoroefact.renware.eu"
 PDF-Documentation = "https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf"
 PyPi-Package = "https://pypi.org/project/xl2roefact/"
 GitHub = "https://github.com/petre-renware/api_to_roefact"
 
 [project.scripts]
-xl2roefact = "src.app_cli:main"
+xl2roefact = "xl2roefact.app_cli:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.version]
 source = "file"
-path = "src/__version__.py"
+path = "xl2roefact/__version__.py"
 
 [tool.pdm.build.wheel-data]
 data = [
     { path = "data/*", relative-to = "data/" },
 ]
 
 [tool.pdm.scripts.build_wheel]
@@ -104,18 +104,18 @@
     "--log-level=WARN",
     "--onefile",
     "--noconfirm",
     "xl2roefact_copy_for_sexe.py",
 ]
 
 [tool.pdm.scripts.post_build_sexe]
-call = "src.libutils:complete_sexe_file"
+call = "xl2roefact.libutils:complete_sexe_file"
 
 [tool.pdm.scripts.build_doc]
-shell = "pydoc-markdown -I src >doc/810.05a-xl2roefact_DLD_specs.md"
+shell = "pydoc-markdown -I xl2roefact >doc/810.05a-xl2roefact_DLD_specs.md"
 
 [tool.pdm.scripts.build_all]
 composite = [
     "build_wheel",
     "build_msi",
     "build_sexe",
     "build_doc",
```

### Comparing `xl2roefact-0.6/src/data/README_app_config_rules.md` & `xl2roefact-0.6rc0/xl2roefact/data/README_app_config_rules.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/src/data/app_settings.yml` & `xl2roefact-0.6rc0/xl2roefact/data/app_settings.yml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/tests/Fact_Petrom_11017969.json` & `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735119047619047%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'proccesed @2024-04-18T04:10:02.798583+00:00 with xl2roefact', delete: "*

 * *              "['cbc_InvoiceTypeCode']}",*

 * * "'meta_info'": "{'last_processing_time': '2024-04-18T04:10:02.798215+00:00', "*

 * *                "'map_JSONkeys_XMLtags': {insert: [(47, ['cbc_InvoiceTypeCode', "*

 * *                "'cbc:InvoiceTypeCode'])], delete: [54]}}"}*

```diff
@@ -169,17 +169,16 @@
                 }
             ],
             "cbc_TaxAmount": 8123.66
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-11-16",
         "cbc_ID": "11017969",
-        "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-10-17",
-        "cbc_Note": "generated @2024-04-26T07:07:20.592596+00:00 with xl2roefact by RENware Software Systems",
+        "cbc_Note": "proccesed @2024-04-18T04:10:02.798583+00:00 with xl2roefact",
         "cbc_TaxPointDate": "2023-11-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 49,
                 8
@@ -485,15 +484,15 @@
         "invoice_max_rows": 49,
         "invoice_worksheet": "Factura(Invoice)",
         "items_table_start_cell": [
             29,
             1
         ],
         "items_table_start_marker": "No. crt.",
-        "last_processing_time": "2024-04-26T07:07:20.592195+00:00",
+        "last_processing_time": "2024-04-18T04:10:02.798215+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
@@ -676,14 +675,18 @@
                 "cac:PartyTaxScheme"
             ],
             [
                 "cbc_DueDate",
                 "cbc:DueDate"
             ],
             [
+                "cbc_InvoiceTypeCode",
+                "cbc:InvoiceTypeCode"
+            ],
+            [
                 "cbc_Note",
                 "cbc:Note"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
             ],
@@ -702,15 +705,11 @@
             [
                 "cbc_PaymentMeansCode",
                 "cbc:PaymentMeansCode"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
-            ],
-            [
-                "cbc_InvoiceTypeCode",
-                "cbc:InvoiceTypeCode"
             ]
         ]
     }
 }
```

### Comparing `xl2roefact-0.6/tests/Fact_Petrom_11017969.xlsx` & `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/tests/Fact_Petrom_11017969.xml` & `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/tests/_test_results.txt` & `xl2roefact-0.6rc0/tests/_test_results.txt`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/tests/fact_RENF1004.json` & `xl2roefact-0.6rc0/tests/fact_RENF1004.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735119047619047%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'proccesed @2024-04-18T04:10:02.876896+00:00 with xl2roefact', delete: "*

 * *              "['cbc_InvoiceTypeCode']}",*

 * * "'meta_info'": "{'last_processing_time': '2024-04-18T04:10:02.876450+00:00', "*

 * *                "'map_JSONkeys_XMLtags': {insert: [(47, ['cbc_InvoiceTypeCode', "*

 * *                "'cbc:InvoiceTypeCode'])], delete: [54]}}"}*

```diff
@@ -196,17 +196,16 @@
                 }
             ],
             "cbc_TaxAmount": 7389.15
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-09-27",
         "cbc_ID": "RENF-1004",
-        "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-08-28",
-        "cbc_Note": "generated @2024-04-26T07:07:20.704934+00:00 with xl2roefact by RENware Software Systems",
+        "cbc_Note": "proccesed @2024-04-18T04:10:02.876896+00:00 with xl2roefact",
         "cbc_TaxPointDate": "2023-09-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 31,
                 9
@@ -560,15 +559,15 @@
         "invoice_max_rows": 31,
         "invoice_worksheet": "FACTURA FINALA",
         "items_table_start_cell": [
             20,
             1
         ],
         "items_table_start_marker": "#",
-        "last_processing_time": "2024-04-26T07:07:20.704495+00:00",
+        "last_processing_time": "2024-04-18T04:10:02.876450+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
@@ -751,14 +750,18 @@
                 "cac:PartyTaxScheme"
             ],
             [
                 "cbc_DueDate",
                 "cbc:DueDate"
             ],
             [
+                "cbc_InvoiceTypeCode",
+                "cbc:InvoiceTypeCode"
+            ],
+            [
                 "cbc_Note",
                 "cbc:Note"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
             ],
@@ -777,15 +780,11 @@
             [
                 "cbc_PaymentMeansCode",
                 "cbc:PaymentMeansCode"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
-            ],
-            [
-                "cbc_InvoiceTypeCode",
-                "cbc:InvoiceTypeCode"
             ]
         ]
     }
 }
```

### Comparing `xl2roefact-0.6/tests/fact_RENF1004.xlsx` & `xl2roefact-0.6rc0/tests/fact_RENF1004.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6/PKG-INFO` & `xl2roefact-0.6rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2roefact
-Version: 0.6
+Version: 0.6rc0
 Summary: Excel invoices data retrieve, export & upload to RO E-Fact system
 Author-Email: Petre Iordanescu <petre.iordanescu@gmail.com>, RENware Software Systems <renware.systems@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -734,15 +734,15 @@
 ![Static Badge](https://img.shields.io/badge/version-{{ xl2roefact_version }}-blue)
 
 Legaturi externe utile:
 
 * [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
 * [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
 * [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
-* [Referinta *dezvoltare software - biblioteca Python*](https://invoicetoroefact.renware.eu/xl2roefact/doc/README_xl2roefact_library.html)
+* [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
 * [Referinta *API*](https://invoicetoroefact.renware.eu/xl2roefact/doc/wrapper_810.05a-xl2roefact_DLD_specs.html)
 <!--Refrence to source doc. If used like that, then must be resolved with an external tool before generating a complete README.html doc. The `mkdoxs` is able to do that but in `PyPi` published version will be unusable
 (./doc/810.05a-xl2roefact_DLD_specs.md)
 -->
 
 
 ## Facilitati
@@ -928,15 +928,15 @@
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
 <!--#NOTE: next section generate application commands in same style as obtained using `--help` CLI options -->
 ::: mkdocs-typer
-    :module: xl2roefact.src.app_cli
+    :module: xl2roefact.app_cli
     :command: app_cli
     :prog_name: xl2roefact
     :depth: 2
 
 
 
 
@@ -952,15 +952,15 @@
 >
 >* una este valoarea introdusa intr-o celula (de ex cu 3 zecimale) si
 >* alta este valoarea afisata (cu 2 zecimale) - aceasta din urma trebuie obtinuta prin formatarea celulei respective de a afisa 2 zecimale prin rotunjire insa valoarea efectiva trebuie sa fie cea originala cu 3 zecimale, lucru (diferenta) care se poate vedea la editarea continutului celulei.
 
 
 ### Reguli recomamdate in configurarea aplicatiei pe specificul Excel al facturilor dumneavoastra
 
-{% include './src/data/README_app_config_rules.md' %}
+{% include './xl2roefact/data/README_app_config_rules.md' %}
 
 
 
 
 ## Tutorial utilizare aplicatie
 
 
@@ -1036,41 +1036,36 @@
 * **`Invoice`** - datele efective ale facturii
 * **`meta_info`**
     * informatii referitoare la procesarea facturii si mapa de conversie a cheii `Invoice` din formatul `JSON` in formatul `XML` cerut de sistemul *RO E-Fact*
     * harta de ajutor in conversia formatului JSON in formatul XML acceptat de sistemul RO E-Fact (cheie `meta_info.map_JSONkeys_XMLtags`) si definititiile XML aferente (cheie `meta_info.invoice_XML_schemes`)
     * alte informatii despre fisierul Excel prelucrat (numele, worksheet cu factura, data si ora procesarii, CRC pentru verificare, etc)
 * **`excel_original_data`** - informatiile originale din fisierul Excel, asa cum au fost ele identificate si gasite precum si locatia (adresele celulelor). Aceste informatii sunt utile in cazul in care exista neclaritati in urma procesuluicde conversie pentru "a intelege" de unde si cum arata informatiile originale din fisierul Excel
 
-Detalii suplimentare despre formatul JSON se gasesc in documentaţia *[Referinta dezvoltare software](./doc/README_xl2roefact_library.md)*.
+<small markdown="1">Pentru detalii suplimentare despre formatul JSON trebyie consultata componenta referitoare la ***[biblioteca `xl2roefact` destinata dezvoltarii software](./doc/README_xl2roefact_library.md)***.</small>
 
 
 
 
 ## Descarcare (download) aplicatie xl2roefact CLI
 
 * [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
 * [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
 * [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
 * [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
 
 
 
 
-## Referinta dezvoltare software
-
-Documentatia **["Referinta dezvoltare software"](./doc/README_xl2roefact_library.md)** ofera detail necesare pentru utilizarea bibliotecii sursa in dezvoltari specifice, extindere si integrare cu alte sisteme.
-
-
 
 
 ## Date identificare
 
 * part number (p/n): `0000-0095-xl2roefact`
-* producator si copyright: RENWare Software Systems (referinte detalii tehnice: Petre Iordanescu, *petre.iordanescu@gmail.com*)
-
+* producator si copyright: RENWare Software Systems
+* author: Petre Iordanescu (petre.iordanescu@gmail.com)
 
 
 
 ## [License](./LICENSE "download")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

