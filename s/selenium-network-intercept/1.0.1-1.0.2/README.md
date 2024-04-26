# Comparing `tmp/selenium-network-intercept-1.0.1.tar.gz` & `tmp/selenium_network_intercept-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-network-intercept-1.0.1.tar", last modified: Wed Apr 10 06:00:16 2024, max compression
+gzip compressed data, was "selenium_network_intercept-1.0.2.tar", last modified: Fri Apr 26 22:12:12 2024, max compression
```

## Comparing `selenium-network-intercept-1.0.1.tar` & `selenium_network_intercept-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.378982 selenium-network-intercept-1.0.1/
--rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-1.0.1/LICENCE
--rw-rw-rw-   0        0        0     6905 2024-04-10 06:00:16.377977 selenium-network-intercept-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6471 2024-04-10 05:59:09.000000 selenium-network-intercept-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.369979 selenium-network-intercept-1.0.1/selenium_network_intercept/
--rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/__init__.py
--rw-rw-rw-   0        0        0       39 2024-04-08 18:15:43.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/exceptions.py
--rw-rw-rw-   0        0        0     4446 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/intercept.py
--rw-rw-rw-   0        0        0     3542 2024-04-09 22:44:25.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/objected.py
--rw-rw-rw-   0        0        0     2226 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/request.py
--rw-rw-rw-   0        0        0     1580 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/response.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.376978 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/
--rw-rw-rw-   0        0        0     6905 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.375979 selenium-network-intercept-1.0.1/selenium_search_file/
--rw-rw-rw-   0        0        0       36 2024-04-10 05:46:53.000000 selenium-network-intercept-1.0.1/selenium_search_file/__init__.py
--rw-rw-rw-   0        0        0     3417 2024-04-10 05:46:45.000000 selenium-network-intercept-1.0.1/selenium_search_file/search_file.py
--rw-rw-rw-   0        0        0       42 2024-04-10 06:00:16.378982 selenium-network-intercept-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-04-10 05:59:55.000000 selenium-network-intercept-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 22:12:12.260239 selenium_network_intercept-1.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium_network_intercept-1.0.2/LICENCE
+-rw-rw-rw-   0        0        0     9579 2024-04-26 22:12:12.260239 selenium_network_intercept-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9145 2024-04-26 22:05:50.000000 selenium_network_intercept-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 22:12:12.251574 selenium_network_intercept-1.0.2/selenium_network_intercept/
+-rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium_network_intercept-1.0.2/selenium_network_intercept/__init__.py
+-rw-rw-rw-   0        0        0     6239 2024-04-26 22:02:08.000000 selenium_network_intercept-1.0.2/selenium_network_intercept/intercept.py
+drwxrwxrwx   0        0        0        0 2024-04-26 22:12:12.258688 selenium_network_intercept-1.0.2/selenium_network_intercept.egg-info/
+-rw-rw-rw-   0        0        0     9579 2024-04-26 22:12:12.000000 selenium_network_intercept-1.0.2/selenium_network_intercept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-26 22:12:12.000000 selenium_network_intercept-1.0.2/selenium_network_intercept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 22:12:12.000000 selenium_network_intercept-1.0.2/selenium_network_intercept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-26 22:12:12.000000 selenium_network_intercept-1.0.2/selenium_network_intercept.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 22:12:12.256780 selenium_network_intercept-1.0.2/selenium_search_file/
+-rw-rw-rw-   0        0        0       36 2024-04-10 05:46:53.000000 selenium_network_intercept-1.0.2/selenium_search_file/__init__.py
+-rw-rw-rw-   0        0        0     3417 2024-04-10 05:46:45.000000 selenium_network_intercept-1.0.2/selenium_search_file/search_file.py
+-rw-rw-rw-   0        0        0       42 2024-04-26 22:12:12.261241 selenium_network_intercept-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-04-26 20:48:45.000000 selenium_network_intercept-1.0.2/setup.py
```

### Comparing `selenium-network-intercept-1.0.1/LICENCE` & `selenium_network_intercept-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.1/PKG-INFO` & `selenium_network_intercept-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,84 @@
-Metadata-Version: 2.1
-Name: selenium-network-intercept
-Version: 1.0.1
-Summary: Interceptador de requisições http não oficial do selenium 4
-Author: Alexandre Mariano
-Author-email: alexandre_mariano@hotmail.com.br
-License: MIT License
-Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept,search download selenium
-Description-Content-Type: text/markdown
-License-File: LICENCE
+## Atualização 1.0.2
+
+Trazendo novidades, agora é possível em vez de pesquisar diretamente pela rota desejada, você buscar todas requisições já realizadas pelo navegador, podendo ser verificado no [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main) utilizando o arquivo `example3.py`.
+
+**Agora tem a possibilida de além de somente fazer uma busca assim:**
+
+```powershell
+request = intercept_http(driver,'/route')
+```
+
+**É possível utilizar também desta forma:**
+
+```python
+request = intercept_http(driver,only_request=True)
+```
+
+Que trará um objeto que terá dois atributos importantes para esta funcionalidade 
+
+- requests
+- responses
+
+Estes atributos trarão a possibilidade de você mesmo validar todas as requisições que foram feitas desde o momento da abertura do navegador, sem preocupar com a implementação interna da biblioteca.
+
+***Mas lembre-se que ainda é possível buscar diretamente pela rota desejada***
+
+---
+
+**Use** 
+
+`request.requests`  Para ter acesso a todas requisições realizadas até o momento da chamada da função
+
+Para atualizar essa lista, utilize `request.update()`
+
+Itere sobre esta lista para fazer a própria varredura e verificar o que desejar por exemplo, buscar pela URL:
+
+```python
+for req in request.requests:
+    print(req.url)
+```
+
+atributos disponíveis para as `requests` e as `responses` 
+
+- type
+- network_method
+- url
+- status_code
+- headers
+
+E especificamente para os tipos “response”
+
+- body
+
+---
+
+**Ao chamar a função, as vezes pode ter a necessidade de atualizar as requisições já passadas para verificar se a requisição específica que você deseja buscar, finalmente apareceu.**
+
+**Use**
+
+```python
+request = intercept_http(driver,only_request=True)
+#O resto da sua automação
+request.update()
+```
+
+Desta maneira, você poderá atualizar constantemente as requisições e atualizar a lista de requisições realizadas.
+
+---
+
+A função `intercept_http` possuí novos parâmetros, alguns desses não sendo necessários envio de nenhum dado, outros, sendo opcionais.
+
+Os adicionados foram:
+
+- update ❌ *Não envie nada neste parâmetro*
+- update_object ❌ *Não envie nada neste parâmetro*
+- static_resource → Enviar como False caso queira que a função valide e retorne requisições para arquivos estáticos como “css,svg,png,jpeg” entre outros.
+- only_request  → Enviar como True caso queira receber somente a lista de requisições para utilizar assim como ensinado aqui no 1.0.2, caso envie como False, que é o padrão, será buscado a rota enviada.
+
 
 ## Atualização 1.0.1
 
 Com a atualização da biblioteca agora é possível verificar se ao interagir com algum elemento em tela usando o selenium, se foi baixado um arquivo em um diretório específico.
 
 Siga o [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main/selenium_search_file) desta funcionalidade para entendê-la e aplicá-la.
 
