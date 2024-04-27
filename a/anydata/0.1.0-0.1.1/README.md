# Comparing `tmp/anydata-0.1.0.tar.gz` & `tmp/anydata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydata-0.1.0.tar", max compression
+gzip compressed data, was "anydata-0.1.1.tar", max compression
```

## Comparing `anydata-0.1.0.tar` & `anydata-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-01 21:27:17.734610 anydata-0.1.0/LICENSE
--rw-r--r--   0        0        0        9 2024-04-01 21:27:17.734734 anydata-0.1.0/README.md
--rw-r--r--   0        0        0       69 2024-04-01 23:18:17.446624 anydata-0.1.0/anydata/__init__.py
--rw-r--r--   0        0        0    10014 2024-04-03 04:10:20.922198 anydata-0.1.0/anydata/core/dataapi.py
--rw-r--r--   0        0        0     7797 2024-04-03 03:04:12.951439 anydata-0.1.0/anydata/core/endpoint.py
--rw-r--r--   0        0        0     6680 2024-04-04 02:31:10.427039 anydata-0.1.0/anydata/engine/functions.py
--rw-r--r--   0        0        0      343 2024-04-01 21:29:01.793515 anydata-0.1.0/anydata/engine/models.py
--rw-r--r--   0        0        0     1303 2024-04-01 21:29:01.800618 anydata-0.1.0/anydata/engine/prompts/system_prompts.py
--rw-r--r--   0        0        0     1156 2024-04-01 21:29:01.800928 anydata-0.1.0/anydata/engine/prompts/user_prompts.py
--rw-r--r--   0        0        0     6148 2024-04-01 21:29:15.125940 anydata-0.1.0/anydata/parsers/.DS_Store
--rw-r--r--   0        0        0     8550 2024-04-01 22:48:49.129458 anydata-0.1.0/anydata/parsers/openapi.py
--rw-r--r--   0        0        0     2039 2024-04-01 23:09:38.254952 anydata-0.1.0/anydata/parsers/response_parser.py
--rw-r--r--   0        0        0     4529 2024-04-03 00:04:13.649448 anydata-0.1.0/anydata/schemas/core.py
--rw-r--r--   0        0        0     2595 2024-04-01 21:29:26.598807 anydata-0.1.0/anydata/schemas/openapi.py
--rw-r--r--   0        0        0      553 2024-04-04 04:54:42.425818 anydata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 anydata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 21:27:17.734610 anydata-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3393 2024-04-13 02:44:50.881249 anydata-0.1.1/README.md
+-rw-r--r--   0        0        0       70 2024-04-05 23:57:59.131667 anydata-0.1.1/anydata/__init__.py
+-rw-r--r--   0        0        0    18782 2024-04-27 19:11:50.495308 anydata-0.1.1/anydata/core/dataapi.py
+-rw-r--r--   0        0        0    11126 2024-04-27 14:45:59.271171 anydata-0.1.1/anydata/core/endpoint.py
+-rw-r--r--   0        0        0     6146 2024-04-05 23:57:59.132977 anydata-0.1.1/anydata/engine/functions.py
+-rw-r--r--   0        0        0      377 2024-04-05 23:57:59.133267 anydata-0.1.1/anydata/engine/models.py
+-rw-r--r--   0        0        0     1303 2024-04-05 23:57:59.133579 anydata-0.1.1/anydata/engine/prompts/system_prompts.py
+-rw-r--r--   0        0        0     1159 2024-04-05 23:57:59.133974 anydata-0.1.1/anydata/engine/prompts/user_prompts.py
+-rw-r--r--   0        0        0       93 2024-04-07 06:53:49.947855 anydata-0.1.1/anydata/exceptions.py
+-rw-r--r--   0        0        0    11192 2024-04-27 17:45:13.060192 anydata-0.1.1/anydata/parsers/openapi.py
+-rw-r--r--   0        0        0     2084 2024-04-27 19:10:03.996974 anydata-0.1.1/anydata/parsers/response_parser.py
+-rw-r--r--   0        0        0     4510 2024-04-05 23:57:59.135519 anydata-0.1.1/anydata/schemas/core.py
+-rw-r--r--   0        0        0     2637 2024-04-05 23:57:59.136123 anydata-0.1.1/anydata/schemas/openapi.py
+-rw-r--r--   0        0        0      745 2024-04-27 19:29:48.001539 anydata-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 anydata-0.1.1/PKG-INFO
```

### Comparing `anydata-0.1.0/LICENSE` & `anydata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anydata-0.1.0/anydata/engine/functions.py` & `anydata-0.1.1/anydata/engine/functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,171 @@
-import json
-import yaml
 from typing import Optional
 import guidance
 from guidance import gen, system, user, assistant, select
 from ..parsers.openapi import OpenAPI
 from ..engine.prompts.system_prompts import (
     RELATIVE_URL_FETCHER,
     REST_API_OPERATION_FETCHER,
     REST_API_PARAMETERS_FETCHER,
 )
 from ..engine.prompts.user_prompts import (
     relative_url_user_prompt,
     rest_api_operation_user_prompt,
-    rest_api_parameters_user_prompt
+    rest_api_parameters_user_prompt,
 )
 
-#%% Chaining guidance operations
+
+# %% Chaining guidance operations
 @guidance
