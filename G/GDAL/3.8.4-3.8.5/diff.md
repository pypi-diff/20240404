# Comparing `tmp/GDAL-3.8.4.tar.gz` & `tmp/GDAL-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GDAL-3.8.4.tar", last modified: Sun Feb 18 15:33:35 2024, max compression
+gzip compressed data, was "GDAL-3.8.5.tar", last modified: Thu Apr  4 17:20:23 2024, max compression
```

## Comparing `GDAL-3.8.4.tar` & `GDAL-3.8.5.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.817569 GDAL-3.8.4/
--rw-r--r--   0 even      (1000) even      (1000)     5375 2024-02-18 15:33:35.817569 GDAL-3.8.4/PKG-INFO
--rw-rw-r--   0 even      (1000) even      (1000)     4488 2024-02-18 15:27:02.000000 GDAL-3.8.4/README.rst
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.789569 GDAL-3.8.4/extensions/
--rw-rw-r--   0 even      (1000) even      (1000)   276603 2024-02-18 15:32:25.000000 GDAL-3.8.4/extensions/gdal_array_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)  1899781 2024-02-18 15:32:21.000000 GDAL-3.8.4/extensions/gdal_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)   126303 2024-02-18 15:32:22.000000 GDAL-3.8.4/extensions/gdalconst_wrap.c
--rw-rw-r--   0 even      (1000) even      (1000)   229118 2024-02-18 15:32:22.000000 GDAL-3.8.4/extensions/gnm_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)  1447479 2024-02-18 15:32:24.000000 GDAL-3.8.4/extensions/ogr_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)   770259 2024-02-18 15:32:25.000000 GDAL-3.8.4/extensions/osr_wrap.cpp
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.785569 GDAL-3.8.4/gdal-utils/
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.817569 GDAL-3.8.4/gdal-utils/GDAL.egg-info/
--rw-r--r--   0 even      (1000) even      (1000)     5375 2024-02-18 15:33:35.000000 GDAL-3.8.4/gdal-utils/GDAL.egg-info/PKG-INFO
--rw-rw-r--   0 even      (1000) even      (1000)     5239 2024-02-18 15:33:35.000000 GDAL-3.8.4/gdal-utils/GDAL.egg-info/SOURCES.txt
--rw-rw-r--   0 even      (1000) even      (1000)        1 2024-02-18 15:33:35.000000 GDAL-3.8.4/gdal-utils/GDAL.egg-info/dependency_links.txt
--rw-rw-r--   0 even      (1000) even      (1000)        1 2023-11-13 17:29:26.000000 GDAL-3.8.4/gdal-utils/GDAL.egg-info/not-zip-safe
--rw-rw-r--   0 even      (1000) even      (1000)       21 2024-02-18 15:33:35.000000 GDAL-3.8.4/gdal-utils/GDAL.egg-info/requires.txt
--rw-rw-r--   0 even      (1000) even      (1000)       18 2024-02-18 15:33:35.000000 GDAL-3.8.4/gdal-utils/GDAL.egg-info/top_level.txt
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.797569 GDAL-3.8.4/gdal-utils/osgeo_utils/
--rw-rw-r--   0 even      (1000) even      (1000)      432 2024-02-08 19:09:22.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/__init__.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.801569 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/
--rw-rw-r--   0 even      (1000) even      (1000)        0 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)     2635 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/array_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     4164 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/base.py
--rw-rw-r--   0 even      (1000) even      (1000)     3447 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/batch_creator.py
--rw-rw-r--   0 even      (1000) even      (1000)    15215 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/color_palette.py
--rw-rw-r--   0 even      (1000) even      (1000)     5649 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/color_table.py
--rw-rw-r--   0 even      (1000) even      (1000)     5384 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/extent_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     8436 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py
--rw-rw-r--   0 even      (1000) even      (1000)     2891 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/numpy_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     5467 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/osr_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     3340 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/progress.py
--rw-rw-r--   0 even      (1000) even      (1000)     6671 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/raster_creation.py
--rw-rw-r--   0 even      (1000) even      (1000)     8828 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/rectangle.py
--rw-rw-r--   0 even      (1000) even      (1000)    16654 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/util.py
--rw-rw-r--   0 even      (1000) even      (1000)   166686 2024-02-07 21:55:33.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal2tiles.py
--rw-rw-r--   0 even      (1000) even      (1000)    15776 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal2xyz.py
--rw-rw-r--   0 even      (1000) even      (1000)    36481 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_calc.py
--rw-rw-r--   0 even      (1000) even      (1000)    16078 2024-02-07 21:55:33.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_edit.py
--rw-rw-r--   0 even      (1000) even      (1000)     9085 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_fillnodata.py
--rw-rw-r--   0 even      (1000) even      (1000)    18738 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_merge.py
--rw-rw-r--   0 even      (1000) even      (1000)    12426 2023-11-09 10:15:22.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_pansharpen.py
--rw-rw-r--   0 even      (1000) even      (1000)    12411 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_polygonize.py
--rw-rw-r--   0 even      (1000) even      (1000)     7587 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_proximity.py
--rw-rw-r--   0 even      (1000) even      (1000)    38844 2023-11-09 10:15:22.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_retile.py
--rw-rw-r--   0 even      (1000) even      (1000)     6682 2023-11-17 17:32:44.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_sieve.py
--rw-rw-r--   0 even      (1000) even      (1000)     5021 2023-11-17 17:32:44.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdalattachpct.py
--rw-rw-r--   0 even      (1000) even      (1000)    20209 2023-11-17 17:32:44.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdalcompare.py
--rw-rw-r--   0 even      (1000) even      (1000)    10018 2023-11-17 17:32:44.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/gdalmove.py
--rw-rw-r--   0 even      (1000) even      (1000)    19311 2023-11-09 10:15:22.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/ogr_layer_algebra.py
--rw-rw-r--   0 even      (1000) even      (1000)    43981 2023-11-09 10:15:22.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/ogrmerge.py
--rw-rw-r--   0 even      (1000) even      (1000)     7753 2023-12-01 17:57:11.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/pct2rgb.py
--rw-rw-r--   0 even      (1000) even      (1000)     7145 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/rgb2pct.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.813569 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/
--rw-rw-r--   0 even      (1000) even      (1000)        0 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)     4632 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/assemblepoly.py
--rw-rw-r--   0 even      (1000) even      (1000)    17347 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py
--rw-rw-r--   0 even      (1000) even      (1000)     2828 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/classify.py
--rw-rw-r--   0 even      (1000) even      (1000)    12326 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/crs2crs2grid.py
--rw-rw-r--   0 even      (1000) even      (1000)    16769 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/densify.py
--rw-rw-r--   0 even      (1000) even      (1000)     8126 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/dump_jp2.py
--rw-rw-r--   0 even      (1000) even      (1000)     9915 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/epsg_tr.py
--rw-rw-r--   0 even      (1000) even      (1000)     3238 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/esri2wkt.py
--rw-rw-r--   0 even      (1000) even      (1000)     4274 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/fft.py
--rw-rw-r--   0 even      (1000) even      (1000)     3008 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/fix_gpkg.py
--rw-rw-r--   0 even      (1000) even      (1000)     3193 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gcps2ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)     5419 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gcps2vec.py
--rw-rw-r--   0 even      (1000) even      (1000)     2580 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gcps2wld.py
--rw-rw-r--   0 even      (1000) even      (1000)     5281 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal2grd.py
--rw-rw-r--   0 even      (1000) even      (1000)     4451 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_auth.py
--rw-rw-r--   0 even      (1000) even      (1000)     8460 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_cp.py
--rw-rw-r--   0 even      (1000) even      (1000)     2561 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py
--rw-rw-r--   0 even      (1000) even      (1000)     8693 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_ls.py
--rw-rw-r--   0 even      (1000) even      (1000)     6670 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_lut.py
--rw-rw-r--   0 even      (1000) even      (1000)     2403 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_mkdir.py
--rw-rw-r--   0 even      (1000) even      (1000)     4426 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py
--rw-rw-r--   0 even      (1000) even      (1000)     4035 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_rm.py
--rw-rw-r--   0 even      (1000) even      (1000)     2538 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_rmdir.py
--rw-rw-r--   0 even      (1000) even      (1000)    11900 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py
--rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalchksum.py
--rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalcopyproj.py
--rw-rw-r--   0 even      (1000) even      (1000)     6067 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalfilter.py
--rw-rw-r--   0 even      (1000) even      (1000)     3021 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalident.py
--rw-rw-r--   0 even      (1000) even      (1000)     3036 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalimport.py
--rw-rw-r--   0 even      (1000) even      (1000)    22270 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)    20066 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdallocationinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)     4095 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/get_soundg.py
--rw-rw-r--   0 even      (1000) even      (1000)     3374 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/histrep.py
--rw-rw-r--   0 even      (1000) even      (1000)     8150 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/hsv_merge.py
--rw-rw-r--   0 even      (1000) even      (1000)    10510 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py
--rw-rw-r--   0 even      (1000) even      (1000)     6440 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/load2odbc.py
--rw-rw-r--   0 even      (1000) even      (1000)     8849 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/loslas2ntv2.py
--rw-rw-r--   0 even      (1000) even      (1000)     2739 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/magphase.py
--rw-rw-r--   0 even      (1000) even      (1000)     2167 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py
--rw-rw-r--   0 even      (1000) even      (1000)     7547 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/mkgraticule.py
--rw-rw-r--   0 even      (1000) even      (1000)    70444 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr2ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)    12810 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr2vrt.py
--rw-rw-r--   0 even      (1000) even      (1000)     7567 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py
--rw-rw-r--   0 even      (1000) even      (1000)    14349 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr_dispatch.py
--rw-rw-r--   0 even      (1000) even      (1000)    21229 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogrinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)    19843 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogrupdate.py
--rw-rw-r--   0 even      (1000) even      (1000)     7724 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/rel.py
--rw-rw-r--   0 even      (1000) even      (1000)     7578 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/tigerpoly.py
--rw-rw-r--   0 even      (1000) even      (1000)     4368 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py
--rw-rw-r--   0 even      (1000) even      (1000)     4055 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/tolatlong.py
--rw-rw-r--   0 even      (1000) even      (1000)     4344 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/val_repl.py
--rw-rw-r--   0 even      (1000) even      (1000)    18476 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py
--rw-rw-r--   0 even      (1000) even      (1000)    16548 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_geoparquet.py
--rw-rw-r--   0 even      (1000) even      (1000)   113359 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_gpkg.py
--rw-rw-r--   0 even      (1000) even      (1000)    70659 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_jp2.py
--rw-rw-r--   0 even      (1000) even      (1000)     4768 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/vec_tr.py
--rw-rw-r--   0 even      (1000) even      (1000)     4843 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/vec_tr_spat.py
--rw-rw-r--   0 even      (1000) even      (1000)     7103 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.817569 GDAL-3.8.4/gdal-utils/scripts/
--rwxrwxr-x   0 even      (1000) even      (1000)      579 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal2tiles.py
--rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal2xyz.py
--rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_calc.py
--rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_edit.py
--rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_fillnodata.py
--rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_merge.py
--rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_pansharpen.py
--rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_polygonize.py
--rwxrwxr-x   0 even      (1000) even      (1000)      335 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_proximity.py
--rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_retile.py
--rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdal_sieve.py
--rwxrwxr-x   0 even      (1000) even      (1000)      331 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdalattachpct.py
--rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdalcompare.py
--rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/gdalmove.py
--rwxrwxr-x   0 even      (1000) even      (1000)      347 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/ogr_layer_algebra.py
--rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/ogrmerge.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/pct2rgb.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-11-06 10:54:53.000000 GDAL-3.8.4/gdal-utils/scripts/rgb2pct.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-02-18 15:33:35.817569 GDAL-3.8.4/osgeo/
--rw-rw-r--   0 even      (1000) even      (1000)     4758 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)   248223 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/gdal.py
--rw-rw-r--   0 even      (1000) even      (1000)    32601 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/gdal_array.py
--rw-rw-r--   0 even      (1000) even      (1000)    12420 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/gdalconst.py
--rw-rw-r--   0 even      (1000) even      (1000)      214 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/gdalnumeric.py
--rw-rw-r--   0 even      (1000) even      (1000)    13770 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/gnm.py
--rw-rw-r--   0 even      (1000) even      (1000)   228585 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)    58490 2024-02-18 15:32:25.000000 GDAL-3.8.4/osgeo/osr.py
--rw-rw-r--   0 even      (1000) even      (1000)       38 2024-02-18 15:33:35.817569 GDAL-3.8.4/setup.cfg
--rw-rw-r--   0 even      (1000) even      (1000)    14340 2024-02-18 15:27:02.000000 GDAL-3.8.4/setup.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.381591 GDAL-3.8.5/
+-rw-r--r--   0 even      (1000) even      (1000)     5375 2024-04-04 17:20:23.381591 GDAL-3.8.5/PKG-INFO
+-rw-rw-r--   0 even      (1000) even      (1000)     4488 2024-04-04 17:09:42.000000 GDAL-3.8.5/README.rst
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.353591 GDAL-3.8.5/extensions/
+-rw-rw-r--   0 even      (1000) even      (1000)   276603 2024-04-04 17:18:42.000000 GDAL-3.8.5/extensions/gdal_array_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)  1899878 2024-04-04 17:18:40.000000 GDAL-3.8.5/extensions/gdal_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)   126303 2024-04-04 17:18:40.000000 GDAL-3.8.5/extensions/gdalconst_wrap.c
+-rw-rw-r--   0 even      (1000) even      (1000)   229118 2024-04-04 17:18:40.000000 GDAL-3.8.5/extensions/gnm_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)  1447479 2024-04-04 17:18:42.000000 GDAL-3.8.5/extensions/ogr_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)   770259 2024-04-04 17:18:41.000000 GDAL-3.8.5/extensions/osr_wrap.cpp
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.349591 GDAL-3.8.5/gdal-utils/
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.381591 GDAL-3.8.5/gdal-utils/GDAL.egg-info/
+-rw-r--r--   0 even      (1000) even      (1000)     5375 2024-04-04 17:20:23.000000 GDAL-3.8.5/gdal-utils/GDAL.egg-info/PKG-INFO
+-rw-rw-r--   0 even      (1000) even      (1000)     5239 2024-04-04 17:20:23.000000 GDAL-3.8.5/gdal-utils/GDAL.egg-info/SOURCES.txt
+-rw-rw-r--   0 even      (1000) even      (1000)        1 2024-04-04 17:20:23.000000 GDAL-3.8.5/gdal-utils/GDAL.egg-info/dependency_links.txt
+-rw-rw-r--   0 even      (1000) even      (1000)        1 2023-11-13 17:29:26.000000 GDAL-3.8.5/gdal-utils/GDAL.egg-info/not-zip-safe
+-rw-rw-r--   0 even      (1000) even      (1000)       21 2024-04-04 17:20:23.000000 GDAL-3.8.5/gdal-utils/GDAL.egg-info/requires.txt
+-rw-rw-r--   0 even      (1000) even      (1000)       18 2024-04-04 17:20:23.000000 GDAL-3.8.5/gdal-utils/GDAL.egg-info/top_level.txt
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.361591 GDAL-3.8.5/gdal-utils/osgeo_utils/
+-rw-rw-r--   0 even      (1000) even      (1000)      432 2024-04-02 10:04:14.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/__init__.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.365591 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/
+-rw-rw-r--   0 even      (1000) even      (1000)        0 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2635 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/array_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4164 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/base.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3447 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/batch_creator.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15215 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/color_palette.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5649 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/color_table.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5384 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/extent_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8436 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2891 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/numpy_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5467 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/osr_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3340 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/progress.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6671 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/raster_creation.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8828 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/rectangle.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16654 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/util.py
+-rw-rw-r--   0 even      (1000) even      (1000)   166757 2024-03-01 13:42:35.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal2tiles.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15776 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal2xyz.py
+-rw-rw-r--   0 even      (1000) even      (1000)    36481 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_calc.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16078 2024-02-07 21:55:33.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_edit.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9085 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_fillnodata.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18738 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_merge.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12426 2023-11-09 10:15:22.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_pansharpen.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12411 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_polygonize.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7587 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_proximity.py
+-rw-rw-r--   0 even      (1000) even      (1000)    38844 2023-11-09 10:15:22.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_retile.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6682 2023-11-17 17:32:44.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_sieve.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5200 2024-04-01 22:32:12.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdalattachpct.py
+-rw-rw-r--   0 even      (1000) even      (1000)    20209 2023-11-17 17:32:44.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdalcompare.py
+-rw-rw-r--   0 even      (1000) even      (1000)    10018 2023-11-17 17:32:44.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/gdalmove.py
+-rw-rw-r--   0 even      (1000) even      (1000)    19311 2023-11-09 10:15:22.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/ogr_layer_algebra.py
+-rw-rw-r--   0 even      (1000) even      (1000)    43981 2023-11-09 10:15:22.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/ogrmerge.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7753 2023-12-01 17:57:11.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/pct2rgb.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7145 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/rgb2pct.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.377591 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/
+-rw-rw-r--   0 even      (1000) even      (1000)        0 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4632 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/assemblepoly.py
+-rw-rw-r--   0 even      (1000) even      (1000)    17347 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2828 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/classify.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12326 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/crs2crs2grid.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16769 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/densify.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8126 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/dump_jp2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9915 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/epsg_tr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3238 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/esri2wkt.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4274 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/fft.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3008 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/fix_gpkg.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3193 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gcps2ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5419 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gcps2vec.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2580 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gcps2wld.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5281 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal2grd.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4451 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_auth.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8460 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_cp.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2561 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8693 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_ls.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6670 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_lut.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2403 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_mkdir.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4426 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4035 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_rm.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2538 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_rmdir.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11900 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalchksum.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3004 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalcopyproj.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6067 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalfilter.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3021 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalident.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3036 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalimport.py
+-rw-rw-r--   0 even      (1000) even      (1000)    22270 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)    20066 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdallocationinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4095 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/get_soundg.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3374 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/histrep.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8150 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/hsv_merge.py
+-rw-rw-r--   0 even      (1000) even      (1000)    10510 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6440 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/load2odbc.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8849 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/loslas2ntv2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2739 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/magphase.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2167 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7547 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/mkgraticule.py
+-rw-rw-r--   0 even      (1000) even      (1000)    70444 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr2ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12810 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr2vrt.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7567 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py
+-rw-rw-r--   0 even      (1000) even      (1000)    14349 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr_dispatch.py
+-rw-rw-r--   0 even      (1000) even      (1000)    21229 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogrinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)    19843 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogrupdate.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7724 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/rel.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7578 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/tigerpoly.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4368 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4055 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/tolatlong.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4344 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/val_repl.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18476 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16548 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_geoparquet.py
+-rw-rw-r--   0 even      (1000) even      (1000)   113359 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_gpkg.py
+-rw-rw-r--   0 even      (1000) even      (1000)    70659 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_jp2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4768 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/vec_tr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4843 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/vec_tr_spat.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7103 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.381591 GDAL-3.8.5/gdal-utils/scripts/
+-rwxrwxr-x   0 even      (1000) even      (1000)      579 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal2tiles.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal2xyz.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_calc.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      315 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_edit.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_fillnodata.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_merge.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_pansharpen.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      339 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_polygonize.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      335 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_proximity.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_retile.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      319 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdal_sieve.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      331 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdalattachpct.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      323 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdalcompare.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/gdalmove.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      347 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/ogr_layer_algebra.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      311 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/ogrmerge.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/pct2rgb.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2023-11-06 10:54:53.000000 GDAL-3.8.5/gdal-utils/scripts/rgb2pct.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2024-04-04 17:20:23.381591 GDAL-3.8.5/osgeo/
+-rw-rw-r--   0 even      (1000) even      (1000)     4758 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)   248626 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/gdal.py
+-rw-rw-r--   0 even      (1000) even      (1000)    32601 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/gdal_array.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12420 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/gdalconst.py
+-rw-rw-r--   0 even      (1000) even      (1000)      214 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/gdalnumeric.py
+-rw-rw-r--   0 even      (1000) even      (1000)    13770 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/gnm.py
+-rw-rw-r--   0 even      (1000) even      (1000)   228585 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)    58490 2024-04-04 17:18:42.000000 GDAL-3.8.5/osgeo/osr.py
+-rw-rw-r--   0 even      (1000) even      (1000)       38 2024-04-04 17:20:23.381591 GDAL-3.8.5/setup.cfg
+-rw-rw-r--   0 even      (1000) even      (1000)    14340 2024-04-04 17:09:42.000000 GDAL-3.8.5/setup.py
```

### Comparing `GDAL-3.8.4/PKG-INFO` & `GDAL-3.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GDAL
-Version: 3.8.4
+Version: 3.8.5
 Summary: GDAL: Geospatial Data Abstraction Library
 Home-page: http://www.gdal.org
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Howard Butler
 Maintainer-email: hobu.inc@gmail.com
 License: MIT
