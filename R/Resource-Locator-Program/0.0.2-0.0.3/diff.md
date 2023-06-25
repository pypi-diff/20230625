# Comparing `tmp/Resource Locator Program-0.0.2.tar.gz` & `tmp/Resource Locator Program-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Resource Locator Program-0.0.2.tar", last modified: Sat Jan  7 00:57:39 2023, max compression
+gzip compressed data, was "Resource Locator Program-0.0.3.tar", last modified: Sun Jun 25 17:08:17 2023, max compression
```

## Comparing `Resource Locator Program-0.0.2.tar` & `Resource Locator Program-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-01-07 00:57:39.505100 Resource Locator Program-0.0.2/
--rw-r--r--   0 rickwierenga   (501) staff       (20)     1075 2023-01-04 19:01:49.000000 Resource Locator Program-0.0.2/LICENSE
--rw-r--r--   0 rickwierenga   (501) staff       (20)     2614 2023-01-07 00:57:39.504989 Resource Locator Program-0.0.2/PKG-INFO
--rw-r--r--   0 rickwierenga   (501) staff       (20)     2317 2023-01-07 00:35:49.000000 Resource Locator Program-0.0.2/README.md
-drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-01-07 00:57:39.503585 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/
--rw-r--r--   0 rickwierenga   (501) staff       (20)     2614 2023-01-07 00:57:39.000000 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/PKG-INFO
--rw-r--r--   0 rickwierenga   (501) staff       (20)      518 2023-01-07 00:57:39.000000 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/SOURCES.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)        1 2023-01-07 00:57:39.000000 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/dependency_links.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)       79 2023-01-07 00:57:39.000000 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/entry_points.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)       17 2023-01-07 00:57:39.000000 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/requires.txt
--rw-r--r--   0 rickwierenga   (501) staff       (20)       25 2023-01-07 00:57:39.000000 Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/top_level.txt
-drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-01-07 00:57:39.504608 Resource Locator Program-0.0.2/resource_locator_program/
--rw-r--r--   0 rickwierenga   (501) staff       (20)     7107 2023-01-07 00:28:55.000000 Resource Locator Program-0.0.2/resource_locator_program/app.py
--rw-r--r--   0 rickwierenga   (501) staff       (20)    13243 2023-01-07 00:28:20.000000 Resource Locator Program-0.0.2/resource_locator_program/path_teacher.py
--rw-r--r--   0 rickwierenga   (501) staff       (20)     9193 2023-01-06 23:27:19.000000 Resource Locator Program-0.0.2/resource_locator_program/resource_locator.py
--rw-r--r--   0 rickwierenga   (501) staff       (20)     5312 2023-01-07 00:22:06.000000 Resource Locator Program-0.0.2/resource_locator_program/setup_screen.py
--rw-r--r--   0 rickwierenga   (501) staff       (20)    10963 2023-01-06 23:55:19.000000 Resource Locator Program-0.0.2/resource_locator_program/shared_widgets.py
--rw-r--r--   0 rickwierenga   (501) staff       (20)       38 2023-01-07 00:57:39.505140 Resource Locator Program-0.0.2/setup.cfg
--rw-r--r--   0 rickwierenga   (501) staff       (20)      635 2023-01-07 00:57:22.000000 Resource Locator Program-0.0.2/setup.py
+drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-06-25 17:08:17.597834 Resource Locator Program-0.0.3/
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     1075 2023-01-04 19:01:49.000000 Resource Locator Program-0.0.3/LICENSE
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     2614 2023-06-25 17:08:17.597719 Resource Locator Program-0.0.3/PKG-INFO
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     2317 2023-01-07 00:35:49.000000 Resource Locator Program-0.0.3/README.md
+drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-06-25 17:08:17.596486 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     2614 2023-06-25 17:08:17.000000 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/PKG-INFO
+-rw-r--r--   0 rickwierenga   (501) staff       (20)      518 2023-06-25 17:08:17.000000 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/SOURCES.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)        1 2023-06-25 17:08:17.000000 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/dependency_links.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       79 2023-06-25 17:08:17.000000 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/entry_points.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       17 2023-06-25 17:08:17.000000 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/requires.txt
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       25 2023-06-25 17:08:17.000000 Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/top_level.txt
+drwxr-xr-x   0 rickwierenga   (501) staff       (20)        0 2023-06-25 17:08:17.597429 Resource Locator Program-0.0.3/resource_locator_program/
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     7107 2023-01-16 23:11:19.000000 Resource Locator Program-0.0.3/resource_locator_program/app.py
+-rw-r--r--   0 rickwierenga   (501) staff       (20)    13365 2023-06-25 17:03:35.000000 Resource Locator Program-0.0.3/resource_locator_program/path_teacher.py
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     9342 2023-06-25 17:02:45.000000 Resource Locator Program-0.0.3/resource_locator_program/resource_locator.py
+-rw-r--r--   0 rickwierenga   (501) staff       (20)     5340 2023-06-25 17:00:04.000000 Resource Locator Program-0.0.3/resource_locator_program/setup_screen.py
+-rw-r--r--   0 rickwierenga   (501) staff       (20)    10963 2023-01-06 23:55:19.000000 Resource Locator Program-0.0.3/resource_locator_program/shared_widgets.py
+-rw-r--r--   0 rickwierenga   (501) staff       (20)       38 2023-06-25 17:08:17.597887 Resource Locator Program-0.0.3/setup.cfg
+-rw-r--r--   0 rickwierenga   (501) staff       (20)      653 2023-06-25 17:08:08.000000 Resource Locator Program-0.0.3/setup.py
```

### Comparing `Resource Locator Program-0.0.2/LICENSE` & `Resource Locator Program-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Resource Locator Program-0.0.2/PKG-INFO` & `Resource Locator Program-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Resource Locator Program
-Version: 0.0.2
+Version: 0.0.3
 Summary: Resource Locator Program
 Home-page: https://www.github.com/pylabrobot/resource-locator-program/
 Author: Rick Wierenga
 Author-email: rick_wierenga@icloud.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Resource Locator Program-0.0.2/README.md` & `Resource Locator Program-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/PKG-INFO` & `Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Resource-Locator-Program
