# Comparing `tmp/restraint-fold-0.1.1.tar.gz` & `tmp/restraint-fold-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restraint-fold-0.1.1.tar", last modified: Mon Jun 12 02:06:39 2023, max compression
+gzip compressed data, was "restraint-fold-0.1.3.tar", last modified: Sun Jun 25 01:27:25 2023, max compression
```

## Comparing `restraint-fold-0.1.1.tar` & `restraint-fold-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1068 2023-06-06 06:19:40.000000 restraint-fold-0.1.1/LICENSE
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2530 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2226 2023-06-12 02:05:51.000000 restraint-fold-0.1.1/README.md
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/fold/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     7708 2023-06-12 01:57:29.000000 restraint-fold-0.1.1/fold/__init__.py
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     3009 2023-06-12 02:04:32.000000 restraint-fold-0.1.1/fold/__main__.py
-drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/restraint_fold.egg-info/
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     2530 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/PKG-INFO
--rw-rw-r--   0 dechin    (1001) dechin    (1001)      249 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/SOURCES.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/dependency_links.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       13 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/requires.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)        5 2023-06-12 02:06:39.000000 restraint-fold-0.1.1/restraint_fold.egg-info/top_level.txt
--rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-12 02:06:39.796523 restraint-fold-0.1.1/setup.cfg
--rw-rw-r--   0 dechin    (1001) dechin    (1001)     1984 2023-06-12 01:59:32.000000 restraint-fold-0.1.1/setup.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-25 01:27:25.882166 restraint-fold-0.1.3/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1068 2023-06-06 06:19:40.000000 restraint-fold-0.1.3/LICENSE
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4527 2023-06-25 01:27:25.882166 restraint-fold-0.1.3/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4223 2023-06-25 01:23:12.000000 restraint-fold-0.1.3/README.md
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-25 01:27:25.878167 restraint-fold-0.1.3/fold/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     9540 2023-06-21 09:14:03.000000 restraint-fold-0.1.3/fold/__init__.py
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4074 2023-06-25 01:21:08.000000 restraint-fold-0.1.3/fold/__main__.py
+drwxrwxr-x   0 dechin    (1001) dechin    (1001)        0 2023-06-25 01:27:25.878167 restraint-fold-0.1.3/restraint_fold.egg-info/
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     4527 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/PKG-INFO
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)      249 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/SOURCES.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        1 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/dependency_links.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       18 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/requires.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)        5 2023-06-25 01:27:25.000000 restraint-fold-0.1.3/restraint_fold.egg-info/top_level.txt
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)       38 2023-06-25 01:27:25.882166 restraint-fold-0.1.3/setup.cfg
+-rw-rw-r--   0 dechin    (1001) dechin    (1001)     1984 2023-06-21 09:11:45.000000 restraint-fold-0.1.3/setup.py
```

### Comparing `restraint-fold-0.1.1/LICENSE` & `restraint-fold-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `restraint-fold-0.1.1/PKG-INFO` & `restraint-fold-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restraint-fold
-Version: 0.1.1
+Version: 0.1.3
 Summary: Simple Protein Structure Parser
 Home-page: https://gitee.com/dechin/restraint-fold/
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
@@ -15,66 +15,71 @@
 - 首先通过pip进行安装：
 ```bash
 $ python3 -m pip install restraint-fold --upgrade -i https://pypi.org/simple
 ```
 - 然后直接在命令行进行使用：
 ```bash
 $ python3 -m fold -h
-usage: __main__.py [-h] [-i I] [-o O] [--simplified SIMPLIFIED]
+usage: __main__.py [-h] [-i I] [-o O] [-oh OH] [--simplified SIMPLIFIED] [--addh ADDH]
 
 optional arguments:
   -h, --help            show this help message and exit
   -i I                  Set the input pdb file path.
   -o O                  Set the output txt file path.
+  -oh OH                Write the hbonds into txt file.
   --simplified SIMPLIFIED
                         Return the simplified information, default to be 0.