-def dataapi_from_prompt(lm: guidance.models.Model,
-                        prompt: str,
-                        openapi: OpenAPI) -> guidance.models.Model:
-    '''
+def dataapi_from_prompt(
+    lm: guidance.models.Model, prompt: str, openapi: OpenAPI
+) -> guidance.models.Model:
+    """
     Chain guidance operations to:
         1. Retrieve the relative URL for an endpoint from the 'openapi' to fulfill the 'prompt'.
         2. Retrieve the REST API operation for the endpoint from the 'openapi' to fulfill the 'prompt'.
         3. Retrieve the REST API parameters for the endpoint from the 'openapi' to fulfill the 'prompt'.
-    '''
+    """
     assert isinstance(openapi, OpenAPI), "openapi must be a valid OpenAPI object."
     lm += relative_url_from_openapi(prompt, openapi)
     lm += rest_api_operation_from_openapi(prompt, openapi)
     lm += rest_api_parameters_from_openapi(prompt, openapi)
     return lm
 
+
 @guidance
-def retry_dataapi_from_prompt(lm: guidance.models.Model,
-                              prompt: str,
-                              openapi: OpenAPI) -> guidance.models.Model:
-    '''
+def retry_dataapi_from_prompt(
+    lm: guidance.models.Model, prompt: str, openapi: OpenAPI
+) -> guidance.models.Model:
+    """
     Retries a failed dataapi_from_prompt operation with instructions from a failed response.
-    '''
+    """
     assert isinstance(openapi, OpenAPI), "openapi must be a valid OpenAPI object."
 
 
-#%% Base guidance operations
+# %% Base guidance operations
 @guidance
-def relative_url_from_openapi(lm: guidance.models.Model,
-                              prompt: str,
-                              openapi: OpenAPI
-                              ) -> guidance.models.Model:
-    '''
+def relative_url_from_openapi(
+    lm: guidance.models.Model, prompt: str, openapi: OpenAPI
+) -> guidance.models.Model:
+    """
     Returns a guidance lm model carrying a relative URL for the endpoint at the 'endpoint' variable.
-    '''
+    """
     endpoints = list(openapi.paths)
     # endpoints_summary = yaml.dump(openapi.summary())
     endpoints_summary = openapi.summary()
     with system():
         lm += RELATIVE_URL_FETCHER
     with user():
         lm += relative_url_user_prompt(prompt, endpoints_summary, endpoints)
     with assistant():
-        lm += select(endpoints, name='endpoint')
+        lm += select(endpoints, name="endpoint")
     return lm
 
+
 @guidance
-def rest_api_operation_from_openapi(lm: guidance.models.Model,
-                                    prompt: str,
-                                    openapi: OpenAPI,
-                                    endpoint: Optional[str]=None
-                                    ) -> guidance.models.Model:
-    '''
+def rest_api_operation_from_openapi(
+    lm: guidance.models.Model,
+    prompt: str,
+    openapi: OpenAPI,
+    endpoint: Optional[str] = None,
+) -> guidance.models.Model:
+    """
     Returns a guidance lm model carrying a REST API operation for the endpoint at the 'method' variable.
-    '''
+    """
     if not endpoint:
-        assert 'endpoint' in lm, "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
-        endpoint = lm['endpoint']
+        assert (
+            "endpoint" in lm
+        ), "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
+        endpoint = lm["endpoint"]
     # endpoint_summary = yaml.dump(openapi.paths_summary()[endpoint])
     endpoint_summary = openapi.paths_summary()[endpoint]
     endpoint_methods = dict(openapi.endpoint_methods)[endpoint]
     with system():
         lm += REST_API_OPERATION_FETCHER
     with user():
         lm += rest_api_operation_user_prompt(prompt, endpoint, endpoint_summary)
     with assistant():
-        lm += select(endpoint_methods, name='method')
+        lm += select(endpoint_methods, name="method")
     return lm
 
+
 @guidance
-def rest_api_parameters_from_openapi(lm: guidance.models.Model,
-                                     prompt: str,
-                                     openapi: OpenAPI,
-                                     endpoint: Optional[str]=None,
-                                     method: Optional[str]=None,
-                                     temperature: Optional[float]=0.0
-                                     ) -> guidance.models.Model:
-    '''
+def rest_api_parameters_from_openapi(
+    lm: guidance.models.Model,
+    prompt: str,
+    openapi: OpenAPI,
+    endpoint: Optional[str] = None,
+    method: Optional[str] = None,
+    temperature: Optional[float] = 0.0,
+) -> guidance.models.Model:
+    """
     Returns a guidance lm model carrying a JSON object with key value pairs for the parameters needed to call the endpoint.
-    '''
+    """
     if not endpoint:
-        assert 'endpoint' in lm, "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
-        endpoint = lm['endpoint']
+        assert (
+            "endpoint" in lm
+        ), "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
+        endpoint = lm["endpoint"]
     if not method:
-        assert 'method' in lm, "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
-        method = lm['method']
+        assert (
+            "method" in lm
+        ), "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
+        method = lm["method"]
     # method_openapi = yaml.dump(openapi.paths_summary(resolve_parameter_references=True)[endpoint][method])
-    method_openapi = openapi.paths_summary(resolve_parameter_references=True)[endpoint][method]
+    method_openapi = openapi.paths_summary(resolve_parameter_references=True)[endpoint][
+        method
+    ]
     with system():
         lm += REST_API_PARAMETERS_FETCHER
     with user():
         lm += rest_api_parameters_user_prompt(prompt, endpoint, method_openapi)
     with assistant():
         lm += gen(name="parameters", temperature=temperature)
     return lm
 
+
 @guidance
-def evaluate_unsuccessful_response(lm: guidance.models.Model,
-                                   prompt: str,
-                                   response: dict,
-                                   endpoint: Optional[str]=None,
-                                   method: Optional[str]=None,
-                                   parameters: Optional[dict]=None
-                                   ) -> guidance.models.Model:
-    '''
+def evaluate_unsuccessful_response(
+    lm: guidance.models.Model,
+    prompt: str,
+    response: dict,
+    endpoint: Optional[str] = None,
+    method: Optional[str] = None,
+    parameters: Optional[dict] = None,
+) -> guidance.models.Model:
+    """
     Evaluates the response from a REST API call and raises an error if the response is unsuccessful.
-    '''
+    """
     if not endpoint:
-        assert 'endpoint' in lm, "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
-        endpoint = lm['endpoint']
+        assert (
+            "endpoint" in lm
+        ), "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
+        endpoint = lm["endpoint"]
     if not method:
-        assert 'method' in lm, "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
-        method = lm['method']
+        assert (
+            "method" in lm
+        ), "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
+        method = lm["method"]
     if not parameters:
-        assert 'parameters' in lm, "If 'parameters' is not provided, it must be captured at the 'parameters' variable in the lm model."
-        parameters = lm['parameters']
+        assert (
+            "parameters" in lm
+        ), "If 'parameters' is not provided, it must be captured at the 'parameters' variable in the lm model."
+        parameters = lm["parameters"]
     with system():
-        lm += '''
+        lm += """
 You only reply with a number corresponding to one of the following options:
     1. The parameters provided are incorrect.
     2. The REST API operation is incorrect.
-    3. The endpoint is incorrect.    
-        '''
+    3. The endpoint is incorrect.
+        """
     with user():
-        lm += f'''
+        lm += f"""
 When attempting to retrieve data for the prompt '{prompt}', a '{method}' request was made to the endpoint '{endpoint}' with the following parameters:
 {parameters}
 The request receive an unsuccessful response with status code '{response.status_code}' and the following content:
 {response.text}
 What do you think is the reason for the unsuccessful response?
-        '''
+        """
     with assistant():
-        lm += select([1, 2, 3], name='reason')
-    return lm
+        lm += select([1, 2, 3], name="reason")
+    return lm
```

### Comparing `anydata-0.1.0/anydata/engine/prompts/system_prompts.py` & `anydata-0.1.1/anydata/engine/prompts/system_prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 REST_API_OPERATIONS_STR = "'get', 'post', 'put', 'delete', 'head', or 'options'"
 
-REST_API_OPERATIONS_LST = ['get', 'post', 'put', 'delete', 'head', 'options']
+REST_API_OPERATIONS_LST = ["get", "post", "put", "delete", "head", "options"]
 
 # EXAMPLE_REST_API_PARAMETERS = '''
 # {"string_parameter": "string_value", "integer_parameter": 20}
 # '''
 
-RELATIVE_URL_FETCHER = '''You only reply with a relative url that starts with '/'. If the endpoint contains path parameters, do not replace them with the parameter values, return the parameter name within curly braces. Return the relative url as described in the API documentation. You don't include anything else in your reply, other than the relative url.
-'''
+RELATIVE_URL_FETCHER = """You only reply with a relative url that starts with '/'. If the endpoint contains path parameters, do not replace them with the parameter values, return the parameter name within curly braces. Return the relative url as described in the API documentation. You don't include anything else in your reply, other than the relative url.
+"""
 
-REST_API_OPERATION_FETCHER = f'''You only reply with one of the following valid REST API operations {REST_API_OPERATIONS_STR}. You don't include anything else in your reply, other than the REST API operation.
-'''
+REST_API_OPERATION_FETCHER = f"""You only reply with one of the following valid REST API operations {REST_API_OPERATIONS_STR}. You don't include anything else in your reply, other than the REST API operation.
+"""
 
 # REST_API_PARAMETERS_FETCHER = f'''You only reply with a json object with key value pairs. The keys are the parameter names and the values are the parameter values for a REST API call to an endpoint.
 # Example answer: {EXAMPLE_REST_API_PARAMETERS}
 # '''
 
-REST_API_PARAMETERS_FETCHER = f'''You only reply with a json object with key value pairs. The keys are the parameter names and the values are the parameter values for a REST API call to an endpoint.
-'''
+REST_API_PARAMETERS_FETCHER = """You only reply with a json object with key value pairs. The keys are the parameter names and the values are the parameter values for a REST API call to an endpoint.
+"""
```

### Comparing `anydata-0.1.0/anydata/engine/prompts/user_prompts.py` & `anydata-0.1.1/anydata/engine/prompts/user_prompts.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 Choose one from the following endpoints:
 {endpoints}
 
 If the endpoint contains path parameters, do not replace them with the parameter values, return the parameter name within curly braces.
     """
 
+
 def rest_api_operation_user_prompt(prompt: str, endpoint: str, openapi: str):
-    return f'''Given the following OpenAPI specification, which REST API method should I use when calling the endpoint {endpoint} to fulfill the prompt '{prompt}'?
+    return f"""Given the following OpenAPI specification, which REST API method should I use when calling the endpoint {endpoint} to fulfill the prompt '{prompt}'?
 
 {openapi}
