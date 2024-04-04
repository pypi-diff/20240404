# Comparing `tmp/blosc2_grok-0.3.2-py3-none-win_amd64.whl.zip` & `tmp/blosc2_grok-0.3.3-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 3977835 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat   322672 b- defN 24-Mar-17 21:55 bin/concrt140.dll
--rw-rw-rw-  2.0 fat   573008 b- defN 24-Mar-17 21:55 bin/msvcp140.dll
--rw-rw-rw-  2.0 fat    35920 b- defN 24-Mar-17 21:55 bin/msvcp140_1.dll
--rw-rw-rw-  2.0 fat   268392 b- defN 24-Mar-17 21:55 bin/msvcp140_2.dll
--rw-rw-rw-  2.0 fat    50280 b- defN 24-Mar-17 21:55 bin/msvcp140_atomic_wait.dll
--rw-rw-rw-  2.0 fat    31856 b- defN 24-Mar-17 21:55 bin/msvcp140_codecvt_ids.dll
--rw-rw-rw-  2.0 fat   119376 b- defN 24-Mar-17 21:55 bin/vcruntime140.dll
--rw-rw-rw-  2.0 fat    49744 b- defN 24-Mar-17 21:55 bin/vcruntime140_1.dll
--rw-rw-rw-  2.0 fat     8237 b- defN 24-Mar-23 17:07 blosc2_grok/__init__.py
--rw-rw-rw-  2.0 fat  1054720 b- defN 24-Mar-23 17:07 blosc2_grok/blosc2_grok.dll
--rw-rw-rw-  2.0 fat      108 b- defN 24-Mar-23 17:03 include/grok-11.0/grk_config.h
--rw-rw-rw-  2.0 fat    51586 b- defN 24-Mar-23 16:58 include/grok-11.0/grok.h
--rw-rw-rw-  2.0 fat 14147676 b- defN 24-Mar-23 17:07 lib/grokj2k.lib
--rw-rw-r--  2.0 fat     5747 b- defN 24-Mar-23 17:07 blosc2_grok-0.3.2.dist-info/METADATA
--rw-rw-r--  2.0 fat      102 b- defN 24-Mar-23 17:07 blosc2_grok-0.3.2.dist-info/WHEEL
--rw-rw-r--  2.0 fat        0 b- defN 24-Mar-23 17:07 blosc2_grok-0.3.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 fat    35355 b- defN 24-Mar-23 17:07 blosc2_grok-0.3.2.dist-info/licenses/LICENSE.txt
--rw-rw-r--  2.0 fat     1469 b- defN 24-Mar-23 17:07 blosc2_grok-0.3.2.dist-info/RECORD
-18 files, 16756248 bytes uncompressed, 3975483 bytes compressed:  76.3%
+Zip file size: 2173712 bytes, number of entries: 18
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 lib64/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 blosc2_grok/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 blosc2_grok.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 include/
+-rw-r--r--  2.0 unx  4870472 b- defN 24-Apr-04 11:44 lib64/libgrokj2k.a
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/licenses/
+-rw-rw-r--  2.0 unx      927 b- defN 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/RECORD
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx     5747 b- defN 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      151 b- defN 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx    34689 b- defN 24-Apr-04 11:44 blosc2_grok-0.3.3.dist-info/licenses/LICENSE.txt
+-rwxr-xr-x  2.0 unx  2190016 b- defN 24-Apr-04 11:44 blosc2_grok/libblosc2_grok.so
+-rw-r--r--  2.0 unx     8010 b- defN 24-Apr-04 11:44 blosc2_grok/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 11:44 include/grok-11.0/
+-rw-r--r--  2.0 unx     1916 b- defN 24-Apr-04 11:44 include/blosc2_grok.h
+-rw-r--r--  2.0 unx      104 b- defN 24-Apr-04 11:44 include/grok-11.0/grk_config.h
+-rw-r--r--  2.0 unx    49993 b- defN 24-Apr-04 11:44 include/grok-11.0/grok.h
+18 files, 7162025 bytes uncompressed, 2171390 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,55 +1,55 @@
-Filename: bin/concrt140.dll
+Filename: lib64/
 Comment: 
 
-Filename: bin/msvcp140.dll
+Filename: blosc2_grok-0.3.3.dist-info/
 Comment: 
 
-Filename: bin/msvcp140_1.dll
+Filename: blosc2_grok/
 Comment: 
 
-Filename: bin/msvcp140_2.dll
+Filename: blosc2_grok.libs/
 Comment: 
 
-Filename: bin/msvcp140_atomic_wait.dll
+Filename: include/
 Comment: 
 
-Filename: bin/msvcp140_codecvt_ids.dll
+Filename: lib64/libgrokj2k.a
 Comment: 
 
-Filename: bin/vcruntime140.dll
+Filename: blosc2_grok-0.3.3.dist-info/licenses/
 Comment: 
 
-Filename: bin/vcruntime140_1.dll
+Filename: blosc2_grok-0.3.3.dist-info/RECORD
 Comment: 
 
-Filename: blosc2_grok/__init__.py
+Filename: blosc2_grok-0.3.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: blosc2_grok/blosc2_grok.dll
+Filename: blosc2_grok-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: include/grok-11.0/grk_config.h
+Filename: blosc2_grok-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: include/grok-11.0/grok.h
+Filename: blosc2_grok-0.3.3.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: lib/grokj2k.lib
+Filename: blosc2_grok/libblosc2_grok.so
 Comment: 
 
-Filename: blosc2_grok-0.3.2.dist-info/METADATA
+Filename: blosc2_grok/__init__.py
 Comment: 
 
-Filename: blosc2_grok-0.3.2.dist-info/WHEEL
+Filename: include/grok-11.0/
 Comment: 
 
-Filename: blosc2_grok-0.3.2.dist-info/entry_points.txt
+Filename: include/blosc2_grok.h
 Comment: 
 
-Filename: blosc2_grok-0.3.2.dist-info/licenses/LICENSE.txt
+Filename: include/grok-11.0/grk_config.h
 Comment: 
 
-Filename: blosc2_grok-0.3.2.dist-info/RECORD
+Filename: include/grok-11.0/grok.h
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## blosc2_grok/__init__.py

```diff
@@ -1,227 +1,227 @@
-##############################################################################
-# blosc2_grok: Grok (JPEG2000 codec) plugin for Blosc2
-#
-# Copyright (c) 2023  The Blosc Development Team <blosc@blosc.org>
-# https://blosc.org
-# License: GNU Affero General Public License v3.0 (see LICENSE.txt)
-##############################################################################
-
-import ctypes
-import os
-import platform
-from enum import Enum
-from pathlib import Path
-import atexit
-import numpy as np
-
-__version__ = "0.3.2"
-
-
-class GrkFileFmt(Enum):
-    """
-    Supported file formats in grok.
-    """
-
-    GRK_FMT_UNK = 0
-    GRK_FMT_J2K = 1
-    GRK_FMT_JP2 = 2
-    GRK_FMT_PXM = 3
-    GRK_FMT_PGX = 4
-    GRK_FMT_PAM = 5
-    GRK_FMT_BMP = 6
-    GRK_FMT_TIF = 7
-    GRK_FMT_RAW = 8  # Big Endian
-    GRK_FMT_PNG = 9
-    GRK_FMT_RAWL = 10  # Little Endian
-    GRK_FMT_JPG = 11
-
-
-class GrkRateControl(Enum):
-    """
-    Available grok rate control algorithms.
-    """
-
-    BISECT = 0  # bisect with all truncation points
-    PCRD_OPT = 1  # bisect with only feasible truncation points
-
-
-class GrkProfile(Enum):
-    """
-    Available grok profiles.
-    """
-
-    GRK_PROFILE_NONE = 0x0000
-    GRK_PROFILE_0 = 0x0001
-    GRK_PROFILE_1 = 0x0002
-    GRK_PROFILE_CINEMA_2K = 0x0003
-    GRK_PROFILE_CINEMA_4K = 0x0004
-    GRK_PROFILE_CINEMA_S2K = 0x0005
-    GRK_PROFILE_CINEMA_S4K = 0x0006
-    GRK_PROFILE_CINEMA_LTS = 0x0007
-    GRK_PROFILE_BC_SINGLE = 0x0100  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
-    GRK_PROFILE_BC_MULTI = 0x0200  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
-    GRK_PROFILE_BC_MULTI_R = 0x0300  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
-    GRK_PROFILE_BC_MASK = 0x030F  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
-    GRK_PROFILE_IMF_2K = 0x0400  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
-    # and sub-level (7-4 LSB, value between 0 and 9)
-    GRK_PROFILE_IMF_4K = 0x0500  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
-    # and sub-level (7-4 LSB, value between 0 and 9)
-    GRK_PROFILE_IMF_8K = 0x0600  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
-    # and sub-level (7-4 LSB, value between 0 and 9)
-    GRK_PROFILE_IMF_2K_R = 0x0700  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
-    # and sub-level (7-4 LSB, value between 0 and 9)
-    GRK_PROFILE_IMF_4K_R = 0x0800  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
-    # and sub-level (7-4 LSB, value between 0 and 9)
-    GRK_PROFILE_IMF_8K_R = 0x0900  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
-    # and sub-level (7-4 LSB, value between 0 and 9)
-    GRK_PROFILE_MASK = 0x0FFF
-    GRK_PROFILE_PART2 = 0x8000  # Must be combined with extensions
-    GRK_PROFILE_PART2_EXTENSIONS_MASK = 0x3FFF
-
-
-class GrkMode(Enum):
-    """
-    Available grok modes (aka codeblock styles).
-    """
-
-    DEFAULT = 0x000
-    LAZY = 0x001  # Selective arithmetic coding bypass
-    RESET = 0x002  # Reset context probabilities on coding pass boundaries
-    TERMALL = 0x004  # Termination on each coding pass
-    VSC = 0x008  # Vertical stripe causal context
-    PTERM = 0x010  # Predictable termination
-    SEGSYM = 0x020  # Segmentation symbols are used
-    HT = 0x040  # high throughput block coding
-    HT_MIXED = 0x080  # high throughput block coding - mixed
-    HT_PHLD = 0x100  # high throughput block coding - placeholder
-    JPH_RSIZ_FLAG = 0x4000  # for JPH, bit 14 of RSIZ must be set to 1
-
-
-def get_libpath():
-    system = platform.system()
-    if system in ["Linux", "Darwin"]:
-        libname = "libblosc2_grok.so"
-    elif system == "Windows":
-        libname = "blosc2_grok.dll"
-    else:
-        raise RuntimeError("Unsupported system: ", system)
-    return os.path.abspath(Path(__file__).parent / libname)
-
-
-libpath = get_libpath()
-lib = ctypes.cdll.LoadLibrary(libpath)
-
-
-def print_libpath():
-    print(libpath, end="")
-
-
-# Deinitialize grok when exiting
-@atexit.register
-def destroy():
-    lib.blosc2_grok_destroy()
-
-
-params_defaults = {
-    'tile_size': (0, 0),
-    'tile_offset': (0, 0),
-    # 'numlayers': 0, # blosc2_grok C func set_params will still receive this param
-    'quality_mode': None,
-    'quality_layers': np.zeros(0, dtype=np.float64),
-    'numgbits': 2,
-    'progression': "LRCP",
-    'num_resolutions': 6,
-    'codeblock_size': (64, 64),
-    'mode': GrkMode.DEFAULT,
-    # 10 - 19
-    'irreversible': False,
-    'roi_compno': -1,
-    'roi_shift': 0,
-    'precinct_size': (0, 0),
-    'offset': (0, 0),
-    'decod_format': GrkFileFmt.GRK_FMT_UNK,
-    'cod_format': GrkFileFmt.GRK_FMT_JP2,
-    'enableTilePartGeneration': False,
-    'mct': 0,
-    'max_cs_size': 0,
-    # 20 - 29
-    'max_comp_size': 0,
-    'rsiz': GrkProfile.GRK_PROFILE_NONE,
-    'framerate': 0,
-    'apply_icc_': False,
-    'rateControlAlgorithm': GrkRateControl.BISECT,
-    'num_threads': 0,
-    'deviceId': 0,
-    'duration': 0,
-    'repeats': 1,
-    'verbose': False,
-}
-
-
-def set_params_defaults(**kwargs):
-    """
-    Set the parameters for grok.
-    :param kwargs: dict
-        See README.md .
-    :return: None
-
-    Warning
-    -------
-    If you first call this with 'cod_format' different from default
-    >>> blosc2_grok.set_default_params({'cod_format': blosc2_grok.GrkFileFmt.GRK_FMT_J2K})
-    and then call it again with some other parameters:
-    >>> blosc2_grok.set_default_params({'irreversible': True})
-    the default for 'cod_format' will be restored to the original blosc2_grok.GrkFileFmt.GRK_FMT_JP2 in grok.
-    """
-    # Check arguments
-    not_supported = [k for k in kwargs.keys() if k not in params_defaults]
-    if not_supported != []:
-        raise ValueError(f"The next params are not supported: {not_supported}")
-
-    # Prepare arguments
-    params = params_defaults.copy()
-    params.update(kwargs)
-    args = params.values()
-    args = list(args)
-
-    # Get number of layers
-    args.insert(2, 0)
-    if args[3] is not None:
-        args[3] = args[3].encode('utf-8')
-        args[2] = args[4].shape[0]
-
-    args[6] = args[6].encode('utf-8')
-
-    # Convert tuples to desired NumPy arrays
-    args[0] = np.array(args[0], dtype=np.int64)
-    args[1] = np.array(args[1], dtype=np.int64)
-    args[8] = np.array(args[8], dtype=np.int64)
-    args[13] = np.array(args[13], dtype=np.int64)
-    args[14] = np.array(args[14], dtype=np.int64)
-
-    # Get value of enumerate
-    args[9] = args[9].value
-    args[15] = args[15].value
-    args[16] = args[16].value
-    args[21] = args[21].value
-    args[24] = args[24].value
-
-    if args[9] == GrkMode.HT and args[3] is not None:
-        raise ValueError("High throughput mode with quality mode activated is not currently supported.")
-
-    lib.blosc2_grok_set_default_params.argtypes = ([np.ctypeslib.ndpointer(dtype=np.int64)] * 2 +
-                                                   [ctypes.c_int] + [ctypes.c_char_p] + [np.ctypeslib.ndpointer(dtype=np.float64)] +
-                                                   [ctypes.c_int] + [ctypes.c_char_p] +
-                                                   [ctypes.c_int] + [np.ctypeslib.ndpointer(dtype=np.int64)] + [ctypes.c_int] +
-                                                   [ctypes.c_bool] + [ctypes.c_int] * 2 + [np.ctypeslib.ndpointer(dtype=np.int64)] +
-                                                   [np.ctypeslib.ndpointer(dtype=np.int64)] +
-                                                   [ctypes.c_int] +
-                                                   [ctypes.c_int] + [ctypes.c_bool] +
-                                                   [ctypes.c_int] * 5 + [ctypes.c_bool] +
-                                                   [ctypes.c_int] * 5 + [ctypes.c_bool])
-
-    lib.blosc2_grok_set_default_params(*args)
-
-
-if __name__ == "__main__":
-    print_libpath()
+##############################################################################
+# blosc2_grok: Grok (JPEG2000 codec) plugin for Blosc2
+#
+# Copyright (c) 2023  The Blosc Development Team <blosc@blosc.org>
+# https://blosc.org
+# License: GNU Affero General Public License v3.0 (see LICENSE.txt)
+##############################################################################
+
+import ctypes
+import os
+import platform
+from enum import Enum
+from pathlib import Path
+import atexit
+import numpy as np
+
+__version__ = "0.3.3"
+
+
+class GrkFileFmt(Enum):
+    """
+    Supported file formats in grok.
+    """
+
+    GRK_FMT_UNK = 0
+    GRK_FMT_J2K = 1
+    GRK_FMT_JP2 = 2
+    GRK_FMT_PXM = 3
+    GRK_FMT_PGX = 4
+    GRK_FMT_PAM = 5
+    GRK_FMT_BMP = 6
+    GRK_FMT_TIF = 7
+    GRK_FMT_RAW = 8  # Big Endian
+    GRK_FMT_PNG = 9
+    GRK_FMT_RAWL = 10  # Little Endian
+    GRK_FMT_JPG = 11
+
+
+class GrkRateControl(Enum):
+    """
+    Available grok rate control algorithms.
+    """
+
+    BISECT = 0  # bisect with all truncation points
+    PCRD_OPT = 1  # bisect with only feasible truncation points
+
+
+class GrkProfile(Enum):
+    """
+    Available grok profiles.
+    """
+
+    GRK_PROFILE_NONE = 0x0000
+    GRK_PROFILE_0 = 0x0001
+    GRK_PROFILE_1 = 0x0002
+    GRK_PROFILE_CINEMA_2K = 0x0003
+    GRK_PROFILE_CINEMA_4K = 0x0004
+    GRK_PROFILE_CINEMA_S2K = 0x0005
+    GRK_PROFILE_CINEMA_S4K = 0x0006
+    GRK_PROFILE_CINEMA_LTS = 0x0007
+    GRK_PROFILE_BC_SINGLE = 0x0100  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
+    GRK_PROFILE_BC_MULTI = 0x0200  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
+    GRK_PROFILE_BC_MULTI_R = 0x0300  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
+    GRK_PROFILE_BC_MASK = 0x030F  # Has to be combined with the target level (3-0 LSB, value between 0 and 11)
+    GRK_PROFILE_IMF_2K = 0x0400  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
+    # and sub-level (7-4 LSB, value between 0 and 9)
+    GRK_PROFILE_IMF_4K = 0x0500  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
+    # and sub-level (7-4 LSB, value between 0 and 9)
+    GRK_PROFILE_IMF_8K = 0x0600  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
+    # and sub-level (7-4 LSB, value between 0 and 9)
+    GRK_PROFILE_IMF_2K_R = 0x0700  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
+    # and sub-level (7-4 LSB, value between 0 and 9)
+    GRK_PROFILE_IMF_4K_R = 0x0800  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
+    # and sub-level (7-4 LSB, value between 0 and 9)
+    GRK_PROFILE_IMF_8K_R = 0x0900  # Has to be combined with the target main-level (3-0 LSB, value between 0 and 11)
+    # and sub-level (7-4 LSB, value between 0 and 9)
+    GRK_PROFILE_MASK = 0x0FFF
+    GRK_PROFILE_PART2 = 0x8000  # Must be combined with extensions
+    GRK_PROFILE_PART2_EXTENSIONS_MASK = 0x3FFF
+
+
+class GrkMode(Enum):
+    """
+    Available grok modes (aka codeblock styles).
+    """
+
+    DEFAULT = 0x000
+    LAZY = 0x001  # Selective arithmetic coding bypass
+    RESET = 0x002  # Reset context probabilities on coding pass boundaries
+    TERMALL = 0x004  # Termination on each coding pass
+    VSC = 0x008  # Vertical stripe causal context
+    PTERM = 0x010  # Predictable termination
+    SEGSYM = 0x020  # Segmentation symbols are used
+    HT = 0x040  # high throughput block coding
+    HT_MIXED = 0x080  # high throughput block coding - mixed
+    HT_PHLD = 0x100  # high throughput block coding - placeholder
+    JPH_RSIZ_FLAG = 0x4000  # for JPH, bit 14 of RSIZ must be set to 1
+
+
+def get_libpath():
+    system = platform.system()
+    if system in ["Linux", "Darwin"]:
+        libname = "libblosc2_grok.so"
+    elif system == "Windows":
+        libname = "blosc2_grok.dll"
+    else:
+        raise RuntimeError("Unsupported system: ", system)
+    return os.path.abspath(Path(__file__).parent / libname)
+
+
+libpath = get_libpath()
+lib = ctypes.cdll.LoadLibrary(libpath)
+
+
+def print_libpath():
+    print(libpath, end="")
+
+
+# Deinitialize grok when exiting
+@atexit.register
+def destroy():
+    lib.blosc2_grok_destroy()
+
+
+params_defaults = {
+    'tile_size': (0, 0),
+    'tile_offset': (0, 0),
+    # 'numlayers': 0, # blosc2_grok C func set_params will still receive this param
+    'quality_mode': None,
+    'quality_layers': np.zeros(0, dtype=np.float64),
+    'numgbits': 2,
+    'progression': "LRCP",
+    'num_resolutions': 6,
+    'codeblock_size': (64, 64),
+    'mode': GrkMode.DEFAULT,
+    # 10 - 19
+    'irreversible': False,
+    'roi_compno': -1,
+    'roi_shift': 0,
+    'precinct_size': (0, 0),
+    'offset': (0, 0),
+    'decod_format': GrkFileFmt.GRK_FMT_UNK,
+    'cod_format': GrkFileFmt.GRK_FMT_JP2,
+    'enableTilePartGeneration': False,
+    'mct': 0,
+    'max_cs_size': 0,
+    # 20 - 29
+    'max_comp_size': 0,
+    'rsiz': GrkProfile.GRK_PROFILE_NONE,
+    'framerate': 0,
+    'apply_icc_': False,
+    'rateControlAlgorithm': GrkRateControl.BISECT,
+    'num_threads': 0,
+    'deviceId': 0,
+    'duration': 0,
+    'repeats': 1,
+    'verbose': False,
+}
+
+
+def set_params_defaults(**kwargs):
+    """
+    Set the parameters for grok.
+    :param kwargs: dict
+        See README.md .
+    :return: None
+
+    Warning
+    -------
+    If you first call this with 'cod_format' different from default
+    >>> blosc2_grok.set_default_params({'cod_format': blosc2_grok.GrkFileFmt.GRK_FMT_J2K})
+    and then call it again with some other parameters:
+    >>> blosc2_grok.set_default_params({'irreversible': True})
+    the default for 'cod_format' will be restored to the original blosc2_grok.GrkFileFmt.GRK_FMT_JP2 in grok.
+    """
+    # Check arguments
+    not_supported = [k for k in kwargs.keys() if k not in params_defaults]
+    if not_supported != []:
+        raise ValueError(f"The next params are not supported: {not_supported}")
+
+    # Prepare arguments
+    params = params_defaults.copy()
+    params.update(kwargs)
+    args = params.values()
+    args = list(args)
+
+    # Get number of layers
+    args.insert(2, 0)
+    if args[3] is not None:
+        args[3] = args[3].encode('utf-8')
+        args[2] = args[4].shape[0]
+
+    args[6] = args[6].encode('utf-8')
+
+    # Convert tuples to desired NumPy arrays
+    args[0] = np.array(args[0], dtype=np.int64)
+    args[1] = np.array(args[1], dtype=np.int64)
+    args[8] = np.array(args[8], dtype=np.int64)
+    args[13] = np.array(args[13], dtype=np.int64)
+    args[14] = np.array(args[14], dtype=np.int64)
+
+    # Get value of enumerate
+    args[9] = args[9].value
+    args[15] = args[15].value
+    args[16] = args[16].value
+    args[21] = args[21].value
+    args[24] = args[24].value
+
+    if args[9] == GrkMode.HT and args[3] is not None:
+        raise ValueError("High throughput mode with quality mode activated is not currently supported.")
+
+    lib.blosc2_grok_set_default_params.argtypes = ([np.ctypeslib.ndpointer(dtype=np.int64)] * 2 +
+                                                   [ctypes.c_int] + [ctypes.c_char_p] + [np.ctypeslib.ndpointer(dtype=np.float64)] +
+                                                   [ctypes.c_int] + [ctypes.c_char_p] +
+                                                   [ctypes.c_int] + [np.ctypeslib.ndpointer(dtype=np.int64)] + [ctypes.c_int] +
+                                                   [ctypes.c_bool] + [ctypes.c_int] * 2 + [np.ctypeslib.ndpointer(dtype=np.int64)] +
+                                                   [np.ctypeslib.ndpointer(dtype=np.int64)] +
+                                                   [ctypes.c_int] +
+                                                   [ctypes.c_int] + [ctypes.c_bool] +
+                                                   [ctypes.c_int] * 5 + [ctypes.c_bool] +
+                                                   [ctypes.c_int] * 5 + [ctypes.c_bool])
+
+    lib.blosc2_grok_set_default_params(*args)
+
+
+if __name__ == "__main__":
+    print_libpath()
```

