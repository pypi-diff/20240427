# Comparing `tmp/m3-cli-3.101.5.tar.gz` & `tmp/m3_cli-3.112.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-cli-3.101.5.tar", last modified: Mon Dec 11 09:54:23 2023, max compression
+gzip compressed data, was "m3_cli-3.112.4.tar", last modified: Sat Apr 27 07:14:54 2024, max compression
```

## Comparing `m3-cli-3.101.5.tar` & `m3_cli-3.112.4.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.905221 m3-cli-3.101.5/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11357 2023-12-11 09:54:18.000000 m3-cli-3.101.5/LICENSE
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    24877 2023-12-11 09:54:23.905221 m3-cli-3.101.5/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    24114 2023-12-11 09:54:18.000000 m3-cli-3.101.5/README.md
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.889221 m3-cli-3.101.5/m3_cli.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    24877 2023-12-11 09:54:23.000000 m3-cli-3.101.5/m3_cli.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4564 2023-12-11 09:54:23.000000 m3-cli-3.101.5/m3_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-12-11 09:54:23.000000 m3-cli-3.101.5/m3_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       35 2023-12-11 09:54:23.000000 m3-cli-3.101.5/m3_cli.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      186 2023-12-11 09:54:23.000000 m3-cli-3.101.5/m3_cli.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        6 2023-12-11 09:54:23.000000 m3-cli-3.101.5/m3_cli.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.817220 m3-cli-3.101.5/m3cli/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   158180 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/commands_def.json
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25054 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/commands_help.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.817220 m3-cli-3.101.5/m3cli/connections/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/connections/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4808 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/connections/rabbitmq_connection.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.817220 m3-cli-3.101.5/m3cli/docs/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/docs/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2715 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/docs/docs_generator.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6628 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.833220 m3-cli-3.101.5/m3cli/m3cli_complete/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      437 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3cli_complete/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      669 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3cli_complete/access_meta.json
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7280 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3cli_complete/autocomplete_setup.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      743 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3cli_complete/bash_m3cli_complete.sh
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6560 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3cli_complete/m3cli_complete.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      850 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/m3cli_complete/zsh_m3cli_complete.sh
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.833220 m3-cli-3.101.5/m3cli/models/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/models/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1844 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/models/interactive_parameter.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.881221 m3-cli-3.101.5/m3cli/plugins/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      857 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/activate-platform-service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      560 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/activate-vlan.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      351 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/add-schedule-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      627 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/add-service-section.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      985 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/apply-terraform-template.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      445 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/aws-management-console.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      498 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/azure-management-console.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.881221 m3-cli-3.101.5/m3cli/plugins/common/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/common/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1220 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/common/schedule_instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3261 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/cost-object-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1354 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/cost-usage-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      552 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/create-image.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      476 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/create-instance-quota.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2689 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/create-key.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1817 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/create-schedule.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      538 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/create-storage-quota.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      347 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/deactivate-platform-service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      400 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/deactivate-vlan.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1895 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/decrypt-password.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      358 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/delete-schedule-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      935 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/delete-service-section.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1023 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/delete-storage.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1286 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/delete-tags.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      564 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/delete-terraform-template.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      954 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-events.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      778 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-images.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1314 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-insights.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      565 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-instance-quota.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3078 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1241 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-keys.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1075 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-platform-service-stacks.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      736 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-platform-services.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      528 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-resources.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1283 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-schedules.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      704 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-script.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      555 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-service-section.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      491 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-shapes.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      475 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-storage-quota.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      889 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-storages.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1246 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-tags.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1047 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-tenants.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      911 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-terraform-stacks.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      686 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-terraform-templates.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      419 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/describe-user-permissions.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      618 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/destroy-terraform-stack.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      153 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/detach-storage.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      500 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/google-management-console.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1898 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/health-check.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1011 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/hourly-report-softline.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1027 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/hourly-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1795 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/import-key.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1550 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/manage-key.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      169 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/manage-termination-protection.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      397 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/move-to-vlan.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      879 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/multitenant-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      983 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/plan-terraform-template.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1608 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/price.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1276 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/publish-platform-service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      854 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/reboot-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      421 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/release-ip.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3070 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/resource-report-softline.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3064 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/resource-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1982 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/run-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1278 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/set-tags.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      854 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/start-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      854 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/stop-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2964 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/subtotal-report-softline.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3034 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/subtotal-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      854 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/terminate-instances.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2598 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/total-report-softline.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2620 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/total-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2903 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/untagged-resource-report.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      900 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/update-platform-service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      708 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/upload-script.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1174 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/upload-terraform-template-from-git.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1341 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/upload-terraform-template.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.881221 m3-cli-3.101.5/m3cli/plugins/utils/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/utils/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2456 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/plugins/utils/plugin_utilities.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.889221 m3-cli-3.101.5/m3cli/services/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1753 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/aes_cipher_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27842 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/commands_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1748 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/environment_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1845 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/help_client.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7005 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactive_options_service.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.889221 m3-cli-3.101.5/m3cli/services/interactivity/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      419 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       84 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/constants.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2229 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/interactive_input_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1822 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/parameters_provider.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2245 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/remote_validation_service.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.889221 m3-cli-3.101.5/m3cli/services/interactivity/varfile/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/varfile/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4408 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/interactivity/varfile/varfile_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3296 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/plugin_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2875 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/rabbitmq_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8814 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/request_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19300 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/response_processor_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      602 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/response_utils.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17203 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/services/validation_service.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-12-11 09:54:23.889221 m3-cli-3.101.5/m3cli/utils/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      771 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/utils/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1199 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/utils/cloud_utils.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10411 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/utils/decorators.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      643 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/utils/interactivity_utils.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4850 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/utils/logger.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11336 2023-12-11 09:54:18.000000 m3-cli-3.101.5/m3cli/utils/utilities.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-12-11 09:54:18.000000 m3-cli-3.101.5/pyproject.toml
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1062 2023-12-11 09:54:23.905221 m3-cli-3.101.5/setup.cfg
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      380 2023-12-11 09:54:18.000000 m3-cli-3.101.5/setup.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.588274 m3_cli-3.112.4/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    11357 2024-04-27 07:14:49.000000 m3_cli-3.112.4/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    24877 2024-04-27 07:14:54.588274 m3_cli-3.112.4/PKG-INFO
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    24114 2024-04-27 07:14:49.000000 m3_cli-3.112.4/README.md
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.588274 m3_cli-3.112.4/m3_cli.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    24877 2024-04-27 07:14:54.000000 m3_cli-3.112.4/m3_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4564 2024-04-27 07:14:54.000000 m3_cli-3.112.4/m3_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        1 2024-04-27 07:14:54.000000 m3_cli-3.112.4/m3_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       35 2024-04-27 07:14:54.000000 m3_cli-3.112.4/m3_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      186 2024-04-27 07:14:54.000000 m3_cli-3.112.4/m3_cli.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        6 2024-04-27 07:14:54.000000 m3_cli-3.112.4/m3_cli.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.552272 m3_cli-3.112.4/m3cli/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)   160183 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/commands_def.json
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    25865 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/commands_help.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.552272 m3_cli-3.112.4/m3cli/connections/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/connections/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4808 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/connections/rabbitmq_connection.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.552272 m3_cli-3.112.4/m3cli/docs/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/docs/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2715 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/docs/docs_generator.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     6604 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.556272 m3_cli-3.112.4/m3cli/m3cli_complete/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      437 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3cli_complete/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      669 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3cli_complete/access_meta.json
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7280 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3cli_complete/autocomplete_setup.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      743 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3cli_complete/bash_m3cli_complete.sh
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     6560 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3cli_complete/m3cli_complete.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      850 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/m3cli_complete/zsh_m3cli_complete.sh
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.560273 m3_cli-3.112.4/m3cli/models/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/models/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1844 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/models/interactive_parameter.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.580274 m3_cli-3.112.4/m3cli/plugins/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      857 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/activate-platform-service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      560 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/activate-vlan.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      351 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/add-schedule-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      627 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/add-service-section.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1006 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/apply-terraform-template.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      445 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/aws-management-console.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      498 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/azure-management-console.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.580274 m3_cli-3.112.4/m3cli/plugins/common/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/common/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1220 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/common/schedule_instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3261 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/cost-object-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1354 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/cost-usage-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      552 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/create-image.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      476 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/create-instance-quota.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2689 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/create-key.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1817 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/create-schedule.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      538 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/create-storage-quota.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      347 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/deactivate-platform-service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      400 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/deactivate-vlan.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1895 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/decrypt-password.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      358 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/delete-schedule-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      935 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/delete-service-section.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      744 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/delete-storage.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1286 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/delete-tags.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      564 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/delete-terraform-template.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      954 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-events.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      778 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-images.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1314 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-insights.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      565 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-instance-quota.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3078 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1241 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-keys.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1075 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-platform-service-stacks.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      736 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-platform-services.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      528 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-resources.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1283 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-schedules.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      704 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-script.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      555 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-service-section.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      491 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-shapes.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      475 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-storage-quota.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      889 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-storages.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1246 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-tags.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1047 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-tenants.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      911 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-terraform-stacks.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      686 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-terraform-templates.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      419 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/describe-user-permissions.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      618 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/destroy-terraform-stack.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      153 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/detach-storage.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      500 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/google-management-console.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1898 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/health-check.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1011 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/hourly-report-softline.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1027 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/hourly-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1795 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/import-key.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1550 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/manage-key.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      169 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/manage-termination-protection.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      397 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/move-to-vlan.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      879 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/multitenant-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1005 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/plan-terraform-template.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1608 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/price.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1276 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/publish-platform-service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      854 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/reboot-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      421 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/release-ip.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3070 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/resource-report-softline.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3064 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/resource-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1982 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/run-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1278 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/set-tags.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      854 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/start-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      854 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/stop-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2964 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/subtotal-report-softline.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3034 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/subtotal-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      854 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/terminate-instances.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2598 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/total-report-softline.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2620 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/total-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2903 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/untagged-resource-report.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      900 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/update-platform-service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      708 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/upload-script.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1174 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/upload-terraform-template-from-git.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1341 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/upload-terraform-template.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.580274 m3_cli-3.112.4/m3cli/plugins/utils/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/utils/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2456 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/plugins/utils/plugin_utilities.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.584274 m3_cli-3.112.4/m3cli/services/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1753 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/aes_cipher_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    28230 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/commands_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1748 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/environment_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1845 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/help_client.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     7284 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactive_options_service.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.584274 m3_cli-3.112.4/m3cli/services/interactivity/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      419 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       84 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/constants.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2229 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/interactive_input_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1826 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/parameters_provider.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2465 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/remote_validation_service.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.584274 m3_cli-3.112.4/m3cli/services/interactivity/varfile/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/varfile/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4408 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/interactivity/varfile/varfile_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     3296 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/plugin_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     2875 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/rabbitmq_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     8836 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/request_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    19300 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/response_processor_service.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      602 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/response_utils.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    17310 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/services/validation_service.py
+drwxrwxr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-27 07:14:54.588274 m3_cli-3.112.4/m3cli/utils/
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      771 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/utils/__init__.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1199 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/utils/cloud_utils.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    10508 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/utils/decorators.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      643 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/utils/interactivity_utils.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     4850 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/utils/logger.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)    11192 2024-04-27 07:14:49.000000 m3_cli-3.112.4/m3cli/utils/utilities.py
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)       86 2024-04-27 07:14:49.000000 m3_cli-3.112.4/pyproject.toml
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)     1062 2024-04-27 07:14:54.588274 m3_cli-3.112.4/setup.cfg
+-rw-rw-r--   0 jenkins   (1002) jenkins   (1002)      380 2024-04-27 07:14:49.000000 m3_cli-3.112.4/setup.py
```

### Comparing `m3-cli-3.101.5/LICENSE` & `m3_cli-3.112.4/LICENSE`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/PKG-INFO` & `m3_cli-3.112.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-cli
-Version: 3.101.5
+Version: 3.112.4
 Summary: The Maestro3 Command Line Interface (CLI) is a unified tool to manage your Maestro services and resources
 Home-page: https://github.com/Maestro-Cloud-Control/m3-cli
 Author: maestrocloudcontrol
 Author-email: support@maestrocontrol.cloud
 Keywords: Maestro3,Command Line Interface,CLI,CLOUD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `m3-cli-3.101.5/README.md` & `m3_cli-3.112.4/README.md`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3_cli.egg-info/PKG-INFO` & `m3_cli-3.112.4/m3_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-cli
-Version: 3.101.5
+Version: 3.112.4
 Summary: The Maestro3 Command Line Interface (CLI) is a unified tool to manage your Maestro services and resources
 Home-page: https://github.com/Maestro-Cloud-Control/m3-cli
 Author: maestrocloudcontrol
 Author-email: support@maestrocontrol.cloud
 Keywords: Maestro3,Command Line Interface,CLI,CLOUD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `m3-cli-3.101.5/m3_cli.egg-info/SOURCES.txt` & `m3_cli-3.112.4/m3_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/commands_def.json` & `m3_cli-3.112.4/m3cli/commands_def.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995304702531265%*

 * *Differences: {"'commands'": "{'run-instances': {'parameters': {'script': OrderedDict([('alias', 'scname'), "*

 * *               "('api_param_name', 'User script'), ('help', 'The name of the script that will be "*

 * *               "applied'), ('required', False), ('validation', OrderedDict([('type', 'string'), "*

 * *               '(\'regex\', \'^[\\\\w\\\\-._ ]{6,32}$\'), (\'regex_error\', "Script name must be '*

 * *               "6-32 characters long and can include only these characters in lower case: 'a-z', "*

 * *               '\'0-9 […]*

```diff
@@ -304,14 +304,15 @@
                 "tenant": {
                     "parent": "tenant"
                 },
                 "variable": {
                     "alias": "var",
                     "api_param_name": "variables",
                     "help": "Parameters with values. \nFormat - key:value for string; key:\"value1, value2, value3\" for list; key1:\"key2=value2\" for object",
+                    "multiple_values": true,
                     "required": false,
                     "validation": {
                         "properties": {
                             "key": {
                                 "type": "string"
                             },
                             "value": {
@@ -326,15 +327,15 @@
         "associate-ip": {
             "alias": "asip",
             "api_action": "ASSOCIATE_IP",
             "groups": [
                 "instance-management",
                 "email-on_run_instance-group"
             ],
-            "help": "Associate static ip with instance",
+            "help": "Associate static IP with instance",
             "help_file": true,
             "output_configuration": {
                 "response_table_headers": [
                     "ipAddress",
                     "tenantName",
                     "regionName",
                     "instanceId"
@@ -415,14 +416,44 @@
             },
             "parameters": {
                 "tenant": {
                     "parent": "tenant"
                 }
             }
         },
+        "billing-region-types": {
+            "alias": "brtypes",
+            "api_action": "GET_BILLING_REGION_TYPES",
+            "groups": [
+                "billing-reports",
+                "cli-price-help"
+            ],
+            "help": "Gets billing region types",
+            "help_file": true,
+            "integration_request": false,
+            "integration_response": true,
+            "output_configuration": {
+                "nullable": true,
+                "response_table_headers": [
+                    "regionType",
+                    "regions"
+                ]
+            },
+            "parameters": {
+                "all": {
+                    "alias": "A",
+                    "api_param_name": "all",
+                    "help": "A flag. Includes inactive regions.",
+                    "required": false,
+                    "validation": {
+                        "type": "bool"
+                    }
+                }
+            }
+        },
         "cost-object-report": {
             "alias": "cosobreport",
             "api_action": "GET_RESOURCE_BILLING_REPORT",
             "groups": [
                 "billing-reports",
                 "cli-price-help"
             ],
@@ -1393,27 +1424,29 @@
         },
         "delete-scripts": {
             "alias": "delscr",
             "api_action": "REMOVE_SCRIPT",
             "groups": [
                 "init-script-management"
             ],
-            "help": "Deletes an init script from your library in Maestro",
+            "help": "Deletes the user script from the specific tenant in Maestro",
             "help_file": true,
+            "integration_request": true,
+            "integration_response": true,
             "output_configuration": {
                 "none": true,
                 "response_table_headers": []
             },
             "parameters": {
                 "cloud": {
                     "parent": "cloud"
                 },
                 "script": {
                     "alias": "scname",
-                    "api_param_name": "fileName",
+                    "api_param_name": "fileNames",
                     "help": "List of the name of the file to be deleted. Pass several values in the following format: value1,value2,value3",
                     "required": true,
                     "validation": {
                         "type": "list"
                     }
                 },
                 "tenant": {
@@ -1501,23 +1534,14 @@
                     "validation": {
                         "type": "string"
                     }
                 },
                 "region": {
                     "parent": "region"
                 },
-                "resource-group": {
-                    "alias": "rgname",
-                    "api_param_name": "resourceGroup",
-                    "help": "The resource group name (for Azure)",
-                    "required": false,
-                    "validation": {
-                        "type": "string"
-                    }
-                },
                 "storage-id": {
                     "alias": "storid",
                     "api_param_name": "volumeId",
                     "help": "The ID of storage",
                     "required": true,
                     "validation": {
                         "type": "string"
@@ -2491,15 +2515,15 @@
         },
         "describe-script": {
             "alias": "dscript",
             "api_action": "DESCRIBE_SCRIPT",
             "groups": [
                 "init-script-management"
             ],
-            "help": "Describes the script files uploaded to Maestro and available for your tenant",
+            "help": "Describes the script files uploaded to Maestro and available for the specific tenant",
             "help_file": true,
             "integration_response": true,
             "output_configuration": {
                 "headers_customization": {
                     "fileName": {
                         "header_display_name": "Script"
                     }
@@ -3080,22 +3104,22 @@
                     }
                 },
                 "tenant": {
                     "parent": "tenant"
                 }
             }
         },
-        "diassociate-ip": {
+        "disassociate-ip": {
             "alias": "dsip",
             "api_action": "DISASSOCIATE_IP",
             "groups": [
                 "instance-management",
                 "email-on_run_instance-group"
             ],
-            "help": "Diassociate static ip with instance",
+            "help": "Disassociate static IP from the instance",
             "help_file": true,
             "output_configuration": {
                 "response_table_headers": [
                     "ipAddress",
                     "tenantName",
                     "regionName",
                     "instanceId"
@@ -3564,14 +3588,23 @@
                     "api_param_name": "from",
                     "help": "The start range date. Format \"dd.mm.yyyy\"",
                     "required": true,
                     "validation": {
                         "type": "date"
                     }
                 },
+                "include-billing-source": {
+                    "alias": "ibs",
+                    "api_param_name": "includeBillingSource",
+                    "help": "A flag. Include billing source for public cloud providers",
+                    "required": false,
+                    "validation": {
+                        "type": "bool"
+                    }
+                },
                 "region": {
                     "alias": "r",
                     "api_param_name": "reportZoneType",
                     "case": "upper",
                     "help": "The cloud providers or the region or the report family. Allowed values: [HARDWARE, AWS, AWS_UNREACHABLE, AZURE, AZURE_NATIVE, GOOGLE, MOBILE, ENTERPRISE, SWIFT_STACK, REPORT_PORTAL, WORKSPACES, AWS_WORKSPACES, AZURE_WORKSPACES, AWS_PAAS, AWS_ATLAS, AZURE_PAAS, GOOGLE_PAAS, PRIVATE_PAAS, PRIVATE]",
                     "required": false,
                     "validation": {
@@ -3669,14 +3702,15 @@
                 "tenant": {
                     "parent": "tenant"
                 },
                 "variable": {
                     "alias": "var",
                     "api_param_name": "variables",
                     "help": "The list of parameters with values. \nFormat - key:value for string; key:\"value1, value2, value3\" for list; key1:\"key2=value2\" for object",
+                    "multiple_values": true,
                     "required": false,
                     "validation": {
                         "properties": {
                             "key": {
                                 "type": "string"
                             },
                             "value": {
@@ -4280,14 +4314,25 @@
                     "case": "upper",
                     "help": "The region name",
                     "required": true,
                     "validation": {
                         "type": "string"
                     }
                 },
+                "script": {
+                    "alias": "scname",
+                    "api_param_name": "User script",
+                    "help": "The name of the script that will be applied",
+                    "required": false,
+                    "validation": {
+                        "regex": "^[\\w\\-._ ]{6,32}$",
+                        "regex_error": "Script name must be 6-32 characters long and can include only these characters in lower case: 'a-z', '0-9', .-_ ",
+                        "type": "string"
+                    }
+                },
                 "shape": {
                     "alias": "shname",
                     "api_param_name": "Shape Alias",
                     "case": "upper",
                     "help": "Required in case of InstanceType not specified. Instance shape is a Maestro name of mapped to InstanceType and corresponding attributes in other CPs. Some possible values: LARGE, MICRO, SMALL, etc ",
                     "required": false,
                     "validation": {
@@ -4301,14 +4346,31 @@
                     "required": false,
                     "validation": {
                         "max_value": 720,
                         "min_value": 1,
                         "type": "number"
                     }
                 },
+                "tag": {
+                    "alias": "tag",
+                    "api_param_name": "tags",
+                    "help": "Tags. Pass several values in the following format: key1:val1,key2:val2,key3:val3",
+                    "required": false,
+                    "validation": {
+                        "properties": {
+                            "key": {
+                                "type": "string"
+                            },
+                            "value": {
+                                "type": "string"
+                            }
+                        },
+                        "type": "object"
+                    }
+                },
                 "tenant": {
                     "alias": "tn",
                     "api_param_name": "tenantDisplayName",
                     "case": "upper",
                     "help": "The tenant name",
                     "required": true,
                     "validation": {
@@ -5011,17 +5073,18 @@
         },
         "upload-script": {
             "alias": "upscr",
             "api_action": "UPLOAD_SCRIPT",
             "groups": [
                 "init-script-management"
             ],
-            "help": "Uploads an init script to tenant's library in Maestro",
+            "help": "Uploads the user script to the specific tenant in Maestro",
             "help_file": true,
             "integration_request": true,
+            "integration_response": true,
             "output_configuration": {
                 "headers_customization": {
                     "fileName": {
                         "header_display_name": "Script"
                     }
                 },
                 "response_table_headers": [
@@ -5033,26 +5096,26 @@
             "parameters": {
                 "cloud": {
                     "parent": "cloud"
                 },
                 "script": {
                     "alias": "scname",
                     "api_param_name": "fileName",
-                    "help": "The name of the script that will be uploaded",
+                    "help": "The name of the script to be uploaded. The file extension(.sh, .cmd, ...) will be taken from 'spath'",
                     "required": true,
                     "validation": {
-                        "regex": "^[\\w\\-._ ]{6,32}$",
-                        "regex_error": "Script name must be 6-32 characters long and can include only these characters in lower case: 'a-z', '0-9', .-_ ",
+                        "regex": "^[\\w\\-_ ]{6,32}$",
+                        "regex_error": "Script name must be 6-32 characters long and can include only these characters in lower case: 'a-z', '0-9', -_ ",
                         "type": "string"
                     }
                 },
                 "source-path": {
                     "alias": "spath",
                     "api_param_name": "filepath",
-                    "help": "The path to the file that will be used as a source of the script",
+                    "help": "The path to the script file. The file extension should be either '.sh', '.bat', 'cmd' or '.ps1'",
                     "required": true,
                     "validation": {
                         "file_extensions": [
                             ".sh",
                             ".bat",
                             ".cmd",
                             ".ps1"
```

### Comparing `m3-cli-3.101.5/m3cli/commands_help.py` & `m3_cli-3.112.4/m3cli/commands_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,18 +382,18 @@
 
 run_instances = """
 Creates instances of the specified configuration
 
 Examples:
 
 1. Runs a single instance:
-        m3 run-instances --image <image_name> ---name <instance_name> --key-name <key_name> --number-of-instances <number> --cloud <cloud> --tenant <tenant_name> --region <region_name> --shape <shape_name>
+        m3 run-instances --image <image_name> ---name <instance_name> --key-name <key_name> --number-of-instances <number> --cloud <cloud> --tenant <tenant_name> --region <region_name> --shape <shape_name> --script <script_name> --tag <tag_key1:val1,tag_key2:val2>
 
 2. Runs several instances from one image:
-        m3 run-instances --image <image_nam> --name <instance_name> --key-name <key_name> --number-of-instances <number> --cloud <cloud> --tenant <tenant_name> --region <region_name> --shape <shape_name>
+        m3 run-instances --image <image_nam> --name <instance_name> --key-name <key_name> --number-of-instances <number> --cloud <cloud> --tenant <tenant_name> --region <region_name> --shape <shape_name> --script <script_name> --tag <tag_key1:val1,tag_key2:val2>
 """
 
 set_tags = """
 Updates instance tags. Applicable in public and private clouds
 
 Examples:
 
@@ -459,24 +459,27 @@
 
 apply_terraform_template = """
 Applies a Terraform template
 
 Examples:
 
 1. Applies a Terraform template:
-        m3 apply-terraform-template --cloud <cloud_name> --templateName <name> --tenant <tenant_name>   
+        m3 apply-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name>   
 
 2. Applies a Terraform template with specific parameters for a string:
-        m3 apply-terraform-template --cloud <cloud_name> --templateName <name> --tenant <tenant_name> --variable <key:value> 
+        m3 apply-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:value> 
 
 3. Applies a Terraform template with specific parameters for a list:
-        m3 apply-terraform-template --cloud <cloud_name> --templateName <name> --tenant <tenant_name> --variable <key:"value1, valueN"> 
+        m3 apply-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:"value1, valueN"> 
 
 4. Applies a Terraform template with specific parameters for an object:
-        m3 apply-terraform-template --cloud <cloud_name> --templateName <name> --tenant <tenant_name> --variable <key1:"key2=value2"> 
+        m3 apply-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key1:"key2=value2"> 
+
+5. Applies a Terraform template with multiple values, which can be a combination of strings, lists, and objects:
+        m3 apply-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:value> --variable <key:"value1,valueN"> --variable <key1:"key2=value2">
 """
 
 delete_terraform_template = """
 Deletes a Terraform template
 
 Example:
     m3 delete-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name>  
@@ -509,18 +512,21 @@
 1. Plans a Terraform template:
         m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name>
 
 2. Plans a Terraform template with a specific value for a string:
         m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:value>
 
 3. Plans a Terraform template with a specific value for a list:
-        m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:value1, valueN>
+        m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:"value1,valueN">
 
 4. Plans a Terraform template with a specific value for an object:
-        m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key1:"key2=value2"> 
+        m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key1:"key2=value2">
+        
+5. Plans a Terraform template with multiple values, which can be a combination of strings, lists, and objects:
+        m3 plan-terraform-template --cloud <cloud_name> --template <name> --tenant <tenant_name> --variable <key:value> --variable <key:"value1,valueN">
 """
 
 total_report = """
 Gets a total billing report for a tenant
 
 Example:
         m3 total-report --tenant-group <tenant_group_name> --from <dd.mm.yyyy> --to <dd.mm.yyyy>
@@ -661,26 +667,33 @@
 associate_ip = """
 Associate specific static IP with instance:
 
 Example:
         m3 associate-ip --tenant <tenant_name> --region <region_name> --static-ip <ip> --instance-id <instance_id>
 """
 
-diassociate_ip = """
-Associate specific static IP with instance:
+disassociate_ip = """
+Disassociate specific static IP from the instance:
 
 Example:
-        m3 diassociate-ip --tenant <tenant_name> --region <region_name> --static-ip <ip>
+        m3 disassociate-ip --tenant <tenant_name> --region <region_name> --static-ip <ip>
 """
 
 multitenant_report = """
 Gets multitenant billing report
     
 Example:
-    m3 multitenant-report --from <dd.mm.yyyy> --to <dd.mm.yyyy> --region <region_zone> --report-type <report_type>
+    m3 multitenant-report --from <dd.mm.yyyy> --to <dd.mm.yyyy> --region <region_zone> --report-type <report_type> --include-billing-source
+"""
+
+billing_region_types = """
+Gets billing region types
+
+Example:
+    m3 billing-region-types --all
 """
 
 upload_terraform_template_from_git = """
 Uploads a Terraform template from Git
 
 Example:
     m3 upload-terraform-template-from-git --branch <branch_name> --cloud <cloud>
```

### Comparing `m3-cli-3.101.5/m3cli/connections/rabbitmq_connection.py` & `m3_cli-3.112.4/m3cli/connections/rabbitmq_connection.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/docs/docs_generator.py` & `m3_cli-3.112.4/m3cli/docs/docs_generator.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/m3.py` & `m3_cli-3.112.4/m3cli/m3.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from m3cli.utils import HEALTH_CHECK_CMD_NAME
 from m3cli.utils.decorators import (cli_response, dynamic_dispatcher)
 from m3cli.utils.logger import exception_handler_formatter
 from m3cli.utils.utilities import perform_version_check
 
 sys.excepthook = exception_handler_formatter
 
-CONTEXT_SETTINGS = dict(allow_extra_args=True,
-                        ignore_unknown_options=True)
+CONTEXT_SETTINGS = dict(allow_extra_args=True, ignore_unknown_options=True)
 
 
 @cli_response(no_output=True)
 def init_commands_service():
     cmd_service = CommandsService(m3cli_path=get_root_dir_path(),
                                   validation_service=ValidationService())
     return cmd_service
```

### Comparing `m3-cli-3.101.5/m3cli/m3cli_complete/access_meta.json` & `m3_cli-3.112.4/m3cli/m3cli_complete/access_meta.json`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/m3cli_complete/autocomplete_setup.py` & `m3_cli-3.112.4/m3cli/m3cli_complete/autocomplete_setup.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/m3cli_complete/bash_m3cli_complete.sh` & `m3_cli-3.112.4/m3cli/m3cli_complete/bash_m3cli_complete.sh`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/m3cli_complete/m3cli_complete.py` & `m3_cli-3.112.4/m3cli/m3cli_complete/m3cli_complete.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/m3cli_complete/zsh_m3cli_complete.sh` & `m3_cli-3.112.4/m3cli/m3cli_complete/zsh_m3cli_complete.sh`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/models/interactive_parameter.py` & `m3_cli-3.112.4/m3cli/models/interactive_parameter.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/activate-platform-service.py` & `m3_cli-3.112.4/m3cli/plugins/activate-platform-service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/activate-vlan.py` & `m3_cli-3.112.4/m3cli/plugins/activate-vlan.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/add-service-section.py` & `m3_cli-3.112.4/m3cli/plugins/add-service-section.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/apply-terraform-template.py` & `m3_cli-3.112.4/m3cli/plugins/apply-terraform-template.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 """
 
 
 def create_custom_request(request):
     request.parameters['task'] = 'PLAN'
     if request.parameters.get('variables'):
         variables = request.parameters.pop('variables')
-        value = list(variables.values())[0]
-        if ',' in value:
-            type = 'LIST'
-            value = value.replace(' ', '').strip('][').split(',')
-        elif '=' in value:
-            type = 'MAP'
-            temp = value.replace(' ', '').split('=')
-            value = {temp[0]: temp[-1]}
-        else:
-            type = 'STRING'
-        name = list(variables.keys())[0]
-        request.parameters['variables'] = {
-            name: {
+        request.parameters['variables'] = {}
+        for name, value in variables.items():
+            if ',' in value:
+                type = 'LIST'
+                value = value.replace(' ', '').strip('][').split(',')
+            elif '=' in value:
+                type = 'MAP'
+                temp = value.replace(' ', '').split('=')
+                value = {temp[0]: temp[-1]}
+            else:
+                type = 'STRING'
+            request.parameters['variables'][name] = {
                 'type': type,
                 'value': value,
                 'sensitive': True,
                 'name': name
             }
-        }
     return request
-
```

### Comparing `m3-cli-3.101.5/m3cli/plugins/common/schedule_instances.py` & `m3_cli-3.112.4/m3cli/plugins/common/schedule_instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/cost-object-report.py` & `m3_cli-3.112.4/m3cli/plugins/cost-object-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/cost-usage-report.py` & `m3_cli-3.112.4/m3cli/plugins/cost-usage-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/create-image.py` & `m3_cli-3.112.4/m3cli/plugins/create-image.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/create-key.py` & `m3_cli-3.112.4/m3cli/plugins/create-key.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/create-schedule.py` & `m3_cli-3.112.4/m3cli/plugins/create-schedule.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/create-storage-quota.py` & `m3_cli-3.112.4/m3cli/plugins/create-storage-quota.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/decrypt-password.py` & `m3_cli-3.112.4/m3cli/plugins/decrypt-password.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/delete-service-section.py` & `m3_cli-3.112.4/m3cli/plugins/delete-service-section.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/delete-storage.py` & `m3_cli-3.112.4/m3cli/plugins/delete-storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,14 @@
 
 def create_custom_request(request):
     params = request.parameters
     region = params['region']
     cloud = region.split('-')[0]
 
     additional_params = {}
-    if cloud == 'AZURE':
-        resource_group = params.get('resourceGroup')
-        if not resource_group:
-            raise AssertionError(
-                'Parameter resource-group is required for AZURE cloud')
-        additional_params['resourceGroupName'] = resource_group
     if cloud == 'GCP' or cloud == 'GGL':
         availability_zone = params.get('availabilityZone')
         if not availability_zone:
             raise AssertionError(
                 'Parameter availability-zone is required for GOOGLE cloud')
         additional_params['availabilityZone'] = availability_zone
     params['params'] = additional_params
```

### Comparing `m3-cli-3.101.5/m3cli/plugins/delete-tags.py` & `m3_cli-3.112.4/m3cli/plugins/delete-tags.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/delete-terraform-template.py` & `m3_cli-3.112.4/m3cli/plugins/delete-terraform-template.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-events.py` & `m3_cli-3.112.4/m3cli/plugins/describe-events.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-images.py` & `m3_cli-3.112.4/m3cli/plugins/describe-images.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-insights.py` & `m3_cli-3.112.4/m3cli/plugins/describe-insights.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-instance-quota.py` & `m3_cli-3.112.4/m3cli/plugins/describe-instance-quota.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-instances.py` & `m3_cli-3.112.4/m3cli/plugins/describe-instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-keys.py` & `m3_cli-3.112.4/m3cli/plugins/describe-keys.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-platform-service-stacks.py` & `m3_cli-3.112.4/m3cli/plugins/describe-platform-service-stacks.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-platform-services.py` & `m3_cli-3.112.4/m3cli/plugins/describe-platform-services.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-resources.py` & `m3_cli-3.112.4/m3cli/plugins/describe-resources.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-schedules.py` & `m3_cli-3.112.4/m3cli/plugins/describe-schedules.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-script.py` & `m3_cli-3.112.4/m3cli/plugins/describe-script.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-service-section.py` & `m3_cli-3.112.4/m3cli/plugins/describe-service-section.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-storages.py` & `m3_cli-3.112.4/m3cli/plugins/describe-storages.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-tags.py` & `m3_cli-3.112.4/m3cli/plugins/describe-tags.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-tenants.py` & `m3_cli-3.112.4/m3cli/plugins/describe-tenants.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-terraform-stacks.py` & `m3_cli-3.112.4/m3cli/plugins/describe-terraform-stacks.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/describe-terraform-templates.py` & `m3_cli-3.112.4/m3cli/plugins/describe-terraform-templates.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/destroy-terraform-stack.py` & `m3_cli-3.112.4/m3cli/plugins/destroy-terraform-stack.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/health-check.py` & `m3_cli-3.112.4/m3cli/plugins/health-check.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/hourly-report-softline.py` & `m3_cli-3.112.4/m3cli/plugins/hourly-report-softline.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/hourly-report.py` & `m3_cli-3.112.4/m3cli/plugins/hourly-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/import-key.py` & `m3_cli-3.112.4/m3cli/plugins/import-key.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/manage-key.py` & `m3_cli-3.112.4/m3cli/plugins/manage-key.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/multitenant-report.py` & `m3_cli-3.112.4/m3cli/plugins/multitenant-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/plan-terraform-template.py` & `m3_cli-3.112.4/m3cli/plugins/plan-terraform-template.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 """
 
 
 def create_custom_request(request):
     request.parameters['task'] = 'PLAN'
     if request.parameters.get('variables'):
         variables = request.parameters.pop('variables')
-        value = list(variables.values())[0]
-        if ',' in value:
-            type = 'LIST'
-            value = value.replace(' ', '').strip('][').split(',')
-        elif '=' in value:
-            type = 'MAP'
-            temp = value.replace(' ', '').split('=')
-            value = {temp[0]: temp[-1]}
-        else:
-            type = 'STRING'
-        name = list(variables.keys())[0]
-        request.parameters['variables'] = {
-            name: {
+        request.parameters['variables'] = {}
+        for name, value in variables.items():
+            if ',' in value:
+                type = 'LIST'
+                value = value.replace(' ', '').strip('][').split(',')
+            elif '=' in value:
+                type = 'MAP'
+                temp = value.replace(' ', '').split('=')
+                value = {temp[0]: temp[-1]}
+            else:
+                type = 'STRING'
+            request.parameters['variables'][name] = {
                 'type': type,
                 'value': value,
                 'sensitive': True,
                 'name': name
             }
-        }
     return request
```

### Comparing `m3-cli-3.101.5/m3cli/plugins/price.py` & `m3_cli-3.112.4/m3cli/plugins/price.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/publish-platform-service.py` & `m3_cli-3.112.4/m3cli/plugins/publish-platform-service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/reboot-instances.py` & `m3_cli-3.112.4/m3cli/plugins/reboot-instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/resource-report-softline.py` & `m3_cli-3.112.4/m3cli/plugins/resource-report-softline.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/resource-report.py` & `m3_cli-3.112.4/m3cli/plugins/resource-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/run-instances.py` & `m3_cli-3.112.4/m3cli/plugins/run-instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/set-tags.py` & `m3_cli-3.112.4/m3cli/plugins/set-tags.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/start-instances.py` & `m3_cli-3.112.4/m3cli/plugins/start-instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/stop-instances.py` & `m3_cli-3.112.4/m3cli/plugins/stop-instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/subtotal-report-softline.py` & `m3_cli-3.112.4/m3cli/plugins/subtotal-report-softline.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/subtotal-report.py` & `m3_cli-3.112.4/m3cli/plugins/subtotal-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/terminate-instances.py` & `m3_cli-3.112.4/m3cli/plugins/terminate-instances.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/total-report-softline.py` & `m3_cli-3.112.4/m3cli/plugins/total-report-softline.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/total-report.py` & `m3_cli-3.112.4/m3cli/plugins/total-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/untagged-resource-report.py` & `m3_cli-3.112.4/m3cli/plugins/untagged-resource-report.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/update-platform-service.py` & `m3_cli-3.112.4/m3cli/plugins/update-platform-service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/upload-script.py` & `m3_cli-3.112.4/m3cli/plugins/upload-script.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/upload-terraform-template-from-git.py` & `m3_cli-3.112.4/m3cli/plugins/upload-terraform-template-from-git.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/upload-terraform-template.py` & `m3_cli-3.112.4/m3cli/plugins/upload-terraform-template.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/plugins/utils/plugin_utilities.py` & `m3_cli-3.112.4/m3cli/plugins/utils/plugin_utilities.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/aes_cipher_service.py` & `m3_cli-3.112.4/m3cli/services/aes_cipher_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/commands_service.py` & `m3_cli-3.112.4/m3cli/services/commands_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 from copy import copy
 from os.path import expanduser
+from typing import Any
 
 from tabulate import tabulate
 
 from m3cli.services.environment_service import (get_configuration_folder_path,
                                                 CONFIGURATION_FOLDER_PATH)
 from m3cli.services.interactive_options_service import \
     INTERACTIVE_OPTIONS_ATTRIBUTE
@@ -391,15 +392,18 @@
         for cmd_name, cmd_def in commands_def.items():
             alias = cmd_def.get(ALIAS_KEY)
             if alias and command_name == alias:
                 command_name = cmd_name
                 return command_name, cmd_def
         return command_name, None
 
-    def get_secure_params(self, command):
+    def get_secure_params(
+            self,
+            command: str,
+    ) -> list[str | Any]:
         """
         Look for parameters to be encrypted.
 
         :param command: inputted command name
         """
         cmd_def = self.commands_def
         domain_parameters = cmd_def.get(DOMAIN_PARAMETERS_KEY)
@@ -517,14 +521,20 @@
             _pretty_list = ', '.join(list(extra_parameters))
             parameters_errors.append(
                 f'The command {incoming_command_name} obtains unexpected '
                 f'params: {_pretty_list};')
 
         # check parameters using validation attr
         for p_name, p_def in params_def.items():
+            if isinstance(incoming_params.get(p_name), list):
+                if not p_def.get("multiple_values"):
+                    parameters_errors.append(
+                        f'Can specify option only once: {p_name};')
+                incoming_params[p_name] = ",".join(incoming_params.get(p_name))
+
             validation_rules = p_def.get(VALIDATION_KEY)
             if not validation_rules:
                 continue
             parameter_type = validation_rules.get('type')
             is_param_present = p_name in incoming_params
             if parameter_type == 'bool':
                 if incoming_params.get(p_name):
```

### Comparing `m3-cli-3.101.5/m3cli/services/environment_service.py` & `m3_cli-3.112.4/m3cli/services/environment_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/help_client.py` & `m3_cli-3.112.4/m3cli/services/help_client.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/interactive_options_service.py` & `m3_cli-3.112.4/m3cli/services/interactive_options_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import json
 import os
 from typing import List, Mapping
 
 import click
 
 from m3cli.models.interactive_parameter import InteractiveParameter
-from m3cli.services.interactivity import STRING_TYPE, \
-    RemoteValidationService, ParametersProvider, VarfileService, \
-    InteractiveInputService
-from m3cli.utils.interactivity_utils import unavailable_values_detector, \
-    get_interactivity_option
+from m3cli.services.interactivity import (
+    STRING_TYPE, RemoteValidationService, ParametersProvider, VarfileService,
+    InteractiveInputService,
+)
+from m3cli.utils.interactivity_utils import (
+    unavailable_values_detector, get_interactivity_option,
+)
 from m3cli.utils.logger import get_logger
+from m3cli.services.request_service import BaseRequest
 
 _LOG = get_logger('interactive_options_service')
 
 INTERACTIVE_OPTIONS_ATTRIBUTE = 'interactive_options'
 VARFILE_PARAMETER = 'variables-file'
 OPTION_NAME_ATTRIBUTE = 'option_name'
 GENERATE_VARFILE_ATTRIBUTE = 'generate_varfile'
@@ -45,22 +48,26 @@
             raise click.exceptions.Exit()
         else:
             filled_params = self._fill_parameter_values(
                 request=request,
                 interactive_parameters=interactive_params)
             return self.add_parameters_to_request(request, filled_params)
 
-    def add_parameters_to_request(self, request,
-                                  filled_params: List[InteractiveParameter]):
+    def add_parameters_to_request(
+            self,
+            request,
+            filled_params: List[InteractiveParameter]
+    ):
         request_parameters = request.parameters if request.parameters else {}
         variables_param_name = get_interactivity_option(
             interactive_options=self.interactive_options,
             option_name=OPTION_NAME_ATTRIBUTE)
-        raw_parameters = {param.name: param.to_raw_parameter()
-                          for param in filled_params}
+        raw_parameters = {
+            param.name: param.to_raw_parameter() for param in filled_params
+        }
         request_parameters.update({
             variables_param_name: raw_parameters
         })
         return request
 
     def _varfile_generation_requested(self):
         return bool(get_interactivity_option(
@@ -95,28 +102,38 @@
     def _fill_parameter_values(self, request, interactive_parameters):
         self._check_parameters_presence(interactive_parameters, request)
         filled_params = self._run_user_prompts(request, interactive_parameters)
         if not self.input_service.approve_parameters(filled_params):
             raise click.exceptions.Exit()
         return filled_params
 
-    def _run_user_prompts(self, request, interactive_parameters):
+    def _run_user_prompts(
+            self,
+            request: BaseRequest,
+            interactive_parameters: List[InteractiveParameter],
+    ):
         filled_params = []
         while interactive_parameters:
             collected_params = self.input_service.collect_user_input(
-                interactive_parameters=interactive_parameters,
-                request=request)
-            invalid_items = self.remote_validation_service \
-                .validate_parameters(collected_params)
+                interactive_parameters=interactive_parameters, request=request,
+            )
+            invalid_items = self.remote_validation_service.validate_parameters(
+                collected_params,
+                request.parameters.get("serviceName"),
+            )
             if invalid_items:
                 self._show_validation_errors(invalid_items)
-                if self.varfile_service.is_varfile_invalid(invalid_items):
+                if self.varfile_service.is_varfile_invalid(
+                        list(invalid_items.keys())
+                ):
                     raise click.exceptions.Exit()
-            filled_params.extend(param for param in interactive_parameters
-                                 if param not in invalid_items)
+            filled_params.extend(
+                param for param in interactive_parameters
+                if param not in invalid_items
+            )
             interactive_parameters = list(invalid_items.keys())
             for param in interactive_parameters:
                 param.force_prompt()
         return filled_params
 
     @staticmethod
     def _check_parameters_presence(interactive_params, request):
@@ -136,16 +153,18 @@
             else:
                 click.echo(
                     f'This service requires a variables file.{os.linesep}'
                     'Use the "generate-platform-service-varfile" command to '
                     'create a template of the variables file.')
             raise click.exceptions.Exit()
 
-    def _show_validation_errors(self,
-                                errors: Mapping[InteractiveParameter, str]):
+    def _show_validation_errors(
+            self,
+            errors: Mapping[InteractiveParameter, str],
+    ):
         click.echo('----------------------------')
         click.echo('Invalid parameters! Errors: ')
         for param, message in errors.items():
             click.echo(f'Parameter \'{param.name}\' '
                        f'of type {param.type}: '
                        f'{message}')
         if self.varfile_service.is_varfile_invalid(list(errors.keys())):
```

### Comparing `m3-cli-3.101.5/m3cli/services/interactivity/interactive_input_service.py` & `m3_cli-3.112.4/m3cli/services/interactivity/interactive_input_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/interactivity/parameters_provider.py` & `m3_cli-3.112.4/m3cli/services/interactivity/parameters_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 
 class ParametersProvider:
 
     def __init__(self, interactive_options):
         self.interactive_options = interactive_options
 
-    def fetch_interactive_parameters(self, request_parameters) \
-            -> List[InteractiveParameter]:
+    def fetch_interactive_parameters(
+            self, request_parameters
+    ) -> List[InteractiveParameter]:
         """
         This function gets parameters for command's request
         which will be asked from user in Interactive mode.
         :return: list of parameters
         """
         api_action = get_interactivity_option(
             interactive_options=self.interactive_options,
```

### Comparing `m3-cli-3.101.5/m3cli/services/interactivity/remote_validation_service.py` & `m3_cli-3.112.4/m3cli/services/interactivity/remote_validation_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 import json
-from typing import List
+from typing import List, Mapping
 
 from m3cli.models.interactive_parameter import (
-    InteractiveParameter, NAME_ATTR)
+    InteractiveParameter, NAME_ATTR
+)
 from m3cli.services.request_service import BaseRequest, POST, SdkClient
 from m3cli.utils.interactivity_utils import get_interactivity_option
 
 VALIDATION_HANDLER_ATTRIBUTE = 'validation_handler'
 ERROR_MESSAGE_ATTR = 'errorMessage'
 
 
 class RemoteValidationService:
 
     def __init__(self, interactive_options):
         self.interactive_options = interactive_options
 
-    def validate_parameters(self, parameters: List[InteractiveParameter]):
+    def validate_parameters(
+            self,
+            parameters: List[InteractiveParameter],
+            service_name: str,
+    ) -> Mapping[InteractiveParameter, str]:
         """
         Validates parameters entered by a user.
         :return: A list of invalid items.
         """
         api_action = get_interactivity_option(
             interactive_options=self.interactive_options,
-            option_name=VALIDATION_HANDLER_ATTRIBUTE)
-        payload = [param.to_raw_parameter()
-                   for param in parameters]
+            option_name=VALIDATION_HANDLER_ATTRIBUTE,
+        )
+        old_payload = [
+            param.to_raw_parameter() for param in parameters
+        ]
+        payload = {
+            'dtoList': old_payload,
+            'serviceName': service_name,
+        }
         validation_result = self._request_remote_validation(
-            api_action=api_action,
-            parameters=payload)
-        invalid_items = [validation_item
-                         for validation_item in validation_result
-                         if validation_item.get(ERROR_MESSAGE_ATTR)]
-
+            api_action=api_action, parameters=payload,
+        )
+        invalid_items = [
+            validation_item for validation_item in validation_result
+            if validation_item.get(ERROR_MESSAGE_ATTR)
+        ]
         invalid_parameters = {}
         for item in invalid_items:
-            parameter = next(param for param in parameters
-                             if param.name == item[NAME_ATTR])
+            parameter = next(
+                param for param in parameters if param.name == item[NAME_ATTR]
+            )
             invalid_parameters[parameter] = item[ERROR_MESSAGE_ATTR]
         return invalid_parameters
 
     @staticmethod
     def _request_remote_validation(api_action, parameters):
         validate_params_request = BaseRequest(
             command='validate_parameters',
             api_action=api_action,
-            parameters=list(parameters),
-            method=POST)
+            parameters=parameters,
+            method=POST,
+        )
         request_mapping, responses = SdkClient().execute(
             request=validate_params_request)
         response_item = responses[0]
         if not response_item.get('data'):
             raise AssertionError(
                 f'Failed to validate parameters while applying '
                 f'interactive mode. Reason: {response_item}. '
```

### Comparing `m3-cli-3.101.5/m3cli/services/interactivity/varfile/varfile_service.py` & `m3_cli-3.112.4/m3cli/services/interactivity/varfile/varfile_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/plugin_service.py` & `m3_cli-3.112.4/m3cli/services/plugin_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/rabbitmq_service.py` & `m3_cli-3.112.4/m3cli/services/rabbitmq_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/request_service.py` & `m3_cli-3.112.4/m3cli/services/request_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from m3cli.utils.utilities import open_creds_file, __load_creds_contents
 
 RESPONSE_ENDING_CHARS = b'}]}'
 
 _LOG = get_logger('request_service')
 
 USER_IDENTIFIER = 'SYSTEM'
+USER_UNKNOWN = 'UNKNOWN'
 CLIENT_IDENTIFIER = "api-server"
 
 POST = 'POST'
 
 HEADER_ENCRYPTED_ACCESS = 'maestro-accesskey'
 HEADER_DATE = 'maestro-date'
 HEADER_ENCRYPTED_DATE = 'maestro-authentication'
@@ -205,15 +206,15 @@
             signature_resolved += '1' + each
         new_request = {
             "headers": {
                 "Content-Type": "application/json",
                 "Accept": "application/json",
                 "maestro-authentication": signature_resolved,
                 "maestro-request-identifier": CLIENT_IDENTIFIER,
-                "maestro-user-identifier": USER_IDENTIFIER,
+                "maestro-user-identifier": USER_UNKNOWN,
                 "maestro-date": str(date),
                 "maestro-accesskey": access_key,
                 "maestro-sdk-version": get_sdk_version(),
                 "maestro-sdk-async": 'false',
                 "host": get_host()
             },
             'data': encrypted_raw_object,
```

### Comparing `m3-cli-3.101.5/m3cli/services/response_processor_service.py` & `m3_cli-3.112.4/m3cli/services/response_processor_service.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/response_utils.py` & `m3_cli-3.112.4/m3cli/services/response_utils.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/services/validation_service.py` & `m3_cli-3.112.4/m3cli/services/validation_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from m3cli.utils.logger import get_logger
 from m3cli.utils.utilities import inherit_dict
 
 _LOG = get_logger('validation_service')
 
 ROOT_DEFAULT = ''
 LIST_SEPARATOR = ','
+LIST_REGEX_PATTERN = r'''(?:"[^"]+"|[^,\s]+)\s*:\s*(?:"[^"]+"|[^,\s]+)|[^,]+'''
 
 VALIDATION_TYPE = 'type'
 VALIDATION_ALLOWED_VALUES = 'allowed_values'
 VALIDATION_REGEX = 'regex'
 VALIDATION_REGEX_ERROR = 'regex_error'
 VALIDATION_MAX_FILE_SIZE = 'max_size_bytes'
 VALIDATION_ALLOWED_FILE_EXTENSIONS = 'file_extensions'
@@ -400,18 +401,18 @@
     @staticmethod
     def adapt_list(actual_value):
         list_values = actual_value.split(LIST_SEPARATOR)
         return [value.strip() for value in list_values]
 
     @staticmethod
     def adapt_object(actual_value):
-        values = actual_value.split(LIST_SEPARATOR)
+        values = re.findall(LIST_REGEX_PATTERN, actual_value)
         object_dict = {}
         for v in values:
-            key, val = v.split(':')
+            key, val = v.replace('"', '').split(':')
             object_dict[key] = val
         return object_dict
 
     @staticmethod
     def adapt_date(actual_value):
         return datetime.strptime(actual_value, '%d.%m.%Y').replace(
             tzinfo=timezone.utc).timestamp() * 1000
```

### Comparing `m3-cli-3.101.5/m3cli/utils/__init__.py` & `m3_cli-3.112.4/m3cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/utils/cloud_utils.py` & `m3_cli-3.112.4/m3cli/utils/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/utils/decorators.py` & `m3_cli-3.112.4/m3cli/utils/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,29 +47,32 @@
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
 def __extract_parameters(parameters_list):
     parameters_dict = {}
-    params_values_count = len(parameters_list)
-    index = 0
-    while index < params_values_count:
-        key = parameters_list[index].replace('--', '')
-        # check key duplication
-        if key in parameters_dict.keys():
-            raise AssertionError(f'Can specify option {parameters_list[index]}'
-                                 f' only once')
-        if (index == params_values_count - 1 or
-                parameters_list[index + 1].startswith('-')):
-            parameters_dict[key] = None
-            index += 1
+    param_pfx = '-'
+    full_param_pfx = '--'
+
+    for index in range(len(parameters_list)):
+        if not parameters_list[index].startswith(param_pfx):
+            continue
+        key = parameters_list[index].replace(full_param_pfx, "")
+        if index < len(parameters_list)-1 and not parameters_list[index+1].startswith(param_pfx):
+            val = parameters_list[index+1]
+        else:
+            val = None
+        if key in parameters_dict:
+            if isinstance(parameters_dict[key], list):
+                parameters_dict[key].append(val)
+            else:
+                parameters_dict[key] = [parameters_dict[key], val]
         else:
-            parameters_dict[key] = parameters_list[index + 1]
-            index += 2
+            parameters_dict[key] = val
     return parameters_dict
 
 
 def __prettify_error(action, error):
     width, _ = get_terminal_size()
     action = action if action[-1:] == '.' else f'{action}!'
     divider = "=" * (width - 1)
@@ -129,20 +132,22 @@
             if ctx.params['help']:
                 click.echo(ACCESS_HELP)
                 return
             elif ('--access_key' or '--secret_key' or '--api_address' or
                   '--path') in ctx.args:
                 try:
                     access = get_non_interactive_access(
-                        *check_args_for_non_interactive_access(ctx))
+                        *check_args_for_non_interactive_access(ctx)
+                    )
                     click.echo(access)
                 except AssertionError as e:
                     action = f'The command \"{ctx.args[0]}\" failed'
-                    response = __prettify_error(action=action,
-                                                error=e)
+                    response = __prettify_error(
+                        action=action, error=e,
+                    )
                     click.echo(response, err=True)
                     raise e
             else:
                 access = get_user_access()
                 click.echo(access)
 
             # if the user has entered credits then switch check_health
@@ -185,16 +190,18 @@
             raise e
         command = ctx.args[0]
 
         if check_health:  # user entered new credentials
             command = 'health-check'
             parameters = {}
 
-        response = func(*args, command=command, parameters=parameters,
-                        view_type=view_type, detailed=detailed, raw_response=raw_response)
+        response = func(
+            *args, command=command, parameters=parameters, view_type=view_type,
+            detailed=detailed, raw_response=raw_response
+        )
         return response
 
     return wrapper
 
 
 def cli_response(stdout=click.echo, params_to_be_secured=None, no_output=None):
     """
```

### Comparing `m3-cli-3.101.5/m3cli/utils/interactivity_utils.py` & `m3_cli-3.112.4/m3cli/utils/interactivity_utils.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/utils/logger.py` & `m3_cli-3.112.4/m3cli/utils/logger.py`

 * *Files identical despite different names*

### Comparing `m3-cli-3.101.5/m3cli/utils/utilities.py` & `m3_cli-3.112.4/m3cli/utils/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,15 @@
 
 CONFIRMATION_MESSAGE = 'Maestro CLI credentials have been already set.\n' \
                        'Do you want to set a new credentials? [y/n]: '
 DEFAULT_API_ADDRESS = 'https://m3api.cloud.epam.com/maestro/api/v3'
 
 
 def inherit_dict(root_dict, child_dict):
-    if root_dict:
-        for root_key, root_value in root_dict.items():
-            if root_key not in child_dict:
-                child_dict[root_key] = root_value
+    child_dict.update({**root_dict, **child_dict})
     return child_dict
 
 
 def _set_credentials_interactively(credentials_path):
     m3sdk_access_key = input('M3 SDK Access key: ')
     if sys.platform.startswith(WINDOWS_SYSTEM):
         print('Use right-click anywhere in the body of the window to paste '
@@ -46,36 +43,44 @@
     os.environ[ACCESS_KEY] = m3sdk_access_key
     os.environ[SECRET_KEY] = m3sdk_secret_key
     os.environ[ADDRESS] = m3sdk_api_address
     __write_credentials_to_file(credentials_path, m3sdk_access_key,
                                 m3sdk_secret_key, m3sdk_api_address)
 
 
-def _set_credentials_by_params(credentials_path, access_key: str = None,
-                               secret_key: str = None,
-                               api_address: str = None):
+def _set_credentials_by_params(
+        credentials_path,
+        access_key: str = None,
+        secret_key: str = None,
+        api_address: str = None,
+):
     api_address = DEFAULT_API_ADDRESS if not api_address else api_address
     os.environ[ACCESS_KEY] = access_key
     os.environ[SECRET_KEY] = secret_key
     os.environ[ADDRESS] = api_address
-    __write_credentials_to_file(credentials_path, access_key, secret_key,
-                                api_address)
+    __write_credentials_to_file(
+        credentials_path, access_key, secret_key, api_address,
+    )
 
 
-def __write_credentials_to_file(credentials_path: str, access_key: str,
-                                secret_key: str, api_address: str):
+def __write_credentials_to_file(
+        credentials_path: str,
+        access_key: str,
+        secret_key: str,
+        api_address: str,
+):
     data = {}
     if os.path.exists(credentials_path):
         with open(credentials_path, 'r') as file:
             try:
                 data = json.load(file)
             except json.decoder.JSONDecodeError:
                 raise SyntaxError(
-                    f'{credentials_path} contains invalid JSON')
-
+                    f'{credentials_path} contains invalid JSON'
+                )
     with open(credentials_path, 'w') as file:
         data.update({ACCESS_KEY: access_key,
                      SECRET_KEY: secret_key,
                      ADDRESS: api_address})
         file.write(json.dumps(data))
 
 
@@ -85,24 +90,29 @@
     """
     creds_path = os.path.join(HOME_DIRECTORY, M3_CLI_RESOURCES_DIR)
     if not os.path.isdir(creds_path):
         os.makedirs(creds_path)
     return creds_path + FOLDERS_SEPARATOR + CREDENTIALS_FILE
 
 
-def get_non_interactive_access(access_key: str, secret_key: str,
-                               api_address=None, path=None):
+def get_non_interactive_access(
+        access_key: str,
+        secret_key: str,
+        api_address=None,
+        path=None,
+) -> str:
     if path:
         creds_filepath = Path(path)
         creds_filepath.mkdir(parents=True, exist_ok=True)
         creds_filepath = creds_filepath / CREDENTIALS_FILE
     else:
         creds_filepath = _get_credentials_file_path()
-    _set_credentials_by_params(creds_filepath, access_key, secret_key,
-                               api_address)
+    _set_credentials_by_params(
+        creds_filepath, access_key, secret_key, api_address,
+    )
     return f'Credentials have been successfully saved in: \n{creds_filepath}'
 
 
 def get_user_access():
     creds_filepath = _get_credentials_file_path()
     if (check_credentials_in_file(creds_filepath)
             and input(CONFIRMATION_MESSAGE).lower().strip() not
@@ -153,14 +163,15 @@
                                      creds_data=data)
 
 
 def get_current_cli_version():
     from importlib.metadata import version as lib_version
     return lib_version('m3-cli')
 
+
 def perform_version_check(invoked_command, is_help_invoked,
                           view_type, detailed):
     """
     Updates the latest version and distribution links of m3cli in the
     /.creds/default.cr file. If there is no such file, it will be created.
 
     The update is performed once a day or when the 'health-check' is invoked
```

### Comparing `m3-cli-3.101.5/setup.cfg` & `m3_cli-3.112.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = m3-cli
-version = 3.101.5
+version = 3.112.4
 author = maestrocloudcontrol
 author_email = support@maestrocontrol.cloud
 keywords = Maestro3, Command Line Interface, CLI, CLOUD
 description = The Maestro3 Command Line Interface (CLI) is a unified tool to manage your Maestro services and resources
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Maestro-Cloud-Control/m3-cli
```

