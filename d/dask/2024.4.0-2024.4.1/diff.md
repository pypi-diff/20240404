# Comparing `tmp/dask-2024.4.0.tar.gz` & `tmp/dask-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-2024.4.0.tar", last modified: Mon Apr  1 19:39:46 2024, max compression
+gzip compressed data, was "dask-2024.4.1.tar", last modified: Thu Apr  4 16:12:05 2024, max compression
```

## Comparing `dask-2024.4.0.tar` & `dask-2024.4.1.tar`

### file list

```diff
@@ -1,500 +1,500 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.999805 dask-2024.4.0/
--rw-r--r--   0 james      (501) staff       (20)     1531 2023-07-17 19:15:27.000000 dask-2024.4.0/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      325 2023-07-17 19:15:27.000000 dask-2024.4.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     3780 2024-04-01 19:39:45.999572 dask-2024.4.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1291 2023-07-17 19:15:27.000000 dask-2024.4.0/README.rst
--rw-r--r--   0 james      (501) staff       (20)     1598 2024-01-23 19:42:07.000000 dask-2024.4.0/conftest.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.874534 dask-2024.4.0/dask/
--rw-r--r--   0 james      (501) staff       (20)      485 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      133 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/__main__.py
--rw-r--r--   0 james      (501) staff       (20)      720 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/_compatibility.py
--rw-r--r--   0 james      (501) staff       (20)      500 2024-04-01 19:39:45.999999 dask-2024.4.0/dask/_version.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.885751 dask-2024.4.0/dask/array/
--rw-r--r--   0 james      (501) staff       (20)     1543 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/array/NUMPY_LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)     5413 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12600 2023-12-20 15:38:57.000000 dask-2024.4.0/dask/array/backends.py
--rw-r--r--   0 james      (501) staff       (20)     9983 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/blockwise.py
--rw-r--r--   0 james      (501) staff       (20)    12304 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/chunk.py
--rw-r--r--   0 james      (501) staff       (20)     5066 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/chunk_types.py
--rw-r--r--   0 james      (501) staff       (20)   191264 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/core.py
--rw-r--r--   0 james      (501) staff       (20)    40514 2023-10-25 14:44:16.000000 dask-2024.4.0/dask/array/creation.py
--rw-r--r--   0 james      (501) staff       (20)     2114 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/cupy_entry_point.py
--rw-r--r--   0 james      (501) staff       (20)      526 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     9146 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/einsumfuncs.py
--rw-r--r--   0 james      (501) staff       (20)     7677 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/fft.py
--rw-r--r--   0 james      (501) staff       (20)    32656 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/gufunc.py
--rw-r--r--   0 james      (501) staff       (20)     1996 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/image.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.886204 dask-2024.4.0/dask/array/lib/
--rw-r--r--   0 james      (501) staff       (20)       77 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/lib/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      101 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/lib/stride_tricks.py
--rw-r--r--   0 james      (501) staff       (20)    53218 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/array/linalg.py
--rw-r--r--   0 james      (501) staff       (20)     6363 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/ma.py
--rw-r--r--   0 james      (501) staff       (20)     6078 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/numpy_compat.py
--rw-r--r--   0 james      (501) staff       (20)    12838 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/optimization.py
--rw-r--r--   0 james      (501) staff       (20)    28479 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/overlap.py
--rw-r--r--   0 james      (501) staff       (20)    10916 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/percentile.py
--rw-r--r--   0 james      (501) staff       (20)    40605 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/random.py
--rw-r--r--   0 james      (501) staff       (20)    28323 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    58469 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/reductions.py
--rw-r--r--   0 james      (501) staff       (20)    10766 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/reshape.py
--rw-r--r--   0 james      (501) staff       (20)    81576 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/routines.py
--rw-r--r--   0 james      (501) staff       (20)    72865 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/slicing.py
--rw-r--r--   0 james      (501) staff       (20)    16184 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/array/stats.py
--rw-r--r--   0 james      (501) staff       (20)     8048 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/svg.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.896863 dask-2024.4.0/dask/array/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/array/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)   162686 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/tests/test_array_core.py
--rw-r--r--   0 james      (501) staff       (20)     6689 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_array_function.py
--rw-r--r--   0 james      (501) staff       (20)     3159 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_array_utils.py
--rw-r--r--   0 james      (501) staff       (20)    23222 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_atop.py
--rw-r--r--   0 james      (501) staff       (20)     3304 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_chunk.py
--rw-r--r--   0 james      (501) staff       (20)    31190 2023-10-25 14:44:16.000000 dask-2024.4.0/dask/array/tests/test_creation.py
--rw-r--r--   0 james      (501) staff       (20)    19888 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_core.py
--rw-r--r--   0 james      (501) staff       (20)     6496 2023-10-25 14:44:16.000000 dask-2024.4.0/dask/array/tests/test_cupy_creation.py
--rw-r--r--   0 james      (501) staff       (20)      594 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_gufunc.py
--rw-r--r--   0 james      (501) staff       (20)    13412 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_linalg.py
--rw-r--r--   0 james      (501) staff       (20)     4303 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_overlap.py
--rw-r--r--   0 james      (501) staff       (20)     2730 2024-03-13 20:06:30.000000 dask-2024.4.0/dask/array/tests/test_cupy_percentile.py
--rw-r--r--   0 james      (501) staff       (20)     9219 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_random.py
--rw-r--r--   0 james      (501) staff       (20)     2224 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_reductions.py
--rw-r--r--   0 james      (501) staff       (20)     7436 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/tests/test_cupy_routines.py
--rw-r--r--   0 james      (501) staff       (20)     4877 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_slicing.py
--rw-r--r--   0 james      (501) staff       (20)     2982 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_cupy_sparse.py
--rw-r--r--   0 james      (501) staff       (20)     8866 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/tests/test_dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     8821 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/tests/test_fft.py
--rw-r--r--   0 james      (501) staff       (20)    21013 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_gufunc.py
--rw-r--r--   0 james      (501) staff       (20)     1482 2023-09-28 22:08:27.000000 dask-2024.4.0/dask/array/tests/test_image.py
--rw-r--r--   0 james      (501) staff       (20)    37415 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/tests/test_linalg.py
--rw-r--r--   0 james      (501) staff       (20)    15714 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/tests/test_masked.py
--rw-r--r--   0 james      (501) staff       (20)     1087 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_numpy_compat.py
--rw-r--r--   0 james      (501) staff       (20)    17446 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_optimization.py
--rw-r--r--   0 james      (501) staff       (20)    26718 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_overlap.py
--rw-r--r--   0 james      (501) staff       (20)     3443 2023-11-07 18:15:20.000000 dask-2024.4.0/dask/array/tests/test_percentiles.py
--rw-r--r--   0 james      (501) staff       (20)    15352 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/tests/test_random.py
--rw-r--r--   0 james      (501) staff       (20)    36262 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/array/tests/test_rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    33283 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/array/tests/test_reductions.py
--rw-r--r--   0 james      (501) staff       (20)     7289 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_reshape.py
--rw-r--r--   0 james      (501) staff       (20)    84472 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/array/tests/test_routines.py
--rw-r--r--   0 james      (501) staff       (20)    32264 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/array/tests/test_slicing.py
--rw-r--r--   0 james      (501) staff       (20)     6592 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_sparse.py
--rw-r--r--   0 james      (501) staff       (20)     5489 2023-09-28 22:08:27.000000 dask-2024.4.0/dask/array/tests/test_stats.py
--rw-r--r--   0 james      (501) staff       (20)     2740 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_svg.py
--rw-r--r--   0 james      (501) staff       (20)      525 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_testing.py
--rw-r--r--   0 james      (501) staff       (20)    17390 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_ufunc.py
--rw-r--r--   0 james      (501) staff       (20)     2706 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_wrap.py
--rw-r--r--   0 james      (501) staff       (20)     1317 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tests/test_xarray.py
--rw-r--r--   0 james      (501) staff       (20)     4737 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/tiledb_io.py
--rw-r--r--   0 james      (501) staff       (20)    10030 2024-03-13 20:06:30.000000 dask-2024.4.0/dask/array/ufunc.py
--rw-r--r--   0 james      (501) staff       (20)    19112 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/array/utils.py
--rw-r--r--   0 james      (501) staff       (20)     6906 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/array/wrap.py
--rw-r--r--   0 james      (501) staff       (20)     5122 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/backends.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.898194 dask-2024.4.0/dask/bag/
--rw-r--r--   0 james      (501) staff       (20)      903 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     9111 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/avro.py
--rw-r--r--   0 james      (501) staff       (20)      763 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/chunk.py
--rw-r--r--   0 james      (501) staff       (20)    86002 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/bag/core.py
--rw-r--r--   0 james      (501) staff       (20)     5464 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/random.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.899021 dask-2024.4.0/dask/bag/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/bag/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3808 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/tests/test_avro.py
--rw-r--r--   0 james      (501) staff       (20)    51280 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/bag/tests/test_bag.py
--rw-r--r--   0 james      (501) staff       (20)     6528 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/tests/test_random.py
--rw-r--r--   0 james      (501) staff       (20)     5049 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/tests/test_text.py
--rw-r--r--   0 james      (501) staff       (20)     6765 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/text.py
--rw-r--r--   0 james      (501) staff       (20)      241 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bag/utils.py
--rw-r--r--   0 james      (501) staff       (20)    54892 2024-04-01 19:10:34.000000 dask-2024.4.0/dask/base.py
--rw-r--r--   0 james      (501) staff       (20)    53276 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/blockwise.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.899487 dask-2024.4.0/dask/bytes/
--rw-r--r--   0 james      (501) staff       (20)       75 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bytes/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6933 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bytes/core.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.900461 dask-2024.4.0/dask/bytes/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/bytes/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5158 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bytes/tests/test_bytes_utils.py
--rw-r--r--   0 james      (501) staff       (20)      530 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bytes/tests/test_compression.py
--rw-r--r--   0 james      (501) staff       (20)     6815 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/bytes/tests/test_http.py
--rw-r--r--   0 james      (501) staff       (20)    11476 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bytes/tests/test_local.py
--rw-r--r--   0 james      (501) staff       (20)    19556 2024-01-29 17:27:45.000000 dask-2024.4.0/dask/bytes/tests/test_s3.py
--rw-r--r--   0 james      (501) staff       (20)      500 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/bytes/utils.py
--rw-r--r--   0 james      (501) staff       (20)     2001 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/cache.py
--rw-r--r--   0 james      (501) staff       (20)     4067 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/callbacks.py
--rw-r--r--   0 james      (501) staff       (20)     5773 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/cli.py
--rw-r--r--   0 james      (501) staff       (20)      523 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/compatibility.py
--rw-r--r--   0 james      (501) staff       (20)    24786 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/config.py
--rw-r--r--   0 james      (501) staff       (20)      959 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/conftest.py
--rw-r--r--   0 james      (501) staff       (20)     1756 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/context.py
--rw-r--r--   0 james      (501) staff       (20)    15772 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/core.py
--rw-r--r--   0 james      (501) staff       (20)     7854 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dask-schema.yaml
--rw-r--r--   0 james      (501) staff       (20)     1955 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dask.yaml
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.908230 dask-2024.4.0/dask/dataframe/
--rw-r--r--   0 james      (501) staff       (20)     5405 2024-04-01 19:10:34.000000 dask-2024.4.0/dask/dataframe/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7642 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/_compat.py
--rw-r--r--   0 james      (501) staff       (20)     2171 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/dataframe/_dtypes.py
--rw-r--r--   0 james      (501) staff       (20)     3974 2024-02-06 16:03:46.000000 dask-2024.4.0/dask/dataframe/_pyarrow.py
--rw-r--r--   0 james      (501) staff       (20)     2743 2023-11-10 20:46:15.000000 dask-2024.4.0/dask/dataframe/_pyarrow_compat.py
--rw-r--r--   0 james      (501) staff       (20)      393 2024-01-25 18:24:19.000000 dask-2024.4.0/dask/dataframe/_testing.py
--rw-r--r--   0 james      (501) staff       (20)    13122 2024-02-01 17:01:41.000000 dask-2024.4.0/dask/dataframe/accessor.py
--rw-r--r--   0 james      (501) staff       (20)    25843 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/backends.py
--rw-r--r--   0 james      (501) staff       (20)     9507 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/categorical.py
--rw-r--r--   0 james      (501) staff       (20)   314038 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/core.py
--rw-r--r--   0 james      (501) staff       (20)     4577 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/dispatch.py
--rw-r--r--   0 james      (501) staff       (20)      552 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/extensions.py
--rw-r--r--   0 james      (501) staff       (20)   117451 2024-04-01 19:10:34.000000 dask-2024.4.0/dask/dataframe/groupby.py
--rw-r--r--   0 james      (501) staff       (20)     2463 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/hyperloglog.py
--rw-r--r--   0 james      (501) staff       (20)    13412 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/indexing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.912429 dask-2024.4.0/dask/dataframe/io/
--rw-r--r--   0 james      (501) staff       (20)      706 2023-09-25 17:06:23.000000 dask-2024.4.0/dask/dataframe/io/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    34437 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/csv.py
--rw-r--r--   0 james      (501) staff       (20)    18830 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/demo.py
--rw-r--r--   0 james      (501) staff       (20)    18384 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/io/hdf.py
--rw-r--r--   0 james      (501) staff       (20)    38600 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/io.py
--rw-r--r--   0 james      (501) staff       (20)    11163 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/dataframe/io/json.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.913719 dask-2024.4.0/dask/dataframe/io/orc/
--rw-r--r--   0 james      (501) staff       (20)       92 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/io/orc/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     4487 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/io/orc/arrow.py
--rw-r--r--   0 james      (501) staff       (20)     7183 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/io/orc/core.py
--rw-r--r--   0 james      (501) staff       (20)      510 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/io/orc/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.915576 dask-2024.4.0/dask/dataframe/io/parquet/
--rw-r--r--   0 james      (501) staff       (20)      166 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/io/parquet/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    72803 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/parquet/arrow.py
--rw-r--r--   0 james      (501) staff       (20)    67054 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/parquet/core.py
--rw-r--r--   0 james      (501) staff       (20)    52314 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/parquet/fastparquet.py
--rw-r--r--   0 james      (501) staff       (20)    32900 2023-10-27 21:32:35.000000 dask-2024.4.0/dask/dataframe/io/parquet/utils.py
--rw-r--r--   0 james      (501) staff       (20)    21270 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/sql.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.918198 dask-2024.4.0/dask/dataframe/io/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/dataframe/io/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    61918 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/tests/test_csv.py
--rw-r--r--   0 james      (501) staff       (20)    11436 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/tests/test_demo.py
--rw-r--r--   0 james      (501) staff       (20)    27324 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/io/tests/test_hdf.py
--rw-r--r--   0 james      (501) staff       (20)    35589 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/tests/test_io.py
--rw-r--r--   0 james      (501) staff       (20)     8812 2023-09-21 15:09:09.000000 dask-2024.4.0/dask/dataframe/io/tests/test_json.py
--rw-r--r--   0 james      (501) staff       (20)     5302 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/io/tests/test_orc.py
--rw-r--r--   0 james      (501) staff       (20)   166161 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/io/tests/test_parquet.py
--rw-r--r--   0 james      (501) staff       (20)    17632 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/io/tests/test_sql.py
--rw-r--r--   0 james      (501) staff       (20)     8041 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/dataframe/io/utils.py
--rw-r--r--   0 james      (501) staff       (20)    14713 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/dataframe/methods.py
--rw-r--r--   0 james      (501) staff       (20)    55455 2024-02-09 22:36:17.000000 dask-2024.4.0/dask/dataframe/multi.py
--rw-r--r--   0 james      (501) staff       (20)     1600 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/numeric.py
--rw-r--r--   0 james      (501) staff       (20)     8780 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/optimize.py
--rw-r--r--   0 james      (501) staff       (20)    20819 2023-10-25 14:44:16.000000 dask-2024.4.0/dask/dataframe/partitionquantiles.py
--rw-r--r--   0 james      (501) staff       (20)    11868 2023-10-27 21:32:31.000000 dask-2024.4.0/dask/dataframe/reshape.py
--rw-r--r--   0 james      (501) staff       (20)    22170 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/rolling.py
--rw-r--r--   0 james      (501) staff       (20)    40190 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/shuffle.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.926099 dask-2024.4.0/dask/dataframe/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/dataframe/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    11131 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_accessors.py
--rw-r--r--   0 james      (501) staff       (20)    70713 2024-01-30 19:27:46.000000 dask-2024.4.0/dask/dataframe/tests/test_arithmetics_reduction.py
--rw-r--r--   0 james      (501) staff       (20)      942 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/tests/test_boolean.py
--rw-r--r--   0 james      (501) staff       (20)    17863 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_categorical.py
--rw-r--r--   0 james      (501) staff       (20)   209289 2024-04-01 19:10:34.000000 dask-2024.4.0/dask/dataframe/tests/test_dataframe.py
--rw-r--r--   0 james      (501) staff       (20)     1457 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_extensions.py
--rw-r--r--   0 james      (501) staff       (20)    14847 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/tests/test_format.py
--rw-r--r--   0 james      (501) staff       (20)   127604 2024-04-01 19:10:34.000000 dask-2024.4.0/dask/dataframe/tests/test_groupby.py
--rw-r--r--   0 james      (501) staff       (20)     2702 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dataframe/tests/test_hashing.py
--rw-r--r--   0 james      (501) staff       (20)     2897 2024-01-30 19:27:46.000000 dask-2024.4.0/dask/dataframe/tests/test_hyperloglog.py
--rw-r--r--   0 james      (501) staff       (20)    23962 2024-02-06 16:03:46.000000 dask-2024.4.0/dask/dataframe/tests/test_indexing.py
--rw-r--r--   0 james      (501) staff       (20)     7990 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/tests/test_merge_column_and_index.py
--rw-r--r--   0 james      (501) staff       (20)      463 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/dataframe/tests/test_methods.py
--rw-r--r--   0 james      (501) staff       (20)    96566 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_multi.py
--rw-r--r--   0 james      (501) staff       (20)     2624 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_numeric.py
--rw-r--r--   0 james      (501) staff       (20)     1188 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/tests/test_optimize_dataframe.py
--rw-r--r--   0 james      (501) staff       (20)     6662 2023-09-25 17:06:24.000000 dask-2024.4.0/dask/dataframe/tests/test_pyarrow.py
--rw-r--r--   0 james      (501) staff       (20)     5059 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_pyarrow_compat.py
--rw-r--r--   0 james      (501) staff       (20)    11551 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/dataframe/tests/test_reshape.py
--rw-r--r--   0 james      (501) staff       (20)    18504 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_rolling.py
--rw-r--r--   0 james      (501) staff       (20)    63506 2024-01-30 19:27:46.000000 dask-2024.4.0/dask/dataframe/tests/test_shuffle.py
--rw-r--r--   0 james      (501) staff       (20)    16922 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/dataframe/tests/test_ufunc.py
--rw-r--r--   0 james      (501) staff       (20)    22240 2024-04-01 19:10:34.000000 dask-2024.4.0/dask/dataframe/tests/test_utils_dataframe.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.926553 dask-2024.4.0/dask/dataframe/tseries/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/dataframe/tseries/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7675 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/dataframe/tseries/resample.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.926873 dask-2024.4.0/dask/dataframe/tseries/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/dataframe/tseries/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7028 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/dataframe/tseries/tests/test_resample.py
--rw-r--r--   0 james      (501) staff       (20)    27538 2023-09-25 17:06:24.000000 dask-2024.4.0/dask/dataframe/utils.py
--rw-r--r--   0 james      (501) staff       (20)     5331 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/datasets.py
--rw-r--r--   0 james      (501) staff       (20)    24814 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/delayed.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.927801 dask-2024.4.0/dask/diagnostics/
--rw-r--r--   0 james      (501) staff       (20)      258 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/diagnostics/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12136 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/diagnostics/profile.py
--rw-r--r--   0 james      (501) staff       (20)    16332 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/diagnostics/profile_visualize.py
--rw-r--r--   0 james      (501) staff       (20)     5001 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/diagnostics/progress.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.928271 dask-2024.4.0/dask/diagnostics/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/diagnostics/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12045 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/diagnostics/tests/test_profiler.py
--rw-r--r--   0 james      (501) staff       (20)     3388 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/diagnostics/tests/test_progress.py
--rw-r--r--   0 james      (501) staff       (20)      715 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/distributed.py
--rw-r--r--   0 james      (501) staff       (20)    16587 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/dot.py
--rw-r--r--   0 james      (501) staff       (20)    19622 2023-10-25 14:44:16.000000 dask-2024.4.0/dask/graph_manipulation.py
--rw-r--r--   0 james      (501) staff       (20)     2492 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/hashing.py
--rw-r--r--   0 james      (501) staff       (20)    35516 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/highlevelgraph.py
--rw-r--r--   0 james      (501) staff       (20)    46004 2023-09-13 17:55:33.000000 dask-2024.4.0/dask/layers.py
--rw-r--r--   0 james      (501) staff       (20)    18896 2023-09-13 17:55:33.000000 dask-2024.4.0/dask/local.py
--rw-r--r--   0 james      (501) staff       (20)      487 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/ml.py
--rw-r--r--   0 james      (501) staff       (20)     8474 2023-09-13 17:55:33.000000 dask-2024.4.0/dask/multiprocessing.py
--rw-r--r--   0 james      (501) staff       (20)    36224 2024-02-09 15:39:56.000000 dask-2024.4.0/dask/optimization.py
--rw-r--r--   0 james      (501) staff       (20)    32839 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/order.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/py.typed
--rw-r--r--   0 james      (501) staff       (20)    12597 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/rewrite.py
--rw-r--r--   0 james      (501) staff       (20)     7621 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/sizeof.py
--rw-r--r--   0 james      (501) staff       (20)     2089 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/system.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.936095 dask-2024.4.0/dask/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.0/dask/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      824 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/tests/test_backends.py
--rw-r--r--   0 james      (501) staff       (20)    33013 2024-02-09 15:39:56.000000 dask-2024.4.0/dask/tests/test_base.py
--rw-r--r--   0 james      (501) staff       (20)     1613 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_cache.py
--rw-r--r--   0 james      (501) staff       (20)     2570 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_callbacks.py
--rw-r--r--   0 james      (501) staff       (20)     1224 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_ci.py
--rw-r--r--   0 james      (501) staff       (20)     7488 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_cli.py
--rw-r--r--   0 james      (501) staff       (20)      379 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_compatibility.py
--rw-r--r--   0 james      (501) staff       (20)    20268 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_config.py
--rw-r--r--   0 james      (501) staff       (20)     1137 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_context.py
--rw-r--r--   0 james      (501) staff       (20)     8203 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/tests/test_core.py
--rw-r--r--   0 james      (501) staff       (20)     1112 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_datasets.py
--rw-r--r--   0 james      (501) staff       (20)    22962 2024-02-09 15:39:56.000000 dask-2024.4.0/dask/tests/test_delayed.py
--rw-r--r--   0 james      (501) staff       (20)    33448 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_distributed.py
--rw-r--r--   0 james      (501) staff       (20)      719 2024-03-13 20:06:30.000000 dask-2024.4.0/dask/tests/test_docs.py
--rw-r--r--   0 james      (501) staff       (20)    12271 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_dot.py
--rw-r--r--   0 james      (501) staff       (20)    15338 2024-01-29 17:27:45.000000 dask-2024.4.0/dask/tests/test_graph_manipulation.py
--rw-r--r--   0 james      (501) staff       (20)     1095 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_hashing.py
--rw-r--r--   0 james      (501) staff       (20)     9231 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_highgraph.py
--rw-r--r--   0 james      (501) staff       (20)     9040 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_layers.py
--rw-r--r--   0 james      (501) staff       (20)     5022 2023-12-13 17:43:46.000000 dask-2024.4.0/dask/tests/test_local.py
--rw-r--r--   0 james      (501) staff       (20)      419 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_ml.py
--rw-r--r--   0 james      (501) staff       (20)     8457 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_multiprocessing.py
--rw-r--r--   0 james      (501) staff       (20)    47821 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_optimization.py
--rw-r--r--   0 james      (501) staff       (20)    69758 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_order.py
--rw-r--r--   0 james      (501) staff       (20)     4684 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_rewrite.py
--rw-r--r--   0 james      (501) staff       (20)     7526 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/tests/test_sizeof.py
--rw-r--r--   0 james      (501) staff       (20)     7228 2024-01-23 19:42:03.000000 dask-2024.4.0/dask/tests/test_spark_compat.py
--rw-r--r--   0 james      (501) staff       (20)     2571 2023-08-21 21:39:12.000000 dask-2024.4.0/dask/tests/test_system.py
--rw-r--r--   0 james      (501) staff       (20)     4749 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_threaded.py
--rw-r--r--   0 james      (501) staff       (20)    39981 2024-03-13 20:06:30.000000 dask-2024.4.0/dask/tests/test_tokenize.py
--rw-r--r--   0 james      (501) staff       (20)     4591 2023-09-15 13:43:23.000000 dask-2024.4.0/dask/tests/test_traceback.py
--rw-r--r--   0 james      (501) staff       (20)     5708 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/tests/test_typing.py
--rw-r--r--   0 james      (501) staff       (20)    23636 2024-01-23 19:42:07.000000 dask-2024.4.0/dask/tests/test_utils.py
--rw-r--r--   0 james      (501) staff       (20)     1598 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/test_utils_test.py
--rw-r--r--   0 james      (501) staff       (20)      211 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/tests/warning_aliases.py
--rw-r--r--   0 james      (501) staff       (20)     3001 2023-09-13 17:55:33.000000 dask-2024.4.0/dask/threaded.py
--rw-r--r--   0 james      (501) staff       (20)    15497 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/typing.py
--rw-r--r--   0 james      (501) staff       (20)    63637 2024-03-13 20:06:34.000000 dask-2024.4.0/dask/utils.py
--rw-r--r--   0 james      (501) staff       (20)     4825 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/utils_test.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.936563 dask-2024.4.0/dask/widgets/
--rw-r--r--   0 james      (501) staff       (20)      792 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.937393 dask-2024.4.0/dask/widgets/templates/
--rw-r--r--   0 james      (501) staff       (20)     1295 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/templates/array.html.j2
--rw-r--r--   0 james      (501) staff       (20)      124 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/templates/dataframe.html.j2
--rw-r--r--   0 james      (501) staff       (20)     2579 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/templates/highlevelgraph.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1981 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/templates/highlevelgraph_layer.html.j2
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.937558 dask-2024.4.0/dask/widgets/tests/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.938027 dask-2024.4.0/dask/widgets/tests/templates/
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/tests/templates/bytes.html.j2
--rw-r--r--   0 james      (501) staff       (20)       39 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/tests/templates/custom_filter.html.j2
--rw-r--r--   0 james      (501) staff       (20)       30 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/tests/templates/example.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1401 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/tests/test_widgets.py
--rw-r--r--   0 james      (501) staff       (20)     1120 2023-07-17 19:15:27.000000 dask-2024.4.0/dask/widgets/widgets.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.998151 dask-2024.4.0/dask.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     3780 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)    14325 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      124 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      532 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        5 2024-04-01 19:39:45.000000 dask-2024.4.0/dask.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.938347 dask-2024.4.0/docs/
--rw-r--r--   0 james      (501) staff       (20)     5741 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/Makefile
--rw-r--r--   0 james      (501) staff       (20)     5186 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/make.bat
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.961276 dask-2024.4.0/docs/source/
--rw-r--r--   0 james      (501) staff       (20)    17900 2024-01-23 19:42:03.000000 dask-2024.4.0/docs/source/10-minutes-to-dask.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.963385 dask-2024.4.0/docs/source/_static/
--rw-r--r--   0 james      (501) staff       (20)    10187 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/config_converter.js
--rw-r--r--   0 james      (501) staff       (20)    11021 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/_static/dask-simple.png
--rw-r--r--   0 james      (501) staff       (20)     2375 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/main-page.css
--rw-r--r--   0 james      (501) staff       (20)    15598 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/profile.html
--rw-r--r--   0 james      (501) staff       (20)    65304 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/stacked_profile.html
--rw-r--r--   0 james      (501) staff       (20)      523 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/style.css
--rw-r--r--   0 james      (501) staff       (20)      365 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0 james      (501) staff       (20)   292662 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/transpose_cyto.html
--rw-r--r--   0 james      (501) staff       (20)    49423 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_static/yaml.min.js
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.963831 dask-2024.4.0/docs/source/_templates/
--rw-r--r--   0 james      (501) staff       (20)      180 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/_templates/layout.html
--rw-r--r--   0 james      (501) staff       (20)     4349 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/adaptive.rst
--rw-r--r--   0 james      (501) staff       (20)     3109 2023-08-21 21:39:12.000000 dask-2024.4.0/docs/source/api.rst
--rw-r--r--   0 james      (501) staff       (20)     7189 2023-08-21 21:39:12.000000 dask-2024.4.0/docs/source/array-api.rst
--rw-r--r--   0 james      (501) staff       (20)     2943 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-assignment.rst
--rw-r--r--   0 james      (501) staff       (20)     4740 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)    13262 2023-08-21 21:39:12.000000 dask-2024.4.0/docs/source/array-chunks.rst
--rw-r--r--   0 james      (501) staff       (20)    18437 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-creation.rst
--rw-r--r--   0 james      (501) staff       (20)     5885 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-design.rst
--rw-r--r--   0 james      (501) staff       (20)     2857 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-gufunc.rst
--rw-r--r--   0 james      (501) staff       (20)    21469 2023-08-21 21:39:12.000000 dask-2024.4.0/docs/source/array-numpy-compatibility.rst
--rw-r--r--   0 james      (501) staff       (20)     6069 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-overlap.rst
--rw-r--r--   0 james      (501) staff       (20)     3924 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-random.rst
--rw-r--r--   0 james      (501) staff       (20)     4137 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-slicing.rst
--rw-r--r--   0 james      (501) staff       (20)     3291 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-sparse.rst
--rw-r--r--   0 james      (501) staff       (20)     2018 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-stack.rst
--rw-r--r--   0 james      (501) staff       (20)     1140 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/array-stats.rst
--rw-r--r--   0 james      (501) staff       (20)     4154 2023-08-21 21:39:12.000000 dask-2024.4.0/docs/source/array.rst
--rw-r--r--   0 james      (501) staff       (20)     1574 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/bag-api.rst
--rw-r--r--   0 james      (501) staff       (20)     4557 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/bag-creation.rst
--rw-r--r--   0 james      (501) staff       (20)     4068 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/bag.rst
--rw-r--r--   0 james      (501) staff       (20)    14042 2024-01-23 19:42:03.000000 dask-2024.4.0/docs/source/best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     5553 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/caching.rst
--rw-r--r--   0 james      (501) staff       (20)   367491 2024-04-01 19:33:17.000000 dask-2024.4.0/docs/source/changelog.rst
--rw-r--r--   0 james      (501) staff       (20)      211 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/cheatsheet.rst
--rw-r--r--   0 james      (501) staff       (20)     4047 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/cli.rst
--rw-r--r--   0 james      (501) staff       (20)    15922 2024-03-13 20:06:34.000000 dask-2024.4.0/docs/source/conf.py
--rw-r--r--   0 james      (501) staff       (20)    16945 2024-03-13 20:06:30.000000 dask-2024.4.0/docs/source/configuration.rst
--rw-r--r--   0 james      (501) staff       (20)    18998 2024-03-13 20:06:30.000000 dask-2024.4.0/docs/source/custom-collections.rst
--rw-r--r--   0 james      (501) staff       (20)     3604 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/custom-graphs.rst
--rw-r--r--   0 james      (501) staff       (20)     4209 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/customize-initialization.rst
--rw-r--r--   0 james      (501) staff       (20)      932 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dashboard-progress-script.py
--rw-r--r--   0 james      (501) staff       (20)    15045 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dashboard.rst
--rw-r--r--   0 james      (501) staff       (20)   203552 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/daskcheatsheet.pdf
--rw-r--r--   0 james      (501) staff       (20)    10542 2024-03-13 20:06:34.000000 dask-2024.4.0/docs/source/dataframe-api.rst
--rw-r--r--   0 james      (501) staff       (20)     9611 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dataframe-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     3951 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dataframe-categoricals.rst
--rw-r--r--   0 james      (501) staff       (20)     5977 2023-12-15 20:02:17.000000 dask-2024.4.0/docs/source/dataframe-create.rst
--rw-r--r--   0 james      (501) staff       (20)     5014 2023-12-15 20:02:17.000000 dask-2024.4.0/docs/source/dataframe-design.rst
--rw-r--r--   0 james      (501) staff       (20)     6224 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dataframe-extend.rst
--rw-r--r--   0 james      (501) staff       (20)      423 2024-03-13 20:06:34.000000 dask-2024.4.0/docs/source/dataframe-extra.rst
--rw-r--r--   0 james      (501) staff       (20)     8032 2023-12-15 20:02:17.000000 dask-2024.4.0/docs/source/dataframe-groupby.rst
--rw-r--r--   0 james      (501) staff       (20)     9351 2024-01-23 19:42:03.000000 dask-2024.4.0/docs/source/dataframe-hive.rst
--rw-r--r--   0 james      (501) staff       (20)     6115 2023-10-25 14:44:16.000000 dask-2024.4.0/docs/source/dataframe-indexing.rst
--rw-r--r--   0 james      (501) staff       (20)     3454 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dataframe-joins.rst
--rw-r--r--   0 james      (501) staff       (20)    13645 2024-03-13 20:06:34.000000 dask-2024.4.0/docs/source/dataframe-legacy-api.rst
--rw-r--r--   0 james      (501) staff       (20)    10545 2024-01-23 19:42:03.000000 dask-2024.4.0/docs/source/dataframe-parquet.rst
--rw-r--r--   0 james      (501) staff       (20)    12661 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/dataframe-sql.rst
--rw-r--r--   0 james      (501) staff       (20)     6608 2024-02-06 16:49:58.000000 dask-2024.4.0/docs/source/dataframe.rst
--rw-r--r--   0 james      (501) staff       (20)      363 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/debugging-performance.rst
--rw-r--r--   0 james      (501) staff       (20)     1696 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/delayed-api.rst
--rw-r--r--   0 james      (501) staff       (20)    17616 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/delayed-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     1497 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/delayed-collections.rst
--rw-r--r--   0 james      (501) staff       (20)     6357 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/delayed.rst
--rw-r--r--   0 james      (501) staff       (20)     3620 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-cli.rst
--rw-r--r--   0 james      (501) staff       (20)     4797 2024-01-26 23:05:40.000000 dask-2024.4.0/docs/source/deploying-cloud.rst
--rw-r--r--   0 james      (501) staff       (20)     2868 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-docker.rst
--rw-r--r--   0 james      (501) staff       (20)      246 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/deploying-extra.rst
--rw-r--r--   0 james      (501) staff       (20)     9939 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-hpc.rst
--rw-r--r--   0 james      (501) staff       (20)     4001 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-kubernetes.rst
--rw-r--r--   0 james      (501) staff       (20)     5823 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-python-advanced.rst
--rw-r--r--   0 james      (501) staff       (20)     2839 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-python.rst
--rw-r--r--   0 james      (501) staff       (20)     1619 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/deploying-ssh.rst
--rw-r--r--   0 james      (501) staff       (20)     8213 2024-02-09 15:39:56.000000 dask-2024.4.0/docs/source/deploying.rst
--rw-r--r--   0 james      (501) staff       (20)    10868 2023-12-14 20:19:54.000000 dask-2024.4.0/docs/source/deployment-considerations.rst
--rw-r--r--   0 james      (501) staff       (20)    13137 2024-03-13 20:06:30.000000 dask-2024.4.0/docs/source/develop.rst
--rw-r--r--   0 james      (501) staff       (20)     4442 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/diagnostics-distributed.rst
--rw-r--r--   0 james      (501) staff       (20)    10407 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/diagnostics-local.rst
--rw-r--r--   0 james      (501) staff       (20)     4548 2024-04-01 19:10:34.000000 dask-2024.4.0/docs/source/ecosystem.rst
--rw-r--r--   0 james      (501) staff       (20)    18500 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/faq.rst
--rw-r--r--   0 james      (501) staff       (20)    25633 2024-02-01 17:01:41.000000 dask-2024.4.0/docs/source/futures.rst
--rw-r--r--   0 james      (501) staff       (20)     5820 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/gpu.rst
--rw-r--r--   0 james      (501) staff       (20)     2541 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/graph_manipulation.rst
--rw-r--r--   0 james      (501) staff       (20)     5433 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/graphs.rst
--rw-r--r--   0 james      (501) staff       (20)     5399 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/graphviz.rst
--rw-r--r--   0 james      (501) staff       (20)     6946 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/high-level-graphs.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.965016 dask-2024.4.0/docs/source/how-to/
--rw-r--r--   0 james      (501) staff       (20)    15531 2024-04-01 19:10:34.000000 dask-2024.4.0/docs/source/how-to/connect-to-remote-data.rst
--rw-r--r--   0 james      (501) staff       (20)    11477 2023-08-21 21:39:12.000000 dask-2024.4.0/docs/source/how-to/debug.rst
--rw-r--r--   0 james      (501) staff       (20)     1722 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/how-to/extend-sizeof.rst
--rw-r--r--   0 james      (501) staff       (20)      433 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/how-to/index.rst
--rw-r--r--   0 james      (501) staff       (20)     6680 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/how-to/selecting-the-collection-backend.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.997424 dask-2024.4.0/docs/source/images/
--rw-r--r--   0 james      (501) staff       (20)    99565 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/10_minutes_array_graph.png
--rw-r--r--   0 james      (501) staff       (20)    22442 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/10_minutes_bag_graph.png
--rw-r--r--   0 james      (501) staff       (20)    56229 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/10_minutes_dataframe_graph.png
--rw-r--r--   0 james      (501) staff       (20)     4059 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/HHMI_Janelia_Color.png
--rw-r--r--   0 james      (501) staff       (20)    18406 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/array.svg
--rw-r--r--   0 james      (501) staff       (20)  1620104 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/async-embarrassing.gif
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.997590 dask-2024.4.0/docs/source/images/changelog/
--rw-r--r--   0 james      (501) staff       (20)    19604 2023-12-01 15:52:50.000000 dask-2024.4.0/docs/source/images/changelog/2023110-rechunking-disk-perf.png
--rw-r--r--   0 james      (501) staff       (20)   540389 2024-01-26 23:05:40.000000 dask-2024.4.0/docs/source/images/cloud-provider-logos.svg
--rw-r--r--   0 james      (501) staff       (20)    10752 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/concurrent-futures-threaded.webp
--rw-r--r--   0 james      (501) staff       (20)   135129 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/crosstalk.svg
--rw-r--r--   0 james      (501) staff       (20)  2367087 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_jupyterlab.png
--rw-r--r--   0 james      (501) staff       (20)    37971 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_link.png
--rw-r--r--   0 james      (501) staff       (20)    68712 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_memory.png
--rw-r--r--   0 james      (501) staff       (20)   281018 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_memory_new.gif
--rw-r--r--   0 james      (501) staff       (20)    25435 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_progress.png
--rw-r--r--   0 james      (501) staff       (20)   276928 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_status.png
--rw-r--r--   0 james      (501) staff       (20)    12009 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_task_processing.png
--rw-r--r--   0 james      (501) staff       (20)    58238 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_task_stream_unhealthy.png
--rw-r--r--   0 james      (501) staff       (20)   103654 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dashboard_taskstream_healthy.png
--rw-r--r--   0 james      (501) staff       (20)   112822 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-adaptive.svg
--rw-r--r--   0 james      (501) staff       (20)    14645 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-array.svg
--rw-r--r--   0 james      (501) staff       (20)   222084 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-cluster-manager.svg
--rw-r--r--   0 james      (501) staff       (20)    18782 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-dataframe.svg
--rw-r--r--   0 james      (501) staff       (20)   381903 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-overview-distributed-callout.svg
--rw-r--r--   0 james      (501) staff       (20)   357643 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-overview-schedulers.svg
--rw-r--r--   0 james      (501) staff       (20)    97471 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask-overview.svg
--rw-r--r--   0 james      (501) staff       (20)     3022 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_horizontal.svg
--rw-r--r--   0 james      (501) staff       (20)     3651 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_horizontal_black.svg
--rw-r--r--   0 james      (501) staff       (20)     3767 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_horizontal_on_blue.svg
--rw-r--r--   0 james      (501) staff       (20)     3738 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_horizontal_on_pink.svg
--rw-r--r--   0 james      (501) staff       (20)     3738 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_horizontal_white.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_icon.svg
--rw-r--r--   0 james      (501) staff       (20)     1571 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_icon_black.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_icon_on_pink.svg
--rw-r--r--   0 james      (501) staff       (20)     1609 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/dask_icon_white.svg
--rw-r--r--   0 james      (501) staff       (20)    20216 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/delayed-inc-double-add.svg
--rw-r--r--   0 james      (501) staff       (20)   104628 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/distributed-overview.svg
--rw-r--r--   0 james      (501) staff       (20)    18297 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/frame-shuffle.svg
--rw-r--r--   0 james      (501) staff       (20)    22979 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/frame-sort.svg
--rw-r--r--   0 james      (501) staff       (20)    12181 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/frame.svg
--rw-r--r--   0 james      (501) staff       (20)   391443 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/images/futures-graph.png
--rw-r--r--   0 james      (501) staff       (20)    41828 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/gputester-msg.png
--rw-r--r--   0 james      (501) staff       (20)   210392 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/growth_of_languages.png
--rw-r--r--   0 james      (501) staff       (20)   167834 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/growth_of_libraries.png
--rw-r--r--   0 james      (501) staff       (20)     4097 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/inc-add.svg
--rw-r--r--   0 james      (501) staff       (20)   123010 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/map-reduce-task-scheduling.svg
--rw-r--r--   0 james      (501) staff       (20)   482302 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/map_blocks_drop_axis.png
--rw-r--r--   0 james      (501) staff       (20)   113067 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/merge_chunks.png
--rw-r--r--   0 james      (501) staff       (20)    63244 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/merge_chunks_false.png
--rw-r--r--   0 james      (501) staff       (20)    13024 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/optimize_dask1.svg
--rw-r--r--   0 james      (501) staff       (20)     8803 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/optimize_dask2.svg
--rw-r--r--   0 james      (501) staff       (20)     5198 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/optimize_dask3.svg
--rw-r--r--   0 james      (501) staff       (20)     4104 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/optimize_dask4.svg
--rw-r--r--   0 james      (501) staff       (20)     2738 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/optimize_dask5.svg
--rw-r--r--   0 james      (501) staff       (20)   292827 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/order-failure.png
--rw-r--r--   0 james      (501) staff       (20)   239828 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/order-success.png
--rw-r--r--   0 james      (501) staff       (20)    40833 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/overlap.svg
--rw-r--r--   0 james      (501) staff       (20)    18785 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/overlapping-blocks.svg
--rw-r--r--   0 james      (501) staff       (20)     4537 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/overlapping-neighbors.svg
--rw-r--r--   0 james      (501) staff       (20)    20533 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/pipeline.svg
--rw-r--r--   0 james      (501) staff       (20)    31576 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/reshape.png
--rw-r--r--   0 james      (501) staff       (20)    31410 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/reshape_problem.png
--rw-r--r--   0 james      (501) staff       (20)    33288 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/reshape_rechunked.png
--rw-r--r--   0 james      (501) staff       (20)    50209 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/scaling-edges.png
--rw-r--r--   0 james      (501) staff       (20)    68476 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/scaling-nodes.png
--rw-r--r--   0 james      (501) staff       (20)    21294 2023-07-17 19:15:13.000000 dask-2024.4.0/docs/source/images/simple-dask.png
--rw-r--r--   0 james      (501) staff       (20)    27572 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/transpose-hlg-hovertooltip.png
--rw-r--r--   0 james      (501) staff       (20)    84492 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/transpose-hlg-html-repr.png
--rw-r--r--   0 james      (501) staff       (20)    39365 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/transpose.svg
--rw-r--r--   0 james      (501) staff       (20)    22446 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/transpose_opt.svg
--rw-r--r--   0 james      (501) staff       (20)   115022 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/trivial.svg
--rw-r--r--   0 james      (501) staff       (20)     2451 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/images/unoverlapping-neighbors.svg
--rw-r--r--   0 james      (501) staff       (20)    12486 2024-02-09 15:39:56.000000 dask-2024.4.0/docs/source/index.rst
--rw-r--r--   0 james      (501) staff       (20)    15500 2024-03-13 20:06:34.000000 dask-2024.4.0/docs/source/install.rst
--rw-r--r--   0 james      (501) staff       (20)      341 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/internals.rst
--rw-r--r--   0 james      (501) staff       (20)      868 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/logos.rst
--rw-r--r--   0 james      (501) staff       (20)     3573 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/maintainers.rst
--rw-r--r--   0 james      (501) staff       (20)    12200 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/optimize.rst
--rw-r--r--   0 james      (501) staff       (20)     7119 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/order.rst
--rw-r--r--   0 james      (501) staff       (20)     4810 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/phases-of-computation.rst
--rw-r--r--   0 james      (501) staff       (20)      857 2023-12-07 19:39:17.000000 dask-2024.4.0/docs/source/presentations.rst
--rw-r--r--   0 james      (501) staff       (20)      868 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/prometheus.rst
--rw-r--r--   0 james      (501) staff       (20)     6010 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/scheduler-overview.rst
--rw-r--r--   0 james      (501) staff       (20)     4493 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/scheduling-policy.rst
--rw-r--r--   0 james      (501) staff       (20)    11015 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/scheduling.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:39:45.997941 dask-2024.4.0/docs/source/scripts/
--rw-r--r--   0 james      (501) staff       (20)     3294 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/scripts/scheduling.py
--rw-r--r--   0 james      (501) staff       (20)     6104 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/shared.rst
--rw-r--r--   0 james      (501) staff       (20)     4562 2023-12-13 17:43:46.000000 dask-2024.4.0/docs/source/software-environments.rst
--rw-r--r--   0 james      (501) staff       (20)     9342 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/spark.rst
--rw-r--r--   0 james      (501) staff       (20)     3967 2023-09-13 17:55:33.000000 dask-2024.4.0/docs/source/spec.rst
--rw-r--r--   0 james      (501) staff       (20)     4754 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/support.rst
--rw-r--r--   0 james      (501) staff       (20)     1831 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/understanding-performance.rst
--rw-r--r--   0 james      (501) staff       (20)    12205 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/user-interfaces.rst
--rw-r--r--   0 james      (501) staff       (20)    11744 2023-07-17 19:15:27.000000 dask-2024.4.0/docs/source/why.rst
--rw-r--r--   0 james      (501) staff       (20)     7059 2024-04-01 19:34:09.000000 dask-2024.4.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2024-04-01 19:39:45.999862 dask-2024.4.0/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)      194 2023-07-17 19:15:27.000000 dask-2024.4.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.323315 dask-2024.4.1/
+-rw-r--r--   0 james      (501) staff       (20)     1531 2023-07-17 19:15:27.000000 dask-2024.4.1/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      325 2023-07-17 19:15:27.000000 dask-2024.4.1/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     3780 2024-04-04 16:12:05.323058 dask-2024.4.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1291 2023-07-17 19:15:27.000000 dask-2024.4.1/README.rst
+-rw-r--r--   0 james      (501) staff       (20)     1598 2024-01-23 19:42:07.000000 dask-2024.4.1/conftest.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.215269 dask-2024.4.1/dask/
+-rw-r--r--   0 james      (501) staff       (20)      485 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      133 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/__main__.py
+-rw-r--r--   0 james      (501) staff       (20)      720 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/_compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2024-04-04 16:12:05.323511 dask-2024.4.1/dask/_version.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.221729 dask-2024.4.1/dask/array/
+-rw-r--r--   0 james      (501) staff       (20)     1543 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/array/NUMPY_LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)     5413 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12600 2023-12-20 15:38:57.000000 dask-2024.4.1/dask/array/backends.py
+-rw-r--r--   0 james      (501) staff       (20)     9983 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/blockwise.py
+-rw-r--r--   0 james      (501) staff       (20)    12304 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/chunk.py
+-rw-r--r--   0 james      (501) staff       (20)     5066 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/chunk_types.py
+-rw-r--r--   0 james      (501) staff       (20)   191264 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/core.py
+-rw-r--r--   0 james      (501) staff       (20)    40514 2023-10-25 14:44:16.000000 dask-2024.4.1/dask/array/creation.py
+-rw-r--r--   0 james      (501) staff       (20)     2114 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/cupy_entry_point.py
+-rw-r--r--   0 james      (501) staff       (20)      526 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     9146 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/einsumfuncs.py
+-rw-r--r--   0 james      (501) staff       (20)     7677 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/fft.py
+-rw-r--r--   0 james      (501) staff       (20)    32656 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     1996 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/image.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.222049 dask-2024.4.1/dask/array/lib/
+-rw-r--r--   0 james      (501) staff       (20)       77 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/lib/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      101 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/lib/stride_tricks.py
+-rw-r--r--   0 james      (501) staff       (20)    53218 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/array/linalg.py
+-rw-r--r--   0 james      (501) staff       (20)     6363 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/ma.py
+-rw-r--r--   0 james      (501) staff       (20)     6078 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/numpy_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    12838 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    28479 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/overlap.py
+-rw-r--r--   0 james      (501) staff       (20)    10916 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/percentile.py
+-rw-r--r--   0 james      (501) staff       (20)    40605 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/random.py
+-rw-r--r--   0 james      (501) staff       (20)    28323 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    58469 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/reductions.py
+-rw-r--r--   0 james      (501) staff       (20)    10766 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    81576 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/routines.py
+-rw-r--r--   0 james      (501) staff       (20)    72865 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/slicing.py
+-rw-r--r--   0 james      (501) staff       (20)    16184 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/array/stats.py
+-rw-r--r--   0 james      (501) staff       (20)     8048 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/svg.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.228802 dask-2024.4.1/dask/array/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/array/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)   162686 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/tests/test_array_core.py
+-rw-r--r--   0 james      (501) staff       (20)     6689 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_array_function.py
+-rw-r--r--   0 james      (501) staff       (20)     3159 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_array_utils.py
+-rw-r--r--   0 james      (501) staff       (20)    23222 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_atop.py
+-rw-r--r--   0 james      (501) staff       (20)     3304 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_chunk.py
+-rw-r--r--   0 james      (501) staff       (20)    31190 2023-10-25 14:44:16.000000 dask-2024.4.1/dask/array/tests/test_creation.py
+-rw-r--r--   0 james      (501) staff       (20)    19888 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_core.py
+-rw-r--r--   0 james      (501) staff       (20)     6496 2023-10-25 14:44:16.000000 dask-2024.4.1/dask/array/tests/test_cupy_creation.py
+-rw-r--r--   0 james      (501) staff       (20)      594 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    13412 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_linalg.py
+-rw-r--r--   0 james      (501) staff       (20)     4303 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_overlap.py
+-rw-r--r--   0 james      (501) staff       (20)     2730 2024-03-13 20:06:30.000000 dask-2024.4.1/dask/array/tests/test_cupy_percentile.py
+-rw-r--r--   0 james      (501) staff       (20)     9219 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_random.py
+-rw-r--r--   0 james      (501) staff       (20)     2224 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)     7436 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/tests/test_cupy_routines.py
+-rw-r--r--   0 james      (501) staff       (20)     4877 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_slicing.py
+-rw-r--r--   0 james      (501) staff       (20)     2982 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_cupy_sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     8866 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/tests/test_dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     8821 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/tests/test_fft.py
+-rw-r--r--   0 james      (501) staff       (20)    21013 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     1482 2023-09-28 22:08:27.000000 dask-2024.4.1/dask/array/tests/test_image.py
+-rw-r--r--   0 james      (501) staff       (20)    37415 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/tests/test_linalg.py
+-rw-r--r--   0 james      (501) staff       (20)    15714 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/tests/test_masked.py
+-rw-r--r--   0 james      (501) staff       (20)     1087 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_numpy_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    17446 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    26718 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_overlap.py
+-rw-r--r--   0 james      (501) staff       (20)     3443 2023-11-07 18:15:20.000000 dask-2024.4.1/dask/array/tests/test_percentiles.py
+-rw-r--r--   0 james      (501) staff       (20)    15352 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/tests/test_random.py
+-rw-r--r--   0 james      (501) staff       (20)    36262 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/array/tests/test_rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    33283 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/array/tests/test_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)     7289 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    84472 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/array/tests/test_routines.py
+-rw-r--r--   0 james      (501) staff       (20)    32264 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/array/tests/test_slicing.py
+-rw-r--r--   0 james      (501) staff       (20)     6592 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     5489 2023-09-28 22:08:27.000000 dask-2024.4.1/dask/array/tests/test_stats.py
+-rw-r--r--   0 james      (501) staff       (20)     2740 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_svg.py
+-rw-r--r--   0 james      (501) staff       (20)      525 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_testing.py
+-rw-r--r--   0 james      (501) staff       (20)    17390 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     2706 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_wrap.py
+-rw-r--r--   0 james      (501) staff       (20)     1317 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tests/test_xarray.py
+-rw-r--r--   0 james      (501) staff       (20)     4737 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/tiledb_io.py
+-rw-r--r--   0 james      (501) staff       (20)    10030 2024-03-13 20:06:30.000000 dask-2024.4.1/dask/array/ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    19112 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/array/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     6906 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/array/wrap.py
+-rw-r--r--   0 james      (501) staff       (20)     5122 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/backends.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.229855 dask-2024.4.1/dask/bag/
+-rw-r--r--   0 james      (501) staff       (20)      903 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     9111 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/avro.py
+-rw-r--r--   0 james      (501) staff       (20)      763 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/chunk.py
+-rw-r--r--   0 james      (501) staff       (20)    86002 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/bag/core.py
+-rw-r--r--   0 james      (501) staff       (20)     5464 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/random.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.230557 dask-2024.4.1/dask/bag/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/bag/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3808 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/tests/test_avro.py
+-rw-r--r--   0 james      (501) staff       (20)    51280 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/bag/tests/test_bag.py
+-rw-r--r--   0 james      (501) staff       (20)     6528 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/tests/test_random.py
+-rw-r--r--   0 james      (501) staff       (20)     5049 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/tests/test_text.py
+-rw-r--r--   0 james      (501) staff       (20)     6765 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/text.py
+-rw-r--r--   0 james      (501) staff       (20)      241 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bag/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    54892 2024-04-01 19:10:34.000000 dask-2024.4.1/dask/base.py
+-rw-r--r--   0 james      (501) staff       (20)    53276 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/blockwise.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.231162 dask-2024.4.1/dask/bytes/
+-rw-r--r--   0 james      (501) staff       (20)       75 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bytes/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6933 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bytes/core.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.232021 dask-2024.4.1/dask/bytes/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/bytes/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5158 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bytes/tests/test_bytes_utils.py
+-rw-r--r--   0 james      (501) staff       (20)      530 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bytes/tests/test_compression.py
+-rw-r--r--   0 james      (501) staff       (20)     6815 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/bytes/tests/test_http.py
+-rw-r--r--   0 james      (501) staff       (20)    11476 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bytes/tests/test_local.py
+-rw-r--r--   0 james      (501) staff       (20)    19556 2024-01-29 17:27:45.000000 dask-2024.4.1/dask/bytes/tests/test_s3.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/bytes/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     2001 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/cache.py
+-rw-r--r--   0 james      (501) staff       (20)     4067 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/callbacks.py
+-rw-r--r--   0 james      (501) staff       (20)     5773 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/cli.py
+-rw-r--r--   0 james      (501) staff       (20)      523 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)    24786 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/config.py
+-rw-r--r--   0 james      (501) staff       (20)      959 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/conftest.py
+-rw-r--r--   0 james      (501) staff       (20)     1756 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/context.py
+-rw-r--r--   0 james      (501) staff       (20)    15772 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/core.py
+-rw-r--r--   0 james      (501) staff       (20)     7854 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dask-schema.yaml
+-rw-r--r--   0 james      (501) staff       (20)     1955 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dask.yaml
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.235769 dask-2024.4.1/dask/dataframe/
+-rw-r--r--   0 james      (501) staff       (20)     5405 2024-04-01 19:10:34.000000 dask-2024.4.1/dask/dataframe/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7642 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/_compat.py
+-rw-r--r--   0 james      (501) staff       (20)     2171 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/dataframe/_dtypes.py
+-rw-r--r--   0 james      (501) staff       (20)     3974 2024-02-06 16:03:46.000000 dask-2024.4.1/dask/dataframe/_pyarrow.py
+-rw-r--r--   0 james      (501) staff       (20)     2743 2023-11-10 20:46:15.000000 dask-2024.4.1/dask/dataframe/_pyarrow_compat.py
+-rw-r--r--   0 james      (501) staff       (20)      393 2024-01-25 18:24:19.000000 dask-2024.4.1/dask/dataframe/_testing.py
+-rw-r--r--   0 james      (501) staff       (20)    13386 2024-04-04 16:02:31.000000 dask-2024.4.1/dask/dataframe/accessor.py
+-rw-r--r--   0 james      (501) staff       (20)    25843 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/backends.py
+-rw-r--r--   0 james      (501) staff       (20)     9507 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   314038 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/core.py
+-rw-r--r--   0 james      (501) staff       (20)     4577 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)      552 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/extensions.py
+-rw-r--r--   0 james      (501) staff       (20)   117451 2024-04-01 19:10:34.000000 dask-2024.4.1/dask/dataframe/groupby.py
+-rw-r--r--   0 james      (501) staff       (20)     2463 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/hyperloglog.py
+-rw-r--r--   0 james      (501) staff       (20)    13412 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/indexing.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.236892 dask-2024.4.1/dask/dataframe/io/
+-rw-r--r--   0 james      (501) staff       (20)      706 2023-09-25 17:06:23.000000 dask-2024.4.1/dask/dataframe/io/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    34437 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/csv.py
+-rw-r--r--   0 james      (501) staff       (20)    18830 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/demo.py
+-rw-r--r--   0 james      (501) staff       (20)    18384 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/io/hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    38600 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/io.py
+-rw-r--r--   0 james      (501) staff       (20)    11163 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/dataframe/io/json.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.237460 dask-2024.4.1/dask/dataframe/io/orc/
+-rw-r--r--   0 james      (501) staff       (20)       92 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/io/orc/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4487 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/io/orc/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)     7183 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/io/orc/core.py
+-rw-r--r--   0 james      (501) staff       (20)      510 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/io/orc/utils.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.238242 dask-2024.4.1/dask/dataframe/io/parquet/
+-rw-r--r--   0 james      (501) staff       (20)      166 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/io/parquet/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    72803 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/parquet/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)    67054 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/parquet/core.py
+-rw-r--r--   0 james      (501) staff       (20)    52314 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/parquet/fastparquet.py
+-rw-r--r--   0 james      (501) staff       (20)    32900 2023-10-27 21:32:35.000000 dask-2024.4.1/dask/dataframe/io/parquet/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    21270 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/sql.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.239608 dask-2024.4.1/dask/dataframe/io/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/dataframe/io/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    61918 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/tests/test_csv.py
+-rw-r--r--   0 james      (501) staff       (20)    11436 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/tests/test_demo.py
+-rw-r--r--   0 james      (501) staff       (20)    27324 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/io/tests/test_hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    35589 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/tests/test_io.py
+-rw-r--r--   0 james      (501) staff       (20)     8812 2023-09-21 15:09:09.000000 dask-2024.4.1/dask/dataframe/io/tests/test_json.py
+-rw-r--r--   0 james      (501) staff       (20)     5302 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/io/tests/test_orc.py
+-rw-r--r--   0 james      (501) staff       (20)   166161 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/io/tests/test_parquet.py
+-rw-r--r--   0 james      (501) staff       (20)    17632 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/io/tests/test_sql.py
+-rw-r--r--   0 james      (501) staff       (20)     8041 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/dataframe/io/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    14713 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/dataframe/methods.py
+-rw-r--r--   0 james      (501) staff       (20)    55455 2024-02-09 22:36:17.000000 dask-2024.4.1/dask/dataframe/multi.py
+-rw-r--r--   0 james      (501) staff       (20)     1600 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/numeric.py
+-rw-r--r--   0 james      (501) staff       (20)     8780 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/optimize.py
+-rw-r--r--   0 james      (501) staff       (20)    20819 2023-10-25 14:44:16.000000 dask-2024.4.1/dask/dataframe/partitionquantiles.py
+-rw-r--r--   0 james      (501) staff       (20)    11868 2023-10-27 21:32:31.000000 dask-2024.4.1/dask/dataframe/reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    22170 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    40190 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/shuffle.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.243395 dask-2024.4.1/dask/dataframe/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/dataframe/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    11131 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_accessors.py
+-rw-r--r--   0 james      (501) staff       (20)    70713 2024-01-30 19:27:46.000000 dask-2024.4.1/dask/dataframe/tests/test_arithmetics_reduction.py
+-rw-r--r--   0 james      (501) staff       (20)      942 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/tests/test_boolean.py
+-rw-r--r--   0 james      (501) staff       (20)    17863 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   209193 2024-04-04 15:04:44.000000 dask-2024.4.1/dask/dataframe/tests/test_dataframe.py
+-rw-r--r--   0 james      (501) staff       (20)     1457 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_extensions.py
+-rw-r--r--   0 james      (501) staff       (20)    14847 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/tests/test_format.py
+-rw-r--r--   0 james      (501) staff       (20)   127454 2024-04-04 15:04:44.000000 dask-2024.4.1/dask/dataframe/tests/test_groupby.py
+-rw-r--r--   0 james      (501) staff       (20)     2702 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dataframe/tests/test_hashing.py
+-rw-r--r--   0 james      (501) staff       (20)     2897 2024-01-30 19:27:46.000000 dask-2024.4.1/dask/dataframe/tests/test_hyperloglog.py
+-rw-r--r--   0 james      (501) staff       (20)    23962 2024-02-06 16:03:46.000000 dask-2024.4.1/dask/dataframe/tests/test_indexing.py
+-rw-r--r--   0 james      (501) staff       (20)     7990 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/tests/test_merge_column_and_index.py
+-rw-r--r--   0 james      (501) staff       (20)      463 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/dataframe/tests/test_methods.py
+-rw-r--r--   0 james      (501) staff       (20)    96566 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_multi.py
+-rw-r--r--   0 james      (501) staff       (20)     2624 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_numeric.py
+-rw-r--r--   0 james      (501) staff       (20)     1188 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/tests/test_optimize_dataframe.py
+-rw-r--r--   0 james      (501) staff       (20)     6662 2023-09-25 17:06:24.000000 dask-2024.4.1/dask/dataframe/tests/test_pyarrow.py
+-rw-r--r--   0 james      (501) staff       (20)     5059 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_pyarrow_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    11551 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/dataframe/tests/test_reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    18504 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    63506 2024-01-30 19:27:46.000000 dask-2024.4.1/dask/dataframe/tests/test_shuffle.py
+-rw-r--r--   0 james      (501) staff       (20)    16922 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/dataframe/tests/test_ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    22240 2024-04-01 19:10:34.000000 dask-2024.4.1/dask/dataframe/tests/test_utils_dataframe.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.243682 dask-2024.4.1/dask/dataframe/tseries/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/dataframe/tseries/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7675 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/dataframe/tseries/resample.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.243961 dask-2024.4.1/dask/dataframe/tseries/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/dataframe/tseries/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7028 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/dataframe/tseries/tests/test_resample.py
+-rw-r--r--   0 james      (501) staff       (20)    27538 2023-09-25 17:06:24.000000 dask-2024.4.1/dask/dataframe/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     5331 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/datasets.py
+-rw-r--r--   0 james      (501) staff       (20)    24814 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/delayed.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.244576 dask-2024.4.1/dask/diagnostics/
+-rw-r--r--   0 james      (501) staff       (20)      258 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/diagnostics/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12136 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/diagnostics/profile.py
+-rw-r--r--   0 james      (501) staff       (20)    16332 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/diagnostics/profile_visualize.py
+-rw-r--r--   0 james      (501) staff       (20)     5001 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/diagnostics/progress.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.244973 dask-2024.4.1/dask/diagnostics/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/diagnostics/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12045 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/diagnostics/tests/test_profiler.py
+-rw-r--r--   0 james      (501) staff       (20)     3388 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/diagnostics/tests/test_progress.py
+-rw-r--r--   0 james      (501) staff       (20)      715 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/distributed.py
+-rw-r--r--   0 james      (501) staff       (20)    16587 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/dot.py
+-rw-r--r--   0 james      (501) staff       (20)    19622 2023-10-25 14:44:16.000000 dask-2024.4.1/dask/graph_manipulation.py
+-rw-r--r--   0 james      (501) staff       (20)     2492 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/hashing.py
+-rw-r--r--   0 james      (501) staff       (20)    35516 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/highlevelgraph.py
+-rw-r--r--   0 james      (501) staff       (20)    46004 2023-09-13 17:55:33.000000 dask-2024.4.1/dask/layers.py
+-rw-r--r--   0 james      (501) staff       (20)    18896 2023-09-13 17:55:33.000000 dask-2024.4.1/dask/local.py
+-rw-r--r--   0 james      (501) staff       (20)      487 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/ml.py
+-rw-r--r--   0 james      (501) staff       (20)     8474 2023-09-13 17:55:33.000000 dask-2024.4.1/dask/multiprocessing.py
+-rw-r--r--   0 james      (501) staff       (20)    36224 2024-02-09 15:39:56.000000 dask-2024.4.1/dask/optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    32839 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/order.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/py.typed
+-rw-r--r--   0 james      (501) staff       (20)    12597 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/rewrite.py
+-rw-r--r--   0 james      (501) staff       (20)     7621 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)     2089 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/system.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.250290 dask-2024.4.1/dask/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:15:13.000000 dask-2024.4.1/dask/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      824 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/tests/test_backends.py
+-rw-r--r--   0 james      (501) staff       (20)    33013 2024-02-09 15:39:56.000000 dask-2024.4.1/dask/tests/test_base.py
+-rw-r--r--   0 james      (501) staff       (20)     1613 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_cache.py
+-rw-r--r--   0 james      (501) staff       (20)     2570 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_callbacks.py
+-rw-r--r--   0 james      (501) staff       (20)     1224 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_ci.py
+-rw-r--r--   0 james      (501) staff       (20)     7488 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_cli.py
+-rw-r--r--   0 james      (501) staff       (20)      379 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)    20268 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_config.py
+-rw-r--r--   0 james      (501) staff       (20)     1137 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_context.py
+-rw-r--r--   0 james      (501) staff       (20)     8203 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/tests/test_core.py
+-rw-r--r--   0 james      (501) staff       (20)     1112 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_datasets.py
+-rw-r--r--   0 james      (501) staff       (20)    22962 2024-02-09 15:39:56.000000 dask-2024.4.1/dask/tests/test_delayed.py
+-rw-r--r--   0 james      (501) staff       (20)    33448 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_distributed.py
+-rw-r--r--   0 james      (501) staff       (20)      719 2024-03-13 20:06:30.000000 dask-2024.4.1/dask/tests/test_docs.py
+-rw-r--r--   0 james      (501) staff       (20)    12271 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_dot.py
+-rw-r--r--   0 james      (501) staff       (20)    15338 2024-01-29 17:27:45.000000 dask-2024.4.1/dask/tests/test_graph_manipulation.py
+-rw-r--r--   0 james      (501) staff       (20)     1095 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_hashing.py
+-rw-r--r--   0 james      (501) staff       (20)     9231 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_highgraph.py
+-rw-r--r--   0 james      (501) staff       (20)     9040 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_layers.py
+-rw-r--r--   0 james      (501) staff       (20)     5022 2023-12-13 17:43:46.000000 dask-2024.4.1/dask/tests/test_local.py
+-rw-r--r--   0 james      (501) staff       (20)      419 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_ml.py
+-rw-r--r--   0 james      (501) staff       (20)     8457 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_multiprocessing.py
+-rw-r--r--   0 james      (501) staff       (20)    47821 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    69758 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_order.py
+-rw-r--r--   0 james      (501) staff       (20)     4684 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_rewrite.py
+-rw-r--r--   0 james      (501) staff       (20)     7526 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/tests/test_sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)     7228 2024-01-23 19:42:03.000000 dask-2024.4.1/dask/tests/test_spark_compat.py
+-rw-r--r--   0 james      (501) staff       (20)     2571 2023-08-21 21:39:12.000000 dask-2024.4.1/dask/tests/test_system.py
+-rw-r--r--   0 james      (501) staff       (20)     4749 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_threaded.py
+-rw-r--r--   0 james      (501) staff       (20)    39981 2024-03-13 20:06:30.000000 dask-2024.4.1/dask/tests/test_tokenize.py
+-rw-r--r--   0 james      (501) staff       (20)     4591 2023-09-15 13:43:23.000000 dask-2024.4.1/dask/tests/test_traceback.py
+-rw-r--r--   0 james      (501) staff       (20)     5708 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/tests/test_typing.py
+-rw-r--r--   0 james      (501) staff       (20)    23636 2024-01-23 19:42:07.000000 dask-2024.4.1/dask/tests/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     1598 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/test_utils_test.py
+-rw-r--r--   0 james      (501) staff       (20)      211 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/tests/warning_aliases.py
+-rw-r--r--   0 james      (501) staff       (20)     3001 2023-09-13 17:55:33.000000 dask-2024.4.1/dask/threaded.py
+-rw-r--r--   0 james      (501) staff       (20)    15497 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/typing.py
+-rw-r--r--   0 james      (501) staff       (20)    63637 2024-03-13 20:06:34.000000 dask-2024.4.1/dask/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     4825 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/utils_test.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.250702 dask-2024.4.1/dask/widgets/
+-rw-r--r--   0 james      (501) staff       (20)      792 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.251672 dask-2024.4.1/dask/widgets/templates/
+-rw-r--r--   0 james      (501) staff       (20)     1295 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/templates/array.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      124 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/templates/dataframe.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     2579 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/templates/highlevelgraph.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1981 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/templates/highlevelgraph_layer.html.j2
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.251847 dask-2024.4.1/dask/widgets/tests/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.252403 dask-2024.4.1/dask/widgets/tests/templates/
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/tests/templates/bytes.html.j2
+-rw-r--r--   0 james      (501) staff       (20)       39 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/tests/templates/custom_filter.html.j2
+-rw-r--r--   0 james      (501) staff       (20)       30 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/tests/templates/example.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1401 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/tests/test_widgets.py
+-rw-r--r--   0 james      (501) staff       (20)     1120 2023-07-17 19:15:27.000000 dask-2024.4.1/dask/widgets/widgets.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.321417 dask-2024.4.1/dask.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     3780 2024-04-04 16:12:05.000000 dask-2024.4.1/dask.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    14325 2024-04-04 16:12:05.000000 dask-2024.4.1/dask.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-04 16:12:05.000000 dask-2024.4.1/dask.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      124 2024-04-04 16:12:05.000000 dask-2024.4.1/dask.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-04 16:12:04.000000 dask-2024.4.1/dask.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      532 2024-04-04 16:12:05.000000 dask-2024.4.1/dask.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        5 2024-04-04 16:12:05.000000 dask-2024.4.1/dask.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.252737 dask-2024.4.1/docs/
+-rw-r--r--   0 james      (501) staff       (20)     5741 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     5186 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/make.bat
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.277146 dask-2024.4.1/docs/source/
+-rw-r--r--   0 james      (501) staff       (20)    17900 2024-01-23 19:42:03.000000 dask-2024.4.1/docs/source/10-minutes-to-dask.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.279781 dask-2024.4.1/docs/source/_static/
+-rw-r--r--   0 james      (501) staff       (20)    10187 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/config_converter.js
+-rw-r--r--   0 james      (501) staff       (20)    11021 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/_static/dask-simple.png
+-rw-r--r--   0 james      (501) staff       (20)     2375 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/main-page.css
+-rw-r--r--   0 james      (501) staff       (20)    15598 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/profile.html
+-rw-r--r--   0 james      (501) staff       (20)    65304 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/stacked_profile.html
+-rw-r--r--   0 james      (501) staff       (20)      523 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/style.css
+-rw-r--r--   0 james      (501) staff       (20)      365 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 james      (501) staff       (20)   292662 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/transpose_cyto.html
+-rw-r--r--   0 james      (501) staff       (20)    49423 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_static/yaml.min.js
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.280480 dask-2024.4.1/docs/source/_templates/
+-rw-r--r--   0 james      (501) staff       (20)      180 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/_templates/layout.html
+-rw-r--r--   0 james      (501) staff       (20)     4349 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/adaptive.rst
+-rw-r--r--   0 james      (501) staff       (20)     3109 2023-08-21 21:39:12.000000 dask-2024.4.1/docs/source/api.rst
+-rw-r--r--   0 james      (501) staff       (20)     7189 2023-08-21 21:39:12.000000 dask-2024.4.1/docs/source/array-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     2943 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-assignment.rst
+-rw-r--r--   0 james      (501) staff       (20)     4740 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)    13262 2023-08-21 21:39:12.000000 dask-2024.4.1/docs/source/array-chunks.rst
+-rw-r--r--   0 james      (501) staff       (20)    18437 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-creation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5885 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-design.rst
+-rw-r--r--   0 james      (501) staff       (20)     2857 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-gufunc.rst
+-rw-r--r--   0 james      (501) staff       (20)    21469 2023-08-21 21:39:12.000000 dask-2024.4.1/docs/source/array-numpy-compatibility.rst
+-rw-r--r--   0 james      (501) staff       (20)     6069 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-overlap.rst
+-rw-r--r--   0 james      (501) staff       (20)     3924 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-random.rst
+-rw-r--r--   0 james      (501) staff       (20)     4137 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-slicing.rst
+-rw-r--r--   0 james      (501) staff       (20)     3291 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-sparse.rst
+-rw-r--r--   0 james      (501) staff       (20)     2018 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-stack.rst
+-rw-r--r--   0 james      (501) staff       (20)     1140 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/array-stats.rst
+-rw-r--r--   0 james      (501) staff       (20)     4154 2023-08-21 21:39:12.000000 dask-2024.4.1/docs/source/array.rst
+-rw-r--r--   0 james      (501) staff       (20)     1574 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/bag-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     4557 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/bag-creation.rst
+-rw-r--r--   0 james      (501) staff       (20)     4068 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/bag.rst
+-rw-r--r--   0 james      (501) staff       (20)    14042 2024-01-23 19:42:03.000000 dask-2024.4.1/docs/source/best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     5553 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/caching.rst
+-rw-r--r--   0 james      (501) staff       (20)   368008 2024-04-04 16:02:59.000000 dask-2024.4.1/docs/source/changelog.rst
+-rw-r--r--   0 james      (501) staff       (20)      211 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/cheatsheet.rst
+-rw-r--r--   0 james      (501) staff       (20)     4047 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/cli.rst
+-rw-r--r--   0 james      (501) staff       (20)    15922 2024-03-13 20:06:34.000000 dask-2024.4.1/docs/source/conf.py
+-rw-r--r--   0 james      (501) staff       (20)    16945 2024-03-13 20:06:30.000000 dask-2024.4.1/docs/source/configuration.rst
+-rw-r--r--   0 james      (501) staff       (20)    18998 2024-03-13 20:06:30.000000 dask-2024.4.1/docs/source/custom-collections.rst
+-rw-r--r--   0 james      (501) staff       (20)     3604 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/custom-graphs.rst
+-rw-r--r--   0 james      (501) staff       (20)     4209 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/customize-initialization.rst
+-rw-r--r--   0 james      (501) staff       (20)      932 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dashboard-progress-script.py
+-rw-r--r--   0 james      (501) staff       (20)    15045 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dashboard.rst
+-rw-r--r--   0 james      (501) staff       (20)   203552 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/daskcheatsheet.pdf
+-rw-r--r--   0 james      (501) staff       (20)    10542 2024-03-13 20:06:34.000000 dask-2024.4.1/docs/source/dataframe-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     9611 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dataframe-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     3951 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dataframe-categoricals.rst
+-rw-r--r--   0 james      (501) staff       (20)     5977 2023-12-15 20:02:17.000000 dask-2024.4.1/docs/source/dataframe-create.rst
+-rw-r--r--   0 james      (501) staff       (20)     5014 2023-12-15 20:02:17.000000 dask-2024.4.1/docs/source/dataframe-design.rst
+-rw-r--r--   0 james      (501) staff       (20)     6224 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dataframe-extend.rst
+-rw-r--r--   0 james      (501) staff       (20)      423 2024-03-13 20:06:34.000000 dask-2024.4.1/docs/source/dataframe-extra.rst
+-rw-r--r--   0 james      (501) staff       (20)     8032 2023-12-15 20:02:17.000000 dask-2024.4.1/docs/source/dataframe-groupby.rst
+-rw-r--r--   0 james      (501) staff       (20)     9351 2024-01-23 19:42:03.000000 dask-2024.4.1/docs/source/dataframe-hive.rst
+-rw-r--r--   0 james      (501) staff       (20)     6115 2023-10-25 14:44:16.000000 dask-2024.4.1/docs/source/dataframe-indexing.rst
+-rw-r--r--   0 james      (501) staff       (20)     3454 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dataframe-joins.rst
+-rw-r--r--   0 james      (501) staff       (20)    13645 2024-03-13 20:06:34.000000 dask-2024.4.1/docs/source/dataframe-legacy-api.rst
+-rw-r--r--   0 james      (501) staff       (20)    10545 2024-01-23 19:42:03.000000 dask-2024.4.1/docs/source/dataframe-parquet.rst
+-rw-r--r--   0 james      (501) staff       (20)    12661 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/dataframe-sql.rst
+-rw-r--r--   0 james      (501) staff       (20)     6608 2024-02-06 16:49:58.000000 dask-2024.4.1/docs/source/dataframe.rst
+-rw-r--r--   0 james      (501) staff       (20)      363 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/debugging-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)     1696 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/delayed-api.rst
+-rw-r--r--   0 james      (501) staff       (20)    17616 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/delayed-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     1497 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/delayed-collections.rst
+-rw-r--r--   0 james      (501) staff       (20)     6357 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/delayed.rst
+-rw-r--r--   0 james      (501) staff       (20)     3620 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-cli.rst
+-rw-r--r--   0 james      (501) staff       (20)     4797 2024-01-26 23:05:40.000000 dask-2024.4.1/docs/source/deploying-cloud.rst
+-rw-r--r--   0 james      (501) staff       (20)     2868 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-docker.rst
+-rw-r--r--   0 james      (501) staff       (20)      246 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/deploying-extra.rst
+-rw-r--r--   0 james      (501) staff       (20)     9939 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-hpc.rst
+-rw-r--r--   0 james      (501) staff       (20)     4001 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-kubernetes.rst
+-rw-r--r--   0 james      (501) staff       (20)     5823 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-python-advanced.rst
+-rw-r--r--   0 james      (501) staff       (20)     2839 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-python.rst
+-rw-r--r--   0 james      (501) staff       (20)     1619 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/deploying-ssh.rst
+-rw-r--r--   0 james      (501) staff       (20)     8213 2024-02-09 15:39:56.000000 dask-2024.4.1/docs/source/deploying.rst
+-rw-r--r--   0 james      (501) staff       (20)    10868 2023-12-14 20:19:54.000000 dask-2024.4.1/docs/source/deployment-considerations.rst
+-rw-r--r--   0 james      (501) staff       (20)    13137 2024-03-13 20:06:30.000000 dask-2024.4.1/docs/source/develop.rst
+-rw-r--r--   0 james      (501) staff       (20)     4442 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/diagnostics-distributed.rst
+-rw-r--r--   0 james      (501) staff       (20)    10407 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/diagnostics-local.rst
+-rw-r--r--   0 james      (501) staff       (20)     4548 2024-04-01 19:10:34.000000 dask-2024.4.1/docs/source/ecosystem.rst
+-rw-r--r--   0 james      (501) staff       (20)    18500 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/faq.rst
+-rw-r--r--   0 james      (501) staff       (20)    25633 2024-02-01 17:01:41.000000 dask-2024.4.1/docs/source/futures.rst
+-rw-r--r--   0 james      (501) staff       (20)     5820 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/gpu.rst
+-rw-r--r--   0 james      (501) staff       (20)     2541 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/graph_manipulation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5433 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/graphs.rst
+-rw-r--r--   0 james      (501) staff       (20)     5399 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/graphviz.rst
+-rw-r--r--   0 james      (501) staff       (20)     6946 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/high-level-graphs.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.281941 dask-2024.4.1/docs/source/how-to/
+-rw-r--r--   0 james      (501) staff       (20)    15531 2024-04-01 19:10:34.000000 dask-2024.4.1/docs/source/how-to/connect-to-remote-data.rst
+-rw-r--r--   0 james      (501) staff       (20)    11477 2023-08-21 21:39:12.000000 dask-2024.4.1/docs/source/how-to/debug.rst
+-rw-r--r--   0 james      (501) staff       (20)     1722 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/how-to/extend-sizeof.rst
+-rw-r--r--   0 james      (501) staff       (20)      433 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/how-to/index.rst
+-rw-r--r--   0 james      (501) staff       (20)     6680 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/how-to/selecting-the-collection-backend.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.320403 dask-2024.4.1/docs/source/images/
+-rw-r--r--   0 james      (501) staff       (20)    99565 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/10_minutes_array_graph.png
+-rw-r--r--   0 james      (501) staff       (20)    22442 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/10_minutes_bag_graph.png
+-rw-r--r--   0 james      (501) staff       (20)    56229 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/10_minutes_dataframe_graph.png
+-rw-r--r--   0 james      (501) staff       (20)     4059 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/HHMI_Janelia_Color.png
+-rw-r--r--   0 james      (501) staff       (20)    18406 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/array.svg
+-rw-r--r--   0 james      (501) staff       (20)  1620104 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/async-embarrassing.gif
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.320675 dask-2024.4.1/docs/source/images/changelog/
+-rw-r--r--   0 james      (501) staff       (20)    19604 2023-12-01 15:52:50.000000 dask-2024.4.1/docs/source/images/changelog/2023110-rechunking-disk-perf.png
+-rw-r--r--   0 james      (501) staff       (20)   540389 2024-01-26 23:05:40.000000 dask-2024.4.1/docs/source/images/cloud-provider-logos.svg
+-rw-r--r--   0 james      (501) staff       (20)    10752 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/concurrent-futures-threaded.webp
+-rw-r--r--   0 james      (501) staff       (20)   135129 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/crosstalk.svg
+-rw-r--r--   0 james      (501) staff       (20)  2367087 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_jupyterlab.png
+-rw-r--r--   0 james      (501) staff       (20)    37971 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_link.png
+-rw-r--r--   0 james      (501) staff       (20)    68712 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_memory.png
+-rw-r--r--   0 james      (501) staff       (20)   281018 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_memory_new.gif
+-rw-r--r--   0 james      (501) staff       (20)    25435 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_progress.png
+-rw-r--r--   0 james      (501) staff       (20)   276928 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_status.png
+-rw-r--r--   0 james      (501) staff       (20)    12009 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_task_processing.png
+-rw-r--r--   0 james      (501) staff       (20)    58238 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_task_stream_unhealthy.png
+-rw-r--r--   0 james      (501) staff       (20)   103654 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dashboard_taskstream_healthy.png
+-rw-r--r--   0 james      (501) staff       (20)   112822 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-adaptive.svg
+-rw-r--r--   0 james      (501) staff       (20)    14645 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-array.svg
+-rw-r--r--   0 james      (501) staff       (20)   222084 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-cluster-manager.svg
+-rw-r--r--   0 james      (501) staff       (20)    18782 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-dataframe.svg
+-rw-r--r--   0 james      (501) staff       (20)   381903 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-overview-distributed-callout.svg
+-rw-r--r--   0 james      (501) staff       (20)   357643 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-overview-schedulers.svg
+-rw-r--r--   0 james      (501) staff       (20)    97471 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask-overview.svg
+-rw-r--r--   0 james      (501) staff       (20)     3022 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_horizontal.svg
+-rw-r--r--   0 james      (501) staff       (20)     3651 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_horizontal_black.svg
+-rw-r--r--   0 james      (501) staff       (20)     3767 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_horizontal_on_blue.svg
+-rw-r--r--   0 james      (501) staff       (20)     3738 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_horizontal_on_pink.svg
+-rw-r--r--   0 james      (501) staff       (20)     3738 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_horizontal_white.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_icon.svg
+-rw-r--r--   0 james      (501) staff       (20)     1571 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_icon_black.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_icon_on_pink.svg
+-rw-r--r--   0 james      (501) staff       (20)     1609 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/dask_icon_white.svg
+-rw-r--r--   0 james      (501) staff       (20)    20216 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/delayed-inc-double-add.svg
+-rw-r--r--   0 james      (501) staff       (20)   104628 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/distributed-overview.svg
+-rw-r--r--   0 james      (501) staff       (20)    18297 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/frame-shuffle.svg
+-rw-r--r--   0 james      (501) staff       (20)    22979 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/frame-sort.svg
+-rw-r--r--   0 james      (501) staff       (20)    12181 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/frame.svg
+-rw-r--r--   0 james      (501) staff       (20)   391443 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/images/futures-graph.png
+-rw-r--r--   0 james      (501) staff       (20)    41828 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/gputester-msg.png
+-rw-r--r--   0 james      (501) staff       (20)   210392 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/growth_of_languages.png
+-rw-r--r--   0 james      (501) staff       (20)   167834 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/growth_of_libraries.png
+-rw-r--r--   0 james      (501) staff       (20)     4097 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/inc-add.svg
+-rw-r--r--   0 james      (501) staff       (20)   123010 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/map-reduce-task-scheduling.svg
+-rw-r--r--   0 james      (501) staff       (20)   482302 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/map_blocks_drop_axis.png
+-rw-r--r--   0 james      (501) staff       (20)   113067 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/merge_chunks.png
+-rw-r--r--   0 james      (501) staff       (20)    63244 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/merge_chunks_false.png
+-rw-r--r--   0 james      (501) staff       (20)    13024 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/optimize_dask1.svg
+-rw-r--r--   0 james      (501) staff       (20)     8803 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/optimize_dask2.svg
+-rw-r--r--   0 james      (501) staff       (20)     5198 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/optimize_dask3.svg
+-rw-r--r--   0 james      (501) staff       (20)     4104 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/optimize_dask4.svg
+-rw-r--r--   0 james      (501) staff       (20)     2738 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/optimize_dask5.svg
+-rw-r--r--   0 james      (501) staff       (20)   292827 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/order-failure.png
+-rw-r--r--   0 james      (501) staff       (20)   239828 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/order-success.png
+-rw-r--r--   0 james      (501) staff       (20)    40833 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/overlap.svg
+-rw-r--r--   0 james      (501) staff       (20)    18785 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/overlapping-blocks.svg
+-rw-r--r--   0 james      (501) staff       (20)     4537 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/overlapping-neighbors.svg
+-rw-r--r--   0 james      (501) staff       (20)    20533 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/pipeline.svg
+-rw-r--r--   0 james      (501) staff       (20)    31576 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/reshape.png
+-rw-r--r--   0 james      (501) staff       (20)    31410 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/reshape_problem.png
+-rw-r--r--   0 james      (501) staff       (20)    33288 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/reshape_rechunked.png
+-rw-r--r--   0 james      (501) staff       (20)    50209 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/scaling-edges.png
+-rw-r--r--   0 james      (501) staff       (20)    68476 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/scaling-nodes.png
+-rw-r--r--   0 james      (501) staff       (20)    21294 2023-07-17 19:15:13.000000 dask-2024.4.1/docs/source/images/simple-dask.png
+-rw-r--r--   0 james      (501) staff       (20)    27572 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/transpose-hlg-hovertooltip.png
+-rw-r--r--   0 james      (501) staff       (20)    84492 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/transpose-hlg-html-repr.png
+-rw-r--r--   0 james      (501) staff       (20)    39365 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/transpose.svg
+-rw-r--r--   0 james      (501) staff       (20)    22446 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/transpose_opt.svg
+-rw-r--r--   0 james      (501) staff       (20)   115022 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/trivial.svg
+-rw-r--r--   0 james      (501) staff       (20)     2451 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/images/unoverlapping-neighbors.svg
+-rw-r--r--   0 james      (501) staff       (20)    12486 2024-02-09 15:39:56.000000 dask-2024.4.1/docs/source/index.rst
+-rw-r--r--   0 james      (501) staff       (20)    15500 2024-03-13 20:06:34.000000 dask-2024.4.1/docs/source/install.rst
+-rw-r--r--   0 james      (501) staff       (20)      341 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/internals.rst
+-rw-r--r--   0 james      (501) staff       (20)      868 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/logos.rst
+-rw-r--r--   0 james      (501) staff       (20)     3573 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/maintainers.rst
+-rw-r--r--   0 james      (501) staff       (20)    12200 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/optimize.rst
+-rw-r--r--   0 james      (501) staff       (20)     7119 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/order.rst
+-rw-r--r--   0 james      (501) staff       (20)     4810 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/phases-of-computation.rst
+-rw-r--r--   0 james      (501) staff       (20)      857 2023-12-07 19:39:17.000000 dask-2024.4.1/docs/source/presentations.rst
+-rw-r--r--   0 james      (501) staff       (20)      868 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/prometheus.rst
+-rw-r--r--   0 james      (501) staff       (20)     6010 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/scheduler-overview.rst
+-rw-r--r--   0 james      (501) staff       (20)     4493 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/scheduling-policy.rst
+-rw-r--r--   0 james      (501) staff       (20)    11015 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/scheduling.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:05.321112 dask-2024.4.1/docs/source/scripts/
+-rw-r--r--   0 james      (501) staff       (20)     3294 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/scripts/scheduling.py
+-rw-r--r--   0 james      (501) staff       (20)     6104 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/shared.rst
+-rw-r--r--   0 james      (501) staff       (20)     4562 2023-12-13 17:43:46.000000 dask-2024.4.1/docs/source/software-environments.rst
+-rw-r--r--   0 james      (501) staff       (20)     9342 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/spark.rst
+-rw-r--r--   0 james      (501) staff       (20)     3967 2023-09-13 17:55:33.000000 dask-2024.4.1/docs/source/spec.rst
+-rw-r--r--   0 james      (501) staff       (20)     4754 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/support.rst
+-rw-r--r--   0 james      (501) staff       (20)     1831 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/understanding-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)    12205 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/user-interfaces.rst
+-rw-r--r--   0 james      (501) staff       (20)    11744 2023-07-17 19:15:27.000000 dask-2024.4.1/docs/source/why.rst
+-rw-r--r--   0 james      (501) staff       (20)     7059 2024-04-04 16:08:14.000000 dask-2024.4.1/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-04-04 16:12:05.323369 dask-2024.4.1/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)      194 2023-07-17 19:15:27.000000 dask-2024.4.1/setup.py
```

### Comparing `dask-2024.4.0/LICENSE.txt` & `dask-2024.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/PKG-INFO` & `dask-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Parallel PyData with Task Scheduling
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/dask/dask/
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,15 @@
 Requires-Dist: numpy>=1.21; extra == "array"
 Provides-Extra: bag
 Provides-Extra: dataframe
 Requires-Dist: dask[array]; extra == "dataframe"
 Requires-Dist: pandas>=1.3; extra == "dataframe"
 Requires-Dist: dask-expr<1.1,>=1.0; extra == "dataframe"
 Provides-Extra: distributed
