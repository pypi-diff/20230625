# Comparing `tmp/pointstorm-1.1.7.tar.gz` & `tmp/pointstorm-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.7.tar", last modified: Fri Jun  2 21:23:16 2023, max compression
+gzip compressed data, was "pointstorm-1.1.8.tar", last modified: Sun Jun 25 19:55:44 2023, max compression
```

## Comparing `pointstorm-1.1.7.tar` & `pointstorm-1.1.8.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.728742 pointstorm-1.1.7/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.7/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:23:16.728578 pointstorm-1.1.7/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.7/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.726433 pointstorm-1.1.7/pointstorm/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.7/pointstorm/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.7/pointstorm/config.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727236 pointstorm-1.1.7/pointstorm/destinations/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.7/pointstorm/destinations/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727785 pointstorm-1.1.7/pointstorm/embedding/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.7/pointstorm/embedding/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.7/pointstorm/embedding/abstract.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.7/pointstorm/embedding/image.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.7/pointstorm/embedding/text.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.7/pointstorm/embedding/time.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727902 pointstorm-1.1.7/pointstorm/ingestion/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.7/pointstorm/ingestion/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.728129 pointstorm-1.1.7/pointstorm/ingestion/cdc/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.7/pointstorm/ingestion/cdc/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.7/pointstorm/ingestion/cdc/debezium.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.728359 pointstorm-1.1.7/pointstorm/ingestion/event/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.7/pointstorm/ingestion/event/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     3732 2023-06-02 19:44:33.000000 pointstorm-1.1.7/pointstorm/ingestion/event/kafka.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.7/pointstorm/monitoring.py
--rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.7/pointstorm/reference_db.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-02 21:23:16.727090 pointstorm-1.1.7/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-02 21:23:16.000000 pointstorm-1.1.7/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.7/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-02 21:23:16.728785 pointstorm-1.1.7/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)     1010 2023-06-02 21:21:33.000000 pointstorm-1.1.7/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.886303 pointstorm-1.1.8/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.8/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-25 19:55:44.886087 pointstorm-1.1.8/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.8/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.882766 pointstorm-1.1.8/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.8/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.8/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.883790 pointstorm-1.1.8/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.8/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884120 pointstorm-1.1.8/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.8/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     1213 2023-06-25 19:54:11.000000 pointstorm-1.1.8/pointstorm/embedding/text.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884298 pointstorm-1.1.8/pointstorm/examples/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:56:08.000000 pointstorm-1.1.8/pointstorm/examples/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884752 pointstorm-1.1.8/pointstorm/examples/kafka/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:56:17.000000 pointstorm-1.1.8/pointstorm/examples/kafka/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      560 2023-06-20 02:30:06.000000 pointstorm-1.1.8/pointstorm/examples/kafka/kafka_producer.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      547 2023-06-20 02:22:00.000000 pointstorm-1.1.8/pointstorm/examples/kafka/run_kafka.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884947 pointstorm-1.1.8/pointstorm/ingestion/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.8/pointstorm/ingestion/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885212 pointstorm-1.1.8/pointstorm/ingestion/cdc/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.8/pointstorm/ingestion/cdc/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.8/pointstorm/ingestion/cdc/debezium.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885454 pointstorm-1.1.8/pointstorm/ingestion/event/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.8/pointstorm/ingestion/event/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     3776 2023-06-25 19:41:33.000000 pointstorm-1.1.8/pointstorm/ingestion/event/kafka.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885632 pointstorm-1.1.8/pointstorm/inputs/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-16 06:13:48.000000 pointstorm-1.1.8/pointstorm/inputs/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.8/pointstorm/monitoring.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885881 pointstorm-1.1.8/pointstorm/producers/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:44:46.000000 pointstorm-1.1.8/pointstorm/producers/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     1014 2023-06-20 02:17:13.000000 pointstorm-1.1.8/pointstorm/producers/text_producer.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.883552 pointstorm-1.1.8/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      813 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)      116 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.8/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-25 19:55:44.886348 pointstorm-1.1.8/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1054 2023-06-25 19:54:29.000000 pointstorm-1.1.8/setup.py
```

### Comparing `pointstorm-1.1.7/LICENSE` & `pointstorm-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.7/PKG-INFO` & `pointstorm-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.7
+Version: 1.1.8
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.7/README.md` & `pointstorm-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.7/pointstorm/ingestion/event/kafka.py` & `pointstorm-1.1.8/pointstorm/ingestion/event/kafka.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 # ML imports
 from transformers import AutoTokenizer, AutoModel
 import torch
 
 # Local imports
 from pointstorm.config import abstract_logger as kafka_logger
