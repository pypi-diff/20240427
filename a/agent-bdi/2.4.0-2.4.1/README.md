# Comparing `tmp/agent-bdi-2.4.0.tar.gz` & `tmp/agent-bdi-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-2.4.0.tar", last modified: Tue Apr  9 08:36:20 2024, max compression
+gzip compressed data, was "agent-bdi-2.4.1.tar", last modified: Sat Apr 27 18:04:20 2024, max compression
```

## Comparing `agent-bdi-2.4.0.tar` & `agent-bdi-2.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.339026 agent-bdi-2.4.0/
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/LICENSE.md
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3202 2024-04-09 08:36:20.338026 agent-bdi-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 08:36:20.339026 agent-bdi-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-04-09 08:36:11.000000 agent-bdi-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.287969 agent-bdi-2.4.0/src/
--rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/__init__.py
--rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/abdi_config.py
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.304458 agent-bdi-2.4.0/src/agent_bdi.egg-info/
--rw-rw-rw-   0        0        0     3202 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.313458 agent-bdi-2.4.0/src/broker/
--rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/__init__.py
--rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/broker_maker.py
--rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/empty_broker.py
--rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/message_broker.py
--rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.0/src/broker/mqtt_broker.py
--rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/notifier.py
--rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/redis_broker.py
--rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/ros_broker.py
--rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/ros_noetic_broker.py
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.318800 agent-bdi-2.4.0/src/core/
--rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.0/src/core/Agent.py
--rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/Belief.py
--rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/Desire.py
--rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/Intention.py
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.326216 agent-bdi-2.4.0/src/holon/
--rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/holon/Blackboard.py
--rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.0/src/holon/Heart.py
--rw-rw-rw-   0        0        0    11104 2024-04-04 18:17:14.000000 agent-bdi-2.4.0/src/holon/HolonicAgent.py
--rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/holon/HolonicDesire.py
--rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/holon/HolonicIntention.py
--rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/holon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.331951 agent-bdi-2.4.0/src/holon/logistics/
--rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.0/src/holon/logistics/__init__.py
--rw-rw-rw-   0        0        0      710 2024-02-24 14:56:32.000000 agent-bdi-2.4.0/src/holon/logistics/base_logistic.py
--rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.0/src/holon/logistics/broker_logistic.py
--rw-rw-rw-   0        0        0     5299 2024-02-26 10:20:43.000000 agent-bdi-2.4.0/src/holon/logistics/loading_coordinator.py
--rw-rw-rw-   0        0        0     6333 2024-04-04 18:40:47.000000 agent-bdi-2.4.0/src/holon/logistics/payload_wrapper.py
--rw-rw-rw-   0        0        0     3570 2024-04-04 18:43:34.000000 agent-bdi-2.4.0/src/holon/logistics/request_logistic.py
--rw-rw-rw-   0        0        0     2367 2024-02-24 20:21:15.000000 agent-bdi-2.4.0/src/holon/logistics/response_logistic.py
--rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.0/src/holon/payload.py
-drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.337018 agent-bdi-2.4.0/tests/
--rw-rw-rw-   0        0        0      762 2024-01-07 09:18:18.000000 agent-bdi-2.4.0/tests/test01.py
--rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.0/tests/test_loadingbal.py
--rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.0/tests/test_request.py
--rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.0/tests/test_send.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.592495 agent-bdi-2.4.1/
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/LICENSE.md
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3202 2024-04-27 18:04:20.591492 agent-bdi-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 18:04:20.592495 agent-bdi-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-04-27 18:03:56.000000 agent-bdi-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.540646 agent-bdi-2.4.1/src/
+-rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/abdi_config.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.555645 agent-bdi-2.4.1/src/agent_bdi.egg-info/
+-rw-rw-rw-   0        0        0     3202 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.568148 agent-bdi-2.4.1/src/broker/
+-rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/broker_maker.py
+-rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/empty_broker.py
+-rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/message_broker.py
+-rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.1/src/broker/mqtt_broker.py
+-rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/notifier.py
+-rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/redis_broker.py
+-rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/ros_broker.py
+-rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/ros_noetic_broker.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.572152 agent-bdi-2.4.1/src/core/
+-rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.1/src/core/Agent.py
+-rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/Belief.py
+-rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/Desire.py
+-rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/Intention.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.579152 agent-bdi-2.4.1/src/holon/
+-rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/holon/Blackboard.py
+-rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.1/src/holon/Heart.py
+-rw-rw-rw-   0        0        0     9850 2024-04-27 15:00:13.000000 agent-bdi-2.4.1/src/holon/HolonicAgent.py
+-rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/holon/HolonicDesire.py
+-rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/holon/HolonicIntention.py
+-rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/holon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.585478 agent-bdi-2.4.1/src/holon/logistics/
+-rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.1/src/holon/logistics/__init__.py
+-rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.1/src/holon/logistics/base_logistic.py
+-rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.1/src/holon/logistics/broker_logistic.py
+-rw-rw-rw-   0        0        0     5299 2024-02-26 10:20:43.000000 agent-bdi-2.4.1/src/holon/logistics/loading_coordinator.py
+-rw-rw-rw-   0        0        0     6333 2024-04-04 18:40:47.000000 agent-bdi-2.4.1/src/holon/logistics/payload_wrapper.py
+-rw-rw-rw-   0        0        0     3709 2024-04-17 17:18:06.000000 agent-bdi-2.4.1/src/holon/logistics/request_logistic.py
+-rw-rw-rw-   0        0        0     3312 2024-04-27 17:02:22.000000 agent-bdi-2.4.1/src/holon/logistics/response_logistic.py
+-rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.1/src/holon/payload.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.590493 agent-bdi-2.4.1/tests/
+-rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.1/tests/test01.py
+-rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.1/tests/test_loadingbal.py
+-rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.1/tests/test_request.py
+-rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.1/tests/test_send.py
```

### Comparing `agent-bdi-2.4.0/PKG-INFO` & `agent-bdi-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.0
+Version: 2.4.1
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.0/README.md` & `agent-bdi-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/setup.py` & `agent-bdi-2.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "2.4.0",
+    version = "2.4.1",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-2.4.0/src/abdi_config.py` & `agent-bdi-2.4.1/src/abdi_config.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-2.4.1/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.0
+Version: 2.4.1
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.0/src/agent_bdi.egg-info/SOURCES.txt` & `agent-bdi-2.4.1/src/agent_bdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/broker_maker.py` & `agent-bdi-2.4.1/src/broker/broker_maker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/empty_broker.py` & `agent-bdi-2.4.1/src/broker/empty_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/message_broker.py` & `agent-bdi-2.4.1/src/broker/message_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/mqtt_broker.py` & `agent-bdi-2.4.1/src/broker/mqtt_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/redis_broker.py` & `agent-bdi-2.4.1/src/broker/redis_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/ros_broker.py` & `agent-bdi-2.4.1/src/broker/ros_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/broker/ros_noetic_broker.py` & `agent-bdi-2.4.1/src/broker/ros_noetic_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/holon/HolonicAgent.py` & `agent-bdi-2.4.1/src/holon/HolonicAgent.py`

 * *Files 23% similar despite different names*

```diff
@@ -188,25 +188,15 @@
             return RequestLogistic(self)
         else:
             return BrokerLogistic(self)
 
 
     @final
     def publish(self, topic, payload=None):