-    '''
+    """
+
 
 def rest_api_parameters_user_prompt(prompt: str, endpoint: str, openapi: str):
-    return f'''Given the following OpenAPI specification, which parameters should I pass when calling the endpoint {endpoint} to return all available data in json format for the prompt '{prompt}'?
+    return f"""Given the following OpenAPI specification, which parameters should I pass when calling the endpoint {endpoint} to return all available data in json format for the prompt '{prompt}'?
 Return only required parameters and optional parameters needed to fulfill the prompt '{prompt}'.
 
 {openapi}
 
 If no parameter is needed to fulfill the prompt '{prompt}', return an empty JSON object.
-    '''
+    """
```

### Comparing `anydata-0.1.0/anydata/parsers/openapi.py` & `anydata-0.1.1/anydata/parsers/openapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import os
 import json
+import yaml
+import requests
+from json.decoder import JSONDecodeError
+from yaml.parser import ParserError
+from urllib.parse import urlparse
 from typing import List, Dict, Union, Tuple
+
 from ..schemas.openapi import Info, Server, PathItem, OPENAPI_OPERATIONS
+from ..exceptions import InvalidOpenAPIFormat
 
-'''
+"""
 How-to from swaggerhub to json:
 https://support.smartbear.com/swaggerhub/docs/en/manage-apis/download-api-definitions-from-swaggerhub.html#:~:text=Open%20the%20API%20in%20the,desired%20format%20%E2%80%93%20YAML%20or%20JSON.
 
 Example:
 https://app.swaggerhub.com/apis-docs/I2875/PM25_Open_Data/1.0.0
 Change /apis-docs/ to /apis/ to get to the Full specification hub
 https://app.swaggerhub.com/apis/I2875/PM25_Open_Data/1.0.0
 Change //app. to //api. to get to the json specification
-'''
+"""
+
 
-#%% OpenAPI components parsers
+# %% OpenAPI components parsers
 def openapi_info_from_dict(openapi_dict: dict) -> Info:
     try:
-        info = Info.from_dict(openapi_dict['info'])
+        info = Info.from_dict(openapi_dict["info"])
     except KeyError:
         info = Info()
     return info
 
+
 def openapi_servers_from_dict(openapi_dict: dict) -> List[Server]:
-    return Server.schema().load(openapi_dict['servers'], many=True)
+    return Server.schema().load(openapi_dict["servers"], many=True)
+
 
 def openapi_paths_from_dict(openapi_dict: dict) -> Dict[str, PathItem]:
-    return {k: PathItem.from_dict(v) for k, v in openapi_dict['paths'].items()}
+    return {k: PathItem.from_dict(v) for k, v in openapi_dict["paths"].items()}
 
-#%% Auxiliary functions
+
+# %% Auxiliary functions
 def resolve_references(relative_dict, complete_dict):
-    '''
+    """
     Recursively resolves references in a dictionary with values from an external dictionary.
     resolve_ref and resolve are encapsulated for a cleaner namespace.
-    '''
+    """
+
     def resolve_ref(complete_element, ref_element):
-        if ref_element.startswith('#'):
-            keys = ref_element.split('/')[1:]
+        if ref_element.startswith("#"):
+            keys = ref_element.split("/")[1:]
             current = complete_element
             for key in keys:
                 current = current[key]
             return current
         return ref_element
 
     def resolve(element):
@@ -51,148 +63,220 @@
         elif isinstance(element, str):
             return resolve_ref(complete_dict, element)
         else:
             return element
 
     return resolve(relative_dict)
 
+
 # OpenAPI instantiation functions
-def openapi_dict_from_json_str(openapi_json: str) -> dict:
-    return json.loads(openapi_json)
+def openapi_dict_from_str(openapi_str: str) -> dict:
+    try:
+        return json.loads(openapi_str)
+    except JSONDecodeError:
+        pass
+    try:
+        return yaml.safe_load(openapi_str)
+    except ParserError:
+        raise InvalidOpenAPIFormat("The input must be a valid JSON or YAML.")
 
-def openapi_dict_from_json_file(openapi_json_file: str) -> dict:
-    assert openapi_json_file.endswith('.json'), "This method expects a .json file."
-    with open(openapi_json_file, 'r') as f:
-        return json.load(f)
-
-def instantiate_openapi(openapi: Union[str, dict]) -> 'OpenAPI':
-        if isinstance(openapi, OpenAPI):
-            return openapi
-        else:
-            try:
-                if isinstance(openapi, dict):
-                    openapi = OpenAPI(openapi)
-                else:
-                    openapi = OpenAPI.from_json(openapi)
-            except Exception as e:
-                raise ValueError(f"An error occurred while parsing the Open API Specification: {e}")
-            return openapi
 
-#%% OpenAPI class
+def openapi_dict_from_file(openapi_file: str) -> dict:
+    with open(openapi_file, "r") as f:
+        openapi_dict = openapi_dict_from_str(f.read())
+    return openapi_dict
+
+
+# %% OpenAPI class
 class OpenAPI:
-    def __init__(self, openapi_dict: dict) -> None:
-        '''
-        Instantiates an OpenAPI object from a dictionary.
-        '''
-        self.info = openapi_info_from_dict(openapi_dict)
-        self.servers = openapi_servers_from_dict(openapi_dict)
-        self.paths = openapi_paths_from_dict(openapi_dict)
-        self.json = openapi_dict
+    """Parser for OpenAPI specifications."""
+
+    def __init__(self, openapi_spec: Union[str, dict]) -> None:
+        """
+        Instantiates an OpenAPI object from an Open API specification. The specification can be a dictionary, a JSON or YAML string, or a file path.
+        """
+        self.json = openapi_spec
+        self.info = openapi_info_from_dict(self._json)
+        self.servers = openapi_servers_from_dict(self._json)
+        self.paths = openapi_paths_from_dict(self._json)
+
+    @property
+    def json(self):
+        return self._json
+
+    @json.setter
+    def json(self, openapi_spec: Union[str, dict]):
+        """Sets the OpenAPI specification as a dictionary. Takes as input a dictionary, a JSON or YAML string, a file path, or a URL.
+
+        Args:
+            openapi_spec (Union[str, dict]): A dictionary, a JSON or YAML string, a file path, or a URL containing the OpenAPI specification.
+
+        Raises:
+            InvalidOpenAPIFormat: Raises on invalid input.
+        """
+        if isinstance(openapi_spec, dict):
+            self._json = openapi_spec
+        elif isinstance(openapi_spec, str):
+            if urlparse(openapi_spec).scheme in ["http", "https"]:
+                openapi_spec = requests.get(openapi_spec).text
+                openapi_spec = openapi_dict_from_str(openapi_spec)
+            elif os.path.isfile(openapi_spec):
+                openapi_spec = openapi_dict_from_file(openapi_spec)
+            else:
+                openapi_spec = openapi_dict_from_str(openapi_spec)
+            self._json = openapi_spec
+        else:
+            raise InvalidOpenAPIFormat(
+                "The OpenAPI specification must be either a dictionary or as a valid JSON or YAML source."
+            )
 
     def to_dict(self):
-        '''
+        """
         Returns the OpenAPI object as a dictionary.
-        This method doesn't reconstruct the originating OpenAPI dictionary.
-        '''
+        This method doesn't reconstruct the originating OpenAPI dictionary, which can be accessed from the `.json` parameter.
+        """
         return {
             "info": self.info._to_dict(),
             "servers": [s._to_dict() for s in self.servers],
-            "paths": {k: v._to_dict() for k, v in self.paths.items()}
+            "paths": {k: v._to_dict() for k, v in self.paths.items()},
         }
 