@@ -140,8 +207,8 @@
                          'serviceIDHD': '23104',
                          'serviceIDOneSeg': '23128'},
                   _status_code=200,
                   _url='https://affiliates.video.globo.com/affiliates/info',
                   _method='GET')
 ```
 
----
+---
```

### Comparing `selenium-network-intercept-1.0.1/README.md` & `selenium_network_intercept-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,96 @@
+Metadata-Version: 2.1
+Name: selenium-network-intercept
+Version: 1.0.2
+Summary: Interceptador de requisições http não oficial do selenium 4
+Author: Alexandre Mariano
+Author-email: alexandre_mariano@hotmail.com.br
+License: MIT License
+Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept,search download selenium
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+## Atualização 1.0.2
+
+Trazendo novidades, agora é possível em vez de pesquisar diretamente pela rota desejada, você buscar todas requisições já realizadas pelo navegador, podendo ser verificado no [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main) utilizando o arquivo `example3.py`.
+
+**Agora tem a possibilida de além de somente fazer uma busca assim:**
+
+```powershell
+request = intercept_http(driver,'/route')
+```
+
+**É possível utilizar também desta forma:**
+
+```python
+request = intercept_http(driver,only_request=True)
+```
+
+Que trará um objeto que terá dois atributos importantes para esta funcionalidade 
+
+- requests
+- responses
+
+Estes atributos trarão a possibilidade de você mesmo validar todas as requisições que foram feitas desde o momento da abertura do navegador, sem preocupar com a implementação interna da biblioteca.
+
+***Mas lembre-se que ainda é possível buscar diretamente pela rota desejada***
+
+---
+
+**Use** 
+
+`request.requests`  Para ter acesso a todas requisições realizadas até o momento da chamada da função
+
+Para atualizar essa lista, utilize `request.update()`
+
+Itere sobre esta lista para fazer a própria varredura e verificar o que desejar por exemplo, buscar pela URL:
+
+```python
+for req in request.requests:
+    print(req.url)
+```
+
+atributos disponíveis para as `requests` e as `responses` 
+
+- type
+- network_method
+- url
+- status_code
+- headers
+
+E especificamente para os tipos “response”
+
+- body
+
+---
+
+**Ao chamar a função, as vezes pode ter a necessidade de atualizar as requisições já passadas para verificar se a requisição específica que você deseja buscar, finalmente apareceu.**
+
+**Use**
+
+```python
+request = intercept_http(driver,only_request=True)
+#O resto da sua automação
+request.update()
+```
+
+Desta maneira, você poderá atualizar constantemente as requisições e atualizar a lista de requisições realizadas.
+
+---
+
+A função `intercept_http` possuí novos parâmetros, alguns desses não sendo necessários envio de nenhum dado, outros, sendo opcionais.
+
+Os adicionados foram:
+
+- update ❌ *Não envie nada neste parâmetro*
+- update_object ❌ *Não envie nada neste parâmetro*
+- static_resource → Enviar como False caso queira que a função valide e retorne requisições para arquivos estáticos como “css,svg,png,jpeg” entre outros.
+- only_request  → Enviar como True caso queira receber somente a lista de requisições para utilizar assim como ensinado aqui no 1.0.2, caso envie como False, que é o padrão, será buscado a rota enviada.
+
+
 ## Atualização 1.0.1
 
 Com a atualização da biblioteca agora é possível verificar se ao interagir com algum elemento em tela usando o selenium, se foi baixado um arquivo em um diretório específico.
 
 Siga o [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main/selenium_search_file) desta funcionalidade para entendê-la e aplicá-la.
 
 
