# Comparing `tmp/codelimit-0.9.2.tar.gz` & `tmp/codelimit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelimit-0.9.2.tar", max compression
+gzip compressed data, was "codelimit-0.9.3.tar", max compression
```

## Comparing `codelimit-0.9.2.tar` & `codelimit-0.9.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    32423 2024-04-19 08:59:08.938110 codelimit-0.9.2/LICENSE
--rw-r--r--   0        0        0     2710 2024-04-19 08:59:08.938110 codelimit-0.9.2/README.md
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/__init__.py
--rwxr-xr-x   0        0        0     2253 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/__main__.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/commands/__init__.py
--rw-r--r--   0        0        0     1457 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/commands/app.py
--rw-r--r--   0        0        0     1968 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/commands/check.py
--rw-r--r--   0        0        0     1457 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/commands/report.py
--rw-r--r--   0        0        0     1303 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/commands/scan.py
--rw-r--r--   0        0        0     1211 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/commands/upload.py
--rw-r--r--   0        0        0     1627 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/CheckResult.py
--rw-r--r--   0        0        0     2303 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Codebase.py
--rw-r--r--   0        0        0      503 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/CodebseEntry.py
--rw-r--r--   0        0        0      566 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Configuration.py
--rw-r--r--   0        0        0      559 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Language.py
--rw-r--r--   0        0        0      643 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/LanguageTotals.py
--rw-r--r--   0        0        0     1166 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Location.py
--rw-r--r--   0        0        0      186 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Measurement.py
--rw-r--r--   0        0        0     1581 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/ScanResultTable.py
--rw-r--r--   0        0        0     1406 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/ScanTotals.py
--rw-r--r--   0        0        0     7184 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Scanner.py
--rw-r--r--   0        0        0      331 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/SourceFile.py
--rw-r--r--   0        0        0      873 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/SourceFileEntry.py
--rw-r--r--   0        0        0      535 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/SourceFolder.py
--rw-r--r--   0        0        0      255 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/SourceFolderEntry.py
--rw-r--r--   0        0        0     1333 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/Token.py
--rw-r--r--   0        0        0     1256 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/TokenRange.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/Expression.py
--rw-r--r--   0        0        0      453 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/Pattern.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/__init__.py
--rw-r--r--   0        0        0      263 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/automata/Automata.py
--rw-r--r--   0        0        0      450 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/automata/DFA.py
--rw-r--r--   0        0        0      444 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/automata/NFA.py
--rw-r--r--   0        0        0      876 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/automata/State.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/automata/__init__.py
--rw-r--r--   0        0        0     3825 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/matcher.py
--rw-r--r--   0        0        0      721 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/Atom.py
--rw-r--r--   0        0        0      389 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/Concat.py
--rw-r--r--   0        0        0      702 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/OneOrMore.py
--rw-r--r--   0        0        0      182 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/Operator.py
--rw-r--r--   0        0        0      701 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/Optional.py
--rw-r--r--   0        0        0      854 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/Union.py
--rw-r--r--   0        0        0      714 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/ZeroOrMore.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/operator/__init__.py
--rw-r--r--   0        0        0      521 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/predicate/Identity.py
--rw-r--r--   0        0        0      336 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/predicate/Predicate.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/predicate/__init__.py
--rw-r--r--   0        0        0     2032 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/gsm/utils.py
--rw-r--r--   0        0        0     1013 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/lexer_utils.py
--rw-r--r--   0        0        0     1583 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/report/Report.py
--rw-r--r--   0        0        0     1343 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/report/ReportReader.py
--rw-r--r--   0        0        0      162 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/report/ReportUnit.py
--rw-r--r--   0        0        0     5087 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/report/ReportWriter.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/report/__init__.py
--rw-r--r--   0        0        0      155 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/scope/Header.py
--rw-r--r--   0        0        0     1227 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/scope/Scope.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/scope/__init__.py
--rw-r--r--   0        0        0     5506 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/scope/scope_utils.py
--rw-r--r--   0        0        0     2083 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/source_utils.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/__init__.py
--rw-r--r--   0        0        0     1404 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/Balanced.py
--rw-r--r--   0        0        0      875 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/Choice.py
--rw-r--r--   0        0        0      659 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/Keyword.py
--rw-r--r--   0        0        0      444 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/Name.py
--rw-r--r--   0        0        0      635 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/Operator.py
--rw-r--r--   0        0        0      629 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/Symbol.py
--rw-r--r--   0        0        0      364 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/TokenPredicate.py
--rw-r--r--   0        0        0      628 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/TokenValue.py
--rw-r--r--   0        0        0        0 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_matching/predicate/__init__.py
--rw-r--r--   0        0        0     1621 2024-04-19 08:59:08.938110 codelimit-0.9.2/codelimit/common/token_utils.py
--rw-r--r--   0        0        0     5762 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/common/utils.py
--rw-r--r--   0        0        0     3139 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/github_auth.py
--rw-r--r--   0        0        0      926 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/C.py
--rw-r--r--   0        0        0      858 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/Cpp.py
--rw-r--r--   0        0        0      707 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/Java.py
--rw-r--r--   0        0        0     1086 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/JavaScript.py
--rw-r--r--   0        0        0     3018 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/Python.py
--rw-r--r--   0        0        0     1610 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/TypeScript.py
--rw-r--r--   0        0        0      236 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/languages/__init__.py
--rw-r--r--   0        0        0     1911 2024-04-19 08:59:08.942110 codelimit-0.9.2/codelimit/utils.py
--rw-r--r--   0        0        0       18 2024-04-19 08:59:34.082136 codelimit-0.9.2/codelimit/version.py
--rw-r--r--   0        0        0     1154 2024-04-19 08:59:34.082136 codelimit-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 codelimit-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    32423 2024-04-27 21:06:06.903355 codelimit-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2710 2024-04-27 21:06:06.903355 codelimit-0.9.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/__init__.py
+-rwxr-xr-x   0        0        0     2253 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/commands/__init__.py
+-rw-r--r--   0        0        0     1457 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/commands/app.py
+-rw-r--r--   0        0        0     2062 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/commands/check.py
+-rw-r--r--   0        0        0     1457 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/commands/report.py
+-rw-r--r--   0        0        0     1303 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/commands/scan.py
+-rw-r--r--   0        0        0     1211 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/commands/upload.py
+-rw-r--r--   0        0        0     1627 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/common/CheckResult.py
+-rw-r--r--   0        0        0     2303 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/common/Codebase.py
+-rw-r--r--   0        0        0      503 2024-04-27 21:06:06.903355 codelimit-0.9.3/codelimit/common/CodebseEntry.py
+-rw-r--r--   0        0        0      566 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/Configuration.py
+-rw-r--r--   0        0        0      559 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/Language.py
+-rw-r--r--   0        0        0      643 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/LanguageTotals.py
+-rw-r--r--   0        0        0     1166 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/Location.py
+-rw-r--r--   0        0        0      186 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/Measurement.py
+-rw-r--r--   0        0        0     1581 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/ScanResultTable.py
+-rw-r--r--   0        0        0     1406 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/ScanTotals.py
+-rw-r--r--   0        0        0     7285 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/Scanner.py
+-rw-r--r--   0        0        0      331 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/SourceFile.py
+-rw-r--r--   0        0        0      873 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/SourceFileEntry.py
+-rw-r--r--   0        0        0      535 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/SourceFolder.py
+-rw-r--r--   0        0        0      255 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/SourceFolderEntry.py
+-rw-r--r--   0        0        0     1333 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/Token.py
+-rw-r--r--   0        0        0     1256 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/TokenRange.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/Expression.py
+-rw-r--r--   0        0        0      453 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/Pattern.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/automata/Automata.py
+-rw-r--r--   0        0        0      450 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/automata/DFA.py
+-rw-r--r--   0        0        0      444 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/automata/NFA.py
+-rw-r--r--   0        0        0      876 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/automata/State.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/automata/__init__.py
+-rw-r--r--   0        0        0     3825 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/matcher.py
+-rw-r--r--   0        0        0      721 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/Atom.py
+-rw-r--r--   0        0        0      389 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/Concat.py
+-rw-r--r--   0        0        0      702 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/OneOrMore.py
+-rw-r--r--   0        0        0      182 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/Operator.py
+-rw-r--r--   0        0        0      701 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/Optional.py
+-rw-r--r--   0        0        0      854 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/Union.py
+-rw-r--r--   0        0        0      714 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/ZeroOrMore.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/operator/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/predicate/Identity.py
+-rw-r--r--   0        0        0      336 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/predicate/Predicate.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/predicate/__init__.py
+-rw-r--r--   0        0        0     2032 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/gsm/utils.py
+-rw-r--r--   0        0        0     1013 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/lexer_utils.py
+-rw-r--r--   0        0        0     1583 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/report/Report.py
+-rw-r--r--   0        0        0     1343 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/report/ReportReader.py
+-rw-r--r--   0        0        0      162 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/report/ReportUnit.py
+-rw-r--r--   0        0        0     5087 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/report/ReportWriter.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/report/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/scope/Header.py
+-rw-r--r--   0        0        0     1227 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/scope/Scope.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/scope/__init__.py
+-rw-r--r--   0        0        0     5506 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/scope/scope_utils.py
+-rw-r--r--   0        0        0     2083 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/source_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/__init__.py
+-rw-r--r--   0        0        0     1404 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/Balanced.py
+-rw-r--r--   0        0        0      875 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/Choice.py
+-rw-r--r--   0        0        0      659 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/Keyword.py
+-rw-r--r--   0        0        0      444 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/Name.py
+-rw-r--r--   0        0        0      635 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/Operator.py
+-rw-r--r--   0        0        0      629 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/Symbol.py
+-rw-r--r--   0        0        0      364 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/TokenPredicate.py
+-rw-r--r--   0        0        0      628 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/TokenValue.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_matching/predicate/__init__.py
+-rw-r--r--   0        0        0     1621 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/token_utils.py
+-rw-r--r--   0        0        0     5762 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/common/utils.py
+-rw-r--r--   0        0        0     3139 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/github_auth.py
+-rw-r--r--   0        0        0      926 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/C.py
+-rw-r--r--   0        0        0      858 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/Cpp.py
+-rw-r--r--   0        0        0      707 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/Java.py
+-rw-r--r--   0        0        0     1086 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/JavaScript.py
+-rw-r--r--   0        0        0     3018 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/Python.py
+-rw-r--r--   0        0        0     1610 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/TypeScript.py
+-rw-r--r--   0        0        0      236 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/languages/__init__.py
+-rw-r--r--   0        0        0     1911 2024-04-27 21:06:06.907355 codelimit-0.9.3/codelimit/utils.py
+-rw-r--r--   0        0        0       18 2024-04-27 21:06:39.583535 codelimit-0.9.3/codelimit/version.py
+-rw-r--r--   0        0        0     1154 2024-04-27 21:06:39.583535 codelimit-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 codelimit-0.9.3/PKG-INFO
```

### Comparing `codelimit-0.9.2/LICENSE` & `codelimit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/README.md` & `codelimit-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/__main__.py` & `codelimit-0.9.3/codelimit/__main__.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/commands/app.py` & `codelimit-0.9.3/codelimit/commands/app.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/commands/check.py` & `codelimit-0.9.3/codelimit/commands/check.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from pathlib import Path
 
 import typer
 from pygments.lexers import get_lexer_for_filename
