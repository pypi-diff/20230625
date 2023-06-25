# Comparing `tmp/kobushi_trackviewer-1.1.4-py3-none-any.whl.zip` & `tmp/kobushi_trackviewer-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 42440 bytes, number of entries: 19
+Zip file size: 42462 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      634 b- defN 21-Aug-15 09:07 kobushi/__init__.py
 -rw-r--r--  2.0 unx      649 b- defN 21-Aug-14 12:53 kobushi/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Oct-15 12:32 kobushi/_version.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-24 15:41 kobushi/_version.py
 -rw-r--r--  2.0 unx     3482 b- defN 21-Aug-20 14:15 kobushi/dialog_multifields.py
--rw-r--r--  2.0 unx    35123 b- defN 22-Oct-15 12:32 kobushi/gui_interface.py
+-rw-r--r--  2.0 unx    35123 b- defN 23-Jun-24 15:41 kobushi/gui_interface.py
 -rw-r--r--  2.0 unx     2999 b- defN 21-Aug-14 12:53 kobushi/loadheader.py
 -rw-r--r--  2.0 unx      761 b- defN 22-Oct-15 12:32 kobushi/loadmapgrammer.py
 -rw-r--r--  2.0 unx     1665 b- defN 22-Apr-18 12:51 kobushi/map-grammer.lark
 -rw-r--r--  2.0 unx     9920 b- defN 22-Oct-15 12:32 kobushi/mapinterpreter.py
 -rw-r--r--  2.0 unx    11615 b- defN 22-Mar-10 13:40 kobushi/mapobj.py
--rw-r--r--  2.0 unx    17185 b- defN 22-May-22 10:19 kobushi/mapplot.py
+-rw-r--r--  2.0 unx    17242 b- defN 23-Jun-24 15:41 kobushi/mapplot.py
 -rw-r--r--  2.0 unx     6306 b- defN 21-Aug-20 14:15 kobushi/othertrack_window.py
--rw-r--r--  2.0 unx    17540 b- defN 22-Apr-21 16:13 kobushi/trackcoordinate.py
--rw-r--r--  2.0 unx    35630 b- defN 22-May-22 10:19 kobushi/trackgenerator.py
--rw-r--r--  2.0 unx     9724 b- defN 22-Oct-15 12:35 kobushi_trackviewer-1.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2749 b- defN 22-Oct-15 12:35 kobushi_trackviewer-1.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-15 12:35 kobushi_trackviewer-1.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Oct-15 12:35 kobushi_trackviewer-1.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1562 b- defN 22-Oct-15 12:35 kobushi_trackviewer-1.1.4.dist-info/RECORD
-19 files, 157666 bytes uncompressed, 39898 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx    17540 b- defN 23-Mar-18 15:38 kobushi/trackcoordinate.py
+-rw-r--r--  2.0 unx    35622 b- defN 23-Jun-24 15:41 kobushi/trackgenerator.py
+-rw-r--r--  2.0 unx     9724 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2749 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1562 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/RECORD
+19 files, 157715 bytes uncompressed, 39920 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: kobushi/trackcoordinate.py
 Comment: 
 
 Filename: kobushi/trackgenerator.py
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.4.dist-info/LICENSE
+Filename: kobushi_trackviewer-1.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.4.dist-info/METADATA
+Filename: kobushi_trackviewer-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.4.dist-info/WHEEL
+Filename: kobushi_trackviewer-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.4.dist-info/top_level.txt
+Filename: kobushi_trackviewer-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.4.dist-info/RECORD
+Filename: kobushi_trackviewer-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kobushi/_version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.4'
+__version__ = '1.1.5'
```

## kobushi/gui_interface.py

```diff
@@ -582,15 +582,15 @@
                     self.profYlim = [float(dialog.variables['min'].get()),float(dialog.variables['max'].get())]
                 else:
                     self.profYlim = None
                 self.plot_all()
     def aboutwindow(self, event=None):
         msg  = 'Kobushi trackviewer\n'
         msg += 'Version '+__version__+'\n\n'