@@ -129,8 +218,8 @@
                          'serviceIDHD': '23104',
                          'serviceIDOneSeg': '23128'},
                   _status_code=200,
                   _url='https://affiliates.video.globo.com/affiliates/info',
                   _method='GET')
 ```
 
----
+---
```

### Comparing `selenium-network-intercept-1.0.1/selenium_network_intercept/intercept.py` & `selenium_network_intercept-1.0.2/selenium_network_intercept/intercept.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 import time
 import json
-from selenium_network_intercept.exceptions import CapabilityNotFound
-from selenium_network_intercept.response import network_response
-from selenium_network_intercept.request import network_request
+from selenium_network_intercept.exceptions.exceptions import CapabilityNotFound,ConflictingArgumentError,ArgumentNotRequestedError
+from selenium_network_intercept.request_types.response import network_response
+from selenium_network_intercept.request_types.request import network_request
 from time import sleep
-from selenium_network_intercept.objected import ObjectIntercepted
+from selenium_network_intercept.objects.objected import ObjectIntercepted
 
 
-def  _get_url(params,req_or_res): #falta teste unitario
+def is_valid_url(url, static_resource : bool):
+    is_valid = False
+    extension = (
+        '.html','.css','.jpg','.jpeg','.png','.woff','.woff2','.js','.ico','.gif','.svg','.php','.webp','.json','.dhtml',
+        '.ghtml','js','css2','.bin')
+    if not static_resource:
+        try:
+            if not(url.endswith(extension)):
+                is_valid = True
+        except:...
+        try:
+            if not(url.endswith(extension)):
+                is_valid = True
+        except:...
+    if static_resource:
+        is_valid = True
+    return is_valid
+
+
+def  _get_url(params,req_or_res):
     try:
         if req_or_res == 'response':
             url = _fix_url(params.get('response').get('url'))
         else:
             url = _fix_url(params.get('request').get('url'))
         return url
     except:...
