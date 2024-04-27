# Comparing `tmp/ypricemagic-3.4.9.tar.gz` & `tmp/ypricemagic-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-3.4.9.tar", last modified: Mon Apr 15 21:58:27 2024, max compression
+gzip compressed data, was "ypricemagic-3.5.0.tar", last modified: Sat Apr 27 19:33:45 2024, max compression
```

## Comparing `ypricemagic-3.4.9.tar` & `ypricemagic-3.5.0.tar`

### file list

```diff
@@ -1,205 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.377562 ypricemagic-3.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.381562 ypricemagic-3.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.381562 ypricemagic-3.4.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.377562 ypricemagic-3.4.9/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.377562 ypricemagic-3.4.9/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/scripts/debug-curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/scripts/debug-price.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/test_uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/dex/test_velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.385562 ypricemagic-3.4.9/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/y/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/y/_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.389562 ypricemagic-3.4.9/y/_db/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/_ep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/price.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/_db/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/classes/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24922 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/interfaces/uniswap/velov2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.393562 ypricemagic-3.4.9/y/prices/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/mooniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/solidly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/uniswap/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/dex/velodrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/popsicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/rkp3r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/solidex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.397562 ypricemagic-3.4.9/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/y/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-15 21:58:17.000000 ypricemagic-3.4.9/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:58:27.401562 ypricemagic-3.4.9/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 21:58:27.000000 ypricemagic-3.4.9/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.402852 ypricemagic-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.374852 ypricemagic-3.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.382852 ypricemagic-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-27 19:33:45.402852 ypricemagic-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.382852 ypricemagic-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.374852 ypricemagic-3.5.0/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.374852 ypricemagic-3.5.0/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.382852 ypricemagic-3.5.0/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.382852 ypricemagic-3.5.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/scripts/debug-curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/scripts/debug-price.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 19:33:45.402852 ypricemagic-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.382852 ypricemagic-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.382852 ypricemagic-3.5.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/dex/test_uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/dex/test_velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/y/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.386852 ypricemagic-3.5.0/y/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/_db/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/_ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/_db/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25389 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32517 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.390852 ypricemagic-3.5.0/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/interfaces/uniswap/velov2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.394852 ypricemagic-3.5.0/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.394852 ypricemagic-3.5.0/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.394852 ypricemagic-3.5.0/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/mooniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/solidly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.394852 ypricemagic-3.5.0/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31574 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/uniswap/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/dex/velodrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.394852 ypricemagic-3.5.0/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.394852 ypricemagic-3.5.0/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/rkp3r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/solidex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.398852 ypricemagic-3.5.0/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22881 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.398852 ypricemagic-3.5.0/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.398852 ypricemagic-3.5.0/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.398852 ypricemagic-3.5.0/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15476 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.398852 ypricemagic-3.5.0/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 19:33:34.000000 ypricemagic-3.5.0/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:33:45.402852 ypricemagic-3.5.0/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-27 19:33:45.000000 ypricemagic-3.5.0/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-27 19:33:45.000000 ypricemagic-3.5.0/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:33:45.000000 ypricemagic-3.5.0/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-27 19:33:45.000000 ypricemagic-3.5.0/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 19:33:45.000000 ypricemagic-3.5.0/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-3.4.9/.github/workflows/codeql-analysis.yml` & `ypricemagic-3.5.0/.github/workflows/codeql-analysis.yml`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     branches: [ master, dev ]
     paths:
       - '**.py'
       - '**/codeql-analysis.yml'
   schedule:
     - cron: '41 4 * * 2'
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+  
 jobs:
   analyze:
     name: Analyze
     runs-on: ubuntu-latest
     permissions:
       actions: read
       contents: read
```

### Comparing `ypricemagic-3.4.9/.github/workflows/deploy-docs.yml` & `ypricemagic-3.5.0/.github/workflows/deploy-docs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
 permissions:
   contents: write
   id-token: write
   pages: write
   
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   build-and-deploy:
     runs-on: ubuntu-latest
     steps:
       - name: Check out code
         uses: actions/checkout@v2
```

### Comparing `ypricemagic-3.4.9/.github/workflows/pytest.yaml` & `ypricemagic-3.5.0/.github/workflows/pytest.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 name: PyTest
 
 on:
-  push:
-    branch: dev
-    paths:
-      - '**.py'
-      - '**/pytest.yaml'
   pull_request:
     # The branches below must be a subset of the branches above
     branches: [ master, dev ]
     paths:
       - '**.py'
       - '**/pytest.yaml'
+      
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     #timeout-minutes: 10
     strategy:
       fail-fast: false
@@ -93,8 +92,8 @@
           ETHERSCAN_TOKEN: ${{ secrets.ETHERSCAN_TOKEN }}
           BSCSCAN_TOKEN: ${{ secrets.BSCSCAN_TOKEN }}
           POLYGONSCAN_TOKEN: ${{ secrets.POLYGONSCAN_TOKEN }}
           FTMSCAN_TOKEN: ${{ secrets.FTMSCAN_TOKEN }}
           ARBISCAN_TOKEN: ${{ secrets.ARBISCAN_TOKEN }}
           OPTISCAN_TOKEN: ${{ secrets.OPTISCAN_TOKEN }}
         run: make test
-      
+
```

### Comparing `ypricemagic-3.4.9/.github/workflows/release.yaml` & `ypricemagic-3.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/CONTRIBUTING.md` & `ypricemagic-3.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/LICENSE.txt` & `ypricemagic-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/Makefile` & `ypricemagic-3.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/PKG-INFO` & `ypricemagic-3.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ypricemagic
-Version: 3.4.9
+Version: 3.5.0
 Summary: Use this tool to extract historical on-chain price data from an archive node. Shoutout to @bantg and @nymmrx for their awesome work on yearn-exporter that made this library possible.
 Home-page: https://github.com/BobTheBuidler/ypricemagic
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 License-File: LICENSE.txt
 Requires-Dist: bobs_lazy_logging==0.0.4
 Requires-Dist: cachetools<4.3,>=4.1.1
 Requires-Dist: checksum_dict>=1.1.1
-Requires-Dist: dank_mids>=4.20.86
+Requires-Dist: dank_mids>=4.20.88
 Requires-Dist: eth-brownie<1.21,>=1.19.3
 Requires-Dist: eth_retry<0.2,>=0.1.19
-Requires-Dist: ez-a-sync<0.20,>=0.18.2
+Requires-Dist: ez-a-sync<0.21,>=0.20.5
 Requires-Dist: inflection<0.6,>=0.1
 Requires-Dist: joblib>=1.0.1
 Requires-Dist: multicall>=0.8.2
 Requires-Dist: pony
```

### Comparing `ypricemagic-3.4.9/README.md` & `ypricemagic-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/Makefile` & `ypricemagic-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/alabaster.css` & `ypricemagic-3.5.0/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/basic.css` & `ypricemagic-3.5.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/doctools.js` & `ypricemagic-3.5.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/language_data.js` & `ypricemagic-3.5.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/pygments.css` & `ypricemagic-3.5.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/searchtools.js` & `ypricemagic-3.5.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/_build/html/_static/sphinx_highlight.js` & `ypricemagic-3.5.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/docs/conf.py` & `ypricemagic-3.5.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 author = 'BobTheBuidler'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
+    'sphinx.ext.viewcode',
     'sphinx.ext.napoleon',
     'sphinx.ext.intersphinx',
     'a_sync.sphinx.ext',
 ]
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
```

### Comparing `ypricemagic-3.4.9/docs/make.bat` & `ypricemagic-3.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/scripts/debug-curve.py` & `ypricemagic-3.5.0/scripts/debug-curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/scripts/debug-price.py` & `ypricemagic-3.5.0/scripts/debug-price.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/setup.py` & `ypricemagic-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/classes/test_erc20.py` & `ypricemagic-3.5.0/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/classes/test_singleton.py` & `ypricemagic-3.5.0/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/fixtures.py` & `ypricemagic-3.5.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/prices/dex/test_balancer.py` & `ypricemagic-3.5.0/tests/prices/dex/test_balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/prices/dex/test_uniswap.py` & `ypricemagic-3.5.0/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/prices/lending/test_aave.py` & `ypricemagic-3.5.0/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/prices/lending/test_compound.py` & `ypricemagic-3.5.0/tests/prices/lending/test_compound.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import pytest
 
 from tests.fixtures import blocks_for_contract
 from y.prices.lending.compound import CToken, compound
 
-CTOKENS = [ctoken.address for troller in compound.trollers.values() for ctoken in troller.__markets__]
+CTOKENS = [ctoken.address for troller in compound.trollers.values() for ctoken in troller.__markets__(sync=True)]
 
 @pytest.mark.parametrize('token', CTOKENS)
 def test_compound_pricing_sync(token):
     print(token)
     #if convert.to_address(token) == '0x892B14321a4FCba80669aE30Bd0cd99a7ECF6aC0':
     #    continue  # creth is broken
     ctoken = CToken(token)
```

### Comparing `ypricemagic-3.4.9/tests/prices/test_chainlink.py` & `ypricemagic-3.5.0/tests/prices/test_chainlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 async def test_chainlink_latest(token):
     if not await chainlink.get_price(token):
         feed = await chainlink.get_feed(token)
         latest_timestamp = await feed.latest_timestamp()
         if latest_timestamp and latest_timestamp + 24 * 60 * 60 < time.time():
             pytest.skip("feed is stale")
         try:
-            assert await feed.contract.aggregator.coroutine() == ZERO_ADDRESS, 'no current price available'
+            assert await feed.contract.aggregator == ZERO_ADDRESS, 'no current price available'
         except AttributeError as e:
             raise AttributeError(*e.args, feed) from e
 
 
 @mainnet_only
 @pytest.mark.parametrize('token', FEEDS)
 @pytest.mark.asyncio_cooperative
@@ -150,15 +150,15 @@
     price = await price
     if not price:
         feed = await chainlink.get_feed(token)
         latest_timestamp = await feed.latest_timestamp()
         if latest_timestamp and latest_timestamp + 24 * 60 * 60 < time.time():
             pytest.skip("feed is stale")
         try:
-            assert await feed.contract.aggregator.coroutine() == ZERO_ADDRESS, f'{feed} no price available before registry'
+            assert await feed.contract.aggregator == ZERO_ADDRESS, f'{feed} no price available before registry'
         except AttributeError as e:
             raise AttributeError(*e.args, feed) from e
 
 
 @pytest.mark.asyncio_cooperative
 async def test_chainlink_nonexistent():
     assert await chainlink.get_feed(ZERO_ADDRESS, sync=False) is None
```

### Comparing `ypricemagic-3.4.9/tests/prices/test_magic.py` & `ypricemagic-3.5.0/tests/prices/test_magic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import asyncio
 from typing import List
 
+import a_sync
 import pytest
 from brownie import chain
 
 from tests.prices.dex.test_uniswap import V1_TOKENS, V2_TOKENS
 from tests.prices.lending.test_aave import ATOKENS
 from tests.prices.lending.test_compound import CTOKENS
 from tests.prices.test_chainlink import FEEDS
@@ -50,15 +51,15 @@
 @pytest.mark.asyncio_cooperative
 async def test_get_prices(block):
     """
     Sometimes this will fail unnecessarily because Chainlink has added some more fiat feeds.
     Just add the failing identifier to 'chainlink_identifiers_not_tokens' below.
     """
     tokens = await relevant_tokens(ALL_TOKENS, block)
-    checked_separately = await asyncio.gather(*[get_price(token, block) for token in tokens])
+    checked_separately = await a_sync.map(get_price, tokens, block=block).values()
     checked_together = await magic.get_prices(tokens, block, fail_to_None=True, skip_cache=True, sync=False)
     for i in range(len(checked_together)):
         assert checked_together[i] == checked_separately[i], f'magic.get_prices price discrepancy for {tokens[i]}'
 
 async def get_price(token, block):
     """ This is just to diagnose issues with the test itself. We may need to exclude certain tokens. """
     try:
@@ -89,10 +90,9 @@
     "0x00000000000000000000000000000000000003d2",
     "0x00000000000000000000000000000000000003Da",
     "0xbBbBBBBbbBBBbbbBbbBbbbbBBbBbbbbBbBbbBBbB",
     "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE",
 ]
 
 async def relevant_tokens(tokens, block):
-    tokens = [token for token in tokens if token not in chainlink_identifiers_not_tokens]
-    creation_blocks = await asyncio.gather(*[contract_creation_block_async(convert.to_address(token)) for token in tokens])
-    return [token for token, deploy_block in zip(tokens, creation_blocks) if deploy_block and deploy_block <= block]
+    tokens = (convert.to_address(token) for token in tokens if token not in chainlink_identifiers_not_tokens)
+    return [token async for token, deploy_block in a_sync.map(contract_creation_block_async, tokens) if deploy_block and deploy_block <= block]
```

### Comparing `ypricemagic-3.4.9/tests/prices/test_popsicle.py` & `ypricemagic-3.5.0/tests/prices/test_popsicle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
-import asyncio
-
+import a_sync
 import pytest
 from brownie import chain
 
 from tests.fixtures import blocks_for_contract
 from y.constants import WRAPPED_GAS_COIN
 from y.networks import Network
 from y.prices import popsicle
@@ -47,10 +46,9 @@
         popsicle.get_price(WRAPPED_GAS_COIN)
 
 @pytest.mark.asyncio_cooperative
 @pytest.mark.parametrize('token',POPSICLES)
 async def test_popsicle_get_price(token):
     assert await popsicle.is_popsicle_lp(token, sync=False), 'Popsicle LP not recognized.'
     blocks = blocks_for_contract(token, 25)
-    prices = await asyncio.gather(*[popsicle.get_price(token, block, sync=False) for block in blocks])
-    for block, price in zip(blocks, prices):
+    async for block, price in a_sync.map(popsicle.get_price, blocks, token=token):
         assert price, f'Failed to fetch price for {token} at block {block}.'
```

### Comparing `ypricemagic-3.4.9/tests/prices/test_synthetix.py` & `ypricemagic-3.5.0/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/prices/test_yearn.py` & `ypricemagic-3.5.0/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/tests/prices/utils/test_buckets.py` & `ypricemagic-3.5.0/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/ENVIRONMENT_VARIABLES.py` & `ypricemagic-3.5.0/y/ENVIRONMENT_VARIABLES.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/__init__.py` & `ypricemagic-3.5.0/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/__init__.py` & `ypricemagic-3.5.0/y/_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/common.py` & `ypricemagic-3.5.0/y/_db/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,38 +136,49 @@
             logger.debug('%s loaded %s objects thru block %s from disk', self, len(self._objects), cached_thru)
             return cached_thru
         return None
 
 _E = TypeVar("_E", bound=_AsyncExecutorMixin)
     
 class Filter(_DiskCachedMixin[T, C]):
-    __slots__ = 'from_block', 'to_block', '_chunk_size', '_chunks_per_batch', '_db_task', '_exc', '_interval', '_lock', '_semaphore', '_sleep_fut', '_sleep_time', '_task', '_verbose', '__dict__'
+    # defaults are stored as class vars to keep instance dicts smaller
+    _chunk_size = BATCH_SIZE
+    _chunks_per_batch = None
+    _exc = None
+    _db_task = None
+    _sleep_fut = None
+    _sleep_time = 60
+    _task = None
+    _semaphore = None
+    _verbose = False
+    __slots__ = 'from_block', 'to_block', '_interval', '_lock', '__dict__'
     def __init__(
         self, 
         from_block: int,
         *, 
         chunk_size: int = BATCH_SIZE, 
         chunks_per_batch: Optional[int] = None,
         sleep_time: int = 60,
         semaphore: Optional[dank_mids.BlockSemaphore] = None,
         executor: Optional[_AsyncExecutorMixin] = None,
         is_reusable: bool = True,
         verbose: bool = False,
     ):
         self.from_block = from_block
-        self._chunk_size = chunk_size
-        self._chunks_per_batch = chunks_per_batch
-        self._exc = None
+        if chunk_size != self._chunk_size:
+            self._chunk_size = chunk_size
+        if chunks_per_batch != self._chunks_per_batch:
+            self._chunks_per_batch = chunks_per_batch
         self._lock = a_sync.CounterLock()
-        self._db_task = None
-        self._semaphore = semaphore
-        self._sleep_fut = None
-        self._sleep_time = sleep_time
-        self._task = None
-        self._verbose = verbose
+        if semaphore != self._semaphore:
+            self._semaphore = semaphore
+        if sleep_time != self._sleep_time:
+            self._sleep_time = sleep_time
+        if verbose != self._verbose:
+            self._verbose = verbose
         super().__init__(executor=executor, is_reusable=is_reusable)
 
     def __aiter__(self) -> AsyncIterator[T]:
         return self._objects_thru(block=None).__aiter__()
         
     def __del__(self) -> None:
         if self._task and not self._task.done():
```

### Comparing `ypricemagic-3.4.9/y/_db/config.py` & `ypricemagic-3.5.0/y/_db/config.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/decorators.py` & `ypricemagic-3.5.0/y/_db/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/entities.py` & `ypricemagic-3.5.0/y/_db/entities.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/exceptions.py` & `ypricemagic-3.5.0/y/_db/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/structs.py` & `ypricemagic-3.5.0/y/_db/structs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/utils/_ep.py` & `ypricemagic-3.5.0/y/_db/utils/_ep.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/utils/bulk.py` & `ypricemagic-3.5.0/y/_db/utils/bulk.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/utils/contract.py` & `ypricemagic-3.5.0/y/_db/utils/contract.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,25 +23,20 @@
         return deploy_block
     get_token = _get_get_token()
     if deploy_block := get_token(address, sync=True).deploy_block:
         logger.debug('%s deploy block from cache: %s', address, deploy_block.number)
         return deploy_block.number
     logger.debug('%s deploy block not cached, fetching from chain', address)
 
-def set_deploy_block(address: str, deploy_block: int) -> None:
-    a_sync.create_task(
-        coro=_set_deploy_block(address, deploy_block),
-        name=f"set_deploy_block {address}: {deploy_block}",
-        skip_gc_until_done=True,
-    )
-
 async def _set_deploy_block(address: str, deploy_block: int) -> None:
     await ensure_block(deploy_block)
     return await __set_deploy_block(address, deploy_block)
 
+set_deploy_block = a_sync.ProcessingQueue(_set_deploy_block, num_workers=10, return_data=False)
+
 @a_sync_write_db_session
 def __set_deploy_block(address: str, deploy_block: int) -> None:
     from y._db.utils._ep import _get_get_token
     get_token = _get_get_token()
     get_token(address, sync=True).deploy_block = (chain.id, deploy_block)
     logger.debug('deploy block cached for %s: %s', address, deploy_block)
```

### Comparing `ypricemagic-3.4.9/y/_db/utils/logs.py` & `ypricemagic-3.5.0/y/_db/utils/logs.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/_db/utils/price.py` & `ypricemagic-3.5.0/y/_db/utils/price.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,21 +27,14 @@
     if price := known_prices_at_block(block).pop(address, None):
         logger.debug("found %s block %s price %s in ydb", address, block, price)
         return price
     if (price := Price.get(token = (chain.id, address), block = (chain.id, block))) and (price:=price.price):
         logger.debug("found %s block %s price %s in ydb", address, block, price)
         return price
 
-def set_price(address: str, block: int, price: Decimal) -> None:
-    a_sync.create_task(
-        coro=_set_price(address, block, price), 
-        name=f"set_price {price} for {address} at {block}", 
-        skip_gc_until_done=True,
-    )
-
 @retry_locked
 async def _set_price(address: str, block: int, price: Decimal) -> None:
     await ensure_block(block, sync=False)
     if address == constants.EEE_ADDRESS:
         address = constants.WRAPPED_GAS_COIN
     await ensure_token(address, sync=False)
     with suppress(InvalidOperation): # happens with really big numbers sometimes. nbd, we can just skip the cache in this case.
@@ -50,12 +43,14 @@
             block = (chain.id, block),
             token = (chain.id, address),
             price = Decimal(price),
             sync = False,
         )
         logger.debug("inserted %s block %s price to ydb: %s", address, block, price)
 