-    @classmethod
-    def from_json(cls, openapi_json: Union[str, os.PathLike]) -> 'OpenAPI':
-        '''
-        This method supports reading from a json string or from a json file path.
-            my_openapi = OpenAPI.from_json('{"info": {"title": "My API"}}')
-            my_openapi = OpenAPI.from_json('path/to/openapi.json')
-        '''
-        if os.path.isfile(openapi_json):
-            return cls(openapi_dict_from_json_file(openapi_json))
-        else:
-            return cls(openapi_dict_from_json_str(openapi_json))
-    
     # Summarizers
     @property
     def endpoint_methods(self) -> List[Tuple[str, List[str]]]:
-        '''
-        Returns a list of tuples with the endpoints and its available methods from OpenAPI paths.
-        (endpoint, [methods])
-        '''
+        """Lists endpoints and its available methods from OpenAPI paths.
+
+        Returns:
+            List[Tuple[str, List[str]]]: List of tuples with the endpoint and its available methods in a format (endpoint, [methods]).
+        """
         endpoints_methods = []
         for endpoint, path_item in self.paths.items():
-            endpoints_methods.append((endpoint, [o for (o, _) in path_item.operations()]))
+            endpoints_methods.append(
+                (endpoint, [o for (o, _) in path_item.operations()])
+            )
         return endpoints_methods
 
     def info_summary(
         self,
-        excluded_info_properties: List[str]=['termsOfService', 'contact', 'license', 'version']
+        excluded_info_properties: List[str] = [
+            "termsOfService",
+            "contact",
+            "license",
+            "version",
+        ],
     ) -> dict:
-        '''
-        Returns a summary of the OpenAPI info.
-        Parameters:
-            - excluded_info_properties: List of properties to exclude from the Info object.
-        Returns a dictionary with the remaining properties.
-        '''
+        """Returns a summary of the OpenAPI info.
+
+        Args:
+            excluded_info_properties (List[str], optional): List of properties to exclude from the Info object. Defaults to [ "termsOfService", "contact", "license", "version", ].
+
+        Returns:
+            dict: Returns a dictionary with the remaining properties.
+        """
         return self.info.summarize(excluded_properties=excluded_info_properties)
-    
-    def servers_summary(self, excluded_server_properties: List[str]=['']) -> List[dict]:
-        '''
-        Returns a summary of the OpenAPI servers.
-        --- This function is currently not excluding any properties from the Server objects. ---
-        Returns a dictionary with the properties of each Server object.
-        '''
-        return [s.summarize(excluded_properties=excluded_server_properties) for s in self.servers]
-    
+
+    def servers_summary(
+        self, excluded_server_properties: List[str] = [""]
+    ) -> List[dict]:
+        """Returns a summary of the OpenAPI servers.
+
+        Args:
+            excluded_server_properties (List[str], optional): List of properties to exclude from the Server objects. Defaults to [""].
+
+        Returns:
+            List[dict]: Returns a dictionary with the properties of each Server object.
+        """
+        return [
+            s.summarize(excluded_properties=excluded_server_properties)
+            for s in self.servers
+        ]
+
     def paths_summary(
         self,
-        excluded_operation_properties: List[str]=['externalDocs', 'operationId'],
-        exclude_non_2XX_responses: bool=True,
-        resolve_parameter_references: bool=True
+        excluded_operation_properties: List[str] = ["externalDocs", "operationId"],
+        exclude_non_2XX_responses: bool = True,
+        resolve_parameter_references: bool = True,
     ) -> dict:
-        '''
+        """
         Returns a summary of the OpenAPI paths and its operations.
-        Parameters:
-            - excluded_operation_properties: List of properties to exclude from the Operation objects.
-            - exclude_non_2XX_responses: If True, excludes non-2XX responses from the 'responses' dictionary of the Operation objects.
-            Default: True
-        Returns a dictionary with the summarized properties of each PathItem and Operation objects.
-        '''
+
+        Args:
+            excluded_operation_properties (List[str], optional): List of properties to exclude from the Operation objects. Defaults to ["externalDocs", "operationId"].
+            exclude_non_2XX_responses (bool, optional): If True, excludes non-2XX responses from the 'responses' dictionary of the Operation objects. Defaults to True.
+            resolve_parameter_references (bool, optional): If True, resolves parameter references from the specification. Defaults to True.
+
+        Returns:
+            dict: A summarized json with the properties of each PathItem and its Operation objects.
+        """
         paths_summary = {}
         for path in self.paths:
             # Extract non-openapi-operations properties from each PathItem
-            paths_summary[path] = {k: v for k, v in self.paths[path]._to_dict().items() if k not in OPENAPI_OPERATIONS}
-            for (method, operation) in self.paths[path].operations():
+            paths_summary[path] = {
+                k: v
+                for k, v in self.paths[path]._to_dict().items()
+                if k not in OPENAPI_OPERATIONS
+            }
+            for method, operation in self.paths[path].operations():
                 # Summarize Operations
-                paths_summary[path][method] = operation.summarize(excluded_properties=excluded_operation_properties)
-                if exclude_non_2XX_responses and operation.responses and 'responses' in paths_summary[path][method]:
+                paths_summary[path][method] = operation.summarize(
+                    excluded_properties=excluded_operation_properties
+                )
+                if (
+                    exclude_non_2XX_responses
+                    and operation.responses
+                    and "responses" in paths_summary[path][method]
+                ):
                     # Excludes non-2XX responses from the paths_summary 'responses' dictionary
                     for response in list(operation.responses):
-                        if response.startswith('2'):
+                        if response.startswith("2"):
                             pass
                         else:
-                            del paths_summary[path][method]['responses'][response]
-                if resolve_parameter_references and 'parameters' in paths_summary[path][method]:
+                            del paths_summary[path][method]["responses"][response]
+                if (
+                    resolve_parameter_references
+                    and "parameters" in paths_summary[path][method]
+                ):
                     # Resolves 'parameters' references with values from the base openapi dictionary
-                    paths_summary[path][method]['parameters'] = resolve_references(
-                        paths_summary[path][method]['parameters'],
-                        self.json
+                    paths_summary[path][method]["parameters"] = resolve_references(
+                        paths_summary[path][method]["parameters"], self.json
                     )
         return paths_summary
-    
+
     def summary(
         self,
-        excluded_info_properties: List[str]=['termsOfService', 'contact', 'license', 'version'],
-        excluded_server_properties: List[str]=[''],
-        excluded_operation_properties: List[str]=['externalDocs', 'operationId', 'parameters', 'responses'],
-        exclude_non_2XX_responses: bool=True,
-        resolve_parameter_references: bool=False
-    ):
-        '''
-        Higher-level summary of the OpenAPI object.
-        Returns a dictionary that includes a summary of the info, servers, and paths parameters.
-        '''
+        excluded_info_properties: List[str] = [
+            "termsOfService",
+            "contact",
+            "license",
+            "version",
+        ],
+        excluded_server_properties: List[str] = [""],
+        excluded_operation_properties: List[str] = [
+            "externalDocs",
+            "operationId",
+            "parameters",
+            "responses",
+        ],
+        exclude_non_2XX_responses: bool = True,
+        resolve_parameter_references: bool = False,
+    ) -> dict:
+        """High-level summary of the OpenAPI object.
+
+        Args:
+            excluded_info_properties (List[str], optional): List of properties to exclude from the Info object. Defaults to [ "termsOfService", "contact", "license", "version", ].
+            excluded_server_properties (List[str], optional): List of properties to exclude from the Server objects. Defaults to [""].
+            excluded_operation_properties (List[str], optional): List of properties to exclude from the Operation objects. Defaults to [ "externalDocs", "operationId", "parameters", "responses", ].
+            exclude_non_2XX_responses (bool, optional): If True, excludes non-2XX responses from the 'responses' dictionary of the Operation objects. Defaults to True.
+            resolve_parameter_references (bool, optional): If True, resolves parameter references from the specification. Defaults to False.
+
+        Returns:
+            dict: A dictionary containing a summary of the info, servers, and paths parameters.
+        """
         return {
             "info": self.info_summary(excluded_info_properties),
             "servers": self.servers_summary(excluded_server_properties),
-            "paths": self.paths_summary(excluded_operation_properties, exclude_non_2XX_responses, resolve_parameter_references)
+            "paths": self.paths_summary(
+                excluded_operation_properties,
+                exclude_non_2XX_responses,
+                resolve_parameter_references,
+            ),
         }
```

### Comparing `anydata-0.1.0/anydata/parsers/response_parser.py` & `anydata-0.1.1/anydata/parsers/response_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 from requests.models import Response
 from typing import Union
+
 try:
     import pandas as pd
+
     is_pandas = True
 except ImportError:
     is_pandas = False
 
-def dataframe_from_array_of_dicts(array: list) -> 'pd.DataFrame':
-    '''
+
+def dataframe_from_array_of_dicts(array: list) -> "pd.DataFrame":
+    """
     Returns a pandas DataFrame from an array of dictionaries.
