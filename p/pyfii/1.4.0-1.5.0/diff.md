# Comparing `tmp/pyfii-1.4.0.tar.gz` & `tmp/pyfii-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfii-1.4.0.tar", last modified: Mon Jun 12 15:49:10 2023, max compression
+gzip compressed data, was "pyfii-1.5.0.tar", last modified: Sun Jun 25 17:15:39 2023, max compression
```

## Comparing `pyfii-1.4.0.tar` & `pyfii-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:49:10.320568 pyfii-1.4.0/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    35149 2023-06-09 19:42:27.000000 pyfii-1.4.0/LICENSE
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:49:10.319798 pyfii-1.4.0/PKG-INFO
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1578 2023-06-12 14:42:00.000000 pyfii-1.4.0/README.md
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      687 2023-06-12 15:48:49.000000 pyfii-1.4.0/pyproject.toml
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)       38 2023-06-12 15:49:10.320758 pyfii-1.4.0/setup.cfg
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:49:10.288459 pyfii-1.4.0/src/
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:49:10.301136 pyfii-1.4.0/src/pyfii/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      153 2023-06-12 15:48:31.000000 pyfii-1.4.0/src/pyfii/__init__.py
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:49:10.318215 pyfii-1.4.0/src/pyfii/cv3d/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     5441 2023-06-09 19:42:27.000000 pyfii-1.4.0/src/pyfii/cv3d/IIID.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3978 2023-06-09 19:42:27.000000 pyfii-1.4.0/src/pyfii/cv3d/IIID2.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:32:24.000000 pyfii-1.4.0/src/pyfii/cv3d/__init__.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1426 2023-06-09 19:42:27.000000 pyfii-1.4.0/src/pyfii/cv3d/transfer.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16682 2023-06-09 19:42:27.000000 pyfii-1.4.0/src/pyfii/drone.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3190 2023-06-09 19:42:27.000000 pyfii-1.4.0/src/pyfii/fii.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16559 2023-06-09 19:42:27.000000 pyfii-1.4.0/src/pyfii/read.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    21818 2023-06-12 15:46:54.000000 pyfii-1.4.0/src/pyfii/show.py
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:49:10.309001 pyfii-1.4.0/src/pyfii.egg-info/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:49:10.000000 pyfii-1.4.0/src/pyfii.egg-info/PKG-INFO
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      359 2023-06-12 15:49:10.000000 pyfii-1.4.0/src/pyfii.egg-info/SOURCES.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        1 2023-06-12 15:49:10.000000 pyfii-1.4.0/src/pyfii.egg-info/dependency_links.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        6 2023-06-12 15:49:10.000000 pyfii-1.4.0/src/pyfii.egg-info/top_level.txt
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-25 17:15:39.474876 pyfii-1.5.0/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    35149 2023-06-09 19:42:27.000000 pyfii-1.5.0/LICENSE
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2163 2023-06-25 17:15:39.474064 pyfii-1.5.0/PKG-INFO
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1578 2023-06-14 23:29:48.000000 pyfii-1.5.0/README.md
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      741 2023-06-25 17:15:29.000000 pyfii-1.5.0/pyproject.toml
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)       38 2023-06-25 17:15:39.475418 pyfii-1.5.0/setup.cfg
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-25 17:15:39.418653 pyfii-1.5.0/src/
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-25 17:15:39.444014 pyfii-1.5.0/src/pyfii/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      153 2023-06-22 08:46:22.000000 pyfii-1.5.0/src/pyfii/__init__.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-25 17:15:39.466550 pyfii-1.5.0/src/pyfii/cv3d/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     5441 2023-06-14 06:57:24.000000 pyfii-1.5.0/src/pyfii/cv3d/IIID.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3978 2023-06-14 06:57:32.000000 pyfii-1.5.0/src/pyfii/cv3d/IIID2.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:32:24.000000 pyfii-1.5.0/src/pyfii/cv3d/__init__.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1426 2023-06-14 06:57:39.000000 pyfii-1.5.0/src/pyfii/cv3d/transfer.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    35005 2023-06-21 19:33:58.000000 pyfii-1.5.0/src/pyfii/drone.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    11479 2023-06-25 15:34:58.000000 pyfii-1.5.0/src/pyfii/fii.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    19534 2023-06-25 16:18:05.000000 pyfii-1.5.0/src/pyfii/read.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    27822 2023-06-25 15:34:58.000000 pyfii-1.5.0/src/pyfii/show.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-25 17:15:39.454169 pyfii-1.5.0/src/pyfii.egg-info/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2163 2023-06-25 17:15:39.000000 pyfii-1.5.0/src/pyfii.egg-info/PKG-INFO
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      395 2023-06-25 17:15:39.000000 pyfii-1.5.0/src/pyfii.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        1 2023-06-25 17:15:39.000000 pyfii-1.5.0/src/pyfii.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        6 2023-06-25 17:15:39.000000 pyfii-1.5.0/src/pyfii.egg-info/top_level.txt
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-25 17:15:39.470667 pyfii-1.5.0/tests/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      777 2023-06-15 06:29:13.000000 pyfii-1.5.0/tests/test.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      357 2023-06-15 09:48:21.000000 pyfii-1.5.0/tests/test_show_4m.py
```

### Comparing `pyfii-1.4.0/LICENSE` & `pyfii-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfii-1.4.0/PKG-INFO` & `pyfii-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyfii
-Version: 1.4.0
+Version: 1.5.0
 Summary: 这个库可以让我们用python写Fii的无人机程序，有三视图模拟飞行的功能，模拟飞行更方便观看
-Author-email: Kevin0412 <kevin0412_xlt@qq.com>
+Author-email: Kevin0412 <kevin0412_xlt@qq.com>, miaooo0000OOOO <1683618861@qq.com>
 Project-URL: Homepage, https://github.com/Kevin0412/pyfii
 Project-URL: Bug Tracker, https://github.com/Kevin0412/pyfii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyfii
 
 ## 简介
 这个库的功能是可以让我们用python写Fii的无人机程序，以解决原软件无运算能力，无循环模块，一块块拖太烦等问题。
```

### Comparing `pyfii-1.4.0/README.md` & `pyfii-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfii-1.4.0/pyproject.toml` & `pyfii-1.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfii"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
   { name="Kevin0412", email="kevin0412_xlt@qq.com" },