+  --addh ADDH           Decide to rebuild hydrogen atoms or not, default to be 0.
 ```
 
 ### 示例
 - 执行一个生成完整的alpha和beta序列的命令：
 ```bash
-$ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt
+$ python3 -m fold -i examples/pdb/case2-optimized.pdb -o examples/case2-secondary.txt
+Analysing alpha:
+100%|████████████████████████████████████████████████████████████████████████████████████████████| 154/154 [00:00<00:00, 14563.23it/s]
+Analysing beta:
+100%|█████████████████████████████████████████████████████████████████████████████████████████████| 746/746 [00:00<00:00, 6425.08it/s]
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 31 32 33 34 35 36 37 39 40 41 42 43 44 45 46 78 79 80 81 82 83 84 85 86 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109
 beta:
-23 24 25 26 27 28 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 86 87 88 89 90 91 92 93 94 95 96 97 98 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157
+23 24 25 26 27 28 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 93 94 95 96 97 98 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157
 ```
 
 ```bash
-$ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt --simplified 1
+$ python3 -m fold -i examples/pdb/case2-optimized.pdb -o examples/case2-secondary.txt --simplified 1
+Analysing alpha:
+100%|████████████████████████████████████████████████████████████████████████████████████████████| 154/154 [00:00<00:00, 17623.61it/s]
+Analysing beta:
+100%|█████████████████████████████████████████████████████████████████████████████████████████████| 746/746 [00:00<00:00, 6416.04it/s]
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
-1~24
-31~36
-39~45
-78~85
-94~97
-99~108
+1~25
+31~37
+39~46
+78~86
+94~109
 
 beta:
 23~28
-46~76
-86~98
-117~157
+46~72
+93~98
+118~157
 ```
 ### 提示
-如果输入的pdb文件中氢原子有缺失，需要先通过Xponge或者Hadder等工具进行补氢，然后再对结构进行解析：
+如果输入的pdb文件中氢原子有缺失，需要加上`--addh 1`自动补充氢原子的选项，或者手动通过Xponge或者Hadder等工具进行补氢，然后再对结构进行解析：
 ```bash
-$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
-$ python3 -m hadder -h
-usage: __main__.py [-h] [-i I] [-o O]
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -i I        Set the input pdb file path.
-  -o O        Set the output pdb file path.
-  
-$ python3 -m hadder -i input.pdb -o ouput.pdb # e.g. $ python3 -m hadder -i examples/case2.pdb -o examples/case2-complete.pdb
-1 H-Adding task with 3032 atoms complete in 0.116 seconds.
+$ python3 -m fold -i examples/pdb/case2.pdb -o examples/case2-secondary.txt --simplified 1 --addh 1
+1 H-Adding task with 2529 atoms complete in 0.09 seconds.
+The new pdb file path is in: /tmp/restraint-fold/92de3be6-12f6-11ee-b491-b07b25070cd2.pdb
+Analysing alpha:
+100%|████████████████████████████████████████████████████████████████████████████████████████████| 154/154 [00:00<00:00, 15845.42it/s]
+Analysing beta:
+100%|█████████████████████████████████████████████████████████████████████████████████████████████| 746/746 [00:00<00:00, 6003.69it/s]
 ```
```

### Comparing `restraint-fold-0.1.1/fold/__init__.py` & `restraint-fold-0.1.3/fold/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import sys
 sys.setrecursionlimit(90000000)
 
 import numpy as np
+from tqdm import trange
 from hadder.parsers import read_pdb
 from hadder.constants import hnames
 
-def get_hbonds(pdb_name, hbond_length=3.5):
+def get_hbonds(pdb_name, hbond_length=3.5, return_hbonds=False):
     res = read_pdb(pdb_name)
     atom_names = res[5]
     group_names = res[0]
     crds = res[6]
     res_names = res[7]
     res_ids = res[8]
     n_index = []
@@ -49,48 +50,69 @@
     n_index = np.array(n_index, np.int32)
     o_index = np.array(o_index, np.int32)
     h_index = np.array(h_index, np.int32)
 
     n_crd = crds[n_index]
     o_crd = crds[o_index]
     h_crd = crds[h_index]
