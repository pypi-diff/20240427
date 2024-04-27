# Comparing `tmp/agency-swarm-0.1.7.tar.gz` & `tmp/agency_swarm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-swarm-0.1.7.tar", last modified: Thu Apr 11 10:16:07 2024, max compression
+gzip compressed data, was "agency_swarm-0.2.0.tar", last modified: Fri Apr 26 15:16:45 2024, max compression
```

## Comparing `agency-swarm-0.1.7.tar` & `agency_swarm-0.2.0.tar`

### file list

```diff
@@ -1,188 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.317707 agency-swarm-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/agency_swarm/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/agency_swarm/agency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42253 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/agency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/agency_swarm/agency/genesis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisAgency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/manifesto.md
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/instructions.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/Devid/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/Devid.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ChangeFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/CommandExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileMover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ListDir.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/format_file_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23014 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/messages/message_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/threads/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/threads/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/threads/thread_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/BaseTool.py
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/ToolFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/tools/oai/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/oai/CodeInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/oai/Retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/oai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/user/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/user/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/util/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/cli/create_agent_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/cli/import_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/util/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/helpers/get_available_agent_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/helpers/list_available_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/agency_swarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/docs/advanced-usage/
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/agencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/agents.md
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/azure-openai.md
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/docs/introduction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/introduction/showcase.md
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/agency_async.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/azure.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/genesis_agency.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/web_browser_agent.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.321707 agency-swarm-0.1.7/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/data/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/csv-test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/generated_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-docx.docx
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-html.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-md.md
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-txt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/ga4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/get-headers-params.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/get-weather.json
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/data/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/tools/ExampleTool1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/demos/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/demos/demo_gradio.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/demos/streaming_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/demos/term_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/test_agency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/test_tool_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.852035 agency_swarm-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.820036 agency_swarm-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.828036 agency_swarm-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/.github/workflows/close-issues.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.828036 agency_swarm-0.2.0/agency_swarm/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.828036 agency_swarm-0.2.0/agency_swarm/agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46433 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/agency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.828036 agency_swarm-0.2.0/agency_swarm/agency/genesis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.828036 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisAgency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/manifesto.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agency/genesis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.832036 agency_swarm-0.2.0/agency_swarm/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.836036 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/instructions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.836036 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.836036 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.836036 agency_swarm-0.2.0/agency_swarm/agents/Devid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/Devid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/ChangeFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/CommandExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/FileMover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/FileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/FileWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/ListDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/util/format_file_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30562 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/messages/message_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/threads/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/threads/thread_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/BaseTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/ToolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/tools/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/oai/CodeInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/oai/FileSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/oai/Retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/tools/oai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.840036 agency_swarm-0.2.0/agency_swarm/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.844035 agency_swarm-0.2.0/agency_swarm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.844035 agency_swarm-0.2.0/agency_swarm/util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/cli/create_agent_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/cli/import_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.844035 agency_swarm-0.2.0/agency_swarm/util/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/helpers/get_available_agent_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/helpers/list_available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/agency_swarm/util/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/agency_swarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-04-26 15:16:45.000000 agency_swarm-0.2.0/agency_swarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-26 15:16:45.000000 agency_swarm-0.2.0/agency_swarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:16:45.000000 agency_swarm-0.2.0/agency_swarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 15:16:45.000000 agency_swarm-0.2.0/agency_swarm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 15:16:45.000000 agency_swarm-0.2.0/agency_swarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 15:16:45.000000 agency_swarm-0.2.0/agency_swarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.844035 agency_swarm-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.844035 agency_swarm-0.2.0/docs/advanced-usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/advanced-usage/agencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/advanced-usage/agents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/advanced-usage/azure-openai.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/advanced-usage/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.844035 agency_swarm-0.2.0/docs/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/introduction/showcase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    49298 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/notebooks/agency_async.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/notebooks/azure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/notebooks/genesis_agency.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/notebooks/web_browser_agent.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:16:45.852035 agency_swarm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.824036 agency_swarm-0.2.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/tests/data/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/csv-test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/generated_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/test-docx.docx
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/test-html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/test-md.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/test-pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/test-txt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/files/test-xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/schemas/ga4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/schemas/get-headers-params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/schemas/get-weather.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/schemas/relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/tests/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/data/tools/ExampleTool1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:16:45.848035 agency_swarm-0.2.0/tests/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/demos/demo_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/demos/streaming_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/demos/term_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/test_agency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-26 15:16:41.000000 agency_swarm-0.2.0/tests/test_tool_factory.py
```

### Comparing `agency-swarm-0.1.7/.github/workflows/docs.yml` & `agency_swarm-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/.github/workflows/publish.yml` & `agency_swarm-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/.github/workflows/test.yml` & `agency_swarm-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/.gitignore` & `agency_swarm-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/CONTRIBUTING.md` & `agency_swarm-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/LICENSE` & `agency_swarm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/PKG-INFO` & `agency_swarm-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.1.7
+Version: 0.2.0
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -30,16 +30,16 @@
 Project-URL: homepage, https://github.com/VRSEN/agency-swarm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.14.2
-Requires-Dist: instructor==0.6.7
+Requires-Dist: openai==1.23.3
+Requires-Dist: instructor==1.2.2
 Requires-Dist: deepdiff==6.7.1
 Requires-Dist: termcolor==2.3.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: rich==13.7.0
 Requires-Dist: jsonref==1.1.0
 
 # 🐝 Agency Swarm
@@ -120,36 +120,38 @@
     
     or convert from OpenAPI schemas:
     
     ```python
     from agency_swarm.tools import ToolFactory
     # using local file
     with open("schemas/your_schema.json") as f:
-        ToolFactory.from_openapi_schema(
+        tools = ToolFactory.from_openapi_schema(
             f.read(),
         )
     
     # using requests
-    ToolFactory.from_openapi_schema(
+    tools = ToolFactory.from_openapi_schema(
         requests.get("https://api.example.com/openapi.json").json(),
     )
     ```
 
-
 3. **Define Agent Roles**: Start by defining the roles of your agents. For example, a CEO agent for managing tasks and a developer agent for executing tasks.
 
     ```python
     from agency_swarm import Agent
     
     ceo = Agent(name="CEO",
                 description="Responsible for client communication, task planning and management.",
                 instructions="You must converse with other agents to ensure complete task execution.", # can be a file like ./instructions.md
                 files_folder="./files", # files to be uploaded to OpenAI
                 schemas_folder="./schemas", # OpenAPI schemas to be converted into tools
-                tools=[MyCustomTool, LangchainTool])
+                tools=[MyCustomTool], 
+                temperature=0.5, # temperature for the agent
+                max_prompt_tokens=25000, # max tokens in conversation history
+                )
     ```
 
     Import from existing agents:
 
    ```bash
    agency-swarm import-agent --name "Devid" --destination "./"
    ```
@@ -167,19 +169,23 @@
     from Developer import Developer
     from VirtualAssistant import VirtualAssistant
    
     dev = Developer()
     va = VirtualAssistant()
     
     agency = Agency([
-        ceo,  # CEO will be the entry point for communication with the user
-        [ceo, dev],  # CEO can initiate communication with Developer
-        [ceo, va],   # CEO can initiate communication with Virtual Assistant
-        [dev, va]    # Developer can initiate communication with Virtual Assistant
-    ], shared_instructions='agency_manifesto.md') # shared instructions for all agents
+           ceo,  # CEO will be the entry point for communication with the user
+           [ceo, dev],  # CEO can initiate communication with Developer
+           [ceo, va],   # CEO can initiate communication with Virtual Assistant
+           [dev, va]    # Developer can initiate communication with Virtual Assistant
+         ], 
+         shared_instructions='agency_manifesto.md', #shared instructions for all agents
+         temperature=0.5, # default temperature for all agents
+         max_prompt_tokens=25000 # default max tokens in conversation history
+    )
     ```
 
      In Agency Swarm, communication flows are directional, meaning they are established from left to right in the agency_chart definition. For instance, in the example above, the CEO can initiate a chat with the developer (dev), and the developer can respond in this chat. However, the developer cannot initiate a chat with the CEO. The developer can initiate a chat with the virtual assistant (va) and assign new tasks.
 
 5. **Run Demo**: 
 Run the demo to see your agents in action!
     
@@ -194,15 +200,15 @@
     ```python
     agency.run_demo()
     ```
     
     Backend version:
     
     ```python
-    completion_output = agency.get_completion("Please create a new website for our client.", yield_messages=False)
+    completion_output = agency.get_completion("Please create a new website for our client.")
     ```
 
 # CLI
 
 ## Genesis Agency
 
 The `genesis` command starts the genesis agency in your terminal to help you create new agencies and agents.
```

### Comparing `agency-swarm-0.1.7/README.md` & `agency_swarm-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,36 +76,38 @@
     
     or convert from OpenAPI schemas:
     
     ```python
     from agency_swarm.tools import ToolFactory
     # using local file
     with open("schemas/your_schema.json") as f:
-        ToolFactory.from_openapi_schema(
+        tools = ToolFactory.from_openapi_schema(
             f.read(),
         )
     
     # using requests
-    ToolFactory.from_openapi_schema(
+    tools = ToolFactory.from_openapi_schema(
         requests.get("https://api.example.com/openapi.json").json(),
     )
     ```
 
-
 3. **Define Agent Roles**: Start by defining the roles of your agents. For example, a CEO agent for managing tasks and a developer agent for executing tasks.
 
     ```python
     from agency_swarm import Agent
     
     ceo = Agent(name="CEO",
                 description="Responsible for client communication, task planning and management.",
                 instructions="You must converse with other agents to ensure complete task execution.", # can be a file like ./instructions.md
                 files_folder="./files", # files to be uploaded to OpenAI
                 schemas_folder="./schemas", # OpenAPI schemas to be converted into tools
-                tools=[MyCustomTool, LangchainTool])
+                tools=[MyCustomTool], 
+                temperature=0.5, # temperature for the agent
+                max_prompt_tokens=25000, # max tokens in conversation history
+                )
     ```
 
     Import from existing agents:
 
    ```bash
    agency-swarm import-agent --name "Devid" --destination "./"
    ```
@@ -123,19 +125,23 @@
     from Developer import Developer
     from VirtualAssistant import VirtualAssistant
    
     dev = Developer()
     va = VirtualAssistant()
     
     agency = Agency([
-        ceo,  # CEO will be the entry point for communication with the user
-        [ceo, dev],  # CEO can initiate communication with Developer
-        [ceo, va],   # CEO can initiate communication with Virtual Assistant
-        [dev, va]    # Developer can initiate communication with Virtual Assistant
-    ], shared_instructions='agency_manifesto.md') # shared instructions for all agents
+           ceo,  # CEO will be the entry point for communication with the user
+           [ceo, dev],  # CEO can initiate communication with Developer
+           [ceo, va],   # CEO can initiate communication with Virtual Assistant
+           [dev, va]    # Developer can initiate communication with Virtual Assistant
+         ], 
+         shared_instructions='agency_manifesto.md', #shared instructions for all agents
+         temperature=0.5, # default temperature for all agents
+         max_prompt_tokens=25000 # default max tokens in conversation history
+    )
     ```
 
      In Agency Swarm, communication flows are directional, meaning they are established from left to right in the agency_chart definition. For instance, in the example above, the CEO can initiate a chat with the developer (dev), and the developer can respond in this chat. However, the developer cannot initiate a chat with the CEO. The developer can initiate a chat with the virtual assistant (va) and assign new tasks.
 
 5. **Run Demo**: 
 Run the demo to see your agents in action!
     
@@ -150,15 +156,15 @@
     ```python
     agency.run_demo()
     ```
     
     Backend version:
     
     ```python
