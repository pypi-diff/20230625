# Comparing `tmp/WIDscript-1.0.8.tar.gz` & `tmp/WIDscript-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WIDscript-1.0.8.tar", last modified: Wed Jun 21 03:55:51 2023, max compression
+gzip compressed data, was "WIDscript-1.1.0.tar", last modified: Sat Jun 24 19:09:57 2023, max compression
```

## Comparing `WIDscript-1.0.8.tar` & `WIDscript-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 03:55:51.485722 WIDscript-1.0.8/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      520 2023-06-21 03:55:51.486723 WIDscript-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-06-21 01:38:12.000000 WIDscript-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      661 2023-06-21 03:55:51.487723 WIDscript-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 03:55:51.464723 WIDscript-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:55:51.474722 WIDscript-1.0.8/src/WIDscript/
--rw-rw-rw-   0        0        0    26867 2023-06-21 03:55:26.000000 WIDscript-1.0.8/src/WIDscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:55:51.485722 WIDscript-1.0.8/src/WIDscript.egg-info/
--rw-rw-rw-   0        0        0      520 2023-06-21 03:55:51.000000 WIDscript-1.0.8/src/WIDscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-21 03:55:51.000000 WIDscript-1.0.8/src/WIDscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 03:55:51.000000 WIDscript-1.0.8/src/WIDscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-21 03:55:51.000000 WIDscript-1.0.8/src/WIDscript.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 19:09:57.165715 WIDscript-1.1.0/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-06-24 19:09:57.166714 WIDscript-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-21 01:38:12.000000 WIDscript-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      661 2023-06-24 19:09:57.168219 WIDscript-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 19:09:57.145676 WIDscript-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 19:09:57.152196 WIDscript-1.1.0/src/WIDscript/
+-rw-rw-rw-   0        0        0    26517 2023-06-24 02:23:53.000000 WIDscript-1.1.0/src/WIDscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:09:57.165715 WIDscript-1.1.0/src/WIDscript.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-06-24 19:09:57.000000 WIDscript-1.1.0/src/WIDscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-24 19:09:57.000000 WIDscript-1.1.0/src/WIDscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:09:57.000000 WIDscript-1.1.0/src/WIDscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 19:09:57.000000 WIDscript-1.1.0/src/WIDscript.egg-info/top_level.txt
```

### Comparing `WIDscript-1.0.8/PKG-INFO` & `WIDscript-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WIDscript
-Version: 1.0.8
+Version: 1.1.0
 Summary: A private wrapper made for WIDOWN releases.
 Home-page: https://github.com/pypa/sampleproject
 Author: WIDOWN
 Author-email: widown.ma@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WIDscript-1.0.8/setup.cfg` & `WIDscript-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2057 4944 7363 7269 7074 0d0a 7665   = WIDscript..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a61  rsion = 1.0.8..a
+00000020: 7273 696f 6e20 3d20 312e 312e 300d 0a61  rsion = 1.1.0..a
 00000030: 7574 686f 7220 3d20 5749 444f 574e 0d0a  uthor = WIDOWN..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2077  author_email = w
 00000050: 6964 6f77 6e2e 6d61 4067 6d61 696c 2e63  idown.ma@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7072 6976 6174 6520 7772 6170  = A private wrap
 00000080: 7065 7220 6d61 6465 2066 6f72 2057 4944  per made for WID
 00000090: 4f57 4e20 7265 6c65 6173 6573 2e0d 0a6c  OWN releases...l
```

### Comparing `WIDscript-1.0.8/src/WIDscript/__init__.py` & `WIDscript-1.1.0/src/WIDscript/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,96 +12,144 @@
 # If you have acquired this content from any other source, it may not be genuine.
 # It could have been "stolen" or someone could be impersonating us.
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 # WIDscript
 
+from    enum           import Enum
+
 from    vapoursynth    import core
 import  vapoursynth    as vs
 
 core = vs.core
 
 from    vskernels      import Hermite, BSpline, Mitchell
-from    dfttest2       import DFTTest, Backend
-from    denoiseMC      import denoiseMC
-from    havsfunc       import SMDegrain, DeHalo_alpha, HQDeringmod
+from    dfttest2       import DFTTest
+from    havsfunc       import DeHalo_alpha, HQDeringmod
 from    kagefunc       import retinex_edgemask
 from    vsmasktools    import retinex
 from    vsdpir_ncnn    import DPIR
 from    vsTAAmbk       import TAAmbk
 from    vsscale        import SSIM
 from    vstools        import finalize_clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