-
+    
     dis_oh = np.linalg.norm(o_crd - h_crd[:, None, :], axis=-1)
     mask_oh = np.where(dis_oh <= hbond_length)
     mh_index_o = mask_oh[0]
     mo_index = mask_oh[1]
     xh_index_o = []
     for idx in mh_index_o:
         h_idx = h_index[idx]
         res_name = res_names[h_idx]
         res_id = res_ids[h_idx]
+        if res_id == 1 and res_name == 'ACE':
+            pass
+        elif res_id == max(res_ids) and res_name == 'NME':
+            pass
+        elif res_id == 1:
+            res_name = 'N' + res_name
+        elif res_id == max(res_ids):
+            res_name = 'C' + res_name
+        else:
+            pass
         res_dict = hnames[res_name]
         for key in res_dict:
             if atom_names[h_idx] not in res_dict[key]:
                 continue
-            for cbk in range(30):
+            for cbk in range(50):
                 if atom_names[h_idx - cbk - 1] == key and res_ids[h_idx - cbk - 1] == res_id:
                     xh_index_o.append(h_idx - cbk - 1)
                     break
     xh_index_o = np.array(xh_index_o, np.int32)
+
     dis_nh = np.linalg.norm(n_crd - h_crd[:, None, :], axis=-1)
     mask_nh = np.where(dis_nh <= hbond_length)
     mh_index_n = mask_nh[0]
     mn_index = mask_nh[1]
     xh_index_n = []
 
     for idx in mh_index_n:
         h_idx = h_index[idx]
         res_name = res_names[h_idx]
         res_id = res_ids[h_idx]
+        if res_id == 1 and res_name == 'ACE':
+            pass
+        elif res_id == max(res_ids) and res_name == 'NME':
+            pass
+        elif res_id == 1:
+            res_name = 'N' + res_name
+        elif res_id == max(res_ids):
+            res_name = 'C' + res_name
+        else:
+            pass
         res_dict = hnames[res_name]
         for key in res_dict:
             if atom_names[h_idx] not in res_dict[key]:
                 continue
-            for cbk in range(30):
+            for cbk in range(50):
                 if atom_names[h_idx - cbk - 1] == key and res_ids[h_idx - cbk - 1] == res_id:
                     xh_index_n.append(h_idx - cbk - 1)
                     break
     xh_index_n = np.array(xh_index_n, np.int32)
 
     hbonds = []
     res_bonds = []
@@ -120,24 +142,29 @@
 
     cos_h = np.einsum('ij,ij->i', xh_vector, hy_vector) / (np.linalg.norm(xh_vector, axis=-1) + 1e-08) / (
             np.linalg.norm(hy_vector, axis=-1) + 1e-08)
     angle_filter = np.where(cos_h > np.cos(np.pi * 43.1 / 180))
 
     hbonds = hbonds[angle_filter]
     res_bonds = res_bonds[angle_filter]
-
+    
+    hbonds = np.unique(hbonds, axis=0)
     res_bonds = np.unique(res_bonds, axis=0)
-    return res_bonds
+    if return_hbonds:
+        return hbonds
+    else:
+        return res_bonds
 
 def get_alpha(pdb_name, hbond_length=3.5):
     res_bonds = get_hbonds(pdb_name, hbond_length=hbond_length)
     alpha = []
     counter = 0
     min_alpha = 4
-    for index in range(np.max(res_bonds) - 3):
+    print ('Analysing alpha:')
+    for index in trange(np.max(res_bonds) - 3):
         tmp_bond_1 = np.array([index, index + 4])
         tmp_bond_2 = tmp_bond_1 + 1
         tmp_bond_3 = tmp_bond_1 + 2
         tmp_bond_4 = np.array([index, index + 3])
         if np.sum(np.isin(res_bonds, tmp_bond_1).sum(axis=-1) == 2) > 0:
             counter += 1
             continue
@@ -160,21 +187,21 @@
             continue
     alpha = np.sort(np.array(alpha, np.int32))
     return alpha
 
 tmp_beta = []
 beta = []
 counter = 0
