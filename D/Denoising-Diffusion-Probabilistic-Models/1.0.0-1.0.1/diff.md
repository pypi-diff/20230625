# Comparing `tmp/Denoising_Diffusion_Probabilistic_Models-1.0.0-py3-none-any.whl.zip` & `tmp/Denoising_Diffusion_Probabilistic_Models-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9618 bytes, number of entries: 11
--rw-r--r--  2.0 unx     6761 b- defN 23-Jun-23 13:23 diffusion/DDMFunctions.py
--rw-r--r--  2.0 unx    10005 b- defN 23-Jun-23 13:23 diffusion/Network.py
--rw-r--r--  2.0 unx     1192 b- defN 23-Jun-23 13:23 diffusion/Scheduler.py
--rw-r--r--  2.0 unx      134 b- defN 23-Jun-23 13:23 diffusion/Test.py
--rw-r--r--  2.0 unx     3457 b- defN 23-Jun-23 13:23 diffusion/Train.py
--rw-r--r--  2.0 unx      189 b- defN 23-Jun-23 13:23 diffusion/__init__.py
--rw-r--r--  2.0 unx      355 b- defN 23-Jun-23 13:23 diffusion/diffusion_process.py
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-23 13:23 Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 13:23 Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-23 13:23 Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jun-23 13:23 Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/RECORD
-11 files, 23604 bytes uncompressed, 7934 bytes compressed:  66.4%
+Zip file size: 9647 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     6979 b- defN 23-Jun-25 11:47 diffusion/DDMFunctions.py
+-rw-r--r--  2.0 unx    10005 b- defN 23-Jun-25 11:47 diffusion/Network.py
+-rw-r--r--  2.0 unx     1192 b- defN 23-Jun-25 11:47 diffusion/Scheduler.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-25 11:47 diffusion/Test.py
+-rw-r--r--  2.0 unx     3457 b- defN 23-Jun-25 11:47 diffusion/Train.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-25 11:47 diffusion/__init__.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Jun-25 11:47 diffusion/diffusion_process.py
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jun-25 11:47 Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD
+11 files, 23822 bytes uncompressed, 7963 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: diffusion/__init__.py
 Comment: 
 
 Filename: diffusion/diffusion_process.py
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/METADATA
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/WHEEL
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/top_level.txt
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/RECORD
+Filename: Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## diffusion/DDMFunctions.py

```diff
@@ -20,14 +20,20 @@
             # デフォルトは線形スケジュール
             # self.betas = torch.linspace(0.0001, 0.02, timesteps)
             self.betas = scheduler.linear_beta_schedule()
             
         elif schedule_type == 'cosine':
             self.betas = scheduler.cosine_beta_schedule()
             
+        elif schedule_type == 'quadratic':
+            self.betas = scheduler.quadratic_beta_schedule()
+
+        elif schedule_type == 'sigmoid':
+            self.betas = scheduler.sigmoid_beta_schedule()
+            
         else:
             pass
         
         self.timesteps = timesteps #300 # 1000
 
         # alphasの定義
         self.alphas = 1. - self.betas
```

## Comparing `Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/RECORD` & `Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-diffusion/DDMFunctions.py,sha256=Zql1JXvLpv60Li3_anXZVJuYw2uOrgc50huYhr7MzeQ,6761
+diffusion/DDMFunctions.py,sha256=KBh012fZb7RmvP45K0Oh33VDagNOWbhDhSZ4Zv5QLGk,6979
 diffusion/Network.py,sha256=DBIyc-o6Q0ScwT6ITI6MNauX3As0vl-hhK2MIPVkEfU,10005
 diffusion/Scheduler.py,sha256=d9TpBH7yrX8QPqNnEhJ04ULLTNGQMdPOg28HWyqtRug,1192
 diffusion/Test.py,sha256=7TsJJE83SWWspqaav9ZmbgYbkXjMleVJyehPdoBkqRk,134
 diffusion/Train.py,sha256=pr7OKXCSX1hk_vIIHmnspl_4az9_b4-cIkS04ut_06k,3457
 diffusion/__init__.py,sha256=HhslOaOBONU0AL5pSzfZesj7SfohsvKoEmoHoKehicQ,189
 diffusion/diffusion_process.py,sha256=XciyhvrGX1an4p0QywgOq3Q3HjAXcKGYVJS7YodIcrw,355
-Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/METADATA,sha256=o5NO4aEAr7cbr5nmFNr5jYwMu9m6RkULzyE8ocNUTos,430
-Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
-Denoising_Diffusion_Probabilistic_Models-1.0.0.dist-info/RECORD,,
+Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/METADATA,sha256=rvNjTCy27_iKp0941Io-MrphDjwH_XF6U287DbTxZ0M,430
+Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
+Denoising_Diffusion_Probabilistic_Models-1.0.1.dist-info/RECORD,,
```

