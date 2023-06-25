# Comparing `tmp/bohrium-sdk-0.2.2.tar.gz` & `tmp/bohrium-sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.2.2.tar", last modified: Tue Jun 13 03:50:37 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.2.3.tar", last modified: Sun Jun 25 03:32:34 2023, max compression
```

## Comparing `bohrium-sdk-0.2.2.tar` & `bohrium-sdk-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.492877 bohrium-sdk-0.2.2/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 03:50:37.491337 bohrium-sdk-0.2.2/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.2/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.473142 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.486495 bohrium-sdk-0.2.2/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.2/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.2/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6887 2023-06-13 03:47:27.000000 bohrium-sdk-0.2.2/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.2/bohriumsdk/database.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.2/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4119 2023-06-12 09:25:17.000000 bohrium-sdk-0.2.2/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.2/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.2/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     7809 2023-06-13 01:39:50.000000 bohrium-sdk-0.2.2/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.490027 bohrium-sdk-0.2.2/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.2/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.2/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4467 2023-06-13 01:43:50.000000 bohrium-sdk-0.2.2/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.2/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-13 03:50:37.492981 bohrium-sdk-0.2.2/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-13 03:48:26.000000 bohrium-sdk-0.2.2/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.274164 bohrium-sdk-0.2.3/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-25 03:32:34.273884 bohrium-sdk-0.2.3/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.3/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.261433 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-25 03:32:34.000000 bohrium-sdk-0.2.3/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.272144 bohrium-sdk-0.2.3/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.3/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.3/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     7164 2023-06-15 01:18:06.000000 bohrium-sdk-0.2.3/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.3/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.3/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-14 13:34:07.000000 bohrium-sdk-0.2.3/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.3/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.3/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     8511 2023-06-15 00:55:51.000000 bohrium-sdk-0.2.3/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-25 03:32:34.273276 bohrium-sdk-0.2.3/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.3/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.3/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-06-25 03:27:49.000000 bohrium-sdk-0.2.3/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.3/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-25 03:32:34.274288 bohrium-sdk-0.2.3/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-25 03:31:44.000000 bohrium-sdk-0.2.3/setup.py
```

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/client.py` & `bohrium-sdk-0.2.3/bohriumsdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,19 +44,24 @@
                 self.config['password'] = password
                 self.base_url = base_url_v1
             if token is not None:
                 self.token = token
             else:
                 self._login()
         elif api_version == "v2":
+            self.env = os.getenv("ENV", "prod")
+
             self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
             if not os.path.exists(self.config_file_location_expand):
                 print("Config File ~/.brmconfig not found! Please visit https://bohrium.dp.tech/personal/setting and click AccessKey create button to generate it !")
                 self.access_key = input("Please enter AccessKey: ")
-                data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
+                if self.env == "test":
+                    data = f"[Credentials]\nbaseUrl=https://openapi.test.dp.tech\naccessKey={self.access_key}"
+                else:
+                    data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
                 with open(self.config_file_location_expand, 'w') as f:
                     f.write(data)
             config = configparser.ConfigParser()
             config.read(self.config_file_location_expand)
             self.base_url = config.get('Credentials', 'baseUrl')
             self.access_key = config.get('Credentials', 'accessKey')
             self.params = {"accessKey": self.access_key}
@@ -98,15 +103,16 @@
                 sys.exit()
             if not resp.ok:
                 try:
                     result = resp.json()
                     err = result.get("error")
                 except:
                     pass
-                time.sleep(0.1 * i)
+                # time.sleep(0.1 * i)
+                time.sleep(20)
                 continue
             # print(resp.text)
             result = resp.json()
             if isinstance(result, str): return result
             if result.get('model', '') == 'gpt-35-turbo':
                 return result['choices'][0]['message']['content']
             elif result['code'] == 0:
@@ -120,15 +126,16 @@
     #     self.login()
     #     return self.token
 
     def check_ak(self):
         url = f"/openapi/v1/ak/get"
         resp = self.get(url=url, params=self.params)
         if resp.get("user_id", 0) != 0:
-            print("AccessKey authorization passed! ")
+            pass
+            # print("AccessKey authorization passed! ")
         return resp
 
     # def login(self):
     #     email = input("Please enter Bohrium Account Email: ")
     #     password = getpass.getpass(prompt="Please enter password: ")
     #     post_data = {
     #         'username': email,
```

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/database.py` & `bohrium-sdk-0.2.3/bohriumsdk/database.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/image.py` & `bohrium-sdk-0.2.3/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/job.py` & `bohrium-sdk-0.2.3/bohriumsdk/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,28 @@
         return data
     
     def log(self, job_id):
         data = self.client.get(f'/openapi/v1/job/{job_id}/log', params=self.client.params)
         return data
 
     def insert(self, **kwargs):