+set_price = a_sync.ProcessingQueue(_set_price, num_workers=50, return_data=False)
+
 @cached(TTLCache(maxsize=1_000, ttl=5*60), lock=threading.Lock())
 @log_result_count("prices", ["block"])
 def known_prices_at_block(number: int) -> Dict[Address, Decimal]:
     """cache and return all known prices at block `number` to minimize db reads"""
     return dict(select((p.token.address, p.price) for p in Price if p.block.chain.id == chain.id and p.block.number == number))
```

### Comparing `ypricemagic-3.4.9/y/_db/utils/token.py` & `ypricemagic-3.5.0/y/_db/utils/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 from functools import lru_cache
 from typing import Dict, Optional, Set
 
 import a_sync
 from brownie import chain, convert
 from cachetools import TTLCache, cached
-from pony.orm import commit, select
+from pony.orm import commit, db_session, select
 
 from y import constants
 from y._db.decorators import a_sync_read_db_session, a_sync_write_db_session, log_result_count
 from y._db.entities import Address, Token, insert
 from y._db.exceptions import EEEError
 from y._db.utils._ep import _get_get_token
 from y.erc20 import decimals
@@ -32,14 +32,15 @@
         return insert(type=Token, chain=chain.id, address=address) or Token.get(chain=chain.id, address=address)
 
 @a_sync.a_sync(default='sync', ram_cache_maxsize=None)
 def ensure_token(address: str) -> None:
     return _ensure_token(address)
 
 @lru_cache(maxsize=None)
+@db_session
 def _ensure_token(address: str) -> None:
     """We can't wrap a `_Wrapped` object with `a_sync` so we have this helper fn"""
     if address not in known_tokens():
         get_token = _get_get_token()
         get_token(address, sync=True)
 
 @a_sync_read_db_session
@@ -49,29 +50,24 @@
     if (bucket := known_buckets().pop(address, None)) is None:
         get_token = _get_get_token()
         bucket = get_token(address, sync=True).bucket
     if bucket:
         logger.debug("found %s bucket %s in ydb", address, bucket)
     return bucket
 
-def set_bucket(address: str, bucket: str) -> None:
-    a_sync.create_task(
-        coro=_set_bucket(address, bucket),
-        name=f"set_bucket {address}: {bucket}",
-        skip_gc_until_done=True,
-    )
-
 @a_sync_write_db_session
 def _set_bucket(address: str, bucket: str) -> None:
     if address == constants.EEE_ADDRESS:
         return
     get_token = _get_get_token()
     get_token(address, sync=True).bucket = bucket
     logger.debug("updated %s bucket in ydb: %s", address, bucket)
 
+set_bucket = a_sync.ProcessingQueue(_set_bucket, num_workers=10, return_data=False)
+
 @a_sync_read_db_session
 def get_symbol(address: str) -> Optional[str]:
     if (symbol := known_symbols().pop(address, None)) is None:
         get_token = _get_get_token()
         symbol = get_token(address, sync=True).symbol
     if symbol:
         logger.debug("found %s symbol %s in ydb", address, symbol)
@@ -147,14 +143,15 @@
         logger.debug("found %s decimals %s in ydb", address, decimals)
         return decimals
 
 
 # startup caches
     
 @cached(TTLCache(maxsize=1, ttl=60*60), lock=threading.Lock())
+@db_session
 @log_result_count("tokens")
 def known_tokens() -> Set[str]:
     """cache and return all known Tokens for this chain to minimize db reads"""
     return set(select(t.address for t in Token if t.chain.id == chain.id))
 
 @cached(TTLCache(maxsize=1, ttl=60*60), lock=threading.Lock())
 @log_result_count("buckets")
```

### Comparing `ypricemagic-3.4.9/y/_db/utils/traces.py` & `ypricemagic-3.5.0/y/_db/utils/traces.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     def traces(self, to_block: Optional[int]) -> AsyncIterator[dict]:
         return self._objects_thru(block=to_block)
 
     async def _fetch_range(self, from_block: int, to_block: int) -> List[dict]:
         try:
             return await dank_mids.web3.provider.make_request("TraceFilter", {})
         except NotImplementedError:
-            results = {block: traces async for block, traces in a_sync.map(self._trace_block, range(from_block, to_block))}
+            results = {block: traces async for block, traces in a_sync.map(self._trace_block, range(from_block, to_block)).map()}
             return list(chain(*[results[i] for i in range(from_block, to_block)]))
         
     async def _trace_block(self, block: int) -> List[dict]:
         return [
             trace for trace in await dank_mids.web3.provider.make_request("TraceBlock", block)
             if (not self.from_addresses or any("from" in x and x["from"] in self.from_addresses for x in [trace, trace.values()]))
             and (not self.to_addresses or any("to" in x and x["to"] in self.to_addresses for x in [trace, trace.values()]))
```

### Comparing `ypricemagic-3.4.9/y/_db/utils/utils.py` & `ypricemagic-3.5.0/y/_db/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 
 import logging
-import threading
 from datetime import datetime, timezone
 from dateutil import parser
 from functools import lru_cache
 from typing import Dict, Optional, Set
 
 import a_sync
-from cachetools import TTLCache, cached
 from pony.orm import commit, select
 from brownie import chain
 
 from y._db.decorators import a_sync_read_db_session, a_sync_write_db_session, a_sync_write_db_session_cached, log_result_count
 from y._db.entities import Block, BlockAtTimestamp, Chain, insert
 
 logger = logging.getLogger(__name__)
@@ -49,66 +47,61 @@
     if ts:
         if isinstance(ts, str):
             # TODO: debug why this happens, but only sometimes
             ts = parser.parse(ts)
         unix = ts.timestamp()
         logger.debug("got Block[%s, %s].timestamp from cache: %s, %s", chain.id, number, unix, ts)
         return unix
-    
-def set_block_timestamp(block: int, timestamp: int) -> None:
-    a_sync.create_task(
-        coro=_set_block_timestamp(block, timestamp),
-        name=f"set_block_timestamp {block}: {timestamp}",
-        skip_gc_until_done=True,
-    )
 
 @a_sync_read_db_session
 def get_block_at_timestamp(timestamp: datetime) -> Optional[int]:
     if block := known_blocks_for_timestamps().pop(timestamp, None):
         logger.debug("found block %s for %s in ydb", block, timestamp)
         return block
     elif entity := BlockAtTimestamp.get(chainid=chain.id, timestamp=timestamp):
         block = entity.block
         logger.debug("found block %s for %s in ydb", block, timestamp)
         return block
-    
-def set_block_at_timestamp(timestamp: datetime, block: int) -> None:
-    a_sync.create_task(
-        coro=_set_block_at_timestamp(timestamp, block),
-        name=f"set_block_at_timestamp {timestamp}: {block}",
-        skip_gc_until_done=True,
-    )
 
 @a_sync_write_db_session
 def _set_block_timestamp(block: int, timestamp: int) -> None:
     from y._db.utils._ep import _get_get_block
     get_block = _get_get_block()
     block = get_block(block, sync=True)
     timestamp = datetime.fromtimestamp(timestamp, tz=timezone.utc)
     block.timestamp = timestamp
     logger.debug("cached %s.timestamp %s", block, timestamp)
 
+set_block_timestamp = a_sync.ProcessingQueue(_set_block_timestamp, num_workers=10, return_data=False)
+
 @a_sync_write_db_session
 def _set_block_at_timestamp(timestamp: datetime, block: int) -> None:
     insert(BlockAtTimestamp, chainid=chain.id, timestamp=timestamp, block=block)
     logger.debug("inserted block %s for %s", block, timestamp)
 
+set_block_at_timestamp = a_sync.ProcessingQueue(_set_block_at_timestamp, num_workers=10, return_data=False)
 
 # startup caches
-    
-@cached(TTLCache(maxsize=1, ttl=60*60), lock=threading.Lock())
+
+@lru_cache(maxsize=1)
 @log_result_count("blocks")
 def known_blocks() -> Set[int]:
     """cache and return all known blocks for this chain to minimize db reads"""
     return set(select(b.number for b in Block if b.chain.id == chain.id))
 
-@cached(TTLCache(maxsize=1, ttl=60*60), lock=threading.Lock())
+@lru_cache(maxsize=1)
 @log_result_count("block timestamps")
 def known_block_timestamps() -> Dict[int, datetime]:
     """cache and return all known block timestamps for this chain to minimize db reads"""
-    return dict(select((b.number, b.timestamp) for b in Block if b.chain.id == chain.id and b.timestamp))
+    query = select((b.number, b.timestamp) for b in Block if b.chain.id == chain.id and b.timestamp)
+    page_size = 100_000
+    timestamps = {}
+    for i in range((query.count() // page_size) + 1):
+        for block, timestamp in query.page(i+1, page_size):
+            timestamps[block] = timestamp
+    return timestamps
 
-@cached(TTLCache(maxsize=1, ttl=60*60), lock=threading.Lock())
+@lru_cache(maxsize=1)
 @log_result_count("blocks for timestamps")
 def known_blocks_for_timestamps() -> Dict[datetime, int]:
     """return all known blocks for timestamps for this chain to minimize db reads"""
     return dict(select((x.timestamp, x.block) for x in BlockAtTimestamp if x.chainid == chain.id))
```

### Comparing `ypricemagic-3.4.9/y/classes/common.py` & `ypricemagic-3.5.0/y/classes/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,24 +38,29 @@
     '''returns a string from a HexString'''
     h = h.hex().rstrip("0")
     if len(h) % 2 != 0:
         h += "0"
     return bytes.fromhex(h).decode("utf-8")
 
 class ContractBase(a_sync.ASyncGenericBase, metaclass=ChecksumASyncSingletonMeta):
-    __slots__ = "address", "asynchronous", "_deploy_block"
+    # defaults are stored as class vars to keep instance dicts smaller
+    asynchronous: bool = False
+    _deploy_block: Optional[int] = None
+    __slots__ = "address",
     def __init__(
         self, 
         address: AnyAddressType, 
         asynchronous: bool = False, 
         _deploy_block: Optional[int] = None,
     ) -> None:
         self.address = convert.to_address(address)
-        self.asynchronous = asynchronous
-        self._deploy_block = _deploy_block
+        if asynchronous:
+            self.asynchronous = asynchronous
+        if _deploy_block:
+            self._deploy_block = _deploy_block
         super().__init__()
     
     def __str__(self) -> str:
         return f'{self.address}'
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} '{self.address}'"
@@ -160,18 +165,15 @@
     async def _scale(self, block: Optional[Block] = None) -> int:
         return 10 ** await self._decimals(block, sync=False)
 
     async def total_supply(self, block: Optional[Block] = None) -> int:
         return await totalSupply(self.address, block=block, sync=False)
 
     async def total_supply_readable(self, block: Optional[Block] = None) -> float:
-        total_supply, scale = await asyncio.gather(
-            self.total_supply(block=block, sync=False),
-            self.__scale__
-        )
+        total_supply, scale = await asyncio.gather(self.total_supply(block=block, sync=False), self.__scale__)
         return total_supply / scale
     
     async def balance_of(self, address: AnyAddressType, block: Optional[Block] = None) -> int:
         return await raw_calls.balanceOf(self.address, address, block=block, sync=False)
     
     async def balance_of_readable(self, address: AnyAddressType, block: Optional[Block] = None) -> float:
         balance, scale = await asyncio.gather(self.balance_of(address, block=block, asynchronous=True), self.__scale__(asynchronous=True))
@@ -229,43 +231,61 @@
     __symbol__: HiddenMethodDescriptor[Self, str]
     __name__: HiddenMethodDescriptor[Self, str]
     __decimals__: HiddenMethodDescriptor[Self, int]
     __scale__: HiddenMethodDescriptor[Self, int]
 
 
 class WeiBalance(a_sync.ASyncGenericBase):
+    # defaults are stored as class vars to keep instance dicts smaller
+    block: Optional[Block] = None
+    asynchronous: bool = False
+    _skip_cache: bool = ENVS.SKIP_CACHE
+    _ignore_pools: Tuple[Pool, ...] = ()
     def __init__(
         self, 
         balance: int,
         token: AnyAddressType,
         block: Optional[Block] = None,
         skip_cache: bool = ENVS.SKIP_CACHE,
         ignore_pools: Tuple[Pool, ...] = (),
         asynchronous: bool = False,
         ) -> None:
 
-        self.asynchronous = asynchronous
+        if asynchronous != self.asynchronous:
+            self.asynchronous = asynchronous
         self.balance = Decimal(balance)
         self.token = ERC20(str(token), asynchronous=self.asynchronous)
-        self.block = block
+        if block != self.block:
+            self.block = block
         super().__init__()
-        self._skip_cache = skip_cache
-        self._ignore_pools = ignore_pools
+        if skip_cache != self._skip_cache:
+            self._skip_cache = skip_cache
+        if ignore_pools != self._ignore_pools:
+            self._ignore_pools = ignore_pools
 
     def __str__(self) -> str:
         return str(self.balance)
     
     def __repr__(self) -> str:
         return f"<WeiBalance token={self.token} balance={self.balance} block={self.block}>"
+    
+    def __hash__(self) -> int:
+        return hash((self.balance, self.token, self.block, self._skip_cache, self._ignore_pools))
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, int):
             return __o == self.balance
         elif isinstance(__o, WeiBalance):
-            return self.balance == __o.balance and self.token == __o.token
+            return (
+                self.balance == __o.balance and 
+                self.token == __o.token and 
+                self.block == __o.block and 
+                self._skip_cache == __o._skip_cache and
+                self._ignore_pools == __o._ignore_pools
+            )
         return False
     
     def __lt__(self, __o: object) -> bool:
         if isinstance(__o, int):
             return __o < self.balance
         elif isinstance(__o, WeiBalance):
             if self.token != __o.token:
@@ -286,23 +306,27 @@
             return 0
         scale = await self.token.__scale__
         readable = self.balance / scale
         self._logger.debug("balance: %s  decimals: %s  readable: %s", self.balance, str(scale).count("0"), readable)
         return readable
     __readable__: HiddenMethodDescriptor[Self, Decimal]
     
-    @a_sync.aka.cached_property
+    @a_sync.aka.property
+    async def price(self) -> Decimal:
+        price = Decimal(await self.token.price(block=self.block, skip_cache=self._skip_cache, ignore_pools=self._ignore_pools, sync=False))
+        self._logger.debug("balance: %s  price: %s", self, price)
+        return price
+    __price__: HiddenMethodDescriptor[Self, Decimal]
+    
+    @a_sync.aka.property
     async def value_usd(self) -> Decimal:
         if self.balance == 0:
             return 0
-        balance, price = await asyncio.gather(
-            self.__readable__,
-            self.token.price(block=self.block, skip_cache=self._skip_cache, ignore_pools=self._ignore_pools, sync=False),
-        )
-        value = balance * Decimal(price)
+        balance, price = await asyncio.gather(self.__readable__, self.__price__)
+        value = balance * price
         self._logger.debug("balance: %s  price: %s  value: %s", balance, price, value)
         return value
     __value_usd__: HiddenMethodDescriptor[Self, Decimal]
     
     @cached_property
     def _logger(self) -> logging.logging.Logger:
         return logging.get_price_logger(self.token.address, self.block, self.__class__.__name__)
```

### Comparing `ypricemagic-3.4.9/y/classes/singleton.py` & `ypricemagic-3.5.0/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/constants.py` & `ypricemagic-3.5.0/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/contracts.py` & `ypricemagic-3.5.0/y/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,17 @@
         - has_method
         - has_methods
         - has_methods_async
         - build_name
         - build_name_async
         - get_code
     """
+    # the default state for Contract objects
+    verified = True
+
     events: ContractEvents
     _ChecksumAddressSingletonMeta__instances: ChecksumAddressDict["Contract"]
 
     @eth_retry.auto_retry
     def __init__(
         self, 
         address: AnyAddressType, 
@@ -224,17 +227,15 @@
             raise ContractNotVerified(address)
 
         with _contract_lock:
             # autofetch-sources: false
             # Try to fetch the contract from the local sqlite db.
             try:
                 super().__init__(address, owner=owner)
-                try:
-                    self.verified = True
-                except AttributeError:
+                if not isinstance(self.verified, bool) and self.verified is not None:
                     logger.warning(f'`Contract("{address}").verified` property will not be usable due to the contract having a `verified` method in its ABI.')
             except AssertionError as e:
                 raise CompilerError("y.Contract objects work best when we bypass compilers. In this case, it will *only* work when we bypass. Please ensure autofetch_sources=False in your brownie-config.yaml and rerun your script.") from e
             except IndexError as e:
                 if str(e) == "pop from an empty deque":
                     raise CompilerError("y.Contract objects work best when we bypass compilers. In this case, it will *only* work when we bypass. Please ensure autofetch_sources=False in your brownie-config.yaml and rerun your script.") from e
                 raise e
@@ -291,32 +292,42 @@
         _setup_events(self)             # Init an event container for each topic
         _squeeze(self)                  # Get rid of unnecessary memory-hog properties
         try:
             self._ttl_cache_popper = "disabled" if cache_ttl is None else asyncio.get_running_loop().call_later(cache_ttl, _pop, cls._ChecksumAddressSingletonMeta__instances, self.address)
         except RuntimeError:
             self._ttl_cache_popper = cache_ttl
         return self
-    
+
     @classmethod
-    @stuck_coro_debugger
     async def coroutine(
         cls, 
         address: AnyAddressType, 
         require_success: bool = True, 
         cache_ttl: Optional[int] = ENVS.CONTRACT_CACHE_TTL,  # units: seconds
     ) -> Self:
         
+        address = str(address)
         # We do this so we don't clog the threadpool with multiple jobs for the same contract.
-        async with address_semaphores[address]:
-            try:
-                contract = cls._ChecksumAddressSingletonMeta__instances[address]
-            except KeyError:
-                if str(address).lower() in ["0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee", ZERO_ADDRESS]:
-                    raise ContractNotFound(f"{address} is not a contract.") from None
-                contract = await contract_threads.run(cls, address, require_success=require_success)
+        try:
+            contract = cls._ChecksumAddressSingletonMeta__instances[address]
+        except KeyError:
+            if address.lower() in ["0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee", ZERO_ADDRESS]:
+                raise ContractNotFound(f"{address} is not a contract.") from None
+            contract = await _contract_queue(address, require_success=require_success, cache_ttl=cache_ttl)
+        return contract
+    
+    @classmethod
+    @stuck_coro_debugger
+    async def _coroutine(
+        cls, 
+        address: AnyAddressType, 
+        require_success: bool = True, 
+        cache_ttl: Optional[int] = ENVS.CONTRACT_CACHE_TTL,  # units: seconds
+    ) -> Self:
+        contract = await contract_threads.run(cls, address, require_success=require_success)
 
         if not contract.verified or contract._ttl_cache_popper == "disabled":
             pass
     
         elif cache_ttl is None:
             if isinstance(contract._ttl_cache_popper, asyncio.TimerHandle):
                 contract._ttl_cache_popper.cancel()
@@ -326,15 +337,15 @@
             cache_ttl = max(contract._ttl_cache_popper, cache_ttl)
             contract._ttl_cache_popper = asyncio.get_running_loop().call_later(cache_ttl, _pop, cls._ChecksumAddressSingletonMeta__instances, contract.address)
 
         elif asyncio.get_running_loop().time() + cache_ttl > contract._ttl_cache_popper.when():
             contract._ttl_cache_popper.cancel()
             contract._ttl_cache_popper = asyncio.get_running_loop().call_later(cache_ttl, _pop, cls._ChecksumAddressSingletonMeta__instances, contract.address)
         return contract
-    
+
     def __init_from_abi__(self, build: Dict, owner: Optional[AccountsType] = None, persist: bool = True) -> None:
         _ContractBase.__init__(self, None, build, {})  # type: ignore
         _DeployedContractBase.__init__(self, build['address'], owner, None)
         if persist:
             _add_deployment(self)
         try:
             self.verified = True
@@ -354,14 +365,15 @@
 
     async def build_name(self, return_None_on_failure: bool = False) -> Optional[str]:
         return await build_name(self.address, return_None_on_failure=return_None_on_failure, sync=False)
     
     async def get_code(self, block: Optional[Block] = None) -> HexBytes:
         return await get_code(self.address, block=block)
 
+_contract_queue = a_sync.SmartProcessingQueue(Contract._coroutine, num_workers=32)
 
 @memory.cache()
 #yLazyLogger(logger)
 def is_contract(address: AnyAddressType) -> bool:
     '''
     Checks to see if the input address is a contract. Returns `True` if:
     - The address is not and has never been a contract
@@ -382,15 +394,15 @@
         return False if response is None else response if return_response else True
     except Exception as e:
         if isinstance(e, ContractLogicError) or call_reverted(e):
             return False
         raise
 
 @stuck_coro_debugger
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=15*60)
 async def has_methods(
     address: AnyAddressType, 
     methods: Tuple[str],
     _func: Callable = all # Union[any, all]
 ) -> bool:
     '''
     Checks to see if a contract has each view method (with no inputs) in `methods`.
@@ -478,15 +490,15 @@
                 raise ContractNotFound(str(e)) from e
             raise ContractNotVerified(str(e)) from e
         else:
             raise
 
     is_verified = bool(data.get("SourceCode"))
     if not is_verified:
-        raise ContractNotVerified(f"Contract source code not verified: {address}")
+        raise ContractNotVerified(f"Contract source code not verified: {address}") from None
     name = data["ContractName"]
     abi = json.loads(data["ABI"])
     implementation = data.get("Implementation")
     return name, abi, implementation
 
 def _resolve_proxy(address) -> Tuple[str, List]:
     address = convert.to_address(address)
```

### Comparing `ypricemagic-3.4.9/y/datatypes.py` & `ypricemagic-3.5.0/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/decorators.py` & `ypricemagic-3.5.0/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/erc20.py` & `ypricemagic-3.5.0/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/exceptions.py` & `ypricemagic-3.5.0/y/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from brownie import Contract as BrownieContract
 from brownie.exceptions import CompilerError
 
+if TYPE_CHECKING:
+    from y.prices.dex.uniswap.v2 import UniswapV2Pool
+
 logger = logging.getLogger(__name__)
 
 # General
 
 class yPriceMagicError(ValueError):
     def __init__(self, exc: Exception, address: str, block: Optional[int], symbol: str):
         from y import Network
@@ -64,25 +67,31 @@
     ]
     return any(trigger in str(e) for trigger in triggers)
 
 
 # Pool detection
 
 class NotAUniswapV2Pool(Exception):
-    pass
+    # NOTE: we use this exc to get the non-pool out of the pool singleton so it doesn't grow forever
+    # TODO: Refactor this goofy thing out
+    def __init__(self, non_pool: "UniswapV2Pool"):
+        from y.prices.dex.uniswap.v2 import UniswapV2Pool
+        UniswapV2Pool._ChecksumASyncSingletonMeta__instances[True].pop(non_pool.address, None)
+        UniswapV2Pool._ChecksumASyncSingletonMeta__instances[False].pop(non_pool.address, None)
+        super().__init__(non_pool.address)
 
 class NotABalancerV2Pool(Exception):
     pass
 
 # Uni
 
 class CantFindSwapPath(Exception):
     pass
 
-class TokenNotFound(Exception):
+class TokenNotFound(ValueError):
     def __init__(self, token, container):
         super().__init__(f"{token} is not in {container}")
 
 # Calls
 
 class CalldataPreparationError(Exception):
     pass
```

### Comparing `ypricemagic-3.4.9/y/interfaces/ERC20.py` & `ypricemagic-3.5.0/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-3.5.0/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/compound/unitroller.py` & `ypricemagic-3.5.0/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-3.5.0/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/multicall2.py` & `ypricemagic-3.5.0/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-3.5.0/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-3.5.0/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/interfaces/uniswap/velov2.py` & `ypricemagic-3.5.0/y/interfaces/uniswap/velov2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/networks.py` & `ypricemagic-3.5.0/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/band.py` & `ypricemagic-3.5.0/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/chainlink.py` & `ypricemagic-3.5.0/y/prices/chainlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y import convert
 from y.classes.common import ERC20
 from y.contracts import Contract, contract_creation_block_async
 from y.datatypes import Address, AnyAddressType, Block, UsdPrice
 from y.exceptions import UnsupportedNetwork
 from y.networks import Network
+from y.utils.cache import a_sync_ttl_cache
 from y.utils.events import ProcessedEvents
 
 logger = logging.getLogger(__name__)
 
 DENOMINATIONS = {
     'ETH': '0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE',
     'BTC': '0xbBbBBBBbbBBBbbbBbbBbbbbBBbBbbbbBbBbbBBbB',
@@ -245,15 +246,15 @@
         for feed in self._feeds:
             yield feed
         if self._feeds_from_events is None:
             return
         async for feed in self._feeds_from_events.objects(to_block=block):
             yield feed
 
-    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=600)
+    @a_sync_ttl_cache
     async def get_feed(self, asset: Address) -> Optional[Feed]:
         asset = convert.to_address(asset)
         async for feed in self._feeds_thru_block(await dank_mids.eth.block_number):
             if asset == feed.asset:
                 return feed
     
     async def has_feed(self, asset: AnyAddressType) -> bool:
```

### Comparing `ypricemagic-3.4.9/y/prices/convex.py` & `ypricemagic-3.5.0/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/dex/balancer/balancer.py` & `ypricemagic-3.5.0/y/prices/dex/balancer/balancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     async def get_pool_price(self, token_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
         versions: List[Union[BalancerV1, BalancerV2]] = await self.versions
         for v in versions:
             if await v.is_pool(token_address, sync=False):
                 return UsdPrice(await v.get_pool_price(token_address, block, skip_cache=skip_cache, sync=False))
             
     @stuck_coro_debugger
-    @a_sync.a_sync(cache_type='memory')
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_price(self, token_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
         if await self.is_balancer_pool(token_address, sync=False):
             return await self.get_pool_price(token_address, block=block, skip_cache=skip_cache, sync=False)
 
         price = None
         
         if ( # NOTE: Only query v2 if block queried > v2 deploy block plus some extra blocks to build up liquidity
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/balancer/v1.py` & `ypricemagic-3.5.0/y/prices/dex/balancer/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import logging
 from decimal import Decimal
 from typing import Dict, List, Optional, Tuple
 
 import a_sync
+from a_sync.property import HiddenMethodDescriptor
 from brownie import chain
 from brownie.convert.datatypes import EthAddress
 from brownie.exceptions import VirtualMachineError
+from typing_extensions import Self
 
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y.classes.common import ERC20
 from y.constants import dai, usdc, wbtc, weth
 from y.contracts import Contract, contract_creation_block_async, has_methods
 from y.datatypes import (Address, AddressOrContract, AnyAddressType, Block,
                          Pool, UsdPrice, UsdValue)
@@ -25,49 +27,48 @@
 logger = logging.getLogger(__name__)
 
 async def _calc_out_value(token_out: AddressOrContract, total_outout: int, scale: float, block: int, skip_cache: bool = ENVS.SKIP_CACHE) -> float:
     out_scale, out_price = await asyncio.gather(ERC20(token_out, asynchronous=True).scale, magic.get_price(token_out, block, skip_cache=skip_cache, sync=False))
     return (total_outout / out_scale) * float(out_price) / scale
 
 class BalancerV1Pool(ERC20):
-    async def tokens(self, block: Optional[Block] = None) -> List[ERC20]:
+    @a_sync.aka.cached_property
+    async def tokens(self) -> List[ERC20]:
         contract = await Contract.coroutine(self.address)
-        tokens = await contract.getCurrentTokens.coroutine(block_identifier=block)
-        return [ERC20(token, asynchronous=self.asynchronous) for token in tokens]
+        return [ERC20(token, asynchronous=self.asynchronous) for token in await contract.getFinalTokens]
+    __tokens__: HiddenMethodDescriptor[Self, List[ERC20]]
     
     @stuck_coro_debugger
     async def get_pool_price(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
         supply = await self.total_supply_readable(block=block, sync=False)
-        if supply == 0:
-            return 0
+        if not supply:
+            return None
         return UsdPrice(await self.get_tvl(block=block, skip_cache=skip_cache, sync=False) / Decimal(supply))
 
     @stuck_coro_debugger
     async def get_tvl(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdValue]:
         token_balances = await self.get_balances(block=block, sync=False)
         good_balances = {
             token: balance
             for token, balance
             in token_balances.items()
             if await token.price(block=block, return_None_on_failure=True, skip_cache=skip_cache, sync=False) is not None
         }
         
-        prices = await asyncio.gather(*[token.price(block=block, return_None_on_failure = True, sync=False) for token in good_balances])
+        prices = await ERC20.price.map(good_balances, block=block, return_None_on_failure=True, skip_cache=skip_cache).values()
 
         # in case we couldn't get prices for all tokens, we can extrapolate from the prices we did get
         good_value = sum(balance * Decimal(price) for balance, price in zip(good_balances.values(),prices))
         if len(good_balances):
             return good_value / len(good_balances) * len(token_balances)
         return None
     
     @stuck_coro_debugger
     async def get_balances(self, block: Optional[Block] = None) -> Dict[ERC20, Decimal]:
-        tokens = await self.tokens(block=block, sync=False)
-        balances = await asyncio.gather(*[self.get_balance(token, block or 'latest', sync=False) for token in tokens])
-        return dict(zip(tokens, balances))
+        return await a_sync.map(self.get_balance, self.__tokens__, block=block or 'latest')
 
     @stuck_coro_debugger
     async def get_balance(self, token: AnyAddressType, block: Block) -> Decimal:
         balance, scale = await asyncio.gather(
             self.check_liquidity(str(token), block, sync=False),
             ERC20(token, asynchronous=True).scale,
         )
@@ -89,29 +90,29 @@
     
     def __str__(self) -> str:
         return "BalancerV1()"
     
     def __repr__(self) -> str:
         return "<BalancerV1>"
     
+    @a_sync.a_sync(ram_cache_ttl=5*60)
     @stuck_coro_debugger
     async def is_pool(self, token_address: AnyAddressType) -> bool:
-        return await has_methods(token_address ,("getCurrentTokens()(address[])", "getTotalDenormalizedWeight()(uint)", "totalSupply()(uint)"), sync=False)
+        return await has_methods(token_address, ("getCurrentTokens()(address[])", "getTotalDenormalizedWeight()(uint)", "totalSupply()(uint)"), sync=False)
 
     @stuck_coro_debugger
-    async def get_pool_price(self, token_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
-        assert await self.is_pool(token_address, sync=False)
+    async def get_pool_price(self, token_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
         return await BalancerV1Pool(token_address, asynchronous=True).get_pool_price(block=block, skip_cache=skip_cache)
     
     @stuck_coro_debugger
     async def get_token_price(self, token_address: AddressOrContract, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
         if block is not None and block < await contract_creation_block_async(self.exchange_proxy, True):
             return None
         scale = 1.0
-        out, totalOutput = await self.get_some_output(token_address, block=block, sync=False)
+        out, totalOutput = await self.get_some_output(token_address, block=block, scale=scale, sync=False)
         if out:
             return await _calc_out_value(out, totalOutput, scale, block=block, skip_cache=skip_cache)
         # Can we get an output if we try smaller size?
         scale = 0.5
         out, totalOutput = await self.get_some_output(token_address, block=block, scale=scale, sync=False) 
         if out:
             return await _calc_out_value(out, totalOutput, scale, block=block, skip_cache=skip_cache)
@@ -149,27 +150,27 @@
         self,
         token_in: AddressOrContract,
         scale: int = 1,
         block: Optional[Block] = None
         ) -> Tuple[EthAddress,int]:
 
         try:
-            out, totalOutput = await self.check_liquidity_against(token_in, weth, block=block, sync=False)
+            out, totalOutput = await self.check_liquidity_against(token_in, weth, block=block, scale=scale, sync=False)
         except (ValueError, VirtualMachineError):
             try:
-                out, totalOutput = await self.check_liquidity_against(token_in, dai, block=block, sync=False)
+                out, totalOutput = await self.check_liquidity_against(token_in, dai, block=block, scale=scale, sync=False)
             except (ValueError, VirtualMachineError):
                 try:
-                    out, totalOutput = await self.check_liquidity_against(token_in, usdc, block=block, sync=False)
+                    out, totalOutput = await self.check_liquidity_against(token_in, usdc, block=block, scale=scale, sync=False)
                 except (ValueError, VirtualMachineError):
                     try:
-                        out, totalOutput = await self.check_liquidity_against(token_in, wbtc, block=block, sync=False)
+                        out, totalOutput = await self.check_liquidity_against(token_in, wbtc, block=block, scale=scale, sync=False)
                     except (ValueError, VirtualMachineError):
                         out = None
                         totalOutput = None
         return out, totalOutput
 
     @stuck_coro_debugger
     async def check_liquidity(self, token: Address, block: Block, ignore_pools: Tuple[Pool, ...] = ()) -> int:
         pools = []
         pools = [pool for pool in pools if pool not in ignore_pools]
-        return max(await asyncio.gather(*[pool.check_liquidity(token, block, sync=False) for pool in pools])) if pools else 0
+        return await BalancerV1Pool.check_liquidity.max(pools, token=token, block=block, sync=False) if pools else 0
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/balancer/v2.py` & `ypricemagic-3.5.0/y/prices/dex/balancer/v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 import asyncio
 import logging
 from collections import defaultdict
-from typing import (AsyncIterator, Awaitable, Dict, List, NewType, Optional,
-                    Tuple)
+from typing import AsyncIterator, Dict, List, NewType, Optional, Tuple
 
 import a_sync
 from a_sync.property import HiddenMethodDescriptor
 from brownie import ZERO_ADDRESS, chain
 from brownie.convert.datatypes import EthAddress
 from brownie.network.contract import ContractCall, ContractTx, OverloadedMethod
 from brownie.network.event import _EventItem
@@ -19,15 +18,15 @@
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y import constants, contracts
 from y.classes.common import ERC20, ContractBase, WeiBalance
 from y.contracts import Contract
 from y.datatypes import Address, AnyAddressType, Block, UsdPrice, UsdValue
 from y.decorators import stuck_coro_debugger
 from y.networks import Network
-from y.utils.cache import a_sync_cache
+from y.utils.cache import a_sync_ttl_cache
 from y.utils.events import ProcessedEvents
 from y.utils.logging import get_price_logger
 from y.utils.raw_calls import raw_call
 
 # TODO: Cache pool tokens for pools that can't change
 
 BALANCER_V2_VAULTS = {
@@ -58,40 +57,38 @@
     def __init__(self, address: AnyAddressType, asynchronous: bool = False) -> None:
         super().__init__(address, asynchronous=asynchronous)
         self._events = BalancerEvents(addresses=address, topics=['0x3c13bc30b8e878c53fd2a36b679409c073afd75950be43d8858768e956fbc20e'])
         if not self._is_cached:
             # we need the contract cached so we can decode logs correctly
             self.contract
     
-    @a_sync_cache
     @stuck_coro_debugger
-    async def list_pools(self, block: Optional[Block] = None) -> List["BalancerV2Pool"]:
-        return [pool async for pool in self._events.events(to_block=block)]
+    async def pools(self, block: Optional[Block] = None) -> AsyncIterator["BalancerV2Pool"]:
+        async for pool in self._events.events(to_block=block):
+            yield pool
 
+    @stuck_coro_debugger
     async def pools_for_token(self, token: Address, block: Optional[Block] = None) -> AsyncIterator["BalancerV2Pool"]:
-        async for pool, info in a_sync.map(lambda pool: pool.tokens(block=block, sync=False), self._events.events(to_block=block)):
+        async for pool, info in BalancerV2Pool.tokens.map(block=block).map(self.pools(block=block), pop=True):
             if token in info:
                 yield pool
                 
-    @a_sync_cache
+    @a_sync_ttl_cache
     @stuck_coro_debugger
     async def get_pool_tokens(self, pool_id: HexBytes, block: Optional[Block] = None):
         contract = await contracts.Contract.coroutine(self.address)
         return await contract.getPoolTokens.coroutine(pool_id, block_identifier = block)
     
-    @a_sync_cache
+    @a_sync_ttl_cache
     @stuck_coro_debugger
     async def get_pool_info(self, poolids: Tuple[HexBytes,...], block: Optional[Block] = None) -> List[Tuple]:
         contract = await contracts.Contract.coroutine(self.address)
-        return await asyncio.gather(*[
-            contract.getPoolTokens.coroutine(poolId, block_identifier=block)
-            for poolId in poolids
-        ])
+        return await contract.getPoolTokens.map(poolids, block_identifier=block)
     
-    @a_sync_cache
+    @a_sync_ttl_cache
     @stuck_coro_debugger
     async def deepest_pool_for(self, token_address: Address, block: Optional[Block] = None) -> Tuple[Optional["BalancerV2Pool"], int]:
         logger = get_price_logger(token_address, block, 'balancer.v2')
         deepest_pool, deepest_balance = None, 0
         async for pool in self.pools_for_token(token_address, block=block):
             info: Dict[ERC20, WeiBalance]
             if info := await pool.get_balances(block=block, sync=False):
@@ -119,78 +116,91 @@
 MESSED_UP_POOLS = {
     Network.Mainnet: [
         "0xF3799CBAe9c028c1A590F4463dFF039b8F4986BE",
     ],
 }.get(chain.id, [])
 
 class BalancerV2Pool(ERC20):
-    __slots__ = "_id", "_messed_up"
-    def __init__(self, address: AnyAddressType, *args, id: Optional[HexBytes] = None, **kwargs):
-        super().__init__(address, *args, **kwargs)
+    # defaults are stored as class vars to keep instance dicts smaller
+    _messed_up = False
+    # internal variables to save calls in some instances
+    # they do not necessarily reflect real life at all times
+    __nonweighted: bool = False
+    __weights: List[int] = None
+    __slots__ = "_id", 
+    def __init__(
+        self, 
+        address: AnyAddressType, 
+        id: Optional[HexBytes] = None, 
+        asynchronous: bool = False, 
+        _deploy_block: Optional[Block] = None,
+    ):
+        super().__init__(address, asynchronous=asynchronous, _deploy_block=_deploy_block)
         self._id = id
-        self._messed_up = self.address in MESSED_UP_POOLS
+        if self.address in MESSED_UP_POOLS:
+            self._messed_up = True
 
-    @a_sync.aka.property
+    @a_sync.aka.cached_property
     async def id(self) -> PoolId:
         if self._id is None:
-            self._id = a_sync.create_task(Call(self.address, ['getPoolId()(bytes32)']), name=f"pool.id for {self}")
-        if hasattr(self._id, "__await__"):
-            self._id = PoolId(await self._id)
+            self._id = await Call(self.address, ['getPoolId()(bytes32)'])
         return self._id
     __id__: HiddenMethodDescriptor[Self, PoolId]
     
     @a_sync.aka.cached_property
     async def vault(self) -> Optional[BalancerV2Vault]:
         vault = await raw_call(self.address, 'getVault()', output='address', sync=False)
         return None if vault == ZERO_ADDRESS else BalancerV2Vault(vault, asynchronous=True)
     __vault__: HiddenMethodDescriptor[Self, Optional[BalancerV2Vault]]
     
     @stuck_coro_debugger
-    async def get_pool_price(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Awaitable[UsdPrice]:
+    async def get_pool_price(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
         tvl, total_supply = await asyncio.gather(
             self.get_tvl(block=block, skip_cache=skip_cache, sync=False),
             self.total_supply_readable(block=block, sync=False),
         )
         return UsdPrice(tvl / total_supply)
         
     @stuck_coro_debugger
-    async def get_tvl(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[Awaitable[UsdValue]]:
-        balances: Dict[ERC20, WeiBalance] = await self.get_balances(block=block, skip_cache=skip_cache, sync=False)
-        if balances:
-            return UsdValue(sum(await asyncio.gather(*[
-                balance.__value_usd__ for balance in balances.values()
-                if balance.token.address != self.address  # NOTE: to prevent an infinite loop for tokens that include themselves in the pool (e.g. bb-a-USDC)
-            ])))
+    async def get_tvl(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdValue]:
+        balances: Dict[ERC20, WeiBalance]
+        if balances := await self.get_balances(block=block, skip_cache=skip_cache, sync=False):
+            return UsdValue(await WeiBalance.value_usd.sum((balance for balance in balances.values() if balance.token.address != self.address), sync=False))
 
-    @a_sync_cache
+    @a_sync_ttl_cache
     @stuck_coro_debugger
     async def get_balances(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Dict[ERC20, WeiBalance]:
         if self._messed_up:
             return {}
         try:
             vault, id = await asyncio.gather(self.__vault__, self.__id__)
         except ContractLogicError:
             if await self.__build_name__ != "CronV1Pool":
                 logger.error("%s is messed up", self)
             return {}
         if vault is None:
             return {}
         tokens, balances, lastChangedBlock = await vault.get_pool_tokens(id, block=block, sync=False)
-        return {ERC20(token, asynchronous=self.asynchronous): WeiBalance(balance, token, block=block, skip_cache=skip_cache) for token, balance in zip(tokens, balances)}
+        return {
+            ERC20(token, asynchronous=self.asynchronous): WeiBalance(balance, token, block=block, skip_cache=skip_cache)
+            for token, balance in zip(tokens, balances)
+        }
 
     @stuck_coro_debugger
     async def get_token_price(self, token_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
-        token_balances, weights = await asyncio.gather(
-            self.get_balances(block=block, skip_cache=skip_cache, sync=False),
-            self.weights(block=block, sync=False),
-        )
-        pool_token_info = list(zip(token_balances.keys(),token_balances.values(), weights))
-        for pool_token, balance, weight in pool_token_info:
+        get_balances_coro = self.get_balances(block=block, skip_cache=skip_cache, sync=False)
+        if self.__nonweighted:
+            token_balances = await get_balances_coro
+            weights = self.__weights
+        else:
+            token_balances, weights = await asyncio.gather(get_balances_coro, self.weights(block=block, sync=False))
+        pool_token_info = list(zip(token_balances.keys(), token_balances.values(), weights))
+        for pool_token, token_balance, token_weight in pool_token_info:
             if pool_token == token_address:
-                token_balance, token_weight = balance, weight
+                break
 
         paired_token_balance: Optional[WeiBalance] = None
         for pool_token, balance, weight in pool_token_info:
             if pool_token in constants.STABLECOINS:
                 paired_token_balance, paired_token_weight = balance, weight
                 break
             elif pool_token == constants.WRAPPED_GAS_COIN:
@@ -199,40 +209,43 @@
             elif len(pool_token_info) == 2 and pool_token != token_address:
                 paired_token_balance, paired_token_weight = balance, weight
                 break
         
         if paired_token_balance is None:
             return None
 
-        token_value_in_pool, token_balance_readable = await asyncio.gather(*[paired_token_balance.__value_usd__, token_balance.__readable__])
+        token_value_in_pool, token_balance_readable = await asyncio.gather(paired_token_balance.__value_usd__, token_balance.__readable__)
         token_value_in_pool /= paired_token_weight * token_weight
         return UsdPrice(token_value_in_pool / token_balance_readable) 
 
     # NOTE: We can't cache this as a cached property because some balancer pool tokens can change. Womp
-    @a_sync_cache
+    @a_sync_ttl_cache
     async def tokens(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Tuple[ERC20]:
         tokens = tuple((await self.get_balances(block=block, skip_cache=skip_cache, sync=False)).keys())
         tokens_history = _tasks_to_help_me_find_pool_types_that_cant_change_tokens[self]
         tokens_history[tokens] += 1
         if len(tokens_history) == 1 and tokens_history[tokens] > 100:
             contract = await contracts.Contract.coroutine(self.address, require_success=False)
             if contract.verified:
                 methods = [k for k, v in contract.__dict__.items() if isinstance(v, (ContractCall, ContractTx, OverloadedMethod))]
                 logger.debug(
                     "%s has 100 blocks with unchanging list of tokens, contract methods are %s", self, methods)
         return tokens
 
-    @a_sync_cache
+    @a_sync_ttl_cache
     @stuck_coro_debugger
     async def weights(self, block: Optional[Block] = None) -> List[int]:
         contract = await Contract.coroutine(self.address)
         try:
             return await contract.getNormalizedWeights.coroutine(block_identifier = block)
-        except (AttributeError,ValueError):
-            return len(await self.tokens(block=block, sync=False))
+        except AttributeError:
+            # Contract has no method `getNormalizedWeights`
+            self.__nonweighted = True
+            num_tokens = len(await self.tokens(block=block, sync=False))
+            self.__weights = [10 ** 18 // num_tokens] * num_tokens
 
 class ImmutableTokensBalancerV2Pool(BalancerV2Pool):
     async def tokens(self, _: Optional[Block] = None) -> List[ERC20]:
         return await self.__tokens
     @a_sync.aka.cached_property
     async def __tokens(self) -> List[ERC20]:
         return await super().tokens()
@@ -255,35 +268,33 @@
     def __init__(self, asynchronous: bool = False) -> None:
         self.asynchronous = asynchronous
         self.vaults = [BalancerV2Vault(vault, asynchronous=self.asynchronous) for vault in BALANCER_V2_VAULTS]
     
     def __str__(self) -> str:
         return "BalancerV2()"
 
+    @a_sync.a_sync(ram_cache_ttl=5*60)
     @stuck_coro_debugger
     async def is_pool(self, token_address: AnyAddressType) -> bool:
         methods = ('getPoolId()(bytes32)','getPausedState()((bool,uint,uint))','getSwapFeePercentage()(uint)')
         return await contracts.has_methods(token_address, methods, sync=False)
     
     @stuck_coro_debugger
     async def get_pool_price(self, pool_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
         return await BalancerV2Pool(pool_address, asynchronous=True).get_pool_price(block=block, skip_cache=skip_cache)
 
     @stuck_coro_debugger
     async def get_token_price(self, token_address: Address, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
-        deepest_pool: Optional[BalancerV2Pool] = await self.deepest_pool_for(token_address, block=block, sync=False)
-        if deepest_pool is None:
-            return
-        return await deepest_pool.get_token_price(token_address, block, skip_cache=skip_cache, sync=False)
+        deepest_pool: Optional[BalancerV2Pool]
+        if deepest_pool := await self.deepest_pool_for(token_address, block=block, sync=False):
+            return await deepest_pool.get_token_price(token_address, block, skip_cache=skip_cache, sync=False)
     
     @stuck_coro_debugger
     async def deepest_pool_for(self, token_address: Address, block: Optional[Block] = None) -> Optional[BalancerV2Pool]:
-        deepest_pools = await asyncio.gather(*[vault.deepest_pool_for(token_address, block=block, sync=False) for vault in self.vaults])
-        deepest_pools = {vault.address: deepest_pool for vault, deepest_pool in zip(self.vaults, deepest_pools) if deepest_pool is not None}
-        if not deepest_pools:
-            return None
-        deepest_pool_balance = max(deepest_pools.values())
-        for pool_address, pool_balance in deepest_pools.values():
-            if pool_balance == deepest_pool_balance and pool_address:
-                return BalancerV2Pool(pool_address, asynchronous=self.asynchronous)
+        deepest_pools = BalancerV2Vault.deepest_pool_for.map(self.vaults, token_address=token_address, block=block)
+        if deepest_pools := {vault.address: deepest_pool async for vault, deepest_pool in deepest_pools if deepest_pool is not None}:
+            deepest_pool_balance = max(dp[1] for dp in deepest_pools.values())
+            for pool_address, pool_balance in deepest_pools.values():
+                if pool_balance == deepest_pool_balance and pool_address:
+                    return BalancerV2Pool(pool_address, asynchronous=self.asynchronous)
 
 balancer = BalancerV2(asynchronous=True)
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/genericamm.py` & `ypricemagic-3.5.0/y/prices/dex/genericamm.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     async def get_tokens(self, lp_token_address: AnyAddressType) -> Tuple[ERC20,ERC20]:
         tokens = await gather_methods(lp_token_address, _TOKEN_METHODS)
         return tuple(ERC20(token, asynchronous=self.asynchronous) for token in tokens)
     
     @stuck_coro_debugger
     async def get_tvl(self, lp_token_address: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdValue:
         lp_token_contract = await Contract.coroutine(lp_token_address)
-        tokens = await self.get_tokens(lp_token_address, sync=False)
-        reserves = await lp_token_contract.getReserves.coroutine(block_identifier=block)
-        reserves = [WeiBalance(reserve, token, block=block, skip_cache=skip_cache) for token, reserve in zip(tokens,reserves)]
-        return UsdValue(sum(await asyncio.gather(*[reserve.__value_usd__ for reserve in reserves])))
+        tokens, reserves = await asyncio.gather(
+            self.get_tokens(lp_token_address, sync=False),
+            lp_token_contract.getReserves.coroutine(block_identifier=block),
+        )
+        reserves = (WeiBalance(reserve, token, block=block, skip_cache=skip_cache) for token, reserve in zip(tokens,reserves))
+        return UsdValue(await WeiBalance.value_usd.sum(reserves, sync=False))
 
 
 generic_amm = GenericAmm(asynchronous=True)
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/mooniswap.py` & `ypricemagic-3.5.0/y/prices/dex/mooniswap.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 elif chain.id == 56:
     router = Contract("0xD41B24bbA51fAc0E4827b6F94C0D6DDeB183cD64")
     gas_coin = Contract("0xbb4CdB9CBd36B01bD1cBaEBF2De08d9173bc095c") #wbnb
 else: 
     router = None
     gas_coin = None
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', ram_cache_ttl=5*60)
 async def is_mooniswap_pool(token: AnyAddressType) -> bool:
     address = convert.to_address(token)
     return False if router is None else await router.isPool.coroutine(address)
 
 @a_sync.a_sync(default='sync')
 async def get_pool_price(token: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
     address = convert.to_address(token)
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/solidly.py` & `ypricemagic-3.5.0/y/prices/dex/solidly.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 from typing import List, Optional, Tuple
 
 from y.datatypes import Address, Block
 from y.decorators import continue_on_revert, stuck_coro_debugger
 from y.exceptions import call_reverted
 from y.prices.dex.uniswap.v2 import Path, UniswapRouterV2, UniswapV2Pool
-from y.utils.cache import a_sync_cache
+from y.utils.cache import a_sync_ttl_cache
 
 
 class SolidlyRouterBase(UniswapRouterV2):
     """
     Solidly is a modified fork of Uni V2.
     The `uniswap_multiplexer` is the entrypoint for pricing using this object.
     """
@@ -35,20 +35,20 @@
 
 class SolidlyPool(UniswapV2Pool):
     pass
 
 class SolidlyRouter(SolidlyRouterBase):
 
     @stuck_coro_debugger
-    @a_sync_cache
+    @a_sync_ttl_cache
     async def pair_for(self, input_token: Address, output_token: Address, stable: bool) -> Address:
         return await self.contract.pairFor.coroutine(input_token, output_token, stable)
     
     @stuck_coro_debugger
-    @a_sync_cache
+    @a_sync_ttl_cache
     async def get_pool(self, input_token: Address, output_token: Address, stable: bool, block: Block) -> Optional[SolidlyPool]:
         pool_address = await self.pair_for(input_token, output_token, stable, sync=False)
         if await self.contract.isPair.coroutine(pool_address, block_identifier=block):
             return SolidlyPool(pool_address, asynchronous=self.asynchronous)
 
     @stuck_coro_debugger
     async def get_routes_from_path(self, path: Path, block: Block) -> List[Tuple[Address, Address, bool]]:
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-3.5.0/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/dex/uniswap/v1.py` & `ypricemagic-3.5.0/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/dex/uniswap/v2.py` & `ypricemagic-3.5.0/y/prices/dex/uniswap/v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
  
 import asyncio
 import itertools
 import logging
 from contextlib import suppress
 from decimal import Decimal
 from functools import cached_property
-from typing import Any, AsyncIterator, Awaitable, Callable, Dict, List, Optional, Tuple
+from typing import Any, AsyncIterator, Callable, Dict, List, Optional, Tuple
 
 import a_sync
+import a_sync.exceptions
 import brownie
 import dank_mids
 from a_sync.property import HiddenMethodDescriptor
 from brownie import chain
 from brownie.network.event import _EventItem
 from dank_mids.exceptions import Revert
 from multicall import Call
@@ -48,101 +49,119 @@
 
 try:
     FACTORY_HELPER = Contract(factory_helper_address)
 except ContractNotVerified:
     FACTORY_HELPER = None
 
 class UniswapV2Pool(ERC20):
-    __slots__ = 'get_reserves', '_token0', '_token1', '_types_assumed'
+    # defaults are stored as class vars to keep instance dicts smaller
+    __token0 = None
+    __token1 = None
+    __types_assumed = True
+    __slots__ = 'get_reserves',
     def __init__(
         self, 
         address: AnyAddressType, 
         token0: Optional[Address] = None, 
         token1: Optional[Address] = None, 
         deploy_block: Optional[int] = None, 
         asynchronous: bool = False,
     ):
         super().__init__(address, asynchronous=asynchronous)
         self.get_reserves = Call(self.address, 'getReserves()((uint112,uint112,uint32))')
-        self._deploy_block = deploy_block
-        self._token0 = token0
-        self._token1 = token1
-        self._types_assumed = True
+        if deploy_block:
+            self._deploy_block = deploy_block
+        if token0:
+            self.__token0 = token0
+        if token1:
+            self.__token1 = token1
         
     @a_sync.aka.cached_property
     async def factory(self) -> Address:
         try: return await raw_call(self.address, 'factory()', output='address', sync=False)
         except ValueError as e:
             if call_reverted(e):
-                raise NotAUniswapV2Pool from e
+                raise NotAUniswapV2Pool(self) from e
             # `is not a valid ETH address` means we got some kind of response from the chain.
             # but couldn't convert to address. If it happens to be a goofy but
             # verified uni fork, maybe we can get factory this way
             okay_errors = ['is not a valid ETH address','invalid opcode','invalid jump destination']
             if all(msg not in str(e) for msg in okay_errors):
                 raise
             contract = await Contract.coroutine(self.address)
             try: 
-                return await contract.factory.coroutine()
+                return await contract.factory
             except AttributeError as exc:
-                raise NotAUniswapV2Pool from exc
+                raise NotAUniswapV2Pool(self) from exc
     __factory__: HiddenMethodDescriptor[Self, Address]
 
     @a_sync.aka.property
     async def tokens(self) -> Tuple[ERC20, ERC20]:
         return await asyncio.gather(self.__token0__, self.__token1__)
-    __tokens__: HiddenMethodDescriptor[Self, ERC20]
+    __tokens__: HiddenMethodDescriptor[Self, Tuple[ERC20, ERC20]]
     
-    @a_sync.aka.property
+    @a_sync.aka.cached_property
     async def token0(self) -> ERC20:
-        if self._token0 is None:
-            try:
-                if token0 := await Call(self.address, ['token0()(address)']):
-                    self._token0 = ERC20(token0, asynchronous=self.asynchronous)
-            except ValueError as e:
-                continue_if_call_reverted(e)
-        if self._token0 is None:
-            raise NotAUniswapV2Pool(self.address)
-        return self._token0
+        # we can keep the instance smaller by popping this since its already cached
+        if token0 := self.__token0:
+            del self.__token0
+            return token0
+        try:
+            if token0 := await Call(self.address, ['token0()(address)']):
+                return ERC20(token0, asynchronous=self.asynchronous)
+        except ValueError as e:
+            continue_if_call_reverted(e)
+        raise NotAUniswapV2Pool(self)
     __token0__: HiddenMethodDescriptor[Self, ERC20]
 
-    @a_sync.aka.property
+    @a_sync.aka.cached_property
     async def token1(self) -> ERC20:
-        if self._token1 is None:
-            try:
-                if token1 := await Call(self.address, ['token1()(address)']):
-                    self._token1 = ERC20(token1, asynchronous=self.asynchronous)
-            except ValueError as e:
-                continue_if_call_reverted(e)
-        if self._token1 is None:
-            raise NotAUniswapV2Pool(self.address)
-        return self._token1
+        # we can keep the instance smaller by popping this since its already cached
+        if token1 := self.__token1:
+            del self.__token1
+            return token1
+        try:
+            if token1 := await Call(self.address, ['token1()(address)']):
+                return ERC20(token1, asynchronous=self.asynchronous)
+        except ValueError as e:
+            continue_if_call_reverted(e)
+        raise NotAUniswapV2Pool(self)
     __token1__: HiddenMethodDescriptor[Self, ERC20]
     
-    @a_sync.a_sync(cache_type='memory')
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     @stuck_coro_debugger
     async def get_price(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
         tvl = await self.tvl(block=block, skip_cache=skip_cache, sync=False)
         if tvl is not None:
             # TODO: move decimal conversion into total_supply_readable
             return UsdPrice(tvl / Decimal(await self.total_supply_readable(block=block, sync=False)))
         return None
     
+    @a_sync.a_sync(ram_cache_maxsize=None, ram_cache_ttl=ENVS.CACHE_TTL)
+    async def get_token_out(self, token_in: Address) -> ERC20:
+        if token_in == (token0 := await self.__token0__):
+            # these return instantly since theyre already cached
+            return await self.__token1__
+        elif token_in == (token1 := await self.__token1__):
+            # these return instantly since theyre already cached
+            return await self.__token0__
+        raise TokenNotFound(token_in, [token0, token1]) from None
+    
     @stuck_coro_debugger
     async def reserves(self, *, block: Optional[Block] = None) -> Optional[Tuple[WeiBalance, WeiBalance]]:
         reserves, tokens = await asyncio.gather(self.get_reserves.coroutine(block_id=block), self.__tokens__, return_exceptions=True)
 
         if isinstance(tokens, Exception):
             raise tokens
 
-        if reserves is None and self._types_assumed:
+        if reserves is None and self.__types_assumed:
             try:
                 await self._check_return_types()
             except AttributeError as e:
-                raise NotAUniswapV2Pool(self.address) from e
+                raise NotAUniswapV2Pool(self) from e
             return await self.reserves(block=block, sync=False)
         
         if reserves is None and self._verified:
             # This shouldn't really run anymore, maybe delete
             contract = await Contract.coroutine(self.address)
             try:
                 reserves = await contract.getReserves.coroutine(block_identifier=block)
@@ -157,38 +176,38 @@
         elif isinstance(reserves, Exception):
             raise reserves
 
         return tuple(WeiBalance(reserves[i], tokens[i], block=block) for i in range(2))
 
     @stuck_coro_debugger
     async def tvl(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[Decimal]:
-        tokens: List[ERC20] = await self.__tokens__
-        prices, reserves = await asyncio.gather(
-            asyncio.gather(*[token.price(block=block, return_None_on_failure=True, skip_cache=skip_cache, sync=False) for token in tokens]),
-            self.reserves(block=block, sync=False),
-        )
-
-        if reserves is None:
+        # start these tasks now
+        price_tasks: a_sync.TaskMapping[ERC20, UsdPrice]
+        price_tasks = ERC20.price.map(self.__tokens__, block=block, return_None_on_failure=True, skip_cache=skip_cache)
+
+        reserves: Tuple[WeiBalance, WeiBalance]
+        if (reserves := await self.reserves(block=block, sync=False)) is None:
+            await price_tasks.close()
             return None
 
-        vals = [
-            None if price is None else Decimal(await reserve.__readable__) * Decimal(price)
+        prices = await price_tasks.values()
+        if vals := [
+            Decimal(await reserve.__readable__) * Decimal(price)
             for reserve, price in zip(reserves, prices)
-        ]
-
-        if vals[0] is not None and not vals[1]:
-            vals[1] = vals[0]
-        if vals[1] is not None and not vals[0]:
-            vals[0] = vals[1]
-
-        logger.debug('reserves: %s', reserves)
-        logger.debug('prices: %s', prices)
-        logger.debug('vals: %s', vals)
-        if vals[0] is not None and vals[1] is not None:
-            return sum(vals)
+            if price is not None
+        ]:
+            if len(vals) == 1:
+                vals *= 2
+            if len(vals) == 2:
+                logger.debug('reserves: %s', reserves)
+                logger.debug('prices: %s', prices)
+                logger.debug('vals: %s', vals)
+                return sum(vals)
+            else:
+                raise Exception("how did we get here?") from None
     
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
     async def check_liquidity(self, token: Address, block: Block) -> int:
         logger.debug("checking %s liquidity for %s at %s", self, token, block)
         if block and block < await self.deploy_block(sync=False):
             logger.debug("block %s is before %s deploy block", block, self)
@@ -205,27 +224,27 @@
 
     @stuck_coro_debugger
     async def is_uniswap_pool(self, block: Optional[Block] = None) -> bool:
         try:
             return all(await asyncio.gather(self.reserves(block=block, sync=False), self.total_supply(block, sync=False)))
         except NotAUniswapV2Pool:
             return False
-        
+    
     async def _check_return_types(self) -> None:
-        if not self._types_assumed:
+        if not self.__types_assumed:
             return
         try:
             contract = await Contract.coroutine(self.address)
             reserves_types = ",".join(output["type"] for output in contract.getReserves.abi["outputs"])
             self._verified = True
             assert reserves_types.count(',') == 2, reserves_types
             self.get_reserves = Call(self.address, f'getReserves()(({reserves_types}))')
         except ContractNotVerified:
             self._verified = False
-        self._types_assumed = False
+        self.__types_assumed = False
 
 
 class PoolsFromEvents(ProcessedEvents[UniswapV2Pool]):
     PairCreated = "0x0d3648bd0f6ba80134a33ba9275ac585d9d315f0ad8355cddefde31afa28d0e9"
     __slots__ = "asynchronous", "label"
     def __init__(self, factory: AnyAddressType, label: str, asynchronous: bool = False):
         self.asynchronous = asynchronous
@@ -307,15 +326,15 @@
             with suppress(CantFindSwapPath):
                 path = await self.get_path_to_stables(token_in, block, _ignore_pools=ignore_pools, sync=False)
                 logger.debug('smrt')
 
         # If we can't find a good path to stables, we might still be able to determine price from price of paired token
         if path is None and (deepest_pool:= await self.deepest_pool(token_in, block, _ignore_pools=ignore_pools, sync=False)):
             logger.debug('deepest pool: %s', deepest_pool)
-            paired_with = (await self.get_pools_for(token_in, sync=False))[deepest_pool]
+            paired_with = await deepest_pool.get_token_out(token_in, sync=False)
             path = [token_in, paired_with]
             quote, out_scale = await asyncio.gather(self.get_quote(amount_in, path, block=block, sync=False), ERC20(path[-1], asynchronous=True).scale)
             logger.debug('quote: %s', quote)
             if quote is not None:
                 amount_out = Decimal(quote[-1]) / out_scale  
                 fees = Decimal(0.997) ** (len(path) - 1)
                 amount_out /= fees
@@ -361,27 +380,22 @@
     @stuck_coro_debugger
     async def pools(self) -> List[UniswapV2Pool]:
         logger.info('Fetching pools for %s on %s. If this is your first time using ypricemagic, this can take a while. Please wait patiently...', self.label, Network.printable())
         pools = [pool async for pool in self._events.pools(to_block=await dank_mids.eth.block_number)]
         all_pairs_len = await raw_call(self.factory, 'allPairsLength()', output='int', sync=False)
         if len(pools) > all_pairs_len:
             raise NotImplementedError('this shouldnt happen again')
-        elif len(pools) < all_pairs_len: # <
-            to_get = all_pairs_len - len(pools)
+        elif (to_get := all_pairs_len - len(pools)): # <
             logger.debug("Oh no! Looks like your node can't look back that far. Checking for the missing %s pools...", to_get)
             factory = await Contract.coroutine(self.factory)
-            async def _load_pool(i):
-                pool = await factory.allPairs.coroutine(i)
-                logger.debug('pool: %s', pool)
-                pool = UniswapV2Pool(address=pool, asynchronous=self.asynchronous)
-                await asyncio.gather(pool.__token0__, pool.__token1__)
-                return pool
-            pools = await asyncio.gather(*[_load_pool(i) for i in range(to_get)]) + pools
+            for i, pool_address in enumerate(await factory.allPairs.map(range(to_get))):
+                pool = UniswapV2Pool(address=pool_address, asynchronous=self.asynchronous)
+                pools.insert(i, pool)
             logger.debug('Done fetching %s missing pools on %s', to_get, self.label)
-        tokens = set(await asyncio.gather(*itertools.chain(*((pool.__token0__, pool.__token1__) for pool in pools))))
+        tokens = set(await UniswapV2Pool.token0.map(pools).values() + await UniswapV2Pool.token1.map(pools).values())
         logger.info('Loaded %s pools supporting %s tokens on %s', len(pools), len(tokens), self.label)
         return pools
     __pools__: HiddenMethodDescriptor[Self, List[UniswapV2Pool]]
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=None, ram_cache_ttl=60*60)
     async def get_pools_for(self, token_in: Address, block: Optional[Block] = None) -> Dict[UniswapV2Pool, Address]:
@@ -393,60 +407,68 @@
                 ]
             except Exception as e:
                 if block is None:
                     raise e
                 if not call_reverted(e) and "out of gas" not in str(e) and "timeout" not in str(e):
                     raise e
                 pool_to_token_out = {}
-                async for pool, (token0, token1) in a_sync.map(_get_tokens, await self.__pools__):
+                pools = await self.__pools__
+                async for pool, (token0, token1) in UniswapV2Pool.tokens.map(pools, concurrency=min(50_000, len(pools))):
                     if token_in == token0:
                         pool_to_token_out[pool] = token1
                     elif token_in == token1:
                         pool_to_token_out[pool] = token0
                 if not pool_to_token_out:
                     logger.debug("no data returned and 0 pools when checking the long way!")
                 else:
                     logger.debug("no data returned but we have pools when checking the long way...")
                 return pool_to_token_out
 
         else:
             pools = await self.__pools__
         pool_to_token_out = {}
-        async for pool, (token0, token1) in a_sync.map(_get_tokens, pools):
+        async for pool, (token0, token1) in UniswapV2Pool.tokens.map(pools, concurrency=min(50_000, len(pools))):
             if token_in == token0:
                 pool_to_token_out[pool] = token1
             elif token_in == token1:
                 pool_to_token_out[pool] = token0
         return pool_to_token_out
 
     @stuck_coro_debugger
-    async def pools_for_token(self, token_address: Address, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Dict[UniswapV2Pool, Address]:
+    async def pools_for_token(self, token_address: Address, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> AsyncIterator[UniswapV2Pool]:
         pools: Dict[UniswapV2Pool, Address]
         
         if chain.id == Network.Mainnet and token_address == WRAPPED_GAS_COIN and self.label == "uniswap v2":
             # This will run out of gas if we use the helper so we bypass it with a known liquid pool
             pools = {UniswapV2Pool("0xB4e16d0168e52d35CaCD2c6185b44281Ec28C9Dc", asynchronous=True): "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"}
         else:
             try:
                 pools = await self.get_pools_for(token_address, sync=False)
             except Exception as e:
+                raise e
                 if 'out of gas' not in str(e) and not call_reverted(e):
                     e.args = (*e.args, self, token_address, block)
                     raise e
                 try:
                     # if it fails with no block we will try once with a block before we fetch the long way
                     pools = await self.get_pools_for(token_address, block=block, sync=False)
                 except Exception as e:
                     e.args = (*e.args, self, token_address, block)
                     raise e
-        pools = {k: v for k, v in pools.items() if k not in _ignore_pools}
-        if pools and block is not None:
-            deploy_blocks = await asyncio.gather(*[pool.deploy_block(when_no_history_return_0=True, sync=False) for pool in pools])
-            pools = {k: v for (k, v), deploy_block in zip(pools.items(), deploy_blocks) if deploy_block <= block}
-        return pools
+        for pool in _ignore_pools:
+            pools.pop(pool, None)
+        if not pools:
+            return
+        elif block is None:
+            for pool in pools:
+                yield pool
+        else:
+            async for pool, deploy_block in a_sync.map(ERC20.deploy_block, pools, when_no_history_return_0=True).map():
+                if deploy_block <= block:
+                    yield pool
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=500)
     async def deepest_pool(self, token_address: AnyAddressType, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Optional[UniswapV2Pool]:
         """returns the deepest pool for `token_address` at `block`, excluding pools in `_ignore_pools`"""
         token_address = convert.to_address(token_address)
         if token_address == WRAPPED_GAS_COIN or token_address in STABLECOINS:
@@ -459,78 +481,76 @@
                 # TODO: debug me!
                 logger.debug('helper reverted for %s at block %s ignore_pools %s: %s', token_address, block, _ignore_pools, e)
             except ValueError as e:
                 if "out of gas" not in str(e):
                     raise e
                 logger.debug('helper out of gas for %s at block %s ignore_pools %s: %s', token_address, block, _ignore_pools, e)
 
-        pools: List[UniswapV2Pool] = list((await self.pools_for_token(token_address, block, _ignore_pools=_ignore_pools, sync=False)).keys())
-        if not pools:
-            return None
-        liquidity = await asyncio.gather(*[pool.check_liquidity(token_address, block, sync=False) for pool in pools])
-
         deepest_pool = None
         deepest_pool_balance = 0
-        for pool, depth in zip(pools, liquidity):
+        pools = self.pools_for_token(token_address, block, _ignore_pools=_ignore_pools)
+        async for pool, depth in UniswapV2Pool.check_liquidity.map(pools, token=token_address, block=block):
             if depth and depth > deepest_pool_balance:
                 deepest_pool = pool
                 deepest_pool_balance = depth
         return deepest_pool
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=500)
     async def deepest_stable_pool(self, token_address: AnyAddressType, block: Optional[Block] = None, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Optional[UniswapV2Pool]:
         """returns the deepest pool for `token_address` at `block` which has `token_address` paired with a stablecoin, excluding pools in `_ignore_pools`"""
-        token_address = convert.to_address(token_address)
-        stable_pools: Dict[UniswapV2Pool, Address] = {
+        pools = self.pools_for_token(convert.to_address(token_address), None, _ignore_pools=_ignore_pools)
+        stable_pools = {
             pool: paired_with
-            for pool, paired_with in (await self.pools_for_token(token_address, None, _ignore_pools=_ignore_pools, sync=False)).items()
+            async for pool, paired_with
+            in UniswapV2Pool.get_token_out.map(pools, token_in=token_address)
             if paired_with in STABLECOINS
         }
         
         if stable_pools:
             if self._supports_uniswap_helper and (block is None or block >= await contract_creation_block_async(FACTORY_HELPER)):
                 deepest_stable_pool, deepest_stable_pool_balance = await FACTORY_HELPER.deepestPoolForFrom.coroutine(token_address, tuple(stable_pools), block_identifier=block)
                 return None if deepest_stable_pool == brownie.ZERO_ADDRESS else UniswapV2Pool(deepest_stable_pool, asynchronous=self.asynchronous)
 
             elif block is not None:
-                deploy_blocks = await asyncio.gather(*[pool.deploy_block(when_no_history_return_0=True, sync=False) for pool in stable_pools])
-                stable_pools = {pool: paired_with for (pool, paired_with), deploy_block in zip(stable_pools.items(), deploy_blocks) if deploy_block <= block}
+                stable_pools = {
+                    pool: stable_pools[pool] 
+                    async for pool, deploy_block 
+                    in a_sync.map(ERC20.deploy_block, stable_pools, when_no_history_return_0=True).map()
+                    if deploy_block <= block
+                }
             
         if not stable_pools:
             return None
         
-        liquidity = await asyncio.gather(*[pool.check_liquidity(token_address, block, sync=False) for pool in stable_pools])
-
         deepest_stable_pool = None
         deepest_stable_pool_balance = 0
-        for pool, depth in zip(stable_pools, liquidity):
+        async for pool, depth in UniswapV2Pool.check_liquidity.map(stable_pools, token=token_address, block=block).map():
             if depth > deepest_stable_pool_balance:
                 deepest_stable_pool = pool
                 deepest_stable_pool_balance = depth
         return deepest_stable_pool
 
     @stuck_coro_debugger
     @a_sync.a_sync(ram_cache_maxsize=500)
     async def get_path_to_stables(self, token: AnyAddressType, block: Optional[Block] = None, _loop_count: int = 0, _ignore_pools: Tuple[UniswapV2Pool,...] = ()) -> Path:
         if _loop_count > 10:
             raise CantFindSwapPath
         token_address = convert.to_address(token)
         path = [token_address]
         deepest_pool = await self.deepest_pool(token_address, block, _ignore_pools, sync=False)
         if deepest_pool:
-            paired_with = (await self.get_pools_for(token_address, sync=False))[deepest_pool]
+            paired_with = await deepest_pool.get_token_out(token_address, sync=False)
             from y.prices.utils.buckets import check_bucket
             if await check_bucket(paired_with, sync=False) and _loop_count == 0:
                 # let's just use the other token to get the price
                 return None
             deepest_stable_pool = await self.deepest_stable_pool(token_address, block, _ignore_pools=_ignore_pools, sync=False)
             if deepest_stable_pool and deepest_pool == deepest_stable_pool:
-                last_step = (await self.get_pools_for(token_address, sync=False))[deepest_stable_pool]
-                path.append(last_step)
+                path.append(await deepest_stable_pool.get_token_out(token_address, sync=False))
                 return path
 
             if path == [token_address]:
                 with suppress(CantFindSwapPath):
                     path.extend(
                         await self.get_path_to_stables(
                             paired_with,
@@ -562,16 +582,19 @@
                 # TODO: debug me!
                 logger.debug('helper reverted on check_liquidity for %s at block %s: %s',token, block, e)
             except ValueError as e:
                 if "out of gas" not in str(e):
                     raise e
                 logger.debug('helper out of gas on check_liquidity for %s at block %s: %s',token, block, e)
                 
-        pools: Dict[UniswapV2Pool, Address] = await self.pools_for_token(token, block=block, _ignore_pools=ignore_pools, sync=False)
-        liquidity = max(await asyncio.gather(*[pool.check_liquidity(token, block) for pool in pools])) if pools else 0
+        pools = self.pools_for_token(token, block=block, _ignore_pools=ignore_pools)
+        try:
+            liquidity = await UniswapV2Pool.check_liquidity.max(pools, token=token, block=block, sync=False)
+        except a_sync.exceptions.EmptySequenceError:
+            return 0
         logger.debug("%s liquidity for %s at %s is %s", self, token, block, liquidity)
         return liquidity
 
     @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
     async def deepest_pool_for(self, token: Address, block: Block = None, *, ignore_pools = []) -> Tuple[Address, int]:
         # sourcery skip: default-mutable-arg
         try:
@@ -604,8 +627,7 @@
             else:                                                                           path = [token_in,wbnb.address,token_out]
         else:
             if WRAPPED_GAS_COIN in (token_in, token_out):                                   path = [token_in, token_out]
             else:                                                                           path = [token_in, WRAPPED_GAS_COIN, token_out]
 
         return path
     
-_get_tokens: Callable[[UniswapV2Pool], Awaitable[Tuple[ERC20, ERC20]]] = lambda pool: asyncio.gather(pool.__token0__, pool.__token1__)
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-3.5.0/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/dex/uniswap/v3.py` & `ypricemagic-3.5.0/y/prices/dex/uniswap/v3.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self,
         address: Address,
         token0: Address, 
         token1: Address, 
         tick_spacing: int, 
         fee: int, 
         deploy_block: int,
-        asynchronous: bool = True
+        asynchronous: bool = False
     ) -> None:
         super().__init__(address, asynchronous=asynchronous)
         self.token0 = ERC20(token0, asynchronous=asynchronous)
         self.token1 = ERC20(token1, asynchronous=asynchronous)
         self.tick_spacing = tick_spacing
         self.fee = fee
         self._deploy_block = deploy_block
@@ -98,14 +98,18 @@
             liquidity = await self[token].balance_of(self.address, block, sync=False)
         except ContractNotVerified:
             logger.debug("%s is not verified and we cannot fetch balance the usual way. returning 0.", token)
             return 0
         logger.debug("%s liquidity for %s at %s: %s", self, token, block, liquidity)
         return liquidity
     
+    @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
+    async def _check_liquidity_token_out(self, token_in: AnyAddressType, block: Block) -> Optional[int]:
+        return await self.check_liquidity(self._get_token_out(token_in), block=block, sync=False)
+    
     @lru_cache
     def _get_token_out(self, token_in: ERC20) -> ERC20:
         if token_in == self.token0:
             return self.token1
         elif token_in == self.token1:
             return self.token0
         raise TokenNotFound(token_in, self)
@@ -202,41 +206,44 @@
             return 0
         
         quoter = await self.__quoter__
         if block and block < await contract_creation_block_async(quoter):
             logger.debug("block %s is before %s deploy block", block, quoter)
             return 0
         
-        token_in_tasks: Dict[UniswapV3Pool, asyncio.Task] = {}
-        token_out_tasks: Dict[UniswapV3Pool, asyncio.Task] = {}
+        token_out_tasks = UniswapV3Pool._check_liquidity_token_out.map(token_in=token, block=block)
         async for pool in self.pools_for_token(token, block):
             if pool not in ignore_pools:
-                token_in_tasks[pool] = asyncio.create_task(pool.check_liquidity(token, block, sync=False))
-                token_out_tasks[pool] = asyncio.create_task(pool.check_liquidity(pool._get_token_out(token), block, sync=False))
+                # the mapping will start the tasks internally
+                token_out_tasks[pool]
+        if not token_out_tasks:
+            return 0
         
         # Since uni v3 liquidity can be provided asymmetrically, the most liquid pool in terms of `token` might not actually be the most liquid pool in terms of `token_out`
         # We need some spaghetticode here to account for these erroneous liquidity values
         # TODO: Refactor this
-        token_out_liquidity: DefaultDict[ERC20, List[asyncio.Task]] = defaultdict(list)
-        for pool, task in token_out_tasks.items():
-            token_out_liquidity[pool._get_token_out(token)].append(task)
+        token_out_liquidity: DefaultDict[ERC20, List[int]] = defaultdict(list)
+        async for pool, liquidity in token_out_tasks:
+            token_out_liquidity[pool._get_token_out(token)].append(liquidity)
         
-        token_out_min_liquidity = {token_out: min(await asyncio.gather(*tasks)) for token_out, tasks in token_out_liquidity.items()}
-        for pool, task in token_out_tasks.items():
+        token_out_min_liquidity = {token_out: min(liquidities) for token_out, liquidities in token_out_liquidity.items()}
+
+        token_in_tasks = UniswapV3Pool.check_liquidity.map(token=token, block=block)
+        async for pool, liquidity in token_out_tasks:
+            token_out_tasks.pop(pool)
             token_out = pool._get_token_out(token)
-            liquidity = await task
             if len(token_out_liquidity[token_out]) > 1 and liquidity == token_out_min_liquidity[token_out]:
                 logger.debug("ignoring liquidity for %s", pool)
-                token_in_tasks.pop(pool)
             elif token_out == weth and liquidity < 10 ** 19:  # 10 ETH
                 # NOTE: this is totally arbitrary, works for all known cases but eventually will probably cause issues
                 logger.debug("insufficient liquidity for %s", pool)
-                token_in_tasks.pop(pool)
+            else:
+                token_in_tasks[pool]
 
-        liquidity = max(await asyncio.gather(*token_in_tasks.values())) if token_in_tasks else 0
+        liquidity = await token_in_tasks.max(pop=True, sync=False) if token_in_tasks else 0
         logger.debug("%s liquidity for %s at %s is %s", self, token, block, liquidity)
         return liquidity
 
 def _encode_path(path) -> bytes:
     types = [type for _, type in zip(path, cycle(['address', 'uint24']))]
     return encode_packed(types, path)
```

### Comparing `ypricemagic-3.4.9/y/prices/dex/velodrome.py` & `ypricemagic-3.5.0/y/prices/dex/velodrome.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 import a_sync
 import dank_mids
 import eth_retry
 from async_lru import alru_cache
 from brownie import chain
 from multicall.call import Call
 
-from y import ENVIRONMENT_VARIABLES as ENVS
 from y.contracts import Contract
 from y.datatypes import Address, AnyAddressType, Block
 from y.decorators import stuck_coro_debugger
 from y.interfaces.uniswap.velov2 import VELO_V2_FACTORY_ABI
 from y.networks import Network
 from y.prices.dex.solidly import SolidlyRouterBase
 from y.prices.dex.uniswap.v2 import Path, UniswapV2Pool
 from y.utils import gather_methods
-from y.utils.cache import a_sync_cache
+from y.utils.cache import a_sync_ttl_cache
 from y.utils.raw_calls import raw_call
 
 _INIT_METHODS = 'token0()(address)', 'token1()(address)', 'stable()(bool)'
 
 logger = logging.getLogger(__name__)
 
 class NoReservesError(Exception):
@@ -50,20 +49,20 @@
 class VelodromeRouterV2(SolidlyRouterBase):
     _supports_uniswap_helper = False
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.default_factory = default_factory[chain.id]
     
     @stuck_coro_debugger
-    @a_sync_cache
+    @a_sync_ttl_cache
     async def pool_for(self, input_token: Address, output_token: Address, stable: bool) -> Address:
         return await self.contract.poolFor.coroutine(input_token, output_token, stable, self.default_factory)
     
     @stuck_coro_debugger
-    @a_sync_cache
+    @a_sync_ttl_cache
     @eth_retry.auto_retry
     async def get_pool(self, input_token: Address, output_token: Address, stable: bool, block: Block) -> Optional[UniswapV2Pool]:
         pool_address = await self.pool_for(input_token, output_token, stable, sync=False)
         if await dank_mids.eth.get_code(str(pool_address), block_identifier=block) not in ['0x',b'']:
             return UniswapV2Pool(pool_address, asynchronous=self.asynchronous)
     
     @a_sync.aka.cached_property
@@ -94,20 +93,19 @@
         all_pools_len = await raw_call(self.factory, 'allPoolsLength()', output='int', sync=False)
 
         if len(pools) > all_pools_len:
             raise ValueError('wtf', len(pools), all_pools_len)
         
         if len(pools) < all_pools_len:
             logger.debug("Oh no! Looks like your node can't look back that far. Checking for the missing %s pools...", all_pools_len - len(pools))
-            pools_your_node_couldnt_get = {
-                i: asyncio.create_task(coro=self._init_pool_from_poolid(i), name=f"load {self} poolId {i}") 
-                for i in range(all_pools_len - len(pools))
-            }
+            pools_your_node_couldnt_get = a_sync.map(self._init_pool_from_poolid, range(all_pools_len - len(pools)), name=f"load {self} poolId")
+            # we want the map populated with tasks for this logger
+            await pools_your_node_couldnt_get._init_loader
             logger.debug('pools: %s', pools_your_node_couldnt_get)
-            pools.update([pool async for id, pool in a_sync.as_completed(pools_your_node_couldnt_get, aiter=True)])
+            pools.update(await pools_your_node_couldnt_get.values())
 
         tokens = set()
         for pool in pools:
             tokens.update(await asyncio.gather(pool.__token0__, pool.__token1__))
         logger.info('Loaded %s pools supporting %s tokens on %s', len(pools), len(tokens), self.label)
         return pools
```

### Comparing `ypricemagic-3.4.9/y/prices/eth_derivs/creth.py` & `ypricemagic-3.5.0/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/eth_derivs/wsteth.py` & `ypricemagic-3.5.0/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/gearbox.py` & `ypricemagic-3.5.0/y/prices/gearbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y.classes.common import ERC20, ContractBase
 from y.contracts import Contract
 from y.datatypes import Address, Block
 from y.exceptions import UnsupportedNetwork
 from y.networks import Network
-from y.utils.cache import a_sync_cache
+from y.utils.cache import a_sync_ttl_cache
 
 registry = "0xA50d4E7D8946a7c90652339CDBd262c375d54D99"
 
 class DieselPool(ContractBase):
     @a_sync.aka.cached_property
     async def contract(self) -> Contract:
         return await Contract.coroutine(self.address)
     __contract__: HiddenMethodDescriptor[Self, Contract]
     
     @a_sync.aka.cached_property
     async def diesel_token(self) -> ERC20:
         contract = await self.__contract__
         try:
-            return ERC20(await contract.dieselToken.coroutine(), asynchronous=self.asynchronous)
+            return ERC20(await contract.dieselToken, asynchronous=self.asynchronous)
         except AttributeError: # NOTE: there could be better ways of doing this with hueristics, not sure yet
             return ERC20(self.address, asynchronous=self.asynchronous)
     __diesel_token__: HiddenMethodDescriptor[Self, ERC20]
     
     @a_sync.aka.cached_property
     async def underlying(self) -> ERC20:
         contract = await self.__contract__
-        return ERC20(await contract.underlyingToken.coroutine(), asynchronous=self.asynchronous)
+        return ERC20(await contract.underlyingToken, asynchronous=self.asynchronous)
     __underlying__: HiddenMethodDescriptor[Self, ERC20]
     
     async def exchange_rate(self, block: Block) -> Decimal:
         underlying: ERC20
         pool, underlying = await asyncio.gather(self.__contract__, self.__underlying__)
         scale = await underlying.__scale__
         return Decimal(await pool.fromDiesel.coroutine(scale, block_identifier=block)) / Decimal(scale)
@@ -59,23 +59,22 @@
         else:
             raise UnsupportedNetwork()
     
     @a_sync.aka.cached_property
     async def registry(self) -> Contract:
         return await Contract.coroutine(registry)
     
-    @a_sync_cache
+    @a_sync_ttl_cache
     async def pools(self) -> List[DieselPool]:
         registry = await self.registry
-        return [DieselPool(pool, asynchronous=self.asynchronous) for pool in await registry.getPools.coroutine()]
+        return [DieselPool(pool, asynchronous=self.asynchronous) for pool in await registry.getPools]
     
     async def diesel_tokens(self) -> Dict[ERC20, DieselPool]:
         pools: List[DieselPool] = await self.pools(sync=False)
-        dtokens = await asyncio.gather(*[pool.__diesel_token__ for pool in pools])
-        return dict(zip(dtokens, pools))
+        return dict(zip(await DieselPool.diesel_token.map(pools).values(), pools))
 
     async def is_diesel_token(self, token: Address) -> bool:
         return token in await self.diesel_tokens(sync=False)
     
     async def get_price(self, token: Address, block: Block, skip_cache: bool = ENVS.SKIP_CACHE) -> Decimal:
         dtokens = await self.diesel_tokens()
         return await dtokens[token].get_price(block, skip_cache=skip_cache, sync=False)
```

### Comparing `ypricemagic-3.4.9/y/prices/lending/aave.py` & `ypricemagic-3.5.0/y/prices/lending/aave.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,35 +92,36 @@
     async def underlying(self, token_address: AddressOrContract) -> ERC20:...
     @abstractproperty
     def _get_reserves_method(self) -> str:...
 
 class AaveMarketV1(AaveMarketBase):
     @a_sync.aka.cached_property
     async def atokens(self) -> List[ERC20]:
-        reserves = await self.get_reserves(sync=False)
-        reserves_data = await asyncio.gather(*[self.get_reserve_data(reserve, sync=False) for reserve in reserves])
-        atokens = [ERC20(reserve_data['aTokenAddress'], asynchronous=self.asynchronous) for reserve_data in reserves_data]
+        reserves_data = a_sync.map(self.get_reserve_data, self.get_reserves(sync=False))
+        atokens = [
+            ERC20(reserve_data['aTokenAddress'], asynchronous=self.asynchronous) 
+            async for _, reserve_data in reserves_data
+        ]
         logger.info('loaded %s v1 atokens for %s', len(atokens), self)
         return atokens
     @a_sync.a_sync(ram_cache_maxsize=256)
     async def underlying(self, token_address: AddressOrContract) -> ERC20:
         underlying = await raw_call(token_address, 'underlyingAssetAddress()', output='address', sync=False)
         return ERC20(underlying)
     _get_reserves_method = 'getReserves()(address[])'
 
 
 _V2_RESERVE_DATA_METHOD = 'getReserveData(address)((uint256,uint128,uint128,uint128,uint128,uint128,uint40,address,address,address,address,uint8))'
 
 class AaveMarketV2(AaveMarketBase):
     @a_sync.aka.cached_property
     async def atokens(self) -> List[ERC20]:
-        reserves = await self.get_reserves(sync=False)
-        reserves_data = await asyncio.gather(*[self.get_reserve_data(reserve, sync=False) for reserve in reserves])
+        reserves_data = a_sync.map(self.get_reserve_data, self.get_reserves(sync=False))
         try:
-            atokens = [ERC20(reserve_data[7], asynchronous=self.asynchronous) for reserve_data in reserves_data]
+            atokens = [ERC20(reserve_data[7], asynchronous=self.asynchronous) async for _, reserve_data in reserves_data]
             logger.info('loaded %s v2 atokens for %s', len(atokens), self)
             return atokens
         except TypeError as e: # TODO figure out what to do about non verified aave markets
             logger.exception(e)
             logger.warning('failed to load tokens for %s', self)
             return []
     async def get_reserve_data(self, reserve: AnyAddressType) -> tuple:
@@ -132,18 +133,17 @@
         return ERC20(underlying, asynchronous=self.asynchronous)
     _get_reserves_method = 'getReservesList()(address[])'
 
 
 class AaveMarketV3(AaveMarketBase):
     @a_sync.aka.cached_property
     async def atokens(self) -> List[ERC20]:
-        reserves = await self.get_reserves(sync=False)
-        reserves_data = await asyncio.gather(*[self.get_reserve_data(reserve, sync=False) for reserve in reserves])
+        reserves_data = a_sync.map(self.get_reserve_data, self.get_reserves(sync=False))
         try:
-            atokens = [ERC20(reserve_data[8], asynchronous=self.asynchronous) for reserve_data in reserves_data]
+            atokens = [ERC20(reserve_data[8], asynchronous=self.asynchronous) async for _, reserve_data in reserves_data]
             logger.info('loaded %s v3 atokens for %s', len(atokens), self)
             return atokens
         except TypeError as e: # TODO figure out what to do about non verified aave markets
             logger.exception(e)
             logger.warning('failed to load tokens for %s', self)
             return []
     @a_sync.a_sync(ram_cache_maxsize=256)
```

### Comparing `ypricemagic-3.4.9/y/prices/lending/compound.py` & `ypricemagic-3.5.0/y/prices/lending/compound.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,20 +208,20 @@
     
     def __contains__(self, token_address: AddressOrContract) -> bool:
         if self.asynchronous:
             raise RuntimeError("'self.asynchronous' must be False and the event loop must not be running")
         return self.is_compound_market(token_address)
     
     async def get_troller(self, token_address: AddressOrContract) -> Optional[Comptroller]:
-        trollers = self.trollers.values()
-        all_markets = await asyncio.gather(*[troller.__markets__ for troller in trollers])
-        for troller, markets in zip(trollers, all_markets):
-            if token_address in markets:
-                return troller
+        if self.trollers:
+            async for troller, markets in Comptroller.markets.map(self.trollers.values()):
+                if token_address in markets:
+                    return troller
             
+    @a_sync.a_sync(ram_cache_ttl=5*60)
     async def is_compound_market(self, token_address: AddressOrContract) -> bool:
         if await self.get_troller(token_address, sync=False):
             return True
 
         # NOTE: Workaround for pools that have since been revoked
         result = await has_methods(token_address, ('isCToken()(bool)','comptroller()(address)','underlying()(address)'), sync=False)
         if result is True:
```

### Comparing `ypricemagic-3.4.9/y/prices/lending/ib.py` & `ypricemagic-3.5.0/y/prices/lending/ib.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from y.contracts import has_methods
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.prices import magic
 from y.utils import gather_methods
 
 logger = logging.getLogger(__name__)
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', ram_cache_ttl=5*60)
 async def is_ib_token(token: AnyAddressType) -> bool:
     return await has_methods(token, ('debtShareToVal(uint)(uint)','debtValToShare(uint)(uint)','token()(address)','totalToken()(uint)','totalSupply()(uint)'), sync=False)
 
 @a_sync.a_sync(default='sync')
 async def get_price(token: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
     address = convert.to_address(token)
     token, total_bal, total_supply = await gather_methods(address, ['token', 'totalToken', 'totalSupply'], block=block)
```

### Comparing `ypricemagic-3.4.9/y/prices/magic.py` & `ypricemagic-3.5.0/y/prices/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
     block = block or await dank_mids.eth.block_number
     token_address = convert.to_address(token_address)
     try:
         return await _get_price(token_address, block, fail_to_None=fail_to_None, ignore_pools=ignore_pools, skip_cache=skip_cache, silent=silent)
     except (ContractNotFound, NonStandardERC20, PriceError) as e:
         symbol = await ERC20(token_address, asynchronous=True).symbol
         if not fail_to_None:
-            raise yPriceMagicError(e, token_address, block, symbol) from e
+            raise_from = None if isinstance(e, PriceError) else e
+            raise yPriceMagicError(e, token_address, block, symbol) from raise_from
 
 GetPrice = Callable[..., Awaitable[Optional[UsdPrice]]]
 
 
 
 @a_sync.a_sync(default='sync')
 async def get_prices(
@@ -81,39 +82,22 @@
     - if `silent == False`, tqdm will be used
 
     When `get_prices` is unable to find a price:
     - if `fail_to_None == True`, ypricemagic will return `None` for that token
     - if `fail_to_None == False`, ypricemagic will raise a yPriceMagicError
     '''
 
-    if block is None:
-        block = await dank_mids.eth.block_number
-
-    prices = await asyncio.gather(
-        *[
-            get_price(
-                token_address=convert.to_address(token), 
-                block=block, 
-                fail_to_None=fail_to_None, 
-                skip_cache=skip_cache, 
-                silent=silent, 
-                sync=False,
-            )
-            for token in token_addresses
-        ],
-        return_exceptions=True
-    )
-
-    if not fail_to_None:
-        raise_if_exception_in(prices)
-    else:
-        for p in prices:
-            if isinstance(p, Exception) and not isinstance(p, PriceError):
-                raise p
-    return prices
+    return await a_sync.map(
+        get_price,
+        token_addresses,
+        block=block or await dank_mids.eth.block_number, 
+        fail_to_None=fail_to_None, 
+        skip_cache=skip_cache, 
+        silent=silent, 
+    ).values()
 
 def __cache(get_price: GetPrice) -> GetPrice:
     @functools.wraps(get_price)
     async def cache_wrap(
         token: AnyAddressType, 
         block: Block,
         *,
```

### Comparing `ypricemagic-3.4.9/y/prices/one_to_one.py` & `ypricemagic-3.5.0/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/popsicle.py` & `ypricemagic-3.5.0/y/prices/popsicle.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from y.utils import gather_methods
 
 _RESERVES_METHODS = 'token0()(address)', 'token1()(address)', 'usersAmounts()((uint,uint))'
 
 logger = logging.getLogger(__name__)
 
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=5*60)
 async def is_popsicle_lp(token_address: AnyAddressType) -> bool:
     # NOTE: contract to check for reference (mainnet): 0xd2C5A739ebfE3E00CFa88A51749d367d7c496CCf
     return await has_methods(token_address, ('token0()(address)','token1()(address)','usersAmounts()((uint,uint))'), sync=False)
 
 @a_sync.a_sync(default='sync')
 async def get_price(token: AnyAddressType, block: Optional[Block] = None, *, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdPrice]:
     address = convert.to_address(token)
@@ -32,17 +32,15 @@
     total_supply = await ERC20(address, asynchronous=True).total_supply_readable(block, sync=False)
     return UsdPrice(total_val / total_supply)
 
 @a_sync.a_sync(default='sync')
 async def get_tvl(token: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdValue]:
     balances: Tuple[WeiBalance, WeiBalance]
     balances = await get_balances(token, block, skip_cache=skip_cache, _async_balance_objects=True, sync=False)
-    if balances is None:
-        return None
-    return UsdValue(sum(await asyncio.gather(*[bal.value_usd for bal in balances])))
+    return UsdValue(await WeiBalance.value_usd.sum(balances)) if balances else None
 
 @a_sync.a_sync(default='sync')
 async def get_balances(token: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE, _async_balance_objects: bool = False) -> Optional[Tuple[WeiBalance,WeiBalance]]:
     try:
         token0, token1, (balance0, balance1) = await gather_methods(convert.to_address(token), _RESERVES_METHODS, block=block)
     except Exception as e:
         if call_reverted(e):
```

### Comparing `ypricemagic-3.4.9/y/prices/rkp3r.py` & `ypricemagic-3.5.0/y/prices/rkp3r.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/solidex.py` & `ypricemagic-3.5.0/y/prices/solidex.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 async def get_price(token: AnyAddressType, block: Optional[int] = None, skip_cache: bool = ENVS.SKIP_CACHE):
     pool = await _get_pool(token)
     return await magic.get_price(pool, block, skip_cache=skip_cache, sync=False)
 
 @alru_cache(maxsize=None)
 async def _get_pool(token) -> EthAddress:
     contract = await Contract.coroutine(token)
-    return await contract.pool.coroutine()
+    return await contract.pool
```

### Comparing `ypricemagic-3.4.9/y/prices/stable_swap/belt.py` & `ypricemagic-3.5.0/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/stable_swap/curve.py` & `ypricemagic-3.5.0/y/prices/stable_swap/curve.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from y.contracts import Contract, contract_creation_block_async
 from y.datatypes import (Address, AddressOrContract, AnyAddressType, Block,
                          Pool, UsdPrice, UsdValue)
 from y.exceptions import (ContractNotVerified, MessedUpBrownieContract,
                           PriceError, UnsupportedNetwork, call_reverted)
 from y.interfaces.curve.CurveRegistry import CURVE_REGISTRY_ABI
 from y.networks import Network
+from y.utils import a_sync_ttl_cache
 from y.utils.events import ProcessedEvents
 from y.utils.multicall import \
     multicall_same_func_same_contract_different_inputs
 from y.utils.raw_calls import raw_call
 
 T = TypeVar('T')
 
@@ -117,41 +118,38 @@
     __slots__ = "identifiers", "_events", 
     def __init__(self, address: Address, asynchronous: bool = False):
         super().__init__(address, asynchronous=asynchronous)
         self.identifiers = defaultdict(list)
         self._events = AddressProviderEvents(self)
     async def get_registry(self) -> EthAddress:
         contract = await Contract.coroutine(self.address)
-        return await contract.get_registry.coroutine()
+        return await contract.get_registry
     async def _load_factories(self) -> None:
         # factory events are quite useless, so we use a different method
         logger.debug("loading pools from metapool factories")
         # TODO: remove this once curve adds to address provider
         if chain.id == Network.Mainnet:
             self.identifiers[Ids.CurveStableswapFactoryNG] = ['0x6A8cbed756804B16E05E741eDaBd5cB544AE21bf']
-        metapool_factories = [
+
+        if metapool_factories := [
             Factory(factory, asynchronous=self.asynchronous)
             for i in [Ids.Metapool_Factory, Ids.crvUSD_Plain_Pools, Ids.Curve_Tricrypto_Factory, Ids.CurveStableswapFactoryNG]
             for factory in self.identifiers[i]
-        ]
-
-        metapool_factory_pools = await asyncio.gather(*[factory.read_pools(sync=False) for factory in metapool_factories])
-        for factory, pool_list in zip(metapool_factories, metapool_factory_pools):
-            for pool in pool_list:
-                # for metpool factories pool is the same as lp token
-                curve.token_to_pool[pool] = pool
-                curve.factories[factory].add(pool)
+        ]:
+            async for factory, pool_list in a_sync.map(Factory.read_pools, metapool_factories):
+                for pool in pool_list:
+                    # for metpool factories pool is the same as lp token
+                    curve.token_to_pool[pool] = pool
+                    curve.factories[factory].add(pool)
 
         # if there are factories that haven't yet been added to the on-chain address provider,
         # please refer to commit 3f70c4246615017d87602e03272b3ed18d594d3c to see how to add them manually
-        logger.debug("loading pools from cryptopool factories")
-        await asyncio.gather(*[
-            Factory(factory, asynchronous=self.asynchronous) 
-            for factory in self.identifiers[Ids.CryptoPool_Factory] + self.identifiers[Ids.Cryptopool_Factory]
-        ])
+        if identifiers := self.identifiers[Ids.CryptoPool_Factory] + self.identifiers[Ids.Cryptopool_Factory]:
+            logger.debug("loading pools from cryptopool factories")
+            await a_sync.map(Factory, identifiers, asynchronous=self.asynchronous)
 
         if not curve._done.is_set():
             logger.info('loaded %s pools from %s registries and %s factories', len(curve.token_to_pool), len(curve.registries), len(curve.factories))
             curve._done.set()
 
 class Registry(_CurveEventsLoader):
     __slots__ = "_events"
@@ -172,15 +170,16 @@
             await Contract.coroutine(self.address)
         except ContractNotVerified:
             if chain.id == Network.xDai:
                 Contract.from_abi("Vyper_contract", self.address, CURVE_REGISTRY_ABI)
             else:
                 # This happens sometimes, not sure why as the contract is verified.
                 brownie.Contract.from_explorer(self.address)
-        return await asyncio.gather(*[self.get_pool(i) for i in range(await self.pool_count())])
+        pool_count = await self.pool_count()
+        return await a_sync.map(self.get_pool, range(pool_count)).values()
     async def _load(self) -> None:
         pool_list = await self.read_pools(sync=False)
         await asyncio.gather(*[self._load_pool(pool) for pool in pool_list if pool not in curve.factories[self.address]])
         logger.debug("loaded %s pools for %s", len(pool_list), self)
         self._loaded.set()
     async def _load_pool(self, pool: Address) -> None:
         factory = await Contract.coroutine(self.address)
@@ -230,14 +229,15 @@
     @a_sync.a_sync(ram_cache_maxsize=256)
     async def get_coin_index(self, coin: AnyAddressType) -> int:
         return [i for i, _coin in enumerate(await self.__coins__) if _coin == coin][0]
     
     @a_sync.aka.cached_property
     async def num_coins(self) -> int:
         return len(await self.__coins__)
+    __num_coins__: HiddenMethodDescriptor[Self, int]
     
     async def get_dy(
         self, 
         coin_ix_in: int, 
         coin_ix_out: int, 
         block: Optional[Block] = None, 
         ignore_pools: Tuple[Pool, ...] = (),
@@ -260,16 +260,15 @@
     async def coins_decimals(self) -> List[int]:
         factory = await self.__factory__
         source = factory or await curve.registry
         coins_decimals = await source.get_decimals.coroutine(self.address)
 
         # pool not in registry
         if not any(coins_decimals):
-            coins = await self.__coins__
-            coins_decimals = await asyncio.gather(*[coin.__decimals__ for coin in coins])
+            coins_decimals = await a_sync.map(ERC20.decimals, await self.__coins__).values()
         
         return [dec for dec in coins_decimals if dec != 0]
     __coins_decimals__: HiddenMethodDescriptor[Self, List[int]]
 
     @a_sync.aka.cached_property
     async def get_underlying_coins(self) -> List[ERC20]:    
         factory = await self.__factory__    
@@ -287,45 +286,35 @@
         if set(coins) == {ZERO_ADDRESS}:
             return await self.__coins__
 
         return [ERC20(coin, asynchronous=self.asynchronous) for coin in coins if coin != ZERO_ADDRESS]
     __get_underlying_coins__: HiddenMethodDescriptor[Self, List[ERC20]]
     
     @a_sync.a_sync(ram_cache_maxsize=1000)
-    async def get_balances(self, block: Optional[Block] = None) -> Dict[ERC20, Decimal]:
+    async def get_balances(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> List[WeiBalance]:
         """
         Get {token: balance} of liquidity in the pool.
         """
-
-        # TODO figure out why these can't be gathered.
-        # Sometimes `self.coins` is a list not a coroutine?
-        #coins, decimals = await gather([
-        #    self.__coins__,
-        #    self.__coins_decimals__,
-        #])
-
         coins = await self.__coins__
-        decimals = await self.__coins_decimals__
-
         try:
             factory = await self.__factory__
             source = factory or await curve.__registry__
             balances = await source.get_balances.coroutine(self.address, block_identifier=block)
-        # fallback for historical queries where registry was not yet deployed
         except ValueError:
-            balances = await asyncio.gather(*[self._get_balance(i, block) for i, _ in enumerate(coins)])
+            # fallback for historical queries where registry was not yet deployed
+            balances = await a_sync.map(self._get_balance, range(len(coins)), block=block).values()
 
         if not any(balances):
             raise ValueError(f'could not fetch balances {self.__str__()} at {block}')
 
-        return {
-            coin: Decimal(balance / 10 ** dec)
-            for coin, balance, dec in zip(coins, balances, decimals)
+        return [
+            WeiBalance(balance, coin, block, skip_cache=skip_cache) 
+            for coin, balance in zip(coins, balances) 
             if coin != ZERO_ADDRESS
-        }
+        ]
     
     async def _get_balance(self, i: int, block: Optional[Block] = None) -> Optional[int]:
         try:
             contract = await Contract.coroutine(self.address)
         except ContractNotVerified:
             # TODO: figure out if we need to build this, usually they get verified quickly 
             return None
@@ -337,44 +326,29 @@
             raise
 
     async def get_tvl(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[UsdValue]:
         """
         Get total value in Curve pool.
         """
         try:
-            balances = await self.get_balances(block=block, sync=False)
+            balances = await self.get_balances(block=block, skip_cache=skip_cache, sync=False)
         except ValueError as e:
             if str(e).startswith("could not fetch balances "):
                 return None
             raise e
-        
-        prices = await asyncio.gather(*[coin.price(block=block, skip_cache=skip_cache, sync=False) for coin in balances])
-
-        return UsdValue(
-            sum(balance * Decimal(price) for balance, price in zip(balances.values(), prices))
-        )
+        return UsdValue(await WeiBalance.value_usd.sum(balances, sync=False))
     
     @a_sync.a_sync(ram_cache_maxsize=100_000, ram_cache_ttl=60*60)
-    async def check_liquidity(self, token: Address, block: Block) -> Optional[int]:
-        deploy_block = await contract_creation_block_async(self.address)
-        if block < deploy_block:
+    async def check_liquidity(self, token: Address, block: Block) -> int:
+        if block < await contract_creation_block_async(self.address):
             return 0
-        i = await self.get_coin_index(token, sync=False)
-        return await self._get_balance(i, block)
-    
-    #@cached_property
-    #def oracle(self) -> Optional[Address]:
-    #    '''
-    #    If `pool` has method `price_oracle`, returns price_oracle address.
-    #    Else, returns `None`.
-    #    '''
-    #    response = raw_call(self.address, 'price_oracle()', output='address', return_None_on_failure=True)
-    #    if response == ZERO_ADDRESS:
-    #        return None
-    #    return response
+        index = await self.get_coin_index(token, sync=False)
+        if balance := await self._get_balance(index, block):
+            return balance
+        return 0
 
 
 
 class CurveRegistry(a_sync.ASyncGenericSingleton):
     __slots__ = "__task", 
     def __init__(self, asynchronous: bool = False) -> None:
         super().__init__()
@@ -422,15 +396,15 @@
                 for factory, factory_pools in self.factories.items()
                 if str(pool) in factory_pools
             )
             return await Contract.coroutine(factory)
         except StopIteration:
             return None    
     
-    @a_sync.a_sync(cache_type='memory')
+    @a_sync_ttl_cache
     async def get_price(self, token: Address, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> Optional[float]:
         pool = await self.get_pool(token, sync=False)
         if pool is None:
             return None
         tvl = await pool.get_tvl(block=block, skip_cache=skip_cache, sync=False)
         if tvl is None:
             return None
@@ -452,41 +426,41 @@
         self, 
         token_in: Address, 
         block: Optional[Block] = None, 
         ignore_pools: Tuple[Pool, ...] = (),
         skip_cache: bool = ENVS.SKIP_CACHE,
     ) -> Optional[UsdPrice]:
         try:
-            pools: List[CurvePool] = (await self.__coin_to_pools__)[token_in]
+            pools = (await self.__coin_to_pools__)[token_in]
         except KeyError:
             return None
         
         pools = [pool for pool in pools if pool not in ignore_pools]
 
         if block is not None:
-            deploy_blocks = await asyncio.gather(*[contract_creation_block_async(pool.address, True) for pool in pools])
-            pools = [pool for pool, deploy_block in zip(pools, deploy_blocks) if deploy_block <= block]
+            pools = [pool async for pool, deploy_block in a_sync.map(contract_creation_block_async, pools).map() if deploy_block <= block]
 
+        if not pools:
+            return None
         # Choose a pool to use for pricing `token_in`.
-        if len(pools) == 1:
+        elif len(pools) == 1:
             pool = pools[0]
         else:
             # Use the pool with deepest liquidity.
-            balances = await asyncio.gather(*[pool.check_liquidity(token_in, block=block, sync=False) for pool in pools], return_exceptions=True)
             deepest_pool, deepest_bal = None, 0
-            for pool, depth in zip(pools, balances):
+            async for pool, depth in CurvePool.check_liquidity.map(pools, token=token_in, block=block).map():
                 if depth > deepest_bal:
                     deepest_pool = pool
                     deepest_bal = depth
             pool = deepest_pool
 
         if pool is None:
             return None
 
-        if len(coins := await pool.__coins__) != 2:
+        if len(await pool.__coins__) != 2:
             # TODO: handle this sitch if necessary
             return
 
         # Get the price for `token_in` using the selected pool.
         # this works for most typical metapools
 
         token_in_ix = await pool.get_coin_index(token_in, sync=False)
@@ -509,25 +483,16 @@
         for pool in pools:
             for coin in await pool.__coins__:
                 mapping[coin].add(pool)
         return {coin: list(pools) for coin, pools in mapping.items()}
     __coin_to_pools__: HiddenMethodDescriptor[Self, Dict[str, List[CurvePool]]]
     
     async def check_liquidity(self, token: Address, block: Block, ignore_pools: Tuple[Pool, ...]) -> int:
-        pools: List[CurvePool] = await self.__coin_to_pools__
-        if token not in pools:
-            return 0
-        if pools := [pool for pool in pools[token] if pool not in ignore_pools]:
-            liqs = [
-                liq for liq
-                in await asyncio.gather(*[pool.check_liquidity(token, block, sync=False) for pool in pools])
-                if liq
-            ]
-            if liqs:
-                return max(liqs)
+        if pools := [pool for pool in (await self.__coin_to_pools__).get(token, []) if pool not in ignore_pools]:
+            return await CurvePool.check_liquidity.max(pools, token=token, block=block, sync=False)
         return 0
     
     @cached_property
     def _done(self) -> a_sync.Event:
         """A helper function to ensure the Event is attached to the correct loop."""
         self._task
         return a_sync.Event(name="curve")
@@ -549,19 +514,16 @@
         await self.address_provider
         logger.debug("curve address provider events loaded, now loading factories and pools")
         # NOTE: Gnosis chain's address provider fails to provide registry via events. Maybe other chains as well.
         if not self.identifiers[Ids.Main_Registry] and (registry := await self.address_provider.get_registry()) != ZERO_ADDRESS:
             self.identifiers[Ids.Main_Registry] = [registry]
         while True:
             # Check if any registries were updated, then ensure all old and new are loaded
-            await asyncio.gather(*[
-                Registry(self.identifiers[i][-1], self, asynchronous=self.asynchronous)
-                for i in [Ids.Main_Registry, Ids.CryptoSwap_Registry]
-                if self.identifiers[i]
-            ])
+            if registries := [self.identifiers[i][-1] for i in [Ids.Main_Registry, Ids.CryptoSwap_Registry] if self.identifiers[i]]:
+                await a_sync.map(Registry, registries, curve=self, asynchronous=self.asynchronous)
             # load metapool and curve v5 factories
             await self.address_provider._load_factories()
             await asyncio.sleep(600)
    
 try: 
     curve: CurveRegistry = CurveRegistry(asynchronous=True)
 except UnsupportedNetwork:
```

### Comparing `ypricemagic-3.4.9/y/prices/stable_swap/ellipsis.py` & `ypricemagic-3.5.0/y/prices/stable_swap/ellipsis.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from y.contracts import Contract, has_methods
 from y.datatypes import AddressOrContract, AnyAddressType, Block, UsdPrice
 from y.utils.raw_calls import raw_call
 
 logger = logging.getLogger(__name__)
 
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=5*60)
 async def is_eps_rewards_pool(token_address: AnyAddressType) -> bool:
     return await has_methods(token_address, ('lpStaker()(address)','rewardTokens(uint)(address)','rewardPerToken(address)(uint)','minter()(address)'), sync=False)
 
 @a_sync.a_sync(default='sync')
 async def get_price(token_address: AddressOrContract, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
     minter = await raw_call(token_address,'minter()',output='address', block=block, sync=False)
     minter = await Contract.coroutine(minter)
@@ -32,13 +32,12 @@
                 minter.balances.coroutine(i, block_identifier = block),
             )
             balance /= await ERC20(coin, asynchronous=True).scale
             balances.append(WeiBalance(balance, coin, block, skip_cache=skip_cache))
             i += 1
         except:
             break
-    coin_values, total_supply = await asyncio.gather(
-        asyncio.gather(*[b.__value_usd__ for b in balances]),
+    tvl, total_supply = await asyncio.gather(
+        WeiBalance.value_usd.sum(balances, sync=False),
         ERC20(token_address, asynchronous=True).total_supply_readable(block),
     )
-    tvl = sum(coin_values)
     return UsdPrice(tvl / Decimal(total_supply))
```

### Comparing `ypricemagic-3.4.9/y/prices/stable_swap/froyo.py` & `ypricemagic-3.5.0/y/prices/stable_swap/froyo.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from y import convert
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.networks import Network
 from y.utils.raw_calls import raw_call
 
 logger = logging.getLogger(__name__)
 
+POOL = '0x83E5f18Da720119fF363cF63417628eB0e9fd523'
+
 def is_froyo(token: AnyAddressType) -> bool:
     address = convert.to_address(token)
     return chain.id == Network.Fantom and address == '0x4f85Bbf3B0265DCEd4Ec72ebD0358ccCf190F1B3'
 
 @a_sync.a_sync(default='sync')
 async def get_price(token: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
-    pool = '0x83E5f18Da720119fF363cF63417628eB0e9fd523'
-    if not token == pool:
+    if not token == POOL:
         return None
-    virtual_price = await raw_call(pool, "get_virtual_price()", block=block, output='int', sync=False)
+    virtual_price = await raw_call(POOL, "get_virtual_price()", block=block, output='int', sync=False)
     return UsdPrice(virtual_price / 1e18)
```

### Comparing `ypricemagic-3.4.9/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-3.5.0/y/prices/stable_swap/mstablefeederpool.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from y.contracts import Contract, has_methods
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.prices import magic
 
 logger = logging.getLogger(__name__)
 
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=5*60)
 async def is_mstable_feeder_pool(address: AnyAddressType) -> bool:
-    return await has_methods(address, ('getPrice()((uint,uint))','mAsset()(address)'), sync=False)
+    return await has_methods(address, ('getPrice()((uint,uint))', 'mAsset()(address)'), sync=False)
 
 @a_sync.a_sync(default='sync')
 async def get_price(token: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
     address = convert.to_address(token)
     contract = await Contract.coroutine(address)
     ratio, masset, scale = await asyncio.gather(
         contract.getPrice.coroutine(block_identifier=block),
```

### Comparing `ypricemagic-3.4.9/y/prices/stable_swap/saddle.py` & `ypricemagic-3.5.0/y/prices/stable_swap/saddle.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from y.prices import magic
 from y.utils.multicall import \
     multicall_same_func_same_contract_different_inputs
 
 logger = logging.getLogger(__name__)
 
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=5*60)
 async def is_saddle_lp(token_address: AnyAddressType) -> bool:
     pool = await get_pool(token_address, sync=False)
     if pool:
         return await has_methods(pool, ('getVirtualPrice()(uint)', 'getA()(uint)','getAPrecise()(uint)'), sync=False)
 
 @a_sync.a_sync(default='sync', ram_cache_ttl=ENVS.CACHE_TTL)
 async def get_pool(token_address: AnyAddressType) -> Address:
@@ -53,20 +53,19 @@
     pool, tokens, balances = await asyncio.gather(
         get_pool(token_address, sync=False),
         get_tokens(token_address, block, sync=False),
         multicall_same_func_same_contract_different_inputs(
             pool, 'getTokenBalance(uint8)(uint)', inputs=[*range(len(tokens))], sync=False
         ),
     )
-    tokens_scale, prices = await asyncio.gather(
-        asyncio.gather(*[token.__scale__ for token in tokens]),
+    scales, prices = await a_sync.gather(
+        ERC20.scale.map(tokens).values(),
         magic.get_prices(tokens, block, skip_cache=skip_cache, silent=True, sync=False),
     )
-    balances = [balance / scale for balance, scale in zip(balances, tokens_scale)]
-    return UsdValue(sum(balance * price for balance, price in zip (balances, prices)))
+    return UsdValue(sum(balance / scale * price for balance, scale, price in zip(balances, scales, prices)))
 
 @a_sync.a_sync(default='sync')
 async def get_tokens(token_address: AnyAddressType, block: Optional[Block] = None) -> List[ERC20]:
     pool, response = await asyncio.gather(
         get_pool(token_address, sync=False),
         multicall_same_func_same_contract_different_inputs(
             pool, 'getToken(uint8)(address)', inputs=[*range(8)], block=block, return_None_on_failure=True, sync=False
```

### Comparing `ypricemagic-3.4.9/y/prices/synthetix.py` & `ypricemagic-3.5.0/y/prices/synthetix.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from y import convert
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y.contracts import Contract, has_method
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.exceptions import UnsupportedNetwork, call_reverted
 from y.networks import Network
+from y.utils import a_sync_ttl_cache
 
 try:
     from eth_abi import encode
     encode_bytes: Callable[[str], bytes] = lambda s: encode(["bytes32"], [s.encode()])
 except ImportError:
     from eth_abi import encode_single
     encode_bytes: Callable[[str], bytes] = lambda s: encode_single("bytes32", s.encode())
@@ -46,27 +47,25 @@
     @a_sync.a_sync(ram_cache_maxsize=256)
     async def get_address(self, name: str, block: Block = None) -> Contract:
         """
         Get contract from Synthetix registry.
         See also https://docs.synthetix.io/addresses/
         """
         address_resolver = await self.__address_resolver__
-        key = encode_bytes(name)
-        address = await address_resolver.getAddress.coroutine(key, block_identifier=block)
+        address = await address_resolver.getAddress.coroutine(encode_bytes(name), block_identifier=block)
         proxy = await Contract.coroutine(address)
         return await Contract.coroutine(await proxy.target.coroutine(block_identifier=block)) if hasattr(proxy, 'target') else proxy
 
     @a_sync.aka.cached_property
     async def synths(self) -> List[EthAddress]:
         """
         Get target addresses of all synths.
         """
         proxy_erc20 = await self.get_address('ProxyERC20', sync=False)
-        synth_count = await proxy_erc20.availableSynthCount.coroutine()
-        synths = await asyncio.gather(*[proxy_erc20.availableSynths.coroutine(i) for i in range(synth_count)])
+        synths = await proxy_erc20.availableSynths.map(range(await proxy_erc20.availableSynthCount))
         logger.info('loaded %s synths', len(synths))
         return synths
         
     async def is_synth(self, token: AnyAddressType) -> bool:
         """returns `True` if a `token` is a synth, `False` if not"""
         token = convert.to_address(token)
         try:
@@ -77,15 +76,15 @@
                 return target in await synthetix.synths and await Call(target, 'proxy()(address)') == token
             return False
         except Exception as e:
             if "invalid jump destination" in str(e):
                 return False
             raise e
     
-    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
+    @a_sync_ttl_cache
     async def get_currency_key(self, token: AnyAddressType) -> Optional[HexString]:
         target = await Call(token, ['target()(address)']) if await has_method(token, 'target()(address)', sync=False) else token
         return await Call(target, ['currencyKey()(bytes32)']) if await has_method(token, 'currencyKey()(bytes32)', sync=False) else None
     
     async def get_price(self, token: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
         """
         Get a price of a synth in dollars.
```

### Comparing `ypricemagic-3.4.9/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-3.5.0/y/prices/tokenized_fund/basketdao.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,16 +20,10 @@
 
 @a_sync.a_sync(default='sync')
 async def get_price(address: EthAddress, block: Optional[Block] = None) -> UsdPrice:
     balances, total_supply = await asyncio.gather(
         Call(address, 'getAssetsAndBalances()(address[],uint[])',block_id=block),
         ERC20(address, asynchronous=True).total_supply_readable(block=block),
     )
-
-    balances = [
-        WeiBalance(balance, token, block)
-        for token, balance
-        in zip(balances[0],balances[1])
-    ]
-
-    tvl = sum(await asyncio.gather(*[bal.__value_usd__ for bal in balances]))
+    balances = (WeiBalance(balance, token, block) for token, balance in zip(balances[0], balances[1]))
+    tvl = await WeiBalance.value_usd.sum(balances, sync=False)
     return UsdPrice(tvl / Decimal(total_supply))
```

### Comparing `ypricemagic-3.4.9/y/prices/tokenized_fund/gelato.py` & `ypricemagic-3.5.0/y/prices/tokenized_fund/gelato.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from y.classes.common import ERC20
 from y.contracts import has_methods
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.utils.raw_calls import raw_call
 
 logger = logging.getLogger(__name__)
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=5*60)
 async def is_gelato_pool(token_address: AnyAddressType) -> bool:
     return await has_methods(token_address, ('gelatoBalance0()(uint)','gelatoBalance1()(uint)'), sync=False)
 
 @a_sync.a_sync(default='sync')
 async def get_price(token: AnyAddressType, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
     address = convert.to_address(token)
```

### Comparing `ypricemagic-3.4.9/y/prices/tokenized_fund/piedao.py` & `ypricemagic-3.5.0/y/prices/tokenized_fund/piedao.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+from decimal import Decimal
 from typing import List, Optional
 
 import a_sync
 from brownie import ZERO_ADDRESS
 from multicall import Call
 
 from y import ENVIRONMENT_VARIABLES as ENVS
@@ -41,16 +42,16 @@
         if not call_reverted(e):
             raise
         return pie_address
 
 async def get_tvl(pie_address: Address, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdValue:
     tokens: List[ERC20]
     pool, tokens = await asyncio.gather(get_bpool(pie_address, block), get_tokens(pie_address, block))
-    token_balances, token_scales, prices = await asyncio.gather(
-        asyncio.gather(*[Call(token.address, ['balanceOf(address)(uint)', pool], block_id=block) for token in tokens]),
-        asyncio.gather(*[token.__scale__ for token in tokens]),
-        magic.get_prices(tokens, block, skip_cache=skip_cache, sync=False),
-    )
-    token_balances = [bal / scale for bal, scale in zip(token_balances, token_scales)]
-    return UsdValue(
-        sum(bal * price for bal, price in zip(token_balances, prices))
-    )
+    return await a_sync.map(get_value, tokens, bpool=pool, block=block, skip_cache=skip_cache).sum(pop=True, sync=False)
+
+async def get_balance(bpool: Address, token: ERC20, block: Optional[Block] = None) -> Decimal:
+    balance, scale = await asyncio.gather(Call(token.address, ['balanceOf(address)(uint)', bpool], block_id=block), token.__scale__)
+    return Decimal(balance) / scale
+
+async def get_value(bpool: Address, token: ERC20, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdValue:
+    balance, price = await asyncio.gather(get_balance(bpool, token, block), token.price(block, skip_cache=skip_cache, sync=False))
+    return UsdValue(balance * Decimal(price))
```

### Comparing `ypricemagic-3.4.9/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-3.5.0/y/prices/tokenized_fund/tokensets.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from y.classes.common import ERC20, WeiBalance
 from y.contracts import Contract, has_methods
 from y.datatypes import AnyAddressType, Block, UsdPrice
 
 logger = logging.getLogger(__name__)
 
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=5*60)
 async def is_token_set(token: AnyAddressType) -> bool:
     return any(await asyncio.gather(
         has_methods(token, ("getComponents()(address[])", "naturalUnit()(uint)"), sync=False),
         has_methods(token, ("getComponents()(address[])", "getModules()(address[])", "getPositions()(address[])"), sync=False),
     ))
 
 @a_sync.a_sync(default='sync')
@@ -35,41 +35,41 @@
     @a_sync.a_sync(ram_cache_maxsize=100)
     async def components(self, block: Optional[Block] = None) -> List[ERC20]:
         contract = await Contract.coroutine(self.address)
         components = await contract.getComponents.coroutine(block_identifier = block)
         return [ERC20(component, asynchronous=self.asynchronous) for component in components]
     
     async def balances(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> List[WeiBalance]:
-        contract = await Contract.coroutine(self.address)
+        contract, components = await asyncio.gather(
+            Contract.coroutine(self.address),
+            self.components(block=block, sync=False),
+        )
         if hasattr(contract, 'getUnits'):
             balances = await contract.getUnits.coroutine(block_identifier = block)
             logger.debug("getUnits: %s", balances)
         elif hasattr(contract, 'getTotalComponentRealUnits'):
-            balances = await asyncio.gather(*[
-                self.get_total_component_real_units.coroutine((component.address, ), block_id=block)
-                for component in await self.components(block, sync=False)
-            ])
+            _components = ((component.address, ) for component in components)
+            balances = await a_sync.map(self.get_total_component_real_units.coroutine, _components, block_id=block).values()
             logger.debug("getTotalComponentRealUnits: %s", balances)
-        balances = [WeiBalance(balance, component, block=block, skip_cache=skip_cache) for component, balance in zip(await self.components(block=block, sync=False), balances)]
+        balances = [WeiBalance(balance, component, block=block, skip_cache=skip_cache) for component, balance in zip(components, balances)]
         return balances
     
     async def get_price(self, block: Optional[Block] = None, skip_cache: bool = ENVS.SKIP_CACHE) -> UsdPrice:
         total_supply = Decimal(await self.total_supply_readable(block=block, sync=False))
         if total_supply == 0:
             logger.debug("total supply is 0, forcing price to $0")
             return UsdPrice(0)
         contract = await Contract.coroutine(self.address)
         if hasattr(contract, "getUnits"):
             balances: List[WeiBalance] = await self.balances(block=block, skip_cache=skip_cache, sync=False)
-            values = await asyncio.gather(*[balance.__value_usd__ for balance in balances])
+            values = await WeiBalance.value_usd.map(balances).values()
             logger.debug("balances: %s  values: %s", balances, values)
             tvl = sum(values)
             price = UsdPrice(tvl / total_supply)
             logger.debug("total supply: %s  tvl: %s  price: %s", total_supply, tvl, price)
             return price
         elif hasattr(contract, "getTotalComponentRealUnits"):
             balances_per_token: List[WeiBalance] = await self.balances(block=block, sync=False)
-            values_per_token = await asyncio.gather(*[balance.__value_usd__ for balance in balances_per_token])
-            price = UsdPrice(sum(values_per_token))
-            logger.debug("balances per token: %s  values per token: %s  price: %s", balances_per_token, values_per_token, price)
+            price = UsdPrice(await WeiBalance.value_usd.sum(balances_per_token, sync=False))
+            logger.debug("balances per token: %s  price: %s", balances_per_token, price)
             return price
         raise NotImplementedError
```

### Comparing `ypricemagic-3.4.9/y/prices/utils/buckets.py` & `ypricemagic-3.5.0/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/utils/sense_check.py` & `ypricemagic-3.5.0/y/prices/utils/sense_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # async: done
 
-import asyncio
 import logging
 from typing import Optional
 
+import a_sync
 from brownie import chain
 
 from y.classes.common import ERC20
 from y.constants import wbtc, weth
 from y.contracts import Contract
 from y.exceptions import NonStandardERC20
 from y.networks import Network
@@ -204,23 +204,23 @@
 
     if bucket in ['uni or uni-like lp', 'balancer pool']:
         return True
 
     elif bucket == 'curve lp':
         underlyings = await CurvePool(token_address, asynchronous=True).coins
         if questionable_underlyings := [und for und in underlyings if und not in ACCEPTABLE_HIGH_PRICES]:
-            return all(await asyncio.gather(*[_exit_sense_check(underlying) for underlying in questionable_underlyings]))
+            return await a_sync.map(_exit_sense_check, questionable_underlyings).all(sync=False)
         return True
     
     elif bucket == 'atoken':
         underlying = await aave.underlying(token_address, sync=False)
     elif bucket == 'compound':
         underlying = await CToken(token_address, asynchronous=True).underlying
     elif bucket == 'solidex':
         contract = await Contract.coroutine(token_address)
-        underlying = await contract.pool.coroutine()
+        underlying = await contract.pool
     elif bucket == 'yearn or yearn-like':
         underlying = await YearnInspiredVault(token_address, asynchronous=True).underlying
     else:
         return False
 
     return underlying in ACCEPTABLE_HIGH_PRICES or await _exit_sense_check(underlying)
```

### Comparing `ypricemagic-3.4.9/y/prices/utils/ypriceapi.py` & `ypricemagic-3.5.0/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/prices/yearn.py` & `ypricemagic-3.5.0/y/prices/yearn.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 force_false = {
     Network.Mainnet: [
         "0x8751D4196027d4e6DA63716fA7786B5174F04C15",  # wibBTC
         "0xF0a93d4994B3d98Fb5e3A2F90dBc2d69073Cb86b",  # PWRD
     ],
 }.get(chain.id, [])
 
-@a_sync.a_sync(default='sync', cache_type='memory')
+@a_sync.a_sync(default='sync', cache_type='memory', ram_cache_ttl=30*60)
 async def is_yearn_vault(token: AnyAddressType) -> bool:
     # wibbtc returns True here even though it doesn't meet the criteria.
     # TODO figure out a better fix. For now I need a fix asap so this works.
     if chain.id == Network.Mainnet and str(token) == "0x8751D4196027d4e6DA63716fA7786B5174F04C15":
         return False
 
     # Yearn-like contracts can use these formats
@@ -87,21 +87,19 @@
     block: Optional[Block] = None,
     skip_cache: bool = ENVS.SKIP_CACHE,
     ignore_pools: Tuple[Pool, ...] = (),
 ) -> UsdPrice:
     return await YearnInspiredVault(token).price(block=block, skip_cache=skip_cache, ignore_pools=ignore_pools, sync=False)
 
 class YearnInspiredVault(ERC20):
-    __slots__ = "_get_share_price", 
+    # defaults are stored as class vars to keep instance dicts smaller
+    _get_share_price = None
     # v1 vaults use getPricePerFullShare scaled to 18 decimals
     # v2 vaults use pricePerShare scaled to underlying token decimals
     # yearnish clones use all sorts of other things, we gotchu covered
-    def __init__(self, address: AnyAddressType, asynchronous: bool = False):
-        super().__init__(address, asynchronous=asynchronous)
-        self._get_share_price = None
     
     @a_sync.aka.cached_property
     async def underlying(self) -> ERC20:
         # special cases
         if chain.id == Network.Arbitrum and self.address == '0x57c7E0D43C05bCe429ce030132Ca40F6FA5839d7':
             return ERC20(await raw_call(self.address, 'usdl()', output='address', sync=False), asynchronous=self.asynchronous)
 
@@ -139,23 +137,33 @@
 
         if share_price is None:
             # this is for element vaults and other 'scaled' share price functions. probe fails because method requires input
             try:
                 contract = await Contract.coroutine(self.address)
                 for method in ['convertToAssets', 'getSharesToUnderlying']:
                     if hasattr(contract, method):
-                        share_price = await getattr(contract, method).coroutine(await self.__scale__, block_identifier=block)
+                        contract_call = getattr(contract, method)
+                        scale = await self.__scale__
+                        class call:
+                            # a hacky way we can cache this weird case and save calls
+                            function = method
+                            @staticmethod
+                            async def coroutine(block_id: Optional[Block]) -> int:
+                                return await contract_call.coroutine(scale, block_identifier=block_id)
+                        share_price = await call.coroutine(block_id=block)
+                        self._get_share_price = call
+
             except ContractNotVerified:
                 pass
 
         if share_price is not None:
             if self._get_share_price and self._get_share_price.function == 'getPricePerFullShare()(uint)':
                 # v1 vaults use getPricePerFullShare scaled to 18 decimals
                 return share_price / Decimal(10 ** 18)
-            underlying: ERC20 = await self.__underlying__
+            underlying = await self.__underlying__
             return Decimal(share_price) / await underlying.__scale__
             
         elif await raw_call(self.address, 'totalSupply()', output='int', block=block, return_None_on_failure=True, sync=False) == 0:
             return None
         
         else:
             raise CantFetchParam(f'share_price for {self}')
```

### Comparing `ypricemagic-3.4.9/y/time.py` & `ypricemagic-3.5.0/y/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import asyncio
 import datetime
 import logging
 import time
 from typing import Union
 
 import a_sync
@@ -15,15 +16,15 @@
     from dank_mids.ENVIRONMENT_VARIABLES import GANACHE_FORK
 except ImportError:
     from dank_mids._config import GANACHE_FORK
 
 from y import ENVIRONMENT_VARIABLES as ENVS
 from y.exceptions import NoBlockFound, NodeNotSynced
 from y.networks import Network
-from y.utils.cache import memory
+from y.utils.cache import a_sync_ttl_cache, memory
 from y.utils.client import get_ethereum_client, get_ethereum_client_async
 from y.utils.logging import yLazyLogger
 
 logger = logging.getLogger(__name__)
 
 @memory.cache()
 @yLazyLogger(logger)
@@ -36,15 +37,15 @@
     if client not in ['tg', 'erigon']:
         return chain[height].timestamp
     header = web3.manager.request_blocking(f"{client}_getHeaderByNumber", [height])
     ts = int(header.timestamp, 16)
     db.set_block_timestamp(height, ts, sync=True)
     return ts
 
-@a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
+@a_sync_ttl_cache
 @eth_retry.auto_retry
 async def get_block_timestamp_async(height: int) -> int:
     import y._db.utils.utils as db
     if ts := await db.get_block_timestamp(height, sync=False):
         return ts
     client = await get_ethereum_client_async()
     if client in ['tg', 'erigon']:
@@ -82,15 +83,15 @@
             lo = mid
     hi = hi - 1
     block = hi if hi != height else None
     logger.debug('last %s block on date %s -> %s', Network.name(), date, block)
     return block
 
 
-@a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
+@a_sync_ttl_cache
 async def get_block_at_timestamp(timestamp: datetime.datetime) -> int:
     import y._db.utils.utils as db
     if block_at_timestamp := await db.get_block_at_timestamp(timestamp):
         return block_at_timestamp
     
     # TODO: invert this and use this fn inside of closest_block_after_timestamp for backwards compatability before deprecating closest_block_after_timestamp
     block_after_timestamp = await closest_block_after_timestamp_async(timestamp)
@@ -120,15 +121,15 @@
         except NoBlockFound:
             time.sleep(.2)
     check_node()
     block = _closest_block_after_timestamp_cached(timestamp)
     logger.debug('closest %s block after timestamp %s -> %s', Network.name(), timestamp, block)
     return block
 
-@a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
+@a_sync_ttl_cache
 async def closest_block_after_timestamp_async(timestamp: Timestamp, wait_for_block_if_needed: bool = False) -> int:
     timestamp = _parse_timestamp(timestamp)
     while wait_for_block_if_needed:
         try:
             return await get_block_at_timestamp(datetime.datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc), sync=False) + 1
         except NoBlockFound:
             await asyncio.sleep(0.2)
```

### Comparing `ypricemagic-3.4.9/y/utils/client.py` & `ypricemagic-3.5.0/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/utils/events.py` & `ypricemagic-3.5.0/y/utils/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     # NOTE: If you don't need the logs in order, you will get your logs faster if you set `chronological` to False.
 
     if from_block is None:
         from y.contracts import contract_creation_block_async
         if address is None:
             from_block = 0
         elif isinstance(address, Iterable) and not isinstance(address, str):
-            from_block = min(await asyncio.gather(*[contract_creation_block_async(addr, True) for addr in address]))
+            from_block = await _lowest_deploy_block(address, when_no_history_return_0=True)
         else:
             from_block = await contract_creation_block_async(address, True)
     if to_block is None:
         to_block = await dank_mids.eth.block_number
     elif run_forever:
         raise TypeError('`to_block` must be None if `run_forever` is True.')
     if from_block > to_block:
@@ -343,15 +343,15 @@
     @async_property
     async def _from_block(self) -> int:
         if self.from_block is None:
             from y.contracts import contract_creation_block_async
             if self.addresses is None:
                 self.from_block = 0
             elif isinstance(self.addresses, Iterable) and not isinstance(self.addresses, str):
-                self.from_block = min(await asyncio.gather(*[contract_creation_block_async(addr, when_no_history_return_0=True) for addr in self.addresses]))
+                self.from_block = await _lowest_deploy_block(self.addresses, when_no_history_return_0=True)
             else:
                 self.from_block = await contract_creation_block_async(self.addresses, when_no_history_return_0=True)
         return self.from_block
     
     async def _fetch_range(self, range_start: int, range_end: int) -> List[LogReceipt]:
         tries = 0
         while True:
@@ -386,8 +386,16 @@
     def _process_event(self, event: _EventItem) -> T:
         ...
     def objects(self, to_block: int) -> AsyncIterator[_EventItem]:
         return self._objects_thru(block=to_block)
     def _extend(self, logs: List[LogReceipt]) -> None:
         for event in decode_logs(logs):
             if self._include_event(event):
-                self._objects.append(self._process_event(event))
+                self._objects.append(self._process_event(event))
+
+async def _lowest_deploy_block(addresses: Iterable[EthAddress], when_no_history_return_0: bool) -> Block:
+    from y.contracts import contract_creation_block_async
+    return await a_sync.map(
+        contract_creation_block_async, 
+        addresses, 
+        when_no_history_return_0=when_no_history_return_0,
+    ).min(sync=False)
```

### Comparing `ypricemagic-3.4.9/y/utils/fakes.py` & `ypricemagic-3.5.0/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/utils/gather.py` & `ypricemagic-3.5.0/y/utils/gather.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/utils/logging.py` & `ypricemagic-3.5.0/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/utils/middleware.py` & `ypricemagic-3.5.0/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/y/utils/multicall.py` & `ypricemagic-3.5.0/y/utils/multicall.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,22 +90,28 @@
 @stuck_coro_debugger
 async def multicall_decimals(
     addresses: Iterable[AddressOrContract], 
     block: Optional[Block] = None,
     return_None_on_failure: bool = True
     ) -> List[int]:
 
+    addresses = [str(address) for address in addresses]
     try: 
-        return await asyncio.gather(*[Call(str(address), ['decimals()(uint256)'], block_id=block) for address in addresses])
+        calls = a_sync.map(Call, addresses, function=['decimals()(uint256)'], block_id=block)
+        return [decimals async for address, decimals in calls]
     except (CannotHandleRequest, InsufficientDataBytes):
         pass # TODO investigate these
     except Exception as e:
         continue_if_call_reverted(e)
 
-    return await asyncio.gather(*[_decimals(address,block=block,return_None_on_failure=return_None_on_failure) for address in addresses])
+    return [
+        decimals 
+        async for decimals 
+        in a_sync.map(_decimals, addresses, block=block, return_None_on_failure=return_None_on_failure).values()
+    ]
 
 @a_sync.a_sync(default='sync')
 @stuck_coro_debugger
 async def multicall_totalSupply(
     addresses: Iterable[AddressOrContract], 
     block: Optional[Block] = None,
     return_None_on_failure: bool = True
```

### Comparing `ypricemagic-3.4.9/y/utils/raw_calls.py` & `ypricemagic-3.5.0/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/ypricemagic/magic.py` & `ypricemagic-3.5.0/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-3.4.9/ypricemagic.egg-info/PKG-INFO` & `ypricemagic-3.5.0/ypricemagic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ypricemagic
-Version: 3.4.9
+Version: 3.5.0
 Summary: Use this tool to extract historical on-chain price data from an archive node. Shoutout to @bantg and @nymmrx for their awesome work on yearn-exporter that made this library possible.
 Home-page: https://github.com/BobTheBuidler/ypricemagic
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 License-File: LICENSE.txt
 Requires-Dist: bobs_lazy_logging==0.0.4
 Requires-Dist: cachetools<4.3,>=4.1.1
 Requires-Dist: checksum_dict>=1.1.1
-Requires-Dist: dank_mids>=4.20.86
+Requires-Dist: dank_mids>=4.20.88
 Requires-Dist: eth-brownie<1.21,>=1.19.3
 Requires-Dist: eth_retry<0.2,>=0.1.19
-Requires-Dist: ez-a-sync<0.20,>=0.18.2
+Requires-Dist: ez-a-sync<0.21,>=0.20.5
 Requires-Dist: inflection<0.6,>=0.1
 Requires-Dist: joblib>=1.0.1
 Requires-Dist: multicall>=0.8.2
 Requires-Dist: pony
```

### Comparing `ypricemagic-3.4.9/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-3.5.0/ypricemagic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .env.sample
 .gitignore
 CONTRIBUTING.md
 LICENSE.txt
 Makefile
 README.md
+brownie-config.yaml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/codeql-analysis.yml
 .github/workflows/deploy-docs.yml
 .github/workflows/pytest.yaml
```