@@ -50,79 +69,97 @@
 options = ChromeOptions()
 options.set_capability('goog:loggingPrefs', {'performance': 'ALL'})
 driver = webdriver.Chrome(options=options)"""
     )
 
 def intercept_http(
     driver,
-    route,
-    delay=5
+    part_of_route=None,
+    *,
+    only_request=False,
+    static_resource=False,
+    delay=5,
+    update=False,
+    update_object=None
     ) -> ObjectIntercepted:
-    
     """
     Obs:
     Recomendado não utilizar a busca pela rota no início da execução do driver, visto que para ser interceptado, é necessário que as rotas já tenham sido finalizadas.
     Intercepta solicitações HTTP feitas por um WebDriver Selenium.
     Pode ser colocado qualquer parte da URL / Rota desejada, contando que não seja parte de uma query.
 
     Args:
         driver: Uma instância de WebDriver Selenium.
-        url_endswith (str): O sufixo da URL para combinar com as solicitações interceptadas.
+        part_of_route (str): Uma parte da URL para ser possível identificar a URL desejada
+        only_request (default=False) : Envie True para retornar somente requisições, sem buscar especificamente por uma
+        static_resource (default=False): Mudar para True caso queira que retorne arquivos estáticos
+        delay: Tempo de espera para a captura dos logs
+        update: Uso interno do sistema, não envie este parâmetro
+        update_object: Uso interno do sistema, não envie este parâmetro
+        
 
     Nota:
         Esta função intercepta solicitações HTTP feitas pela instância fornecida de WebDriver. Ela busca
-        solicitações cujas URLs terminam com o sufixo especificado (`url_endswith`). Não sendo necessário enviar 
+        solicitações cujas URLs terminam com o sufixo especificado (`part_of_route`). Não sendo necessário enviar 
         informações como query na URL, somente a rota necessária.
         Para cada solicitação interceptada, ela recupera informações relevantes, como o corpo da solicitação, 
         código de status, URL e método HTTP, e as encapsula em uma instância de ObjectIntercepted.