-    completion_output = agency.get_completion("Please create a new website for our client.", yield_messages=False)
+    completion_output = agency.get_completion("Please create a new website for our client.")
     ```
 
 # CLI
 
 ## Genesis Agency
 
 The `genesis` command starts the genesis agency in your terminal to help you create new agencies and agents.
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/agency.py` & `agency_swarm-0.2.0/agency_swarm/agency/agency.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import inspect
 import json
 import os
 import queue
 import threading
 import uuid
 from enum import Enum
-from typing import List, TypedDict, Callable, Any, Dict, Literal, Union
+from typing import List, TypedDict, Callable, Any, Dict, Literal, Union, Optional
 
+from openai.types.beta import AssistantToolChoice
 from openai.types.beta.threads import Message
+from openai.types.beta.threads.message import Attachment
 from openai.types.beta.threads.runs import RunStep
 from pydantic import Field, field_validator, model_validator
 from rich.console import Console
 from typing_extensions import override
 
 from agency_swarm.agents import Agent
 from agency_swarm.messages import MessageOutput
 from agency_swarm.messages.message_output import MessageOutputLive
 from agency_swarm.threads import Thread
-from agency_swarm.tools import BaseTool
+from agency_swarm.tools import BaseTool, FileSearch, CodeInterpreter
 from agency_swarm.user import User
 
 from agency_swarm.util.streaming import AgencyEventHandler
 
 console = Console()
 
 
@@ -43,26 +45,37 @@
     def __init__(self,
                  agency_chart: List,
                  shared_instructions: str = "",
                  shared_files: Union[str, List[str]] = None,
                  async_mode: Literal['threading'] = None,
                  settings_path: str = "./settings.json",
                  settings_callbacks: SettingsCallbacks = None,
-                 threads_callbacks: ThreadsCallbacks = None):
+                 threads_callbacks: ThreadsCallbacks = None,
+                 temperature: float = 0.3,
+                 top_p: float = 1.0,
+                 max_prompt_tokens: int = None,
+                 max_completion_tokens: int = None,
+                 truncation_strategy: dict = None,
+                 ):
         """
         Initializes the Agency object, setting up agents, threads, and core functionalities.
 
         Parameters:
             agency_chart: The structure defining the hierarchy and interaction of agents within the agency.
             shared_instructions (str, optional): A path to a file containing shared instructions for all agents. Defaults to an empty string.
             shared_files (Union[str, List[str]], optional): A path to a folder or a list of folders containing shared files for all agents. Defaults to None.
             async_mode (str, optional): The mode for asynchronous message processing. Defaults to None.
             settings_path (str, optional): The path to the settings file for the agency. Must be json. If file does not exist, it will be created. Defaults to None.
             settings_callbacks (SettingsCallbacks, optional): A dictionary containing functions to load and save settings for the agency. The keys must be "load" and "save". Both values must be defined. Defaults to None.
             threads_callbacks (ThreadsCallbacks, optional): A dictionary containing functions to load and save threads for the agency. The keys must be "load" and "save". Both values must be defined. Defaults to None.
+            temperature (float, optional): The temperature value to use for the agents. Agent specific values will override this. Defaults to 0.3.
+            top_p (float, optional): The top_p value to use for the agents. Agent specific values will override this. Defaults to None.
+            max_prompt_tokens (int, optional): The maximum number of tokens allowed in the prompt for each agent. Agent specific values will override this. Defaults to None.
+            max_completion_tokens (int, optional): The maximum number of tokens allowed in the completion for each agent. Agent specific values will override this. Defaults to None.
+            truncation_strategy (dict, optional): The truncation strategy to use for the completion for each agent. Agent specific values will override this. Defaults to None.
 
         This constructor initializes various components of the Agency, including CEO, agents, threads, and user interactions. It parses the agency chart to set up the organizational structure and initializes the messaging tools, agents, and threads necessary for the operation of the agency. Additionally, it prepares a main thread for user interactions.
         """
         self.async_mode = async_mode
         if self.async_mode == "threading":
             from agency_swarm.threads.thread_async import ThreadAsync
             self.ThreadType = ThreadAsync
@@ -74,84 +87,103 @@
         self.main_recipients = []
         self.main_thread = None
         self.recipient_agents = None  # for autocomplete
         self.shared_files = shared_files if shared_files else []
         self.settings_path = settings_path
         self.settings_callbacks = settings_callbacks
         self.threads_callbacks = threads_callbacks
+        self.temperature = temperature
+        self.top_p = top_p
+        self.max_prompt_tokens = max_prompt_tokens
+        self.max_completion_tokens = max_completion_tokens
+        self.truncation_strategy = truncation_strategy
 
         if os.path.isfile(os.path.join(self._get_class_folder_path(), shared_instructions)):
             self._read_instructions(os.path.join(self._get_class_folder_path(), shared_instructions))
         elif os.path.isfile(shared_instructions):
             self._read_instructions(shared_instructions)
         else:
             self.shared_instructions = shared_instructions
 
         self._parse_agency_chart(agency_chart)
         self._create_special_tools()
         self._init_agents()
         self._init_threads()
 
-    def get_completion(self, message: str, message_files=None, yield_messages=True, recipient_agent=None,
-                       additional_instructions=None):
+    def get_completion(self, message: str,
+                       message_files: List[str] = None,
+                       yield_messages: bool = False,
+                       recipient_agent: Agent = None,
+                       additional_instructions: str = None,
+                       attachments: List[dict] = None,
+                       tool_choice: dict = None,
+                       ):
         """
         Retrieves the completion for a given message from the main thread.
 
         Parameters:
             message (str): The message for which completion is to be retrieved.
-            message_files (list, optional): A list of file ids to be sent as attachments with the message. Defaults to None.
+            message_files (list, optional): A list of file ids to be sent as attachments with the message. When using this parameter, files will be assigned both to file_search and code_interpreter tools if available. It is recommended to assign files to the most sutiable tool manually, using the attachments parameter.  Defaults to None.
             yield_messages (bool, optional): Flag to determine if intermediate messages should be yielded. Defaults to True.
             recipient_agent (Agent, optional): The agent to which the message should be sent. Defaults to the first agent in the agency chart.
             additional_instructions (str, optional): Additional instructions to be sent with the message. Defaults to None.
+            attachments (List[dict], optional): A list of attachments to be sent with the message, following openai format. Defaults to None.
+            tool_choice (dict, optional): The tool choice for the recipient agent to use. Defaults to None.
+
         Returns:
             Generator or final response: Depending on the 'yield_messages' flag, this method returns either a generator yielding intermediate messages or the final response from the main thread.
         """
-        gen = self.main_thread.get_completion(message=message, message_files=message_files,
-                                              yield_messages=yield_messages, recipient_agent=recipient_agent,
-                                              additional_instructions=additional_instructions)
-
-        if not yield_messages:
-            while True:
-                try:
-                    next(gen)
-                except StopIteration as e:
-                    return e.value
+        if yield_messages:
+            print("Warning: yield_messages parameter is deprecated. Use streaming instead.")
 
-        return gen
-
-    def get_completion_stream(self, message: str, event_handler: type(AgencyEventHandler), message_files=None,
-                              recipient_agent=None, additional_instructions: str = None):
+        return self.main_thread.get_completion(message=message,
+                                               message_files=message_files,
+                                               attachments=attachments,
+                                               recipient_agent=recipient_agent,
+                                               additional_instructions=additional_instructions,
+                                               tool_choice=tool_choice)
+
+    def get_completion_stream(self,
+                              message: str,
+                              event_handler: type(AgencyEventHandler),
+                              message_files: List[str] = None,
+                              recipient_agent: Agent = None,
+                              additional_instructions: str = None,
+                              attachments: List[dict] = None,
+                              tool_choice: dict = None
+                              ):
         """
         Generates a stream of completions for a given message from the main thread.
 
         Parameters:
             message (str): The message for which completion is to be retrieved.
             event_handler (type(AgencyEventHandler)): The event handler class to handle the completion stream. https://github.com/openai/openai-python/blob/main/helpers.md
-            message_files (list, optional): A list of file ids to be sent as attachments with the message. Defaults to None.
+            message_files (list, optional): A list of file ids to be sent as attachments with the message. When using this parameter, files will be assigned both to file_search and code_interpreter tools if available. It is recommended to assign files to the most sutiable tool manually, using the attachments parameter.  Defaults to None.
             recipient_agent (Agent, optional): The agent to which the message should be sent. Defaults to the first agent in the agency chart.
             additional_instructions (str, optional): Additional instructions to be sent with the message. Defaults to None.
+            attachments (List[dict], optional): A list of attachments to be sent with the message, following openai format. Defaults to None.
+            tool_choice (dict, optional): The tool choice for the recipient agent to use. Defaults to None.
+
         Returns:
             Final response: Final response from the main thread.
         """
         if self.async_mode:
             raise Exception("Streaming is not supported in async mode.")
 
         if not inspect.isclass(event_handler):
             raise Exception("Event handler must not be an instance.")
 
-        gen = self.main_thread.get_completion_stream(message=message, event_handler=event_handler,
-                                                     message_files=message_files, recipient_agent=recipient_agent,
-                                                     additional_instructions=additional_instructions)
-
-        while True:
-            try:
-                next(gen)
-            except StopIteration as e:
-                event_handler.on_all_streams_end()
-                return e.value
+        return self.main_thread.get_completion_stream(message=message,
+                                                      message_files=message_files,
+                                                      event_handler=event_handler,
+                                                      attachments=attachments,
+                                                      recipient_agent=recipient_agent,
+                                                      additional_instructions=additional_instructions,
+                                                      tool_choice=tool_choice
+                                                      )
 
     def demo_gradio(self, height=450, dark_mode=True, **kwargs):
         """
         Launches a Gradio-based demo interface for the agency chatbot.
 
         Parameters:
             height (int, optional): The height of the chatbot widget in the Gradio interface. Default is 600.
@@ -280,15 +312,15 @@
                     chatbot_queue.put(str(snapshot.function))
 
                     if snapshot.function.name == "SendMessage":
                         try:
                             args = eval(snapshot.function.arguments)
                             recipient = args["recipient"]
                             self.message_output = MessageOutput("text", self.recipient_agent_name, recipient,
-                                                                    args["message"])
+                                                                args["message"])
 
                             chatbot_queue.put("[new_message]")
                             chatbot_queue.put(self.message_output.get_formatted_content())
                         except Exception as e:
                             pass
 
                     self.message_output = None
@@ -323,15 +355,15 @@
                 nonlocal message_file_ids
                 nonlocal message_file_names
                 nonlocal recipient_agent
                 print("Message files: ", message_file_ids)
                 # Replace this with your actual chatbot logic
 
                 completion_thread = threading.Thread(target=self.get_completion_stream, args=(
-                original_message, GradioEventHandler, message_file_ids, recipient_agent))
+                    original_message, GradioEventHandler, message_file_ids, recipient_agent))
                 completion_thread.start()
 
                 message_file_ids = []
                 message_file_names = []
 
                 new_message = True
                 while True:
@@ -437,15 +469,15 @@
 
             @override
             def on_tool_call_created(self, tool_call):
                 # TODO: add support for code interpreter and retirieval tools
 
                 if tool_call.type == "function":
                     self.message_output = MessageOutputLive("function", self.recipient_agent_name, self.agent_name,
-                                                        str(tool_call.function))
+                                                            str(tool_call.function))
 
             @override
             def on_tool_call_delta(self, delta, snapshot):
                 self.message_output.cprint_update(str(snapshot.function))
 
             @override
             def on_tool_call_done(self, snapshot):
@@ -493,14 +525,17 @@
 
         self._setup_autocomplete()  # Prepare readline for autocomplete
 
         while True:
             console.rule()
             text = input("👤 USER: ")
 
+            if not text:
+                continue
+
             if text.lower() == "exit":
                 break
 
             recipient_agent = None
             if "@" in text:
                 recipient_agent = text.split("@")[1].split(" ")[0]
                 text = text.replace(f"@{recipient_agent}", "").strip()
@@ -545,20 +580,34 @@
             if "temp_id" in agent.id:
                 agent.id = None
 
             agent.add_shared_instructions(self.shared_instructions)
             agent.settings_path = self.settings_path
 
             if self.shared_files:
+                if isinstance(self.shared_files, str):
+                    self.shared_files = [self.shared_files]
+
                 if isinstance(agent.files_folder, str):
                     agent.files_folder = [agent.files_folder]
                     agent.files_folder += self.shared_files
                 elif isinstance(agent.files_folder, list):
                     agent.files_folder += self.shared_files
 
+            if self.temperature is not None and agent.temperature is None:
+                agent.temperature = self.temperature
+            if self.top_p and agent.top_p is None:
+                agent.top_p = self.top_p
+            if self.max_prompt_tokens is not None and agent.max_prompt_tokens is None:
+                agent.max_prompt_tokens = self.max_prompt_tokens
+            if self.max_completion_tokens is not None and agent.max_completion_tokens is None:
+                agent.max_completion_tokens = self.max_completion_tokens
+            if self.truncation_strategy is not None and agent.truncation_strategy is None:
+                agent.truncation_strategy = self.truncation_strategy
+
             agent.init_oai()
 
         if self.settings_callbacks:
             with open(self.agents[0].get_settings_path(), 'r') as f:
                 settings = f.read()
             settings = json.loads(settings)
             self.settings_callbacks["save"](settings)
@@ -753,58 +802,54 @@
             agent_descriptions += recipient_agent.name + ": "
             agent_descriptions += recipient_agent.description + "\n"
 
         outer_self = self
 
         class SendMessage(BaseTool):
             my_primary_instructions: str = Field(...,
-                                      description="Please repeat your primary instructions step-by-step, including both completed "
-                                                  "and the following next steps that you need to perfrom. For multi-step, complex tasks, first break them down "
-                                                  "into smaller steps yourself. Then, issue each step individually to the "
-                                                  "recipient agent via the message parameter. Each identified step should be "
-                                                  "sent in separate message. Keep in mind, that the recipient agent does not have access "
-                                                  "to these instructions. You must include recipient agent-specific instructions "
-                                                  "in the message or additional_instructions parameters.")
+                                                 description="Please repeat your primary instructions step-by-step, including both completed "
+                                                             "and the following next steps that you need to perfrom. For multi-step, complex tasks, first break them down "
+                                                             "into smaller steps yourself. Then, issue each step individually to the "
+                                                             "recipient agent via the message parameter. Each identified step should be "
+                                                             "sent in separate message. Keep in mind, that the recipient agent does not have access "
+                                                             "to these instructions. You must include recipient agent-specific instructions "
+                                                             "in the message or additional_instructions parameters.")
             recipient: recipients = Field(..., description=agent_descriptions)
             message: str = Field(...,
                                  description="Specify the task required for the recipient agent to complete. Focus on "
                                              "clarifying what the task entails, rather than providing exact "
                                              "instructions.")
-            message_files: List[str] = Field(default=None,
-                                             description="A list of file ids to be sent as attachments to this message. Only use this if you have the file id that starts with 'file-'.",
-                                             examples=["file-1234", "file-5678"])
+            message_files: Optional[List[str]] = Field(default=None,
+                                                       description="A list of file ids to be sent as attachments to this message. Only use this if you have the file id that starts with 'file-'.",
+                                                       examples=["file-1234", "file-5678"])
             additional_instructions: str = Field(default=None,
                                                  description="Any additional instructions or clarifications that you would like to provide to the recipient agent.")
             one_call_at_a_time: bool = True
 
             @model_validator(mode='after')
             def validate_files(self):
-                if "file-" in self.message or (self.additional_instructions and "file-" in self.additional_instructions):
+                if "file-" in self.message or (
+                        self.additional_instructions and "file-" in self.additional_instructions):
                     if not self.message_files:
                         raise ValueError("You must include file ids in message_files parameter.")
 
             @field_validator('recipient')
             def check_recipient(cls, value):
                 if value.value not in recipient_names:
                     raise ValueError(f"Recipient {value} is not valid. Valid recipients are: {recipient_names}")
                 return value
 
             def run(self):
                 thread = outer_self.agents_and_threads[self.caller_agent.name][self.recipient.value]
 
                 if not outer_self.async_mode:
-                    gen = thread.get_completion(message=self.message,
-                                                message_files=self.message_files,
-                                                event_handler=self.event_handler,
-                                                additional_instructions=self.additional_instructions)
-                    try:
-                        while True:
-                            yield next(gen)
-                    except StopIteration as e:
-                        message = e.value
+                    message = thread.get_completion(message=self.message,
+                                                    message_files=self.message_files,
+                                                    event_handler=self.event_handler,
+                                                    additional_instructions=self.additional_instructions)
                 else:
                     message = thread.get_completion_async(message=self.message,
                                                           message_files=self.message_files,
                                                           additional_instructions=self.additional_instructions)
 
                 return message or ""
 
@@ -897,7 +942,14 @@
         """
         Retrieves the absolute path of the directory containing the class file.
 
         Returns:
             str: The absolute path of the directory where the class file is located.
         """
         return os.path.abspath(os.path.dirname(inspect.getfile(self.__class__)))
+
+    def delete(self):
+        """
+        This method deletes the agency and all its agents, cleaning up any files and vector stores associated with each agent.
+        """
+        for agent in self.agents:
+            agent.delete()
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/instructions.md` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/instructions.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 
 The user will communicate to you each agent that needs to be created. Below are your instructions that needs to be followed for each agent communicated by the user.
 
 **Primary Instructions:**
 1. First, read the manifesto using `ReadManifesto` tool if you have not already done so. This file contains the agency manifesto that describes the agency's purpose and goals.
 2. If a similar agent to the requested one is accessible through the `ImportAgent` tool, import this agent and inform the user that the agent has been created. Skip the following steps.
 3. If not, create a new agent using `CreateAgentTemplate` tool. 