-        # logistic_topic = topic
-        # packed_payload = payload
-        
-        # for logistic in self._logistics:
-        #     logistic_topic, packed_payload = logistic.pack(logistic_topic, packed_payload)
-            
-        # logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {packed_payload}")
-        # return self._broker.publish(logistic_topic, packed_payload)
-        # logistic = self.get_logistic(topic)
-        # packed = logistic.pack(payload)
-        # return self._publish(topic, packed)
+        # logger.debug(f"topic: {topic}, payload: {payload}")
         return self._broker.publish(topic, payload)
 
 
     @final
     def _publish(self, topic, payload=None):
         return self._broker.publish(topic, payload)
         
@@ -291,39 +281,22 @@
 
 
     @final
     def _on_message(self, topic:str, payload, payload_info=None):
         if topic in self._topic_handlers:
             topic_handler = self._topic_handlers[topic]
             if len(inspect.signature(topic_handler).parameters) == 2:
-                self._topic_handlers[topic](topic, payload)
+                return self._topic_handlers[topic](topic, payload)
             else:
-                self._topic_handlers[topic](topic, payload, payload_info)
+                return self._topic_handlers[topic](topic, payload, payload_info)
         else:
             if len(inspect.signature(self.on_message).parameters) == 2:
-                self.on_message(topic, payload)
+                return self.on_message(topic, payload)
             else:
-                self.on_message(topic, payload, payload_info)
-        
-        
-    # def _process_message(self, topic:str, payload):
-    #     logger.debug(f"payload: {len(payload)}")
-    #     if payload and self._request_logistic.is_request(payload):
-    #         logger.debug("message is_request")
-    #         threading.Thread(target=self._on_request, args=(topic, payload)).start()
-    #         # self._on_request(topic, payload)
-    #     elif payload and self._request_logistic.is_response(payload):
-    #         logger.debug(f"message is_response")
-    #         self._on_response(topic, payload)
-    #     else:
-    #         logger.debug(f"unmanaged payload")
-    #         if topic in self._topic_handlers:
-    #             self._topic_handlers[topic](topic, payload)
-    #         else:
-    #             self.on_message(topic, payload)
+                return self.on_message(topic, payload, payload_info)
 
 
     def on_message(self, topic:str, payload, payload_info=None):
         pass
```

### Comparing `agent-bdi-2.4.0/src/holon/logistics/loading_coordinator.py` & `agent-bdi-2.4.1/src/holon/logistics/loading_coordinator.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/holon/logistics/payload_wrapper.py` & `agent-bdi-2.4.1/src/holon/logistics/payload_wrapper.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/src/holon/logistics/request_logistic.py` & `agent-bdi-2.4.1/src/holon/logistics/request_logistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,29 @@
         self.agent.publish(logistic_topic, packed_payload)
         
         return request_token
 
 
     def subscribe(self, topic, topic_handler=None, datatype="str"):
         response_topic = f"{self.response_topic_header}.{topic}"
+        logger.debug(f"response_topic: {response_topic}")
         self.agent.subscribe(response_topic, datatype, self.handle_response)
         RequestLogistic.__handlers[self.response_topic_header] = topic_handler
 
 
     def handle_response(self, topic:str, payload):
         responsed_topic = topic[len(self.response_topic_header)+1:]
         unpacked = self._payload_wrapper.unpack(payload)
         logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}")
 
         if topic_handler := RequestLogistic.__handlers[self.response_topic_header]:
             self.agent.set_topic_handler(responsed_topic, topic_handler)
-        self.agent._on_message(responsed_topic, unpacked["content"], payload_info=unpacked["request_token"])
+        self.agent._on_message(topic=responsed_topic, 
+                               payload=unpacked["content"], 
+                               payload_info=unpacked["request_token"])
 
 
     # def handle_response(self, topic:str, payload):
     #     responsed_topic = topic[len(self.response_topic_header)+1:]
     #     # unpacked = self.unpack(payload)
     #     unpacked = self._payload_wrapper.unpack(payload)
     #     if unpacked["receiver"] == self.agent.agent_id:
```

### Comparing `agent-bdi-2.4.0/src/holon/logistics/response_logistic.py` & `agent-bdi-2.4.1/src/holon/logistics/response_logistic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import uuid
+import threading
 
 from abdi_config import LOGGER_NAME
 from holon.HolonicAgent import HolonicAgent
 from holon.logistics.base_logistic import BaseLogistic
 from holon.logistics.payload_wrapper import PayloadWrapper
 
 
@@ -14,46 +14,55 @@
 
 class ResponseLogistic(BaseLogistic):
     def __init__(self, agent:HolonicAgent):
         self.agent = agent
         self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
         
         
