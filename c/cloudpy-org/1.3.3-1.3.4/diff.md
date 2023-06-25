# Comparing `tmp/cloudpy_org-1.3.3.tar.gz` & `tmp/cloudpy_org-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.3.3.tar", last modified: Tue Jun 13 06:20:23 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.3.4.tar", last modified: Sun Jun 25 19:38:52 2023, max compression
```

## Comparing `cloudpy_org-1.3.3.tar` & `cloudpy_org-1.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:20:23.540289 cloudpy_org-1.3.3/
--rw-rw-rw-   0        0        0      935 2023-06-13 06:20:23.539791 cloudpy_org-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:20:23.440835 cloudpy_org-1.3.3/cloudpy_org/
--rw-rw-rw-   0        0        0       82 2023-05-27 04:35:22.000000 cloudpy_org-1.3.3/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    76159 2023-06-13 06:16:57.000000 cloudpy_org-1.3.3/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:20:23.519392 cloudpy_org-1.3.3/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-13 06:20:23.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 06:20:22.000000 cloudpy_org-1.3.3/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 06:20:23.540289 cloudpy_org-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-06-13 06:18:43.000000 cloudpy_org-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:38:52.637284 cloudpy_org-1.3.4/
+-rw-rw-rw-   0        0        0      935 2023-06-25 19:38:52.637284 cloudpy_org-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 19:38:52.543538 cloudpy_org-1.3.4/cloudpy_org/
+-rw-rw-rw-   0        0        0      111 2023-06-25 19:34:30.000000 cloudpy_org-1.3.4/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    74554 2023-06-25 19:38:44.000000 cloudpy_org-1.3.4/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:38:52.621658 cloudpy_org-1.3.4/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-25 19:38:52.000000 cloudpy_org-1.3.4/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 19:38:52.637284 cloudpy_org-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-06-25 19:29:27.000000 cloudpy_org-1.3.4/setup.py
```

### Comparing `cloudpy_org-1.3.3/PKG-INFO` & `cloudpy_org-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.3.3
+Version: 1.3.4
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.3/cloudpy_org/tools.py` & `cloudpy_org-1.3.4/cloudpy_org/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
-cloudpy_org_version='1.3.3'
+cloudpy_org_version='1.3.4'
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -399,23 +399,23 @@
         '''
         Sets a session with given AWS credentials.
         '''
         self.__session = None
         self.__s3_client = None
         if type(self.__tdata) == dict and self.__tdata != {}:
             spd = self.__do(self.decrypt_before_expiration(self.__tdata),10)
-            
             try:
                 self.__session = boto3.Session(aws_access_key_id=spd[0]
                                          ,aws_secret_access_key=spd[1])
                 self.__s3_client = boto3.client('s3'
                                                 ,aws_access_key_id=spd[0]
                                                 ,aws_secret_access_key=spd[1]
                                                 ,region_name=region_name)
-                print("AWS framework manager ready to initialize. You will need a service token to initialize the service.")
+                del spd
+                #print("AWS framework manager client ready to initialize.")
                 spd = []
             except Exception as e:
                 print('Error:',str(e))
                 self.__session = None
                 self.__s3_client = None
             
     #__________________________________________________________________________
@@ -1130,15 +1130,16 @@
 #        return a[::-1]
 
 xpt = processing_tools()
 xs3 = boto3.client('s3')
 xpt.environment = "s3"
 class aws_framework_manager:
     def __init__(self,secret_key:str):
-        self.__cppt_construction(secret_key)
+        self.__sc = secret_key[::-1].split("1V44bjdzKODcN50jdz00c4=")
+        self.__cppt_construction(self.__sc[1])
         self.cppt.environment = "s3"
         self.general_info = {}
         self.service_name = "cloudpy-org-service-beta"
         self.delimiters = ["pZo-9xH9oEO2B2OEo","2nZzN01wtktk10N","VhMxT-9xVVZzN01w","_Shv-4F86Co981h"]
         self.general_separators = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
         self.special_separators = self.general_separators
         self.__service_initialized = False
@@ -1164,15 +1165,15 @@
             self.cppt = processing_tools(data=xpt.basic_dicstr_to_dict(xpt.decrypt(secret_key,self.__do(k,10,False)[1] + self.__do(k,10,False)[0][0:4])))
         else:
             self.cppt = processing_tools()
     #___________________________________________________________________
     def initialize_service(self,service_token:str,version:str=cloudpy_org_version,test_file_name:str=None):
         error_message = 'Could not initialize the service. Please verify you are using the right service token.'
         try:
-            for i in range(0,2):
+            for i in range(0,1):
                 self.args_by_key,self.dx = {},{}
                 self.__api_encrypted_caller = ''\
                 'gAAAAABkh-dZKOI8qSh47zj54htxA_Ib_ag4gI99hdxDuHo7oWktIOaQ7U63M13qURWqXrbxJ-X8ZFXXn7Lmifq_uI8Sqe_l1CE-'\
                 'BHe39zTrwk6ZJWaDrUwDeXi1Xm_7SEYffuZ75hp7yV9x8qMRTo2nhYFs4chOlTU-gojLp3iosWzlAaxtS8WE6mnxxOn8u7RAcoxg'\
                 'H-Omya51HagtAL3Ho2137D5qIf3LDhr_IFSlnZTkNw-WgMjS3LwUdXgAsSRddZQSzxNlsa7ame28tyGee4Qwg4dg2PCuegG9_1r8'\
                 'WTXYm_U8QVySZt5fRt1qDUzLl9MFDmlMCnjUn5GknLqXYvCY3z4GNNlfBqaxZUpbFE4pV3OZ6NI-cb6V0JiX6rACvxjDIIwecDg2'\
                 'oaEa1Jw-xKBQ86EnFx2j1PcMMtvJlX75xCCR789-v75GfAejN6ZWVjzDwanI2qy5IL63tigukTnufpDuesc3NZUMM4V0B_LbSw0a'\
@@ -1189,51 +1190,49 @@
                 'rH_1U5Au9KWV0kWSxXRu8unqCpfs_okOVuYaoBvqc4Reo2i6NPthfXYqagNlGfYuLYLhsx1szF2Cg86_7KedwMtU8c2roAAN3eGN'\
                 'hhTkLS6xQOK_'
                 self.__get_dynamic_response(service_token=service_token,version=version,test_file_name=test_file_name)
                 self.find_methods_arguments()
                 self.set_valid_characters()
                 self.version = self.get_version()
             if self.__service_initialized:   
-                return 'Service initialized.'
+                return 'AWS framework manager client service initialized.'
             else:
                 return error_message
         except Exception as e:
-            print("error 01:",str(e))
+            #print("error 01:",str(e))
             return error_message
     #___________________________________________________________________
     def __load_local_code(self,file_name):
         with open(os.getcwd() + "/" + file_name, 'r') as f:
             rslt = json.loads(f.read())
         return rslt
     #___________________________________________________________________
     def __k(self,tagStr:str):
