# Comparing `tmp/whatsapp-chat-exporter-0.9.1.tar.gz` & `tmp/whatsapp-chat-exporter-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chat-exporter-0.9.1.tar", last modified: Tue May 16 16:15:20 2023, max compression
+gzip compressed data, was "whatsapp-chat-exporter-0.9.5.tar", last modified: Sun Jun 25 05:59:08 2023, max compression
```

## Comparing `whatsapp-chat-exporter-0.9.1.tar` & `whatsapp-chat-exporter-0.9.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:15:20.332943 whatsapp-chat-exporter-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-16 16:15:20.332943 whatsapp-chat-exporter-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:15:20.328943 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/whatsapp.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:15:20.332943 whatsapp-chat-exporter-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:15:20.328943 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:08.370844 whatsapp-chat-exporter-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-25 05:59:08.370844 whatsapp-chat-exporter-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:08.370844 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29916 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/extract_exported.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/extract_iphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/extract_iphone_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/whatsapp.html
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:59:08.370844 whatsapp-chat-exporter-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-25 05:58:58.000000 whatsapp-chat-exporter-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:59:08.370844 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-25 05:59:08.000000 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-25 05:59:08.000000 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:59:08.000000 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 05:59:08.000000 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-25 05:59:08.000000 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 05:59:08.000000 whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/top_level.txt
```

### Comparing `whatsapp-chat-exporter-0.9.1/LICENSE` & `whatsapp-chat-exporter-0.9.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Knugi
+Copyright (c) 2021-2023 Knugi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `whatsapp-chat-exporter-0.9.1/PKG-INFO` & `whatsapp-chat-exporter-0.9.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: whatsapp-chat-exporter
-Version: 0.9.1
-Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
-Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
-Author: KnugiHK
-Author-email: hello@knugi.com
-License: MIT
-Keywords: android,ios,parsing,history,iphone,whatsapp,messagecustomizable,android-backup,crypt12,whatsapp-chat-exporter,whatsapp-export,whatsapp-database,whatsapp-database-parser,whatsapp-conversations,iphone-backup,crypt14,crypt15,messages
-Platform: any
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Utilities
-Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: android_backup
-Provides-Extra: crypt12
-Provides-Extra: crypt14
-Provides-Extra: crypt15
-License-File: LICENSE
-
 # Whatsapp-Chat-Exporter
 [![Latest in Pypi](https://img.shields.io/pypi/v/whatsapp-chat-exporter?label=Latest%20in%20Pypi)](https://pypi.org/project/whatsapp-chat-exporter/)
 ![License MIT](https://img.shields.io/pypi/l/whatsapp-chat-exporter)
 [![Python](https://img.shields.io/pypi/pyversions/Whatsapp-Chat-Exporter)](https://pypi.org/project/Whatsapp-Chat-Exporter/)
 
 A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Inspired by [Telegram Chat Export Tool](https://telegram.org/blog/export-and-more).  
 **If you plan to uninstall WhatsApp or delete your WhatsApp account, please make a backup of your WhatsApp database. You may want to use this exporter again on the same database in the future as the exporter develops**
@@ -71,14 +40,16 @@
 In order to support the decryption, install pycryptodome if it is not installed
 ```sh
 pip install pycryptodome # Or 
 pip install whatsapp-chat-exporter["android_backup"] # install along with this software
 ```
 ### Crypt15 is now the easiest way to decrypt a backup. If you have the 32 bytes hex key generated when you enable End-to-End encrypted backup, you can use it to decrypt the backup. If you do not have the 32 bytes hex key, you can still use the key file extracted just like extacting key file for Crypt12 and Crypt14 to decrypt the backup.
 #### Crypt12 or Crypt14
+You will need the decryption key file from your phone. If you have root access, you can find it as `/data/data/com.whatsapp/files/key`. Otherwise, if you used WhatsApp-Key-DB-Extractor before, it will appear in the WhatsApp backup directory as `WhatsApp/Databases/.nomedia`.
+
 Place the decryption key file (key) and the encrypted WhatsApp Backup (msgstore.db.crypt14) in the working directory. If you also want the name of your contacts, get the contact database, which is called wa.db. And copy the WhatsApp (Media) directory from your phone directly.
 
 And now, you should have something like this in the working directory.
 
 ![Android folder structure with WhatsApp Backup](imgs/android_structure_backup.png)
 #### Extracting
 Simply invoke the following command from shell.
@@ -104,70 +75,87 @@
 wtsexporter -a -k encrypted_backup.key -b msgstore.db.crypt15
 ```
 If you have the 32 bytes hex key, simply put the hex key in the -k option and invoke the command from shell like this:
 ```sh
 wtsexporter -a -k 432435053b5204b08e5c3823423399aa30ff061435ab89bc4e6713969cdaa5a8 -b msgstore.db.crypt15
 ```
 
-## Working with iPhone
-Do an iPhone Backup with iTunes first.
-### Encrypted iPhone Backup
-**If you are working on unencrypted iPhone backup, skip this**
+## Working with iOS/iPadOS (iPhone or iPad)
+Do an iPhone/iPad Backup with iTunes first.
+* iPhone backup on Mac: https://support.apple.com/HT211229
+* iPhone backup on Windows: https://support.apple.com/HT212156
+* iPad backup: https://support.apple.com/guide/ipad/ipad9a74df05xx/ipados
+### Encrypted iOS/iPadOS Backup
+**If you are working on unencrypted iOS/iPadOS backup, skip this**
 