-Version: 0.0.2
+Version: 0.0.3
 Summary: Resource Locator Program
 Home-page: https://www.github.com/pylabrobot/resource-locator-program/
 Author: Rick Wierenga
 Author-email: rick_wierenga@icloud.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Resource Locator Program-0.0.2/Resource_Locator_Program.egg-info/SOURCES.txt` & `Resource Locator Program-0.0.3/Resource_Locator_Program.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Resource Locator Program-0.0.2/resource_locator_program/app.py` & `Resource Locator Program-0.0.3/resource_locator_program/app.py`

 * *Files identical despite different names*

### Comparing `Resource Locator Program-0.0.2/resource_locator_program/path_teacher.py` & `Resource Locator Program-0.0.3/resource_locator_program/path_teacher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import traceback
 from typing import Optional
 
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QFont
 from PyQt6.QtWidgets import (
   QGroupBox,
@@ -278,24 +279,25 @@
 
     self.general_layout.addWidget(self.mover_group)
 
     self.build_path_widget = BuildPathEditorWidget(
       get_location=self.get_location,
       put_plate=self.put_plate)
     self.general_layout.addWidget(self.build_path_widget)
+    self.build_path_widget.disable()
 
   def pick_up_plate(self, plate):
     try:
-      self.lh.backend.pick_up_resource(
+      asyncio.run(self.lh.backend.pick_up_resource(
         resource=plate,
         grip_direction=GripDirection.FRONT,
         pickup_distance_from_top=PICKUP_DISTANCE_FROM_TOP,
         offset=Coordinate.zero(),
-      )
-    except Exception as e:
+      ))
+    except Exception as e: # pylint: disable=broad-except
       print(traceback.format_exc())
       show_error_alert(
         title="An error occurred while picking up plate.",
         description=str(e),
         details=traceback.format_exc())
     else:
       self.controller_disabled = False
@@ -322,23 +324,23 @@
       site = site_or_location
       location = site_or_location.get_absolute_location()
     else:
       site = None
       location = site_or_location
 
     try:
-      self.lh.backend.release_picked_up_resource(
+      asyncio.run(self.lh.backend.release_picked_up_resource(
         resource=self.picked_up_plate,
         location=location,
         offset=Coordinate.zero(),
         grip_direction=GripDirection.FRONT,
         pickup_distance_from_top=PICKUP_DISTANCE_FROM_TOP,
         minimum_traverse_height_at_beginning_of_a_command=
           int(self._location.z + self.picked_up_plate.get_size_z() / 2) * 10 # "minimum" is scam
-      )
+      ))
     except Exception as e:
       print(traceback.format_exc())
       show_error_alert(
         title="An error occurred while putting plate.",
         description=str(e),
         details=traceback.format_exc())
       raise e
@@ -373,21 +375,21 @@
     assert self.picked_up_plate is not None
 
     super().set_location(x=x, y=y, z=z)
 
     self.controller_disabled = True
 
     try:
-      self.lh.backend.move_picked_up_resource(
+      asyncio.run(self.lh.backend.move_picked_up_resource(
         location=self._location,
         resource=self.picked_up_plate,
         grip_direction=GripDirection.FRONT,
         minimum_traverse_height_at_beginning_of_a_command=
           int(self._location.z + self.picked_up_plate.get_size_z() / 2) * 10 # "minimum" is scam
-      )
+      ))
     except Exception as e:
       traceback.print_exc()
       show_error_alert(
         title="Error while moving plate",
         description=str(e),
         details=traceback.format_exc())
     else:
```

### Comparing `Resource Locator Program-0.0.2/resource_locator_program/resource_locator.py` & `Resource Locator Program-0.0.3/resource_locator_program/resource_locator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import traceback
 
 from PyQt6.QtWidgets import (
   QFileDialog,
   QGroupBox,
   QHBoxLayout,
   QLabel,
@@ -154,35 +155,36 @@
 
     self.tip_racks_widget = TipRacksWidget(
       pick_up_tip_a1=self.pick_up_tip_a1, drop_tip_a1=self.drop_tip_a1, lh=self.lh)
     self.general_layout.addWidget(self.tip_racks_widget)
 
     self.general_layout.addWidget(self.mover_group)
 
-    self.unlocated_resources_widget = UnlocatedResourcesWidget(get_location=self.get_location, lh=self.lh)
+    self.unlocated_resources_widget = UnlocatedResourcesWidget(
+      get_location=self.get_location, lh=self.lh)
     self.general_layout.addWidget(self.unlocated_resources_widget)
 
     self.save_button = QPushButton("Save to file")
     self.save_button.clicked.connect(self.save)
     self.general_layout.addWidget(self.save_button)
 
   def set_location(self, x=None, y=None, z=None):
     super().set_location(x, y, z)
 
     self.controller_disabled = True
 
     try:
       if x is not None:
-        self.lh.backend.move_channel_x(self.lh.backend.num_channels - 1, x)
+        asyncio.run(self.lh.backend.move_channel_x(self.lh.backend.num_channels - 1, x))
         self.display.set_x(x)
       if y is not None:
-        self.lh.backend.move_channel_y(self.lh.backend.num_channels - 1, y)
+        asyncio.run(self.lh.backend.move_channel_y(self.lh.backend.num_channels - 1, y))
         self.display.set_y(y)
       if z is not None:
-        self.lh.backend.move_channel_z(self.lh.backend.num_channels - 1, z)
+        asyncio.run(self.lh.backend.move_channel_z(self.lh.backend.num_channels - 1, z))
         self.display.set_z(z)
     except Exception as e:
       traceback.print_exc()
       show_error_alert(
         title="Error while moving y axis",
         description=str(e),
         details=traceback.format_exc())
@@ -190,16 +192,17 @@
       self.controller_disabled = False
 
   def pick_up_tip_a1(self, tip_rack: TipRack):
     tip = tip_rack.get_tip("A1")
 
     try:
       self.tip_racks_widget.start_pick_up_tip_a1()
-      self.lh.pick_up_tips(tip_rack["A1"], use_channels=[self.lh.backend.num_channels - 1])
-    except Exception as e:
+      asyncio.run(
+        self.lh.pick_up_tips(tip_rack["A1"], use_channels=[self.lh.backend.num_channels - 1]))
+    except Exception as e: # pylint: disable=broad-except
       self.tip_racks_widget.pick_up_tip_failed()
       traceback.print_exc()
       show_error_alert(
         title="Error while picking up tip",
         description=str(e),
         details=traceback.format_exc())
     else:
@@ -216,15 +219,16 @@
       self.unlocated_resources_widget.setDisabled(False)
       self.controller_disabled = False
       self.lock_tab()
 
   def drop_tip_a1(self, tip_rack: TipRack):
     try:
       self.tip_racks_widget.start_drop_tip_a1()
-      self.lh.drop_tips(tip_rack["A1"], use_channels=[self.lh.backend.num_channels - 1])
+      asyncio.run(
+        self.lh.drop_tips(tip_rack["A1"], use_channels=[self.lh.backend.num_channels - 1]))
     except Exception as e:
       self.tip_racks_widget.drop_tip_failed()
       traceback.print_exc()
       show_error_alert(
         title="Error while dropping up tip",
         description=str(e),
         details=traceback.format_exc())
@@ -248,15 +252,15 @@
     super().build_ui()
 
     self.tip_racks_widget.build_ui()
     self.unlocated_resources_widget.build_ui()
 
   def start(self):
     try:
-      self.lh.backend.prepare_for_manual_channel_operation()
+      asyncio.run(self.lh.backend.prepare_for_manual_channel_operation())
     except Exception as e:
       traceback.print_exc()
       show_error_alert(
         title="Error moving channels",
         description=str(e),
         details=traceback.format_exc())
```

### Comparing `Resource Locator Program-0.0.2/resource_locator_program/setup_screen.py` & `Resource Locator Program-0.0.3/resource_locator_program/setup_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 import os
 import threading
 import textwrap
 import traceback
 
 from PyQt6.QtCore import Qt, pyqtSignal
@@ -129,15 +130,15 @@
   def _setup(self):
     self.loading_label.show()
     self.setup_button.hide()
     self.file_picker.setEnabled(False)
 
     def setup():
       try:
-        self.lh.setup()
+        asyncio.run(self.lh.setup())
       except Exception as e:
         print(traceback.format_exc())
 
         self.setup_finished_signal.emit((False, e))
       else:
         self.setup_finished_signal.emit((True, None))
```

### Comparing `Resource Locator Program-0.0.2/resource_locator_program/shared_widgets.py` & `Resource Locator Program-0.0.3/resource_locator_program/shared_widgets.py`

 * *Files identical despite different names*

### Comparing `Resource Locator Program-0.0.2/setup.py` & `Resource Locator Program-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from distutils.core import setup
 
 
-with open("README.md", "r") as f:
+with open("README.md", "r", encoding="utf-8") as f:
   long_description = f.read()
 
 
 setup(name="Resource Locator Program",
-  version="0.0.2",
+  version="0.0.3",
   description="Resource Locator Program",
   long_description=long_description,
   long_description_content_type="text/markdown",
   author="Rick Wierenga",
   author_email="rick_wierenga@icloud.com",
   url="https://www.github.com/pylabrobot/resource-locator-program/",
   install_requires=["PyQt6", "pylabrobot"],
```

