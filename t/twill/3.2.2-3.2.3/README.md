# Comparing `tmp/twill-3.2.2.tar.gz` & `tmp/twill-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twill-3.2.2.tar", last modified: Sun Jan 28 13:55:52 2024, max compression
+gzip compressed data, was "twill-3.2.3.tar", last modified: Tue Mar  5 19:48:10 2024, max compression
```

## Comparing `twill-3.2.2.tar` & `twill-3.2.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.344427 twill-3.2.2/
--rw-rw-rw-   0        0        0     1152 2023-10-22 19:40:05.000000 twill-3.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      332 2023-11-05 21:22:45.000000 twill-3.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4560 2024-01-28 13:55:52.340430 twill-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1109 2023-11-02 20:14:50.000000 twill-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:51.982959 twill-3.2.2/docs/
--rw-rw-rw-   0        0        0      633 2020-04-04 20:48:04.000000 twill-3.2.2/docs/Makefile
--rw-rw-rw-   0        0        0     2627 2020-04-04 20:48:04.000000 twill-3.2.2/docs/browsing.rst
--rw-rw-rw-   0        0        0     7326 2024-01-28 13:53:56.000000 twill-3.2.2/docs/changelog.rst
--rw-rw-rw-   0        0        0    11202 2023-11-23 20:32:02.000000 twill-3.2.2/docs/commands.rst
--rw-rw-rw-   0        0        0     2240 2023-11-02 21:12:42.000000 twill-3.2.2/docs/conf.py
--rw-rw-rw-   0        0        0     1297 2024-01-15 20:14:58.000000 twill-3.2.2/docs/developer.rst
--rw-rw-rw-   0        0        0      828 2020-04-04 20:48:04.000000 twill-3.2.2/docs/examples.rst
--rw-rw-rw-   0        0        0     6644 2020-04-04 20:48:04.000000 twill-3.2.2/docs/extensions.rst
--rw-rw-rw-   0        0        0      436 2020-04-04 20:48:04.000000 twill-3.2.2/docs/index.rst
--rw-rw-rw-   0        0        0     1449 2020-04-04 20:48:04.000000 twill-3.2.2/docs/install.rst
--rwxrwxrwx   0        0        0      760 2020-04-04 17:46:35.000000 twill-3.2.2/docs/make.bat
--rw-rw-rw-   0        0        0     3838 2023-11-02 14:44:37.000000 twill-3.2.2/docs/other.rst
--rw-rw-rw-   0        0        0     4709 2023-11-02 19:56:56.000000 twill-3.2.2/docs/overview.rst
--rw-rw-rw-   0        0        0     4734 2023-11-01 17:47:48.000000 twill-3.2.2/docs/python-api.rst
--rw-rw-rw-   0        0        0       13 2023-11-02 20:40:54.000000 twill-3.2.2/docs/requirements.txt
--rw-rw-rw-   0        0        0     4872 2023-11-02 14:58:35.000000 twill-3.2.2/docs/testing.rst
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:51.910406 twill-3.2.2/extras/
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:51.997934 twill-3.2.2/extras/examples/
--rw-rw-rw-   0        0        0      544 2020-04-04 17:46:35.000000 twill-3.2.2/extras/examples/discard-sf-mailman-msgs.twill
--rw-rw-rw-   0        0        0      307 2023-11-01 16:38:09.000000 twill-3.2.2/extras/examples/extend-example.py
--rw-rw-rw-   0        0        0      707 2021-02-13 22:32:03.000000 twill-3.2.2/extras/examples/quixote-demo.twill
--rw-rw-rw-   0        0        0      159 2020-04-04 17:46:35.000000 twill-3.2.2/extras/examples/set-user-agent.twill
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.003934 twill-3.2.2/extras/maxq/
--rw-rw-rw-   0        0        0      694 2020-04-04 17:46:35.000000 twill-3.2.2/extras/maxq/README.txt
--rw-rw-rw-   0        0        0     4041 2023-11-01 17:39:05.000000 twill-3.2.2/extras/maxq/TwillScriptGenerator.java
--rw-rw-rw-   0        0        0     5551 2024-01-28 13:44:51.000000 twill-3.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-28 13:55:52.345429 twill-3.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:51.913405 twill-3.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.044455 twill-3.2.2/src/twill/
--rw-rw-rw-   0        0        0     3177 2023-11-01 16:47:47.000000 twill-3.2.2/src/twill/__init__.py
--rw-rw-rw-   0        0        0      107 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/__main__.py
--rw-rw-rw-   0        0        0    11675 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/agents.py
--rw-rw-rw-   0        0        0    25899 2023-11-23 20:32:02.000000 twill-3.2.2/src/twill/browser.py
--rw-rw-rw-   0        0        0    25950 2023-11-23 20:32:02.000000 twill-3.2.2/src/twill/commands.py
--rw-rw-rw-   0        0        0      327 2023-10-22 11:27:00.000000 twill-3.2.2/src/twill/errors.py
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.103459 twill-3.2.2/src/twill/extensions/
--rw-rw-rw-   0        0        0       28 2023-10-22 11:28:52.000000 twill-3.2.2/src/twill/extensions/__init__.py
--rw-rw-rw-   0        0        0     1044 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/argparse.py
--rw-rw-rw-   0        0        0     5003 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/check_links.py
--rw-rw-rw-   0        0        0      985 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/csv_iterate.py
--rw-rw-rw-   0        0        0     1066 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/dirstack.py
--rw-rw-rw-   0        0        0     4149 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/dns_check.py
--rw-rw-rw-   0        0        0     3495 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/formfill.py
--rw-rw-rw-   0        0        0     1462 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/mailman_sf.py
--rw-rw-rw-   0        0        0     2151 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/match_parse.py
--rw-rw-rw-   0        0        0     2938 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/require.py
--rw-rw-rw-   0        0        0      743 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/extensions/shell_test.py
--rw-rw-rw-   0        0        0     3985 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/fork.py
--rw-rw-rw-   0        0        0     1348 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/namespaces.py
--rw-rw-rw-   0        0        0     9681 2023-11-01 16:38:09.000000 twill-3.2.2/src/twill/parse.py
--rw-rw-rw-   0        0        0       64 2023-10-22 20:00:51.000000 twill-3.2.2/src/twill/py.typed
--rw-rw-rw-   0        0        0    15490 2024-01-28 11:20:34.000000 twill-3.2.2/src/twill/shell.py
--rw-rw-rw-   0        0        0     2556 2023-11-01 16:50:23.000000 twill-3.2.2/src/twill/unit.py
--rw-rw-rw-   0        0        0    15230 2024-01-28 12:43:52.000000 twill-3.2.2/src/twill/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.338428 twill-3.2.2/src/twill.egg-info/
--rw-rw-rw-   0        0        0     4560 2024-01-28 13:55:51.000000 twill-3.2.2/src/twill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3113 2024-01-28 13:55:51.000000 twill-3.2.2/src/twill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-28 13:55:51.000000 twill-3.2.2/src/twill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-01-28 13:55:51.000000 twill-3.2.2/src/twill.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      190 2024-01-28 13:55:51.000000 twill-3.2.2/src/twill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-28 13:55:51.000000 twill-3.2.2/src/twill.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.315348 twill-3.2.2/tests/
--rw-rw-rw-   0        0        0      244 2021-02-13 22:33:57.000000 twill-3.2.2/tests/README.txt
--rw-rw-rw-   0        0        0       28 2023-10-22 11:28:52.000000 twill-3.2.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1082 2023-11-01 17:01:40.000000 twill-3.2.2/tests/conftest.py
--rw-rw-rw-   0        0        0     3174 2023-11-01 16:59:42.000000 twill-3.2.2/tests/mock_dns.py
--rw-rw-rw-   0        0        0    18964 2024-01-28 11:26:01.000000 twill-3.2.2/tests/server.py
--rw-rw-rw-   0        0        0      111 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_back.py
--rw-rw-rw-   0        0        0      749 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_back.twill
--rw-rw-rw-   0        0        0      434 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_basic.py
--rw-rw-rw-   0        0        0     3378 2021-02-13 23:44:14.000000 twill-3.2.2/tests/test_basic.twill
--rw-rw-rw-   0        0        0      934 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_broken_html.py
--rw-rw-rw-   0        0        0       95 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_buildbot.py
--rw-rw-rw-   0        0        0      157 2023-11-23 18:20:31.000000 twill-3.2.2/tests/test_check_links.py
--rw-rw-rw-   0        0        0      179 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_check_links.twill
--rw-rw-rw-   0        0        0     1599 2023-11-23 20:32:02.000000 twill-3.2.2/tests/test_checkbox.py
--rw-rw-rw-   0        0        0      179 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_dns.py
--rw-rw-rw-   0        0        0      863 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_dns.twill
--rw-rw-rw-   0        0        0      120 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_equiv_refresh.py
--rw-rw-rw-   0        0        0      757 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_equiv_refresh.twill
--rw-rw-rw-   0        0        0      111 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_find.py
--rw-rw-rw-   0        0        0      453 2021-12-04 12:35:07.000000 twill-3.2.2/tests/test_find.twill
--rw-rw-rw-   0        0        0     1595 2023-11-23 20:32:02.000000 twill-3.2.2/tests/test_find_links.py
--rw-rw-rw-   0        0        0     1380 2023-11-23 20:32:02.000000 twill-3.2.2/tests/test_form.py
--rw-rw-rw-   0        0        0     2043 2022-10-30 12:18:38.000000 twill-3.2.2/tests/test_form.twill
--rw-rw-rw-   0        0        0      162 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_formfill.py
--rw-rw-rw-   0        0        0     1111 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_formfill.twill
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:51.922405 twill-3.2.2/tests/test_gather/
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.321349 twill-3.2.2/tests/test_gather/00-testme/
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/00-testme/x-script.twill
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/00-testme/y-script.txt
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.327355 twill-3.2.2/tests/test_gather/01-test/
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/01-test/a.notwill
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/01-test/b.twill
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.332356 twill-3.2.2/tests/test_gather/02-test2/
-drwxrwxrwx   0        0        0        0 2024-01-28 13:55:52.334355 twill-3.2.2/tests/test_gather/02-test2/02-subtest/
--rw-rw-rw-   0        0        0        0 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/02-test2/02-subtest/d.twill
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/02-test2/c.bak
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_gather/02-test2/c.twill
--rw-rw-rw-   0        0        0      632 2024-01-28 12:43:52.000000 twill-3.2.2/tests/test_gather.py
--rw-rw-rw-   0        0        0      299 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_global_form.py
--rw-rw-rw-   0        0        0      234 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_global_form.twill
--rw-rw-rw-   0        0        0     2240 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_go.py
--rw-rw-rw-   0        0        0      312 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_go.twill
--rw-rw-rw-   0        0        0        7 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_go_exit.twill
--rw-rw-rw-   0        0        0       17 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_go_fail.twill
--rw-rw-rw-   0        0        0       26 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_go_fail2.twill
--rw-rw-rw-   0        0        0      114 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_headers.py
--rw-rw-rw-   0        0        0      257 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_headers.twill
--rw-rw-rw-   0        0        0      116 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_http_auth.py
--rw-rw-rw-   0        0        0      411 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_http_auth.twill
--rw-rw-rw-   0        0        0      117 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_http_codes.py
--rw-rw-rw-   0        0        0      329 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_http_codes.twill
--rw-rw-rw-   0        0        0      111 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_info.py
--rw-rw-rw-   0        0        0       51 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_info.twill
--rw-rw-rw-   0        0        0      130 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_match_parse.py
--rw-rw-rw-   0        0        0      263 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_match_parse.twill
--rw-rw-rw-   0        0        0     1793 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_misc.py
--rw-rw-rw-   0        0        0      115 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_multisub.py
--rw-rw-rw-   0        0        0      403 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_multisub.twill
--rw-rw-rw-   0        0        0      580 2023-11-23 20:32:02.000000 twill-3.2.2/tests/test_radiobutton.py
--rw-rw-rw-   0        0        0     1687 2024-01-28 10:51:53.000000 twill-3.2.2/tests/test_shell.py
--rw-rw-rw-   0        0        0      281 2023-10-22 02:57:37.000000 twill-3.2.2/tests/test_shell.twill
--rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_shell_fail.twill
--rw-rw-rw-   0        0        0      374 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_show.py
--rw-rw-rw-   0        0        0      873 2022-10-30 13:45:18.000000 twill-3.2.2/tests/test_show.twill
--rw-rw-rw-   0        0        0     1578 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_tidy.py
--rw-rw-rw-   0        0        0      556 2023-11-23 20:32:02.000000 twill-3.2.2/tests/test_timeout.py
--rw-rw-rw-   0        0        0     1091 2023-11-23 20:32:02.000000 twill-3.2.2/tests/test_two_forms.py
--rw-rw-rw-   0        0        0      833 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_unit_support.py
--rw-rw-rw-   0        0        0      143 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_unit_support.twill
--rw-rw-rw-   0        0        0     1620 2024-01-28 13:36:15.000000 twill-3.2.2/tests/test_utils.py
--rw-rw-rw-   0        0        0      545 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_variables.py
--rw-rw-rw-   0        0        0      472 2020-04-04 17:46:35.000000 twill-3.2.2/tests/test_variables.twill
--rw-rw-rw-   0        0        0     2848 2023-11-02 17:28:44.000000 twill-3.2.2/tests/test_wsgi.py
--rw-rw-rw-   0        0        0      110 2023-11-01 16:38:09.000000 twill-3.2.2/tests/test_xml.py
--rw-rw-rw-   0        0        0       72 2021-02-13 17:27:36.000000 twill-3.2.2/tests/test_xml.twill
--rw-rw-rw-   0        0        0     4294 2023-11-01 18:01:46.000000 twill-3.2.2/tests/utils.py
--rw-rw-rw-   0        0        0      716 2024-01-28 11:01:09.000000 twill-3.2.2/tox.ini
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.264494 twill-3.2.3/
+-rw-rw-rw-   0        0        0     1152 2024-01-28 14:15:02.000000 twill-3.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      332 2023-11-05 21:22:45.000000 twill-3.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4560 2024-03-05 19:48:10.262496 twill-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2024-01-28 14:15:10.000000 twill-3.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.867555 twill-3.2.3/docs/
+-rw-rw-rw-   0        0        0      633 2020-04-04 20:48:04.000000 twill-3.2.3/docs/Makefile
+-rw-rw-rw-   0        0        0     2627 2020-04-04 20:48:04.000000 twill-3.2.3/docs/browsing.rst
+-rw-rw-rw-   0        0        0     7440 2024-03-05 19:36:49.000000 twill-3.2.3/docs/changelog.rst
+-rw-rw-rw-   0        0        0    11202 2023-11-23 20:32:02.000000 twill-3.2.3/docs/commands.rst
+-rw-rw-rw-   0        0        0     2240 2024-01-28 14:15:32.000000 twill-3.2.3/docs/conf.py
+-rw-rw-rw-   0        0        0     1297 2024-01-28 14:15:39.000000 twill-3.2.3/docs/developer.rst
+-rw-rw-rw-   0        0        0      828 2020-04-04 20:48:04.000000 twill-3.2.3/docs/examples.rst
+-rw-rw-rw-   0        0        0     6644 2020-04-04 20:48:04.000000 twill-3.2.3/docs/extensions.rst
+-rw-rw-rw-   0        0        0      436 2020-04-04 20:48:04.000000 twill-3.2.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1449 2020-04-04 20:48:04.000000 twill-3.2.3/docs/install.rst
+-rwxrwxrwx   0        0        0      760 2020-04-04 17:46:35.000000 twill-3.2.3/docs/make.bat
+-rw-rw-rw-   0        0        0     3838 2023-11-02 14:44:37.000000 twill-3.2.3/docs/other.rst
+-rw-rw-rw-   0        0        0     4709 2023-11-02 19:56:56.000000 twill-3.2.3/docs/overview.rst
+-rw-rw-rw-   0        0        0     4734 2023-11-01 17:47:48.000000 twill-3.2.3/docs/python-api.rst
+-rw-rw-rw-   0        0        0       13 2023-11-02 20:40:54.000000 twill-3.2.3/docs/requirements.txt
+-rw-rw-rw-   0        0        0     4872 2023-11-02 14:58:35.000000 twill-3.2.3/docs/testing.rst
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.788904 twill-3.2.3/extras/
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.882566 twill-3.2.3/extras/examples/
+-rw-rw-rw-   0        0        0      544 2020-04-04 17:46:35.000000 twill-3.2.3/extras/examples/discard-sf-mailman-msgs.twill
+-rw-rw-rw-   0        0        0      307 2023-11-01 16:38:09.000000 twill-3.2.3/extras/examples/extend-example.py
+-rw-rw-rw-   0        0        0      707 2021-02-13 22:32:03.000000 twill-3.2.3/extras/examples/quixote-demo.twill
+-rw-rw-rw-   0        0        0      159 2020-04-04 17:46:35.000000 twill-3.2.3/extras/examples/set-user-agent.twill
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.887079 twill-3.2.3/extras/maxq/
+-rw-rw-rw-   0        0        0      694 2020-04-04 17:46:35.000000 twill-3.2.3/extras/maxq/README.txt
+-rw-rw-rw-   0        0        0     4041 2023-11-01 17:39:05.000000 twill-3.2.3/extras/maxq/TwillScriptGenerator.java
+-rw-rw-rw-   0        0        0     5591 2024-03-05 19:42:56.000000 twill-3.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-05 19:48:10.264494 twill-3.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.792901 twill-3.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.927080 twill-3.2.3/src/twill/
+-rw-rw-rw-   0        0        0     3177 2024-01-28 14:15:02.000000 twill-3.2.3/src/twill/__init__.py
+-rw-rw-rw-   0        0        0      107 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/__main__.py
+-rw-rw-rw-   0        0        0    11675 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/agents.py
+-rw-rw-rw-   0        0        0    25899 2023-11-23 20:32:02.000000 twill-3.2.3/src/twill/browser.py
+-rw-rw-rw-   0        0        0    25965 2024-03-05 19:23:13.000000 twill-3.2.3/src/twill/commands.py
+-rw-rw-rw-   0        0        0      327 2023-10-22 11:27:00.000000 twill-3.2.3/src/twill/errors.py
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.016511 twill-3.2.3/src/twill/extensions/
+-rw-rw-rw-   0        0        0       28 2023-10-22 11:28:52.000000 twill-3.2.3/src/twill/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1044 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/argparse.py
+-rw-rw-rw-   0        0        0     5003 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/check_links.py
+-rw-rw-rw-   0        0        0      985 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/csv_iterate.py
+-rw-rw-rw-   0        0        0     1066 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/dirstack.py
+-rw-rw-rw-   0        0        0     4149 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/dns_check.py
+-rw-rw-rw-   0        0        0     3495 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/formfill.py
+-rw-rw-rw-   0        0        0     1462 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/mailman_sf.py
+-rw-rw-rw-   0        0        0     2151 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/match_parse.py
+-rw-rw-rw-   0        0        0     2938 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/require.py
+-rw-rw-rw-   0        0        0      743 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/extensions/shell_test.py
+-rw-rw-rw-   0        0        0     3985 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/fork.py
+-rw-rw-rw-   0        0        0     1348 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/namespaces.py
+-rw-rw-rw-   0        0        0     9681 2023-11-01 16:38:09.000000 twill-3.2.3/src/twill/parse.py
+-rw-rw-rw-   0        0        0       64 2023-10-22 20:00:51.000000 twill-3.2.3/src/twill/py.typed
+-rw-rw-rw-   0        0        0    15490 2024-01-28 11:20:34.000000 twill-3.2.3/src/twill/shell.py
+-rw-rw-rw-   0        0        0     2556 2023-11-01 16:50:23.000000 twill-3.2.3/src/twill/unit.py
+-rw-rw-rw-   0        0        0    15230 2024-01-28 12:43:52.000000 twill-3.2.3/src/twill/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.260494 twill-3.2.3/src/twill.egg-info/
+-rw-rw-rw-   0        0        0     4560 2024-03-05 19:48:09.000000 twill-3.2.3/src/twill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3113 2024-03-05 19:48:09.000000 twill-3.2.3/src/twill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-05 19:48:09.000000 twill-3.2.3/src/twill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-03-05 19:48:09.000000 twill-3.2.3/src/twill.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      190 2024-03-05 19:48:09.000000 twill-3.2.3/src/twill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-03-05 19:48:09.000000 twill-3.2.3/src/twill.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.239775 twill-3.2.3/tests/
+-rw-rw-rw-   0        0        0      244 2021-02-13 22:33:57.000000 twill-3.2.3/tests/README.txt
+-rw-rw-rw-   0        0        0       28 2023-10-22 11:28:52.000000 twill-3.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1082 2023-11-01 17:01:40.000000 twill-3.2.3/tests/conftest.py
+-rw-rw-rw-   0        0        0     3174 2023-11-01 16:59:42.000000 twill-3.2.3/tests/mock_dns.py
+-rw-rw-rw-   0        0        0    18964 2024-01-28 11:26:01.000000 twill-3.2.3/tests/server.py
+-rw-rw-rw-   0        0        0      111 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_back.py
+-rw-rw-rw-   0        0        0      749 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_back.twill
+-rw-rw-rw-   0        0        0      434 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_basic.py
+-rw-rw-rw-   0        0        0     3378 2021-02-13 23:44:14.000000 twill-3.2.3/tests/test_basic.twill
+-rw-rw-rw-   0        0        0      934 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_broken_html.py
+-rw-rw-rw-   0        0        0       95 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_buildbot.py
+-rw-rw-rw-   0        0        0      157 2023-11-23 18:20:31.000000 twill-3.2.3/tests/test_check_links.py
+-rw-rw-rw-   0        0        0      179 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_check_links.twill
+-rw-rw-rw-   0        0        0     1599 2023-11-23 20:32:02.000000 twill-3.2.3/tests/test_checkbox.py
+-rw-rw-rw-   0        0        0      179 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_dns.py
+-rw-rw-rw-   0        0        0      863 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_dns.twill
+-rw-rw-rw-   0        0        0      120 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_equiv_refresh.py
+-rw-rw-rw-   0        0        0      757 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_equiv_refresh.twill
+-rw-rw-rw-   0        0        0      111 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_find.py
+-rw-rw-rw-   0        0        0      453 2021-12-04 12:35:07.000000 twill-3.2.3/tests/test_find.twill
+-rw-rw-rw-   0        0        0     1595 2023-11-23 20:32:02.000000 twill-3.2.3/tests/test_find_links.py
+-rw-rw-rw-   0        0        0     1380 2023-11-23 20:32:02.000000 twill-3.2.3/tests/test_form.py
+-rw-rw-rw-   0        0        0     2043 2022-10-30 12:18:38.000000 twill-3.2.3/tests/test_form.twill
+-rw-rw-rw-   0        0        0      162 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_formfill.py
+-rw-rw-rw-   0        0        0     1111 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_formfill.twill
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:09.800905 twill-3.2.3/tests/test_gather/
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.244775 twill-3.2.3/tests/test_gather/00-testme/
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/00-testme/x-script.twill
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/00-testme/y-script.txt
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.248774 twill-3.2.3/tests/test_gather/01-test/
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/01-test/a.notwill
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/01-test/b.twill
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.252776 twill-3.2.3/tests/test_gather/02-test2/
+drwxrwxrwx   0        0        0        0 2024-03-05 19:48:10.257494 twill-3.2.3/tests/test_gather/02-test2/02-subtest/
+-rw-rw-rw-   0        0        0        0 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/02-test2/02-subtest/d.twill
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/02-test2/c.bak
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_gather/02-test2/c.twill
+-rw-rw-rw-   0        0        0      632 2024-01-28 12:43:52.000000 twill-3.2.3/tests/test_gather.py
+-rw-rw-rw-   0        0        0      299 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_global_form.py
+-rw-rw-rw-   0        0        0      234 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_global_form.twill
+-rw-rw-rw-   0        0        0     2240 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_go.py
+-rw-rw-rw-   0        0        0      312 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_go.twill
+-rw-rw-rw-   0        0        0        7 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_go_exit.twill
+-rw-rw-rw-   0        0        0       17 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_go_fail.twill
+-rw-rw-rw-   0        0        0       26 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_go_fail2.twill
+-rw-rw-rw-   0        0        0      114 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_headers.py
+-rw-rw-rw-   0        0        0      257 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_headers.twill
+-rw-rw-rw-   0        0        0      116 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_http_auth.py
+-rw-rw-rw-   0        0        0      411 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_http_auth.twill
+-rw-rw-rw-   0        0        0      117 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_http_codes.py
+-rw-rw-rw-   0        0        0      329 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_http_codes.twill
+-rw-rw-rw-   0        0        0      111 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_info.py
+-rw-rw-rw-   0        0        0       51 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_info.twill
+-rw-rw-rw-   0        0        0      130 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_match_parse.py
+-rw-rw-rw-   0        0        0      263 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_match_parse.twill
+-rw-rw-rw-   0        0        0     1793 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_misc.py
+-rw-rw-rw-   0        0        0      115 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_multisub.py
+-rw-rw-rw-   0        0        0      403 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_multisub.twill
+-rw-rw-rw-   0        0        0      580 2023-11-23 20:32:02.000000 twill-3.2.3/tests/test_radiobutton.py
+-rw-rw-rw-   0        0        0     1687 2024-01-28 10:51:53.000000 twill-3.2.3/tests/test_shell.py
+-rw-rw-rw-   0        0        0      281 2023-10-22 02:57:37.000000 twill-3.2.3/tests/test_shell.twill
+-rw-rw-rw-   0        0        0        8 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_shell_fail.twill
+-rw-rw-rw-   0        0        0      374 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_show.py
+-rw-rw-rw-   0        0        0      873 2022-10-30 13:45:18.000000 twill-3.2.3/tests/test_show.twill
+-rw-rw-rw-   0        0        0     1578 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_tidy.py
+-rw-rw-rw-   0        0        0      556 2023-11-23 20:32:02.000000 twill-3.2.3/tests/test_timeout.py
+-rw-rw-rw-   0        0        0     1091 2023-11-23 20:32:02.000000 twill-3.2.3/tests/test_two_forms.py
+-rw-rw-rw-   0        0        0      833 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_unit_support.py
+-rw-rw-rw-   0        0        0      143 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_unit_support.twill
+-rw-rw-rw-   0        0        0     1620 2024-01-28 13:36:15.000000 twill-3.2.3/tests/test_utils.py
+-rw-rw-rw-   0        0        0      545 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_variables.py
+-rw-rw-rw-   0        0        0      472 2020-04-04 17:46:35.000000 twill-3.2.3/tests/test_variables.twill
+-rw-rw-rw-   0        0        0     2848 2023-11-02 17:28:44.000000 twill-3.2.3/tests/test_wsgi.py
+-rw-rw-rw-   0        0        0      110 2023-11-01 16:38:09.000000 twill-3.2.3/tests/test_xml.py
+-rw-rw-rw-   0        0        0       72 2021-02-13 17:27:36.000000 twill-3.2.3/tests/test_xml.twill
+-rw-rw-rw-   0        0        0     4294 2023-11-01 18:01:46.000000 twill-3.2.3/tests/utils.py
+-rw-rw-rw-   0        0        0      713 2024-03-05 19:29:32.000000 twill-3.2.3/tox.ini
```

### Comparing `twill-3.2.2/LICENSE.txt` & `twill-3.2.3/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License, https://opensource.org/licenses/MIT
 