-        must_fill = ['job_type', 'oss_path', 'project_id', 'scass_type', 'command', 'platform', 'image_address', 'job_id']
+        must_fill = ['job_type', 'oss_path', 'project_id', 'scass_type', 'cmd', 'platform', 'image_address', 'job_id']
         # must_fill = ['job_type', 'oss_path', 'project_id', 'scass_type', 'command', 'platform', 'image_name']
         for each in must_fill:
             if each not in kwargs:
                 raise ValueError(f'{each} is required when submitting job')
         camel_data = {humps.camelize(k): v for k, v in kwargs.items()}
         if not isinstance(camel_data['ossPath'], list):
             camel_data['ossPath'] = [camel_data['ossPath']]
         if 'logFile' in camel_data:
             camel_data['logFiles'] = camel_data['logFile']
         if 'logFiles' in camel_data and not isinstance(camel_data['logFiles'], list):
             camel_data['logFiles'] = [camel_data['logFiles']]
         #if self.client.debug:
-        print(camel_data)
+        # print(camel_data)
         data = self.client.post(f"/openapi/v2/job/add", json=camel_data, params=self.client.params)
         return data
 
 
     def detail(self, job_id):
         data = self.client.get(f'/openapi/v1/job/{job_id}', params=self.client.params)
         return data
@@ -84,15 +84,15 @@
     def create(self, project_id, name='', group_id=0):
         data = {
             'projectId': project_id
         }
         if name:
             data['name'] = name
         if group_id:
-            data['groupId'] = group_id
+            data['bohrGroupId'] = group_id
         try:
             data = self.client.post(f'/openapi/v1/job/create', json=data, params=self.client.params)
         except Exception as e:
             raise e
         return data
     
     def create_job_group(self, project_id, job_group_name):
```

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/node.py` & `bohrium-sdk-0.2.3/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/project.py` & `bohrium-sdk-0.2.3/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/storage.py` & `bohrium-sdk-0.2.3/bohriumsdk/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from bohriumsdk.client import Client
 from bohriumsdk.job import Job
 import requests
 import json
 import base64
 import os
 from tqdm import tqdm
+import time
 
 _DEFAULT_CHUNK_SIZE = 50 * 1024 * 1024
 _DEFAULT_ITERATE_MAX_OBJECTS = 50
 class Parameter(object):
     contentType: str
     contentEncoding: str
     contentLanguage: str
@@ -26,17 +27,20 @@
     def __init__(
             self,
             base_url: str = "https://openapi.dp.tech",
             client: Client = None,
         ) -> None:
         
         self.base_url = base_url
-        self.host = "https://tiefblue.test.dp.tech"
+        if client.env == "test":
+            self.host = "https://tiefblue.test.dp.tech"
+        else:
+            self.host = "https://tiefblue.dp.tech"
         self.client = client
-        pass
+
     
     def encode_base64(
             self, 
             parameter: dict = {}
         ) -> str:
         j = json.dumps(parameter)
         return base64.b64encode(j.encode()).decode()
@@ -53,15 +57,15 @@
         param = {
             "path": object_key,
             'option': parameter
         }
 
         if parameter:
             param["option"] = parameter.__dict__
-        print(param)
+        # print(param)
         headers = {}
         headers[self.TIEFBLUE_HEADER_KEY] = self.encode_base64(param)
         headers['Authorization'] = "Bearer " + token
 
         # req = self.client.post(f"/api/upload/binary", data=body)
         url = f"/api/upload/binary"
         
@@ -163,15 +167,15 @@
         parameter.contentDisposition = f'attachment; filename="{disposition}"'
         bar_format = "{l_bar}{bar}| {n:.02f}/{total:.02f} %  [{elapsed}<{remaining}, {rate_fmt}{postfix}]"
         with open(file_path, 'r') as f:
             pbar = tqdm(total=100, desc=f"Uploading {disposition}", smoothing=0.01, bar_format=bar_format,
                         disable=not progress_bar)
             f.seek(0)
             if size < _DEFAULT_CHUNK_SIZE * 2:
-                print(object_key)
+                # print(object_key)
                 self.write(object_key=object_key, token=token, data=f.buffer, parameter=parameter)
                 pbar.update(100)
                 pbar.close()
                 return
             chunks = split_size_by_part_size(size, chunk_size)
             initial_key = self.init_upload_by_part(object_key, parameter).get('initialKey')
             part_string = []
@@ -185,14 +189,32 @@
             pbar.close()
             return self.complete_upload_by_part(object_key, initial_key, part_string)
 
     def download_from_file(self):
 
         data = self.client.get()
 
+    def download_from_url(self, url, save_file):
+        ret = None
+        for retry_count in range(3):
+            try:
+                ret = requests.get(url, stream=True)
+            except Exception as e:
+                continue
+            if ret.ok:
+                break
+            else:
+                time.sleep(retry_count)
+                ret = None
+        if ret is not None:
+            ret.raise_for_status()
+            with open(save_file, "wb") as f:
+                for chunk in ret.iter_content(chunk_size=8192):
+                    f.write(chunk)
+            ret.close()
 
     def _dump_parameter(self, parameter):
         j = json.dumps(parameter)
         return base64.b64encode(j.encode()).decode()
     
     def decode_base64(self, encode_data):
         data = json.loads(base64.b64decode(encode_data).decode('utf-8'))
```

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/test.py` & `bohrium-sdk-0.2.3/bohriumsdk/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,25 @@
     # ak = c.generate_access_key("ak")
     # print(ak)
     j = Job(c)
     s = Storage(client = c)
     #data = j.detail()
     #print(j.log(10009242))
     data = j.create(project_id=154, name="test-env-job")