-4. Tell the ToolCreator or OpenAPICreator agent to create tools or APIs for this agent. Make sure to also communicate the agent description, name and a summary of the processes that it needs to perform. CEO Agents do not need to utilize any tools, so you can skip this and the following steps.
-5. If there are no issues and tools or APIs have been successfully created, notify the user that the agent has been created. Otherwise, try to resolve any issues with the tool creator before reporting back to the user.
+4. Tell the `ToolCreator` agent to create tools or APIs for this agent. Make sure to also communicate the agent description, name and a summary of the processes that it needs to perform. CEO Agents do not need to utilize any tools, so you can skip this and the following steps.
+5. If there are no issues and tools have been successfully created, notify the user that the agent has been created. Otherwise, try to resolve any issues with the tool creator before reporting back to the user.
 6. Repeat this process for each agent that needs to be created, as instructed by the user.
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import shutil
 from typing import List
 
-from pydantic import Field, model_validator, field_validator
+from pydantic import Field, model_validator
 
 from agency_swarm import BaseTool
 from agency_swarm.agency.genesis.util import check_agency_path
 from agency_swarm.util import create_agent_template
 
 allowed_tools: List = ["CodeInterpreter"]
 
@@ -69,20 +69,19 @@
                               code_interpreter=True if "CodeInterpreter" in self.default_tools else None,
                               include_example_tool=False)
 
         # # create or append to init file
         path = self.shared_state.get("agency_path")
         folder_name = self.agent_name.lower().replace(" ", "_")
         class_name = self.agent_name.replace(" ", "").strip()
-        global_init_path = os.path.join(path, "__init__.py")
-        if not os.path.isfile(global_init_path):
-            with open(global_init_path, "w") as f:
+        if not os.path.isfile("__init__.py"):
+            with open("__init__.py", "w") as f:
                 f.write(f"from .{folder_name} import {class_name}")
         else:
-            with open(global_init_path, "a") as f:
+            with open("__init__.py", "a") as f:
                 f.write(f"\nfrom .{folder_name} import {class_name}")
 
         # add agent on second line to agency.py
         with open("agency.py", "r") as f:
             lines = f.readlines()
             lines.insert(1, f"from {self.agent_name} import {self.agent_name}\n")
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisAgency.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisAgency.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,36 +4,25 @@
 from .GenesisCEO import GenesisCEO
 from .OpenAPICreator import OpenAPICreator
 from .ToolCreator import ToolCreator
 from agency_swarm.util.helpers import get_available_agent_descriptions
 
 class GenesisAgency(Agency):
     def __init__(self, with_browsing=True, **kwargs):
+        if "max_prompt_tokens" not in kwargs:
+            kwargs["max_prompt_tokens"] = 25000
 
         if 'agency_chart' not in kwargs:
             agent_creator = AgentCreator()
             genesis_ceo = GenesisCEO()
-
-            agent_descriptions = get_available_agent_descriptions()
-
-            genesis_ceo.instructions += (
-                "\nAdditionally, there are several pre-built agents available in the agency swarm framework that you can use out of the box.\n"
-                + agent_descriptions + "\n"
-                "If any of the available agents match the requirements for one of the agents in the agency, you can add this agent in the agency chart.\n"
-                "Then, instruct the agent creator to simply import the agent.\n"
-                "If possible, prefer to use this method instead of instructing AgentCreator to create a new agent from scratch.\n"
-            )
-
             tool_creator = ToolCreator()
             openapi_creator = OpenAPICreator()
             kwargs['agency_chart'] = [
                 genesis_ceo, tool_creator, agent_creator,
                 [genesis_ceo, agent_creator],
-                # [agent_creator, openapi_creator],
-                # [openapi_creator, browsing_agent],
                 [agent_creator, tool_creator],
             ]
 
             if with_browsing:
                 from agency_swarm.agents.BrowsingAgent import BrowsingAgent
                 browsing_agent = BrowsingAgent()
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from pathlib import Path
+
 from agency_swarm import Agent
 from .tools.CreateAgencyFolder import CreateAgencyFolder
 from .tools.FinalizeAgency import FinalizeAgency
 from .tools.ReadRequirements import ReadRequirements
 
 
 class GenesisCEO(Agent):
     def __init__(self):
         super().__init__(
             description="Acts as the overseer and communicator across the agency, ensuring alignment with the "
                         "agency's goals.",
             instructions="./instructions.md",
             tools=[CreateAgencyFolder, FinalizeAgency, ReadRequirements],
+            temperature=0.4,
         )
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/instructions.md` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/instructions.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,22 +56,31 @@
 
         # create init file
         with open("__init__.py", "w") as f:
             f.write("")
 
         # create agency.py
         with open("agency.py", "w") as f:
-            f.write("from agency_swarm import Agency\n\n\n")
-            f.write(f"agency = Agency({agency_chart},\nshared_instructions='./agency_manifesto.md')\n\n")
-            f.write("if __name__ == '__main__':\n")
-            f.write("    agency.demo_gradio()\n")
+            f.write(agency_py.format(agency_chart=agency_chart))
 
         # write manifesto
         path = os.path.join("agency_manifesto.md")
         with open(path, "w") as f:
             f.write(self.manifesto)
 
         os.chdir(self.shared_state.get('default_folder'))
 
         return f"Agency folder has been created. You can now tell AgentCreator to create agents for {self.agency_name}.\n"
 
 
+agency_py = """from agency_swarm import Agency
+
+
+agency = Agency({agency_chart},
+                shared_instructions='./agency_manifesto.md', # shared instructions for all agents
+                max_prompt_tokens=25000, # default tokens in conversation for all agents
+                temperature=0.3, # default temperature for all agents
+                )
+                
+if __name__ == '__main__':
+    agency.demo_gradio()
+"""
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/instructions.md` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/instructions.md` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/instructions.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-# ToolCreator Agent Instructions
+# Devid Operational Guide
 
-As a ToolCreator Agent within the Agency Swarm framework, your mission is to develop tools that enhance the capabilities of other agents. These tools are pivotal for enabling agents to communicate, collaborate, and efficiently achieve their collective objectives. Below are detailed instructions to guide you through the process of creating tools, ensuring they are both functional and align with the framework's standards.
+As an AI software developer known as Devid, your role involves reading, writing, and modifying files to fulfill tasks derived from user requests. 
 
-**Here are your primary instructions:**
-1. Determine which tools the agent must utilize to perform it's role. Make an educated guess if the user has not specified any tools or APIs. Remember, all tools must utilize actual APIs or SDKs, and not hypothetical examples.
-2. Create these tools one at a time, using `CreateTool` function. Below are detailed instructions to guide you through the process of creating tools, ensuring they are both functional and align with the framework's standards.
-3. Test each tool with the `TestTool` function to ensure it is working as expected. (if possible)
-4. Once all the necessary tools are created, notify the user.
-
-### Best Practices
-
-- **Documentation:** Ensure each class and method is well-documented. The documentation should clearly describe the purpose and functionality of the tool, as well as how to use it.
-
-- **Code Quality:** Write clean, readable, and efficient code. Adhere to the PEP 8 style guide for Python code.
-
-- **Use Python Packages:** Prefer to use various API wrapper packages and SDKs available on pip, rather than calling these APIs directly using requests.
-
-- **Expect API Keys to be defined as env variables**: If a tool requires an API key or an access token, it must be accessed from the environment using os package and set globally to be used inside the run method. 
-
-- **Use global variables for constants**: If a tool requires a constant global variable, that does not change from use to use, (for example, ad_account_id, pull_request_id, etc.), also define them as constant global variables above the tool class, instead of inside Pydantic `Field`.
-
-- **Test your code**: To test your code, you can use `TestTool` tool when possible.
-
-Remember, you must include the whole python tool code snippet inside the `CreateTool` tool. Each tool code snippet you use inside the `TestTool` must be an actual ready to use code. It must not contain any placeholders or hypothetical examples.
+**Operational Environment**:
+- You have direct access to the internet, system executions, or environment variables. 
+- Interaction with the local file system to read, write, and modify files is permitted.
+- Python is installed in your environment, enabling the execution of Python scripts and code snippets.
+- Node.js and npm are also installed, allowing for the execution of Node.js scripts and code snippets.
+- Installation of additional third-party libraries is within your capabilities.
+- Execution of commands in the terminal to compile and run code is possible.
+
+## Primary Instructions:
+
+1. Begin by fully understanding the task at hand. Use the `myfiles_browser` tool to access and review any files uploaded by the user. If initial access to files fails, retry the operation until successful. Continue browsing the files until you have gathered sufficient information to proceed. Skip this step if no files were provided.
+2. Verify your current directory's path and contents with `ListDir` and `CheckCurrentDir`. If necessary, navigate to the correct directory using the `DirectoryNavigator` tool or create a new directory for the task.
+3. Utilize the `FileWriter` for creating or modifying files. To read a file, employ the `FileReader` tool. Always modify local files when executing tasks and avoid sending code snippets to the user. Work on one file at a time and refrain from creating or modifying multiple files simultaneously. Complete each file with `FileWriter` before proceeding to the next, integrating these files into the dependencies of the main file.
+4. Execute your written code with the `CommandExecutor` by running the appropriate terminal commands. Iteratively debug and test to achieve the desired outcome. Seek clarification from the user only after all internal resolution efforts have been exhausted. To install additional libraries, execute the necessary terminal commands.
+5. Repeat the above steps for each task.
 
+**Important Note**: Your capabilities include accessing and interacting with local files, online resources, and the terminal. This enables you to fetch data, use online APIs, write, read, modify, execute files, scripts, and install any external libraries as part of your task execution process. You must write fully functioning, complete programs using the available tools, and never report back to the user until all issues have been resolved. Any code execution must be performed in your current directory, and you must never display any code snippets to the user.
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agency/genesis/util.py` & `agency_swarm-0.2.0/agency_swarm/agency/genesis/util.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from agency_swarm.agents import Agent
 from .tools.util.selenium import set_selenium_config
-from agency_swarm.tools.oai import Retrieval
+from agency_swarm.tools.oai import FileSearch
 from typing_extensions import override
 
 
 class BrowsingAgent(Agent):
     def __init__(self, selenium_config=None):
         super().__init__(
             name="BrowsingAgent",
             description="This agent is designed to navigate and search web effectively.",
             instructions="./instructions.md",
             files_folder="./files",
             schemas_folder="./schemas",
-            tools=[Retrieval],
-            tools_folder="./tools"
+            tools=[FileSearch],
+            tools_folder="./tools",
+            temperature = 0,
+            max_prompt_tokens = 25000,
         )
 
         if selenium_config is not None:
             set_selenium_config(selenium_config)
 
     @override
     def response_validator(self, message):
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/instructions.md` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/instructions.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,27 +29,17 @@
 
         # Save the PDF to a file
         with open("exported_file.pdf", "wb") as f:
             f.write(pdf_bytes)
 
         file_id = client.files.create(file=open("exported_file.pdf", "rb"), purpose="assistants",).id
 
-        # update caller agent assistant
-        self.caller_agent.file_ids.append(file_id)
-
-        client.beta.assistants.update(
-            assistant_id=self.caller_agent.id,
-            file_ids=self.caller_agent.file_ids
-        )
-
         self.shared_state.set("file_id", file_id)
 
-        return ("Success. File exported with id: `" + file_id +
-                "` You can now use myfiles_browser tool to analyze the contents of this webpage " +
-                "or send this file id back to the user.")
+        return "Success. File exported with id: `" + file_id + "` You can now send this file id back to the user."
 
 
 if __name__ == "__main__":
     wd = get_web_driver()
     wd.get("https://www.google.com")
     tool = ExportFile()
     tool.run()
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/Scroll.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/Scroll.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py` & `agency_swarm-0.2.0/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/Devid.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/Devid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing_extensions import override
 import re
 from agency_swarm.agents import Agent
-from agency_swarm.tools import Retrieval
+from agency_swarm.tools import FileSearch
 from instructor import llm_validator
 
 
 class Devid(Agent):
     def __init__(self):
         super().__init__(
             name="Devid",
             description="Devid is an AI software engineer capable of performing advanced coding tasks.",
             instructions="./instructions.md",
             files_folder="./files",
             schemas_folder="./schemas",
-            tools=[Retrieval],
+            tools=[FileSearch],
             tools_folder="./tools",
             validation_attempts=1,
+            temperature=0,
+            max_prompt_tokens=25000,
         )
 
     @override
     def response_validator(self, message):
         pattern = r'(```)((.*\n){5,})(```)'
 
         if re.search(pattern, message):
@@ -32,10 +34,10 @@
         llm_validator(statement="Verify whether the update from the AI Developer Agent confirms the task's "
                                 "successful completion. If the task remains unfinished, provide guidance "
                                 "within the 'reason' argument on the next steps the agent should take. For "
                                 "instance, if the agent encountered an error, advise the inclusion of debug "
                                 "statements for another attempt. Should the agent outline potential "
                                 "solutions or further actions, direct the agent to execute those plans. "
                                 "Message does not have to contain code snippets. Just confirmation.",
-                      openai_client=self.client)(message)
+                      client=self.client)(message)
 
         return message
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ChangeFile.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/ChangeFile.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/CommandExecutor.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/CommandExecutor.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/DirectoryNavigator.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/DirectoryNavigator.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileMover.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/FileMover.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileReader.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/FileReader.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileWriter.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/FileWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         ..., description="The path of the file to write or modify. Will create directories if they don't exist."
     )
     requirements: str = Field(
         ...,
         description="The comprehensive requirements explaning how the file should be written or modified. This should be a detailed description of what the file should contain, inlcuding example inputs, desired behaviour and ideal outputs. It must not contain any code or implementation details."
     )
     details: str = Field(
-        ..., description="Additional details like error messages, or class, function, and variable names from other files that this file depends on."
+        None, description="Additional details like error messages, or class, function, and variable names from other files that this file depends on."
     )
     documentation: Optional[str] = Field(
         None, description="Relevant documentation extracted with the myfiles_browser tool. You must pass all the relevant code from the documentaion, as this tool does not have access to those files."
     )
     mode: Literal["write", "modify"] = Field(
         ..., description="The mode of operation for the tool. 'write' is used to create a new file or overwrite an existing one. 'modify' is used to modify an existing file."
     )
