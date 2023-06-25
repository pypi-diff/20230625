# Comparing `tmp/tahoma-2.2.9.tar.gz` & `tmp/tahoma-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.9.tar", last modified: Fri Jun 23 17:54:40 2023, max compression
+gzip compressed data, was "tahoma-2.3.0.tar", last modified: Sun Jun 25 19:02:26 2023, max compression
```

## Comparing `tahoma-2.2.9.tar` & `tahoma-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.491258 tahoma-2.2.9/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.9/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.9/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7707 2023-06-23 17:54:40.491365 tahoma-2.2.9/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7045 2023-06-23 17:52:14.000000 tahoma-2.2.9/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7044 2023-06-23 17:52:07.000000 tahoma-2.2.9/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.9/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       50 2023-06-23 17:52:37.000000 tahoma-2.2.9/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-06-23 17:54:40.491734 tahoma-2.2.9/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.9/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.485951 tahoma-2.2.9/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.9/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-06-23 17:29:50.000000 tahoma-2.2.9/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    11260 2023-06-07 10:08:50.000000 tahoma-2.2.9/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.489594 tahoma-2.2.9/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.9/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.9/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.9/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    48166 2023-06-23 17:45:50.000000 tahoma-2.2.9/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.490108 tahoma-2.2.9/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.9/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.490936 tahoma-2.2.9/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.9/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.9/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.488341 tahoma-2.2.9/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7707 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       50 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-25 19:02:26.134292 tahoma-2.3.0/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.3.0/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.3.0/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     8423 2023-06-25 19:02:26.134409 tahoma-2.3.0/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7761 2023-06-25 19:00:45.000000 tahoma-2.3.0/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7761 2023-06-25 19:00:53.000000 tahoma-2.3.0/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.3.0/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       50 2023-06-23 17:52:37.000000 tahoma-2.3.0/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-06-25 19:02:26.134702 tahoma-2.3.0/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.3.0/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-25 19:02:26.129011 tahoma-2.3.0/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.3.0/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-06-25 18:45:58.000000 tahoma-2.3.0/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    11260 2023-06-07 10:08:50.000000 tahoma-2.3.0/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-25 19:02:26.132692 tahoma-2.3.0/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.3.0/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.3.0/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.3.0/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    50433 2023-06-25 18:57:06.000000 tahoma-2.3.0/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-25 19:02:26.133223 tahoma-2.3.0/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-06-25 18:45:58.000000 tahoma-2.3.0/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-25 19:02:26.133999 tahoma-2.3.0/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.3.0/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.3.0/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-25 19:02:26.131435 tahoma-2.3.0/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     8423 2023-06-25 19:02:26.000000 tahoma-2.3.0/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-06-25 19:02:26.000000 tahoma-2.3.0/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-06-25 19:02:26.000000 tahoma-2.3.0/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-06-25 19:02:26.000000 tahoma-2.3.0/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       50 2023-06-25 19:02:26.000000 tahoma-2.3.0/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-06-25 19:02:26.000000 tahoma-2.3.0/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.9/LICENSE` & `tahoma-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.9/PKG-INFO` & `tahoma-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.9
+Version: 2.3.0
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -106,43 +106,51 @@
 
 # Usage : 
 `python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
-You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+- You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+- As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
 
-You can also run many commands during the same process without restarting tahoma :
+- You can also run many commands during the same process without restarting tahoma :
 
 For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
-There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+- There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
 
 For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
+- Since it is impossible to stop an RTS device, there is the possibility to cancel the immediate preceding command (without affecting a 'wait for <SECONDS>' command). To do this you can use the command 'cancel last action' or 'annuler precedente commande' just after a command that opens or closes an RTS device.
+
+For example :
+
+`tahoma open shutter kitchen wait for 2 cancel last action` : It will stop the kitchen shutter after 2 seconds
+
+`tahoma open shutter kitchen open shutter room6 cancel last action` : It will only stop the room6 shutter
 
 Exemples :
+Here are some example commands :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
 - tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
 - tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
 - tahoma get sensor ["Front door"] 
 - tahoma on plug office
 - tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
 - tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
 - tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
 - tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
-
+- tahoma open shutter kitchen open shutter room6 wait for 2 cancel last action` (It will stop the room6 shutter after 2 seconds)
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.9/PYPI_README.md` & `tahoma-2.3.0/PYPI_README.md`

 * *Files 5% similar despite different names*

```diff
@@ -91,43 +91,51 @@
 
 # Usage : 
 `python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
-You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+- You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+- As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
 
-You can also run many commands during the same process without restarting tahoma :
+- You can also run many commands during the same process without restarting tahoma :
 
 For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
-There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+- There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
 
 For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
+- Since it is impossible to stop an RTS device, there is the possibility to cancel the immediate preceding command (without affecting a 'wait for <SECONDS>' command). To do this you can use the command 'cancel last action' or 'annuler precedente commande' just after a command that opens or closes an RTS device.
+
+For example :
+
+`tahoma open shutter kitchen wait for 2 cancel last action` : It will stop the kitchen shutter after 2 seconds
+
+`tahoma open shutter kitchen open shutter room6 cancel last action` : It will only stop the room6 shutter
 
 Exemples :
+Here are some example commands :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
 - tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
 - tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
 - tahoma get sensor ["Front door"] 
 - tahoma on plug office
 - tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
 - tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
 - tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
 - tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
-
+- tahoma open shutter kitchen open shutter room6 wait for 2 cancel last action` (It will stop the room6 shutter after 2 seconds)
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.9/README.md` & `tahoma-2.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -91,42 +91,51 @@
 
 # Usage : 
 `python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
-You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+- You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+- As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
 
-You can also run many commands during the same process without restarting tahoma :
+- You can also run many commands during the same process without restarting tahoma :
 
 For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
-There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+- There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
 
 For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
+- Since it is impossible to stop an RTS device, there is the possibility to cancel the immediate preceding command (without affecting a 'wait for <SECONDS>' command). To do this you can use the command 'cancel last action' or 'annuler precedente commande' just after a command that opens or closes an RTS device.
+
+For example :
+
+`tahoma open shutter kitchen wait for 2 cancel last action` : It will stop the kitchen shutter after 2 seconds
+
+`tahoma open shutter kitchen open shutter room6 cancel last action` : It will only stop the room6 shutter
 
 Exemples :
+Here are some example commands :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
 - tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
 - tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
 - tahoma get sensor ["Front door"] 
 - tahoma on plug office
 - tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
 - tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
 - tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
 - tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
+- tahoma open shutter kitchen open shutter room6 wait for 2 cancel last action` (It will stop the room6 shutter after 2 seconds)
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.9/pyproject.toml` & `tahoma-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.9/tahoma/get_devices_url.py` & `tahoma-2.3.0/tahoma/get_devices_url.py`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.9/tahoma/icons/connected_house.png` & `tahoma-2.3.0/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.9/tahoma/icons/water heater.png` & `tahoma-2.3.0/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.9/tahoma/tahoma.py` & `tahoma-2.3.0/tahoma/tahoma.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,26 +104,31 @@
         print( "" )
         print( " - List of possible CATEGORIES : \n "+str(list_categories) )
         print( " - Liste des CATEGORIES possibles : \n "+str(list_categories_french) )
         print( "" )
         print( ' - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unique word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n You can also use the full NAME with [""].\n For instance ["Alarm 2"]\n See tahoma --list or tahoma --help for info.')
         print( "" )
         print( " You must provide at least 3 arguments" )
-        print( " For instance : python3 tahoma open shutter kitchen")
+        print( " For instance :  tahoma open shutter kitchen")
         print( "\n You can close a shutter or a sunscreen to a specific level (IO protocols only)")
-        print( " For instance :python3 tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%" )
+        print( " For instance : tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%" )
         print( "" )
         print( " You can also provide, as many as you wish, orders on the same line." ) 
         print( " Tahoma will execute all orders one by one in the same process ;-)" )
         print( " For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation " )
         print( "" )
         print( " You can add a wait function with 'wait for' or 'sleep for'")
         print( " Tahoma will wait the time in seconds you have specified")
         print( " For instance : tahoma open shutter kitchen wait for 20 on plug room")
         print( "" )
+        print( " The STOP action for shutters and sunscreens doesn't work with RTS protocols. " ) 
+        print( " Instead you can cancel the immediate preceding command (without affecting a 'wait for <SECONDS>' command)." )
+        print( " To do this you can use the command 'cancel last action' just after a command that opens or closes an RTS device." )
+        print( " For instance : 'tahoma open shutter kitchen wait for 2 cancel last action' : It will stop the kitchen shutter after 2 seconds" )
+        print( "" )
         print( " FIRST you must configure login and password : sudo tahoma -c " )
         print( " It will be stored there : \n "+passwd_file )
         print( "" )
         print( " THEN you must download the list of all yours devices : sudo tahoma -g " )
         print( " It will be stored there : \n "+list_of_tahoma_devices )
         print( "" )
         print( "                     To get help : tahoma -h " )
@@ -234,20 +239,22 @@
                     print( passwd_file+" is removed" )
                 except : 
                     print("The file was already removed")
             exit()
 
     for arg in sys.argv :
         if arg == '-h' or arg == '--help' :
-            print("tahoma -h, --help : "+version+"\n\nUsage:\n tahoma ACTION CATEGORY NAME \n\n You must provide at least three arguments\n For instance : tahoma open shutter kitchen or tahoma ouvrir volet cuisine\n\n You can close a shutter or a sunscreen to a specific level (IO protocols only)\n For instance : tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%\n\n You can also provide, as many as you wish, orders on the same line\n Tahoma will execute all orders one by one in the same process ;-)\n For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation\n\nHelp options :\n -h,   --help                      Show this help\n -hf,  --help-french               Show this help in french\n -i,   --info                      Show more info\n\nPlugin options :\n -v,   --version                   Show the version of the plugin\n -c,   --configure                 To configure the plugin and store login and password in a text file which is located here : "+passwd_file+" Use with sudo !\n -u,   --username                  If you don't want to store the login, you can provide the mail-address with this option\n -p,   --password                  If you don't want to store the password, you can provide it with this option\n -g,   --getlist                   Download the list of devices and store them here : "+list_of_tahoma_devices+" Use with sudo !\n -l,   --list                      Show the complet list of devices installed\n -la,  --list-actions              Show the list of possible ACTIONS by CATEGORIES\n -lc,  --list-categories           Show all supported CATEGORIES of devices\n -lnf, --list-names                Show all installed devices by there NAMES\n\nCommand options :\n wait for <seconds>                Tahoma will wait for <seconds> seconds to execute next action\n sleep for <seconds>\n")
+            print("tahoma -h, --help : "+version+"\n\nUsage:\n tahoma ACTION CATEGORY NAME \n\n You must provide at least three arguments\n For instance : tahoma open shutter kitchen or tahoma ouvrir volet cuisine\n\n You can close a shutter or a sunscreen to a specific level (IO protocols only)\n For instance : tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%\n\n You can also provide, as many as you wish, orders on the same line\n Tahoma will execute all orders one by one in the same process ;-)\n For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation\n\nHelp options :\n -h,   --help                      Show this help\n -hf,  --help-french               Show this help in french\n -i,   --info                      Show more info\n\nPlugin options :\n -v,   --version                   Show the version of the plugin\n -c,   --configure                 To configure the plugin and store login and password in a text file which is located here : "+passwd_file+" Use with sudo !\n -u,   --username                  If you don't want to store the login, you can provide the mail-address with this option\n -p,   --password                  If you don't want to store the password, you can provide it with this option\n -g,   --getlist                   Download the list of devices and store them here : "+list_of_tahoma_devices+" Use with sudo !\n -l,   --list                      Show the complet list of devices installed\n -la,  --list-actions              Show the list of possible ACTIONS by CATEGORIES\n -lc,  --list-categories           Show all supported CATEGORIES of devices\n -lnf, --list-names                Show all installed devices by there NAMES\n\nCommand options :\n wait for <seconds>\n sleep for <seconds>               Tahoma will wait for <seconds> seconds to execute next action\n cancel last action                Tahoma will cancel the immediate preceding command (without affecting the 'wait for' command). This is useful for stopping an RTS device\n")
+            check_last_release ()
             exit()
 
     for arg in sys.argv :
         if arg == '-hf' or arg == '--help-french' :
-            print("tahoma -h --help : "+version+"\n\nUsage:\n tahoma ACTION CATEGORIE NOM \n\n Vous devez fournir au moins trois arguments\n Par exemple : tahoma ouvrir volet cuisine ou tahoma open shutter kitchen\n\n Vous pouvez fermer des rideaux ou des volets à un niveau precis (Seulement pour les équipements utilisant le protocole IO)\n Par exemple : tahoma 25 volet cuisine. Les volets vont s'ouvrir de 75% ou se fermer de 25%\n\n Vous pouvez aussi spécifier autant de commandes que vous le souhaitez sur la même ligne :\n Tahoma va executer chaque commande l'une aprés l'autre durant le même processus\n Par exemple : tahoma ouvrir volet cuisine confort chauffage salon\n\nOptions de l’aide :\n -h, --help                        Affiche les options de l’aide en anglais\n\nOptions de l’application :\n -v, --version                     Affiche la version de l’application\n -i, --info                        Afficher plus d'infos sur tahoma\n -c, --configure                   Renseigner l'identifiant et le mot de passe dans un fichier texte pour ne pas devoir les renseigner à chaque fois. Le fichier texte se situe dans : "+passwd_file+" Utiliser sudo !\n -u, --username                    Renseigner le nom d'utilisateur\n -p, --password                    Renseigner le mot de passe de Somfy-connect\n -g, --getlist                     Télécharge la liste des équipements et la stocke dans "+list_of_tahoma_devices+" Utiliser sudo !\n -l, --list                        Affiche la liste téléchargée des équipements\n -laf, --list-actions-french       Affiche la liste des ACTIONS possibles en français par CATEGORIES\n -lcf, --list-categories-french    Affiche toutes les CATEGORIES d'équipements pris en charge en français\n -lnf, --list-names-french         Affiche les NOMS des équipements installés par categories en français\n\nOptions de commande :\n attendre pendant <secondes>       Tahoma attendra <secondes> secondes avant d'éxécuter la commande suivante\n")
+            print("tahoma -h --help : "+version+"\n\nUsage:\n tahoma ACTION CATEGORIE NOM \n\n Vous devez fournir au moins trois arguments\n Par exemple : tahoma ouvrir volet cuisine ou tahoma open shutter kitchen\n\n Vous pouvez fermer des rideaux ou des volets à un niveau precis (Seulement pour les équipements utilisant le protocole IO)\n Par exemple : tahoma 25 volet cuisine. Les volets vont s'ouvrir de 75% ou se fermer de 25%\n\n Vous pouvez aussi spécifier autant de commandes que vous le souhaitez sur la même ligne :\n Tahoma va executer chaque commande l'une aprés l'autre durant le même processus\n Par exemple : tahoma ouvrir volet cuisine confort chauffage salon\n\nOptions de l’aide :\n -h, --help                        Affiche les options de l’aide en anglais\n\nOptions de l’application :\n -v, --version                     Affiche la version de l’application\n -i, --info                        Afficher plus d'infos sur tahoma\n -c, --configure                   Renseigner l'identifiant et le mot de passe dans un fichier texte pour ne pas devoir les renseigner à chaque fois. Le fichier texte se situe dans : "+passwd_file+" Utiliser sudo !\n -u, --username                    Renseigner le nom d'utilisateur\n -p, --password                    Renseigner le mot de passe de Somfy-connect\n -g, --getlist                     Télécharge la liste des équipements et la stocke dans "+list_of_tahoma_devices+" Utiliser sudo !\n -l, --list                        Affiche la liste téléchargée des équipements\n -laf, --list-actions-french       Affiche la liste des ACTIONS possibles en français par CATEGORIES\n -lcf, --list-categories-french    Affiche toutes les CATEGORIES d'équipements pris en charge en français\n -lnf, --list-names-french         Affiche les NOMS des équipements installés par categories en français\n\nOptions de commande :\n attendre pendant <secondes>       Tahoma attendra <secondes> secondes avant d'éxécuter la commande suivante\n annuler precedente commande       Tahoma annulera la commande précédente immédiate (sans affecter la commande 'attendre pendant'). Ceci est utile pour arrêter un périphérique RTS.")
+            check_last_release ()
             exit()
 
     for arg in sys.argv :
         if arg == '-lc' or arg == '--list-categories' :
             print( "tahoma can control this type of devices's categories :\n"+str(list_categories))
             exit()
 
@@ -409,15 +416,15 @@
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
                 fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
                 fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
-                print("Be careful! The 'stop' function is only available for IO protocols. It doesn't work with RTS devices, it will use the 'MY'function instead...")
+                print("Please note that the 'stop' ACTION is only compatible with IO protocols and will not work with RTS devices. If you are using an RTS device, please use the command 'tahoma CANCEL LAST ACTION' instead.")
                 fonction = Command(OverkizCommand.STOP)
             elif remove_accent(action).upper() == 'MY' :
                 fonction = Command(OverkizCommand.MY)
             elif str(action).isnumeric() == True :
                 fonction = Command(OverkizCommand.SET_CLOSURE, [int(action)])
                 print('Will close to '+str(action)+' %')
                 print("Be careful! This function is only available for IO protocols. It doesn't work with RTS devices...")
@@ -459,15 +466,15 @@
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
                 fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
                 fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
-                print("Be careful! The 'stop' function is only available for IO protocols. It doesn't work with RTS devices, it will use the 'MY'function instead...")
+                print("Please note that the 'stop' function is only compatible with IO protocols and will not work with RTS devices. If you are using an RTS device, please use the command 'tahoma CANCEL LAST ACTION' instead.")
                 fonction = Command(OverkizCommand.STOP)
             elif remove_accent(action).upper() == 'MY' :
                 fonction = Command(OverkizCommand.MY)
             elif str(action).isnumeric() == True :
                 fonction = Command(OverkizCommand.SET_CLOSURE, [int(action)])
                 print('Will close to '+str(action)+' %')
                 print("Be careful! This function is only available for IO protocols. It doesn't work with RTS devices...")
@@ -708,28 +715,34 @@
 #                     command_state.append(i.split(",")[3])
 
         ##########################WAIT FUNCTION
 
         elif remove_accent(action) == 'wait' or remove_accent(action) == 'sleep' or remove_accent(action) == 'attendre':
             url.append(int(name))
 
+        ##########################CANCEL LAST ACTION FUNCTION
+
+        elif remove_accent(action) == 'cancel' or remove_accent(action) == 'annuler':
+            url.append('pass')
+
         ##########################
 
         else :
             print( "\nThe <CATEGORY> you have entered doesn't exist.\nChoose one of this category : "+str(list_categories)+"\nUse tahoma --help-categories or tahoma --list-categories for info")
 
 
     ##########################MAIN FUNCTION
 
         try:
             async def main() -> None:
                 try :
                     j=0
                     for device_url in url :
                         if str(device_url).isnumeric() == True :
+                            print("Waiting for "+str(device_url)+" second(s).")
                             time.sleep(int(device_url))
                         else :
                             if remove_accent(category) == 'scene' or remove_accent(category) == 'scenario':
                                 try :
                                     async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
                                         await client.login()
                                         exec_id = await client.execute_scenario(device_url)
@@ -737,14 +750,26 @@
                             elif remove_accent(category) == 'sensor' or remove_accent(category) == 'capteur':
                                 try:
                                     async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
                                         get_state = await client.get_state(device_url)
                                         state_function=str(command_state[j]).replace("['","").replace("']","")
                                         print('The '+str(good_name[j])+' is '+str(eval(state_function)))
                                 except :pass
+                            elif remove_accent(action).upper() == 'CANCEL' or remove_accent(action).upper() == 'ANNULER':
+                                try:
+                                    async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
+                                        await client.login()
+                                        executions = await client.get_current_executions()
+                                        for execution in executions:
+                                            execution_id=str(execution.id)
+                                        try:
+                                            await client.cancel_command(str(execution_id))
+                                            print("The command with execution ID  : "+execution_id+" has been successfully cancelled.")
+                                        except: pass
+                                except : pass
                             else :
                                 try :
                                     async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
                                         await client.login()
                                         exec_id = await client.execute_command( device_url, fonction )
                                 except : pass
                             j=j+1
```