-Copyright 2005-2023 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
+Copyright 2005-2024 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `twill-3.2.2/PKG-INFO` & `twill-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: twill
-Version: 3.2.2
+Version: 3.2.3
 Summary: A web browsing and testing language
 Author: C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
 Maintainer-email: Christoph Zwerschke <cito@online.de>
 License: The MIT License, https://opensource.org/licenses/MIT
         
-        Copyright 2005-2023 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
+        Copyright 2005-2024 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -53,16 +53,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: lxml<5,>=4.9
 Requires-Dist: httpx<1,>=0.26.0
 Requires-Dist: pyparsing<4,>=3.1
 Provides-Extra: docs
-Requires-Dist: sphinx<6,>=5.2; extra == "docs"
-Requires-Dist: sphinx_rtd_theme<2,>=1; extra == "docs"
+Requires-Dist: sphinx<8,>=7.2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme<3,>=2; extra == "docs"
 Provides-Extra: tidy
 Requires-Dist: pytidylib<0.4,>=0.3; extra == "tidy"
 Provides-Extra: tests
 Requires-Dist: tox<5,>=4; extra == "tests"
 Requires-Dist: pytest<9,>=8; extra == "tests"
 Requires-Dist: pytidylib<0.4,>=0.3; extra == "tests"
 Requires-Dist: quixote<4,>=3.6; extra == "tests"
@@ -74,12 +74,12 @@
 
 The current version 3.2 supports Python 3.8 to 3.12.
 
 Take a look at the [changelog](https://twill-tools.github.io/twill/changelog.html) to find a list of all changes and improvements made since version 2. For a brief overview of twill's history starting from its early days, see the [acknowledgements and history](https://twill-tools.github.io/twill/overview.html#acknowledgements-and-history) section.
 
 The full [documentation](https://twill-tools.github.io/twill/) is included in the distribution and provided online via [GitHub](https://twill-tools.github.io/twill/) and [ReadTheDocs](https://twill.readthedocs.io/en/latest/).
 
-Copyright (c) 2005-2023 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
+Copyright (c) 2005-2024 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
 
 Newer versions have been created and are maintained by [Christoph Zwerschke](https://github.com/Cito).
  
 twill is available for use, modification, and distribution under the MIT license.
```