+class cFormatEnum(str, Enum):
+    YUV420P10 = "YUV420P10",
+    YUV420P16 = "YUV420P16",
+    RGBS      = "RGBS"
+    
+############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
+
+def format(clip    : vs.VideoNode,
+           cFormat : cFormatEnum = cFormatEnum.YUV420P16) :
+        
+    match cFormat :
+        case "YUV420P10":
+            if (clip.format.name != cFormatEnum.YUV420P10) : clip = core.resize.Spline36(clip, format=vs.YUV420P10, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+        case "YUV420P16":
+            if (clip.format.name != cFormatEnum.YUV420P16) : clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+        case "RGBS":
+            if (clip.format.name != cFormatEnum.RGBS)      : clip = core.resize.Spline36(clip, format=vs.RGBS, matrix_in_s="709", dither_type="error_diffusion")
+        case _:
+            raise ValueError("Invalid value")
+                 
+    return clip
+
+############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
+
 def initClip(clip,
-             fps      : int  = 24000,
-             floatFPS : bool = True) :
-             
+             isInterlaced  : bool = False,
+             setResolution : bool = False,
+             siWidth       : int  = 704,
+             siHeight      : int  = 480,
+             fps           : int  = 24000,
+             floatFPS      : bool = True) :
+    
     # Importing the video
     clip = core.lsmas.LWLibavSource(clip)
-
+    
+    if (isInterlaced == True) :
+        
+        #Restores Progressive Frames
+        clip = core.vivtc.VFM(clip, order=1, cthresh=10)
+
+        #Restores framerate to 23.976fps from 29.97fps by removing duplicate frames.
+        clip = core.vivtc.VDecimate(clip)
+        
+    if (setResolution == True) :
+        
+        # Changes Aspect Ratio to Fullscreen
+        clip = clip.resize.Spline36(siWidth, siHeight, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+        
     # Verifying whether FPS are float or not, in order to then define the FPS of the source.
     clip = clip.std.AssumeFPS(fpsnum=fps, fpsden=1001) if (floatFPS == True) else clip.std.AssumeFPS(fpsnum=fps)
 
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
-def splice_clip(clip              : vs.VideoNode,
+def spliceClip(clip              : vs.VideoNode,
                 source            : vs.VideoNode,
-                parameters_slice,
+                parameters_slice  : dict = None,
                 useInOut          : bool = False,
-                inOutPath                = None) :
-    
-    slice         = everything(source, **parameters_slice) if (useInOut == False) else initClip(inOutPath)
+                inOutPath         : str  = None) :
     
-    start, end    = parameters_slice['start'], parameters_slice['end']
+    start, end    = parameters_slice['start'], parameters_slice['end'] + 1
+    if (start == None or end == None or end == 1) : raise ValueError("'None' isn't a valid value !")
+
+    if (useInOut == True and inOutPath == None)   : raise ValueError("'None' isn't a valid path !")
     
-    clip          = core.std.Splice([clip[:start], slice, clip[end:]])
+    slice = everything(source, **parameters_slice) if (useInOut == False) else initClip(inOutPath)
+    clip  = core.std.Splice([clip[:start], slice, clip[end:]])
     
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def downscale(clip     : vs.VideoNode,
               dsWidth  : int = 1920,
               dsHeight : int = 1080) :
 
-    clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip)
 
     # Downscaling using high quality algo.
     clip = SSIM.scale(clip, dsWidth, dsHeight)
 
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def hdr2SDR(clip    : vs.VideoNode,
             dst_max : int   = 110,
             src_max : int   = 4000,
             src_min : float = 0.0050) :
     
-    clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip)
 
     # Tonemapping for HDR to SDR. Change src_max and src_min according to the source.
     clip = core.placebo.Tonemap(clip, src_csp=1, dst_csp=0, dst_prim=3, dynamic_peak_detection=1, dst_max=dst_max, src_max=src_max, src_min=src_min, tone_mapping_function=6, tone_mapping_mode=4, gamut_mode=0)
 
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def mage(clip             : vs.VideoNode,
          thsxdxMultiplier : float = 0.65) :
 
