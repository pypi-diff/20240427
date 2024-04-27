# Comparing `tmp/iam_actions-1.2.20240426.tar.gz` & `tmp/iam_actions-1.2.20240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240426.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240427.tar", max compression
```

## Comparing `iam_actions-1.2.20240426.tar` & `iam_actions-1.2.20240427.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/README.md
--rw-r--r--   0        0        0      228 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/__init__.py
--rw-r--r--   0        0        0  4814922 2024-04-26 02:20:42.339376 iam_actions-1.2.20240426/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-26 02:18:23.854990 iam_actions-1.2.20240426/iam_actions/generate/services.py
--rw-r--r--   0        0        0   626155 2024-04-26 02:20:42.339376 iam_actions-1.2.20240426/iam_actions/policies.json
--rw-r--r--   0        0        0   209050 2024-04-26 02:20:42.339376 iam_actions-1.2.20240426/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   607542 2024-04-26 02:20:42.339376 iam_actions-1.2.20240426/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-26 02:20:42.995378 iam_actions-1.2.20240426/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240426/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240426/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-27 02:17:51.595873 iam_actions-1.2.20240427/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/README.md
+-rw-r--r--   0        0        0      228 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4812377 2024-04-27 02:18:54.395571 iam_actions-1.2.20240427/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-27 02:17:51.599873 iam_actions-1.2.20240427/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   625917 2024-04-27 02:18:54.395571 iam_actions-1.2.20240427/iam_actions/policies.json
+-rw-r--r--   0        0        0   209050 2024-04-27 02:18:54.395571 iam_actions-1.2.20240427/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   607313 2024-04-27 02:18:54.395571 iam_actions-1.2.20240427/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-27 02:18:55.075568 iam_actions-1.2.20240427/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240427/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240427/PKG-INFO
```

### Comparing `iam_actions-1.2.20240426/LICENSE` & `iam_actions-1.2.20240427/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/README.md` & `iam_actions-1.2.20240427/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/actions.json` & `iam_actions-1.2.20240427/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999797759505588%*

 * *Differences: {"'codepipeline'": "{'RollbackStage': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                   "'RollbackStage'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *                   "AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'healthlake'": "{'SearchEverything': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                 "'SearchEverything'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *                 "AWS'), ('orphan', False), ('r […]*

```diff
@@ -29452,14 +29452,22 @@
             "condition_keys": [],
             "description": "Grants permission to resume the pipeline execution by retrying the last failed actions in a stage",
             "orphan": false,
             "resources": [
                 "stage"
             ]
         },
+        "RollbackStage": {
+            "access_level": "Undocumented",
+            "action": "RollbackStage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartPipelineExecution": {
             "access_level": "Write",
             "action": "StartPipelineExecution",
             "condition_keys": [],
             "description": "Grants permission to run the most recent revision through the pipeline",
             "orphan": false,
             "resources": [
@@ -80702,14 +80710,22 @@
             "access_level": "Undocumented",
             "action": "ReadResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "SearchEverything": {
+            "access_level": "Undocumented",
+            "action": "SearchEverything",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SearchWithGet": {
             "access_level": "Undocumented",
             "action": "SearchWithGet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -169688,24 +169704,14 @@
             "orphan": false,
             "resources": [
                 "fleet"
             ]
         }
     },
     "workmail": {
-        "AddMembersToGroup": {
-            "access_level": "Write",
-            "action": "AddMembersToGroup",
-            "condition_keys": [],
-            "description": "Grants permission to add a list of members (users or groups) to a group",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "AllowVendedLogDeliveryForResource": {
             "access_level": "Write",
             "action": "AllowVendedLogDeliveryForResource",
             "condition_keys": [],
             "description": "Grants permission to configure vended log delivery for WorkMail audit logs",
             "orphan": false,
             "resources": [
@@ -170066,22 +170072,14 @@
             "condition_keys": [],
             "description": "Grants permission to deregister a mail domain from an organization",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "DescribeDirectories": {
-            "access_level": "List",
-            "action": "DescribeDirectories",
-            "condition_keys": [],
-            "description": "Grants permission to show a list of directories available for use in creating an organization",
-            "orphan": false,
-            "resources": []
-        },
         "DescribeEmailMonitoringConfiguration": {
             "access_level": "Read",
             "action": "DescribeEmailMonitoringConfiguration",
             "condition_keys": [],
             "description": "Grants permission to retrieve the email monitoring configuration for an organization",
             "orphan": false,
             "resources": [
@@ -170124,52 +170122,24 @@
             "condition_keys": [],
             "description": "Grants permission to read the details of an inbound mail flow rule configured for an organization",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "DescribeKmsKeys": {
-            "access_level": "List",
-            "action": "DescribeKmsKeys",
-            "condition_keys": [],
-            "description": "Grants permission to show a list of KMS Keys available for use in creating an organization",
-            "orphan": false,
-            "resources": []
-        },
         "DescribeMailDomains": {
             "access_level": "List",
             "action": "DescribeMailDomains",
             "condition_keys": [],
             "description": "Grants permission to show the details of all mail domains associated with the organization",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "DescribeMailGroups": {
-            "access_level": "List",
-            "action": "DescribeMailGroups",
-            "condition_keys": [],
-            "description": "Grants permission to show the details of all groups associated with the organization",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
-        "DescribeMailUsers": {
-            "access_level": "List",
-            "action": "DescribeMailUsers",
-            "condition_keys": [],
-            "description": "Grants permission to show the details of all users associated with the organization",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "DescribeMailboxExportJob": {
             "access_level": "Read",
             "action": "DescribeMailboxExportJob",
             "condition_keys": [],
             "description": "Grants permission to retrieve details of a mailbox export job",
             "orphan": false,
             "resources": [
@@ -170182,22 +170152,14 @@
             "condition_keys": [],
             "description": "Grants permission to read details of an organization",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "DescribeOrganizations": {
-            "access_level": "List",
-            "action": "DescribeOrganizations",
-            "condition_keys": [],
-            "description": "Grants permission to show a summary of all organizations associated with the account",
-            "orphan": false,
-            "resources": []
-        },
         "DescribeOutboundMailFlowRule": {
             "access_level": "Read",
             "action": "DescribeOutboundMailFlowRule",
             "condition_keys": [],
             "description": "Grants permission to read the details of an outbound mail flow rule configured for an organization",
             "orphan": false,
             "resources": [
@@ -170330,24 +170292,14 @@
             "condition_keys": [],
             "description": "Grants permission to get the details of the mail domain",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "GetMailGroupDetails": {
-            "access_level": "Read",
-            "action": "GetMailGroupDetails",
-            "condition_keys": [],
-            "description": "Grants permission to get the details of the mail group",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "GetMailboxDetails": {
             "access_level": "Read",
             "action": "GetMailboxDetails",
             "condition_keys": [],
             "description": "Grants permission to read the details of the user's mailbox",
             "orphan": false,
             "resources": [
@@ -170510,24 +170462,14 @@
             "condition_keys": [],
             "description": "Grants permission to list the mailbox permissions associated with a user, group, or resource mailbox",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "ListMembersInMailGroup": {
-            "access_level": "Read",
-            "action": "ListMembersInMailGroup",
-            "condition_keys": [],
-            "description": "Grants permission to get a list of all the members in a mail group",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "ListMobileDeviceAccessOverrides": {
             "access_level": "Read",
             "action": "ListMobileDeviceAccessOverrides",
             "condition_keys": [],
             "description": "Grants permission to list the mobile device access overrides",
             "orphan": false,
             "resources": [
@@ -170691,64 +170633,34 @@
             "condition_keys": [],
             "description": "Grants permission to register an existing and disabled user, group, or resource for use by associating a mailbox and calendaring capabilities",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "RemoveMembersFromGroup": {
-            "access_level": "Write",
-            "action": "RemoveMembersFromGroup",
-            "condition_keys": [],
-            "description": "Grants permission to remove members from a mail group",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "ResetPassword": {
             "access_level": "Write",
             "action": "ResetPassword",
             "condition_keys": [],
             "description": "Grants permission to allow the administrator to reset the password for a user",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "ResetUserPassword": {
-            "access_level": "Write",
-            "action": "ResetUserPassword",
-            "condition_keys": [],
-            "description": "Grants permission to reset the password for a user's account",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "SearchMembers": {
             "access_level": "Read",
             "action": "SearchMembers",
             "condition_keys": [],
             "description": "Grants permission to perform a prefix search to find a specific user in a mail group",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "SetAdmin": {
-            "access_level": "Write",
-            "action": "SetAdmin",
-            "condition_keys": [],
-            "description": "Grants permission to mark a user as being an administrator",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "SetDefaultMailDomain": {
             "access_level": "Write",
             "action": "SetDefaultMailDomain",
             "condition_keys": [],
             "description": "Grants permission to set the default mail domain for the organization",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20240426/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240427/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240427/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/generate/generate.py` & `iam_actions-1.2.20240427/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240427/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240427/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/generate/services.py` & `iam_actions-1.2.20240427/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/policies.json` & `iam_actions-1.2.20240427/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999983886529714%*

 * *Differences: {"'serviceMap'": "{'AWS CodePipeline': {'Actions': {insert: [(33, 'RollbackStage')]}}, 'Amazon "*

 * *                 "WorkMail': {'Actions': {delete: [105, 103, 101, 83, 65, 50, 47, 46, 44, 38, "*

 * *                 "0]}}, 'AWS HealthLake': {'Actions': {insert: [(13, 'SearchEverything')]}}}"}*

```diff
@@ -2410,14 +2410,15 @@
                 "PutJobFailureResult",
                 "PutJobSuccessResult",
                 "PutThirdPartyJobFailureResult",
                 "PutThirdPartyJobSuccessResult",
                 "PutWebhook",
                 "RegisterWebhookWithThirdParty",
                 "RetryStageExecution",
+                "RollbackStage",
                 "StartPipelineExecution",
                 "StopPipelineExecution",
                 "TagResource",
                 "UntagResource",
                 "UpdateActionType",
                 "UpdatePipeline"
             ],