### Comparing `twill-3.2.2/README.md` & `twill-3.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 
 The current version 3.2 supports Python 3.8 to 3.12.
 
 Take a look at the [changelog](https://twill-tools.github.io/twill/changelog.html) to find a list of all changes and improvements made since version 2. For a brief overview of twill's history starting from its early days, see the [acknowledgements and history](https://twill-tools.github.io/twill/overview.html#acknowledgements-and-history) section.
 
 The full [documentation](https://twill-tools.github.io/twill/) is included in the distribution and provided online via [GitHub](https://twill-tools.github.io/twill/) and [ReadTheDocs](https://twill.readthedocs.io/en/latest/).
 
-Copyright (c) 2005-2023 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
+Copyright (c) 2005-2024 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
 
 Newer versions have been created and are maintained by [Christoph Zwerschke](https://github.com/Cito).
  
 twill is available for use, modification, and distribution under the MIT license.
```

### Comparing `twill-3.2.2/docs/Makefile` & `twill-3.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/browsing.rst` & `twill-3.2.3/docs/browsing.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/changelog.rst` & `twill-3.2.3/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. _changelog:
 
 =========
 ChangeLog
 =========
 
+3.2.3 (released 2024-03-05)
+---------------------------
+* Adds 'timeout' to the list of exported commends (#22).
+
 3.2.2 (released 2024-01-28)
 ---------------------------
 * Fixes the broken interactive shell.
 * Fixes 'run_file' when specifying files in a subdirectory without extension.
 
 3.2.1 (released 2023-11-23)
 ---------------------------
```

### Comparing `twill-3.2.2/docs/commands.rst` & `twill-3.2.3/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/conf.py` & `twill-3.2.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 version = line.split("=")[1].strip().strip('"')
                 return version
     raise Exception("Cannot determine project version")
 
 
 project = "twill"
 author = "C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al"
-copyright = "2023, " + author
+copyright = "2024, " + author
 
 # The full version, including alpha/beta/rc tags
 version = release = project_version()
 
 language = "en"
```

### Comparing `twill-3.2.2/docs/developer.rst` & `twill-3.2.3/docs/developer.rst`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 All code taken from twill 0.x is Copyright (C) 2005-2007
 C. Titus Brown <titus@idyll.org>.
 
 In plain English: C. Titus Brown owns the original code, but you're
 welcome to use it, update it, subsume it into other projects, and
 distribute it freely. However, you must retain copyright attribution.
 
-Newer versions 1.x, 2.x and 3.x are also Copyright (C) 2007-2023
+Newer versions 1.x, 2.x and 3.x are also Copyright (C) 2007-2024
 Ben R. Taylor, Adam V. Brandizzi, Christoph Zwerschke et al.
 
 The newer versions are released under the same `MIT license`_.
 
 .. _MIT license: http://www.opensource.org/licenses/mit-license.php
 
 Developer releases
```

### Comparing `twill-3.2.2/docs/examples.rst` & `twill-3.2.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/extensions.rst` & `twill-3.2.3/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/install.rst` & `twill-3.2.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/make.bat` & `twill-3.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/other.rst` & `twill-3.2.3/docs/other.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/overview.rst` & `twill-3.2.3/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/python-api.rst` & `twill-3.2.3/docs/python-api.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/docs/testing.rst` & `twill-3.2.3/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/extras/examples/discard-sf-mailman-msgs.twill` & `twill-3.2.3/extras/examples/discard-sf-mailman-msgs.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/extras/examples/quixote-demo.twill` & `twill-3.2.3/extras/examples/quixote-demo.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/extras/maxq/README.txt` & `twill-3.2.3/extras/maxq/README.txt`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/extras/maxq/TwillScriptGenerator.java` & `twill-3.2.3/extras/maxq/TwillScriptGenerator.java`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/pyproject.toml` & `twill-3.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "twill"
-version = "3.2.2"
+version = "3.2.3"
 
 description = "A web browsing and testing language"
 keywords = ["web", "testing",  "browsing", "automation"]
 
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
@@ -42,16 +42,16 @@
   "lxml >=4.9, <5",
   "httpx >=0.26.0, <1",
   "pyparsing >=3.1, <4",
 ]
 
 [project.optional-dependencies]
 docs = [
-  "sphinx >=5.2, <6",
-  "sphinx_rtd_theme >=1, <2"
+  "sphinx >=7.2, <8",
+  "sphinx_rtd_theme >=2, <3"
 ]
 tidy = [
   "pytidylib >=0.3, <0.4"
 ]
 tests = [
   "tox >=4, <5",
   "pytest >=8, <9",
@@ -87,14 +87,18 @@
 warn_unused_ignores = true
 disallow_untyped_defs = false
 
 [tool.black]
 line-length = 79
 
 [tool.ruff]
+line-length = 79
+target-version = "py38"
+
+[tool.ruff.lint]
 select = [
   "A",      # flake8-builtins
   "ANN",    # flake8-annotations
   "ARG",    # flake8-unused-arguments
   "B",      # flake8-bugbear
   "BLE",    # flake8-blind-except
   "C4",     # flake8-comprehensions
@@ -146,30 +150,28 @@
   "D213",  # multi-line docstrings should not start at second line
   "EM101", "EM102",  # allows exceptions with literal and f-strings
   "ISC001",  # allow string literal concatenatin for auto-formatting
   "PTH123",  # allow builtin-open
   "TRY003",  # allow specific messages outside the exception class
   "TRY301",  # allow raise
 ]
-line-length = 79
-target-version = "py38"
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "double"
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 25
 
-[tool.ruff.pylint]
+[tool.ruff.lint.pylint]
 max-args = 12
 max-branches = 25
 max-returns = 7
 max-statements = 75
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "src/twill/commands.py" = [
   "A001",  # may shadow builtins
   "D400", "D401", "D415",  # allow more flexible docstrings
   "S102"  # allow use of exec
 ]
 "src/twill/fork.py" = [
   "T201"  # allow using print()
@@ -196,9 +198,9 @@
   "D",  # do not require docstrings
   "ANN201",  # do no trequre return types
   "S101",  # allow assert statements
   "PLR2004",  # allow magic values
 ]
 
 [build-system]
-requires = ["setuptools >=68"]
+requires = ["setuptools >=69"]
 build-backend = "setuptools.build_meta"
```

### Comparing `twill-3.2.2/src/twill/__init__.py` & `twill-3.2.3/src/twill/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of the twill source distribution.
 #
 # twill is an extensible scriptlet language for testing Web apps,
 # available at https://github.com/twill-tools/twill.
 #
-# Copyright (c) 2005-2023
+# Copyright (c) 2005-2024
 # by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
 #
 # This program and all associated source code files are released under the
 # terms of the MIT license; please see the included LICENSE file for more
 # information, or go to https://opensource.org/licenses/mit-license.php.
 
 """The twill web browsing and testing language and associated utilities.
```

### Comparing `twill-3.2.2/src/twill/agents.py` & `twill-3.2.3/src/twill/agents.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/browser.py` & `twill-3.2.3/src/twill/browser.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/commands.py` & `twill-3.2.3/src/twill/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     "showhtml",
     "show_html",
     "showlinks",
     "show_links",
     "sleep",
     "submit",
     "tidy_ok",
+    "timeout",
     "title",
     "url",
 ]
 
 
 def reset_browser(base_url: str = "") -> None:
     """>> reset_browser [base_url]
```

### Comparing `twill-3.2.2/src/twill/extensions/argparse.py` & `twill-3.2.3/src/twill/extensions/argparse.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/check_links.py` & `twill-3.2.3/src/twill/extensions/check_links.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/csv_iterate.py` & `twill-3.2.3/src/twill/extensions/csv_iterate.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/dirstack.py` & `twill-3.2.3/src/twill/extensions/dirstack.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/dns_check.py` & `twill-3.2.3/src/twill/extensions/dns_check.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/formfill.py` & `twill-3.2.3/src/twill/extensions/formfill.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/mailman_sf.py` & `twill-3.2.3/src/twill/extensions/mailman_sf.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/match_parse.py` & `twill-3.2.3/src/twill/extensions/match_parse.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/require.py` & `twill-3.2.3/src/twill/extensions/require.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/extensions/shell_test.py` & `twill-3.2.3/src/twill/extensions/shell_test.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/fork.py` & `twill-3.2.3/src/twill/fork.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/namespaces.py` & `twill-3.2.3/src/twill/namespaces.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/parse.py` & `twill-3.2.3/src/twill/parse.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/shell.py` & `twill-3.2.3/src/twill/shell.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/unit.py` & `twill-3.2.3/src/twill/unit.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill/utils.py` & `twill-3.2.3/src/twill/utils.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/src/twill.egg-info/PKG-INFO` & `twill-3.2.3/src/twill.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: twill
-Version: 3.2.2
+Version: 3.2.3
 Summary: A web browsing and testing language
 Author: C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
 Maintainer-email: Christoph Zwerschke <cito@online.de>
 License: The MIT License, https://opensource.org/licenses/MIT
         
-        Copyright 2005-2023 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
+        Copyright 2005-2024 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -53,16 +53,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: lxml<5,>=4.9
 Requires-Dist: httpx<1,>=0.26.0
 Requires-Dist: pyparsing<4,>=3.1
 Provides-Extra: docs
-Requires-Dist: sphinx<6,>=5.2; extra == "docs"
-Requires-Dist: sphinx_rtd_theme<2,>=1; extra == "docs"
+Requires-Dist: sphinx<8,>=7.2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme<3,>=2; extra == "docs"
 Provides-Extra: tidy
 Requires-Dist: pytidylib<0.4,>=0.3; extra == "tidy"
 Provides-Extra: tests
 Requires-Dist: tox<5,>=4; extra == "tests"
 Requires-Dist: pytest<9,>=8; extra == "tests"
 Requires-Dist: pytidylib<0.4,>=0.3; extra == "tests"
 Requires-Dist: quixote<4,>=3.6; extra == "tests"
@@ -74,12 +74,12 @@
 
 The current version 3.2 supports Python 3.8 to 3.12.
 
 Take a look at the [changelog](https://twill-tools.github.io/twill/changelog.html) to find a list of all changes and improvements made since version 2. For a brief overview of twill's history starting from its early days, see the [acknowledgements and history](https://twill-tools.github.io/twill/overview.html#acknowledgements-and-history) section.
 
 The full [documentation](https://twill-tools.github.io/twill/) is included in the distribution and provided online via [GitHub](https://twill-tools.github.io/twill/) and [ReadTheDocs](https://twill.readthedocs.io/en/latest/).
 
-Copyright (c) 2005-2023 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
+Copyright (c) 2005-2024 by C. Titus Brown, Ben R. Taylor, Christoph Zwerschke et al.
 
 Newer versions have been created and are maintained by [Christoph Zwerschke](https://github.com/Cito).
  
 twill is available for use, modification, and distribution under the MIT license.
```

### Comparing `twill-3.2.2/src/twill.egg-info/SOURCES.txt` & `twill-3.2.3/src/twill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/conftest.py` & `twill-3.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/mock_dns.py` & `twill-3.2.3/tests/mock_dns.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/server.py` & `twill-3.2.3/tests/server.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_back.twill` & `twill-3.2.3/tests/test_back.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_basic.twill` & `twill-3.2.3/tests/test_basic.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_broken_html.py` & `twill-3.2.3/tests/test_broken_html.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_checkbox.py` & `twill-3.2.3/tests/test_checkbox.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_dns.twill` & `twill-3.2.3/tests/test_dns.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_equiv_refresh.twill` & `twill-3.2.3/tests/test_equiv_refresh.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_find_links.py` & `twill-3.2.3/tests/test_find_links.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_form.py` & `twill-3.2.3/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_form.twill` & `twill-3.2.3/tests/test_form.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_formfill.twill` & `twill-3.2.3/tests/test_formfill.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_gather.py` & `twill-3.2.3/tests/test_gather.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_go.py` & `twill-3.2.3/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_misc.py` & `twill-3.2.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_radiobutton.py` & `twill-3.2.3/tests/test_radiobutton.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_shell.py` & `twill-3.2.3/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_show.twill` & `twill-3.2.3/tests/test_show.twill`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_tidy.py` & `twill-3.2.3/tests/test_tidy.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_timeout.py` & `twill-3.2.3/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_two_forms.py` & `twill-3.2.3/tests/test_two_forms.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_unit_support.py` & `twill-3.2.3/tests/test_unit_support.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_utils.py` & `twill-3.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_variables.py` & `twill-3.2.3/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/test_wsgi.py` & `twill-3.2.3/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tests/utils.py` & `twill-3.2.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `twill-3.2.2/tox.ini` & `twill-3.2.3/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tox]
 envlist = py3{8,9,10,11,12}, ruff, mypy, docs, manifest
 
 [testenv:ruff]
 basepython = python3.11
-deps = ruff>=0.1.14,<0.2
+deps = ruff>=0.3,<0.4
 commands =
     ruff check src/twill tests extras
     ruff format --check src/twill tests extras
 
 [testenv:mypy]
 basepython = python3.11
 deps =
```