-Requires-Dist: distributed==2024.4.0; extra == "distributed"
+Requires-Dist: distributed==2024.4.1; extra == "distributed"
 Provides-Extra: diagnostics
 Requires-Dist: bokeh>=2.4.2; extra == "diagnostics"
 Requires-Dist: jinja2>=2.10.3; extra == "diagnostics"
 Provides-Extra: delayed
 Provides-Extra: complete
 Requires-Dist: dask[array,dataframe,diagnostics,distributed]; extra == "complete"
 Requires-Dist: pyarrow>=7.0; extra == "complete"
```

### Comparing `dask-2024.4.0/README.rst` & `dask-2024.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/conftest.py` & `dask-2024.4.1/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/_compatibility.py` & `dask-2024.4.1/dask/_compatibility.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/NUMPY_LICENSE.txt` & `dask-2024.4.1/dask/array/NUMPY_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/__init__.py` & `dask-2024.4.1/dask/array/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/backends.py` & `dask-2024.4.1/dask/array/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/blockwise.py` & `dask-2024.4.1/dask/array/blockwise.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/chunk.py` & `dask-2024.4.1/dask/array/chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/chunk_types.py` & `dask-2024.4.1/dask/array/chunk_types.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/core.py` & `dask-2024.4.1/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/creation.py` & `dask-2024.4.1/dask/array/creation.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/cupy_entry_point.py` & `dask-2024.4.1/dask/array/cupy_entry_point.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/dispatch.py` & `dask-2024.4.1/dask/array/dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/einsumfuncs.py` & `dask-2024.4.1/dask/array/einsumfuncs.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/fft.py` & `dask-2024.4.1/dask/array/fft.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/gufunc.py` & `dask-2024.4.1/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/image.py` & `dask-2024.4.1/dask/array/image.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/linalg.py` & `dask-2024.4.1/dask/array/linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/ma.py` & `dask-2024.4.1/dask/array/ma.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/numpy_compat.py` & `dask-2024.4.1/dask/array/numpy_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/optimization.py` & `dask-2024.4.1/dask/array/optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/overlap.py` & `dask-2024.4.1/dask/array/overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/percentile.py` & `dask-2024.4.1/dask/array/percentile.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/random.py` & `dask-2024.4.1/dask/array/random.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/rechunk.py` & `dask-2024.4.1/dask/array/rechunk.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/reductions.py` & `dask-2024.4.1/dask/array/reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/reshape.py` & `dask-2024.4.1/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/routines.py` & `dask-2024.4.1/dask/array/routines.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/slicing.py` & `dask-2024.4.1/dask/array/slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/stats.py` & `dask-2024.4.1/dask/array/stats.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/svg.py` & `dask-2024.4.1/dask/array/svg.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_array_core.py` & `dask-2024.4.1/dask/array/tests/test_array_core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_array_function.py` & `dask-2024.4.1/dask/array/tests/test_array_function.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_array_utils.py` & `dask-2024.4.1/dask/array/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_atop.py` & `dask-2024.4.1/dask/array/tests/test_atop.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_chunk.py` & `dask-2024.4.1/dask/array/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_creation.py` & `dask-2024.4.1/dask/array/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_core.py` & `dask-2024.4.1/dask/array/tests/test_cupy_core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_creation.py` & `dask-2024.4.1/dask/array/tests/test_cupy_creation.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_gufunc.py` & `dask-2024.4.1/dask/array/tests/test_cupy_gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_linalg.py` & `dask-2024.4.1/dask/array/tests/test_cupy_linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_overlap.py` & `dask-2024.4.1/dask/array/tests/test_cupy_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_percentile.py` & `dask-2024.4.1/dask/array/tests/test_cupy_percentile.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_random.py` & `dask-2024.4.1/dask/array/tests/test_cupy_random.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_reductions.py` & `dask-2024.4.1/dask/array/tests/test_cupy_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_routines.py` & `dask-2024.4.1/dask/array/tests/test_cupy_routines.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_slicing.py` & `dask-2024.4.1/dask/array/tests/test_cupy_slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_cupy_sparse.py` & `dask-2024.4.1/dask/array/tests/test_cupy_sparse.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_dispatch.py` & `dask-2024.4.1/dask/array/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_fft.py` & `dask-2024.4.1/dask/array/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_gufunc.py` & `dask-2024.4.1/dask/array/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_image.py` & `dask-2024.4.1/dask/array/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_linalg.py` & `dask-2024.4.1/dask/array/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_masked.py` & `dask-2024.4.1/dask/array/tests/test_masked.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_numpy_compat.py` & `dask-2024.4.1/dask/array/tests/test_numpy_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_optimization.py` & `dask-2024.4.1/dask/array/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_overlap.py` & `dask-2024.4.1/dask/array/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_percentiles.py` & `dask-2024.4.1/dask/array/tests/test_percentiles.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_random.py` & `dask-2024.4.1/dask/array/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_rechunk.py` & `dask-2024.4.1/dask/array/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_reductions.py` & `dask-2024.4.1/dask/array/tests/test_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_reshape.py` & `dask-2024.4.1/dask/array/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_routines.py` & `dask-2024.4.1/dask/array/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_slicing.py` & `dask-2024.4.1/dask/array/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_sparse.py` & `dask-2024.4.1/dask/array/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_stats.py` & `dask-2024.4.1/dask/array/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_svg.py` & `dask-2024.4.1/dask/array/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_testing.py` & `dask-2024.4.1/dask/array/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_ufunc.py` & `dask-2024.4.1/dask/array/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_wrap.py` & `dask-2024.4.1/dask/array/tests/test_wrap.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tests/test_xarray.py` & `dask-2024.4.1/dask/array/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/tiledb_io.py` & `dask-2024.4.1/dask/array/tiledb_io.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/ufunc.py` & `dask-2024.4.1/dask/array/ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/utils.py` & `dask-2024.4.1/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/array/wrap.py` & `dask-2024.4.1/dask/array/wrap.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/backends.py` & `dask-2024.4.1/dask/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/__init__.py` & `dask-2024.4.1/dask/bag/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/avro.py` & `dask-2024.4.1/dask/bag/avro.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/chunk.py` & `dask-2024.4.1/dask/bag/chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/core.py` & `dask-2024.4.1/dask/bag/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/random.py` & `dask-2024.4.1/dask/bag/random.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/tests/test_avro.py` & `dask-2024.4.1/dask/bag/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/tests/test_bag.py` & `dask-2024.4.1/dask/bag/tests/test_bag.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/tests/test_random.py` & `dask-2024.4.1/dask/bag/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/tests/test_text.py` & `dask-2024.4.1/dask/bag/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bag/text.py` & `dask-2024.4.1/dask/bag/text.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/base.py` & `dask-2024.4.1/dask/base.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/blockwise.py` & `dask-2024.4.1/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bytes/core.py` & `dask-2024.4.1/dask/bytes/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bytes/tests/test_bytes_utils.py` & `dask-2024.4.1/dask/bytes/tests/test_bytes_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bytes/tests/test_compression.py` & `dask-2024.4.1/dask/bytes/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bytes/tests/test_http.py` & `dask-2024.4.1/dask/bytes/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bytes/tests/test_local.py` & `dask-2024.4.1/dask/bytes/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/bytes/tests/test_s3.py` & `dask-2024.4.1/dask/bytes/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/cache.py` & `dask-2024.4.1/dask/cache.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/callbacks.py` & `dask-2024.4.1/dask/callbacks.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/cli.py` & `dask-2024.4.1/dask/cli.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/compatibility.py` & `dask-2024.4.1/dask/compatibility.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/config.py` & `dask-2024.4.1/dask/config.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/conftest.py` & `dask-2024.4.1/dask/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/context.py` & `dask-2024.4.1/dask/context.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/core.py` & `dask-2024.4.1/dask/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dask-schema.yaml` & `dask-2024.4.1/dask/dask-schema.yaml`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dask.yaml` & `dask-2024.4.1/dask/dask.yaml`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/__init__.py` & `dask-2024.4.1/dask/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/_compat.py` & `dask-2024.4.1/dask/dataframe/_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/_dtypes.py` & `dask-2024.4.1/dask/dataframe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/_pyarrow.py` & `dask-2024.4.1/dask/dataframe/_pyarrow.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/_pyarrow_compat.py` & `dask-2024.4.1/dask/dataframe/_pyarrow_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/accessor.py` & `dask-2024.4.1/dask/dataframe/accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 import warnings
 
 import numpy as np
 import pandas as pd
 
 from dask.dataframe._compat import check_to_pydatetime_deprecation
 from dask.utils import derived_from
