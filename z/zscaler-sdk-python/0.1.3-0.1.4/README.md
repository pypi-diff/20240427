# Comparing `tmp/zscaler_sdk_python-0.1.3.tar.gz` & `tmp/zscaler_sdk_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_sdk_python-0.1.3.tar", max compression
+gzip compressed data, was "zscaler_sdk_python-0.1.4.tar", max compression
```

## Comparing `zscaler_sdk_python-0.1.3.tar` & `zscaler_sdk_python-0.1.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1113 2024-04-25 03:50:00.568967 zscaler_sdk_python-0.1.3/LICENSE.md
--rw-r--r--   0        0        0    15600 2024-04-25 03:50:00.568967 zscaler_sdk_python-0.1.3/README.md
--rw-r--r--   0        0        0     2290 2024-04-25 03:50:53.977218 zscaler_sdk_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1278 2024-04-25 03:50:53.985218 zscaler_sdk_python-0.1.3/zscaler/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/__init__.py
--rw-r--r--   0        0        0     3195 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/cache.py
--rw-r--r--   0        0        0     1479 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/no_op_cache.py
--rw-r--r--   0        0        0     4967 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/cache/zscaler_cache.py
--rw-r--r--   0        0        0      738 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/constants.py
--rw-r--r--   0        0        0        0 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/__init__.py
--rw-r--r--   0        0        0      172 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/error.py
--rw-r--r--   0        0        0      638 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/http_error.py
--rw-r--r--   0        0        0      628 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/errors/zscaler_api_error.py
--rw-r--r--   0        0        0       63 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/exceptions/__init__.py
--rw-r--r--   0        0        0     2025 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/exceptions/exceptions.py
--rw-r--r--   0        0        0     2099 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/logger.py
--rw-r--r--   0        0        0        0 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0        0        0      639 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/user_agent.py
--rw-r--r--   0        0        0    19073 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/utils.py
--rw-r--r--   0        0        0    21568 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/__init__.py
--rw-r--r--   0        0        0     1534 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/activate.py
--rw-r--r--   0        0        0    14194 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0        0        0     2372 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/apptotal.py
--rw-r--r--   0        0        0     2992 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/audit_logs.py
--rw-r--r--   0        0        0     3140 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/authentication_settings.py
--rw-r--r--   0        0        0     2754 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/client.py
--rw-r--r--   0        0        0    18513 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/cloud_apps.py
--rw-r--r--   0        0        0     2872 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/device_management.py
--rw-r--r--   0        0        0    27473 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/dlp.py
--rw-r--r--   0        0        0      794 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/errors.py
--rw-r--r--   0        0        0    39908 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/firewall.py
--rw-r--r--   0        0        0    11686 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/forwarding_control.py
--rw-r--r--   0        0        0     2909 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/isolation_profile.py
--rw-r--r--   0        0        0     5835 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/labels.py
--rw-r--r--   0        0        0    30762 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/locations.py
--rw-r--r--   0        0        0     6724 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/sandbox.py
--rw-r--r--   0        0        0     6792 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/security.py
--rw-r--r--   0        0        0     5298 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/ssl_inspection.py
--rw-r--r--   0        0        0    30729 2024-04-25 03:50:00.588967 zscaler_sdk_python-0.1.3/zscaler/zia/traffic.py
--rw-r--r--   0        0        0    14484 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/url_categories.py
--rw-r--r--   0        0        0    14319 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/url_filtering.py
--rw-r--r--   0        0        0    13735 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/users.py
--rw-r--r--   0        0        0    12376 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/web_dlp.py
--rw-r--r--   0        0        0     1897 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/workload_groups.py
--rw-r--r--   0        0        0     6842 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zia/zpa_gateway.py
--rw-r--r--   0        0        0     2709 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/README.md
--rw-r--r--   0        0        0    24300 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/__init__.py
--rw-r--r--   0        0        0    13187 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments.py
--rw-r--r--   0        0        0    12445 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0        0        0    12019 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0        0        0     7942 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/certificates.py
--rw-r--r--   0        0        0     3804 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/client.py
--rw-r--r--   0        0        0     2667 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0        0        0    20370 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/connectors.py
--rw-r--r--   0        0        0     6189 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/emergency_access.py
--rw-r--r--   0        0        0      844 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/errors.py
--rw-r--r--   0        0        0     2764 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/idp.py
--rw-r--r--   0        0        0    34309 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/inspection.py
--rw-r--r--   0        0        0     3176 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/isolation_profile.py
--rw-r--r--   0        0        0    21113 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/lss.py
--rw-r--r--   0        0        0     2734 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/machine_groups.py
--rw-r--r--   0        0        0    30350 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/policies.py
--rw-r--r--   0        0        0     4317 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/posture_profiles.py
--rw-r--r--   0        0        0    32017 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0        0        0     9887 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/provisioning.py
--rw-r--r--   0        0        0     3632 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/saml_attributes.py
--rw-r--r--   0        0        0     4172 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/scim_attributes.py
--rw-r--r--   0        0        0     5041 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/scim_groups.py
--rw-r--r--   0        0        0     6103 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/segment_groups.py
--rw-r--r--   0        0        0     7776 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/server_groups.py
--rw-r--r--   0        0        0     6477 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/servers.py
--rw-r--r--   0        0        0    15428 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/service_edges.py
--rw-r--r--   0        0        0     4377 2024-04-25 03:50:00.592968 zscaler_sdk_python-0.1.3/zscaler/zpa/trusted_networks.py
--rw-r--r--   0        0        0    17368 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-04-26 16:08:53.596135 zscaler_sdk_python-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0    15600 2024-04-26 16:08:53.596135 zscaler_sdk_python-0.1.4/README.md
+-rw-r--r--   0        0        0     2290 2024-04-26 16:09:36.320207 zscaler_sdk_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1278 2024-04-26 16:09:36.324207 zscaler_sdk_python-0.1.4/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4967 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      738 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-04-26 16:08:53.616135 zscaler_sdk_python-0.1.4/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    24300 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    13187 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     7942 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3804 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20849 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    34309 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0     3176 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0        0        0    21113 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0    30350 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0     4317 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    32017 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     5041 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7776 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     4377 2024-04-26 16:08:53.620135 zscaler_sdk_python-0.1.4/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17368 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.4/PKG-INFO
```

### Comparing `zscaler_sdk_python-0.1.3/LICENSE.md` & `zscaler_sdk_python-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/README.md` & `zscaler_sdk_python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/pyproject.toml` & `zscaler_sdk_python-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zscaler-sdk-python"
-version = "0.1.3"
+version = "0.1.4"
 description = "Official Python SDK for the Zscaler Products (Beta)"
 authors = ["Zscaler, Inc. <devrel@zscaler.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zscaler/zscaler-sdk-python"
 repository = "https://github.com/zscaler/zscaler-sdk-python"
 documentation = "https://zscaler-sdk-python.readthedocs.io"
```

### Comparing `zscaler_sdk_python-0.1.3/zscaler/__init__.py` & `zscaler_sdk_python-0.1.4/zscaler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler_sdk_python-0.1.3/zscaler/cache/cache.py` & `zscaler_sdk_python-0.1.4/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.1.4/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.1.4/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/constants.py` & `zscaler_sdk_python-0.1.4/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.1.4/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.1.4/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.1.4/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/logger.py` & `zscaler_sdk_python-0.1.4/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.1.4/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/user_agent.py` & `zscaler_sdk_python-0.1.4/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/utils.py` & `zscaler_sdk_python-0.1.4/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/activate.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/client.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/errors.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/labels.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/locations.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/security.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/users.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.1.4/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/README.md` & `zscaler_sdk_python-0.1.4/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/app_segments.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/client.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/connectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
 from box import Box, BoxList
 from requests import Response
-
+import os
 from zscaler.utils import add_id_groups, pick_version_profile, snake_to_camel
 from zscaler.zpa.client import ZPAClient
 
 
 class AppConnectorControllerAPI:
     reformat_params = [
         ("connector_ids", "connectors"),
@@ -377,15 +377,15 @@
 
         Examples:
             >>> zpa.connectors.delete_connector_group('1876541121')
 
         """
         return self.rest.delete(f"appConnectorGroup/{group_id}").status_code
 
-    def get_connector_schedule(self) -> Box:
+    def get_connector_schedule(self, customer_id=None) -> Box:
         """
         Returns the configured App Connector Schedule frequency.
 
         Args:
             id (str): Unique identifier for the App Connector auto deletion config.
                 Required for the PUT request to update the App Connector Settings frequency.
             customer_id (str): Unique identifier of the ZPA tenant.
@@ -398,15 +398,24 @@
         Returns:
             :obj:`Box`: The Auto Delete frequency of the App Connector for the specified customer.
 
         Examples:
             >>> pprint(zpa.connectors.get_connector_schedule)
         """
 
-        response = self.rest.get("/assistantSchedule")
+        # Fetch customer_id from environment if not provided
+        if customer_id is None:
+            customer_id = os.getenv("ZPA_CUSTOMER_ID")
+
+        if not customer_id:
+            raise ValueError(
+                "customer_id is required either as a function argument or as an environment variable ZPA_CUSTOMER_ID"
+            )
+
+        response = self.rest.get("/connectorSchedule")
         if isinstance(response, Response):
             return None
         return response
 
     def add_connector_schedule(self, frequency, interval, disabled, **kwargs) -> Box:
         """
         Configure an App Connector schedule frequency to delete inactive connectors based on
@@ -444,22 +453,22 @@
             "deleteDisabled": disabled,
         }
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        response = self.rest.post("assistantSchedule", json=payload)
+        response = self.rest.post("connectorSchedule", json=payload)
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code >= 400:  # Check if status code indicates an error
                 raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-    def update_schedule(self, scheduler_id: str, **kwargs) -> bool:
+    def update_connector_schedule(self, scheduler_id: str, **kwargs) -> bool:
         """
         Updates App Connector schedule frequency to delete the inactive connectors based on
         the configured frequency.
 
         Args:
             scheduler_id (str): Unique identifier for the scheduler.
             customer_id (str): Unique identifier of the ZPA tenant.
@@ -478,23 +487,26 @@
 
         Examples:
             Updating connector schedule:
 
             >>> result = zpa.connectors.update_schedule('10', frequency_interval='10')
             >>> print(result)  # True if successful, False otherwise
         """
-        # Get the current schedule
-        current_schedule = self.get_connector_schedule(scheduler_id=scheduler_id)
+        # Get the current schedule by customer ID
+        customer_id = kwargs.get("customer_id")
+        if not customer_id:
+            raise ValueError("customer_id must be provided as a keyword argument.")
+
+        current_schedule = self.get_connector_schedule(customer_id=customer_id)
+
+        if not current_schedule:
+            raise ValueError("No existing schedule found for the provided customer ID.")
 
         # Update the schedule with provided arguments
         for key, value in kwargs.items():
-            # Check for customer_id and convert it to int if it's a string
-            if key == "customer_id":
-                value = int(value) if isinstance(value, str) and value.isdigit() else value
-
             current_schedule[snake_to_camel(key)] = value
 
         # Send the updated schedule to the server
-        response = self.rest.put(f"assistantSchedule/{scheduler_id}", json=current_schedule)
+        response = self.rest.put(f"connectorSchedule/{scheduler_id}", json=current_schedule.to_dict())
 
         # Return True if the update was successful (204 No Content), False otherwise
         return response.status_code == 204
```

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/isolation_profile.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/machine_groups.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/policies.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/zscaler/zpa/trusted_networks.py` & `zscaler_sdk_python-0.1.4/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.3/PKG-INFO` & `zscaler_sdk_python-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://github.com/zscaler/zscaler-sdk-python
 License: MIT
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Requires-Python: >=3.8,<4.0
```

