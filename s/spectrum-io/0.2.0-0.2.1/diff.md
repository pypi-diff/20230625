# Comparing `tmp/spectrum_io-0.2.0.tar.gz` & `tmp/spectrum_io-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_io-0.2.0.tar", max compression
+gzip compressed data, was "spectrum_io-0.2.1.tar", max compression
```

## Comparing `spectrum_io-0.2.0.tar` & `spectrum_io-0.2.1.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0     1072 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/LICENSE
--rw-r--r--   0        0        0     2411 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/README.rst
--rw-r--r--   0        0        0     2338 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/__init__.py
--rw-r--r--   0        0        0      351 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/__main__.py
--rw-r--r--   0        0        0      103 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/file/__init__.py
--rw-r--r--   0        0        0      556 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/file/csv.py
--rw-r--r--   0        0        0     5912 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/file/hdf5.py
--rw-r--r--   0        0        0        0 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/py.typed
--rw-r--r--   0        0        0      104 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/__init__.py
--rw-r--r--   0        0        0     9611 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/msraw.py
--rw-r--r--   0        0        0     3742 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/thermo_raw.py
--rwxr-xr-x   0        0        0    33200 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll
--rwxr-xr-x   0        0        0     5384 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb
--rwxr-xr-x   0        0        0    17827 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml
--rwxr-xr-x   0        0        0   136192 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll
--rwxr-xr-x   0        0        0    73260 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb
--rwxr-xr-x   0        0        0   607957 2023-06-01 16:20:57.409868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml
--rwxr-xr-x   0        0        0   904704 2023-06-01 16:20:57.413868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll
--rwxr-xr-x   0        0        0   245016 2023-06-01 16:20:57.413868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb
--rwxr-xr-x   0        0        0   726825 2023-06-01 16:20:57.417868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml
--rwxr-xr-x   0        0        0   636928 2023-06-01 16:20:57.421868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll
--rwxr-xr-x   0        0        0   281820 2023-06-01 16:20:57.421868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb
--rwxr-xr-x   0        0        0  1215406 2023-06-01 16:20:57.429868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml
--rwxr-xr-x   0        0        0    15360 2023-06-01 16:20:57.429868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll
--rw-r--r--   0        0        0    11324 2023-06-01 16:20:57.429868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE
--rwxr-xr-x   0        0        0  1689600 2023-06-01 16:20:57.437868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll
--rwxr-xr-x   0        0        0  3688730 2023-06-01 16:20:57.449868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml
--rwxr-xr-x   0        0        0    45168 2023-06-01 16:20:57.449868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll
--rwxr-xr-x   0        0        0   229376 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll
--rwxr-xr-x   0        0        0   181640 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml
--rwxr-xr-x   0        0        0    52224 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll
--rwxr-xr-x   0        0        0    40909 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml
--rwxr-xr-x   0        0        0   701992 2023-06-01 16:20:57.457868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll
--rwxr-xr-x   0        0        0   698888 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml
--rwxr-xr-x   0        0        0    34304 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll
--rwxr-xr-x   0        0        0    61952 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll
--rwxr-xr-x   0        0        0    50343 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml
--rwxr-xr-x   0        0        0   159232 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll
--rwxr-xr-x   0        0        0    91970 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml
--rwxr-xr-x   0        0        0    20856 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll
--rwxr-xr-x   0        0        0     3445 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml
--rwxr-xr-x   0        0        0    28552 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll
--rwxr-xr-x   0        0        0    64416 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml
--rwxr-xr-x   0        0        0   141184 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll
--rwxr-xr-x   0        0        0    13585 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml
--rwxr-xr-x   0        0        0   115856 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll
--rwxr-xr-x   0        0        0   180815 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml
--rwxr-xr-x   0        0        0    16768 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll
--rwxr-xr-x   0        0        0    17733 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml
--rwxr-xr-x   0        0        0    33672 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll
--rwxr-xr-x   0        0        0   218987 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml
--rwxr-xr-x   0        0        0    18312 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll
--rwxr-xr-x   0        0        0    89643 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml
--rwxr-xr-x   0        0        0   758664 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll
--rwxr-xr-x   0        0        0     2048 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml
--rwxr-xr-x   0        0        0    25232 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll
--rwxr-xr-x   0        0        0      134 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.xml
--rw-r--r--   0        0        0     6509 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE
--rw-r--r--   0        0        0   404480 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0        0        0  1433139 2023-06-01 16:20:57.485869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml
--rw-r--r--   0        0        0   639488 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll
--rw-r--r--   0        0        0  1547413 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml
--rw-r--r--   0        0        0   174592 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe
--rw-r--r--   0        0        0     3096 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config
--rw-r--r--   0        0        0    56512 2023-06-01 16:20:57.493868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb
--rw-r--r--   0        0        0  4630427 2023-06-01 16:20:57.509869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip
--rw-r--r--   0        0        0      920 2023-06-01 16:20:57.509869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config
--rwxr-xr-x   0        0        0   270336 2023-06-01 16:20:57.513869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll
--rwxr-xr-x   0        0        0  1513051 2023-06-01 16:20:57.517869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml
--rwxr-xr-x   0        0        0   480768 2023-06-01 16:20:57.521869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll
--rwxr-xr-x   0        0        0  1086558 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml
--rwxr-xr-x   0        0        0    69632 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll
--rw-r--r--   0        0        0      122 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/__init__.py
--rw-r--r--   0        0        0     4410 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/mascot.py
--rw-r--r--   0        0        0     4507 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/maxquant.py
--rw-r--r--   0        0        0     3634 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/msfragger.py
--rw-r--r--   0        0        0     2685 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/search_results.py
--rw-r--r--   0        0        0      191 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/__init__.py
--rw-r--r--   0        0        0    22116 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/digest.py
--rw-r--r--   0        0        0    45056 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib
--rw-r--r--   0        0        0     7918 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/dlib.py
--rw-r--r--   0        0        0    98385 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/msp/myPrositLib.msp
--rw-r--r--   0        0        0     3997 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/msp.py
--rw-r--r--   0        0        0     1148 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/spectral_library.py
--rw-r--r--   0        0        0   565091 2023-06-01 16:20:57.529869 spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
--rw-r--r--   0        0        0     4999 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut.py
--rw-r--r--   0        0        0     3618 1970-01-01 00:00:00.000000 spectrum_io-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-25 12:55:35.701807 spectrum_io-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2411 2023-06-25 12:55:35.701807 spectrum_io-0.2.1/README.rst
+-rw-r--r--   0        0        0     2338 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1048 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/__main__.py
+-rw-r--r--   0        0        0      103 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/file/__init__.py
+-rw-r--r--   0        0        0      556 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/file/csv.py
+-rw-r--r--   0        0        0     5912 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/file/hdf5.py
+-rw-r--r--   0        0        0        0 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/py.typed
+-rw-r--r--   0        0        0      104 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/__init__.py
+-rw-r--r--   0        0        0    11999 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/msraw.py
+-rw-r--r--   0        0        0     3752 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/thermo_raw.py
+-rwxr-xr-x   0        0        0    33200 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll
+-rwxr-xr-x   0        0        0     5384 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb
+-rwxr-xr-x   0        0        0    17827 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml
+-rwxr-xr-x   0        0        0   136192 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll
+-rwxr-xr-x   0        0        0    73260 2023-06-25 12:55:35.705807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb
+-rwxr-xr-x   0        0        0   607957 2023-06-25 12:55:35.709807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml
+-rwxr-xr-x   0        0        0   904704 2023-06-25 12:55:35.713807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll
+-rwxr-xr-x   0        0        0   245016 2023-06-25 12:55:35.717807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb
+-rwxr-xr-x   0        0        0   726825 2023-06-25 12:55:35.717807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml
+-rwxr-xr-x   0        0        0   636928 2023-06-25 12:55:35.721807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll
+-rwxr-xr-x   0        0        0   281820 2023-06-25 12:55:35.725807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb
+-rwxr-xr-x   0        0        0  1215406 2023-06-25 12:55:35.729807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml
+-rwxr-xr-x   0        0        0    15360 2023-06-25 12:55:35.729807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll
+-rw-r--r--   0        0        0    11324 2023-06-25 12:55:35.729807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE
+-rwxr-xr-x   0        0        0  1689600 2023-06-25 12:55:35.737807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll
+-rwxr-xr-x   0        0        0  3688730 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml
+-rwxr-xr-x   0        0        0    45168 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll
+-rwxr-xr-x   0        0        0   229376 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll
+-rwxr-xr-x   0        0        0   181640 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml
+-rwxr-xr-x   0        0        0    52224 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll
+-rwxr-xr-x   0        0        0    40909 2023-06-25 12:55:35.749807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml
+-rwxr-xr-x   0        0        0   701992 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll
+-rwxr-xr-x   0        0        0   698888 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml
+-rwxr-xr-x   0        0        0    34304 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll
+-rwxr-xr-x   0        0        0    61952 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll
+-rwxr-xr-x   0        0        0    50343 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml
+-rwxr-xr-x   0        0        0   159232 2023-06-25 12:55:35.757807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll
+-rwxr-xr-x   0        0        0    91970 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml
+-rwxr-xr-x   0        0        0    20856 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll
+-rwxr-xr-x   0        0        0     3445 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml
+-rwxr-xr-x   0        0        0    28552 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll
+-rwxr-xr-x   0        0        0    64416 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml
+-rwxr-xr-x   0        0        0   141184 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll
+-rwxr-xr-x   0        0        0    13585 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml
+-rwxr-xr-x   0        0        0   115856 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll
+-rwxr-xr-x   0        0        0   180815 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml
+-rwxr-xr-x   0        0        0    16768 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll
+-rwxr-xr-x   0        0        0    17733 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml
+-rwxr-xr-x   0        0        0    33672 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll
+-rwxr-xr-x   0        0        0   218987 2023-06-25 12:55:35.761807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml
+-rwxr-xr-x   0        0        0    18312 2023-06-25 12:55:35.765807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll
+-rwxr-xr-x   0        0        0    89643 2023-06-25 12:55:35.765807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml
+-rwxr-xr-x   0        0        0   758664 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll
+-rwxr-xr-x   0        0        0     2048 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml
+-rwxr-xr-x   0        0        0    25232 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll
+-rwxr-xr-x   0        0        0      134 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.xml
+-rw-r--r--   0        0        0     6509 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE
+-rw-r--r--   0        0        0   404480 2023-06-25 12:55:35.769807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0        0        0  1433139 2023-06-25 12:55:35.781808 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml
+-rw-r--r--   0        0        0   639488 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll
+-rw-r--r--   0        0        0  1547413 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml
+-rw-r--r--   0        0        0   174592 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe
+-rw-r--r--   0        0        0     3096 2023-06-25 12:55:35.785807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config
+-rw-r--r--   0        0        0    56512 2023-06-25 12:55:35.789807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb
+-rw-r--r--   0        0        0  4630427 2023-06-25 12:55:35.805807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip
+-rw-r--r--   0        0        0      920 2023-06-25 12:55:35.805807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config
+-rwxr-xr-x   0        0        0   270336 2023-06-25 12:55:35.805807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll
+-rwxr-xr-x   0        0        0  1513051 2023-06-25 12:55:35.809807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml
+-rwxr-xr-x   0        0        0   480768 2023-06-25 12:55:35.813807 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll
+-rwxr-xr-x   0        0        0  1086558 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml
+-rwxr-xr-x   0        0        0    69632 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll
+-rw-r--r--   0        0        0      122 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/__init__.py
+-rw-r--r--   0        0        0     4410 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/mascot.py
+-rw-r--r--   0        0        0     4507 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/maxquant.py
+-rw-r--r--   0        0        0     4143 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/msamanda.py
+-rw-r--r--   0        0        0     3634 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/msfragger.py
+-rw-r--r--   0        0        0     2685 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/search_result/search_results.py
+-rw-r--r--   0        0        0      191 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/__init__.py
+-rw-r--r--   0        0        0    22118 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/digest.py
+-rw-r--r--   0        0        0    45056 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/dlib/myPrositLib.dlib
+-rw-r--r--   0        0        0     7918 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/dlib.py
+-rw-r--r--   0        0        0    98385 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/msp/myPrositLib.msp
+-rw-r--r--   0        0        0     3997 2023-06-25 12:55:35.817808 spectrum_io-0.2.1/spectrum_io/spectral_library/msp.py
+-rw-r--r--   0        0        0     1148 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/spectral_library.py
+-rw-r--r--   0        0        0   565091 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
+-rw-r--r--   0        0        0     4999 2023-06-25 12:55:35.821807 spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut.py
+-rw-r--r--   0        0        0     3618 1970-01-01 00:00:00.000000 spectrum_io-0.2.1/PKG-INFO
```

### Comparing `spectrum_io-0.2.0/LICENSE` & `spectrum_io-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/README.rst` & `spectrum_io-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/pyproject.toml` & `spectrum_io-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_io"
-version = "0.2.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.2.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "IO related functionalities for oktoberfest."
 authors = ["Mario Picciani <mario.picciani@tum.de>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_io"
 repository = "https://github.com/wilhelm-lab/spectrum_io"
 documentation = "https://spectrum_io.readthedocs.io"
```

### Comparing `spectrum_io-0.2.0/spectrum_io/__init__.py` & `spectrum_io-0.2.1/spectrum_io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for spectrum_io."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 from . import file, raw
```

### Comparing `spectrum_io-0.2.0/spectrum_io/file/csv.py` & `spectrum_io-0.2.1/spectrum_io/file/csv.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/file/hdf5.py` & `spectrum_io-0.2.1/spectrum_io/file/hdf5.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/msraw.py` & `spectrum_io-0.2.1/spectrum_io/raw/msraw.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,48 +9,94 @@
 import pymzml
 from pyteomics import mzml
 from spectrum_fundamentals.constants import MZML_DATA_COLUMNS
 
 logger = logging.getLogger(__name__)
 
 
-def get_mass_analyzer(file_path: Path) -> str:
+def check_analyzer(mass_analyzers: Dict[str, str]) -> Dict[str, str]:
+    """
+    Convert mass analyzer accession ids to internal format.
+
+    :param mass_analyzers: dictionary with instrumentConfigurationRef, analyzer accession
+    :raises AssertionError: if the mass analyzer metadata cannot be found in the file or the search
+        was conducted with an unsupported mass analyzer.
+    :return: dictionary with instrumentConfigurationRef, one of (ITMS, FTMS, TOF)
+    """
+    for elem in mass_analyzers.keys():
+        accession = mass_analyzers[elem]
+        if accession in ["MS:1000079", "MS:1000484"]:  # fourier transform ion cyclotron, orbitrap
+            mass_analyzers[elem] = "FTMS"
+        elif accession in ["MS:1000082", "MS:1000264"]:  # quadrupole ion-trap, io-trap
+            mass_analyzers[elem] = "ITMS"
+        elif accession in ["MS:1000084"]:  # TOF
+            mass_analyzers[elem] = "TOF"
+        else:
+            raise AssertionError(f"The mass analyzer with accession {accession} is not supported.")
+    return mass_analyzers
+
+
+def get_mass_analyzer(file_path: Path) -> Dict[str, str]:
     """
     Retrieve mass analyzer information from mzml file.
 
     This is using the description of the mzml format to check for specific accessions in the mzml file
     that are not covered by pyteomics or pymzml. The documentation can be found here:
     https://raw.githubusercontent.com/HUPO-PSI/psi-ms-CV/master/psi-ms.obo
 
     :param file_path: The path to the mzml file to parse
-    :raises AssertionError: if the mass analyzer metadata cannot be found in the file or the search
-        was conducted with an unsupported mass analyzer.
-    :return: A string that is either FTMS or ITMS to represent the respective mass analyzer category.
+    :return: A dictionary with instrumentConfigurationId, mass analyzer (ITMS, FTMS or TOF) to represent
+        the respective mass analyzer category for each MS level that is present in the mzml file, i.e. MS1/MS2/MS3.
     """
-    tree = ElementTree.parse(file_path)
-    root = tree.getroot()
-    namespace = {"ns0": "http://psi.hupo.org/ms/mzml"}
-    analyzer = root.find(
-        ".//ns0:instrumentConfigurationList/ns0:instrumentConfiguration/ns0:componentList/ns0:analyzer/ns0:cvParam",
-        namespace,
-    )
-    if analyzer is None:
-        raise AssertionError("The mass analyzer information can not be retrieved from the mzml file!")
-
-    acc = analyzer.get("accession")
-    if acc in ["MS:1000079", "MS:1000484"]:  # fourier transform ion cyclotron, orbitrap
-        mass_analyzer = "FTMS"
-    elif acc in ["MS:1000082", "MS:1000264"]:  # quadrupole ion-trap, io-trap
-        mass_analyzer = "ITMS"
-    elif acc in ["MS:1000084"]:  # TOF
-        mass_analyzer = "TOF"
-    else:
-        raise AssertionError(f"The mass analyzer with accession {acc} ({analyzer.get('name')}) is not supported.")
+    context = ElementTree.iterparse(file_path, events=("start", "end"))
+    _, root = next(context)  # Get the root element
+
+    namespace = "{http://psi.hupo.org/ms/mzml}"
+    mass_analyzers = {}
+
+    config_id = None
+    accession = None
+    within_instrument_configuration_list = False
+    within_instrument_configuration = False
+
+    for event, element in context:
+        if event == "start" and element.tag == f"{namespace}instrumentConfigurationList":
+            within_instrument_configuration_list = True
+        elif event == "end" and element.tag == f"{namespace}instrumentConfigurationList":
+            within_instrument_configuration_list = False
+            break
+        elif (
+            within_instrument_configuration_list
+            and event == "start"
+            and element.tag == f"{namespace}instrumentConfiguration"
+        ):
+            within_instrument_configuration = True
+            config_id = element.attrib.get("id")
+        elif (
+            within_instrument_configuration
+            and element.tag == f"{namespace}analyzer"
+            and element.attrib.get("order") == "2"
+            and event == "start"
+        ):
+            accession = None  # Reset accession
+        elif (
+            within_instrument_configuration
+            and element.tag == f"{namespace}cvParam"
+            and element.get("accession") is not None
+        ):
+            if accession is None:
+                accession = element.attrib.get("accession")
+        elif (
+            within_instrument_configuration and event == "end" and element.tag == f"{namespace}instrumentConfiguration"
+        ):
+            within_instrument_configuration = False
+            if config_id is not None and accession is not None:
+                mass_analyzers[config_id] = accession
 
-    return mass_analyzer
+    return check_analyzer(mass_analyzers)
 
 
 class MSRaw:
     """Main to read mzml file and generate dataframe containing intensities and m/z values."""
 
     def __init__(self, path: Optional[Union[str, Path]] = None, output_path: Optional[Union[str, Path]] = None):
         """
@@ -102,26 +148,27 @@
                 mass_analyzer = get_mass_analyzer(file_path)
                 logger.info(f"Reading mzML file: {file_path}")
                 data_iter = mzml.read(source=str(file_path), *args, **kwargs)
                 file_name = file_path.stem
                 for spec in data_iter:
                     if spec["ms level"] != 1:  # filter out ms1 spectra if there are any
                         spec_id = spec["id"].split("scan=")[-1]
+                        instrument_configuration_ref = spec["scanList"]["scan"][0]["instrumentConfigurationRef"]
                         fragmentation = spec["scanList"]["scan"][0]["filter string"].split("@")[1][:3].upper()
                         mz_range = spec["scanList"]["scan"][0]["filter string"].split("[")[1][:-1]
                         rt = spec["scanList"]["scan"][0]["scan start time"]
                         key = f"{file_name}_{spec_id}"
                         data[key] = [
                             file_name,
                             spec_id,
                             spec["intensity array"],
                             spec["m/z array"],
                             mz_range,
                             rt,
-                            mass_analyzer,
+                            mass_analyzer[instrument_configuration_ref],
                             fragmentation,
                         ]
                 data_iter.close()
         else:
             raise AssertionError("Choose either 'pymzml' or 'pyteomics'")
 
         data = pd.DataFrame.from_dict(data, orient="index", columns=MZML_DATA_COLUMNS)
@@ -179,41 +226,43 @@
         data_iter = pymzml.run.Reader(file_path, args=args, kwargs=kwargs)
         file_name = file_path.stem
         mass_analyzer = get_mass_analyzer(file_path)
         if scanidx is None:
             for spec in data_iter:
                 if spec.ms_level != 1:  # filter out ms1 spectra if there are any
                     key = f"{file_name}_{spec.ID}"
+                    instrument_configuration_ref = spec["scanList"]["scan"][0]["instrumentConfigurationRef"]
                     filter_string = str(spec.element.find(".//*[@accession='MS:1000512']").get("value"))
                     fragmentation = filter_string.split("@")[1][:3].upper()
                     mz_range = filter_string.split("[")[1][:-1]
                     data[key] = [
                         file_name,
                         spec.ID,
                         spec.i,
                         spec.mz,
                         mz_range,
                         spec.scan_time_in_minutes(),
-                        mass_analyzer,
+                        mass_analyzer[instrument_configuration_ref],
                         fragmentation,
                     ]
         else:
             for idx in scanidx:
                 spec = data_iter[idx]
                 # this does not work if some spectra are filtered out, e.g. mzML files with only MS2 spectra, see:
                 # https://github.com/pymzml/pymzML/blob/a883ff0e61fd97465b0a74667233ff594238e335/pymzml/file_classes
                 # /standardMzml.py#L81-L84
                 key = f"{file_name}_{spec.ID}"
+                instrument_configuration_ref = spec["scanList"]["scan"][0]["instrumentConfigurationRef"]
                 filter_string = str(spec.element.find(".//*[@accession='MS:1000512']").get("value"))
                 fragmentation = filter_string.split("@")[1][:3].upper()
                 mz_range = filter_string.split("[")[1][:-1]
                 data[key] = [
                     file_name,
                     spec.ID,
                     spec.i,
                     spec.mz,
                     mz_range,
                     spec.scan_time_in_minutes(),
-                    mass_analyzer,
+                    mass_analyzer[instrument_configuration_ref],
                     fragmentation,
                 ]
         data_iter.close()
```

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/thermo_raw.py` & `spectrum_io-0.2.1/spectrum_io/raw/thermo_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def _assemble_arg_list(input_path: Path, output_path: Path, ms_level: List[int], gzip: bool) -> List[Union[str, Path]]:
     exec_path = Path(__file__).parent.absolute()  # get path of parent directory of this file
     exec_path /= "utils/ThermoRawFileParser/ThermoRawFileParser.exe"
     exec_arg_list: List[Union[str, Path]] = [
         exec_path,
         f"--msLevel={','.join([str(l) for l in ms_level])}",
         "-i",
-        input_path,
+        input_path.resolve(),
         "-b",
         output_path,
     ]
     if gzip:
         exec_arg_list.append("-g")
     if "linux" in platform or platform == "darwin":
         exec_arg_list.insert(0, "mono")
```

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll` & `spectrum_io-0.2.1/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/search_result/mascot.py` & `spectrum_io-0.2.1/spectrum_io/search_result/mascot.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/search_result/maxquant.py` & `spectrum_io-0.2.1/spectrum_io/search_result/maxquant.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/search_result/msfragger.py` & `spectrum_io-0.2.1/spectrum_io/search_result/msfragger.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/search_result/search_results.py` & `spectrum_io-0.2.1/spectrum_io/search_result/search_results.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/digest.py` & `spectrum_io-0.2.1/spectrum_io/spectral_library/digest.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
     name = None
     seq: List[str] = []
     with open(file_path) as fp:
         for line in itertools.chain(fp, [">"]):
             line = line.rstrip()
             if line.startswith(">"):
                 if name:
-                    seq = "".join(seq)
+                    seq = ["".join(seq)]
                     if db in ["target", "concat"]:
                         yield (name, seq)
 
                     if db in ["decoy", "concat"]:
                         rev_seq = seq[::-1]
                         if hasspecial_aas:
                             rev_seq = swap_special_aas(rev_seq, special_aas)
```

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib` & `spectrum_io-0.2.1/spectrum_io/spectral_library/dlib/myPrositLib.dlib`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/dlib.py` & `spectrum_io-0.2.1/spectrum_io/spectral_library/dlib.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/msp/myPrositLib.msp` & `spectrum_io-0.2.1/spectrum_io/spectral_library/msp/myPrositLib.msp`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/msp.py` & `spectrum_io-0.2.1/spectrum_io/spectral_library/msp.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/spectral_library.py` & `spectrum_io-0.2.1/spectrum_io/spectral_library/spectral_library.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv` & `spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut/myPrositLib.csv`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut.py` & `spectrum_io-0.2.1/spectrum_io/spectral_library/spectronaut.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.2.0/PKG-INFO` & `spectrum_io-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-io
-Version: 0.2.0
+Version: 0.2.1
 Summary: IO related functionalities for oktoberfest.
 Home-page: https://github.com/wilhelm-lab/spectrum_io
 License: MIT
 Author: Mario Picciani
 Author-email: mario.picciani@tum.de
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