+        
+        Caso envie static_resource False para não considerar arquivos estáticos, saiba que os arquivos serão os seguintes : ('.html','.css','.jpg','.jpeg','.png','.woff','.woff2','.js','.ico','.gif','.svg','.php','.webp','.json','.dhtml','.ghtml','js','css2','.bin') 
     """
+    if part_of_route and only_request:
+        raise ConflictingArgumentError('Não utilize os argumentos `part_of_route` e `only_request` juntos.')
+    
     verify_capabilities(driver)
     
     initial_time = time.time()
     logs1 = driver.get_log('performance') 
 
     sleep(delay)
-    
-    object_intercepted = ObjectIntercepted(route)
+    if not update:
+        object_intercepted = ObjectIntercepted(part_of_route,driver)
+    else:
+        object_intercepted = update_object
     logs2 = driver.get_log('performance')
     logs = logs1 + logs2
     
     
     for log in logs:
         message = json.loads(log.get('message')).get('message')
         params  = json.loads(log.get('message')).get('message').get('params')
         method  = json.loads(log.get('message')).get('message').get('method')
         response  = json.loads(log.get('message')).get('message').get('params').get('response')
         request  = json.loads(log.get('message')).get('message').get('params').get('request')
 
         response_url = _get_url(params,'response')
         request_url  = _get_url(params,'request')
         
-        if 'Network.responseReceived' == method:
+
+
+        if 'Network.responseReceived' == method and is_valid_url(response_url,static_resource):
             network_response(
                 driver,
                 params,
                 message,
-                route,
+                part_of_route,
                 response_url,
                 object_intercepted,
-                response
+                response,
+                only_requests=only_request
             )
         
         
-        if 'Network.requestWillBeSent' == method:
+        if 'Network.requestWillBeSent' == method and is_valid_url(request_url,static_resource):
             network_request(
                 params,
                 message,
-                route,
+                part_of_route,
                 request_url,
                 object_intercepted,
-                request
+                request,
+                only_request=only_request
             )
         
-        object_intercepted.set_list_of_responses(response_url)
-        object_intercepted.set_list_of_requests(request_url)
-        
     end_time = time.time()
     object_intercepted.time = end_time - initial_time
     
     return object_intercepted
```

### Comparing `selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/PKG-INFO` & `selenium_network_intercept-1.0.2/selenium_network_intercept.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,96 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
 Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept,search download selenium
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
+## Atualização 1.0.2
+
+Trazendo novidades, agora é possível em vez de pesquisar diretamente pela rota desejada, você buscar todas requisições já realizadas pelo navegador, podendo ser verificado no [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main) utilizando o arquivo `example3.py`.
+
+**Agora tem a possibilida de além de somente fazer uma busca assim:**
+
+```powershell
+request = intercept_http(driver,'/route')
+```
+
+**É possível utilizar também desta forma:**
+
+```python
+request = intercept_http(driver,only_request=True)
+```
+
+Que trará um objeto que terá dois atributos importantes para esta funcionalidade 
+
+- requests
+- responses
+
+Estes atributos trarão a possibilidade de você mesmo validar todas as requisições que foram feitas desde o momento da abertura do navegador, sem preocupar com a implementação interna da biblioteca.
+
+***Mas lembre-se que ainda é possível buscar diretamente pela rota desejada***
+
+---
+
+**Use** 
+
+`request.requests`  Para ter acesso a todas requisições realizadas até o momento da chamada da função
+
+Para atualizar essa lista, utilize `request.update()`
+
+Itere sobre esta lista para fazer a própria varredura e verificar o que desejar por exemplo, buscar pela URL:
+
+```python
+for req in request.requests:
+    print(req.url)
+```
+
+atributos disponíveis para as `requests` e as `responses` 
+
+- type
+- network_method
+- url
+- status_code
+- headers
+
+E especificamente para os tipos “response”
+
+- body
+
+---
+
+**Ao chamar a função, as vezes pode ter a necessidade de atualizar as requisições já passadas para verificar se a requisição específica que você deseja buscar, finalmente apareceu.**
+
+**Use**
+
+```python
+request = intercept_http(driver,only_request=True)
+#O resto da sua automação
+request.update()
+```
+
+Desta maneira, você poderá atualizar constantemente as requisições e atualizar a lista de requisições realizadas.
+
+---
+
+A função `intercept_http` possuí novos parâmetros, alguns desses não sendo necessários envio de nenhum dado, outros, sendo opcionais.
+
+Os adicionados foram:
+
+- update ❌ *Não envie nada neste parâmetro*
+- update_object ❌ *Não envie nada neste parâmetro*
+- static_resource → Enviar como False caso queira que a função valide e retorne requisições para arquivos estáticos como “css,svg,png,jpeg” entre outros.
+- only_request  → Enviar como True caso queira receber somente a lista de requisições para utilizar assim como ensinado aqui no 1.0.2, caso envie como False, que é o padrão, será buscado a rota enviada.
+
+
 ## Atualização 1.0.1
 
 Com a atualização da biblioteca agora é possível verificar se ao interagir com algum elemento em tela usando o selenium, se foi baixado um arquivo em um diretório específico.
 
 Siga o [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main/selenium_search_file) desta funcionalidade para entendê-la e aplicá-la.
```

### Comparing `selenium-network-intercept-1.0.1/selenium_search_file/search_file.py` & `selenium_network_intercept-1.0.2/selenium_search_file/search_file.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.1/setup.py` & `selenium_network_intercept-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 file = open('README.md', 'r',encoding='utf-8')
 readme = file.read()
 
 
 setup(
     name='selenium-network-intercept',
-    version='1.0.1',
+    version='1.0.2',
     license='MIT License',
     author='Alexandre Mariano',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='alexandre_mariano@hotmail.com.br',
     keywords=['selenium', 'network', 'intercept','http','requests','selenium network intercept','selenium intercept','search download selenium'],
     description='Interceptador de requisições http não oficial do selenium 4',
```

