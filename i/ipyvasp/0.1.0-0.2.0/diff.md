# Comparing `tmp/ipyvasp-0.1.0.tar.gz` & `tmp/ipyvasp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.1.0.tar", last modified: Sat Sep  3 00:33:38 2022, max compression
+gzip compressed data, was "ipyvasp-0.2.0.tar", last modified: Sun Jun 25 19:52:26 2023, max compression
```

## Comparing `ipyvasp-0.1.0.tar` & `ipyvasp-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-09-03 00:33:38.510397 ipyvasp-0.1.0/
--rw-rw-rw-   0        0        0     1263 2022-09-02 23:29:48.000000 ipyvasp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       77 2022-09-03 00:33:38.510397 ipyvasp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       54 2022-09-02 23:01:39.000000 ipyvasp-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-03 00:33:38.494784 ipyvasp-0.1.0/ipyvasp/
--rw-rw-rw-   0        0        0     4284 2022-09-03 00:30:05.000000 ipyvasp-0.1.0/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0    47096 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/api.py
--rw-rw-rw-   0        0        0     2644 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/cli.py
--rw-rw-rw-   0        0        0    25605 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/iplots.py
--rw-rw-rw-   0        0        0    46231 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/parser.py
--rw-rw-rw-   0        0        0    18280 2022-09-02 15:39:44.000000 ipyvasp-0.1.0/ipyvasp/serializer.py
--rw-rw-rw-   0        0        0    89377 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/sio.py
--rw-rw-rw-   0        0        0    78959 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/splots.py
--rw-rw-rw-   0        0        0    22523 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/surfaces.py
--rw-rw-rw-   0        0        0    14078 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    65722 2022-09-02 23:42:20.000000 ipyvasp-0.1.0/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2022-09-03 00:33:38.510397 ipyvasp-0.1.0/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0       77 2022-09-03 00:33:38.000000 ipyvasp-0.1.0/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2022-09-03 00:33:38.000000 ipyvasp-0.1.0/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-03 00:33:38.000000 ipyvasp-0.1.0/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-09-03 00:33:38.000000 ipyvasp-0.1.0/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-03 00:33:38.510397 ipyvasp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       82 2022-09-03 00:33:18.000000 ipyvasp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.335606 ipyvasp-0.2.0/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-06-25 19:52:26.335606 ipyvasp-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.305290 ipyvasp-0.2.0/ipyvasp/
+-rw-rw-rw-   0        0        0     1803 2023-06-25 19:47:14.000000 ipyvasp-0.2.0/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0    38537 2023-06-25 03:01:51.000000 ipyvasp-0.2.0/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    87865 2023-06-25 16:38:58.000000 ipyvasp-0.2.0/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.2.0/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     2712 2023-06-24 19:19:43.000000 ipyvasp-0.2.0/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.334597 ipyvasp-0.2.0/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.2.0/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37749 2023-06-25 19:45:39.000000 ipyvasp-0.2.0/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34873 2023-06-25 19:28:26.000000 ipyvasp-0.2.0/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    27729 2023-06-25 15:48:45.000000 ipyvasp-0.2.0/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    11584 2023-06-25 16:42:49.000000 ipyvasp-0.2.0/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    20575 2023-06-25 16:39:06.000000 ipyvasp-0.2.0/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.2.0/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11417 2023-06-25 16:39:16.000000 ipyvasp-0.2.0/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    23766 2023-06-25 19:47:03.000000 ipyvasp-0.2.0/ipyvasp/surface.py
+-rw-rw-rw-   0        0        0    15028 2023-06-25 16:39:20.000000 ipyvasp-0.2.0/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44839 2023-06-25 16:39:34.000000 ipyvasp-0.2.0/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:52:26.329406 ipyvasp-0.2.0/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0       77 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 19:52:26.000000 ipyvasp-0.2.0/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 19:52:26.335606 ipyvasp-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       86 2023-06-25 19:47:34.000000 ipyvasp-0.2.0/setup.py
```

### Comparing `ipyvasp-0.1.0/LICENSE` & `ipyvasp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.1.0/ipyvasp/cli.py` & `ipyvasp-0.2.0/ipyvasp/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from . import __version__, __doc__, docs, example
-from .sio import str2kpath, InvokeMaterialsProject, _save_mp_API
-import argparse
-from argparse import RawTextHelpFormatter
-def main():
-    print(f'ipyvasp\n=======\nVersion: {__version__}')
-    print(__doc__)
-    print('Loading Online DOCS...')
-    docs()
-    
-def wroking_example():
-    print('Loading Example...')
-    example()
-
-    
-def get_kpath():
-    parser = argparse.ArgumentParser(description='Process KPATH string.', formatter_class=RawTextHelpFormatter)
-    
-    parser.add_argument('kpath_str', help='''kpath multiline string e.g.:\n\t0 0 0 !$\Gamma$ 5\n\t1/2 1/2 1/2 !L 3\n\t0 0 1/2 !A\n\
-will add 5 kpoints in the interval 1 and 3 in interval 2.\
-Empty lines are taken as breaks in path.''')
-    parser.add_argument('-w', '--weight',type=int, default=None)
-    parser.add_argument('-n', '--n',type=int, default=10, help='Number of kpoints per unit length.')
-    parser.add_argument('-z','--ibzkpt', type=str, help='IBZKPT file path, useful for HSE06 calculations.')
-    
-    args = parser.parse_args()
-    
-    return str2kpath(args.kpath_str,weight=args.weight,n=args.n, ibzkpt=args.ibzkpt)
-
-def poscar():
-    parser = argparse.ArgumentParser(description='Download POSCAR from Materials Project Website.')
-    
-    parser.add_argument('formula',type=str, help='Formula like "GaAs"')
-    parser.add_argument('-i','--mp_id',type=str, help='ID of crystal as on Materials Project Website (optional).')
-    parser.add_argument('-M', '--max_sites',type=int, help='Number of max sites in POSCAR, do not need if --mp_id given.')
-    parser.add_argument('-m', '--min_sites',type=int, help='Number of min sites in POSCAR, do not need if --mp_id given.')
-    parser.add_argument('-k','--api_key',type=str, help= 'Materials project API key. Save it using `ipyvasp_save_mp_key` just once.')
-    
-    args = parser.parse_args()
-    mp = InvokeMaterialsProject(api_key=args.api_key)
-    output = mp.request(args.formula,mp_id=args.mp_id,max_sites=args.max_sites, min_sites=args.min_sites)
-    
-    if output:
-        for car in output:
-            print("\ncar\n{('='*66}")
-            car.export_poscar().write(outfile = None) # write POSCAR to stdout
-    else:
-        print('No POSCAR found with provided input, try increasing range')
-        
-def api_key_save():
-    parser = argparse.ArgumentParser(description='Saves API key from Materials Project website on your local machine for every time use.')
-    parser.add_argument('api_key',type=str, help='Get API key from Materilas Project website and enter here.')
-    args = parser.parse_args()
-    return _save_mp_API(api_key=args.api_key)
+from . import __version__, __doc__, docs, example
+from ._lattice import get_kpath as gkpath, InvokeMaterialsProject, _save_mp_API
+import argparse
+from argparse import RawTextHelpFormatter
+
+def main():
+    print(f'ipyvasp\n=======\nVersion: {__version__}')
+    print(__doc__)
+    print('Loading Online DOCS...')
+    docs()
+    
+def wroking_example():
+    print('Loading Example...')
+    example()
+
+    
+def get_kpath():
+    parser = argparse.ArgumentParser(description='Process KPATH string.', formatter_class=RawTextHelpFormatter)
+    
+    parser.add_argument('kpath_str', help='''kpath multiline string e.g.:\n\t0 0 0 !$\Gamma$ 5\n\t1/2 1/2 1/2 !L 3\n\t0 0 1/2 !A\n\
+will add 5 kpoints in the interval 1 and 3 in interval 2.\
+Empty lines are taken as breaks in path.''')
+    parser.add_argument('-w', '--weight',type=int, default=None)
+    parser.add_argument('-n', '--n',type=int, default=10, help='Number of kpoints per unit length.')
+    parser.add_argument('-z','--ibzkpt', type=str, help='IBZKPT file path, useful for HSE06 calculations.')
+    
+    args = parser.parse_args()
+    
+    return gkpath(args.kpath_str,weight=args.weight,n=args.n, ibzkpt=args.ibzkpt)
+
+def poscar():
+    parser = argparse.ArgumentParser(description='Download POSCAR from Materials Project Website.')
+    
+    parser.add_argument('formula',type=str, help='Formula like "GaAs"')
+    parser.add_argument('-i','--mp_id',type=str, help='ID of crystal as on Materials Project Website (optional).')
+    parser.add_argument('-M', '--max_sites',type=int, help='Number of max sites in POSCAR, do not need if --mp_id given.')
+    parser.add_argument('-m', '--min_sites',type=int, help='Number of min sites in POSCAR, do not need if --mp_id given.')
+    parser.add_argument('-k','--api_key',type=str, help= 'Materials project API key. Save it using `ipyvasp_save_mp_key` just once.')
+    
+    args = parser.parse_args()
+    mp = InvokeMaterialsProject(api_key=args.api_key)
+    output = mp.request(args.formula,mp_id=args.mp_id,max_sites=args.max_sites, min_sites=args.min_sites)
+    
+    if output:
+        for car in output:
+            print("\ncar\n{('='*66}")
+            car.export_poscar().write(outfile = None) # write POSCAR to stdout
+    else:
+        print('No POSCAR found with provided input, try increasing range')
+        
+def api_key_save():
+    parser = argparse.ArgumentParser(description='Saves API key from Materials Project website on your local machine for every time use.')
+    parser.add_argument('api_key',type=str, help='Get API key from Materilas Project website and enter here.')
+    args = parser.parse_args()
+    return _save_mp_API(api_key=args.api_key)
```

### Comparing `ipyvasp-0.1.0/ipyvasp/iplots.py` & `ipyvasp-0.2.0/ipyvasp/surface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,482 +1,566 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: InteractivePlots.ipynb (unless otherwise specified).
+__all__ = ["SpinDataFrame"]
 
-__all__ = ['iplot2html', 'iplot_rgb_lines', 'iplot_dos_lines']
-
-# Cell
 import numpy as np
-import matplotlib as mpl
+import pandas as pd
+from scipy.interpolate import griddata
 import matplotlib.pyplot as plt
 
-import plotly.graph_objects as go
+# Inside packages import
+from .core import parser as vp, serializer
+from .core import plot_toolkit as ptk
+from .lattice import POSCAR
+from .bsdos import _format_input
+
+
+# Need to get it from source like Vasprun, and then get_evals
+def _collect_spin_data(source, bands=[0], projections={"A": ([0], [0])}):
+    if not isinstance(bands, (list, tuple)):
+        raise TypeError("`bands` must be list/tuple of integer.")
+    atoms, orbs, *_ = _format_input(projections, sys_info=source.summary)
+
+    def per_band_data(band):
+        kpoints = source.kpoints
+        evals = {k: v[..., band] for k, v in source.evals.items() if k in "eud"}
+        spins = {k: v[..., band, :] for k, v in source.spins.items() if k in "sxyzud"}
+
+        df_dict = {f"k{k}": v for k, v in zip("xyz", kpoints.T)}
+        df_dict["band"] = [
+            (band + source.evals.indices[0] + 1) for i in range(len(kpoints))
+        ]
+
+        for k, v in evals.items():
+            df_dict[k if k == "e" else f"e{k}"] = v.T.flatten() - source.summary.EFERMI
+
+        for i, (a, o) in enumerate(zip(atoms, orbs)):
+            for k, v in spins.items():
+                if k in "sxyzud":
+                    key = k if k == "s" else f"s{k}"
+                    df_dict[f"{key}_{i}"] = (
+                        v.take(a, axis=0)
+                        .take(o, axis=2)
+                        .sum(axis=2)
+                        .sum(axis=0)
+                        .T.flatten()
+                    )
+
+        return df_dict
+
+    main_dict = per_band_data(bands[0])
+    for b in bands[1:]:
+        data = per_band_data(b)
+        for k, v in main_dict.items():
+            main_dict[k] = [*main_dict[k], *data[k]]
+
+    if (
+        atoms
+    ):  # NOTE: Make room for negative peak to peak. Only scale if projections given
+        _max = []
+        for k, v in main_dict.items():
+            if k.startswith("s"):
+                _max.append(np.abs(v).max())
+
+        _max = max(_max)
+        for k, v in main_dict.items():
+            if k.startswith("s"):
+                main_dict[k] = v / (_max if _max != 0 else 1)
+    return main_dict
 
-# Inside packages import to work both with package and jupyter notebook.
-try:
-    from ipyvasp import parser as vp
-    from ipyvasp import splots as sp
-    from ipyvasp import utils as gu
-except:
-    import ipyvasp.parser as vp
-    import ipyvasp.splots as sp
-    import ipyvasp.utils as gu
-
-# Cell
-def _get_rgb_data(
-    kpath       = None,
-    evals_set   = None,
-    pros_set    = None,
-    elements    = [[0],[],[]],
-    orbs        = [[0],[],[]],
-    interp_nk   = {},
-    occs_set    = None,
-    kpoints     = None,
-    ):
-    """
-    - Returns a formatted RGB colored data to pass into `_rgb2plotly` function. Two arguments, `elements` and `orbs` should be in one-to-one correspondence. Returned item has transpose data shape, so that main iteration is over bands.
-    - **Parameters**
-        - kapath   : `export_vasprun`().kpath or `get_kpts`().kpath.
-        - evals_set: `export_vasprun`().bands.evals or `get_evals`().evals. If calculations are spin-polarized, it will be `...evals.SpinUp/SpinDown` for both. You need to apply twice for SpinUp and SpinDown separately.
-        - pros_set : `export_vasprun().pro_bands.pros` or `get_bands_pro_set`().pros. If calculations are spin-polarized, it will be `...pros.SpinUp/SpinDown` for both. You need to create collections twice for SpinUp and SpinDown separately.
-        - elements : List three lists of ions to project on, each element could be `range(start,stop,step)` as well, remember that `stop` is not included in python. so `range(0,2)` will generate 0 and 1 indices.
-        - orbs     : List of three lists of orbitals indices. `[[red],[green],[blue]]`, you can create any color by this combination. For example, to get `s-orbital in yellow color`, you will use `[[0],[0],[]]`. Do not remove empty list from there, it will not effect your orbital selection.
-        - interp_nk   : Dictionary with keys 'n' and 'k' for interpolation.
-        - occs_set: `export_vasprun`().bands.occs or `get_evals`().occs. If calculations are spin-polarized, it will be `...occs.SpinUp/SpinDown` for both. You need to apply twice for SpinUp and SpinDown separately.
-    - **Returns**
-        - kpath    : List of path of NKPTS. (interpolated if given.)
-        - evals    : An (NBAND,NKPTS) numpy arry.
-        - occs     : An (NBAND,NKPTS) numpy arry.
-        - colors   : An (NBANDS,NKPTS,3) numpy array.
-        - widths   : An (NBAND,NKPTS) numpy arry, its actually colors summed along z-axis.
-        - norms    : An (NBAND,NKPTS) numpy arry, normalized as 100%.
-        - kpoints  : List of NKPTS. (interpolated if given.)
-    """
-    if pros_set == []:
-        raise ValueError("Can not plot an empty eigenvalues object\n"
-                         "Try with large energy range.")
-    if len(orbs) < 3 :
-        raise ValueError("orbs have structure [[],[],[]], do not reduce structure even if it is empty.")
-    elif len(elements) <3:
-        raise ValueError("elements have structure [[],[],[]], do not reduce structure even if it is empty.")
-    else:
-       r = np.take(pros_set,orbs[0],axis=3).sum(axis=3)
-       r = np.take(r,list(elements[0]),axis=0).sum(axis=0)
-       g = np.take(pros_set,orbs[1],axis=3).sum(axis=3)
-       g = np.take(g,list(elements[1]),axis=0).sum(axis=0)
-       b = np.take(pros_set,orbs[2],axis=3).sum(axis=3)
-       b = np.take(b,list(elements[2]),axis=0).sum(axis=0)
-       if interp_nk:
-           from ipyvasp import utils as gu
-           knew,evals = gu.interpolate_data(kpath,evals_set,**interp_nk)
-           _,occs = gu.interpolate_data(kpath,occs_set,**interp_nk)
-           _, kpoints = gu.interpolate_data(kpath,kpoints,**interp_nk)
-           r  = gu.interpolate_data(kpath,r,**interp_nk)[1].clip(min=0)
-           g  = gu.interpolate_data(kpath,g,**interp_nk)[1].clip(min=0)
-           b  = gu.interpolate_data(kpath,b,**interp_nk)[1].clip(min=0)
-       else:
-           knew,evals, occs, kpoints = kpath,evals_set, occs_set, kpoints
-
-       evals = np.transpose(evals)
-       occs = np.transpose(occs)
-       max_c = max(max(map(max,r[:,:])),max(map(max,g[:,:])),max(map(max,b[:,:])))
-       if max_c == 0:
-           max_c=1 # Avoid divide by 0.
-       _cl = np.concatenate((r,g,b)).reshape((3,-1,np.shape(r)[1])).swapaxes(0,2)
-       rgb = _cl/max_c # Normalized overall data
-       norms = (rgb*100).astype(int) # Normalized overall data
-       widths = 0.0001+ np.sum(rgb,axis=2) #should be before scale colors
-
-       # Now scale colors to 1 at each point.
-       cl_max=np.max(_cl,axis=2)
-       cl_max[cl_max==0.0] = 1 # avoid divide by zero. Contributions are 4 digits only.
-       rgb = _cl/cl_max[:,:,np.newaxis] # Normalized per point
 
-       return knew,evals,occs, rgb, widths, norms, kpoints
-
-# Cell
-def _flip_even_patches(array_1d, patch_length):
-    """
-    - When you reshape bands data to 1D array, you may need to draw lines which do not link ends of plot, for that, it is required to flip patches, so that next band start from where 1st end and so one.
-    - **Parameters**
-        - array_1d     : Numpy 1d array or list.
-        - patch_length : length of xaxis patches, e.g NKPTS.
-    - **Returns**
-        - 1D list
-    - ** Example**
-        > k=[1,2,3,1,2,3]
-        > _flip_even_patches(k,3)
-        > [1,2,3,3,2,1]
+class SpinDataFrame(pd.DataFrame):
     """
-    out_put = []
-    n= patch_length
-    for i in range(len(array_1d)):
-        if i % 2 != 0:
-            out_put.extend(np.flip(array_1d[i*n:(i+1)*n]))
-        else:
-            out_put.extend(array_1d[i*n:(i+1)*n])
-    return out_put
+    Spin data from vasprun.xml is converted to a dataframe.
 
-# Cell
-def _rgb2plotly(rgb_data=None,mode='markers',max_width=None,showlegend=False,name='',labels=['s','p','d'],symbol=0,bands_indices = None):
-    """
-    - Returns data object of plotly's figure using `_get_rgb_data`. Returned data could be fed to a plolty's figure.
-    - ** Parameters**
-        - rgb_data    : output of `_get_rgb_data`.
-        - mode        : Three plotting modes are available:
-            - 'markers' : Plot whole data as a single scatter object. Its too fast.
-            - 'bands'   : Plot data such that each band is accessible via legend.
-            - 'lines'   : A replica of `matplotlib LineCollection` object. It plots at each point separately, slower than other two modes.
-        - max_width  : Line/Scatter thickness is scaled to `max_width`. None by default and represent actual data.
-        - name       : Name to be shown on hover text or legend.
-        - labels     : Optional, show red green blue colors corresponding orbitals.
-        - showlegend : Optional, only suitbale if spin up/down or 'bands' mode is ON.
-        - symbol     : Plotly's marker symbol. 0 for circle, 5/6 for Up/Down.
-        - bands_indices : `len(bands_indices) == NBANDS` should hold. `export_vasprun().bands.indices` or `get_evals().indices`.
-    """
-    if mode not in ('markers','bands','lines'):
-        raise TypeError("Argument `mode` expects one of ['markers','bands','lines'], got '{}'.".format(mode))
-    if rgb_data:
-        k,en,occ, rgb,lws, norms, kpoints = rgb_data
-        _indices = range(np.shape(en)[1]) if bands_indices is None else bands_indices
-
-        _names = [["<sub>{}</sub>".format(int(1+i)) for j in range(len(en[0]))]
-                  for i in _indices]
-        clrs=(255*rgb).astype(int).clip(min=0,max=255) #clip in color range
-        colors=[['rgb({},{},{})'.format(*i) for i in _c] for _c in clrs]
-        txts=[['Projection: [{0}]</br>Norm (%): [{1}, {2}, {3}]'.format(', '.join(labels),*_n) for _n in _norm] for _norm in norms]
-
-        if max_width:
-            lws = max_width*lws/np.max(lws)
-
-        ktext = [f'{x:>7.3f}{y:>7.3f}{z:>7.3f}' for (x,y,z) in kpoints]
-        h_template = "</br>{} </br></br>Band: {}{}  Occ: {:>7.4f}</br>K<sub>{}</sub>: {}"
-        h_text=[[h_template.format(t,name,l,o,i, ktext[i]) for i,(t,l,o) in enumerate(zip(ts,ns,os))]
-                for ts,ns,os in zip(txts,_names,occ)]
-        data=[]
-        if mode == 'lines':
-            lc = [[[k[i:i+2],ke[i:i+2]] for i in range(len(ke)-1)] for ke in en]
-            lws = 0.5*(lws[:,:-1] + lws[:,1:])
-            # Zip auto picks colors,lws,h_text in same number as en
-            data = [
-             go.Scatter(x=pt[0],y=pt[1],name=name, mode="lines",line=dict(color=c, width=w),
-             showlegend=showlegend,hovertext=h)
-                for pts,cs,ws,hs in zip(lc,colors,lws,h_text)
-                    for pt,c,w,h in zip(pts,cs,ws,hs)]
-
-        if mode == 'markers':
-            nkpts = len(k) # should not move up or down.
-            k = [k for bands in range(len(en))]
-            k,en,colors,lws,h_text = [np.reshape(item,(-1)) for item in [k,en,colors,lws,h_text]]
-            # Make lines reverse at even line.
-            k,en,colors,lws,h_text =[_flip_even_patches(arr,nkpts) for arr in [k,en,colors,lws,h_text]]
-            data.append(go.Scatter(x=k,y=en,mode='markers', name=name,
-                        marker=dict(color=colors,size=lws,symbol=symbol),line=dict(width=0.001,
-                        color='rgba(255,255,250,0)'),showlegend=showlegend,hovertext=h_text)
-                        )
-        if mode == 'bands':
-            # idx should be a separate index for picking data, not same as labeling hovertext, because bands could be picked without a range but like 1,7,9 etc as well
-            for idx,lab,e,c,w,t in zip(range(len(_indices)),_indices,en,colors,lws,h_text):
-                line_color = 'rgb({},{},{})'.format(*np.max(clrs[idx],axis=0))
-                line_width = np.max(w)/8
-                data.append(go.Scatter(x=k,y=e,mode='markers+lines',
-                            name="{}<sub>{}</sub>".format(name,str(lab+1)),
-                            marker=dict(color=c,size=w,symbol=symbol),line_width= line_width,
-                            line_color=line_color,showlegend=showlegend,hovertext=t)
-                           )
-        return data
+    Parameters
+    ----------
+    path : path to `vasprun.xml` or auto picks in current directory.
+    bands : list of band indices [zero based here], In output data frame you will see corresponding band number based on full data.
+    atoms : list of atoms to plot. inner list contains ions indices. Can leave empty to discard projection data.
+    orbs : list of orbitals to plot. inner list contains orbitals indices. Can leave empty to discard projection data
+    skipk : if not None, auto skipped unnecessary k-points.
+    elim : if not None, filtered out unnecessary bands.
+    data : if not None, data is loaded from given data/pickle/json/dict and validated. Many other parameters are ignored when data is given.
+
+    Returns
+    -------
+    SpinDataFrame : dataframe with colums as k-points, eigenvalues[with fermi energy subtracted], spin components projected over selected ions and orbtials.
+
+    Methods
+    -------
+    sliced : Slice data in a plane orthogonal to given `column` at given `value`.
+    masked : Mask data over a constant value in a given column. Useful for plotting fermi level/surface.
+    splot : plot data in a 2D plot.
+    splot3d : plot data in a 3D plot.
+    join/append/concat/+/+= : Append another SpinDataFrame to this one with same columns and copy metadata.
+    send_metadata : Copy metadata from this to another SpinDataFrame, some methods may not carry over metadata, useful in that case.
+    get_data : Return data as collection of numpy arrays with kpoints already sent to BZ. Use .to_json() to export to json for plotting in other libraries/languages like Mathematica.
 
-# Cell
-def iplot2html(fig,filename=None,out_string=False,modebar=True):
-    """
-    - Writes plotly's figure as HTML file or display in IPython which is accessible when online. It is different than plotly's `fig.to_html` as it is minimal in memory. If you need to have offline working file, just use `fig.write_html('file.html')` which will be larger in size.
-    - **Parameters**
-        - fig      : A plotly's figure object.
-        - filename : Name of file to save fig. Defualt is None and show plot in Colab/Online or return hrml string.
-        - out_string: If True, returns HTML string, if False displays graph if possible.
+    All other methods are inherited from pd.DataFrame. If you apply some method that do not pass metadat, then use `send_metadata` to copy metadata to traget SpinDataFrame.
     """
-    import uuid # Unique div-id required,otherwise jupyterlab renders at one place only and overwite it.
-    div_id = "graph-{}".format(uuid.uuid1())
-    fig_json = fig.to_json()
-    # a simple HTML template
-    if filename:
-        _filename = gu.prevent_overwrite(filename)
-        template = """<html>
-        <head>
-        <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
-        </head>
-        <body>
-            <div id='{}'></div>
-            <script>
-                var fig_data = {}
-                Plotly.react('{}', fig_data.data, fig_data.layout);
-            </script>
-        </body>
-        </html>"""
-
-        # write the JSON to the HTML template
-        with open(_filename, 'w') as f:
-            f.write(template.format(div_id,fig_json,div_id))
-
-    else:
-        if modebar==True: #Only for docs issue
-            config = "{displayModeBar: true,scrollZoom: true}"
-        else:
-            config = "{displayModeBar: false,scrollZoom: true}"
-        template = """<div>
-        <script src='https://cdn.plot.ly/plotly-latest.min.js'></script>
-            <div id='{}'><!-- Plotly chart DIV --></div>
-            <script>
-                var data = {};
-                var config = {};
-                Plotly.newPlot('{}', data.data,data.layout,config);
-            </script>
-        </div>""".format(div_id,fig_json,config,div_id)
-        if out_string is True:
-            return template
-        else:
-            from IPython.display import HTML
-            return HTML(template)
 