-    # The "MAGE" function aims to fix any issues present in the original video clip such as agressive noise, while preserving details and improving sharpness.
+    """## MAGE - Managing All Grain Elegantly, made by Clybius and modified by WIDOWN.
+    
+    The "MAGE" function aims to fix any issues present in the original video clip such as agressive noise, while preserving details and improving sharpness.\n
+    It is recommended to use it for anim-type content because otherwise, it can create "wrapping" effects, similar to those caused by AI video interpolation.
+    
+    """
 
-    # Defining a YUV420P16 variable for further filtering with MAGE script.
-    clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip)
 
     # all levels for MAnalyse
     super = core.mv.Super(clip, hpad=32, vpad=32, rfilter=4)
 
     # Truemotion for max denoising on original vid
     backward2 = core.mv.Analyse(super, isb=True, blksize=32, overlap=16, delta=2, search=5, truemotion=True)
     backward  = core.mv.Analyse(super, isb=True, blksize=32, overlap=16, search=5, truemotion=True)
@@ -150,152 +198,114 @@
     # Take original clip, and apply it on top of the denoised clip via the mask.
     clipDN = core.std.MaskedMerge(clipDN, clip, dmask, planes=0)
 
     # 2nd pass light denoise, lower or raise `sigma` for lower or higher strength.
     clipDN = DFTTest(clipDN, sigma=0.9, tbsize=3, ssystem=1)
 
     # Bicubic Spline Desharpening
-    clipDNS = clipDN # Copy clip
-
-    clipDNSU = Hermite().scale(clipDNS, clipDN.width * 1.5, clipDN.height * 1.5) # Resize using hermite bicubic (0,1)
-    clipDNU  = BSpline().scale(clipDN, clipDN.width * 1.5, clipDN.height * 1.5) # Base bspline (0,0)
-
-    clipDNS = core.std.MakeDiff(clipDNU, clipDNSU) # Make diff of the two
-    clipDNS = Mitchell().scale(clipDNS, clipDN.width, clipDN.height) # Scale down using "natural" bicubic (0.333, 0.333)
-
-    clipDN = core.std.MergeDiff(clipDN, clipDNS) # Finally, merge together
-
-    return clipDN
-
-############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
-
-def ddn(clip           : vs.VideoNode,
-        bm3dSigma      : float = 0.3,
-        ddnRemBinarize : int   = 500,
-        smdThSAD       : int   = 250) :
+    clipDNS  = clipDN
     
-    # WARNING : OUTDATED.
+    clipDNSU = Hermite().scale(clipDNS, clipDN.width * 1.5, clipDN.height * 1.5)
+    clipDNU  = BSpline().scale(clipDN, clipDN.width * 1.5, clipDN.height * 1.5)
     
-    # The "DDN" function is designed to enhance the quality of a video clip by addressing common issues such as noise and banding.
+    clipDNS  = core.std.MakeDiff(clipDNU, clipDNSU)
     
