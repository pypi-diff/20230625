# Comparing `tmp/sdqrcode-0.3.0.tar.gz` & `tmp/sdqrcode-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.0.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.1.tar", max compression
```

## Comparing `sdqrcode-0.3.0.tar` & `sdqrcode-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-06-25 09:10:51.988845 sdqrcode-0.3.0/LICENSE
--rw-r--r--   0        0        0     3778 2023-06-25 09:10:51.988845 sdqrcode-0.3.0/README.md
--rw-r--r--   0        0        0      474 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2410 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     1761 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      628 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      708 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0     8974 2023-06-25 09:10:52.012846 sdqrcode-0.3.0/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 sdqrcode-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-25 10:02:14.561147 sdqrcode-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5343 2023-06-25 10:02:14.561147 sdqrcode-0.3.1/README.md
+-rw-r--r--   0        0        0      474 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2410 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     1749 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      616 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      696 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0     8892 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0     6133 1970-01-01 00:00:00.000000 sdqrcode-0.3.1/PKG-INFO
```

### Comparing `sdqrcode-0.3.0/LICENSE` & `sdqrcode-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.0/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.1/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.0/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.1/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         self.controlnet_units = []
         for name, unit in self.config["controlnet_units"].items():
             cn_unit = ControlNetModel.from_pretrained(unit["model"])
             self.controlnet_units.append(cn_unit)
 
         self.pipeline = StableDiffusionControlNetPipeline.from_pretrained(
-            self.config["global"]["model_name_or_path_or_api_name"],
+            self.config["global"]["model_name_or_path"],
             controlnet=self.controlnet_units,
         ).to("cuda")
 
         # todo setup scheduler
 
     def generate_sd_qrcode(
         self,
```

### Comparing `sdqrcode-0.3.0/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.1/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.0/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.1/src/sdqrcode/configs/default_auto.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 global:
   prompt: "a beautiful minecraft landscape, lights and shadows"
-  model_name_or_path_or_api_name: "6ce0161689"
+  model_name_or_path: "6ce0161689"
   steps: 20
   sampler_name: Euler a
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
```

### Comparing `sdqrcode-0.3.0/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.1/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 global:
   prompt: "a beautiful minecraft landscape, lights and shadows"
-  model_name_or_path_or_api_name: "SG161222/Realistic_Vision_V2.0"
+  model_name_or_path: "SG161222/Realistic_Vision_V2.0"
   steps: 20
   # sampler_name: Euler a not implemented yet
   cfg_scale: 7
-  width: 512
-  height: 512
+  width: 768
+  height: 768
   seed: -1
 
 controlnet_units:
   brightness:
     model: ioclab/control_v1p_sd15_brightness
     #module: none not implemented yet
     weight: 0.35
```

### Comparing `sdqrcode-0.3.0/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.1/src/sdqrcode/sdqrcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     return config
 
 
 def update_config_dict(
     config: dict,
     prompt: str = None,
-    model_name_or_path_or_api_name: str = None,
+    model_name_or_path: str = None,
     steps: int = None,
     cfg_scale: float = None,
     width: int = None,
     height: int = None,
     seed: int = None,
     controlnet_model_names: list[str] = None,
     controlnet_weights: list[float] = None,
@@ -120,18 +120,16 @@
     qrcode_box_size: int = None,
     qrcode_border: int = None,
     qrcode_fill_color: str = None,
     qrcode_back_color: str = None,
 ):
     if prompt is not None:
         config["global"]["prompt"] = prompt
-    if model_name_or_path_or_api_name is not None:
-        config["global"][
-            "model_name_or_path_or_api_name"
-        ] = model_name_or_path_or_api_name
+    if model_name_or_path is not None:
+        config["global"]["model_name_or_path"] = model_name_or_path
     if steps is not None:
         config["global"]["steps"] = steps
     if cfg_scale is not None:
         config["global"]["cfg_scale"] = cfg_scale
     if width is not None:
         config["global"]["width"] = width
     if height is not None:
@@ -171,15 +169,15 @@
     auto_api_https: bool = None,
     auto_api_username: str = None,
     auto_api_password: str = None,
     **config_kwargs,
 ):
     """
     config_kwargs:
-        model_name_or_path_or_api_name: str = None,
+        model_name_or_path: str = None,
         steps: int = None,
         cfg_scale: float = None,
         width: int = None,
         height: int = None,
         seed: int = None,
         prompt: str = None,
         controlnet_model_names: list[str] = None,
```