-        msg += 'Copyright © 2021-2022 konawasabi\n'
+        msg += 'Copyright © 2021-2023 konawasabi\n'
         msg += 'Released under the Apache License, Version 2.0 .\n'
         msg += 'https://www.apache.org/licenses/LICENSE-2.0'
         tk.messagebox.showinfo(message=msg)
     def customdialog_test(self, event=None):
         dialog_obj = dialog_multifields.dialog_multifields(self,\
                                         [{'name':'A', 'type':'str', 'label':'test A', 'default':'alpha'},\
                                         {'name':'B', 'type':'Double', 'label':'test B', 'default':100}],\
```

## kobushi/mapplot.py

```diff
@@ -13,18 +13,21 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 '''
 import numpy as np
 from . import trackcoordinate as tc
 from . import trackgenerator as tgen
 import matplotlib.transforms
+import pdb
 
 
 class Mapplot():
     def __init__(self,env,cp_arbdistribution=None,unitdist_default=None):
+        if False:
+            pdb.set_trace()
         self.environment = env
         self.environment.cp_arbdistribution = cp_arbdistribution
         self.environment.cp_defaultrange = [0,0]
         
         trackgenerator = tgen.TrackGenerator(self.environment,unitdist_default=unitdist_default)
         self.environment.owntrack_pos = trackgenerator.generate_owntrack()
         self.environment.owntrack_curve = trackgenerator.generate_curveradius_dist()
```

## kobushi/trackgenerator.py

```diff
@@ -508,24 +508,24 @@
                     
         for element in self.owntrack_position: # 自軌道が指定されている全ての距離程について計算する
             if self.distrange['min'] > element[0]: # 対象となる軌道が最初に現れる距離程にまだ達していないか？
                 continue
             for tpkey in ['x.position','x.radius','y.position','y.radius']: # ポインタを進める
                 while trackptr[tpkey].overNextpoint(element[0]):
                     trackptr[tpkey].seeknext()
+                    self.pos['last'][tpkey] = self.pos['next'][tpkey]
                     if trackptr[tpkey].pointer['next'] != None:
-                        self.pos['last'][tpkey] = self.pos['next'][tpkey]
                         k = 'next'
                         newval = self.data[trackptr[tpkey].pointer[k]]['value']
                         self.pos[k][tpkey] = newval if newval != 'c' else self.pos['last'][tpkey]
             for tpkey in ['interpolate_func','center','gauge']: # ポインタを進める
                 while trackptr[tpkey].onNextpoint(element[0]):
                     trackptr[tpkey].seeknext()
+                    self.pos['last'][tpkey] = self.pos['next'][tpkey]
                     if trackptr[tpkey].pointer['next'] != None:
-                        self.pos['last'][tpkey] = self.pos['next'][tpkey]
                         k = 'next'
                         newval = self.data[trackptr[tpkey].pointer[k]]['value']
                         self.pos[k][tpkey] = newval if newval != 'c' else self.pos['last'][tpkey]
             
             if trackptr['x.position'].pointer['last'] != None and trackptr['x.position'].pointer['next'] != None: # skip_dimension に従って計算するかどうか判断する
                 for k in ['last','next']:
                     self.pos[k]['x.distance'] = self.data[trackptr['x.position'].pointer[k]]['distance']
```

## Comparing `kobushi_trackviewer-1.1.4.dist-info/LICENSE` & `kobushi_trackviewer-1.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kobushi_trackviewer-1.1.4.dist-info/METADATA` & `kobushi_trackviewer-1.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobushi-trackviewer
-Version: 1.1.4
+Version: 1.1.5
 Summary: Trackviewer for BVE trainsim 5/6
 Home-page: https://github.com/konawasabi/kobushi-trackviewer/
 Author: Konawasabi
 Author-email: webmaster@konawasabi.riceball.jp
 License: Apache License 2.0
 Keywords: BVE trainsim
 Description-Content-Type: text/markdown
```

## Comparing `kobushi_trackviewer-1.1.4.dist-info/RECORD` & `kobushi_trackviewer-1.1.5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 kobushi/__init__.py,sha256=_OBJRtuhwlJl97iwmsRFAjWTMcS1F7fivZjoumsd8qk,634
 kobushi/__main__.py,sha256=zrMhFiAoyKL6DprEbJWok4KNmlsu-fVIA7xT581287E,649
-kobushi/_version.py,sha256=PjrAut5wUOgcQz79krZcrxCW7JYdU9nfMwMc8EdCaFo,22
+kobushi/_version.py,sha256=hTCioFruYR1lv7FF57n5II-8lYry8FuIYb1fA4g2ccc,22
 kobushi/dialog_multifields.py,sha256=hWcMMg8KOFql3NC-jQueRrnNUJpQutSI9IOjLh6cleU,3482
-kobushi/gui_interface.py,sha256=Pb8MygCCwVMefQgv4AjUOdyZFr_fh5j3o4Wf3cNfl94,35123
+kobushi/gui_interface.py,sha256=SqpZ9EK3vIj3zWDOEw3zRSLYAL0QGn_iH5wZMxRwz94,35123
 kobushi/loadheader.py,sha256=rLutNKL6VAgZXNwyaLmkiz8j3I6VOs93XqqbxFD6Ods,2999
 kobushi/loadmapgrammer.py,sha256=f5OHCL2l483D0IkBLTulsfQZfLcDmyidutt7TDjSHbU,761
 kobushi/map-grammer.lark,sha256=PxlMWCVglsMQMdF80Vfiz6vgGhL-GdLxhWJ58vrT2tw,1665
 kobushi/mapinterpreter.py,sha256=8UuvA5gf5bweLL65GJqUVpF4oSLH8lzlldgJMW22eW4,9920
 kobushi/mapobj.py,sha256=0usquigcUu1BhPf3sHsdOHkFesbVe31LIhhyutbp4aw,11615
-kobushi/mapplot.py,sha256=i21600ptYd9D7J7W-Y8pTCD8PUnCX9Axy0D15wldqO4,17185
+kobushi/mapplot.py,sha256=BLCquNYeJSkMHkfMlm62vwLTfTj5aY26NI-fpEhg4Ck,17242
 kobushi/othertrack_window.py,sha256=662M8YTWkASbnhet6G9ZupYVO8Pi9zT_p8HgZizERPA,6306
 kobushi/trackcoordinate.py,sha256=dwu44v5uvA8yUcJOs50eNLzktOFJJT28pUhccXGJRR8,17540
-kobushi/trackgenerator.py,sha256=v4TQRb31lZtwzVZSmp1tTpnrgUOToV1_u3V46GHijNs,35630
-kobushi_trackviewer-1.1.4.dist-info/LICENSE,sha256=OURbRZ-GYhaD-XMftqfQcIGdw3mEDo71L2K7HGiUIpE,9724
-kobushi_trackviewer-1.1.4.dist-info/METADATA,sha256=fbSQCZzWuZ2Wn7PFNNkqAjD6ZpmpUq0jZ_y9Rp7VumU,2749
-kobushi_trackviewer-1.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kobushi_trackviewer-1.1.4.dist-info/top_level.txt,sha256=g2m4m7gw1NgwbluSrxfBImA8GHjvuXwFnHgkagrMPB0,8
-kobushi_trackviewer-1.1.4.dist-info/RECORD,,
+kobushi/trackgenerator.py,sha256=9p_elvjclxYnqrxaLwMaFrZkw-exg5ocUijVihy5614,35622
+kobushi_trackviewer-1.1.5.dist-info/LICENSE,sha256=OURbRZ-GYhaD-XMftqfQcIGdw3mEDo71L2K7HGiUIpE,9724
+kobushi_trackviewer-1.1.5.dist-info/METADATA,sha256=fqNeL_3a5UnKOdOsjM35O7tzDqNFXXqmjeaRKqHGOcU,2749
+kobushi_trackviewer-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kobushi_trackviewer-1.1.5.dist-info/top_level.txt,sha256=g2m4m7gw1NgwbluSrxfBImA8GHjvuXwFnHgkagrMPB0,8
+kobushi_trackviewer-1.1.5.dist-info/RECORD,,
```