+from pointstorm.embedding.text import Document, embedding
 
 class KafkaIngestionException(Exception):
     pass
 
 class KafkaTextEmbeddings():
-    def __init__(self, kafka_topic, kafka_bootstrap_server, kafka_group_id, text_field, huggingface_model_name):
+    def __init__(self, kafka_topic, kafka_bootstrap_server, kafka_config, huggingface_model_name):
         self.kafka_topic = kafka_topic
         self.kafka_bootstrap_server = kafka_bootstrap_server
-        self.kafka_group_id = kafka_group_id
-        self.text_field = text_field
+        self.kafka_config = kafka_config
         self.model_name = huggingface_model_name
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         self.model = AutoModel.from_pretrained(self.model_name)
         # self.previous_messages = self.get_previous_messages()
 
     #     def set_topic(self, kafka_topic):
     #         self.kafka_topic = kafka_topic
@@ -62,41 +62,46 @@
 
     #             if not topic_partitions:
     #                 consumer.close()
     #                 break
         
     #     return previous_messages
 
-    def vectorize(self, message):
+    def set_output(self, output):
+        # TODO: Add output
+        self.output = output
+
+    def embedding(self, message):
         """
-        Vectorize the message using the trained model
+        Generating embedding using text embedding class
         """
 
-        if self.text_field in json.loads(message[1]):
-            message = str(json.loads(message[1])[self.text_field])
+        if "raw_text" in json.loads(message[1]):
+            message = str(json.loads(message[1])["raw_text"])
         else:
             raise KafkaIngestionException("Message does not contain the specified text field: " + self.text_field)
+        
+        # doc = Document(
+        #     id=
+        #     text=message,
+        #     )
         inputs = self.tokenizer(message, return_tensors="pt", padding=True, truncation=True)
 
         with torch.no_grad():
             outputs = self.model(**inputs)
 
         embeddings = outputs.last_hidden_state.mean(dim=1).numpy()
         kafka_logger.info(f"Generated embeddings for message: {message}, {embeddings}")
     
     def run(self):
         input_config = KafkaInput(
             brokers=[self.kafka_bootstrap_server],
             topics=[self.kafka_topic],
-            add_config={
-                'group.id': self.kafka_group_id,
-                'auto.offset.reset': 'earliest',
-                'enable.auto.commit': True
-            }
+            add_config=self.kafka_config
         )
 
         kafka_logger.info("Started KafkaTextEmbeddings for topic: " + self.kafka_topic)
         flow = Dataflow()
         flow.input(self.kafka_topic, input_config)
-        flow.map(self.vectorize)
+        flow.map(self.embedding)
         flow.output("stdout", StdOutput())
         run_main(flow)
```

### Comparing `pointstorm-1.1.7/pointstorm.egg-info/PKG-INFO` & `pointstorm-1.1.8/pointstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.7
+Version: 1.1.8
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.7/pointstorm.egg-info/SOURCES.txt` & `pointstorm-1.1.8/pointstorm.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pointstorm/__init__.py
 pointstorm/config.py
 pointstorm/monitoring.py
-pointstorm/reference_db.py
 pointstorm.egg-info/PKG-INFO
 pointstorm.egg-info/SOURCES.txt
 pointstorm.egg-info/dependency_links.txt
 pointstorm.egg-info/requires.txt
 pointstorm.egg-info/top_level.txt
 pointstorm/destinations/__init__.py
 pointstorm/embedding/__init__.py
-pointstorm/embedding/abstract.py
-pointstorm/embedding/image.py
 pointstorm/embedding/text.py
-pointstorm/embedding/time.py
+pointstorm/examples/__init__.py
+pointstorm/examples/kafka/__init__.py
+pointstorm/examples/kafka/kafka_producer.py
+pointstorm/examples/kafka/run_kafka.py
 pointstorm/ingestion/__init__.py
 pointstorm/ingestion/cdc/__init__.py
 pointstorm/ingestion/cdc/debezium.py
 pointstorm/ingestion/event/__init__.py
-pointstorm/ingestion/event/kafka.py
+pointstorm/ingestion/event/kafka.py
+pointstorm/inputs/__init__.py
+pointstorm/producers/__init__.py
+pointstorm/producers/text_producer.py
```

### Comparing `pointstorm-1.1.7/setup.py` & `pointstorm-1.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     install_requires=[
         'bytewax==0.16.0',
         'requests>=2.28.0',
         'kafka-python==2.0.2',
         'confluent-kafka',
         'faker',
         'transformers',
-        'torch'
+        'torch',
+        'pydantic',
+        'unstructured'
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