-# Cell
-def iplot_rgb_lines(
-    path_evr    = None,
-    elements    = [[],[],[]],
-    orbs        = [[],[],[]],
-    labels      = ['','',''],
-    mode        = 'markers',
-    elim        = [],
-    Fermi     = None,
-    skipk       = None,
-    kseg_inds  = [],
-    max_width   = 6,
-    title       = None,
-    ktick_inds  = [0,-1],
-    ktick_vals  = ['Γ','M'],
-    figsize     = None,
-    interp_nk   = {},
-    query_data  = {}
+    _metadata = [
+        "_current_attrs",
+        "sys_info",
+        "poscar",
+        "projection",
+    ]  # These are passed after operations to new dataframe.
+
+    def __init__(
+        self,
+        *args,
+        path=None,
+        bands=[0],
+        projections={"A": ([0], [0])},
+        elim=None,
+        skipk=None,
+        data=None,
+        **kwargs,
     ):
-    """
-    - Returns plotly's figure object, takes care of spin-polarized calculations automatically. `elements`,`orbs` and `labels` are required to be one-to-one lists of size 3 where each item in list could be another list or integer.
-    - **Parameters**
-        - path_evr  : Path/to/vasprun.xml or xml output of `read_asxml`.
-        - elements   : List of size 3 of list of indices of ions. If not given, picks all ions for each orbital.
-        - orbs       : List of size 3 of list of orbital indices, if not gievn, s,p,d plotted.
-        - labels  : List of labels for projection.
-        - mode       : Three plotting modes are available:
-            - 'markers' : Plot whole data as a single scatter object. Its too fast.
-            - 'bands'   : Plot data such that each band is accessible via legend.
-            - 'lines'   : A replica of `matplotlib LineCollection` object. It plots at each point separately, slower than other two modes.
-
-        - interp_nk   : Dictionary with keys 'n' and 'k' for interpolation.
-        - figsize   : Tuple(width,height) in pixels, e.g. (700,400).
-        - query_data : Dictionary with keys as label and values as list of length 2. len(query_data) <=3 should hold for RGB plots. If given, used in place of elements, orbs and labels arguments.
-                        Example: {'s':([0,1],[0]),'p':([0,1],[1,2,3]),'d':([0,1],[4,5,6,7,8])} will pick up s,p,d orbitals of first two ions of system.
-        - **Other Parameters**
-            - ktick_inds, ktick_vals,elim,kseg_inds,max_width,title etc.
-    """
-    if mode not in ('markers','bands','lines'):
-        raise TypeError("Argument `mode` expects one of ['markers','bands','lines'], got '{}'.".format(mode))
-
-    vr = vp._validate_evr(path_evr=path_evr,skipk=skipk,elim=elim)
+        raise NotImplementedError("This class is not ready yet.")
+        if not (
+            path or args
+        ):  # It works fine without path given, but it is not recommended.
+            path = "./vasprun.xml"
+        if path or data:  # Don't updates args otherwise
+            for k in kwargs.keys():  # Do not let pass parameters to kwargs in this case
+                raise ValueError(f"SpinDataFrame got unexpected keyword argument {k!r}")
+
+            spin_data = None  # To avoid access before assignment
+            if data:
+                spin_data = serializer.SpinData.validated(data)
+            elif isinstance(path, str):
+                try:  # Check if 4 sets of data are there.
+                    spin_data = vp.export_spin_data(
+                        path, spins="sxyz", skipk=skipk, elim=elim
+                    )
+                except:  # If not 4 sets
+                    spin_data = vp.export_spin_data(
+                        path, spins="s", skipk=skipk, elim=elim
+                    )
+            else:
+                raise ValueError("Invalid path or data!")
 
-    # Fix orbitals, elements and labels lengths very early.
-    if query_data:
-        elements, orbs, labels = sp._format_input(query_data,rgb=False) # prefer over elements, orbs and labels
-    elements,orbs,labels = sp._validate_input(elements,orbs,labels,vr.sys_info,rgb=True)
-
-    ## Main working here.
-    if vr.pro_bands == None:
-        raise ValueError("Can not plot an empty eigenvalues object.\n"
-                         "Try with large energy range.")
-
-    if Fermi == None:
-        Fermi = vr.fermi
-    K = vp.join_ksegments(vr.kpath,kseg_inds = kseg_inds)
-    xticks=[K[i] for i in ktick_inds]
-    xlim=[min(K),max(K)]
-    if elim:
-        ylim = [min(elim),max(elim)]
-    else:
-        ylim=[-10,10]
-    #====Title Name======
-    SYSTEM=vr.sys_info.SYSTEM
-    if title == None:
-        title= "{}[{}]".format(SYSTEM,','.join(labels))
-    # After All Fixing
-    ISPIN=vr.sys_info.ISPIN
-    args_dict=dict(orbs=orbs,elements=elements,interp_nk=interp_nk) # Do not scale color there, scale here.
-    data,showlegend,name=[],False,'' # Place holder
-
-    if mode=='bands':
-            showlegend=True
-    kpoints = vr.kpoints
-    if ISPIN == 1:
-        En=vr.bands.evals-Fermi
-        Oc = vr.bands.occs
-        Pros=vr.pro_bands.pros
-        new_args=dict(kpath=K, evals_set=En, pros_set=Pros, occs_set = Oc, **args_dict)
-        rgb_lines=_get_rgb_data(kpoints = kpoints,**new_args)
-        data=_rgb2plotly(rgb_data=rgb_lines,mode=mode,showlegend=showlegend,
-                           labels=labels,name='B',max_width=max_width,bands_indices= vr.bands.indices)
-    if ISPIN == 2:
-        if mode == 'markers':
-            showlegend=True
-        En1=vr.bands.evals.SpinUp-Fermi
-        En2=vr.bands.evals.SpinDown-Fermi
-        Oc1 = vr.bands.occs.SpinUp
-        Oc2 = vr.bands.occs.SpinDown
-        Pros1=vr.pro_bands.pros.SpinUp
-        Pros2=vr.pro_bands.pros.SpinDown
-        new_args1=dict(kpath=K, evals_set=En1, pros_set=Pros1,occs_set = Oc1,**args_dict)
-        rgb_lines1=_get_rgb_data(kpoints = kpoints,**new_args1)
-        data1=_rgb2plotly(rgb_data=rgb_lines1,mode=mode,symbol=0,showlegend=showlegend,
-                            labels=labels,name='B<sup>↑</sup>',max_width=max_width,bands_indices= vr.bands.indices)
-        new_args2=dict(kpath=K, evals_set=En2, pros_set=Pros2,occs_set = Oc2,**args_dict)
-        rgb_lines2=_get_rgb_data(kpoints = kpoints,**new_args2)
-        data2=_rgb2plotly(rgb_data=rgb_lines2,mode=mode,symbol=100,showlegend=showlegend,
-                            labels=labels,name='B<sup>↓</sup>',max_width=max_width,bands_indices= vr.bands.indices)
-        data=[[d1,d2] for d1,d2 in zip(data1,data2)]
-        data=[d for ds in data for d in ds]
-
-    # Initiate figure
-    fig=go.Figure(data=data)
-    fig.update_layout(title=title,margin=go.layout.Margin(l=60,r=50,b=40,t=75,pad=0),
-            yaxis=go.layout.YAxis(title_text='Energy (eV)',range=ylim),
-            xaxis=go.layout.XAxis(ticktext=ktick_vals, tickvals=xticks,tickmode="array",range=xlim),
-            font=dict(family="stix, serif",size=14))
-    if(figsize!=None):
-        fig.update_layout(width=figsize[0],height=figsize[1],autosize=False)
-    #Draw lines at breakpoints
-    if kseg_inds:
-        kargs_dict = dict(mode='lines',line=dict(color='rgb(222,222,222)',width=1.2),showlegend=False)
-        for pt in kseg_inds:
-            fig.add_trace(go.Scatter(x=[K[pt],K[pt]],y=ylim,**kargs_dict))
-            fig.add_trace(go.Scatter(x=[K[pt],K[pt]],y=ylim,**kargs_dict))
-    update_args = dict(linewidth=0.1,linecolor='rgba(222,222,222,0.1)', mirror=True)
-    fig.update_xaxes(showgrid=True,zeroline=False,showline=True,**update_args)
-    fig.update_yaxes(showgrid=False,zeroline=True,showline=True,**update_args)
-    return fig
-
-# Cell
-def iplot_dos_lines(
-    path_evr      = None,
-    elements      = [[0,],],
-    orbs          = [[0],],
-    labels        = ['s',],
-    elim          = [],
-    colormap      = 'gist_rainbow',
-    tdos_color    = (0.5,0.95,0),
-    linewidth     = 2,
-    fill_area     = True,
-    vertical      = False,
-    Fermi       = None,
-    figsize       = None,
-    spin          = 'both',
-    interp_nk     = {},
-    title         = None,
-    query_data    = {}
+            if spin_data:
+                out_dict = _collect_spin_data(
+                    spin_data, bands=bands, atoms=atoms, orbs=orbs
+                )
+                super().__init__(out_dict)
+                self.sys_info = spin_data.sys_info
+                atoms, orbs, *_ = _format_input(projections, sys_info=self.sys_info)
+                self.projection = serializer.Dict2Data(
+                    {
+                        f"_{i}": {"ions": e, "orbs": o}
+                        for i, (e, o) in enumerate(zip(atoms, orbs))
+                    }
+                )
+                # Path below is used to get kpoints info
+                self.poscar = POSCAR(path=path, data=spin_data.poscar)
+                self._current_attrs = {
+                    "cmap": "viridis"
+                }  # To store attributes of current plot for use in colorbar.
+
+        else:  # This part is only for operations on dataframe.
+            if (
+                len(args) == 1
+            ):  # This gives hack to load data from a file in current directory.
+                if (args[0] is None) or isinstance(
+                    args[0], str
+                ):  # If path is given as positional argument
+                    raise ValueError("SpinDataFrame expects no positional argument!")
+            super().__init__(*args, **kwargs)
+
+    @property
+    def _constructor(self):
+        "That's main hero of this class. This is called when you apply some method of slice it."
+        return SpinDataFrame
+
+    @property
+    def fermi(self):
+        "Fermi energy based on occupancy. Returns `self.Fermi` if occupancies cannot be resolved."
+        return self.sys_info.fermi
+
+    @property
+    def Fermi(self):
+        "Fermi energy given in vasprun.xml."
+        return self.sys_info.Fermi
+
+    def append(self, other):
+        "Append another SpinDataFrame to this one with same columns."
+        for k in other.columns:
+            if k not in self.columns:
+                raise ValueError(f"Column {k} in other is not not in this DataFrame!")
+        if len(self.columns) != len(other.columns):
+            raise ValueError("Columns are not same!")
+        out_df = super().append(other)
+        self.send_metadata(out_df)
+        return out_df
+
+    def join(self, other):
+        "Same as self.append"
+        return self.append(other)
+
+    def concat(self, other):
+        "Same as self.append"
+        return self.append(other)
+
+    def __add__(self, other):
+        "Same as self.append"
+        return self.append(other)
+
+    def get_data(self, shift=0):
+        """Access Data with transformed KPOINTS based on current Brillouin Zone.
+        shift is used to shift kpoints before any other operation.
+        If You need to have kpoints in primitive/regular BZ, first use .poscar.get_bz() that set that kind of BZ.
+        """
+        bands = np.unique(self["band"].to_numpy()).astype(int)
+        out_dict = {"SYSTEM": self.sys_info.SYSTEM}
+        out_dict["atoms"] = self.poscar.data.types
+        out_dict["orbitals"] = self.sys_info.fields
+        out_dict["projection"] = self.projection
+        out_dict["bz"] = self.poscar.bz.to_dict()
+        out_dict["bz"]["specials"] = self.poscar.bz.specials.to_dict()
+        out_dict["bz"][
+            "normals"
+        ] = self.poscar.bz.normals._asdict()  # Named tuple to dict
+
+        for band in bands:
+            name = f"band_{band}"
+            df = self[self["band"] == band].sort_values(by=["kx", "ky", "kz"])
+            kx, ky, kz = df.poscar.bring_in_bz(
+                df[["kx", "ky", "kz"]].to_numpy(), sys_info=df.sys_info, shift=shift
+            ).T
+            out_dict[name] = {"kx": kx, "ky": ky, "kz": kz}
+
+            for k in df.columns:
+                if k not in ("band", *out_dict[name].keys()):
+                    out_dict[name][k] = df[k].to_numpy()
+
+        return serializer.Dict2Data(out_dict)
+
+    def masked(self, column, value, tol=1e-2, n=None, band=None, method="linear"):
+        """Mask dataframe with a given value, using a tolerance.
+        If n is given, (band should also be given to avoid multivalued interpolation error) data values are interpolated to grid of size (l,m,n) where n is longest side.
+        n could be arbirarily large as mask will filter out data outside the tolerance.
+        """
+        if n and not isinstance(n, (int, np.integer)):
+            raise TypeError(
+                "`n` must be an integer to be applied to short side of grid."
+            )
+        if isinstance(n, (int, np.integer)) and not isinstance(band, (int, np.integer)):
+            raise ValueError(
+                "A single `band`(int) from dataframe must be given to mask data."
+                "Interpolation does not give correct results for multiple values over a point (x,y,z)."
+            )
+
+        column_vals = self[column].to_numpy()
+        cmin, cmax = column_vals.min(), column_vals.max()
+        if (value < cmin) or (value > cmax):
+            raise ValueError("value is outside of column data range!")
+
+        df = self.copy()  # To avoid changing original dataframe
+        if n and band:
+            bands_exist = np.unique(self.band)
+            if band not in bands_exist:
+                raise ValueError(
+                    "Band {} is not in dataframe! Available: {}".format(
+                        band, bands_exist
+                    )
+                )
+
+            _self_ = df[df["band"] == band]  # Single band dataframe
+            df.drop(df.index, inplace=True)  # only columns names there and metadata
+            kxyz = _self_[["kx", "ky", "kz"]].to_numpy()
+            lx, *_, hx = _self_["kx"].sort_values(inplace=False)
+            ly, *_, hy = _self_["ky"].sort_values(inplace=False)
+            lz, *_, hz = _self_["kz"].sort_values(inplace=False)
+            vs = np.array([hx - lx, hy - ly, hz - lz])
+            nx, ny, nz = nxyz = (vs / vs.max() * n).astype(int)
+            nijk = [i for i, n in enumerate(nxyz) if n > 0]
+
+            if len(nijk) < 2:
+                raise ValueError(
+                    "At least two of kx,ky,kz must have non-coplanar points."
+                )
+
+            if len(nijk) == 3:
+                xyz = kxyz.T
+                XYZ = [
+                    a.flatten()
+                    for a in np.mgrid[
+                        lx : hx : nx * 1j, ly : hy : ny * 1j, lz : hz : nz * 1j
+                    ]
+                ]
+                for name, index in zip("xyz", range(3)):
+                    df[f"k{name}"] = XYZ[index]
+            else:
+                [l1, l2], [h1, h2], [n1, n2] = np.array(
+                    [[lx, ly, lz], [hx, hy, hz], [nx, ny, nz]]
+                )[:, nijk]
+                xyz = kxyz.T[nijk]
+                XYZ = [
+                    a.flatten() for a in np.mgrid[l1 : h1 : n1 * 1j, l2 : h2 : n2 * 1j]
+                ]
+                for name, index in zip("xyz", range(3)):
+                    if index in nijk:
+                        df[f"k{name}"] = XYZ[index]
+                    else:
+                        df[f"k{name}"] = np.zeros_like(XYZ[0])
+
+            for c in [_c for _c in _self_.columns if _c not in "kxkykz"]:
+                df[c] = griddata(
+                    tuple(xyz), _self_[c].to_numpy(), tuple(XYZ), method=method
+                )
+
+            del _self_  # To free memory
+
+            df = df.round(6).dropna()
+
+            # SCALE DATA NOTE: See if negative peak to peak scaling required
+            _max = []
+            for k in [c for c in df.columns if c.startswith("s")]:
+                _max.append(np.abs(df[k]).max())
+
+            _max = max(_max)
+            for k in [c for c in df.columns if c.startswith("s")]:
+                df[k] = df[k] / (_max if _max != 0 else 1)
+
+        # Make sure to keep metadata, it doesn't work otherwise.
+        self.send_metadata(df)
+
+        # Sort based on distance, so arrows are drawn in correct order
+        out_df = df[
+            np.logical_and((df[column] < (value + tol)), (df[column] > (value - tol)))
+        ]
+        return out_df.sort_values(by=["kx", "ky", "kz"])
+
+    def send_metadata(self, target_spin_dataframe):
+        "Copy metadata from this to another SpinDataFrame."
+        for k in self._metadata:
+            setattr(target_spin_dataframe, k, getattr(self, k))
+
+    def sliced(self, column="kz", value=0):
+        "Slice data in a plane orthogonal to given `column` at given `value`"
+        return self[self[column] == value]
+
+    def _collect_arrows_data(self, arrows):
+        arrows_data = []
+        for arr in arrows:
+            if arr not in ["", *self.columns]:
+                raise ValueError(f"{arr!r} is not a column in the dataframe")
+            arrows_data.append(
+                self[arr] if arr else np.zeros_like(self["kx"].to_numpy())
+            )
+
+        return np.array(arrows_data).T
+
+    def _collect_kxyz(self, *xyz, shift=0):
+        "Return tuple(kxyz, k_order)"
+        _kxyz = ["kx", "ky", "kz"]
+        kij = [_kxyz.index(a) for a in xyz if a in _kxyz]
+        kxyz = self[["kx", "ky", "kz"]].to_numpy()
+        kxyz = self.poscar.bring_in_bz(kxyz, sys_info=self.sys_info, shift=shift)
+
+        # Handle third axis as energy as well
+        if len(xyz) == 3 and xyz[2].startswith("e"):
+            kxyz[:, 2] = self[xyz[2]].to_numpy()
+            kij = [*kij, 2]  # Add energy to kij, it must be of size 2 before
+
+        return kxyz, kij
+
+    def _validate_columns(self, *args):
+        for arg in args:
+            if arg not in self.columns:
+                raise ValueError(f"{arg!r} is not a column in the dataframe")
+
+    def splot(
+        self,
+        *args,
+        arrows=[],
+        every=1,
+        norm=1,
+        marker="H",
+        ax=None,
+        quiver_kws={},
+        shift=0,
+        **kwargs,
     ):
         """
-        - Returns plotly's figure. If given,elements,orbs colors, and labels must have same length. If not given, zeroth ions is plotted with s-orbital.
-        - **Parameters**)
-            - path_evr   : Path/to/vasprun.xml or output of `export_vasprun`. Auto picks in CWD.
-            - elements   : List [[0,],] of ions indices, by defualt plot first ion's projections.
-            - orbs       : List [[0,],] lists of indices of orbitals, could be empty.
-            - labels     : List [str,] of orbitals labels. len(labels) == len(orbs) must hold.
-            - elim       : [min,max] of energy range.
-            - Fermi    : If not given, automatically picked from `export_vasprun`.
-            - colormap   : Matplotlib's standard color maps. Default is 'gist_ranibow'. Use 'RGB' if want to compare with `iplot_rgb_lines` with 3 projection inputs (len(orbs)==3).
-            - fill_area  : Default is True and plots filled area for dos. If False, plots lines only.
-            - vertical   : False, If True, plots along y-axis.
-            - interp_nk  : Dictionary with keys 'n' and 'k' for interpolation.
-            - figsize    : Tuple(width,height) in pixels, e.g. (700,400).
-            - query_data : Dictionary with keys as label and values as list of length 2. If given, used in place of elements, orbs and labels arguments.
-                        Example: {'s':([0,1],[0]),'p':([0,1],[1,2,3]),'d':([0,1],[4,5,6,7,8])} will pick up s,p,d orbitals of first two ions of system.
-        - **Returns**
-            - fig        : Plotly's figure object.
+        Plot energy in 2D with/without arrows.
+
+        Parameters
+        ----------
+        *args : 3 or 4 names of columns, representing [X,Y,Energy,[Anything]], from given args, last one is colormapped. If kwargs has color, that takes precedence.
+        arrows : 2 or 3 names of columns, representing [U,V,[color]]. If quiver_kws has color, that takes precedence.
+        every : every nth point is plotted as arrow.
+        norm : normalization factor for size of arrows.
+        marker : marker to use for scatter, use s as another argument to change size.
+        ax : matplotlib axes to plot on (defaults to auto create one).
+        quiver_kws : these are passed to matplotlib.pyplot.quiver.
+        shift : A number or a list of three numbers that will be added to kpoints before any other operation.
+
+        **kwargs are passed to matplotlib.pyplot.scatter.
+
+        Returns
+        --------
+        ax : matplotlib axes. It has additinal method `colorbar` to plot colorbar from most recent plot.
         """
-        if query_data:
-            elements,orbs,labels = sp._format_input(query_data,rgb=False) # prefer query_data over elements,orbs,labels
-            # These are validated inisde _collect_dos, no need here
-        en,tdos,pdos,vr=None,None,None,None # Place holders for defining
-        cl_dos = sp._collect_dos(path_evr=path_evr,elim=elim,
-                            elements=elements, orbs=orbs,labels=labels,
-                            Fermi=Fermi, spin='both',interp_nk=interp_nk)
-        try:
-            en,tdos,pdos,labels,vr = cl_dos
-        except:
-            raise ValueError("Try with large energy range.")
-
-        labels=[label.replace('$','').replace('^↑','<sup>↑</sup>').replace('^↓','<sup>↓</sup>') for label in labels]
-        # Make additional colors for spin down. Inverted colors are better.
-        if(elim):
-            ylim=[min(elim),max(elim)]
+        if arrows and len(arrows) not in [2, 3]:
+            raise ValueError(
+                '`arrows ` requires 2 or 3 items form spin data [s1,s2,[color]], one of s1,s2 could be "".'
+            )
+        if len(args) not in [3, 4]:
+            raise ValueError(
+                "splot takes 3 or 4 positional arguments [X,Y,E,[Anything]], last one is colormapped if kwargs don't have color."
+            )
+
+        self._validate_columns(*args)
+        kxyz, kij = self._collect_kxyz(*args[:2], shift=shift)
+        ax = ax or ptk.get_axes()
+        minmax_c = [0, 1]
+        cmap = kwargs.get("cmap", self._current_attrs["cmap"])
+
+        if arrows:
+            arrows_data = self._collect_arrows_data(arrows)
+            cmap = quiver_kws.get("cmap", cmap)
+            if "color" in quiver_kws:
+                cmap = None  # No colorbar for color only
+                arrows_data = arrows_data[:, :2]  # color takes precedence
+            ax.quiver(
+                *kxyz[::every].T[kij], *(norm * arrows_data[::every].T), **quiver_kws
+            )
+
+            if len(arrows) == 3 and "color" not in quiver_kws:
+                cmap = quiver_kws.get("cmap", "viridis")  # Fallback to default
+                minmax_c = [arrows_data[:, 2].min(), arrows_data[:, 2].max()]
         else:
-            ylim=[-10,10]
-        # Fix elements and colors length
-        if colormap in plt.colormaps():
-            from matplotlib.pyplot import cm
-            if len(tdos) == 2:
-                c_map   = cm.get_cmap(colormap)
-                c_vals  = np.linspace(0,1,2*len(orbs))
-                colors  = c_map(c_vals)
-            else:
-                c_map   = cm.get_cmap(colormap)
-                c_vals  = np.linspace(0,1,len(orbs))
-                colors  = c_map(c_vals)
-            # Fix for RGB comparison
-            if len(tdos) == 2 and 'both' in spin and len(orbs)==3:
-                colors[[-1,-2]]= colors[[-2,-1]] #Flip last two colors only
+            _C = self[args[-1]]  # Most right arg is color mapped
+            kwargs["marker"] = marker  # Avoid double marker
+            if "color" in kwargs:
+                kwargs["c"] = kwargs["color"]
+                del kwargs["color"]  # keep one
+                cmap = None  # No colorbar
+
+            kwargs["c"] = kwargs.get("c", _C)
+            ax.scatter(*kxyz.T[kij], **kwargs)
+            minmax_c = [min(_C), max(_C)]
+
+        self._current_attrs = {"ax": ax, "minmax_c": minmax_c, "cmap": cmap}
+        return ax
+
+    def splot3d(
+        self,
+        *args,
+        arrows=[],
+        every=1,
+        norm=1,
+        marker="H",
+        ax=None,
+        quiver_kws={"arrowstyle": "-|>", "size": 1},
+        shift=0,
+        **kwargs,
+    ):
+        """
+        Plot energy in 3D with/without arrows.
+
+        Parameters
+        ----------
+        *args : 3, 4 or 5 names of columns, representing [X,Y,[Z or Energy],Energy, [Anything]], out of given args, last one is color mapped. if kwargs has color, that takes precedence.
+        arrows : 3 or 4 names of columns, representing [U,V,W,[color]]. If color is not given, magnitude of arrows is color mapped. If quiver_kws has color, that takes precedence.
+        every : every nth point is plotted as arrow.
+        norm : normalization factor for size of arrows.
+        marker : marker to use for scatter, use s as another argument to change size.
+        ax : matplotlib 3d axes to plot on (defaults to auto create one).
+        quiver_kws : these are passed to ipyvasp.quiver3d.
+        shift : A number or a list of three numbers that will be added to kpoints before any other operation.
+
+        **kwargs are passed to matplotlib.pyplot.scatter.
+
+        Returns
+        -------
+        ax : matplotlib 3d axes. It has additinal method `colorbar` to plot colorbar from most recent plot.
+        """
+        if arrows and len(arrows) not in [3, 4]:
+            raise ValueError(
+                '`arrows ` requires 3 or 4 items form spin data [s1,s2, s2, [color]], one of s1,s2,s3 could be "".'
+            )
+        if len(args) not in [3, 4, 5]:
+            raise ValueError(
+                "splot3d takes 3, 4 or 5 positional arguments [X,Y,E] or [X,Y,Z,E,[Anything]], right-most is color mapped if kwargs don't have color."
+            )
+
+        if not args[2][0] in "ek":
+            raise ValueError("Z axis must be in [kx,ky,kz, energy]!")
+
+        self._validate_columns(*args)
+        kxyz, kij = self._collect_kxyz(*args[:3], shift=shift)
+        ax = ax or ptk.get_axes(axes_3d=True)
+        minmax_c = [0, 1]
+        cmap = kwargs.get("cmap", self._current_attrs["cmap"])
+
+        if arrows:
+            arrows_data = self._collect_arrows_data(arrows)
+            cmap = quiver_kws.get("cmap", cmap)
+            if "color" in quiver_kws:  # color takes precedence
+                quiver_kws["C"] = quiver_kws["color"]
+                quiver_kws.pop("color")  # It is not in FancyArrowPatch
+                cmap = None  # No colorbar
+            elif len(arrows) == 4:
+                array = arrows_data[::every, 3]
+                array = (array - array.min()) / np.ptp(array)
+                quiver_kws["C"] = plt.get_cmap(cmap)(array)
+                minmax_c = [arrows_data[:, 3].min(), arrows_data[:, 3].max()]
+            elif len(arrows) == 3:
+                array = np.linalg.norm(arrows_data[::every, :3], axis=1)
+                minmax_c = [array.min(), array.max()]  # Fist set then normalize
+                array = (array - array.min()) / np.ptp(array)
+                quiver_kws["C"] = plt.get_cmap(cmap)(array)
+
+            if "cmap" in quiver_kws:
+                quiver_kws.pop("cmap")  # It is not in quiver3d
+
+            ptk.quiver3d(
+                *kxyz[::every].T[kij],
+                *(norm * arrows_data[::every].T[:3]),
+                **quiver_kws,
+                ax=ax,
+            )
+
         else:
-            raise ValueError("`colormap` expects one of the follwoing:\n{}".format(plt.colormaps()))
-        # Total DOS colors
-        t_color=mpl.colors.to_rgb(tdos_color)
-        it_color=gu.transform_color(t_color,c = -1) #inverts for c = -1
-        #========Title Name========
-        SYSTEM=vr.sys_info.SYSTEM
-        if(title==None):
-            title="{}".format(SYSTEM)
-
-        fig = go.Figure()
-        fig.update_layout(title=title,margin=go.layout.Margin(l=60,r=50,b=40,t=75,pad=0),\
-                          font=dict(family="stix, serif",size=14))
-        if(figsize!=None):
-            fig.update_layout(width=figsize[0],height=figsize[1],autosize=False)
-        if(vertical==False):
-            if(fill_area==False):
-                fill=None
-            if(fill_area==True):
-                fill='tozeroy'
-            args_dic=dict(mode='lines',line_width=linewidth,fill=fill)
-            fig.update_xaxes(range=ylim,title='Energy (eV)')
-            if(len(tdos)==2):   # Spin polarized.
-                fig.add_scatter(x=en,y=tdos[0],line_color='rgb({},{},{})'.format(*[int(255*i) for i in t_color]),\
-                                 name='TDOS<sup>↑</sup>',**args_dic)
-                fig.add_scatter(x=en,y=tdos[1],line_color='rgb({},{},{})'.format(*[int(255*i) for i in it_color]),\
-                                 name='TDOS<sup>↓</sup>',**args_dic)
-            else:   # unpolarized.
-                fig.add_trace(go.Scatter(x=en,y=tdos,line_color='rgb({},{},{})'.format(*[int(255*i) for i in t_color]),\
-                              name='TDOS',**args_dic))
-            for p,l,c in zip(pdos,labels,colors):
-                fig.add_trace(go.Scatter(x=en,y=p,line_color='rgb({},{},{})'.format(*[int(255*i) for i in c]),\
-                               name=l,**args_dic))
-        if(vertical==True):
-            if(fill_area==False):
-                fill=None
-            if(fill_area==True):
-                fill='tozerox'
-            args_dic=dict(mode='lines',line_width=linewidth,fill=fill)
-            fig.update_yaxes(range=ylim,title='Energy (eV)')
-            if(len(tdos)==2):   # Spin polarized.
-                fig.add_scatter(y=en,x=tdos[0],line_color='rgb({},{},{})'.format(*[int(255*i) for i in t_color]),\
-                                name='TDOS<sup>↑</sup>',**args_dic)
-                fig.add_scatter(y=en,x=tdos[1],line_color='rgb({},{},{})'.format(*[int(255*i) for i in it_color]),\
-                                name='TDOS<sup>↓</sup>',**args_dic)
-            else:   # unpolarized.
-                fig.add_trace(go.Scatter(y=en,x=tdos,line_color='rgb({},{},{})'.format(*[int(255*i) for i in t_color]),\
-                                name='TDOS',**args_dic))
-            for p,l,c in zip(pdos,labels,colors):
-                fig.add_trace(go.Scatter(y=en,x=p,line_color='rgb({},{},{})'.format(*[int(255*i) for i in c]),\
-                                name=l,**args_dic))
-        fig.update_xaxes(showgrid=True, zeroline=True,showline=True, linewidth=0.1, linecolor='rgba(222,222,222,0.1)', mirror=True)
-        fig.update_yaxes(showgrid=True, zeroline=True,showline=True, linewidth=0.1, linecolor='rgba(222,222,222,0.1)', mirror=True)
-        return fig
+            _C = self[args[-1]]  # Most righht arg is color mapped
+            kwargs["marker"] = marker  # Avoid double marker
+            if "color" in kwargs:
+                kwargs["c"] = kwargs["color"]
+                del kwargs["color"]  # keep one
+                cmap = None  # No colorbar
+
+            kwargs["c"] = kwargs.get("c", _C)
+            ax.scatter(*kxyz.T[kij], **kwargs)
+            minmax_c = [min(_C), max(_C)]
+
+        self._current_attrs = {"ax": ax, "minmax_c": minmax_c, "cmap": cmap}
+        return ax
+
+    def colorbar(self, cax=None, nticks=6, digits=2, **kwargs):
+        "Add colobar to most recent plot. kwargs are passed to ipyvasp.splots.add_colorbar"
+        if not self._current_attrs["ax"]:
+            raise ValueError(
+                "No plot has been made yet by using `splot, splot3d` or already consumed by `colorbar`"
+            )
+        if not self._current_attrs["cmap"]:
+            raise ValueError("No Mappable for colorbar found!")
+
+        ax = self._current_attrs["ax"]
+        cmap = self._current_attrs["cmap"]
+        minmax_c = self._current_attrs["minmax_c"]
+        self._current_attrs["ax"] = None  # Reset
+        self._current_attrs["cmap"] = None  # Reset
+        if ax.name == "3d":
+            cax = cax or plt.gcf().add_axes([0.85, 0.15, 0.03, 0.7])
+
+        return ptk.add_colorbar(
+            ax,
+            cmap,
+            cax=cax,
+            ticks=np.linspace(*minmax_c, nticks, endpoint=True),
+            digits=digits,
+            **kwargs,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ipyvasp-0.1.0/ipyvasp/serializer.py` & `ipyvasp-0.2.0/ipyvasp/lattice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,450 +1,535 @@
-import os
-import json
-import pickle
-from collections import namedtuple
-from contextlib import suppress
-from copy import deepcopy
+__all__ = ["POSCAR", "download_structure", "periodic_table", "get_kpath", "get_kmesh"]
+
+from pathlib import Path
+from contextlib import redirect_stdout
+from io import StringIO
 
 import numpy as np
+from pandas.io.clipboard import clipboard_get, clipboard_set
 
 
-def dict2tuple(name,d):
-    """Converts a dictionary (nested as well) to namedtuple, accessible via index and dot notation as well as by unpacking.
-    - **Parameters**
-        - name: Name of the tuple.
-        - d   : Dictionary, nested works as well.
-    """
-    return namedtuple(name,d.keys())(
-           *(dict2tuple(k.upper(),v) if isinstance(v,dict) else v for k,v in d.items())
-           )
-
-class Dict2Data:
-    _req_keys = ()
-    _subclasses = ()
-    """
-    - Returns a Data object with dictionary keys as attributes of Data accessible by dot notation or by key. Once an attribute is created, it can not be changed from outside.
-    - **Parmeters**
-        - dict : Python dictionary (nested as well) containing any python data types.
-    - **Methods**
-        - to_dict  : Converts a Data object to dictionary if it could be made a dictionary, otherwise throws relevant error.
-        - to_json  : Converts to json str or save to file if `outfil` given. Accepts `indent` as parameter.
-        - to_pickle: Converts to bytes str or save to file if `outfile` given.
-        - to_tuple : Converts to a named tuple.
-    - **Example**
-        > x = Dict2Data({'A':1,'B':{'C':2}})
-        > x
-        > Data(
-        >     A = 1
-        >     B = Data(
-        >         C = 2
-        >         )
-        >     )
-        > x.B.to_dict()
-        > {'C': 2}
-    """
-    def __init__(self,d):
-        if not hasattr(self.__class__,'_req_keys'):
-            raise AttributeError("Derived class of `Dict2Data` should have attribute '_req_keys'")
-        if isinstance(d,(self.__class__, Dict2Data)):
-            d = d.to_dict() # if nested Dict2Data , must expand
-        # Check if all required keys are present in main level of subclasses
-        for key in self.__class__._req_keys:
-            if key not in d:
-                raise ValueError(f"Invalid input for {self.__class__.__name__}")
-        # ===================
-        for a,b in d.items(): 
-            if isinstance(b,(self.__class__, Dict2Data)):
-                b = b.to_dict() # expands self instance !must here.
-            
-            if a == 'poscar' and 'extra_info' in b:
-                setattr(self,a, PoscarData(b)) # Enables custom methods for PoscarData
-            elif isinstance(b,(list,tuple)):
-                setattr(self,a,[Dict2Data(x) if isinstance(x,dict) else x for x in b])
-            else:
-                setattr(self,a,Dict2Data(b) if isinstance(b,dict) else b)
-    
-    @classmethod
-    def validated(cls, data):
-        "Validate data like it's own or from json/pickle file/string."
-        if isinstance(data,cls):
-            return data
-        
-        if isinstance(data,(str,bytes)):
-            new_data = load(data)
-            if not isinstance(new_data,cls):
-                raise TypeError(f"Data is not of type {cls}.")
-            return new_data
-        
-        if isinstance(data,Dict2Data) and cls is not Dict2Data: # Check for other classes strictly   
-            data_keys = data.keys()
-            for key in cls._req_keys:
-                if key not in data_keys:
-                    raise KeyError(f"Invalid data for {cls.__name__}")
-            
-        return cls(data) # make of that type at end
-        
-    def to_dict(self):
-        """Converts a `Dict2Data` object (root or nested level) to a dictionary.
-        """
-        result = {}
-        for k,v in self.__dict__.items():
-            if isinstance(v,(self.__class__,Dict2Data)):
-                result.update({k:Dict2Data.to_dict(v)})
-            else:
-                result.update({k:v})
-        return deepcopy(result) # prevent accidental changes in numpy arrays
-    
-    def copy(self):
-        "Copy of self to avoid changes during inplace operations on numpy arrays."
-        return self.__class__(self.to_dict()) # make a copy of self through dictionary, otherwise it does not work
-    
-    def to_json(self,outfile:str = None,indent:int = 1):
-        """Dumps a `Dict2Data` object (root or nested level) to json.
-        - **Parameters**
-            - outfile : Default is None and returns string. If given, writes to file.
-            - indent  : Json indent. Default is 1.
+from .core import serializer
+from .core import spatial_toolkit as stk
+from .utils import _sig_kwargs, _sub_doc
+from . import _lattice as plat
+from ._lattice import (
+    periodic_table,
+    get_kpath,
+    get_kmesh,
+)  # need these as direct access
+
+
+def download_structure(
+    formula, mp_id=None, max_sites=None, min_sites=None, api_key=None, save_key=False
+):
+    """
+    Download structure data from Materials project website.
+
+    Parameters
+    ----------
+    formula : chemical formula of the material.
+    mp_id : Materials project id of material.
+    max_sites : maximum number of sites in structure to download.
+    min_sites : minimum number of sites in structure to download.
+
+    Other Parameters
+    ----------------
+    api_key : API key from Materials project websit, if you use save_key=True, never required again.
+    save_key : Save API key to file. You can save any time of key or device changed.
+
+    Return
+    ------
+    list : List of Structure data containing attribute/method `cif`/`export_poscar, write_cif` etc.
+
+
+    .. note::
+        max_sites and min_sites are used to filter the number of sites in structure, or use mp_id to download a specific structure.
+    """
+    mp = plat.InvokeMaterialsProject(api_key=api_key)
+    output = mp.request(
+        formula=formula, mp_id=mp_id, max_sites=max_sites, min_sites=min_sites
+    )  # make a request
+    if save_key and isinstance(api_key, str):
+        mp.save_api_key(api_key)
+    if mp.success:
+        return output
+    else:
+        raise ConnectionError("Connection was not sccessful. Try again!")
+
+
+class POSCAR:
+    _cb_instance = {}  # Loads last clipboard data if not changed
+    _mp_instance = {}  # Loads last mp data if not changed
+
+    def __init__(self, path=None, content=None, data=None):
         """
-        return dump(self,dump_to='json',outfile=outfile,indent=indent)
+        POSCAR class to contain data and related methods, data is PoscarData, json/tuple file/string.
+        Do not use `data` yourself, it's for operations on poscar.
 
-    def to_pickle(self,outfile:str=None):
-        """Dumps a `Dict2Data` or subclass object (root or nested level) to pickle.
-        - **Parameters**
-            - outfile : Default is None and returns string. If given, writes to file.
+        Parameters
+        ----------
+        path : path to file
+        content : string of POSCAR content
+        data : PoscarData object. This assumes positions are in fractional coordinates.
+
+        Prefrence order: data > content > path
         """
-        return dump(self,dump_to='pickle',outfile=outfile)
+        self._path = Path(path or "POSCAR")  # Path to file
+        self._content = content
 
-    def to_tuple(self):
-        """Creates a namedtuple."""
-        return dict2tuple('Data',self.to_dict())
+        if data:
+            self._data = serializer.PoscarData.validated(data)
+        else:
+            self._data = plat.export_poscar(path=str(self.path), content=content)
+        # These after data to work with data
+        self._bz = self.get_bz(primitive=False)  # Get defualt regular BZ from sio
+        self._cell = self.get_cell()  # Get defualt cell
+        self._plane = None  # Get defualt plane, changed with splot_bz
+        self._ax = None  # Get defualt axis, changed with splot_bz
 
     def __repr__(self):
-        items= []
-        for k,v in self.__dict__.items():
-            if type(v) not in (str,float,int,range,bool,None,True,False) and not isinstance(v,Dict2Data):
-                if isinstance(v,np.ndarray):
-                    v = "<{}:shape={}>".format(v.__class__.__name__,np.shape(v))
-                elif type(v) in (list,tuple):
-                    v = ("<{}:len={}>".format(v.__class__.__name__,len(v)) if len(v) > 10 else v)
-                else:
-                    v = v.__class__
-            if isinstance(v,Dict2Data):
-                v = repr(v).replace("\n","\n    ")
-            items.append(f"    {k} = {v}")
-
-        return "Data(\n{}\n)".format('\n'.join(items))
-    def __getstate__(self):
-        pass  #This is for pickling
-
-    def __setattr__(self, name, value):
-        if name in self.__dict__:
-            raise AttributeError(f"Outside assignment is restricted for already present attribute.")
+        atoms = ", ".join([f"{k}={len(v)}" for k, v in self._data.types.items()])
+        lat = ", ".join(
+            [
+                f"{k}={v}"
+                for k, v in zip(
+                    "abcαβγ", (*self._data.norms.round(3), *self._data.angles.round(3))
+                )
+            ]
+        )
+        return f"{self.__class__.__name__}({atoms}, {lat})"
+
+    def __str__(self):
+        return self.content
+
+    @property
+    def path(self):
+        return self._path
+
+    def to_ase(self):
+        """Convert to ase.Atoms format. You need to have ase installed.
+        You can apply all ase methods on this object after conversion.
+
+        Example
+        -------
+        >>> from ase.visualize import view
+        >>> structure = poscar.to_ase()
+        >>> view(structure) # POSCAR.view() also uses this method if viewer is given.
+        >>> reciprocal_lattice = structure.cell.get_bravais_lattice()
+        >>> reciprocal_lattice.plt_bz() # Plot BZ usinn ase, it also plots suggested band path.
+        """
+        from ase import Atoms
+
+        symbols = [
+            lab.split()[0] for lab in self.data.labels
+        ]  # Remove numbers from labels
+        return Atoms(
+            symbols=symbols, positions=self.data.positions, cell=self.data.basis
+        )
+
+    def view(self, viewer=None, **kwargs):
+        """View POSCAR in notebook. If viewer is given it will be passed ase.visualize.view. You need to have ase installed.
+
+        kwargs are passed to self.splot_lattice if viewer is None, otherwise a  single keyword argument `data` is passed to ase viewer.
+        data should be volumetric data for ase.visualize.view, such as charge density, spin density, etc.
+        """
+        if viewer is None:
+            return plat.view_poscar(self.data, **kwargs)
         else:
-            self.__dict__[name] = value
-    # Dictionary-wise access
-    def keys(self):
-        return self.__dict__.keys()
-    
-    def values(self):
-        return self.__dict__.values()
-    
-    def __getitem__(self,key):
-        return self.__dict__[key]
-    
-    def items(self):
-        return self.__dict__.items()
-
-    
-class VasprunData(Dict2Data):
-    _req_keys = ('kpath','bands','poscar')
-    def __init__(self,d):
-        super().__init__(d)
-    
-    def __repr__(self):
-        return super().__repr__().replace("Data","VasprunData",1)
-    
-    def get_fermi(self,tol=1e-3):
-        "Fermi energy based on occupancy. Returns `self.Fermi` if occupancies cannot be resolved. `tol` is the value of occupnacy to ignore as filled."
+            from ase.visualize import view
+
+            return view(self.to_ase(), viewer=viewer, data=kwargs.get("data", None))
+
+    def view_kpath(self):
+        "Initialize a KpathWidget instance to view kpath for current POSCAR, and you can select others too."
+        from .widgets import KpathWidget
+
+        return KpathWidget(path=str(self.path.parent), glob=self.path.name)
+
+    @classmethod
+    def from_file(cls, path):
+        "Load data from POSCAR file"
+        return cls(path=path)
+
+    @classmethod
+    def from_string(cls, content):
+        "content should be a valid POSCAR string"
         try:
-            if self.sys_info.ISPIN == 1:
-                return float(self.bands.evals[self.bands.occs > 0].max())
-                
-            else: # ISPIN 2
-                energies = []
-                for attr in ['SpinUp','SpinDown']:
-                    energies.append(self.bands.evals[attr][self.bands.occs[attr] > 0].max())
-                return float(max(energies))
+            return cls(content=content)
         except:
-            return self.Fermi
-    
-    @property
-    def fermi(self):
-        "Fermi energy based on occupancy. Use .get_fermi() if you want to limit the occupancy tolerance."
-        return self.get_fermi(tol=1e-3)
-    
-    @property
-    def Fermi(self):
-        "Fermi energy given in vasprun.xml."
-        return self.bands.Fermi
-    
-class SpinData(Dict2Data):
-    _req_keys = ('kpoints','spins','poscar')
-    def __init__(self,d):
-        super().__init__(d)
-        with suppress(BaseException): # Silently set fermi if not present
-            self.sys_info.fermi = self.fermi
-    
-    def __repr__(self):
-        return super().__repr__().replace("Data","SpinData",1)
-    
-    def get_fermi(self, tol = 1e-3):
-        "Fermi energy based on occupancy. Returns `self.Fermi` if occupancies cannot be resolved. `tol` is the value of occupnacy to ignore as filled."
+            raise ValueError(f"Invalid POSCAR string!!!!!\n{content}")
+
+    @classmethod
+    def from_materials_project(cls, formula, mp_id, api_key=None, save_key=False):
+        """Downloads POSCAR from materials project. `mp_id` should be string associated with a material on their website. `api_key` is optional if not saved.
+        Get your API key from https://legacy.materialsproject.org/open and save it using `save_key` to avoid entering it everytime.
+        """
+        if cls._mp_instance and cls._mp_instance["kwargs"] == {
+            "formula": formula,
+            "mp_id": mp_id,
+        }:
+            if (
+                api_key and save_key
+            ):  # If user wants to save key even if data is loaded from cache
+                plat._save_mp_API(api_key)
+
+            return cls._mp_instance["instance"]
+
+        instance = cls(
+            data=download_structure(
+                formula=formula, mp_id=mp_id, api_key=api_key, save_key=save_key
+            )[0].export_poscar()
+        )
+        cls._mp_instance = {
+            "instance": instance,
+            "kwargs": {"formula": formula, "mp_id": mp_id},
+        }
+        return instance
+
+    @classmethod
+    def from_cif(cls, path):
+        "Load data from cif file"
+        p = Path(path)
+        if not p.is_file():
+            raise FileNotFoundError(f"File {path!r} does not exists")
+
+        with p.open("r", encoding="utf-8") as f:
+            cif_str = f.read()
+            poscar_content = plat._cif_str_to_poscar_str(
+                cif_str, "Exported from cif file using ipyvasp"
+            )
+
+        return cls.from_string(poscar_content)
+
+    @classmethod
+    def new(cls, basis, sites, scale=1, name=None):
+        """
+        Crate a new POSCAR instance from basis and sites.
+
+        Parameters
+        ----------
+        basis : array_like of shape (3, 3)
+        sites : dict, key is element and value is array_like of shape (n, 3)
+            For example, {'Mg': [[0, 0, 0]], 'Cl': [[1/3, 2/3,0.214],[2/3,1/3,0.786]]} for MgCl2.
+        scale : int or float used to scale basis and kept in metadata to use when writing to file.
+        name : str, name of the structure, if None, will be inferred from sites.
+        """
+        if np.ndim(basis) != 2 and np.shape(basis) != (3, 3):
+            raise ValueError("basis should be a 3x3 array")
+        if not isinstance(scale, (int, float, np.integer)):
+            raise ValueError("scale should be a number")
+
+        basis = np.array(basis) * scale  # scale basis, we add scale to metdata later
+
+        if not isinstance(sites, dict):
+            raise ValueError(
+                "sites should be a dictionary of elements and their positions"
+            )
+        type_dict, positions, start = {}, [], 0
+        for key, value in sites.items():
+            if not isinstance(key, str):
+                raise ValueError("sites key should be a string like 'Al'")
+            if np.ndim(value) != 2 and np.shape(value)[1] != 3:
+                raise ValueError("sites value should be an array of shape (n, 3)")
+            if np.max(value) > 1.01 or np.min(value) < -0.01:
+                raise ValueError(
+                    "sites value should be in fractional coordinates between 0 and 1"
+                )
+            type_dict[key] = range(start, start + len(value))
+            positions.extend(value)  # direct stacking of positions
+            start += len(value)
+
+        positions = np.array(positions)
+
+        out_dict = {
+            "SYSTEM": name if name else "".join(type_dict.keys()),
+            "basis": basis,
+            "metadata": {
+                "scale": scale,
+                "cartesian": False,
+                "comment": "Created using ipyvasp.lattice.POSCAR.new method",
+            },
+            "positions": positions,
+            "types": type_dict,
+        }
+        return cls(data=out_dict)
+
+    @classmethod
+    def from_clipborad(cls):
+        "Read POSCAR from clipboard (based on clipboard reader impelemented by pandas library) It picks the latest from clipboard."
         try:
-            if self.sys_info.ISPIN == 1:
-                return float(self.evals.e[self.evals.occs > tol].max())
-                
-            else: # ISPIN 2
-                energies = []
-                for a, b in [('u','SpinUp'),('d','SpinDown')]:
-                    energies.append(self.evals[a][self.evals.occs[b] > tol].max())
-                return float(max(energies))
+            instance = cls.from_string(
+                content=clipboard_get()
+            )  # read from clipboard while allowing error for bad data
+            if isinstance(instance, cls):  # if valid POSCAR string
+                cls._cb_instance = {"instance": instance}  # cache instance
+                return instance
         except:
-            return self.Fermi
-    
-    @property
-    def fermi(self):
-        "Fermi energy based on occupancy. Use .get_fermi() if you want to limit the occupancy tolerance."
-        return self.get_fermi(tol = 1e-3)
-    
-    @property
-    def Fermi(self):
-        "Fermi energy given in vasprun.xml."
-        return self.evals.Fermi
-    
-class PoscarData(Dict2Data):
-    _req_keys = ('basis','unique','extra_info')
-    def __init__(self,d):
-        super().__init__(d)
-    
-    def __repr__(self):
-        return super().__repr__().replace("Data","PoscarData",1)
-    
-    @property
-    def coords(self):
-        """Returns the lattice coordinates in cartesian space of the atoms in the poscar data.
-        """
-        from .sio import to_R3 # To avoid circular import
-        return to_R3(self.basis, self.positions)
-    
-    @property
-    def rec_basis(self):
-        "Returns the reciprocal lattice basis of the atoms in the poscar data. Gets automatically updated when the lattice is changed."
-        return np.linalg.inv(self.basis).T
-    
-    @property
-    def norms(self):
-        "Returns the norm of the lattice basis of the atoms in the poscar data. Gets automatically updated when the lattice is changed."
-        return np.linalg.norm(self.basis,axis=1)
-    
-    @property
-    def rec_norms(self):
-        "Returns the norm of the reciprocal lattice basis of the atoms in the poscar data. Gets automatically updated when the lattice is changed."
-        return np.linalg.norm(self.rec_basis,axis=1)
-    
-    @property
-    def angles(self):
-        "Returns the angles of the lattice basis of the atoms in the poscar data. Gets automatically updated when the lattice is changed."
-        norms = self.norms # Calculate once
-        rad_angles = np.array([
-            np.abs(np.arccos(np.dot(self.basis[:,2],self.basis[:,1])/norms[2]/norms[1])),
-            np.abs(np.arccos(np.dot(self.basis[:,2],self.basis[:,0])/norms[2]/norms[0])),
-            np.abs(np.arccos(np.dot(self.basis[:,1],self.basis[:,0])/norms[1]/norms[0]))
-        ])
-        return np.degrees(rad_angles)
-        
-    @property
-    def rec_angles(self):
-        "Returns the angles of reciprocal lattice basis of the atoms in the poscar data. Gets automatically updated when the lattice is changed."
-        rec_norms = self.rec_norms # Calculate once
-        rec_basis = self.rec_basis # Calculate once
-        rad_angles = np.array([
-            np.abs(np.arccos(np.dot(rec_basis[:,2],rec_basis[:,1])/rec_norms[2]/rec_norms[1])),
-            np.abs(np.arccos(np.dot(rec_basis[:,2],rec_basis[:,0])/rec_norms[2]/rec_norms[0])),
-            np.abs(np.arccos(np.dot(rec_basis[:,1],rec_basis[:,0])/rec_norms[1]/rec_norms[0]))
-        ])
-        return np.degrees(rad_angles)
-    
-    @property
-    def volume(self):
-        "Returns the volume of the lattice."
-        return np.abs(np.linalg.det(self.basis)) # Didn't think much if negative or positive
-    
-    @property
-    def rec_volume(self):
-        "Returns the volume of the reciprocal lattice."
-        return np.abs(np.linalg.det(self.rec_basis))
-    
-    @property
-    def labels(self):
-        "Returns the labels of the atoms in the poscar data."
-        return np.array([f'{k} {v - vs.start + 1}' for k,vs in self.unique.items() for v in vs])
-    
-    def get_bond_length(self,atom1,atom2):
-        "Returns the bond length between two atoms names should be as 'Ga', 'As'"
-        all_dist =[]
-        for idx in self.unique[atom1]:
-            others = self.unique[atom2]
-            all_dist = [*all_dist,*np.linalg.norm(self.coords[others] - self.coords[idx,:], axis = 1)] # Get the second closest distance, first is itself
-        
-        all_dist = np.array(all_dist)
-        all_dist = all_dist[all_dist > 0] # Remove 0 distances
-        return np.min(all_dist)
-    
-    def write(self, outfile = None, overwrite = False):
-        "Writes the poscar data to a file."
-        from .sio import write_poscar # To avoid circular import
-        return write_poscar(self,outfile = outfile,overwrite = overwrite)
-        
-
-class GridData(Dict2Data):
-    _req_keys = ('path','poscar','SYSTEM')
-    def __init__(self,d):
-        super().__init__(d)
-    
-    def __repr__(self):
-        return super().__repr__().replace("Data","GridData",1)
-    
-    @property
-    def coords(self):
-        "Returns coordinates of the grid points in shape (3,Nx, Ny,Nz). (x,y,z) = i/Nx*a + j/Ny*b + k/Nz*c, where (a,b,c) is the lattice vector. and i,j,k are the grid indices. as 0-Nx-1, 0-Ny-1, 0-Nz-1."
-        shape = self.values.shape
-        Nx, Ny, Nz = shape
-        ix,iy,iz = np.indices(shape)
-        a1,a2,a3 = self.poscar.basis
-        return np.array([
-            ix*a1[0]/Nx + iy*a2[0]/Ny + iz*a3[0]/Nz,
-            ix*a1[1]/Nx + iy*a2[1]/Ny + iz*a3[1]/Nz,
-            ix*a1[2]/Nx + iy*a2[2]/Ny + iz*a3[2]/Nz
-        ])
-            
-
-class OutcarData(Dict2Data):
-    _req_keys = ('site_pot','ion_pot','basis')
-    def __init__(self,d):
-        super().__init__(d)
-    
-    def __repr__(self):
-        return super().__repr__().replace("Data","OutcarData",1)
+            if cls._cb_instance:
+                print(
+                    "Loading from previously cached clipboard data, as current data is not valid POSCAR string."
+                )
+                return cls._cb_instance["instance"]
+            else:
+                raise ValueError(
+                    "Clipboard does not contain valid POSCAR string and no previous data is cached."
+                )
+
+    def to_clipboard(self):
+        "Writes POSCAR to clipboard (as implemented by pandas library) for copy in other programs such as vim."
+        clipboard_set(self.content)  # write to clipboard
 
+    @property
+    def data(self):
+        "Data object in POSCAR."
+        return self._data
 
-class EncodeFromNumpy(json.JSONEncoder):
-    """
-    - Serializes python/Numpy objects via customizing json encoder.
-    - **Usage**
-        - `json.dumps(python_dict, cls=EncodeFromNumpy)` to get json string.
-        - `json.dump(*args, cls=EncodeFromNumpy)` to create a file.json.
-    """
-    def default(self, obj):
-        if isinstance(obj, np.ndarray):
-            return {
-                "_kind_": "ndarray",
-                "_value_": obj.tolist()
-            }
-        if isinstance(obj, np.integer):
-            return int(obj)
-        elif isinstance(obj, np.floating):
-            return float(obj)
-        elif isinstance(obj,range):
-            value = list(obj)
-            return {
-                "_kind_" : "range",
-                "_value_" : [value[0],value[-1]+1]
-            }
-        return super(EncodeFromNumpy, self).default(obj)
+    def copy(self):
+        "Copy POSCAR object. It avoids accidental changes to numpy arrays in original object."
+        return self.__class__(data=self._data.copy())
 
+    @property
+    def content(self):
+        "POSCAR content."
+        with redirect_stdout(StringIO()) as f:
+            self.write(outfile=None)  # print to stdout
+            return f.getvalue()
+
+    @property
+    def bz(self):
+        return self._bz
+
+    @property
+    def cell(self):
+        return self._cell
+
+    @_sub_doc(stk.get_bz, {"basis :.*loop :": "loop :"})
+    @_sig_kwargs(stk.get_bz, ("basis",))
+    def get_bz(self, **kwargs):
+        self._bz = stk.get_bz(self._data.rec_basis, **kwargs)
+        return self._bz
+
+    def get_cell(self, loop=True):
+        "See docs of `get_bz`, same except space is inverted and no factor of 2pi."
+        self._cell = serializer.CellData(
+            stk.get_bz(  # data.basis makes prmitive cell in direct space
+                basis=self.data.basis, loop=loop, primitive=True
+            ).to_dict()
+        )  # cell must be primitive
+        return self._cell
+
+    @_sub_doc(plat.splot_bz, {"bz_data :.*plane :": "plane :"})
+    @_sig_kwargs(plat.splot_bz, ("bz_data",))
+    def splot_bz(self, plane=None, **kwargs):
+        self._plane = plane  # Set plane for splot_kpath
+        new_ax = plat.splot_bz(bz_data=self._bz, plane=plane, **kwargs)
+        self._ax = new_ax  # Set ax for splot_kpath
+        self._zoffset = kwargs.get("zoffset", 0)  # Set zoffset for splot_kpath
+        return new_ax
+
+    def splot_kpath(
+        self, kpoints, labels=None, fmt_label=lambda x: (x, {"color": "blue"}), **kwargs
+    ):
+        """Plot k-path over existing BZ.
+
+        Parameters
+        ----------
+        kpoints : array_like
+            List of k-points in fractional coordinates. e.g. [(0,0,0),(0.5,0.5,0.5),(1,1,1)] in order of path.
+        labels : list
+            List of labels for each k-point in same order as kpoints.
+        fmt_label : callable
+            Function that takes a label from labels and should return a string or (str, dict) of which dict is passed to ``plt.text``.
 
 
-class DecodeToNumpy(json.JSONDecoder):
-    """
-    - Deserilizes JSON object to Python/Numpy's objects.
-    - **Usage**
-        - `json.loads(json_string,cls=DecodeToNumpy)` from string, use `json.load()` for file.
-    """
-    def __init__(self, *args, **kwargs):
-        json.JSONDecoder.__init__(self, object_hook=self.object_hook, *args, **kwargs)
+        kwargs are passed to ``plt.plot`` with some defaults.
 
-    def object_hook(self, obj):
-        if '_kind_' not in obj:
-            return obj
-        kind = obj['_kind_']
-        if kind == 'ndarray':
-            return np.array(obj['_value_'])
-        elif kind == 'range':
-            value = obj['_value_']
-            return range(value[0],value[-1])
-        return obj
+        You can get ``kpoints = POSCAR.get_bz().specials.masked(lambda x,y,z : (-0.1 < z 0.1) & (x >= 0) & (y >= 0))`` to get k-points in positive xy plane.
+        Then you can reorder them by an indexer like ``kpoints = kpoints[[0,1,2,0,7,6]]``, note double brackets, and also that point at zero index is taken twice.
 
-    
-def dump(dict_data = None, dump_to = 'pickle',outfile = None,indent=1):
-    """
-    - Dump an `export_vasprun` or `load_export`'s `Data` object or any dictionary to json or pickle string/file. It convert `Dict2Data` to dictionary before serializing to json/pickle, so json/pickle.loads() of converted Data would be a simple dictionary, pass that to `Dict2Data` to again make accessible via dot notation.
-    - **Parameters**
-        - dict_data: Any dictionary/Dict2Data(or subclass Data) object containg numpy arrays, including `export_vasprun` or `load_export` output.
-        - dump_to  : Defualt is `pickle` or `json`.
-        - outfile  : Defualt is None and return string. File name does not require extension.
-        - indent   : Defualt is 1. Only works for json.
-    """
-    if dump_to not in ['pickle','json']:
-        raise ValueError("`dump_to` expects 'pickle' or 'json', got '{}'".format(dump_to))
-    try: 
-        dict_obj = dict_data.to_dict() # Change Data object to dictionary
-        dict_obj = {'_loader_':dict_data.__class__.__name__,'_data_':dict_obj} # Add class name to dictionary for reconstruction
-    except: 
-        dict_obj = dict_data
-    if dump_to == 'pickle':
-        if outfile == None:
-            return pickle.dumps(dict_obj)
-        outfile = os.path.splitext(outfile)[0] + '.pickle'
-        with open(outfile,'wb') as f:
-            pickle.dump(dict_obj,f)
-    if dump_to == 'json':
-        if outfile == None:
-            return json.dumps(dict_obj,cls = EncodeFromNumpy,indent=indent)
-        outfile = os.path.splitext(outfile)[0] + '.json'
-        with open(outfile,'w') as f:
-            json.dump(dict_obj,f,cls = EncodeFromNumpy,indent=indent)
-    return None
+        .. tip::
+            You can use this function multiple times to plot multiple/broken paths over same BZ.
+        """
+        if not self._bz or not self._ax:
+            raise ValueError("BZ not found, use `splot_bz` first")
 
+        if not np.ndim(kpoints) == 2 and np.shape(kpoints)[-1] == 3:
+            raise ValueError("kpoints must be 2D array of shape (N,3)")
 
-def load(file_or_str):
-    """
-    - Loads a json/pickle dumped file or string by auto detecting it.
-    - **Parameters**
-        - file_or_str : Filename of pickl/json or their string. 
-    """
-    out = {}
-    if not isinstance(file_or_str,bytes):
-        try: #must try, else fails due to path length issue
-            if os.path.isfile(file_or_str):
-                if '.pickle' in file_or_str:
-                    with open(file_or_str,'rb') as f:
-                        out = pickle.load(f)
-
-                elif '.json' in file_or_str:
-                    with open(file_or_str,'r') as f:
-                        out = json.load(f,cls = DecodeToNumpy)
-
-            else: out = json.loads(file_or_str,cls = DecodeToNumpy)
-            # json.loads required in else and except both as long str > 260 causes issue in start of try block
-        except: out = json.loads(file_or_str,cls = DecodeToNumpy)
-    elif isinstance(file_or_str,bytes):
-            out = pickle.loads(file_or_str)
-    
-
-    if type(out) is dict:
-        if '_loader_' in out:
-            return globals()[out['_loader_']](out['_data_'])
-    else:
-        if hasattr(out, '_loader_'):
-            return globals()[out._loader_](out._data_)
-        
-    return out # Retruns usual dictionaries
+        ijk = [0, 1, 2]
+        _mapping = {
+            "xy": [0, 1],
+            "xz": [0, 2],
+            "yz": [1, 2],
+            "zx": [2, 0],
+            "zy": [2, 1],
+            "yx": [1, 0],
+        }
+        _zoffset = [0, 0, 0]
+        if self._plane:
+            _zoffset = (
+                [0, 0, self._zoffset]
+                if self._plane in "xyx"
+                else [0, self._zoffset, 0]
+                if self._plane in "xzx"
+                else [self._zoffset, 0, 0]
+            )
+
+        if isinstance(self._plane, str) and self._plane in _mapping:
+            if getattr(self._ax, "name", None) != "3d":
+                ijk = _mapping[
+                    self._plane
+                ]  # only change indices if axes is not 3d, even if plane is given
+
+        if not labels:
+            labels = [
+                "[{0:5.2f}, {1:5.2f}, {2:5.2f}]".format(x, y, z) for x, y, z in kpoints
+            ]
+
+        plat._validate_label_func(fmt_label, labels[0])
+
+        coords = self.to_R3(kpoints, reciprocal=True)
+        if _zoffset and self._plane:
+            normal = (
+                [0, 0, 1]
+                if self._plane in "xyx"
+                else [0, 1, 0]
+                if self._plane in "xzx"
+                else [1, 0, 0]
+            )
+            coords = plat.to_plane(normal, coords) + _zoffset
+
+        coords = coords[:, ijk]  # select only required indices
+        kwargs = {
+            **dict(color="blue", linewidth=0.8, marker=".", markersize=10),
+            **kwargs,
+        }  # need some defaults
+        self._ax.plot(*coords.T, **kwargs)
+
+        for c, text in zip(coords, labels):
+            lab, textkws = fmt_label(text), {}
+            if isinstance(lab, (list, tuple)):
+                lab, textkws = lab
+            self._ax.text(*c, lab, **textkws)
+
+        return self._ax
+
+    @_sig_kwargs(plat.splot_bz, ("bz_data",))
+    def splot_cell(self, plane=None, **kwargs):
+        "See docs of `splot_bz`, everything is same except space is inverted."
+        return plat.splot_bz(bz_data=self._cell, plane=plane, **kwargs)
+
+    @_sub_doc(plat.iplot_bz, {"bz_data :.*fill :": "fill :"})
+    @_sig_kwargs(plat.iplot_bz, ("bz_data",))
+    def iplot_bz(self, **kwargs):
+        return plat.iplot_bz(bz_data=self._bz, **kwargs)
+
+    @_sig_kwargs(plat.iplot_bz, ("bz_data", "special_kpoints"))
+    def iplot_cell(self, **kwargs):
+        "See docs of `iplot_bz`, everything is same except space is iverted."
+        return plat.iplot_bz(bz_data=self._cell, special_kpoints=False, **kwargs)
+
+    @_sub_doc(plat.splot_lattice)
+    @_sig_kwargs(plat.splot_lattice, ("poscar_data", "plane"))
+    def splot_lattice(self, plane=None, **kwargs):
+        return plat.splot_lattice(self._data, plane=plane, **kwargs)
+
+    @_sub_doc(plat.iplot_lattice)
+    @_sig_kwargs(plat.iplot_lattice, ("poscar_data",))
+    def iplot_lattice(self, **kwargs):
+        return plat.iplot_lattice(self._data, **kwargs)
+
+    @_sub_doc(plat.write_poscar)
+    @_sig_kwargs(plat.write_poscar, ("poscar_data",))
+    def write(self, outfile=None, **kwargs):
+        return plat.write_poscar(self._data, outfile=outfile, **kwargs)
+
+    @_sub_doc(plat.join_poscars)
+    @_sig_kwargs(plat.join_poscars, ("poscar_data", "other"))
+    def join(self, other, direction="c", **kwargs):
+        return self.__class__(
+            data=plat.join_poscars(
+                poscar_data=self._data, other=other.data, direction=direction, **kwargs
+            )
+        )
+
+    @_sub_doc(plat.scale_poscar)
+    @_sig_kwargs(plat.scale_poscar, ("poscar_data",))
+    def scale(self, scale=(1, 1, 1), **kwargs):
+        return self.__class__(data=plat.scale_poscar(self._data, scale, **kwargs))
+
+    @_sub_doc(plat.rotate_poscar)
+    def rotate(self, angle_deg, axis_vec):
+        return self.__class__(
+            data=plat.rotate_poscar(self._data, angle_deg=angle_deg, axis_vec=axis_vec)
+        )
+
+    @_sub_doc(plat.set_zdir)
+    def set_zdir(self, hkl, phi=0):
+        return self.__class__(data=plat.set_zdir(self._data, hkl, phi=phi))
+
+    @_sub_doc(plat.translate_poscar)
+    def translate(self, offset):
+        return self.__class__(data=plat.translate_poscar(self._data, offset=offset))
+
+    @_sub_doc(plat.repeat_poscar)
+    def repeat(self, n, direction):
+        return self.__class__(
+            data=plat.repeat_poscar(self._data, n=n, direction=direction)
+        )
+
+    @_sub_doc(plat.mirror_poscar)
+    def mirror(self, direction):
+        return self.__class__(data=plat.mirror_poscar(self._data, direction=direction))
+
+    @_sub_doc(stk.get_TM, replace={"basis1": "self.basis"})
+    def get_TM(self, target_basis):
+        return stk.get_TM(self._data.basis, target_basis)
+
+    @_sub_doc(plat.transform_poscar)
+    def transform(self, transformation, zoom=2, tol=1e-2):
+        return self.__class__(
+            data=plat.transform_poscar(self._data, transformation, zoom=zoom, tol=tol)
+        )
+
+    @_sub_doc(plat.transpose_poscar)
+    def transpose(self, axes=[1, 0, 2]):
+        return self.__class__(data=plat.transpose_poscar(self._data, axes=axes))
+
+    @_sub_doc(plat.add_vaccum)
+    def add_vaccum(self, thickness, direction, left=False):
+        return self.__class__(
+            data=plat.add_vaccum(
+                self._data, thickness=thickness, direction=direction, left=left
+            )
+        )
+
+    @_sub_doc(plat.add_atoms)
+    def add_atoms(self, name, positions):
+        return self.__class__(
+            data=plat.add_atoms(self._data, name=name, positions=positions)
+        )
+
+    @_sub_doc(plat.convert_poscar)
+    def convert(self, atoms_mapping, basis_factor):
+        return self.__class__(
+            data=plat.convert_poscar(
+                self._data, atoms_mapping=atoms_mapping, basis_factor=basis_factor
+            )
+        )
+
+    @_sub_doc(plat.strain_poscar)
+    def strain(self, strain_matrix):
+        return self.__class__(
+            data=plat.strain_poscar(self._data, strain_matrix=strain_matrix)
+        )
+
+    @_sub_doc(get_kmesh, {"poscar_data :.*\*args :": "*args :"})
+    @_sig_kwargs(get_kmesh, ("poscar_data",))
+    def get_kmesh(self, *args, **kwargs):
+        return get_kmesh(self.data, *args, **kwargs)
+
+    @_sub_doc(get_kpath, {"rec_basis :.*\n\n": "\n\n"})
+    @_sig_kwargs(get_kpath, ("rec_basis",))
+    def get_kpath(self, kpoints, n=5, **kwargs):
+        return get_kpath(kpoints, n=n, **kwargs, rec_basis=self.data.rec_basis)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipyvasp-0.1.0/ipyvasp/sio.py` & `ipyvasp-0.2.0/ipyvasp/_lattice.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1810 +1,2323 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: StructureIO.ipynb (unless otherwise specified).
-
-__all__ = ['atomic_number', 'atoms_color', 'periodic_table', 'Arrow3D', 'fancy_quiver3d', 'get_selective_dynamics',
-           'write_poscar', 'export_poscar', 'InvokeMaterialsProject', 'get_kpath', 'read_ticks', 'str2kpath',
-           'get_kmesh', 'order', 'rotation', 'get_bz', 'splot_bz', 'iplot_bz', 'to_R3', 'to_basis', 'kpoints2bz',
-           'fix_sites', 'translate_poscar', 'get_pairs', 'iplot_lat', 'splot_lat', 'join_poscars', 'repeat_poscar',
-           'scale_poscar', 'rotate_poscar', 'mirror_poscar', 'convert_poscar', 'get_transform_matrix',
-           'transform_poscar', 'add_vaccum', 'transpose_poscar', 'add_atoms']
-
-# Cell
-import sys, os, re
+import re
 import json
 import numpy as np
 from pathlib import Path
 import requests as req
-from collections import namedtuple
-from itertools import product
+import inspect
+from itertools import combinations
 from functools import lru_cache
 
-from scipy.spatial import ConvexHull, Voronoi, KDTree
+from scipy.spatial import ConvexHull, KDTree
 import plotly.graph_objects as go
-import matplotlib.pyplot as plt
-import matplotlib.colors as mplc #For viewpoint
-from mpl_toolkits import mplot3d
+
+import matplotlib.pyplot as plt  # For viewpoint
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
-# Inside packages import to work both with package and jupyter notebook.
-try:
-    from ipyvasp import parser as vp, serializer
-    from ipyvasp import splots as sp
-    from ipyvasp import utils
-except:
-    import ipyvasp.parser as vp
-    import ipyvasp.splots as sp
-    import ipyvasp.serializer as serializer
-    import ipyvasp.utils as utils
+
+from ipywidgets import interactive
+
+# Inside packages import
+from .core import plot_toolkit as ptk
+from .core import parser as vp, serializer
+from .core.spatial_toolkit import (
+    to_plane,
+    rotation,
+    inside_convexhull,
+    to_basis,
+    to_R3,
+    get_TM,
+    get_bz,
+)
+from .core.plot_toolkit import quiver3d
 
 
 # These colors are taken from Mathematica's ColorData["Atoms"]
-_atom_colors = {'H': (0.7, 0.8, 0.7), 'He': (0.8367, 1.0, 1.0),
-    'Li': (0.7994, 0.9976, 0.5436), 'Be': (0.7706, 0.0442, 0.9643), 'B': (1.0, 0.5, 0), 'C': (0.4, 0.4, 0.4), 'N': (143/255,143/255,1), 'O': (0.8005, 0.1921, 0.2015), 'F': (128/255, 1, 0), 'Ne': (0.6773, 0.9553, 0.9284),
-    'Na': (0.6587, 0.8428, 0.4922),'Mg': (0.6283, 0.0783, 0.8506),'Al': (173/255, 178/255, 189/255),'Si': (248/255, 209/255, 152/255),'P': (1,165/255,0),'S': (1,200/255,50/255),'Cl': (0,0.9,0),'Ar': (0.5461, 0.8921, 0.8442),
-    'K':  (0.534, 0.7056, 0.4207), 'Ca': (0.4801, 0.0955, 0.7446), 'Sc': (0.902, 0.902, 0.902), 'Ti': (0.749, 0.7804, 0.7608), 'V': (0.651, 0.6706, 0.651), 'Cr': (0.5412, 0.7804, 0.6), 'Mn': (0.6118, 0.7804, 0.4784), 'Fe': (0.32,0.33,0.35),
-    'Co': (0.9412, 0.6275, 0.5647), 'Ni': (141/255, 142/255, 140/255), 'Cu': (184/255, 115/255, 51/255), 'Zn': (186/255, 196/255, 200/255),'Ga': (90/255, 180/255, 189/255),'Ge': (0.6051, 0.5765, 0.6325),'As': (50/255,71/255,57/255),'Se': (0.9172, 0.0707, 0.6578),
-    'Br': (161/255, 61/255, 45/255),'Kr': (0.426, 0.8104, 0.7475),'Rb': (0.4254, 0.5859, 0.3292),'Sr': (0.326, 0.096, 0.6464),'Y': (0.531, 1.0, 1.0),'Zr': (0.4586, 0.9186, 0.9175),'Nb': (0.385, 0.8417, 0.8349),'Mo': (0.3103, 0.7693, 0.7522),
-    'Tc': (0.2345, 0.7015, 0.6694), 'Ru': (0.1575, 0.6382, 0.5865), 'Rh': (0.0793, 0.5795, 0.5036), 'Pd': (0.0, 0.5252, 0.4206), 'Ag': (0.7529, 0.7529, 0.7529), 'Cd': (0.8,0.67,0.73), 'In': (228/255, 228/255, 228/255), 'Sn': (0.398, 0.4956, 0.4915),
-    'Sb': (158/255,99/255,181/255), 'Te': (0.8167, 0.0101, 0.4513), 'I': (48/255, 25/255, 52/255), 'Xe': (0.3169, 0.7103, 0.6381), 'Cs': (0.3328, 0.4837, 0.2177), 'Ba': (0.1659, 0.0797, 0.556), 'La': (0.9281, 0.3294, 0.7161), 'Ce': (0.8948, 0.3251, 0.7314),
-    'Pr': (0.8652, 0.3153, 0.708), 'Nd': (0.8378, 0.3016, 0.663), 'Pm': (0.812, 0.2856, 0.6079), 'Sm': (0.7876, 0.2683, 0.5499), 'Eu': (0.7646, 0.2504, 0.4933), 'Gd': (0.7432, 0.2327, 0.4401), 'Tb': (0.7228, 0.2158, 0.3914), 'Dy': (0.7024, 0.2004, 0.3477),
-    'Ho': (0.68, 0.1874, 0.3092), 'Er': (0.652, 0.1778, 0.2768), 'Tm': (0.6136, 0.173, 0.2515), 'Yb': (0.5579, 0.1749, 0.2346), 'Lu': (0.4757, 0.1856, 0.2276), 'Hf': (0.7815, 0.7166, 0.7174), 'Ta': (0.7344, 0.6835, 0.5445), 'W': (0.6812, 0.6368, 0.3604),
-    'Re': (0.6052, 0.5563, 0.3676), 'Os': (0.5218, 0.4692, 0.3821), 'Ir': (0.4456, 0.3991, 0.3732), 'Pt': (0.8157, 0.8784, 0.8157), 'Au': (0.8, 0.7, 0.2), 'Hg': (0.7216, 0.8157, 0.7216), 'Tl': (0.651, 0.302, 0.3294), 'Pb': (0.3412, 0.3804, 0.349),
-    'Bi': (10/255, 49/255, 93/255), 'Po': (0.6706, 0.0, 0.3608), 'At': (0.4588, 0.2706, 0.3098), 'Rn': (0.2188, 0.5916, 0.5161), 'Fr': (0.2563, 0.3989, 0.0861), 'Ra': (0.0, 0.0465, 0.4735), 'Ac': (0.322, 0.9885, 0.7169), 'Th': (0.3608, 0.943, 0.6717),
-    'Pa': (0.3975, 0.8989, 0.628), 'U': (0.432, 0.856, 0.586), 'Np': (0.4645, 0.8145, 0.5455), 'Pu': (0.4949, 0.7744, 0.5067), 'Am': (0.5233, 0.7355, 0.4695), 'Cm': (0.5495, 0.698, 0.4338), 'Bk': (0.5736, 0.6618, 0.3998), 'Cf': (0.5957, 0.6269, 0.3675),
-    'Es': (0.6156, 0.5934, 0.3367), 'Fm': (0.6335, 0.5612, 0.3075), 'Md': (0.6493, 0.5303, 0.2799), 'No': (0.663, 0.5007, 0.254), 'Lr': (0.6746, 0.4725, 0.2296), 'Rf': (0.6841, 0.4456, 0.2069), 'Db': (0.6915, 0.42, 0.1858), 'Sg': (0.6969, 0.3958, 0.1663),
-    'Bh': (0.7001, 0.3728, 0.1484), 'Hs': (0.7013, 0.3512, 0.1321), 'Mt': (0.7004, 0.331, 0.1174), 'Ds': (0.6973, 0.312, 0.1043), 'Rg': (0.6922, 0.2944, 0.0928), 'Cn': (0.6851, 0.2781, 0.083), 'Nh': (0.6758, 0.2631, 0.0747), 'Fl': (0.6644, 0.2495, 0.0681),
-    'Mc': (0.6509, 0.2372, 0.0631), 'Lv': (0.6354, 0.2262, 0.0597), 'Ts': (0.6354, 0.2262, 0.0566), 'Og': (0.6354, 0.2262, 0.0528)}
+_atom_colors = {
+    "H": (0.7, 0.8, 0.7),
+    "He": (0.8367, 1.0, 1.0),
+    "Li": (0.7994, 0.9976, 0.5436),
+    "Be": (0.7706, 0.0442, 0.9643),
+    "B": (1.0, 0.5, 0),
+    "C": (0.4, 0.4, 0.4),
+    "N": (143 / 255, 143 / 255, 1),
+    "O": (0.8005, 0.1921, 0.2015),
+    "F": (128 / 255, 1, 0),
+    "Ne": (0.6773, 0.9553, 0.9284),
+    "Na": (0.6587, 0.8428, 0.4922),
+    "Mg": (0.6283, 0.0783, 0.8506),
+    "Al": (173 / 255, 178 / 255, 189 / 255),
+    "Si": (248 / 255, 209 / 255, 152 / 255),
+    "P": (1, 165 / 255, 0),
+    "S": (1, 200 / 255, 50 / 255),
+    "Cl": (0, 0.9, 0),
+    "Ar": (0.5461, 0.8921, 0.8442),
+    "K": (0.534, 0.7056, 0.4207),
+    "Ca": (0.4801, 0.0955, 0.7446),
+    "Sc": (0.902, 0.902, 0.902),
+    "Ti": (0.749, 0.7804, 0.7608),
+    "V": (0.651, 0.6706, 0.651),
+    "Cr": (0.5412, 0.7804, 0.6),
+    "Mn": (0.6118, 0.7804, 0.4784),
+    "Fe": (0.32, 0.33, 0.35),
+    "Co": (0.9412, 0.6275, 0.5647),
+    "Ni": (141 / 255, 142 / 255, 140 / 255),
+    "Cu": (184 / 255, 115 / 255, 51 / 255),
+    "Zn": (186 / 255, 196 / 255, 200 / 255),
+    "Ga": (90 / 255, 180 / 255, 189 / 255),
+    "Ge": (0.6051, 0.5765, 0.6325),
+    "As": (50 / 255, 71 / 255, 57 / 255),
+    "Se": (0.9172, 0.0707, 0.6578),
+    "Br": (161 / 255, 61 / 255, 45 / 255),
+    "Kr": (0.426, 0.8104, 0.7475),
+    "Rb": (0.4254, 0.5859, 0.3292),
+    "Sr": (0.326, 0.096, 0.6464),
+    "Y": (0.531, 1.0, 1.0),
+    "Zr": (0.4586, 0.9186, 0.9175),
+    "Nb": (0.385, 0.8417, 0.8349),
+    "Mo": (0.3103, 0.7693, 0.7522),
+    "Tc": (0.2345, 0.7015, 0.6694),
+    "Ru": (0.1575, 0.6382, 0.5865),
+    "Rh": (0.0793, 0.5795, 0.5036),
+    "Pd": (0.0, 0.5252, 0.4206),
+    "Ag": (0.7529, 0.7529, 0.7529),
+    "Cd": (0.8, 0.67, 0.73),
+    "In": (228 / 255, 228 / 255, 228 / 255),
+    "Sn": (0.398, 0.4956, 0.4915),
+    "Sb": (158 / 255, 99 / 255, 181 / 255),
+    "Te": (0.8167, 0.0101, 0.4513),
+    "I": (48 / 255, 25 / 255, 52 / 255),
+    "Xe": (0.3169, 0.7103, 0.6381),
+    "Cs": (0.3328, 0.4837, 0.2177),
+    "Ba": (0.1659, 0.0797, 0.556),
+    "La": (0.9281, 0.3294, 0.7161),
+    "Ce": (0.8948, 0.3251, 0.7314),
+    "Pr": (0.8652, 0.3153, 0.708),
+    "Nd": (0.8378, 0.3016, 0.663),
+    "Pm": (0.812, 0.2856, 0.6079),
+    "Sm": (0.7876, 0.2683, 0.5499),
+    "Eu": (0.7646, 0.2504, 0.4933),
+    "Gd": (0.7432, 0.2327, 0.4401),
+    "Tb": (0.7228, 0.2158, 0.3914),
+    "Dy": (0.7024, 0.2004, 0.3477),
+    "Ho": (0.68, 0.1874, 0.3092),
+    "Er": (0.652, 0.1778, 0.2768),
+    "Tm": (0.6136, 0.173, 0.2515),
+    "Yb": (0.5579, 0.1749, 0.2346),
+    "Lu": (0.4757, 0.1856, 0.2276),
+    "Hf": (0.7815, 0.7166, 0.7174),
+    "Ta": (0.7344, 0.6835, 0.5445),
+    "W": (0.6812, 0.6368, 0.3604),
+    "Re": (0.6052, 0.5563, 0.3676),
+    "Os": (0.5218, 0.4692, 0.3821),
+    "Ir": (0.4456, 0.3991, 0.3732),
+    "Pt": (0.8157, 0.8784, 0.8157),
+    "Au": (0.8, 0.7, 0.2),
+    "Hg": (0.7216, 0.8157, 0.7216),
+    "Tl": (0.651, 0.302, 0.3294),
+    "Pb": (0.3412, 0.3804, 0.349),
+    "Bi": (10 / 255, 49 / 255, 93 / 255),
+    "Po": (0.6706, 0.0, 0.3608),
+    "At": (0.4588, 0.2706, 0.3098),
+    "Rn": (0.2188, 0.5916, 0.5161),
+    "Fr": (0.2563, 0.3989, 0.0861),
+    "Ra": (0.0, 0.0465, 0.4735),
+    "Ac": (0.322, 0.9885, 0.7169),
+    "Th": (0.3608, 0.943, 0.6717),
+    "Pa": (0.3975, 0.8989, 0.628),
+    "U": (0.432, 0.856, 0.586),
+    "Np": (0.4645, 0.8145, 0.5455),
+    "Pu": (0.4949, 0.7744, 0.5067),
+    "Am": (0.5233, 0.7355, 0.4695),
+    "Cm": (0.5495, 0.698, 0.4338),
+    "Bk": (0.5736, 0.6618, 0.3998),
+    "Cf": (0.5957, 0.6269, 0.3675),
+    "Es": (0.6156, 0.5934, 0.3367),
+    "Fm": (0.6335, 0.5612, 0.3075),
+    "Md": (0.6493, 0.5303, 0.2799),
+    "No": (0.663, 0.5007, 0.254),
+    "Lr": (0.6746, 0.4725, 0.2296),
+    "Rf": (0.6841, 0.4456, 0.2069),
+    "Db": (0.6915, 0.42, 0.1858),
+    "Sg": (0.6969, 0.3958, 0.1663),
+    "Bh": (0.7001, 0.3728, 0.1484),
+    "Hs": (0.7013, 0.3512, 0.1321),
+    "Mt": (0.7004, 0.331, 0.1174),
+    "Ds": (0.6973, 0.312, 0.1043),
+    "Rg": (0.6922, 0.2944, 0.0928),
+    "Cn": (0.6851, 0.2781, 0.083),
+    "Nh": (0.6758, 0.2631, 0.0747),
+    "Fl": (0.6644, 0.2495, 0.0681),
+    "Mc": (0.6509, 0.2372, 0.0631),
+    "Lv": (0.6354, 0.2262, 0.0597),
+    "Ts": (0.6354, 0.2262, 0.0566),
+    "Og": (0.6354, 0.2262, 0.0528),
+}
+
+_atom_numbers = {k: i for i, k in enumerate(_atom_colors.keys())}
 
-_atom_numbers = {k:i for i,k in enumerate(_atom_colors.keys())}
 
 def atomic_number(atom):
     "Return atomic number of atom"
     return _atom_numbers[atom]
 
+
 def atoms_color():
     "Defualt color per atom used for plotting the crystal lattice"
-    return serializer.Dict2Data({k:[round(_v,4) for _v in rgb] for k,rgb in _atom_colors.items()})
+    return serializer.Dict2Data(
+        {k: [round(_v, 4) for _v in rgb] for k, rgb in _atom_colors.items()}
+    )
+
 
 def periodic_table():
     "Display colorerd elements in periodic table."
-    _copy_names = np.array([f'$^{{{str(i+1)}}}${k}' for i,k in enumerate(_atom_colors.keys())])
+    _copy_names = np.array(
+        [f"$^{{{str(i+1)}}}${k}" for i, k in enumerate(_atom_colors.keys())]
+    )
     _copy_array = np.array(list(_atom_colors.values()))
 
-    array = np.ones((180,3))
-    names = ['' for i in range(180)] # keep as list before modification
+    array = np.ones((180, 3))
+    names = ["" for i in range(180)]  # keep as list before modification
 
-    inds = [(0,0),(17,1),
-            (18,2),(19,3),*[(30+i,4+i) for i in range(8)],
-            *[(48+i,12+i) for i in range(6)],
-            *[(54+i,18+i) for i in range(18)],
-            *[(72+i,36+i) for i in range(18)],
-            *[(90+i,54+i) for i in range(3)],*[(93+i,71+i) for i in range(15)],
-            *[(108+i,86+i) for i in range(3)],*[(111+i,103+i) for i in range(15)],
-            *[(147+i,57+i) for i in range(14)],
-            *[(165+i,89+i) for i in range(14)]
-            ]
+    inds = [
+        (0, 0),
+        (17, 1),
+        (18, 2),
+        (19, 3),
+        *[(30 + i, 4 + i) for i in range(8)],
+        *[(48 + i, 12 + i) for i in range(6)],
+        *[(54 + i, 18 + i) for i in range(18)],
+        *[(72 + i, 36 + i) for i in range(18)],
+        *[(90 + i, 54 + i) for i in range(3)],
+        *[(93 + i, 71 + i) for i in range(15)],
+        *[(108 + i, 86 + i) for i in range(3)],
+        *[(111 + i, 103 + i) for i in range(15)],
+        *[(147 + i, 57 + i) for i in range(14)],
+        *[(165 + i, 89 + i) for i in range(14)],
+    ]
 
-    for i,j in inds:
+    for i, j in inds:
         array[i] = _copy_array[j]
         names[i] = _copy_names[j]
 
-    array = np.reshape(array,(10,18,3))
-    names = np.reshape(names,(10,18))
-    ax = sp.get_axes((9,4.5))
+    array = np.reshape(array, (10, 18, 3))
+    names = np.reshape(names, (10, 18))
+    ax = ptk.get_axes((9, 4.5))
     ax.imshow(array)
 
     for i in range(18):
         for j in range(10):
-            c = 'k' if np.linalg.norm(array[j,i]) > 1 else 'w'
-            plt.text(i,j,names[j,i],color = c,ha='center',va='center')
+            c = "k" if np.linalg.norm(array[j, i]) > 1 else "w"
+            plt.text(i, j, names[j, i], color=c, ha="center", va="center")
     ax.set_axis_off()
-    plt.show()
-
-# Cell
-from matplotlib.patches import FancyArrowPatch
-from mpl_toolkits.mplot3d import proj3d
-
-class Arrow3D(FancyArrowPatch):
-    """Draw 3D fancy arrow."""
-    def __init__(self, x, y, z, u, v, w, *args, **kwargs):
-        FancyArrowPatch.__init__(self, (0, 0), (0, 0), *args, **kwargs)
-        self._verts3d = [x,x+u], [y,y+v], [z,z+w]
-
-    def draw(self, renderer):
-        xs3d, ys3d, zs3d = self._verts3d
-        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M) #renderer>M for < 3.4 but we don't need it
-        self.set_positions((xs[0], ys[0]), (xs[1], ys[1]))
-        super().draw(renderer)
-
-    def do_3d_projection(self, renderer): # For matplotlib >= 3.5
-        xs3d, ys3d, zs3d = self._verts3d
-        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M)
-        self.set_positions((xs[0], ys[0]), (xs[1], ys[1]))
-        return min(zs)
-
-    def on(self,ax):
-        ax.add_artist(self)
-
-def fancy_quiver3d(X,Y,Z,U,V,W,ax=None,C = 'r',L = 0.7,mutation_scale=10,**kwargs):
-    """Plots 3D arrows on a given ax. See [FancyArrowPatch](https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.patches.FancyArrowPatch.html).
-    - **Parameters**
-        - X, Y, Z : 1D arrays of coordinates of arrows' tail point.
-        - U, V, W : 1D arrays of dx,dy,dz of arrows.
-        - ax: 3D axes, if not given, auto created.
-        - C : 1D colors array mapping for arrows. Could be one color.
-        - L : 1D linwidths array mapping for arrows. Could be one linewidth.
-        - mutation_scale: Arrow head width/size scale. Default is 10.
-        - kwargs: FancyArrowPatch's keyword arguments excluding positions,color, lw and mutation_scale, shrinkA, shrinkB which are already used. An important keyword argument is `arrowstyle` which could be '->','-|>', their inverted forms and many more. See on matplotlib.
-    """
-    if not ax:
-        ax = sp.get_axes(figsize=(3.4,3.4),axes_3d=True) # Same aspect ratio.
-    if not isinstance(C,(list,tuple,np.ndarray)):
-        C = [[*mplc.to_rgb(C)] for x in X]
-    C = np.array(C) # Safe for list
-
-    if not isinstance(L,(list,tuple,np.ndarray)):
-        L = [L for x in X]
-    args_dict = dict(mutation_scale=mutation_scale,shrinkA=0, shrinkB=0)
-    for x,y,z,u,v,w,c,l in zip(X,Y,Z,U,V,W,C,L):
-        Arrow3D(x, y, z, u, v, w, color=c,lw=l,**args_dict,**kwargs).on(ax)
-
     return ax
 
-# Cell
-def get_selective_dynamics(poscar_data, *, a = None, b = None, c = None) -> np.ndarray:
-    """Returns selective dynamics array for a given POSCAR or None if no inputb given. By default, if a direction is not given, it turns ON with others.
-    - **Parameters**
-        - poscar_data: POSCAR data.
-        - a, b, c: Arrays of shape (N,2) that contain ranges in fractional coordinates to turn selective dynamics on.
-
-    - **Usage**
-        - `get_selective_dynamics(poscar_data, a = [(0,0.1),(0.9,1)])` will turn selective dynamics on for the first and last 10% of the unit cell in a-direction as T T T.
-        - `get_selective_dynamics(poscar_data, a = [(0,0.1),(0.9,1)], b = [(0,0.1),(0.9,1)])` will turn selective dynamics on for the first and last 10% of the unit cell in ab-plane in form of T T T, F T T and T F T whichever applies.
-    """
-    if (a is None) and (b is None) and (c is None):
-        return None
-
-    out_array = np.array([['F','F','F'] for a in poscar_data.positions]) # Default array
-    x, y, z = poscar_data.positions.T
 
-    if (np.ndim(a) == 2) and (np.shape(a)[1] == 2):
-        for left, right in a:
-            out_array[(x >= left) & (x <= right),0] = 'T'
-    elif a is not None:
-        raise ValueError(f'`a` should be None or array of ranges of shape (N,2) to turn on selective dynamics. got {a!r}')
-
-    if (np.ndim(b) == 2) and (np.shape(b)[1] == 2):
-        for left, right in b:
-            out_array[(y >= left) & (y <= right),1] = 'T'
-    elif b is not None:
-        raise ValueError(f'`b` should be None or array of ranges of shape (N,2) to turn on selective dynamics. got {b!r}')
-
-    if (np.ndim(c) == 2) and (np.shape(c)[1] == 2):
-        for left, right in c:
-            out_array[(z >= left) & (z <= right),2] = 'T'
-    elif c is not None:
-        raise ValueError(f'`c` should be None or array of ranges of shape (N,2) to turn on selective dynamics. got {c!r}')
-
-    # Now Turn ON what is not given but present in other directions
-    if a is None:
-        out_array[(out_array[:,1] == 'T')|(out_array[:,2] == 'T'), 0] = 'T'
-
-    if b is None:
-        out_array[(out_array[:,0] == 'T')|(out_array[:,2] == 'T'), 1] = 'T'
-
-    if c is None:
-        out_array[(out_array[:,0] == 'T')|(out_array[:,1] == 'T'), 2] = 'T'
-
-    return np.array(['  '.join(arr) for arr in out_array])
-
-def write_poscar(poscar_data, outfile = None, selective_dynamics = None, overwrite = False):
-    """Writes poscar data object to a file or returns string
-    - **Parameters**
-        - poscar_data: Output of `export_poscar`,`join_poscars` etc.
-        - outfile  : str,file path to write on.
-        - selective_dynamics  : A list ['T T T','F F F',...] strings to turn on selective dynamics at required sites. Use `get_selective_dynamics` to build this list precisely.
-        - overwrite: bool, if file already exists, overwrite=True changes it.
+def write_poscar(poscar_data, outfile=None, selective_dynamics=None, overwrite=False):
+    """Writes POSCAR data to a file or returns string
 
-    **Note**: POSCAR is only written in direct format even if it was loaded from cartesian format.
-    """
-    _comment = poscar_data.extra_info.comment
-    out_str = f'{poscar_data.SYSTEM}  # ' + (_comment or 'Created by Pivopty')
-    scale = poscar_data.extra_info.scale
+    Parameters
+    ----------
+    outfile : PathLike
+    selective_dynamics : callable
+        If given, should be a function like `f(index,x,y,z) -> (bool, bool, bool)`
+        which turns on/off selective dynamics for each atom based in each dimension.
+        See `ipyvasp.POSCAR.data.get_selective_dynamics` for more info.
+    overwrite: bool
+        If file already exists, overwrite=True changes it.
+
+
+    .. note::
+        POSCAR is only written in direct format even if it was loaded from cartesian format.
+    """
+    _comment = poscar_data.metadata.comment
+    out_str = f"{poscar_data.SYSTEM}  # " + (_comment or "Created by Pivopty")
+    scale = poscar_data.metadata.scale
     out_str += "\n  {:<20.14f}\n".format(scale)
-    out_str += '\n'.join(["{:>22.16f}{:>22.16f}{:>22.16f}".format(*a) for a in poscar_data.basis/scale])
-    uelems = poscar_data.unique.to_dict()
-    out_str += "\n  " + '    '.join(uelems.keys())
-    out_str += "\n  " + '    '.join([str(len(v)) for v in uelems.values()])
+    out_str += "\n".join(
+        ["{:>22.16f}{:>22.16f}{:>22.16f}".format(*a) for a in poscar_data.basis / scale]
+    )
+    uelems = poscar_data.types.to_dict()
+    out_str += "\n  " + "    ".join(uelems.keys())
+    out_str += "\n  " + "    ".join([str(len(v)) for v in uelems.values()])
+
     if selective_dynamics is not None:
         out_str += "\nSelective Dynamics"
 
     out_str += "\nDirect\n"
     positions = poscar_data.positions
     pos_list = ["{:>21.16f}{:>21.16f}{:>21.16f}".format(*a) for a in positions]
+
     if selective_dynamics is not None:
-        if len(pos_list) != len(selective_dynamics):
-            raise ValueError("len(selective_dynamics) != len(sites).")
-        pos_list = [f"{p}   {s}" for p,s in zip(pos_list,selective_dynamics)]
-    out_str += '\n'.join(pos_list)
+        sd = poscar_data.get_selective_dynamics(selective_dynamics).values()
+        pos_list = [f"{p}   {s}" for p, s in zip(pos_list, sd)]
+
+    out_str += "\n".join(pos_list)
     if outfile:
-        if not os.path.isfile(outfile):
-            with open(outfile,'w') as f:
+        path = Path(outfile)
+        if not path.is_file():
+            with path.open("w", encoding="utf-8") as f:
                 f.write(out_str)
 
-        elif overwrite and os.path.isfile(outfile):
-            with open(outfile,'w') as f:
+        elif overwrite and path.is_file():
+            with path.open("w", encoding="utf-8") as f:
                 f.write(out_str)
         else:
-            raise FileExistsError(f"{outfile!r} exists, can not overwrite, \nuse overwrite=True if you want to chnage.")
+            raise FileExistsError(
+                f"{outfile!r} exists, can not overwrite, \nuse overwrite=True if you want to chnage."
+            )
     else:
         print(out_str)
 
-def export_poscar(path = None,content = None):
-    """Export POSCAR file to python objects. Only Direct POSCAR supported.
-    - **Parameters**
-        - path: Path/to/POSCAR file. Auto picks in CWD.
-        - content: POSCAR content as string, This takes precedence to path.
+
+def export_poscar(path=None, content=None):
+    """Export POSCAR file to python objects.
+
+    Parameters
+    ----------
+    path : PathLike
+        Path/to/POSCAR file. Auto picks in CWD.
+    content : str
+        POSCAR content as string, This takes precedence to path.
     """
-    if content and isinstance(content,str):
-        path = content.splitlines() # This acts as slice for islice2array.
-    elif not path:
-        path = './POSCAR'
-        if not os.path.isfile(path):
-            raise FileNotFoundError(f"{path!r} not found.")
-    header = vp.islice2array(path,start=0,nlines=1,raw=True,exclude=None).split('#',1)
+    if content and isinstance(content, str):
+        file_lines = [f"{line}\n" for line in content.splitlines()]
+    else:
+        P = Path(path or "./POSCAR")
+        if not P.is_file():
+            raise FileNotFoundError(f"{str(P)} not found.")
+
+        with P.open("r", encoding="utf-8") as f:
+            file_lines = f.readlines()
+
+    header = file_lines[0].split("#", 1)
     SYSTEM = header[0].strip()
-    comment = header[1].strip() if len(header) > 1 else 'Exported by Pivopty'
+    comment = header[1].strip() if len(header) > 1 else "Exported by Pivopty"
 
-    scale = float(vp.islice2array(path,start=1,nlines=1,exclude=None,raw=True).strip())
-    if scale < 0: # If that is for volume
+    scale = float(file_lines[1].strip())
+    if scale < 0:  # If that is for volume
         scale = 1
-    basis = scale*vp.islice2array(path,start=2,nlines=3,exclude=None).reshape((-1,3))
-    #volume = np.linalg.det(basis)
-    #rec_basis = np.linalg.inv(basis).T # general formula
-    out_dict = {'SYSTEM':SYSTEM,#'volume':volume,
-                'basis':basis,#'rec_basis':rec_basis,
-                'extra_info':{'comment':comment,'scale':scale}}
-
-    elems = vp.islice2array(path,raw=True,start=5,nlines=1,exclude=None).split()
-    ions = vp.islice2array(path,start=6,nlines=1,exclude=None)
-    N = np.sum(ions).astype(int)
-    inds = np.cumsum([0,*ions]).astype(int)
+
+    basis = scale * vp.gen2numpy(file_lines[2:5], (3, 3), [-1, -1], exclude=None)
+    # volume = np.linalg.det(basis)
+    # rec_basis = np.linalg.inv(basis).T # general formula
+    out_dict = {
+        "SYSTEM": SYSTEM,  #'volume':volume,
+        "basis": basis,  #'rec_basis':rec_basis,
+        "metadata": {"comment": comment, "scale": scale},
+    }
+
+    elems = file_lines[5].split()
+    ions = [int(i) for i in file_lines[6].split()]
+    N = int(np.sum(ions))  # Must be py int, not numpy
+    inds = np.cumsum([0, *ions]).astype(int)
     # Check Cartesian and Selective Dynamics
-    lines = vp.islice2array(path,start=7,nlines=2,exclude=None,raw=True).splitlines()
-    lines = [l.strip() for l in lines] # remove whitespace or tabs
-    out_dict['extra_info']['cartesian'] = True if ((lines[0][0] in 'cCkK') or (lines[1][0] in 'cCkK')) else False
-    # Two lines are excluded in below command before start. so start = 7-2
-    positions = vp.islice2array(path,start=5,exclude="^\s+[a-zA-Z]|^[a-zA-Z]",cols=[0,1,2]).reshape((-1,3))[:N]
+    lines = [l.strip() for l in file_lines[7:9]]  # remove whitespace or tabs
+    out_dict["metadata"]["cartesian"] = (
+        True if ((lines[0][0] in "cCkK") or (lines[1][0] in "cCkK")) else False
+    )
+
+    poslines = vp.gen2numpy(
+        file_lines[7:],
+        (N, 6),
+        (-1, [0, 1, 2]),
+        exclude="^\s+[a-zA-Z]|^[a-zA-Z]",
+        raw=True,
+    ).splitlines()  # handle selective dynamics word here
+    positions = np.array(
+        [line.split()[:3] for line in poslines], dtype=float
+    )  # this makes sure only first 3 columns are taken
 
-    if out_dict['extra_info']['cartesian']:
-        positions = scale*to_basis(basis, positions)
+    if out_dict["metadata"]["cartesian"]:
+        positions = scale * to_basis(basis, positions)
         print(("Cartesian format found in POSCAR file, converted to direct format."))
 
     unique_d = {}
-    for i,e in enumerate(elems):
-        unique_d.update({e:range(inds[i],inds[i+1])})
+    for i, e in enumerate(elems):
+        unique_d.update({e: range(inds[i], inds[i + 1])})
 
     elem_labels = []
     for i, name in enumerate(elems):
-        for ind in range(inds[i],inds[i+1]):
+        for ind in range(inds[i], inds[i + 1]):
             elem_labels.append(f"{name} {str(ind - inds[i] + 1)}")
-    out_dict.update({'positions':positions,#'labels':elem_labels,
-                     'unique':unique_d})
+    out_dict.update({"positions": positions, "types": unique_d})  #'labels':elem_labels,
     return serializer.PoscarData(out_dict)
 
+
 # Cell
 def _save_mp_API(api_key):
-    """
-    - Save materials project api key for autoload in functions.
-    """
-    home = str(Path.home())
-    file = os.path.join(home,'.ipyvasprc')
+    "Save materials project api key for autoload in functions. This works only for legacy API."
+    path = Path.home() / ".ipyvasprc"
     lines = []
-    if os.path.isfile(file):
-        with open(file,'r') as fr:
+    if path.is_file():
+        with path.open("r") as fr:
             lines = fr.readlines()
-            lines = [line for line in lines if 'MP_API_KEY' not in line]
+            lines = [line for line in lines if "MP_API_KEY" not in line]
 
-    with open(file,'w') as fw:
+    with path.open("w") as fw:
         fw.write("MP_API_KEY = {}".format(api_key))
         for line in lines:
             fw.write(line)
 
+
 # Cell
-def _load_mp_data(formula,api_key=None,mp_id=None,max_sites = None, min_sites = None):
-    """
-    - Returns fetched data using request api of python form materials project website.
-    - **Parameters**
-        - formula  : Material formula such as 'NaCl'.
-        - api_key  : API key for your account from material project site. Auto picks if you already used `_save_mp_API` function.
-        - mp_id     : Optional, you can specify material ID to filter results.
-        - max_sites : Maximum number of sites. If None, sets `min_sites + 1`, if `min_sites = None`, gets all data.
-        - min_sites : Minimum number of sites. If None, sets `max_sites + 1`, if `max_sites = None`, gets all data.
-    """
+def _load_mp_data(formula, api_key=None, mp_id=None, max_sites=None, min_sites=None):
     if api_key is None:
         try:
-            home = str(Path.home())
-            file = os.path.join(home,'.ipyvasprc')
-            with open(file,'r') as f:
-                lines=f.readlines()
+            path = Path.home() / ".ipyvasprc"
+            with path.open("r") as f:
+                lines = f.readlines()
                 for line in lines:
-                    if 'MP_API_KEY' in line:
-                        api_key = line.split('=')[1].strip()
+                    if "MP_API_KEY" in line:
+                        api_key = line.split("=")[1].strip()
         except:
-            raise ValueError("api_key not given. provide in argument or generate in file using `_save_mp_API(your_mp_api_key)")
-
-    #url must be a raw string
-    url = r"https://legacy.materialsproject.org/rest/v2/materials/{}/vasp?API_KEY={}".format(formula,api_key)
-    resp = req.request(method='GET',url=url)
+            raise ValueError(
+                "api_key not given. provide in argument or generate in file using `_save_mp_API(your_mp_api_key)"
+            )
+
+    # url must be a raw string
+    url = r"https://legacy.materialsproject.org/rest/v2/materials/{}/vasp?API_KEY={}".format(
+        formula, api_key
+    )
+    resp = req.request(method="GET", url=url)
     if resp.status_code != 200:
         raise ValueError("Error in fetching data from materials project. Try again!")
 
     jl = json.loads(resp.text)
-    if not 'response' in jl: #check if response
+    if not "response" in jl:  # check if response
         raise ValueError("Either formula {!r} or API_KEY is incorrect.".format(formula))
 
-    all_res = jl['response']
+    all_res = jl["response"]
 
     if max_sites != None and min_sites != None:
         lower, upper = min_sites, max_sites
     elif max_sites == None and min_sites != None:
         lower, upper = min_sites, min_sites + 1
     elif max_sites != None and min_sites == None:
         lower, upper = max_sites - 1, max_sites
     else:
-        lower, upper = '-1', '-1' # Unknown
+        lower, upper = "-1", "-1"  # Unknown
 
-    if lower != '-1' and upper != '-1':
-        sel_res=[]
+    if lower != "-1" and upper != "-1":
+        sel_res = []
         for res in all_res:
-            if res['nsites'] <= upper and res['nsites'] >= lower:
+            if res["nsites"] <= upper and res["nsites"] >= lower:
                 sel_res.append(res)
         return sel_res
     # Filter to mp_id at last. more preferred
-    if mp_id !=None:
+    if mp_id != None:
         for res in all_res:
-            if mp_id == res['material_id']:
+            if mp_id == res["material_id"]:
                 return [res]
     return all_res
 
-# Cell
+
+def _cif_str_to_poscar_str(cif_str, comment=None):
+    # Using it in other places too
+    lines = [
+        line for line in cif_str.splitlines() if line.strip()
+    ]  # remove empty lines
+
+    abc = []
+    abc_ang = []
+    index = 0
+    for ys in lines:
+        if "_cell" in ys:
+            if "_length" in ys:
+                abc.append(ys.split()[1])
+            if "_angle" in ys:
+                abc_ang.append(ys.split()[1])
+            if "_volume" in ys:
+                volume = float(ys.split()[1])
+        if "_structural" in ys:
+            top = ys.split()[1] + f" # {comment}" if comment else ys.split()[1]
+    for i, ys in enumerate(lines):
+        if "_atom_site_occupancy" in ys:
+            index = i + 1  # start collecting pos.
+    poses = lines[index:]
+    pos_str = ""
+    for pos in poses:
+        s_p = pos.split()
+        pos_str += "{0:>12}  {1:>12}  {2:>12}  {3}\n".format(*s_p[3:6], s_p[0])
+
+    names = [re.sub("\d+", "", pos.split()[1]).strip() for pos in poses]
+    types = []
+    for name in names:
+        if name not in types:
+            types.append(name)  # unique types, don't use numpy here.
+
+    # ======== Cleaning ===========
+    abc_ang = [float(ang) for ang in abc_ang]
+    abc = [float(a) for a in abc]
+    a = "{0:>22.16f} {1:>22.16f} {2:>22.16f}".format(1.0, 0.0, 0.0)  # lattic vector a.
+    to_rad = 0.017453292519
+    gamma = abc_ang[2] * to_rad
+    bx, by = abc[1] * np.cos(gamma), abc[1] * np.sin(gamma)
+    b = "{0:>22.16f} {1:>22.16f} {2:>22.16f}".format(
+        bx / abc[0], by / abc[0], 0.0
+    )  # lattic vector b.
+    cz = volume / (abc[0] * by)
+    cx = abc[2] * np.cos(abc_ang[1] * to_rad)
+    cy = (abc[1] * abc[2] * np.cos(abc_ang[0] * to_rad) - bx * cx) / by
+    c = "{0:>22.16f} {1:>22.16f} {2:>22.16f}".format(
+        cx / abc[0], cy / abc[0], cz / abc[0]
+    )  # lattic vector b.
+
+    elems = "\t".join(types)
+    nums = [str(len([n for n in names if n == t])) for t in types]
+    nums = "\t".join(nums)
+    content = (
+        f"{top}\n  {abc[0]}\n {a}\n {b}\n {c}\n  {elems}\n  {nums}\nDirect\n{pos_str}"
+    )
+    return content
+
+
 class InvokeMaterialsProject:
     """Connect to materials project and get data using `api_key` from their site.
-    Usage:
-    ```python
-    from ipyvaspr.sio import InvokeMaterialsProject # or import ipyvasp.InvokeMaterialsProject as InvokeMaterialsProject
-    mp = InvokeMaterialsProject(api_key='your_api_key')
-    outputs = mp.request(formula='NaCl') #returns list of structures from response
-    outupts[0].export_poscar() #returns poscar data
-    outputs[0].cif #returns cif data
-    ```"""
-    def __init__(self,api_key=None):
+
+    Usage
+    -----
+    >>> from ipyvaspr.sio import InvokeMaterialsProject # or import ipyvasp.InvokeMaterialsProject as InvokeMaterialsProject
+    >>> mp = InvokeMaterialsProject(api_key='your_api_key')
+    >>> outputs = mp.request(formula='NaCl') #returns list of structures from response
+    >>> outupts[0].export_poscar() #returns poscar data
+    >>> outputs[0].cif #returns cif data
+    """
+
+    def __init__(self, api_key=None):
         "Request Materials Project acess. api_key is on their site. Your only need once and it is saved for later."
         self.api_key = api_key
         self.__response = None
         self.success = False
 
-    def save_api_key(self,api_key):
+    def save_api_key(self, api_key):
         "Save api_key for auto reloading later."
         _save_mp_API(api_key)
 
-    @lru_cache(maxsize=2) #cache for 2 calls
-    def request(self,formula,mp_id=None,max_sites = None,min_sites=None):
-        """Fetch data using request api of python form materials project website. After request, you can access `cifs` and `poscars`.
-        - **Parameters**
-            - formula  : Material formula such as 'NaCl'.
-            - mp_id     : Optional, you can specify material ID to filter results.
-            - max_sites : Maximum number of sites. If None, sets `min_sites + 1`, if `min_sites = None`, gets all data.
-            - min_sites : Minimum number of sites. If None, sets `max_sites + 1`, if `max_sites = None`, gets all data.
-        """
-        self.__response = _load_mp_data(formula = formula,api_key = self.api_key, mp_id = mp_id, max_sites = max_sites,min_sites=min_sites)
+    @lru_cache(maxsize=2)  # cache for 2 calls
+    def request(self, formula, mp_id=None, max_sites=None, min_sites=None):
+        "Fetch data using request api of python form materials project website. After request, you can access `cifs` and `poscars`."
+        self.__response = _load_mp_data(
+            formula=formula,
+            api_key=self.api_key,
+            mp_id=mp_id,
+            max_sites=max_sites,
+            min_sites=min_sites,
+        )
         if self.__response == []:
             raise req.HTTPError("Error in request. Check your api_key or formula.")
 
         class Structure:
-            def __init__(self,response):
-                self._cif    = response['cif']
-                self.symbol  = response['spacegroup']['symbol']
-                self.crystal = response['spacegroup']['crystal_system']
-                self.unit    = response['unit_cell_formula']
-                self.mp_id   = response['material_id']
+            def __init__(self, response):
+                self._cif = response["cif"]
+                self.symbol = response["spacegroup"]["symbol"]
+                self.crystal = response["spacegroup"]["crystal_system"]
+                self.unit = response["unit_cell_formula"]
+                self.mp_id = response["material_id"]
 
             @property
             def cif(self):
                 return self._cif
 
             def __repr__(self):
                 return f"Structure(unit={self.unit},mp_id={self.mp_id!r},symbol={self.symbol!r},crystal={self.crystal!r},cif='{self._cif[:10]}...')"
 
-            def write_cif(self,outfile = None):
-                if isinstance(outfile,str):
-                    with open(outfile,'w') as f:
+            def write_cif(self, outfile=None):
+                if isinstance(outfile, str):
+                    with open(outfile, "w") as f:
                         f.write(self._cif)
                 else:
                     print(self._cif)
 
-            def write_poscar(self,outfile = None, overwrite = False):
-                "Use `ipyvasp.api.POSCAR.write/ipyvasp.sio.write_poscar` if you need extra options."
-                write_poscar(self.export_poscar(),outfile = outfile, overwrite = overwrite)
+            def write_poscar(self, outfile=None, overwrite=False):
+                "Use `ipyvasp.lattice.POSCAR.write` if you need extra options."
+                write_poscar(self.export_poscar(), outfile=outfile, overwrite=overwrite)
 
             def export_poscar(self):
-                lines = self._cif.split('\n')
-                if '' in lines.copy():
-                    lines.remove('')
-                abc = []
-                abc_ang = []
-                index = 0
-                for ys in lines:
-                    if '_cell' in ys:
-                        if '_length' in ys:
-                            abc.append(ys.split()[1])
-                        if '_angle' in ys:
-                            abc_ang.append(ys.split()[1])
-                        if '_volume' in ys:
-                            volume = float(ys.split()[1])
-                    if '_structural' in ys:
-                        top = ys.split()[1] + f" # [{self.mp_id!r}][{self.symbol!r}][{self.crystal!r}] Created by ipyvasp using Materials Project Database"
-                for i,ys in enumerate(lines):
-                    if '_atom_site_occupancy' in ys:
-                        index = i +1 # start collecting pos.
-                poses = lines[index:]
-                pos_str = ""
-                for pos in poses:
-                    s_p = pos.split()
-                    pos_str += "{0:>12}  {1:>12}  {2:>12}  {3}\n".format(*s_p[3:6],s_p[0])
-
-                # ======== Cleaning ===========
-                abc_ang = [float(ang) for ang in abc_ang]
-                abc     = [float(a) for a in abc]
-                a = "{0:>22.16f} {1:>22.16f} {2:>22.16f}".format(1.0,0.0,0.0) # lattic vector a.
-                to_rad = 0.017453292519
-                gamma = abc_ang[2]*to_rad
-                bx,by = abc[1]*np.cos(gamma),abc[1]*np.sin(gamma)
-                b = "{0:>22.16f} {1:>22.16f} {2:>22.16f}".format(bx/abc[0],by/abc[0],0.0) # lattic vector b.
-                cz = volume/(abc[0]*by)
-                cx = abc[2]*np.cos(abc_ang[1]*to_rad)
-                cy = (abc[1]*abc[2]*np.cos(abc_ang[0]*to_rad)-bx*cx)/by
-                c = "{0:>22.16f} {1:>22.16f} {2:>22.16f}".format(cx/abc[0],cy/abc[0],cz/abc[0]) # lattic vector b.
-
-                elems = [elem for elem in self.unit.keys()]
-                elems = '\t'.join(elems)
-                nums  = [str(int(self.unit[elem])) for elem in self.unit.keys()]
-                nums  = '\t'.join(nums)
-                content = f"{top}\n  {abc[0]}\n {a}\n {b}\n {c}\n  {elems}\n  {nums}\nDirect\n{pos_str}"
-                return export_poscar(content = content)
-
+                "Export poscar data form cif content."
+                content = _cif_str_to_poscar_str(
+                    self._cif,
+                    comment=f"[{self.mp_id!r}][{self.symbol!r}][{self.crystal!r}] Created by ipyvasp using Materials Project Database",
+                )
+                return export_poscar(content=content)
 
         # get cifs
         structures = []
         for res in self.__response:
             structures.append(Structure(res))
 
-        self.success = True # set success flag
+        self.success = True  # set success flag
         return structures
 
-# Cell
-def get_kpath(*patches, n = 5,weight= None ,ibzkpt = None,outfile=None, rec_basis = None):
-    """
-    Generate list of kpoints along high symmetry path. Options are write to file or return KPOINTS list.
-    It generates uniformly spaced point with input `n` as just a scale factor of number of points per unit length.
-    You can also specify custom number of kpoints in an interval by putting number of kpoints as 4th entry in left kpoint.
-    - **Parameters**
-        - *ptaches : Any number of disconnected patches where a single patch is a dictionary like {'label': (x,y,z,[N]), ...} where x,y,z is high symmetry point and
-                    N (optional) is number of points in current inteval, points in a connected path patch are at least two i.e. `{'p1':[x1,y1,z1],'p2':[x2,y2,z2]}`.
-                    A key of a patch should be string reperenting the label of the high symmetry point. A key that starts with '_' is ignored, so you can add points without high symmetry points as well.
-        - n        : int, number per length of body diagonal of rec_basis, this makes uniform steps based on distance between points.
-        - weight : Float, if None, auto generates weights.
-        - ibzkpt : Path to ibzkpt file, required for HSE calculations.
-        - outfile: Path/to/file to write kpoints.
-        - rec_basis: Reciprocal basis 3x3 array to use for calculating uniform points.
+
+def _str2kpoints(kpts_str):
+    hsk_list = []
+    for j, line in enumerate(kpts_str.splitlines()):
+        if line.strip():  # Make sure line is not empty
+            data = line.split()
+            if len(data) < 3:
+                raise ValueError(f"Line {j + 1} has less than 3 values.")
+
+            point = [float(i) for i in data[:3]]
+
+            if len(data) == 4:
+                _4th = (
+                    data[3]
+                    if re.search("\$\\\\[a-zA-Z]+\$|[a-zA-Z]+|[α-ωΑ-Ω]+|\|_", line)
+                    else int(data[3])
+                )
+                point.append(_4th)
+            elif len(data) == 5:
+                _5th = int(data[4])
+                point = point + [data[3], _5th]
+
+            hsk_list.append(point)
+    return hsk_list
+
+
+def get_kpath(kpoints, n=5, weight=None, ibzkpt=None, outfile=None, rec_basis=None):
+    """Generate list of kpoints along high symmetry path. Options are write to file or return KPOINTS list.
+    It generates uniformly spaced point with input `n` as just a scale factor of number of points per average length of `rec_basis`.
+
+    Parameters
+    ----------
+    kpoints : list or str
+        Any number points as [(x,y,z,[label],[N]), ...]. N adds as many points in current interval.
+        To disconnect path at a point, provide it as (x,y,z,[label], 0), next point will be start of other patch.
+        If `kpoints` is a multiline string, it is converted to list of points. Each line should be in format "x y z [label] [N]".
+    n : int
+        Number of point per averge length of `rec_basis`, this makes uniform steps based on distance between points.
+        If (x,y,z,[label], N) is provided, this is ignored for that specific interval. If `rec_basis` is not provided, each interval has exactly `n` points.
+        Number of points in each interval is at least 2 even if `n` is less than 2 to keep end points anyway.
+    weight : float
+        None by default to auto generates weights.
+    ibzkpt : PathLike
+        Path to ibzkpt file, required for HSE calculations.
+    outfile : PathLike
+        Path/to/file to write kpoints.
+    rec_basis : array_like
+        Reciprocal basis 3x3 array to use for calculating uniform points.
+
 
     If `outfile = None`, KPONITS file content is printed.
     """
-    if len(patches) == 0:
-        raise ValueError("Please provide at least one high symmetry path consisting of two points.")
+    if isinstance(kpoints, str):
+        kpoints = _str2kpoints(kpoints)
+    elif not isinstance(kpoints, (list, tuple, np.ndarray)):
+        raise TypeError(
+            f"kpoints must be a sequence as [(x,y,z,[label],[N]), ...], or multiline string got {kpoints}"
+        )
+
+    if len(kpoints) < 2:
+        raise ValueError("At least two points are required.")
+
+    fixed_patches = []
+    where_zero = []
+    for idx, point in enumerate(kpoints):
+        if not isinstance(point, (list, tuple)):
+            raise TypeError(
+                f"kpoint must be a list or tuple as (x,y,z,[label],[N]),  got {point}"
+            )
+
+        cpt = point  # same for length 5, 4 with last entry as string
+
+        if len(point) == 3:
+            cpt = [*point, ""]  # make (x,y,z,label)
+        elif len(point) == 4:
+            if isinstance(point[3], (int, np.integer)):
+                cpt = [*point[:3], "", point[-1]]  # add full point as (x,y,z,label, N)
+            elif not isinstance(point[3], str):
+                raise TypeError(
+                    f"4th entry in kpoint should be string label or int number of points for next interval if label is skipped, got {point}"
+                )
+        elif len(point) == 5:
+            if not isinstance(point[3], str):
+                raise TypeError(
+                    f"4th entry in kpoint should be string label when 5 entries are given, got {point}"
+                )
+            if not isinstance(point[4], (int, np.integer)):
+                raise TypeError(
+                    f"5th entry in kpoint should be an integer to add that many points in interval, got {point}"
+                )
+        else:
+            raise ValueError(f"Expects kpoint as (x,y,z,[label],[N]), got {point}")
 
-    hsk_list, labels = [], []
-    for patch in patches:
-        if not isinstance(patch,dict):
-            raise TypeError("Patche must be a dictionary as {'label': (x,y,z,[N]), ...}")
-        if len(patch.keys()) < 2:
-            raise ValueError("Please provide at least one high symmetry path consisting of two points.")
-        _patch = []
-        for k,v in patch.items():
-            if not isinstance(k,str):
-                raise TypeError("Label must be a string")
-            if (not isinstance(v,(list,tuple,set,np.ndarray))) and (len(v) not in [3,4]):
-                raise TypeError("Value must be a list or tuple of length 3 or 4, like (x,y,z,[N])")
-            labels.append('skip' if k.startswith('_') else k)
-            _patch.append(v)
-        hsk_list.append(_patch)
-
-    xs,ys,zs, inds,joinat = [],[],[],[0],[] # 0 in inds list is important
-    _labels = []
-    _len_prev = 0
-    for j,a in enumerate(hsk_list):
-        for i in range(len(a)-1):
-            try:
-                _m = a[i][3] # number of points given explicitly.
-            except IndexError:
-                if rec_basis is not None and np.size(rec_basis) == 9:
-                    basis = np.array(rec_basis)
-                    coords = to_R3(basis,[a[i][:3],a[i+1][:3]])
-                    largest_dist = np.linalg.norm(basis.sum(axis=0)) # body diagonal
-                    _m = np.rint(np.linalg.norm(coords[0] - coords[1])*n/largest_dist).astype(int)
-                else:
-                    _vec = [_a-_b for _a,_b in zip(a[i][:3],a[i+1] )] # restruct point if 4 entries
-                    _m = np.rint(np.linalg.norm(_vec)*n).astype(int) # Calculate
+        if isinstance(cpt[-1], (int, np.integer)) and cpt[-1] == 0:
+            if idx - 1 in where_zero:
+                raise ValueError(
+                    f"Break at adjacent kpoints {idx}, {idx+1} is not allowed!"
+                )
+            if any([idx < 1, idx > (len(kpoints) - 3)]):
+                raise ValueError("Bad break at edges!")
+            where_zero.append(idx)
+
+        fixed_patches.append(cpt)
+
+    def add_points(p1, p2, npts, rec_basis):
+        lab = p2[3]  # end point label
+        if len(p1) == 5:
+            m = p1[4]  # number of points given explicitly.
+            lab = (
+                f"<={p1[3]}|{lab}" if m == 0 else lab
+            )  # merge labels in case user wants to break path
+        elif rec_basis is not None and np.size(rec_basis) == 9:
+            basis = np.array(rec_basis)
+            coords = to_R3(basis, [p1[:3], p2[:3]])
+            _mean = np.mean(
+                np.linalg.norm(basis, axis=1)
+            )  # average length of basis vectors
+            m = np.rint(npts * np.linalg.norm(coords[0] - coords[1]) / _mean).astype(
+                int
+            )  # number of points in interval
+        else:
+            m = npts  # equal number of points in each interval, given by n.
 
-            _m = _m if _m >= 2 else 2 # minimum of 2 points in a path
+        # Doing m - 1 in an interval, so along with last point, total n points are generated per interval.
+        Np = max(m - 1, 1)  # At least 2 points. one is given by end point of interval.
+        X = np.linspace(p1[0], p2[0], Np, endpoint=False)
+        Y = np.linspace(p1[1], p2[1], Np, endpoint=False)
+        Z = np.linspace(p1[2], p2[2], Np, endpoint=False)
+
+        kpts = [(x, y, z) for x, y, z in zip(X, Y, Z)]
+        return (kpts, Np, lab)
+
+    points, numbers, labels = [], [0], [fixed_patches[0][3]]
+    for p1, p2 in zip(fixed_patches[:-1], fixed_patches[1:]):
+        kp, m, lab = add_points(p1, p2, n, rec_basis)
+        points.extend(kp)
+        numbers.append(numbers[-1] + m)
+        labels.append(lab)
+        if lab.startswith("<="):
+            labels[-2] = ""  # remove label for end of interval if broken, added here
+    else:  # Add last point at end of for loop
+        points.append(p2[:3])
+
+    if weight is None and points:
+        weight = 0 if ibzkpt else 1 / len(points)  # With IBZKPT, we need zero weight
+
+    out_str = [
+        "{0:>16.10f}{1:>16.10f}{2:>16.10f}{3:>12.6f}".format(x, y, z, weight)
+        for x, y, z in points
+    ]
+    out_str = "\n".join(out_str)
 
-            inds.append(inds[-1]+_m) #Append first then do next
-            _labels.append(labels[i+_len_prev])
-            if j !=0 and i == 0:
-                joinat.append(inds[-2]) # Add previous in joinpath and label
-                if 'skip' not in _labels[-2]:
-                    _labels[-1] = _labels[-2] + '|' + _labels[-1]
-                    _labels = [*_labels[:-2],_labels[-1]] # Drop the label we added before
-
-            xs.append(list(np.linspace(a[i][0],a[i+1][0],_m)))
-            ys.append(list(np.linspace(a[i][1],a[i+1][1],_m)))
-            zs.append(list(np.linspace(a[i][2],a[i+1][2],_m)))
-
-        _labels.append(labels[len(a) -1 +_len_prev]) # Add last in current interval
-        _len_prev += len(a)
-
-    xs = [y for z in xs for y in z] #flatten values.
-    ys = [y for z in ys for y in z]
-    zs = [y for z in zs for y in z]
-
-    if weight == None and xs:
-        weight = 1/len(xs)
-
-    out_str = ["{0:>16.10f}{1:>16.10f}{2:>16.10f}{3:>12.6f}".format(x,y,z,weight) for x,y,z in zip(xs,ys,zs)]
-    out_str = '\n'.join(out_str)
-    N = np.size(xs)
-    if ibzkpt != None:
-        if os.path.isfile(ibzkpt):
-            with open(ibzkpt,'r') as f:
-                lines = f.readlines()
+    N = len(points)
+    if (PI := Path(ibzkpt or "")).is_file():  # handles None automatically
+        with PI.open("r") as f:
+            lines = f.readlines()
 
-            N = int(lines[1].strip())+N # Update N.
-            slines = lines[3:N+4]
-            ibz_str = ''.join(slines)
-            out_str = "{}\n{}".format(ibz_str,out_str) # Update out_str
-    if inds:
-        inds[-1] = -1 # last index to -1
-
-    inds = [i for k,i in enumerate(inds) if 'skip' != _labels[k]]
-    _labels = [l.replace('|skip','') for l in _labels if l != 'skip']
-    top_str = "Automatically generated using ipyvasp with HSK-INDS = {}, LABELS = {}, SEG-INDS = {}\n\t{}\nReciprocal Lattice".format(inds,_labels,joinat,N)
-    out_str = "{}\n{}".format(top_str,out_str)
+        N = int(lines[1].strip()) + N  # Update N.
+        slines = lines[3 : N + 4]
+        ibz_str = "".join(slines)
+        out_str = "{}\n{}".format(ibz_str.strip("\n"), out_str)
+
+    path_info = ", ".join(
+        f"{idx}:{lab}" for idx, lab in zip(numbers, labels) if lab != ""
+    )
+
+    top_str = "Automatically generated using ipyvasp for HSK-PATH {}\n\t{}\nReciprocal Lattice".format(
+        path_info, N
+    )
+    out_str = "{}\n{}".format(top_str, out_str)
     if outfile != None:
-        with open(outfile,'w') as f:
+        with open(outfile, "w", encoding="utf-8") as f:  # allow unicode
             f.write(out_str)
     else:
         print(out_str)
 
-def read_ticks(kpoints_file_path):
-    "Reads ticks values and labels in header of kpoint file. Returns dictionary of `ktick_inds`,`ktick_vals`,`kseg_inds` that can be unpacked to plotting functions. If not exist in header, returns empty values(still valid)."
-    out_dict = dict(ktick_inds=[],ktick_vals=[],kseg_inds=[])
-    if os.path.isfile(kpoints_file_path):
-        head = vp.islice2array(kpoints_file_path,exclude=None,raw=True,nlines=1)
-        if 'HSK-INDS' in head:
-            hsk = head.split('HSK-INDS')[1].split(']')[0].split('[')[1].split(',')
-            out_dict['ktick_inds'] = [int(h) for h in hsk if h]
-        if 'LABELS' in head:
-            labs = head.split('LABELS')[1].split(']')[0].split('[')[1].split(',')
-            out_dict['ktick_vals'] = [l.replace("'","").replace('"','').strip() for l in labs if l]
-        if 'SEG-INDS' in head:
-            segs = head.split('SEG-INDS')[1].split(']')[0].split('[')[1].split(',')
-            out_dict['kseg_inds'] = [int(s) for s in segs if s]
-    return out_dict
 
 # Cell
-def str2kpath(kpath_str,n = 5, weight = None, ibzkpt = None, outfile = None, rec_basis = None):
-    """Get Kpath from a string of kpoints (Line-Mode like). Useful in Terminal.
-    - **Parameters**
-        - kpath_str: str, a multiline string similiar to line mode of KPOINTS, initial 4 lines are not required.
-            - If you do not want to label a point, label it as 'skip' and it will be removed.
-            - You can add an interger at end of a line to customize number of points in a given patch.
-            - Each empty line breaks the path, so similar points before and after empty line are useless here.
-        - n      : int, number per length of body diagonal of rec_basis, this makes uniform steps based on distance between points.
-        - weight : Float, if None, auto generates weights.
-        - ibzkpt : Path to ibzkpt file, required for HSE calculations.
-        - outfile: Path/to/file to write kpoints.
-        - rec_basis: Reciprocal basis 3x3 array to use for calculating uniform points.
-
-    - **Example**
-        > str2kpath('''0 0 0 !$\Gamma$ 3
-                    0.25 0.25 0.25 !L''')
-        > Automatically generated using ipyvasp with HSK-INDS = [0, -1], LABELS = ['$\\Gamma$', 'L'], SEG-INDS = []
-	    >   3
-        > Reciprocal Lattice
-        >   0.0000000000    0.0000000000    0.0000000000    0.333333
-        >   0.1250000000    0.1250000000    0.1250000000    0.333333
-        >   0.2500000000    0.2500000000    0.2500000000    0.333333
-    """
-    lines = kpath_str.splitlines()
+def get_kmesh(
+    poscar_data,
+    *args,
+    shift=0,
+    weight=None,
+    cartesian=False,
+    ibzkpt=None,
+    outfile=None,
+    endpoint=True,
+):
+    """Generates uniform mesh of kpoints. Options are write to file, or return KPOINTS list.
+
+    Parameters
+    ----------
+    poscar_data : ipyvasp.POSCAR.data
+    *args : tuple
+        1 or 3 integers which decide shape of mesh. If 1, mesh points equally spaced based on data from POSCAR.
+    shift : float
+        Only works if cartesian = False. Defualt is 0. Could be a number or list of three numbers to add to interval [0,1].
+    weight : float
+        If None, auto generates weights.
+    cartesian : bool
+        If True, generates cartesian mesh.
+    ibzkpt : PathLike
+        Path to ibzkpt file, required for HSE calculations.
+    outfile : PathLike
+        Path/to/file to write kpoints.
+    endpoint : bool
+        Default True, include endpoints in mesh at edges away from origin.
 
-    skipN = 0
-    for _n, line in enumerate(lines[:6]): #Handle strings from AFLOW-like softwares
-        if line.strip().isalpha():
-            skipN = _n + 1
-
-    where_blanks = [i for i,line in enumerate(lines) if line.strip() == '']
-
-    hsk_list, labels = [],[]
-    for j,line in enumerate(lines[skipN:]):
-        if line.strip():
-            _labs = re.findall('\$\\\\[a-zA-Z]+\$|[a-zA-Z]+|[α-ωΑ-Ω]+|\|', line)
-            labels.append(_labs[0] if _labs else '')
-            _ks = re.findall('[-+\d]*[.][\d+]+|[-+]*\d+/\d+|[-+]*\d+',line)
-            _ks = [[float(k) for k in w.split('/')] if '/' in w else float(w) for w in _ks]
-
-            for i,_k in enumerate(_ks):
-                if type(_k) == list and len(_k) == 2:
-                    _ks[i] = _k[0]/_k[1]
-                elif type(_k) == list and len(_k) != 2:
-                    print(f'Check if you provide fraction correctly in line {j+1+skipN}!')
-
-            if len(_ks) == 4:
-                try: _ks[3] = int(_ks[3])
-                except: print(f'4th number in line {j+1+skipN} should be integer!')
-
-            hsk_list.append(_ks)
-
-    if where_blanks:
-        filtered = [w-i for i,w in enumerate(where_blanks)]
-        where_blanks = np.unique([0,*filtered,len(hsk_list)]).tolist()
-
-    patches = [] if where_blanks else [{k:v for v,k in zip(hsk_list,labels)},] #Fix up both
-    for a,b in zip(where_blanks[:-1], where_blanks[1:]):
-        if b - a < 2:
-            raise ValueError(f"There should be at least two points in a patch of path at line {a+1}!")
-        patches.append({k:v for v,k in zip(hsk_list[a:b],labels[a:b])})
 
-    return get_kpath(*patches,n=n,weight=weight,ibzkpt=ibzkpt,outfile=outfile, rec_basis = rec_basis)
-
-# Cell
-def _get_basis(path_pos):
-    """Returns given(computed) and inverted basis as tuple(given,inverted).
-    - **Parameters**
-        - path_pos: path/to/POSCAR or 3 given vectors as rows of a matrix."""
-    if isinstance(path_pos,(list,tuple,np.ndarray)) and np.ndim(path_pos) ==2:
-        basis = np.array(path_pos)
-    elif isinstance(path_pos,str) or isinstance(path_pos,type(None)):
-        basis = export_poscar(path_pos).basis
-    else:
-        raise FileNotFoundError("{!r} does not exist or not 3 by 3 list.".format(path_pos))
-    # Process. 2π is not included in vasp output
-    rec_basis = np.linalg.inv(basis).T # Compact Formula
-    Basis = namedtuple('Basis', ['given', 'inverted'])
-    return Basis(basis,rec_basis)
+    If `outfile = None`, KPOINTS file content is printed.
 
-# Cell
-def get_kmesh(poscar_data, *args, shift = 0, weight = None, cartesian = False, ibzkpt= None, outfile=None, endpoint = True):
-    """**Note**: Use `ipyvasp.POSCAR.get_kmesh` to get k-mesh based on current POSCAR.
-    - Generates uniform mesh of kpoints. Options are write to file, or return KPOINTS list.
-    - **Parameters**
-        - poscar_data: export_poscar() or export_vasprun().poscar().
-        - *args: 1 or 3 integers which decide shape of mesh. If 1, mesh points equally spaced based on data from POSCAR.
-        - shift  : Only works if cartesian = False. Defualt is 0. Could be a number or list of three numbers to add to interval [0,1].
-        - weight : Float, if None, auto generates weights.
-        - cartesian: If True, generates cartesian mesh.
-        - ibzkpt : Path to ibzkpt file, required for HSE calculations.
-        - outfile: Path/to/file to write kpoints.
-        - endpoint: Default True, include endpoints in mesh at edges away from origin.
-
-    If `outfile = None`, KPOINTS file content is printed."""
-    if len(args) not in [1,3]:
+    """
+    if len(args) not in [1, 3]:
         raise ValueError("get_kmesh() takes 1 or 3 args!")
 
     if cartesian:
-        norms = np.ptp(poscar_data.rec_basis,axis=0)
+        norms = np.ptp(poscar_data.rec_basis, axis=0)
     else:
-        norms = np.linalg.norm(poscar_data.rec_basis, axis = 1)
+        norms = np.linalg.norm(poscar_data.rec_basis, axis=1)
 
     if len(args) == 1:
-        if not isinstance(args[0],int):
+        if not isinstance(args[0], (int, np.integer)):
             raise ValueError("get_kmesh expects integer for first positional argument!")
-        nx,ny,nz = [args[0] for _ in range(3)]
+        nx, ny, nz = [args[0] for _ in range(3)]
 
-        weights = norms/np.max(norms) # For making largest side at given n
-        nx, ny, nz = np.rint(weights*args[0]).astype(int)
+        weights = norms / np.max(norms)  # For making largest side at given n
+        nx, ny, nz = np.rint(weights * args[0]).astype(int)
 
     elif len(args) == 3:
-        for i,a in enumerate(args):
-            if not isinstance(a,int):
+        for i, a in enumerate(args):
+            if not isinstance(a, (int, np.integer)):
                 raise ValueError("get_kmesh expects integer at position {}!".format(i))
-        nx,ny,nz = list(args)
+        nx, ny, nz = list(args)
 
-    low,high = np.array([[0,0,0],[1,1,1]]) + shift
+    low, high = np.array([[0, 0, 0], [1, 1, 1]]) + shift
     if cartesian:
-        verts = get_bz(poscar_data.basis, primitive=False).vertices
-        low, high = np.min(verts,axis=0), np.max(verts,axis=0)
-        low = (low * 2 * np.pi / poscar_data.extra_info.scale).round(12) # Cartesian KPOINTS are in unit of 2pi/SCALE
-        high = (high * 2 * np.pi / poscar_data.extra_info.scale).round(12)
+        verts = get_bz(poscar_data.rec_basis, primitive=False).vertices
+        low, high = np.min(verts, axis=0), np.max(verts, axis=0)
+        low = (low * 2 * np.pi / poscar_data.metadata.scale).round(
+            12
+        )  # Cartesian KPOINTS are in unit of 2pi/SCALE
+        high = (high * 2 * np.pi / poscar_data.metadata.scale).round(12)
 
-    (lx,ly,lz),(hx,hy,hz) = low,high
+    (lx, ly, lz), (hx, hy, hz) = low, high
     points = []
-    for k in np.linspace(lz,hz,nz, endpoint = endpoint):
-        for j in np.linspace(ly,hy,ny, endpoint = endpoint):
-            for i in np.linspace(lx,hx,nx, endpoint = endpoint):
-                points.append([i,j,k])
+    for k in np.linspace(lz, hz, nz, endpoint=endpoint):
+        for j in np.linspace(ly, hy, ny, endpoint=endpoint):
+            for i in np.linspace(lx, hx, nx, endpoint=endpoint):
+                points.append([i, j, k])
 
     points = np.array(points)
     points[np.abs(points) < 1e-10] = 0
 
     if len(points) == 0:
-        raise ValueError('No KPOINTS in BZ from given input. Try larger input!')
+        raise ValueError("No KPOINTS in BZ from given input. Try larger input!")
 
     if weight == None and len(points) != 0:
-        weight = float(1/len(points))
+        weight = float(1 / len(points))
 
-    out_str = ["{0:>16.10f}{1:>16.10f}{2:>16.10f}{3:>12.6f}".format(x,y,z,weight) for x,y,z in points]
-    out_str = '\n'.join(out_str)
+    out_str = [
+        "{0:>16.10f}{1:>16.10f}{2:>16.10f}{3:>12.6f}".format(x, y, z, weight)
+        for x, y, z in points
+    ]
+    out_str = "\n".join(out_str)
     N = len(points)
-    if ibzkpt and os.path.isfile(ibzkpt):
-        with open(ibzkpt,'r') as f:
+    if ibzkpt and (PI := Path(ibzkpt)):
+        with PI.open("r", encoding="utf-8") as f:
             lines = f.readlines()
 
-        if (cartesian == False) and (lines[2].strip()[0] in 'cCkK'):
-            raise ValueError("ibzkpt file is in cartesian coordinates, use get_kmesh(...,cartesian = True)!")
-
-        N = int(lines[1].strip())+N # Update N.
-        slines = lines[3:N+4]
-        ibz_str = ''.join(slines)
-        out_str = "{}\n{}".format(ibz_str,out_str) # Update out_str
-    mode = 'Reciprocal' if cartesian == False else 'Cartesian'
-    top_str = "Generated uniform mesh using ipyvasp, GRID-SHAPE = [{},{},{}]\n\t{}\n{}".format(nx,ny,nz,N,mode)
-    out_str = "{}\n{}".format(top_str,out_str)
+        if (cartesian == False) and (lines[2].strip()[0] in "cCkK"):
+            raise ValueError(
+                "ibzkpt file is in cartesian coordinates, use get_kmesh(...,cartesian = True)!"
+            )
+
+        N = int(lines[1].strip()) + N  # Update N.
+        slines = lines[3 : N + 4]
+        ibz_str = "".join(slines)
+        out_str = "{}\n{}".format(ibz_str, out_str)  # Update out_str
+    mode = "Reciprocal" if cartesian == False else "Cartesian"
+    top_str = "Generated uniform mesh using ipyvasp, GRID-SHAPE = [{},{},{}]\n\t{}\n{}".format(
+        nx, ny, nz, N, mode
+    )
+    out_str = "{}\n{}".format(top_str, out_str)
     if outfile != None:
-        with open(outfile,'w') as f:
+        with open(outfile, "w", encoding="utf-8") as f:
             f.write(out_str)
     else:
         print(out_str)
 
-# Cell
-def _tan_inv(vy,vx):
-    """
-    - Returns full angle from x-axis counter clockwise.
-    - **Parameters**
-        - vy : Perpendicular componet of vector including sign.
-        - vx : Base compoent of vector including sign.
-    """
-    angle = 0  # Place hodler to handle exceptions
-    if vx == 0 and vy == 0:
-        angle = 0
-    elif vx == 0 and np.sign(vy) == -1:
-        angle = 3*np.pi/2
-    elif vx == 0 and np.sign(vy) == 1:
-        angle = np.pi/2
-    else:
-        theta = abs(np.arctan(vy/vx))
-        if np.sign(vx) == 1 and np.sign(vy) == 1:
-            angle = theta
-        if np.sign(vx) == -1 and np.sign(vy) == 1:
-            angle = np.pi - theta
-        if np.sign(vx) == -1 and np.sign(vy) == -1:
-            angle = np.pi + theta
-        if np.sign(vx) == 1 and np.sign(vy) == -1:
-            angle = 2*np.pi - theta
-        if np.sign(vx) == -1 and vy == 0:
-            angle = np.pi
-        if np.sign(vx) == 1 and vy == 0:
-            angle = 2*np.pi
-    return angle
-
-def order(points,loop=True):
-    """
-    - Returns indices of counterclockwise ordered vertices of a plane in 3D.
-    - **Parameters**
-        - points: numpy array of shape (N,3) or List[List(len=3)].
-        - loop  : Default is True and appends start point at end to make a loop.
-    - **Example**
-        > pts = np.array([[1,0,3],[0,0,0],[0,1,2]])
-        > inds = order(pts)
-        > pts[inds]
-        ```
-        array([[1, 2, 3],
-               [0, 0, 0],
-               [1, 0, 3]
-               [0, 1, 2]])
-        ```
-    """
-    points = np.array(points) # Make array.
-    # Fix points if start point is zero.
-    if np.sum(points[0]) == 0:
-        points = points + 0.5
-
-    center = np.mean(points,axis=0) # 3D cent point.
-    vectors = points - center # Relative to center
-
-    ex = vectors[0]/np.linalg.norm(vectors[0])  # i
-    ey = np.cross(center,ex)
-    ey = ey/np.linalg.norm(ey)  # j
-
-    angles= []
-    for i, v in enumerate(vectors):
-        vx = np.dot(v,ex)
-        vy = np.dot(v,ey)
-        angle = _tan_inv(vy,vx)
-        angles.append([i,angle])
-
-    s_angs = np.array(angles)
-    ss = s_angs[s_angs[:,1].argsort()] #Sort it.
-
-    if loop: # Add first at end for completing loop.
-        ss = np.concatenate((ss,[ss[0]]))
-
-    return ss[:,0].astype(int) # Order indices.
-
-
-def _out_bz_plane(test_point,plane):
-    """
-    - Returns True if test_point is between plane and origin. Could be used to sample BZ mesh in place of ConvexHull.
-    - **Parameters**
-        - test_points: 3D point.
-        - plane      : List of at least three coplanar 3D points.
-    """
-    outside = True
-    p_test = np.array(test_point)
-    plane = np.unique(plane,axis=0) #Avoid looped shape.
-    c = np.mean(plane,axis=0) #center
-    _dot_ = np.dot(p_test-c,c)
-    if _dot_ < -1e-5:
-        outside = False
-    return outside
-
-
-def _rad_angle(v1,v2):
-    """
-    - Returns interier angle between two vectors.
-    - **Parameters**
-        - v1,v2 : Two vectors/points in 3D.
-    """
-    v1 = np.array(v1)
-    v2 = np.array(v2)
-    norm  = np.linalg.norm(v1)*np.linalg.norm(v2)
-    dot_p = np.round(np.dot(v1,v2)/norm,12)
-    angle = np.arccos(dot_p)
-    return angle
-
-from scipy.spatial.transform import Rotation
-def rotation(angle_deg,axis_vec):
-    """Get a scipy Rotation object at given `angle_deg` around `axis_vec`.
-    Usage:
-        rot = rotation(60,[0,0,1])
-        rot.apply([1,1,1])
-        [-0.3660254  1.3660254  1.] #give this
-    """
-    axis_vec = np.array(axis_vec)/np.linalg.norm(axis_vec) # Normalization
-    angle_rad = np.deg2rad(angle_deg)
-    return Rotation.from_rotvec(angle_rad * axis_vec)
 
 # Cell
-def get_bz(path_pos = None,loop = True,digits=8,primitive=False):
-    """
-    - Return required information to construct first Brillouin zone in form of tuple (basis, normals, vertices, faces).
-    - **Parameters**
-        - path_pos : POSCAR file path or list of 3 Real space vectors in 3D as list[list,list,list].
-        - loop   : If True, joins the last vertex of a BZ plane to starting vertex in order to complete loop.
-        - digits : int, rounding off decimal places, no effect on intermediate calculations, just for pretty final results.
-        - primitive: Defualt is False and returns Wigner-Seitz cell, If True returns parallelipiped in rec_basis.
-
-    - **Attributes**
-        - basis   : get_bz().basis, recprocal lattice basis.
-        - normals : get_bz().normals, all vertors that are perpendicular BZ faces/planes.
-        - vertices: get_bz().vertices, all vertices of BZ, could be input into ConvexHull for constructing 3D BZ.
-        - faces   : get_bz().faces, vertices arranged into faces, could be input to Poly3DCollection of matplotlib for creating BZ from faces' patches.
-        - specials : get_bz().specials, Data with attributes `coords`,`kpoints` and `near` in on-one correspondence for high symmetry KPOINTS in recirprocal coordinates space. `near` gives indices of nearest special points around a vertex. All vertices with z > 0 are included.
-    """
-    basis = _get_basis(path_pos).inverted # Reads
-    b1, b2, b3 = basis # basis are reciprocal basis
-    # Get all vectors for BZ
-    if primitive:
-        b0 = np.array([0,0,0])
-        bd = b1+b2+b3 #Diagonal point
-        faces = np.array([
-                 [b0, b1, b1+b2, b2],
-                 [b0,b2,b2+b3,b3],
-                 [b0,b3,b3+b1,b1],
-                 [b1,b1+b2,b1+b3,bd],
-                 [b2,b2+b1,b2+b3,bd],
-                 [b3,b3+b1,b3+b2,bd]
-                ])
-    else:
-        vectors = []
-        for i,j,k in product([0,1,-1],[0,1,-1],[0,1,-1]):
-            vectors.append(i*b1+j*b2+k*b3)
-        vectors = np.array(vectors)
-        # Generate voronoi diagram
-        vor = Voronoi(vectors)
-        faces = []
-        vrd = vor.ridge_dict
-        for r in vrd:
-            if r[0] == 0 or r[1] == 0:
-                verts_in_face = np.array([vor.vertices[i] for i in vrd[r]])
-                faces.append(verts_in_face)
-        #faces = np.array(faces) # should be a list instead as not regular shape.
-
-    verts = [v for vs in faces for v in vs]
-    verts = np.unique(verts,axis=0)
-
-    face_vectors = []
-    for f in faces:
-        face_vectors.append(np.mean(f,axis=0)) # In primitive point at face center
-    if primitive == False:
-        face_vectors = [2*f for f in face_vectors] # In regular, cross plane as well.
-
-    # Order Faces.
-    faces = [face[order(face,loop=loop)] for face in faces] # order based on given value of loop
-
-    # High symmerty KPOINTS in primitive BZ (positive only)
-    mid_faces = np.array([np.mean(np.unique(face,axis=0),axis=0) for face in faces])
-    mid_edges = []
-    for f in faces:
-        for i in range(len(f)-1):
-            # Do not insert point between unique vertices
-            if np.isclose(np.linalg.norm(f[i]),np.linalg.norm(f[i+1])):
-                mid_edges.append(np.mean([f[i],f[i+1]],axis=0))
-    if mid_edges!=[]:
-        mid_edges = np.unique(mid_edges,axis=0) # because faces share edges
-        mid_faces = np.concatenate([mid_faces,mid_edges])
-    # Bring all high symmetry points together.
-    mid_all = np.concatenate([[[0,0,0]],mid_faces,verts]) # Coords
-    mid_basis_all = np.array([np.linalg.solve(basis.T,v) for v in mid_all]) # Kpoints
-
-    # Round off results
-    mid_all_p    = np.round(mid_all,digits) # Coordinates
-    mid_basis_p  = np.round(mid_basis_all,digits) # Relative points
-    basis        = np.round(basis,digits)
-    face_vectors = np.round(face_vectors,digits)
-    verts        = np.round(verts,digits)
-    faces        = tuple([np.round(face,digits) for face in faces])
-
-    #Order special points near each vertex for z > 0.
-    _arrs = []
-    for v in verts[verts[:,2]>=0]: # Only upper hemisphere.
-        _arr = []
-        for i,c in enumerate(mid_all_p): # coordinates.
-            _arr.append([i, np.linalg.norm(v-c)])
-        _arr = np.array(_arr)
-        _arr = _arr[_arr[:,1].argsort()][:,0].astype(int)
-        upto = np.where(_arr == 0)[0][0]
-        _arrs.append([0,*_arr[:upto]])
-    one2one  = {'coords': mid_all_p ,'kpoints': mid_basis_p,'near': _arrs}
-    out_dict = {'basis':basis, 'normals':face_vectors, 'vertices':verts,
-                'faces':faces,'specials':one2one}
-    return serializer.dict2tuple('BZ',out_dict)
-
-
-# Cell
-def splot_bz(bz_data, ax = None, plane=None,color='blue',fill=True,vectors=True,v3=False,vname='b',colormap='plasma',light_from=(1,1,1),alpha=0.4):
-    """
-    - Plots matplotlib's static figure.
-    - **Parameters**
-        - bz_data    : Output of `get_bz`.
-        - fill       : True by defult, determines whether to fill surface of BZ or not.
-        - color      : color to fill surface and stroke color.
-        - vectors    : Plots basis vectors, default is True.
-        - v3         : Plots 3rd vector as well. Only works in 2D and when `vectors=True`.
-        - plane      : Default is None and plots 3D surface. Can take 'xy','yz','zx' to plot in 2D.
-        - ax         : Auto generated by default, 2D/3D axes, auto converts in 3D on demand as well.
-        - vname      : Default is `b` for reciprocal space, can set `a` for plotting cell as after `get_bz(get_bz().basis)` you get real space lattice back if `primitive=True` both times.
-        - colormap  : If None, single color is applied, only works in 3D and `fill=True`. Colormap is applied along z.
-        - light_from: Point from where light is thrown on BZ planes, default is (1,1,1). Only works on plane in 3D.
-        - alpha    : Opacity of filling in range [0,1]. Increase for clear viewpoint.
-    - **Returns**
-        - ax   : Matplotlib's 2D axes if `plane=None`.
-        - ax3d : Matplotlib's 2D axes if `plane` is given.
-
-    > Tip: `splot_bz(rec_basis,primitive=True)` will plot cell in real space.
-    """
-    label = r"$k_{}$" if vname=='b' else "{}"
-    if not ax: #For both 3D and 2D, initialize 2D axis.
-        ax = sp.get_axes(figsize=(3.4,3.4)) #For better display
-
-    _label = r'\vec{}'.format(vname) # For both
-
-    valid_planes = 'xyzxzyx' # cylic
-    if plane and plane not in valid_planes:
-        raise ValueError(f"`plane` expects value in 'xyzxzyx' or None, got {plane!r}")
-    elif plane and plane in valid_planes: #Project 2D
-        faces = bz_data.faces
-        ind = valid_planes.index(plane)
-        arr = [0,1,2,0,2,1,0]
-        i, j = arr[ind], arr[ind+1]
-        _ = [ax.plot(f[:,i],f[:,j],color=(color),lw=0.7) for f in faces]
+def splot_bz(
+    bz_data,
+    plane=None,
+    ax=None,
+    color="blue",
+    fill=True,
+    vectors=(0, 1, 2),
+    colormap=None,
+    shade=True,
+    alpha=0.4,
+    zoffset=0,
+    **kwargs,
+):
+    """Plots matplotlib's static figure of Brillouin zone. You can also plot in 2D on a 3D axes.
+
+    Parameters
+    ----------
+    bz_data : Output of `get_bz`.
+    plane : str
+        Default is None and plots 3D surface. Can take 'xy','yz','zx' to plot in 2D.
+    fill : bool
+        True by defult, determines whether to fill surface of BZ or not.
+    color : Any
+        Color to fill surface and stroke color. Default is 'blue'. Can be any valid matplotlib color.
+    vectors : tuple
+        Tuple of indices of basis vectors to plot. Default is (0,1,2). All three are plotted in 3D
+        (you can turn of by None or empty tuple), whhile you can specify any two/three in 2D.
+    ax : matplotlib.pyplot.Axes
+        Auto generated by default, 2D/3D axes, auto converts in 3D on demand as well.
+    colormap : str
+        If None, single color is applied, only works in 3D and `fill=True`. Colormap is applied along z.
+    shade : bool
+        Shade polygons or not. Only works in 3D and `fill=True`.
+    alpha : float
+        Opacity of filling in range [0,1]. Increase for clear viewpoint.
+    zoffset : float
+        Only used if plotting in 2D over a 3D axis. Default is 0. Any plane 'xy','yz' etc.
+
+
+    kwargs are passed to `plt.plot` or `Poly3DCollection` if `fill=True`.
+
+    Returns
+    -------
+    matplotlib.pyplot.Axes
+        Matplotlib's 2D axes if `plane=None` otherswise 3D axes.
+    """
+    vname = "a" if bz_data.__class__.__name__ == "CellData" else "b"
+    label = r"$k_{}/2π$" if vname == "b" else "{}"
+    if not ax:  # For both 3D and 2D, initialize 2D axis.
+        ax = ptk.get_axes(figsize=(3.4, 3.4))  # For better display
+
+    _label = r"\vec{" + vname + "}"  # For both
+
+    if vectors and not isinstance(vectors, (tuple, list)):
+        raise ValueError(f"`vectors` expects tuple or list, got {vectors!r}")
+
+    if vectors is None:
+        vectors = ()  # Empty tuple to make things work below
+
+    for v in vectors:
+        if v not in [0, 1, 2]:
+            raise ValueError(f"`vectors` expects values in [0,1,2], got {vectors!r}")
+
+    name = kwargs.pop("label", None)  # will set only on single line
+    kwargs.pop("zdir", None)  # 2D plot on 3D axes is only supported in xy plane.
+
+    if plane:  # Project 2D, works on 3D axes as well
+        kwargs = {"solid_capstyle": "round", **kwargs}
+        is3d = getattr(ax, "name", "") == "3d"
+        normals = {
+            "xy": (0, 0, 1),
+            "yz": (1, 0, 0),
+            "zx": (0, 1, 0),
+            "yx": (0, 0, -1),
+            "zy": (-1, 0, 0),
+            "xz": (0, -1, 0),
+        }
+        if plane not in normals:
+            raise ValueError(
+                f"`plane` expects value in 'xyzxzyx' or None, got {plane!r}"
+            )
+
+        z0 = (
+            [0, 0, zoffset]
+            if plane in "xyx"
+            else [0, zoffset, 0]
+            if plane in "xzx"
+            else [zoffset, 0, 0]
+        )
+        idxs = {
+            "xy": [0, 1],
+            "yz": [1, 2],
+            "zx": [2, 0],
+            "yx": [1, 0],
+            "zy": [2, 1],
+            "xz": [0, 2],
+        }
+        for idx, f in enumerate(bz_data.faces_coords):
+            g = to_plane(normals[plane], f) + z0
+            (line,) = ax.plot(
+                *(g.T if is3d else g[:, idxs[plane]].T), color=color, **kwargs
+            )
+            if idx == 0:
+                line.set_label(name)  # only one line
 
         if vectors:
-            if v3:
-                s_basis = bz_data.basis
-                ijk = [0,1,2]
-            else:
-                s_basis = bz_data.basis[[i,j]]# Only two.
-                ijk = [i,j]
+            s_basis = to_plane(normals[plane], bz_data.basis[(vectors,)])
 
-            for k,y in zip(ijk,s_basis):
-                l = "\n" + r" ${}_{}$".format(_label,k+1)
-                ax.text(0.8*y[i],0.8*y[j], l, va='center',ha='left')
-                ax.scatter([y[i]],[y[j]],color='w',s=0.0005) # Must be to scale below arrow.
-
-            s_zero = [0 for s_b in s_basis] # either 3 or 2.
-            ax.quiver(s_zero,s_zero,*s_basis.T[[i,j]],lw=0.9,color='k',angles='xy', scale_units='xy', scale=1)
-
-        ax.set_xlabel(label.format(valid_planes[i]))
-        ax.set_ylabel(label.format(valid_planes[j]))
-        ax.set_aspect(1) # Must for 2D axes to show actual lengths of BZ
+            for k, b in zip(vectors, s_basis):
+                x, y = b[idxs[plane]]
+                l = r" ${}_{} $".format(_label, k + 1)
+                l = l + "\n" if y < 0 else "\n" + l
+                ha = "right" if x < 0 else "left"
+                xyz = 0.8 * b + z0 if is3d else np.array([0.8 * x, 0.8 * y])
+                ax.text(
+                    *xyz, l, va="center", ha=ha, clip_on=True
+                )  # must clip to have limits of axes working.
+                ax.scatter(
+                    *(xyz / 0.8), color="w", s=0.0005
+                )  # Must be to scale below arrow.
+            if is3d:
+                XYZ, UVW = (np.ones_like(s_basis) * z0).T, s_basis.T
+                quiver3d(
+                    *XYZ, *UVW, C="k", L=0.7, ax=ax, arrowstyle="-|>", mutation_scale=7
+                )
+            else:
+                s_zero = [0 for _ in s_basis]  # either 3 or 2.
+                ax.quiver(
+                    s_zero,
+                    s_zero,
+                    *s_basis[:, idxs[plane]].T,
+                    lw=0.9,
+                    color="navy",
+                    angles="xy",
+                    scale_units="xy",
+                    scale=1,
+                )
+
+        ax.set_xlabel(label.format(idxs[plane][0]))
+        ax.set_ylabel(label.format(idxs[plane][1]))
+        if is3d:
+            ind = [i for i in range(3) if i not in idxs[plane]][0]
+            ax.set_zlabel(label.format(ind))
+            ax.set_aspect("equal")
+            zmin, zmax = ax.get_zlim()
+            if zoffset > zmax:
+                zmax = zoffset
+            elif zoffset < zmin:
+                zmin = zoffset
+            ax.set_zlim([zmin, zmax])
+        else:
+            ax.set_aspect("equal")  # Must for 2D axes to show actual lengths of BZ
         return ax
-    else: # Plot 3D
-        if ax and ax.name == "3d":
+    else:  # Plot 3D
+        if getattr(ax, "name", "") == "3d":  # handle None or 2D axes passed.
             ax3d = ax
         else:
             pos = ax.get_position()
             fig = ax.get_figure()
             ax.remove()
-            ax3d = fig.add_axes(pos,projection='3d',azim=45,elev=30,proj_type='ortho')
+            ax3d = fig.add_axes(
+                pos, projection="3d", azim=45, elev=30, proj_type="ortho"
+            )
 
         if fill:
             if colormap:
-                colormap = colormap if colormap in plt.colormaps() else 'viridis'
-                cz = [np.mean(np.unique(f,axis=0),axis=0)[2] for f in bz_data.faces]
-                levels = (cz - np.min(cz))/np.ptp(cz) # along Z.
+                colormap = colormap if colormap in plt.colormaps() else "viridis"
+                cz = [
+                    np.mean(np.unique(f, axis=0), axis=0)[2]
+                    for f in bz_data.faces_coords
+                ]
+                levels = (cz - np.min(cz)) / np.ptp(cz)  # along Z.
                 colors = plt.cm.get_cmap(colormap)(levels)
             else:
-                colors = np.array([[*mplc.to_rgb(color)] for f in bz_data.faces]) # Single color.
-            if light_from:
-                intensity = bz_data.normals.dot(light_from) #Plane facing light
-                intensity = (intensity - np.min(intensity) + 0.2)/np.ptp(intensity)
-                intensity = intensity.clip(0,1)
-                colors = np.array([i*c[:3] for i, c in zip(intensity,colors)])
+                colors = np.array(
+                    [[*mplc.to_rgb(color)] for f in bz_data.faces_coords]
+                )  # Single color.
+
+            poly = Poly3DCollection(
+                bz_data.faces_coords,
+                edgecolors=[
+                    color,
+                ],
+                facecolors=colors,
+                alpha=alpha,
+                shade=shade,
+                label=name,
+                **kwargs,
+            )
 
-            poly = Poly3DCollection(bz_data.faces,edgecolors=[color,],facecolors=colors, alpha=alpha)
-            ax3d.add_collection3d(poly)
+            ax3d.add_collection(poly)
             ax3d.autoscale_view()
         else:
-            _ = [ax3d.plot3D(f[:,0],f[:,1],f[:,2],color=(color),lw=0.7) for f in bz_data.faces]
+            kwargs = {"solid_capstyle": "round", **kwargs}
+            (line,) = [
+                ax3d.plot3D(f[:, 0], f[:, 1], f[:, 2], color=(color), **kwargs)
+                for f in bz_data.faces_coords
+            ][0]
+            line.set_label(name)  # only one line
 
         if vectors:
-            for k,v in enumerate(0.35*bz_data.basis):
-                ax3d.text(*v,r"${}_{}$".format(_label,k+1),va='center',ha='center')
-
-            XYZ,UVW = [[0,0,0],[0,0,0],[0,0,0]], 0.3*bz_data.basis.T
-            fancy_quiver3d(*XYZ,*UVW,C='k',L=0.7,ax=ax3d,arrowstyle="-|>",mutation_scale=7)
-
-        l_ = np.min(bz_data.vertices,axis=0)
-        h_ = np.max(bz_data.vertices,axis=0)
-        ax3d.set_xlim([l_[0],h_[0]])
-        ax3d.set_ylim([l_[1],h_[1]])
-        ax3d.set_zlim([l_[2],h_[2]])
+            for k, v in enumerate(0.35 * bz_data.basis):
+                ax3d.text(
+                    *v, r"${}_{}$".format(_label, k + 1), va="center", ha="center"
+                )
+
+            XYZ, UVW = [[0, 0, 0], [0, 0, 0], [0, 0, 0]], 0.3 * bz_data.basis.T
+            quiver3d(
+                *XYZ, *UVW, C="k", L=0.7, ax=ax3d, arrowstyle="-|>", mutation_scale=7
+            )
+
+        l_ = np.min(bz_data.vertices, axis=0)
+        h_ = np.max(bz_data.vertices, axis=0)
+        ax3d.set_xlim([l_[0], h_[0]])
+        ax3d.set_ylim([l_[1], h_[1]])
+        ax3d.set_zlim([l_[2], h_[2]])
 
         # Set aspect to same as data.
-        ax3d.set_box_aspect(np.ptp(bz_data.vertices,axis=0))
+        ax3d.set_box_aspect(np.ptp(bz_data.vertices, axis=0))
 
-        ax3d.set_xlabel(label.format('x'))
-        ax3d.set_ylabel(label.format('y'))
-        ax3d.set_zlabel(label.format('z'))
+        ax3d.set_xlabel(label.format("x"))
+        ax3d.set_ylabel(label.format("y"))
+        ax3d.set_zlabel(label.format("z"))
         return ax3d
 
-# Cell
-def iplot_bz(bz_data,fill = True,color = 'rgba(168,204,216,0.4)',background = 'rgb(255,255,255)',vname = 'b', special_kpoints = True, alpha=0.4,ortho3d=True,fig=None):
-    """
-    - Plots interactive figure showing axes,BZ surface, special points and basis, each of which could be hidden or shown.
-    - **Parameters**
-        - bz_data    : Output of `get_bz`.
-        - fill       : True by defult, determines whether to fill surface of BZ or not.
-        - color      : color to fill surface 'rgba(168,204,216,0.4)` by default.
-        - background : Plot background color, default is 'rgb(255,255,255)'.
-        - vname      : Default is `b` for reciprocal space, can set `a` for plotting cell as after `get_bz(get_bz().basis)` you get real space lattice back if `primitive=True` both times.
-        - special_kpoints : True by default, determines whether to plot special points or not.
-        - alpha      : Opacity of BZ planes.
-        - ortho3d    : Default is True, decides whether x,y,z are orthogonal or perspective.
-        - fig        : (Optional) Plotly's `go.Figure`. If you want to plot on another plotly's figure, provide that.
-    - **Returns**
-        - fig   : plotly.graph_object's Figure instance.
 
-    > Tip: `iplot_bz(rec_basis,primitive=True)` will plot cell in real space.
+# Cell
+def iplot_bz(
+    bz_data,
+    fill=False,
+    color="rgba(168,204,216,0.8)",
+    special_kpoints=True,
+    alpha=0.4,
+    ortho3d=True,
+    fig=None,
+    **kwargs,
+):
+    """Plots interactive figure showing axes,BZ surface, special points and basis, each of which could be hidden or shown.
+
+    Parameters
+    ----------
+    bz_data : Output of `get_bz`.
+    fill : bool
+        False by defult, determines whether to fill surface of BZ or not.
+    color : str
+        Color to fill surface 'rgba(168,204,216,0.4)` by default. This sholud be a valid Plotly color.
+    special_kpoints : bool or callable
+        True by default, determines whether to plot special points or not.
+        You can also proivide a mask function f(x,y,z) -> bool which will be used to filter special points based on their fractional coordinates.
+    alpha : float
+        Opacity of BZ planes.
+    ortho3d : bool
+        Default is True, decides whether x,y,z are orthogonal or perspective.
+    fig : plotly.graph_objects.Figure
+        Plotly's `go.Figure`. If you want to plot on another plotly's figure, provide that.
+
+
+    kwargs are passed to `plotly.graph_objects.Scatter3d` for BZ lines.
+
+    Returns
+    -------
+    plotly.graph_objects.Figure
     """
     if not fig:
         fig = go.Figure()
     # Name fixing
-    axes_text = ["<b>k</b><sub>x</sub>","","<b>k</b><sub>y</sub>","","<b>k</b><sub>z</sub>"]
-    s_name = 'BZ'
-    a_name = 'Axes'
-    if vname == 'a':
-        axes_text = ["<b>x</b>","","<b>y</b>","","<b>z</b>"] # Real space
-        s_name = 'Lattice'
-        a_name = 'RealAxes'
+    vname = "a" if bz_data.__class__.__name__ == "CellData" else "b"
+    axes_text = [
+        "<b>k</b><sub>x</sub>/2π",
+        "",
+        "<b>k</b><sub>y</sub>/2π",
+        "",
+        "<b>k</b><sub>z</sub>/2π",
+    ]
+    if vname == "a":
+        axes_text = ["<b>x</b>", "", "<b>y</b>", "", "<b>z</b>"]  # Real space
 
+    zone_name = kwargs.pop("name", "BZ" if vname == "b" else "Lattice")
     # Axes
-    _len = 0.5*np.mean(bz_data.basis)
-    fig.add_trace(go.Scatter3d(x=[_len,0,0,0,0],y=[0,0,_len,0,0],z=[0,0,0,0,_len],
-        mode='lines+text',
-        text= axes_text,
-        line_color='green', legendgroup=a_name,name=a_name))
-    fig.add_trace(go.Cone(x=[0.95*_len,0,0],y=[0,0.95*_len,0],z=[0,0,0.95*_len],
-        u=[0.2*_len,0,0],v=[0,0.2*_len,0],w=[0,0,0.2*_len],showscale=False,
-        colorscale='Greens',legendgroup=a_name,name=a_name))
+    _len = 0.5 * np.mean(bz_data.basis)
+    fig.add_trace(
+        go.Scatter3d(
+            x=[_len, 0, 0, 0, 0],
+            y=[0, 0, _len, 0, 0],
+            z=[0, 0, 0, 0, _len],
+            mode="lines+text",
+            text=axes_text,
+            line_color="skyblue",
+            legendgroup="Axes",
+            name="Axes",
+        )
+    )
+    fig.add_trace(
+        go.Cone(
+            x=[_len, 0, 0],
+            y=[0, _len, 0],
+            z=[0, 0, _len],
+            u=[1, 0, 0],
+            v=[0, 1, 0],
+            w=[0, 0, 1],
+            showscale=False,
+            sizemode="absolute",
+            sizeref=0.5,
+            anchor="tail",
+            colorscale=["skyblue" for _ in range(3)],
+            legendgroup="Axes",
+            name="Axes",
+        )
+    )
+
     # Basis
-    for i,b in enumerate(bz_data.basis):
-        fig.add_trace(go.Scatter3d(x=[0,b[0]], y=[0,b[1]],z=[0,b[2]],
-            mode='lines+text',legendgroup="{}<sub>{}</sub>".format(vname,i+1), line_color='red',
-            name="<b>{}</b><sub>{}</sub>".format(vname,i+1),text=["","<b>{}</b><sub>{}</sub>".format(vname,i+1)]))
-        fig.add_trace(go.Cone(x=[0.95*b[0]],y=[0.95*b[1]],z=[0.95*b[2]],
-            u=[0.2*b[0]],v=[0.2*b[1]],w=[0.2*b  [2]],showscale=False,colorscale='Reds',
-            legendgroup="{}<sub>{}</sub>".format(vname,i+1),name="<b>{}</b><sub>{}</sub>".format(vname,i+1)))
+    for i, b in enumerate(bz_data.basis):
+        fig.add_trace(
+            go.Scatter3d(
+                x=[0, b[0]],
+                y=[0, b[1]],
+                z=[0, b[2]],
+                mode="lines+text",
+                legendgroup="{}<sub>{}</sub>".format(vname, i + 1),
+                line_color="red",
+                name="<b>{}</b><sub>{}</sub>".format(vname, i + 1),
+                text=["", "<b>{}</b><sub>{}</sub>".format(vname, i + 1)],
+            )
+        )
+
+        uvw = b / np.linalg.norm(b)  # Unit vector for cones
+        fig.add_trace(
+            go.Cone(
+                x=[b[0]],
+                y=[b[1]],
+                z=[b[2]],
+                u=uvw[0:1],
+                v=uvw[1:2],
+                w=uvw[2:],
+                showscale=False,
+                colorscale="Reds",
+                sizemode="absolute",
+                sizeref=0.02,
+                anchor="tail",
+                legendgroup="{}<sub>{}</sub>".format(vname, i + 1),
+                name="<b>{}</b><sub>{}</sub>".format(vname, i + 1),
+            )
+        )
 
     # Faces
     legend = True
-    for pts in bz_data.faces:
-        fig.add_trace(go.Scatter3d(x=pts[:,0], y=pts[:,1],z=pts[:,2],
-            mode='lines',line_color=color, legendgroup=s_name,name=s_name,
-            showlegend=legend))
-        legend = False # Only first legend to show for all
+    for pts in bz_data.faces_coords:
+        fig.add_trace(
+            go.Scatter3d(
+                x=pts[:, 0],
+                y=pts[:, 1],
+                z=pts[:, 2],
+                mode="lines",
+                line_color=color,
+                legendgroup=zone_name,
+                name=zone_name,
+                showlegend=legend,
+                **kwargs,
+            )
+        )
+
+        legend = False  # Only first legend to show for all
 
     if fill:
         xc = bz_data.vertices[ConvexHull(bz_data.vertices).vertices]
-        fig.add_trace(go.Mesh3d(x=xc[:, 0], y=xc[:, 1], z=xc[:, 2],
-                        color=color,
-                        opacity=alpha,
-                        alphahull=0,
-                        lighting=dict(diffuse=0.5),
-                        legendgroup=s_name,name=s_name))
+        fig.add_trace(
+            go.Mesh3d(
+                x=xc[:, 0],
+                y=xc[:, 1],
+                z=xc[:, 2],
+                color=color,
+                opacity=alpha,
+                alphahull=0,
+                lighting=dict(diffuse=0.5),
+                legendgroup=zone_name,
+                name=zone_name,
+            )
+        )
 
     # Special Points only if in reciprocal space.
-    if vname == 'b' and special_kpoints:
-        texts,values =[],[]
-        norms = np.round(np.linalg.norm(bz_data.specials.coords,axis=1),5)
-        sps = bz_data.specials
-        for key,value, (i,norm) in zip(sps.kpoints, sps.coords, enumerate(norms)):
-            texts.append("P{}</br>d = {}</br> Index = {}".format(key,norm,i))
-            values.append([[*value,norm]])
-
-        values = np.array(values).reshape((-1,4))
-        norm_max = np.max(values[:,3])
-        c_vals = np.array([int(v*255/norm_max) for v in values[:,3]])
+    if vname == "b" and special_kpoints:
+        if callable(special_kpoints):
+            skpts = bz_data.specials.masked(special_kpoints)
+        else:
+            skpts = bz_data.specials
+
+        for tr in fig.data:  # hide all traces hover made before
+            tr.hoverinfo = "none"  # avoid overlapping with special points
+
+        texts, values = [], []
+        norms = np.round(np.linalg.norm(skpts.coords, axis=1), 8)
+        for key, value, norm in zip(skpts.kpoints.round(6), skpts.coords, norms):
+            texts.append("K = {}</br>d = {}".format(key, norm))
+            values.append([[*value, norm]])
+
+        values = np.array(values).reshape((-1, 4))
+        norm_max = np.max(values[:, 3])
+        c_vals = np.array([int(v * 255 / norm_max) for v in values[:, 3]])
         colors = [0 for i in c_vals]
         _unique = np.unique(np.sort(c_vals))[::-1]
-        _lnp = np.linspace(0,255,len(_unique)-1)
-        _u_colors = ["rgb({},0,{})".format(r,b) for b,r in zip(_lnp,_lnp[::-1])]
-        for _un,_uc in zip(_unique[:-1],_u_colors):
+        _lnp = np.linspace(0, 255, len(_unique) - 1)
+        _u_colors = ["rgb({},0,{})".format(r, b) for b, r in zip(_lnp, _lnp[::-1])]
+        for _un, _uc in zip(_unique[:-1], _u_colors):
             _index = np.where(c_vals == _un)[0]
             for _ind in _index:
-                colors[_ind]=_uc
+                colors[_ind] = _uc
 
-        colors[0]= "rgb(255,215,0)" # Gold color at Gamma!.
-        fig.add_trace(go.Scatter3d(x=values[:,0], y=values[:,1],z=values[:,2],
-                hovertext=texts,name="HSK",marker=dict(color=colors,size=4),mode='markers'))
-    proj = dict(projection=dict(type = "orthographic")) if ortho3d else {}
-    camera = dict(center=dict(x=0.1, y=0.1, z=0.1),**proj)
-    fig.update_layout(scene_camera=camera,paper_bgcolor=background, plot_bgcolor=background,
-        font_family="Times New Roman",font_size= 14,
-        scene = dict(aspectmode='data',xaxis = dict(showbackground=False,visible=False),
-                        yaxis = dict(showbackground=False,visible=False),
-                        zaxis = dict(showbackground=False,visible=False)),
-                        margin=dict(r=10, l=10,b=10, t=30))
+        colors[0] = "rgb(255,215,0)"  # Gold color at Gamma!.
+        fig.add_trace(
+            go.Scatter3d(
+                x=values[:, 0],
+                y=values[:, 1],
+                z=values[:, 2],
+                hovertext=texts,
+                name="HSK",
+                marker=dict(color=colors, size=4),
+                mode="markers",
+            )
+        )
+
+    proj = dict(projection=dict(type="orthographic")) if ortho3d else {}
+    camera = dict(center=dict(x=0.1, y=0.1, z=0.1), **proj)
+    fig.update_layout(
+        template="plotly_white",
+        scene_camera=camera,
+        font_family="Times New Roman",
+        font_size=14,
+        scene=dict(
+            aspectmode="data",
+            xaxis=dict(showbackground=False, visible=False),
+            yaxis=dict(showbackground=False, visible=False),
+            zaxis=dict(showbackground=False, visible=False),
+        ),
+        margin=dict(r=10, l=10, b=10, t=30),
+    )
     return fig
 
-# Cell
-def to_R3(basis,points):
-    """Transforms coordinates of points (relative to non-othogonal basis) into orthogonal space.
-    - **Parameters**
-        - basis : Non-orthogonal basis of real or reciprocal space.
-        - points: 3D points relative to basis, such as KPOINTS and Lattice Points.
-
-    **Note**: Do not use this function if points are Cartesian or provide identity basis.
-    """
-    rec_basis = np.array(basis)
-    points = np.array(points)
-    # Formula to make coordinates from relative points.
-    # kx, ky, kz = n1*b1 + n2*b2 +n3*b3
-    #            = [n1, n2, n3].dot(rec_basis)
-    coords = points.dot(rec_basis)
-    return coords
-
-def to_basis(basis,coords):
-    """Transforms coordinates of points (relative to othogonal basis) into basis space.
-    - **Parameters**
-        - basis : Non-orthogonal basis of real or reciprocal space.
-        - points: 3D points relative to cartesian axes, such as KPOINTS and Lattice Points.
-    """
-    return np.dot(np.linalg.inv(basis).T,coords.T).T
-
-# Cell
-def kpoints2bz(bz_data,kpoints,sys_info = None, primitive=False, shift = 0):
-    """Brings KPOINTS inside BZ. Applies `to_R3` only if `primitive=True`.
-    - **Parameters**
-        - bz_data  : Output of get_bz(), make sure use same value of `primitive` there and here.
-        - kpoints  : List or array of KPOINTS to transorm into BZ or R3.
-        - sys_info : If given, returns kpoints using that information. Useful If kpoints are cartesian and you need to scale those.
-        - primitive: Default is False and brings kpoints into regular BZ. If True, returns `to_R3()`.
-        - shift    : This value is added to kpoints before any other operation, single number of list of 3 numbers for each direction.
-
-    **Note**: If kpoints are Cartesian, provide sys_info, otherwise it will go wrong.
-    """
-    kpoints = np.array(kpoints) + shift
-    if sys_info is not None:
-        if sys_info.space_info.cartesian_kpoints:
-            return to_R3(bz_data.basis,kpoints) # Already relative to basis of BZ
-
-    if primitive:
-        return to_R3(bz_data.basis,kpoints)
-
-    cent_planes = [np.mean(np.unique(face,axis=0),axis=0) for face in bz_data.faces]
-
-    out_coords = np.empty(np.shape(kpoints)) # To store back
-
-    def inside(coord,cent_planes):
-        _dots_ = np.max([np.dot(coord-c, c) for c in cent_planes]) #max in all planes
-        #print(_dots_)
-        if np.max(_dots_) > 1e-8: # Outside
-            return [] # empty for comparison
-        else: # Inside
-            return list(coord) # Must be in list form
-
-
-    from itertools import product
-    for i,p in enumerate(kpoints):
-        for q in product([0,1,-1],[0,1,-1],[0,1,-1]):
-            # First translate, then make coords, then feed it back
-            #print(q)
-            pos = to_R3(bz_data.basis, p + np.array(q))
-            r = inside(pos,cent_planes)
-            if r:
-                #print(p,'-->',r)
-                out_coords[i] = r
-                StopIteration
-
-    return out_coords # These may have duplicates, apply np.unique(out_coords,axis=0). do this in surface plots
 
 # Cell
-def fix_sites(poscar_data,tol=1e-2,eqv_sites=False,translate=None):
+def _fix_sites(poscar_data, tol=1e-2, eqv_sites=False, translate=None):
     """Add equivalent sites to make a full data shape of lattice. Returns same data after fixing.
-    - **Parameters**
-        - poscar_data: Output of `export_poscar` or `export_vasprun().poscar`.
-        - tol   : Tolerance value. Default is 0.01.
-        - eqv_sites: If True, add sites on edges and faces. If False, just fix coordinates, i.e. `pos > 1 - tol -> pos - 1`, useful for merging poscars to make slabs.
-        - translate: A number(+/-) or list of three numbers to translate in a,b,c directions.
-    """
-    pos = poscar_data.positions.copy() # We can also do poscar_data.copy().positions that copies all contents.
-    labels = poscar_data.labels
-    out_dict = poscar_data.to_dict() # For output
+    It should not be exposed mostly be used in visualizations"""
+    pos = (
+        poscar_data.positions.copy()
+    )  # We can also do poscar_data.copy().positions that copies all contents.
+    labels = np.array(poscar_data.labels)  # We need to store equivalent labels as well
+    out_dict = poscar_data.to_dict()  # For output
 
-    if translate and isinstance(translate,(int,float)):
-        pos = pos + (translate - int(translate)) # Only translate in 0 - 1
+    if translate and isinstance(translate, (int, np.integer, float)):
+        pos = pos + (translate - int(translate))  # Only translate in 0 - 1
     elif translate and len(translate) == 3:
         txyz = np.array([translate])
         pos = pos + (txyz - txyz.astype(int))
 
     # Fix coordinates of sites distributed on edges and faces
-    pos -= (pos > (1 - tol)).astype(int) # Move towards orign for common fixing like in joining POSCARs
-    out_dict['positions'] = pos
-    out_dict['extra_info']['comment'] = 'Modified by ipyvasp'
+    pos -= (pos > (1 - tol)).astype(
+        int
+    )  # Move towards orign for common fixing like in joining POSCARs
+    out_dict["positions"] = pos
+    out_dict["metadata"]["comment"] = "Modified by ipyvasp"
 
     # Add equivalent sites on edges and faces if given,handle each sepecies separately
     if eqv_sites:
         new_dict, start = {}, 0
-        for k,v in out_dict['unique'].items():
+        for k, v in out_dict["types"].items():
             vpos = pos[v]
-            pos_x = vpos[((vpos[:,0] + 1) < (tol +1))] + [[1,0,0]] # Add 1 to x if within tol
-            pos_y = vpos[((vpos[:,1] + 1) < (tol +1))] + [[0,1,0]] # Add 1 to y on modified and if within tol
-            pos_z = vpos[((vpos[:,2] + 1) < (tol +1))] + [[0,0,1]] # Add 1 to z and if within tol
-            pos_xy = vpos[((vpos[:,0:2] + 1) < (tol +1)).all(axis = 1)] + [[1,1,0]] # Add 1 to x and y and if within tol
-            pos_yz = vpos[((vpos[:,1:3] + 1) < (tol +1)).all(axis = 1)] + [[0,1,1]] # Add 1 to y and z and if within tol
-            pos_zx = vpos[((vpos[:,[0,2]] + 1) < (tol +1)).all(axis = 1)] + [[1,0,1]] # Add 1 to z and x and if within tol
-            pos_xyz = vpos[((vpos + 1) < (tol +1)).all(axis=1)] + [[1,1,1]] # Add 1 to x,y,z and if within tol
-            new_dict[k] = {'pos':np.vstack([vpos,pos_x,pos_y,pos_z,pos_xy,pos_yz,pos_zx,pos_xyz])}
-            new_dict[k]['range'] = range(start,start+len(new_dict[k]['pos']))
-            start += len(new_dict[k]['pos'])
-
-        out_dict['positions'] = np.vstack([new_dict[k]['pos'] for k in new_dict.keys()])
-        out_dict['unique'] = {k:new_dict[k]['range'] for k in new_dict.keys()}
+            vlabs = labels[v]
+            inds = np.array(v)
+            cond_ops = [
+                (
+                    ((vpos[:, 0] + 1) < (tol + 1)),
+                    [[1, 0, 0]],
+                ),  # Add 1 to x if within tol
+                (
+                    ((vpos[:, 1] + 1) < (tol + 1)),
+                    [[0, 1, 0]],
+                ),  # Add 1 to y on modified and if within tol
+                (
+                    ((vpos[:, 2] + 1) < (tol + 1)),
+                    [[0, 0, 1]],
+                ),  # Add 1 to z and if within tol
+                (
+                    ((vpos[:, 0:2] + 1) < (tol + 1)).all(axis=1),
+                    [[1, 1, 0]],
+                ),  # Add 1 to x and y if within tol
+                (
+                    ((vpos[:, 1:3] + 1) < (tol + 1)).all(axis=1),
+                    [[0, 1, 1]],
+                ),  # Add 1 to y and z if within tol
+                (
+                    ((vpos[:, [0, 2]] + 1) < (tol + 1)).all(axis=1),
+                    [[1, 0, 1]],
+                ),  # Add 1 to x and z if within tol
+                (
+                    ((vpos + 1) < (tol + 1)).all(axis=1),
+                    [[1, 1, 1]],
+                ),  # Add 1 to all if within tol
+            ]
+            spos = [vpos[c] + op for c, op in cond_ops]
+            slab = [vlabs[c] for c, op in cond_ops]
+            sinds = [inds[c] for c, op in cond_ops]
+
+            new_dict[k] = {
+                "pos": np.vstack([vpos, *spos]),
+                "lab": np.hstack([vlabs, *slab]),
+                "inds": np.hstack([inds, *sinds]),
+            }
+            new_dict[k]["range"] = range(start, start + len(new_dict[k]["pos"]))
+            start += len(new_dict[k]["pos"])
+
+        out_dict["positions"] = np.vstack([new_dict[k]["pos"] for k in new_dict.keys()])
+        out_dict["metadata"]["eqv_labels"] = np.hstack(
+            [new_dict[k]["lab"] for k in new_dict.keys()]
+        )
+
+        out_dict["metadata"]["eqv_indices"] = np.hstack(
+            [new_dict[k]["inds"] for k in new_dict.keys()]
+        )
+        out_dict["types"] = {k: new_dict[k]["range"] for k in new_dict.keys()}
 
     return serializer.PoscarData(out_dict)
 
+
 def translate_poscar(poscar_data, offset):
-    """ Translate sites of a PPSCAR. Usully a farction of integarers like 1/2,1/4 etc.
-    - **Parameters**
-        - poscar_data: Output of `export_poscar` or `export_vasprun().poscar`.
-        - offset: A number(+/-) or list of three numbers to translate in a,b,c directions.
-    """
-    return fix_sites(poscar_data, translate = offset, eqv_sites=False)
+    """Translate sites of a POSCAR with a given offset as a number or list of three number.
+    Usully a farction of integarers like 1/2,1/4 etc."""
+    return _fix_sites(poscar_data, translate=offset, eqv_sites=False)
 
-def get_pairs(poscar_data, positions, r, tol=1e-3):
+
+def get_pairs(basis, positions, r, tol=1e-3):
     """Returns a tuple of Lattice (coords,pairs), so coords[pairs] given nearest site bonds.
-    - **Parameters**
-        - poscar_data: Output of `export_poscar` or `export_vasprun().poscar`.
-        - positions: Array(N,3) of fractional positions of lattice sites. If coordinates positions, provide unity basis.
-        - r        : Cartesian distance between the pairs in units of Angstrom e.g. 1.2 -> 1.2E-10.
-        - tol      : Tolerance value. Default is 10^-3.
+
+    Parameters
+    ----------
+    basis : array_like
+        3x3 array of lattice basis vectors in rows.
+    positions : array_like
+        Array(N,3) of fractional positions of lattice sites. If coordinates positions, provide unity basis.
+    r : float
+        Cartesian distance between the pairs in units of Angstrom e.g. 1.2 -> 1.2E-10.
+    tol : float
+        Tolerance value. Default is 10^-3.
     """
-    basis = np.identity(3) if poscar_data.extra_info.cartesian else poscar_data.basis
-    coords = to_R3(basis,positions)
+    coords = to_R3(basis, positions)
     tree = KDTree(coords)
-    inds = np.array([[*p] for p in tree.query_pairs(r,eps=tol)])
-    return serializer.dict2tuple('Lattice',{'coords':coords,'pairs':inds})
+    inds = np.array([[*p] for p in tree.query_pairs(r, eps=tol)])
+    return serializer.dict2tuple("Lattice", {"coords": coords, "pairs": inds})
+
 
-def _get_bond_length(poscar_data,given=None,tol=1e-3):
-    "tol is add to calculated bond length in order to fix small differences, paramater `given` in range [0,1] which is scaled to V^(1/3)."
-    if given != None:
-        return given*poscar_data.volume**(1/3) + tol
+def _get_bond_length(poscar_data, given=None):
+    "`given` bond length should be in range [0,1] which is scaled to V^(1/3)."
+    if given is not None:
+        return given * poscar_data.volume ** (1 / 3)
     else:
-        basis = np.identity(3) if poscar_data.extra_info.cartesian else poscar_data.basis
-        _coords = to_R3(basis,poscar_data.positions)
-        _arr = sorted(np.linalg.norm(_coords[1:] - _coords[0],axis=1)) # Sort in ascending. returns list
-        return np.mean(_arr[:2]) + tol if _arr else 1 #Between nearest and second nearest.
+        keys = list(poscar_data.types.keys())
+        if len(keys) == 1:
+            keys = [*keys, *keys]  # strill need it to be a list of two elements
+
+        dists = [poscar_data.get_distance(k1, k2) for k1, k2 in combinations(keys, 2)]
+        return (
+            np.mean(dists) * 1.05
+        )  # Add 5% margin over mean distance, this covers same species too, and in multiple species, this will stop bonding between same species.
+
+
+def _masked_data(poscar_data, mask_sites):
+    "Returns indices of sites which satisfy the mask_sites function."
+    if not callable(mask_sites):
+        raise TypeError("`mask_sites` should be a callable function.")
+
+    if len(inspect.signature(mask_sites).parameters) != 4:
+        raise ValueError(
+            "`mask_sites` takes exactly 4 arguments: (index,x,y,z) in fractional coordinates"
+        )
+
+    if not isinstance(mask_sites(0, 0, 0, 0), bool):
+        raise TypeError("`mask_sites` should return a boolean value.")
+
+    eqv_inds = None
+    if hasattr(poscar_data.metadata, "eqv_indices"):
+        eqv_inds = tuple(poscar_data.metadata.eqv_indices)
+
+    pick = []
+    for i, pos in enumerate(poscar_data.positions):
+        idx = eqv_inds[i] if eqv_inds else i  # map to original index
+        if mask_sites(idx, *pos):
+            pick.append(i)
+    return pick  # could be duplicate indices
+
+
+# Cell
+def iplot_lattice(
+    poscar_data,
+    sizes=10,
+    colors=None,
+    bond_length=None,
+    tol=1e-2,
+    bond_tol=1e-3,
+    eqv_sites=True,
+    translate=None,
+    fig=None,
+    ortho3d=True,
+    mask_sites=None,
+    bond_kws=dict(line_width=4),
+    site_kws=dict(line_color="rgba(1,1,1,0)", line_width=0.001, opacity=1),
+    plot_cell=True,
+    **kwargs,
+):
+    """Plotly's interactive plot of lattice.
+
+    Parameters
+    ----------
+    sizes : float or tuple
+        Size of sites. Either one int/float or list equal to type of ions.
+    colors : tuple
+        Sequence of colors for each type. Automatically generated if not provided.
+    bond_length : float
+        Length of bond in fractional unit [0,1]. It is scaled to V^1/3 and auto calculated if not provides.
+    mask_sites : callable
+        Provide a mask function `f(index, x,y,z) -> bool` to show only selected sites.
+        For example, to show only sites with z > 0.5, use `mask_sites = lambda i, x,y,z: x > 0.5`.
+    bond_kws : dict
+        Keyword arguments passed to `plotly.graph_objects.Scatter3d` for bonds.
+        Default is jus hint, you can use any keyword argument that is accepted by `plotly.graph_objects.Scatter3d`.
+    site_kws : dict
+        Keyword arguments passed to `plotly.graph_objects.Scatter3d` for sites.
+        Default is jus hint, you can use any keyword argument that is accepted by `plotly.graph_objects.Scatter3d`.
+    plot_cell : bool
+        Defult is True. Plot unit cell with default settings.
+        If you want to customize, use `POSCAR.iplot_cell(fig = <return of iplot_lattice>)` function.
+
+
+    kwargs are passed to `iplot_bz`.
+    """
+    poscar_data = _fix_sites(
+        poscar_data, tol=tol, eqv_sites=eqv_sites, translate=translate
+    )
+    bond_length = _get_bond_length(poscar_data, given=bond_length)
+
+    sites = None
+    pos = poscar_data.positions
+    if (
+        mask_sites is not None
+    ):  # not None is important, as it can be False given by user
+        sites = _masked_data(poscar_data, mask_sites)
+        pos = poscar_data.positions[sites]
+        if not sites:
+            raise ValueError("No sites found with given mask_sites function.")
+
+    coords, pairs = get_pairs(
+        poscar_data.basis, pos, r=bond_length, tol=bond_tol
+    )  # bond tolernce should be smaller than cell tolernce.
 
-# Cell
-def iplot_lat(poscar_data,sizes=10,colors = None,
-              bond_length=None,tol=1e-2,bond_tol=1e-3,eqv_sites=True,
-              translate = None,
-              line_width=4,edge_color = 'black',
-              fill=False,alpha=0.4, ortho3d=True,fig=None):
-    """Interactive plot of lattice.
-    - **Main Parameters**
-        - poscar_data: Output of export_poscar or export_vasprun().poscar.
-        - sizes      : Size of sites. Either one int/float or list equal to type of ions.
-        - colors     : Sequence of colors for each type. Automatically generated if not provided.
-        - bond_length: Length of bond in fractional unit [0,1]. It is scaled to V^1/3 and auto calculated if not provides.
-    Other parameters just mean what they seem to be.
-    """
-    poscar_data = fix_sites(poscar_data,tol=tol,eqv_sites=eqv_sites,translate=translate)
-    bond_length = _get_bond_length(poscar_data,given=bond_length,tol=tol)
-    coords, pairs = get_pairs(poscar_data,
-                        positions = poscar_data.positions,
-                        r=bond_length,tol = bond_tol) # bond tolernce shpuld be smaller than cell tolernce.
     if not fig:
         fig = go.Figure()
 
-    uelems = poscar_data.unique.to_dict()
-    if not isinstance(sizes,(list,tuple,np.ndarray)):
+    uelems = poscar_data.types.to_dict()
+    if not isinstance(sizes, (list, tuple, np.ndarray)):
         sizes = [sizes for elem in uelems.keys()]
 
     if colors and len(colors) != len(uelems.keys()):
-        print('Warning: Number of colors does not match number of elements. Using default colors.')
+        print(
+            "Warning: Number of colors does not match number of atom types. Using default colors."
+        )
 
     if (colors is None) or len(colors) != len(uelems.keys()):
         colors = [_atom_colors[elem] for elem in uelems.keys()]
-        colors = ['rgb({},{},{})'.format(*[int(_c*255) for _c in c]) for c in colors]
+        colors = ["rgb({},{},{})".format(*[int(_c * 255) for _c in c]) for c in colors]
 
-    _colors = np.array([colors[i] for i,vs in enumerate(uelems.values()) for v in vs])
-    h_text = np.array( poscar_data.labels)
+    _colors = np.array([colors[i] for i, vs in enumerate(uelems.values()) for v in vs])
 
     if np.any(pairs):
-        coords_p = coords[pairs] #paired points
-        _colors = _colors[pairs] # Colors at pairs
+        coords_p = coords[pairs]  # paired points
+        _colors = _colors[pairs]  # Colors at pairs
         coords_n = []
         colors_n = []
-        for c_p, _c in zip(coords_p,_colors):
-            mid = np.mean(c_p,axis=0)
-            arr = np.concatenate([c_p[0],mid,mid,c_p[1]]).reshape((-1,2,3))
-            coords_n = [*coords_n,*arr] # Same shape
-            colors_n = [*colors_n,*_c] # same shape.
+        for c_p, _c in zip(coords_p, _colors):
+            mid = np.mean(c_p, axis=0)
+            arr = np.concatenate([c_p[0], mid, mid, c_p[1]]).reshape((-1, 2, 3))
+            coords_n = [*coords_n, *arr]  # Same shape
+            colors_n = [*colors_n, *_c]  # same shape.
 
         coords_n = np.array(coords_n)
         colors_n = np.array(colors_n)
 
-        for (i, cp),c in zip(enumerate(coords_n),colors_n):
+        bond_kws = {"line_width": 4, **bond_kws}
+
+        for (i, cp), c in zip(enumerate(coords_n), colors_n):
             showlegend = True if i == 0 else False
-            fig.add_trace(go.Scatter3d(
-                x = cp[:,0].T,
-                y = cp[:,1].T,
-                z = cp[:,2].T,
-                mode='lines',line_color = c,
-                legendgroup='Bonds',showlegend=showlegend,
-                name='Bonds',line_width=line_width))
-
-    for (k,v),c,s in zip(uelems.items(),colors,sizes):
-        fig.add_trace(go.Scatter3d(
-            x = coords[v][:,0].T,
-            y = coords[v][:,1].T,
-            z = coords[v][:,2].T,
-            mode='markers',marker_color = c,
-            hovertext = h_text[v],
-            line_color='rgba(1,1,1,0)',line_width=0.001,
-            marker_size = s,opacity=1,name=k))
-
-    bz = get_bz(path_pos= poscar_data.rec_basis, primitive=True)
-    _ = iplot_bz(bz,fig=fig,vname='a',color=edge_color,
-                fill=fill,alpha=alpha,ortho3d=ortho3d)
+            fig.add_trace(
+                go.Scatter3d(
+                    x=cp[:, 0].T,
+                    y=cp[:, 1].T,
+                    z=cp[:, 2].T,
+                    mode="lines",
+                    line_color=c,
+                    legendgroup="Bonds",
+                    showlegend=showlegend,
+                    name="Bonds",
+                    **bond_kws,
+                )
+            )
+
+    site_kws = {
+        **dict(line_color="rgba(1,1,1,0)", line_width=0.001, opacity=1),
+        **site_kws,
+    }
+    for (k, v), c, s in zip(uelems.items(), colors, sizes):
+        if sites:
+            v = [i for i in v if i in sites]  # Only show selected sites.
+            coords = poscar_data.coords[v]
+            labs = poscar_data.labels[v]
+        else:
+            coords = poscar_data.coords[v]
+            labs = poscar_data.labels[v]
+
+        fig.add_trace(
+            go.Scatter3d(
+                x=coords[:, 0].T,
+                y=coords[:, 1].T,
+                z=coords[:, 2].T,
+                mode="markers",
+                marker_color=c,
+                hovertext=labs,
+                marker_size=s,
+                name=k,
+                **site_kws,
+            )
+        )
+
+    if plot_cell:
+        bz_data = serializer.CellData(
+            get_bz(poscar_data.basis, primitive=True).to_dict()
+        )  # Make cell for correct vector notations
+        iplot_bz(bz_data, fig=fig, ortho3d=ortho3d, special_kpoints=False, **kwargs)
+    else:
+        if kwargs:
+            print("Warning: kwargs are ignored as plot_cell is False.")
+        # These thing are update in iplot_bz function, but if plot_cell is False, then we need to update them here.
+        proj = dict(projection=dict(type="orthographic")) if ortho3d else {}
+        camera = dict(center=dict(x=0.1, y=0.1, z=0.1), **proj)
+        fig.update_layout(
+            template="plotly_white",
+            scene_camera=camera,
+            font_family="Times New Roman",
+            font_size=14,
+            scene=dict(
+                aspectmode="data",
+                xaxis=dict(showbackground=False, visible=False),
+                yaxis=dict(showbackground=False, visible=False),
+                zaxis=dict(showbackground=False, visible=False),
+            ),
+            margin=dict(r=10, l=10, b=10, t=30),
+        )
     return fig
 
-# Cell
-def splot_lat(poscar_data,plane = None, sizes=50,colors=None,colormap=None,
-              bond_length=None,tol=1e-2,bond_tol=1e-3,eqv_sites=True,
-              translate = None,
-              line_width=1,edge_color=((1,0.5,0,0.4)),
-              vectors=True,v3=False,
-              light_from=(1,1,1),
-              fill=False,alpha=0.4,ax=None,alpha_points = 0.7):
-    """Static plot of lattice.
-    - **Main Parameters**
-        - poscar_data: Output of export_poscar or export_vasprun().poscar.
-        - plane      : Plane to plot. Either 'xy','xz','yz' or None for 3D plot.
-        - sizes      : Size of sites. Either one int/float or list equal to type of ions.
-        - bond_length: Length of bond in fractional unit [0,1]. It is scaled to V^1/3 and auto calculated if not provides.
-        - colors: Sequence of colors for each ion type. If None, automatically generated.
-        - colormap: This is passed to splot_bz.
-        - alpha_points: Opacity of points and bonds.
-    Other parameters just mean what they seem to be.
 
-    > Tip: Use `plt.style.use('ggplot')` for better 3D perception.
+def _validate_label_func(fmt_label, parameter):
+    if not callable(fmt_label):
+        raise ValueError("fmt_label must be a callable function.")
+    if len(inspect.signature(fmt_label).parameters.values()) != 1:
+        raise ValueError("fmt_label must have only one argument.")
+
+    test_out = fmt_label(parameter)
+    if isinstance(test_out, (list, tuple)):
+        if len(test_out) != 2:
+            raise ValueError(
+                "fmt_label must return string or a list/tuple of length 2."
+            )
+
+        if not isinstance(test_out[0], str):
+            raise ValueError(
+                "Fisrt item in return of `fmt_label` must return a string! got {}".format(
+                    type(test_out[0])
+                )
+            )
+
+        if not isinstance(test_out[1], dict):
+            raise ValueError(
+                "Second item in return of `fmt_label` must return a dictionary of keywords to pass to `plt.text`! got {}".format(
+                    type(test_out[1])
+                )
+            )
+
+    elif not isinstance(test_out, str):
+        raise ValueError("fmt_label must return a string or a list/tuple of length 2.")
+
+
+# Cell
+def splot_lattice(
+    poscar_data,
+    plane=None,
+    sizes=50,
+    colors=None,
+    bond_length=None,
+    tol=1e-2,
+    bond_tol=1e-3,
+    eqv_sites=True,
+    translate=None,
+    ax=None,
+    mask_sites=None,
+    showlegend=True,
+    fmt_label=None,
+    site_kws=dict(alpha=0.7),
+    bond_kws=dict(alpha=0.7, lw=1),
+    plot_cell=True,
+    **kwargs,
+):
+    """Matplotlib Static plot of lattice.
+
+    Parameters
+    ----------
+    plane : str
+        Plane to plot. Either 'xy','xz','yz' or None for 3D plot.
+    sizes : float or tuple
+        Size of sites. Either one int/float or list equal to type of ions.
+    colors : tuple
+        Sequence of colors for each ion type. If None, automatically generated.
+    bond_length : float
+        Length of bond in fractional unit [0,1]. It is scaled to V^1/3 and auto calculated if not provides.
+    alpha : float
+        Opacity of points and bonds.
+    mask_sites : callable
+        Provide a mask function `f(index, x,y,z) -> bool` to show only selected sites.
+        For example, to show only sites with z > 0.5, use `mask_sites = lambda i,x,y,z: x > 0.5`.
+    showlegend : bool
+        Default is True, show legend for each ion type.
+    site_kws : dict
+        Keyword arguments to pass to `plt.scatter` for plotting sites.
+        Default is just hint, you can pass any keyword argument that `plt.scatter` accepts.
+    bond_kws : dict
+        Keyword arguments to pass to `plt.plot` for plotting bonds.
+        Default is just hint, you can pass any keyword argument that `plt.plot` accepts.
+    fmt_label : callable
+        If given, each site label is passed to it like fmt_label('Ga 1').
+        It must return a string or a list/tuple of length 2 with first item as label and second item as dictionary of keywords to pass to `plt.text`.
+    plot_cell : bool
+        Default is True, plot unit cell with default settings.
+        To customize options, use `plot_cell = False` and do `POSCAR.splot_cell(ax = <return of splot_lattice>)`.
+
+
+    kwargs are passed to `splot_bz`.
+
+    .. tip::
+        Use `plt.style.use('ggplot')` for better 3D perception.
     """
-    #Plane fix
-    if plane and plane not in 'xyzxzyx':
+    # Plane fix
+    if plane and plane not in "xyzxzyx":
         raise ValueError("plane expects in 'xyzxzyx' or None.")
     if plane:
-        ind = 'xyzxzyx'.index(plane)
-        arr = [0,1,2,0,2,1,0]
-        ix,iy = arr[ind], arr[ind+1]
-    poscar_data = fix_sites(poscar_data,tol=tol,eqv_sites=eqv_sites,translate=translate)
-    bond_length = _get_bond_length(poscar_data,given=bond_length,tol=tol)
-    coords, pairs = get_pairs(poscar_data,
-                        positions = poscar_data.positions,
-                        r=bond_length,tol = bond_tol) # bond tolernce shpuld be smaller than cell tolernce.
-    bz = get_bz( poscar_data.rec_basis, primitive=True)
-    ax = splot_bz(bz,ax=ax,vname='a',
-                color=edge_color,colormap=colormap,
-                fill=fill,alpha=alpha,plane=plane,v3=v3,
-                vectors=vectors,light_from=light_from)
+        ind = "xyzxzyx".index(plane)
+        arr = [0, 1, 2, 0, 2, 1, 0]
+        ix, iy = arr[ind], arr[ind + 1]
+
+    poscar_data = _fix_sites(
+        poscar_data, tol=tol, eqv_sites=eqv_sites, translate=translate
+    )
+    bond_length = _get_bond_length(poscar_data, given=bond_length)
+
+    sites = None
+    pos = poscar_data.positions  # take all sites
+    if mask_sites is not None:  # not None is important, user can give anything
+        sites = _masked_data(poscar_data, mask_sites)
+        pos = poscar_data.positions[sites]
+        if not sites:
+            raise ValueError("No sites found with given mask_sites function.")
+
+    coords, pairs = get_pairs(
+        poscar_data.basis, positions=pos, r=bond_length, tol=bond_tol
+    )  # bond tolernce should be smaller than cell tolernce.
+
+    labels = [poscar_data.labels[i] for i in sites] if sites else poscar_data.labels
+    if fmt_label is not None:
+        _validate_label_func(fmt_label, labels[0])
+
+    if plot_cell:
+        bz_data = serializer.CellData(
+            get_bz(poscar_data.basis, primitive=True).to_dict()
+        )  # For correct vectors
+        ax = splot_bz(bz_data, plane=plane, ax=ax, **kwargs)
+    else:
+        ax = ax or ptk.get_axes(axes_3d=True if plane is None else False)
+        if kwargs:
+            print("Warning: kwargs are not used when plot_cell = False.")
 
-    uelems = poscar_data.unique.to_dict()
-    if not isinstance(sizes,(list,tuple, np.ndarray)):
+    uelems = poscar_data.types.to_dict()
+    if not isinstance(sizes, (list, tuple, np.ndarray)):
         sizes = [sizes for elem in uelems.keys()]
 
     if colors and len(colors) != len(uelems.keys()):
-        print('Warning: Number of colors does not match number of elements. Using default colors.')
+        print(
+            "Warning: Number of colors does not match number of atom types. Using default colors."
+        )
 
     if (colors is None) or len(colors) != len(uelems.keys()):
         colors = [_atom_colors[elem] for elem in uelems.keys()]
 
     # Before doing other stuff, create something for legend.
-    for (k,v),c,s in zip(uelems.items(),colors,sizes):
-        ax.scatter([],[],s=s,color=c,label=k) # Works both for 3D and 2D.
+    for (k, v), c, s in zip(uelems.items(), colors, sizes):
+        ax.scatter([], [], s=s, color=c, label=k)  # Works both for 3D and 2D.
 
     # Now change colors and sizes to whole array size
-    colors = np.array([colors[i] for i,vs in enumerate(uelems.values()) for v in vs])
-    sizes = np.array([sizes[i] for i,vs in enumerate(uelems.values()) for v in vs])
+    colors = np.array([colors[i] for i, vs in enumerate(uelems.values()) for v in vs])
+    sizes = np.array([sizes[i] for i, vs in enumerate(uelems.values()) for v in vs])
+
+    if sites:
+        colors = colors[sites]
+        sizes = sizes[sites]
 
     if np.any(pairs):
-        coords_p = coords[pairs] #paired points
-        _colors = colors[pairs] # Colors at pairs
+        coords_p = coords[pairs]  # paired points
+        _colors = colors[pairs]  # Colors at pairs
         coords_n = []
         colors_n = []
-        for c_p, _c in zip(coords_p,_colors):
-            mid = np.mean(c_p,axis=0)
-            arr = np.concatenate([c_p[0],mid,mid,c_p[1]]).reshape((-1,2,3))
-            coords_n = [*coords_n,*arr] # Same shape
-            colors_n = [*colors_n,*_c] # same shape.
+        for c_p, _c in zip(coords_p, _colors):
+            mid = np.mean(c_p, axis=0)
+            arr = np.concatenate([c_p[0], mid, mid, c_p[1]]).reshape((-1, 2, 3))
+            coords_n = [*coords_n, *arr]  # Same shape
+            colors_n = [*colors_n, *_c]  # same shape.
 
         coords_n = np.array(coords_n)
         colors_n = np.array(colors_n)
 
+        bond_kws = {
+            "alpha": 0.7,
+            "solid_capstyle": "butt",
+            **bond_kws,
+        }  # bond_kws overrides alpha and solid_capstyle only
         if not plane:
-            _ = [ax.plot(*c.T,c=_c,lw=line_width, alpha = alpha_points) for c,_c in zip(coords_n,colors_n)]
-        elif plane in 'xyzxzyx':
-            _ = [ax.plot(c[:,ix],c[:,iy],c=_c,lw=line_width, alpha = alpha_points) for c,_c in zip(coords_n,colors_n)]
+            _ = [ax.plot(*c.T, c=_c, **bond_kws) for c, _c in zip(coords_n, colors_n)]
+        elif plane in "xyzxzyx":
+            _ = [
+                ax.plot(c[:, ix], c[:, iy], c=_c, **bond_kws)
+                for c, _c in zip(coords_n, colors_n)
+            ]
 
     if not plane:
-        ax.scatter(coords[:,0],coords[:,1],coords[:,2],c = colors ,s =sizes,depthshade=False,alpha=alpha_points)
-    elif plane in 'xyzxzyx':
-        iz, = [i for i in range(3) if i not in (ix,iy)]
-        zorder = coords[:,iz].argsort()
-        if plane in 'yxzy': # Left handed
+        site_kws = {
+            **dict(alpha=0.7, depthshade=False),
+            **site_kws,
+        }  # site_kws overrides alpha only
+        ax.scatter(
+            coords[:, 0], coords[:, 1], coords[:, 2], c=colors, s=sizes, **site_kws
+        )
+        if fmt_label:
+            for i, coord in enumerate(coords):
+                lab, textkws = fmt_label(labels[i]), {}
+                if isinstance(lab, (list, tuple)):
+                    lab, textkws = lab
+                ax.text(*coord, lab, **textkws)
+        # Set aspect to same as data.
+        ax.set_box_aspect(np.ptp(bz_data.vertices, axis=0))
+
+    elif plane in "xyzxzyx":
+        site_kws = {**dict(alpha=0.7, zorder=3), **site_kws}
+        (iz,) = [i for i in range(3) if i not in (ix, iy)]
+        zorder = coords[:, iz].argsort()
+        if plane in "yxzy":  # Left handed
             zorder = zorder[::-1]
-        ax.scatter(coords[zorder][:,ix],coords[zorder][:,iy],c = colors[zorder] ,s =sizes[zorder],zorder=3, alpha= alpha_points)
+        ax.scatter(
+            coords[zorder][:, ix],
+            coords[zorder][:, iy],
+            c=colors[zorder],
+            s=sizes[zorder],
+            **site_kws,
+        )
+
+        if fmt_label:
+            labels = [labels[i] for i in zorder]  # Reorder labels
+            for i, coord in enumerate(coords[zorder]):
+                lab, textkws = fmt_label(labels[i]), {}
+                if isinstance(lab, (list, tuple)):
+                    lab, textkws = lab
+                ax.text(*coord[[ix, iy]], lab, **textkws)
+
+        # Set aspect to display real shape.
+        ax.set_aspect("equal")
 
     ax.set_axis_off()
-    sp.add_legend(ax)
+    if showlegend:
+        ptk.add_legend(ax)
     return ax
 
+
 # Cell
-def join_poscars(poscar1,poscar2,direction='c',tol=1e-2, system = None):
-    """Joins two POSCARs in a given direction. In-plane lattice parameters are kept from `poscar1` and basis of `poscar2` parallel to `direction` is modified while volume is kept same.
-    - **Parameters**
-        - poscar1, poscar2:  Base and secondary POSCARs respectivly. Output of `export_poscar` or similar object from other functions.
-        - direction: The joining direction. It is general and can join in any direction along basis. Expect one of ['a','b','c'].
-        - tol: Default is 0.01. It is used to bring sites near 1 to near zero in order to complete sites in plane. Vasp relaxation could move a point, say at 0.00100 to 0.99800 which is not useful while merging sites.
-        - system: If system is given, it is written on top of file. Otherwise, it is infered from atomic species.
+def join_poscars(poscar_data, other, direction="c", tol=1e-2, system=None):
+    """Joins two POSCARs in a given direction. In-plane lattice parameters are kept from
+    first poscar and out of plane basis vector of other is modified while volume is kept same.
+
+    Parameters
+    ----------
+    other : type(self)
+        Other POSCAR to be joined with this POSCAR.
+    direction : str
+        The joining direction. It is general and can join in any direction along basis. Expect one of ['a','b','c'].
+    tol : float
+        Default is 0.01. It is used to bring sites near 1 to near zero in order to complete sites in plane.
+        Vasp relaxation could move a point, say at 0.00100 to 0.99800 which is not useful while merging sites.
+    system : str
+        If system is given, it is written on top of file. Otherwise, it is infered from atomic species.
     """
-    _poscar1 = fix_sites(poscar1,tol=tol,eqv_sites=False)
-    _poscar2 = fix_sites(poscar2,tol=tol,eqv_sites=False)
+    _poscar1 = _fix_sites(poscar_data, tol=tol, eqv_sites=False)
+    _poscar2 = _fix_sites(other, tol=tol, eqv_sites=False)
     pos1 = _poscar1.positions.copy()
     pos2 = _poscar2.positions.copy()
 
-    s1,s2 = 0.5, 0.5 # Half length for each.
-    a1,b1,c1 = np.linalg.norm(_poscar1.basis,axis=1)
-    a2,b2,c2 = np.linalg.norm(_poscar2.basis,axis=1)
-    basis = _poscar1.basis.copy() # Must be copied, otherwise change outside.
+    s1, s2 = 0.5, 0.5  # Half length for each.
+    a1, b1, c1 = np.linalg.norm(_poscar1.basis, axis=1)
+    a2, b2, c2 = np.linalg.norm(_poscar2.basis, axis=1)
+    basis = _poscar1.basis.copy()  # Must be copied, otherwise change outside.
 
     # Processing in orthogonal space since a.(b x c) = abc sin(theta)cos(phi), and theta and phi are same for both.
-    if direction in 'cC':
-        c2 = (a2*b2)/(a1*b1)*c2 # Conservation of volume for right side to stretch in c-direction.
-        netc = c1+c2
-        s1, s2 = c1/netc, c2/netc
-        pos1[:,2] = s1*pos1[:,2]
-        pos2[:,2] = s2*pos2[:,2] + s1
-        basis[2] = netc*basis[2]/np.linalg.norm(basis[2]) #Update 3rd vector
-
-    elif direction in 'bB':
-        b2 = (a2*c2)/(a1*c1)*b2 # Conservation of volume for right side to stretch in b-direction.
-        netb = b1+b2
-        s1, s2 = b1/netb, b2/netb
-        pos1[:,1] = s1*pos1[:,1]
-        pos2[:,1] = s2*pos2[:,1] + s1
-        basis[1] = netb*basis[1]/np.linalg.norm(basis[1]) #Update 2nd vector
-
-    elif direction in 'aA':
-        a2 = (b2*c2)/(b1*c1)*a2 # Conservation of volume for right side to stretch in a-direction.
-        neta = a1+a2
-        s1, s2 = a1/neta, a2/neta
-        pos1[:,0] = s1*pos1[:,0]
-        pos2[:,0] = s2*pos2[:,0] + s1
-        basis[0] = neta*basis[0]/np.linalg.norm(basis[0]) #Update 1st vector
+    if direction in "cC":
+        c2 = (
+            (a2 * b2) / (a1 * b1) * c2
+        )  # Conservation of volume for right side to stretch in c-direction.
+        netc = c1 + c2
+        s1, s2 = c1 / netc, c2 / netc
+        pos1[:, 2] = s1 * pos1[:, 2]
+        pos2[:, 2] = s2 * pos2[:, 2] + s1
+        basis[2] = netc * basis[2] / np.linalg.norm(basis[2])  # Update 3rd vector
+
+    elif direction in "bB":
+        b2 = (
+            (a2 * c2) / (a1 * c1) * b2
+        )  # Conservation of volume for right side to stretch in b-direction.
+        netb = b1 + b2
+        s1, s2 = b1 / netb, b2 / netb
+        pos1[:, 1] = s1 * pos1[:, 1]
+        pos2[:, 1] = s2 * pos2[:, 1] + s1
+        basis[1] = netb * basis[1] / np.linalg.norm(basis[1])  # Update 2nd vector
+
+    elif direction in "aA":
+        a2 = (
+            (b2 * c2) / (b1 * c1) * a2
+        )  # Conservation of volume for right side to stretch in a-direction.
+        neta = a1 + a2
+        s1, s2 = a1 / neta, a2 / neta
+        pos1[:, 0] = s1 * pos1[:, 0]
+        pos2[:, 0] = s2 * pos2[:, 0] + s1
+        basis[0] = neta * basis[0] / np.linalg.norm(basis[0])  # Update 1st vector
 
     else:
         raise Exception("direction expects one of ['a','b','c']")
 
     scale = np.linalg.norm(basis[0])
-    u1 = _poscar1.unique.to_dict()
-    u2 = _poscar2.unique.to_dict()
-    u_all = ({**u1,**u2}).keys() # Union of unique elements to keep track of order.
-
+    u1 = _poscar1.types.to_dict()
+    u2 = _poscar2.types.to_dict()
+    u_all = ({**u1, **u2}).keys()  # Union of unique atom types to keep track of order.
 
     pos_all = []
     i_all = []
     for u in u_all:
         _i_ = 0
         if u in u1.keys():
             _i_ = len(u1[u])
-            pos_all = [*pos_all,*pos1[u1[u]]]
+            pos_all = [*pos_all, *pos1[u1[u]]]
         if u in u2.keys():
             _i_ = _i_ + len(u2[u])
-            pos_all = [*pos_all,*pos2[u2[u]]]
+            pos_all = [*pos_all, *pos2[u2[u]]]
         i_all.append(_i_)
 
-    i_all = np.cumsum([0,*i_all]) # Do it after labels
-    uelems = {_u:range(i_all[i],i_all[i+1]) for i,_u in enumerate(u_all)}
-    sys = system or ''.join(uelems.keys())
-    iscartesian = poscar1.extra_info.cartesian or poscar2.extra_info.cartesian
-    extra_info = {'cartesian':iscartesian, 'scale': scale, 'comment': 'Modified by ipyvasp'}
-    out_dict = {'SYSTEM':sys,'basis':basis,'extra_info':extra_info,'positions':np.array(pos_all),'unique':uelems}
+    i_all = np.cumsum([0, *i_all])  # Do it after labels
+    uelems = {_u: range(i_all[i], i_all[i + 1]) for i, _u in enumerate(u_all)}
+    sys = system or "".join(uelems.keys())
+    iscartesian = poscar_data.metadata.cartesian or other.metadata.cartesian
+    metadata = {
+        "cartesian": iscartesian,
+        "scale": scale,
+        "comment": "Modified by ipyvasp",
+    }
+    out_dict = {
+        "SYSTEM": sys,
+        "basis": basis,
+        "metadata": metadata,
+        "positions": np.array(pos_all),
+        "types": uelems,
+    }
     return serializer.PoscarData(out_dict)
 
 
 # Cell
 def repeat_poscar(poscar_data, n, direction):
     """Repeat a given POSCAR.
-    - **Parameters**
-        - path_poscar: Path/to/POSCAR or `poscar` data object.
-        - n: Number of repetitions.
-        - direction: Direction of repetition. Can be 'a', 'b' or 'c'.
+
+    Parameters
+    ----------
+    n : int
+        Number of repetitions.
+    direction : str
+        Direction of repetition. Can be 'a', 'b' or 'c'.
     """
-    if not isinstance(n, int) and n < 2:
+    if not isinstance(n, (int, np.integer)) and n < 2:
         raise ValueError("n must be an integer greater than 1.")
     given_poscar = poscar_data
-    for i in range(1,n):
-        poscar_data = join_poscars(given_poscar, poscar_data,direction = direction)
+    for i in range(1, n):
+        poscar_data = join_poscars(given_poscar, poscar_data, direction=direction)
     return poscar_data
 
-def scale_poscar(poscar_data,scale = (1,1,1),tol=1e-2):
+
+def scale_poscar(poscar_data, scale=(1, 1, 1), tol=1e-2):
     """Create larger/smaller cell from a given POSCAR. Can be used to repeat a POSCAR with integer scale values.
-    - **Parameters**
-        - poscar_data: `poscar` data object.
-        - scale: Tuple of three values along (a,b,c) vectors. int or float values. If number of sites are not as expected in output, tweak `tol` instead of `scale`. You can put a minus sign with `tol` to get more sites and plus sign to reduce sites.
-        - tol: It is used such that site positions are blow `1 - tol`, as 1 belongs to next cell, not previous one.
-    **Tip:** scale = (2,2,2) enlarges a cell and next operation of (1/2,1/2,1/2) should bring original cell back.
-    **Caveat:** A POSACR scaled with Non-integer values should only be used for visualization purposes, Not for any other opration such as making supercells, joining POSCARs.
+
+    Parameters
+    ----------
+    scale : tuple
+        Tuple of three values along (a,b,c) vectors. int or float values. If number of sites are not as expected in output,
+        tweak `tol` instead of `scale`. You can put a minus sign with `tol` to get more sites and plus sign to reduce sites.
+    tol : float
+        It is used such that site positions are blow `1 - tol`, as 1 belongs to next cell, not previous one.
+
+
+    .. note::
+        ``scale = (2,2,2)`` enlarges a cell and next operation of ``(1/2,1/2,1/2)`` should bring original cell back.
+
+    .. warning::
+        A POSCAR scaled with Non-integer values should only be used for visualization purposes, Not for any other opration such as making supercells, joining POSCARs.
     """
-    ii, jj, kk = np.ceil(scale).astype(int) # Need int for joining.
+    ii, jj, kk = np.ceil(scale).astype(int)  # Need int for joining.
 
-    if tuple(scale) == (1,1,1): # No need to scale.
+    if tuple(scale) == (1, 1, 1):  # No need to scale.
         return poscar_data
 
     if ii >= 2:
-        poscar_data = repeat_poscar(poscar_data,ii,direction='a')
+        poscar_data = repeat_poscar(poscar_data, ii, direction="a")
 
     if jj >= 2:
-        poscar_data = repeat_poscar(poscar_data,jj,direction='b')
+        poscar_data = repeat_poscar(poscar_data, jj, direction="b")
 
     if kk >= 2:
-        poscar_data = repeat_poscar(poscar_data,kk,direction='c')
+        poscar_data = repeat_poscar(poscar_data, kk, direction="c")
 
     if np.all([s == int(s) for s in scale]):
-        return poscar_data # No need to prcess further in case of integer scaling.
+        return poscar_data  # No need to prcess further in case of integer scaling.
 
-    new_poscar = poscar_data.to_dict() # Update in it
+    new_poscar = poscar_data.to_dict()  # Update in it
 
     # Get clip fraction
-    fi, fj, fk = scale[0]/ii, scale[1]/jj, scale[2]/kk
+    fi, fj, fk = scale[0] / ii, scale[1] / jj, scale[2] / kk
 
     # Clip at end according to scale, change length of basis as fractions.
-    pos   = poscar_data.positions.copy()/np.array([fi,fj,fk]) # rescale for clip
+    pos = poscar_data.positions.copy() / np.array([fi, fj, fk])  # rescale for clip
     basis = poscar_data.basis.copy()
-    for i,f in zip(range(3),[fi,fj,fk]):
-        basis[i] = f*basis[i] # Basis rescale for clip
+    for i, f in zip(range(3), [fi, fj, fk]):
+        basis[i] = f * basis[i]  # Basis rescale for clip
 
-    new_poscar['basis'] = basis
-    new_poscar['extra_info']['scale'] = np.linalg.norm(basis[0])
-    new_poscar['extra_info']['comment'] = f'Modified by ipyvasp'
+    new_poscar["basis"] = basis
+    new_poscar["metadata"]["scale"] = np.linalg.norm(basis[0])
+    new_poscar["metadata"]["comment"] = f"Modified by ipyvasp"
 
-    uelems = poscar_data.unique.to_dict()
+    uelems = poscar_data.types.to_dict()
     # Minus in below for block is because if we have 0-2 then 1 belongs to next cell not original.
-    positions,shift = [],0
-    for key,value in uelems.items():
-        s_p = pos[value] # Get positions of key
-        s_p = s_p[(s_p < 1 - tol).all(axis=1)] # Get sites within tolerance
+    positions, shift = [], 0
+    for key, value in uelems.items():
+        s_p = pos[value]  # Get positions of key
+        s_p = s_p[(s_p < 1 - tol).all(axis=1)]  # Get sites within tolerance
 
         if len(s_p) == 0:
-            raise Exception(f'No sites found for {key!r}, cannot scale down. Increase scale!')
-
-        uelems[key] = range(shift,shift + len(s_p))
-        positions = [*positions,*s_p] # Pick sites
-        shift += len(s_p) #Update for next element
+            raise Exception(
+                f"No sites found for {key!r}, cannot scale down. Increase scale!"
+            )
+
+        uelems[key] = range(shift, shift + len(s_p))
+        positions = [*positions, *s_p]  # Pick sites
+        shift += len(s_p)  # Update for next element
 
-    new_poscar['unique']    = uelems
-    new_poscar['positions'] = np.array(positions)
+    new_poscar["types"] = uelems
+    new_poscar["positions"] = np.array(positions)
     return serializer.PoscarData(new_poscar)
 
-def rotate_poscar(poscar_data,angle_deg,axis_vec):
+
+def rotate_poscar(poscar_data, angle_deg, axis_vec):
     """Rotate a given POSCAR.
-    - **Parameters**
-        - path_poscar: Path/to/POSCAR or `poscar` data object.
-        - angle_deg: Rotation angle in degrees.
-        - axis_vec : (x,y,z) of axis about which rotation takes place. Axis passes through origin.
+
+    Parameters
+    ----------
+    angle_deg : float
+        Rotation angle in degrees.
+    axis_vec : array_like
+        Vector (x,y,z) of axis about which rotation takes place. Axis passes through origin.
     """
-    rot = rotation(angle_deg=angle_deg,axis_vec=axis_vec)
+    rot = rotation(angle_deg=angle_deg, axis_vec=axis_vec)
     p_dict = poscar_data.to_dict()
-    p_dict['basis'] = rot.apply(p_dict['basis']) # Rotate basis so that they are transpose
-    p_dict['extra_info']['comment'] = f'Modified by ipyvasp'
+    p_dict["basis"] = rot.apply(
+        p_dict["basis"]
+    )  # Rotate basis so that they are transpose
+    p_dict["metadata"]["comment"] = f"Modified by ipyvasp"
     return serializer.PoscarData(p_dict)
 
+
+def set_zdir(poscar_data, hkl, phi=0):
+    """Set z-direction of POSCAR along a given hkl direction and returns new data.
+
+    Parameters
+    ----------
+    hkl : tuple
+        (h,k,l) of the direction along which z-direction is to be set.
+        Vector is constructed as h*a + k*b + l*c in cartesian coordinates.
+    phi: float
+        Rotation angle in degrees about z-axis to set a desired rotated view.
+
+    Returns
+    -------
+    New instance of poscar with z-direction set along hkl.
+    """
+    if not isinstance(hkl, (list, tuple, np.ndarray)) and len(hkl) != 3:
+        raise ValueError("hkl must be a list, tuple or numpy array of length 3.")
+
+    p_dict = poscar_data.to_dict()
+    basis = p_dict["basis"]
+    zvec = to_R3(basis, [hkl])[0]  # in cartesian coordinates
+    angle = np.arccos(
+        zvec.dot([0, 0, 1]) / np.linalg.norm(zvec)
+    )  # Angle between zvec and z-axis
+    rot = rotation(
+        angle_deg=np.rad2deg(angle), axis_vec=np.cross(zvec, [0, 0, 1])
+    )  # Rotation matrix
+    new_basis = rot.apply(basis)  # Rotate basis so that zvec is along z-axis
+    p_dict["basis"] = new_basis
+    p_dict["metadata"]["comment"] = f"Modified by ipyvasp"
+    new_pos = serializer.PoscarData(p_dict)
+
+    if phi:  # Rotate around z-axis
+        return rotate_poscar(new_pos, angle_deg=phi, axis_vec=[0, 0, 1])
+
+    return new_pos
+
+
 def mirror_poscar(poscar_data, direction):
     "Mirror a POSCAR in a given direction. Sometime you need it before joining two POSCARs"
-    poscar = poscar_data.to_dict() # Avoid modifying original
-    idx = 'abc'.index(direction) # Check if direction is valid
-    poscar['positions'][:,idx] = 1 - poscar['positions'][:,idx] # Trick: Mirror by subtracting from 1. not by multiplying with -1.
-    return serializer.PoscarData(poscar) # Return new POSCAR
+    poscar = poscar_data.to_dict()  # Avoid modifying original
+    idx = "abc".index(direction)  # Check if direction is valid
+    poscar["positions"][:, idx] = (
+        1 - poscar["positions"][:, idx]
+    )  # Trick: Mirror by subtracting from 1. not by multiplying with -1.
+    return serializer.PoscarData(poscar)  # Return new POSCAR
+
 
 def convert_poscar(poscar_data, atoms_mapping, basis_factor):
     """Convert a POSCAR to a similar structure of other atomic types or same type with strained basis.
-    `atoms_mapping` is a dictionary of {old_atom: new_atom} like {'Ga':'Al'} will convert GaAs to AlAs structure.
-    `basis_factor` is a scaling factor multiplied with basis vectors, single value (useful for conversion to another type)
-    or list of three values to scale along (a,b,c) vectors (useful for strained structures).
-    """
-    poscar_data = poscar_data.to_dict() # Avoid modifying original
-    poscar_data['unique'] = {atoms_mapping.get(k,k):v for k,v in poscar_data['unique'].items()} # Update types
-    basis = poscar_data['basis'].copy() # Get basis to avoid modifying original
-
-    if isinstance(basis_factor,(int,float)):
-        poscar_data['basis'] = basis_factor*basis # Rescale basis
-    elif isinstance(basis_factor,(list,tuple,np.ndarray)):
+
+    Parameters
+    ----------
+    atoms_mapping : dict
+        A dictionary of {old_atom: new_atom} like {'Ga':'Al'} will convert GaAs to AlAs structure.
+    basis_factor : float
+        A scaling factor multiplied with basis vectors, single value (useful for conversion to another type)
+        or list of three values to scale along (a,b,c) vectors (useful for strained structures).
+
+
+    .. note::
+        This can be used to strain basis vectors uniformly only. For non-uniform strain, use :func:`ipyvasp.POSCAR.strain`.
+    """
+    poscar_data = poscar_data.to_dict()  # Avoid modifying original
+    poscar_data["types"] = {
+        atoms_mapping.get(k, k): v for k, v in poscar_data["types"].items()
+    }  # Update types
+    basis = poscar_data["basis"].copy()  # Get basis to avoid modifying original
+
+    if isinstance(basis_factor, (int, np.integer, float)):
+        poscar_data["basis"] = basis_factor * basis  # Rescale basis
+    elif isinstance(basis_factor, (list, tuple, np.ndarray)):
         if len(basis_factor) != 3:
-            raise Exception('basis_factor should be a list/tuple/array of length 3')
+            raise Exception("basis_factor should be a list/tuple/array of length 3")
 
         if np.ndim(basis_factor) != 1:
-            raise Exception('basis_factor should be a list/tuple/array of 3 int/float values')
-
-        poscar_data['basis'] = np.array([
-            basis_factor[0]*basis[0],
-            basis_factor[1]*basis[1],
-            basis_factor[2]*basis[2]
-        ])
+            raise Exception(
+                "basis_factor should be a list/tuple/array of 3 int/float values"
+            )
+
+        poscar_data["basis"] = np.array(
+            [
+                basis_factor[0] * basis[0],
+                basis_factor[1] * basis[1],
+                basis_factor[2] * basis[2],
+            ]
+        )
     else:
-        raise Exception('basis_factor should be a list/tuple/array of 3 int/float values, got {}'.format(type(basis_factor)))
-
-    return serializer.PoscarData(poscar_data) # Return new POSCAR
-
-def get_transform_matrix(poscar_data, target_basis):
-    "Returns a transformation matrix that gives `target_bsis` when applied on basis of current lattice. Useful in transforming crystal structure."
-    return np.matmul(target_basis, np.linalg.inv(poscar_data.basis)).round(16)
-
-def transform_poscar(poscar_data, transform_matrix, repeat_given = [2,2,2],tol = 1e-2):
-    """Transform a POSCAR with a given transformation matrix.
-    Use `get_transform_matrix` to get transformation matrix from one basis to another.
-    `repeat_given` is used to repeat the POSCAR before applying transformation matrix to include
-    all possible sites in resultant cell."""
-    new_basis = np.matmul(transform_matrix,poscar_data.basis) # Transforms basis to target basis
-
-    if len(repeat_given) != 3:
-        raise ValueError('`repeat_given` must be a list of three integers.')
-
-    for rep in repeat_given: # Repeat if needed
-        if not isinstance(rep,(int,np.int)) and rep >= 1:
-            raise ValueError('`repeat_given` must have all values as integer >= 1.')
-
-    for n, _dir in zip(repeat_given,'abc'): # Repeat if needed for including atoms in new cell
-        poscar_data = repeat_poscar(poscar_data,n,direction=_dir)
-
-    center_coords = poscar_data.coords - poscar_data.coords.mean(axis=0, keepdims=True) # Center around origin
-    points = to_basis(new_basis,center_coords) # Transform coordinates to new basis around origin
-
-    new_poscar = poscar_data.to_dict() # Update in it
-    new_poscar['basis'] = new_basis
-    new_poscar['extra_info']['scale'] = np.linalg.norm(new_basis[0])
-    new_poscar['extra_info']['comment'] = f'Transformed by ipyvasp'
-
-    uelems = poscar_data.unique.to_dict()
-    positions,shift, unique_dict = [],0, {}
-    for key,value in uelems.items():
-        s_p = points[value] # Get positions of key
-        s_p = s_p[((s_p > -tol) & (s_p < 1 - tol)).all(axis=1)] # Get sites within tolerance
-
-        if len(s_p) == 0:
-            raise Exception(f'No sites found for {key!r}, transformation stopped! You may need to increase `repeat_given` parameter.')
-
-        unique_dict[key] = range(shift,shift + len(s_p))
-        positions = [*positions,*s_p] # Pick sites
-        shift += len(s_p) #Update for next element
+        raise Exception(
+            "basis_factor should be a list/tuple/array of 3 int/float values, got {}".format(
+                type(basis_factor)
+            )
+        )
+
+    return serializer.PoscarData(poscar_data)  # Return new POSCAR
+
+
+def transform_poscar(poscar_data, transformation, zoom=2, tol=1e-2):
+    """Transform a POSCAR with a given transformation matrix or function that takes old basis and return target basis.
+    Use `get_TM(basis1, basis2)` to get transformation matrix from one basis to another or function to return new basis of your choice.
+    An example of transformation function is `lambda a,b,c: a + b, a-b, c` which will give a new basis with a+b, a-b, c as basis vectors.
+
+    You may find errors due to missing atoms in the new basis, use `zoom` to increase the size of given cell to include any possible site in new cell.
+
+    Examples
+    --------
+    - FCC primitive → 111 hexagonal cell: ``lambda a,b,c: (a-c,b-c,a+b+c) ~ [[1,0,-1],[0,1,-1],[1,1,1]]``
+    - FCC primitive → FCC unit cell: ``lambda a,b,c: (b+c -a,a+c-b,a+b-c) ~ [[-1,1,1],[1,-1,1],[1,1,-1]]``
+    - FCC unit cell → 110 tetragonal cell: ``lambda a,b,c: (a-b,a+b,c) ~ [[1,-1,0],[1,1,0],[0,0,1]]``
+    """
+    if callable(transformation):
+        new_basis = np.array(transformation(*poscar_data.basis))  # mostly a tuple
+        if new_basis.shape != (3, 3):
+            raise Exception(
+                "transformation function should return a tuple equivalent to 3x3 matrix"
+            )
+    elif np.ndim(transformation) == 2 and np.shape(transformation) == (3, 3):
+        new_basis = np.matmul(transformation, poscar_data.basis)
+    else:
+        raise Exception(
+            "transformation should be a function that accept 3 arguemnts or 3x3 matrix"
+        )
+
+    def get_cell_vertices(basis):
+        verts = get_bz(basis, primitive=True).vertices
+        return verts - np.mean(
+            verts, axis=0
+        )  # Center around origin, otherwise it never going to be inside convex hull
+
+    TM = get_TM(
+        poscar_data.basis, new_basis
+    )  # Transformation matrix to save before scaling
+    old_numbers = [len(v) for v in poscar_data.types.to_dict().values()]
+    chull = ConvexHull(
+        np.max([zoom, 2]) * get_cell_vertices(new_basis)
+    )  # Convex hull of new cell, make it at least two times to avoid losing sites because of translation
+
+    while any(
+        inside_convexhull(chull, get_cell_vertices(poscar_data.basis))
+    ):  # Check if all vertices of old cell are inside new cell
+        poscar_data = scale_poscar(
+            poscar_data, [2, 2, 2], tol=tol
+        )  # Repeat in all directions
+
+    points = to_basis(
+        new_basis, poscar_data.coords
+    )  # Transform coordinates to new basis around origin
+    points = points - np.mean(points, axis=0)  # Center around origin, to include all
+
+    new_poscar = poscar_data.to_dict()  # Update in it
+    new_poscar["basis"] = new_basis
+    new_poscar["metadata"]["scale"] = np.linalg.norm(new_basis[0])
+    new_poscar["metadata"]["comment"] = f"Transformed by ipyvasp"
+    new_poscar["metadata"][
+        "TM"
+    ] = TM  # Save transformation matrix in both function and matrix given
+
+    uelems = poscar_data.types.to_dict()
+    positions, shift, unique_dict = [], 0, {}
+    for key, value in uelems.items():
+        s_p = points[value]
+        s_p = s_p[
+            ((s_p > -tol) & (s_p < 1 - tol)).all(axis=1)
+        ]  # Get sites within tolerance, for very far sites
+
+        if s_p.size == 0:
+            raise Exception(
+                f"No sites found for {key!r}, transformation stopped! You may need to modify `transformation` or increase `zoom` value."
+            )
+
+        unique_dict[key] = range(shift, shift + len(s_p))
+        positions = [*positions, *s_p]  # Pick sites
+        shift += len(s_p)  # Update for next element
+
+    # Final check if crystal is still same
+    new_numbers = [len(v) for v in unique_dict.values()]
+    ratio = [
+        round(new / old, 4) for new, old in zip(new_numbers, old_numbers)
+    ]  # Round to avoid floating point errors,can cover 1 to 10000 atoms transformation
+    if len(np.unique(ratio)) != 1:
+        raise Exception(
+            f"Transformation failed, atoms proportion changed: {old_numbers} -> {new_numbers}, if your transformation is an allowed one for this structure, increase `zoom` value."
+        )
 
-    new_poscar['unique']  = unique_dict
-    new_poscar['positions'] = np.array(positions)
+    new_poscar["types"] = unique_dict
+    new_poscar["positions"] = np.array(positions)
     return serializer.PoscarData(new_poscar)
 
-def add_vaccum(poscar_data, thickness, direction, left = False):
+
+def add_vaccum(poscar_data, thickness, direction, left=False):
     """Add vacuum to a POSCAR.
-    - **Parameters**
-        - poscar_data: `poscar` data object.
-        - thickness: Thickness of vacuum in Angstrom.
-        - direction: Direction of vacuum. Can be 'a', 'b' or 'c'.
-        - left: If True, vacuum is added to left of sites. By default, vacuum is added to right of sites.
-    """
-    if direction not in 'abc':
-        raise Exception('Direction must be a, b or c.')
 
-    poscar_dict = poscar_data.to_dict() # Avoid modifying original
-    basis = poscar_dict['basis'].copy() # Copy basis to avoid modifying original
-    pos = poscar_dict['positions'].copy() # Copy positions to avoid modifying original
-    idx = 'abc'.index(direction)
-    norm = np.linalg.norm(basis[idx]) # Get length of basis vector
-    s1, s2 = norm/(norm + thickness), thickness/(norm + thickness) # Get scaling factors
-    basis[idx,:] *= (thickness + norm)/norm # Add thickness to basis
-    poscar_dict['basis'] = basis
+    Parameters
+    ----------
+    thickness : float
+        Thickness of vacuum in Angstrom.
+    direction : str
+        Direction of vacuum. Can be 'a', 'b' or 'c'.
+    left : bool
+        If True, vacuum is added to left of sites. By default, vacuum is added to right of sites.
+    """
+    if direction not in "abc":
+        raise Exception("Direction must be a, b or c.")
+
+    poscar_dict = poscar_data.to_dict()  # Avoid modifying original
+    basis = poscar_dict["basis"].copy()  # Copy basis to avoid modifying original
+    pos = poscar_dict["positions"].copy()  # Copy positions to avoid modifying original
+    idx = "abc".index(direction)
+    norm = np.linalg.norm(basis[idx])  # Get length of basis vector
+    s1, s2 = norm / (norm + thickness), thickness / (norm + thickness)  # Get scaling
+    basis[idx, :] *= (thickness + norm) / norm  # Add thickness to basis
+    poscar_dict["basis"] = basis
     if left:
-        pos[:,idx] *= s2 # Scale down positions
-        pos[:,idx] += s1 # Add vacuum to left of sites
-        poscar_dict['positions'] = pos
+        pos[:, idx] *= s2  # Scale down positions
+        pos[:, idx] += s1  # Add vacuum to left of sites
+        poscar_dict["positions"] = pos
     else:
-        pos[:,idx] *= s1 # Scale down positions
-        poscar_dict['positions'] = pos
+        pos[:, idx] *= s1  # Scale down positions
+        poscar_dict["positions"] = pos
 
-    return serializer.PoscarData(poscar_dict) # Return new POSCAR
+    return serializer.PoscarData(poscar_dict)  # Return new POSCAR
 
 
-# Cell
-def transpose_poscar(poscar_data, axes = [1,0,2]):
+def transpose_poscar(poscar_data, axes=[1, 0, 2]):
     "Transpose a POSCAR by switching basis from [0,1,2] -> `axes`. By Default, x and y are transposed."
-    if isinstance(axes,(list,tuple, np.ndarray)) and len(axes) == 3:
-        if not all(isinstance(i,(int,np.int)) for i in axes):
-            raise ValueError('`axes` must be a list of three integers.')
-
-        poscar_data = poscar_data.to_dict() #
-        basis = poscar_data['basis'].copy() # Copy basis to avoid modifying original
-        positions = poscar_data['positions'].copy() # Copy positions to avoid modifying original
-        poscar_data['basis'] = basis[axes] # Transpose basis
-        poscar_data['positions'] = positions[:,axes] # Transpose positions
-        return serializer.PoscarData(poscar_data) # Return new POSCAR
+    if isinstance(axes, (list, tuple, np.ndarray)) and len(axes) == 3:
+        if not all(isinstance(i, (int, np.integer)) for i in axes):
+            raise ValueError("`axes` must be a list of three integers.")
+
+        poscar_data = poscar_data.to_dict()  #
+        basis = poscar_data["basis"].copy()  # Copy basis to avoid modifying original
+        positions = poscar_data[
+            "positions"
+        ].copy()  # Copy positions to avoid modifying original
+        poscar_data["basis"] = basis[axes]  # Transpose basis
+        poscar_data["positions"] = positions[:, axes]  # Transpose positions
+        return serializer.PoscarData(poscar_data)  # Return new POSCAR
     else:
-        raise Exception('`axes` must be a squence of length 3.')
+        raise Exception("`axes` must be a squence of length 3.")
+
 
 def add_atoms(poscar_data, name, positions):
     "Add atoms with a `name` to a POSCAR at given `positions` in fractional coordinates."
-    if name in poscar_data.unique.keys():
-        raise Exception(f'{name!r} already exists in POSCAR. Cannot add duplicate atoms.')
+    if name in poscar_data.types.keys():
+        raise Exception(
+            f"{name!r} already exists in POSCAR. Cannot add duplicate atoms."
+        )
 
     positions = np.array(positions)
     if (not np.ndim(positions) == 2) or (not positions.shape[1] == 3):
-        raise ValueError('`positions` must be a 2D array of shape (n,3)')
+        raise ValueError("`positions` must be a 2D array of shape (n,3)")
+
+    new_pos = np.vstack([poscar_data.positions, positions])  # Add new pos
+
+    unique = poscar_data.types.to_dict()  # avoid modifying original
+    unique[name] = range(len(poscar_data.positions), len(new_pos))
+
+    data = poscar_data.to_dict()  # Copy data to avoid modifying original
+    data["types"] = unique  # Update unique dictionary
+    data["positions"] = new_pos  # Update positions
+    data["SYSTEM"] = f'{data["SYSTEM"]}+{name}'  # Update SYSTEM
+    data["metadata"][
+        "comment"
+    ] = f'{data["metadata"]["comment"]} + Added {name!r}'  # Update comment
+
+    return serializer.PoscarData(data)  # Return new POSCAR
+
+
+def strain_poscar(poscar_data, strain_matrix):
+    "Strain a POSCAR by a given 3x3 `strain_matrix` to be multiplied with basis (elementwise) and return a new POSCAR."
+    if not isinstance(strain_matrix, np.ndarray):
+        strain_matrix = np.array(strain_matrix)
+
+    if strain_matrix.shape != (3, 3):
+        raise ValueError("`strain_matrix` must be a 3x3 matrix to multiply with basis.")
+
+    poscar_data = poscar_data.to_dict()  #
+    poscar_data["basis"] = (
+        poscar_data["basis"] * strain_matrix
+    )  # Update basis by elemetwise multiplication
+    poscar_data["metadata"][
+        "comment"
+    ] = f'{poscar_data["metadata"]["comment"]} + Strained POSCAR'  # Update comment
+    return serializer.PoscarData(poscar_data)  # Return new POSCAR
 
-    new_pos = np.vstack([poscar_data.positions,positions]) # Add new positions to existing ones
 
-    unique = poscar_data.unique.to_dict() # Copy unique dictionary to avoid modifying original
-    unique[name] = range(len(poscar_data.positions),len(new_pos)) # Add new unique element
+def view_poscar(poscar_data, **kwargs):
+    "View a POSCAR in a jupyter notebook. kwargs are passed to splot_lattice. After setting a view, you can do view.f(**view.kwargs) to get same plot in a cell."
 
-    data = poscar_data.to_dict() # Copy data to avoid modifying original
-    data['unique'] = unique # Update unique dictionary
-    data['positions'] = new_pos # Update positions
-    data['SYSTEM'] = f'{data["SYSTEM"]}+{name}' # Update SYSTEM
-    data['extra_info']['comment'] = f'{data["extra_info"]["comment"]} + Added {name!r}' # Update comment
+    def view(elev=30, azim=30, roll=0):
+        ax = splot_lattice(poscar_data, **kwargs)
+        ax.view_init(elev=elev, azim=azim, roll=roll)
 
-    return serializer.PoscarData(data) # Return new POSCAR
+    return interactive(view, elev=(0, 180), azim=(0, 360), roll=(0, 360))
```

### Comparing `ipyvasp-0.1.0/ipyvasp/utils.py` & `ipyvasp-0.2.0/ipyvasp/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,309 +1,421 @@
+__all__ = [
+    "get_file_size",
+    "set_dir",
+    "interpolate_data",
+    "rolling_mean",
+    "list_files",
+    "color",
+    "transform_color",
+    "create_colormap",
+]
+
 import re
 import os
-import glob
-from collections import namedtuple
-from subprocess import Popen, PIPE
 from contextlib import contextmanager
+from pathlib import Path
+from inspect import signature, getdoc
 
 
 import numpy as np
 from scipy.interpolate import make_interp_spline
 from scipy.ndimage.filters import convolve1d
 
+from matplotlib.colors import LinearSegmentedColormap
+import matplotlib.pyplot as plt
+
 
-def get_file_size(path):
+def get_file_size(path: str):
     """Return file size"""
-    if os.path.isfile(path):
-        size = os.stat(path).st_size
-        for unit in ['Bytes','KB','MB','GB','TB']:
+    if (p := Path(path)).is_file():
+        size = p.stat.st_size
+        for unit in ["Bytes", "KB", "MB", "GB", "TB"]:
             if size < 1024.0:
-                return "%3.2f %s" % (size,unit)
+                return "%3.2f %s" % (size, unit)
             size /= 1024.0
     else:
-        return ''
+        return ""
+
+
+def _sig_kwargs(from_func, skip_params=()):
+    "Add signature to decorated function form other function"
+
+    def wrapper(func, skip_params=skip_params):
+        sig = signature(from_func)
+        if not isinstance(skip_params, (list, tuple)):
+            raise TypeError("skip_params must be list or tuple")
+
+        this_sig = signature(func)
+        all_params = list(this_sig.parameters.values())
+        other_params = [
+            value for value in all_params if value.kind.name != "VAR_KEYWORD"
+        ]
+
+        if other_params == all_params:  # no **kwargs
+            return func
+
+        skip_params = list(skip_params) + [
+            value.name for value in other_params
+        ]  # skip params already in func as positional or keyword
+        target_params = [
+            value for value in sig.parameters.values() if value.name not in skip_params
+        ]
+        target_sig = sig.replace(parameters=other_params + target_params)
+        func.__signature__ = target_sig
+        return func
+
+    return wrapper
+
+
+def _sub_doc(from_func, replace={}):
+    """Assing __doc__ from other function. Replace words in docs where need."""
+
+    def wrapper(func):
+        docs = getdoc(from_func)
+        if not isinstance(replace, dict):
+            raise TypeError("replace must be dict of 'match':'replace'")
+
+        for k, v in replace.items():
+            docs = re.sub(k, v, docs, count=1, flags=re.DOTALL)
+        func.__doc__ = docs
+        return func
+
+    return wrapper
+
+
+def _fmt_doc(fmt_dict):
+    "Format docstring with keys from given dict"
+
+    def wrapper(func):
+        docs = func.__doc__  # Not by getdoc here, needs proper formatting
+        if not isinstance(fmt_dict, dict):
+            raise TypeError("fmt_dict must be dict of 'match':'replace'")
+        func.__doc__ = docs.format(**fmt_dict)
+        return func
+
+    return wrapper
+
 
 @contextmanager
-def set_dir(path):
-    "work in some directory and come back"
-    current = os.getcwd()
+def set_dir(path: str):
+    "Context manager to work in some directory and come back"
+    current = os.getcwd()  # not available in pathlib yet
     try:
         os.chdir(path)
         yield
     finally:
         os.chdir(current)
 
-def interpolate_data(x,y,n=10,k=3):
+
+def interpolate_data(x: np.ndarray, y: np.ndarray, n: int = 10, k: int = 3) -> tuple:
     """
-    - Returns interpolated xnew,ynew. If two points are same, it will add 0.1*min(dx>0) to compensate it.
-    - **Parameters**
-        - x: 1D array of size p,
-        - y: ndarray of size p*q*r,....
-        - n: Number of points to add between two given points.
-        - k: Polynomial order to interpolate.
-
-    - Only axis 0 will be interpolated. If you want general interploation, use `from scipy.interpolate import make_interp_spline, BSpline`
-
-    - **General Usage**: K(p),E(p,q) input from bandstructure.
-        - `Knew,Enew= interpolate_data(K,E,n=10,k=3)`. cubic interploation
-    """
-    #Add very small values at simliar points to make interpolation work.
-    ind=[i for i in range(0,len(x)) if x[i-1]==x[i]] #Duplicate indices
-    xa=np.unique(x)
-    dx=0.1*np.min(xa[1:]-xa[:-1])
-    if(ind):
-        for pt in ind:
-            x[pt:]=x[pt:]-x[pt]+x[pt-1]+dx
-    # Now Apply interpolation
-    xnew=[np.linspace(x[i],x[i+1],n) for i in range(len(x)-1)]
-    xnew=np.reshape(xnew,(-1))
-    spl = make_interp_spline(x, y, k=k) #BSpline object
-    ynew = spl(xnew)
-    return xnew,ynew
-
-def rolling_mean(X:np.ndarray, period:float, period_right:float = None, interface:float = None, mode:str = 'wrap', smoothness:int = 2) -> np.ndarray:
-    """Caluate rolling mean of array X using scipy.ndimage.filters.convolve1d.
-    
-    - **Parameters**
-        - X: 1D numpy array.
-        - period: float in range [0,1]. Period of rolling mean. Applies left side of X from center if period_right is given.
-        - period_right: float in range [0,1]. Period of rolling mean on right side of X from center.
-        - interface: float in range [0,1]. The point that divides X into left and right, like in a slab calculation.
-        - mode: string. Mode of convolution. Default is wrap to keep periodcity of crystal in slab caluation. Read scipy.ndimage.filters.convolve1d for more info.
-        - smoothness: int. Default is 2. Order of making the output smoother. Larger is better but can't be too large as there will be points lost at each convolution.
-    
-    Returns convolved array of same size as X if mode is 'wrap'. May be smaller if mode is something else.
+    Returns interpolated xnew,ynew. If two points are same, it will add 0.1*min(dx>0) to compensate it.
+
+    Parameters
+    ----------
+    x : ndarry, 1D array of size p,
+    y : ndarray, ndarray of size p*q*r,....
+    n : int, Number of points to add between two given points.
+    k : int, Polynomial order to interpolate.
+
+
+    Example
+    -------
+    For ``K(p),E(p,q)`` input from bandstructure, do ``Knew, Enew = interpolate_data(K,E,n=10,k=3)`` for cubic interploation.
+
+    Returns
+    -------
+    tuple: (xnew, ynew) after interpolation.
+
+
+    .. note::
+        Only axis 0 will be interpolated. If you want general interploation, use ``from scipy.interpolate import make_interp_spline, BSpline``.
+    """
+    # Avoid adding points between same points, like in kpath patches
+    inds = [i for i in range(0, len(x)) if x[i - 1] == x[i]]  # Duplicate indices
+    if inds:
+        inds = [0, *inds, len(x)]  # Indices to split x
+        ranges = list(zip(inds[:-1], inds[1:]))  # we are using this twice,so make list
+        for p, q in ranges:
+            if q - p == 1:  # means three consecutive points have same value
+                raise ValueError(
+                    f"Three or more duplicate values found at index {p} in array `x`, at most two allowed for broken kpath like scenario."
+                )
+        arrays = [[x[i:j], y[i:j]] for i, j in ranges]  # Split x,y into arrays
+    else:
+        arrays = [(x, y)]
+
+    new_as, new_bs = [], []
+    for a, b in arrays:
+        anew = [np.linspace(a[i], a[i + 1], n) for i in range(len(a) - 1)]
+        anew = np.reshape(anew, (-1))
+        spl = make_interp_spline(a, b, k=k)  # BSpline object
+        bnew = spl(anew)
+        new_as.append(anew)
+        new_bs.append(bnew)
+
+    if len(new_as) == 1:
+        return new_as[0], new_bs[0]
+
+    return np.concatenate(new_as, axis=0), np.concatenate(new_bs, axis=0)
+
+
+def rolling_mean(
+    X: np.ndarray,
+    period: float,
+    period_right: float = None,
+    interface: float = None,
+    mode: str = "wrap",
+    smoothness: int = 2,
+) -> np.ndarray:
+    """
+    Caluate rolling mean of array X using scipy.ndimage.filters.convolve1d.
+
+    Parameters
+    ----------
+    X : ndarray, 1D numpy array.
+    period : float, In range [0,1]. Period of rolling mean. Applies left side of X from center if period_right is given.
+    period_right : float, In range [0,1]. Period of rolling mean on right side of X from center.
+    interface : float, In range [0,1]. The point that divides X into left and right, like in a slab calculation.
+    mode : string, Mode of convolution. Default is wrap to keep periodcity of crystal in slab caluation. Read scipy.ndimage.filters.convolve1d for more info.
+    smoothness : int, Default is 2. Order of making the output smoother. Larger is better but can't be too large as there will be points lost at each convolution.
+
+    Returns
+    -------
+    ndarray: convolved array of same size as X if mode is 'wrap'. May be smaller if mode is something else.
     """
     if period_right is None:
         period_right = period
-    
+
     if interface is None:
         interface = 0.5
-        
+
     if smoothness < 1:
-        raise ValueError('smoothness must be >= 1')
-    
-    wx = np.linspace(0, 1, X.size, endpoint = False) # x-axis for making weights for convolution, 0 to 1 - (last point is not included in VASP grid).
-    x1, x2, x3, x4 = period_right, interface - period, interface + period_right, 1 - period
-    m1, m2, m3 = 0.5/x1, 1/(x2-x3), 0.5/(1-x4) # Slopes
-    weights_L = np.piecewise(wx,  # .----.____. Looks like this
-                [
-                    wx < x1, # left side reflected by right side
-                    (wx >= x1) & (wx <= x2), # left side
-                    (wx > x2) & (wx<x3), # middle contribution from left and right
-                    (wx>=x3) & (wx<=x4), # right side
-                    wx > x4 # right side reflected by left side
-                ], 
-                [
-                    lambda z:  m1*(z-x1)+1,
-                    1, 
-                    lambda z: m2*(z-x2) + 1,
-                    0, 
-                    lambda z: m3*(z-x4)
-                ])
-    
-    weights_R =  1 - weights_L # .____.----. Looks like this
-    
-    L = int(period*X.size) # Left periodictity
-    R = int(period_right*X.size) # Right Periodicity
-    
-    kernel_L = np.ones((L,))/L
-    kernel_R = np.ones((R,))/R
-    
-    mean_L = convolve1d(X,kernel_L,mode = mode)
-    mean_R = convolve1d(X,kernel_R,mode = mode)
-    
-    mean_all = weights_L*mean_L + weights_R*mean_R
-    
+        raise ValueError("smoothness must be >= 1")
+
+    wx = np.linspace(
+        0, 1, X.size, endpoint=False
+    )  # x-axis for making weights for convolution, 0 to 1 - (last point is not included in VASP grid).
+    x1, x2, x3, x4 = (
+        period_right,
+        interface - period,
+        interface + period_right,
+        1 - period,
+    )
+    m1, m2, m3 = 0.5 / x1, 1 / (x2 - x3), 0.5 / (1 - x4)  # Slopes
+    weights_L = np.piecewise(
+        wx,  # .----.____. Looks like this
+        [
+            wx < x1,  # left side reflected by right side
+            (wx >= x1) & (wx <= x2),  # left side
+            (wx > x2) & (wx < x3),  # middle contribution from left and right
+            (wx >= x3) & (wx <= x4),  # right side
+            wx > x4,  # right side reflected by left side
+        ],
+        [
+            lambda z: m1 * (z - x1) + 1,
+            1,
+            lambda z: m2 * (z - x2) + 1,
+            0,
+            lambda z: m3 * (z - x4),
+        ],
+    )
+
+    weights_R = 1 - weights_L  # .____.----. Looks like this
+
+    L = int(period * X.size)  # Left periodictity
+    R = int(period_right * X.size)  # Right Periodicity
+
+    kernel_L = np.ones((L,)) / L
+    kernel_R = np.ones((R,)) / R
+
+    mean_L = convolve1d(X, kernel_L, mode=mode)
+    mean_R = convolve1d(X, kernel_R, mode=mode)
+
+    mean_all = weights_L * mean_L + weights_R * mean_R
+
     if smoothness > 1:
-        p_l, p_r = period/2, period_right/2 # Should be half of period for smoothing each time
+        p_l, p_r = (
+            period / 2,
+            period_right / 2,
+        )  # Should be half of period for smoothing each time
         for _ in range(smoothness - 1):
-            mean_all = rolling_mean(mean_all, period = p_l, period_right = p_r, interface = interface, mode = mode, smoothness = 1)
-            p_l, p_r = p_l/2, p_r/2
-    
+            mean_all = rolling_mean(
+                mean_all,
+                period=p_l,
+                period_right=p_r,
+                interface=interface,
+                mode=mode,
+                smoothness=1,
+            )
+            p_l, p_r = p_l / 2, p_r / 2
+
     return mean_all
 
-def ps2py(ps_command='Get-ChildItem', exec_type='-Command', path_to_ps='powershell.exe'):
+
+def list_files(path=".", glob="*", exclude=None, files_only=False, dirs_only=False):
     """
-    - Captures powershell output in python.
-    - **Parameters**
-        - ps_command: enclose ps_command in ' ' or " ".
-        - exec_type : type of execution, default '-Command', could be '-File'.
-        - path_to_ps: path to powerhell.exe if not added to PATH variables.
-    """
-    try: # Works on Linux and Windows if PS version > 5.
-        cmd = ['pwsh', '-ExecutionPolicy', 'Bypass', exec_type, ps_command]
-        proc = Popen(cmd, stdout=PIPE, stderr=PIPE)
-    except FileNotFoundError:
-        try: # Works only on Windows.
-            cmd = ['powershell', '-ExecutionPolicy', 'Bypass', exec_type, ps_command]
-            proc = Popen(cmd, stdout=PIPE, stderr=PIPE)
-        except FileNotFoundError:
-            # Works in case nothing above works and you know where is executable.
-            cmd = [path_to_ps, '-ExecutionPolicy', 'Bypass', exec_type, ps_command]
-            proc = Popen(cmd, stdout=PIPE, stderr=PIPE)
-
-    out=[]; #save to out.
-    while True:
-        line = proc.stdout.readline()
-        if line!=b'':
-            line=line.strip()
-            u_line=line.decode("utf-8")
-            out.append(u_line)
-        else:
-            break
-    out=[item for item in out if item!=''] #filter out empty lines
-    return out
-
-def ps2std(ps_command='Get-ChildItem', exec_type='-Command', path_to_ps='powershell.exe'):
-    """
-    - Prints powershell output in python std.
-    - **Parameters**
-        - ps_command: enclose ps_command in ' ' or " ".
-        - exec_type: type of execution, default '-Command', could be '-File'.
-        - path_to_ps: path to powerhell.exe if not added to PATH variables.
-    """
-    out = ps2py(path_to_ps=path_to_ps,exec_type=exec_type,ps_command=ps_command)
-    for item in out:
-        print(item)
-    return None
-
-
-def get_child_items(path = os.getcwd(),depth=None,recursive=True,include=None,exclude=None,filesOnly=False,dirsOnly= False):
-    """
-    - Returns selected directories/files recursively from a parent directory.
-    - **Parameters**
-        - path    : path to a parent directory, default is `"."`
-        - depth   : int, subdirectories depth to get recursively, default is None to list all down.
-        - recursive : If False, only list current directory items, if True,list all items recursively down the file system.
-        - include: Default is None and includes everything. String of patterns separated by | to keep, could be a regular expression.
-        - exclude: Default is None and removes nothing. String of patterns separated by | to drop,could be a regular expression.
-        - filesOnly : Boolean, if True, returns only files.
-        - dirsOnly  : Boolean, if True, returns only directories.
-    - **Returns**
-        - GLOB : Tuple (children,parent), children is list of selected directories/files and parent is given path. Access by index of by `get_child_items().{children,path}`.
-    """
-    path = os.path.abspath(path) # important
-    pattern = path + '**/**' # Default pattern
-    if depth != None and type(depth) == int:
-        pattern = path + '/'.join(['*' for i in range(depth+1)])
-        if glob.glob(pattern) == []: #If given depth is more, fall back.
-            pattern = path + '**/**' # Fallback to default pattern if more depth to cover all.
-    glob_files = glob.iglob(pattern, recursive=recursive)
-    if dirsOnly == True:
-        glob_files = filter(lambda f: os.path.isdir(f),glob_files)
-    if filesOnly == True:
-        glob_files = filter(lambda f: os.path.isfile(f),glob_files)
-    list_dirs=[]
-    for g_f in glob_files:
-        list_dirs.append(os.path.relpath(g_f,path))
-    # Include check
-    if include:
-        list_dirs = [l for l in list_dirs if re.search(include,l)]
-    # Exclude check
+    Returns a tuple of files in a directory recursively based on glob pattern.
+
+    Parameters
+    ----------
+    path : str, current directory by default
+    glob : str, glob pattern, '*' by default
+    exclude : str, regular expression pattern to exclude files
+    files_only : bool, if True, returns only files
+    dirs_only : bool, if True, returns only directories
+
+    Returns
+    -------
+    tuple of pathlib.Path objects
+    """
+    if files_only and dirs_only:
+        raise ValueError("files_only and dirs_only cannot be both True")
+
+    path = Path(path)
+    files = [p for p in path.glob(glob)]
     if exclude:
-        list_dirs = [l for l in list_dirs if not re.search(exclude,l)]
-    # Keep only unique
-    req_dirs = list(np.unique(list_dirs))
-    out_files = namedtuple('GLOB',['children','parent'])
-    return out_files(req_dirs,os.path.abspath(path))
-
-def prevent_overwrite(path):
-    """Prevents overwiting as file/directory by adding numbers in given file/directory path."""
-    if os.path.exists(path):
-        name, ext = os.path.splitext(path)
+        files = [p for p in files if not re.search(exclude, str(p))]
+    if files_only:
+        files = [p for p in files if p.is_file()]
+    if dirs_only:
+        files = [p for p in files if p.is_dir()]
+    return tuple(files)
+
+
+@contextmanager
+def prevent_overwrite(path) -> Path:
+    """Contextmanager to prevents overwiting as file by adding numbers in given path.
+
+    >>> with prevent_overwrite("file.txt") as path:
+    >>>     print(path) # file.txt if it doesn't exist, file-1.txt if it exists, file-2.txt if file-1.txt exists and so on.
+    """
+    out_path = Path(path)
+    if out_path.exists():
         # Check existing files
         i = 0
-        _path = name + '-{}' + ext
-        while os.path.isfile(_path.format(i)):
-            i +=1
-        out_path = _path.format(i)
+        name = out_path.stem + "-{}" + out_path.suffix
+        while Path(name.format(i)).is_file():
+            i += 1
+        out_path = Path(name.format(i))
         print(f"Found existing path: {path!r}\nConverting to: {out_path!r}")
-        return out_path
-    return path
+
+    yield out_path
+
 
 class color:
-     def bg(text,r,g,b):
-          """Provide r,g,b component in range 0-255"""
-          return f"\033[48;2;{r};{g};{b}m{text}\033[00m"
-     def fg(text,r,g,b):
-          """Provide r,g,b component in range 0-255"""
-          return f"\033[38;2;{r};{g};{b}m{text}\033[00m"
-     # Usual Colos
-     r  = lambda text: f"\033[0;91m {text}\033[00m"
-     rb = lambda text: f"\033[1;91m {text}\033[00m"
-     g  = lambda text: f"\033[0;92m {text}\033[00m"
-     gb = lambda text: f"\033[1;92m {text}\033[00m"
-     b  = lambda text: f"\033[0;34m {text}\033[00m"
-     bb = lambda text: f"\033[1;34m {text}\033[00m"
-     y  = lambda text: f"\033[0;93m {text}\033[00m"
-     yb = lambda text: f"\033[1;93m {text}\033[00m"
-     m  = lambda text: f"\033[0;95m {text}\033[00m"
-     mb = lambda text: f"\033[1;95m {text}\033[00m"
-     c  = lambda text: f"\033[0;96m {text}\033[00m"
-     cb = lambda text: f"\033[1;96m {text}\033[00m"
-
-def nav_links(current_index=0,
-            doc_url = r"https://massgh.github.io/ipyvasp/",
-            items   = ["Index",
-                       "Example",
-                       "StaticPlots",
-                       "InteractivePlots",
-                       "SpinProjectedSurfaces",
-                       "StructureIO",
-                       "Widgets",
-                       "MainAPI",
-                       ],
-            horizontal = False,
-            out_string = False):
-    from IPython.display import Markdown
-    links   = [doc_url+item if not 'Index' in item else doc_url for item in items]
-    style = """<style>a{text-decoration: none !important;color:lightkblue;font-weight:bold;}
-                a:focus,a:active,a:hover{color:hotpink !important;}</style>\n"""
-    md_str = style
-    for i,(link,item) in enumerate(zip(links,items)):
-        if current_index == i: item = "{}●".format(item)
-        if not horizontal:
-            md_str += "> [&nbsp;`▶` {}&nbsp;]({})  \n".format(item,link)
-        else:
-            md_str += "> [&nbsp;`▶` {}&nbsp;]({})\n".format(item,link)
-    if out_string:
-        return md_str
-    return Markdown(md_str)
-
-def transform_color(arr,s=1,c=1,b=0,mixing_matrix=None):
-    """
-    - Color transformation such as brightness, contrast, saturation and mixing of an input color array. `c = -1` would invert color,keeping everything else same.
-    - **Parameters**
-        - arr: input array, a single RGB/RGBA color or an array with inner most dimension equal to 3 or 4. e.g. [[[0,1,0,1],[0,0,1,1]]].
-        - c  : contrast, default is 1. Can be a float in [-1,1].
-        - s  : saturation, default is 1. Can be a float in [-1,1]. If s = 0, you get a gray scale image.
-        - b  : brightness, default is 0. Can be a float in [-1,1] or list of three brightnesses for RGB components.
-        - mixing_matrix: A 3x3 matrix to mix RGB values, such as `pp.color_matrix`.
-
-    [Recoloring](https://docs.microsoft.com/en-us/windows/win32/gdiplus/-gdiplus-recoloring-use?redirectedfrom=MSDN)
-    [Rainmeter](https://docs.rainmeter.net/tips/colormatrix-guide/)
-    """
-    arr = np.array(arr) # Must
-    t = (1-c)/2 # For fixing gray scale when contrast is 0.
-    whiteness = np.array(b)+t # need to clip to 1 and 0 after adding to color.
-    sr = (1-s)*0.2125 #red saturation from red luminosity
-    sg = (1-s)*0.7154 #green saturation from green luminosity
-    sb = (1-s)*0.0721 #blue saturation from blue luminosity
+    def bg(text, r, g, b):
+        """Provide r,g,b component in range 0-255"""
+        return f"\033[48;2;{r};{g};{b}m{text}\033[00m"
+
+    def fg(text, r, g, b):
+        """Provide r,g,b component in range 0-255"""
+        return f"\033[38;2;{r};{g};{b}m{text}\033[00m"
+
+    # Usual Colos
+    r = lambda text: f"\033[0;91m {text}\033[00m"
+    rb = lambda text: f"\033[1;91m {text}\033[00m"
+    g = lambda text: f"\033[0;92m {text}\033[00m"
+    gb = lambda text: f"\033[1;92m {text}\033[00m"
+    b = lambda text: f"\033[0;34m {text}\033[00m"
+    bb = lambda text: f"\033[1;34m {text}\033[00m"
+    y = lambda text: f"\033[0;93m {text}\033[00m"
+    yb = lambda text: f"\033[1;93m {text}\033[00m"
+    m = lambda text: f"\033[0;95m {text}\033[00m"
+    mb = lambda text: f"\033[1;95m {text}\033[00m"
+    c = lambda text: f"\033[0;96m {text}\033[00m"
+    cb = lambda text: f"\033[1;96m {text}\033[00m"
+
+
+def transform_color(
+    arr: np.ndarray,
+    s: float = 1,
+    c: float = 1,
+    b: float = 0,
+    mixing_matrix: np.ndarray = None,
+) -> np.ndarray:
+    """
+    Color transformation such as brightness, contrast, saturation and mixing of an input color array. ``c = -1`` would invert color,keeping everything else same.
+
+    Parameters
+    ----------
+    arr : ndarray, input array, a single RGB/RGBA color or an array with inner most dimension equal to 3 or 4. e.g. [[[0,1,0,1],[0,0,1,1]]].
+    c : float, contrast, default is 1. Can be a float in [-1,1].
+    s : float, saturation, default is 1. Can be a float in [-1,1]. If s = 0, you get a gray scale image.
+    b : float, brightness, default is 0. Can be a float in [-1,1] or list of three brightnesses for RGB components.
+    mixing_matrix : ndarray, A 3x3 matrix to mix RGB values, such as `ipyvas.utils.color_matrix`.
+
+    Returns
+    -------
+    ndarray: Transformed color array of same shape as input array.
+
+    See `Recoloring <https://docs.microsoft.com/en-us/windows/win32/gdiplus/-gdiplus-recoloring-use?redirectedfrom=MSDN>`_
+    and `Rainmeter <https://docs.rainmeter.net/tips/colormatrix-guide/>`_ for useful information on color transformation.
+    """
+    arr = np.array(arr)  # Must
+    t = (1 - c) / 2  # For fixing gray scale when contrast is 0.
+    whiteness = np.array(b) + t  # need to clip to 1 and 0 after adding to color.
+    sr = (1 - s) * 0.2125  # red saturation from red luminosity
+    sg = (1 - s) * 0.7154  # green saturation from green luminosity
+    sb = (1 - s) * 0.0721  # blue saturation from blue luminosity
     # trans_matrix is multiplied from left, or multiply its transpose from right.
     # trans_matrix*color is not normalized but value --> value - int(value) to keep in [0,1].
-    trans_matrix = np.array([
-        [c*(sr+s), c*sg,      c*sb],
-        [c*sr,   c*(sg+s),    c*sb],
-        [c*sr,     c*sg,  c*(sb+s)]])
+    trans_matrix = np.array(
+        [
+            [c * (sr + s), c * sg, c * sb],
+            [c * sr, c * (sg + s), c * sb],
+            [c * sr, c * sg, c * (sb + s)],
+        ]
+    )
     if np.ndim(arr) == 1:
-        new_color = np.dot(trans_matrix,arr)
+        new_color = np.dot(trans_matrix, arr)
     else:
-        new_color = np.dot(arr[...,:3],trans_matrix.T)
-    if mixing_matrix is not None and np.size(mixing_matrix)==9:
-        new_color = np.dot(new_color,np.transpose(mixing_matrix))
-    new_color[new_color > 1] = new_color[new_color > 1] - new_color[new_color > 1].astype(int)
-    new_color = np.clip(new_color + whiteness,a_max=1,a_min=0)
-    if np.shape(arr)[-1]==4:
-        axis = len(np.shape(arr))-1 #Add back Alpha value if present
-        new_color = np.concatenate([new_color,arr[...,3:]],axis=axis)
-    return new_color
+        new_color = np.dot(arr[..., :3], trans_matrix.T)
+    if mixing_matrix is not None and np.size(mixing_matrix) == 9:
+        new_color = np.dot(new_color, np.transpose(mixing_matrix))
+    new_color[new_color > 1] = new_color[new_color > 1] - new_color[
+        new_color > 1
+    ].astype(int)
+    new_color = np.clip(new_color + whiteness, a_max=1, a_min=0)
+    if np.shape(arr)[-1] == 4:
+        axis = len(np.shape(arr)) - 1  # Add back Alpha value if present
+        new_color = np.concatenate([new_color, arr[..., 3:]], axis=axis)
+    return new_color
+
+
+# color_marices for quick use
+color_matrix = np.array(
+    [[0.5, 0, 0.5, 1], [0.5, 0.5, 0, 1], [0, 0.5, 0.5, 0.2], [1, 1, 0.2, 0]]
+)  # lights up to see colors a little bit
+rbg_matrix = np.array([[1, 0, 0], [0, 0, 1], [0, 1, 0]])  # Red, Blue, Green
+cmy_matrix = np.array(
+    [[0, 0.5, 0.5, 1], [0.5, 0, 0.5, 1], [0.5, 0.5, 0, 0.2], [1, 1, 0.2, 0]]
+)  # Generates CMYK color palette
+
+
+# Register 'RGB' colormap in current session
+RGB = LinearSegmentedColormap.from_list(
+    "RGB", [(0.9, 0, 0), (0.9, 0.9, 0), (0, 0.9, 0), (0, 0.9, 0.9), (0, 0, 0.9)]
+)
+CMY = LinearSegmentedColormap.from_list(
+    "CMY", [(0, 0.9, 0.9), (0, 0, 0.9), (0.9, 0, 0.9), (0.9, 0, 0), (0.9, 0.9, 0)]
+)
+plt.register_cmap("RGB", RGB)
+plt.register_cmap("CMY", CMY)
+
+
+def create_colormap(name="RB", colors=[(0.9, 0, 0), (0, 0, 0.9)]):
+    """
+    Create and register a custom colormap from a list of RGB colors. and then use it's name in plottoing functions to get required colors.
+
+    Parameters
+    ----------
+    name: str, name of the colormap
+    colors: list of RGB colors, e.g. [(0.9,0,0),(0,0,0.9)] or named colors, e.g. ['red','blue'], add as many colors as you want.
+
+    Returns
+    -------
+    Colormap object which you can use to get colors from. like cm = create_colormap(); cm(0.5) which will return a color at center of map
+    """
+    RB = LinearSegmentedColormap.from_list(name, colors)
+    plt.register_cmap(name, RB)
+    return RB
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