-    
+
     # print(data)
     file_path = "/Users/dingzhaohan/Downloads/out.zip"
     file_name = os.path.basename(file_path)
     token = data["token"]
     print(data)
     #print(j.list_by_page(job_group_id=2107148))
     jid = data["jobId"]
     # j.get_job_token(jid)
     object_key = os.path.join(data["storePath"], file_name)
+    print(object_key)
     res = s.upload_From_file_multi_part(object_key=object_key, file_path=file_path,  token=token, progress_bar=True)
     #res = s.upload_from_file(object_key=object_key, file_path=file_path, token=token)
     # s.download_from_file()
 
     #res = s.read(object_key=res["path"], token=token)
     #print(res)
 
@@ -52,21 +53,28 @@
         'input_file_method': 1,
         "job_type": "container",
         "job_name": "test-name",
         "project_id": 154,
         "scass_type": "c2_m4_cpu",
         "cmd": "echo 1asdfasdfasdfasdfasdfasdfasdf11 >> test.result;",
         "log_files": ["test.result"],
+        "out_files": ["test.result"],
         "platform": "ali",
         "image_address": "registry.dp.tech/dev/test/ubuntu:20.04-py3.10",
         "job_id": jid
     }
     j.insert(**data)
     #print(a["items"][0].keys())
 
+def test_job_detail():
+    c = Client()
+    j = Job(client=c)
+    data = j.detail(10059657)
+    print(data["status"])
+
 def test_node():
     c = Client()
     node = Node(c)
     node.print_node(154)
     # data = node.list_server(154)
     # print(data)
     # headers = data[0].keys()
@@ -101,15 +109,15 @@
     object_key = os.path.join(resp["storePath"], file_name)
 
     res = s.upload_From_file_multi_part(file_path=file_path, object_key=object_key, token=token)
     #res = s.upload_from_file(object_key=object_key, file_path=file_path, token=token)
     print(res)
     # filename = "a.txt"
     # object_key = os.path.join(resp["storePath"], filename)
-    # 
+    #
     # print(resp)
     # param = Parameter()
     # param.userMeta = {
     #         "a": "b",
     #         "ever":"17"
     #     }
     # param.contentType = "text/plain"
@@ -147,10 +155,10 @@
     prompt = "你好"
     res = c.chat(prompt)
     print(res)
 
 
 if __name__ == "__main__":
     test_chat()
-    # test_job()
+    # test_job_detail()
     # test_base64()
-    # test_db()
+    # test_db()
```

### Comparing `bohrium-sdk-0.2.2/bohriumsdk/util.py` & `bohrium-sdk-0.2.3/bohriumsdk/util.py`

 * *Files identical despite different names*