@@ -24,16 +25,23 @@
 
 def _bind_property(cls, pd_cls, attr, min_version=None):
     def func(self):
         return self._property_map(attr)
 
     func.__name__ = attr
     func.__qualname__ = f"{cls.__name__}.{attr}"
+    original_prop = getattr(pd_cls, attr)
+    if isinstance(original_prop, property):
+        method = original_prop.fget
+    elif isinstance(original_prop, functools.cached_property):
+        method = original_prop.func
+    else:
+        method = original_prop
     try:
-        func.__wrapped__ = getattr(pd_cls, attr)
+        func.__wrapped__ = method
     except Exception:
         pass
     setattr(cls, attr, property(derived_from(pd_cls, version=min_version)(func)))
 
 
 def maybe_wrap_pandas(obj, x):
     if isinstance(x, np.ndarray):
```

### Comparing `dask-2024.4.0/dask/dataframe/backends.py` & `dask-2024.4.1/dask/dataframe/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/categorical.py` & `dask-2024.4.1/dask/dataframe/categorical.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/core.py` & `dask-2024.4.1/dask/dataframe/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/dispatch.py` & `dask-2024.4.1/dask/dataframe/dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/extensions.py` & `dask-2024.4.1/dask/dataframe/extensions.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/groupby.py` & `dask-2024.4.1/dask/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/hyperloglog.py` & `dask-2024.4.1/dask/dataframe/hyperloglog.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/indexing.py` & `dask-2024.4.1/dask/dataframe/indexing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/__init__.py` & `dask-2024.4.1/dask/dataframe/io/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/csv.py` & `dask-2024.4.1/dask/dataframe/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/demo.py` & `dask-2024.4.1/dask/dataframe/io/demo.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/hdf.py` & `dask-2024.4.1/dask/dataframe/io/hdf.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/io.py` & `dask-2024.4.1/dask/dataframe/io/io.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/json.py` & `dask-2024.4.1/dask/dataframe/io/json.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/orc/arrow.py` & `dask-2024.4.1/dask/dataframe/io/orc/arrow.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/orc/core.py` & `dask-2024.4.1/dask/dataframe/io/orc/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/parquet/arrow.py` & `dask-2024.4.1/dask/dataframe/io/parquet/arrow.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/parquet/core.py` & `dask-2024.4.1/dask/dataframe/io/parquet/core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/parquet/fastparquet.py` & `dask-2024.4.1/dask/dataframe/io/parquet/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/parquet/utils.py` & `dask-2024.4.1/dask/dataframe/io/parquet/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/sql.py` & `dask-2024.4.1/dask/dataframe/io/sql.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_csv.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_demo.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_hdf.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_hdf.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_io.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_json.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_orc.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_orc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_parquet.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/tests/test_sql.py` & `dask-2024.4.1/dask/dataframe/io/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/io/utils.py` & `dask-2024.4.1/dask/dataframe/io/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/methods.py` & `dask-2024.4.1/dask/dataframe/methods.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/multi.py` & `dask-2024.4.1/dask/dataframe/multi.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/numeric.py` & `dask-2024.4.1/dask/dataframe/numeric.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/optimize.py` & `dask-2024.4.1/dask/dataframe/optimize.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/partitionquantiles.py` & `dask-2024.4.1/dask/dataframe/partitionquantiles.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/reshape.py` & `dask-2024.4.1/dask/dataframe/reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/rolling.py` & `dask-2024.4.1/dask/dataframe/rolling.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/shuffle.py` & `dask-2024.4.1/dask/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_accessors.py` & `dask-2024.4.1/dask/dataframe/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_arithmetics_reduction.py` & `dask-2024.4.1/dask/dataframe/tests/test_arithmetics_reduction.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_boolean.py` & `dask-2024.4.1/dask/dataframe/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_categorical.py` & `dask-2024.4.1/dask/dataframe/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_dataframe.py` & `dask-2024.4.1/dask/dataframe/tests/test_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -4451,17 +4451,14 @@
 
     ddf2 = ddf.assign(y=ddf.x + 1, z=ddf.x - 1)
     ddf[["a", "b"]] = ddf2[["y", "z"]]
 
     assert_eq(df, ddf)
 
 
