# Comparing `tmp/fastlifeweb-0.6.0.tar.gz` & `tmp/fastlifeweb-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlifeweb-0.6.0.tar", max compression
+gzip compressed data, was "fastlifeweb-0.6.1.tar", max compression
```

## Comparing `fastlifeweb-0.6.0.tar` & `fastlifeweb-0.6.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1504 2024-01-05 08:56:46.068218 fastlifeweb-0.6.0/LICENSE
--rw-r--r--   0        0        0      510 2024-04-13 13:57:35.096106 fastlifeweb-0.6.0/README.md
--rw-r--r--   0        0        0     2146 2024-04-25 21:24:25.508890 fastlifeweb-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      317 2024-04-25 16:49:13.210655 fastlifeweb-0.6.0/src/fastlife/__init__.py
--rw-r--r--   0        0        0       91 2024-01-14 12:49:19.832886 fastlifeweb-0.6.0/src/fastlife/configurator/__init__.py
--rw-r--r--   0        0        0      216 2024-03-29 07:03:39.778516 fastlifeweb-0.6.0/src/fastlife/configurator/base.py
--rw-r--r--   0        0        0     5740 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/configurator/configurator.py
--rw-r--r--   0        0        0     1463 2024-04-13 13:57:35.099439 fastlifeweb-0.6.0/src/fastlife/configurator/registry.py
--rw-r--r--   0        0        0     1489 2024-04-13 13:57:35.099439 fastlifeweb-0.6.0/src/fastlife/configurator/settings.py
--rw-r--r--   0        0        0        0 2023-09-22 06:52:58.847518 fastlifeweb-0.6.0/src/fastlife/py.typed
--rw-r--r--   0        0        0        0 2023-09-18 06:50:01.267211 fastlifeweb-0.6.0/src/fastlife/request/__init__.py
--rw-r--r--   0        0        0     3713 2024-04-25 16:58:19.366153 fastlifeweb-0.6.0/src/fastlife/request/form_data.py
--rw-r--r--   0        0        0     3237 2024-04-25 17:04:06.717636 fastlifeweb-0.6.0/src/fastlife/request/model_result.py
--rw-r--r--   0        0        0        0 2024-01-14 12:49:19.832886 fastlifeweb-0.6.0/src/fastlife/security/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/security/csrf.py
--rw-r--r--   0        0        0      509 2024-03-29 07:03:39.778516 fastlifeweb-0.6.0/src/fastlife/security/policy.py
--rw-r--r--   0        0        0      838 2024-03-29 07:03:39.778516 fastlifeweb-0.6.0/src/fastlife/session/__init__.py
--rw-r--r--   0        0        0     3049 2024-04-19 06:48:48.276132 fastlifeweb-0.6.0/src/fastlife/session/middleware.py
--rw-r--r--   0        0        0     1458 2024-03-29 07:03:39.778516 fastlifeweb-0.6.0/src/fastlife/session/serializer.py
--rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/shared_utils/__init__.py
--rw-r--r--   0        0        0      472 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/shared_utils/infer.py
--rw-r--r--   0        0        0     1410 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/shared_utils/resolver.py
--rw-r--r--   0        0        0      677 2024-04-13 13:57:35.099439 fastlifeweb-0.6.0/src/fastlife/templates/A.jinja
--rw-r--r--   0        0        0     1137 2024-04-13 13:57:35.099439 fastlifeweb-0.6.0/src/fastlife/templates/Button.jinja
--rw-r--r--   0        0        0      447 2024-04-21 09:51:45.697435 fastlifeweb-0.6.0/src/fastlife/templates/Checkbox.jinja
--rw-r--r--   0        0        0       59 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/CsrfToken.jinja
--rw-r--r--   0        0        0      367 2024-04-20 12:30:01.651834 fastlifeweb-0.6.0/src/fastlife/templates/Form.jinja
--rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/H1.jinja
--rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/H2.jinja
--rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/H3.jinja
--rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/H4.jinja
--rw-r--r--   0        0        0      193 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/H5.jinja
--rw-r--r--   0        0        0      191 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/H6.jinja
--rw-r--r--   0        0        0      120 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/templates/Hidden.jinja
--rw-r--r--   0        0        0      638 2024-04-14 21:06:08.222497 fastlifeweb-0.6.0/src/fastlife/templates/Input.jinja
--rw-r--r--   0        0        0      170 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/Label.jinja
--rw-r--r--   0        0        0      121 2024-04-15 06:29:06.881534 fastlifeweb-0.6.0/src/fastlife/templates/Option.jinja
--rw-r--r--   0        0        0      164 2024-04-13 13:57:35.102773 fastlifeweb-0.6.0/src/fastlife/templates/P.jinja
--rw-r--r--   0        0        0      723 2024-04-13 13:57:35.106106 fastlifeweb-0.6.0/src/fastlife/templates/Radio.jinja
--rw-r--r--   0        0        0      480 2024-04-20 16:07:29.325194 fastlifeweb-0.6.0/src/fastlife/templates/Select.jinja
--rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/templates/__init__.py
--rw-r--r--   0        0        0      281 2024-04-21 07:55:52.000197 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Boolean.jinja
--rw-r--r--   0        0        0      670 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Checklist.jinja
--rw-r--r--   0        0        0      500 2024-04-15 06:29:02.724849 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Dropdown.jinja
--rw-r--r--   0        0        0      121 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Error.jinja
--rw-r--r--   0        0        0       83 2024-03-30 15:07:08.088027 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Hidden.jinja
--rw-r--r--   0        0        0      123 2024-04-13 13:57:35.106106 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Hint.jinja
--rw-r--r--   0        0        0      449 2024-04-13 13:57:35.106106 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Model.jinja
--rw-r--r--   0        0        0     1380 2024-04-14 07:07:58.770652 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Sequence.jinja
--rw-r--r--   0        0        0      450 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Text.jinja
--rw-r--r--   0        0        0      950 2024-04-15 05:32:37.810352 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Union.jinja
--rw-r--r--   0        0        0      287 2024-04-24 06:47:08.537681 fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Widget.jinja
--rw-r--r--   0        0        0      234 2024-04-13 13:57:35.106106 fastlifeweb-0.6.0/src/fastlife/templating/__init__.py
--rw-r--r--   0        0        0     1378 2024-04-13 13:57:35.109439 fastlifeweb-0.6.0/src/fastlife/templating/binding.py
--rw-r--r--   0        0        0      181 2024-04-13 13:57:35.109439 fastlifeweb-0.6.0/src/fastlife/templating/renderer/__init__.py
--rw-r--r--   0        0        0     1552 2024-04-25 16:59:39.386488 fastlifeweb-0.6.0/src/fastlife/templating/renderer/abstract.py
--rw-r--r--   0        0        0     3977 2024-04-25 16:59:53.489880 fastlifeweb-0.6.0/src/fastlife/templating/renderer/jinjax.py
--rw-r--r--   0        0        0        0 2023-12-02 23:16:17.801084 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/__init__.py
--rw-r--r--   0        0        0     2808 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/base.py
--rw-r--r--   0        0        0      436 2024-04-24 05:54:40.214145 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/boolean.py
--rw-r--r--   0        0        0      850 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/checklist.py
--rw-r--r--   0        0        0      901 2024-04-14 07:07:58.773985 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/dropdown.py
--rw-r--r--   0        0        0    14162 2024-04-25 16:59:43.529838 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/factory.py
--rw-r--r--   0        0        0      308 2024-04-14 07:07:58.773985 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/hidden.py
--rw-r--r--   0        0        0      986 2024-04-20 17:18:08.717664 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/model.py
--rw-r--r--   0        0        0     1347 2024-04-14 07:07:58.773985 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/sequence.py
--rw-r--r--   0        0        0      879 2024-04-25 16:49:13.213989 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/text.py
--rw-r--r--   0        0        0     1689 2024-04-14 07:07:58.777319 fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/union.py
--rw-r--r--   0        0        0       67 2023-09-16 21:42:04.218390 fastlifeweb-0.6.0/src/fastlife/testing/__init__.py
--rw-r--r--   0        0        0    20220 2024-04-25 21:22:58.432744 fastlifeweb-0.6.0/src/fastlife/testing/testclient.py
--rw-r--r--   0        0        0      154 2024-01-14 12:49:19.836219 fastlifeweb-0.6.0/src/fastlife/views/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-25 16:56:28.099028 fastlifeweb-0.6.0/src/fastlife/views/pydantic_form.py
--rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 fastlifeweb-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-01-05 08:56:46.068218 fastlifeweb-0.6.1/LICENSE
+-rw-r--r--   0        0        0      510 2024-04-13 13:57:35.096106 fastlifeweb-0.6.1/README.md
+-rw-r--r--   0        0        0     2147 2024-04-27 06:30:38.110546 fastlifeweb-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      317 2024-04-25 16:49:13.210655 fastlifeweb-0.6.1/src/fastlife/__init__.py
+-rw-r--r--   0        0        0       91 2024-01-14 12:49:19.832886 fastlifeweb-0.6.1/src/fastlife/configurator/__init__.py
+-rw-r--r--   0        0        0      216 2024-03-29 07:03:39.778516 fastlifeweb-0.6.1/src/fastlife/configurator/base.py
+-rw-r--r--   0        0        0     5740 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/configurator/configurator.py
+-rw-r--r--   0        0        0     1463 2024-04-13 13:57:35.099439 fastlifeweb-0.6.1/src/fastlife/configurator/registry.py
+-rw-r--r--   0        0        0     1489 2024-04-13 13:57:35.099439 fastlifeweb-0.6.1/src/fastlife/configurator/settings.py
+-rw-r--r--   0        0        0        0 2023-09-22 06:52:58.847518 fastlifeweb-0.6.1/src/fastlife/py.typed
+-rw-r--r--   0        0        0        0 2023-09-18 06:50:01.267211 fastlifeweb-0.6.1/src/fastlife/request/__init__.py
+-rw-r--r--   0        0        0     3713 2024-04-25 16:58:19.366153 fastlifeweb-0.6.1/src/fastlife/request/form_data.py
+-rw-r--r--   0        0        0     3237 2024-04-25 17:04:06.717636 fastlifeweb-0.6.1/src/fastlife/request/model_result.py
+-rw-r--r--   0        0        0        0 2024-01-14 12:49:19.832886 fastlifeweb-0.6.1/src/fastlife/security/__init__.py
+-rw-r--r--   0        0        0     1025 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/security/csrf.py
+-rw-r--r--   0        0        0      509 2024-03-29 07:03:39.778516 fastlifeweb-0.6.1/src/fastlife/security/policy.py
+-rw-r--r--   0        0        0      838 2024-03-29 07:03:39.778516 fastlifeweb-0.6.1/src/fastlife/session/__init__.py
+-rw-r--r--   0        0        0     3049 2024-04-19 06:48:48.276132 fastlifeweb-0.6.1/src/fastlife/session/middleware.py
+-rw-r--r--   0        0        0     1458 2024-03-29 07:03:39.778516 fastlifeweb-0.6.1/src/fastlife/session/serializer.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/shared_utils/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-25 16:49:13.213989 fastlifeweb-0.6.1/src/fastlife/shared_utils/infer.py
+-rw-r--r--   0        0        0     1410 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/shared_utils/resolver.py
+-rw-r--r--   0        0        0      677 2024-04-13 13:57:35.099439 fastlifeweb-0.6.1/src/fastlife/templates/A.jinja
+-rw-r--r--   0        0        0     1137 2024-04-13 13:57:35.099439 fastlifeweb-0.6.1/src/fastlife/templates/Button.jinja
+-rw-r--r--   0        0        0      447 2024-04-21 09:51:45.697435 fastlifeweb-0.6.1/src/fastlife/templates/Checkbox.jinja
+-rw-r--r--   0        0        0       59 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/CsrfToken.jinja
+-rw-r--r--   0        0        0      367 2024-04-20 12:30:01.651834 fastlifeweb-0.6.1/src/fastlife/templates/Form.jinja
+-rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/H1.jinja
+-rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/H2.jinja
+-rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/H3.jinja
+-rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/H4.jinja
+-rw-r--r--   0        0        0      193 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/H5.jinja
+-rw-r--r--   0        0        0      191 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/H6.jinja
+-rw-r--r--   0        0        0      120 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/templates/Hidden.jinja
+-rw-r--r--   0        0        0      638 2024-04-14 21:06:08.222497 fastlifeweb-0.6.1/src/fastlife/templates/Input.jinja
+-rw-r--r--   0        0        0      170 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/Label.jinja
+-rw-r--r--   0        0        0      121 2024-04-15 06:29:06.881534 fastlifeweb-0.6.1/src/fastlife/templates/Option.jinja
+-rw-r--r--   0        0        0      164 2024-04-13 13:57:35.102773 fastlifeweb-0.6.1/src/fastlife/templates/P.jinja
+-rw-r--r--   0        0        0      723 2024-04-13 13:57:35.106106 fastlifeweb-0.6.1/src/fastlife/templates/Radio.jinja
+-rw-r--r--   0        0        0      480 2024-04-20 16:07:29.325194 fastlifeweb-0.6.1/src/fastlife/templates/Select.jinja
+-rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/templates/__init__.py
+-rw-r--r--   0        0        0      467 2024-04-26 09:16:07.765719 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Boolean.jinja
+-rw-r--r--   0        0        0      775 2024-04-26 13:16:48.166348 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Checklist.jinja
+-rw-r--r--   0        0        0      548 2024-04-26 13:16:09.336225 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Dropdown.jinja
+-rw-r--r--   0        0        0      121 2024-04-25 16:49:13.213989 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Error.jinja
+-rw-r--r--   0        0        0       83 2024-03-30 15:07:08.088027 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Hidden.jinja
+-rw-r--r--   0        0        0      123 2024-04-13 13:57:35.106106 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Hint.jinja
+-rw-r--r--   0        0        0      501 2024-04-26 13:26:56.471598 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Model.jinja
+-rw-r--r--   0        0        0     1430 2024-04-26 13:22:29.780757 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Sequence.jinja
+-rw-r--r--   0        0        0      450 2024-04-25 16:49:13.213989 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Text.jinja
+-rw-r--r--   0        0        0      992 2024-04-26 13:23:26.807603 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Union.jinja
+-rw-r--r--   0        0        0      287 2024-04-24 06:47:08.537681 fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Widget.jinja
+-rw-r--r--   0        0        0      234 2024-04-13 13:57:35.106106 fastlifeweb-0.6.1/src/fastlife/templating/__init__.py
+-rw-r--r--   0        0        0     1378 2024-04-13 13:57:35.109439 fastlifeweb-0.6.1/src/fastlife/templating/binding.py
+-rw-r--r--   0        0        0      181 2024-04-13 13:57:35.109439 fastlifeweb-0.6.1/src/fastlife/templating/renderer/__init__.py
+-rw-r--r--   0        0        0     1552 2024-04-25 16:59:39.386488 fastlifeweb-0.6.1/src/fastlife/templating/renderer/abstract.py
+-rw-r--r--   0        0        0     3977 2024-04-25 16:59:53.489880 fastlifeweb-0.6.1/src/fastlife/templating/renderer/jinjax.py
+-rw-r--r--   0        0        0        0 2023-12-02 23:16:17.801084 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/__init__.py
+-rw-r--r--   0        0        0     2808 2024-04-25 16:49:13.213989 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/base.py
+-rw-r--r--   0        0        0      544 2024-04-26 08:59:51.842944 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/boolean.py
+-rw-r--r--   0        0        0     1009 2024-04-26 13:19:29.753523 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/checklist.py
+-rw-r--r--   0        0        0     1009 2024-04-26 13:13:08.312322 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/dropdown.py
+-rw-r--r--   0        0        0    14779 2024-04-27 06:19:17.648436 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/factory.py
+-rw-r--r--   0        0        0      308 2024-04-14 07:07:58.773985 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/hidden.py
+-rw-r--r--   0        0        0     1094 2024-04-26 13:26:44.128226 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/model.py
+-rw-r--r--   0        0        0     1455 2024-04-26 13:20:20.643684 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/sequence.py
+-rw-r--r--   0        0        0      879 2024-04-25 16:49:13.213989 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/text.py
+-rw-r--r--   0        0        0     1797 2024-04-26 13:23:14.240897 fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/union.py
+-rw-r--r--   0        0        0       67 2023-09-16 21:42:04.218390 fastlifeweb-0.6.1/src/fastlife/testing/__init__.py
+-rw-r--r--   0        0        0    20220 2024-04-25 21:22:58.432744 fastlifeweb-0.6.1/src/fastlife/testing/testclient.py
+-rw-r--r--   0        0        0      154 2024-01-14 12:49:19.836219 fastlifeweb-0.6.1/src/fastlife/views/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-25 16:56:28.099028 fastlifeweb-0.6.1/src/fastlife/views/pydantic_form.py
+-rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 fastlifeweb-0.6.1/PKG-INFO
```

### Comparing `fastlifeweb-0.6.0/LICENSE` & `fastlifeweb-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/pyproject.toml` & `fastlifeweb-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
   "Development Status :: 4 - Beta",
   "Framework :: AsyncIO",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet :: WWW/HTTP",
 ]