### Comparing `tahoma-2.2.9/tahoma.egg-info/PKG-INFO` & `tahoma-2.3.0/tahoma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.9
+Version: 2.3.0
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -106,43 +106,51 @@
 
 # Usage : 
 `python3 tahoma.py [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
-You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
+- You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
-As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
+- As name you can use a unic word like `bath` or the full name with `[""]` like `["bath 1st floor"]`
 
-You can also run many commands during the same process without restarting tahoma :
+- You can also run many commands during the same process without restarting tahoma :
 
 For instance : `tahoma arm alarm garden open shutter ["room 6"] confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
-There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
+- There is also a wait functionality with `wait for` or `sleep for` or `attendre pendant` :
 
 For instance : `tahoma open shutter kitchen wait for 20 close shutter kitchen`
 
+- Since it is impossible to stop an RTS device, there is the possibility to cancel the immediate preceding command (without affecting a 'wait for <SECONDS>' command). To do this you can use the command 'cancel last action' or 'annuler precedente commande' just after a command that opens or closes an RTS device.
+
+For example :
+
+`tahoma open shutter kitchen wait for 2 cancel last action` : It will stop the kitchen shutter after 2 seconds
+
+`tahoma open shutter kitchen open shutter room6 cancel last action` : It will only stop the room6 shutter
 
 Exemples :
+Here are some example commands :
 
 - tahoma open shutter kitchen
 - tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
 - tahoma get sensor ["Luminance sensor garden"] (You can use the full name of the device with `["<NAME>"]` )
 - tahoma get sensor door (You will receive all the informations about all the sensors with the name `door` in the house in one time)
 - tahoma get sensor ["Front door"] 
 - tahoma on plug office
 - tahoma open shutter ["room 6"]
 - tahoma arm alarm garden
 - tahoma confort heater dining
 - tahoma get sensor ['heater dining room']
 - tahoma launch scene morning
 - tahoma arm alarm garden wait for 10 open shutter room6 sleep for 7 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
 - tahoma comfort heater dining wait for 3 get sensor ["Heater dining room"]
-
+- tahoma open shutter kitchen open shutter room6 wait for 2 cancel last action` (It will stop the room6 shutter after 2 seconds)
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] :
```

### Comparing `tahoma-2.2.9/tahoma.egg-info/SOURCES.txt` & `tahoma-2.3.0/tahoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