-@pytest.mark.skipif(
-    DASK_EXPR_ENABLED, reason="Can't make this work with dynamic access"
-)
 def test_attribute_assignment():
     df = pd.DataFrame({"x": [1, 2, 3, 4, 5], "y": [1.0, 2.0, 3.0, 4.0, 5.0]})
     ddf = dd.from_pandas(df, npartitions=2)
 
     ddf.y = ddf.x + ddf.y
     assert_eq(ddf, df.assign(y=df.x + df.y))
```

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_extensions.py` & `dask-2024.4.1/dask/dataframe/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_format.py` & `dask-2024.4.1/dask/dataframe/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_groupby.py` & `dask-2024.4.1/dask/dataframe/tests/test_groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -3353,15 +3353,14 @@
 def test_groupby_numeric_only_None_column_name():
     df = pd.DataFrame({"a": [1, 2, 3], None: ["a", "b", "c"]})
     ddf = dd.from_pandas(df, npartitions=1)
     with pytest.raises(NotImplementedError):
         ddf.groupby(lambda x: x).mean(numeric_only=False)
 
 
-@pytest.mark.skipif(DASK_EXPR_ENABLED, reason="Aggregation not supported")
 @pytest.mark.skipif(not PANDAS_GE_140, reason="requires pandas >= 1.4.0")
 @pytest.mark.parametrize("shuffle_method", [True, False])
 def test_dataframe_named_agg(shuffle_method):
     df = pd.DataFrame(
         {
             "a": [1, 1, 2, 2],
             "b": [1, 2, 5, 6],
@@ -3378,15 +3377,14 @@
         shuffle_method=shuffle_method,
         x=pd.NamedAgg("b", aggfunc="sum"),
         y=pd.NamedAgg("c", aggfunc=partial(np.std, ddof=1)),
     )
     assert_eq(expected, actual)
 
 
-@pytest.mark.skipif(DASK_EXPR_ENABLED, reason="Aggregation not supported")
 @pytest.mark.skipif(not PANDAS_GE_140, reason="requires pandas >= 1.4.0")
 @pytest.mark.parametrize("shuffle_method", [True, False])
 @pytest.mark.parametrize("agg", ["count", "mean", partial(np.var, ddof=1)])
 def test_series_named_agg(shuffle_method, agg):
     df = pd.DataFrame(
         {
             "a": [5, 4, 3, 5, 4, 2, 3, 2],
```

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_hashing.py` & `dask-2024.4.1/dask/dataframe/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_hyperloglog.py` & `dask-2024.4.1/dask/dataframe/tests/test_hyperloglog.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_indexing.py` & `dask-2024.4.1/dask/dataframe/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_merge_column_and_index.py` & `dask-2024.4.1/dask/dataframe/tests/test_merge_column_and_index.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_multi.py` & `dask-2024.4.1/dask/dataframe/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_numeric.py` & `dask-2024.4.1/dask/dataframe/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_optimize_dataframe.py` & `dask-2024.4.1/dask/dataframe/tests/test_optimize_dataframe.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_pyarrow.py` & `dask-2024.4.1/dask/dataframe/tests/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_pyarrow_compat.py` & `dask-2024.4.1/dask/dataframe/tests/test_pyarrow_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_reshape.py` & `dask-2024.4.1/dask/dataframe/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_rolling.py` & `dask-2024.4.1/dask/dataframe/tests/test_rolling.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_shuffle.py` & `dask-2024.4.1/dask/dataframe/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_ufunc.py` & `dask-2024.4.1/dask/dataframe/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tests/test_utils_dataframe.py` & `dask-2024.4.1/dask/dataframe/tests/test_utils_dataframe.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tseries/resample.py` & `dask-2024.4.1/dask/dataframe/tseries/resample.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/tseries/tests/test_resample.py` & `dask-2024.4.1/dask/dataframe/tseries/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dataframe/utils.py` & `dask-2024.4.1/dask/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/datasets.py` & `dask-2024.4.1/dask/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/delayed.py` & `dask-2024.4.1/dask/delayed.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/diagnostics/profile.py` & `dask-2024.4.1/dask/diagnostics/profile.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/diagnostics/profile_visualize.py` & `dask-2024.4.1/dask/diagnostics/profile_visualize.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/diagnostics/progress.py` & `dask-2024.4.1/dask/diagnostics/progress.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/diagnostics/tests/test_profiler.py` & `dask-2024.4.1/dask/diagnostics/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/diagnostics/tests/test_progress.py` & `dask-2024.4.1/dask/diagnostics/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/distributed.py` & `dask-2024.4.1/dask/distributed.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/dot.py` & `dask-2024.4.1/dask/dot.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/graph_manipulation.py` & `dask-2024.4.1/dask/graph_manipulation.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/hashing.py` & `dask-2024.4.1/dask/hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/highlevelgraph.py` & `dask-2024.4.1/dask/highlevelgraph.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/layers.py` & `dask-2024.4.1/dask/layers.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/local.py` & `dask-2024.4.1/dask/local.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/multiprocessing.py` & `dask-2024.4.1/dask/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/optimization.py` & `dask-2024.4.1/dask/optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/order.py` & `dask-2024.4.1/dask/order.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/rewrite.py` & `dask-2024.4.1/dask/rewrite.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/sizeof.py` & `dask-2024.4.1/dask/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/system.py` & `dask-2024.4.1/dask/system.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_backends.py` & `dask-2024.4.1/dask/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_base.py` & `dask-2024.4.1/dask/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_cache.py` & `dask-2024.4.1/dask/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_callbacks.py` & `dask-2024.4.1/dask/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_ci.py` & `dask-2024.4.1/dask/tests/test_ci.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_cli.py` & `dask-2024.4.1/dask/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_config.py` & `dask-2024.4.1/dask/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_context.py` & `dask-2024.4.1/dask/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_core.py` & `dask-2024.4.1/dask/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_datasets.py` & `dask-2024.4.1/dask/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_delayed.py` & `dask-2024.4.1/dask/tests/test_delayed.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_distributed.py` & `dask-2024.4.1/dask/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_docs.py` & `dask-2024.4.1/dask/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_dot.py` & `dask-2024.4.1/dask/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_graph_manipulation.py` & `dask-2024.4.1/dask/tests/test_graph_manipulation.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_hashing.py` & `dask-2024.4.1/dask/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_highgraph.py` & `dask-2024.4.1/dask/tests/test_highgraph.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_layers.py` & `dask-2024.4.1/dask/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_local.py` & `dask-2024.4.1/dask/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_multiprocessing.py` & `dask-2024.4.1/dask/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_optimization.py` & `dask-2024.4.1/dask/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_order.py` & `dask-2024.4.1/dask/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_rewrite.py` & `dask-2024.4.1/dask/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_sizeof.py` & `dask-2024.4.1/dask/tests/test_sizeof.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_spark_compat.py` & `dask-2024.4.1/dask/tests/test_spark_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_system.py` & `dask-2024.4.1/dask/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_threaded.py` & `dask-2024.4.1/dask/tests/test_threaded.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_tokenize.py` & `dask-2024.4.1/dask/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_traceback.py` & `dask-2024.4.1/dask/tests/test_traceback.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_typing.py` & `dask-2024.4.1/dask/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_utils.py` & `dask-2024.4.1/dask/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/tests/test_utils_test.py` & `dask-2024.4.1/dask/tests/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/threaded.py` & `dask-2024.4.1/dask/threaded.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/typing.py` & `dask-2024.4.1/dask/typing.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/utils.py` & `dask-2024.4.1/dask/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/utils_test.py` & `dask-2024.4.1/dask/utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/widgets/__init__.py` & `dask-2024.4.1/dask/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/widgets/templates/array.html.j2` & `dask-2024.4.1/dask/widgets/templates/array.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/widgets/templates/highlevelgraph.html.j2` & `dask-2024.4.1/dask/widgets/templates/highlevelgraph.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/widgets/templates/highlevelgraph_layer.html.j2` & `dask-2024.4.1/dask/widgets/templates/highlevelgraph_layer.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/widgets/tests/test_widgets.py` & `dask-2024.4.1/dask/widgets/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask/widgets/widgets.py` & `dask-2024.4.1/dask/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask.egg-info/PKG-INFO` & `dask-2024.4.1/dask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Parallel PyData with Task Scheduling
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/dask/dask/
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,15 @@
 Requires-Dist: numpy>=1.21; extra == "array"
 Provides-Extra: bag
 Provides-Extra: dataframe
 Requires-Dist: dask[array]; extra == "dataframe"
 Requires-Dist: pandas>=1.3; extra == "dataframe"
 Requires-Dist: dask-expr<1.1,>=1.0; extra == "dataframe"
 Provides-Extra: distributed