## include/grok-11.0/grk_config.h

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-/* Grok Version */
-#define GRK_VERSION_MAJOR 11
-#define GRK_VERSION_MINOR 0
-#define GRK_VERSION_BUILD 0
+/* Grok Version */
+#define GRK_VERSION_MAJOR 11
+#define GRK_VERSION_MINOR 0
+#define GRK_VERSION_BUILD 0
```

## include/grok-11.0/grok.h

 * *Ordering differences only*

```diff
@@ -1,1593 +1,1593 @@
-/*
- *    Copyright (C) 2016-2023 Grok Image Compression Inc.
- *
- *    This source code is free software: you can redistribute it and/or  modify
- *    it under the terms of the GNU Affero General Public License, version 3,
- *    as published by the Free Software Foundation.
- *
- *    This source code is distributed in the hope that it will be useful,
- *    but WITHOUT ANY WARRANTY; without even the implied warranty of
- *    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- *    GNU Affero General Public License for more details.
- *
- *    You should have received a copy of the GNU Affero General Public License
- *    along with this program.  If not, see <http://www.gnu.org/licenses/>.
- *
- *
- *    This source code incorporates work covered by the BSD 2-clause license.
- *    Please see the LICENSE file in the root directory for details.
- *
- */
-#pragma once
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include "grk_config.h"
-#include <stdint.h>
-#include <stdio.h>
-#include <stdbool.h>
-#include <limits.h>
-
-#ifdef _WIN32
-#define GRK_CALLCONV __stdcall
-#ifdef GRK_STATIC
-#define GRK_API
-#else
-#ifdef GRK_EXPORTS
-#define GRK_API __declspec(dllexport)
-#else
-#define GRK_API __declspec(dllimport)
-#endif
-#endif
-#else
-#define GRK_CALLCONV
-#ifdef GRK_STATIC
-#define GRK_API __attribute__((visibility("hidden")))
-#else
-#define GRK_API __attribute__((visibility("default")))
-#endif
-#endif
-
-/**
- * Progression order
- * */
-typedef enum _GRK_PROG_ORDER
-{
-  GRK_PROG_UNKNOWN = -1, /**< place-holder */
-  GRK_LRCP = 0, /**< layer-resolution-component-precinct order */
-  GRK_RLCP = 1, /**< resolution-layer-component-precinct order */
-  GRK_RPCL = 2, /**< resolution-precinct-component-layer order */
-  GRK_PCRL = 3, /**< precinct-component-resolution-layer order */
-  GRK_CPRL = 4, /**< component-precinct-resolution-layer order */
-  GRK_NUM_PROGRESSION_ORDERS = 5 /** number of possible progression orders */
-} GRK_PROG_ORDER;
-
-/**
- * Supported color spaces
- * */
-typedef enum _GRK_COLOR_SPACE
-{
-  GRK_CLRSPC_UNKNOWN = 0, /**< unknown */
-  GRK_CLRSPC_SRGB = 2, /**< sRGB */
-  GRK_CLRSPC_GRAY = 3, /**< grayscale */
-  GRK_CLRSPC_SYCC = 4, /**< standard YCC (YUV) */
-  GRK_CLRSPC_EYCC = 5, /**< extended YCC */
-  GRK_CLRSPC_CMYK = 6, /**< CMYK */
-  GRK_CLRSPC_DEFAULT_CIE = 7, /**< default CIE LAB */
-  GRK_CLRSPC_CUSTOM_CIE = 8, /**< custom CIE LAB */
-  GRK_CLRSPC_ICC = 9 /**< ICC profile */
-} GRK_COLOR_SPACE;
-
-/* JPEG 2000 standard colour space enumeration */
-typedef enum _GRK_ENUM_COLOUR_SPACE
-{
-  GRK_ENUM_CLRSPC_UNKNOWN = 0xFFFFFFFF,
-  GRK_ENUM_CLRSPC_BILEVEL1 = 0,
-  GRK_ENUM_CLRSPC_YCBCR1 = 1,
-  GRK_ENUM_CLRSPC_YCBCR2 = 3,
-  GRK_ENUM_CLRSPC_YCBCR3 = 4,
-  GRK_ENUM_CLRSPC_PHOTO_YCC = 9, /* Kodak PhotoYCC */
-  GRK_ENUM_CLRSPC_CMY = 11, /* cyan, magenta, yellow */
-  GRK_ENUM_CLRSPC_CMYK = 12, /* cyan, magenta, yellow, black */
-  GRK_ENUM_CLRSPC_YCCK = 13,
-  GRK_ENUM_CLRSPC_CIE = 14,
-  GRK_ENUM_CLRSPC_BILEVEL2 = 15,
-  GRK_ENUM_CLRSPC_SRGB = 16,
-  GRK_ENUM_CLRSPC_GRAY = 17,
-  GRK_ENUM_CLRSPC_SYCC = 18, /* standard YCC */
-  GRK_ENUM_CLRSPC_CIEJAB = 19,
-  GRK_ENUM_CLRSPC_ESRGB = 20,
-  GRK_ENUM_CLRSPC_ROMMRGB = 21, /* Reference Output Medium Metric RGB */
-  GRK_ENUM_CLRSPC_YPBPR60 = 22,
-  GRK_ENUM_CLRSPC_YPBPR50 = 23,
-  GRK_ENUM_CLRSPC_EYCC = 24, /* extended YCC */
-} GRK_ENUM_COLOUR_SPACE;
-
-#define GRK_NUM_COMMENTS_SUPPORTED 256
-#define GRK_NUM_ASOC_BOXES_SUPPORTED 256
-#define GRK_MAX_COMMENT_LENGTH (UINT16_MAX - 2)
-#define GRK_MAX_SUPPORTED_IMAGE_PRECISION 16 /* Maximum supported precision in library */
-
-/* BIBO analysis - extra bits needed to avoid overflow:
-
- Lossless:
- without colour transform: 4 extra bits
- with colour transform:    5 extra bits
-
- Lossy:
-
- Need 1 extra bit
-
- So,  worst-case scenario is lossless with colour transform : need to add 5 more bits to prec to
- avoid overflow
- */
-#define BIBO_EXTRA_BITS 7
-
-#define GRK_MAX_PASSES (3 * (GRK_MAX_SUPPORTED_IMAGE_PRECISION + BIBO_EXTRA_BITS) - 2)
-
-/**
- * Logging callback
- *
- * @param msg               message
- * @param client_data       client data passed to callback
- * */
-typedef void (*grk_msg_callback)(const char* msg, void* client_data);
-
-/**
- *
- * Grok ref-counted object
- *
- */
-typedef struct _grk_object
-{
-  void* wrapper;
-} grk_object;
-
-/**
- * Progression order change
- *
- */
-typedef struct _grk_progression
-{
-  GRK_PROG_ORDER progression;
-  char progressionString[5];
-  GRK_PROG_ORDER specifiedCompressionPocProg;
-  uint32_t tileno;
-  /** tile dimensions */
-  uint32_t tx0;
-  uint32_t ty0;
-  uint32_t tx1;
-  uint32_t ty1;
-  /** progression order bounds specified by POC */
-  uint16_t compS;
-  uint16_t compE;
-  uint8_t resS;
-  uint8_t resE;
-  uint64_t precS;
-  uint64_t precE;
-  uint16_t layS;
-  uint16_t layE;
-  uint16_t tpCompS;
-  uint16_t tpCompE;
-  uint8_t tpResS;
-  uint8_t tpResE;
-  uint64_t tpPrecE;
-  uint16_t tpLayE;
-  uint32_t tp_txS;
-  uint32_t tp_txE;
-  uint32_t tp_tyS;
-  uint32_t tp_tyE;
-  uint32_t dx;
-  uint32_t dy;
-  uint16_t comp_temp;
-  uint8_t res_temp;
-  uint64_t prec_temp;
-  uint16_t lay_temp;
-  uint32_t tx0_temp;
-  uint32_t ty0_temp;
-} grk_progression;
-
-/** RAW component compress parameters */
-typedef struct _grk_raw_comp_cparameters
-{
-  uint8_t dx; /** subsampling in X direction */
-  uint8_t dy; /** subsampling in Y direction */
-  /*@}*/
-} grk_raw_comp_cparameters;
-
-/**RAW image compress parameters */
-typedef struct _grk_raw_cparameters
-{
-  uint32_t width; /** width of the raw image */
-  uint32_t height; /** height of the raw image */
-  uint16_t numcomps; /** number of components of the raw image */
-  uint8_t prec; /** bit depth of the raw image */
-  bool sgnd; /** signed/unsigned raw image */
-  grk_raw_comp_cparameters* comps; /** raw components parameters */
-} grk_raw_cparameters;
-
-/**
- * Rate control algorithms
-  GRK_RATE_CONTROL_BISECT: bisect with all truncation points
-  GRK_RATE_CONTROL_PCRD_OPT: bisect with only feasible truncation points
- */
-typedef enum _GRK_RATE_CONTROL_ALGORITHM
-{
-  GRK_RATE_CONTROL_BISECT,
-  GRK_RATE_CONTROL_PCRD_OPT
-} GRK_RATE_CONTROL_ALGORITHM;
-
-/**
- * All supported file formats
- */
-typedef enum _GRK_SUPPORTED_FILE_FMT
-{
-  GRK_FMT_UNK,
-  GRK_FMT_J2K,
-  GRK_FMT_JP2,
-  GRK_FMT_PXM,
-  GRK_FMT_PGX,
-  GRK_FMT_PAM,
-  GRK_FMT_BMP,
-  GRK_FMT_TIF,
-  GRK_FMT_RAW, /* MSB / Big Endian */
-  GRK_FMT_PNG,
-  GRK_FMT_RAWL, /* LSB / Little Endian */
-  GRK_FMT_JPG
-} GRK_SUPPORTED_FILE_FMT;
-
-/**
- * Supported JPEG 2000 formats
- */
-typedef enum _GRK_CODEC_FORMAT
-{
-  GRK_CODEC_UNK, /**< unknown format */
-  GRK_CODEC_J2K, /**< JPEG 2000 code stream format */
-  GRK_CODEC_JP2 /**< JP2 file format */
-} GRK_CODEC_FORMAT;
-
-#define GRK_PATH_LEN 4096 /* Maximum allowed filename size */
-#define GRK_MAX_LAYERS 100 /* Maximum number of quality layers */
-
-/*
- * Note: range for number of decomposition levels is 0-32
- * So, accordingly, range for number of resolutions is 1-33
- */
-#define GRK_J2K_MAX_DECOMP_LVLS                                    \
-  32 /* Maximum number of decomposition levels allowed by standard \
-      */
-#define GRK_J2K_MAXRLVLS \
-  (GRK_J2K_MAX_DECOMP_LVLS + 1) /* Maximum number of resolution levels allowed by standard*/
-#define GRK_J2K_MAXBANDS \
-  (3 * GRK_J2K_MAXRLVLS - 2) /*  Maximum number of sub-bands allowed by standard */
-
-/**
- * Note: "component" refers to an image component as decompressed
- * from the code stream, while "channel" refers to a component resulting
- * from the application of a Palette box LUT and a Component mapping box.
- */
-
-/**
- Component mappings: component index, mapping type, palette column
- */
-typedef struct _grk_component_mapping_comp
-{
-  uint16_t component_index;
-  uint8_t mapping_type;
-  uint8_t palette_column;
-} grk_component_mapping_comp;
-
-/**
- Palette data
- */
-typedef struct _grk_palette_data
-{
-  int32_t* lut;
-  uint16_t num_entries;
-  grk_component_mapping_comp* component_mapping;
-  uint8_t num_channels;
-  bool* channel_sign;
-  uint8_t* channel_prec;
-} grk_palette_data;
-
-/***
- * Channel Definition box structures and enums.
- * When no Component mapping box is present, it is still possible to have
- * a Channel defintion box, in which case channels are associated with components
- * in the obvious way : channel `k` corresponds to component `k`.
- * */
-
-/* channel type */
-typedef enum _GRK_CHANNEL_TYPE
-{
-  GRK_CHANNEL_TYPE_COLOUR = 0,
-  GRK_CHANNEL_TYPE_OPACITY = 1,
-  GRK_CHANNEL_TYPE_PREMULTIPLIED_OPACITY = 2,
-  GRK_CHANNEL_TYPE_UNSPECIFIED = 65535U
-
-} GRK_CHANNEL_TYPE;
-
-/* channel association */
-typedef enum _GRK_CHANNEL_ASSOC
-{
-
-  GRK_CHANNEL_ASSOC_WHOLE_IMAGE = 0,
-  GRK_CHANNEL_ASSOC_COLOUR_1 = 1,
-  GRK_CHANNEL_ASSOC_COLOUR_2 = 2,
-  GRK_CHANNEL_ASSOC_COLOUR_3 = 3,
-  GRK_CHANNEL_ASSOC_UNASSOCIATED = 65535U
-
-} GRK_CHANNEL_ASSOC;
-
-/**
- Channel definition: channel index, type, association
- */
-typedef struct _grk_channel_description
-{
-  uint16_t channel;
-  uint16_t typ;
-  uint16_t asoc;
-} grk_channel_description;
-
-/**
- Channel definitions and number of definitions
- */
-typedef struct _grk_channel_definition
-{
-  grk_channel_description* descriptions;
-  uint16_t num_channel_descriptions;
-} grk_channel_definition;
-
-/**
- ICC profile, palette, channel definition
- */
-typedef struct _grk_color
-{
-  uint8_t* icc_profile_buf;
-  uint32_t icc_profile_len;
-  char* icc_profile_name;
-  grk_channel_definition* channel_definition;
-  grk_palette_data* palette;
-  bool has_colour_specification_box;
-} grk_color;
-
-/**
- * Association box info
- */
-typedef struct _grk_asoc
-{
-  uint32_t level; /* 0 for root level */
-  const char* label;
-  uint8_t* xml;
-  uint32_t xml_len;
-} grk_asoc;
-
-/**
- * Precision mode
- */
-typedef enum _grk_precision_mode
-{
-  GRK_PREC_MODE_CLIP,
-  GRK_PREC_MODE_SCALE
-} grk_precision_mode;
-
-/**
- * Precision
- */
-typedef struct _grk_precision
-{
-  uint8_t prec;
-  grk_precision_mode mode;
-} grk_precision;
-
-/**
- * Header info
- */
-typedef struct _grk_header_info
-{
-  /******************************************
-  set by client only if decompressing to file
-  *******************************************/
-  GRK_SUPPORTED_FILE_FMT decompressFormat;
-  bool forceRGB;
-  bool upsample;
-  grk_precision* precision;
-  uint32_t numPrecision;
-  bool splitByComponent;
-  bool singleTileDecompress;
-  /****************************************/
-
-  /*****************************************
-  populated by library after reading header
-  ******************************************/
-  /** initial code block width, default to 64 */
-  uint32_t cblockw_init;
-  /** initial code block height, default to 64 */
-  uint32_t cblockh_init;
-  /** 1 : use the irreversible DWT 9-7, 0 : use lossless compression (default) */
-  bool irreversible;
-  /** multi-component transform identifier */
-  uint32_t mct;
-  /** RSIZ value
-   To be used to combine GRK_PROFILE_*, GRK_EXTENSION_* and (sub)levels values. */
-  uint16_t rsiz;
-  /** number of resolutions */
-  uint32_t numresolutions;
-  /*********************************************************
-  coding style can be specified in main header COD segment,
-  tile header COD segment, and tile component COC segment.
-  *********************************************************/
-  /* !!!! assume that coding style does not vary across tile components */
-  uint8_t csty;
-  /*******************************************************************
-  code block style is specified in main header COD segment, and can
-  be overridden in a tile header.  !!! Assume that style does
-  not vary across tiles !!!
-  *******************************************************************/
-  uint8_t cblk_sty;
-  /** initial precinct width */
-  uint32_t prcw_init[GRK_J2K_MAXRLVLS];
-  /** initial precinct height */
-  uint32_t prch_init[GRK_J2K_MAXRLVLS];
-  /** XTOsiz */
-  uint32_t tx0;
-  /** YTOsiz */
-  uint32_t ty0;
-  /** XTsiz */
-  uint32_t t_width;
-  /** YTsiz */
-  uint32_t t_height;
-  /** tile grid width */
-  uint32_t t_grid_width;
-  /** tile grid height  */
-  uint32_t t_grid_height;
-  /** maximum number of layers */
-  uint16_t max_layers_;
-  /*************************************
-  note: xml_data will remain valid
-   until codec is destroyed
-   ************************************/
-  uint8_t* xml_data;
-  size_t xml_data_len;
-  size_t num_comments;
-  char* comment[GRK_NUM_COMMENTS_SUPPORTED];
-  uint16_t comment_len[GRK_NUM_COMMENTS_SUPPORTED];
-  bool isBinaryComment[GRK_NUM_COMMENTS_SUPPORTED];
-
-  grk_asoc asocs[GRK_NUM_ASOC_BOXES_SUPPORTED];
-  uint32_t num_asocs;
-} grk_header_info;
-
-typedef struct _grk_io_buf
-{
-  uint8_t* data_;
-  size_t offset_;
-  size_t len_;
-  size_t allocLen_;
-  bool pooled_;
-  uint32_t index_;
-} grk_io_buf;
-
-typedef struct _grk_io_init
-{
-  uint32_t maxPooledRequests_;
-
-} grk_io_init;
-
-typedef bool (*grk_io_callback)(uint32_t threadId, grk_io_buf buffer, void* io_user_data);
-typedef void (*grk_io_register_reclaim_callback)(grk_io_init io_init,
-                                                 grk_io_callback reclaim_callback,
-                                                 void* io_user_data, void* reclaim_user_data);
-typedef bool (*grk_io_pixels_callback)(uint32_t threadId, grk_io_buf buffer, void* user_data);
-
-/**
- * read stream callback
- *
- * @buffer buffer to write stream to
- * @numBytes number of bytes to write to buffer
- * @user_data user data
- *
- */
-typedef size_t (*grk_stream_read_fn)(uint8_t* buffer, size_t numBytes, void* user_data);
-
-/**
- * write stream callback
- *
- * @buffer buffer to read stream from
- * @numBytes number of bytes to read from buffer
- * @user_data user data
- *
- */
-typedef size_t (*grk_stream_write_fn)(const uint8_t* buffer, size_t numBytes, void* user_data);
-
-/**
- * seek (absolute) callback
- *
- * @offset absolute stream offset
- * @user_data user data
- *
- */
-typedef bool (*grk_stream_seek_fn)(uint64_t offset, void* user_data);
-
-/**
- * free user data callback
- *
- * @user_data user data
- *
- */
-typedef void (*grk_stream_free_user_data_fn)(void* user_data);
-
-/**
- * JPEG 2000 stream parameters. Client must populate one of the following options :
- * 1. File
- * 2. Buffer
- * 3. Callback
- */
-typedef struct _grk_stream_params
-{
-  /* 1. File */
-  const char* file;
-
-  /* 2. Buffer */
-  uint8_t* buf;
-  size_t buf_len;
-  /* length of compressed stream (set by compressor, not client) */
-  size_t buf_compressed_len;
-
-  /* 3. Callback */
-  grk_stream_read_fn read_fn;
-  grk_stream_write_fn write_fn;
-  grk_stream_seek_fn seek_fn;
-  grk_stream_free_user_data_fn free_user_data_fn; // optional
-  void* user_data;
-  size_t stream_len; // must be set for read stream
-  size_t double_buffer_len; // optional - default value is 1024 * 1024
-} grk_stream_params;
-
-typedef enum _GRK_TILE_CACHE_STRATEGY
-{
-  GRK_TILE_CACHE_NONE, /* no tile caching */
-  GRK_TILE_CACHE_IMAGE /* cache final tile image */
-} GRK_TILE_CACHE_STRATEGY;
-
-/**
- * Core decompression parameters
- * */
-typedef struct _grk_decompress_core_params
-{
-  /**
-   Set the number of highest resolution levels to be discarded.
-   The image resolution is effectively divided by 2 to the power of the number of discarded
-   levels. The reduce factor is limited by the smallest total number of decomposition levels among
-   tiles. if greater than zero, then image is decoded to original dimension divided by
-   2^(reduce); if equal to zero or not used, image is decompressed to full resolution
-   */
-  uint8_t reduce;
-  /**
-   Set the maximum number of quality layers to decompress.
-   If there are fewer quality layers than the specified number, all quality layers will be
-   decompressed. if != 0, then only the first "layer" layers are decompressed; if == 0 or not
-   used, all the quality layers are decompressed
-   */
-  uint16_t layers_to_decompress_;
-  GRK_TILE_CACHE_STRATEGY tileCacheStrategy;
-
-  uint32_t randomAccessFlags_;
-
-  grk_io_pixels_callback io_buffer_callback;
-  void* io_user_data;
-  grk_io_register_reclaim_callback io_register_client_callback;
-} grk_decompress_core_params;
-
-#define GRK_DECOMPRESS_COMPRESSION_LEVEL_DEFAULT (UINT_MAX)
-
-/**
- * Decompression parameters
- */
-typedef struct _grk_decompress_params
-{
-  /** core library parameters */
-  grk_decompress_core_params core;
-  /** input file name */
-  char infile[GRK_PATH_LEN];
-  /** output file name */
-  char outfile[GRK_PATH_LEN];
-  /** input file format*/
-  GRK_CODEC_FORMAT decod_format;
-  /** output file format*/
-  GRK_SUPPORTED_FILE_FMT cod_format;
-  /** Decompress window left boundary */
-  float dw_x0;
-  /** Decompress window right boundary */
-  float dw_x1;
-  /** Decompress window up boundary */
-  float dw_y0;
-  /** Decompress window bottom boundary */
-  float dw_y1;
-  /** tile number of the decompressed tile*/
-  uint16_t tileIndex;
-  bool singleTileDecompress;
-  grk_precision* precision;
-  uint32_t numPrecision;
-  /* force output colorspace to RGB */
-  bool force_rgb;
-  /* upsample components according to their dx/dy values */
-  bool upsample;
-  /* split output components to different files */
-  bool split_pnm;
-  /* serialize XML metadata to disk */
-  bool io_xml;
-  uint32_t compression;
-  /*****************************************************
-  compression "quality". Meaning of "quality" depends
-  on file format we are writing to
-  *****************************************************/
-  uint32_t compressionLevel;
-  /** Verbose mode */
-  bool verbose_;
-  int32_t deviceId;
-  uint32_t duration; /* in seconds */
-  uint32_t kernelBuildOptions;
-  uint32_t repeats;
-  uint32_t numThreads;
-  void* user_data;
-} grk_decompress_parameters;
-
-/**
- * Image component
- * */
-typedef struct _grk_image_comp
-{
-  /** x component offset compared to the whole image */
-  uint32_t x0;
-  /** y component offset compared to the whole image */
-  uint32_t y0;
-  /** data width */
-  uint32_t w;
-  /** data stride */
-  uint32_t stride;
-  /** data height */
-  uint32_t h;
-  /** XRsiz: horizontal separation of a sample of component with respect to the reference
-   * grid */
-  uint8_t dx;
-  /** YRsiz: vertical separation of a sample of component with respect to the reference grid
-   */
-  uint8_t dy;
-  /** precision */
-  uint8_t prec;
-  /* signed */
-  bool sgnd;
-  GRK_CHANNEL_TYPE type;
-  GRK_CHANNEL_ASSOC association;
-  /* component registration coordinates */
-  uint16_t Xcrg, Ycrg;
-  /** image component data */
-  int32_t* data;
-} grk_image_comp;
-
-/* Image meta data: colour, IPTC and XMP */
-typedef struct _grk_image_meta
-{
-  grk_object obj;
-  grk_color color;
-  uint8_t* iptc_buf;
-  size_t iptc_len;
-  uint8_t* xmp_buf;
-  size_t xmp_len;
-} grk_image_meta;
-
-typedef struct _grk_image
-{
-  grk_object obj;
-  /** XOsiz: horizontal offset from the origin of the reference grid
-   *  to the left side of the image area */
-  uint32_t x0;
-  /** YOsiz: vertical offset from the origin of the reference grid
-   *  to the top side of the image area */
-  uint32_t y0;
-  /** Xsiz: width of the reference grid */
-  uint32_t x1;
-  /** Ysiz: height of the reference grid */
-  uint32_t y1;
-  /** number of components in the image */
-  uint16_t numcomps;
-  GRK_COLOR_SPACE color_space;
-  bool paletteApplied_;
-  bool channelDefinitionApplied_;
-  bool has_capture_resolution;
-  double capture_resolution[2];
-  bool has_display_resolution;
-  double display_resolution[2];
-  GRK_SUPPORTED_FILE_FMT decompressFormat;
-  bool forceRGB;
-  bool upsample;
-  grk_precision* precision;
-  uint32_t numPrecision;
-  bool hasMultipleTiles;
-  bool splitByComponent;
-  uint16_t decompressNumComps;
-  uint32_t decompressWidth;
-  uint32_t decompressHeight;
-  uint8_t decompressPrec;
-  GRK_COLOR_SPACE decompressColourSpace;
-  grk_io_buf interleavedData;
-  uint32_t rowsPerStrip; // for storage to output format
-  uint32_t rowsPerTask; // for scheduling
-  uint64_t packedRowBytes;
-  grk_image_meta* meta;
-  grk_image_comp* comps;
-} grk_image;
-
-/*************************************************
-Structs to pass data between grok and plugin
-************************************************/
-/**
- * Plugin pass
- */
-typedef struct _grk_plugin_pass
-{
-  double distortionDecrease; /* distortion decrease up to and including this pass */
-  size_t rate; /* rate up to and including this pass */
-  size_t length; /* stream length for this pass */
-} grk_plugin_pass;
-
-/**
- * Plugin code block
- */
-typedef struct _grk_plugin_code_block
-{
-  /**************************
-  debug info
-  **************************/
-  uint32_t x0, y0, x1, y1;
-  unsigned int* contextStream;
-  /***************************/
-  uint32_t numPix;
-  uint8_t* compressedData;
-  uint32_t compressedDataLength;
-  uint8_t numBitPlanes;
-  size_t numPasses;
-  grk_plugin_pass passes[GRK_MAX_PASSES];
-  unsigned int sortedIndex;
-} grk_plugin_code_block;
-
-/**
- * Plugin precinct
- */
-typedef struct _grk_plugin_precinct
-{
-  uint64_t numBlocks;
-  grk_plugin_code_block** blocks;
-} grk_plugin_precinct;
-
-/**
- * Plugin band
- */
-typedef struct _grk_plugin_band
-{
-  uint8_t orientation;
-  uint64_t numPrecincts;
-  grk_plugin_precinct** precincts;
-  float stepsize;
-} grk_plugin_band;
-
-/**
- * Plugin resolution
- */
-typedef struct _grk_plugin_resolution
-{
-  size_t level;
-  size_t numBands;
-  grk_plugin_band** band;
-} grk_plugin_resolution;
-
-/**
- * Plugin tile component
- */
-typedef struct grk_plugin_tile_component
-{
-  size_t numResolutions;
-  grk_plugin_resolution** resolutions;
-} grk_plugin_tile_component;
-
-#define GRK_DECODE_HEADER (1 << 0)
-#define GRK_DECODE_T2 (1 << 1)
-#define GRK_DECODE_T1 (1 << 2)
-#define GRK_DECODE_POST_T1 (1 << 3)
-#define GRK_PLUGIN_DECODE_CLEAN (1 << 4)
-#define GRK_DECODE_ALL \
-  (GRK_PLUGIN_DECODE_CLEAN | GRK_DECODE_HEADER | GRK_DECODE_T2 | GRK_DECODE_T1 | GRK_DECODE_POST_T1)
-
-/**
- * Plugin tile
- */
-typedef struct _grk_plugin_tile
-{
-  uint32_t decompress_flags;
-  size_t numComponents;
-  grk_plugin_tile_component** tileComponents;
-} grk_plugin_tile;
-
-/* opaque codec object */
-typedef grk_object grk_codec;
-
-/**
- * Library version
- */
-GRK_API const char* GRK_CALLCONV grk_version(void);
-
-/**
- * Initialize library
- *
- * @param pluginPath 	path to plugin
- * @param numthreads 	number of threads to use for compress/decompress
- */
-GRK_API void GRK_CALLCONV grk_initialize(const char* pluginPath, uint32_t numthreads, bool verbose);
-
-/**
- * De-initialize library
- */
-GRK_API void GRK_CALLCONV grk_deinitialize();
-
-/**
- * Increment ref count
- */
-GRK_API grk_object* GRK_CALLCONV grk_object_ref(grk_object* obj);
-
-/*
- * Decrement ref count
- *
- */
-GRK_API void GRK_CALLCONV grk_object_unref(grk_object* obj);
-
-GRK_API void GRK_CALLCONV grk_set_msg_handlers(grk_msg_callback info_callback, void* info_user_data,
-                                               grk_msg_callback warn_callback, void* warn_user_data,
-                                               grk_msg_callback error_callback,
-                                               void* error_user_data);
-
-/**
- * Create image
- *
- * @param numcmpts      number of components
- * @param cmptparms     component parameters
- * @param clrspc        image color space
- * @param alloc_data    if true, allocate component data buffers
- *
- * @return returns      a new image if successful, otherwise NULL
- * */
-GRK_API grk_image* GRK_CALLCONV grk_image_new(uint16_t numcmpts, grk_image_comp* cmptparms,
-                                              GRK_COLOR_SPACE clrspc, bool alloc_data);
-
-GRK_API grk_image_meta* GRK_CALLCONV grk_image_meta_new(void);
-
-/**
- * Detect jpeg 2000 format from file
- * Format is either GRK_FMT_J2K or GRK_FMT_JP2
- *
- * @param fileName file name
- * @param fmt pointer to detected format
- *
- * @return true if format was detected, otherwise false
- *
- */
-GRK_API bool GRK_CALLCONV grk_decompress_detect_format(const char* fileName, GRK_CODEC_FORMAT* fmt);
-
-/**
- * Initialize stream parameters with default values
- *
- * @param parameters stream parameters
- */
-GRK_API void GRK_CALLCONV grk_set_default_stream_params(grk_stream_params* params);
-
-/**
- * Initialize decompress parameters with default values
- *
- * @param parameters decompression parameters
- */
-GRK_API void GRK_CALLCONV grk_decompress_set_default_params(grk_decompress_parameters* parameters);
-
-/**
- * Initialize decompressor
- *
- * @param stream_params 	source stream parameters
- * @param core_params 	decompress core parameters
- *
- * @return grk_codec* if successful, otherwise NULL
- */
-GRK_API grk_codec* GRK_CALLCONV grk_decompress_init(grk_stream_params* stream_params,
-                                                    grk_decompress_core_params* core_params);
-
-/**
- * Decompress JPEG 2000 header
- *
- * @param	codec				decompression codec
- * @param	header_info			information read from JPEG 2000 header.
- *
- * @return true					if the main header of the code stream and the JP2 header
- * 							 	is correctly read.
- */
-GRK_API bool GRK_CALLCONV grk_decompress_read_header(grk_codec* codec,
-                                                     grk_header_info* header_info);
-
-/**
- * Get decompressed tile image
- *
- * @param	codec				decompression codec
- * @param	tileIndex			tile index
- *
- * @return pointer to decompressed image
- */
-GRK_API grk_image* GRK_CALLCONV grk_decompress_get_tile_image(grk_codec* codec, uint16_t tileIndex);
-
-/**
- * Get decompressed composite image
- *
- * @param	codec				decompression codec
- *
- * @return pointer to decompressed image
- */
-GRK_API grk_image* GRK_CALLCONV grk_decompress_get_composited_image(grk_codec* codec);
-
-/**
- * Set the given area to be decompressed. This function should be called
- * right after grk_decompress_read_header is called, and before any tile header is read.
- *
- * @param	codec			decompression codec
- * @param	start_x		    left position of the rectangle to decompress (in image coordinates).
- * @param	end_x			the right position of the rectangle to decompress (in image
- * coordinates).
- * @param	start_y		    up position of the rectangle to decompress (in image coordinates).
- * @param	end_y			bottom position of the rectangle to decompress (in image coordinates).
- *
- * @return	true			if the area could be set.
- */
-GRK_API bool GRK_CALLCONV grk_decompress_set_window(grk_codec* codec, float start_x, float start_y,
-                                                    float end_x, float end_y);
-
-/**
- * Decompress image from a JPEG 2000 code stream
- *
- * @param codec 	decompression codec
- * @param tile		tile struct from plugin
- *
- * @return 			true if successful, otherwise false
- * */
-GRK_API bool GRK_CALLCONV grk_decompress(grk_codec* codec, grk_plugin_tile* tile);
-
-/**
- * Decompress a specific tile
- *
- * @param	codec			decompression codec
- * @param	tileIndex		index of the tile to be decompressed
- *
- * @return					true if successful, otherwise false
- */
-GRK_API bool GRK_CALLCONV grk_decompress_tile(grk_codec* codec, uint16_t tileIndex);
-
-/* COMPRESSION FUNCTIONS*/
-
-/**
- * Compress parameters
- * */
-typedef struct _grk_cparameters
-{
-  /** size of tile: tile_size_on = false (not in argument) or = true (in argument) */
-  bool tile_size_on;
-  /** XTOsiz */
-  uint32_t tx0;
-  /** YTOsiz */
-  uint32_t ty0;
-  /** XTsiz */
-  uint32_t t_width;
-  /** YTsiz */
-  uint32_t t_height;
-  /** number of layers */
-  uint16_t numlayers;
-  /** rate control allocation by rate/distortion curve */
-  bool allocationByRateDistoration;
-  /** layers rates expressed as compression ratios.
-   *  They might be subsequently limited by the max_cs_size field */
-  double layer_rate[GRK_MAX_LAYERS];
-  /** rate control allocation by fixed_PSNR quality */
-  bool allocationByQuality;
-  /** layer PSNR values */
-  double layer_distortion[GRK_MAX_LAYERS];
-  char* comment[GRK_NUM_COMMENTS_SUPPORTED];
-  uint16_t comment_len[GRK_NUM_COMMENTS_SUPPORTED];
-  bool is_binary_comment[GRK_NUM_COMMENTS_SUPPORTED];
-  size_t num_comments;
-  /** csty : coding style */
-  uint8_t csty;
-  /* number of guard bits */
-  uint8_t numgbits;
-  /** progression order (default is LRCP) */
-  GRK_PROG_ORDER prog_order;
-  /** progressions */
-  grk_progression progression[GRK_J2K_MAXRLVLS];
-  /** number of progression order changes (POCs), default to 0 */
-  uint32_t numpocs;
-  /** number of resolutions */
-  uint8_t numresolution;
-  /** initial code block width  (default to 64) */
-  uint32_t cblockw_init;
-  /** initial code block height (default to 64) */
-  uint32_t cblockh_init;
-  /** code block style */
-  uint8_t cblk_sty;
-  /** 1 : use the irreversible DWT 9-7, 0 :
-   *  use lossless compression (default) */
-  bool irreversible;
-  /** region of interest: affected component in [0..3];
-   *  -1 indicates no ROI */
-  int32_t roi_compno;
-  /** region of interest: upshift value */
-  uint32_t roi_shift;
-  /* number of precinct size specifications */
-  uint32_t res_spec;
-  /** initial precinct width */
-  uint32_t prcw_init[GRK_J2K_MAXRLVLS];
-  /** initial precinct height */
-  uint32_t prch_init[GRK_J2K_MAXRLVLS];
-  /** input file name */
-  char infile[GRK_PATH_LEN];
-  /** output file name */
-  char outfile[GRK_PATH_LEN];
-  /** subimage compressing: origin image offset in x direction */
-  uint32_t image_offset_x0;
-  /** subimage compressing: origin image offset in y direction */
-  uint32_t image_offset_y0;
-  /** subsampling value for dx */
-  uint8_t subsampling_dx;
-  /** subsampling value for dy */
-  uint8_t subsampling_dy;
-  /** input file format*/
-  GRK_SUPPORTED_FILE_FMT decod_format;
-  /** output file format*/
-  GRK_SUPPORTED_FILE_FMT cod_format;
-  grk_raw_cparameters raw_cp;
-  /** Tile part generation*/
-  bool enableTilePartGeneration;
-  /** new tile part progression divider */
-  uint8_t newTilePartProgressionDivider;
-  /** MCT (multiple component transform) */
-  uint8_t mct;
-  /** Naive implementation of MCT restricted to a single reversible array based
-   compressing without offset concerning all the components. */
-  void* mct_data;
-  /**
-   * Maximum size (in bytes) for the whole code stream.
-   * If equal to zero, code stream size limitation is not considered
-   * If it does not comply with layer_rate, max_cs_size prevails
-   * and a warning is issued.
-   * */
-  uint64_t max_cs_size;
-  /**
-   * Maximum size (in bytes) for each component.
-   * If == 0, component size limitation is not considered
-   * */
-  uint64_t max_comp_size;
-  /** RSIZ value
-   To be used to combine GRK_PROFILE_*, GRK_EXTENSION_* and (sub)levels values. */
-  uint16_t rsiz;
-  uint16_t framerate;
-
-  /* set to true if input file stores capture resolution */
-  bool write_capture_resolution_from_file;
-  double capture_resolution_from_file[2];
-
-  bool write_capture_resolution;
-  double capture_resolution[2];
-
-  bool write_display_resolution;
-  double display_resolution[2];
-
-  bool apply_icc_;
-
-  GRK_RATE_CONTROL_ALGORITHM rateControlAlgorithm;
-  uint32_t numThreads;
-  int32_t deviceId;
-  uint32_t duration; /* seconds */
-  uint32_t kernelBuildOptions;
-  uint32_t repeats;
-  bool writePLT;
-  bool writeTLM;
-  bool verbose;
-  bool sharedMemoryInterface;
-} grk_cparameters;
-
-/**
- Set compressing parameters to default values:
-
- Lossless
- Single tile
- Size of precinct : 2^15 x 2^15 (i.e. single precinct)
- Size of code block : 64 x 64
- Number of resolutions: 6
- No SOP marker in the code stream
- No EPH marker in the code stream
- No mode switches
- Progression order: LRCP
- No ROI upshifted
- Image origin lies at (0,0)
- Tile origin lies at (0,0)
- Reversible DWT 5-3 transform
-
- @param parameters Compression parameters
- */
-GRK_API void GRK_CALLCONV grk_compress_set_default_params(grk_cparameters* parameters);
-
-/**
- * Set up the compressor parameters using the current image and user parameters.
- *
- * @param codec 		compression codec
- * @param parameters 	compression parameters
- * @param image 		input image
- */
-GRK_API grk_codec* GRK_CALLCONV grk_compress_init(grk_stream_params* stream_params,
-                                                  grk_cparameters* parameters, grk_image* p_image);
-
-/**
- * Compress an image into a JPEG 2000 code stream using plugin
- *
- * @param codec 		compression codec
- * @param tile			plugin tile
- *
- * @return 				number of bytes written if successful, 0 otherwise
- */
-GRK_API uint64_t GRK_CALLCONV grk_compress(grk_codec* codec, grk_plugin_tile* tile);
-
-/**
- * Dump codec information to file
- *
- * @param	codec			decompression codec
- * @param	info_flag		type of information dump.
- * @param	output_stream	codec information is dumped to output stream
- *
- */
-GRK_API void GRK_CALLCONV grk_dump_codec(grk_codec* codec, uint32_t info_flag, FILE* output_stream);
-
-/**
- * Set the MCT matrix to use.
- *
- * @param	parameters		the parameters to change.
- * @param	encodingMatrix	the compressing matrix.
- * @param	dc_shift		the dc shift coefficients to use.
- * @param	nbComp			the number of components of the image.
- *
- * @return	true if the parameters could be set.
- */
-GRK_API bool GRK_CALLCONV grk_set_MCT(grk_cparameters* parameters, float* encodingMatrix,
-                                      int32_t* dc_shift, uint32_t nbComp);
-
-#define GRK_IMG_INFO 1 /* Basic image information provided to the user */
-#define GRK_J2K_MH_INFO 2 /* Codestream information based only on the main header */
-#define GRK_J2K_TH_INFO 4 /* Tile information based on the current tile header */
-#define GRK_J2K_TCH_INFO 8 /**< Tile/Component information of all tiles */
-#define GRK_J2K_MH_IND 16 /**< Codestream index based only on the main header */
-#define GRK_J2K_TH_IND 32 /**< Tile index based on the current tile */
-#define GRK_JP2_INFO 128 /**< JP2 file information */
-#define GRK_JP2_IND 256 /**< JP2 file index */
-
-#define GRK_CBLKSTY_LAZY 0x001 /**< Selective arithmetic coding bypass */
-#define GRK_CBLKSTY_RESET 0x002 /**< Reset context probabilities on coding pass boundaries */
-#define GRK_CBLKSTY_TERMALL 0x004 /**< Termination on each coding pass */
-#define GRK_CBLKSTY_VSC 0x008 /**< Vertical stripe causal context */
-#define GRK_CBLKSTY_PTERM 0x010 /**< Predictable termination */
-#define GRK_CBLKSTY_SEGSYM 0x020 /**< Segmentation symbols are used */
-#define GRK_CBLKSTY_HT 0x040 /**< high throughput block coding */
-#define GRK_CBLKSTY_HT_MIXED 0x080 /**< high throughput block coding - mixed*/
-#define GRK_CBLKSTY_HT_PHLD 0x100 /**< high throughput block coding - placeholder */
-#define GRK_JPH_RSIZ_FLAG 0x4000 /**<for JPH, bit 14 of RSIZ must be set to 1 */
-
-/*****************************************************************************
- * JPEG 2000 Profiles, see Table A.10 from 15444-1 (updated in various AMDs)
- *
- * These values help choose the RSIZ value for the JPEG 2000 code stream.
- * The RSIZ value forces various compressing options, as detailed in Table A.10.
- * If GRK_PROFILE_PART2 is chosen, it must be combined with one or more extensions
- * described below.
- *
- *   Example: rsiz = GRK_PROFILE_PART2 | GRK_EXTENSION_MCT;
- *
- * For broadcast profiles, the GRK_PROFILE_X value has to be combined with the target
- * level (3-0 LSB, value between 0 and 11):
- *   Example: rsiz = GRK_PROFILE_BC_MULTI | 0x0005; //level equals 5
- *
- * For IMF profiles, the GRK_PROFILE_X value has to be combined with the target main-level
- * (3-0 LSB, value between 0 and 11) and sub-level (7-4 LSB, value between 0 and 9):
- *   Example: rsiz = GRK_PROFILE_IMF_2K | 0x0040 | 0x0005; // main-level equals 5 and sub-level
- * equals 4
- *
- * */
-#define GRK_PROFILE_NONE 0x0000 /** no profile, conform to 15444-1 */
-#define GRK_PROFILE_0 0x0001 /** Profile 0 as described in 15444-1,Table A.45 */
-#define GRK_PROFILE_1 0x0002 /** Profile 1 as described in 15444-1,Table A.45 */
-#define GRK_PROFILE_CINEMA_2K 0x0003 /** 2K cinema profile defined in 15444-1 AMD1 */
-#define GRK_PROFILE_CINEMA_4K 0x0004 /** 4K cinema profile defined in 15444-1 AMD1 */
-#define GRK_PROFILE_CINEMA_S2K 0x0005 /** Scalable 2K cinema profile defined in 15444-1 AMD2 */
-#define GRK_PROFILE_CINEMA_S4K 0x0006 /** Scalable 4K cinema profile defined in 15444-1 AMD2 */
-#define GRK_PROFILE_CINEMA_LTS \
-  0x0007 /** Long term storage cinema profile defined in 15444-1 AMD2 */
-#define GRK_PROFILE_BC_SINGLE 0x0100 /** Single Tile Broadcast profile defined in 15444-1 AMD3 */
-#define GRK_PROFILE_BC_MULTI 0x0200 /** Multi Tile Broadcast profile defined in 15444-1 AMD3 */
-#define GRK_PROFILE_BC_MULTI_R \
-  0x0300 /** Multi Tile Reversible Broadcast profile defined in 15444-1 AMD3 */
-#define GRK_PROFILE_BC_MASK 0x030F /** Mask for broadcast profile including main level */
-#define GRK_PROFILE_IMF_2K 0x0400 /** 2K Single Tile Lossy IMF profile defined in 15444-1 AMD8 */
-#define GRK_PROFILE_IMF_4K 0x0500 /** 4K Single Tile Lossy IMF profile defined in 15444-1 AMD8 */
-#define GRK_PROFILE_IMF_8K 0x0600 /** 8K Single Tile Lossy IMF profile defined in 15444-1 AMD8 */
-#define GRK_PROFILE_IMF_2K_R \
-  0x0700 /** 2K Single/Multi Tile Reversible IMF profile defined in 15444-1 AMD8 */
-#define GRK_PROFILE_IMF_4K_R \
-  0x0800 /** 4K Single/Multi Tile Reversible IMF profile defined in 15444-1 AMD8 */
-#define GRK_PROFILE_IMF_8K_R \
-  0x0900 /** 8K Single/Multi Tile Reversible IMF profile defined in 15444-1 AMD8 */
-#define GRK_PROFILE_MASK 0x0FFF /** Mask for profile bits */
-#define GRK_PROFILE_PART2 0x8000 /** At least 1 extension defined in 15444-2 (Part-2) */
-#define GRK_PROFILE_PART2_EXTENSIONS_MASK 0x3FFF // Mask for Part-2 extension bits
-
-/**
- * JPEG 2000 Part-2 extensions
- * */
-#define GRK_EXTENSION_NONE 0x0000 /** No Part-2 extension */
-#define GRK_EXTENSION_MCT 0x0100 /** Custom MCT support */
-#define GRK_IS_PART2(v) ((v)&GRK_PROFILE_PART2)
-
-#define GRK_IS_CINEMA(v) (((v) >= GRK_PROFILE_CINEMA_2K) && ((v) <= GRK_PROFILE_CINEMA_S4K))
-#define GRK_IS_STORAGE(v) ((v) == GRK_PROFILE_CINEMA_LTS)
-
-/*
- *
- * *********************************************
- * Broadcast level (3-0 LSB) (15444-1 AMD4,AMD8)
- * *********************************************
- *
- * indicates maximum bit rate and sample rate for a code stream
- *
- * Note: Mbit/s == 10^6 bits/s;  Msamples/s == 10^6 samples/s
- *
- * 0:       no maximum rate
- * 1:       200 Mbits/s, 65  Msamples/s
- * 2:       200 Mbits/s, 130 Msamples/s
- * 3:       200 Mbits/s, 195 Msamples/s
- * 4:       400 Mbits/s, 260 Msamples/s
- * 5:       800Mbits/s,  520 Msamples/s
- * >= 6:    2^(level-6) * 1600 Mbits/s, 2^(level-6) * 1200 Msamples/s
- *
- * Note: level cannot be greater than 11
- *
- * ****************
- * Broadcast tiling
- * ****************
- *
- * Either single-tile or multi-tile. Multi-tile only permits
- * 1 or 4 tiles per frame, where multiple tiles have identical
- * sizes, and are configured in either 2x2 or 1x4 layout.
- *
- *************************************************************
- *
- * ***************************************
- * IMF main-level (3-0) LSB (15444-1 AMD8)
- * ***************************************
- *
- * main-level indicates maximum number of samples per second,
- * as listed above.
- *
- *
- * **************************************
- * IMF sub-level (7-4) LSB (15444-1 AMD8)
- * **************************************
- *
- * sub-level indicates maximum bit rate for a code stream:
- *
- * 0:   no maximum rate
- * >0:  2^sub-level * 100 Mbits/second
- *
- * Note: sub-level cannot be greater than 9, and cannot be larger
- * then maximum of (main-level -2) and 1.
- *
- */
-
-#define GRK_GET_IMF_OR_BROADCAST_PROFILE(v) \
-  ((v)&0x0f00) /** Extract profile without mainlevel/sublevel */
-
-#define GRK_LEVEL_MAX 11U /** Maximum (main) level */
-#define GRK_GET_LEVEL(v) ((v)&0xf) /** Extract (main) level */
-
-/******* BROADCAST **********************************************************/
-
-#define GRK_IS_BROADCAST(v)                                                        \
-  (((v) >= GRK_PROFILE_BC_SINGLE) && ((v) <= (GRK_PROFILE_BC_MULTI_R | 0x000b)) && \
-   (((v)&0xf) <= 0xb))
-
-/* Maximum component sampling Rate (Mbits/sec) per level */
-#define GRK_BROADCAST_LEVEL_1_MBITSSEC 200U /** Mbits/sec for level 1 */
-#define GRK_BROADCAST_LEVEL_2_MBITSSEC 200U /** Mbits/sec for level 2 */
-#define GRK_BROADCAST_LEVEL_3_MBITSSEC 200U /** Mbits/sec for level 3 */
-#define GRK_BROADCAST_LEVEL_4_MBITSSEC 400U /** Mbits/sec for level 4 */
-#define GRK_BROADCAST_LEVEL_5_MBITSSEC 800U /** Mbits/sec for level 5 */
-#define GRK_BROADCAST_LEVEL_6_MBITSSEC 1600U /** Mbits/sec for level 6 */
-#define GRK_BROADCAST_LEVEL_7_MBITSSEC 3200U /** Mbits/sec for level 7 */
-#define GRK_BROADCAST_LEVEL_8_MBITSSEC 6400U /** Mbits/sec for level 8 */
-#define GRK_BROADCAST_LEVEL_9_MBITSSEC 12800U /** Mbits/sec for level 9 */
-#define GRK_BROADCAST_LEVEL_10_MBITSSEC 25600U /** Mbits/sec for level 10 */
-#define GRK_BROADCAST_LEVEL_11_MBITSSEC 51200U /** Mbits/sec for level 11 */
-
-#define GRK_BROADCAST_LEVEL_1_MSAMPLESSEC 64U /** MSamples/sec for level 1 */
-#define GRK_BROADCAST_LEVEL_2_MSAMPLESSEC 130U /** MSamples/sec for level 2 */
-#define GRK_BROADCAST_LEVEL_3_MSAMPLESSEC 195U /** MSamples/sec for level 3 */
-#define GRK_BROADCAST_LEVEL_4_MSAMPLESSEC 260U /** MSamples/sec for level 4 */
-#define GRK_BROADCAST_LEVEL_5_MSAMPLESSEC 520U /** MSamples/sec for level 5 */
-#define GRK_BROADCAST_LEVEL_6_MSAMPLESSEC 1200U /** MSamples/sec for level 6 */
-#define GRK_BROADCAST_LEVEL_7_MSAMPLESSEC 2400U /** MSamples/sec for level 7 */
-#define GRK_BROADCAST_LEVEL_8_MSAMPLESSEC 4800U /** MSamples/sec for level 8 */
-#define GRK_BROADCAST_LEVEL_9_MSAMPLESSEC 9600U /** MSamples/sec for level 9 */
-#define GRK_BROADCAST_LEVEL_10_MSAMPLESSEC 19200U /** MSamples/sec for level 10 */
-#define GRK_BROADCAST_LEVEL_11_MSAMPLESSEC 38400U /** MSamples/sec for level 11 */
-
-/********IMF *****************************************************************/
-
-#define GRK_IS_IMF(v)                                                         \
-  (((v) >= GRK_PROFILE_IMF_2K) && ((v) <= (GRK_PROFILE_IMF_8K_R | 0x009b)) && \
-   (((v)&0xf) <= 0xb) && (((v)&0xf0) <= 0x90))
-
-/* Maximum component sampling rate (MSamples/sec) per main level */
-#define GRK_IMF_MAINLEVEL_1_MSAMPLESSEC 65U /** MSamples/sec for main level 1 */
-#define GRK_IMF_MAINLEVEL_2_MSAMPLESSEC 130U /** MSamples/sec for main level 2 */
-#define GRK_IMF_MAINLEVEL_3_MSAMPLESSEC 195U /** MSamples/sec for main level 3 */
-#define GRK_IMF_MAINLEVEL_4_MSAMPLESSEC 260U /** MSamples/sec for main level 4 */
-#define GRK_IMF_MAINLEVEL_5_MSAMPLESSEC 520U /** MSamples/sec for main level 5 */
-#define GRK_IMF_MAINLEVEL_6_MSAMPLESSEC 1200U /** MSamples/sec for main level 6 */
-#define GRK_IMF_MAINLEVEL_7_MSAMPLESSEC 2400U /** MSamples/sec for main level 7 */
-#define GRK_IMF_MAINLEVEL_8_MSAMPLESSEC 4800U /** MSamples/sec for main level 8 */
-#define GRK_IMF_MAINLEVEL_9_MSAMPLESSEC 9600U /** MSamples/sec for main level 9 */
-#define GRK_IMF_MAINLEVEL_10_MSAMPLESSEC 19200U /** MSamples/sec for main level 10 */
-#define GRK_IMF_MAINLEVEL_11_MSAMPLESSEC 38400U /** MSamples/sec for main level 11 */
-
-#define GRK_IMF_SUBLEVEL_MAX 9U /** Maximum IMF sublevel */
-#define GRK_GET_IMF_SUBLEVEL(v) (((v) >> 4) & 0xf) /** Extract IMF sub level */
-
-/** Maximum compressed bit rate (Mbits/s) per IMF sub level */
-#define GRK_IMF_SUBLEVEL_1_MBITSSEC 200U /** Mbits/s for IMF sub level 1 */
-#define GRK_IMF_SUBLEVEL_2_MBITSSEC 400U /** Mbits/s for IMF sub level 2 */
-#define GRK_IMF_SUBLEVEL_3_MBITSSEC 800U /** Mbits/s for IMF sub level 3 */
-#define GRK_IMF_SUBLEVEL_4_MBITSSEC 1600U /** Mbits/s for IMF sub level 4 */
-#define GRK_IMF_SUBLEVEL_5_MBITSSEC 3200U /** Mbits/s for IMF sub level 5 */
-#define GRK_IMF_SUBLEVEL_6_MBITSSEC 6400U /** Mbits/s for IMF sub level 6 */
-#define GRK_IMF_SUBLEVEL_7_MBITSSEC 12800U /** Mbits/s for IMF sub level 7 */
-#define GRK_IMF_SUBLEVEL_8_MBITSSEC 25600U /** Mbits/s for IMF sub level 8 */
-#define GRK_IMF_SUBLEVEL_9_MBITSSEC 51200U /** Mbits/s for IMF sub level 9 */
-/**********************************************************************************/
-
-/**
- * JPEG 2000 cinema profile code stream and component size limits
- * */
-
-#define GRK_CINEMA_DCI_MAX_BANDWIDTH 250000000
-
-#define GRK_CINEMA_24_CS 1302083 /** Maximum code stream length @ 24fps */
-#define GRK_CINEMA_24_COMP 1041666 /** Maximum size per color component @ 24fps */
-
-#define GRK_CINEMA_48_CS 651041 /** Maximum code stream length @ 48fps */
-#define GRK_CINEMA_48_COMP 520833 /** Maximum size per color component @ 48fps */
-
-#define GRK_CINEMA_4K_DEFAULT_NUM_RESOLUTIONS 7
-
-/*
- *
- * CIE Lab #defines
- */
-#define GRK_CUSTOM_CIELAB_SPACE 0x0
-#define GRK_DEFAULT_CIELAB_SPACE 0x44454600 /* 'DEF' */
-#define GRK_CIE_DAY ((((uint32_t)'C') << 24) + (((uint32_t)'T') << 16))
-#define GRK_CIE_D50 ((uint32_t)0x00443530)
-#define GRK_CIE_D65 ((uint32_t)0x00443635)
-#define GRK_CIE_D75 ((uint32_t)0x00443735)
-#define GRK_CIE_SA ((uint32_t)0x00005341)
-#define GRK_CIE_SC ((uint32_t)0x00005343)
-#define GRK_CIE_F2 ((uint32_t)0x00004632)
-#define GRK_CIE_F7 ((uint32_t)0x00004637)
-#define GRK_CIE_F11 ((uint32_t)0x00463131)
-
-/**
- * Toggle random access markers
- */
-#define GRK_RANDOM_ACCESS_PLT 1 /* use PLT marker if present */
-#define GRK_RANDOM_ACCESS_TLM 2 /* use TLM marker if present */
-#define GRK_RANDOM_ACCESS_PLM 4 /* use PLM marker if present */
-
-/*************************************************************************************
- Plugin Interface
- *************************************************************************************/
-
-/*
- Plugin management
- */
-
-typedef struct _grk_plugin_load_info
-{
-  const char* pluginPath;
-  bool verbose;
-} grk_plugin_load_info;
-
-/**
- * Load plugin
- *
- * @param info		plugin loading info
- */
-GRK_API bool GRK_CALLCONV grk_plugin_load(grk_plugin_load_info info);
-
-/**
- * Release plugin resources
- */
-GRK_API void GRK_CALLCONV grk_plugin_cleanup(void);
-
-/* No debug is done on plugin. Production setting. */
-#define GRK_PLUGIN_STATE_NO_DEBUG 0x0
-
-/*
- For compress debugging, the plugin first performs a T1 compress.
- Then:
- 1. perform host DWT on plugin MCT data, and write to host image
- This way, both plugin and host start from same point
- (assume MCT is equivalent for both host and plugin)
- 2. map plugin DWT data, compare with host DWT, and then write to plugin image
- At this point in the code, the plugin image holds plugin DWT data. And if no warnings are
- triggered, then we can safely say that host and plugin DWT data are identical.
- 3. Perform host compress, skipping MCT and DWT (they have already been performed)
- 4. during host compress, each context that is formed is compared against context stream from plugin
- 5. rate control - synch with plugin code stream, and compare
- 6. T2 and store to disk
- */
-
-#define GRK_PLUGIN_STATE_DEBUG 0x1
-#define GRK_PLUGIN_STATE_PRE_TR1 0x2
-#define GRK_PLUGIN_STATE_DWT_QUANTIZATION 0x4
-#define GRK_PLUGIN_STATE_MCT_ONLY 0x8
-
-/**
- * Get debug state of plugin
- */
-GRK_API uint32_t GRK_CALLCONV grk_plugin_get_debug_state();
-
-/*
- Plugin compressing
- */
-typedef struct _grk_plugin_init_info
-{
-  int32_t deviceId;
-  bool verbose;
-  const char* license;
-  const char* server;
-} grk_plugin_init_info;
-
-/**
- * Initialize plugin
- */
-GRK_API bool GRK_CALLCONV grk_plugin_init(grk_plugin_init_info initInfo);
-
-typedef struct grk_plugin_compress_user_callback_info
-{
-  const char* input_file_name;
-  bool outputFileNameIsRelative;
-  const char* output_file_name;
-  grk_cparameters* compressor_parameters;
-  grk_image* image;
-  grk_plugin_tile* tile;
-  grk_stream_params stream_params;
-  unsigned int error_code;
-  bool transferExifTags;
-} grk_plugin_compress_user_callback_info;
-
-typedef uint64_t (*GRK_PLUGIN_COMPRESS_USER_CALLBACK)(grk_plugin_compress_user_callback_info* info);
-
-typedef struct grk_plugin_compress_batch_info
-{
-  const char* input_dir;
-  const char* output_dir;
-  grk_cparameters* compress_parameters;
-  GRK_PLUGIN_COMPRESS_USER_CALLBACK callback;
-} grk_plugin_compress_batch_info;
-
-/**
- * Compress with plugin
- *
- * @param compress_parameters 	compress parameters
- * @param callback				callback
- */
-GRK_API int32_t GRK_CALLCONV grk_plugin_compress(grk_cparameters* compress_parameters,
-                                                 GRK_PLUGIN_COMPRESS_USER_CALLBACK callback);
-
-/**
- * Batch compress with plugin
- *
- * @param input_dir				directory holding input images
- * @param output_dir			directory holding compressed output images
- * @param compress_parameters 	compress parameters
- * @param callback				callback
- *
- * @return 0 if successful
- *
- */
-GRK_API int32_t GRK_CALLCONV grk_plugin_batch_compress(grk_plugin_compress_batch_info info);
-
-/**
- * Wait for batch job to complete
- */
-GRK_API void GRK_CALLCONV grk_plugin_wait_for_batch_complete(void);
-
-/**
- * Stop batch compress
- */
-GRK_API void GRK_CALLCONV grk_plugin_stop_batch_compress(void);
-
-/*
- Plugin decompression
- */
-
-typedef int (*GROK_INIT_DECOMPRESSORS)(grk_header_info* header_info, grk_image* image);
-
-typedef struct _grk_plugin_decompress_callback_info
-{
-  size_t deviceId;
-  GROK_INIT_DECOMPRESSORS init_decompressors_func;
-  const char* input_file_name;
-  const char* output_file_name;
-  /* input file format 0: J2K, 1: JP2 */
-  GRK_CODEC_FORMAT decod_format;
-  /* output file format 0: PGX, 1: PxM, 2: BMP etc */
-  GRK_SUPPORTED_FILE_FMT cod_format;
-  grk_codec* codec;
-  grk_header_info header_info;
-  grk_decompress_parameters* decompressor_parameters;
-  grk_image* image;
-  bool plugin_owns_image;
-  grk_plugin_tile* tile;
-  unsigned int error_code;
-  uint32_t decompress_flags;
-  uint32_t full_image_x0;
-  uint32_t full_image_y0;
-  void* user_data;
-} grk_plugin_decompress_callback_info;
-
-typedef int32_t (*grk_plugin_decompress_callback)(grk_plugin_decompress_callback_info* info);
-
-/**
- * Decompress with plugin
- *
- * @param decompress_parameters  decompress parameters
- * @param callback  			 callback
- */
-GRK_API int32_t GRK_CALLCONV grk_plugin_decompress(grk_decompress_parameters* decompress_parameters,
-                                                   grk_plugin_decompress_callback callback);
-
-/**
- * Initialize batch decompress
- *
- * @param input_dir input directory holding compressed images
- * @param output_dir output directory holding decompressed images
- * @param decompress_parameters  decompress parameters
- * @param callback  			 callback
- *
- * @return 0 if successful
- */
-GRK_API int32_t GRK_CALLCONV grk_plugin_init_batch_decompress(
-    const char* input_dir, const char* output_dir, grk_decompress_parameters* decompress_parameters,
-    grk_plugin_decompress_callback callback);
-
-/**
- * Initiate batch decompress
- */
-GRK_API int32_t GRK_CALLCONV grk_plugin_batch_decompress(void);
-
-/**
- * Stop batch decompress
- */
-GRK_API void GRK_CALLCONV grk_plugin_stop_batch_decompress(void);
-
-#ifdef __cplusplus
-}
-#endif
+/*
+ *    Copyright (C) 2016-2023 Grok Image Compression Inc.
+ *
+ *    This source code is free software: you can redistribute it and/or  modify
+ *    it under the terms of the GNU Affero General Public License, version 3,
+ *    as published by the Free Software Foundation.
+ *
+ *    This source code is distributed in the hope that it will be useful,
+ *    but WITHOUT ANY WARRANTY; without even the implied warranty of
+ *    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ *    GNU Affero General Public License for more details.
+ *
+ *    You should have received a copy of the GNU Affero General Public License
+ *    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+ *
+ *
+ *    This source code incorporates work covered by the BSD 2-clause license.
+ *    Please see the LICENSE file in the root directory for details.
+ *
+ */
+#pragma once
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "grk_config.h"
+#include <stdint.h>
+#include <stdio.h>
+#include <stdbool.h>
+#include <limits.h>
+
+#ifdef _WIN32
+#define GRK_CALLCONV __stdcall
+#ifdef GRK_STATIC
+#define GRK_API
+#else
+#ifdef GRK_EXPORTS
+#define GRK_API __declspec(dllexport)
+#else
+#define GRK_API __declspec(dllimport)
+#endif
+#endif
+#else
+#define GRK_CALLCONV
+#ifdef GRK_STATIC
+#define GRK_API __attribute__((visibility("hidden")))
+#else
+#define GRK_API __attribute__((visibility("default")))
+#endif
+#endif
+
+/**
+ * Progression order
+ * */
+typedef enum _GRK_PROG_ORDER
+{
+  GRK_PROG_UNKNOWN = -1, /**< place-holder */
+  GRK_LRCP = 0, /**< layer-resolution-component-precinct order */
+  GRK_RLCP = 1, /**< resolution-layer-component-precinct order */
+  GRK_RPCL = 2, /**< resolution-precinct-component-layer order */
+  GRK_PCRL = 3, /**< precinct-component-resolution-layer order */
+  GRK_CPRL = 4, /**< component-precinct-resolution-layer order */
+  GRK_NUM_PROGRESSION_ORDERS = 5 /** number of possible progression orders */
+} GRK_PROG_ORDER;
+
+/**
+ * Supported color spaces
+ * */
+typedef enum _GRK_COLOR_SPACE
+{
+  GRK_CLRSPC_UNKNOWN = 0, /**< unknown */
+  GRK_CLRSPC_SRGB = 2, /**< sRGB */
+  GRK_CLRSPC_GRAY = 3, /**< grayscale */
+  GRK_CLRSPC_SYCC = 4, /**< standard YCC (YUV) */
+  GRK_CLRSPC_EYCC = 5, /**< extended YCC */
+  GRK_CLRSPC_CMYK = 6, /**< CMYK */
+  GRK_CLRSPC_DEFAULT_CIE = 7, /**< default CIE LAB */
+  GRK_CLRSPC_CUSTOM_CIE = 8, /**< custom CIE LAB */
+  GRK_CLRSPC_ICC = 9 /**< ICC profile */
+} GRK_COLOR_SPACE;
+
+/* JPEG 2000 standard colour space enumeration */
+typedef enum _GRK_ENUM_COLOUR_SPACE
+{
+  GRK_ENUM_CLRSPC_UNKNOWN = 0xFFFFFFFF,
+  GRK_ENUM_CLRSPC_BILEVEL1 = 0,
+  GRK_ENUM_CLRSPC_YCBCR1 = 1,
+  GRK_ENUM_CLRSPC_YCBCR2 = 3,
+  GRK_ENUM_CLRSPC_YCBCR3 = 4,
+  GRK_ENUM_CLRSPC_PHOTO_YCC = 9, /* Kodak PhotoYCC */
+  GRK_ENUM_CLRSPC_CMY = 11, /* cyan, magenta, yellow */
+  GRK_ENUM_CLRSPC_CMYK = 12, /* cyan, magenta, yellow, black */
+  GRK_ENUM_CLRSPC_YCCK = 13,
+  GRK_ENUM_CLRSPC_CIE = 14,
+  GRK_ENUM_CLRSPC_BILEVEL2 = 15,
+  GRK_ENUM_CLRSPC_SRGB = 16,
+  GRK_ENUM_CLRSPC_GRAY = 17,
+  GRK_ENUM_CLRSPC_SYCC = 18, /* standard YCC */
+  GRK_ENUM_CLRSPC_CIEJAB = 19,
+  GRK_ENUM_CLRSPC_ESRGB = 20,
+  GRK_ENUM_CLRSPC_ROMMRGB = 21, /* Reference Output Medium Metric RGB */
+  GRK_ENUM_CLRSPC_YPBPR60 = 22,
+  GRK_ENUM_CLRSPC_YPBPR50 = 23,
+  GRK_ENUM_CLRSPC_EYCC = 24, /* extended YCC */
+} GRK_ENUM_COLOUR_SPACE;
+
+#define GRK_NUM_COMMENTS_SUPPORTED 256
+#define GRK_NUM_ASOC_BOXES_SUPPORTED 256
+#define GRK_MAX_COMMENT_LENGTH (UINT16_MAX - 2)
+#define GRK_MAX_SUPPORTED_IMAGE_PRECISION 16 /* Maximum supported precision in library */
+
+/* BIBO analysis - extra bits needed to avoid overflow:
+
+ Lossless:
+ without colour transform: 4 extra bits
+ with colour transform:    5 extra bits
+
+ Lossy:
+
+ Need 1 extra bit
+
+ So,  worst-case scenario is lossless with colour transform : need to add 5 more bits to prec to
+ avoid overflow
+ */
+#define BIBO_EXTRA_BITS 7
+
+#define GRK_MAX_PASSES (3 * (GRK_MAX_SUPPORTED_IMAGE_PRECISION + BIBO_EXTRA_BITS) - 2)
+
+/**
+ * Logging callback
+ *
+ * @param msg               message
+ * @param client_data       client data passed to callback
+ * */
+typedef void (*grk_msg_callback)(const char* msg, void* client_data);
+
+/**
+ *
+ * Grok ref-counted object
+ *
+ */
+typedef struct _grk_object
+{
+  void* wrapper;
+} grk_object;
+
+/**
+ * Progression order change
+ *
+ */
+typedef struct _grk_progression
+{
+  GRK_PROG_ORDER progression;
+  char progressionString[5];
+  GRK_PROG_ORDER specifiedCompressionPocProg;
+  uint32_t tileno;
+  /** tile dimensions */
+  uint32_t tx0;
+  uint32_t ty0;
+  uint32_t tx1;
+  uint32_t ty1;
+  /** progression order bounds specified by POC */
+  uint16_t compS;
+  uint16_t compE;
+  uint8_t resS;
+  uint8_t resE;
+  uint64_t precS;
+  uint64_t precE;
+  uint16_t layS;
+  uint16_t layE;
+  uint16_t tpCompS;
+  uint16_t tpCompE;
+  uint8_t tpResS;
+  uint8_t tpResE;
+  uint64_t tpPrecE;
+  uint16_t tpLayE;
+  uint32_t tp_txS;
+  uint32_t tp_txE;
+  uint32_t tp_tyS;
+  uint32_t tp_tyE;
+  uint32_t dx;
+  uint32_t dy;
+  uint16_t comp_temp;
+  uint8_t res_temp;
+  uint64_t prec_temp;
+  uint16_t lay_temp;
+  uint32_t tx0_temp;
+  uint32_t ty0_temp;
+} grk_progression;
+
+/** RAW component compress parameters */
+typedef struct _grk_raw_comp_cparameters
+{
+  uint8_t dx; /** subsampling in X direction */
+  uint8_t dy; /** subsampling in Y direction */
+  /*@}*/
+} grk_raw_comp_cparameters;
+
+/**RAW image compress parameters */
+typedef struct _grk_raw_cparameters
+{
+  uint32_t width; /** width of the raw image */
+  uint32_t height; /** height of the raw image */
+  uint16_t numcomps; /** number of components of the raw image */
+  uint8_t prec; /** bit depth of the raw image */
+  bool sgnd; /** signed/unsigned raw image */
+  grk_raw_comp_cparameters* comps; /** raw components parameters */
+} grk_raw_cparameters;
+
+/**
+ * Rate control algorithms
+  GRK_RATE_CONTROL_BISECT: bisect with all truncation points
+  GRK_RATE_CONTROL_PCRD_OPT: bisect with only feasible truncation points
+ */
+typedef enum _GRK_RATE_CONTROL_ALGORITHM
+{
+  GRK_RATE_CONTROL_BISECT,
+  GRK_RATE_CONTROL_PCRD_OPT
+} GRK_RATE_CONTROL_ALGORITHM;
+
+/**
+ * All supported file formats
+ */
+typedef enum _GRK_SUPPORTED_FILE_FMT
+{
+  GRK_FMT_UNK,
+  GRK_FMT_J2K,
+  GRK_FMT_JP2,
+  GRK_FMT_PXM,
+  GRK_FMT_PGX,
+  GRK_FMT_PAM,
+  GRK_FMT_BMP,
+  GRK_FMT_TIF,
+  GRK_FMT_RAW, /* MSB / Big Endian */
+  GRK_FMT_PNG,
+  GRK_FMT_RAWL, /* LSB / Little Endian */
+  GRK_FMT_JPG
+} GRK_SUPPORTED_FILE_FMT;
+
+/**
+ * Supported JPEG 2000 formats
+ */
+typedef enum _GRK_CODEC_FORMAT
+{
+  GRK_CODEC_UNK, /**< unknown format */
+  GRK_CODEC_J2K, /**< JPEG 2000 code stream format */
+  GRK_CODEC_JP2 /**< JP2 file format */
+} GRK_CODEC_FORMAT;
+
+#define GRK_PATH_LEN 4096 /* Maximum allowed filename size */
+#define GRK_MAX_LAYERS 100 /* Maximum number of quality layers */
+
+/*
+ * Note: range for number of decomposition levels is 0-32
+ * So, accordingly, range for number of resolutions is 1-33
+ */
+#define GRK_J2K_MAX_DECOMP_LVLS                                    \
+  32 /* Maximum number of decomposition levels allowed by standard \
+      */
+#define GRK_J2K_MAXRLVLS \
+  (GRK_J2K_MAX_DECOMP_LVLS + 1) /* Maximum number of resolution levels allowed by standard*/
+#define GRK_J2K_MAXBANDS \
+  (3 * GRK_J2K_MAXRLVLS - 2) /*  Maximum number of sub-bands allowed by standard */
+
+/**
+ * Note: "component" refers to an image component as decompressed
+ * from the code stream, while "channel" refers to a component resulting
+ * from the application of a Palette box LUT and a Component mapping box.
+ */
+
+/**
+ Component mappings: component index, mapping type, palette column
+ */
+typedef struct _grk_component_mapping_comp
+{
+  uint16_t component_index;
+  uint8_t mapping_type;
+  uint8_t palette_column;
+} grk_component_mapping_comp;
+
+/**
+ Palette data
+ */
+typedef struct _grk_palette_data
+{
+  int32_t* lut;
+  uint16_t num_entries;
+  grk_component_mapping_comp* component_mapping;
+  uint8_t num_channels;
+  bool* channel_sign;
+  uint8_t* channel_prec;
+} grk_palette_data;
+
+/***
+ * Channel Definition box structures and enums.
+ * When no Component mapping box is present, it is still possible to have
+ * a Channel defintion box, in which case channels are associated with components
+ * in the obvious way : channel `k` corresponds to component `k`.
+ * */
+
+/* channel type */
+typedef enum _GRK_CHANNEL_TYPE
+{
+  GRK_CHANNEL_TYPE_COLOUR = 0,
+  GRK_CHANNEL_TYPE_OPACITY = 1,
+  GRK_CHANNEL_TYPE_PREMULTIPLIED_OPACITY = 2,
+  GRK_CHANNEL_TYPE_UNSPECIFIED = 65535U
+
+} GRK_CHANNEL_TYPE;
+
+/* channel association */
+typedef enum _GRK_CHANNEL_ASSOC
+{
+
+  GRK_CHANNEL_ASSOC_WHOLE_IMAGE = 0,
+  GRK_CHANNEL_ASSOC_COLOUR_1 = 1,
+  GRK_CHANNEL_ASSOC_COLOUR_2 = 2,
+  GRK_CHANNEL_ASSOC_COLOUR_3 = 3,
+  GRK_CHANNEL_ASSOC_UNASSOCIATED = 65535U
+
+} GRK_CHANNEL_ASSOC;
+
+/**
+ Channel definition: channel index, type, association
+ */
+typedef struct _grk_channel_description
+{
+  uint16_t channel;
+  uint16_t typ;
+  uint16_t asoc;
+} grk_channel_description;
+
+/**
+ Channel definitions and number of definitions
+ */
+typedef struct _grk_channel_definition
+{
+  grk_channel_description* descriptions;
+  uint16_t num_channel_descriptions;
+} grk_channel_definition;
+
+/**
+ ICC profile, palette, channel definition
+ */
+typedef struct _grk_color
+{
+  uint8_t* icc_profile_buf;
+  uint32_t icc_profile_len;
+  char* icc_profile_name;
+  grk_channel_definition* channel_definition;
+  grk_palette_data* palette;
+  bool has_colour_specification_box;
+} grk_color;
+
+/**
+ * Association box info
+ */
+typedef struct _grk_asoc
+{
+  uint32_t level; /* 0 for root level */
+  const char* label;
+  uint8_t* xml;
+  uint32_t xml_len;
+} grk_asoc;
+
+/**
+ * Precision mode
+ */
+typedef enum _grk_precision_mode
+{
+  GRK_PREC_MODE_CLIP,
+  GRK_PREC_MODE_SCALE
+} grk_precision_mode;
+
+/**
+ * Precision
+ */
+typedef struct _grk_precision
+{
+  uint8_t prec;
+  grk_precision_mode mode;
+} grk_precision;
+
+/**
+ * Header info
+ */
+typedef struct _grk_header_info
+{
+  /******************************************
+  set by client only if decompressing to file
+  *******************************************/
+  GRK_SUPPORTED_FILE_FMT decompressFormat;
+  bool forceRGB;
+  bool upsample;
+  grk_precision* precision;
+  uint32_t numPrecision;
+  bool splitByComponent;
+  bool singleTileDecompress;
+  /****************************************/
+
+  /*****************************************
+  populated by library after reading header
+  ******************************************/
+  /** initial code block width, default to 64 */
+  uint32_t cblockw_init;
+  /** initial code block height, default to 64 */
+  uint32_t cblockh_init;
+  /** 1 : use the irreversible DWT 9-7, 0 : use lossless compression (default) */
+  bool irreversible;
+  /** multi-component transform identifier */
+  uint32_t mct;
+  /** RSIZ value
+   To be used to combine GRK_PROFILE_*, GRK_EXTENSION_* and (sub)levels values. */
+  uint16_t rsiz;
+  /** number of resolutions */
+  uint32_t numresolutions;
+  /*********************************************************
+  coding style can be specified in main header COD segment,
+  tile header COD segment, and tile component COC segment.
+  *********************************************************/
+  /* !!!! assume that coding style does not vary across tile components */
+  uint8_t csty;
+  /*******************************************************************
+  code block style is specified in main header COD segment, and can
+  be overridden in a tile header.  !!! Assume that style does
+  not vary across tiles !!!
+  *******************************************************************/
+  uint8_t cblk_sty;
+  /** initial precinct width */
+  uint32_t prcw_init[GRK_J2K_MAXRLVLS];
+  /** initial precinct height */
+  uint32_t prch_init[GRK_J2K_MAXRLVLS];
+  /** XTOsiz */
+  uint32_t tx0;
+  /** YTOsiz */
+  uint32_t ty0;
+  /** XTsiz */
+  uint32_t t_width;
+  /** YTsiz */
+  uint32_t t_height;
+  /** tile grid width */
+  uint32_t t_grid_width;
+  /** tile grid height  */
+  uint32_t t_grid_height;
+  /** maximum number of layers */
+  uint16_t max_layers_;
+  /*************************************
+  note: xml_data will remain valid
+   until codec is destroyed
+   ************************************/
+  uint8_t* xml_data;
+  size_t xml_data_len;
+  size_t num_comments;
+  char* comment[GRK_NUM_COMMENTS_SUPPORTED];
+  uint16_t comment_len[GRK_NUM_COMMENTS_SUPPORTED];
+  bool isBinaryComment[GRK_NUM_COMMENTS_SUPPORTED];
+
+  grk_asoc asocs[GRK_NUM_ASOC_BOXES_SUPPORTED];
+  uint32_t num_asocs;
+} grk_header_info;
+
+typedef struct _grk_io_buf
+{
+  uint8_t* data_;
+  size_t offset_;
+  size_t len_;
+  size_t allocLen_;
+  bool pooled_;
+  uint32_t index_;
+} grk_io_buf;
+
+typedef struct _grk_io_init
+{
+  uint32_t maxPooledRequests_;
+
+} grk_io_init;
+
+typedef bool (*grk_io_callback)(uint32_t threadId, grk_io_buf buffer, void* io_user_data);
+typedef void (*grk_io_register_reclaim_callback)(grk_io_init io_init,
+                                                 grk_io_callback reclaim_callback,
+                                                 void* io_user_data, void* reclaim_user_data);
+typedef bool (*grk_io_pixels_callback)(uint32_t threadId, grk_io_buf buffer, void* user_data);
+
+/**
+ * read stream callback
+ *
+ * @buffer buffer to write stream to
+ * @numBytes number of bytes to write to buffer
+ * @user_data user data
+ *
+ */
+typedef size_t (*grk_stream_read_fn)(uint8_t* buffer, size_t numBytes, void* user_data);
+
+/**
+ * write stream callback
+ *
+ * @buffer buffer to read stream from
+ * @numBytes number of bytes to read from buffer
+ * @user_data user data
+ *
+ */
+typedef size_t (*grk_stream_write_fn)(const uint8_t* buffer, size_t numBytes, void* user_data);
+
+/**
+ * seek (absolute) callback
+ *
+ * @offset absolute stream offset
+ * @user_data user data
+ *
+ */
+typedef bool (*grk_stream_seek_fn)(uint64_t offset, void* user_data);
+
+/**
+ * free user data callback
+ *
+ * @user_data user data
+ *
+ */
+typedef void (*grk_stream_free_user_data_fn)(void* user_data);
+
+/**
+ * JPEG 2000 stream parameters. Client must populate one of the following options :
+ * 1. File
+ * 2. Buffer
+ * 3. Callback
+ */
+typedef struct _grk_stream_params
+{
+  /* 1. File */
+  const char* file;
+
+  /* 2. Buffer */
+  uint8_t* buf;
+  size_t buf_len;
+  /* length of compressed stream (set by compressor, not client) */
+  size_t buf_compressed_len;
+
+  /* 3. Callback */
+  grk_stream_read_fn read_fn;
+  grk_stream_write_fn write_fn;
+  grk_stream_seek_fn seek_fn;
+  grk_stream_free_user_data_fn free_user_data_fn; // optional
+  void* user_data;
+  size_t stream_len; // must be set for read stream
+  size_t double_buffer_len; // optional - default value is 1024 * 1024
+} grk_stream_params;
+
+typedef enum _GRK_TILE_CACHE_STRATEGY
+{
+  GRK_TILE_CACHE_NONE, /* no tile caching */
+  GRK_TILE_CACHE_IMAGE /* cache final tile image */
+} GRK_TILE_CACHE_STRATEGY;
+
+/**
+ * Core decompression parameters
+ * */
+typedef struct _grk_decompress_core_params
+{
+  /**
+   Set the number of highest resolution levels to be discarded.
+   The image resolution is effectively divided by 2 to the power of the number of discarded
+   levels. The reduce factor is limited by the smallest total number of decomposition levels among
+   tiles. if greater than zero, then image is decoded to original dimension divided by
+   2^(reduce); if equal to zero or not used, image is decompressed to full resolution
+   */
+  uint8_t reduce;
+  /**
+   Set the maximum number of quality layers to decompress.
+   If there are fewer quality layers than the specified number, all quality layers will be
+   decompressed. if != 0, then only the first "layer" layers are decompressed; if == 0 or not
+   used, all the quality layers are decompressed
+   */
+  uint16_t layers_to_decompress_;
+  GRK_TILE_CACHE_STRATEGY tileCacheStrategy;
+
+  uint32_t randomAccessFlags_;
+
+  grk_io_pixels_callback io_buffer_callback;
+  void* io_user_data;
+  grk_io_register_reclaim_callback io_register_client_callback;
+} grk_decompress_core_params;
+
+#define GRK_DECOMPRESS_COMPRESSION_LEVEL_DEFAULT (UINT_MAX)
+
+/**
+ * Decompression parameters
+ */
+typedef struct _grk_decompress_params
+{
+  /** core library parameters */
+  grk_decompress_core_params core;
+  /** input file name */
+  char infile[GRK_PATH_LEN];
+  /** output file name */
+  char outfile[GRK_PATH_LEN];
+  /** input file format*/
+  GRK_CODEC_FORMAT decod_format;
+  /** output file format*/
+  GRK_SUPPORTED_FILE_FMT cod_format;
+  /** Decompress window left boundary */
+  float dw_x0;
+  /** Decompress window right boundary */
+  float dw_x1;
+  /** Decompress window up boundary */
+  float dw_y0;
+  /** Decompress window bottom boundary */
+  float dw_y1;
+  /** tile number of the decompressed tile*/
+  uint16_t tileIndex;
+  bool singleTileDecompress;
+  grk_precision* precision;
+  uint32_t numPrecision;
+  /* force output colorspace to RGB */
+  bool force_rgb;
+  /* upsample components according to their dx/dy values */
+  bool upsample;
+  /* split output components to different files */
+  bool split_pnm;
+  /* serialize XML metadata to disk */
+  bool io_xml;
+  uint32_t compression;
+  /*****************************************************
+  compression "quality". Meaning of "quality" depends
+  on file format we are writing to
+  *****************************************************/
+  uint32_t compressionLevel;
+  /** Verbose mode */
+  bool verbose_;
+  int32_t deviceId;
+  uint32_t duration; /* in seconds */
+  uint32_t kernelBuildOptions;
+  uint32_t repeats;
+  uint32_t numThreads;
+  void* user_data;
+} grk_decompress_parameters;
+
+/**
+ * Image component
+ * */
+typedef struct _grk_image_comp
+{
+  /** x component offset compared to the whole image */
+  uint32_t x0;
+  /** y component offset compared to the whole image */
+  uint32_t y0;
+  /** data width */
+  uint32_t w;
+  /** data stride */
+  uint32_t stride;
+  /** data height */
+  uint32_t h;
+  /** XRsiz: horizontal separation of a sample of component with respect to the reference
+   * grid */
+  uint8_t dx;
+  /** YRsiz: vertical separation of a sample of component with respect to the reference grid
+   */
+  uint8_t dy;
+  /** precision */
+  uint8_t prec;
+  /* signed */
+  bool sgnd;
+  GRK_CHANNEL_TYPE type;
+  GRK_CHANNEL_ASSOC association;
+  /* component registration coordinates */
+  uint16_t Xcrg, Ycrg;
+  /** image component data */
+  int32_t* data;
+} grk_image_comp;
+
+/* Image meta data: colour, IPTC and XMP */
+typedef struct _grk_image_meta
+{
+  grk_object obj;
+  grk_color color;
+  uint8_t* iptc_buf;
+  size_t iptc_len;
+  uint8_t* xmp_buf;
+  size_t xmp_len;
+} grk_image_meta;
+
+typedef struct _grk_image
+{
+  grk_object obj;
+  /** XOsiz: horizontal offset from the origin of the reference grid
+   *  to the left side of the image area */
+  uint32_t x0;
+  /** YOsiz: vertical offset from the origin of the reference grid
+   *  to the top side of the image area */
+  uint32_t y0;
+  /** Xsiz: width of the reference grid */
+  uint32_t x1;
+  /** Ysiz: height of the reference grid */
+  uint32_t y1;
+  /** number of components in the image */
+  uint16_t numcomps;
+  GRK_COLOR_SPACE color_space;
+  bool paletteApplied_;
+  bool channelDefinitionApplied_;
+  bool has_capture_resolution;
+  double capture_resolution[2];
+  bool has_display_resolution;
+  double display_resolution[2];
+  GRK_SUPPORTED_FILE_FMT decompressFormat;
+  bool forceRGB;
+  bool upsample;
+  grk_precision* precision;
+  uint32_t numPrecision;
+  bool hasMultipleTiles;
+  bool splitByComponent;
+  uint16_t decompressNumComps;
+  uint32_t decompressWidth;
+  uint32_t decompressHeight;
+  uint8_t decompressPrec;
+  GRK_COLOR_SPACE decompressColourSpace;
+  grk_io_buf interleavedData;
+  uint32_t rowsPerStrip; // for storage to output format
+  uint32_t rowsPerTask; // for scheduling
+  uint64_t packedRowBytes;
+  grk_image_meta* meta;
+  grk_image_comp* comps;
+} grk_image;
+
+/*************************************************
+Structs to pass data between grok and plugin
+************************************************/
+/**
+ * Plugin pass
+ */
+typedef struct _grk_plugin_pass
+{
+  double distortionDecrease; /* distortion decrease up to and including this pass */
+  size_t rate; /* rate up to and including this pass */
+  size_t length; /* stream length for this pass */
+} grk_plugin_pass;
+
+/**
+ * Plugin code block
+ */
+typedef struct _grk_plugin_code_block
+{
+  /**************************
+  debug info
+  **************************/
+  uint32_t x0, y0, x1, y1;
+  unsigned int* contextStream;
+  /***************************/
+  uint32_t numPix;
+  uint8_t* compressedData;
+  uint32_t compressedDataLength;
+  uint8_t numBitPlanes;
+  size_t numPasses;
+  grk_plugin_pass passes[GRK_MAX_PASSES];
+  unsigned int sortedIndex;
+} grk_plugin_code_block;
+
+/**
+ * Plugin precinct
+ */
+typedef struct _grk_plugin_precinct
+{
+  uint64_t numBlocks;
+  grk_plugin_code_block** blocks;
+} grk_plugin_precinct;
+
+/**
+ * Plugin band
+ */
+typedef struct _grk_plugin_band
+{
+  uint8_t orientation;
+  uint64_t numPrecincts;
+  grk_plugin_precinct** precincts;
+  float stepsize;
+} grk_plugin_band;
+
+/**
+ * Plugin resolution
+ */
+typedef struct _grk_plugin_resolution
+{
+  size_t level;
+  size_t numBands;
+  grk_plugin_band** band;
+} grk_plugin_resolution;
+
+/**
+ * Plugin tile component
+ */
+typedef struct grk_plugin_tile_component
+{
+  size_t numResolutions;
+  grk_plugin_resolution** resolutions;
+} grk_plugin_tile_component;
+
+#define GRK_DECODE_HEADER (1 << 0)
+#define GRK_DECODE_T2 (1 << 1)
+#define GRK_DECODE_T1 (1 << 2)
+#define GRK_DECODE_POST_T1 (1 << 3)
+#define GRK_PLUGIN_DECODE_CLEAN (1 << 4)
+#define GRK_DECODE_ALL \
+  (GRK_PLUGIN_DECODE_CLEAN | GRK_DECODE_HEADER | GRK_DECODE_T2 | GRK_DECODE_T1 | GRK_DECODE_POST_T1)
+
+/**
+ * Plugin tile
+ */
+typedef struct _grk_plugin_tile
+{
+  uint32_t decompress_flags;
+  size_t numComponents;
+  grk_plugin_tile_component** tileComponents;
+} grk_plugin_tile;
+
+/* opaque codec object */
+typedef grk_object grk_codec;
+
+/**
+ * Library version
+ */
+GRK_API const char* GRK_CALLCONV grk_version(void);
+
+/**
+ * Initialize library
+ *
+ * @param pluginPath 	path to plugin
+ * @param numthreads 	number of threads to use for compress/decompress
+ */
+GRK_API void GRK_CALLCONV grk_initialize(const char* pluginPath, uint32_t numthreads, bool verbose);
+
+/**
+ * De-initialize library
+ */
+GRK_API void GRK_CALLCONV grk_deinitialize();
+
+/**
+ * Increment ref count
+ */
+GRK_API grk_object* GRK_CALLCONV grk_object_ref(grk_object* obj);
+
+/*
+ * Decrement ref count
+ *
+ */
+GRK_API void GRK_CALLCONV grk_object_unref(grk_object* obj);
+
+GRK_API void GRK_CALLCONV grk_set_msg_handlers(grk_msg_callback info_callback, void* info_user_data,
+                                               grk_msg_callback warn_callback, void* warn_user_data,
+                                               grk_msg_callback error_callback,
+                                               void* error_user_data);
+
+/**
+ * Create image
+ *
+ * @param numcmpts      number of components
+ * @param cmptparms     component parameters
+ * @param clrspc        image color space
+ * @param alloc_data    if true, allocate component data buffers
+ *
+ * @return returns      a new image if successful, otherwise NULL
+ * */
+GRK_API grk_image* GRK_CALLCONV grk_image_new(uint16_t numcmpts, grk_image_comp* cmptparms,
+                                              GRK_COLOR_SPACE clrspc, bool alloc_data);
+
+GRK_API grk_image_meta* GRK_CALLCONV grk_image_meta_new(void);
+
+/**
+ * Detect jpeg 2000 format from file
+ * Format is either GRK_FMT_J2K or GRK_FMT_JP2
+ *
+ * @param fileName file name
+ * @param fmt pointer to detected format
+ *
+ * @return true if format was detected, otherwise false
+ *
+ */
+GRK_API bool GRK_CALLCONV grk_decompress_detect_format(const char* fileName, GRK_CODEC_FORMAT* fmt);
+
+/**
+ * Initialize stream parameters with default values
+ *
+ * @param parameters stream parameters
+ */
+GRK_API void GRK_CALLCONV grk_set_default_stream_params(grk_stream_params* params);
+
+/**
+ * Initialize decompress parameters with default values
+ *
+ * @param parameters decompression parameters
+ */
+GRK_API void GRK_CALLCONV grk_decompress_set_default_params(grk_decompress_parameters* parameters);
+
+/**
+ * Initialize decompressor
+ *
+ * @param stream_params 	source stream parameters
+ * @param core_params 	decompress core parameters
+ *
+ * @return grk_codec* if successful, otherwise NULL
+ */
+GRK_API grk_codec* GRK_CALLCONV grk_decompress_init(grk_stream_params* stream_params,
+                                                    grk_decompress_core_params* core_params);
+
+/**
+ * Decompress JPEG 2000 header
+ *
+ * @param	codec				decompression codec
+ * @param	header_info			information read from JPEG 2000 header.
+ *
+ * @return true					if the main header of the code stream and the JP2 header
+ * 							 	is correctly read.
+ */
+GRK_API bool GRK_CALLCONV grk_decompress_read_header(grk_codec* codec,
+                                                     grk_header_info* header_info);
+
+/**
+ * Get decompressed tile image
+ *
+ * @param	codec				decompression codec
+ * @param	tileIndex			tile index
+ *
+ * @return pointer to decompressed image
+ */
+GRK_API grk_image* GRK_CALLCONV grk_decompress_get_tile_image(grk_codec* codec, uint16_t tileIndex);
+
+/**
+ * Get decompressed composite image
+ *
+ * @param	codec				decompression codec
+ *
+ * @return pointer to decompressed image
+ */
+GRK_API grk_image* GRK_CALLCONV grk_decompress_get_composited_image(grk_codec* codec);
+
+/**
+ * Set the given area to be decompressed. This function should be called
+ * right after grk_decompress_read_header is called, and before any tile header is read.
+ *
+ * @param	codec			decompression codec
+ * @param	start_x		    left position of the rectangle to decompress (in image coordinates).
+ * @param	end_x			the right position of the rectangle to decompress (in image
+ * coordinates).
+ * @param	start_y		    up position of the rectangle to decompress (in image coordinates).
+ * @param	end_y			bottom position of the rectangle to decompress (in image coordinates).
+ *
+ * @return	true			if the area could be set.
+ */
+GRK_API bool GRK_CALLCONV grk_decompress_set_window(grk_codec* codec, float start_x, float start_y,
+                                                    float end_x, float end_y);
+
+/**
+ * Decompress image from a JPEG 2000 code stream
+ *
+ * @param codec 	decompression codec
+ * @param tile		tile struct from plugin
+ *
+ * @return 			true if successful, otherwise false
+ * */
+GRK_API bool GRK_CALLCONV grk_decompress(grk_codec* codec, grk_plugin_tile* tile);
+
+/**
+ * Decompress a specific tile
+ *
+ * @param	codec			decompression codec
+ * @param	tileIndex		index of the tile to be decompressed
+ *
+ * @return					true if successful, otherwise false
+ */
+GRK_API bool GRK_CALLCONV grk_decompress_tile(grk_codec* codec, uint16_t tileIndex);
+
+/* COMPRESSION FUNCTIONS*/
+
+/**
+ * Compress parameters
+ * */
+typedef struct _grk_cparameters
+{
+  /** size of tile: tile_size_on = false (not in argument) or = true (in argument) */
+  bool tile_size_on;
+  /** XTOsiz */
+  uint32_t tx0;
+  /** YTOsiz */
+  uint32_t ty0;
+  /** XTsiz */
+  uint32_t t_width;
+  /** YTsiz */
+  uint32_t t_height;
+  /** number of layers */
+  uint16_t numlayers;
+  /** rate control allocation by rate/distortion curve */
+  bool allocationByRateDistoration;
+  /** layers rates expressed as compression ratios.
+   *  They might be subsequently limited by the max_cs_size field */
+  double layer_rate[GRK_MAX_LAYERS];
+  /** rate control allocation by fixed_PSNR quality */
+  bool allocationByQuality;
+  /** layer PSNR values */
+  double layer_distortion[GRK_MAX_LAYERS];
+  char* comment[GRK_NUM_COMMENTS_SUPPORTED];
+  uint16_t comment_len[GRK_NUM_COMMENTS_SUPPORTED];
+  bool is_binary_comment[GRK_NUM_COMMENTS_SUPPORTED];
+  size_t num_comments;
+  /** csty : coding style */
+  uint8_t csty;
+  /* number of guard bits */
+  uint8_t numgbits;
+  /** progression order (default is LRCP) */
+  GRK_PROG_ORDER prog_order;
+  /** progressions */
+  grk_progression progression[GRK_J2K_MAXRLVLS];
+  /** number of progression order changes (POCs), default to 0 */
+  uint32_t numpocs;
+  /** number of resolutions */
+  uint8_t numresolution;
+  /** initial code block width  (default to 64) */
+  uint32_t cblockw_init;
+  /** initial code block height (default to 64) */
+  uint32_t cblockh_init;
+  /** code block style */
+  uint8_t cblk_sty;
+  /** 1 : use the irreversible DWT 9-7, 0 :
+   *  use lossless compression (default) */
+  bool irreversible;
+  /** region of interest: affected component in [0..3];
+   *  -1 indicates no ROI */
+  int32_t roi_compno;
+  /** region of interest: upshift value */
+  uint32_t roi_shift;
+  /* number of precinct size specifications */
+  uint32_t res_spec;
+  /** initial precinct width */
+  uint32_t prcw_init[GRK_J2K_MAXRLVLS];
+  /** initial precinct height */
+  uint32_t prch_init[GRK_J2K_MAXRLVLS];
+  /** input file name */
+  char infile[GRK_PATH_LEN];
+  /** output file name */
+  char outfile[GRK_PATH_LEN];
+  /** subimage compressing: origin image offset in x direction */
+  uint32_t image_offset_x0;
+  /** subimage compressing: origin image offset in y direction */
+  uint32_t image_offset_y0;
+  /** subsampling value for dx */
+  uint8_t subsampling_dx;
+  /** subsampling value for dy */
+  uint8_t subsampling_dy;
+  /** input file format*/
+  GRK_SUPPORTED_FILE_FMT decod_format;
+  /** output file format*/
+  GRK_SUPPORTED_FILE_FMT cod_format;
+  grk_raw_cparameters raw_cp;
+  /** Tile part generation*/
+  bool enableTilePartGeneration;
+  /** new tile part progression divider */
+  uint8_t newTilePartProgressionDivider;
+  /** MCT (multiple component transform) */
+  uint8_t mct;
+  /** Naive implementation of MCT restricted to a single reversible array based
+   compressing without offset concerning all the components. */
+  void* mct_data;
+  /**
+   * Maximum size (in bytes) for the whole code stream.
+   * If equal to zero, code stream size limitation is not considered
+   * If it does not comply with layer_rate, max_cs_size prevails
+   * and a warning is issued.
+   * */
+  uint64_t max_cs_size;
+  /**
+   * Maximum size (in bytes) for each component.
+   * If == 0, component size limitation is not considered
+   * */
+  uint64_t max_comp_size;
+  /** RSIZ value
+   To be used to combine GRK_PROFILE_*, GRK_EXTENSION_* and (sub)levels values. */
+  uint16_t rsiz;
+  uint16_t framerate;
+
+  /* set to true if input file stores capture resolution */
+  bool write_capture_resolution_from_file;
+  double capture_resolution_from_file[2];
+
+  bool write_capture_resolution;
+  double capture_resolution[2];
+
+  bool write_display_resolution;
+  double display_resolution[2];
+
+  bool apply_icc_;
+
+  GRK_RATE_CONTROL_ALGORITHM rateControlAlgorithm;
+  uint32_t numThreads;
+  int32_t deviceId;
+  uint32_t duration; /* seconds */
+  uint32_t kernelBuildOptions;
+  uint32_t repeats;
+  bool writePLT;
+  bool writeTLM;
+  bool verbose;
+  bool sharedMemoryInterface;
+} grk_cparameters;
+
+/**
+ Set compressing parameters to default values:
+
+ Lossless
+ Single tile
+ Size of precinct : 2^15 x 2^15 (i.e. single precinct)
+ Size of code block : 64 x 64
+ Number of resolutions: 6
+ No SOP marker in the code stream
+ No EPH marker in the code stream
+ No mode switches
+ Progression order: LRCP
+ No ROI upshifted
+ Image origin lies at (0,0)
+ Tile origin lies at (0,0)
+ Reversible DWT 5-3 transform
+
+ @param parameters Compression parameters
+ */
+GRK_API void GRK_CALLCONV grk_compress_set_default_params(grk_cparameters* parameters);
+
+/**
+ * Set up the compressor parameters using the current image and user parameters.
+ *
+ * @param codec 		compression codec
+ * @param parameters 	compression parameters
+ * @param image 		input image
+ */
+GRK_API grk_codec* GRK_CALLCONV grk_compress_init(grk_stream_params* stream_params,
+                                                  grk_cparameters* parameters, grk_image* p_image);
+
+/**
+ * Compress an image into a JPEG 2000 code stream using plugin
+ *
+ * @param codec 		compression codec
+ * @param tile			plugin tile
+ *
+ * @return 				number of bytes written if successful, 0 otherwise
+ */
+GRK_API uint64_t GRK_CALLCONV grk_compress(grk_codec* codec, grk_plugin_tile* tile);
+
+/**
+ * Dump codec information to file
+ *
+ * @param	codec			decompression codec
+ * @param	info_flag		type of information dump.
+ * @param	output_stream	codec information is dumped to output stream
+ *
+ */
+GRK_API void GRK_CALLCONV grk_dump_codec(grk_codec* codec, uint32_t info_flag, FILE* output_stream);
+
+/**
+ * Set the MCT matrix to use.
+ *
+ * @param	parameters		the parameters to change.
+ * @param	encodingMatrix	the compressing matrix.
+ * @param	dc_shift		the dc shift coefficients to use.
+ * @param	nbComp			the number of components of the image.
+ *
+ * @return	true if the parameters could be set.
+ */
+GRK_API bool GRK_CALLCONV grk_set_MCT(grk_cparameters* parameters, float* encodingMatrix,
+                                      int32_t* dc_shift, uint32_t nbComp);
+
+#define GRK_IMG_INFO 1 /* Basic image information provided to the user */
+#define GRK_J2K_MH_INFO 2 /* Codestream information based only on the main header */
+#define GRK_J2K_TH_INFO 4 /* Tile information based on the current tile header */
+#define GRK_J2K_TCH_INFO 8 /**< Tile/Component information of all tiles */
+#define GRK_J2K_MH_IND 16 /**< Codestream index based only on the main header */
+#define GRK_J2K_TH_IND 32 /**< Tile index based on the current tile */
+#define GRK_JP2_INFO 128 /**< JP2 file information */
+#define GRK_JP2_IND 256 /**< JP2 file index */
+
+#define GRK_CBLKSTY_LAZY 0x001 /**< Selective arithmetic coding bypass */
+#define GRK_CBLKSTY_RESET 0x002 /**< Reset context probabilities on coding pass boundaries */
+#define GRK_CBLKSTY_TERMALL 0x004 /**< Termination on each coding pass */
+#define GRK_CBLKSTY_VSC 0x008 /**< Vertical stripe causal context */
+#define GRK_CBLKSTY_PTERM 0x010 /**< Predictable termination */
+#define GRK_CBLKSTY_SEGSYM 0x020 /**< Segmentation symbols are used */
+#define GRK_CBLKSTY_HT 0x040 /**< high throughput block coding */
+#define GRK_CBLKSTY_HT_MIXED 0x080 /**< high throughput block coding - mixed*/
+#define GRK_CBLKSTY_HT_PHLD 0x100 /**< high throughput block coding - placeholder */
+#define GRK_JPH_RSIZ_FLAG 0x4000 /**<for JPH, bit 14 of RSIZ must be set to 1 */
+
+/*****************************************************************************
+ * JPEG 2000 Profiles, see Table A.10 from 15444-1 (updated in various AMDs)
+ *
+ * These values help choose the RSIZ value for the JPEG 2000 code stream.
+ * The RSIZ value forces various compressing options, as detailed in Table A.10.
+ * If GRK_PROFILE_PART2 is chosen, it must be combined with one or more extensions
+ * described below.
+ *
+ *   Example: rsiz = GRK_PROFILE_PART2 | GRK_EXTENSION_MCT;
+ *
+ * For broadcast profiles, the GRK_PROFILE_X value has to be combined with the target
+ * level (3-0 LSB, value between 0 and 11):
+ *   Example: rsiz = GRK_PROFILE_BC_MULTI | 0x0005; //level equals 5
+ *
+ * For IMF profiles, the GRK_PROFILE_X value has to be combined with the target main-level
+ * (3-0 LSB, value between 0 and 11) and sub-level (7-4 LSB, value between 0 and 9):
+ *   Example: rsiz = GRK_PROFILE_IMF_2K | 0x0040 | 0x0005; // main-level equals 5 and sub-level
+ * equals 4
+ *
+ * */
+#define GRK_PROFILE_NONE 0x0000 /** no profile, conform to 15444-1 */
+#define GRK_PROFILE_0 0x0001 /** Profile 0 as described in 15444-1,Table A.45 */
+#define GRK_PROFILE_1 0x0002 /** Profile 1 as described in 15444-1,Table A.45 */
+#define GRK_PROFILE_CINEMA_2K 0x0003 /** 2K cinema profile defined in 15444-1 AMD1 */
+#define GRK_PROFILE_CINEMA_4K 0x0004 /** 4K cinema profile defined in 15444-1 AMD1 */
+#define GRK_PROFILE_CINEMA_S2K 0x0005 /** Scalable 2K cinema profile defined in 15444-1 AMD2 */
+#define GRK_PROFILE_CINEMA_S4K 0x0006 /** Scalable 4K cinema profile defined in 15444-1 AMD2 */
+#define GRK_PROFILE_CINEMA_LTS \
+  0x0007 /** Long term storage cinema profile defined in 15444-1 AMD2 */
+#define GRK_PROFILE_BC_SINGLE 0x0100 /** Single Tile Broadcast profile defined in 15444-1 AMD3 */
+#define GRK_PROFILE_BC_MULTI 0x0200 /** Multi Tile Broadcast profile defined in 15444-1 AMD3 */
+#define GRK_PROFILE_BC_MULTI_R \
+  0x0300 /** Multi Tile Reversible Broadcast profile defined in 15444-1 AMD3 */
+#define GRK_PROFILE_BC_MASK 0x030F /** Mask for broadcast profile including main level */
+#define GRK_PROFILE_IMF_2K 0x0400 /** 2K Single Tile Lossy IMF profile defined in 15444-1 AMD8 */
+#define GRK_PROFILE_IMF_4K 0x0500 /** 4K Single Tile Lossy IMF profile defined in 15444-1 AMD8 */
+#define GRK_PROFILE_IMF_8K 0x0600 /** 8K Single Tile Lossy IMF profile defined in 15444-1 AMD8 */
+#define GRK_PROFILE_IMF_2K_R \
+  0x0700 /** 2K Single/Multi Tile Reversible IMF profile defined in 15444-1 AMD8 */
+#define GRK_PROFILE_IMF_4K_R \
+  0x0800 /** 4K Single/Multi Tile Reversible IMF profile defined in 15444-1 AMD8 */
+#define GRK_PROFILE_IMF_8K_R \
+  0x0900 /** 8K Single/Multi Tile Reversible IMF profile defined in 15444-1 AMD8 */
+#define GRK_PROFILE_MASK 0x0FFF /** Mask for profile bits */
+#define GRK_PROFILE_PART2 0x8000 /** At least 1 extension defined in 15444-2 (Part-2) */
+#define GRK_PROFILE_PART2_EXTENSIONS_MASK 0x3FFF // Mask for Part-2 extension bits
+
+/**
+ * JPEG 2000 Part-2 extensions
+ * */
+#define GRK_EXTENSION_NONE 0x0000 /** No Part-2 extension */
+#define GRK_EXTENSION_MCT 0x0100 /** Custom MCT support */
+#define GRK_IS_PART2(v) ((v)&GRK_PROFILE_PART2)
+
+#define GRK_IS_CINEMA(v) (((v) >= GRK_PROFILE_CINEMA_2K) && ((v) <= GRK_PROFILE_CINEMA_S4K))
+#define GRK_IS_STORAGE(v) ((v) == GRK_PROFILE_CINEMA_LTS)
+
+/*
+ *
+ * *********************************************
+ * Broadcast level (3-0 LSB) (15444-1 AMD4,AMD8)
+ * *********************************************
+ *
+ * indicates maximum bit rate and sample rate for a code stream
+ *
+ * Note: Mbit/s == 10^6 bits/s;  Msamples/s == 10^6 samples/s
+ *
+ * 0:       no maximum rate
+ * 1:       200 Mbits/s, 65  Msamples/s
+ * 2:       200 Mbits/s, 130 Msamples/s
+ * 3:       200 Mbits/s, 195 Msamples/s
+ * 4:       400 Mbits/s, 260 Msamples/s
+ * 5:       800Mbits/s,  520 Msamples/s
+ * >= 6:    2^(level-6) * 1600 Mbits/s, 2^(level-6) * 1200 Msamples/s
+ *
+ * Note: level cannot be greater than 11
+ *
+ * ****************
+ * Broadcast tiling
+ * ****************
+ *
+ * Either single-tile or multi-tile. Multi-tile only permits
+ * 1 or 4 tiles per frame, where multiple tiles have identical
+ * sizes, and are configured in either 2x2 or 1x4 layout.
+ *
+ *************************************************************
+ *
+ * ***************************************
+ * IMF main-level (3-0) LSB (15444-1 AMD8)
+ * ***************************************
+ *
+ * main-level indicates maximum number of samples per second,
+ * as listed above.
+ *
+ *
+ * **************************************
+ * IMF sub-level (7-4) LSB (15444-1 AMD8)
+ * **************************************
+ *
+ * sub-level indicates maximum bit rate for a code stream:
+ *
+ * 0:   no maximum rate
+ * >0:  2^sub-level * 100 Mbits/second
+ *
+ * Note: sub-level cannot be greater than 9, and cannot be larger
+ * then maximum of (main-level -2) and 1.
+ *
+ */
+
+#define GRK_GET_IMF_OR_BROADCAST_PROFILE(v) \
+  ((v)&0x0f00) /** Extract profile without mainlevel/sublevel */
+
+#define GRK_LEVEL_MAX 11U /** Maximum (main) level */
+#define GRK_GET_LEVEL(v) ((v)&0xf) /** Extract (main) level */
+
+/******* BROADCAST **********************************************************/
+
+#define GRK_IS_BROADCAST(v)                                                        \
+  (((v) >= GRK_PROFILE_BC_SINGLE) && ((v) <= (GRK_PROFILE_BC_MULTI_R | 0x000b)) && \
+   (((v)&0xf) <= 0xb))
+
+/* Maximum component sampling Rate (Mbits/sec) per level */
+#define GRK_BROADCAST_LEVEL_1_MBITSSEC 200U /** Mbits/sec for level 1 */
+#define GRK_BROADCAST_LEVEL_2_MBITSSEC 200U /** Mbits/sec for level 2 */
+#define GRK_BROADCAST_LEVEL_3_MBITSSEC 200U /** Mbits/sec for level 3 */
+#define GRK_BROADCAST_LEVEL_4_MBITSSEC 400U /** Mbits/sec for level 4 */
+#define GRK_BROADCAST_LEVEL_5_MBITSSEC 800U /** Mbits/sec for level 5 */
+#define GRK_BROADCAST_LEVEL_6_MBITSSEC 1600U /** Mbits/sec for level 6 */
+#define GRK_BROADCAST_LEVEL_7_MBITSSEC 3200U /** Mbits/sec for level 7 */
+#define GRK_BROADCAST_LEVEL_8_MBITSSEC 6400U /** Mbits/sec for level 8 */
+#define GRK_BROADCAST_LEVEL_9_MBITSSEC 12800U /** Mbits/sec for level 9 */
+#define GRK_BROADCAST_LEVEL_10_MBITSSEC 25600U /** Mbits/sec for level 10 */
+#define GRK_BROADCAST_LEVEL_11_MBITSSEC 51200U /** Mbits/sec for level 11 */
+
+#define GRK_BROADCAST_LEVEL_1_MSAMPLESSEC 64U /** MSamples/sec for level 1 */
+#define GRK_BROADCAST_LEVEL_2_MSAMPLESSEC 130U /** MSamples/sec for level 2 */
+#define GRK_BROADCAST_LEVEL_3_MSAMPLESSEC 195U /** MSamples/sec for level 3 */
+#define GRK_BROADCAST_LEVEL_4_MSAMPLESSEC 260U /** MSamples/sec for level 4 */
+#define GRK_BROADCAST_LEVEL_5_MSAMPLESSEC 520U /** MSamples/sec for level 5 */
+#define GRK_BROADCAST_LEVEL_6_MSAMPLESSEC 1200U /** MSamples/sec for level 6 */
+#define GRK_BROADCAST_LEVEL_7_MSAMPLESSEC 2400U /** MSamples/sec for level 7 */
+#define GRK_BROADCAST_LEVEL_8_MSAMPLESSEC 4800U /** MSamples/sec for level 8 */
+#define GRK_BROADCAST_LEVEL_9_MSAMPLESSEC 9600U /** MSamples/sec for level 9 */
+#define GRK_BROADCAST_LEVEL_10_MSAMPLESSEC 19200U /** MSamples/sec for level 10 */
+#define GRK_BROADCAST_LEVEL_11_MSAMPLESSEC 38400U /** MSamples/sec for level 11 */
+
+/********IMF *****************************************************************/
+
+#define GRK_IS_IMF(v)                                                         \
+  (((v) >= GRK_PROFILE_IMF_2K) && ((v) <= (GRK_PROFILE_IMF_8K_R | 0x009b)) && \
+   (((v)&0xf) <= 0xb) && (((v)&0xf0) <= 0x90))
+
+/* Maximum component sampling rate (MSamples/sec) per main level */
+#define GRK_IMF_MAINLEVEL_1_MSAMPLESSEC 65U /** MSamples/sec for main level 1 */
+#define GRK_IMF_MAINLEVEL_2_MSAMPLESSEC 130U /** MSamples/sec for main level 2 */
+#define GRK_IMF_MAINLEVEL_3_MSAMPLESSEC 195U /** MSamples/sec for main level 3 */
+#define GRK_IMF_MAINLEVEL_4_MSAMPLESSEC 260U /** MSamples/sec for main level 4 */
+#define GRK_IMF_MAINLEVEL_5_MSAMPLESSEC 520U /** MSamples/sec for main level 5 */
+#define GRK_IMF_MAINLEVEL_6_MSAMPLESSEC 1200U /** MSamples/sec for main level 6 */
+#define GRK_IMF_MAINLEVEL_7_MSAMPLESSEC 2400U /** MSamples/sec for main level 7 */
+#define GRK_IMF_MAINLEVEL_8_MSAMPLESSEC 4800U /** MSamples/sec for main level 8 */
+#define GRK_IMF_MAINLEVEL_9_MSAMPLESSEC 9600U /** MSamples/sec for main level 9 */
+#define GRK_IMF_MAINLEVEL_10_MSAMPLESSEC 19200U /** MSamples/sec for main level 10 */
+#define GRK_IMF_MAINLEVEL_11_MSAMPLESSEC 38400U /** MSamples/sec for main level 11 */
+
+#define GRK_IMF_SUBLEVEL_MAX 9U /** Maximum IMF sublevel */
+#define GRK_GET_IMF_SUBLEVEL(v) (((v) >> 4) & 0xf) /** Extract IMF sub level */
+
+/** Maximum compressed bit rate (Mbits/s) per IMF sub level */
+#define GRK_IMF_SUBLEVEL_1_MBITSSEC 200U /** Mbits/s for IMF sub level 1 */
+#define GRK_IMF_SUBLEVEL_2_MBITSSEC 400U /** Mbits/s for IMF sub level 2 */
+#define GRK_IMF_SUBLEVEL_3_MBITSSEC 800U /** Mbits/s for IMF sub level 3 */
+#define GRK_IMF_SUBLEVEL_4_MBITSSEC 1600U /** Mbits/s for IMF sub level 4 */
+#define GRK_IMF_SUBLEVEL_5_MBITSSEC 3200U /** Mbits/s for IMF sub level 5 */
+#define GRK_IMF_SUBLEVEL_6_MBITSSEC 6400U /** Mbits/s for IMF sub level 6 */
+#define GRK_IMF_SUBLEVEL_7_MBITSSEC 12800U /** Mbits/s for IMF sub level 7 */
+#define GRK_IMF_SUBLEVEL_8_MBITSSEC 25600U /** Mbits/s for IMF sub level 8 */
+#define GRK_IMF_SUBLEVEL_9_MBITSSEC 51200U /** Mbits/s for IMF sub level 9 */
+/**********************************************************************************/
+
+/**
+ * JPEG 2000 cinema profile code stream and component size limits
+ * */
+
+#define GRK_CINEMA_DCI_MAX_BANDWIDTH 250000000
+
+#define GRK_CINEMA_24_CS 1302083 /** Maximum code stream length @ 24fps */
+#define GRK_CINEMA_24_COMP 1041666 /** Maximum size per color component @ 24fps */
+
+#define GRK_CINEMA_48_CS 651041 /** Maximum code stream length @ 48fps */
+#define GRK_CINEMA_48_COMP 520833 /** Maximum size per color component @ 48fps */
+
+#define GRK_CINEMA_4K_DEFAULT_NUM_RESOLUTIONS 7
+
+/*
+ *
+ * CIE Lab #defines
+ */
+#define GRK_CUSTOM_CIELAB_SPACE 0x0
+#define GRK_DEFAULT_CIELAB_SPACE 0x44454600 /* 'DEF' */
+#define GRK_CIE_DAY ((((uint32_t)'C') << 24) + (((uint32_t)'T') << 16))
+#define GRK_CIE_D50 ((uint32_t)0x00443530)
+#define GRK_CIE_D65 ((uint32_t)0x00443635)
+#define GRK_CIE_D75 ((uint32_t)0x00443735)
+#define GRK_CIE_SA ((uint32_t)0x00005341)
+#define GRK_CIE_SC ((uint32_t)0x00005343)
+#define GRK_CIE_F2 ((uint32_t)0x00004632)
+#define GRK_CIE_F7 ((uint32_t)0x00004637)
+#define GRK_CIE_F11 ((uint32_t)0x00463131)
+
+/**
+ * Toggle random access markers
+ */
+#define GRK_RANDOM_ACCESS_PLT 1 /* use PLT marker if present */
+#define GRK_RANDOM_ACCESS_TLM 2 /* use TLM marker if present */
+#define GRK_RANDOM_ACCESS_PLM 4 /* use PLM marker if present */
+
+/*************************************************************************************
+ Plugin Interface
+ *************************************************************************************/
+
+/*
+ Plugin management
+ */
+
+typedef struct _grk_plugin_load_info
+{
+  const char* pluginPath;
+  bool verbose;
+} grk_plugin_load_info;
+
+/**
+ * Load plugin
+ *
+ * @param info		plugin loading info
+ */
+GRK_API bool GRK_CALLCONV grk_plugin_load(grk_plugin_load_info info);
+
+/**
+ * Release plugin resources
+ */
+GRK_API void GRK_CALLCONV grk_plugin_cleanup(void);
+
+/* No debug is done on plugin. Production setting. */
+#define GRK_PLUGIN_STATE_NO_DEBUG 0x0
+
+/*
+ For compress debugging, the plugin first performs a T1 compress.
+ Then:
+ 1. perform host DWT on plugin MCT data, and write to host image
+ This way, both plugin and host start from same point
+ (assume MCT is equivalent for both host and plugin)
+ 2. map plugin DWT data, compare with host DWT, and then write to plugin image
+ At this point in the code, the plugin image holds plugin DWT data. And if no warnings are
+ triggered, then we can safely say that host and plugin DWT data are identical.
+ 3. Perform host compress, skipping MCT and DWT (they have already been performed)
+ 4. during host compress, each context that is formed is compared against context stream from plugin
+ 5. rate control - synch with plugin code stream, and compare
+ 6. T2 and store to disk
+ */
+
+#define GRK_PLUGIN_STATE_DEBUG 0x1
+#define GRK_PLUGIN_STATE_PRE_TR1 0x2
+#define GRK_PLUGIN_STATE_DWT_QUANTIZATION 0x4
+#define GRK_PLUGIN_STATE_MCT_ONLY 0x8
+
+/**
+ * Get debug state of plugin
+ */
+GRK_API uint32_t GRK_CALLCONV grk_plugin_get_debug_state();
+
+/*
+ Plugin compressing
+ */
+typedef struct _grk_plugin_init_info
+{
+  int32_t deviceId;
+  bool verbose;
+  const char* license;
+  const char* server;
+} grk_plugin_init_info;
+
+/**
+ * Initialize plugin
+ */
+GRK_API bool GRK_CALLCONV grk_plugin_init(grk_plugin_init_info initInfo);
+
+typedef struct grk_plugin_compress_user_callback_info
+{
+  const char* input_file_name;
+  bool outputFileNameIsRelative;
+  const char* output_file_name;
+  grk_cparameters* compressor_parameters;
+  grk_image* image;
+  grk_plugin_tile* tile;
+  grk_stream_params stream_params;
+  unsigned int error_code;
+  bool transferExifTags;
+} grk_plugin_compress_user_callback_info;
+
+typedef uint64_t (*GRK_PLUGIN_COMPRESS_USER_CALLBACK)(grk_plugin_compress_user_callback_info* info);
+
+typedef struct grk_plugin_compress_batch_info
+{
+  const char* input_dir;
+  const char* output_dir;
+  grk_cparameters* compress_parameters;
+  GRK_PLUGIN_COMPRESS_USER_CALLBACK callback;
+} grk_plugin_compress_batch_info;
+
+/**
+ * Compress with plugin
+ *
+ * @param compress_parameters 	compress parameters
+ * @param callback				callback
+ */
+GRK_API int32_t GRK_CALLCONV grk_plugin_compress(grk_cparameters* compress_parameters,
+                                                 GRK_PLUGIN_COMPRESS_USER_CALLBACK callback);
+
+/**
+ * Batch compress with plugin
+ *
+ * @param input_dir				directory holding input images
+ * @param output_dir			directory holding compressed output images
+ * @param compress_parameters 	compress parameters
+ * @param callback				callback
+ *
+ * @return 0 if successful
+ *
+ */
+GRK_API int32_t GRK_CALLCONV grk_plugin_batch_compress(grk_plugin_compress_batch_info info);
+
+/**
+ * Wait for batch job to complete
+ */
+GRK_API void GRK_CALLCONV grk_plugin_wait_for_batch_complete(void);
+
+/**
+ * Stop batch compress
+ */
+GRK_API void GRK_CALLCONV grk_plugin_stop_batch_compress(void);
+
+/*
+ Plugin decompression
+ */
+
+typedef int (*GROK_INIT_DECOMPRESSORS)(grk_header_info* header_info, grk_image* image);
+
+typedef struct _grk_plugin_decompress_callback_info
+{
+  size_t deviceId;
+  GROK_INIT_DECOMPRESSORS init_decompressors_func;
+  const char* input_file_name;
+  const char* output_file_name;
+  /* input file format 0: J2K, 1: JP2 */
+  GRK_CODEC_FORMAT decod_format;
+  /* output file format 0: PGX, 1: PxM, 2: BMP etc */
+  GRK_SUPPORTED_FILE_FMT cod_format;
+  grk_codec* codec;
+  grk_header_info header_info;
+  grk_decompress_parameters* decompressor_parameters;
+  grk_image* image;
+  bool plugin_owns_image;
+  grk_plugin_tile* tile;
+  unsigned int error_code;
+  uint32_t decompress_flags;
+  uint32_t full_image_x0;
+  uint32_t full_image_y0;
+  void* user_data;
+} grk_plugin_decompress_callback_info;
+
+typedef int32_t (*grk_plugin_decompress_callback)(grk_plugin_decompress_callback_info* info);
+
+/**
+ * Decompress with plugin
+ *
+ * @param decompress_parameters  decompress parameters
+ * @param callback  			 callback
+ */
+GRK_API int32_t GRK_CALLCONV grk_plugin_decompress(grk_decompress_parameters* decompress_parameters,
+                                                   grk_plugin_decompress_callback callback);
+
+/**
+ * Initialize batch decompress
+ *
+ * @param input_dir input directory holding compressed images
+ * @param output_dir output directory holding decompressed images
+ * @param decompress_parameters  decompress parameters
+ * @param callback  			 callback
+ *
+ * @return 0 if successful
+ */
+GRK_API int32_t GRK_CALLCONV grk_plugin_init_batch_decompress(
+    const char* input_dir, const char* output_dir, grk_decompress_parameters* decompress_parameters,
+    grk_plugin_decompress_callback callback);
+
+/**
+ * Initiate batch decompress
+ */
+GRK_API int32_t GRK_CALLCONV grk_plugin_batch_decompress(void);
+
+/**
+ * Stop batch decompress
+ */
+GRK_API void GRK_CALLCONV grk_plugin_stop_batch_decompress(void);
+
+#ifdef __cplusplus
+}
+#endif
```

## Comparing `blosc2_grok-0.3.2.dist-info/METADATA` & `blosc2_grok-0.3.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blosc2_grok
-Version: 0.3.2
+Version: 0.3.3
 Summary: Grok (JPEG2000 codec) plugin for Blosc2.
 Keywords: plugin blosc2
 Author-Email: Blosc Development Team <contact@blosc.org>
 License: GNU Affero General Public License version 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
```

## Comparing `blosc2_grok-0.3.2.dist-info/licenses/LICENSE.txt` & `blosc2_grok-0.3.3.dist-info/licenses/LICENSE.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,666 +1,666 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
- For Blosc - A blocking, shuffling and lossless compression library
-
- Copyright (c) 2023-present, The Blosc Development Team <blosc@blosc.org>
- All rights reserved.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+ For Blosc - A blocking, shuffling and lossless compression library
+
+ Copyright (c) 2023-present, The Blosc Development Team <blosc@blosc.org>
+ All rights reserved.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