-    '''
-    if not is_pandas:
-        raise ImportError("Please install the 'pandas' package using `pip install pandas` to use this function.")
+    """
+    assert is_pandas, ImportError("Please install the 'pandas' package using `pip install pandas` to use this function.")
     try:
         return pd.DataFrame.from_dict(array, orient="columns")
     except Exception as e:
-        print(f"An error occurred while converting the array of type {type(array)} into a DataFrame: {e}")
+        print(
+            f"An error occurred while converting the array of type {type(array)} into a DataFrame: {e}"
+        )
         raise
 
-def json_response_to_pandas(response: Response) -> Union['pd.DataFrame', dict]:
-    '''
+
+def json_response_to_pandas(response: Response) -> Union["pd.DataFrame", dict]:
+    """
     Returns a pandas DataFrame from the response.
     If the response contains more than one array that can be converted into a DataFrame, it returns a dictionary of DataFrames.
-    '''
-    assert isinstance(response, Response), "response should be a requests.models.Response object"
+    """
+    assert isinstance(
+        response, Response
+    ), "response should be a requests.models.Response object"
     response = response.json()
     # Some APIs return a list of json at the top level. In this case, pass the list to the DataFrame constructor.
     if isinstance(response, list):
         return dataframe_from_array_of_dicts(response)
-    
+
     # In most cases, the response will be a dictionary. Look for arrays in the response and pass to the DataFrame constructor.
     array_keys = [key for key in response.keys() if isinstance(response[key], list)]
     # Single array found in response
     if len(array_keys) == 1:
         return dataframe_from_array_of_dicts(response[array_keys[0]])
     # Multiple arrays found in response
     elif len(array_keys) > 1:
         dfs = {}
         for key in array_keys:
             dfs[key] = dataframe_from_array_of_dicts(response[key])
-        print(f"Parser retrieved multiple DataFrames. Returning a dictionary of DataFrames with keys:\n{list(dfs.keys())}")
+        print(
+            f"Parser retrieved multiple DataFrames. Returning a dictionary of DataFrames with keys:\n{list(dfs.keys())}"
+        )
         return dfs
     else:
         print(f"No arrays found in response with {response.keys()}.")
-        return
+        return
```

### Comparing `anydata-0.1.0/anydata/schemas/core.py` & `anydata-0.1.1/anydata/schemas/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import copy
 from typing import Optional
-from requests.sessions import Session
 from collections.abc import MutableMapping
 from requests.sessions import Session, merge_setting
 
+
 class ABCDataAPI(MutableMapping):
-    '''
+    """
     Abstract Base Class for DataAPI
-    '''
+    """
+
     def __setitem__(self, key, value):
         self.__dict__[key] = value
 
     def __getitem__(self, key):
         try:
             return self.__dict__[key]
         except KeyError:
@@ -25,38 +26,40 @@
 
     def __iter__(self):
         raise NotImplementedError("Object of type DataAPI is not iterable")
 
     def __len__(self):
         raise TypeError("Object of type DataAPI has no len()")
 
+
 class EndpointSession(Session):
-    '''
+    """
     Base Class for Endpoint.
 
     Wrapper around requests.Session with a fixed endpoint (relative URL) and list of
     available methods.
-    '''
+    """
+
     def __init__(
-            self,
-            base_url: str,
-            endpoint: str,
-            method: str,
-            params: Optional[dict] = None,  # super: {}
-            body: Optional[dict] = None,    # renaming from Session.data
-            headers: Optional[dict] = None, # super: default_headers()
-            cookies: Optional[dict] = None, # super: cookiejar_from_dict({})
-            files: Optional[dict] = None,
-            auth: Optional[dict] = None,    # super: None
-            timeout: Optional[int] = None,
-            allow_redirects: Optional[bool] = True,
-            proxies: Optional[dict] = None, # super: {}
-            stream: Optional[bool] = False, # super: False
-            verify: Optional[bool] = True,  # super: True
-            cert: Optional[str] = None,     # super: None
+        self,
+        base_url: str,
+        endpoint: str,
+        method: str,
+        params: Optional[dict] = None,  # super: {}
+        body: Optional[dict] = None,  # renaming from Session.data
+        headers: Optional[dict] = None,  # super: default_headers()
+        cookies: Optional[dict] = None,  # super: cookiejar_from_dict({})
+        files: Optional[dict] = None,
+        auth: Optional[dict] = None,  # super: None
+        timeout: Optional[int] = None,
+        allow_redirects: Optional[bool] = True,
+        proxies: Optional[dict] = None,  # super: {}
+        stream: Optional[bool] = False,  # super: False
+        verify: Optional[bool] = True,  # super: True
+        cert: Optional[str] = None,  # super: None
     ):
         self.base_url = base_url
         self.endpoint = endpoint
         self.method = method
         self.body = body
         self.files = files
         self.timeout = timeout
@@ -74,54 +77,55 @@
         self.params = copy.deepcopy(params)
         self.auth = auth
         self.stream = stream
         self.verify = verify
         self.cert = cert
 
     def request(
-            self,
-            endpoint: Optional[str] = None,
-            params: Optional[dict] = None,
-            body: Optional[dict] = None,
-            headers: Optional[dict] = None,
-            files: Optional[dict] = None,
-            timeout: Optional[int] = None,
-            stream: Optional[bool] = False
+        self,
+        endpoint: Optional[str] = None,
+        params: Optional[dict] = None,
+        body: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        files: Optional[dict] = None,
+        timeout: Optional[int] = None,
+        stream: Optional[bool] = False,
     ):
-        '''
+        """
         At request time, you can redefine:
         - endpoint: relative URL
         - params: query string parameters
         - body: request body
         - headers: request headers
         - files: files to be sent with the request
         - timeout: request timeout
         - stream: flag to set stream mode
         All other parameters are set at session creation time.
-        '''
+        """
 
         # If 'endpoint' is not explicitly defined, use the default endpoint