-    clip_YUV420P16 = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
-
-    # Defining motion compensated denoising.
-    def denoised_dft(clip_YUV420P16) :
-        return DFTTest(clip_YUV420P16, sigma=8, backend=Backend.CPU, tbsize=5)
-
-    # First pass denoising using denoiseMC, then converting to RGBS for BM3D.
-    _1p_denoising = denoiseMC(clip_YUV420P16, radius=5, denoise_fn=denoised_dft)
-    _1p_denoising = core.resize.Spline36(_1p_denoising, format=vs.RGBS, matrix_in_s="709", dither_type="error_diffusion")
-
-    # Denoising using BM3D to create a denoised edge clip, using the first pass denoising as ref, then converting to YUV420P16.
-    denoised_edgeclip = core.resize.Spline36(clip, format=vs.RGBS, matrix_in_s="709", dither_type="error_diffusion")
-    denoised_edgeclip = core.bm3dcpu.BM3D(denoised_edgeclip, ref=_1p_denoising, sigma=bm3dSigma, chroma=False)
-    denoised_edgeclip = core.resize.Spline36(denoised_edgeclip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
-
-    # Creating a retinex edge mask before applying SMDegrain to keep fine details.
-    mask = retinex_edgemask(denoised_edgeclip).std.Binarize(ddnRemBinarize).std.Inflate()
-
-    # Second pass denoising using BM3D on the first pass denoising, then converting to YUV420P16 for the third pass.
-    _2p_denoising = core.bm3dcpu.BM3D(_1p_denoising, sigma=bm3dSigma, chroma=False)
-    _2p_denoising = core.resize.Spline36(_2p_denoising, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
-
-    # Third pass denoising using SMDegrain on the second pass denoising.
-    _3p_denoising = SMDegrain(_2p_denoising, tr=1, pel=2, Str=1.1, contrasharp=True, RefineMotion=True, thSAD=smdThSAD, chroma=False, plane=0, search=3, blksize=16, overlap=8, hpad=16, vpad=16)
-
-    # Take the denoised edge clip, and apply it on top of the debanded clip via the mask.
-    ddn_final = core.std.MaskedMerge(_3p_denoising, denoised_edgeclip, mask)
-
-    return ddn_final
+    clipDNS  = Mitchell().scale(clipDNS, clipDN.width, clipDN.height)
+    
+    clipDN   = core.std.MergeDiff(clipDN, clipDNS)
+    # Bicubic Spline Desharpening
+    
+    return clipDN
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def upscale(clip          : vs.VideoNode,
             isAnime       : bool = True,
             fsrcnnxPath   : str  = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1.glsl",
             fsrcnnxLaPath : str  = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1_LineArt.glsl",
             usWidth       : int  = 1920,
             usHeight      : int  = 1080) :
     
     # Verifying which upcaling model should be used depending on the content.
     fsrcnnxFinalPath = fsrcnnxLaPath if (isAnime == True) else fsrcnnxPath
 
-    #Defining a YUV420P16 variable for more accuracy.
-    clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip)
 
     # Upscaling using high quality algo.
     clip = core.placebo.Shader(clip, fsrcnnxFinalPath,  usWidth, usHeight, filter="catmull_rom", antiring=0.7)
     
+    return clip
+    
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
-def edgeHealing(clip         : vs.VideoNode,
-                useDehaloing : bool = True,
-                useDeringing : bool = True,
-                useAA        : bool = True,
-                useUsAA      : bool = True) :
-    
-    #Defining a YUV420P16 variable for more accuracy.
-    clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
-    
-    # Dehalo & Dering edges.
-    if (useDehaloing == True) : clip = DeHalo_alpha(clip, darkstr=0.4)
-    if (useDeringing == True) : clip = HQDeringmod(clip, mrad=8, nrmode=0, darkthr=True)
+def dehalo(clip : vs.VideoNode) :
+    clip = format(clip)
+    clip = DeHalo_alpha(clip, darkstr=0.4)
+    return clip
 
-    # If AA is enabled, will then check if upscaling based AA should be used or not. CAUTION : Upscaled based one will destroy grain pattern.
-    if (useAA == True) : clip = TAAmbk(clip, aatype='Nnedi3UpscaleSangNom', opencl=True) if (useUsAA == True) else TAAmbk(clip, aatype='Eedi3', opencl=True)
+############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
+    
+def dering(clip : vs.VideoNode) :
+    clip = format(clip)
+    clip = HQDeringmod(clip, mrad=8, nrmode=0, darkthr=True)
+    return clip
+
+############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
+def aa(clip    : vs.VideoNode,
+       useUsAA : bool = True) :
+    
+    clip = format(clip)
+    clip = TAAmbk(clip, aatype='Nnedi3UpscaleSangNom', opencl=True) if (useUsAA == True) else TAAmbk(clip, aatype='Eedi3', opencl=True)
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def dpir(clip                   : vs.VideoNode,
          dpirTileDenominator    : int  = 2,
          dpirDeblocking         : bool = True,
          dpirDenoising          : bool = True,
          dpirDeblockingStrength : int  = 15,
          dpirDenoisingStrength  : int  = 1) :
     
-    # Defining a RGBS variable because its needed before using DPIR.
-    clip = core.resize.Spline36(clip, format=vs.RGBS, matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip, cFormatEnum.RGBS)
 
     # Divide frames by tiles to save on VRAM.
     dpirTileW = int(clip.width  / dpirTileDenominator)
     dpirTileH = int(clip.height / dpirTileDenominator)
 
     # AI Assisted deblocking & denoising.
     if (dpirDeblocking == True) : clip = DPIR(task='deblock').run(clip, strength=dpirDeblockingStrength, tile_w=dpirTileW, tile_h=dpirTileH)
-    if (dpirDenoising == True)  : clip = DPIR(task='denoise').run(clip, strength=dpirDenoisingStrength,  tile_w=dpirTileW, tile_h=dpirTileH)
+    if (dpirDenoising  == True) : clip = DPIR(task='denoise').run(clip, strength=dpirDenoisingStrength,  tile_w=dpirTileW, tile_h=dpirTileH)
     
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def deband(clip          : vs.VideoNode,
            dbRemBinarize : int = 1500) :
 
-    clip_edge = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip_edge = format(clip)
 
-    # Creating a retinex edge mask before applying SMDegrain to keep fine details.
+    # Creating a retinex edge mask before applying debanding to keep fine details.
     mask = retinex_edgemask(clip_edge).std.Binarize(dbRemBinarize).std.Inflate()
 
-    # Debanding using placebo.Deband on the third pass denoising on all planes, then converting to YUV420P16 for the final merging.
-    clip = core.resize.Spline36(clip, format=vs.RGBS, matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip, cFormatEnum.RGBS)
     clip = core.placebo.Deband(clip, planes = 1 | 2 | 4, iterations=4, radius=8, threshold=8, grain=6, dither = True, dither_algo = 0)
-    clip = core.resize.Spline36(clip, format=vs.YUV420P16, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip)
 
-    # # Take the denoised edge clip, and apply it on top of the debanded clip via the mask.
+    # # Take the edge clip, and apply it on top of the debanded clip via the mask.
     clip = core.std.MaskedMerge(clip, clip_edge, mask)
 
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def finalize(clip: vs.VideoNode) :
-    # Defining a YUV420P10 variable from the final of the filtering chain, before finalizing and exporting it.
-    clip = core.resize.Spline36(clip, format=vs.YUV420P10, matrix_s="709", matrix_in_s="709", dither_type="error_diffusion")
+    clip = format(clip, cFormatEnum.YUV420P10)
     clip = finalize_clip(clip)
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def everything(clip                   : vs.VideoNode,
                #
@@ -311,27 +321,21 @@
                dst_max                : int   = 110,
                src_max                : int   = 4000,
                src_min                : float = 0.0050,
                #
                useMAGE                : bool  = False,
                thsxdxMultiplier       : float = 0.65,
                #
-               useDDN                 : bool  = False,
-               bm3dSigma              : float = 0.3,
-               ddnRemBinarize         : int   = 500,
-               smdThSAD               : int   = 250,
-               #
                useUpscaling           : bool  = False,
                isAnime                : bool  = True,
                fsrcnnxPath            : str   = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1.glsl",
                fsrcnnxLaPath          : str   = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1_LineArt.glsl",
                usWidth                : int   = 1920,
                usHeight               : int   = 1080,
                #
-               useEdgeHealing         : bool  = False,
                useDehaloing           : bool  = True,
                useDeringing           : bool  = True,
                useAA                  : bool  = True,
                useUsAA                : bool  = True,
                #
                useDPIR                : bool  = False,
                dpirTileDenominator    : int   = 2,
@@ -345,15 +349,16 @@
                #
                useFinalizing          : bool  = True) :
     
     if (slice          == True) : clip = clip[start:end]
     if (useDownscaling == True) : clip = downscale(clip, dsWidth, dsHeight)
     if (useHDR2SDR     == True) : clip = hdr2SDR(clip, dst_max, src_max, src_min)
     if (useMAGE        == True) : clip = mage(clip, thsxdxMultiplier)
-    if (useDDN         == True) : clip = ddn(clip, bm3dSigma, ddnRemBinarize, smdThSAD)
     if (useUpscaling   == True) : clip = upscale(clip, isAnime, fsrcnnxPath, fsrcnnxLaPath, usWidth, usHeight)
-    if (useEdgeHealing == True) : clip = edgeHealing(clip, useDehaloing, useDeringing, useAA, useUsAA)
+    if (useDehaloing   == True) : clip = dehalo(clip)
+    if (useDeringing   == True) : clip = dering(clip)
+    if (useAA          == True) : clip = aa(clip, useUsAA)
     if (useDPIR        == True) : clip = dpir(clip, dpirTileDenominator, dpirDeblocking, dpirDenoising, dpirDeblockingStrength, dpirDenoisingStrength)
     if (useDebanding   == True) : clip = deband(clip, dbRemBinarize)
     if (useFinalizing  == True) : clip = finalize(clip)
     
     return clip
```

### Comparing `WIDscript-1.0.8/src/WIDscript.egg-info/PKG-INFO` & `WIDscript-1.1.0/src/WIDscript.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WIDscript
-Version: 1.0.8
+Version: 1.1.0
 Summary: A private wrapper made for WIDOWN releases.
 Home-page: https://github.com/pypa/sampleproject
 Author: WIDOWN
 Author-email: widown.ma@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