-If you want to work on an encrypted iPhone Backup, you should install iphone_backup_decrypt from [KnugiHK/iphone_backup_decrypt](https://github.com/KnugiHK/iphone_backup_decrypt) before you run the extract_iphone_media.py.
+If you want to work on an encrypted iOS/iPadOS Backup, you should install iphone_backup_decrypt from [KnugiHK/iphone_backup_decrypt](https://github.com/KnugiHK/iphone_backup_decrypt) before you run the extract_iphone_media.py.
 ```sh
 pip install git+https://github.com/KnugiHK/iphone_backup_decrypt
 ```
 ### Extracting
 Simply invoke the following command from shell, remember to replace the username and device id correspondingly in the command.
+#### Windows
 ```sh
 wtsexporter -i -b "C:\Users\[Username]\AppData\Roaming\Apple Computer\MobileSync\Backup\[device id]"
 ```
+#### Mac
+```sh
+wtsexporter -i -b "~/Library/Application Support/MobileSync/Backup/[device id]"
+```
 
 ## Results
 After extracting, you will get these:
 #### Private Message
 ![Private Message](imgs/pm.png)
 
 #### Group Message
 ![Group Message](imgs/group.png)
 
+*The above screenshots were taken longgggggggggggggg ago. I am going to update them when possible.*
+
 ## More options
 Invoke the wtsexporter with --help option will show you all options available.
 ```sh
 > wtsexporter --help
-usage: wtsexporter [options]
+usage: wtsexporter [-h] [-a] [-i] [-e EXPORTED] [-w WA] [-m MEDIA] [-b BACKUP] [-o OUTPUT] [-j [JSON]] [-d DB] [-k KEY] [-t TEMPLATE] [-s] [-c] [--offline OFFLINE] [--size [SIZE]]
+                   [--no-html] [--check-update] [--assume-first-as-me]
 
 options:
   -h, --help            show this help message and exit
   -a, --android         Define the target as Android
-  -i, --iphone, --ios   Define the target as iPhone
+  -i, --iphone, --ios   Define the target as iPhone/iPad
+  -e EXPORTED, --exported EXPORTED
+                        Define the target as exported chat file and specify the path to the file
   -w WA, --wa WA        Path to contact database (default: wa.db/ContactsV2.sqlite)
   -m MEDIA, --media MEDIA
                         Path to WhatsApp media folder (default: WhatsApp)
   -b BACKUP, --backup BACKUP
                         Path to Android (must be used together with -k)/iPhone WhatsApp backup
   -o OUTPUT, --output OUTPUT
                         Output to specific directory (default: result)
   -j [JSON], --json [JSON]
                         Save the result to a single JSON file (default if present: result.json)
   -d DB, --db DB        Path to database file (default: msgstore.db/7c7fba66680ef796b916b067077cc246adacf01d)
   -k KEY, --key KEY     Path to key file
   -t TEMPLATE, --template TEMPLATE
                         Path to custom HTML template
-  -e, --embedded        Embed media into HTML file (not yet implemented)
   -s, --showkey         Show the HEX key used to decrypt the database
   -c, --move-media      Move the media directory to output directory if the flag is set, otherwise copy it
   --offline OFFLINE     Relative path to offline static files
-  --size SIZE, --output-size SIZE
-                        Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
+  --size [SIZE], --output-size [SIZE], --split [SIZE]
+                        Maximum (rough) size of a single output file in bytes, 0 for auto
   --no-html             Do not output html files
-  --check-update        Check for updates
+  --check-update        Check for updates (require Internet access)
+  --assume-first-as-me  Assume the first message in a chat as sent by me (must be used together with -e)
+
+WhatsApp Chat Exporter: 0.9.5 Licensed with MIT
 ```
 
 # To do
 See [issues](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues).
 
 # Copyright
 This is a MIT licensed project.
 
 The Telegram Desktop's export is the reference for whatsapp.html in this repo
+
+WhatsApp Chat Exporter is not affiliated, associated, authorized, endorsed by, or in any way officially connected with the WhatsApp LLC, or any of its subsidiaries or its affiliates. The official WhatsApp LLC website can be found at https://www.whatsapp.com/.
```

### Comparing `whatsapp-chat-exporter-0.9.1/README.md` & `whatsapp-chat-exporter-0.9.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: whatsapp-chat-exporter
+Version: 0.9.5
+Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Android, iOS, iPadOS, Crypt12, Crypt14, Crypt15 supported.
+Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
+Author: KnugiHK
+Author-email: hello@knugi.com
+License: MIT
+Keywords: android,ios,parsing,history,iphone,message,crypt15,customizable,whatsapp,android-backup,messages,crypt14,crypt12,whatsapp-chat-exporter,whatsapp-export,iphone-backup,whatsapp-database,whatsapp-database-parser,whatsapp-conversations
+Platform: any
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Utilities
+Classifier: Topic :: Database
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: android_backup
+Provides-Extra: crypt12
+Provides-Extra: crypt14
+Provides-Extra: crypt15
+Provides-Extra: all
+Provides-Extra: everything
+Provides-Extra: backup
+License-File: LICENSE
+
 # Whatsapp-Chat-Exporter
 [![Latest in Pypi](https://img.shields.io/pypi/v/whatsapp-chat-exporter?label=Latest%20in%20Pypi)](https://pypi.org/project/whatsapp-chat-exporter/)
 ![License MIT](https://img.shields.io/pypi/l/whatsapp-chat-exporter)
 [![Python](https://img.shields.io/pypi/pyversions/Whatsapp-Chat-Exporter)](https://pypi.org/project/Whatsapp-Chat-Exporter/)
 
 A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Inspired by [Telegram Chat Export Tool](https://telegram.org/blog/export-and-more).  
 **If you plan to uninstall WhatsApp or delete your WhatsApp account, please make a backup of your WhatsApp database. You may want to use this exporter again on the same database in the future as the exporter develops**
@@ -40,14 +74,16 @@
 In order to support the decryption, install pycryptodome if it is not installed
 ```sh
 pip install pycryptodome # Or 
 pip install whatsapp-chat-exporter["android_backup"] # install along with this software
 ```
 ### Crypt15 is now the easiest way to decrypt a backup. If you have the 32 bytes hex key generated when you enable End-to-End encrypted backup, you can use it to decrypt the backup. If you do not have the 32 bytes hex key, you can still use the key file extracted just like extacting key file for Crypt12 and Crypt14 to decrypt the backup.
 #### Crypt12 or Crypt14
+You will need the decryption key file from your phone. If you have root access, you can find it as `/data/data/com.whatsapp/files/key`. Otherwise, if you used WhatsApp-Key-DB-Extractor before, it will appear in the WhatsApp backup directory as `WhatsApp/Databases/.nomedia`.
+
 Place the decryption key file (key) and the encrypted WhatsApp Backup (msgstore.db.crypt14) in the working directory. If you also want the name of your contacts, get the contact database, which is called wa.db. And copy the WhatsApp (Media) directory from your phone directly.
 
 And now, you should have something like this in the working directory.
 
 ![Android folder structure with WhatsApp Backup](imgs/android_structure_backup.png)
 #### Extracting
 Simply invoke the following command from shell.
@@ -73,70 +109,87 @@
 wtsexporter -a -k encrypted_backup.key -b msgstore.db.crypt15
 ```
 If you have the 32 bytes hex key, simply put the hex key in the -k option and invoke the command from shell like this:
 ```sh
 wtsexporter -a -k 432435053b5204b08e5c3823423399aa30ff061435ab89bc4e6713969cdaa5a8 -b msgstore.db.crypt15
 ```
 
-## Working with iPhone
-Do an iPhone Backup with iTunes first.
-### Encrypted iPhone Backup
-**If you are working on unencrypted iPhone backup, skip this**
+## Working with iOS/iPadOS (iPhone or iPad)
+Do an iPhone/iPad Backup with iTunes first.
+* iPhone backup on Mac: https://support.apple.com/HT211229
+* iPhone backup on Windows: https://support.apple.com/HT212156
+* iPad backup: https://support.apple.com/guide/ipad/ipad9a74df05xx/ipados
+### Encrypted iOS/iPadOS Backup
+**If you are working on unencrypted iOS/iPadOS backup, skip this**
 
-If you want to work on an encrypted iPhone Backup, you should install iphone_backup_decrypt from [KnugiHK/iphone_backup_decrypt](https://github.com/KnugiHK/iphone_backup_decrypt) before you run the extract_iphone_media.py.
+If you want to work on an encrypted iOS/iPadOS Backup, you should install iphone_backup_decrypt from [KnugiHK/iphone_backup_decrypt](https://github.com/KnugiHK/iphone_backup_decrypt) before you run the extract_iphone_media.py.
 ```sh
 pip install git+https://github.com/KnugiHK/iphone_backup_decrypt
 ```
 ### Extracting
 Simply invoke the following command from shell, remember to replace the username and device id correspondingly in the command.
+#### Windows
 ```sh
 wtsexporter -i -b "C:\Users\[Username]\AppData\Roaming\Apple Computer\MobileSync\Backup\[device id]"
 ```
+#### Mac
+```sh
+wtsexporter -i -b "~/Library/Application Support/MobileSync/Backup/[device id]"
+```
 
 ## Results
 After extracting, you will get these:
 #### Private Message
 ![Private Message](imgs/pm.png)
 
 #### Group Message
 ![Group Message](imgs/group.png)
 
+*The above screenshots were taken longgggggggggggggg ago. I am going to update them when possible.*
+
 ## More options
 Invoke the wtsexporter with --help option will show you all options available.
 ```sh
 > wtsexporter --help
-usage: wtsexporter [options]
+usage: wtsexporter [-h] [-a] [-i] [-e EXPORTED] [-w WA] [-m MEDIA] [-b BACKUP] [-o OUTPUT] [-j [JSON]] [-d DB] [-k KEY] [-t TEMPLATE] [-s] [-c] [--offline OFFLINE] [--size [SIZE]]
+                   [--no-html] [--check-update] [--assume-first-as-me]
 
 options:
   -h, --help            show this help message and exit
   -a, --android         Define the target as Android
-  -i, --iphone, --ios   Define the target as iPhone
+  -i, --iphone, --ios   Define the target as iPhone/iPad
+  -e EXPORTED, --exported EXPORTED
+                        Define the target as exported chat file and specify the path to the file
   -w WA, --wa WA        Path to contact database (default: wa.db/ContactsV2.sqlite)
   -m MEDIA, --media MEDIA
                         Path to WhatsApp media folder (default: WhatsApp)
   -b BACKUP, --backup BACKUP
                         Path to Android (must be used together with -k)/iPhone WhatsApp backup
   -o OUTPUT, --output OUTPUT
                         Output to specific directory (default: result)
   -j [JSON], --json [JSON]
                         Save the result to a single JSON file (default if present: result.json)
   -d DB, --db DB        Path to database file (default: msgstore.db/7c7fba66680ef796b916b067077cc246adacf01d)
   -k KEY, --key KEY     Path to key file
   -t TEMPLATE, --template TEMPLATE
                         Path to custom HTML template
-  -e, --embedded        Embed media into HTML file (not yet implemented)
   -s, --showkey         Show the HEX key used to decrypt the database
   -c, --move-media      Move the media directory to output directory if the flag is set, otherwise copy it
   --offline OFFLINE     Relative path to offline static files
-  --size SIZE, --output-size SIZE
-                        Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
+  --size [SIZE], --output-size [SIZE], --split [SIZE]
+                        Maximum (rough) size of a single output file in bytes, 0 for auto
   --no-html             Do not output html files
-  --check-update        Check for updates
+  --check-update        Check for updates (require Internet access)
+  --assume-first-as-me  Assume the first message in a chat as sent by me (must be used together with -e)
+
+WhatsApp Chat Exporter: 0.9.5 Licensed with MIT
 ```
 
 # To do
 See [issues](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues).
 
 # Copyright
 This is a MIT licensed project.
 
 The Telegram Desktop's export is the reference for whatsapp.html in this repo
+
+WhatsApp Chat Exporter is not affiliated, associated, authorized, endorsed by, or in any way officially connected with the WhatsApp LLC, or any of its subsidiaries or its affiliates. The official WhatsApp LLC website can be found at https://www.whatsapp.com/.
```

### Comparing `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/__main__.py` & `whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-try:
-    from .__init__ import __version__
-except ImportError:
-    from Whatsapp_Chat_Exporter.__init__ import __version__
-from Whatsapp_Chat_Exporter import extract, extract_iphone
-from Whatsapp_Chat_Exporter import extract_iphone_media
-from Whatsapp_Chat_Exporter.data_model import ChatStore
-from Whatsapp_Chat_Exporter.utility import Crypt, check_update
-from argparse import ArgumentParser
+#!/usr/bin/python3
+
 import os
 import sqlite3
 import shutil
 import json
 import string
+import glob
+from Whatsapp_Chat_Exporter import extract_exported, extract_iphone
+from Whatsapp_Chat_Exporter import extract, extract_iphone_media
+from Whatsapp_Chat_Exporter.data_model import ChatStore
+from Whatsapp_Chat_Exporter.utility import Crypt, check_update, import_from_json
+from argparse import ArgumentParser, SUPPRESS
 from sys import exit
+try:
+    from .__init__ import __version__
+except ImportError:
+    from Whatsapp_Chat_Exporter.__init__ import __version__
 
 
 def main():
     parser = ArgumentParser(
         description = 'A customizable Android and iPhone WhatsApp database parser that '
                       'will give you the history of your WhatsApp conversations inHTML '
                       'and JSON. Android Backup Crypt12, Crypt14 and Crypt15 supported.',
@@ -34,14 +37,21 @@
         '--iphone',
         '--ios',
         dest='iphone',
         default=False,
         action='store_true',
         help="Define the target as iPhone/iPad")
     parser.add_argument(
+        "-e",
+        "--exported",
+        dest="exported",
+        default=None,
+        help="Define the target as exported chat file and specify the path to the file"
+    )
+    parser.add_argument(
         "-w",
         "--wa",
         dest="wa",
         default=None,
         help="Path to contact database (default: wa.db/ContactsV2.sqlite)")
     parser.add_argument(
         "-m",
@@ -89,20 +99,19 @@
         "-t",
         "--template",
         dest="template",
         default=None,
         help="Path to custom HTML template"
     )
     parser.add_argument(
-        "-e",
         "--embedded",
         dest="embedded",
         default=False,
         action='store_true',
-        help="Embed media into HTML file (not yet implemented)"
+        help=SUPPRESS or "Embed media into HTML file (not yet implemented)"
     )
     parser.add_argument(
         "-s",
         "--showkey",
         dest="showkey",
         default=False,
         action='store_true',
@@ -121,48 +130,79 @@
         dest="offline",
         default=None,
         help="Relative path to offline static files"
     )
     parser.add_argument(
         "--size",
         "--output-size",
+        "--split",
         dest="size",
+        nargs='?',
+        type=int,
+        const=0,
         default=None,
-        help="Maximum size of a single output file in bytes, 0 for auto (not yet implemented)"
+        help="Maximum (rough) size of a single output file in bytes, 0 for auto"
     )
     parser.add_argument(
         "--no-html",
         dest="no_html",
         default=False,
         action='store_true',
         help="Do not output html files"
     )
     parser.add_argument(
         "--check-update",
         dest="check_update",
         default=False,
         action='store_true',
-        help="Check for updates"
+        help="Check for updates (require Internet access)"
+    )
+    parser.add_argument(
+        "--assume-first-as-me",
+        dest="assume_first_as_me",
+        default=False,
+        action='store_true',
+        help="Assume the first message in a chat as sent by me (must be used together with -e)"
+    )
+    parser.add_argument(
+        "--no-avatar",
+        dest="no_avatar",
+        default=False,
+        action='store_true',
+        help="Do not render avatar in HTML output"
+    )
+    parser.add_argument(
+        "--import",
+        dest="import_json",
+        default=False,
+        action='store_true',
+        help="Import JSON file and convert to HTML output"
     )
     args = parser.parse_args()
 
     # Check for updates
     if args.check_update:
         exit(check_update())
 
     # Sanity checks
-    if args.android and args.iphone:
+    if args.android and args.iphone and args.exported and args.import_json:
         print("You must define only one device type.")
         exit(1)
-    if not args.android and not args.iphone:
+    if not args.android and not args.iphone and not args.exported and not args.import_json:
         print("You must define the device type.")
         exit(1)
     if args.no_html and not args.json:
         print("You must either specify a JSON output file or enable HTML output.")
         exit(1)
+    if args.import_json and (args.android or args.iphone or args.exported or args.no_html):
+        print("You can only use --import with -j and without --no-html.")
+        exit(1)
+    elif args.import_json and not os.path.isfile(args.json):
+        print("JSON file not found.")
+        exit(1)
 
     data = {}
 
     if args.android:
         contacts = extract.contacts
         messages = extract.messages
         media = extract.media
@@ -208,73 +248,114 @@
         if args.media is None:
             args.media = "WhatsApp"
 
         if os.path.isfile(contact_db):
             with sqlite3.connect(contact_db) as db:
                 db.row_factory = sqlite3.Row
                 contacts(db, data)
-
     elif args.iphone:
         import sys
         if "--iphone" in sys.argv:
-            print("WARNING: The --iphone flag is deprecated and will be removed in the future. Use --ios instead.")
+            print(
+                "WARNING: The --iphone flag is deprecated and will"
+                "be removed in the future. Use --ios instead."
+            )
+        contacts = extract_iphone.contacts
         messages = extract_iphone.messages
         media = extract_iphone.media
         vcard = extract_iphone.vcard
-        create_html = extract_iphone.create_html
+        create_html = extract.create_html
+        if args.media is None:
+            args.media = "AppDomainGroup-group.net.whatsapp.WhatsApp.shared"
         if args.backup is not None:
-            extract_iphone_media.extract_media(args.backup)
+            if not os.path.isdir(args.media):
+                extract_iphone_media.extract_media(args.backup)
+            else:
+                print("WhatsApp directory already exists, skipping WhatsApp file extraction.")
         if args.db is None:
             msg_db = "7c7fba66680ef796b916b067077cc246adacf01d"
         else:
             msg_db = args.db
         if args.wa is None:
             contact_db = "ContactsV2.sqlite"
         else:
             contact_db = args.wa
-        if args.media is None:
-            args.media = "Message"
+        if os.path.isfile(contact_db):
+            with sqlite3.connect(contact_db) as db:
+                db.row_factory = sqlite3.Row
+                contacts(db, data)
+
+    if not args.exported and not args.import_json:
+        if os.path.isfile(msg_db):
+            with sqlite3.connect(msg_db) as db:
+                db.row_factory = sqlite3.Row
+                messages(db, data, args.media)
+                media(db, data, args.media)
+                vcard(db, data)
+                if args.android:
+                    extract.calls(db, data)
+            if not args.no_html:
+                create_html(
+                    data,
+                    args.output,
+                    args.template,
+                    args.embedded,
+                    args.offline,
+                    args.size,
+                    args.no_avatar
+                )
+        else:
+            print(
+                "The message database does not exist. You may specify the path "
+                "to database file with option -d or check your provided path."
+            )
+            exit(2)
 
-    if os.path.isfile(msg_db):
-        with sqlite3.connect(msg_db) as db:
-            db.row_factory = sqlite3.Row
-            messages(db, data)
-            media(db, data, args.media)
-            vcard(db, data)
+        if os.path.isdir(args.media):
+            media_path = os.path.join(args.output, args.media)
+            if os.path.isdir(media_path):
+                print("\nWhatsApp directory already exists in output directory. Skipping...", end="\n")
+            else:
+                if not args.move_media:
+                    if os.path.isdir(media_path):
+                        print("\nWhatsApp directory already exists in output directory. Skipping...", end="\n")
+                    else:
+                        print("\nCopying media directory...", end="\n")
+                        shutil.copytree(args.media, media_path)
+                else:
+                    try:
+                        shutil.move(args.media, f"{args.output}/")
+                    except PermissionError:
+                        print("\nCannot remove original WhatsApp directory. "
+                            "Perhaps the directory is opened?", end="\n")
+    elif args.exported:
+        extract_exported.messages(args.exported, data, args.assume_first_as_me)
         if not args.no_html:
-            create_html(
+            extract.create_html(
                 data,
                 args.output,
                 args.template,
                 args.embedded,
                 args.offline,
                 args.size
             )
-    else:
-        print(
-            "The message database does not exist. You may specify the path "
-            "to database file with option -d or check your provided path."
+        for file in glob.glob(r'*.*'):
+            shutil.copy(file, args.output)
+    elif args.import_json:
+        import_from_json(args.json, data)
+        extract.create_html(
+            data,
+            args.output,
+            args.template,
+            args.embedded,
+            args.offline,
+            args.size
         )
-        exit(2)
-
-    if os.path.isdir(args.media):
-        if os.path.isdir(f"{args.output}/{args.media}"):
-            print("Media directory already exists in output directory. Skipping...")
-        else:
-            if not args.move_media:
-                print("Copying media directory...")
-                shutil.copytree(args.media, f"{args.output}/WhatsApp")
-            else:
-                try:
-                    shutil.move(args.media, f"{args.output}/")
-                except PermissionError:
-                    print("Cannot remove original WhatsApp directory. "
-                        "Perhaps the directory is opened?")
 
-    if args.json:
+    if args.json and not args.import_json:
         if isinstance(data[next(iter(data))], ChatStore):
             data = {jik: chat.to_json() for jik, chat in data.items()}
         with open(args.json, "w") as f:
             data = json.dumps(data)
             print(f"\nWriting JSON file...({int(len(data)/1024/1024)}MB)")
             f.write(data)
     else:
```

### Comparing `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/data_model.py` & `whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/data_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,98 @@
+#!/usr/bin/python3
+
+import os
 from datetime import datetime
 from typing import Union
 
 
 class ChatStore():
-    def __init__(self, name=None):
+    def __init__(self, type, name=None, media=None):
         if name is not None and not isinstance(name, str):
             raise TypeError("Name must be a string or None")
         self.name = name
         self.messages = {}
+        self.type = type
+        if media is not None:
+            from Whatsapp_Chat_Exporter.utility import Device
+            if self.type == Device.IOS:
+                self.my_avatar = os.path.join(media, "Media/Profile/Photo.jpg")
+            elif self.type == Device.ANDROID:
+                self.my_avatar = None  # TODO: Add Android support
+            else:
+                self.my_avatar = None
+        else:
+            self.my_avatar = None
+        self.their_avatar = None
+        self.their_avatar_thumb = None
+        self.status = None
     
     def add_message(self, id, message):
         if not isinstance(message, Message):
-            raise TypeError("Chat must be a Chat object")
+            raise TypeError("message must be a Message object")
         self.messages[id] = message
 
     def delete_message(self, id):
         if id in self.messages:
             del self.messages[id]
 
     def to_json(self):
-        serialized_msgs = {id : msg.to_json() for id,msg in self.messages.items()}
-        return {'name' : self.name, 'messages' : serialized_msgs}
+        serialized_msgs = {id: msg.to_json() for id, msg in self.messages.items()}
+        return {
+            'name': self.name,
+            'type': self.type,
+            'my_avatar': self.my_avatar,
+            'their_avatar': self.their_avatar,
+            'their_avatar_thumb': self.their_avatar_thumb,
+            'status': self.status,
+            'messages': serialized_msgs
+        }
+
+    def get_last_message(self):
+        return tuple(self.messages.values())[-1]
+
+    def get_messages(self):
+        return self.messages.values()
+
 
 class Message():
-    def __init__(self, from_me: Union[bool,int], timestamp: int, time: str, key_id: int):
+    def __init__(self, from_me: Union[bool,int], timestamp: int, time: Union[int,float,str], key_id: int):
         self.from_me = bool(from_me)
         self.timestamp = timestamp / 1000 if timestamp > 9999999999 else timestamp
-        self.time = datetime.fromtimestamp(time/1000).strftime("%H:%M")
+        if isinstance(time, int) or isinstance(time, float):
+            self.time = datetime.fromtimestamp(time/1000).strftime("%H:%M")
+        elif isinstance(time, str):
+            self.time = time
+        else:
+            raise TypeError("Time must be a string or integer")
         self.media = False
         self.key_id = key_id
         self.meta = False
         self.data = None
         self.sender = None
+        self.safe = False
+        self.mime = None
         # Extra
         self.reply = None
         self.quoted_data = None
         self.caption = None
+        self.thumb = None # Android specific
+        self.sticker = False
     
     def to_json(self):
         return {
             'from_me'     : self.from_me,
             'timestamp'   : self.timestamp,
             'time'        : self.time,
             'media'       : self.media,
             'key_id'      : self.key_id,
             'meta'        : self.meta,
             'data'        : self.data,
             'sender'      : self.sender,
+            'safe'        : self.safe,
+            'mime'        : self.mime,
             'reply'       : self.reply,
             'quoted_data' : self.quoted_data,
-            'caption'     : self.caption
+            'caption'     : self.caption,
+            'thumb'       : self.thumb,
+            'sticker'     : self.sticker
         }
```

### Comparing `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract.py` & `whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/extract.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 import shutil
 import re
 import io
 import hmac
 from pathlib import Path
 from mimetypes import MimeTypes
 from hashlib import sha256
+from base64 import b64decode, b64encode
 from Whatsapp_Chat_Exporter.data_model import ChatStore, Message
-from Whatsapp_Chat_Exporter.utility import sanitize_except, determine_day, Crypt
+from Whatsapp_Chat_Exporter.utility import MAX_SIZE, ROW_SIZE, determine_metadata, get_status_location
+from Whatsapp_Chat_Exporter.utility import rendering, Crypt, Device, get_file_name, setup_template
 from Whatsapp_Chat_Exporter.utility import brute_force_offset, CRYPT14_OFFSETS
 
 try:
     import zlib
     from Crypto.Cipher import AES
 except ModuleNotFoundError:
     support_backup = False
@@ -45,15 +47,15 @@
 
 def _extract_encrypted_key(keyfile):
     key_stream = b""
     for byte in javaobj.loads(keyfile):
         key_stream += byte.to_bytes(1, "big", signed=True)
 
     return _generate_hmac_of_hmac(key_stream)
-    
+
 
 def decrypt_backup(database, key, output, crypt=Crypt.CRYPT14, show_crypt15=False):
     if not support_backup:
         return 1
     if isinstance(key, io.IOBase):
         key = key.read()
         if crypt is not Crypt.CRYPT15:
@@ -78,15 +80,15 @@
     elif crypt == Crypt.CRYPT15:
         if not support_crypt15:
             return 1
         if len(database) < 131:
             raise ValueError("The crypt15 file must be at least 131 bytes")
         t1 = t2 = None
         iv = database[8:24]
-        db_offset = database[0] + 2 # Skip protobuf + protobuf size and backup type
+        db_offset = database[0] + 2  # Skip protobuf + protobuf size and backup type
         db_ciphertext = database[db_offset:]
 
     if t1 != t2:
         raise ValueError("The signature of key file and backup file mismatch")
 
     if crypt == Crypt.CRYPT15:
         if len(key) == 32:
@@ -126,15 +128,15 @@
                             continue
                         else:
                             decompressed = True
                             print(
                                 f"The offsets of your IV and database are {start_iv} and "
                                 f"{start_db}, respectively. To include your offsets in the "
                                 "program, please report it by creating an issue on GitHub: "
-                                "https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues/new"
+                                "https://github.com/KnugiHK/Whatsapp-Chat-Exporter/discussions/47"
                             )
                             break
                     if not decompressed:
                         return 2
             else:
                 return 3
         else:
@@ -148,76 +150,105 @@
 
 
 def contacts(db, data):
     # Get contacts
     c = db.cursor()
     c.execute("""SELECT count() FROM wa_contacts""")
     total_row_number = c.fetchone()[0]
-    print(f"Gathering contacts...({total_row_number})")
+    print(f"Processing contacts...({total_row_number})")
 
-    c.execute("""SELECT jid, display_name FROM wa_contacts; """)
+    c.execute("""SELECT jid, COALESCE(display_name, wa_name) as display_name, status FROM wa_contacts; """)
     row = c.fetchone()
     while row is not None:
-        data[row["jid"]] = ChatStore(row["display_name"])
+        data[row["jid"]] = ChatStore(Device.ANDROID, row["display_name"])
+        if row["status"] is not None:
+            data[row["jid"]].status = row["status"]
         row = c.fetchone()
 
 
-def messages(db, data):
+def messages(db, data, media_folder):
     # Get message history
     c = db.cursor()
     try:
         c.execute("""SELECT count() FROM messages""")
     except sqlite3.OperationalError:
         c.execute("""SELECT count() FROM message""")
     total_row_number = c.fetchone()[0]
-    print(f"Gathering messages...(0/{total_row_number})", end="\r")
+    print(f"Processing messages...(0/{total_row_number})", end="\r")
 
     phone_number_re = re.compile(r"[0-9]+@s.whatsapp.net")
     try:
         c.execute("""SELECT messages.key_remote_jid,
                             messages._id,
                             messages.key_from_me,
                             messages.timestamp,
                             messages.data,
                             messages.status,
                             messages.edit_version,
                             messages.thumb_image,
                             messages.remote_resource,
-                            messages.media_wa_type,
+                            CAST(messages.media_wa_type as INTEGER) as media_wa_type,
                             messages.latitude,
                             messages.longitude,
                             messages_quotes.key_id as quoted,
                             messages.key_id,
                             messages_quotes.data as quoted_data,
-                            messages.media_caption
+                            messages.media_caption,
+							missed_call_logs.video_call,
+                            chat.subject as chat_subject,
+                            message_system.action_type,
+                            message_system_group.is_me_joined,
+                            jid_old.raw_string as old_jid,
+                            jid_new.raw_string as new_jid
                     FROM messages
                         LEFT JOIN messages_quotes
                             ON messages.quoted_row_id = messages_quotes._id
+						LEFT JOIN missed_call_logs
+							ON messages._id = missed_call_logs.message_row_id
+                        INNER JOIN jid jid_global
+                            ON messages.key_remote_jid = jid_global.raw_string
+                        LEFT JOIN chat
+                            ON chat.jid_row_id = jid_global._id
+                        LEFT JOIN message_system
+                            ON message_system.message_row_id = messages._id
+                        LEFT JOIN message_system_group
+                            ON message_system_group.message_row_id = messages._id
+                        LEFT JOIN message_system_number_change
+                            ON message_system_number_change.message_row_id = messages._id
+                        LEFT JOIN jid jid_old
+                            ON jid_old._id = message_system_number_change.old_jid_row_id
+                        LEFT JOIN jid jid_new
+                            ON jid_new._id = message_system_number_change.new_jid_row_id
                     WHERE messages.key_remote_jid <> '-1';"""
         )
     except sqlite3.OperationalError:
         try:
             c.execute("""SELECT jid_global.raw_string as key_remote_jid,
                             message._id,
                             message.from_me as key_from_me,
                             message.timestamp,
                             message.text_data as data,
                             message.status,
                             message_future.version as edit_version,
                             message_thumbnail.thumbnail as thumb_image,
                             message_media.file_path as remote_resource,
-                            message_media.mime_type as media_wa_type,
                             message_location.latitude,
                             message_location.longitude,
                             message_quoted.key_id as quoted,
                             message.key_id,
                             message_quoted.text_data as quoted_data,
-                            message.message_type,
+                            message.message_type as media_wa_type,
                             jid_group.raw_string as group_sender_jid,
-                            chat.subject as chat_subject
+                            chat.subject as chat_subject,
+							missed_call_logs.video_call,
+                            message.sender_jid_row_id,
+                            message_system.action_type,
+                            message_system_group.is_me_joined,
+                            jid_old.raw_string as old_jid,
+                            jid_new.raw_string as new_jid
                     FROM message
                         LEFT JOIN message_quoted
                             ON message_quoted.message_row_id = message._id
                         LEFT JOIN message_location
                             ON message_location.message_row_id = message._id
                         LEFT JOIN message_media
                             ON message_media.message_row_id = message._id
@@ -227,234 +258,278 @@
                             ON message_future.message_row_id = message._id
                         LEFT JOIN chat
                             ON chat._id = message.chat_row_id
                         INNER JOIN jid jid_global
                             ON jid_global._id = chat.jid_row_id
                         LEFT JOIN jid jid_group
                             ON jid_group._id = message.sender_jid_row_id
+						LEFT JOIN missed_call_logs
+							ON message._id = missed_call_logs.message_row_id
+                        LEFT JOIN message_system
+                            ON message_system.message_row_id = message._id
+                        LEFT JOIN message_system_group
+                            ON message_system_group.message_row_id = message._id
+                        LEFT JOIN message_system_number_change
+                            ON message_system_number_change.message_row_id = message._id
+                        LEFT JOIN jid jid_old
+                            ON jid_old._id = message_system_number_change.old_jid_row_id
+                        LEFT JOIN jid jid_new
+                            ON jid_new._id = message_system_number_change.new_jid_row_id
                         WHERE key_remote_jid <> '-1';"""
             )
         except Exception as e:
             raise e
         else:
             table_message = True
     else:
         table_message = False
     i = 0
-    content = c.fetchone()
+    while True:
+        try:
+            content = c.fetchone()
+        except sqlite3.OperationalError:
+            continue
+        else:
+            break
     while content is not None:
         if content["key_remote_jid"] not in data:
-            data[content["key_remote_jid"]] = ChatStore()
+            data[content["key_remote_jid"]] = ChatStore(Device.ANDROID, content["chat_subject"])
         if content["key_remote_jid"] is None:
-            continue # Not sure
-        data[content["key_remote_jid"]].add_message(content["_id"], Message(
-            from_me=content["key_from_me"],
+            continue  # Not sure
+        if "sender_jid_row_id" in content:
+            sender_jid_row_id = content["sender_jid_row_id"]
+        else:
+            sender_jid_row_id = None
+        message = Message(
+            from_me=not sender_jid_row_id and content["key_from_me"],
             timestamp=content["timestamp"],
             time=content["timestamp"],
             key_id=content["key_id"],
-        ))    
+        )
+        if isinstance(content["data"], bytes):
+            message.data = ("The message is binary data and its base64 is "
+                '<a href="https://gchq.github.io/CyberChef/#recipe=From_Base64'
+                "('A-Za-z0-9%2B/%3D',true,false)Text_Encoding_Brute_Force"
+                f"""('Decode')&input={b64encode(b64encode(content["data"])).decode()}">""")
+            message.data += b64encode(content["data"]).decode("utf-8") + "</a>"
+            message.safe = message.meta = True
+            data[content["key_remote_jid"]].add_message(content["_id"], message)
+            i += 1
+            content = c.fetchone()
+            continue
         if "-" in content["key_remote_jid"] and content["key_from_me"] == 0:
-            name = None
+            name = fallback = None
             if table_message:
-                if content["chat_subject"] is not None:
+                if content["sender_jid_row_id"] > 0:
                     _jid = content["group_sender_jid"]
-                else:
-                    _jid = content["key_remote_jid"]
-                if _jid in data:
-                    name = data[_jid].name
-                    fallback = _jid.split('@')[0] if "@" in _jid else None
-                else:
-                    fallback = None
+                    if _jid in data:
+                        name = data[_jid].name
+                    if "@" in _jid:
+                        fallback = _jid.split('@')[0]
             else:
-                if content["remote_resource"] in data:
-                    name = data[content["remote_resource"]].name
+                if content["remote_resource"] is not None:
+                    if content["remote_resource"] in data:
+                        name = data[content["remote_resource"]].name
                     if "@" in content["remote_resource"]:
                         fallback = content["remote_resource"].split('@')[0]
-                    else:
-                        fallback = None
-                else:
-                    fallback = None
 
-            data[content["key_remote_jid"]].messages[content["_id"]].sender = name or fallback
+            message.sender = name or fallback
         else:
-            data[content["key_remote_jid"]].messages[content["_id"]].sender = None
+            message.sender = None
 
         if content["quoted"] is not None:
-            data[content["key_remote_jid"]].messages[content["_id"]].reply = content["quoted"]
-            data[content["key_remote_jid"]].messages[content["_id"]].quoted_data = content["quoted_data"]
+            message.reply = content["quoted"]
+            if content["quoted_data"] is not None and len(content["quoted_data"]) > 200:
+                message.quoted_data = content["quoted_data"][:201] + "..."
+            else:
+                message.quoted_data = content["quoted_data"]
         else:
-            data[content["key_remote_jid"]].messages[content["_id"]].reply = None
+            message.reply = None
 
         if not table_message and content["media_caption"] is not None:
             # Old schema
-            data[content["key_remote_jid"]].messages[content["_id"]].caption = content["media_caption"]
-        elif table_message and content["message_type"] == 1 and content["data"] is not None:
+            message.caption = content["media_caption"]
+        elif table_message and content["media_wa_type"] == 1 and content["data"] is not None:
             # New schema
-            data[content["key_remote_jid"]].messages[content["_id"]].caption = content["data"]
+            message.caption = content["data"]
         else:
-            data[content["key_remote_jid"]].messages[content["_id"]].caption = None
+            message.caption = None
 
-        if content["status"] == 6:  # 6 = Metadata, otherwise it's a message
-            if (not table_message and "-" in content["key_remote_jid"]) or \
-               (table_message and content["chat_subject"] is not None):
-                # Is Group
-                if content["data"] is not None:
-                    try:
-                        int(content["data"])
-                    except ValueError:
-                        msg = f"The group name changed to {content['data']}"
-                        data[content["key_remote_jid"]].messages[content["_id"]].data = msg
-                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
-                    else:
-                        data[content["key_remote_jid"]].delete_message(content["_id"])
+        if content["status"] == 6:  # 6 = Metadata, otherwise assume a message
+            message.meta = True
+            name = fallback = None
+            if table_message:
+                if content["sender_jid_row_id"] > 0:
+                    _jid = content["group_sender_jid"]
+                    if _jid in data:
+                        name = data[_jid].name
+                    if "@" in _jid:
+                        fallback = _jid.split('@')[0]
                 else:
-                    thumb_image = content["thumb_image"]
-                    if thumb_image is not None:
-                        if b"\x00\x00\x01\x74\x00\x1A" in thumb_image:
-                            # Add user
-                            added = phone_number_re.search(
-                                thumb_image.decode("unicode_escape"))[0]
-                            if added in data:
-                                name_right = data[added].name
-                            else:
-                                name_right = added.split('@')[0]
-                            if content["remote_resource"] is not None:
-                                if content["remote_resource"] in data:
-                                    name_left = data[content["remote_resource"]].name
-                                else:
-                                    name_left = content["remote_resource"].split('@')[0]
-                                msg = f"{name_left} added {name_right or 'You'}"
-                            else:
-                                msg = f"Added {name_right or 'You'}"
-                        elif b"\xac\xed\x00\x05\x74\x00" in thumb_image:
-                            # Changed number
-                            original = content["remote_resource"].split('@')[0]
-                            changed = thumb_image[7:].decode().split('@')[0]
-                            msg = f"{original} changed to {changed}"
-                        data[content["key_remote_jid"]].messages[content["_id"]].data = msg
-                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
-                    else:
-                        if content["data"] is None:
-                            data[content["key_remote_jid"]].delete_message(content["_id"])
+                    name = "You"
             else:
-                # Private chat
-                if content["data"] is None and content["thumb_image"] is None:
-                    data[content["key_remote_jid"]].delete_message(content["_id"])
-
-        else:
+                _jid = content["remote_resource"]
+                if _jid is not None:
+                    if _jid in data:
+                        name = data[_jid].name
+                    if "@" in _jid:
+                        fallback = _jid.split('@')[0]
+                else:
+                    name = "You"
+            message.data = determine_metadata(content, name or fallback)
+            if isinstance(message.data, str) and "<br>" in message.data:
+                message.safe = True
+            if message.data is None:
+                if content["video_call"] is not None:  # Missed call
+                    message.meta = True
+                    if content["video_call"] == 1:
+                        message.data = "A video call was missed"
+                    elif content["video_call"] == 0:
+                        message.data = "A voice call was missed"
+                elif content["data"] is None and content["thumb_image"] is None:
+                    message.meta = True
+                    message.data = None
+        else:
+            # Real message
+            if content["media_wa_type"] == 20: # Sticker is a message
+                message.sticker = True
             if content["key_from_me"] == 1:
-                if content["status"] == 5 and content["edit_version"] == 7 or table_message and content["message_type"] == 15:
+                if content["status"] == 5 and content["edit_version"] == 7 or table_message and content["media_wa_type"] == 15:
                     msg = "Message deleted"
-                    data[content["key_remote_jid"]].messages[content["_id"]].meta = True
+                    message.meta = True
                 else:
-                    if content["media_wa_type"] == "5":
+                    if content["media_wa_type"] == 5:
                         msg = f"Location shared: {content['latitude'], content['longitude']}"
-                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
+                        message.meta = True
                     else:
                         msg = content["data"]
                         if msg is not None:
                             if "\r\n" in msg:
                                 msg = msg.replace("\r\n", "<br>")
                             if "\n" in msg:
                                 msg = msg.replace("\n", "<br>")
             else:
-                if content["status"] == 0 and content["edit_version"] == 7 or table_message and content["message_type"] == 15:
+                if content["status"] == 0 and content["edit_version"] == 7 or table_message and content["media_wa_type"] == 15:
                     msg = "Message deleted"
-                    data[content["key_remote_jid"]].messages[content["_id"]].meta = True
+                    message.meta = True
                 else:
-                    if content["media_wa_type"] == "5":
+                    if content["media_wa_type"] == 5:
                         msg = f"Location shared: {content['latitude'], content['longitude']}"
-                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
+                        message.meta = True
                     else:
                         msg = content["data"]
                         if msg is not None:
                             if "\r\n" in msg:
                                 msg = msg.replace("\r\n", "<br>")
                             if "\n" in msg:
                                 msg = msg.replace("\n", "<br>")
+            message.data = msg
 
-            data[content["key_remote_jid"]].messages[content["_id"]].data = msg
-
+        data[content["key_remote_jid"]].add_message(content["_id"], message)
         i += 1
         if i % 1000 == 0:
-            print(f"Gathering messages...({i}/{total_row_number})", end="\r")
-        content = c.fetchone()
-    print(f"Gathering messages...({total_row_number}/{total_row_number})", end="\r")
+            print(f"Processing messages...({i}/{total_row_number})", end="\r")
+        while True:
+            try:
+                content = c.fetchone()
+            except sqlite3.OperationalError:
+                continue
+            else:
+                break
+    print(f"Processing messages...({total_row_number}/{total_row_number})", end="\r")
 
 
 def media(db, data, media_folder):
     # Get media
     c = db.cursor()
     c.execute("""SELECT count() FROM message_media""")
     total_row_number = c.fetchone()[0]
-    print(f"\nGathering media...(0/{total_row_number})", end="\r")
+    print(f"\nProcessing media...(0/{total_row_number})", end="\r")
     i = 0
     try:
         c.execute("""SELECT messages.key_remote_jid,
                         message_row_id,
                         file_path,
                         message_url,
                         mime_type,
-                        media_key
+                        media_key,
+                        file_hash,
+						thumbnail
                  FROM message_media
                     INNER JOIN messages
                         ON message_media.message_row_id = messages._id
+					LEFT JOIN media_hash_thumbnail
+						ON message_media.file_hash = media_hash_thumbnail.media_hash
                 ORDER BY messages.key_remote_jid ASC"""
         )
     except sqlite3.OperationalError:
         c.execute("""SELECT jid.raw_string as key_remote_jid,
                     message_row_id,
                     file_path,
                     message_url,
                     mime_type,
-                    media_key
+                    media_key,
+                    file_hash,
+                    thumbnail
                 FROM message_media
                 INNER JOIN message
                     ON message_media.message_row_id = message._id
                 LEFT JOIN chat
                     ON chat._id = message.chat_row_id
                 INNER JOIN jid
                     ON jid._id = chat.jid_row_id
+                LEFT JOIN media_hash_thumbnail
+						ON message_media.file_hash = media_hash_thumbnail.media_hash
                 ORDER BY jid.raw_string ASC"""
         )
     content = c.fetchone()
     mime = MimeTypes()
+    if not os.path.isdir(f"{media_folder}/thumbnails"):
+        Path(f"{media_folder}/thumbnails").mkdir(parents=True, exist_ok=True)
     while content is not None:
         file_path = f"{media_folder}/{content['file_path']}"
-        data[content["key_remote_jid"]].messages[content["message_row_id"]].media = True
+        message = data[content["key_remote_jid"]].messages[content["message_row_id"]]
+        message.media = True
         if os.path.isfile(file_path):
-            data[content["key_remote_jid"]].messages[content["message_row_id"]].data = file_path
+            message.data = file_path
             if content["mime_type"] is None:
                 guess = mime.guess_type(file_path)[0]
                 if guess is not None:
-                    data[content["key_remote_jid"]].messages[content["message_row_id"]].mime = guess
+                    message.mime = guess
                 else:
-                    data[content["key_remote_jid"]].messages[content["message_row_id"]].mime = "data/data"
+                    message.mime = "application/octet-stream"
             else:
-                data[content["key_remote_jid"]].messages[content["message_row_id"]].mime = content["mime_type"]
+                message.mime = content["mime_type"]
         else:
-            # if "https://mmg" in content[4]:
-            # try:
-            # r = requests.get(content[3])
-            # if r.status_code != 200:
-            # raise RuntimeError()
-            # except:
-            # data[content[0]]["messages"][content[1]]["data"] = "{The media is missing}"
-            # data[content[0]]["messages"][content[1]]["media"] = True
-            # data[content[0]]["messages"][content[1]]["mime"] = "media"
-            # else:
-            data[content["key_remote_jid"]].messages[content["message_row_id"]].data = "The media is missing"
-            data[content["key_remote_jid"]].messages[content["message_row_id"]].mime = "media"
-            data[content["key_remote_jid"]].messages[content["message_row_id"]].meta = True
+            if False: # Block execution
+                try:
+                    r = requests.get(content["message_url"])
+                    if r.status_code != 200:
+                        raise RuntimeError()
+                except:
+                    message.data = "The media is missing"
+                    message.mime = "media"
+                    message.meta = True
+                else:
+                    ...
+            message.data = "The media is missing"
+            message.mime = "media"
+            message.meta = True
+        if content["thumbnail"] is not None:
+            thumb_path = f"{media_folder}/thumbnails/{b64decode(content['file_hash']).hex()}.png"
+            if not os.path.isfile(thumb_path):
+                with open(thumb_path, "wb") as f:
+                    f.write(content["thumbnail"])
+            message.thumb = thumb_path
         i += 1
         if i % 100 == 0:
-            print(f"Gathering media...({i}/{total_row_number})", end="\r")
+            print(f"Processing media...({i}/{total_row_number})", end="\r")
         content = c.fetchone()
     print(
-        f"Gathering media...({total_row_number}/{total_row_number})", end="\r")
+        f"Processing media...({total_row_number}/{total_row_number})", end="\r")
 
 
 def vcard(db, data):
     c = db.cursor()
     try:
         c.execute("""SELECT message_row_id,
                         messages.key_remote_jid,
@@ -475,157 +550,172 @@
                         ON message_vcard.message_row_id = message._id
                     LEFT JOIN chat
                         ON chat._id = message.chat_row_id
                     INNER JOIN jid
                         ON jid._id = chat.jid_row_id
                  ORDER BY message.chat_row_id ASC;"""
         )
-    
+
     rows = c.fetchall()
     total_row_number = len(rows)
-    print(f"\nGathering vCards...(0/{total_row_number})", end="\r")
+    print(f"\nProcessing vCards...(0/{total_row_number})", end="\r")
     base = "WhatsApp/vCards"
     if not os.path.isdir(base):
         Path(base).mkdir(parents=True, exist_ok=True)
     for index, row in enumerate(rows):
         media_name = row["media_name"] if row["media_name"] is not None else ""
         file_name = "".join(x for x in media_name if x.isalnum())
-        file_path = f"{base}/{file_name}.vcf"
+        file_name = file_name.encode('utf-8')[:230].decode('utf-8', 'ignore')
+        file_path = os.path.join(base, f"{file_name}.vcf")
         if not os.path.isfile(file_path):
             with open(file_path, "w", encoding="utf-8") as f:
                 f.write(row["vcard"])
-        data[row["key_remote_jid"]].messages[row["message_row_id"]].data = media_name + \
+        message = data[row["key_remote_jid"]].messages[row["message_row_id"]]
+        message.data = media_name + \
             "The vCard file cannot be displayed here, " \
             f"however it should be located at {file_path}"
-        data[row["key_remote_jid"]].messages[row["message_row_id"]].mime = "text/x-vcard"
-        data[row["key_remote_jid"]].messages[row["message_row_id"]].meta = True
-        print(f"Gathering vCards...({index + 1}/{total_row_number})", end="\r")
+        message.mime = "text/x-vcard"
+        message.meta = True
+        print(f"Processing vCards...({index + 1}/{total_row_number})", end="\r")
+
+
+def calls(db, data):
+    c = db.cursor()
+    c.execute("""SELECT count() FROM call_log""")
+    total_row_number = c.fetchone()[0]
+    if total_row_number == 0:
+        return
+    print(f"\nProcessing calls...({total_row_number})", end="\r")
+    c.execute("""SELECT call_log._id,
+                        jid.raw_string,
+                        from_me,
+                        call_id,
+                        timestamp,
+                        video_call,
+                        duration,
+                        call_result,
+                        bytes_transferred
+                FROM call_log
+                    INNER JOIN jid
+                        ON call_log.jid_row_id = jid._id"""
+    )
+    chat = ChatStore(Device.ANDROID, "WhatsApp Calls")
+    content = c.fetchone()
+    while content is not None:
+        call = Message(
+            from_me=content["from_me"],
+            timestamp=content["timestamp"],
+            time=content["timestamp"],
+            key_id=content["call_id"],
+        )
+        _jid = content["raw_string"]
+        if _jid in data:
+            name = data[_jid].name
+            fallback = _jid.split('@')[0] if "@" in _jid else None
+            call.sender = name or fallback
+
+        call.meta = True
+        call.data = (
+            f"A {'video' if content['video_call'] else 'voice'} "
+            f"call {'to' if call.from_me else 'from'} "
+            f"{name or fallback} was "
+        )
+        if content['call_result'] == 2:
+            call.data += "not answered." if call.from_me else "missed."
+        elif content['call_result'] == 3:
+            call.data += "unavailable."
+        elif content['call_result'] == 5:
+            call.data += (
+                f"initiated and lasted for {content['duration']} second(s) "
+                f"with {content['bytes_transferred']} bytes transferred."
+            )
+        chat.add_message(content["_id"], call)
+        content = c.fetchone()
+    data["000000000000000"] = chat
 
 
 def create_html(
         data,
         output_folder,
         template=None,
         embedded=False,
         offline_static=False,
-        maximum_size=None
+        maximum_size=None,
+        no_avatar=False
     ):
-    if template is None:
-        template_dir = os.path.dirname(__file__)
-        template_file = "whatsapp.html"
-    else:
-        template_dir = os.path.dirname(template)
-        template_file = os.path.basename(template)
-    templateLoader = jinja2.FileSystemLoader(searchpath=template_dir)
-    templateEnv = jinja2.Environment(loader=templateLoader)
-    templateEnv.globals.update(determine_day=determine_day)
-    templateEnv.filters['sanitize_except'] = sanitize_except
-    template = templateEnv.get_template(template_file)
+    template = setup_template(template, no_avatar)
 
     total_row_number = len(data)
-    print(f"\nCreating HTML...(0/{total_row_number})", end="\r")
+    print(f"\nGenerating chats...(0/{total_row_number})", end="\r")
 
     if not os.path.isdir(output_folder):
         os.mkdir(output_folder)
 
-    w3css = "https://www.w3schools.com/w3css/4/w3.css"
-    if offline_static:
-        import urllib.request
-        static_folder = os.path.join(output_folder, offline_static)
-        if not os.path.isdir(static_folder):
-            os.mkdir(static_folder)
-        w3css_path = os.path.join(static_folder, "w3.css")
-        if not os.path.isfile(w3css_path):
-            with urllib.request.urlopen(w3css) as resp:
-                with open(w3css_path, "wb") as f:
-                    f.write(resp.read())
-        w3css = os.path.join(offline_static, "w3.css")
+    w3css = get_status_location(output_folder, offline_static)
 
     for current, contact in enumerate(data):
-        if len(data[contact].messages) == 0:
+        chat = data[contact]
+        if len(chat.messages) == 0:
             continue
-        phone_number = contact.split('@')[0]
-        if "-" in contact:
-            file_name = ""
-        else:
-            file_name = phone_number
-
-        if data[contact].name is not None:
-            if file_name != "":
-                file_name += "-"
-            file_name += data[contact].name.replace("/", "-")
-            name = data[contact].name
-        else:
-            name = phone_number
-        safe_file_name = ''
-        safe_file_name = "".join(x for x in file_name if x.isalnum() or x in "- ")
-        with open(f"{output_folder}/{safe_file_name}.html", "w", encoding="utf-8") as f:
-            f.write(
-                template.render(
-                    name=name,
-                    msgs=data[contact].messages.values(),
-                    my_avatar=None,
-                    their_avatar=f"WhatsApp/Avatars/{contact}.j",
-                    w3css=w3css
-                )
+        safe_file_name, name = get_file_name(contact, chat)
+
+        if maximum_size is not None:
+            current_size = 0
+            current_page = 1
+            render_box = []
+            if maximum_size == 0:
+                maximum_size = MAX_SIZE
+            last_msg = chat.get_last_message().key_id
+            for message in chat.get_messages():
+                if message.data is not None and not message.meta and not message.media:
+                    current_size += len(message.data) + ROW_SIZE
+                else:
+                    current_size += ROW_SIZE + 100  # Assume media and meta HTML are 100 bytes
+                if current_size > maximum_size:
+                    output_file_name = f"{output_folder}/{safe_file_name}-{current_page}.html"
+                    rendering(
+                        output_file_name,
+                        template,
+                        name,
+                        render_box,
+                        contact,
+                        w3css,
+                        f"{safe_file_name}-{current_page + 1}.html",
+                        chat
+                    )
+                    render_box = [message]
+                    current_size = 0
+                    current_page += 1
+                else:
+                    if message.key_id == last_msg:
+                        if current_page == 1:
+                            output_file_name = f"{output_folder}/{safe_file_name}.html"
+                        else:
+                            output_file_name = f"{output_folder}/{safe_file_name}-{current_page}.html"
+                        rendering(
+                            output_file_name,
+                            template,
+                            name,
+                            render_box,
+                            contact,
+                            w3css,
+                            False,
+                            chat
+                        )
+                    else:
+                        render_box.append(message)
+        else:
+            output_file_name = f"{output_folder}/{safe_file_name}.html"
+            rendering(
+                output_file_name,
+                template,
+                name,
+                chat.get_messages(),
+                contact,
+                w3css,
+                False,
+                chat
             )
         if current % 10 == 0:
-            print(f"Creating HTML...({current}/{total_row_number})", end="\r")
-
-    print(f"Creating HTML...({total_row_number}/{total_row_number})", end="\r")
-
-
-if __name__ == "__main__":
-    from optparse import OptionParser
-    parser = OptionParser()
-    parser.add_option(
-        "-w",
-        "--wa",
-        dest="wa",
-        default="wa.db",
-        help="Path to contact database")
-    parser.add_option(
-        "-m",
-        "--media",
-        dest="media",
-        default="WhatsApp",
-        help="Path to WhatsApp media folder"
-    )
-    # parser.add_option(
-    #     "-t",
-    #     "--template",
-    #     dest="html",
-    #     default="wa.db",
-    #     help="Path to HTML template")
-    (options, args) = parser.parse_args()
-    msg_db = "msgstore.db"
-    output_folder = "temp"
-    contact_db = options.wa
-    media_folder = options.media
-
-    if len(args) == 1:
-        msg_db = args[0]
-    elif len(args) == 2:
-        msg_db = args[0]
-        output_folder = args[1]
-
-    data = {}
-
-    if os.path.isfile(contact_db):
-        with sqlite3.connect(contact_db) as db:
-            contacts(db, data)
-    if os.path.isfile(msg_db):
-        with sqlite3.connect(msg_db) as db:
-            messages(db, data)
-            media(db, data, media_folder)
-            vcard(db, data)
-        create_html(data, output_folder)
-
-    if not os.path.isdir(f"{output_folder}/WhatsApp"):
-        shutil.move(media_folder, f"{output_folder}/")
-
-    with open("result.json", "w") as f:
-        data = json.dumps(data)
-        print(f"\nWriting JSON file...({int(len(data)/1024/1024)}MB)")
-        f.write(data)
+            print(f"Generating chats...({current}/{total_row_number})", end="\r")
 
-    print("Everything is done!")
+    print(f"Generating chats...({total_row_number}/{total_row_number})", end="\r")
```

### Comparing `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone.py` & `whatsapp-chat-exporter-0.9.5/Whatsapp_Chat_Exporter/utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,332 +1,292 @@
-#!/usr/bin/python3
-
-import sqlite3
-import json
 import jinja2
+import json
 import os
-import shutil
-from pathlib import Path
+from bleach import clean as sanitize
+from markupsafe import Markup
 from datetime import datetime
-from mimetypes import MimeTypes
-from Whatsapp_Chat_Exporter.utility import sanitize_except, determine_day, APPLE_TIME
+from enum import IntEnum
+from Whatsapp_Chat_Exporter.data_model import ChatStore
+try:
+    from enum import StrEnum
+except ImportError:
+    # < Python 3.11
+    from enum import Enum
+    class StrEnum(str, Enum):
+        pass
+
+
+MAX_SIZE = 4 * 1024 * 1024  # Default 4MB
+ROW_SIZE = 0x3D0
+
+
+def sanitize_except(html):
+    return Markup(sanitize(html, tags=["br"]))
+
+
+def determine_day(last, current):
+    last = datetime.fromtimestamp(last).date()
+    current = datetime.fromtimestamp(current).date()
+    if last == current:
+        return None
+    else:
+        return current
 
 
-def messages(db, data):
-    c = db.cursor()
-    # Get contacts
-    c.execute("""SELECT count() FROM ZWACHATSESSION""")
-    total_row_number = c.fetchone()[0]
-    print(f"Gathering contacts...({total_row_number})")
-
-    c.execute("""SELECT ZCONTACTJID, ZPARTNERNAME FROM ZWACHATSESSION; """)
-    row = c.fetchone()
-    while row is not None:
-        data[row[0]] = {"name": row[1], "messages": {}}
-        row = c.fetchone()
-
-    # Get message history
-    c.execute("""SELECT count() FROM ZWAMESSAGE""")
-    total_row_number = c.fetchone()[0]
-    print(f"Gathering messages...(0/{total_row_number})", end="\r")
-
-    c.execute("""SELECT COALESCE(ZFROMJID, ZTOJID),
-                        ZWAMESSAGE.Z_PK,
-                        ZISFROMME,
-                        ZMESSAGEDATE,
-                        ZTEXT,
-                        ZMESSAGETYPE,
-                        ZWAGROUPMEMBER.ZMEMBERJID
-                 FROM main.ZWAMESSAGE
-                    LEFT JOIN main.ZWAGROUPMEMBER
-                        ON main.ZWAMESSAGE.ZGROUPMEMBER = main.ZWAGROUPMEMBER.Z_PK;""")
-    i = 0
-    content = c.fetchone()
-    while content is not None:
-        if content[0] not in data:
-            data[content[0]] = {"name": None, "messages": {}}
-        ts = APPLE_TIME + content[3]
-        data[content[0]]["messages"][content[1]] = {
-            "from_me": bool(content[2]),
-            "timestamp": ts,
-            "time": datetime.fromtimestamp(ts).strftime("%H:%M"),
-            "media": False,
-            "reply": None,
-            "caption": None,
-            "meta": False,
-            "data": None
-        }
-        if "-" in content[0] and content[2] == 0:
-            name = None
-            if content[6] is not None:
-                if content[6] in data:
-                    name = data[content[6]]["name"]
-                if "@" in content[6]:
-                    fallback = content[6].split('@')[0]
-                else:
-                    fallback = None
-            else:
-                fallback = None
-            data[content[0]]["messages"][content[1]]["sender"] = name or fallback
-        else:
-            data[content[0]]["messages"][content[1]]["sender"] = None
-        if content[5] == 6:
-            # Metadata
-            if "-" in content[0]:
-                # Group
-                if content[4] is not None:
-                    # Chnaged name
-                    try:
-                        int(content[4])
-                    except ValueError:
-                        msg = f"The group name changed to {content[4]}"
-                        data[content[0]]["messages"][content[1]]["data"] = msg
-                        data[content[0]]["messages"][content[1]]["meta"] = True
-                    else:
-                        del data[content[0]]["messages"][content[1]]
-                else:
-                    data[content[0]]["messages"][content[1]]["data"] = None
-            else:
-                data[content[0]]["messages"][content[1]]["data"] = None
-        else:
-            # real message
-            if content[2] == 1:
-                if content[5] == 14:
-                    msg = "Message deleted"
-                    data[content[0]]["messages"][content[1]]["meta"] = True
-                else:
-                    msg = content[4]
-                    if msg is not None:
-                        if "\r\n" in msg:
-                            msg = msg.replace("\r\n", "<br>")
-                        if "\n" in msg:
-                            msg = msg.replace("\n", "<br>")
-            else:
-                if content[5] == 14:
-                    msg = "Message deleted"
-                    data[content[0]]["messages"][content[1]]["meta"] = True
-                else:
-                    msg = content[4]
-                    if msg is not None:
-                        if "\r\n" in msg:
-                            msg = msg.replace("\r\n", "<br>")
-                        if "\n" in msg:
-                            msg = msg.replace("\n", "<br>")
-            data[content[0]]["messages"][content[1]]["data"] = msg
-        i += 1
-        if i % 1000 == 0:
-            print(f"Gathering messages...({i}/{total_row_number})", end="\r")
-        content = c.fetchone()
-    print(
-        f"Gathering messages...({total_row_number}/{total_row_number})", end="\r")
-
-
-def media(db, data, media_folder):
-    c = db.cursor()
-    # Get media
-    c.execute("""SELECT count() FROM ZWAMEDIAITEM""")
-    total_row_number = c.fetchone()[0]
-    print(f"\nGathering media...(0/{total_row_number})", end="\r")
-    i = 0
-    c.execute("""SELECT COALESCE(ZWAMESSAGE.ZFROMJID, ZWAMESSAGE.ZTOJID) as _id,
-                        ZMESSAGE,
-                        ZMEDIALOCALPATH,
-                        ZMEDIAURL,
-                        ZVCARDSTRING,
-                        ZMEDIAKEY,
-                        ZTITLE
-                 FROM ZWAMEDIAITEM
-                    INNER JOIN ZWAMESSAGE
-                        ON ZWAMEDIAITEM.ZMESSAGE = ZWAMESSAGE.Z_PK
-                 WHERE ZMEDIALOCALPATH IS NOT NULL
-                 ORDER BY _id ASC""")
-    content = c.fetchone()
-    mime = MimeTypes()
-    while content is not None:
-        file_path = f"{media_folder}/{content[2]}"
-        data[content[0]]["messages"][content[1]]["media"] = True
-
-        if os.path.isfile(file_path):
-            data[content[0]]["messages"][content[1]]["data"] = file_path
-            if content[4] is None:
-                guess = mime.guess_type(file_path)[0]
-                if guess is not None:
-                    data[content[0]]["messages"][content[1]]["mime"] = guess
+def check_update():
+    import urllib.request
+    import json
+    from sys import platform
+    from .__init__ import __version__
+
+    package_url_json = "https://pypi.org/pypi/whatsapp-chat-exporter/json"
+    try:
+        raw = urllib.request.urlopen(package_url_json)
+    except Exception:
+        print("Failed to check for updates.")
+        return 1
+    else:
+        with raw:
+            package_info = json.load(raw)
+            latest_version = tuple(map(int, package_info["info"]["version"].split(".")))
+            current_version = tuple(map(int, __version__.split(".")))
+            if current_version < latest_version:
+                print("===============Update===============")
+                print("A newer version of WhatsApp Chat Exporter is available.")
+                print("Current version: " + __version__)
+                print("Latest version: " + package_info["info"]["version"])
+                if platform == "win32":
+                    print("Update with: pip install --upgrade whatsapp-chat-exporter")
                 else:
-                    data[content[0]]["messages"][content[1]]["mime"] = "data/data"
+                    print("Update with: pip3 install --upgrade whatsapp-chat-exporter")
+                print("====================================")
             else:
-                data[content[0]]["messages"][content[1]]["mime"] = content[4]
-        else:
-            # if "https://mmg" in content[4]:
-            # try:
-            # r = requests.get(content[3])
-            # if r.status_code != 200:
-            # raise RuntimeError()
-            # except:
-            # data[content[0]]["messages"][content[1]]["data"] = "{The media is missing}"
-            # data[content[0]]["messages"][content[1]]["mime"] = "media"
-            # else:
-            data[content[0]]["messages"][content[1]]["data"] = "The media is missing"
-            data[content[0]]["messages"][content[1]]["mime"] = "media"
-            data[content[0]]["messages"][content[1]]["meta"] = True
-        if content[6] is not None:
-            data[content[0]]["messages"][content[1]]["caption"] = content[6]
-        i += 1
-        if i % 100 == 0:
-            print(f"Gathering media...({i}/{total_row_number})", end="\r")
-        content = c.fetchone()
-    print(
-        f"Gathering media...({total_row_number}/{total_row_number})", end="\r")
-
-
-def vcard(db, data):
-    c = db.cursor()
-    c.execute("""SELECT DISTINCT ZWAVCARDMENTION.ZMEDIAITEM,
-                        ZWAMEDIAITEM.ZMESSAGE,
-                        COALESCE(ZWAMESSAGE.ZFROMJID,
-                        ZWAMESSAGE.ZTOJID) as _id,
-                        ZVCARDNAME,
-                        ZVCARDSTRING
-                 FROM ZWAVCARDMENTION
-                    INNER JOIN ZWAMEDIAITEM
-                        ON ZWAVCARDMENTION.ZMEDIAITEM = ZWAMEDIAITEM.Z_PK
-                    INNER JOIN ZWAMESSAGE
-                        ON ZWAMEDIAITEM.ZMESSAGE = ZWAMESSAGE.Z_PK""")
-    rows = c.fetchall()
-    total_row_number = len(rows)
-    print(f"\nGathering vCards...(0/{total_row_number})", end="\r")
-    base = "Message/vCards"
-    if not os.path.isdir(base):
-        Path(base).mkdir(parents=True, exist_ok=True)
-    for index, row in enumerate(rows):
-        file_name = "".join(x for x in row[3] if x.isalnum())
-        file_path = f"{base}/{file_name[:200]}.vcf"
-        if not os.path.isfile(file_path):
-            with open(file_path, "w", encoding="utf-8") as f:
-                f.write(row[4])
-        data[row[2]]["messages"][row[1]]["data"] = row[3] + \
-            "The vCard file cannot be displayed here, " \
-            f"however it should be located at {file_path}"
-        data[row[2]]["messages"][row[1]]["mime"] = "text/x-vcard"
-        data[row[2]]["messages"][row[1]]["media"] = True
-        data[row[2]]["messages"][row[1]]["meta"] = True
-        print(f"Gathering vCards...({index + 1}/{total_row_number})", end="\r")
+                print("You are using the latest version of WhatsApp Chat Exporter.")
+    return 0
 
 
-def create_html(data, output_folder, template=None, embedded=False, offline_static=False, maximum_size=None):
-    if template is None:
-        template_dir = os.path.dirname(__file__)
-        template_file = "whatsapp.html"
+def rendering(
+        output_file_name,
+        template,
+        name,
+        msgs,
+        contact,
+        w3css,
+        next,
+        chat,
+    ):
+    if chat.their_avatar_thumb is None and chat.their_avatar is not None:
+        their_avatar_thumb = chat.their_avatar
     else:
-        template_dir = os.path.dirname(template)
-        template_file = os.path.basename(template)
-    templateLoader = jinja2.FileSystemLoader(searchpath=template_dir)
-    templateEnv = jinja2.Environment(loader=templateLoader)
-    templateEnv.globals.update(determine_day=determine_day)
-    templateEnv.filters['sanitize_except'] = sanitize_except
-    template = templateEnv.get_template(template_file)
+        their_avatar_thumb = chat.their_avatar_thumb
+    with open(output_file_name, "w", encoding="utf-8") as f:
+        f.write(
+            template.render(
+                name=name,
+                msgs=msgs,
+                my_avatar=chat.my_avatar,
+                their_avatar=chat.their_avatar,
+                their_avatar_thumb=their_avatar_thumb,
+                w3css=w3css,
+                next=next,
+                status=chat.status,
+            )
+        )
 
-    total_row_number = len(data)
-    print(f"\nCreating HTML...(0/{total_row_number})", end="\r")
 
-    if not os.path.isdir(output_folder):
-        os.mkdir(output_folder)
+class Device(StrEnum):
+    IOS = "ios"
+    ANDROID = "android"
+    EXPORTED = "exported"
+
+
+def import_from_json(json_file, data):
+    from Whatsapp_Chat_Exporter.data_model import ChatStore, Message
+    with open(json_file, "r") as f:
+        temp_data = json.loads(f.read())
+    total_row_number = len(tuple(temp_data.keys()))
+    print(f"Importing chats from JSON...(0/{total_row_number})", end="\r")
+    for index, (jid, chat_data) in enumerate(temp_data.items()):
+        chat = ChatStore(chat_data.get("type"), chat_data.get("name"))
+        chat.my_avatar = chat_data.get("my_avatar")
+        chat.their_avatar = chat_data.get("their_avatar")
+        chat.their_avatar_thumb = chat_data.get("their_avatar_thumb")
+        chat.status = chat_data.get("status")
+        for id, msg in chat_data.get("messages").items():
+            message = Message(
+                msg["from_me"],
+                msg["timestamp"],
+                msg["time"],
+                msg["key_id"],
+            )
+            message.media = msg.get("media")
+            message.meta = msg.get("meta")
+            message.data = msg.get("data")
+            message.sender = msg.get("sender")
+            message.safe = msg.get("safe")
+            message.mime = msg.get("mime")
+            message.reply = msg.get("reply")
+            message.quoted_data = msg.get("quoted_data")
+            message.caption = msg.get("caption")
+            message.thumb = msg.get("thumb")
+            message.sticker = msg.get("sticker")
+            chat.add_message(id, message)
+        data[jid] = chat
+        print(f"Importing chats from JSON...({index + 1}/{total_row_number})", end="\r")
+
+
+def get_file_name(contact: str, chat: ChatStore):
+    if "@" not in contact and contact not in ("000000000000000", "000000000000001", "ExportedChat"):
+        raise ValueError("Unexpected contact format: " + contact)
+    phone_number = contact.split('@')[0]
+    if "-" in contact:
+        file_name = ""
+    else:
+        file_name = phone_number
+
+    if chat.name is not None:
+        if file_name != "":
+            file_name += "-"
+        file_name += chat.name.replace("/", "-")
+        name = chat.name
+    else:
+        name = phone_number
+
+    return "".join(x for x in file_name if x.isalnum() or x in "- "), name
 
-    w3css = "https://www.w3schools.com/w3css/4/w3.css"
-    if offline_static:
-        import urllib.request
-        static_folder = os.path.join(output_folder, offline_static)
-        if not os.path.isdir(static_folder):
-            os.mkdir(static_folder)
-        w3css_path = os.path.join(static_folder, "w3.css")
-        if not os.path.isfile(w3css_path):
-            with urllib.request.urlopen(w3css) as resp:
-                with open(w3css_path, "wb") as f: f.write(resp.read())
-        w3css = os.path.join(offline_static, "w3.css")
-
-    for current, contact in enumerate(data):
-        if len(data[contact]["messages"]) == 0:
-            continue
-        phone_number = contact.split('@')[0]
-        if "-" in contact:
-            file_name = ""
-        else:
-            file_name = phone_number
 
-        if data[contact]["name"] is not None:
-            if file_name != "":
-                file_name += "-"
-            file_name += data[contact]["name"].replace("/", "-")
-            name = data[contact]["name"]
+# Android Specific
+CRYPT14_OFFSETS = (
+    {"iv": 67, "db": 191},
+    {"iv": 67, "db": 190},
+    {"iv": 66, "db": 99},
+    {"iv": 67, "db": 193},
+    {"iv": 67, "db": 194},
+)
+
+
+class Crypt(IntEnum):
+    CRYPT15 = 15
+    CRYPT14 = 14
+    CRYPT12 = 12
+
+
+def brute_force_offset(max_iv=200, max_db=200):
+    for iv in range(0, max_iv):
+        for db in range(0, max_db):
+            yield iv, iv + 16, db
+
+
+def determine_metadata(content, init_msg):
+    msg = init_msg if init_msg else ""
+    if content["is_me_joined"] == 1:  # Override
+        return f"You were added into the group by {msg}"
+    if content["action_type"] == 1:
+        msg += f''' changed the group name to "{content['data']}"'''
+    elif content["action_type"] == 4:
+        msg += " was added to the group"
+    elif content["action_type"] == 5:
+        msg += " left the group"
+    elif content["action_type"] == 6:
+        msg += f" changed the group icon"
+    elif content["action_type"] == 7:
+        msg = "You were removed"
+    elif content["action_type"] == 8:
+        msg += ("WhatsApp Internal Error Occurred: "
+                "you cannot send message to this group")
+    elif content["action_type"] == 9:
+        msg += " created a broadcast channel"
+    elif content["action_type"] == 10:
+        try:
+            old = content['old_jid'].split('@')[0]
+            new = content['new_jid'].split('@')[0]
+        except (AttributeError, IndexError):
+            return None
+        else:
+            msg = f"{old} changed their number to {new}"
+    elif content["action_type"] == 11:
+        msg += f''' created a group with name: "{content['data']}"'''
+    elif content["action_type"] == 12:
+        msg += f" added someone"  # TODO: Find out who
+    elif content["action_type"] == 13:
+        return  # Someone left the group
+    elif content["action_type"] == 14:
+        msg += f" removed someone"  # TODO: Find out who
+    elif content["action_type"] == 15:
+        return  # Someone promoted someone as an admin
+    elif content["action_type"] == 18:
+        if msg != "You":
+            msg = f"The security code between you and {msg} changed"
+        else:
+            msg = "The security code in this chat changed"
+    elif content["action_type"] == 19:
+        msg = "This chat is now end-to-end encrypted"
+    elif content["action_type"] == 20:
+        msg = "Someone joined this group by using a invite link"  # TODO: Find out who
+    elif content["action_type"] == 27:
+        msg += " changed the group description to:<br>"
+        msg += content['data'].replace("\n", '<br>')
+    elif content["action_type"] == 28:
+        try:
+            old = content['old_jid'].split('@')[0]
+            new = content['new_jid'].split('@')[0]
+        except (AttributeError, IndexError):
+            return None
         else:
-            name = phone_number
+            msg = f"{old} changed their number to {new}"
+    elif content["action_type"] == 46:
+        return # Voice message in PM??? Seems no need to handle.
+    elif content["action_type"] == 47:
+        msg = "The contact is an official business account"
+    elif content["action_type"] == 50:
+        msg = "The contact's account type changed from business to standard"
+    elif content["action_type"] == 56:
+        msg = "Messgae timer was enabled/updated/disabled"
+    elif content["action_type"] == 57:
+        if msg != "You":
+            msg = f"The security code between you and {msg} changed"
+        else:
+            msg = "The security code in this chat changed"
+    elif content["action_type"] == 58:
+        msg = "You blocked this contact"
+    elif content["action_type"] == 67:
+        return  # (PM) this contact use secure service from Facebook???
+    elif content["action_type"] == 69:
+        return  # (PM) this contact use secure service from Facebook??? What's the difference with 67????
+    else:
+        return  # Unsupported
+    return msg
 
-        safe_file_name = ''
-        safe_file_name = "".join(x for x in file_name if x.isalnum() or x in "- ")
-        with open(f"{output_folder}/{safe_file_name}.html", "w", encoding="utf-8") as f:
-            f.write(
-                template.render(
-                    name=name,
-                    msgs=data[contact]["messages"].values(),
-                    my_avatar=None,
-                    their_avatar=f"WhatsApp/Avatars/{contact}.j",
-                    w3css=w3css
-                )
-            )
-        if current % 10 == 0:
-            print(f"Creating HTML...({current}/{total_row_number})", end="\r")
 
-    print(f"Creating HTML...({total_row_number}/{total_row_number})", end="\r")
+def get_status_location(output_folder, offline_static):
+    w3css = "https://www.w3schools.com/w3css/4/w3.css"
+    if not offline_static:
+        return w3css
+    import urllib.request
+    static_folder = os.path.join(output_folder, offline_static)
+    if not os.path.isdir(static_folder):
+        os.mkdir(static_folder)
+    w3css_path = os.path.join(static_folder, "w3.css")
+    if not os.path.isfile(w3css_path):
+        with urllib.request.urlopen(w3css) as resp:
+            with open(w3css_path, "wb") as f: f.write(resp.read())
+    w3css = os.path.join(offline_static, "w3.css")
 
 
-if __name__ == "__main__":
-    from optparse import OptionParser
-    parser = OptionParser()
-    parser.add_option(
-        "-w",
-        "--wa",
-        dest="wa",
-        default="wa.db",
-        help="Path to contact database")
-    parser.add_option(
-        "-m",
-        "--media",
-        dest="media",
-        default="Message",
-        help="Path to WhatsApp media folder"
+def setup_template(template, no_avatar):
+    if template is None:
+        template_dir = os.path.dirname(__file__)
+        template_file = "whatsapp.html"
+    else:
+        template_dir = os.path.dirname(template)
+        template_file = os.path.basename(template)
+    template_loader = jinja2.FileSystemLoader(searchpath=template_dir)
+    template_env = jinja2.Environment(loader=template_loader, autoescape=True)
+    template_env.globals.update(
+        determine_day=determine_day,
+        no_avatar=no_avatar
     )
-    # parser.add_option(
-    #     "-t",
-    #     "--template",
-    #     dest="html",
-    #     default="wa.db",
-    #     help="Path to HTML template")
-    (options, args) = parser.parse_args()
-    msg_db = "7c7fba66680ef796b916b067077cc246adacf01d"
-    output_folder = "temp"
-    contact_db = options.wa
-    media_folder = options.media
-
-    if len(args) == 1:
-        msg_db = args[0]
-    elif len(args) == 2:
-        msg_db = args[0]
-        output_folder = args[1]
-
-    data = {}
-
-    if os.path.isfile(msg_db):
-        with sqlite3.connect(msg_db) as db:
-            messages(db, data)
-            media(db, data, media_folder)
-            vcard(db, data)
-        create_html(data, output_folder)
-
-    if not os.path.isdir(f"{output_folder}/WhatsApp"):
-        shutil.move(media_folder, f"{output_folder}/")
-
-    with open("result.json", "w") as f:
-        data = json.dumps(data)
-        print(f"\nWriting JSON file...({int(len(data)/1024/1024)}MB)")
-        f.write(data)
+    template_env.filters['sanitize_except'] = sanitize_except
+    return template_env.get_template(template_file)
 
-    print("Everything is done!")
+# iOS Specific
+APPLE_TIME = datetime.timestamp(datetime(2001, 1, 1))
```

### Comparing `whatsapp-chat-exporter-0.9.1/setup.py` & `whatsapp-chat-exporter-0.9.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,56 +8,62 @@
     version = search(r'__version__ = "(.*?)"', f.read()).group(1)
 
 setuptools.setup(
     name="whatsapp-chat-exporter",
     version=version,
     author="KnugiHK",
     author_email="hello@knugi.com",
-    description="A Whatsapp database parser that will give you the "
-                "history of your Whatsapp conversations in HTML and JSON.",
+    description=("A Whatsapp database parser that will give you the "
+                "history of your Whatsapp conversations in HTML and JSON. "
+                "Android, iOS, iPadOS, Crypt12, Crypt14, Crypt15 supported."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords=[
-        "android", "ios", "parsing", "history","iphone", "whatsapp", "message"
-        "customizable", "android-backup", "crypt12", "whatsapp-chat-exporter",
-        "whatsapp-export", "whatsapp-database", "whatsapp-database-parser",
-        "whatsapp-conversations", "iphone-backup", "crypt14", "crypt15", "messages"
+        "android", "ios", "parsing", "history", "iphone", "message", "crypt15",
+        "customizable", "whatsapp", "android-backup", "messages", "crypt14", 
+        "crypt12", "whatsapp-chat-exporter", "whatsapp-export", "iphone-backup",
+        "whatsapp-database", "whatsapp-database-parser", "whatsapp-conversations"
     ],
     platforms=["any"],
     url="https://github.com/KnugiHK/Whatsapp-Chat-Exporter",
     packages=setuptools.find_packages(),
     package_data={
         '': ['whatsapp.html']
     },
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "Topic :: Communications :: Chat",
         "Topic :: Utilities",
         "Topic :: Database"
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'jinja2',
         'bleach'
     ],
     extras_require={
         'android_backup':  ["pycryptodome", "javaobj-py3"],
         'crypt12':  ["pycryptodome"],
         'crypt14':  ["pycryptodome"],
-        'crypt15':  ["pycryptodome", "javaobj-py3"]
+        'crypt15':  ["pycryptodome", "javaobj-py3"],
+        'all': ["pycryptodome", "javaobj-py3"],
+        'everything': ["pycryptodome", "javaobj-py3"],
+        'backup': ["pycryptodome", "javaobj-py3"]
     },
     entry_points={
         "console_scripts": [
-            "wtsexporter = Whatsapp_Chat_Exporter.__main__:main"
+            "wtsexporter = Whatsapp_Chat_Exporter.__main__:main",
+            "waexporter = Whatsapp_Chat_Exporter.__main__:main",
+            "whatsapp-chat-exporter = Whatsapp_Chat_Exporter.__main__:main"
         ]
     }
 )
```

### Comparing `whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/PKG-INFO` & `whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-exporter
-Version: 0.9.1
-Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
+Version: 0.9.5
+Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Android, iOS, iPadOS, Crypt12, Crypt14, Crypt15 supported.
 Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
 Author: KnugiHK
 Author-email: hello@knugi.com
 License: MIT
-Keywords: android,ios,parsing,history,iphone,whatsapp,messagecustomizable,android-backup,crypt12,whatsapp-chat-exporter,whatsapp-export,whatsapp-database,whatsapp-database-parser,whatsapp-conversations,iphone-backup,crypt14,crypt15,messages
+Keywords: android,ios,parsing,history,iphone,message,crypt15,customizable,whatsapp,android-backup,messages,crypt14,crypt12,whatsapp-chat-exporter,whatsapp-export,iphone-backup,whatsapp-database,whatsapp-database-parser,whatsapp-conversations
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Utilities
 Classifier: Topic :: Database
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: android_backup
 Provides-Extra: crypt12
 Provides-Extra: crypt14
 Provides-Extra: crypt15
+Provides-Extra: all
+Provides-Extra: everything
+Provides-Extra: backup
 License-File: LICENSE
 
 # Whatsapp-Chat-Exporter
 [![Latest in Pypi](https://img.shields.io/pypi/v/whatsapp-chat-exporter?label=Latest%20in%20Pypi)](https://pypi.org/project/whatsapp-chat-exporter/)
 ![License MIT](https://img.shields.io/pypi/l/whatsapp-chat-exporter)
 [![Python](https://img.shields.io/pypi/pyversions/Whatsapp-Chat-Exporter)](https://pypi.org/project/Whatsapp-Chat-Exporter/)
 
@@ -71,14 +74,16 @@
 In order to support the decryption, install pycryptodome if it is not installed
 ```sh
 pip install pycryptodome # Or 
 pip install whatsapp-chat-exporter["android_backup"] # install along with this software
 ```
 ### Crypt15 is now the easiest way to decrypt a backup. If you have the 32 bytes hex key generated when you enable End-to-End encrypted backup, you can use it to decrypt the backup. If you do not have the 32 bytes hex key, you can still use the key file extracted just like extacting key file for Crypt12 and Crypt14 to decrypt the backup.
 #### Crypt12 or Crypt14
+You will need the decryption key file from your phone. If you have root access, you can find it as `/data/data/com.whatsapp/files/key`. Otherwise, if you used WhatsApp-Key-DB-Extractor before, it will appear in the WhatsApp backup directory as `WhatsApp/Databases/.nomedia`.
+
 Place the decryption key file (key) and the encrypted WhatsApp Backup (msgstore.db.crypt14) in the working directory. If you also want the name of your contacts, get the contact database, which is called wa.db. And copy the WhatsApp (Media) directory from your phone directly.
 
 And now, you should have something like this in the working directory.
 
 ![Android folder structure with WhatsApp Backup](imgs/android_structure_backup.png)
 #### Extracting
 Simply invoke the following command from shell.
@@ -104,70 +109,87 @@
 wtsexporter -a -k encrypted_backup.key -b msgstore.db.crypt15
 ```
 If you have the 32 bytes hex key, simply put the hex key in the -k option and invoke the command from shell like this:
 ```sh
 wtsexporter -a -k 432435053b5204b08e5c3823423399aa30ff061435ab89bc4e6713969cdaa5a8 -b msgstore.db.crypt15
 ```
 
-## Working with iPhone
-Do an iPhone Backup with iTunes first.
-### Encrypted iPhone Backup
-**If you are working on unencrypted iPhone backup, skip this**
+## Working with iOS/iPadOS (iPhone or iPad)
+Do an iPhone/iPad Backup with iTunes first.
+* iPhone backup on Mac: https://support.apple.com/HT211229
+* iPhone backup on Windows: https://support.apple.com/HT212156
+* iPad backup: https://support.apple.com/guide/ipad/ipad9a74df05xx/ipados
+### Encrypted iOS/iPadOS Backup
+**If you are working on unencrypted iOS/iPadOS backup, skip this**
 
-If you want to work on an encrypted iPhone Backup, you should install iphone_backup_decrypt from [KnugiHK/iphone_backup_decrypt](https://github.com/KnugiHK/iphone_backup_decrypt) before you run the extract_iphone_media.py.
+If you want to work on an encrypted iOS/iPadOS Backup, you should install iphone_backup_decrypt from [KnugiHK/iphone_backup_decrypt](https://github.com/KnugiHK/iphone_backup_decrypt) before you run the extract_iphone_media.py.
 ```sh
 pip install git+https://github.com/KnugiHK/iphone_backup_decrypt
 ```
 ### Extracting
 Simply invoke the following command from shell, remember to replace the username and device id correspondingly in the command.
+#### Windows
 ```sh
 wtsexporter -i -b "C:\Users\[Username]\AppData\Roaming\Apple Computer\MobileSync\Backup\[device id]"
 ```
+#### Mac
+```sh
+wtsexporter -i -b "~/Library/Application Support/MobileSync/Backup/[device id]"
+```
 
 ## Results
 After extracting, you will get these:
 #### Private Message
 ![Private Message](imgs/pm.png)
 
 #### Group Message
 ![Group Message](imgs/group.png)
 
+*The above screenshots were taken longgggggggggggggg ago. I am going to update them when possible.*
+
 ## More options
 Invoke the wtsexporter with --help option will show you all options available.
 ```sh
 > wtsexporter --help
-usage: wtsexporter [options]
+usage: wtsexporter [-h] [-a] [-i] [-e EXPORTED] [-w WA] [-m MEDIA] [-b BACKUP] [-o OUTPUT] [-j [JSON]] [-d DB] [-k KEY] [-t TEMPLATE] [-s] [-c] [--offline OFFLINE] [--size [SIZE]]
+                   [--no-html] [--check-update] [--assume-first-as-me]
 
 options:
   -h, --help            show this help message and exit
   -a, --android         Define the target as Android
-  -i, --iphone, --ios   Define the target as iPhone
+  -i, --iphone, --ios   Define the target as iPhone/iPad
+  -e EXPORTED, --exported EXPORTED
+                        Define the target as exported chat file and specify the path to the file
   -w WA, --wa WA        Path to contact database (default: wa.db/ContactsV2.sqlite)
   -m MEDIA, --media MEDIA
                         Path to WhatsApp media folder (default: WhatsApp)
   -b BACKUP, --backup BACKUP
                         Path to Android (must be used together with -k)/iPhone WhatsApp backup
   -o OUTPUT, --output OUTPUT
                         Output to specific directory (default: result)
   -j [JSON], --json [JSON]
                         Save the result to a single JSON file (default if present: result.json)
   -d DB, --db DB        Path to database file (default: msgstore.db/7c7fba66680ef796b916b067077cc246adacf01d)
   -k KEY, --key KEY     Path to key file
   -t TEMPLATE, --template TEMPLATE
                         Path to custom HTML template
-  -e, --embedded        Embed media into HTML file (not yet implemented)
   -s, --showkey         Show the HEX key used to decrypt the database
   -c, --move-media      Move the media directory to output directory if the flag is set, otherwise copy it
   --offline OFFLINE     Relative path to offline static files
-  --size SIZE, --output-size SIZE
-                        Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
+  --size [SIZE], --output-size [SIZE], --split [SIZE]
+                        Maximum (rough) size of a single output file in bytes, 0 for auto
   --no-html             Do not output html files
-  --check-update        Check for updates
+  --check-update        Check for updates (require Internet access)
+  --assume-first-as-me  Assume the first message in a chat as sent by me (must be used together with -e)
+
+WhatsApp Chat Exporter: 0.9.5 Licensed with MIT
 ```
 
 # To do
 See [issues](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues).
 
 # Copyright
 This is a MIT licensed project.
 
 The Telegram Desktop's export is the reference for whatsapp.html in this repo
+
+WhatsApp Chat Exporter is not affiliated, associated, authorized, endorsed by, or in any way officially connected with the WhatsApp LLC, or any of its subsidiaries or its affiliates. The official WhatsApp LLC website can be found at https://www.whatsapp.com/.
```

### Comparing `whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/SOURCES.txt` & `whatsapp-chat-exporter-0.9.5/whatsapp_chat_exporter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE
 README.md
 setup.py
 Whatsapp_Chat_Exporter/__init__.py
 Whatsapp_Chat_Exporter/__main__.py
 Whatsapp_Chat_Exporter/data_model.py
 Whatsapp_Chat_Exporter/extract.py
+Whatsapp_Chat_Exporter/extract_exported.py
 Whatsapp_Chat_Exporter/extract_iphone.py
 Whatsapp_Chat_Exporter/extract_iphone_media.py
-Whatsapp_Chat_Exporter/extract_new.py
 Whatsapp_Chat_Exporter/utility.py
 Whatsapp_Chat_Exporter/whatsapp.html
 whatsapp_chat_exporter.egg-info/PKG-INFO
 whatsapp_chat_exporter.egg-info/SOURCES.txt
 whatsapp_chat_exporter.egg-info/dependency_links.txt
 whatsapp_chat_exporter.egg-info/entry_points.txt
 whatsapp_chat_exporter.egg-info/requires.txt
```