-version = "0.6.0"
+version = "0.6.1"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 beautifulsoup4 = {version = "^4.12.2", extras = ["testing"]}
 behave = "^1.2.6"
 fastapi = "^0.110.0"
 itsdangerous = "^2.1.2"
 jinjax = "^0.34"
 markupsafe = "^2.1.3"
 multidict = "^6.0.5"
-pydantic = "2.5.1"
+pydantic = "^2.5.3"
 pydantic-settings = "^2.0.3"
 python-multipart = "^0.0.6"
 venusian = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = "^4.12.2"
 black = "^23.3.0"
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/configurator/configurator.py` & `fastlifeweb-0.6.1/src/fastlife/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/configurator/registry.py` & `fastlifeweb-0.6.1/src/fastlife/configurator/registry.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/configurator/settings.py` & `fastlifeweb-0.6.1/src/fastlife/configurator/settings.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/request/form_data.py` & `fastlifeweb-0.6.1/src/fastlife/request/form_data.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/request/model_result.py` & `fastlifeweb-0.6.1/src/fastlife/request/model_result.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/security/csrf.py` & `fastlifeweb-0.6.1/src/fastlife/security/csrf.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/session/__init__.py` & `fastlifeweb-0.6.1/src/fastlife/session/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/session/middleware.py` & `fastlifeweb-0.6.1/src/fastlife/session/middleware.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/session/serializer.py` & `fastlifeweb-0.6.1/src/fastlife/session/serializer.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/shared_utils/resolver.py` & `fastlifeweb-0.6.1/src/fastlife/shared_utils/resolver.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/A.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/A.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/Button.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/Button.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/Input.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/Input.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/Radio.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/Radio.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Checklist.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Checklist.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 #}
 
 <pydantic_form.Widget widget={widget} removable={widget.removable}>
   <div class="pt-4">
     <details open>
       <summary class="justify-between items-center font-medium cursor-pointer">
         <H3>{{widget.title}}</H3>