-Requires-Dist: distributed==2024.4.0; extra == "distributed"
+Requires-Dist: distributed==2024.4.1; extra == "distributed"
 Provides-Extra: diagnostics
 Requires-Dist: bokeh>=2.4.2; extra == "diagnostics"
 Requires-Dist: jinja2>=2.10.3; extra == "diagnostics"
 Provides-Extra: delayed
 Provides-Extra: complete
 Requires-Dist: dask[array,dataframe,diagnostics,distributed]; extra == "complete"
 Requires-Dist: pyarrow>=7.0; extra == "complete"
```

### Comparing `dask-2024.4.0/dask.egg-info/SOURCES.txt` & `dask-2024.4.1/dask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/dask.egg-info/requires.txt` & `dask-2024.4.1/dask.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 [delayed]
 
 [diagnostics]
 bokeh>=2.4.2
 jinja2>=2.10.3
 
 [distributed]
-distributed==2024.4.0
+distributed==2024.4.1
 
 [test]
 pandas[test]
 pytest
 pytest-cov
 pytest-rerunfailures
 pytest-timeout
```

### Comparing `dask-2024.4.0/docs/Makefile` & `dask-2024.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/make.bat` & `dask-2024.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/10-minutes-to-dask.rst` & `dask-2024.4.1/docs/source/10-minutes-to-dask.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/config_converter.js` & `dask-2024.4.1/docs/source/_static/config_converter.js`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/dask-simple.png` & `dask-2024.4.1/docs/source/_static/dask-simple.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/main-page.css` & `dask-2024.4.1/docs/source/_static/main-page.css`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/profile.html` & `dask-2024.4.1/docs/source/_static/profile.html`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/stacked_profile.html` & `dask-2024.4.1/docs/source/_static/stacked_profile.html`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/style.css` & `dask-2024.4.1/docs/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/transpose_cyto.html` & `dask-2024.4.1/docs/source/_static/transpose_cyto.html`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/_static/yaml.min.js` & `dask-2024.4.1/docs/source/_static/yaml.min.js`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/adaptive.rst` & `dask-2024.4.1/docs/source/adaptive.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/api.rst` & `dask-2024.4.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-api.rst` & `dask-2024.4.1/docs/source/array-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-assignment.rst` & `dask-2024.4.1/docs/source/array-assignment.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-best-practices.rst` & `dask-2024.4.1/docs/source/array-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-chunks.rst` & `dask-2024.4.1/docs/source/array-chunks.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-creation.rst` & `dask-2024.4.1/docs/source/array-creation.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-design.rst` & `dask-2024.4.1/docs/source/array-design.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-gufunc.rst` & `dask-2024.4.1/docs/source/array-gufunc.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-numpy-compatibility.rst` & `dask-2024.4.1/docs/source/array-numpy-compatibility.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-overlap.rst` & `dask-2024.4.1/docs/source/array-overlap.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-random.rst` & `dask-2024.4.1/docs/source/array-random.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-slicing.rst` & `dask-2024.4.1/docs/source/array-slicing.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-sparse.rst` & `dask-2024.4.1/docs/source/array-sparse.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-stack.rst` & `dask-2024.4.1/docs/source/array-stack.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array-stats.rst` & `dask-2024.4.1/docs/source/array-stats.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/array.rst` & `dask-2024.4.1/docs/source/array.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/bag-api.rst` & `dask-2024.4.1/docs/source/bag-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/bag-creation.rst` & `dask-2024.4.1/docs/source/bag-creation.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/bag.rst` & `dask-2024.4.1/docs/source/bag.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/best-practices.rst` & `dask-2024.4.1/docs/source/best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/caching.rst` & `dask-2024.4.1/docs/source/caching.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/changelog.rst` & `dask-2024.4.1/docs/source/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Changelog
 =========
 
