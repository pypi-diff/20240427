# Comparing `tmp/ALLMDEV-1.2.4-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 9781 bytes, number of entries: 12
+Zip file size: 13619 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
+-rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/agent_rag.py
+-rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agent_ragrun.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
+-rw-rw-rw-  2.0 fat     1945 b- defN 24-Apr-26 04:23 ALLMDEV/fasty.py
 -rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-20 10:27 ALLMDEV/generate.py
 -rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     1985 b- defN 24-Apr-25 11:09 ALLMDEV/rag.py
 -rw-rw-rw-  2.0 fat     3016 b- defN 24-Apr-25 07:21 ALLMDEV/ragrun.py
--rw-rw-rw-  2.0 fat     3144 b- defN 24-Apr-25 07:25 ALLMDEV/ragserve.py
--rw-rw-rw-  2.0 fat     3227 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      192 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      911 b- defN 24-Apr-25 12:35 ALLMDEV-1.2.4.dist-info/RECORD
-12 files, 26284 bytes uncompressed, 8269 bytes compressed:  68.5%
+-rw-rw-rw-  2.0 fat     3425 b- defN 24-Apr-27 09:06 ALLMDEV/ragserve.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 24-Apr-27 09:32 ALLMDEV-1.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 09:32 ALLMDEV-1.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      201 b- defN 24-Apr-27 09:32 ALLMDEV-1.2.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-27 09:32 ALLMDEV-1.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1141 b- defN 24-Apr-27 09:32 ALLMDEV-1.2.5.dist-info/RECORD
+15 files, 35468 bytes uncompressed, 11761 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,13 +1,22 @@
 Filename: ALLMDEV/__init__.py
 Comment: 
 
+Filename: ALLMDEV/agent_rag.py
+Comment: 
+
+Filename: ALLMDEV/agent_ragrun.py
+Comment: 
+
 Filename: ALLMDEV/cli.py
 Comment: 
 
+Filename: ALLMDEV/fasty.py
+Comment: 
+
 Filename: ALLMDEV/generate.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
 Filename: ALLMDEV/rag.py
@@ -15,23 +24,23 @@
 
 Filename: ALLMDEV/ragrun.py
 Comment: 
 
 Filename: ALLMDEV/ragserve.py
 Comment: 
 
-Filename: ALLMDEV-1.2.4.dist-info/METADATA
+Filename: ALLMDEV-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.2.4.dist-info/WHEEL
+Filename: ALLMDEV-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.2.4.dist-info/entry_points.txt
+Filename: ALLMDEV-1.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.4.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.4.dist-info/RECORD
+Filename: ALLMDEV-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/ragserve.py

```diff
@@ -1,19 +1,17 @@
 from flask import Flask, request, jsonify
 from llama_index.llms.llama_cpp import LlamaCPP
 from .instruct import load_model
 import os
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
+import argparse
 
 
-persist_directory = 'db'
-embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
 
-db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
 
 app = Flask(__name__)
 
 # Check if apiconfig.txt exists in the model folder
 config_file_path = os.path.join('model', 'apiconfig.txt')
 if not os.path.exists(config_file_path):
     # Create apiconfig.txt with default values
@@ -57,15 +55,20 @@
     max_new_tokens=512,
     context_window=3900,
     model_kwargs={"n_gpu_layers": 0},
     verbose=False,
 )
 
 @app.route('/v1/chat/completions', methods=['POST'])
-def chat():
+def chat(persist_directory):
+
+    
+    embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
+
+    db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
     user_input = request.json.get("input")
 
     if user_input.lower() == "exit":
         return jsonify({"response": "Exiting chat."})
 
     prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query:<s>[INST] {prompt} [/INST]"
     docs = db.similarity_search(user_input,k=1)
@@ -74,14 +77,19 @@
 
     response_iter = llm.stream_complete(prompt)
     response_text = ''.join(response.delta for response in response_iter)
 
     return jsonify({"response": response_text})
 
 def main():
+        parser = argparse.ArgumentParser()
+        parser.add_argument("--agent", type=str, help="Name of the agent to query.")
+        args = parser.parse_args()
+        agentname=args.agent
+        persist_directory = os.path.join('db', agentname)
         print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
         if cert_file is not "" and cert_key is not "":
             app.run(host=host, port=port, debug=False, ssl_context=[cert_file,cert_key])
         else:
             app.run(host=host, port=port, debug=False)
 
 if __name__ == "__main__":
```

## Comparing `ALLMDEV-1.2.4.dist-info/METADATA` & `ALLMDEV-1.2.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.2.4
+Version: 1.2.5
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -55,34 +55,40 @@
 ```bash
 allm-serve
 ```
 
 ==========================================================================================================================================
 
 
-## ALLM RAG 
+## ALLM AGENTS 
 
-## Local RAG Inference
+## Local Agent Inference
 
-To initiate local RAG inference, begin by ingesting your documents into the vector database using the allm-createagent command:
+To create local agent, begin by loading your knowledge documents into the database using the allm-newagent command and specifying the agent name:
 
 ```bash
-allm-createagent --doc "document_path"
+allm-newagent --doc "document_path" --agent agent_name
 ```
 
-After successfully ingesting the document, you can start the local RAG inference with the allm-agentchat command:
+or
+
+```bash
+allm-newagent --dir "directory containing files to be ingested" --agent agent_name
+```
+
+After agent is created successfully with your knowledge document, you can start the local agent chat with the allm-agentchat command:
 
 
 ```bash
-allm-agentchat --name 'model_name_or_path'
+allm-agentchat --agent agent name
 ```
 
+After your agents are created you can also initiate agent-specific API server using the allm-agentapi command:
 
-Alternatively, you can also initiate RAG inference on the API server using the allm-agentapi command:
 
 ```bash
-allm-agentapi 
+allm-agentapi --agent agent name
 ```
 
 ## Supported Model names
 Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
```