@@ -34,15 +34,15 @@
 bindings for GDAL/OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the https://gdal.org/api/python_bindings.html#tutorials includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.8.4 or greater) and header files (gdal-devel)
+ * libgdal (3.8.5 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.8.4/README.rst` & `GDAL-3.8.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 bindings for GDAL/OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the https://gdal.org/api/python_bindings.html#tutorials includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.8.4 or greater) and header files (gdal-devel)
+ * libgdal (3.8.5 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.8.4/extensions/gdal_array_wrap.cpp` & `GDAL-3.8.5/extensions/gdal_array_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/extensions/gdal_wrap.cpp` & `GDAL-3.8.5/extensions/gdal_wrap.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -49963,14 +49963,19 @@
   if (swig_obj[4]) {
     {
       /* %typemap(in) ( void* callback_data=NULL)  */
       psProgressInfo->psPyCallbackData = swig_obj[4] ;
     }
   }
   {
+    if (!arg1) {
+      SWIG_exception(SWIG_ValueError,"Received a NULL pointer.");
+    }
+  }
+  {
     const int bLocalUseExceptions = GetUseExceptions();
     if ( bLocalUseExceptions ) {
       pushErrorHandler();
     }
     {
       SWIG_PYTHON_THREAD_BEGIN_ALLOW;
       result = (int)wrapper_GDALWarpDestDS(arg1,arg2,arg3,arg4,SWIG_STD_MOVE(arg5),arg6);
```

### Comparing `GDAL-3.8.4/extensions/gdalconst_wrap.c` & `GDAL-3.8.5/extensions/gdalconst_wrap.c`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/extensions/gnm_wrap.cpp` & `GDAL-3.8.5/extensions/gnm_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/extensions/ogr_wrap.cpp` & `GDAL-3.8.5/extensions/ogr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/extensions/osr_wrap.cpp` & `GDAL-3.8.5/extensions/osr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/GDAL.egg-info/PKG-INFO` & `GDAL-3.8.5/gdal-utils/GDAL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GDAL
-Version: 3.8.4
+Version: 3.8.5
 Summary: GDAL: Geospatial Data Abstraction Library
 Home-page: http://www.gdal.org
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Howard Butler
 Maintainer-email: hobu.inc@gmail.com
 License: MIT
@@ -34,15 +34,15 @@
 bindings for GDAL/OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the https://gdal.org/api/python_bindings.html#tutorials includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.8.4 or greater) and header files (gdal-devel)
+ * libgdal (3.8.5 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.8.4/gdal-utils/GDAL.egg-info/SOURCES.txt` & `GDAL-3.8.5/gdal-utils/GDAL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/array_util.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/array_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/base.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/base.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/batch_creator.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/batch_creator.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/color_palette.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/color_palette.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/color_table.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/color_table.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/extent_util.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/extent_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/numpy_util.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/numpy_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/osr_util.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/osr_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/progress.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/progress.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/raster_creation.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/raster_creation.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/rectangle.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/rectangle.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/auxiliary/util.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/auxiliary/util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal2tiles.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal2tiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1569,15 +1569,18 @@
         )
         # Remove useless side car file
         aux_xml = tilefilename + ".aux.xml"
         if gdal.VSIStatL(aux_xml) is not None:
             gdal.Unlink(aux_xml)
 
     if options.verbose:
-        logger.debug(f"\tbuild from zoom {base_tz}, tiles: %s" % ",".join(base_tiles))
+        logger.debug(
+            f"\tbuild from zoom {base_tz}, tiles: %s"
+            % ",".join(["(%d, %d)" % (t[0], t[1]) for t in base_tiles])
+        )
 
     # Create a KML file for this tile.
     if tile_job_info.kml:
         swne = get_tile_swne(tile_job_info, options)
         if swne is not None:
             with my_open(
                 os.path.join(
```

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal2xyz.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal2xyz.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_calc.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_calc.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_edit.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_edit.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_fillnodata.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_fillnodata.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_merge.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_merge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_pansharpen.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_pansharpen.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_polygonize.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_polygonize.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_proximity.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_proximity.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_retile.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_retile.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdal_sieve.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdal_sieve.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdalattachpct.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdalattachpct.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,47 +107,55 @@
     # =============================================================================
 
     ct = get_color_table(pct_filename)
     if pct_filename is not None and ct is None:
         print("No color table on file ", pct_filename)
         return None, 1
 
-    # =============================================================================
-    # Create a MEM clone of the source file.
-    # =============================================================================
-
-    src_ds = open_ds(src_filename)
-
-    mem_ds = gdal.GetDriverByName("MEM").CreateCopy("mem", src_ds)
-
-    # =============================================================================
-    # Assign the color table in memory.
-    # =============================================================================
-
-    mem_ds.GetRasterBand(1).SetRasterColorTable(ct)
-    mem_ds.GetRasterBand(1).SetRasterColorInterpretation(gdal.GCI_PaletteIndex)
-
-    # =============================================================================
-    # Write the dataset to the output file.
-    # =============================================================================
-
+    # Figure out destination driver
     if not driver_name:
         driver_name = GetOutputDriverFor(dst_filename)
 
     dst_driver = gdal.GetDriverByName(driver_name)
     if dst_driver is None:
-        print('"%s" driver not registered.' % driver_name)
+        print(f'"{driver_name}" driver not registered.')
         return None, 1
 
-    if driver_name.upper() == "MEM":
-        out_ds = mem_ds
+    src_ds = open_ds(src_filename)
+    if src_ds is None:
+        print(f"Cannot open {src_filename}")
+        return None, 1
+
+    if driver_name.upper() == "VRT":
+        # For VRT, create the VRT first from the source dataset, so it
+        # correctly refers to it
+        out_ds = dst_driver.CreateCopy(dst_filename or "", src_ds)
+        if out_ds is None:
+            print(f"Cannot create {dst_filename}")
+            return None, 1
+
+        # And now assign the color table to the VRT
+        out_ds.GetRasterBand(1).SetRasterColorTable(ct)
+        out_ds.GetRasterBand(1).SetRasterColorInterpretation(gdal.GCI_PaletteIndex)
     else:
-        out_ds = dst_driver.CreateCopy(dst_filename or "", mem_ds)
+        # Create a MEM clone of the source file.
+        mem_ds = gdal.GetDriverByName("MEM").CreateCopy("mem", src_ds)
+
+        # Assign the color table in memory.
+        mem_ds.GetRasterBand(1).SetRasterColorTable(ct)
+        mem_ds.GetRasterBand(1).SetRasterColorInterpretation(gdal.GCI_PaletteIndex)
+
+        # Write the dataset to the output file.
+        if driver_name.upper() == "MEM":
+            out_ds = mem_ds
+        else:
+            out_ds = dst_driver.CreateCopy(dst_filename or "", mem_ds)
+
+        mem_ds = None
 
-    mem_ds = None
     src_ds = None
 
     return out_ds, 0
 
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv))
```

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdalcompare.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdalcompare.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/gdalmove.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/gdalmove.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/ogr_layer_algebra.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/ogr_layer_algebra.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/ogrmerge.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/ogrmerge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/pct2rgb.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/pct2rgb.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/rgb2pct.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/rgb2pct.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/assemblepoly.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/assemblepoly.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/classify.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/classify.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/crs2crs2grid.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/crs2crs2grid.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/densify.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/densify.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/dump_jp2.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/dump_jp2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/epsg_tr.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/epsg_tr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/esri2wkt.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/esri2wkt.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/fft.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/fft.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/fix_gpkg.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/fix_gpkg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gcps2ogr.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gcps2ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gcps2vec.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gcps2vec.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gcps2wld.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gcps2wld.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal2grd.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal2grd.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_auth.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_auth.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_cp.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_cp.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_ls.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_ls.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_lut.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_lut.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_mkdir.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_mkdir.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_rm.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_rm.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_rmdir.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_rmdir.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalchksum.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalchksum.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalcopyproj.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalcopyproj.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalfilter.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalfilter.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalident.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalident.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalimport.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalimport.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdalinfo.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdalinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/gdallocationinfo.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/gdallocationinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/get_soundg.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/get_soundg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/histrep.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/histrep.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/hsv_merge.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/hsv_merge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/load2odbc.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/load2odbc.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/loslas2ntv2.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/loslas2ntv2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/magphase.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/magphase.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/mkgraticule.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/mkgraticule.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr2ogr.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr2ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr2vrt.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr2vrt.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogr_dispatch.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogr_dispatch.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogrinfo.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogrinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/ogrupdate.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/ogrupdate.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/rel.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/rel.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/tigerpoly.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/tigerpoly.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/tolatlong.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/tolatlong.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/val_repl.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/val_repl.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_geoparquet.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_geoparquet.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_gpkg.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_gpkg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/validate_jp2.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/validate_jp2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/vec_tr.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/vec_tr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/vec_tr_spat.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/vec_tr_spat.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py` & `GDAL-3.8.5/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/gdal-utils/scripts/gdal2tiles.py` & `GDAL-3.8.5/gdal-utils/scripts/gdal2tiles.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/osgeo/__init__.py` & `GDAL-3.8.5/osgeo/__init__.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/osgeo/gdal.py` & `GDAL-3.8.5/osgeo/gdal.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,16 @@
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
         format = 'text'
         if '-json' in new_options:
             format = 'json'
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format == 'json':
             new_options += ['-json']
         elif format != "text":
             raise Exception("Invalid value for format")
         if '-json' in new_options:
             format = 'json'
         if computeMinMax:
@@ -451,15 +452,16 @@
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
         format = 'text'
         if '-json' in new_options:
             format = 'json'
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format == 'json':
             new_options += ['-json']
         elif format != "text":
             raise Exception("Invalid value for format")
         if '-json' in new_options:
             format = 'json'
         if SQLStatement:
@@ -526,15 +528,16 @@
         options can be be an array of strings, a string or let empty and filled from other keywords."""
 
     options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if detailed:
             new_options += ['-detailed']
         if array:
             new_options += ['-array', array]
         if limit:
             new_options += ['-limit', str(limit)]
         if arrayoptions:
@@ -683,15 +686,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if outputType != gdalconst.GDT_Unknown:
             new_options += ['-ot', GetDataTypeName(outputType)]
         if maskBand != None:
             new_options += ['-mask', str(maskBand)]
         if bandList != None:
@@ -938,15 +942,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if srcBands:
             for b in srcBands:
                 new_options += ['-srcband', str(b)]
         if dstBands:
             for b in dstBands:
                 new_options += ['-dstband', str(b)]
         if format is not None:
@@ -1284,15 +1289,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-f', format]
         if srcSRS is not None:
             new_options += ['-s_srs', str(srcSRS)]
         if dstSRS is not None:
             if reproject:
                 new_options += ['-t_srs', str(dstSRS)]
@@ -1553,15 +1559,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if creationOptions is not None:
             if isinstance(creationOptions, dict):
                 for k, v in creationOptions.items():
                     new_options += ['-co', f'{k}={v}']
             else:
@@ -1685,15 +1692,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if creationOptions is not None:
             if isinstance(creationOptions, dict):
                 for k, v in creationOptions.items():
                     new_options += ['-co', f'{k}={v}']
             else:
@@ -1830,15 +1838,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if outputType != gdalconst.GDT_Unknown:
             new_options += ['-ot', GetDataTypeName(outputType)]
         if width != 0 or height != 0:
             new_options += ['-outsize', str(width), str(height)]
         if creationOptions is not None:
@@ -1997,15 +2006,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if outputType != gdalconst.GDT_Unknown:
             new_options += ['-ot', GetDataTypeName(outputType)]
         if creationOptions is not None:
             if isinstance(creationOptions, dict):
                 for k, v in creationOptions.items():
@@ -2180,15 +2190,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if bands is not None:
             for b in bands:
                 new_options += ['-b', str(b)]
         if combineBands:
             new_options += ["-combine_bands", combineBands]
@@ -2396,15 +2407,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if resolution is not None:
             new_options += ['-resolution', str(resolution)]
         if outputBounds is not None:
             new_options += ['-te', _strHighPrec(outputBounds[0]), _strHighPrec(outputBounds[1]), _strHighPrec(outputBounds[2]), _strHighPrec(outputBounds[3])]
         if xRes is not None and yRes is not None:
             new_options += ['-tr', _strHighPrec(xRes), _strHighPrec(yRes)]
         if targetAlignedPixels:
@@ -2524,15 +2536,16 @@
         options = []
     else:
         options = [] if options is None else options
 
     if isinstance(options, str):
         new_options = ParseCommandLine(options)
     else:
-        new_options = options
+        import copy
+        new_options = copy.copy(options)
         if format is not None:
             new_options += ['-of', format]
         if creationOptions is not None:
             if isinstance(creationOptions, dict):
                 for k, v in creationOptions.items():
                     new_options += ['-co', f'{k}={v}']
             else:
```

### Comparing `GDAL-3.8.4/osgeo/gdal_array.py` & `GDAL-3.8.5/osgeo/gdal_array.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/osgeo/gdalconst.py` & `GDAL-3.8.5/osgeo/gdalconst.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/osgeo/gnm.py` & `GDAL-3.8.5/osgeo/gnm.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/osgeo/ogr.py` & `GDAL-3.8.5/osgeo/ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/osgeo/osr.py` & `GDAL-3.8.5/osgeo/osr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.8.4/setup.py` & `GDAL-3.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from glob import glob
 
 from setuptools.command.build_ext import build_ext
 from setuptools import setup
 from setuptools import find_packages
 from setuptools import Extension
 
-version = '3.8.4'
+version = '3.8.5'
 
 # If CXX is defined in the environment, it will be used to link the .so
 # but setuptools will be confused if it is made of several words like 'ccache g++'
 # and it will try to use only the first word.
 # See https://lists.osgeo.org/pipermail/gdal-dev/2016-July/044686.html
 # Note: in general when doing "make", CXX will not be defined, unless it is defined as
 # an environment variable, but in that case it is the value of GDALmake.opt that
```

