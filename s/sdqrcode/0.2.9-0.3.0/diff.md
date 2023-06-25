# Comparing `tmp/sdqrcode-0.2.9.tar.gz` & `tmp/sdqrcode-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.2.9.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.0.tar", max compression
```

## Comparing `sdqrcode-0.2.9.tar` & `sdqrcode-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-06-24 20:59:52.797309 sdqrcode-0.2.9/LICENSE
--rw-r--r--   0        0        0     3778 2023-06-24 20:59:52.797309 sdqrcode-0.2.9/README.md
--rw-r--r--   0        0        0      474 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     2410 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     1867 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      628 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      713 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0     8930 2023-06-24 20:59:52.821309 sdqrcode-0.2.9/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 sdqrcode-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-25 09:10:51.988845 sdqrcode-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3778 2023-06-25 09:10:51.988845 sdqrcode-0.3.0/README.md
+-rw-r--r--   0        0        0      474 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2410 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     1761 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      628 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      708 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0     8974 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 sdqrcode-0.3.0/PKG-INFO
```

### Comparing `sdqrcode-0.2.9/LICENSE` & `sdqrcode-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.9/README.md` & `sdqrcode-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.9/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.0/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.9/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.0/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,11 +47,8 @@
             height=self.config["global"]["height"],
             num_inference_steps=self.config["global"]["steps"],
             image=[qr_code_img for _ in range(len(controlnet_weights))],
             controlnet_guidance=controlnet_startstops,
             controlnet_conditioning_scale=controlnet_weights,
         )
 
-        if return_cn_imgs:
-            return r.images
-        else:
-            return r.images[0 : -len(self.controlnet_units)]
+        return r.images
```

### Comparing `sdqrcode-0.2.9/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.0/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.9/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.0/src/sdqrcode/configs/default_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.2.9/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.0/src/sdqrcode/sdqrcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,17 @@
             username=auto_api_username,
             password=auto_api_password,
             config=self.config,
         )
 
     def generate_sd_qrcode(
         self,
+        return_cn_imgs: bool = False,
         **config_kwargs,
-    ) -> PIL.Image.Image:
+    ) -> list[PIL.Image.Image]:
         self.config = update_config_dict(
             config=self.config,
             **config_kwargs,
         )
 
         error_name_to_enum = {
             "low": qrcode.constants.ERROR_CORRECT_L,
```

### Comparing `sdqrcode-0.2.9/PKG-INFO` & `sdqrcode-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.2.9
+Version: 0.3.0
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