+        <pydantic_form.Error text={widget.error} />
       </summary>
       <div>
         {% for value in widget.value %}
         <div class="flex items-center mb-4">
           <Checkbox name={value.field_name} type="checkbox" id={value.id} value={value.value} checked={value.checked} />
           <Label for={value.id} class="ms-2 text-base text-neutral-900 dark:text-white">{{value.label}}</Label>
+          <pydantic_form.Error text={value.error} />
         </div>
         {% endfor %}
       </div>
   </div>
 </pydantic_form.Widget>
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Sequence.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Sequence.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {# def widget, children_widgets, type #}
 
 <pydantic_form.Widget widget={widget} removable={widget.removable}>
   <details id="{{widget.id}}" open>
     <summary class="justify-between items-center font-medium cursor-pointer">
       <H3>{{widget.title}}</H3>
+      <pydantic_form.Error text={widget.error} />
     </summary>
     <div>
       {% set fnGetName = "get" + widget.id.replace("-", "_") %}
       <script>
         function {{ fnGetName }} () {
           const el = document.getElementById("{{widget.id}}-content");
           const len = el.dataset.length;
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templates/pydantic_form/Union.jinja` & `fastlifeweb-0.6.1/src/fastlife/templates/pydantic_form/Union.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {# def widget, child, types, parent_type #}
 
 <pydantic_form.Widget widget={widget}>
   <div id="{{widget.id}}">
     <details open>
       <summary class="justify-between items-center font-medium cursor-pointer">
         <H3>{{widget.title}}</H3>
+        <pydantic_form.Error text={widget.error} />
       </summary>
       <div hx-sync="this" id="{{widget.id}}-child">
         {% if child %}
         {{ child }}
         {% else %}
         {% for typ in types %}
-        <Button type="button" hx-target="closest div" hx-get={typ.url} hx-vals={typ.params|tojson}
-          id={typ.id}
+        <Button type="button" hx-target="closest div" hx-get={typ.url} hx-vals={typ.params|tojson} id={typ.id}
           onclick={"document.getElementById('" + widget.id +"-remove-btn').hidden=false"}>{{typ.title}}</Button>
         {% endfor %}
         {% endif %}
       </div>
-      <Button type="button" id={widget.id + "-remove-btn" } hx-target={"#" + widget.id} hx-vals={parent_type.params|tojson}
-        hx-get={parent_type.url} hidden={not child}>
+      <Button type="button" id={widget.id + "-remove-btn" } hx-target={"#" + widget.id}
+        hx-vals={parent_type.params|tojson} hx-get={parent_type.url} hidden={not child}>
         Remove
       </Button>
     </details>
   </div>
 </pydantic_form.Widget>
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/binding.py` & `fastlifeweb-0.6.1/src/fastlife/templating/binding.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/abstract.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/abstract.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/jinjax.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/jinjax.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/base.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/base.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/checklist.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/checklist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Sequence
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from .base import Widget
 
 
 class Checkable(BaseModel):
     label: str
     name: str
     value: str
     token: str
     checked: bool
+    error: str | None = Field(default=None)
 
     @property
     def id(self) -> str:
         id = f"{self.name}-{self.value}-{self.token}"
         return id.replace(".", "-").replace("_", "-")
 
     @property
@@ -25,16 +26,22 @@
 class ChecklistWidget(Widget[Sequence[Checkable]]):
     def __init__(
         self,
         name: str,
         *,
         title: str | None,
         value: Sequence[Checkable],
+        error: str | None = None,
         token: str,
         removable: bool,
     ) -> None:
         super().__init__(
-            name, value=value, token=token, title=title, removable=removable
+            name,
+            value=value,
+            error=error,
+            token=token,
+            title=title,
+            removable=removable,
         )
 
     def get_template(self) -> str:
         return "pydantic_form.Checklist"
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/dropdown.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/dropdown.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 class DropDownWidget(Widget[str]):
     def __init__(
         self,
         name: str,
         *,
         title: Optional[str],
         value: Optional[str] = None,
+        error: str | None = None,
         options: Sequence[Tuple[str, str]] | Sequence[str],
         removable: bool = False,
         token: Optional[str] = None,
         hint: Optional[str] = None,
     ) -> None:
         super().__init__(
-            name, value=value, title=title, token=token, removable=removable
+            name,
+            value=value,
+            error=error,
+            title=title,
+            token=token,
+            removable=removable,
         )
         self.options: list[dict[str, str]] = []
         for opt in options:
             if isinstance(opt, tuple):
                 self.options.append({"value": opt[0], "text": opt[1]})
             else:
                 self.options.append({"value": opt, "text": opt})
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/factory.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                         widget(
                             name,
                             value=value,
                             removable=removable,
                             title=field.title if field else "",
                             aria_label=field.description if field else None,
                             token=self.token,
+                            error=form_errors.get(name),
                         ),
                     )
 
         type_origin = get_origin(typ)
         if type_origin:
             if is_union(typ):
                 return self.build_union(name, typ, field, value, form_errors, removable)
@@ -171,14 +172,15 @@
             )
         return ModelWidget(
             field_name,
             value=list(ret.values()),
             removable=removable,
             title=get_title(typ),
             token=self.token,
+            error=form_errors.get(field_name),
         )
 
     def build_union(
         self,
         field_name: str,
         field_type: Type[Any],
         field: Optional[FieldInfo],
@@ -229,14 +231,15 @@
             field_name,
             # we assume those types are BaseModel
             value=child,
             children_types=types,  # type: ignore
             title=field.title if field else "",
             token=self.token,
             removable=removable,
+            error=form_errors.get(field_name),
         )
 
         return widget
 
     def build_sequence(
         self,
         field_name: str,
@@ -263,14 +266,15 @@
             field_name,
             hint=field.description if field else "",
             title=field.title if field else "",
             value=items,
             item_type=typ,  # type: ignore
             token=self.token,
             removable=removable,
+            error=form_errors.get(field_name),
         )
 
     def build_set(
         self,
         field_name: str,
         field_type: Type[Any],
         field: Optional[FieldInfo],
@@ -287,40 +291,43 @@
                 choices = [
                     Checkable(
                         label=c,
                         value=c,
                         checked=c in value if value else False,  # type: ignore
                         name=field_name,
                         token=self.token,
+                        error=form_errors.get(f"{field_name}-{c}"),
                     )
                     for c in litchoice
                 ]
 
             else:
                 raise NotImplementedError
         elif issubclass(choice_wrapper, Enum):
             choices = [
                 Checkable(
                     label=e.value,
                     value=e.name,
                     checked=e.name in value if value else False,  # type: ignore
                     name=field_name,
                     token=self.token,
+                    error=form_errors.get(f"{field_name}-{e.name}"),
                 )
                 for e in choice_wrapper
             ]
         else:
             raise NotImplementedError
 
         return ChecklistWidget(
             field_name,
             title=field.title if field else "",
             token=self.token,
             value=choices,
             removable=removable,
+            error=form_errors.get(field_name),
         )
 
     def build_boolean(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
@@ -330,14 +337,15 @@
     ) -> Widget[Any]:
         return BooleanWidget(
             field_name,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=value,
+            error=form_errors.get(field_name),
         )
 
     def build_emailtype(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
@@ -350,14 +358,15 @@
             hint=field.description if field else "",
             input_type="email",
             placeholder=str(field.examples[0]) if field and field.examples else None,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=str(value),
+            error=form_errors.get(field_name),
         )
 
     def build_secretstr(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
@@ -370,14 +379,15 @@
             hint=field.description if field else "",
             input_type="password",
             placeholder=str(field.examples[0]) if field and field.examples else None,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=value.get_secret_value() if isinstance(value, SecretStr) else value,
+            error=form_errors.get(field_name),
         )
 
     def build_literal(
         self,
         field_name: str,
         field_type: Type[Any],  # a literal actually
         field: FieldInfo | None,
@@ -395,14 +405,15 @@
         return DropDownWidget(
             field_name,
             options=choices,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=str(value),
+            error=form_errors.get(field_name),
         )
 
     def build_enum(
         self,
         field_name: str,
         field_type: Type[Any],  # an enum subclass
         field: FieldInfo | None,
@@ -414,14 +425,15 @@
         return DropDownWidget(
             field_name,
             options=options,  # type: ignore
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=str(value),
+            error=form_errors.get(field_name),
         )
 
     def build_simpletype(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/model.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 
 class ModelWidget(Widget[Sequence[Widget[Any]]]):
     def __init__(
         self,
         name: str,
         *,
         value: Sequence[Widget[Any]],
+        error: str | None = None,
         removable: bool,
         title: str,
         token: str,
     ):
         super().__init__(
-            name, title=title, value=value, removable=removable, token=token
+            name,
+            title=title,
+            value=value,
+            error=error,
+            removable=removable,
+            token=token,
         )
 
     def get_template(self) -> str:
         return "pydantic_form.Model"
 
     def to_html(self, renderer: AbstractTemplateRenderer) -> Markup:
         """Return the html version"""
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/sequence.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,26 @@
     def __init__(
         self,
         name: str,
         *,
         title: Optional[str],
         hint: Optional[str],
         value: Optional[Sequence[Widget[Any]]],
+        error: str | None = None,
         item_type: Type[Any],
         token: str,
         removable: bool,
     ):
         super().__init__(
-            name, value=value, title=title, token=token, removable=removable
+            name,
+            value=value,
+            error=error,
+            title=title,
+            token=token,
+            removable=removable,
         )
         self.item_type = item_type
         self.hint = hint
 
     def get_template(self) -> str:
         return "pydantic_form/Sequence"
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/text.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/text.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/templating/renderer/widgets/union.py` & `fastlifeweb-0.6.1/src/fastlife/templating/renderer/widgets/union.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,26 @@
 class UnionWidget(Widget[Widget[Any]]):
     def __init__(
         self,
         name: str,
         *,
         title: Optional[str],
         value: Optional[Widget[Any]],
+        error: str | None = None,
         children_types: Sequence[Type[BaseModel]],
         token: str,
         removable: bool,
     ):
         super().__init__(
-            name, value=value, title=title, token=token, removable=removable
+            name,
+            value=value,
+            error=error,
+            title=title,
+            token=token,
+            removable=removable,
         )
         self.children_types = children_types
         self.parent_name = name
 
     def build_types(self, route_prefix: str) -> Sequence[TypeWrapper]:
         return [
             TypeWrapper(typ, route_prefix, self.name, self.token)
```

### Comparing `fastlifeweb-0.6.0/src/fastlife/testing/testclient.py` & `fastlifeweb-0.6.1/src/fastlife/testing/testclient.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/src/fastlife/views/pydantic_form.py` & `fastlifeweb-0.6.1/src/fastlife/views/pydantic_form.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.6.0/PKG-INFO` & `fastlifeweb-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlifeweb
-Version: 0.6.0
+Version: 0.6.1
 Summary: High-level web framework
 Home-page: https://github.com/mardiros/fastlife
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Requires-Dist: beautifulsoup4[testing] (>=4.12.2,<5.0.0)
 Requires-Dist: behave (>=1.2.6,<2.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
 Requires-Dist: jinjax (>=0.34,<0.35)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: multidict (>=6.0.5,<7.0.0)
-Requires-Dist: pydantic (==2.5.1)
+Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: venusian (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/mardiros/fastlife
 Description-Content-Type: text/markdown
 
 # Fastlife
```