@@ -98,15 +98,15 @@
         messages.insert(0, history[0])
 
         n = 0
         error_message = ""
         while n < 3:
             resp = client.chat.completions.create(
                 messages=messages,
-                model="gpt-4-turbo-preview",
+                model="gpt-4-turbo",
                 temperature=0,
             )
 
             content = resp.choices[0].message.content
 
             messages.append(
                 {
@@ -185,16 +185,16 @@
         return v
 
     def validate_content(self, v):
         client = get_openai_client()
 
         llm_validator(
             statement="Check if the code is bug-free. Code should be considered in isolation, with the understanding that it is part of a larger, fully developed program that strictly adheres to these standards of completeness and correctness. All files, elements, components, functions, or modules referenced within this snippet are assumed to exist in other parts of the project and are also devoid of any errors, ensuring a cohesive and error-free integration across the entire software solution. Certain placeholders may be present.",
-                      openai_client=client,
-                      model="gpt-4-turbo-preview",
+                      client=client,
+                      model="gpt-4-turbo",
                       temperature=0,
                       allow_override=False
                       )(v)
 
         return v
 
     @field_validator("requirements", mode="after")
@@ -231,14 +231,12 @@
             raise ValueError(
                 "Documentation does not contain a code snippet. Please provide relevant documentation extracted with the myfiles_browser tool. You must pass all the relevant code snippets information, as this tool does not have access to those files."
             )
 
 
 if __name__ == "__main__":
     tool = FileWriter(
-        chain_of_thought="Step 1: Import the necessary libraries. \n\n Step 2: Define the function that takes a list of integers as input and returns the sum of all the integers in the list. \n\n Step 3: Write the function that takes a list of integers as input and returns the sum of all the integers in the list. \n\n Step 4: Write the code to test the function. \n\n Step 5: Save the file.",
-        language="python",
-        file_path="my_file.py",
-        requirements="The file should contain a function that takes a list of integers as input and returns the sum of all the integers in the list.",
-        dependencies="import numpy as np"
+        requirements="Write a program that takes a list of integers as input and returns the sum of all the integers in the list.",
+        mode="write",
+        file_path="test.py",
     )
     print(tool.run())
```

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ListDir.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/ListDir.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/format_file_deps.py` & `agency_swarm-0.2.0/agency_swarm/agents/Devid/tools/util/format_file_deps.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/agents/agent.py` & `agency_swarm-0.2.0/agency_swarm/agents/agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+import copy
 import inspect
 import json
 import os
-from typing import Dict, Union, Any, Type
+from typing import Dict, Union, Any, Type, Literal, TypedDict, Optional
 from typing import List
 
 from deepdiff import DeepDiff
 from openai import NotFoundError
+from openai.types.beta.assistant import ToolResources
 
-from agency_swarm.tools import BaseTool, ToolFactory
-from agency_swarm.tools import Retrieval, CodeInterpreter
+from agency_swarm.tools import BaseTool, ToolFactory, Retrieval
+from agency_swarm.tools import FileSearch, CodeInterpreter
 from agency_swarm.util.oai import get_openai_client
 from agency_swarm.util.openapi import validate_openapi_spec
 
 
+class ExampleMessage(TypedDict):
+    role: Literal["user", "assistant"]
+    content: str
+    attachments: Optional[List[dict]]
+    metadata: Optional[Dict[str, str]]
+
+
 class Agent():
     @property
     def assistant(self):
         if self._assistant is None:
             raise Exception("Assistant is not initialized. Please run init_oai() first.")
         return self._assistant
 
@@ -43,75 +52,100 @@
 
     def __init__(
             self,
             id: str = None,
             name: str = None,
             description: str = None,
             instructions: str = "",
-            tools: List[Union[Type[BaseTool], Type[Retrieval], Type[CodeInterpreter]]] = None,
+            tools: List[Union[Type[BaseTool], Type[FileSearch], Type[CodeInterpreter], type[Retrieval]]] = None,
+            tool_resources: ToolResources = None,
+            temperature: float = None,
+            top_p: float = None,
+            response_format: str | dict = "auto",
             tools_folder: str = None,
             files_folder: Union[List[str], str] = None,
             schemas_folder: Union[List[str], str] = None,
             api_headers: Dict[str, Dict[str, str]] = None,
             api_params: Dict[str, Dict[str, str]] = None,
             file_ids: List[str] = None,
             metadata: Dict[str, str] = None,
-            model: str = "gpt-4-turbo-preview",
+            model: str = "gpt-4-turbo",
             validation_attempts: int = 1,
+            max_prompt_tokens: int = None,
+            max_completion_tokens: int = None,
+            truncation_strategy: dict = None,
+            examples: List[ExampleMessage] = None,
     ):
         """
         Initializes an Agent with specified attributes, tools, and OpenAI client.
 
         Parameters:
             id (str, optional): Loads the assistant from OpenAI assistant ID. Assistant will be created or loaded from settings if ID is not provided. Defaults to None.
             name (str, optional): Name of the agent. Defaults to the class name if not provided.
             description (str, optional): A brief description of the agent's purpose. Defaults to None.
             instructions (str, optional): Path to a file containing specific instructions for the agent. Defaults to an empty string.
             tools (List[Union[Type[BaseTool], Type[Retrieval], Type[CodeInterpreter]]], optional): A list of tools (as classes) that the agent can use. Defaults to an empty list.
+            tool_resources (ToolResources, optional): A set of resources that are used by the assistant's tools. The resources are specific to the type of tool. For example, the code_interpreter tool requires a list of file IDs, while the file_search tool requires a list of vector store IDs. Defaults to None.
+            temperature (float, optional): The temperature parameter for the OpenAI API. Defaults to None.
+            top_p (float, optional): The top_p parameter for the OpenAI API. Defaults to None.
+            response_format (Dict, optional): The response format for the OpenAI API. Defaults to None.
             tools_folder (str, optional): Path to a directory containing tools associated with the agent. Each tool must be defined in a separate file. File must be named as the class name of the tool. Defaults to None.
             files_folder (Union[List[str], str], optional): Path or list of paths to directories containing files associated with the agent. Defaults to None.
             schemas_folder (Union[List[str], str], optional): Path or list of paths to directories containing OpenAPI schemas associated with the agent. Defaults to None.
             api_headers (Dict[str,Dict[str, str]], optional): Headers to be used for the openapi requests. Each key must be a full filename from schemas_folder. Defaults to an empty dictionary.
             api_params (Dict[str, Dict[str, str]], optional): Extra params to be used for the openapi requests. Each key must be a full filename from schemas_folder. Defaults to an empty dictionary.
-            file_ids (List[str], optional): List of file IDs for files associated with the agent. Defaults to an empty list.
             metadata (Dict[str, str], optional): Metadata associated with the agent. Defaults to an empty dictionary.
             model (str, optional): The model identifier for the OpenAI API. Defaults to "gpt-4-turbo-preview".
             validation_attempts (int, optional): Number of attempts to validate the response with response_validator function. Defaults to 1.
+            max_prompt_tokens (int, optional): Maximum number of tokens allowed in the prompt. Defaults to None.
+            max_completion_tokens (int, optional): Maximum number of tokens allowed in the completion. Defaults to None.
+            truncation_strategy (TruncationStrategy, optional): Truncation strategy for the OpenAI API. Defaults to None.
+            examples (List[Dict], optional): A list of example messages for the agent. Defaults to None.
 
         This constructor sets up the agent with its unique properties, initializes the OpenAI client, reads instructions if provided, and uploads any associated files.
         """
         # public attributes
         self.id = id
         self.name = name if name else self.__class__.__name__
         self.description = description
         self.instructions = instructions
         self.tools = tools[:] if tools is not None else []
         self.tools = [tool for tool in self.tools if tool.__name__ != "ExampleTool"]
+        self.tool_resources = tool_resources
+        self.temperature = temperature
+        self.top_p = top_p
+        self.response_format = response_format
         self.tools_folder = tools_folder
         self.files_folder = files_folder if files_folder else []
         self.schemas_folder = schemas_folder if schemas_folder else []
         self.api_headers = api_headers if api_headers else {}
         self.api_params = api_params if api_params else {}
-        self.file_ids = file_ids if file_ids else []
         self.metadata = metadata if metadata else {}
         self.model = model
         self.validation_attempts = validation_attempts
+        self.max_prompt_tokens = max_prompt_tokens
+        self.max_completion_tokens = max_completion_tokens
+        self.truncation_strategy = truncation_strategy
+        self.examples = examples
 
         self.settings_path = './settings.json'
 
         # private attributes
         self._assistant: Any = None
         self._shared_instructions = None
 
         # init methods
         self.client = get_openai_client()
         self._read_instructions()
 
         # upload files
         self._upload_files()
+        if file_ids:
+            print("Warning: 'file_ids' parameter is deprecated. Please use 'tool_resources' parameter instead.")
+            self.add_file_ids(file_ids, "file_search")
 
         self._parse_schemas()
         self._parse_tools_folder()
 
     # --- OpenAI Assistant Methods ---
 
     def init_oai(self):
@@ -129,17 +163,23 @@
 
         # load assistant from id
         if self.id:
             self.assistant = self.client.beta.assistants.retrieve(self.id)
             self.instructions = self.assistant.instructions
             self.name = self.assistant.name
             self.description = self.assistant.description
-            self.file_ids = self.assistant.file_ids
+            self.temperature = self.assistant.temperature
+            self.top_p = self.assistant.top_p
+            self.response_format = self.assistant.response_format
+            if not isinstance(self.response_format, str):
+                self.response_format = self.response_format.model_dump()
+            self.tool_resources = self.assistant.tool_resources.model_dump()
             self.metadata = self.assistant.metadata
             self.model = self.assistant.model
+            self.tool_resources = self.assistant.tool_resources.model_dump()
             # update assistant if parameters are different
             if not self._check_parameters(self.assistant.model_dump()):
                 self._update_assistant()
             return self
 
         # load assistant from settings
         if os.path.exists(path):
@@ -147,34 +187,42 @@
                 settings = json.load(f)
                 # iterate settings and find the assistant with the same name
                 for assistant_settings in settings:
                     if assistant_settings['name'] == self.name:
                         try:
                             self.assistant = self.client.beta.assistants.retrieve(assistant_settings['id'])
                             self.id = assistant_settings['id']
+                            if self.assistant.tool_resources:
+                                self.tool_resources = self.assistant.tool_resources.model_dump()
                             # update assistant if parameters are different
                             if not self._check_parameters(self.assistant.model_dump()):
                                 print("Updating assistant... " + self.name)
                                 self._update_assistant()
                             self._update_settings()
                             return self
                         except NotFoundError:
                             continue
 
         # create assistant if settings.json does not exist or assistant with the same name does not exist
         self.assistant = self.client.beta.assistants.create(
+            model=self.model,
             name=self.name,
             description=self.description,
             instructions=self.instructions,
             tools=self.get_oai_tools(),
-            file_ids=self.file_ids,
+            tool_resources=self.tool_resources,
             metadata=self.metadata,
-            model=self.model
+            temperature=self.temperature,
+            top_p=self.top_p,
+            response_format=self.response_format,
         )
 
+        if self.assistant.tool_resources:
+            self.tool_resources = self.assistant.tool_resources.model_dump()
+
         self.id = self.assistant.id
 
         self._save_settings()
 
         return self
 
     def _update_assistant(self):
@@ -189,15 +237,18 @@
         """
 
         params = {
             "name": self.name,
             "description": self.description,
             "instructions": self.instructions,
             "tools": self.get_oai_tools(),
-            "file_ids": self.file_ids,
+            "tool_resources": self.tool_resources,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+            "response_format": self.response_format,
             "metadata": self.metadata,
             "model": self.model
         }
         params = {k: v for k, v in params.items() if v}
         self.assistant = self.client.beta.assistants.update(
             self.id,
             **params,
@@ -222,14 +273,17 @@
                 if len(file_name) > 1:
                     return file_name[-1] if "file-" in file_name[-1] else None
                 else:
                     return None
 
         files_folders = self.files_folder if isinstance(self.files_folder, list) else [self.files_folder]
 
+        file_search_ids = []
+        code_interpreter_ids = []
+
         for files_folder in files_folders:
             if isinstance(files_folder, str):
                 f_path = files_folder
 
                 if not os.path.isdir(f_path):
                     f_path = os.path.join(self.get_class_folder_path(), files_folder)
                     f_path = os.path.normpath(f_path)
@@ -237,57 +291,85 @@
                 if os.path.isdir(f_path):
                     f_paths = os.listdir(f_path)
 
                     f_paths = [f for f in f_paths if not f.startswith(".")]
 
                     f_paths = [os.path.join(f_path, f) for f in f_paths]
 
-                    # uploading files
+                    code_interpreter_file_extensions = [
+                        ".json",  # JSON
+                        ".csv",  # CSV
+                        ".xml",  # XML
+                        ".jpeg",  # JPEG
+                        ".jpg",  # JPEG
+                        ".gif",  # GIF
+                        ".png",  # PNG
+                        ".zip"  # ZIP
+                    ]
+
                     for f_path in f_paths:
+                        file_ext = os.path.splitext(f_path)[1]
+
                         f_path = f_path.strip()
                         file_id = get_id_from_file(f_path)
                         if file_id:
                             print("File already uploaded. Skipping... " + os.path.basename(f_path))
-                            self.file_ids.append(file_id)
                         else:
                             print("Uploading new file... " + os.path.basename(f_path))
                             with open(f_path, 'rb') as f:
                                 file_id = self.client.with_options(
                                     timeout=80 * 1000,
                                 ).files.create(file=f, purpose="assistants").id
-                                self.file_ids.append(file_id)
                                 f.close()
                             add_id_to_file(f_path, file_id)
+
+                        if file_ext in code_interpreter_file_extensions:
+                            code_interpreter_ids.append(file_id)
+                        else:
+                            file_search_ids.append(file_id)
                 else:
                     print(f"Files folder '{f_path}' is not a directory. Skipping...", )
             else:
                 print("Files folder path must be a string or list of strings. Skipping... ", files_folder)
 
-        if Retrieval not in self.tools and CodeInterpreter not in self.tools and self.file_ids:
-            print("Detected files without Retrieval. Adding Retrieval tool...")
-            self.add_tool(Retrieval)
+        if FileSearch not in self.tools and file_search_ids:
+            print("Detected files without FileSearch. Adding FileSearch tool...")
+            self.add_tool(FileSearch)
+        if CodeInterpreter not in self.tools and code_interpreter_ids:
+            print("Detected files without FileSearch. Adding FileSearch tool...")
+            self.add_tool(CodeInterpreter)
+
+        self.add_file_ids(file_search_ids, "file_search")
+        self.add_file_ids(code_interpreter_ids, "code_interpreter")
 
     # --- Tool Methods ---
 
+    # TODO: fix 2 methods below
     def add_tool(self, tool):
         if not isinstance(tool, type):
             raise Exception("Tool must not be initialized.")
-        if issubclass(tool, Retrieval):
+        if issubclass(tool, FileSearch):
             # check that tools name is not already in tools
             for t in self.tools:
-                if issubclass(t, Retrieval):
+                if issubclass(t, FileSearch):
                     return
             self.tools.append(tool)
         elif issubclass(tool, CodeInterpreter):
             for t in self.tools:
+                if issubclass(t, CodeInterpreter):
+                    return
+            self.tools.append(tool)
+        elif issubclass(tool, Retrieval):
+            for t in self.tools:
                 if issubclass(t, Retrieval):
                     return
             self.tools.append(tool)
         elif issubclass(tool, BaseTool):
             if tool.__name__ == "ExampleTool":
+                print("Skipping importing ExampleTool...")
                 return
             for t in self.tools:
                 if t.__name__ == tool.__name__:
                     self.tools.remove(t)
             self.tools.append(tool)
         else:
             raise Exception("Invalid tool type.")
@@ -295,18 +377,20 @@
     def get_oai_tools(self):
         tools = []
         for tool in self.tools:
             if not isinstance(tool, type):
                 print(tool)
                 raise Exception("Tool must not be initialized.")
 
-            if issubclass(tool, Retrieval):
+            if issubclass(tool, FileSearch):
                 tools.append(tool().model_dump())
             elif issubclass(tool, CodeInterpreter):
                 tools.append(tool().model_dump())
+            elif issubclass(tool, Retrieval):
+                tools.append(tool().model_dump())
             elif issubclass(tool, BaseTool):
                 tools.append({
                     "type": "function",
                     "function": tool.openai_schema
                 })
             else:
                 raise Exception("Invalid tool type.")
@@ -382,15 +466,16 @@
                     print("Items in tools folder must be files. Skipping... ", f_path)
         else:
             print("Tools folder path is not a directory. Skipping... ", self.tools_folder)
 
     def get_openapi_schema(self, url):
         """Get openapi schema that contains all tools from the agent as different api paths. Make sure to call this after agency has been initialized."""
         if self.assistant is None:
-            raise Exception("Assistant is not initialized. Please initialize the agency first, before using this method")
+            raise Exception(
+                "Assistant is not initialized. Please initialize the agency first, before using this method")
 
         return ToolFactory.get_openapi_schema(self.tools, url)
 
     # --- Settings Methods ---
 
     def _check_parameters(self, assistant_settings):
         """
@@ -400,31 +485,51 @@
             assistant_settings (dict): A dictionary containing the settings of an assistant.
 
         Returns:
             bool: True if all the agent's parameters match the assistant settings, False otherwise.
 
         This method compares the current agent's parameters such as name, description, instructions, tools, file IDs, metadata, and model with the given assistant settings. It uses DeepDiff to compare complex structures like tools and metadata. If any parameter does not match, it returns False; otherwise, it returns True.
         """
-
         if self.name != assistant_settings['name']:
             return False
+
         if self.description != assistant_settings['description']:
             return False
+
         if self.instructions != assistant_settings['instructions']:
             return False
+
         tools_diff = DeepDiff(self.get_oai_tools(), assistant_settings['tools'], ignore_order=True)
         if tools_diff != {}:
             return False
-        if set(self.file_ids) != set(assistant_settings['file_ids']):
+
+        if self.temperature != assistant_settings['temperature']:
             return False
+
+        if self.top_p != assistant_settings['top_p']:
+            return False
+
+        tool_resources_settings = copy.deepcopy(self.tool_resources)
+        if tool_resources_settings and tool_resources_settings.get('file_search'):
+            tool_resources_settings['file_search'].pop('vector_stores', None)
+        tool_resources_diff = DeepDiff(tool_resources_settings, assistant_settings['tool_resources'], ignore_order=True)
+        if tool_resources_diff != {}:
+            return False
+
         metadata_diff = DeepDiff(self.metadata, assistant_settings['metadata'], ignore_order=True)
         if metadata_diff != {}:
             return False
+
         if self.model != assistant_settings['model']:
             return False
+
+        response_format_diff = DeepDiff(self.response_format, assistant_settings['response_format'], ignore_order=True)
+        if response_format_diff != {}:
+            return False
+
         return True
 
     def _save_settings(self):
         path = self.get_settings_path()
         # check if settings.json exists
         if not os.path.isfile(path):
             with open(path, 'w') as f:
@@ -449,29 +554,70 @@
                         settings[i] = self.assistant.model_dump()
                         break
             with open(path, 'w') as f:
                 json.dump(settings, f, indent=4)
 
     # --- Helper Methods ---
 
+    def add_file_ids(self, file_ids: List[str], tool_resource: Literal["code_interpreter", "file_search"]):
+        if not file_ids:
+            return
+
+        if self.tool_resources is None:
+            self.tool_resources = {}
+
+        if tool_resource == "code_interpreter":
+            if CodeInterpreter not in self.tools:
+                raise Exception("CodeInterpreter tool not found in tools.")
+
+            if tool_resource not in self.tool_resources or self.tool_resources[
+                tool_resource] is None:
+                self.tool_resources[tool_resource] = {
+                    "file_ids": file_ids
+                }
+
+            self.tool_resources[tool_resource]['file_ids'] = file_ids
+        elif tool_resource == "file_search":
+            if FileSearch not in self.tools:
+                raise Exception("FileSearch tool not found in tools.")
+
+            if tool_resource not in self.tool_resources or self.tool_resources[
+                tool_resource] is None:
+                self.tool_resources[tool_resource] = {
+                    "vector_stores": [{
+                        "file_ids": file_ids
+                    }]
+                }
+            elif not self.tool_resources[tool_resource].get('vector_store_ids'):
+                self.tool_resources[tool_resource]['vector_stores'] = [{
+                    "file_ids": file_ids
+                }]
+            else:
+                vector_store_id = self.tool_resources[tool_resource]['vector_store_ids'][0]
+                self.client.beta.vector_stores.file_batches.create(
+                    vector_store_id=vector_store_id,
+                    file_ids=file_ids
+                )
+        else:
+            raise Exception("Invalid tool resource.")
+
     def get_settings_path(self):
         return self.settings_path
 
     def _read_instructions(self):
         class_instructions_path = os.path.normpath(os.path.join(self.get_class_folder_path(), self.instructions))
         if os.path.isfile(class_instructions_path):
             with open(class_instructions_path, 'r') as f:
                 self.instructions = f.read()
         elif os.path.isfile(self.instructions):
             with open(self.instructions, 'r') as f:
                 self.instructions = f.read()
         elif "./instructions.md" in self.instructions or "./instructions.txt" in self.instructions:
             raise Exception("Instructions file not found.")
 
-
     def get_class_folder_path(self):
         try:
             # First, try to use the __file__ attribute of the module
             return os.path.abspath(os.path.dirname(self.__module__.__file__))
         except AttributeError:
             # If that fails, fall back to inspect
             class_file = inspect.getfile(self.__class__)
@@ -488,20 +634,37 @@
             self.instructions = self.instructions.strip().strip("\n")
             self._shared_instructions = instructions
 
         self.instructions = self._shared_instructions + "\n\n" + self.instructions
 
     # --- Cleanup Methods ---
     def delete(self):
+        """Deletes assistant, all vector stores, and all files associated with the agent."""
         self._delete_assistant()
         self._delete_files()
         self._delete_settings()
 
     def _delete_files(self):
-        for file_id in self.file_ids:
+        if not self.tool_resources:
+            return
+
+        file_ids = []
+        if self.tool_resources.get('code_interpreter'):
+            file_ids = self.tool_resources['code_interpreter'].get('file_ids', [])
+
+        if self.tool_resources.get('file_search'):
+            file_search_vector_store_ids = self.tool_resources['file_search'].get('vector_store_ids', [])
+            for vector_store_id in file_search_vector_store_ids:
+                files = self.client.beta.vector_stores.files.list(vector_store_id=vector_store_id, limit=100)
+                for file in files:
+                    file_ids.append(file.id)
+
+                self.client.beta.vector_stores.delete(vector_store_id)
+
+        for file_id in file_ids:
             self.client.files.delete(file_id)
 
     def _delete_assistant(self):
         self.client.beta.assistants.delete(self.id)
         self._delete_settings()
 
     def _delete_settings(self):
```

### Comparing `agency-swarm-0.1.7/agency_swarm/cli.py` & `agency_swarm-0.2.0/agency_swarm/cli.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/messages/message_output.py` & `agency_swarm-0.2.0/agency_swarm/messages/message_output.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/threads/thread.py` & `agency_swarm-0.2.0/agency_swarm/threads/thread.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import inspect
 import json
 import time
-from typing import Literal
+from typing import Literal, List, Optional
 
 from openai import BadRequestError
+from openai.types.beta import AssistantToolChoice
+from openai.types.beta.threads.message import Attachment
+from openai.types.beta.threads.run import TruncationStrategy
 
+from agency_swarm.tools import FileSearch, CodeInterpreter
 from agency_swarm.util.streaming import AgencyEventHandler
 from agency_swarm.agents import Agent
 from agency_swarm.messages import MessageOutput
 from agency_swarm.user import User
 from agency_swarm.util.oai import get_openai_client
 
 
@@ -27,83 +31,112 @@
     def init_thread(self):
         if self.id:
             self.thread = self.client.beta.threads.retrieve(self.id)
         else:
             self.thread = self.client.beta.threads.create()
             self.id = self.thread.id
 
-    def get_completion_stream(self, message: str, event_handler: type(AgencyEventHandler), message_files=None,
+            if self.recipient_agent.examples:
+                for example in self.recipient_agent.examples:
+                    self.client.beta.threads.messages.create(
+                        thread_id=self.id,
+                        **example,
+                    )
+
+    def get_completion_stream(self,
+                              message: str,
+                              event_handler: type(AgencyEventHandler),
+                              message_files: List[str] = None,
+                              attachments: Optional[List[Attachment]] = None,
                               recipient_agent=None,
-                              additional_instructions: str = None):
-        return self.get_completion(message, message_files, False, recipient_agent, additional_instructions,
-                                   event_handler)
+                              additional_instructions: str = None,
+                              tool_choice: AssistantToolChoice = None):
+
+        return self.get_completion(message,
+                                   message_files,
+                                   attachments,
+                                   recipient_agent,
+                                   additional_instructions,
+                                   event_handler,
+                                   tool_choice,
+                                   yield_messages=False)
+
+    def get_completion(self,
+                       message: str,
+                       message_files: List[str] = None,
+                       attachments: Optional[List[dict]] = None,
+                       recipient_agent=None,
+                       additional_instructions: str = None,
+                       event_handler: type(AgencyEventHandler) = None,
+                       tool_choice: AssistantToolChoice = None,
+                       yield_messages: bool = False
+                       ):
+        if yield_messages:
+            # warn that it is deprecated
+            print("Warning: yield_messages is deprecated. Use get_completion_stream instead.")
+
+        if message_files:
+            recipient_tools = []
+
+            if FileSearch in self.recipient_agent.tools:
+                recipient_tools.append({"type": "file_search"})
+            if CodeInterpreter in self.recipient_agent.tools:
+                recipient_tools.append({"type": "code_interpreter"})
+
+            for file_id in message_files:
+                attachments.append({"file_id": file_id,
+                                    "tools": recipient_tools or [{"type": "file_search"}]})
 
-    def get_completion(self, message: str, message_files=None, yield_messages=True, recipient_agent=None,
-                       additional_instructions: str = None, event_handler: type(AgencyEventHandler) = None):
         if not self.thread:
             self.init_thread()
 
         if not recipient_agent:
             recipient_agent = self.recipient_agent
 
         if event_handler:
-            yield_messages = False
             event_handler.agent_name = self.agent.name
             event_handler.recipient_agent_name = recipient_agent.name
 
         # Determine the sender's name based on the agent type
         sender_name = "user" if isinstance(self.agent, User) else self.agent.name
         playground_url = f'https://platform.openai.com/playground?assistant={recipient_agent.assistant.id}&mode=assistant&thread={self.thread.id}'
         print(f'THREAD:[ {sender_name} -> {recipient_agent.name} ]: URL {playground_url}')
 
         # send message
         self.client.beta.threads.messages.create(
             thread_id=self.thread.id,
             role="user",
             content=message,
-            file_ids=message_files if message_files else [],
+            attachments=attachments
         )
 
-        if yield_messages:
-            yield MessageOutput("text", self.agent.name, recipient_agent.name, message)
-
-        self._create_run(recipient_agent, additional_instructions, event_handler)
+        self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
 
         error_attempts = 0
         validation_attempts = 0
         full_message = ""
         while True:
             self._run_until_done()
 
             # function execution
             if self.run.status == "requires_action":
                 tool_calls = self.run.required_action.submit_tool_outputs.tool_calls
                 tool_outputs = []
                 tool_names = []
                 for tool_call in tool_calls:
-                    if yield_messages:
-                        yield MessageOutput("function", recipient_agent.name, self.agent.name,
-                                            str(tool_call.function))
-
                     output = self.execute_tool(tool_call, recipient_agent, event_handler, tool_names)
                     if inspect.isgenerator(output):
                         try:
                             while True:
                                 item = next(output)
-                                if isinstance(item, MessageOutput) and yield_messages:
-                                    yield item
                         except StopIteration as e:
                             output = e.value
-                            if event_handler:
-                                event_handler.agent_name = self.agent.name
-                                event_handler.recipient_agent_name = recipient_agent.name
-                    else:
-                        if yield_messages:
-                            yield MessageOutput("function_output", tool_call.function.name, recipient_agent.name,
-                                                output)
+                    if event_handler:
+                        event_handler.agent_name = self.agent.name
+                        event_handler.recipient_agent_name = recipient_agent.name
 
                     tool_outputs.append({"tool_call_id": tool_call.id, "output": str(output)})
                     tool_names.append(tool_call.function.name)
 
                 # submit tool outputs
                 try:
                     self._submit_tool_outputs(tool_outputs, event_handler)
@@ -111,15 +144,15 @@
                     if 'Runs in status "expired"' in e.message:
                         self.client.beta.threads.messages.create(
                             thread_id=self.thread.id,
                             role="user",
                             content="Please repeat the exact same function calls again in the same order."
                         )
 
-                        self._create_run(recipient_agent, additional_instructions, event_handler)
+                        self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
 
                         self._run_until_done()
 
                         if self.run.status != "requires_action":
                             raise Exception("Run Failed. Error: ", self.run.last_error)
 
                         # change tool call ids
@@ -132,91 +165,91 @@
                         raise e
             # error
             elif self.run.status == "failed":
                 full_message += self._get_last_message_text() + "\n"
                 # retry run 2 times
                 if error_attempts < 1 and "something went wrong" in self.run.last_error.message.lower():
                     time.sleep(1)
-                    self._create_run(recipient_agent, additional_instructions, event_handler)
+                    self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
                     error_attempts += 1
                 elif 1 <= error_attempts < 5 and "something went wrong" in self.run.last_error.message.lower():
                     self.client.beta.threads.messages.create(
                         thread_id=self.thread.id,
                         role="user",
                         content="Continue."
                     )
-                    self._create_run(recipient_agent, additional_instructions, event_handler)
+                    self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
                     error_attempts += 1
                 else:
                     raise Exception("OpenAI Run Failed. Error: ", self.run.last_error.message)
             # return assistant message
             else:
                 full_message += self._get_last_message_text()
 
-                if yield_messages:
-                    yield MessageOutput("text", recipient_agent.name, self.agent.name, full_message)
-
                 if recipient_agent.response_validator:
                     try:
                         if isinstance(recipient_agent, Agent):
                             recipient_agent.response_validator(message=full_message)
                     except Exception as e:
-                        full_message = ""
                         if validation_attempts < recipient_agent.validation_attempts:
                             message = self.client.beta.threads.messages.create(
                                 thread_id=self.thread.id,
                                 role="user",
                                 content=str(e),
                             )
 
-                            if yield_messages:
-                                yield MessageOutput("text", self.agent.name, recipient_agent.name,
-                                                    message.content[0].text.value)
-
                             if event_handler:
                                 handler = event_handler()
                                 handler.on_message_created(message)
                                 handler.on_message_done(message)
 
                             validation_attempts += 1
 
-                            self._create_run(recipient_agent, additional_instructions, event_handler)
+                            self._create_run(recipient_agent, additional_instructions, event_handler, tool_choice)
 
                             continue
 
                 return full_message
 
-    def _create_run(self, recipient_agent, additional_instructions, event_handler):
+    def _create_run(self, recipient_agent, additional_instructions, event_handler, tool_choice):
         if event_handler:
-            with self.client.beta.threads.runs.create_and_stream(
+            with self.client.beta.threads.runs.stream(
                     thread_id=self.thread.id,
                     event_handler=event_handler(),
                     assistant_id=recipient_agent.id,
                     additional_instructions=additional_instructions,
+                    tool_choice=tool_choice,
+                    max_prompt_tokens=recipient_agent.max_prompt_tokens,
+                    max_completion_tokens=recipient_agent.max_completion_tokens,
+                    truncation_strategy=recipient_agent.truncation_strategy,
             ) as stream:
                 stream.until_done()
                 self.run = stream.get_final_run()
         else:
-            self.run = self.client.beta.threads.runs.create(
+            self.run = self.client.beta.threads.runs.create_and_poll(
                 thread_id=self.thread.id,
                 assistant_id=recipient_agent.id,
                 additional_instructions=additional_instructions,
+                tool_choice=tool_choice,
+                max_prompt_tokens=recipient_agent.max_prompt_tokens,
+                max_completion_tokens=recipient_agent.max_completion_tokens,
+                truncation_strategy=recipient_agent.truncation_strategy,
             )
 
     def _run_until_done(self):
         while self.run.status in ['queued', 'in_progress', "cancelling"]:
             time.sleep(0.5)
             self.run = self.client.beta.threads.runs.retrieve(
                 thread_id=self.thread.id,
                 run_id=self.run.id
             )
 
     def _submit_tool_outputs(self, tool_outputs, event_handler):
         if not event_handler:
-            self.run = self.client.beta.threads.runs.submit_tool_outputs(
+            self.run = self.client.beta.threads.runs.submit_tool_outputs_and_poll(
                 thread_id=self.thread.id,
                 run_id=self.run.id,
                 tool_outputs=tool_outputs
             )
         else:
             with self.client.beta.threads.runs.submit_tool_outputs_stream(
                     thread_id=self.thread.id,
```

### Comparing `agency-swarm-0.1.7/agency_swarm/threads/thread_async.py` & `agency_swarm-0.2.0/agency_swarm/threads/thread_async.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,64 @@
 import threading
-from typing import Literal
+from typing import Literal, Optional, List
+
+from openai.types.beta import AssistantToolChoice
 
 from agency_swarm.agents import Agent
 from agency_swarm.threads import Thread
 from agency_swarm.user import User
 
 
 class ThreadAsync(Thread):
     def __init__(self, agent: Literal[Agent, User], recipient_agent: Agent):
         super().__init__(agent, recipient_agent)
         self.pythread = None
         self.response = None
 
-    def worker(self, message: str, message_files=None, additional_instructions: str = None):
-        gen = super().get_completion(message=message,
-                                     message_files=message_files,
-                                     yield_messages=False,  # yielding is not supported in async mode
-                                     additional_instructions=additional_instructions)
-        while True:
-            try:
-                next(gen)
-            except StopIteration as e:
-                self.response = f"""{self.recipient_agent.name}'s Response: '{e.value}'"""
-                break
+    def worker(self,
+               message: str,
+               message_files: List[str] = None,
+               attachments: Optional[List[dict]] = None,
+               recipient_agent=None,
+               additional_instructions: str = None,
+               tool_choice: AssistantToolChoice = None
+               ):
+        output = super().get_completion(message=message,
+                                        message_files=message_files,
+                                        attachments=attachments,
+                                        recipient_agent=recipient_agent,
+                                        additional_instructions=additional_instructions,
+                                        tool_choice=tool_choice)
+
+        self.response = f"""{self.recipient_agent.name}'s Response: '{output}'"""
 
         return
 
-    def get_completion_async(self, message: str, message_files=None, additional_instructions: str = None):
+    def get_completion_async(self,
+                             message: str,
+                             message_files: List[str] = None,
+                             attachments: Optional[List[dict]] = None,
+                             recipient_agent=None,
+                             additional_instructions: str = None,
+                             tool_choice: AssistantToolChoice = None,
+                             ):
         if self.pythread and self.pythread.is_alive():
             return "System Notification: 'Agent is busy, so your message was not received. Please always use 'GetResponse' tool to check for status first, before using 'SendMessage' tool again for the same agent.'"
         elif self.pythread and not self.pythread.is_alive():
             self.pythread.join()
             self.pythread = None
             self.response = None
 
         run = self.get_last_run()
 
         if run and run.status in ['queued', 'in_progress', 'requires_action']:
             return "System Notification: 'Agent is busy, so your message was not received. Please always use 'GetResponse' tool to check for status first, before using 'SendMessage' tool again for the same agent.'"
 
         self.pythread = threading.Thread(target=self.worker,
-                                         args=(message, message_files, additional_instructions))
+                                         args=(message, message_files, attachments, recipient_agent, additional_instructions, tool_choice))
 
         self.pythread.start()
 
         return "System Notification: 'Task has started. Please notify the user that they can tell you to check the status later. You can do this with the 'GetResponse' tool, after you have been instructed to do so. Don't mention the tool itself to the user. "
 
     def check_status(self, run=None):
         if not run:
```

### Comparing `agency-swarm-0.1.7/agency_swarm/tools/BaseTool.py` & `agency_swarm-0.2.0/agency_swarm/tools/BaseTool.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/tools/ToolFactory.py` & `agency_swarm-0.2.0/agency_swarm/tools/ToolFactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,17 @@
         file_path = os.path.relpath(file_path)
         # Normalize the file path to be absolute and extract components
         directory, file_name = os.path.split(file_path)
         import_path = os.path.splitext(file_path)[0].replace(os.sep, ".")
         class_name = os.path.splitext(file_name)[0]
 
         exec_globals = globals()
+
+        sys.path.append(os.getcwd())
+
         exec(f"from {import_path} import {class_name}", exec_globals)
 
         imported_class = exec_globals.get(class_name)
         if not imported_class:
             raise ImportError(f"Could not import {class_name} from {import_path}")
 
         # Check if the imported class is a subclass of BaseTool
```

### Comparing `agency-swarm-0.1.7/agency_swarm/util/cli/create_agent_template.py` & `agency_swarm-0.2.0/agency_swarm/util/cli/create_agent_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,29 +68,31 @@
         super().__init__(
             name="{agent_name}",
             description="{agent_description}",
             instructions="./instructions.{ext}",
             files_folder="./files",
             schemas_folder="./schemas",
             tools=[{code_interpreter}],
-            tools_folder="./tools"
+            tools_folder="./tools",
+            temperature=0.3,
+            max_prompt_tokens=25000,
         )
         
     def response_validator(self, message):
         return message
 """
 
 example_tool_template = """from agency_swarm.tools import BaseTool
 from pydantic import Field
 import os
 
 account_id = "MY_ACCOUNT_ID"
 api_key = os.getenv("MY_API_KEY") # or access_token = os.getenv("MY_ACCESS_TOKEN")
 
-class MyCustomTool(BaseTool):
+class ExampleTool(BaseTool):
     \"\"\"
     A brief description of what the custom tool does.
     The docstring should clearly explain the tool's purpose and functionality.
     It will be used by the agent to determine when to use this tool.
     \"\"\"
 
     # Define the fields with descriptions using Pydantic Field
@@ -104,9 +106,9 @@
         This method should utilize the fields defined above to perform the task.
         Docstring is not required for this method and will not be used by the agent.
         \"\"\"
         # Your custom tool logic goes here
         # do_something(self.example_field, api_key, account_id)
 
         # Return the result of the tool's operation as a string
-        return "Result of MyCustomTool operation"
+        return "Result of ExampleTool operation"
 """
```

### Comparing `agency-swarm-0.1.7/agency_swarm/util/cli/import_agent.py` & `agency_swarm-0.2.0/agency_swarm/util/cli/import_agent.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/util/event_handler.py` & `agency_swarm-0.2.0/agency_swarm/util/event_handler.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/util/helpers/get_available_agent_descriptions.py` & `agency_swarm-0.2.0/agency_swarm/util/helpers/get_available_agent_descriptions.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/util/helpers/list_available_agents.py` & `agency_swarm-0.2.0/agency_swarm/util/helpers/list_available_agents.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/util/oai.py` & `agency_swarm-0.2.0/agency_swarm/util/oai.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         if client is None:
             # Check if the API key is set
             api_key = openai.api_key or os.getenv('OPENAI_API_KEY')
             if api_key is None:
                 raise ValueError("OpenAI API key is not set. Please set it using set_openai_key.")
             client = instructor.patch(openai.OpenAI(api_key=api_key,
                                                     timeout=httpx.Timeout(60.0, read=30, connect=5.0),
-                                                    max_retries=5))
+                                                    max_retries=5,
+                                                    default_headers={"OpenAI-Beta": "assistants=v2"})
+                                      )
     return client
 
 
 def set_openai_client(new_client):
     global client
     with client_lock:
         client = instructor.patch(new_client)
```

### Comparing `agency-swarm-0.1.7/agency_swarm/util/openapi.py` & `agency_swarm-0.2.0/agency_swarm/util/openapi.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm/util/schema.py` & `agency_swarm-0.2.0/agency_swarm/util/schema.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/agency_swarm.egg-info/PKG-INFO` & `agency_swarm-0.2.0/agency_swarm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.1.7
+Version: 0.2.0
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -30,16 +30,16 @@
 Project-URL: homepage, https://github.com/VRSEN/agency-swarm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.14.2
-Requires-Dist: instructor==0.6.7
+Requires-Dist: openai==1.23.3
+Requires-Dist: instructor==1.2.2
 Requires-Dist: deepdiff==6.7.1
 Requires-Dist: termcolor==2.3.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: rich==13.7.0
 Requires-Dist: jsonref==1.1.0
 
 # 🐝 Agency Swarm
@@ -120,36 +120,38 @@
     
     or convert from OpenAPI schemas:
     
     ```python
     from agency_swarm.tools import ToolFactory
     # using local file
     with open("schemas/your_schema.json") as f:
-        ToolFactory.from_openapi_schema(
+        tools = ToolFactory.from_openapi_schema(
             f.read(),
         )
     
     # using requests
-    ToolFactory.from_openapi_schema(
+    tools = ToolFactory.from_openapi_schema(
         requests.get("https://api.example.com/openapi.json").json(),
     )
     ```
 
-
 3. **Define Agent Roles**: Start by defining the roles of your agents. For example, a CEO agent for managing tasks and a developer agent for executing tasks.
 
     ```python
     from agency_swarm import Agent
     
     ceo = Agent(name="CEO",
                 description="Responsible for client communication, task planning and management.",
                 instructions="You must converse with other agents to ensure complete task execution.", # can be a file like ./instructions.md
                 files_folder="./files", # files to be uploaded to OpenAI
                 schemas_folder="./schemas", # OpenAPI schemas to be converted into tools
-                tools=[MyCustomTool, LangchainTool])
+                tools=[MyCustomTool], 
+                temperature=0.5, # temperature for the agent
+                max_prompt_tokens=25000, # max tokens in conversation history
+                )
     ```
 
     Import from existing agents:
 
    ```bash
    agency-swarm import-agent --name "Devid" --destination "./"
    ```
@@ -167,19 +169,23 @@
     from Developer import Developer
     from VirtualAssistant import VirtualAssistant
    
     dev = Developer()
     va = VirtualAssistant()
     
     agency = Agency([
-        ceo,  # CEO will be the entry point for communication with the user
-        [ceo, dev],  # CEO can initiate communication with Developer
-        [ceo, va],   # CEO can initiate communication with Virtual Assistant
-        [dev, va]    # Developer can initiate communication with Virtual Assistant
-    ], shared_instructions='agency_manifesto.md') # shared instructions for all agents
+           ceo,  # CEO will be the entry point for communication with the user
+           [ceo, dev],  # CEO can initiate communication with Developer
+           [ceo, va],   # CEO can initiate communication with Virtual Assistant
+           [dev, va]    # Developer can initiate communication with Virtual Assistant
+         ], 
+         shared_instructions='agency_manifesto.md', #shared instructions for all agents
+         temperature=0.5, # default temperature for all agents
+         max_prompt_tokens=25000 # default max tokens in conversation history
+    )
     ```
 
      In Agency Swarm, communication flows are directional, meaning they are established from left to right in the agency_chart definition. For instance, in the example above, the CEO can initiate a chat with the developer (dev), and the developer can respond in this chat. However, the developer cannot initiate a chat with the CEO. The developer can initiate a chat with the virtual assistant (va) and assign new tasks.
 
 5. **Run Demo**: 
 Run the demo to see your agents in action!
     
@@ -194,15 +200,15 @@
     ```python
     agency.run_demo()
     ```
     
     Backend version:
     
     ```python
-    completion_output = agency.get_completion("Please create a new website for our client.", yield_messages=False)
+    completion_output = agency.get_completion("Please create a new website for our client.")
     ```
 
 # CLI
 
 ## Genesis Agency
 
 The `genesis` command starts the genesis agency in your terminal to help you create new agencies and agents.
```

### Comparing `agency-swarm-0.1.7/agency_swarm.egg-info/SOURCES.txt` & `agency_swarm-0.2.0/agency_swarm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 mkdocs.yml
 pyproject.toml
 requirements.txt
 requirements_docs.txt
 requirements_test.txt
 run_tests.py
 setup.py
+.github/workflows/close-issues.yml
 .github/workflows/docs.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 agency_swarm/__init__.py
 agency_swarm/cli.py
 agency_swarm.egg-info/PKG-INFO
 agency_swarm.egg-info/SOURCES.txt
@@ -89,14 +90,15 @@
 agency_swarm/threads/__init__.py
 agency_swarm/threads/thread.py
 agency_swarm/threads/thread_async.py
 agency_swarm/tools/BaseTool.py
 agency_swarm/tools/ToolFactory.py
 agency_swarm/tools/__init__.py
 agency_swarm/tools/oai/CodeInterpreter.py
+agency_swarm/tools/oai/FileSearch.py
 agency_swarm/tools/oai/Retrieval.py
 agency_swarm/tools/oai/__init__.py
 agency_swarm/user/__init__.py
 agency_swarm/user/user.py
 agency_swarm/util/__init__.py
 agency_swarm/util/event_handler.py
 agency_swarm/util/oai.py
@@ -116,14 +118,15 @@
 docs/index.md
 docs/quick_start.md
 docs/advanced-usage/agencies.md
 docs/advanced-usage/agents.md
 docs/advanced-usage/azure-openai.md
 docs/advanced-usage/tools.md
 docs/introduction/showcase.md
+notebooks/Agency_Swarm_with_Open_Source_Model.ipynb
 notebooks/agency_async.ipynb
 notebooks/azure.ipynb
 notebooks/genesis_agency.ipynb
 notebooks/web_browser_agent.ipynb
 tests/__init__.py
 tests/test_agency.py
 tests/test_tool_factory.py
```

### Comparing `agency-swarm-0.1.7/docs/advanced-usage/agencies.md` & `agency_swarm-0.2.0/docs/advanced-usage/agencies.md`

 * *Files 9% similar despite different names*

```diff
@@ -105,14 +105,22 @@
 
 If you would like to use a different file path for the settings, other than default `settings.json`, you can specify a `settings_path` parameter. All your agent states will then be saved and loaded from this file. If this file does not exist, it will be created, along with new Assistants on your OpenAI account.
 
 ```python
 agency = Agency([ceo], settings_path='my_settings.json') 
 ```
 
+### Temperture and Max Token Controls
+
+You can also specify parameters like `temperature`, `top_p`, `max_completion_tokens`,  `max_prompt_tokens` and `truncation_strategy`, parameters for the entire agency. These parameters will be used as default values for all agents in the agency, however, you can still override them for individual agents by specifying them in the agent's constructor.
+
+```python
+agency = Agency([ceo], temperature=0.3, max_prompt_tokens=25000) 
+```
+
 ## Running the Agency
 
 When it comes to running the agency, you have 3 options:
 
 1. **Run it inside a Gradio interface**: The most convenient way to get started.
 2. **Get completion from the agency**: For backend or custom integrations.
 3. **Run it from your terminal**: Best for quick debugging and testing.
@@ -122,18 +130,30 @@
 ```python
 agency.demo_gradio(height=700) 
 ```
 
 ### Get completion from the agency
 
 ```python
-response = agency.get_completion("I want you to build me a website", yield_messages=False)
+response = agency.get_completion("I want you to build me a website", 
+                                 additional_instructions="This is an additional instruction for the task.",
+                                 tool_choice={"type": "function", "function": {"name": "SendMessage"}},
+                                 attachments=[],
+                                 )
 print(response)
 ```
 
 ### Running the Agency from your terminal
 
 ```bash
 agency.run_demo()
 ```
 
-To talk to one of the top level agents when running the agency from your terminal, you can use **mentions feature**, similar to how you would use it inside ChatGPT. Simply mention the agent name in the message like `@Developer I want you to build me a website`. The message will then be sent to the Developer agent, instead of the CEO. You can also use tab to autocomplete the agent name after the `@` symbol.
+To talk to one of the top level agents when running the agency from your terminal, you can use **mentions feature**, similar to how you would use it inside ChatGPT. Simply mention the agent name in the message like `@Developer I want you to build me a website`. The message will then be sent to the Developer agent, instead of the CEO. You can also use tab to autocomplete the agent name after the `@` symbol.
+
+## Deleting the Agency
+
+If you would like to delete the agency and all its agents with all associated files and vector stores, you can use the `delete` method.
+
+```python
+agency.delete()
+```
```

### Comparing `agency-swarm-0.1.7/docs/advanced-usage/agents.md` & `agency_swarm-0.2.0/docs/advanced-usage/agents.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 
 ```python
 from agency_swarm import Agent
 
 agent = Agent(name="My Agent",
               description="This is a description of my agent.",
               instructions="These are the instructions for my agent.",
-              tools=["ToolClass1", "ToolClass1"])
+              tools=[ToolClass1, ToolClass2],
+              temperature=0.3,
+              max_prompt_tokens=25000
+            )
 ```
 
 ### Create agent template locally using CLI
 
 This CLI command simplifies the process of creating a structured environment for each agent.
 
 #### **Command Syntax:**
@@ -69,33 +72,65 @@
     def __init__(self):
         super().__init__(
             name="agent_name",
             description="agent_description",
             instructions="./instructions.md",
             files_folder="./files",
             schemas_folder="./schemas",
-            tools_folder="./tools"
+            tools_folder="./tools",
+            temperature=0.3,
+            max_prompt_tokens=25000,
+            examples=[]
         )
 
     def response_validator(self, message: str) -> str:
         """This function is used to validate the response before sending it to the user or another agent."""
         if "bad word" in message:
-            return "Please don't use bad words."
+            raise ValueError("Please don't use bad words.")
         
         return message
 ```
 
 To initialize the agent, you can simply import the agent and instantiate it:
 
 ```python
 from AgentName import AgentName
 
 agent = AgentName()
 ```
 
+### Few-Shot Examples
+
+You can now also provide **few-shot** examples for each agent. These examples help the agent to understand how to respond. The format for examples follows [message object format on OpenAI](https://platform.openai.com/docs/api-reference/messages/createMessage):
+
+```python
+examples=[
+    {
+        "role": "user",
+        "content": "Hi!",
+        "attachments": [],
+        "metadata": {},
+    },
+    {
+        "role": "assistant",
+        "content": "Hi! I am the CEO. I am here to help you with your tasks. Please tell me what you need help with.",
+        "attachments": [],
+        "metadata": {},
+    }
+]
+
+agent.examples = examples
+```
+
+or you can also provide them when initializing the agent in init method:
+
+```python
+agent = Agent(examples=examples)
+```
+
 ### Importing existing agents
 
 For the most complex and requested use cases, we will be creating premade agents that you can import and reuse in your own projects. To import an existing agent, you can run the following CLI command:
 
 ```bash
 agency-swarm import-agent --name "AgentName" --destination "/path/to/directory"
 ```
```

### Comparing `agency-swarm-0.1.7/docs/advanced-usage/azure-openai.md` & `agency_swarm-0.2.0/docs/advanced-usage/azure-openai.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/docs/advanced-usage/tools.md` & `agency_swarm-0.2.0/docs/advanced-usage/tools.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/docs/contributing.md` & `agency_swarm-0.2.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/docs/deployment.md` & `agency_swarm-0.2.0/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/docs/examples.md` & `agency_swarm-0.2.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/docs/index.md` & `agency_swarm-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/docs/quick_start.md` & `agency_swarm-0.2.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/mkdocs.yml` & `agency_swarm-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/notebooks/agency_async.ipynb` & `agency_swarm-0.2.0/notebooks/agency_async.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/notebooks/azure.ipynb` & `agency_swarm-0.2.0/notebooks/azure.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/notebooks/genesis_agency.ipynb` & `agency_swarm-0.2.0/notebooks/genesis_agency.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/notebooks/web_browser_agent.ipynb` & `agency_swarm-0.2.0/notebooks/web_browser_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/pyproject.toml` & `agency_swarm-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "openai==1.14.2",
-    "instructor==0.6.7",
+    "openai==1.23.3",
+    "instructor==1.2.2",
     "deepdiff==6.7.1",
     "termcolor==2.3.0",
     "python-dotenv==1.0.0",
     "rich==13.7.0",
     "jsonref==1.1.0"
 ]
 requires-python = ">=3.7"
```

### Comparing `agency-swarm-0.1.7/run_tests.py` & `agency_swarm-0.2.0/run_tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import unittest
 import os
 import sys
 
 if __name__ == '__main__':
+    os.environ["DEBUG_MODE"] = "True"
+
     # Change the current working directory to 'tests'
     os.chdir('tests')
 
     # Create a test suite combining all test cases
     loader = unittest.TestLoader()
     suite = loader.discover(start_dir='.', pattern='test*.py')
```

### Comparing `agency-swarm-0.1.7/setup.py` & `agency_swarm-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='agency-swarm',
-    version='0.1.7',
+    version='0.2.0',
     author='VRSEN',
     author_email='arseny9795@gmail.com',
     description='An opensource agent orchestration framework built on top of the latest OpenAI Assistants API.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VRSEN/agency-swarm',
     packages=find_packages(exclude=['tests', 'tests.*']),
```

### Comparing `agency-swarm-0.1.7/tests/data/files/csv-test.csv` & `agency_swarm-0.2.0/tests/data/files/csv-test.csv`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/files/generated_data.json` & `agency_swarm-0.2.0/tests/data/files/generated_data.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/files/test-docx.docx` & `agency_swarm-0.2.0/tests/data/files/test-docx.docx`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/files/test-html.html` & `agency_swarm-0.2.0/tests/data/files/test-html.html`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/files/test-pdf.pdf` & `agency_swarm-0.2.0/tests/data/files/test-pdf.pdf`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/schemas/ga4.json` & `agency_swarm-0.2.0/tests/data/schemas/ga4.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/schemas/get-headers-params.json` & `agency_swarm-0.2.0/tests/data/schemas/get-headers-params.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/schemas/get-weather.json` & `agency_swarm-0.2.0/tests/data/schemas/get-weather.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/data/schemas/relevance.json` & `agency_swarm-0.2.0/tests/data/schemas/relevance.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/demos/demo_gradio.py` & `agency_swarm-0.2.0/tests/demos/demo_gradio.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import gradio as gr
 
 sys.path.insert(0, './agency-swarm')
 
 from agency_swarm import set_openai_key, Agent
 
 from agency_swarm.agency.agency import Agency
-from agency_swarm.tools.oai import Retrieval
+from agency_swarm.tools.oai import FileSearch
 
 ceo = Agent(name="CEO",
             description="Responsible for client communication, task planning and management.",
             instructions="Analyze uploaded files with myfiles_browser tool.", # can be a file like ./instructions.md
-            tools=[Retrieval])
+            tools=[FileSearch])
 
 
 test_agent = Agent(name="Test Agent1",
                      description="Responsible for testing.",
                      instructions="Read files with myfiles_browser tool.", # can be a file like ./instructions.md
-                     tools=[Retrieval])
+                     tools=[FileSearch])
 
 test_agent2 = Agent(name="Test Agent2",
                      description="Responsible for testing.",
                      instructions="Read files with myfiles_browser tool.", # can be a file like ./instructions.md
-                     tools=[Retrieval])
+                     tools=[FileSearch])
 
 
 
 agency = Agency([
     ceo, test_agent, test_agent2
 ], shared_instructions="")
```

### Comparing `agency-swarm-0.1.7/tests/demos/streaming_demo.py` & `agency_swarm-0.2.0/tests/demos/streaming_demo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import sys
+import time
 import unittest
 
 from agency_swarm import Agent, BaseTool
 from agency_swarm.agency.agency import Agency
 
 sys.path.insert(0, '../agency-swarm')
 
 
 class StreamingTest(unittest.TestCase):
     def setUp(self):
         class TestTool(BaseTool):
             def run(self):
+                time.sleep(10)
+                print('done')
                 return "Test Successful"
 
         self.ceo = Agent(name="ceo", instructions="You are a CEO of an agency made for testing purposes.",
                          model='gpt-3.5-turbo')
         self.test_agent1 = Agent(name="test_agent1", tools=[TestTool], model='gpt-3.5-turbo')
         self.test_agent2 = Agent(name="test_agent2", model='gpt-3.5-turbo')
```

### Comparing `agency-swarm-0.1.7/tests/demos/term_demo.py` & `agency_swarm-0.2.0/tests/demos/term_demo.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.7/tests/test_agency.py` & `agency_swarm-0.2.0/tests/test_agency.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,48 +4,50 @@
 import shutil
 import sys
 import time
 import unittest
 
 from openai.types.beta.threads.runs import ToolCall
 
-from agency_swarm.tools import CodeInterpreter, Retrieval
+from agency_swarm.tools import CodeInterpreter, FileSearch
 
 sys.path.insert(0, '../agency-swarm')
 from agency_swarm.util import create_agent_template
 
-from agency_swarm import set_openai_key, Agent, Agency, AgencyEventHandler
+from agency_swarm import set_openai_key, Agent, Agency, AgencyEventHandler, get_openai_client
 from typing_extensions import override
 from agency_swarm.tools import BaseTool
 
+os.environ["DEBUG_MODE"] = "True"
 
 class AgencyTest(unittest.TestCase):
     TestTool = None
     agency = None
     agent2 = None
     agent1 = None
     ceo = None
     num_schemas = None
     num_files = None
+    client = None
 
     # testing loading agents from db
     loaded_thread_ids = None
     loaded_agents_settings = None
     settings_callbacks = None
     threads_callbacks = None
 
-
     @classmethod
     def setUpClass(cls):
         cls.num_files = 0
         cls.num_schemas = 0
         cls.ceo = None
         cls.agent1 = None
         cls.agent2 = None
         cls.agency = None
+        cls.client = get_openai_client()
 
         # testing loading agents from db
         cls.loaded_thread_ids = {}
         cls.loaded_agents_settings = []
 
         def save_settings_callback(settings):
             cls.loaded_agents_settings = settings
@@ -59,37 +61,39 @@
             cls.loaded_thread_ids = agents_and_thread_ids
 
         cls.threads_callbacks = {
             "load": lambda: cls.loaded_thread_ids,
             "save": save_thread_callback,
         }
 
-
         if not os.path.exists("./test_agents"):
             os.mkdir("./test_agents")
         else:
             shutil.rmtree("./test_agents")
             os.mkdir("./test_agents")
 
         # create init file
         with open("./test_agents/__init__.py", "w") as f:
             f.write("")
 
         # create agent templates in test_agents
         create_agent_template("CEO", "CEO Test Agent", path="./test_agents",
                               instructions="Your task is to tell TestAgent1 to say test to another test agent. If the "
                                            "agent, does not respond or something goes wrong please say 'error' and "
-                                           "nothing else. Otherwise say 'success' and nothing else.")
+                                           "nothing else. Otherwise say 'success' and nothing else.",
+                              include_example_tool=True)
         create_agent_template("TestAgent1", "Test Agent 1", path="./test_agents",
                               instructions="Your task is to say test to another test agent using SendMessage tool. "
                                            "If the agent, does not "
                                            "respond or something goes wrong please say 'error' and nothing else. "
-                                            "Otherwise say 'success' and nothing else.", code_interpreter=True)
+                                           "Otherwise say 'success' and nothing else.", code_interpreter=True,
+                              include_example_tool=False)
         create_agent_template("TestAgent2", "Test Agent 2", path="./test_agents",
-                              instructions="Please respond to the user that test was a success.")
+                              instructions="After using TestTool, please respond to the user that test was a success in JSON format. You can use the following format: {'test': 'success'}.",
+                              include_example_tool=False)
 
         sys.path.insert(0, './test_agents')
 
         # copy files from data/files to test_agents/TestAgent1/files
         for file in os.listdir("./data/files"):
             shutil.copyfile("./data/files/" + file, "./test_agents/TestAgent1/files/" + file)
             cls.num_files += 1
@@ -115,39 +119,63 @@
                 return "Test Successful"
 
         cls.TestTool = TestTool
 
         from test_agents.CEO import CEO
         from test_agents.TestAgent1 import TestAgent1
         from test_agents.TestAgent2 import TestAgent2
-        cls.ceo = CEO()
         cls.agent1 = TestAgent1()
-        cls.agent1.add_tool(Retrieval)
+        cls.agent1.add_tool(FileSearch)
+        cls.agent1.truncation_strategy = {
+            "type": "last_messages",
+            "last_messages": 10
+        }
+
         cls.agent2 = TestAgent2()
         cls.agent2.add_tool(cls.TestTool)
 
+        cls.agent2.response_format = {
+            "type": "json_object",
+        }
+
+        cls.ceo = CEO()
+        cls.ceo.examples = [
+            {
+                "role": "user",
+                "content": "Hi!"
+            },
+            {
+                "role": "assistant",
+                "content": "Hi! I am the CEO. I am here to help you with your testing. Please tell me who to send message to."
+            }
+        ]
+
+        cls.ceo.max_completion_tokens = 100
+
     def test_1_init_agency(self):
         """it should initialize agency with agents"""
         self.__class__.agency = Agency([
             self.__class__.ceo,
             [self.__class__.ceo, self.__class__.agent1],
             [self.__class__.agent1, self.__class__.agent2]],
             shared_instructions="This is a shared instruction",
             settings_callbacks=self.__class__.settings_callbacks,
             threads_callbacks=self.__class__.threads_callbacks,
+            temperature=0,
         )
 
         self.check_all_agents_settings()
 
     def test_2_load_agent(self):
         """it should load existing assistant from settings"""
         from test_agents.TestAgent1 import TestAgent1
         agent3 = TestAgent1()
         agent3.add_shared_instructions(self.__class__.agency.shared_instructions)
         agent3.tools = self.__class__.agent1.tools
+        agent3.top_p = self.__class__.agency.top_p
         agent3 = agent3.init_oai()
 
         print("agent3", agent3.assistant.model_dump())
         print("agent1", self.__class__.agent1.assistant.model_dump())
 
         self.assertTrue(self.__class__.agent1.id == agent3.id)
 
@@ -172,25 +200,63 @@
         self.assertTrue(agent3._check_parameters(self.__class__.agent1.assistant.model_dump()))
 
         self.check_agent_settings(agent3)
 
     def test_4_agent_communication(self):
         """it should communicate between agents"""
         print("TestAgent1 tools", self.__class__.agent1.tools)
-        message = self.__class__.agency.get_completion("Please tell TestAgent1 to say test to TestAgent2.", yield_messages=False)
+        message = self.__class__.agency.get_completion("Please tell TestAgent1 to say test to TestAgent2.",
+                                                       tool_choice={"type": "function", "function": {"name": "SendMessage"}})
 
         self.assertFalse('error' in message.lower())
 
         for agent_name, threads in self.__class__.agency.agents_and_threads.items():
             for other_agent_name, thread in threads.items():
                 self.assertTrue(thread.id in self.__class__.loaded_thread_ids[agent_name][other_agent_name])
 
         for agent in self.__class__.agency.agents:
             self.assertTrue(agent.id in [settings['id'] for settings in self.__class__.loaded_agents_settings])
 
+        # assistants v2 checks
+        main_thread = self.__class__.agency.main_thread
+        main_thread_id = main_thread.id
+
+        thread_messages = self.__class__.client.beta.threads.messages.list(main_thread_id, limit=100, order="asc")
+
+        self.assertTrue(len(thread_messages.data) == 4)
+
+        self.assertTrue(thread_messages.data[0].content[0].text.value == "Hi!")
+
+        run = main_thread.run
+        self.assertTrue(run.max_prompt_tokens == self.__class__.ceo.max_prompt_tokens)
+        self.assertTrue(run.max_completion_tokens == self.__class__.ceo.max_completion_tokens)
+        self.assertTrue(run.tool_choice.type == "function")
+
+        agent1_thread = self.__class__.agency.agents_and_threads[self.__class__.ceo.name][self.__class__.agent1.name]
+
+        agent1_thread_id = agent1_thread.id
+
+        agent1_thread_messages = self.__class__.client.beta.threads.messages.list(agent1_thread_id, limit=100)
+
+        self.assertTrue(len(agent1_thread_messages.data) == 2)
+
+        agent1_run = agent1_thread.run
+
+        self.assertTrue(agent1_run.truncation_strategy.type == "last_messages")
+        self.assertTrue(agent1_run.truncation_strategy.last_messages == 10)
+
+        agent2_thread = self.__class__.agency.agents_and_threads[self.__class__.agent1.name][self.__class__.agent2.name]
+
+        agent2_message = agent2_thread._get_last_message_text()
+
+        try:
+            json.loads(agent2_message)
+        except json.JSONDecodeError as e:
+            self.assertTrue(False)
+
     def test_5_agent_communication_stream(self):
         """it should communicate between agents using streaming"""
         print("TestAgent1 tools", self.__class__.agent1.tools)
 
         test_tool_used = False
         test_agent2_used = False
 
@@ -207,15 +273,16 @@
                     nonlocal test_tool_used
                     test_tool_used = True
 
         message = self.__class__.agency.get_completion_stream(
             "Please tell TestAgent1 to tell TestAgent 2 to use test tool.",
             event_handler=EventHandler,
             additional_instructions="Your message to TestAgent1 should be exactly as follows: "
-                                    "'Please tell TestAgent2 to use test tool.'",)
+                                    "'Please tell TestAgent2 to use test tool.'",
+            tool_choice={"type": "function", "function": {"name": "SendMessage"}})
 
         # self.assertFalse('error' in message.lower())
 
         self.assertTrue(test_tool_used)
         self.assertTrue(test_agent2_used)
 
         self.assertTrue(self.__class__.TestTool.shared_state.get("test_tool_used"))
@@ -234,29 +301,40 @@
         previous_loaded_thread_ids = self.__class__.loaded_thread_ids
         previous_loaded_agents_settings = self.__class__.loaded_agents_settings
 
         from test_agents.CEO import CEO
         from test_agents.TestAgent1 import TestAgent1
         from test_agents.TestAgent2 import TestAgent2
         agent1 = TestAgent1()
-        agent1.add_tool(Retrieval)
+        agent1.add_tool(FileSearch)
+
+        agent1.truncation_strategy = {
+            "type": "last_messages",
+            "last_messages": 10
+        }
+
         agent2 = TestAgent2()
         agent2.add_tool(self.__class__.TestTool)
 
+        agent2.response_format = {
+            "type": "json_object",
+        }
+
         ceo = CEO()
 
         # check that agents are loaded
         agency = Agency([
             ceo,
             [ceo, agent1],
             [agent1, agent2]],
             shared_instructions="This is a shared instruction",
             settings_path="./settings2.json",
             settings_callbacks=self.__class__.settings_callbacks,
             threads_callbacks=self.__class__.threads_callbacks,
+            temperature=0,
         )
 
         # check that settings are the same
         self.assertTrue(len(agency.agents) == len(self.__class__.agency.agents))
 
         os.remove("settings.json")
         os.rename("settings2.json", "settings.json")
@@ -279,43 +357,48 @@
         # reset loaded thread ids
         self.__class__.loaded_thread_ids = {}
 
         self.__class__.agency = Agency([
             self.__class__.ceo,
             [self.__class__.ceo, self.__class__.agent1],
             [self.__class__.agent1, self.__class__.agent2]],
-            shared_instructions="This is a shared instruction",
+            shared_instructions="",
             settings_callbacks=self.__class__.settings_callbacks,
             threads_callbacks=self.__class__.threads_callbacks,
             async_mode='threading',
+            temperature=0,
         )
 
         self.check_all_agents_settings(True)
 
     def test_8_async_agent_communication(self):
         """it should communicate between agents asynchronously"""
         print("TestAgent1 tools", self.__class__.agent1.tools)
-        self.__class__.agency.get_completion("Please tell TestAgent1 to say test to TestAgent2.",
-                                                       yield_messages=False)
+        self.__class__.agency.get_completion("Please tell TestAgent2 hello.",
+                                             tool_choice={"type": "function", "function": {"name": "SendMessage"}},
+                                             recipient_agent=self.__class__.agent1)
 
         time.sleep(10)
 
-        message = self.__class__.agency.get_completion("Please check response. If the GetResponse function output includes `TestAgent1's Response` (for example, that the message was sent to Test Agent 2, the process or the task has started, initiated, etc.), say 'success'. If the function output does not include `TestAgent1's Response`, or if you get a System Notification, or an error instead, say 'error'.",
-                                                       yield_messages=False)
-
-        self.assertFalse('error' in message.lower())
+        message = self.__class__.agency.get_completion(
+            "Please check response. If output includes `TestAgent2's Response`, say 'success'. If the function output does not include `TestAgent2's Response`, or if you get a System Notification, or an error instead, say 'error'.",
+            tool_choice={"type": "function", "function": {"name": "GetResponse"}},
+            recipient_agent=self.__class__.agent1)
+
+        if 'error' in message.lower():
+            print(self.__class__.agency.get_completion("Explain why you said error."))
+            self.assertFalse('error' in message.lower())
 
         for agent_name, threads in self.__class__.agency.agents_and_threads.items():
             for other_agent_name, thread in threads.items():
                 self.assertTrue(thread.id in self.__class__.loaded_thread_ids[agent_name][other_agent_name])
 
         for agent in self.__class__.agency.agents:
             self.assertTrue(agent.id in [settings['id'] for settings in self.__class__.loaded_agents_settings])
 
-
     # --- Helper methods ---
 
     def get_class_folder_path(self):
         return os.path.abspath(os.path.dirname(inspect.getfile(self.__class__)))
 
     def check_agent_settings(self, agent, async_mode=False):
         try:
@@ -328,36 +411,45 @@
                         self.assertTrue(agent._check_parameters(assistant_settings))
 
             assistant = agent.assistant
             self.assertTrue(assistant)
             self.assertTrue(agent._check_parameters(assistant.model_dump()))
             if agent.name == "TestAgent1":
                 num_tools = 3 if not async_mode else 4
-                self.assertTrue(len(assistant.file_ids) == self.__class__.num_files)
-                for file_id in assistant.file_ids:
-                    self.assertTrue(file_id in agent.file_ids)
+
+                self.assertTrue(len(assistant.tool_resources.model_dump()['code_interpreter']['file_ids']) == 3)
+                self.assertTrue(len(assistant.tool_resources.model_dump()['file_search']['vector_store_ids']) == 1)
+
+                vector_store_id = assistant.tool_resources.model_dump()['file_search']['vector_store_ids'][0]
+                vector_store_files = agent.client.beta.vector_stores.files.list(
+                    vector_store_id=vector_store_id
+                )
+
+                file_ids = [file.id for file in vector_store_files.data]
+
+                self.assertTrue(len(file_ids) == 5)
                 # check retrieval tools is there
-                print("assistant tools", assistant.tools)
                 self.assertTrue(len(assistant.tools) == num_tools)
                 self.assertTrue(len(agent.tools) == num_tools)
                 self.assertTrue(assistant.tools[0].type == "code_interpreter")
-                self.assertTrue(assistant.tools[1].type == "retrieval")
+                self.assertTrue(assistant.tools[1].type == "file_search")
                 self.assertTrue(assistant.tools[2].type == "function")
                 self.assertTrue(assistant.tools[2].function.name == "SendMessage")
                 if async_mode:
                     self.assertTrue(assistant.tools[3].type == "function")
                     self.assertTrue(assistant.tools[3].function.name == "GetResponse")
             elif agent.name == "TestAgent2":
                 self.assertTrue(len(assistant.tools) == self.__class__.num_schemas + 1)
                 for tool in assistant.tools:
                     self.assertTrue(tool.type == "function")
                     self.assertTrue(tool.function.name in [tool.__name__ for tool in agent.tools])
             elif agent.name == "CEO":
                 num_tools = 1 if not async_mode else 2
-                self.assertTrue(len(assistant.file_ids) == 0)
+                self.assertFalse(assistant.tool_resources.code_interpreter)
+                self.assertFalse(assistant.tool_resources.file_search)
                 self.assertTrue(len(assistant.tools) == num_tools)
             else:
                 pass
         except Exception as e:
             print("Error checking agent settings ", agent.name)
             raise e
 
@@ -366,14 +458,12 @@
         self.check_agent_settings(self.__class__.agent1, async_mode=async_mode)
         self.check_agent_settings(self.__class__.agent2, async_mode=async_mode)
 
     @classmethod
     def tearDownClass(cls):
         shutil.rmtree("./test_agents")
         os.remove("./settings.json")
-        cls.ceo.delete()
-        cls.agent1.delete()
-        cls.agent2.delete()
+        cls.agency.delete()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `agency-swarm-0.1.7/tests/test_tool_factory.py` & `agency_swarm-0.2.0/tests/test_tool_factory.py`

 * *Files identical despite different names*