+counter_1 = 0
 
 def _get_beta(res_bonds, start, end):
     global beta
     global counter
     global tmp_beta
     pair = np.array([start-1, end+1])
-    pair_2 = np.array([start-2, end+2])
     if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
         if start-1 not in tmp_beta:
             tmp_beta.extend([start-1])
         if end+1 not in tmp_beta:
             tmp_beta.extend([end+1])
         counter += 1
         return _get_beta(res_bonds, start-1, end+1)
@@ -187,25 +214,56 @@
     else:
         if counter > 4:
             beta.extend(tmp_beta)
         counter = 1
         tmp_beta = []
         return 0
 
+def _get_beta_1(res_bonds, start, end):
+    global beta
+    global counter_1
+    global tmp_beta
+    pair = np.array([start+1, end+1])
+    if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+        if start-1 not in tmp_beta:
+            tmp_beta.extend([start+1])
+        if end+1 not in tmp_beta:
+            tmp_beta.extend([end+1])
+        counter_1 += 1
+        return _get_beta(res_bonds, start+1, end+1)
+    elif counter_1 > 1 and np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
+        if start-2 not in tmp_beta:
+            tmp_beta.extend([start+2])
+        if end+2 not in tmp_beta:
+            tmp_beta.extend([end+2])
+        counter_1 += 1
+    else:
+        if counter_1 > 4:
+            beta.extend(tmp_beta)
+        counter_1 = 1
+        tmp_beta = []
+        return 0
+
 def get_beta(pdb_name, hbond_length=3.5):
     res_bonds = get_hbonds(pdb_name, hbond_length=hbond_length)
     global tmp_beta
     global beta
-    for index, bond in enumerate(res_bonds):
+    print ('Analysing beta:')
+    for index in trange(len(res_bonds)):
+        bond = res_bonds[index]
         start = bond[0]
         end = bond[1]
         pair = np.array([start-1, end+1])
+        pair_1 = np.array([start+1, end+1])
         if np.sum(np.isin(res_bonds, pair).sum(axis=-1)==2)>0:
             tmp_beta.extend([start, end])
             _ = _get_beta(res_bonds, start, end)
+        elif np.sum(np.isin(res_bonds, pair_1).sum(axis=-1)==2)>0:
+            tmp_beta.extend([start, end])
+            _ = _get_beta_1(res_bonds, start, end)
         else:
             continue
     beta = np.array(beta, np.int32)
     beta = np.unique(beta)
     beta = np.sort(beta)
     return beta
```

### Comparing `restraint-fold-0.1.1/fold/__main__.py` & `restraint-fold-0.1.3/fold/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,63 +16,91 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import os
 import argparse
-from fold import get_alpha, get_beta, get_residue_type
+import uuid
+from fold import get_hbonds, get_alpha, get_beta, get_residue_type
+from hadder import AddHydrogen
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-i", help="Set the input pdb file path.")
 parser.add_argument("-o", help="Set the output txt file path.")
+parser.add_argument("-oh", help="Write the hbonds into txt file.")
 parser.add_argument("--simplified", help="Return the simplified information, default to be 0.", default='0')
+parser.add_argument("--addh", help="Decide to rebuild hydrogen atoms or not, default to be 0.", default='0')
 
 args = parser.parse_args()
 pdb_name = args.i
 save_txt_name = args.o
+hbond_txt = args.oh
 use_simplified = args.simplified
+addh = args.addh
+
+task_id = uuid.uuid1()
+if not os.path.exists('/tmp/restraint-fold/'):
+    os.mkdir('/tmp/restraint-fold/')
+addh_pdb = '/tmp/restraint-fold/{}.pdb'.format(task_id)
+
+if addh == '1':
+    AddHydrogen(pdb_name, addh_pdb)
+    print ('The new pdb file path is in: {}'.format(addh_pdb))
+    pdb_name = addh_pdb
 
 alphas = get_alpha(pdb_name, hbond_length=3.5)