@@ -5210,14 +5211,15 @@
                 "DescribeFHIRImportJob",
                 "GetCapabilities",
                 "ListFHIRDatastores",
                 "ListFHIRExportJobs",
                 "ListFHIRImportJobs",
                 "ListTagsForResource",
                 "ReadResource",
+                "SearchEverything",
                 "SearchWithGet",
                 "SearchWithPost",
                 "StartFHIRExportJob",
                 "StartFHIRImportJob",
                 "TagResource",
                 "UntagResource",
                 "UpdateResource"
@@ -21931,15 +21933,14 @@
                 "aws:TagKeys"
             ]
         },
         "Amazon WorkMail": {
             "ARNFormat": "arn:aws:workmail:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:workmail:.+:.+:.+",
             "Actions": [
-                "AddMembersToGroup",
                 "AllowVendedLogDeliveryForResource",
                 "AssociateDelegateToResource",
                 "AssociateMemberToGroup",
                 "AssumeImpersonationRole",
                 "CancelMailboxExportJob",
                 "CreateAlias",
                 "CreateAvailabilityConfiguration",
@@ -21969,42 +21970,36 @@
                 "DeleteOutboundMailFlowRule",
                 "DeleteResource",
                 "DeleteRetentionPolicy",
                 "DeleteSmtpGateway",
                 "DeleteUser",
                 "DeregisterFromWorkMail",
                 "DeregisterMailDomain",
-                "DescribeDirectories",
                 "DescribeEmailMonitoringConfiguration",
                 "DescribeEntity",
                 "DescribeGroup",
                 "DescribeInboundDmarcSettings",
                 "DescribeInboundMailFlowRule",
-                "DescribeKmsKeys",
                 "DescribeMailDomains",
-                "DescribeMailGroups",
-                "DescribeMailUsers",
                 "DescribeMailboxExportJob",
                 "DescribeOrganization",
-                "DescribeOrganizations",
                 "DescribeOutboundMailFlowRule",
                 "DescribeResource",
                 "DescribeSmtpGateway",
                 "DescribeUser",
                 "DisassociateDelegateFromResource",
                 "DisassociateMemberFromGroup",
                 "EnableMailDomain",
                 "GetAccessControlEffect",
                 "GetDefaultRetentionPolicy",
                 "GetImpersonationRole",
                 "GetImpersonationRoleEffect",
                 "GetJournalingRules",
                 "GetMailDomain",
                 "GetMailDomainDetails",
-                "GetMailGroupDetails",
                 "GetMailboxDetails",
                 "GetMobileDeviceAccessEffect",
                 "GetMobileDeviceAccessOverride",
                 "GetMobileDeviceDetails",
                 "GetMobileDevicesForUser",
                 "GetMobilePolicyDetails",
                 "ListAccessControlRules",
@@ -22014,15 +22009,14 @@
                 "ListGroups",
                 "ListGroupsForEntity",
                 "ListImpersonationRoles",
                 "ListInboundMailFlowRules",
                 "ListMailDomains",
                 "ListMailboxExportJobs",
                 "ListMailboxPermissions",
-                "ListMembersInMailGroup",
                 "ListMobileDeviceAccessOverrides",
                 "ListMobileDeviceAccessRules",
                 "ListOrganizations",
                 "ListOutboundMailFlowRules",
                 "ListResourceDelegates",
                 "ListResources",
                 "ListSmtpGateways",
@@ -22032,19 +22026,16 @@
                 "PutEmailMonitoringConfiguration",
                 "PutInboundDmarcSettings",
                 "PutMailboxPermissions",
                 "PutMobileDeviceAccessOverride",
                 "PutRetentionPolicy",
                 "RegisterMailDomain",
                 "RegisterToWorkMail",
-                "RemoveMembersFromGroup",
                 "ResetPassword",
-                "ResetUserPassword",
                 "SearchMembers",
-                "SetAdmin",
                 "SetDefaultMailDomain",
                 "SetJournalingRules",
                 "SetMobilePolicyDetails",
                 "StartMailboxExportJob",
                 "TagResource",
                 "TestAvailabilityConfiguration",
                 "TestInboundMailFlowRules",
```

### Comparing `iam_actions-1.2.20240426/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240427/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240426/iam_actions/services.json` & `iam_actions-1.2.20240427/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999831466254656%*

 * *Differences: {"'codepipeline'": "{'Actions': {insert: [(33, 'RollbackStage')]}}",*

 * * "'healthlake'": "{'Actions': {insert: [(13, 'SearchEverything')]}}",*

 * * "'workmail'": "{'Actions': {delete: [105, 103, 101, 83, 65, 50, 47, 46, 44, 38, 0]}}"}*

```diff
@@ -4510,14 +4510,15 @@
             "PutJobFailureResult",
             "PutJobSuccessResult",
             "PutThirdPartyJobFailureResult",
             "PutThirdPartyJobSuccessResult",
             "PutWebhook",
             "RegisterWebhookWithThirdParty",
             "RetryStageExecution",
+            "RollbackStage",
             "StartPipelineExecution",
             "StopPipelineExecution",
             "TagResource",
             "UntagResource",
             "UpdateActionType",
             "UpdatePipeline"
         ],
@@ -11023,14 +11024,15 @@
             "DescribeFHIRImportJob",
             "GetCapabilities",
             "ListFHIRDatastores",
             "ListFHIRExportJobs",
             "ListFHIRImportJobs",
             "ListTagsForResource",
             "ReadResource",
+            "SearchEverything",
             "SearchWithGet",
             "SearchWithPost",
             "StartFHIRExportJob",
             "StartFHIRImportJob",
             "TagResource",
             "UntagResource",
             "UpdateResource"
@@ -23968,15 +23970,14 @@
         "ARNFormats": [
             "arn:aws:workmail:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:workmail:.+:.+:.+"
         ],
         "Actions": [
-            "AddMembersToGroup",
             "AllowVendedLogDeliveryForResource",
             "AssociateDelegateToResource",
             "AssociateMemberToGroup",
             "AssumeImpersonationRole",
             "CancelMailboxExportJob",
             "CreateAlias",
             "CreateAvailabilityConfiguration",
@@ -24006,42 +24007,36 @@
             "DeleteOutboundMailFlowRule",
             "DeleteResource",
             "DeleteRetentionPolicy",
             "DeleteSmtpGateway",
             "DeleteUser",
             "DeregisterFromWorkMail",
             "DeregisterMailDomain",
-            "DescribeDirectories",
             "DescribeEmailMonitoringConfiguration",
             "DescribeEntity",
             "DescribeGroup",
             "DescribeInboundDmarcSettings",
             "DescribeInboundMailFlowRule",
-            "DescribeKmsKeys",
             "DescribeMailDomains",
-            "DescribeMailGroups",
-            "DescribeMailUsers",
             "DescribeMailboxExportJob",
             "DescribeOrganization",
-            "DescribeOrganizations",
             "DescribeOutboundMailFlowRule",
             "DescribeResource",
             "DescribeSmtpGateway",
             "DescribeUser",
             "DisassociateDelegateFromResource",
             "DisassociateMemberFromGroup",
             "EnableMailDomain",
             "GetAccessControlEffect",
             "GetDefaultRetentionPolicy",
             "GetImpersonationRole",
             "GetImpersonationRoleEffect",
             "GetJournalingRules",
             "GetMailDomain",
             "GetMailDomainDetails",
-            "GetMailGroupDetails",
             "GetMailboxDetails",
             "GetMobileDeviceAccessEffect",
             "GetMobileDeviceAccessOverride",
             "GetMobileDeviceDetails",
             "GetMobileDevicesForUser",
             "GetMobilePolicyDetails",
             "ListAccessControlRules",
@@ -24051,15 +24046,14 @@
             "ListGroups",
             "ListGroupsForEntity",
             "ListImpersonationRoles",
             "ListInboundMailFlowRules",
             "ListMailDomains",
             "ListMailboxExportJobs",
             "ListMailboxPermissions",
-            "ListMembersInMailGroup",
             "ListMobileDeviceAccessOverrides",
             "ListMobileDeviceAccessRules",
             "ListOrganizations",
             "ListOutboundMailFlowRules",
             "ListResourceDelegates",
             "ListResources",
             "ListSmtpGateways",
@@ -24069,19 +24063,16 @@
             "PutEmailMonitoringConfiguration",
             "PutInboundDmarcSettings",
             "PutMailboxPermissions",
             "PutMobileDeviceAccessOverride",
             "PutRetentionPolicy",
             "RegisterMailDomain",
             "RegisterToWorkMail",
-            "RemoveMembersFromGroup",
             "ResetPassword",
-            "ResetUserPassword",
             "SearchMembers",
-            "SetAdmin",
             "SetDefaultMailDomain",
             "SetJournalingRules",
             "SetMobilePolicyDetails",
             "StartMailboxExportJob",
             "TagResource",
             "TestAvailabilityConfiguration",
             "TestInboundMailFlowRules",
```

### Comparing `iam_actions-1.2.20240426/pyproject.toml` & `iam_actions-1.2.20240427/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240426"
+version = "1.2.20240427"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240426/setup.py` & `iam_actions-1.2.20240427/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240426',
+    'version': '1.2.20240427',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240426/PKG-INFO` & `iam_actions-1.2.20240427/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240426
+Version: 1.2.20240427
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