-    def publish(self, topic, payload):
-        sender_id = self.request_payload['sender']
-        request_id = self.request_payload['request_id']
-        logistic_topic = f"{PUBLISH_HEADER}.{sender_id}.{request_id}.{topic}"
-        packed_payload = self._payload_wrapper.wrap_for_response(payload, self.request_payload)
-        # logistic_topic, packed_payload = self.pack(topic, payload)
-        logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
-        self.agent.publish(logistic_topic, packed_payload)
+    # def publish(self, topic, payload):
+    #     sender_id = self.request_payload['sender']
+    #     request_id = self.request_payload['request_id']
+    #     logistic_topic = f"{PUBLISH_HEADER}.{sender_id}.{request_id}.{topic}"
+    #     packed_payload = self._payload_wrapper.wrap_for_response(payload, self.request_payload)
+    #     logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
+    #     # logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)}")
+    #     # self.agent.publish(logistic_topic, str(packed_payload))
+    #     self.agent.publish(logistic_topic, packed_payload)
 
 
     def subscribe(self, topic, topic_handler=None, datatype="str"):
         request_topic = f"{SUBSCRIBE_HEADER}.{topic}"
         logger.debug(f"request_topic: {request_topic}")
         self.agent.subscribe(request_topic, datatype, self.handle_request)
-        
+
         if topic_handler:
             self.agent.set_topic_handler(topic, topic_handler)
 
         
     def handle_request(self, topic:str, payload):
         logger.debug(f"topic: {topic}, payload: {str(payload)[:300]}...")
         request_topic = topic[len(SUBSCRIBE_HEADER)+1:]
-        self.request_payload = self._payload_wrapper.unpack(payload)
-        content = self.request_payload["content"]
-        # logger.debug(f"request_topic: {request_topic}, agent_id: {self.agent.agent_id}, content: {content}")
-        self.agent._on_message(request_topic, content)
-
-
-    # def pack(self, topic:str, payload):
-    #     if topic == self.request_topic:
-    #         packed = self._payload_wrapper.wrap_for_response(payload, self.request_payload)
-    #         return f"{PUBLISH_HEADER}.{topic}", packed
-    #     else:
-    #         return topic, payload
-
-
-    # def unpack(self, payload):
-    #     unpacked = self._payload_wrapper.unpack(payload)
-    #     return unpacked
+        request_payload = self._payload_wrapper.unpack(payload)
+        
+        def on_message(request_topic, request_payload):
+            output = self.agent._on_message(request_topic, request_payload["content"])
+            if output and isinstance(output, tuple) and len(output) == 2:
+                resp_topic, resp_result = output
+                sender_id = request_payload['sender']
+                request_id = request_payload['request_id']
+                logistic_topic = f"{PUBLISH_HEADER}.{sender_id}.{request_id}.{resp_topic}"
+                packed_payload = self._payload_wrapper.wrap_for_response(resp_result, request_payload)
+                logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
+                self.agent.publish(logistic_topic, packed_payload)
+            
+        threading.Thread(target=on_message, 
+                         args=(request_topic, request_payload)).start()
+        # self.agent._on_message(request_topic, request_payload["content"])
+
+        
+    # def handle_request(self, topic:str, payload):
+    #     logger.debug(f"topic: {topic}, payload: {str(payload)[:300]}...")
+    #     request_topic = topic[len(SUBSCRIBE_HEADER)+1:]
+    #     self.request_payload = self._payload_wrapper.unpack(payload)
+    #     content = self.request_payload["content"]
+    #     # logger.debug(f"request_topic: {request_topic}, agent_id: {self.agent.agent_id}, content: {content}")
+    #     self.agent._on_message(request_topic, content)
```

### Comparing `agent-bdi-2.4.0/tests/test_loadingbal.py` & `agent-bdi-2.4.1/tests/test_loadingbal.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/tests/test_request.py` & `agent-bdi-2.4.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.0/tests/test_send.py` & `agent-bdi-2.4.1/tests/test_send.py`

 * *Files identical despite different names*