+        # Explicitly defined endpoints allows endpoints with path parameters to be formatted at request time
         if not endpoint:
             endpoint = self.endpoint
 
         # Submits user defined 'params', 'body', 'headers', 'files',
         # and 'timeout' settings to Session.request().
         # Session.request() handles a merge of explict settings on request time
         # and settings defined at Session via merge_setting() function.
         resp = super().request(
             method=self.method,
-            url=self.base_url+endpoint,
+            url=self.base_url + endpoint,
             params=params or self.params,
             data=body or self.body,
             headers=headers or self.headers,
             cookies=self._cookies,
             files=files or self.files,
             auth=self.auth,
             timeout=timeout or self.timeout,
             allow_redirects=self.allow_redirects,
             proxies=self._proxies,
             hooks=self.hooks,
             stream=stream or self.stream,
             verify=self.verify,
-            cert=self.cert
+            cert=self.cert,
         )
-        return resp
+        return resp
```

### Comparing `anydata-0.1.0/anydata/schemas/openapi.py` & `anydata-0.1.1/anydata/schemas/openapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,106 @@
 import inspect
 from typing import Optional, List
-from abc import ABC, abstractmethod
+from abc import ABC
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 
-OPENAPI_OPERATIONS = ['get', 'put', 'post', 'delete', 'options', 'head', 'patch', 'trace']
+OPENAPI_OPERATIONS = [
+    "get",
+    "put",
+    "post",
+    "delete",
+    "options",
+    "head",
+    "patch",
+    "trace",
+]
+
 
 @dataclass_json
 class OpenAPIABC(ABC):
     ...
-    
+
     def _to_dict(self):
-        '''
+        """
         Wrapper around to_dict() method to remove None values from the dictionary representation.
-        '''
+        """
         return {k: v for k, v in self.to_dict().items() if v is not None}
-    
+
     def summarize(self, excluded_properties: List[str]):
-        '''
+        """
         Returns the object in dictionary format excluding the properties in the excluded_properties list.
-        '''
-        return {k: v for k, v in self._to_dict().items() if k not in excluded_properties}
+        """
+        return {
+            k: v for k, v in self._to_dict().items() if k not in excluded_properties
+        }
+
 
 # Info OpenAPI Component
 @dataclass
 class Contact(OpenAPIABC):
     name: Optional[str] = None
     url: Optional[str] = None
     email: Optional[str] = None
 
+
 @dataclass
 class License(OpenAPIABC):
     name: Optional[str] = None
     identifier: Optional[str] = None
     url: Optional[str] = None
 
+
 @dataclass
 class Info(OpenAPIABC):
     title: Optional[str] = None
     summary: Optional[str] = None
     description: Optional[str] = None
     termsOfService: Optional[str] = None
     contact: Optional[Contact] = None
     license: Optional[License] = None
     version: Optional[str] = None
 
+
 # Server OpenAPI Component
 @dataclass
 class Server(OpenAPIABC):
     url: str
     description: Optional[str] = None
     variables: Optional[dict] = None
 
+
 # Path OpenAPI Component
 @dataclass
 class ExternalDocumentation(OpenAPIABC):
     url: str
     description: Optional[str] = None
 
+
 @dataclass
 class Operation(OpenAPIABC):
     tags: Optional[List[str]] = None
     summary: Optional[str] = None
     description: Optional[str] = None
     externalDocs: Optional[ExternalDocumentation] = None
     operationId: Optional[str] = None
     parameters: Optional[List[dict]] = None
     requestBody: Optional[dict] = None
     responses: Optional[dict] = None
     deprecated: Optional[bool] = None
 
+
 @dataclass
 class PathItem(OpenAPIABC):
     summary: Optional[str] = None
     description: Optional[str] = None
     get: Optional[Operation] = None
     put: Optional[Operation] = None
     post: Optional[Operation] = None
     delete: Optional[Operation] = None
     options: Optional[Operation] = None
     head: Optional[Operation] = None
     patch: Optional[Operation] = None
     trace: Optional[Operation] = None
 
     def operations(self):
-        return inspect.getmembers(self, lambda a: isinstance(a, Operation))
+        return inspect.getmembers(self, lambda a: isinstance(a, Operation))
```

### Comparing `anydata-0.1.0/pyproject.toml` & `anydata-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 [tool.poetry]
 name = "anydata"
-version = "0.1.0"
+version = "0.1.1"
 description = "Smart framework to interact with and fetch data from REST APIs."
 authors = ["Erich Silva <erich@esilva.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
-guidance = "^0.1.13"
 dataclasses-json = "^0.6.4"
 pyyaml = "^6.0.1"
+guidance = { version = "^0.1.13", optional = true }
+
+[tool.poetry.extras]
+guidance = ["guidance"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
-ruff = "^0.3.5"
+ruff = "^0.1.0"
 python-dotenv = "^1.0.1"
+pre-commit = "^3.7.0"
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+"anydata/engine/models.py" = ["F401"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