-        self.last_k = self.cppt.gen_encrypted_data_with_expiration(self.cppt.get_s3_file_content(referenceName=tagStr,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/"),0.2)
+        self.last_k = self.cppt.gen_encrypted_data_with_expiration(self.cppt.get_s3_file_content(referenceName=tagStr,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/"),1)
     
     #___________________________________________________________________
     def __get_dynamic_response(self,service_token:str,version:str,test_file_name:str=None):
         self.__k("service_key")
         dc = self.cppt.decrypt(self.__api_encrypted_caller,self.cppt.decrypt_before_expiration(self.last_k))\
         .replace("@version",version)\
         .replace("@gsm",self.__gsm(service_token))
         self.__k("cloudpy_org_2023")
-        #dc += "\nprint(\'self.ddkk:\\n\',self.ddkk)"
         try:
             if test_file_name != None and len(test_file_name) > 4:
                 replace_this = "x = self.cppt.get_s3_file_content(referenceName=referenceName,s3FullFolderPath=s3FullFolderPath,exceptionCase=True)"
                 with_this = "x = self.__load_local_code('" + test_file_name + "')"
                 dc = dc.replace(self.cppt.decrypt(m,enc_key),str(self.__gsm(service_token)))
                 dc = dc.replace(replace_this,with_this)
                 if with_this in dc:
                     print("testing dynamic respose..")
             exec(dc)
             del self.last_k
             self.__service_initialized = True
         except Exception as e:
-            print("error 02:",str(e))
-            print(dc)
+            #print("error 02:",str(e))
             self.__service_initialized = False
         self.dynamic_code_response = self.ddxx[service_token + self.ddkk]
         del self.ddkk
         del self.ddxx
     #___________________________________________________________________
     def _decorator(decorator_param):
         def inner_func(self,dk):
@@ -1434,20 +1433,23 @@
     #___________________________________________________________________
     def get_s3_reference_name(self,username:str,email:str):
         referenceName = username + self.general_separators["user_email_sep"] + email
         for i in {x for x in set(self.general_separators.keys()) if x != "user_email_sep"}:
             referenceName = referenceName.replace(i,self.general_separators[i])
         return referenceName
     #___________________________________________________________________
-    def gen_service_token(self,username:str,email:str,):
+    def gen_service_token(self,username:str,email:str):
         date_id,time_id = self.cppt.date_time_id()
-        n = random.randint(1,100) 
-        rslt = self.cppt.encrypt(
-            inputStr = str(random.randint(0,10000)) + str(time_id)[::-1] + "-3-cloudpy-org-3-" + self.get_s3_reference_name(username=username,email=email) + "-3-cloudpy-org-3-" + str(date_id) + "_" + str(time_id)
-            ,keyStr=self.cppt.get_s3_file_content(referenceName="tek",s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/")[str(n)])
+        n = random.randint(1,100)
+        inputStr = str(random.randint(0,10000)) 
+        inputStr += str(time_id)[::-1] 
+        inputStr += "-3-cloudpy-org-3-" 
+        inputStr += self.get_s3_reference_name(username=username,email=email) 
+        inputStr += "-3-cloudpy-org-3-" + str(date_id) + "_" + str(time_id)
+        rslt = self.cppt.encrypt(inputStr = inputStr,keyStr=self.cppt.get_s3_file_content(referenceName="tek",s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/")[str(n)])
         part1 = rslt[0:int(len(rslt)/2)]
         part2 = rslt.replace(part1,"")
         delimiter = self.delimiters[random.randint(0,3)] 
         rslt = part1 + delimiter + str(n) + delimiter + part2
         return rslt
     #___________________________________________________________________
     def reference_from_service_token(self,service_token:str):
@@ -1482,41 +1484,26 @@
         print("s3://" + self.service_name + "/settings/secrets/users/")
         return self.cppt.get_s3_file_content(
             referenceName = self.reference_from_service_token(service_token=service_token)
             ,s3FullFolderPath="s3://" + self.service_name + "/settings/secrets/users/")
     #___________________________________________________________________    
     def __gsm(self,service_token:str):
         date_id,time_id = self.cppt.date_time_id()
-        ec = ''\
-        'gAAAAABkiAbFHLTMhA9MQaucvVp2uiwJckgAKW6cvE3Dq8Qrbmmp3XplBrrg1NegfsRWkIX3o4xCpTzF2wqcDPYMQzyAUC77u20n'\
-        'Edihq8AcmKHXbsyLoiirrcuAmJTaI8jBzZe5gsPSIsYVU6FX_6VrwtqwZ3xQn-LMGMJJjzIHG9wXEFpVp7cY8VLCq0213YG4n9CR'\
-        '55WwCIXigAdDyRjdI_Skh7xmZEa5JsQnhiaP7kabB9_aHnxxafoR4BJoR2_Soay8dE3LO1gbxXXBpWZJ7quLnoiPnSydPGlFSodN'\
-        'tmHj_UzEZNY9vmOOoqCVED0X6pbZxp1PXOIL8woeXP45co1l-uPihOopQxuJjyfJ4VUvl59m_hyycsYR4G42bqSvnOQjR5veRZyQ'\
-        '2OHgg3XwBFVQnpb_pPBKnBtHDN0RlILfsGk5xCOLBWOhbbEkvPh8uQsw8l3X26ED9Ja0ZDXdV_RV5PlKW2RuJNuApYHt8nXyWLyp'\
-        'wvCasAWTTGGHc1KJRX4TDgbfO8MS9EbHAPEXOEDuZ04qJdsuTq17EmsdGuhjiUIU0RBMfQ1iEvbH8wUldoXpRDpehBjE8tSaXL8y'\
-        'pien1SDZ5I_TNkboijT5oPvvS8vbr2eADt1wsCZwd5y-wyLY59dEoQ0Gf5nuxNM44AsqCgI3yiaZunAUDrigOhrI-OUl3ro22Q60'\
-        'okhPUqghD5rVyeMciizC8zQnEn5Ly12q0I0vRuZ-cDfepKpm_45jWtk9houUzo4AF1p0G22xeWD0JPECT8P6xPAHRYZjQZtYnZ3P'\
-        'pt_EcuiThCDI-AW3FM6XaBB9bD-tHWflWjFT3X39dxijDFwnOZ4DkErSiOl9Vhd2xBgsdEtY2iWcpr6u6ZgrDRpU2bqQa-QtFKK1'\
-        'm2POmuIv1H7fvnaQJWm1y92pVukFyqSkQpcw52Z2ABMasdrehQInQdrCsNSPmSZ0F5qjFby3RU9-MOjdQClhs_rTOofDQ8FoZKYd'\
-        's4_xK4hyOV74RiCzq1v62x77jfv2hD_wpjhRpd-VYapkQjCVhnDWbZh3P5xgBr_y8YizKUUU_l5b0MpZXD29NfOOgMLcUvDD_BQv'\
-        'vFcnTpqIQm9qkMLH6RA5Bb1PM3vm3OgnMxChYw16hV-Gp-QvZ7jXUpEhO0WQaVCsJWFJv7j006iyV5eh2y462HWudd5_9jJLwa0T'\
-        'VhO2vGXZuBJoGydtIvF0Hz6eZLUYOF-GmOFBcOqTC5CzbMXYhfs689pv4gfweTOqJ0RgPk1b3380HLzthHu6dCgnjV2rkK8YVA1S'\
-        'vGpPi1pdzjtFyurW7sekOit6xX1m4sdmFLTjzUaC3D-gaKmOuG0bUrz9gtXBjLiCII-e0f5-dI0AjG2yyorJ1pfh0IBui61z9ZH_'\
-        'H02v7HD5uW9GH-nOFB7xuRyOiv1bnYXYY97OeEQOyVg0_iBqX0eIAwVi-JAAic8o7bceOUsHmFE5bGhGZGWwxRXFruaSvN3WXkNQ'\
-        'uQCyXz7CjqQBRlKZMIES_OYivVHKne0LoTInK9doFvAMcvGMsfDoqXOy5Y89dxFPEy0ZnEGK_zgtBYJOpBYB2XhHl7PkaCRvQW5T'\
-        'RI3eGNnpVmc-rF6XpuFzrFTb4am8QybRYFOsV_1uXQcbS3-EYHafamZi2FFjulHrmjYf1nWiMrOEBVoBc3ISiz799ubnNH0yRA=='
-        
-        kwe = ''\
-        '*-*7161=0JhWNOtvTKFdqKiws_r58XKjsxgdROqRnUSAdtTThrt*-*71appnnqom-03202-17*-*N17*-*517*-*L17*-*W17*-*'\
-        'N17*-*O17*-*J17*-*Y17*-*1317*-*Q17*-*1317*-*S17*-*J17*-*1717*-*517*-*M17*-*0417*-*A17*-*0617*-*1117*'\
-        '-*717*-*0617*-*E17*-*417*-*2217*-*1917*-*2417*-*0117*-*T17*-*0017*-*R17*-*317*-*E17*-*F17*-*A17*-*31'\
-        '7*-*O17*-*017*-*617*-*1117*-*1317*-*=<****>gAAAAABkiAbF_mKCjCjq8bwzRht_DToYrt1dRuYYSta5G_FnUw6cMoge5'\
-        'BmZrxHvP2iHO-ncpqq_rGHd_CF5CEWf4lcR0Sst-fOWgaUGwWADReCZ5OOH7K0='
-        
-        rslt = {'encrypted_content': ec
-                ,'keystr_with_expiration': kwe
+        dat = xpt.basic_dicstr_to_dict(self.__sc[0])
+        rslt = {'encrypted_content': dat['encrypted_content']
+                ,'keystr_with_expiration': dat['keystr_with_expiration']
                 ,'date_id': date_id
                 ,'timestr': self.cppt.seconds_to_timestr(time_id)
                 ,'service_token': service_token}
-        del ec
-        del kwe
-        return str(rslt)
+        del dat
+        return str(rslt)
+def aws_framework_manager_client(username_or_email:str="",pwd:str="",local:bool=False):
+    url_base = "https://www.cloudpy.org/"
+    if local:
+        url_base = "http://localhost/"
+    url = url_base + "gen_authentication_token"
+    token = requests.post(url_base + "gen_authentication_token",json = {"username_or_email":username_or_email,"pwd":pwd} ,verify=False).text
+    secret_key = requests.post(url_base + "authenticate_with_token",json={"token":token},verify=False).text
+    service_token= requests.post(url_base + "gen_service_token",json={"secret_key":secret_key},verify=False).text
+    fm = aws_framework_manager(secret_key=secret_key)
+    print(fm.initialize_service(service_token=service_token))
+    return fm
```

### Comparing `cloudpy_org-1.3.3/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.3.4/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.3.3
+Version: 1.3.4
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.3/setup.py` & `cloudpy_org-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.3.3",
+    version="1.3.4",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