-betas = get_beta(pdb_name, hbond_length=4.0)
+betas = get_beta(pdb_name, hbond_length=3.5)
+
+if save_txt_name is not None:
+    if use_simplified == '0':
+        with open(save_txt_name, 'w') as file:
+            file.write('alpha:\n')
+            file.write(' '.join(list(map(str,alphas))))
+            file.write('\n')
+            file.write('beta:\n')
+            file.write(' '.join(list(map(str,betas))))
+    else:
+        with open(save_txt_name, 'w') as file:
+            file.write('alpha:\n')
+            for i in range(len(alphas)):
+                if i == 0:
+                    file.write(str(alphas[i]))
+                    file.write('~')
+                elif i == len(alphas)-1:
+                    file.write(str(alphas[i]))
+                    file.write('\n')
+                elif alphas[i] != alphas[i-1]+1:
+                    file.write(str(alphas[i-1]))
+                    file.write('\n')
+                    file.write(str(alphas[i]))
+                    file.write('~')
+                else:
+                    continue
+            file.write('\n')
+            file.write('beta:\n')
+            for i in range(len(betas)):
+                if i == 0:
+                    file.write(str(betas[i]))
+                    file.write('~')
+                elif i == len(betas)-1:
+                    file.write(str(betas[i]))
+                    file.write('\n')
+                elif betas[i] != betas[i-1]+1:
+                    file.write(str(betas[i-1]))
+                    file.write('\n')
+                    file.write(str(betas[i]))
+                    file.write('~')
+                else:
+                    continue
+
+
+if hbond_txt is not None:
+    hbonds = get_hbonds(pdb_name, return_hbonds=True)
+    with open(hbond_txt, 'w') as file:
+        file.write('Hbonds:\n')
+        file.write('{}\n'.format(hbonds.shape[0]))
+        for bond in hbonds:
+            file.write('{}\t{}\n'.format(bond[0], bond[1]))
 
-if use_simplified == '0':
-    with open(save_txt_name, 'w') as file:
-        file.write('alpha:\n')
-        file.write(' '.join(list(map(str,alphas))))
-        file.write('\n')
-        file.write('beta:\n')
-        file.write(' '.join(list(map(str,betas))))
-else:
-    with open(save_txt_name, 'w') as file:
-        file.write('alpha:\n')
-        for i in range(len(alphas)):
-            if i == 0:
-                file.write(str(alphas[i]))
-                file.write('~')
-            elif i == len(alphas)-1:
-                file.write(str(alphas[i]))
-                file.write('\n')
-            elif alphas[i] != alphas[i-1]+1:
-                file.write(str(alphas[i-1]))
-                file.write('\n')
-                file.write(str(alphas[i]))
-                file.write('~')
-            else:
-                continue
-        file.write('\n')
-        file.write('beta:\n')
-        for i in range(len(betas)):
-            if i == 0:
-                file.write(str(betas[i]))
-                file.write('~')
-            elif i == len(betas)-1:
-                file.write(str(betas[i]))
-                file.write('\n')
-            elif betas[i] != betas[i-1]+1:
-                file.write(str(betas[i-1]))
-                file.write('\n')
-                file.write(str(betas[i]))
-                file.write('~')
-            else:
-                continue
```

### Comparing `restraint-fold-0.1.1/restraint_fold.egg-info/PKG-INFO` & `restraint-fold-0.1.3/restraint_fold.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restraint-fold
-Version: 0.1.1
+Version: 0.1.3
 Summary: Simple Protein Structure Parser
 Home-page: https://gitee.com/dechin/restraint-fold/
 Author: Dechin CHEN
 Author-email: dechin.phy@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