+.. _v2024.4.1:
+
+2024.4.1
+--------
+
+This is a minor bugfix release that that fixes an error when importing
+``dask.dataframe`` with Python 3.11.9.
+
+See :pr:`11035` and :pr:`11039` from `Richard (Rick) Zamora`_ for details.
+
+.. dropdown:: Additional changes
+
+  - Remove skips for named aggregations (:pr:`11036`) `Patrick Hoefler`_
+  - Don't deep-copy read-only buffers on unpickle (:pr-distributed:`8609`) `crusaderky`_
+  - Add ``dask-expr`` to ``dask`` conda recipe (:pr-distributed:`8601`) `Charles Blackmon-Luca`_
+
+
 .. _v2024.4.0:
 
 2024.4.0
 --------
 
 Highlights
 ^^^^^^^^^^
```

### Comparing `dask-2024.4.0/docs/source/cli.rst` & `dask-2024.4.1/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/conf.py` & `dask-2024.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/configuration.rst` & `dask-2024.4.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/custom-collections.rst` & `dask-2024.4.1/docs/source/custom-collections.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/custom-graphs.rst` & `dask-2024.4.1/docs/source/custom-graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/customize-initialization.rst` & `dask-2024.4.1/docs/source/customize-initialization.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dashboard-progress-script.py` & `dask-2024.4.1/docs/source/dashboard-progress-script.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dashboard.rst` & `dask-2024.4.1/docs/source/dashboard.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/daskcheatsheet.pdf` & `dask-2024.4.1/docs/source/daskcheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-api.rst` & `dask-2024.4.1/docs/source/dataframe-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-best-practices.rst` & `dask-2024.4.1/docs/source/dataframe-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-categoricals.rst` & `dask-2024.4.1/docs/source/dataframe-categoricals.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-create.rst` & `dask-2024.4.1/docs/source/dataframe-create.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-design.rst` & `dask-2024.4.1/docs/source/dataframe-design.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-extend.rst` & `dask-2024.4.1/docs/source/dataframe-extend.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-groupby.rst` & `dask-2024.4.1/docs/source/dataframe-groupby.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-hive.rst` & `dask-2024.4.1/docs/source/dataframe-hive.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-indexing.rst` & `dask-2024.4.1/docs/source/dataframe-indexing.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-joins.rst` & `dask-2024.4.1/docs/source/dataframe-joins.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-legacy-api.rst` & `dask-2024.4.1/docs/source/dataframe-legacy-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-parquet.rst` & `dask-2024.4.1/docs/source/dataframe-parquet.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe-sql.rst` & `dask-2024.4.1/docs/source/dataframe-sql.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/dataframe.rst` & `dask-2024.4.1/docs/source/dataframe.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/delayed-api.rst` & `dask-2024.4.1/docs/source/delayed-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/delayed-best-practices.rst` & `dask-2024.4.1/docs/source/delayed-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/delayed-collections.rst` & `dask-2024.4.1/docs/source/delayed-collections.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/delayed.rst` & `dask-2024.4.1/docs/source/delayed.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-cli.rst` & `dask-2024.4.1/docs/source/deploying-cli.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-cloud.rst` & `dask-2024.4.1/docs/source/deploying-cloud.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-docker.rst` & `dask-2024.4.1/docs/source/deploying-docker.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-hpc.rst` & `dask-2024.4.1/docs/source/deploying-hpc.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-kubernetes.rst` & `dask-2024.4.1/docs/source/deploying-kubernetes.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-python-advanced.rst` & `dask-2024.4.1/docs/source/deploying-python-advanced.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-python.rst` & `dask-2024.4.1/docs/source/deploying-python.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying-ssh.rst` & `dask-2024.4.1/docs/source/deploying-ssh.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deploying.rst` & `dask-2024.4.1/docs/source/deploying.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/deployment-considerations.rst` & `dask-2024.4.1/docs/source/deployment-considerations.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/develop.rst` & `dask-2024.4.1/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/diagnostics-distributed.rst` & `dask-2024.4.1/docs/source/diagnostics-distributed.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/diagnostics-local.rst` & `dask-2024.4.1/docs/source/diagnostics-local.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/ecosystem.rst` & `dask-2024.4.1/docs/source/ecosystem.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/faq.rst` & `dask-2024.4.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/futures.rst` & `dask-2024.4.1/docs/source/futures.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/gpu.rst` & `dask-2024.4.1/docs/source/gpu.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/graph_manipulation.rst` & `dask-2024.4.1/docs/source/graph_manipulation.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/graphs.rst` & `dask-2024.4.1/docs/source/graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/graphviz.rst` & `dask-2024.4.1/docs/source/graphviz.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/high-level-graphs.rst` & `dask-2024.4.1/docs/source/high-level-graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/how-to/connect-to-remote-data.rst` & `dask-2024.4.1/docs/source/how-to/connect-to-remote-data.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/how-to/debug.rst` & `dask-2024.4.1/docs/source/how-to/debug.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/how-to/extend-sizeof.rst` & `dask-2024.4.1/docs/source/how-to/extend-sizeof.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/how-to/selecting-the-collection-backend.rst` & `dask-2024.4.1/docs/source/how-to/selecting-the-collection-backend.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/10_minutes_array_graph.png` & `dask-2024.4.1/docs/source/images/10_minutes_array_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/10_minutes_bag_graph.png` & `dask-2024.4.1/docs/source/images/10_minutes_bag_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/10_minutes_dataframe_graph.png` & `dask-2024.4.1/docs/source/images/10_minutes_dataframe_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/HHMI_Janelia_Color.png` & `dask-2024.4.1/docs/source/images/HHMI_Janelia_Color.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/array.svg` & `dask-2024.4.1/docs/source/images/array.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/async-embarrassing.gif` & `dask-2024.4.1/docs/source/images/async-embarrassing.gif`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/changelog/2023110-rechunking-disk-perf.png` & `dask-2024.4.1/docs/source/images/changelog/2023110-rechunking-disk-perf.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/cloud-provider-logos.svg` & `dask-2024.4.1/docs/source/images/cloud-provider-logos.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/concurrent-futures-threaded.webp` & `dask-2024.4.1/docs/source/images/concurrent-futures-threaded.webp`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/crosstalk.svg` & `dask-2024.4.1/docs/source/images/crosstalk.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_jupyterlab.png` & `dask-2024.4.1/docs/source/images/dashboard_jupyterlab.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_link.png` & `dask-2024.4.1/docs/source/images/dashboard_link.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_memory.png` & `dask-2024.4.1/docs/source/images/dashboard_memory.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_memory_new.gif` & `dask-2024.4.1/docs/source/images/dashboard_memory_new.gif`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_progress.png` & `dask-2024.4.1/docs/source/images/dashboard_progress.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_status.png` & `dask-2024.4.1/docs/source/images/dashboard_status.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_task_processing.png` & `dask-2024.4.1/docs/source/images/dashboard_task_processing.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_task_stream_unhealthy.png` & `dask-2024.4.1/docs/source/images/dashboard_task_stream_unhealthy.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dashboard_taskstream_healthy.png` & `dask-2024.4.1/docs/source/images/dashboard_taskstream_healthy.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-adaptive.svg` & `dask-2024.4.1/docs/source/images/dask-adaptive.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-array.svg` & `dask-2024.4.1/docs/source/images/dask-array.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-cluster-manager.svg` & `dask-2024.4.1/docs/source/images/dask-cluster-manager.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-dataframe.svg` & `dask-2024.4.1/docs/source/images/dask-dataframe.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-overview-distributed-callout.svg` & `dask-2024.4.1/docs/source/images/dask-overview-distributed-callout.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-overview-schedulers.svg` & `dask-2024.4.1/docs/source/images/dask-overview-schedulers.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask-overview.svg` & `dask-2024.4.1/docs/source/images/dask-overview.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_horizontal.svg` & `dask-2024.4.1/docs/source/images/dask_horizontal.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_horizontal_black.svg` & `dask-2024.4.1/docs/source/images/dask_horizontal_black.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_horizontal_on_blue.svg` & `dask-2024.4.1/docs/source/images/dask_horizontal_on_blue.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_horizontal_on_pink.svg` & `dask-2024.4.1/docs/source/images/dask_horizontal_on_pink.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_horizontal_white.svg` & `dask-2024.4.1/docs/source/images/dask_horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_icon.svg` & `dask-2024.4.1/docs/source/images/dask_icon.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_icon_black.svg` & `dask-2024.4.1/docs/source/images/dask_icon_black.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_icon_on_pink.svg` & `dask-2024.4.1/docs/source/images/dask_icon_on_pink.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/dask_icon_white.svg` & `dask-2024.4.1/docs/source/images/dask_icon_white.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/delayed-inc-double-add.svg` & `dask-2024.4.1/docs/source/images/delayed-inc-double-add.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/distributed-overview.svg` & `dask-2024.4.1/docs/source/images/distributed-overview.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/frame-shuffle.svg` & `dask-2024.4.1/docs/source/images/frame-shuffle.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/frame-sort.svg` & `dask-2024.4.1/docs/source/images/frame-sort.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/frame.svg` & `dask-2024.4.1/docs/source/images/frame.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/futures-graph.png` & `dask-2024.4.1/docs/source/images/futures-graph.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/gputester-msg.png` & `dask-2024.4.1/docs/source/images/gputester-msg.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/growth_of_languages.png` & `dask-2024.4.1/docs/source/images/growth_of_languages.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/growth_of_libraries.png` & `dask-2024.4.1/docs/source/images/growth_of_libraries.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/inc-add.svg` & `dask-2024.4.1/docs/source/images/inc-add.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/map-reduce-task-scheduling.svg` & `dask-2024.4.1/docs/source/images/map-reduce-task-scheduling.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/map_blocks_drop_axis.png` & `dask-2024.4.1/docs/source/images/map_blocks_drop_axis.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/merge_chunks.png` & `dask-2024.4.1/docs/source/images/merge_chunks.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/merge_chunks_false.png` & `dask-2024.4.1/docs/source/images/merge_chunks_false.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/optimize_dask1.svg` & `dask-2024.4.1/docs/source/images/optimize_dask1.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/optimize_dask2.svg` & `dask-2024.4.1/docs/source/images/optimize_dask2.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/optimize_dask3.svg` & `dask-2024.4.1/docs/source/images/optimize_dask3.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/optimize_dask4.svg` & `dask-2024.4.1/docs/source/images/optimize_dask4.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/optimize_dask5.svg` & `dask-2024.4.1/docs/source/images/optimize_dask5.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/order-failure.png` & `dask-2024.4.1/docs/source/images/order-failure.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/order-success.png` & `dask-2024.4.1/docs/source/images/order-success.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/overlap.svg` & `dask-2024.4.1/docs/source/images/overlap.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/overlapping-blocks.svg` & `dask-2024.4.1/docs/source/images/overlapping-blocks.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/overlapping-neighbors.svg` & `dask-2024.4.1/docs/source/images/overlapping-neighbors.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/pipeline.svg` & `dask-2024.4.1/docs/source/images/pipeline.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/reshape.png` & `dask-2024.4.1/docs/source/images/reshape.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/reshape_problem.png` & `dask-2024.4.1/docs/source/images/reshape_problem.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/reshape_rechunked.png` & `dask-2024.4.1/docs/source/images/reshape_rechunked.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/scaling-edges.png` & `dask-2024.4.1/docs/source/images/scaling-edges.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/scaling-nodes.png` & `dask-2024.4.1/docs/source/images/scaling-nodes.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/simple-dask.png` & `dask-2024.4.1/docs/source/images/simple-dask.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/transpose-hlg-hovertooltip.png` & `dask-2024.4.1/docs/source/images/transpose-hlg-hovertooltip.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/transpose-hlg-html-repr.png` & `dask-2024.4.1/docs/source/images/transpose-hlg-html-repr.png`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/transpose.svg` & `dask-2024.4.1/docs/source/images/transpose.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/transpose_opt.svg` & `dask-2024.4.1/docs/source/images/transpose_opt.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/trivial.svg` & `dask-2024.4.1/docs/source/images/trivial.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/images/unoverlapping-neighbors.svg` & `dask-2024.4.1/docs/source/images/unoverlapping-neighbors.svg`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/index.rst` & `dask-2024.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/install.rst` & `dask-2024.4.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/logos.rst` & `dask-2024.4.1/docs/source/logos.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/maintainers.rst` & `dask-2024.4.1/docs/source/maintainers.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/optimize.rst` & `dask-2024.4.1/docs/source/optimize.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/order.rst` & `dask-2024.4.1/docs/source/order.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/phases-of-computation.rst` & `dask-2024.4.1/docs/source/phases-of-computation.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/presentations.rst` & `dask-2024.4.1/docs/source/presentations.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/prometheus.rst` & `dask-2024.4.1/docs/source/prometheus.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/scheduler-overview.rst` & `dask-2024.4.1/docs/source/scheduler-overview.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/scheduling-policy.rst` & `dask-2024.4.1/docs/source/scheduling-policy.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/scheduling.rst` & `dask-2024.4.1/docs/source/scheduling.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/scripts/scheduling.py` & `dask-2024.4.1/docs/source/scripts/scheduling.py`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/shared.rst` & `dask-2024.4.1/docs/source/shared.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/software-environments.rst` & `dask-2024.4.1/docs/source/software-environments.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/spark.rst` & `dask-2024.4.1/docs/source/spark.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/spec.rst` & `dask-2024.4.1/docs/source/spec.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/support.rst` & `dask-2024.4.1/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/understanding-performance.rst` & `dask-2024.4.1/docs/source/understanding-performance.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/user-interfaces.rst` & `dask-2024.4.1/docs/source/user-interfaces.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/docs/source/why.rst` & `dask-2024.4.1/docs/source/why.rst`

 * *Files identical despite different names*

### Comparing `dask-2024.4.0/pyproject.toml` & `dask-2024.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 dataframe = [
     "dask[array]",
     # NOTE: dask-expr is pinning pandas>2. To use pandas<2, please install dask
     # without using the dataframe extra
     "pandas >= 1.3",
     "dask-expr >= 1.0, <1.1",  # dask-expr pins the dask version
 ]
-distributed = ["distributed == 2024.4.0"]
+distributed = ["distributed == 2024.4.1"]
 diagnostics = [
     "bokeh >= 2.4.2",
     "jinja2 >= 2.10.3",
 ]
 # keeping for backwards compatibility
 delayed = []
 complete = [
```