+from pygments.util import ClassNotFound
 
 from codelimit.common.CheckResult import CheckResult
 from codelimit.common.Scanner import is_excluded, scan_file
 from codelimit.common.lexer_utils import lex
 from codelimit.common.utils import load_language_by_name
 from codelimit.languages import language_names
 
@@ -33,15 +34,18 @@
             or check_result.unmaintainable > 0
     ):
         check_result.report()
     raise typer.Exit(code=exit_code)
 
 
 def check_file(path: Path, check_result: CheckResult):
-    lexer = get_lexer_for_filename(path)
+    try:
+        lexer = get_lexer_for_filename(path)
+    except ClassNotFound:
+        return
     lexer_name = lexer.__class__.name
     if lexer_name in language_names:
         with open(path) as f:
             code = f.read()
         tokens = lex(lexer, code, False)
         lexer_name = load_language_by_name(lexer.__class__.name)
         if lexer_name:
```

### Comparing `codelimit-0.9.2/codelimit/commands/report.py` & `codelimit-0.9.3/codelimit/commands/report.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/commands/scan.py` & `codelimit-0.9.3/codelimit/commands/scan.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/commands/upload.py` & `codelimit-0.9.3/codelimit/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/CheckResult.py` & `codelimit-0.9.3/codelimit/common/CheckResult.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/Codebase.py` & `codelimit-0.9.3/codelimit/common/Codebase.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/Configuration.py` & `codelimit-0.9.3/codelimit/common/Configuration.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/Language.py` & `codelimit-0.9.3/codelimit/common/Language.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/LanguageTotals.py` & `codelimit-0.9.3/codelimit/common/LanguageTotals.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/Location.py` & `codelimit-0.9.3/codelimit/common/Location.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/ScanResultTable.py` & `codelimit-0.9.3/codelimit/common/ScanResultTable.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/ScanTotals.py` & `codelimit-0.9.3/codelimit/common/ScanTotals.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/Scanner.py` & `codelimit-0.9.3/codelimit/common/Scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,32 +45,36 @@
         def add_file_entry(entry: SourceFileEntry):
             scan_totals.add(entry)
             table = ScanResultTable(scan_totals)
             live.update(table)
 
         _scan_folder(codebase, path, cached_report, add_file_entry)
     if len(scan_totals.languages()) > 1:
-        print_footer(scan_totals)
+        print_totals(scan_totals)
+    print_refactor_candidates(scan_totals)
     return codebase
 
 
 def print_header(cached_report, path):
     print(f"  [bold]Code Limit[/bold]: {version}")
     print(
         f"  [bold]Scan date[/bold]: {datetime.now().isoformat(sep=' ', timespec='seconds')}"
     )
     print(f"  [bold]Scan root[/bold]: {path.resolve().absolute()}")
     if cached_report:
         print("  [bold]Found cached report, only analyzing changed files[/bold]")
 
 
-def print_footer(scan_totals: ScanTotals):
+def print_totals(scan_totals: ScanTotals):
     print(f"  [bold]Total lines of code[/bold]: {scan_totals.total_loc():n}")
     print(f"  [bold]Total files[/bold]: {scan_totals.total_files():n}")
     print(f"  [bold]Total functions[/bold]: {scan_totals.total_functions():n}")
+
+
+def print_refactor_candidates(scan_totals: ScanTotals):
     total_hard_to_maintain = scan_totals.total_hard_to_maintain()
     if total_hard_to_maintain > 0:
         print(
             f"  [dark_orange]\u26A0[/dark_orange] {total_hard_to_maintain} functions are hard-to-maintain."
         )
     total_unmaintainable = scan_totals.total_unmaintainable()
     if total_unmaintainable > 0:
```

### Comparing `codelimit-0.9.2/codelimit/common/SourceFileEntry.py` & `codelimit-0.9.3/codelimit/common/SourceFileEntry.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/SourceFolder.py` & `codelimit-0.9.3/codelimit/common/SourceFolder.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/Token.py` & `codelimit-0.9.3/codelimit/common/Token.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/TokenRange.py` & `codelimit-0.9.3/codelimit/common/TokenRange.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/Expression.py` & `codelimit-0.9.3/codelimit/common/gsm/Expression.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/automata/State.py` & `codelimit-0.9.3/codelimit/common/gsm/automata/State.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/matcher.py` & `codelimit-0.9.3/codelimit/common/gsm/matcher.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/operator/Atom.py` & `codelimit-0.9.3/codelimit/common/gsm/operator/Atom.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/operator/OneOrMore.py` & `codelimit-0.9.3/codelimit/common/gsm/operator/OneOrMore.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/operator/Optional.py` & `codelimit-0.9.3/codelimit/common/gsm/operator/Optional.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/operator/Union.py` & `codelimit-0.9.3/codelimit/common/gsm/operator/Union.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/operator/ZeroOrMore.py` & `codelimit-0.9.3/codelimit/common/gsm/operator/ZeroOrMore.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/predicate/Identity.py` & `codelimit-0.9.3/codelimit/common/gsm/predicate/Identity.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/gsm/utils.py` & `codelimit-0.9.3/codelimit/common/gsm/utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/lexer_utils.py` & `codelimit-0.9.3/codelimit/common/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/report/Report.py` & `codelimit-0.9.3/codelimit/common/report/Report.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/report/ReportReader.py` & `codelimit-0.9.3/codelimit/common/report/ReportReader.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/report/ReportWriter.py` & `codelimit-0.9.3/codelimit/common/report/ReportWriter.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/scope/Scope.py` & `codelimit-0.9.3/codelimit/common/scope/Scope.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/scope/scope_utils.py` & `codelimit-0.9.3/codelimit/common/scope/scope_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/source_utils.py` & `codelimit-0.9.3/codelimit/common/source_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_matching/predicate/Balanced.py` & `codelimit-0.9.3/codelimit/common/token_matching/predicate/Balanced.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_matching/predicate/Choice.py` & `codelimit-0.9.3/codelimit/common/token_matching/predicate/Choice.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_matching/predicate/Keyword.py` & `codelimit-0.9.3/codelimit/common/token_matching/predicate/Keyword.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_matching/predicate/Operator.py` & `codelimit-0.9.3/codelimit/common/token_matching/predicate/Operator.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_matching/predicate/Symbol.py` & `codelimit-0.9.3/codelimit/common/token_matching/predicate/Symbol.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_matching/predicate/TokenValue.py` & `codelimit-0.9.3/codelimit/common/token_matching/predicate/TokenValue.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/token_utils.py` & `codelimit-0.9.3/codelimit/common/token_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/common/utils.py` & `codelimit-0.9.3/codelimit/common/utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/github_auth.py` & `codelimit-0.9.3/codelimit/github_auth.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/languages/C.py` & `codelimit-0.9.3/codelimit/languages/C.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/languages/Cpp.py` & `codelimit-0.9.3/codelimit/languages/Cpp.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/languages/Java.py` & `codelimit-0.9.3/codelimit/languages/Java.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/languages/JavaScript.py` & `codelimit-0.9.3/codelimit/languages/JavaScript.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/languages/Python.py` & `codelimit-0.9.3/codelimit/languages/Python.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/languages/TypeScript.py` & `codelimit-0.9.3/codelimit/languages/TypeScript.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/codelimit/utils.py` & `codelimit-0.9.3/codelimit/utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.2/pyproject.toml` & `codelimit-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codelimit"
-version = "0.9.2"
+version = "0.9.3"
 description = ""
 authors = ["Rob van der Leek <robvanderleek@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 codelimit = "codelimit.__main__:cli"
```

### Comparing `codelimit-0.9.2/PKG-INFO` & `codelimit-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codelimit
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 License: GPL-3.0-or-later
 Author: Rob van der Leek
 Author-email: robvanderleek@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