@@ -15,66 +15,71 @@
 - 首先通过pip进行安装：
 ```bash
 $ python3 -m pip install restraint-fold --upgrade -i https://pypi.org/simple
 ```
 - 然后直接在命令行进行使用：
 ```bash
 $ python3 -m fold -h
-usage: __main__.py [-h] [-i I] [-o O] [--simplified SIMPLIFIED]
+usage: __main__.py [-h] [-i I] [-o O] [-oh OH] [--simplified SIMPLIFIED] [--addh ADDH]
 
 optional arguments:
   -h, --help            show this help message and exit
   -i I                  Set the input pdb file path.
   -o O                  Set the output txt file path.
+  -oh OH                Write the hbonds into txt file.
   --simplified SIMPLIFIED
                         Return the simplified information, default to be 0.
+  --addh ADDH           Decide to rebuild hydrogen atoms or not, default to be 0.
 ```
 
 ### 示例
 - 执行一个生成完整的alpha和beta序列的命令：
 ```bash
-$ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt
+$ python3 -m fold -i examples/pdb/case2-optimized.pdb -o examples/case2-secondary.txt
+Analysing alpha:
+100%|████████████████████████████████████████████████████████████████████████████████████████████| 154/154 [00:00<00:00, 14563.23it/s]
+Analysing beta:
+100%|█████████████████████████████████████████████████████████████████████████████████████████████| 746/746 [00:00<00:00, 6425.08it/s]
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 31 32 33 34 35 36 37 39 40 41 42 43 44 45 46 78 79 80 81 82 83 84 85 86 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109
 beta:
-23 24 25 26 27 28 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 86 87 88 89 90 91 92 93 94 95 96 97 98 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157
+23 24 25 26 27 28 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 93 94 95 96 97 98 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157
 ```
 
 ```bash
-$ python3 -m fold -i fold/pdb/case2-optimized.pdb -o case2-secondary.txt --simplified 1
+$ python3 -m fold -i examples/pdb/case2-optimized.pdb -o examples/case2-secondary.txt --simplified 1
+Analysing alpha:
+100%|████████████████████████████████████████████████████████████████████████████████████████████| 154/154 [00:00<00:00, 17623.61it/s]
+Analysing beta:
+100%|█████████████████████████████████████████████████████████████████████████████████████████████| 746/746 [00:00<00:00, 6416.04it/s]
 ```
 得到的结果如下所示：
 ```txt
 # case2-secondary.txt
 alpha:
-1~24
-31~36
-39~45
-78~85
-94~97
-99~108
+1~25
+31~37
+39~46
+78~86
+94~109
 
 beta:
 23~28
-46~76
-86~98
-117~157
+46~72
+93~98
+118~157
 ```
 ### 提示
-如果输入的pdb文件中氢原子有缺失，需要先通过Xponge或者Hadder等工具进行补氢，然后再对结构进行解析：
+如果输入的pdb文件中氢原子有缺失，需要加上`--addh 1`自动补充氢原子的选项，或者手动通过Xponge或者Hadder等工具进行补氢，然后再对结构进行解析：
 ```bash
-$ python3 -m pip install hadder --upgrade -i https://pypi.org/simple
-$ python3 -m hadder -h
-usage: __main__.py [-h] [-i I] [-o O]
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -i I        Set the input pdb file path.
-  -o O        Set the output pdb file path.
-  
-$ python3 -m hadder -i input.pdb -o ouput.pdb # e.g. $ python3 -m hadder -i examples/case2.pdb -o examples/case2-complete.pdb
-1 H-Adding task with 3032 atoms complete in 0.116 seconds.
+$ python3 -m fold -i examples/pdb/case2.pdb -o examples/case2-secondary.txt --simplified 1 --addh 1
+1 H-Adding task with 2529 atoms complete in 0.09 seconds.
+The new pdb file path is in: /tmp/restraint-fold/92de3be6-12f6-11ee-b491-b07b25070cd2.pdb
+Analysing alpha:
+100%|████████████████████████████████████████████████████████████████████████████████████████████| 154/154 [00:00<00:00, 15845.42it/s]
+Analysing beta:
+100%|█████████████████████████████████████████████████████████████████████████████████████████████| 746/746 [00:00<00:00, 6003.69it/s]
 ```
```

### Comparing `restraint-fold-0.1.1/setup.py` & `restraint-fold-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="restraint-fold",
-    version="0.1.1",
+    version="0.1.3",
     description="Simple Protein Structure Parser",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT License",
 
     url="https://gitee.com/dechin/restraint-fold/",
     author="Dechin CHEN",
```