+  { name="miaooo0000OOOO", email="1683618861@qq.com"}
 ]
 description = "这个库可以让我们用python写Fii的无人机程序，有三视图模拟飞行的功能，模拟飞行更方便观看"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `pyfii-1.4.0/src/pyfii/cv3d/IIID.py` & `pyfii-1.5.0/src/pyfii/cv3d/IIID.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.4.0/src/pyfii/cv3d/IIID2.py` & `pyfii-1.5.0/src/pyfii/cv3d/IIID2.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.4.0/src/pyfii/cv3d/transfer.py` & `pyfii-1.5.0/src/pyfii/cv3d/transfer.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.4.0/src/pyfii/read.py` & `pyfii-1.5.0/src/pyfii/read.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 import time
 import warnings
 
+def str2bgr(color):
+    return (int(color[5:7],16),int(color[3:5],16),int(color[1:3],16))
+
 def read_xml_points(data):
     data=data.split('\n')
     xml=[]
     n=0
     for d in data:
         n+=1
         #print(d.split('  ')[-1],str(len(d.split('  '))))
@@ -25,18 +28,21 @@
     for d in data:
         n+=1
         #print(d.split('  ')[-1],str(len(d.split('  '))))
         xml.append(d.split('  ')[-1])
         lenxml.append(len(d.split('  ')))
     dots=[]
     warns=[]
+    end=time
     for k in range(len(xml)):
         if xml[k][1:6]=='block':
             #print(xml[k].split('"')[1])
             if xml[k].split('"')[1][0:14]=='block_inittime':
+                if time>int(xml[k+1][19:21])*60000+int(xml[k+1][22:24])*1000:
+                    raise Warning("Block intime error.时间开始模块摆放错误")
                 time=int(xml[k+1][19:21])*60000+int(xml[k+1][22:24])*1000
                 #print(time)
             elif xml[k].split('"')[1][0:11]=='block_delay':
                 time+=int(xml[k+2][19:-8])
                 #print(time)
             elif xml[k].split('"')[1][0:19]=='Goertek_MoveToCoord':
                 if vel==0:
@@ -45,29 +51,33 @@
                 if acc==0:
                     acc=100
                     warns.append("Acceleration is not defined.Default 100cm/s^2.加速度未定义。默认100cm/s^2。")
                 x=int(xml[k+1][16:-8])
                 y=int(xml[k+2][16:-8])
                 #print(time,x,y,int(xml[k+3][16:-8]))
                 dots.append([time,x,y,int(xml[k+3][16:-8]),vel,acc,"move2"])
+                end=max(time,end)
             elif xml[k].split('"')[1][0:13]=='Goertek_Start':
                 if len(fii)==0:
                     x=int(xml[k].split('"')[3])
                     y=int(xml[k].split('"')[5])
                 else:
                     x=fii[0]
                     y=fii[1]
                 #print(time,x,y,0)
                 dots.append([time,x,y,0,200,400,"move2"])
+                end=max(time,end)
             elif xml[k].split('"')[1][0:15]=='Goertek_TakeOff':
                 #print(time,x,y,int(xml[k+1][18:-8]))
                 dots.append([time,x,y,int(xml[k+1][18:-8]),200,400,"move2"])
+                end=max(time,end)
             elif xml[k].split('"')[1][0:12]=='Goertek_Land':
                 #print(time,x,y,0)
                 dots.append([time,"land"])
+                end=max(time,end)
             elif xml[k].split('"')[1][0:23]=='Goertek_HorizontalSpeed':
                 vel=int(xml[k+1][17:-8])
                 acc=int(xml[k+2][17:-8])
             elif xml[k].split('"')[1][0:13]=='Goertek_Point':
                 points[xml[k+1][19:-8]]=[int(xml[k+2][16:-8]),int(xml[k+3][16:-8]),int(xml[k+4][16:-8])]
             elif xml[k].split('"')[1][0:19]=='Goertek_MoveToPoint':
                 if vel==0:
@@ -75,14 +85,15 @@
                     warns.append("Velcity is not defined.Default 60cm/s.速度未定义。默认60cm/s。")
                 if acc==0:
                     acc=100
                     warns.append("Acceleration is not defined.Default 100cm/s^2.加速度未定义。默认100cm/s^2。")
                 x=points[xml[k+1][20:-8]][0]
                 y=points[xml[k+1][20:-8]][1]
                 dots.append([time,x,y,points[xml[k+1][20:-8]][2],vel,acc,"move2"])
+                end=max(time,end)
             elif xml[k].split('"')[1][0:15]=='controls_repeat':
                 newxml=''
                 for g in range(k+3,len(lenxml)):
                     if lenxml[g]==lenxml[k+1]:
                         break
                     newxml+='  '*lenxml[g]+xml[g]
                     newxml+='\n'
@@ -91,91 +102,129 @@
                     repeat=read_xml(newxml*(int(xml[k+1][20:-8])-1),[],time,x,y,z,vel,acc,w,points)
                     #print(repeat[0])
                     for dot in repeat[0]:
                         dots.append(dot)
                     for warn in repeat[1]:
                         warns.append(warn)
                     time=repeat[2]
+                    end=repeat[3]
             elif xml[k].split('"')[1][0:12]=='Goertek_Move':
                 if vel==0:
                     vel=60
                     warns.append("Velcity is not defined.Default 60cm/s.速度未定义。默认60cm/s。")
                 if acc==0:
                     acc=100
                     warns.append("Acceleration is not defined.Default 100cm/s^2.加速度未定义。默认100cm/s^2。")
                 x=int(xml[k+1][16:-8])
                 y=int(xml[k+2][16:-8])
                 dots.append([time,x,y,int(xml[k+3][16:-8]),vel,acc,"move"])
+                end=max(time,end)
                 #raise Warning("Goertek_Move is not recommended.方向移动不建议使用。")
             elif xml[k].split('"')[1][0:14]=='Goertek_TurnTo':
                 if w==0:
                     w=60
                     warns.append("Arate is not defined.Default 60°/s.角速度未定义。默认60°/s。")
                 if xml[k+1][28]=='l':
                     angle=int(xml[k+2][20:-8])
                     dots.append([time,angle,w,"turn2"])
+                    end=max(time,end)
                 elif xml[k+1][28]=='r':
                     angle=-int(xml[k+2][20:-8])
                     dots.append([time,angle,w,"turn2"])
+                    end=max(time,end)
                 #print(angle)
             elif xml[k].split('"')[1][0:12]=='Goertek_Turn':
                 if w==0:
                     w=60
                     warns.append("Arate is not defined.Default 60°/s.角速度未定义。默认60°/s。")
                 if xml[k+1][28]=='l':
                     angle=int(xml[k+2][20:-8])
                 elif xml[k+1][28]=='r':
                     angle=-int(xml[k+2][20:-8])
                 dots.append([time,angle,w,"turn"])
+                end=max(time,end)
                 #print(angle)
             elif xml[k].split('"')[1][0:23]=='Goertek_AngularVelocity':
                 w=int(xml[k+1][16:-8])
                 #print(w)
-    return(dots,warns,time)
+            elif "Goertek_LEDTurnOnAllSingleColor" in xml[k]:
+                color = str2bgr(xml[k+1].split('>')[1].split('<')[0])
+                dots.append([time, color, 'TurnOnAllSingleColor'])
+                end=max(time,end)
+            elif "Goertek_LEDTurnOffAll" in xml[k]:
+                dots.append([time,'TurnOffAll'])
+                end=max(time,end)
+    return(dots,warns,time,end)
 
-def dots2angle(dots,warns,fps=200):#将指令转化为转圈动作
+def dots2angle(dots,warns,end,fps=200):#将指令转化为转圈动作
     time=0
     a=0
     w=60
     angle=0
     angles=[]
+    k=0
+    k1=0
     while(True):
-        k=-1
         for n in range(len(dots)):
-            if time-dots[n][0]>0:
-                k=n
+            if time-dots[n][0]>0 and dots[n][-1] in ['turn2','turn','turned']:
+                k1=n
+        k=k1
         if dots[k][-1]=='turn':
             angle=a+dots[k][1]
             w=dots[k][2]
+            dots[k][-1]='turned'
         elif dots[k][-1]=='turn2':
             angle=dots[k][1]%360
             a=a%360
             w=dots[k][2]
             if a-angle>180:
                 a-=360
             elif angle-a>180:
                 angle-=360
         w1=w/fps
         if abs(a-angle)>w1:
             a+=(angle-a)/abs(angle-a)*w1
         else:
             a=angle
         angles.append((time,float(a)))
-        if k==len(dots)-1:
+        if time>end:
             break
         time+=1000/fps
     return(angles)
 
+def dots2led(dots,warns,end,fps=200):#将指令转化为灯光
+    time=0
+    led=(-1,-1,-1)
+    leds=[]
+    k=0
+    k1=0
+    while(True):
+        for n in range(len(dots)):
+            if time-dots[n][0]>0 and dots[n][-1] in ['TurnOnAllSingleColor','TurnOffAll']:
+                k1=n
+        k=k1
+        if dots[k][-1]=='TurnOnAllSingleColor':
+            led=dots[k][1]
+        elif dots[k][-1]=='TurnOffAll':
+            led=(-1,-1,-1)
+        leds.append((time,led))
+        if time>end:
+            break
+        time+=1000/fps
+    return(leds)
+
+
 def dots2line(file,fii=[],fps=200,points={}):#将指令转换为飞行轨迹
-    dots,warns,time=read_xml(file,fii,points=points)
+    dots,warns,time,end=read_xml(file,fii,points=points)
     '''for dot in dots:
         print(dot)
     #print(dots,len(dots))
     #time.sleep(1000)'''
-    angles=dots2angle(dots,warns,fps)
+    angles=dots2angle(dots,warns,end,fps)
+    leds=dots2led(dots,warns,end,fps)
     '''for a in angles:
         print(a)'''
     x=float(dots[0][1])
     y=float(dots[0][2])
     z=float(dots[0][3])
     time=0
     #v=0
@@ -219,17 +268,22 @@
             vel=200
             acc=400
         alenth=vel**2/(2*acc)
         R=(X**2+Y**2+Z**2)**0.5
         if R==0:
             moving=False
             if len(lines)>=len(angles):
-                lines.append((time,x,y,z,angles[-1][1]))
+                angle=angles[-1][1]
+            else:
+                angle=angles[len(lines)][1]
+            if len(lines)>=len(leds):
+                led=leds[-1][1]
             else:
-                lines.append((time,x,y,z,angles[len(lines)][1]))
+                led=leds[len(lines)][1]
+            lines.append((time,x,y,z,angle,led))
             #print('\r'+str((time,x,y,z)),end='')
             a=0
         if a==0 and R!=0:#静止初始状态
             #Rs=[]
             ast=time/1000#action start time
             if R>=2*alenth:#距离是否大于全速加速减速的前进距离
                 slenth=alenth
@@ -246,17 +300,22 @@
                 if slow:
                     if v==0:
                         x=x1
                         y=y1
                         z=z1
                         #dots[k][-1]='moved'
                         if len(lines)>=len(angles):
-                            lines.append((time,x,y,z,angles[-1][1]))
+                            angle=angles[-1][1]
                         else:
-                            lines.append((time,x,y,z,angles[len(lines)][1]))
+                            angle=angles[len(lines)][1]
+                        if len(lines)>=len(leds):
+                            led=leds[-1][1]
+                        else:
+                            led=leds[len(lines)][1]
+                        lines.append((time,x,y,z,angle,led))
                         #print(time)
                         break
                     if v-400/fps>0:
                         r+=v/fps-200/(fps**2)
                         v-=400/fps
                     else:
                         r+=v**2/800
@@ -281,27 +340,37 @@
                         x+=float(dots[k][1])
                         y+=float(dots[k][2])
                         z+=float(dots[k][3])
                         dots[k][-1]='moved'
                     elif dots[k][-1]=='land':
                         z=0
                     if len(lines)>=len(angles):
-                        lines.append((time,x,y,z,angles[-1][1]))
+                        angle=angles[-1][1]
+                    else:
+                        angle=angles[len(lines)][1]
+                    if len(lines)>=len(leds):
+                        led=leds[-1][1]
                     else:
-                        lines.append((time,x,y,z,angles[len(lines)][1]))
+                        led=leds[len(lines)][1]
+                    lines.append((time,x,y,z,angle,led))
                     #print('\r'+str((time,x,y,z)),end='')
                     #print(time)
                     break
                 x1=x+r*X/R
                 y1=y+r*Y/R
                 z1=z+r*Z/R
                 if len(lines)>=len(angles):
-                    lines.append((time,x1,y1,z1,angles[-1][1]))
+                    angle=angles[-1][1]
+                else:
+                    angle=angles[len(lines)][1]
+                if len(lines)>=len(leds):
+                    led=leds[-1][1]
                 else:
-                    lines.append((time,x1,y1,z1,angles[len(lines)][1]))
+                    led=leds[len(lines)][1]
+                lines.append((time,x1,y1,z1,angle,led))
                 #print('\r'+str((time,x1,y1,z1)),end='')
                 time+=1000/fps
                 for n in range(len(dots)):
                     if time-dots[n][0]>0 and dots[n][-1] in ['move2','move','land','moved']:
                         if n-k>0:
                             #warnings.warn(str(int(time/100)/10)+"s:Action isn't completed.动作未完成。",Warning,3)
                             #raise Warning(str(int(time/100)/10)+"s:Action isn't completed.动作未完成。")
@@ -323,88 +392,108 @@
             y=dots[k][2]
             z=dots[k][3]
         else:
             x+=X/R*v
             y+=Y/R*v
             z+=Z/R*v
         #print(time/1000,x,y,z)'''
-        if k==len(dots)-1:
-            if len(dots[-1])>3:
-                if z==dots[-1][3]:
+        if k==len(dots)-1 or time>end:
+            m=-1
+            breakable=False
+            while True:
+                if dots[m][-1]=='land':
                     break
-            elif z==0:
+                if len(dots[m])>3:
+                    if z==dots[m][3]:
+                        breakable=True
+                    break
+                m-=1
+            if breakable:
+                break
+            if z==0:
                 break
         time+=1000/fps
     '''for t in range(10,120000,10):
         lines.append((time+t,x,y,z))'''
     return(lines,time*fps/1000,warns)
 
-def read_fii(name):
+def read_fii(path,getfeild=False,fps=200):
+    '''
+    读入.fii文件
+    path 所在文件夹的路径
+    '''
     time_start=time.time()
-    for root, dirs, files in os.walk(name):
+    for root, dirs, files in os.walk(path):
         for file in files:
             if os.path.splitext(file)[1] == '.fii':
-                fii_name=(os.path.join(root , file))
-    with open(fii_name, "r",encoding='utf-8') as F:
+                fii_path=(os.path.join(root , file))
+    with open(fii_path, "r",encoding='utf-8') as F:
         data = F.read()
     data=data.split('\n')
     xml=[]
     n=0
     for d in data:
         n+=1
         #print(d.split('  ')[-1],str(len(d.split('  '))))
         xml.append(d.split('  ')[-1])
     drones=[]
-    music=[name+"/动作组/"]
+    music=[path+"/动作组/"]
     for k in range(len(xml)):
         #print(xml[k].split('"'))
         if xml[k][1:10]=='MusicName':
             music.append(xml[k].split('"')[1])
         if xml[k][1:8]=='Actions':
             #print(xml[k].split('"')[1][0])
             drones.append(xml[k].split('"')[1])
+        if xml[k][1:6]=='AreaL':
+            feild=int(xml[k].split('"')[1][0])
+    if len(music)==1:
+        music=[]
     dots=[]
     t0=0
     n=0
     points={}
     for drone in drones:
-        with open(name+'/动作组/'+drone+'/webCodeAll.xml', "r",encoding='utf-8') as F:
+        with open(path+'/动作组/'+drone+'/webCodeAll.xml', "r",encoding='utf-8') as F:
             file = F.read()
         for dic in read_xml_points(file).items():
             points[dic[0]]=dic[1]
     for drone in drones:
         for k in range(len(xml)):
             if xml[k][1:16]=='ActionFlightPos' and xml[k].split('"')[1][0:4]==drone:
                 if xml[k][16]=='X':
                     x=int(xml[k].split('"')[1].split('pos')[1])
                 elif xml[k][16]=='Y':
                     y=int(xml[k].split('"')[1].split('pos')[1])
                 #print(xml[k].split('"')[1])
-        with open(name+'/动作组/'+drone+'/webCodeAll.xml', "r",encoding='utf-8') as F:
+        with open(path+'/动作组/'+drone+'/webCodeAll.xml', "r",encoding='utf-8') as F:
             file = F.read()
         try:
-            line=dots2line(file,fii=[x,y],points=points)
+            line=dots2line(file,fii=[x,y],fps=fps,points=points)
             '''with open(name+'/动作组/'+drone+'line.csv','w',encoding='utf-8') as F:
                 F.write('time,x,y,z,angle\n')
                 for l in line[0]:
                     for li in l:
                         F.write(str(li))
                         F.write(',')
                     F.write('\n')'''
         except:
-            raise Warning('No take off place.起飞位置未定义。')
+            raise Exception('No take off place.起飞位置未定义。')
         dots.append(line[0])
         t0=max(t0,line[1])
         n+=1
         if len(line[2])>0:
             for warn in line[2]:
                 warnings.warn('d'+str(n)+' 无人机'+str(n)+':'+warn,Warning,2)
         print('\r'+str(n)+'/'+str(len(drones)),end='')
     print('\n读取文件与轨迹计算耗时：'+str(int((time.time()-time_start)*1000+0.5)/1000)+'秒')
-    return dots,t0,music
+    if getfeild:
+        return dots,t0,music,feild
+    else:
+        return dots,t0,music
 
 '''def read_py(fii):
     time_start=time.time()
     dots=[]
     t0=0
     n=0
     for d in fii.ds:
@@ -414,8 +503,8 @@
         n+=1
         if len(line[2])>0:
             for warn in line[2]:
                 warnings.warn('d'+str(n)+':'+warn,Warning,2)
         print('\r'+str(n)+'/'+str(len(fii.ds)),end='')
     print('\n轨迹计算耗时：'+str(int((time.time()-time_start)*1000+0.5)/1000)+'秒')
     return dots,t0'''
-    
+
```

### Comparing `pyfii-1.4.0/src/pyfii/show.py` & `pyfii-1.5.0/src/pyfii/show.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+import cmath
 import os
 import time
 import uuid
 import warnings
+import shutil
 
 import cv2
 import numpy as np
 import pygame
 from ffmpy import FFmpeg
 
-from .cv3d import IIID,IIID2
+from .cv3d import IIID, IIID2
+
 
 # 视频添加音频
 def video_add_audio(video_path: str, audio_path: str,output_path:str):
     _ext_video = os.path.basename(video_path).strip().split('.')[-1]
     _ext_audio = os.path.basename(audio_path).strip().split('.')[-1]
     if _ext_audio not in ['mp3', 'wav']:
-        raise Exception('audio format not support')
-    _codec = 'copy'
-    if _ext_audio == 'wav':
-        _codec = 'aac'
-    result =output_path.format(uuid.uuid4(), _ext_video)
-    ff = FFmpeg(
-        inputs={video_path: None, audio_path: None},
-        outputs={result: '-map 0:v -map 1:a -c:v copy -c:a {} -shortest'.format(_codec)})
-    print(ff.cmd)
-    ff.run()
-    return result
+        print('No music!')
+        shutil.copy(video_path,video_path[0:-12]+'.mp4')
+    else:
+        _codec = 'copy'
+        if _ext_audio == 'wav':
+            _codec = 'aac'
+        result =output_path.format(uuid.uuid4(), _ext_video)
+        ff = FFmpeg(
+            inputs={video_path: None, audio_path: None},
+            outputs={result: '-map 0:v -map 1:a -c:v copy -c:a {} -shortest'.format(_codec)})
+        print(ff.cmd)
+        ff.run()
+        return result
 
 '''def nothing(x):
     pass'''
 
 def color(n,m=0):
     n=180-n*180/7
     if m>0:
@@ -39,50 +44,90 @@
         n=(-abs(n))%180
         h,s,v=int(n),255,int(255+m)
     img=np.zeros((1,1,3),np.uint8)
     img[0][0]=(h,s,v)
     img=cv2.cvtColor(img,cv2.COLOR_HSV2BGR)
     return(int(img[0][0][0]),int(img[0][0][1]),int(img[0][0][2]))
 
-def draw_drone(img,x,y,color,a=0,up=False):
-    if up:
-        cv2.circle(img,(int(x-21/2*np.cos(np.pi/4+a)),int(y+21/2*np.sin(np.pi/4+a))),8,color,1)
-        cv2.circle(img,(int(x-21/2*np.cos(3*np.pi/4+a)),int(y+21/2*np.sin(3*np.pi/4+a))),8,color,1)
-        cv2.circle(img,(int(x-21/2*np.cos(-3*np.pi/4+a)),int(y+21/2*np.sin(-3*np.pi/4+a))),8,color,1)
-        cv2.circle(img,(int(x-21/2*np.cos(-np.pi/4+a)),int(y+21/2*np.sin(-np.pi/4+a))),8,color,1)
-        cv2.line(img,(int(x-21/2*np.cos(np.pi/4+a)),int(y+21/2*np.sin(np.pi/4+a))),(int(x-21/2*np.cos(-3*np.pi/4+a)),int(y+21/2*np.sin(-3*np.pi/4+a))),color,1)
-        cv2.line(img,(int(x-21/2*np.cos(-np.pi/4+a)),int(y+21/2*np.sin(-np.pi/4+a))),(int(x-21/2*np.cos(3*np.pi/4+a)),int(y+21/2*np.sin(3*np.pi/4+a))),color,1)
-    else:
-        cv2.ellipse(img,(int(x+21/(2**0.5)/2),int(y-1/4*7.6)),(8,2),0,0,360,color,1)
-        cv2.ellipse(img,(int(x-21/(2**0.5)/2),int(y-1/4*7.6)),(8,2),0,0,360,color,1)
-        cv2.ellipse(img,(int(x-21/(2**0.5)/2),int(y-3/4*7.6)),(8,2),0,0,360,color,1)
-        cv2.ellipse(img,(int(x+21/(2**0.5)/2),int(y-3/4*7.6)),(8,2),0,0,360,color,1)
-        cv2.line(img,(int(x+21/(2**0.5)/2),int(y-1/4*7.6)),(int(x-21/(2**0.5)/2),int(y-3/4*7.6)),color,1)
-        cv2.line(img,(int(x-21/(2**0.5)/2),int(y-1/4*7.6)),(int(x+21/(2**0.5)/2),int(y-3/4*7.6)),color,1)
+def draw_drone(img,x,y,color,a=0,led=(-1,-1,-1),up=False,skin=1):
+    if skin==0:
+        if up:
+            cv2.circle(img,(int(x),int(y)),15,color,-1)
+        else:
+            cv2.rectangle(img,(int(x)-15,int(y)+5),(int(x)+15,int(y)-5),color,-1)
+    elif skin==1:
+        if up:
+            cv2.circle(img,(int(x-21/2*np.cos(np.pi/4+a)),int(y+21/2*np.sin(np.pi/4+a))),8,color,1)
+            cv2.circle(img,(int(x-21/2*np.cos(3*np.pi/4+a)),int(y+21/2*np.sin(3*np.pi/4+a))),8,color,1)
+            cv2.circle(img,(int(x-21/2*np.cos(-3*np.pi/4+a)),int(y+21/2*np.sin(-3*np.pi/4+a))),8,color,1)
+            cv2.circle(img,(int(x-21/2*np.cos(-np.pi/4+a)),int(y+21/2*np.sin(-np.pi/4+a))),8,color,1)
+            cv2.line(img,(int(x-21/2*np.cos(np.pi/4+a)),int(y+21/2*np.sin(np.pi/4+a))),(int(x-21/2*np.cos(-3*np.pi/4+a)),int(y+21/2*np.sin(-3*np.pi/4+a))),color,1)
+            cv2.line(img,(int(x-21/2*np.cos(-np.pi/4+a)),int(y+21/2*np.sin(-np.pi/4+a))),(int(x-21/2*np.cos(3*np.pi/4+a)),int(y+21/2*np.sin(3*np.pi/4+a))),color,1)
+            if led[0]>-1:
+                cv2.circle(img,(int(x),int(y)),5,led,-1)
+        else:
+            cv2.ellipse(img,(int(x+21/(2**0.5)/2),int(y-1/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.ellipse(img,(int(x-21/(2**0.5)/2),int(y-1/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.ellipse(img,(int(x-21/(2**0.5)/2),int(y-3/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.ellipse(img,(int(x+21/(2**0.5)/2),int(y-3/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.line(img,(int(x+21/(2**0.5)/2),int(y-1/4*7.6)),(int(x-21/(2**0.5)/2),int(y-3/4*7.6)),color,1)
+            cv2.line(img,(int(x-21/(2**0.5)/2),int(y-1/4*7.6)),(int(x+21/(2**0.5)/2),int(y-3/4*7.6)),color,1)
+            if led[0]>-1:
+                cv2.circle(img,(int(x),int(y-1/2*7.6)),5,led,-1)
+    elif skin==2:
+        if up:
+            red_square=np.array([[x+16*np.cos(a),y+16*np.sin(a)],[x+16*np.cos(a+np.pi/2),y+16*np.sin(a+np.pi/2)],[x+16*np.cos(a+np.pi),y+16*np.sin(a+np.pi)],[x+16*np.cos(a-np.pi/2),y+16*np.sin(a-np.pi/2)]],np.int32)
+            fu=[np.array([[x+((-7-6j)*cmath.e**(a*1j)).real,y+((-7-6j)*cmath.e**(a*1j)).imag],[x+((-6-5j)*cmath.e**(a*1j)).real,y+((-6-5j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-8-2j)*cmath.e**(a*1j)).real,y+((-8-2j)*cmath.e**(a*1j)).imag],[x+((-5-3j)*cmath.e**(a*1j)).real,y+((-5-3j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-5-3j)*cmath.e**(a*1j)).real,y+((-5-3j)*cmath.e**(a*1j)).imag],[x+((-8+3j)*cmath.e**(a*1j)).real,y+((-8+3j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-6-0j)*cmath.e**(a*1j)).real,y+((-6-0j)*cmath.e**(a*1j)).imag],[x+((-6+6j)*cmath.e**(a*1j)).real,y+((-6+6j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-6+1j)*cmath.e**(a*1j)).real,y+((-6+1j)*cmath.e**(a*1j)).imag],[x+((-5+2j)*cmath.e**(a*1j)).real,y+((-5+2j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-3-5j)*cmath.e**(a*1j)).real,y+((-3-5j)*cmath.e**(a*1j)).imag],[x+((5-5j)*cmath.e**(a*1j)).real,y+((5-5j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-2-3j)*cmath.e**(a*1j)).real,y+((-2-3j)*cmath.e**(a*1j)).imag],[x+((4-3j)*cmath.e**(a*1j)).real,y+((4-3j)*cmath.e**(a*1j)).imag],
+            [x+((4-1j)*cmath.e**(a*1j)).real,y+((4-1j)*cmath.e**(a*1j)).imag],[x+((-2-1j)*cmath.e**(a*1j)).real,y+((-2-1j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-3+1j)*cmath.e**(a*1j)).real,y+((-3+1j)*cmath.e**(a*1j)).imag],[x+((5+1j)*cmath.e**(a*1j)).real,y+((5+1j)*cmath.e**(a*1j)).imag],
+            [x+((5+5j)*cmath.e**(a*1j)).real,y+((5+5j)*cmath.e**(a*1j)).imag],[x+((-3+5j)*cmath.e**(a*1j)).real,y+((-3+5j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((-3+3j)*cmath.e**(a*1j)).real,y+((-3+3j)*cmath.e**(a*1j)).imag],[x+((5+3j)*cmath.e**(a*1j)).real,y+((5+3j)*cmath.e**(a*1j)).imag]],np.int32),
+            np.array([[x+((1+1j)*cmath.e**(a*1j)).real,y+((1+1j)*cmath.e**(a*1j)).imag],[(x+(1+5j)*cmath.e**(a*1j)).real,y+((1+5j)*cmath.e**(a*1j)).imag]],np.int32)]
+            img=cv2.fillPoly(img,[red_square],color=[0,0,255])
+            img=cv2.polylines(img,fu,isClosed=True,color=[0,0,0],thickness=1)
+        else:
+            cv2.ellipse(img,(int(x+21/(2**0.5)/2),int(y-1/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.ellipse(img,(int(x-21/(2**0.5)/2),int(y-1/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.ellipse(img,(int(x-21/(2**0.5)/2),int(y-3/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.ellipse(img,(int(x+21/(2**0.5)/2),int(y-3/4*7.6)),(8,2),0,0,360,color,1)
+            cv2.line(img,(int(x+21/(2**0.5)/2),int(y-1/4*7.6)),(int(x-21/(2**0.5)/2),int(y-3/4*7.6)),color,1)
+            cv2.line(img,(int(x-21/(2**0.5)/2),int(y-1/4*7.6)),(int(x+21/(2**0.5)/2),int(y-3/4*7.6)),color,1)
+            if led[0]>-1:
+                cv2.circle(img,(int(x),int(y-1/2*7.6)),5,led,-1)
 
-def drone3d(aixs,x,y,z,c,a):
+def drone3d(aixs,x,y,z,c,a,led=(-1,-1,-1)):
     aixs.append([(x+21/2*np.cos(np.pi/4+a),y+21/2*np.sin(np.pi/4+a),z),c,(14.9-21/4*2**0.5),1,'ring'])
     aixs.append([(x+21/2*np.cos(3*np.pi/4+a),y+21/2*np.sin(3*np.pi/4+a),z),c,(14.9-21/4*2**0.5),1,'ring'])
     aixs.append([(x+21/2*np.cos(-3*np.pi/4+a),y+21/2*np.sin(-3*np.pi/4+a),z),c,(14.9-21/4*2**0.5),1,'ring'])
     aixs.append([(x+21/2*np.cos(-np.pi/4+a),y+21/2*np.sin(-np.pi/4+a),z),c,(14.9-21/4*2**0.5),1,'ring'])
     aixs.append([(x+21/2*np.cos(np.pi/4+a),y+21/2*np.sin(np.pi/4+a),z),(x+21/2*np.cos(-3*np.pi/4+a),y+21/2*np.sin(-3*np.pi/4+a),z),c,1,8,'line'])
     aixs.append([(x+21/2*np.cos(-np.pi/4+a),y+21/2*np.sin(-np.pi/4+a),z),(x+21/2*np.cos(3*np.pi/4+a),y+21/2*np.sin(3*np.pi/4+a),z),c,1,8,'line'])
+    if led[0]>-1:
+        aixs.append([(x,y,z),led,5,-1,'sphere'])
+    else:
+        aixs.append([(x,y,z),c,1,-1,'sphere'])
 
 '''def color(n):
     n=n*180/7
     x=255
     if int((n%765)/255)==0:
         return(255-n%255,n%255,x)
     if int((n%765)/255)==1:
         return(n%255,x,255-n%255)
     if int((n%765)/255)==2:
         return(x,255-n%255,n%255)'''
 
-def show(data,t0,music,show=True,save="",FPS=200,ThreeD=False,imshow=[120,-15],d=(600,450),track=[]):
-    t0=int(t0+0.5)+300
+def show(data,t0,music,feild=6,show=True,save="",FPS=200,max_fps=200,ThreeD=False,imshow=[120,-15],d=(600,450),track=[],skin=1):
+    t0=int(t0+0.5)+3*max_fps
     if len(save)>0 and not ThreeD:
         show=False
         video = cv2.VideoWriter(save+"_process.mp4", cv2.VideoWriter_fourcc('M', 'P', '4', 'V'), FPS,(1200,600))
     if len(save)>0 and ThreeD:
         if len(track)==0:
             video = cv2.VideoWriter(save+"_process.mp4", cv2.VideoWriter_fourcc('M', 'P', '4', 'V'), FPS,(1280,720))
         else:
@@ -115,42 +160,69 @@
             else:
                 for x in range(150):
                     cv2.rectangle(img,(600+(a-4)*150+x,570),(600+(a-4)*150+x,600),color(a,(x-75)/75*125),-1)
         for x in range(4):
             cv2.rectangle(img,(600+x*150,540),(750+x*150,570),(255,255,255),1)
             cv2.rectangle(img,(600+x*150,570),(750+x*150,600),(255,255,255),1)
         cv2.rectangle(img,(1120,570),(1200,600),(255,255,255),1)
+        if feild==4:
+            cv2.rectangle(img,(20,580),(380,220),(255,255,255),1)
+            cv2.rectangle(img,(1000,0),(1000,540),(255,255,255),1)
         font=cv2.FONT_HERSHEY_SIMPLEX
         cv2.putText(img,'front',(600,260), font, 1,(255,255,255),1)
         cv2.putText(img,'right',(600,530), font, 1,(255,255,255),1)
         cv2.imwrite('gui.png',img)
         #生成可视化界面↑
     if ThreeD:
-        center=(280,280,165)#三维渲染旋转中心
+        if feild==6:
+            center=(280,280,165)#三维渲染旋转中心
+        if feild==4:
+            center=(180,180,165)#三维渲染旋转中心
         lines=[]#三维渲染的线
-        lines.append([(0,0,0),(600,0,0),(0,0,255),1,8,'line'])
-        lines.append([(0,0,0),(0,600,0),(0,255,0),1,8,'line'])
-        lines.append([(0,0,0),(0,0,300),(255,0,0),1,8,'line'])
+        if feild==6:
+            lines.append([(-20,-20,0),(580,-20,0),(0,0,255),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,580,0),(0,255,0),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,-20,300),(255,0,0),1,8,'line'])
+            lines.append([(-20,-20,0),(580,-20,0),(0,0,255),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,580,0),(0,255,0),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,-20,300),(255,0,0),1,8,'line'])
+            lines.append([(0,0,0),(560,0,0),(255,255,255),1,8,'line'])
+            lines.append([(0,0,0),(0,560,0),(255,255,255),1,8,'line'])
+            lines.append([(0,560,0),(560,560,0),(255,255,255),1,8,'line'])
+            lines.append([(560,0,0),(560,560,0),(255,255,255),1,8,'line'])
+        if feild==4:
+            lines.append([(-20,-20,0),(380,-20,0),(0,0,255),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,380,0),(0,255,0),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,-20,300),(255,0,0),1,8,'line'])
+            lines.append([(-20,-20,0),(380,-20,0),(0,0,255),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,380,0),(0,255,0),1,8,'line'])
+            lines.append([(-20,-20,0),(-20,-20,300),(255,0,0),1,8,'line'])
+            lines.append([(0,0,0),(360,0,0),(255,255,255),1,8,'line'])
+            lines.append([(0,0,0),(0,360,0),(255,255,255),1,8,'line'])
+            lines.append([(0,360,0),(360,360,0),(255,255,255),1,8,'line'])
+            lines.append([(360,0,0),(360,360,0),(255,255,255),1,8,'line'])
         for x in range(1,57):
+            if feild==4 and x>36:
+                break
             if x%10==5:
-                lines.append([(x*10,0,0),(x*10,40,40),(255,255,0),1,8,'line'])
-                lines.append([(0,x*10,0),(40,x*10,40),(255,0,255),1,8,'line'])
+                lines.append([(x*10,-20,0),(x*10,20,40),(255,255,0),1,8,'line'])
+                lines.append([(-20,x*10,0),(20,x*10,40),(255,0,255),1,8,'line'])
             elif x%10==0:
-                lines.append([(x*10,0,0),(x*10,50,50),(255,255,0),1,8,'line'])
-                lines.append([(0,x*10,0),(50,x*10,50),(255,0,255),1,8,'line'])
+                lines.append([(x*10,-20,0),(x*10,30,50),(255,255,0),1,8,'line'])
+                lines.append([(-20,x*10,0),(30,x*10,50),(255,0,255),1,8,'line'])
             else:
-                lines.append([(x*10,0,0),(x*10,30,30),(255,255,0),1,8,'line'])
-                lines.append([(0,x*10,0),(30,x*10,30),(255,0,255),1,8,'line'])
+                lines.append([(x*10,-20,0),(x*10,10,30),(255,255,0),1,8,'line'])
+                lines.append([(-20,x*10,0),(10,x*10,30),(255,0,255),1,8,'line'])
         for x in range(8,26):
             if x%10==5:
-                lines.append([(0,0,x*10),(40,40,x*10),(0,255,255),1,8,'line'])
+                lines.append([(-20,-20,x*10),(20,20,x*10),(0,255,255),1,8,'line'])
             elif x%10==0:
-                lines.append([(0,0,x*10),(50,50,x*10),(0,255,255),1,8,'line'])
+                lines.append([(-20,-20,x*10),(30,30,x*10),(0,255,255),1,8,'line'])
             else:
-                lines.append([(0,0,x*10),(30,30,x*10),(0,255,255),1,8,'line'])
+                lines.append([(-20,-20,x*10),(10,10,x*10),(0,255,255),1,8,'line'])
         i=imshow[0]
     if (show and len(save)==0) or (ThreeD and len(save)==0):
         if len(music)>1:
             for root, dirs, files in os.walk(music[0]):
                 for file in files:
                     if os.path.splitext(file)[0]==music[1]:
                         music_name=(os.path.join(root , file))
@@ -176,42 +248,44 @@
             for a in range(len(data)):
                 if len(data[a])>k:
                     t=max(t,data[a][k][0]/1000)
                     x=data[a][k][1]
                     y=data[a][k][2]
                     z=data[a][k][3]
                     angle=data[a][k][4]
+                    led=data[a][k][5]
                 else:
                     t=max(t,data[a][-1][0]/1000)
                     x=data[a][-1][1]
                     y=data[a][-1][2]
                     z=data[a][-1][3]
                     angle=data[a][-1][4]
+                    led=data[a][-1][5]
                 '''cv2.circle(img2,(x,560-y),15,color(a),-1)
                 cv2.rectangle(img2,(560+x-15,250-z+5),(560+x+15,250-z-5),color(a),-1)
                 cv2.rectangle(img2,(560+y-15,500-z+5),(560+y+15,500-z-5),color(a),-1)'''
                 if (show or len(save)>0) and not ThreeD:
                     if a<4:
                         cv2.putText(img2,str(a+1)+' ('+str(int(x*1+0.5))+','+str(int(y*1+0.5))+','+str(int(z*1+0.5))+')',(600+a*150,560), font, 0.5,(255,255,255),1)
                     else:
                         cv2.putText(img2,str(a+1)+' ('+str(int(x*1+0.5))+','+str(int(y*1+0.5))+','+str(int(z*1+0.5))+')',(a*150,590), font, 0.5,(255,255,255),1)#在img2上画出无人机的位置并显示坐标
-                aixs.append((x,y,z,angle,a))
+                aixs.append((x,y,z,angle,led,a))
         if (show or len(save)>0) and not ThreeD:
             Xs=sorted(aixs,key=lambda x:x[0])
             Ys=sorted(aixs,key=lambda x:x[1],reverse=True)
             Zs=sorted(aixs,key=lambda x:x[2])
             #根据距离远近渲染
             for X in Xs:
-                draw_drone(img2,620+X[1],540-X[2],color(X[4],(X[0]-280)/280*125))
+                draw_drone(img2,620+X[1],540-X[2],color(X[5],(X[0]-280)/280*125),led=X[4],skin=skin)
                 #cv2.rectangle(img2,(int(560+X[1]-15),int(500-X[2]+5)),(int(560+X[1]+15),int(500-X[2]-5)),color(X[3],(X[0]-280)/280*125),-1)
             for Y in Ys:
-                draw_drone(img2,620+Y[0],270-Y[2],color(Y[4],(Y[1]-280)/280*125))
+                draw_drone(img2,620+Y[0],270-Y[2],color(Y[5],(280-Y[1])/280*125),led=Y[4],skin=skin)
                 #cv2.rectangle(img2,(int(560+Y[0]-15),int(250-Y[2]+5)),(int(560+Y[0]+15),int(250-Y[2]-5)),color(Y[3],(280-Y[1])/280*125),-1)
             for Z in Zs:
-                draw_drone(img2,20+Z[0],580-Z[1],color(Z[4],(Z[2]-125)/125*125),a=Z[3]/180*np.pi,up=True)
+                draw_drone(img2,20+Z[0],580-Z[1],color(Z[5],(Z[2]-125)/125*125),a=Z[3]/180*np.pi,led=Z[4],up=True,skin=skin)
                 #cv2.circle(img2,(Z[0],560-Z[1]),15,color(Z[3],(Z[2]-125)/125*125),-1)
         #print(Xs)
         #print(aixs)
         if not ThreeD:
             for m in range(len(aixs)):
                 for n in range(m+1,len(aixs)):#计算距离
                     distance=((aixs[m][0]-aixs[n][0])**2+(aixs[m][1]-aixs[n][1])**2)**0.5
@@ -222,28 +296,28 @@
                             cv2.circle(img2,(int(20+aixs[m][0]),int(580-aixs[m][1])),20,(0,0,255),3)
                             cv2.circle(img2,(int(620+aixs[m][0]),int(270-aixs[m][2])),20,(0,0,255),3)
                             cv2.circle(img2,(int(620+aixs[m][1]),int(540-aixs[m][2])),20,(0,0,255),3)
                             cv2.circle(img2,(int(20+aixs[n][0]),int(580-aixs[n][1])),20,(0,0,255),3)
                             cv2.circle(img2,(int(620+aixs[n][0]),int(270-aixs[n][2])),20,(0,0,255),3)
                             cv2.circle(img2,(int(620+aixs[n][1]),int(540-aixs[n][2])),20,(0,0,255),3)#错误红点标记
         if (show or len(save)>0) and not ThreeD:
-            cv2.putText(img2,str(t),(1050,590),font,0.5,(255,255,255),1)#在img2上显示时间
+            cv2.putText(img2,str(int(t*1000)/1000),(1050,590),font,0.5,(255,255,255),1)#在img2上显示时间
         time_fps=time.time()
         if len(save)==0 and show or (ThreeD and len(save)==0):
-            k=int((time_fps-time_read)*200)
+            k=int((time_fps-time_read)*max_fps)
         if show and not ThreeD:
             f+=1
             if f==1:
                 time_fps=time.time()
                 try:
                     fps=str(int(10/(time_fps-time_FPS)+0.5)/10)
                     fs=int(float(fps)/10+0.5)*10
                 except:
-                    fps='200.0'
-                    fs=200
+                    fps=str(float(max_fps))
+                    fs=max_fps
                 if fs==0:
                     fs=10
             elif f%fs==0:
                 fps=str(int(fs*10/(time_fps-time_FPS)+0.5)/10)
                 time_FPS=time_fps
         if len(save)>0:
             fps=str(int(FPS*10+0.5)/10)
@@ -258,68 +332,70 @@
             #Esc键退出
             if key == 27:
                 break
             elif key==32:#空格暂停
                 if len(music)>0:
                     pygame.mixer.music.stop()
                 cv2.waitKey(0)
-                time_read=time.time()-k/200
+                time_read=time.time()-k/max_fps
                 if len(music)>0:
-                    pygame.mixer.music.play(start=k/200)
+                    pygame.mixer.music.play(start=k/max_fps)
             elif key==ord('q'):#后退
-                k-=100
+                k-=max_fps
                 #time_read+=0.5
                 if time_read>time_fps:
                     time_read=time_fps
                 if k<0:
                     k=0
                 if len(music)>0:
                     pygame.mixer.music.stop()
                 cv2.waitKey(0)
-                time_read=time.time()-k/200
+                time_read=time.time()-k/max_fps
                 if len(music)>0:
-                    pygame.mixer.music.play(start=k/200)
+                    pygame.mixer.music.play(start=k/max_fps)
             elif key==ord('e'):#快进
                 #time_read-=0.5
-                k+=100
+                k+=max_fps
                 if len(music)>0:
                     pygame.mixer.music.stop()
                 cv2.waitKey(0)
-                time_read=time.time()-k/200
+                time_read=time.time()-k/max_fps
                 if len(music)>0:
-                    pygame.mixer.music.play(start=k/200)
+                    pygame.mixer.music.play(start=k/max_fps)
             #time_read-=t-cv2.getTrackbarPos('time','img')
         #print('\r'+str(t)+'/'+str((t0-300)/100)+'  ',end='')
         
         if ThreeD:
             texts=[]#显示的文字
             t=0
             for a in range(len(data)):
                 if len(data[a])>k:
                     t=max(t,data[a][k][0]/1000)
                     x=data[a][k][1]
                     y=data[a][k][2]
                     z=data[a][k][3]
                     angle=data[a][k][4]
+                    led=data[a][k][5]
                 else:
                     t=max(t,data[a][-1][0]/1000)
                     x=data[a][-1][1]
                     y=data[a][-1][2]
                     z=data[a][-1][3]
                     angle=data[a][-1][4]
+                    led=data[a][-1][5]
                 c=color(a)
                 #aixs.append([(x,y,z),c,5,1,'ring'])
                 #drone.append([x,y,z,c])
-                drone3d(aixs,x,y,z,color(a,127),angle/180*np.pi)
+                drone3d(aixs,x,y,z,color(a,127),angle/180*np.pi,led)
                 drone3d(aixs,x,y,0,color(a,-127),angle/180*np.pi)
                 texts.append([str(a+1)+'('+str(int(x+0.5))+','+str(int(y+0.5))+','+str(int(z+0.5))+')',(0,140+30*a),0.5,c,1,'text'])
-            texts.append(['T+'+str(t),(0,80),0.5,(255,255,255),1,'text'])
+            texts.append(['T+'+str(int(t*1000)/1000),(0,80),0.5,(255,255,255),1,'text'])
             errors=[]#圈出错误的飞机
-            for m in range(0,len(aixs),12):
-                for n in range(m+12,len(aixs),12):#计算距离
+            for m in range(0,len(aixs),14):
+                for n in range(m+14,len(aixs),14):#计算距离
                     distance=((aixs[m][0][0]-aixs[n][0][0]+aixs[m+2][0][0]-aixs[n+2][0][0])**2+(aixs[m][0][1]-aixs[n][0][1]+aixs[m+2][0][1]-aixs[n+2][0][1])**2)**0.5/2
                     if distance<51:
                         warnings.warn('In '+str(int(t))+'s,distance between d'+str(int(m/12+1))+' and d'+str(int(n/12+1))+' is less than '+str((int(distance/17)+1)*17)+'cm.在'+str(int(t))+'秒，无人机'+str(int(m/12+1))+'和无人机'+str(int(n/12+1))+'之间的距离小于'+str((int(distance/17)+1)*17)+'厘米。',Warning,2)
                         #print(t,distance,int(distance/20),m+1,n+1)#距离太近就输出错误
                         if len(track)==0:
                             errors.append([((aixs[m][0][0]+aixs[m+2][0][0])/2,(aixs[m][0][1]+aixs[m+2][0][1])/2,aixs[m][0][2]),(0,0,255),10,1,'sphere'])#错误红圈标记
                             errors.append([((aixs[n][0][0]+aixs[n+2][0][0])/2,(aixs[n][0][1]+aixs[n+2][0][1])/2,aixs[n][0][2]),(0,0,255),10,1,'sphere'])
@@ -330,16 +406,16 @@
             f+=1
             if f==1:
                 time_fps=time.time()
                 try:
                     fps=str(int(10/(time_fps-time_FPS)+0.5)/10)
                     fs=int(float(fps)/10+0.5)*10
                 except:
-                    fps='200.0'
-                    fs=200
+                    fps=str(float(max_fps))
+                    fs=max_fps
                 if fs==0:
                     fs=10
             elif f%fs==0:
                 fps=str(int(fs*10/(time_fps-time_FPS)+0.5)/10)
                 time_FPS=time_fps
             if len(save)>0:
                 fps=str(int(FPS*10+0.5)/10)
@@ -366,52 +442,52 @@
                 #Esc键退出
                 if key == 27:
                     break
                 elif key==32:#长按空格键暂停，暂停后可以按wasd旋转，按esc退出暂停
                     if len(music)>0:
                         pygame.mixer.music.stop()
                     imshow[0],imshow[1]=IIID.show(aixs+lines+errors+texts,center,1280,720,[imshow[0],imshow[1],1],d)
-                    i=imshow[0]-int(k/200*36+0.5)
-                    time_read=time.time()-k/200
+                    i=imshow[0]-int(k/max_fps*36+0.5)
+                    time_read=time.time()-k/max_fps
                     if len(music)>0:
-                        pygame.mixer.music.play(start=k/200)
+                        pygame.mixer.music.play(start=k/max_fps)
                 elif key==ord('q'):#后退
-                    k-=200
+                    k-=max_fps
                     #time_read+=0.5
                     if time_read>time_fps:
                         time_read=time_fps
                     if k<0:
                         k=0
                     if len(music)>0:
                         pygame.mixer.music.stop()
                     cv2.waitKey(0)
-                    time_read=time.time()-k/200
+                    time_read=time.time()-k/max_fps
                     if len(music)>0:
-                        pygame.mixer.music.play(start=k/200)
+                        pygame.mixer.music.play(start=k/max_fps)
                 elif key==ord('e'):#快进
-                    k+=200
+                    k+=max_fps
                     if len(music)>0:
                         pygame.mixer.music.stop()
                     cv2.waitKey(0)
-                    time_read=time.time()-k/200
+                    time_read=time.time()-k/max_fps
                     if len(music)>0:
-                        pygame.mixer.music.play(start=k/200)
+                        pygame.mixer.music.play(start=k/max_fps)
             
         if not show and len(save)==0 and not ThreeD:
             k+=1
         if len(save)>0:
             if ThreeD:
                 video.write(img)
             else:
                 video.write(img2)
-            K+=200/FPS
+            K+=max_fps/FPS
             k=int(K+0.5)
     if (show and len(save)==0) or (ThreeD and len(save)==0):
         cv2.destroyAllWindows()
-        if len(music)>0:
+        if len(music)>1 or (len(music)==1 and music[0].split('.')[-1] in ['mp3','wav']):
             pygame.mixer.music.stop()
     timer=time.time()-time_read
     print('平均帧率：'+str(int(10*f/timer+0.5)/10))
     print('飞行总时间：'+str(int((time.time()-time_read)*1000+0.5)/1000)+'秒')
     if len(save)>0:
         print('视频保存中')
         video.release()#储存视频
@@ -420,15 +496,17 @@
             for root, dirs, files in os.walk(music[0]):
                 for file in files:
                     if os.path.splitext(file)[0]==music[1]:
                         music_name=(os.path.join(root , file))
             if os.path.exists(save+'.mp4'):
                 os.remove(save+'.mp4')
             video_add_audio(save+"_process.mp4",music_name,save+'.mp4')
-            os.remove(save+'_process.mp4')
         elif len(music)==1:
             print('音频添加中')
             if os.path.exists(save+'.mp4'):
                 os.remove(save+'.mp4')
             video_add_audio(save+"_process.mp4",music[0],save+'.mp4')
-            os.remove(save+'_process.mp4')
-        print(save+".mp4保存成功")
+        else:
+            print('No music!')
+            shutil.copy(save+"_process.mp4",save+'.mp4')
+        os.remove(save+'_process.mp4')
+        print(save+".mp4保存成功")
```

### Comparing `pyfii-1.4.0/src/pyfii.egg-info/PKG-INFO` & `pyfii-1.5.0/src/pyfii.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyfii
-Version: 1.4.0
+Version: 1.5.0
 Summary: 这个库可以让我们用python写Fii的无人机程序，有三视图模拟飞行的功能，模拟飞行更方便观看
-Author-email: Kevin0412 <kevin0412_xlt@qq.com>
+Author-email: Kevin0412 <kevin0412_xlt@qq.com>, miaooo0000OOOO <1683618861@qq.com>
 Project-URL: Homepage, https://github.com/Kevin0412/pyfii
 Project-URL: Bug Tracker, https://github.com/Kevin0412/pyfii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyfii
 
 ## 简介
 这个库的功能是可以让我们用python写Fii的无人机程序，以解决原软件无运算能力，无循环模块，一块块拖太烦等问题。
```

