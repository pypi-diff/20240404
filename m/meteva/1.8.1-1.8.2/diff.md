# Comparing `tmp/meteva-1.8.1.tar.gz` & `tmp/meteva-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteva-1.8.1.tar", last modified: Tue Mar 26 08:46:55 2024, max compression
+gzip compressed data, was "meteva-1.8.2.tar", last modified: Thu Apr  4 16:14:42 2024, max compression
```

## Comparing `meteva-1.8.1.tar` & `meteva-1.8.2.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.363635 meteva-1.8.1/
--rw-rw-rw-   0        0        0      940 2024-03-26 08:46:55.362690 meteva-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      108 2024-02-23 15:27:40.000000 meteva-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:54.911636 meteva-1.8.1/meteva/
--rw-rw-rw-   0        0        0      254 2024-03-26 01:40:27.000000 meteva-1.8.1/meteva/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:54.922635 meteva-1.8.1/meteva/base/
--rw-rw-rw-   0        0        0      174 2020-03-12 03:56:51.000000 meteva-1.8.1/meteva/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:54.933635 meteva-1.8.1/meteva/base/basicdata/
--rw-rw-rw-   0        0        0      143 2021-04-20 14:24:26.000000 meteva-1.8.1/meteva/base/basicdata/__init__.py
--rw-rw-rw-   0        0        0     1266 2023-11-13 02:13:55.000000 meteva-1.8.1/meteva/base/basicdata/const.py
--rw-rw-rw-   0        0        0     7386 2023-07-03 13:42:46.000000 meteva-1.8.1/meteva/base/basicdata/ctl.py
--rw-rw-rw-   0        0        0    19260 2023-04-21 03:19:11.000000 meteva-1.8.1/meteva/base/basicdata/dicts.py
--rw-rw-rw-   0        0        0    11165 2022-12-20 01:27:25.000000 meteva-1.8.1/meteva/base/basicdata/grid.py
--rw-rw-rw-   0        0        0    32686 2024-03-05 12:30:49.000000 meteva-1.8.1/meteva/base/basicdata/grid_data.py
--rw-rw-rw-   0        0        0      669 2020-03-20 01:16:06.000000 meteva-1.8.1/meteva/base/basicdata/keys.py
--rw-rw-rw-   0        0        0     7163 2022-09-17 14:18:55.000000 meteva-1.8.1/meteva/base/basicdata/sta_data.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:54.949643 meteva-1.8.1/meteva/base/fun/
--rw-rw-rw-   0        0        0      532 2022-05-08 03:56:06.000000 meteva-1.8.1/meteva/base/fun/__init__.py
--rw-rw-rw-   0        0        0    30617 2024-02-12 23:48:02.000000 meteva-1.8.1/meteva/base/fun/combining.py
--rw-rw-rw-   0        0        0    28007 2024-01-07 04:30:26.000000 meteva-1.8.1/meteva/base/fun/computing.py
--rw-rw-rw-   0        0        0    18705 2024-03-04 12:58:48.000000 meteva-1.8.1/meteva/base/fun/diagnosing.py
--rw-rw-rw-   0        0        0    35296 2024-02-21 15:22:08.000000 meteva-1.8.1/meteva/base/fun/grouping.py
--rw-rw-rw-   0        0        0    34810 2024-02-28 06:31:06.000000 meteva-1.8.1/meteva/base/fun/interpolating.py
--rw-rw-rw-   0        0        0    14417 2023-04-23 14:30:42.000000 meteva-1.8.1/meteva/base/fun/nearing.py
--rw-rw-rw-   0        0        0    56372 2023-07-20 03:21:30.000000 meteva-1.8.1/meteva/base/fun/selecting.py
--rw-rw-rw-   0        0        0    36232 2023-08-31 06:14:58.000000 meteva-1.8.1/meteva/base/fun/statisticing.py
--rw-rw-rw-   0        0        0    10676 2022-08-09 06:51:25.000000 meteva-1.8.1/meteva/base/fun/timing.py
--rw-rw-rw-   0        0        0     7042 2023-04-23 13:10:39.000000 meteva-1.8.1/meteva/base/fun/transformating.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:54.979634 meteva-1.8.1/meteva/base/io/
--rw-rw-rw-   0        0        0    21310 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/base/io/CMADaasAccess.py
--rw-rw-rw-   0        0        0    13513 2020-03-04 02:07:45.000000 meteva-1.8.1/meteva/base/io/DataBlock_pb2.py
--rw-rw-rw-   0        0        0     1085 2020-03-04 02:07:45.000000 meteva-1.8.1/meteva/base/io/GDS_data_service.py
--rw-rw-rw-   0        0        0     1288 2020-11-12 11:24:12.000000 meteva-1.8.1/meteva/base/io/SignGenUtil.py
--rw-rw-rw-   0        0        0      471 2022-08-08 08:44:26.000000 meteva-1.8.1/meteva/base/io/__init__.py
--rw-rw-rw-   0        0        0     2987 2020-09-15 02:05:05.000000 meteva-1.8.1/meteva/base/io/clienthandler.py
--rw-rw-rw-   0        0        0     1649 2020-07-06 02:31:29.000000 meteva-1.8.1/meteva/base/io/encoding.py
--rw-rw-rw-   0        0        0    16712 2021-02-15 14:14:53.000000 meteva-1.8.1/meteva/base/io/ftpconn.py
--rw-rw-rw-   0        0        0     1749 2021-04-29 03:15:02.000000 meteva-1.8.1/meteva/base/io/httpclient.py
--rw-rw-rw-   0        0        0     7967 2021-02-15 14:14:53.000000 meteva-1.8.1/meteva/base/io/httpconn.py
--rw-rw-rw-   0        0        0     4709 2021-02-15 14:14:53.000000 meteva-1.8.1/meteva/base/io/loglib.py
--rw-rw-rw-   0        0        0     6048 2022-08-12 07:45:29.000000 meteva-1.8.1/meteva/base/io/print_grib_info.py
--rw-rw-rw-   0        0        0    21031 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/base/io/read_graphydata.py
--rw-rw-rw-   0        0        0    78755 2024-03-26 07:33:20.000000 meteva-1.8.1/meteva/base/io/read_griddata.py
--rw-rw-rw-   0        0        0    91613 2024-02-29 15:27:44.000000 meteva-1.8.1/meteva/base/io/read_stadata.py
--rw-rw-rw-   0        0        0     4670 2023-03-02 08:36:03.000000 meteva-1.8.1/meteva/base/io/write_array.py
--rw-rw-rw-   0        0        0    10893 2024-02-23 08:01:29.000000 meteva-1.8.1/meteva/base/io/write_griddata.py
--rw-rw-rw-   0        0        0    12830 2023-10-10 05:58:04.000000 meteva-1.8.1/meteva/base/io/write_stadata.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.000635 meteva-1.8.1/meteva/base/tool/
--rw-rw-rw-   0        0        0     1216 2023-03-01 02:53:13.000000 meteva-1.8.1/meteva/base/tool/__init__.py
--rw-rw-rw-   0        0        0    54048 2024-02-23 03:35:58.000000 meteva-1.8.1/meteva/base/tool/color_tools.py
--rw-rw-rw-   0        0        0    13819 2022-02-26 00:32:32.000000 meteva-1.8.1/meteva/base/tool/copy_tools.py
--rw-rw-rw-   0        0        0     1248 2023-04-04 14:53:16.000000 meteva-1.8.1/meteva/base/tool/frprmn2.py
--rw-rw-rw-   0        0        0     4695 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/base/tool/grib_tools.py
--rw-rw-rw-   0        0        0     8797 2023-07-04 02:34:53.000000 meteva-1.8.1/meteva/base/tool/maskout.py
--rw-rw-rw-   0        0        0    11675 2023-06-20 14:47:49.000000 meteva-1.8.1/meteva/base/tool/math_tools.py
--rw-rw-rw-   0        0        0    12484 2024-01-18 07:10:32.000000 meteva-1.8.1/meteva/base/tool/path_tools.py
--rw-rw-rw-   0        0        0   180509 2024-02-23 05:27:55.000000 meteva-1.8.1/meteva/base/tool/plot_tools.py
--rw-rw-rw-   0        0        0    35597 2024-02-23 03:38:22.000000 meteva-1.8.1/meteva/base/tool/plot_tools_adv.py
--rw-rw-rw-   0        0        0     4851 2022-02-27 12:00:59.000000 meteva-1.8.1/meteva/base/tool/process_tools.py
--rw-rw-rw-   0        0        0     3647 2020-09-18 14:05:02.000000 meteva-1.8.1/meteva/base/tool/station_tools.py
--rw-rw-rw-   0        0        0     5637 2021-09-29 03:54:03.000000 meteva-1.8.1/meteva/base/tool/time_tools.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.001636 meteva-1.8.1/meteva/method/
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.293634 meteva-1.8.1/meteva/method/Vector/
--rw-rw-rw-   0        0        0      624 2024-02-22 04:04:47.000000 meteva-1.8.1/meteva/method/Vector/__init__.py
--rw-rw-rw-   0        0        0    33207 2024-02-22 07:27:38.000000 meteva-1.8.1/meteva/method/Vector/plot.py
--rw-rw-rw-   0        0        0    46040 2022-08-19 06:02:13.000000 meteva-1.8.1/meteva/method/Vector/score.py
--rw-rw-rw-   0        0        0      387 2023-09-22 07:51:37.000000 meteva-1.8.1/meteva/method/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.012635 meteva-1.8.1/meteva/method/continuous/
--rw-rw-rw-   0        0        0     1128 2024-01-27 14:08:41.000000 meteva-1.8.1/meteva/method/continuous/__init__.py
--rw-rw-rw-   0        0        0    40762 2024-02-23 01:50:41.000000 meteva-1.8.1/meteva/method/continuous/plot.py
--rw-rw-rw-   0        0        0    54412 2024-02-22 03:32:35.000000 meteva-1.8.1/meteva/method/continuous/score.py
--rw-rw-rw-   0        0        0     1248 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/method/continuous/skill.py
--rw-rw-rw-   0        0        0     5417 2023-12-26 02:41:16.000000 meteva-1.8.1/meteva/method/continuous/table.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.018635 meteva-1.8.1/meteva/method/ensemble/
--rw-rw-rw-   0        0        0      211 2021-08-16 08:04:20.000000 meteva-1.8.1/meteva/method/ensemble/__init__.py
--rw-rw-rw-   0        0        0     4412 2022-02-26 23:44:42.000000 meteva-1.8.1/meteva/method/ensemble/plot.py
--rw-rw-rw-   0        0        0     4630 2022-04-21 02:55:24.000000 meteva-1.8.1/meteva/method/ensemble/score.py
--rw-rw-rw-   0        0        0        0 2020-03-04 02:07:36.000000 meteva-1.8.1/meteva/method/ensemble/table.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.025634 meteva-1.8.1/meteva/method/multi_category/
--rw-rw-rw-   0        0        0      543 2021-06-02 08:05:58.000000 meteva-1.8.1/meteva/method/multi_category/__init__.py
--rw-rw-rw-   0        0        0    15473 2022-11-14 03:23:59.000000 meteva-1.8.1/meteva/method/multi_category/plot.py
--rw-rw-rw-   0        0        0    21927 2022-04-21 02:55:24.000000 meteva-1.8.1/meteva/method/multi_category/score.py
--rw-rw-rw-   0        0        0     7803 2022-12-28 08:27:35.000000 meteva-1.8.1/meteva/method/multi_category/table.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.030635 meteva-1.8.1/meteva/method/probability/
--rw-rw-rw-   0        0        0      308 2022-03-02 14:27:29.000000 meteva-1.8.1/meteva/method/probability/__init__.py
--rw-rw-rw-   0        0        0    21703 2022-10-23 06:25:47.000000 meteva-1.8.1/meteva/method/probability/plot.py
--rw-rw-rw-   0        0        0     7341 2022-04-21 02:55:24.000000 meteva-1.8.1/meteva/method/probability/score.py
--rw-rw-rw-   0        0        0     2628 2022-04-21 02:55:24.000000 meteva-1.8.1/meteva/method/probability/table.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.032637 meteva-1.8.1/meteva/method/space/
--rw-rw-rw-   0        0        0      802 2024-02-21 07:49:52.000000 meteva-1.8.1/meteva/method/space/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.036635 meteva-1.8.1/meteva/method/space/acc/
--rw-rw-rw-   0        0        0       82 2023-10-04 03:56:47.000000 meteva-1.8.1/meteva/method/space/acc/__init__.py
--rw-rw-rw-   0        0        0    10168 2024-03-26 08:45:02.000000 meteva-1.8.1/meteva/method/space/acc/acc.py
--rw-rw-rw-   0        0        0      747 2023-09-15 14:42:11.000000 meteva-1.8.1/meteva/method/space/acc/acc_climate_pre.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.043635 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/
--rw-rw-rw-   0        0        0      134 2023-10-01 08:10:28.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.060635 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/
--rw-rw-rw-   0        0        0      244 2023-10-01 08:15:28.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/__init__.py
--rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py
--rw-rw-rw-   0        0        0      774 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0     1560 2024-02-18 07:34:44.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py
--rw-rw-rw-   0        0        0     4594 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py
--rw-rw-rw-   0        0        0     2530 2023-08-21 23:56:50.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/im.py
--rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py
--rw-rw-rw-   0        0        0     3977 2024-02-18 07:34:44.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py
--rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py
--rw-rw-rw-   0        0        0      625 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py
--rw-rw-rw-   0        0        0     1978 2023-08-22 00:02:02.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py
--rw-rw-rw-   0        0        0      278 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_prep.py
--rw-rw-rw-   0        0        0     5528 2023-08-22 00:02:02.000000 meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.063635 meteva-1.8.1/meteva/method/space/cra/
--rw-rw-rw-   0        0        0       62 2024-02-21 07:47:43.000000 meteva-1.8.1/meteva/method/space/cra/__init__.py
--rw-rw-rw-   0        0        0     5824 2024-02-21 13:13:05.000000 meteva-1.8.1/meteva/method/space/cra/cra.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.068634 meteva-1.8.1/meteva/method/space/fqi/
--rw-rw-rw-   0        0        0       65 2023-10-01 08:00:00.000000 meteva-1.8.1/meteva/method/space/fqi/__init__.py
--rw-rw-rw-   0        0        0     5179 2023-09-23 11:58:12.000000 meteva-1.8.1/meteva/method/space/fqi/fqi.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.094635 meteva-1.8.1/meteva/method/space/fqi/lib/
--rw-rw-rw-   0        0        0      366 2023-10-01 08:03:25.000000 meteva-1.8.1/meteva/method/space/fqi/lib/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-08-22 02:14:25.000000 meteva-1.8.1/meteva/method/space/fqi/lib/aaft2d.py
--rw-rw-rw-   0        0        0      658 2023-01-29 06:47:11.000000 meteva-1.8.1/meteva/method/space/fqi/lib/ampstats.py
--rw-rw-rw-   0        0        0       93 2023-01-24 09:38:13.000000 meteva-1.8.1/meteva/method/space/fqi/lib/cbind.py
--rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.1/meteva/method/space/fqi/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0      947 2023-04-02 10:16:53.000000 meteva-1.8.1/meteva/method/space/fqi/lib/distfun.py
--rw-rw-rw-   0        0        0      947 2023-03-26 09:44:16.000000 meteva-1.8.1/meteva/method/space/fqi/lib/fft2d.py
--rw-rw-rw-   0        0        0     2531 2023-08-22 02:11:26.000000 meteva-1.8.1/meteva/method/space/fqi/lib/im.py
--rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/fqi/lib/loc_list_setup.py
--rw-rw-rw-   0        0        0      278 2021-06-01 19:24:10.000000 meteva-1.8.1/meteva/method/space/fqi/lib/locmeasures2d_prep.py
--rw-rw-rw-   0        0        0     4102 2024-02-18 12:48:31.000000 meteva-1.8.1/meteva/method/space/fqi/lib/locperf.py
--rw-rw-rw-   0        0        0      262 2023-03-25 10:39:31.000000 meteva-1.8.1/meteva/method/space/fqi/lib/locperfer.py
--rw-rw-rw-   0        0        0      158 2023-01-28 04:35:01.000000 meteva-1.8.1/meteva/method/space/fqi/lib/mae.py
--rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.1/meteva/method/space/fqi/lib/solutionset.py
--rw-rw-rw-   0        0        0     2398 2023-08-22 02:14:05.000000 meteva-1.8.1/meteva/method/space/fqi/lib/surrogater2d.py
--rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.1/meteva/method/space/fqi/lib/util.py
--rw-rw-rw-   0        0        0      274 2023-01-26 07:28:17.000000 meteva-1.8.1/meteva/method/space/fqi/lib/zapsmall.py
--rw-rw-rw-   0        0        0     1008 2023-08-22 02:11:50.000000 meteva-1.8.1/meteva/method/space/fqi/uiqi.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.097634 meteva-1.8.1/meteva/method/space/fss/
--rw-rw-rw-   0        0        0     1725 2021-11-23 02:49:29.000000 meteva-1.8.1/meteva/method/space/fss/__init__.py
--rw-rw-rw-   0        0        0     8387 2023-04-22 14:53:18.000000 meteva-1.8.1/meteva/method/space/fss/fss.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.109636 meteva-1.8.1/meteva/method/space/fuzzy_logic/
--rw-rw-rw-   0        0        0      194 2023-10-01 07:24:57.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-08-21 03:43:04.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/fss.py
--rw-rw-rw-   0        0        0     2273 2023-09-06 03:36:58.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/fuzzy.py
--rw-rw-rw-   0        0        0     1806 2023-09-04 07:58:00.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/joint.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.134635 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/
--rw-rw-rw-   0        0        0      492 2023-10-01 08:15:28.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/__init__.py
--rw-rw-rw-   0        0        0      783 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0      860 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/fss2dfun.py
--rw-rw-rw-   0        0        0     1908 2023-08-20 08:53:21.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py
--rw-rw-rw-   0        0        0     7349 2023-09-06 09:36:29.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2d.py
--rw-rw-rw-   0        0        0     1016 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py
--rw-rw-rw-   0        0        0     1243 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py
--rw-rw-rw-   0        0        0     1266 2023-09-04 08:38:48.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py
--rw-rw-rw-   0        0        0     6283 2023-08-22 01:44:20.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py
--rw-rw-rw-   0        0        0     3456 2023-09-25 03:11:25.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py
--rw-rw-rw-   0        0        0     7289 2023-08-20 13:30:27.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py
--rw-rw-rw-   0        0        0      188 2023-08-20 12:21:58.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/mincvg2dfun.py
--rw-rw-rw-   0        0        0      183 2023-08-21 03:05:37.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/multicon2dfun.py
--rw-rw-rw-   0        0        0      536 2023-09-06 03:46:36.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py
--rw-rw-rw-   0        0        0      715 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/thresholder.py
--rw-rw-rw-   0        0        0      811 2023-08-21 03:06:59.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py
--rw-rw-rw-   0        0        0     4704 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/vxstats.py
--rw-rw-rw-   0        0        0      275 2021-06-06 10:14:33.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/zapsmall.py
--rw-rw-rw-   0        0        0     2255 2023-09-07 06:37:55.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/minimum_coverage.py
--rw-rw-rw-   0        0        0     2233 2023-09-06 09:01:35.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/multi_event.py
--rw-rw-rw-   0        0        0     2218 2023-09-06 03:36:58.000000 meteva-1.8.1/meteva/method/space/fuzzy_logic/pragmatic.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.138635 meteva-1.8.1/meteva/method/space/geo_box_plot/
--rw-rw-rw-   0        0        0     2496 2023-09-25 04:29:49.000000 meteva-1.8.1/meteva/method/space/geo_box_plot/GeoBoxPlot.py
--rw-rw-rw-   0        0        0       24 2023-10-02 02:14:48.000000 meteva-1.8.1/meteva/method/space/geo_box_plot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.146635 meteva-1.8.1/meteva/method/space/geometric_characterizations/
--rw-rw-rw-   0        0        0       86 2023-10-01 08:16:08.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/__init__.py
--rw-rw-rw-   0        0        0     5187 2024-02-18 08:43:27.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/aindex.py
--rw-rw-rw-   0        0        0     2664 2023-09-24 12:12:06.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/cindex.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.153636 meteva-1.8.1/meteva/method/space/geometric_characterizations/lib/
--rw-rw-rw-   0        0        0       55 2023-10-01 08:21:38.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/lib/__init__.py
--rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py
--rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/lib/util.py
--rw-rw-rw-   0        0        0     2934 2023-09-24 11:40:50.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/sindex.py
--rw-rw-rw-   0        0        0     1859 2023-08-22 00:10:29.000000 meteva-1.8.1/meteva/method/space/geometric_characterizations/spatial_index.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.156637 meteva-1.8.1/meteva/method/space/hausdorff_metric/
--rw-rw-rw-   0        0        0       43 2023-10-01 08:17:18.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.167690 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/
--rw-rw-rw-   0        0        0      150 2023-10-01 08:21:38.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/__init__.py
--rw-rw-rw-   0        0        0      829 2021-05-23 18:14:16.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/as_unitname.py
--rw-rw-rw-   0        0        0      947 2023-04-02 10:14:50.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/distfun.py
--rw-rw-rw-   0        0        0     4731 2023-04-02 10:09:41.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/distmap.py
--rw-rw-rw-   0        0        0     2518 2023-08-22 00:16:03.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/im.py
--rw-rw-rw-   0        0        0     1467 2021-05-23 18:14:16.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py
--rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/solutionset.py
--rw-rw-rw-   0        0        0     5361 2024-02-18 09:02:26.000000 meteva-1.8.1/meteva/method/space/hausdorff_metric/locperf.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.220635 meteva-1.8.1/meteva/method/space/mode/
--rw-rw-rw-   0        0        0     1960 2023-08-24 01:06:15.000000 meteva-1.8.1/meteva/method/space/mode/__init__.py
--rw-rw-rw-   0        0        0      161 2021-02-04 10:20:28.000000 meteva-1.8.1/meteva/method/space/mode/angles_psp.py
--rw-rw-rw-   0        0        0      384 2021-02-04 10:20:28.000000 meteva-1.8.1/meteva/method/space/mode/as_psp.py
--rw-rw-rw-   0        0        0      910 2021-03-10 13:04:02.000000 meteva-1.8.1/meteva/method/space/mode/bearing.py
--rw-rw-rw-   0        0        0     4059 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/censqdelta.py
--rw-rw-rw-   0        0        0    11638 2022-05-30 12:33:28.000000 meteva-1.8.1/meteva/method/space/mode/centmatch.py
--rw-rw-rw-   0        0        0    13874 2023-12-22 00:57:57.000000 meteva-1.8.1/meteva/method/space/mode/consistent.py
--rw-rw-rw-   0        0        0     3537 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/data_pre.py
--rw-rw-rw-   0        0        0     1497 2022-02-25 08:34:50.000000 meteva-1.8.1/meteva/method/space/mode/deltametric.py
--rw-rw-rw-   0        0        0     3541 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/deltamm.py
--rw-rw-rw-   0        0        0    18089 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/deltammSqCen.py
--rw-rw-rw-   0        0        0     3530 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/deltamm_bak.py
--rw-rw-rw-   0        0        0     4801 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/distmap.py
--rw-rw-rw-   0        0        0     6070 2024-02-22 03:58:40.000000 meteva-1.8.1/meteva/method/space/mode/feature_axis.py
--rw-rw-rw-   0        0        0     4087 2022-06-24 14:09:57.000000 meteva-1.8.1/meteva/method/space/mode/feature_comps.py
--rw-rw-rw-   0        0        0    32379 2023-08-22 14:03:20.000000 meteva-1.8.1/meteva/method/space/mode/feature_finder.py
--rw-rw-rw-   0        0        0    10157 2023-02-07 02:37:08.000000 meteva-1.8.1/meteva/method/space/mode/feature_match_analyzer.py
--rw-rw-rw-   0        0        0     2456 2022-06-10 12:47:16.000000 meteva-1.8.1/meteva/method/space/mode/feature_props.py
--rw-rw-rw-   0        0        0     5142 2022-06-11 09:04:30.000000 meteva-1.8.1/meteva/method/space/mode/feature_table.py
--rw-rw-rw-   0        0        0    10478 2022-06-30 15:07:24.000000 meteva-1.8.1/meteva/method/space/mode/interester.py
--rw-rw-rw-   0        0        0      748 2022-02-24 23:16:53.000000 meteva-1.8.1/meteva/method/space/mode/intersect.py
--rw-rw-rw-   0        0        0      201 2021-02-04 10:20:28.000000 meteva-1.8.1/meteva/method/space/mode/lengths_psp.py
--rw-rw-rw-   0        0        0     1358 2023-04-23 02:57:31.000000 meteva-1.8.1/meteva/method/space/mode/load.py
--rw-rw-rw-   0        0        0     1365 2021-02-04 10:20:28.000000 meteva-1.8.1/meteva/method/space/mode/loc_list_setup.py
--rw-rw-rw-   0        0        0     3987 2022-02-25 08:35:16.000000 meteva-1.8.1/meteva/method/space/mode/locperf.py
--rw-rw-rw-   0        0        0     7803 2022-02-25 06:16:09.000000 meteva-1.8.1/meteva/method/space/mode/make_SpatialVx_bak.py
--rw-rw-rw-   0        0        0     7943 2022-02-24 23:16:53.000000 meteva-1.8.1/meteva/method/space/mode/make_spatialVx.py
--rw-rw-rw-   0        0        0    11321 2022-06-30 15:12:30.000000 meteva-1.8.1/meteva/method/space/mode/merge_force.py
--rw-rw-rw-   0        0        0      203 2022-02-24 23:16:53.000000 meteva-1.8.1/meteva/method/space/mode/midpoints_psp.py
--rw-rw-rw-   0        0        0    18185 2022-02-24 23:16:53.000000 meteva-1.8.1/meteva/method/space/mode/minboundmatch.py
--rw-rw-rw-   0        0        0     5727 2023-02-07 02:37:07.000000 meteva-1.8.1/meteva/method/space/mode/operater.py
--rw-rw-rw-   0        0        0    32345 2023-08-01 13:36:13.000000 meteva-1.8.1/meteva/method/space/mode/plot.py
--rw-rw-rw-   0        0        0     7757 2022-02-27 12:41:23.000000 meteva-1.8.1/meteva/method/space/mode/regress2.py
--rw-rw-rw-   0        0        0     2226 2022-06-10 07:15:34.000000 meteva-1.8.1/meteva/method/space/mode/sma.py
--rw-rw-rw-   0        0        0    10465 2023-07-27 07:47:11.000000 meteva-1.8.1/meteva/method/space/mode/tran_to_dataframe.py
--rw-rw-rw-   0        0        0      519 2021-02-04 10:20:28.000000 meteva-1.8.1/meteva/method/space/mode/utils.py
--rw-rw-rw-   0        0        0     4595 2023-03-20 12:31:25.000000 meteva-1.8.1/meteva/method/space/point_to_area.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.228636 meteva-1.8.1/meteva/method/space/pphindcast/
--rw-rw-rw-   0        0        0      134 2023-10-01 08:21:38.000000 meteva-1.8.1/meteva/method/space/pphindcast/__init__.py
--rw-rw-rw-   0        0        0     6295 2023-05-12 01:24:44.000000 meteva-1.8.1/meteva/method/space/pphindcast/kernel2dmeitsjer.py
--rw-rw-rw-   0        0        0     2976 2023-08-22 02:29:43.000000 meteva-1.8.1/meteva/method/space/pphindcast/kernel2dsmooth.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.247663 meteva-1.8.1/meteva/method/space/pphindcast/lib/
--rw-rw-rw-   0        0        0      272 2023-10-01 08:21:38.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/__init__.py
--rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/as_unitname.py
--rw-rw-rw-   0        0        0       86 2021-09-05 14:49:53.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/datagrabber.py
--rw-rw-rw-   0        0        0     1081 2021-10-24 16:33:14.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/hoods2dPrep.py
--rw-rw-rw-   0        0        0     2512 2023-08-22 00:21:36.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/im.py
--rw-rw-rw-   0        0        0     6295 2023-05-11 14:59:50.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py
--rw-rw-rw-   0        0        0     2963 2023-08-22 00:21:36.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/kernel2dsmooth.py
--rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/make_spatialVx.py
--rw-rw-rw-   0        0        0      719 2023-01-11 13:49:43.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/thresholder.py
--rw-rw-rw-   0        0        0     4704 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/pphindcast/lib/vxstats.py
--rw-rw-rw-   0        0        0     6087 2023-09-24 15:02:06.000000 meteva-1.8.1/meteva/method/space/pphindcast/pphindcast2d.py
--rw-rw-rw-   0        0        0      275 2023-05-12 01:24:46.000000 meteva-1.8.1/meteva/method/space/pphindcast/zapsmall.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.260637 meteva-1.8.1/meteva/method/space/rigider/
--rw-rw-rw-   0        0        0      394 2021-11-01 03:34:12.000000 meteva-1.8.1/meteva/method/space/rigider/__init__.py
--rw-rw-rw-   0        0        0    10874 2021-11-02 02:23:51.000000 meteva-1.8.1/meteva/method/space/rigider/fint2d.py
--rw-rw-rw-   0        0        0     8093 2021-10-29 08:05:10.000000 meteva-1.8.1/meteva/method/space/rigider/fint2d_old.py
--rw-rw-rw-   0        0        0     1114 2021-10-28 01:37:41.000000 meteva-1.8.1/meteva/method/space/rigider/imomenter.py
--rw-rw-rw-   0        0        0      431 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/rigider/mij.py
--rw-rw-rw-   0        0        0      191 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/rigider/q_loss_rigid.py
--rw-rw-rw-   0        0        0      465 2021-11-01 13:32:37.000000 meteva-1.8.1/meteva/method/space/rigider/rigid_transform.py
--rw-rw-rw-   0        0        0    14406 2024-02-21 13:04:04.000000 meteva-1.8.1/meteva/method/space/rigider/rigider.py
--rw-rw-rw-   0        0        0      275 2021-10-24 18:01:18.000000 meteva-1.8.1/meteva/method/space/rigider/zapsmall.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.263637 meteva-1.8.1/meteva/method/space/s1/
--rw-rw-rw-   0        0        0     2234 2023-09-25 04:01:56.000000 meteva-1.8.1/meteva/method/space/s1/S1.py
--rw-rw-rw-   0        0        0       16 2023-10-01 09:00:39.000000 meteva-1.8.1/meteva/method/space/s1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.266644 meteva-1.8.1/meteva/method/space/saller/
--rw-rw-rw-   0        0        0      329 2021-04-17 00:33:40.000000 meteva-1.8.1/meteva/method/space/saller/__init__.py
--rw-rw-rw-   0        0        0     5904 2022-07-27 01:17:46.000000 meteva-1.8.1/meteva/method/space/saller/saller.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.280636 meteva-1.8.1/meteva/method/space/significance/
--rw-rw-rw-   0        0        0     4074 2022-11-08 08:43:59.000000 meteva-1.8.1/meteva/method/space/significance/LocSig.py
--rw-rw-rw-   0        0        0      214 2022-11-24 08:03:54.000000 meteva-1.8.1/meteva/method/space/significance/__init__.py
--rw-rw-rw-   0        0        0     3646 2022-11-03 07:56:35.000000 meteva-1.8.1/meteva/method/space/significance/bootstrap.py
--rw-rw-rw-   0        0        0     1670 2022-11-03 08:11:48.000000 meteva-1.8.1/meteva/method/space/significance/bootstrap_ci.py
--rw-rw-rw-   0        0        0     4023 2022-11-20 14:11:12.000000 meteva-1.8.1/meteva/method/space/significance/is_sig.py
--rw-rw-rw-   0        0        0      854 2022-11-20 14:11:12.000000 meteva-1.8.1/meteva/method/space/significance/sig_coverage.py
--rw-rw-rw-   0        0        0    13422 2022-11-25 08:07:10.000000 meteva-1.8.1/meteva/method/space/significance/significance.py
--rw-rw-rw-   0        0        0     2506 2022-11-20 14:16:05.000000 meteva-1.8.1/meteva/method/space/significance/spatbiasFS.py
--rw-rw-rw-   0        0        0     1748 2022-11-03 08:16:02.000000 meteva-1.8.1/meteva/method/space/significance/tsboot.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.282635 meteva-1.8.1/meteva/method/space/uqi/
--rw-rw-rw-   0        0        0       20 2023-09-22 07:51:37.000000 meteva-1.8.1/meteva/method/space/uqi/__init__.py
--rw-rw-rw-   0        0        0      989 2023-09-22 08:31:14.000000 meteva-1.8.1/meteva/method/space/uqi/uqi.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.288635 meteva-1.8.1/meteva/method/space/vgm/
--rw-rw-rw-   0        0        0      167 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/method/space/vgm/__init__.py
--rw-rw-rw-   0        0        0     1692 2022-02-27 00:17:20.000000 meteva-1.8.1/meteva/method/space/vgm/rdist.py
--rw-rw-rw-   0        0        0    13416 2022-02-27 00:17:20.000000 meteva-1.8.1/meteva/method/space/vgm/structurogram.py
--rw-rw-rw-   0        0        0     7840 2022-02-27 00:17:20.000000 meteva-1.8.1/meteva/method/space/vgm/structurogram_matrix.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.298635 meteva-1.8.1/meteva/method/weather_system/
--rw-rw-rw-   0        0        0       25 2024-02-22 12:26:37.000000 meteva-1.8.1/meteva/method/weather_system/__init__.py
--rw-rw-rw-   0        0        0    15316 2024-02-11 03:37:27.000000 meteva-1.8.1/meteva/method/weather_system/identify.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.305639 meteva-1.8.1/meteva/method/yes_or_no/
--rw-rw-rw-   0        0        0      850 2023-10-02 14:10:45.000000 meteva-1.8.1/meteva/method/yes_or_no/__init__.py
--rw-rw-rw-   0        0        0    11060 2022-02-27 00:17:20.000000 meteva-1.8.1/meteva/method/yes_or_no/plot.py
--rw-rw-rw-   0        0        0    36054 2023-10-29 14:33:23.000000 meteva-1.8.1/meteva/method/yes_or_no/score.py
--rw-rw-rw-   0        0        0     2995 2023-03-03 07:52:23.000000 meteva-1.8.1/meteva/method/yes_or_no/skill.py
--rw-rw-rw-   0        0        0     7738 2022-04-21 02:55:24.000000 meteva-1.8.1/meteva/method/yes_or_no/table.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.314636 meteva-1.8.1/meteva/perspact/
--rw-rw-rw-   0        0        0      125 2024-02-22 14:20:03.000000 meteva-1.8.1/meteva/perspact/__init__.py
--rw-rw-rw-   0        0        0     7983 2024-03-26 08:35:53.000000 meteva-1.8.1/meteva/perspact/middel_high.py
--rw-rw-rw-   0        0        0    33147 2024-01-27 14:06:47.000000 meteva-1.8.1/meteva/perspact/middle_prepare.py
--rw-rw-rw-   0        0        0    11614 2024-02-23 06:31:38.000000 meteva-1.8.1/meteva/perspact/multi_element_veri.py
--rw-rw-rw-   0        0        0    37870 2024-01-05 07:16:22.000000 meteva-1.8.1/meteva/perspact/score.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.316640 meteva-1.8.1/meteva/product/
--rw-rw-rw-   0        0        0      216 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/product/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.326634 meteva-1.8.1/meteva/product/application/
--rw-rw-rw-   0        0        0      533 2022-02-25 22:41:50.000000 meteva-1.8.1/meteva/product/application/__init__.py
--rw-rw-rw-   0        0        0    10138 2022-05-26 01:55:16.000000 meteva-1.8.1/meteva/product/application/data_collection.py
--rw-rw-rw-   0        0        0     3846 2020-06-10 05:57:46.000000 meteva-1.8.1/meteva/product/application/data_distribute.py
--rw-rw-rw-   0        0        0    24149 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/product/application/data_prepare.py
--rw-rw-rw-   0        0        0     2240 2021-09-20 08:13:53.000000 meteva-1.8.1/meteva/product/application/fun.py
--rw-rw-rw-   0        0        0     2951 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/product/application/terrain_height_correction.py
--rw-rw-rw-   0        0        0     9895 2020-03-04 02:07:44.000000 meteva-1.8.1/meteva/product/application/time_compare.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.328634 meteva-1.8.1/meteva/product/presentation/
--rw-rw-rw-   0        0        0        0 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/product/presentation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.351681 meteva-1.8.1/meteva/product/program/
--rw-rw-rw-   0        0        0     1247 2023-07-07 02:14:59.000000 meteva-1.8.1/meteva/product/program/__init__.py
--rw-rw-rw-   0        0        0    19079 2023-01-13 06:11:18.000000 meteva-1.8.1/meteva/product/program/diurnal.py
--rw-rw-rw-   0        0        0    17966 2023-05-25 06:33:55.000000 meteva-1.8.1/meteva/product/program/error_ana_list.py
--rw-rw-rw-   0        0        0     5761 2022-02-27 12:41:23.000000 meteva-1.8.1/meteva/product/program/error_ana_scatter.py
--rw-rw-rw-   0        0        0    30270 2023-11-16 01:25:36.000000 meteva-1.8.1/meteva/product/program/fun.py
--rw-rw-rw-   0        0        0     6702 2023-10-31 00:43:33.000000 meteva-1.8.1/meteva/product/program/plot.py
--rw-rw-rw-   0        0        0    10578 2023-11-27 13:37:54.000000 meteva-1.8.1/meteva/product/program/process_compare.py
--rw-rw-rw-   0        0        0      971 2022-06-07 02:04:19.000000 meteva-1.8.1/meteva/product/program/sample_statistic.py
--rw-rw-rw-   0        0        0    40965 2023-12-26 03:32:01.000000 meteva-1.8.1/meteva/product/program/score.py
--rw-rw-rw-   0        0        0   148120 2024-02-20 02:32:36.000000 meteva-1.8.1/meteva/product/program/space_compare.py
--rw-rw-rw-   0        0        0     1960 2020-09-27 01:08:16.000000 meteva-1.8.1/meteva/product/program/table.py
--rw-rw-rw-   0        0        0    63209 2023-11-16 01:27:22.000000 meteva-1.8.1/meteva/product/program/time_compare.py
--rw-rw-rw-   0        0        0     5564 2022-07-11 14:46:12.000000 meteva-1.8.1/meteva/product/program/time_space_compare.py
--rw-rw-rw-   0        0        0     2407 2024-01-17 14:09:44.000000 meteva-1.8.1/meteva/product/program/typhoon.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.358635 meteva-1.8.1/meteva/product/regulation/
--rw-rw-rw-   0        0        0      206 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/product/regulation/__init__.py
--rw-rw-rw-   0        0        0     8570 2022-05-20 03:12:02.000000 meteva-1.8.1/meteva/product/regulation/environment.py
--rw-rw-rw-   0        0        0     7069 2020-12-26 09:01:13.000000 meteva-1.8.1/meteva/product/regulation/short_term_heavy_rainfall.py
--rw-rw-rw-   0        0        0     3011 2022-08-11 07:10:19.000000 meteva-1.8.1/meteva/product/regulation/temperature.py
--rw-rw-rw-   0        0        0    16261 2023-05-30 01:00:40.000000 meteva-1.8.1/meteva/product/regulation/thunderstrom_gale.py
-drwxrwxrwx   0        0        0        0 2024-03-26 08:46:55.360635 meteva-1.8.1/meteva.egg-info/
--rw-rw-rw-   0        0        0      940 2024-03-26 08:46:54.000000 meteva-1.8.1/meteva.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11718 2024-03-26 08:46:54.000000 meteva-1.8.1/meteva.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 08:46:54.000000 meteva-1.8.1/meteva.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2024-03-26 08:46:54.000000 meteva-1.8.1/meteva.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-26 08:46:54.000000 meteva-1.8.1/meteva.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 08:46:55.363635 meteva-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2341 2024-03-26 01:59:36.000000 meteva-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:42.062904 meteva-1.8.2/
+-rw-rw-rw-   0        0        0      940 2024-04-04 16:14:42.061968 meteva-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2024-02-23 15:27:40.000000 meteva-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:38.851526 meteva-1.8.2/meteva/
+-rw-rw-rw-   0        0        0      254 2024-04-04 16:14:04.000000 meteva-1.8.2/meteva/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:38.863528 meteva-1.8.2/meteva/base/
+-rw-rw-rw-   0        0        0      174 2020-03-12 03:56:51.000000 meteva-1.8.2/meteva/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:38.947085 meteva-1.8.2/meteva/base/basicdata/
+-rw-rw-rw-   0        0        0      143 2021-04-20 14:24:26.000000 meteva-1.8.2/meteva/base/basicdata/__init__.py
+-rw-rw-rw-   0        0        0     1266 2023-11-13 02:13:55.000000 meteva-1.8.2/meteva/base/basicdata/const.py
+-rw-rw-rw-   0        0        0     7386 2023-07-03 13:42:46.000000 meteva-1.8.2/meteva/base/basicdata/ctl.py
+-rw-rw-rw-   0        0        0    19260 2023-04-21 03:19:11.000000 meteva-1.8.2/meteva/base/basicdata/dicts.py
+-rw-rw-rw-   0        0        0    11165 2022-12-20 01:27:25.000000 meteva-1.8.2/meteva/base/basicdata/grid.py
+-rw-rw-rw-   0        0        0    32686 2024-03-05 12:30:49.000000 meteva-1.8.2/meteva/base/basicdata/grid_data.py
+-rw-rw-rw-   0        0        0      669 2020-03-20 01:16:06.000000 meteva-1.8.2/meteva/base/basicdata/keys.py
+-rw-rw-rw-   0        0        0     7163 2022-09-17 14:18:55.000000 meteva-1.8.2/meteva/base/basicdata/sta_data.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.214771 meteva-1.8.2/meteva/base/fun/
+-rw-rw-rw-   0        0        0      532 2022-05-08 03:56:06.000000 meteva-1.8.2/meteva/base/fun/__init__.py
+-rw-rw-rw-   0        0        0    30617 2024-02-12 23:48:02.000000 meteva-1.8.2/meteva/base/fun/combining.py
+-rw-rw-rw-   0        0        0    28007 2024-01-07 04:30:26.000000 meteva-1.8.2/meteva/base/fun/computing.py
+-rw-rw-rw-   0        0        0    18705 2024-03-04 12:58:48.000000 meteva-1.8.2/meteva/base/fun/diagnosing.py
+-rw-rw-rw-   0        0        0    35296 2024-02-21 15:22:08.000000 meteva-1.8.2/meteva/base/fun/grouping.py
+-rw-rw-rw-   0        0        0    34810 2024-02-28 06:31:06.000000 meteva-1.8.2/meteva/base/fun/interpolating.py
+-rw-rw-rw-   0        0        0    14417 2023-04-23 14:30:42.000000 meteva-1.8.2/meteva/base/fun/nearing.py
+-rw-rw-rw-   0        0        0    56419 2024-04-03 00:23:48.000000 meteva-1.8.2/meteva/base/fun/selecting.py
+-rw-rw-rw-   0        0        0    36232 2023-08-31 06:14:58.000000 meteva-1.8.2/meteva/base/fun/statisticing.py
+-rw-rw-rw-   0        0        0    10676 2022-08-09 06:51:25.000000 meteva-1.8.2/meteva/base/fun/timing.py
+-rw-rw-rw-   0        0        0     7042 2023-04-23 13:10:39.000000 meteva-1.8.2/meteva/base/fun/transformating.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.600834 meteva-1.8.2/meteva/base/io/
+-rw-rw-rw-   0        0        0    21310 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/base/io/CMADaasAccess.py
+-rw-rw-rw-   0        0        0    13513 2020-03-04 02:07:45.000000 meteva-1.8.2/meteva/base/io/DataBlock_pb2.py
+-rw-rw-rw-   0        0        0     1085 2020-03-04 02:07:45.000000 meteva-1.8.2/meteva/base/io/GDS_data_service.py
+-rw-rw-rw-   0        0        0     1288 2020-11-12 11:24:12.000000 meteva-1.8.2/meteva/base/io/SignGenUtil.py
+-rw-rw-rw-   0        0        0      471 2022-08-08 08:44:26.000000 meteva-1.8.2/meteva/base/io/__init__.py
+-rw-rw-rw-   0        0        0     2987 2020-09-15 02:05:05.000000 meteva-1.8.2/meteva/base/io/clienthandler.py
+-rw-rw-rw-   0        0        0     1649 2020-07-06 02:31:29.000000 meteva-1.8.2/meteva/base/io/encoding.py
+-rw-rw-rw-   0        0        0    16712 2021-02-15 14:14:53.000000 meteva-1.8.2/meteva/base/io/ftpconn.py
+-rw-rw-rw-   0        0        0     1749 2021-04-29 03:15:02.000000 meteva-1.8.2/meteva/base/io/httpclient.py
+-rw-rw-rw-   0        0        0     7967 2021-02-15 14:14:53.000000 meteva-1.8.2/meteva/base/io/httpconn.py
+-rw-rw-rw-   0        0        0     4709 2021-02-15 14:14:53.000000 meteva-1.8.2/meteva/base/io/loglib.py
+-rw-rw-rw-   0        0        0     6048 2022-08-12 07:45:29.000000 meteva-1.8.2/meteva/base/io/print_grib_info.py
+-rw-rw-rw-   0        0        0    21031 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/base/io/read_graphydata.py
+-rw-rw-rw-   0        0        0    81459 2024-04-02 06:05:14.000000 meteva-1.8.2/meteva/base/io/read_griddata.py
+-rw-rw-rw-   0        0        0    91613 2024-02-29 15:27:44.000000 meteva-1.8.2/meteva/base/io/read_stadata.py
+-rw-rw-rw-   0        0        0     4670 2023-03-02 08:36:03.000000 meteva-1.8.2/meteva/base/io/write_array.py
+-rw-rw-rw-   0        0        0    10893 2024-02-23 08:01:29.000000 meteva-1.8.2/meteva/base/io/write_griddata.py
+-rw-rw-rw-   0        0        0    12830 2023-10-10 05:58:04.000000 meteva-1.8.2/meteva/base/io/write_stadata.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.841901 meteva-1.8.2/meteva/base/tool/
+-rw-rw-rw-   0        0        0     1216 2023-03-01 02:53:13.000000 meteva-1.8.2/meteva/base/tool/__init__.py
+-rw-rw-rw-   0        0        0    54048 2024-02-23 03:35:58.000000 meteva-1.8.2/meteva/base/tool/color_tools.py
+-rw-rw-rw-   0        0        0    13819 2022-02-26 00:32:32.000000 meteva-1.8.2/meteva/base/tool/copy_tools.py
+-rw-rw-rw-   0        0        0     1248 2023-04-04 14:53:16.000000 meteva-1.8.2/meteva/base/tool/frprmn2.py
+-rw-rw-rw-   0        0        0     4695 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/base/tool/grib_tools.py
+-rw-rw-rw-   0        0        0     8797 2023-07-04 02:34:53.000000 meteva-1.8.2/meteva/base/tool/maskout.py
+-rw-rw-rw-   0        0        0    11675 2023-06-20 14:47:49.000000 meteva-1.8.2/meteva/base/tool/math_tools.py
+-rw-rw-rw-   0        0        0    12484 2024-01-18 07:10:32.000000 meteva-1.8.2/meteva/base/tool/path_tools.py
+-rw-rw-rw-   0        0        0   180509 2024-02-23 05:27:55.000000 meteva-1.8.2/meteva/base/tool/plot_tools.py
+-rw-rw-rw-   0        0        0    35597 2024-02-23 03:38:22.000000 meteva-1.8.2/meteva/base/tool/plot_tools_adv.py
+-rw-rw-rw-   0        0        0     4851 2022-02-27 12:00:59.000000 meteva-1.8.2/meteva/base/tool/process_tools.py
+-rw-rw-rw-   0        0        0     3647 2020-09-18 14:05:02.000000 meteva-1.8.2/meteva/base/tool/station_tools.py
+-rw-rw-rw-   0        0        0     5637 2021-09-29 03:54:03.000000 meteva-1.8.2/meteva/base/tool/time_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.851898 meteva-1.8.2/meteva/method/
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.426875 meteva-1.8.2/meteva/method/Vector/
+-rw-rw-rw-   0        0        0      624 2024-02-22 04:04:47.000000 meteva-1.8.2/meteva/method/Vector/__init__.py
+-rw-rw-rw-   0        0        0    33207 2024-02-22 07:27:38.000000 meteva-1.8.2/meteva/method/Vector/plot.py
+-rw-rw-rw-   0        0        0    46040 2022-08-19 06:02:13.000000 meteva-1.8.2/meteva/method/Vector/score.py
+-rw-rw-rw-   0        0        0      387 2023-09-22 07:51:37.000000 meteva-1.8.2/meteva/method/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:39.998948 meteva-1.8.2/meteva/method/continuous/
+-rw-rw-rw-   0        0        0     1128 2024-01-27 14:08:41.000000 meteva-1.8.2/meteva/method/continuous/__init__.py
+-rw-rw-rw-   0        0        0    40762 2024-02-23 01:50:41.000000 meteva-1.8.2/meteva/method/continuous/plot.py
+-rw-rw-rw-   0        0        0    54412 2024-02-22 03:32:35.000000 meteva-1.8.2/meteva/method/continuous/score.py
+-rw-rw-rw-   0        0        0     1248 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/method/continuous/skill.py
+-rw-rw-rw-   0        0        0     5417 2023-12-26 02:41:16.000000 meteva-1.8.2/meteva/method/continuous/table.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.025974 meteva-1.8.2/meteva/method/ensemble/
+-rw-rw-rw-   0        0        0      211 2021-08-16 08:04:20.000000 meteva-1.8.2/meteva/method/ensemble/__init__.py
+-rw-rw-rw-   0        0        0     4412 2022-02-26 23:44:42.000000 meteva-1.8.2/meteva/method/ensemble/plot.py
+-rw-rw-rw-   0        0        0     4630 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/ensemble/score.py
+-rw-rw-rw-   0        0        0        0 2020-03-04 02:07:36.000000 meteva-1.8.2/meteva/method/ensemble/table.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.060950 meteva-1.8.2/meteva/method/multi_category/
+-rw-rw-rw-   0        0        0      602 2024-04-04 15:25:22.000000 meteva-1.8.2/meteva/method/multi_category/__init__.py
+-rw-rw-rw-   0        0        0    15473 2022-11-14 03:23:59.000000 meteva-1.8.2/meteva/method/multi_category/plot.py
+-rw-rw-rw-   0        0        0    27982 2024-04-04 16:02:06.000000 meteva-1.8.2/meteva/method/multi_category/score.py
+-rw-rw-rw-   0        0        0     7803 2022-12-28 08:27:35.000000 meteva-1.8.2/meteva/method/multi_category/table.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.114949 meteva-1.8.2/meteva/method/probability/
+-rw-rw-rw-   0        0        0      308 2022-03-02 14:27:29.000000 meteva-1.8.2/meteva/method/probability/__init__.py
+-rw-rw-rw-   0        0        0    21703 2022-10-23 06:25:47.000000 meteva-1.8.2/meteva/method/probability/plot.py
+-rw-rw-rw-   0        0        0     7341 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/probability/score.py
+-rw-rw-rw-   0        0        0     2628 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/probability/table.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.160003 meteva-1.8.2/meteva/method/space/
+-rw-rw-rw-   0        0        0      802 2024-02-21 07:49:52.000000 meteva-1.8.2/meteva/method/space/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.189005 meteva-1.8.2/meteva/method/space/acc/
+-rw-rw-rw-   0        0        0       82 2023-10-04 03:56:47.000000 meteva-1.8.2/meteva/method/space/acc/__init__.py
+-rw-rw-rw-   0        0        0    10168 2024-03-26 08:45:02.000000 meteva-1.8.2/meteva/method/space/acc/acc.py
+-rw-rw-rw-   0        0        0      747 2023-09-15 14:42:11.000000 meteva-1.8.2/meteva/method/space/acc/acc_climate_pre.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.211004 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/
+-rw-rw-rw-   0        0        0      134 2023-10-01 08:10:28.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.294002 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/
+-rw-rw-rw-   0        0        0      244 2023-10-01 08:15:28.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/__init__.py
+-rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py
+-rw-rw-rw-   0        0        0      774 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0     1560 2024-02-18 07:34:44.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py
+-rw-rw-rw-   0        0        0     4594 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py
+-rw-rw-rw-   0        0        0     2530 2023-08-21 23:56:50.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/im.py
+-rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py
+-rw-rw-rw-   0        0        0     3977 2024-02-18 07:34:44.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py
+-rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py
+-rw-rw-rw-   0        0        0      625 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py
+-rw-rw-rw-   0        0        0     1978 2023-08-22 00:02:02.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py
+-rw-rw-rw-   0        0        0      278 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_prep.py
+-rw-rw-rw-   0        0        0     5528 2023-08-22 00:02:02.000000 meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.307023 meteva-1.8.2/meteva/method/space/cra/
+-rw-rw-rw-   0        0        0       62 2024-02-21 07:47:43.000000 meteva-1.8.2/meteva/method/space/cra/__init__.py
+-rw-rw-rw-   0        0        0     5824 2024-02-21 13:13:05.000000 meteva-1.8.2/meteva/method/space/cra/cra.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.329005 meteva-1.8.2/meteva/method/space/fqi/
+-rw-rw-rw-   0        0        0       65 2023-10-01 08:00:00.000000 meteva-1.8.2/meteva/method/space/fqi/__init__.py
+-rw-rw-rw-   0        0        0     5179 2023-09-23 11:58:12.000000 meteva-1.8.2/meteva/method/space/fqi/fqi.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.388005 meteva-1.8.2/meteva/method/space/fqi/lib/
+-rw-rw-rw-   0        0        0      366 2023-10-01 08:03:25.000000 meteva-1.8.2/meteva/method/space/fqi/lib/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-08-22 02:14:25.000000 meteva-1.8.2/meteva/method/space/fqi/lib/aaft2d.py
+-rw-rw-rw-   0        0        0      658 2023-01-29 06:47:11.000000 meteva-1.8.2/meteva/method/space/fqi/lib/ampstats.py
+-rw-rw-rw-   0        0        0       93 2023-01-24 09:38:13.000000 meteva-1.8.2/meteva/method/space/fqi/lib/cbind.py
+-rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.2/meteva/method/space/fqi/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0      947 2023-04-02 10:16:53.000000 meteva-1.8.2/meteva/method/space/fqi/lib/distfun.py
+-rw-rw-rw-   0        0        0      947 2023-03-26 09:44:16.000000 meteva-1.8.2/meteva/method/space/fqi/lib/fft2d.py
+-rw-rw-rw-   0        0        0     2531 2023-08-22 02:11:26.000000 meteva-1.8.2/meteva/method/space/fqi/lib/im.py
+-rw-rw-rw-   0        0        0     1467 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/fqi/lib/loc_list_setup.py
+-rw-rw-rw-   0        0        0      278 2021-06-01 19:24:10.000000 meteva-1.8.2/meteva/method/space/fqi/lib/locmeasures2d_prep.py
+-rw-rw-rw-   0        0        0     4102 2024-02-18 12:48:31.000000 meteva-1.8.2/meteva/method/space/fqi/lib/locperf.py
+-rw-rw-rw-   0        0        0      262 2023-03-25 10:39:31.000000 meteva-1.8.2/meteva/method/space/fqi/lib/locperfer.py
+-rw-rw-rw-   0        0        0      158 2023-01-28 04:35:01.000000 meteva-1.8.2/meteva/method/space/fqi/lib/mae.py
+-rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.2/meteva/method/space/fqi/lib/solutionset.py
+-rw-rw-rw-   0        0        0     2398 2023-08-22 02:14:05.000000 meteva-1.8.2/meteva/method/space/fqi/lib/surrogater2d.py
+-rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.2/meteva/method/space/fqi/lib/util.py
+-rw-rw-rw-   0        0        0      274 2023-01-26 07:28:17.000000 meteva-1.8.2/meteva/method/space/fqi/lib/zapsmall.py
+-rw-rw-rw-   0        0        0     1008 2023-08-22 02:11:50.000000 meteva-1.8.2/meteva/method/space/fqi/uiqi.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.395002 meteva-1.8.2/meteva/method/space/fss/
+-rw-rw-rw-   0        0        0     1725 2021-11-23 02:49:29.000000 meteva-1.8.2/meteva/method/space/fss/__init__.py
+-rw-rw-rw-   0        0        0     8387 2023-04-22 14:53:18.000000 meteva-1.8.2/meteva/method/space/fss/fss.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.484058 meteva-1.8.2/meteva/method/space/fuzzy_logic/
+-rw-rw-rw-   0        0        0      194 2023-10-01 07:24:57.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-08-21 03:43:04.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/fss.py
+-rw-rw-rw-   0        0        0     2273 2023-09-06 03:36:58.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/fuzzy.py
+-rw-rw-rw-   0        0        0     1806 2023-09-04 07:58:00.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/joint.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.677592 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/
+-rw-rw-rw-   0        0        0      492 2023-10-01 08:15:28.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/__init__.py
+-rw-rw-rw-   0        0        0      783 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0      860 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fss2dfun.py
+-rw-rw-rw-   0        0        0     1908 2023-08-20 08:53:21.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py
+-rw-rw-rw-   0        0        0     7349 2023-09-06 09:36:29.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2d.py
+-rw-rw-rw-   0        0        0     1016 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py
+-rw-rw-rw-   0        0        0     1243 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py
+-rw-rw-rw-   0        0        0     1266 2023-09-04 08:38:48.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py
+-rw-rw-rw-   0        0        0     6283 2023-08-22 01:44:20.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py
+-rw-rw-rw-   0        0        0     3456 2023-09-25 03:11:25.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py
+-rw-rw-rw-   0        0        0     7289 2023-08-20 13:30:27.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py
+-rw-rw-rw-   0        0        0      188 2023-08-20 12:21:58.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/mincvg2dfun.py
+-rw-rw-rw-   0        0        0      183 2023-08-21 03:05:37.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/multicon2dfun.py
+-rw-rw-rw-   0        0        0      536 2023-09-06 03:46:36.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py
+-rw-rw-rw-   0        0        0      715 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder.py
+-rw-rw-rw-   0        0        0      811 2023-08-21 03:06:59.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py
+-rw-rw-rw-   0        0        0     4704 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/vxstats.py
+-rw-rw-rw-   0        0        0      275 2021-06-06 10:14:33.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/zapsmall.py
+-rw-rw-rw-   0        0        0     2255 2023-09-07 06:37:55.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/minimum_coverage.py
+-rw-rw-rw-   0        0        0     2233 2023-09-06 09:01:35.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/multi_event.py
+-rw-rw-rw-   0        0        0     2218 2023-09-06 03:36:58.000000 meteva-1.8.2/meteva/method/space/fuzzy_logic/pragmatic.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.695594 meteva-1.8.2/meteva/method/space/geo_box_plot/
+-rw-rw-rw-   0        0        0     2496 2023-09-25 04:29:49.000000 meteva-1.8.2/meteva/method/space/geo_box_plot/GeoBoxPlot.py
+-rw-rw-rw-   0        0        0       24 2023-10-02 02:14:48.000000 meteva-1.8.2/meteva/method/space/geo_box_plot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.744592 meteva-1.8.2/meteva/method/space/geometric_characterizations/
+-rw-rw-rw-   0        0        0       86 2023-10-01 08:16:08.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/__init__.py
+-rw-rw-rw-   0        0        0     5187 2024-02-18 08:43:27.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/aindex.py
+-rw-rw-rw-   0        0        0     2664 2023-09-24 12:12:06.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/cindex.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.756595 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/
+-rw-rw-rw-   0        0        0       55 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/__init__.py
+-rw-rw-rw-   0        0        0      774 2021-06-23 19:31:41.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py
+-rw-rw-rw-   0        0        0      140 2021-06-22 19:11:40.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/util.py
+-rw-rw-rw-   0        0        0     2934 2023-09-24 11:40:50.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/sindex.py
+-rw-rw-rw-   0        0        0     1859 2023-08-22 00:10:29.000000 meteva-1.8.2/meteva/method/space/geometric_characterizations/spatial_index.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.758594 meteva-1.8.2/meteva/method/space/hausdorff_metric/
+-rw-rw-rw-   0        0        0       43 2023-10-01 08:17:18.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:40.770594 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/
+-rw-rw-rw-   0        0        0      150 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/__init__.py
+-rw-rw-rw-   0        0        0      829 2021-05-23 18:14:16.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/as_unitname.py
+-rw-rw-rw-   0        0        0      947 2023-04-02 10:14:50.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distfun.py
+-rw-rw-rw-   0        0        0     4731 2023-04-02 10:09:41.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distmap.py
+-rw-rw-rw-   0        0        0     2518 2023-08-22 00:16:03.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/im.py
+-rw-rw-rw-   0        0        0     1467 2021-05-23 18:14:16.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py
+-rw-rw-rw-   0        0        0      625 2021-07-04 16:17:42.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/solutionset.py
+-rw-rw-rw-   0        0        0     5361 2024-02-18 09:02:26.000000 meteva-1.8.2/meteva/method/space/hausdorff_metric/locperf.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.163305 meteva-1.8.2/meteva/method/space/mode/
+-rw-rw-rw-   0        0        0     1960 2023-08-24 01:06:15.000000 meteva-1.8.2/meteva/method/space/mode/__init__.py
+-rw-rw-rw-   0        0        0      161 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/angles_psp.py
+-rw-rw-rw-   0        0        0      384 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/as_psp.py
+-rw-rw-rw-   0        0        0      910 2021-03-10 13:04:02.000000 meteva-1.8.2/meteva/method/space/mode/bearing.py
+-rw-rw-rw-   0        0        0     4059 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/censqdelta.py
+-rw-rw-rw-   0        0        0    11638 2022-05-30 12:33:28.000000 meteva-1.8.2/meteva/method/space/mode/centmatch.py
+-rw-rw-rw-   0        0        0    13874 2023-12-22 00:57:57.000000 meteva-1.8.2/meteva/method/space/mode/consistent.py
+-rw-rw-rw-   0        0        0     3537 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/data_pre.py
+-rw-rw-rw-   0        0        0     1497 2022-02-25 08:34:50.000000 meteva-1.8.2/meteva/method/space/mode/deltametric.py
+-rw-rw-rw-   0        0        0     3541 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/deltamm.py
+-rw-rw-rw-   0        0        0    18089 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/deltammSqCen.py
+-rw-rw-rw-   0        0        0     3530 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/deltamm_bak.py
+-rw-rw-rw-   0        0        0     4801 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/distmap.py
+-rw-rw-rw-   0        0        0     6070 2024-02-22 03:58:40.000000 meteva-1.8.2/meteva/method/space/mode/feature_axis.py
+-rw-rw-rw-   0        0        0     4087 2022-06-24 14:09:57.000000 meteva-1.8.2/meteva/method/space/mode/feature_comps.py
+-rw-rw-rw-   0        0        0    32379 2023-08-22 14:03:20.000000 meteva-1.8.2/meteva/method/space/mode/feature_finder.py
+-rw-rw-rw-   0        0        0    10157 2023-02-07 02:37:08.000000 meteva-1.8.2/meteva/method/space/mode/feature_match_analyzer.py
+-rw-rw-rw-   0        0        0     2456 2022-06-10 12:47:16.000000 meteva-1.8.2/meteva/method/space/mode/feature_props.py
+-rw-rw-rw-   0        0        0     5142 2022-06-11 09:04:30.000000 meteva-1.8.2/meteva/method/space/mode/feature_table.py
+-rw-rw-rw-   0        0        0    10478 2022-06-30 15:07:24.000000 meteva-1.8.2/meteva/method/space/mode/interester.py
+-rw-rw-rw-   0        0        0      748 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/intersect.py
+-rw-rw-rw-   0        0        0      201 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/lengths_psp.py
+-rw-rw-rw-   0        0        0     1358 2023-04-23 02:57:31.000000 meteva-1.8.2/meteva/method/space/mode/load.py
+-rw-rw-rw-   0        0        0     1365 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/loc_list_setup.py
+-rw-rw-rw-   0        0        0     3987 2022-02-25 08:35:16.000000 meteva-1.8.2/meteva/method/space/mode/locperf.py
+-rw-rw-rw-   0        0        0     7803 2022-02-25 06:16:09.000000 meteva-1.8.2/meteva/method/space/mode/make_SpatialVx_bak.py
+-rw-rw-rw-   0        0        0     7943 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/make_spatialVx.py
+-rw-rw-rw-   0        0        0    11321 2022-06-30 15:12:30.000000 meteva-1.8.2/meteva/method/space/mode/merge_force.py
+-rw-rw-rw-   0        0        0      203 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/midpoints_psp.py
+-rw-rw-rw-   0        0        0    18185 2022-02-24 23:16:53.000000 meteva-1.8.2/meteva/method/space/mode/minboundmatch.py
+-rw-rw-rw-   0        0        0     5727 2023-02-07 02:37:07.000000 meteva-1.8.2/meteva/method/space/mode/operater.py
+-rw-rw-rw-   0        0        0    32345 2023-08-01 13:36:13.000000 meteva-1.8.2/meteva/method/space/mode/plot.py
+-rw-rw-rw-   0        0        0     7757 2022-02-27 12:41:23.000000 meteva-1.8.2/meteva/method/space/mode/regress2.py
+-rw-rw-rw-   0        0        0     2226 2022-06-10 07:15:34.000000 meteva-1.8.2/meteva/method/space/mode/sma.py
+-rw-rw-rw-   0        0        0    10465 2023-07-27 07:47:11.000000 meteva-1.8.2/meteva/method/space/mode/tran_to_dataframe.py
+-rw-rw-rw-   0        0        0      519 2021-02-04 10:20:28.000000 meteva-1.8.2/meteva/method/space/mode/utils.py
+-rw-rw-rw-   0        0        0     4595 2023-03-20 12:31:25.000000 meteva-1.8.2/meteva/method/space/point_to_area.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.184306 meteva-1.8.2/meteva/method/space/pphindcast/
+-rw-rw-rw-   0        0        0      134 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/pphindcast/__init__.py
+-rw-rw-rw-   0        0        0     6295 2023-05-12 01:24:44.000000 meteva-1.8.2/meteva/method/space/pphindcast/kernel2dmeitsjer.py
+-rw-rw-rw-   0        0        0     2976 2023-08-22 02:29:43.000000 meteva-1.8.2/meteva/method/space/pphindcast/kernel2dsmooth.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.201306 meteva-1.8.2/meteva/method/space/pphindcast/lib/
+-rw-rw-rw-   0        0        0      272 2023-10-01 08:21:38.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/__init__.py
+-rw-rw-rw-   0        0        0      829 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/as_unitname.py
+-rw-rw-rw-   0        0        0       86 2021-09-05 14:49:53.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/datagrabber.py
+-rw-rw-rw-   0        0        0     1081 2021-10-24 16:33:14.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/hoods2dPrep.py
+-rw-rw-rw-   0        0        0     2512 2023-08-22 00:21:36.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/im.py
+-rw-rw-rw-   0        0        0     6295 2023-05-11 14:59:50.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py
+-rw-rw-rw-   0        0        0     2963 2023-08-22 00:21:36.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dsmooth.py
+-rw-rw-rw-   0        0        0     7157 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/make_spatialVx.py
+-rw-rw-rw-   0        0        0      719 2023-01-11 13:49:43.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/thresholder.py
+-rw-rw-rw-   0        0        0     4704 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/pphindcast/lib/vxstats.py
+-rw-rw-rw-   0        0        0     6087 2023-09-24 15:02:06.000000 meteva-1.8.2/meteva/method/space/pphindcast/pphindcast2d.py
+-rw-rw-rw-   0        0        0      275 2023-05-12 01:24:46.000000 meteva-1.8.2/meteva/method/space/pphindcast/zapsmall.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.266307 meteva-1.8.2/meteva/method/space/rigider/
+-rw-rw-rw-   0        0        0      394 2021-11-01 03:34:12.000000 meteva-1.8.2/meteva/method/space/rigider/__init__.py
+-rw-rw-rw-   0        0        0    10874 2021-11-02 02:23:51.000000 meteva-1.8.2/meteva/method/space/rigider/fint2d.py
+-rw-rw-rw-   0        0        0     8093 2021-10-29 08:05:10.000000 meteva-1.8.2/meteva/method/space/rigider/fint2d_old.py
+-rw-rw-rw-   0        0        0     1114 2021-10-28 01:37:41.000000 meteva-1.8.2/meteva/method/space/rigider/imomenter.py
+-rw-rw-rw-   0        0        0      431 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/rigider/mij.py
+-rw-rw-rw-   0        0        0      191 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/rigider/q_loss_rigid.py
+-rw-rw-rw-   0        0        0      465 2021-11-01 13:32:37.000000 meteva-1.8.2/meteva/method/space/rigider/rigid_transform.py
+-rw-rw-rw-   0        0        0    14406 2024-02-21 13:04:04.000000 meteva-1.8.2/meteva/method/space/rigider/rigider.py
+-rw-rw-rw-   0        0        0      275 2021-10-24 18:01:18.000000 meteva-1.8.2/meteva/method/space/rigider/zapsmall.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.283307 meteva-1.8.2/meteva/method/space/s1/
+-rw-rw-rw-   0        0        0     2234 2023-09-25 04:01:56.000000 meteva-1.8.2/meteva/method/space/s1/S1.py
+-rw-rw-rw-   0        0        0       16 2023-10-01 09:00:39.000000 meteva-1.8.2/meteva/method/space/s1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.299306 meteva-1.8.2/meteva/method/space/saller/
+-rw-rw-rw-   0        0        0      329 2021-04-17 00:33:40.000000 meteva-1.8.2/meteva/method/space/saller/__init__.py
+-rw-rw-rw-   0        0        0     5904 2022-07-27 01:17:46.000000 meteva-1.8.2/meteva/method/space/saller/saller.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.362821 meteva-1.8.2/meteva/method/space/significance/
+-rw-rw-rw-   0        0        0     4074 2022-11-08 08:43:59.000000 meteva-1.8.2/meteva/method/space/significance/LocSig.py
+-rw-rw-rw-   0        0        0      214 2022-11-24 08:03:54.000000 meteva-1.8.2/meteva/method/space/significance/__init__.py
+-rw-rw-rw-   0        0        0     3646 2022-11-03 07:56:35.000000 meteva-1.8.2/meteva/method/space/significance/bootstrap.py
+-rw-rw-rw-   0        0        0     1670 2022-11-03 08:11:48.000000 meteva-1.8.2/meteva/method/space/significance/bootstrap_ci.py
+-rw-rw-rw-   0        0        0     4023 2022-11-20 14:11:12.000000 meteva-1.8.2/meteva/method/space/significance/is_sig.py
+-rw-rw-rw-   0        0        0      854 2022-11-20 14:11:12.000000 meteva-1.8.2/meteva/method/space/significance/sig_coverage.py
+-rw-rw-rw-   0        0        0    13422 2022-11-25 08:07:10.000000 meteva-1.8.2/meteva/method/space/significance/significance.py
+-rw-rw-rw-   0        0        0     2506 2022-11-20 14:16:05.000000 meteva-1.8.2/meteva/method/space/significance/spatbiasFS.py
+-rw-rw-rw-   0        0        0     1748 2022-11-03 08:16:02.000000 meteva-1.8.2/meteva/method/space/significance/tsboot.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.365824 meteva-1.8.2/meteva/method/space/uqi/
+-rw-rw-rw-   0        0        0       20 2023-09-22 07:51:37.000000 meteva-1.8.2/meteva/method/space/uqi/__init__.py
+-rw-rw-rw-   0        0        0      989 2023-09-22 08:31:14.000000 meteva-1.8.2/meteva/method/space/uqi/uqi.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.422875 meteva-1.8.2/meteva/method/space/vgm/
+-rw-rw-rw-   0        0        0      167 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/method/space/vgm/__init__.py
+-rw-rw-rw-   0        0        0     1692 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/space/vgm/rdist.py
+-rw-rw-rw-   0        0        0    13416 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/space/vgm/structurogram.py
+-rw-rw-rw-   0        0        0     7840 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/space/vgm/structurogram_matrix.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.453941 meteva-1.8.2/meteva/method/weather_system/
+-rw-rw-rw-   0        0        0       25 2024-02-22 12:26:37.000000 meteva-1.8.2/meteva/method/weather_system/__init__.py
+-rw-rw-rw-   0        0        0    15316 2024-02-11 03:37:27.000000 meteva-1.8.2/meteva/method/weather_system/identify.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.544874 meteva-1.8.2/meteva/method/yes_or_no/
+-rw-rw-rw-   0        0        0      850 2023-10-02 14:10:45.000000 meteva-1.8.2/meteva/method/yes_or_no/__init__.py
+-rw-rw-rw-   0        0        0    11060 2022-02-27 00:17:20.000000 meteva-1.8.2/meteva/method/yes_or_no/plot.py
+-rw-rw-rw-   0        0        0    36054 2023-10-29 14:33:23.000000 meteva-1.8.2/meteva/method/yes_or_no/score.py
+-rw-rw-rw-   0        0        0     2995 2023-03-03 07:52:23.000000 meteva-1.8.2/meteva/method/yes_or_no/skill.py
+-rw-rw-rw-   0        0        0     7738 2022-04-21 02:55:24.000000 meteva-1.8.2/meteva/method/yes_or_no/table.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.635591 meteva-1.8.2/meteva/perspact/
+-rw-rw-rw-   0        0        0      167 2024-03-27 01:02:36.000000 meteva-1.8.2/meteva/perspact/__init__.py
+-rw-rw-rw-   0        0        0     8873 2024-04-04 14:21:50.000000 meteva-1.8.2/meteva/perspact/middel_high.py
+-rw-rw-rw-   0        0        0    33147 2024-01-27 14:06:47.000000 meteva-1.8.2/meteva/perspact/middle_prepare.py
+-rw-rw-rw-   0        0        0    11614 2024-02-23 06:31:38.000000 meteva-1.8.2/meteva/perspact/multi_element_veri.py
+-rw-rw-rw-   0        0        0    37870 2024-01-05 07:16:22.000000 meteva-1.8.2/meteva/perspact/score.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.654839 meteva-1.8.2/meteva/product/
+-rw-rw-rw-   0        0        0      216 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.757839 meteva-1.8.2/meteva/product/application/
+-rw-rw-rw-   0        0        0      533 2022-02-25 22:41:50.000000 meteva-1.8.2/meteva/product/application/__init__.py
+-rw-rw-rw-   0        0        0    10138 2022-05-26 01:55:16.000000 meteva-1.8.2/meteva/product/application/data_collection.py
+-rw-rw-rw-   0        0        0     3846 2020-06-10 05:57:46.000000 meteva-1.8.2/meteva/product/application/data_distribute.py
+-rw-rw-rw-   0        0        0    24149 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/application/data_prepare.py
+-rw-rw-rw-   0        0        0     2240 2021-09-20 08:13:53.000000 meteva-1.8.2/meteva/product/application/fun.py
+-rw-rw-rw-   0        0        0     2951 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/application/terrain_height_correction.py
+-rw-rw-rw-   0        0        0     9895 2020-03-04 02:07:44.000000 meteva-1.8.2/meteva/product/application/time_compare.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.759863 meteva-1.8.2/meteva/product/presentation/
+-rw-rw-rw-   0        0        0        0 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/presentation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:41.973903 meteva-1.8.2/meteva/product/program/
+-rw-rw-rw-   0        0        0     1247 2023-07-07 02:14:59.000000 meteva-1.8.2/meteva/product/program/__init__.py
+-rw-rw-rw-   0        0        0    19079 2023-01-13 06:11:18.000000 meteva-1.8.2/meteva/product/program/diurnal.py
+-rw-rw-rw-   0        0        0    17966 2023-05-25 06:33:55.000000 meteva-1.8.2/meteva/product/program/error_ana_list.py
+-rw-rw-rw-   0        0        0     5761 2022-02-27 12:41:23.000000 meteva-1.8.2/meteva/product/program/error_ana_scatter.py
+-rw-rw-rw-   0        0        0    30270 2023-11-16 01:25:36.000000 meteva-1.8.2/meteva/product/program/fun.py
+-rw-rw-rw-   0        0        0     6702 2023-10-31 00:43:33.000000 meteva-1.8.2/meteva/product/program/plot.py
+-rw-rw-rw-   0        0        0    10578 2023-11-27 13:37:54.000000 meteva-1.8.2/meteva/product/program/process_compare.py
+-rw-rw-rw-   0        0        0      971 2022-06-07 02:04:19.000000 meteva-1.8.2/meteva/product/program/sample_statistic.py
+-rw-rw-rw-   0        0        0    40965 2023-12-26 03:32:01.000000 meteva-1.8.2/meteva/product/program/score.py
+-rw-rw-rw-   0        0        0   148120 2024-02-20 02:32:36.000000 meteva-1.8.2/meteva/product/program/space_compare.py
+-rw-rw-rw-   0        0        0     1960 2020-09-27 01:08:16.000000 meteva-1.8.2/meteva/product/program/table.py
+-rw-rw-rw-   0        0        0    63209 2023-11-16 01:27:22.000000 meteva-1.8.2/meteva/product/program/time_compare.py
+-rw-rw-rw-   0        0        0     5564 2022-07-11 14:46:12.000000 meteva-1.8.2/meteva/product/program/time_space_compare.py
+-rw-rw-rw-   0        0        0     2407 2024-01-17 14:09:44.000000 meteva-1.8.2/meteva/product/program/typhoon.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:42.038905 meteva-1.8.2/meteva/product/regulation/
+-rw-rw-rw-   0        0        0      206 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/regulation/__init__.py
+-rw-rw-rw-   0        0        0     8570 2022-05-20 03:12:02.000000 meteva-1.8.2/meteva/product/regulation/environment.py
+-rw-rw-rw-   0        0        0     7069 2020-12-26 09:01:13.000000 meteva-1.8.2/meteva/product/regulation/short_term_heavy_rainfall.py
+-rw-rw-rw-   0        0        0     3011 2022-08-11 07:10:19.000000 meteva-1.8.2/meteva/product/regulation/temperature.py
+-rw-rw-rw-   0        0        0    16261 2023-05-30 01:00:40.000000 meteva-1.8.2/meteva/product/regulation/thunderstrom_gale.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:14:42.059904 meteva-1.8.2/meteva.egg-info/
+-rw-rw-rw-   0        0        0      940 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11718 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 16:14:38.000000 meteva-1.8.2/meteva.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 16:14:42.062904 meteva-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     2341 2024-03-26 01:59:36.000000 meteva-1.8.2/setup.py
```

### Comparing `meteva-1.8.1/PKG-INFO` & `meteva-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteva
-Version: 1.8.1
+Version: 1.8.2
 Summary: A collections of functions for meteorological verification.
 Author: liucouhua,daikan,wangbaoli,tangbuxing
 Author-email: liucouhua@163.com
 License: GPL3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meteva-1.8.1/meteva/base/basicdata/const.py` & `meteva-1.8.2/meteva/base/basicdata/const.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/basicdata/ctl.py` & `meteva-1.8.2/meteva/base/basicdata/ctl.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/basicdata/dicts.py` & `meteva-1.8.2/meteva/base/basicdata/dicts.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/basicdata/grid.py` & `meteva-1.8.2/meteva/base/basicdata/grid.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/basicdata/grid_data.py` & `meteva-1.8.2/meteva/base/basicdata/grid_data.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/basicdata/keys.py` & `meteva-1.8.2/meteva/base/basicdata/keys.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/basicdata/sta_data.py` & `meteva-1.8.2/meteva/base/basicdata/sta_data.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/__init__.py` & `meteva-1.8.2/meteva/base/fun/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/combining.py` & `meteva-1.8.2/meteva/base/fun/combining.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/computing.py` & `meteva-1.8.2/meteva/base/fun/computing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/diagnosing.py` & `meteva-1.8.2/meteva/base/fun/diagnosing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/grouping.py` & `meteva-1.8.2/meteva/base/fun/grouping.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/interpolating.py` & `meteva-1.8.2/meteva/base/fun/interpolating.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/nearing.py` & `meteva-1.8.2/meteva/base/fun/nearing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/selecting.py` & `meteva-1.8.2/meteva/base/fun/selecting.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,17 +774,19 @@
     sta1 = sta_with_province_name.loc[sta_with_province_name['province_name'].isin(province_name_list)]
     sta1 = sta1.drop(['province_name'], axis=1)
 
     return sta1
 
 def not_nan(sta):
     danames = meteva.base.get_stadata_names(sta)
-    sta1 = sta.copy()
-    for name in danames:
-        sta1 = sta[pd.notnull(sta1[name])]
+    # sta1 = sta.copy()
+    # for name in danames:
+    #     sta1 = sta[pd.notnull(sta1[name])]
+    sta1 = sta.dropna(subset=danames)
+
     return sta1
 
 #返回站点参数字典列表
 def by_loc_dict(data,s):
     '''
     s 应具备如下样式
     s = {'member':["ecmwf","grapes"],列表形式
```

### Comparing `meteva-1.8.1/meteva/base/fun/statisticing.py` & `meteva-1.8.2/meteva/base/fun/statisticing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/timing.py` & `meteva-1.8.2/meteva/base/fun/timing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/fun/transformating.py` & `meteva-1.8.2/meteva/base/fun/transformating.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/CMADaasAccess.py` & `meteva-1.8.2/meteva/base/io/CMADaasAccess.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/DataBlock_pb2.py` & `meteva-1.8.2/meteva/base/io/DataBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/GDS_data_service.py` & `meteva-1.8.2/meteva/base/io/GDS_data_service.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/SignGenUtil.py` & `meteva-1.8.2/meteva/base/io/SignGenUtil.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/clienthandler.py` & `meteva-1.8.2/meteva/base/io/clienthandler.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/encoding.py` & `meteva-1.8.2/meteva/base/io/encoding.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/ftpconn.py` & `meteva-1.8.2/meteva/base/io/ftpconn.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/httpclient.py` & `meteva-1.8.2/meteva/base/io/httpclient.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/httpconn.py` & `meteva-1.8.2/meteva/base/io/httpconn.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/loglib.py` & `meteva-1.8.2/meteva/base/io/loglib.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/print_grib_info.py` & `meteva-1.8.2/meteva/base/io/print_grib_info.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/read_graphydata.py` & `meteva-1.8.2/meteva/base/io/read_graphydata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/read_griddata.py` & `meteva-1.8.2/meteva/base/io/read_griddata.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,33 +161,40 @@
     """
     if not os.path.exists(filename):
         print(filename+" not exists")
         return
     try:
         ds0 = xr.open_dataset(filename)
 
-        #如果文件中包含多层次多时效数据，通过先选择
-        dict_sel = {}
-        if level is not None:
-            if level_dim is not None:
-                if ds0[level_dim].values.size>1:
-                    dict_sel[level_dim] = level
-            else:
-                if ds0["level"].values.size > 1:
-                    dict_sel["level"] = level
-        if dtime is not None:
-            if dtime_dim is not None:
-                if ds0[dtime_dim].values.size > 1:
-                    dict_sel[dtime_dim] = dtime
-            else:
-                if ds0["dtime"].values.size > 1:
-                    dict_sel["dtime"] = dtime
-        if len(dict_sel.keys())>0 and value_name is not None:
-            ds0 = ds0[value_name]
-            ds0 = ds0.loc[dict_sel]
+        try:
+            #如果文件中包含多层次多时效数据，通过先选择部分时效、层次，提升效率
+            dict_sel = {}
+            if level is not None:
+                if level_dim is not None:
+                    if ds0[level_dim].values.size>1:
+                        dict_sel[level_dim] = level
+                else:
+                    if "level" in ds0.coords:
+                        if ds0["level"].values.size > 1:
+                            dict_sel["level"] = level
+            if dtime is not None:
+                if dtime_dim is not None:
+                    if ds0[dtime_dim].values.size > 1:
+                        dict_sel[dtime_dim] = dtime
+                else:
+                    if "dtime" in ds0.coords:
+                        if ds0["dtime"].values.size > 1:
+                            dict_sel["dtime"] = dtime
+            if len(dict_sel.keys())>0 and value_name is not None:
+                ds0 = ds0[value_name]
+                ds0 = ds0.loc[dict_sel]
+        except:
+            #如果不能提取
+            pass
+
         da1 = meteva.base.xarray_to_griddata(ds0,value_name=value_name,member_dim=member_dim,level_dim=level_dim,time_dim=time_dim,dtime_dim=dtime_dim,
                                              lat_dim=lat_dim,lon_dim=lon_dim)
 
         #如果有level参数
         if level is not None:
             level_list = []
             if isinstance(level, list):
@@ -332,27 +339,83 @@
 def read_griddata_from_grib(filename,level_type= None,grid = None,
             value_name = None,member_dim = None,time_dim = None,dtime_dim = None,lat_dim = None,lon_dim = None,
                          level=None, time=None, dtime=None, data_name="data0",filter_by_keys = {},dtime_units = "hour",outer_value = None,show = False):
     try:
 
         if level_type is not None:filter_by_keys['typeOfLevel'] = level_type
         if "typeOfLevel" in filter_by_keys.keys(): level_type = filter_by_keys['typeOfLevel']
-        if level is not None:
-            filter_by_keys['level'] = level
         ds0 = xr.open_dataset(filename, engine="cfgrib", backend_kwargs={'filter_by_keys': filter_by_keys,"indexpath": ""},)
+        try:
+            #如果文件中包含多层次多时效数据，通过先选择部分时效、层次，提升效率
+            dict_sel = {}
+            if level is not None:
+                if level_type is not None:
+                    if ds0[level_type].values.size>1:
+                        dict_sel[level_type] = level
+                else:
+                    if "level" in ds0.coords:
+                        if ds0["level"].values.size > 1:
+                            dict_sel["level"] = level
+            if dtime is not None:
+                if dtime_dim is not None:
+                    if ds0[dtime_dim].values.size > 1:
+                        dict_sel[dtime_dim] = dtime
+                else:
+                    if "dtime" in ds0.coords:
+                        if ds0["dtime"].values.size > 1:
+                            dict_sel["dtime"] = dtime
+            if len(dict_sel.keys())>0 and value_name is not None:
+                ds0 = ds0[value_name]
+                ds0 = ds0.loc[dict_sel]
+        except:
+            #如果不能提取
+            pass
+
+
         da1 = meteva.base.xarray_to_griddata(ds0,value_name=value_name,member_dim=member_dim,level_dim=level_type,time_dim=time_dim,dtime_dim=dtime_dim,
                                              lat_dim=lat_dim,lon_dim=lon_dim)
         ds0.close()
         meteva.base.reset(da1)
+
+        # 如果有level参数
+        if level is not None:
+            level_list = []
+            if isinstance(level, list):
+                level_list = level
+            elif isinstance(level, np.ndarray):
+                level_list = level.tolist()
+            else:
+                level_list = [level]
+
+            # 如果level参数和数据文件里面正好都是一层，就认为level是用来设置层次参数的
+            if len(da1.coords["level"]) == 1 and len(level_list) == 1:
+                meteva.base.set_griddata_coords(da1, level_list=level_list)
+            else:
+                # 如果level参数和数据文件不都为1层，则认为level是用来提取某些层次数据的
+                da1 = meteva.base.in_level_list(da1, level_list=level_list)
+
+        # 如果有dtime参数
+        if dtime is not None:
+            dtime_list = []
+            if isinstance(dtime, list):
+                dtime_list = dtime
+            elif isinstance(dtime, np.ndarray):
+                dtime_list = dtime.tolist()
+            else:
+                dtime_list = [dtime]
+
+            # 如果level参数和数据文件里面正好都是一个时效，就认为dtime是用来设置时效参数的
+            if len(da1.coords["dtime"]) == 1 and len(dtime_list) == 1:
+                meteva.base.set_griddata_coords(da1, dtime_list=dtime_list)
+            else:
+                # 如果level参数和数据文件不都为1时效，则认为level是用来提取某些时效数据的
+                da1 = meteva.base.in_dtime_list(da1, dtime_list=dtime_list)
+
         if time is not None and len(da1.coords["time"])==1:
             meteva.base.set_griddata_coords(da1,gtime=[time])
-        if dtime is not None and len(da1.coords["dtime"])==1:
-            meteva.base.set_griddata_coords(da1,dtime_list=[dtime])
-        if level is not None and len(da1.coords["level"])==1:
-            meteva.base.set_griddata_coords(da1,level_list=[level])
         if data_name is not None and len(da1.coords["member"])==1:
             meteva.base.set_griddata_coords(da1,member_list=[data_name])
 
         da1.attrs["dtime_units"] = dtime_units
         if grid is None:
             #da1.name = "data0"
             if show:
```

### Comparing `meteva-1.8.1/meteva/base/io/read_stadata.py` & `meteva-1.8.2/meteva/base/io/read_stadata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/write_array.py` & `meteva-1.8.2/meteva/base/io/write_array.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/write_griddata.py` & `meteva-1.8.2/meteva/base/io/write_griddata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/io/write_stadata.py` & `meteva-1.8.2/meteva/base/io/write_stadata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/__init__.py` & `meteva-1.8.2/meteva/base/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/color_tools.py` & `meteva-1.8.2/meteva/base/tool/color_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/copy_tools.py` & `meteva-1.8.2/meteva/base/tool/copy_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/frprmn2.py` & `meteva-1.8.2/meteva/base/tool/frprmn2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/grib_tools.py` & `meteva-1.8.2/meteva/base/tool/grib_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/maskout.py` & `meteva-1.8.2/meteva/base/tool/maskout.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/math_tools.py` & `meteva-1.8.2/meteva/base/tool/math_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/path_tools.py` & `meteva-1.8.2/meteva/base/tool/path_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/plot_tools.py` & `meteva-1.8.2/meteva/base/tool/plot_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/plot_tools_adv.py` & `meteva-1.8.2/meteva/base/tool/plot_tools_adv.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/process_tools.py` & `meteva-1.8.2/meteva/base/tool/process_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/station_tools.py` & `meteva-1.8.2/meteva/base/tool/station_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/base/tool/time_tools.py` & `meteva-1.8.2/meteva/base/tool/time_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/Vector/__init__.py` & `meteva-1.8.2/meteva/method/Vector/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/Vector/plot.py` & `meteva-1.8.2/meteva/method/Vector/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/Vector/score.py` & `meteva-1.8.2/meteva/method/Vector/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/continuous/__init__.py` & `meteva-1.8.2/meteva/method/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/continuous/plot.py` & `meteva-1.8.2/meteva/method/continuous/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/continuous/score.py` & `meteva-1.8.2/meteva/method/continuous/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/continuous/skill.py` & `meteva-1.8.2/meteva/method/continuous/skill.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/continuous/table.py` & `meteva-1.8.2/meteva/method/continuous/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/ensemble/plot.py` & `meteva-1.8.2/meteva/method/ensemble/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/ensemble/score.py` & `meteva-1.8.2/meteva/method/ensemble/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/multi_category/__init__.py` & `meteva-1.8.2/meteva/method/multi_category/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,8 +2,9 @@
 from . import score
 from . import table
 from . import plot
 from .score import hk,hk_tcof,hss,hss_tcof,tc,tcof,accuracy,accuracy_tc,accuracy_tcof,hfmc_multi,ts_multi,ets_multi,bias_multi,far_multi,mr_multi
 from .score import hfmc_grade,ts_grade,ets_grade,bias_grade,far_grade,mr_grade,seeps_ctable,seeps,seeps_skill
 from .score import pod_grade,pofd_grade,sr_grade,pod_multi,pofd_multi,sr_multi
 from .table import contingency_table_multicategory,frequency_table
-from .plot import frequency_histogram,performance_grade,performance_multi
+from .plot import frequency_histogram,performance_grade,performance_multi
+from .score import murphy_score,get_s_array,murphy_ctable
```

### Comparing `meteva-1.8.1/meteva/method/multi_category/plot.py` & `meteva-1.8.2/meteva/method/multi_category/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/multi_category/score.py` & `meteva-1.8.2/meteva/method/multi_category/score.py`

 * *Files 16% similar despite different names*

```diff
@@ -611,8 +611,148 @@
     :param Fo:
     :param p1:
     :param significant_rain_threshold:
     :return:
     '''
     seeps_array = seeps(Ob,Fo,p1= p1,threshold=threshold)
     skill = 1- seeps_array
-    return skill
+    return skill
+
+
+def show_valid_k1_k2(p1,p2,p3):
+    x = np.arange(201)*0.01-1
+    y = np.arange(201)*0.01-1
+    valid_index = np.zeros((201,201))
+    for i in range(201):
+        for j in range(201):
+            k2 = x[i]
+            k1 = y[j]
+
+            s11 = (p3 + p1*(p3-p2) * k1 + p3*(p2+p3)*k2) / (p1 * (p1+p3))
+            s13 = -(1+(p1+p2)*k1 + (p2+p3)*k2)/(p1+p3)
+            s22 = -(p1*k1 + p3 *k2)/p2
+            s33 = (p1+p1*(p1+p2)*k1 + p3*(p1-p2)*k2)/(p3*(p1+p3))
+
+            if (i == 125 and j == 50):
+                print()
+
+            # 非顺序条件
+            if k1 < s11 and k1 < s22 and k2 <s22 and k2 < s33 and s13 < s11 and s13 < s33:
+                valid_index[i,j] = 1
+
+                #顺序条件
+                if s13< k1 and s13 < k2:
+                    valid_index[i, j] += 1
+    print(valid_index)
+    import matplotlib.pyplot as plt
+    plt.pcolormesh(valid_index.T)
+    plt.show()
+
+def get_s_array(p1,p2,p3,k1=-0.25,k2=-0.25):
+    '''
+    根据3分类预报问题的实况气候概率p1,p2和p3， 确定Murphy评分的评分权重矩阵。
+    评分权重的确定原理简单叙述如下：
+    3分类预报的完整检验信息可由一个3×3的列联表表示。列联表中的元素p_ij表示 观测为第i类,预报为第j类的样本数。
+    总的评分等于列联表每个元素×一个权重系数后求和得到 sum(p_ij * s_ij)。 为此需要确定9个评分权重系数。
+    一般来说对角线上的权重系数s_ii 应该是正的，表示奖励， 非对角线上的s_ij是负的表示惩罚。那这9个评分权重该取为多少，
+    用它们做评价才是公平的？ 为此主要考虑2点，一是如果全部报对（列联表的元素全部集中在对角线上），评分应为1，另外，
+    随机预报的评分应该为0，这2个条件可以构成关于权重系数的4个方程构成的方程组，这个方程组中包含3个分类的实况概率p1、p2、p3，
+    构成的已知参数。如果考虑这个评分矩阵是对称的，则一共有6个待定系数，因此它是一个欠定问题。为此有两个评分权重系数必须事先指定，
+    为此令 k1 = s12, k2 = s23， 在此基础上可以计算出其它4个系数 s11,s22,s33,s13.
+    根据Murphy的分析，k1和k2的取值范围为(-0.5,0)时，计算出的评分权重可以满足：
+    s12 < s11,s12<s22, s23<s22,s23<s33, s13<s12,s13<s23。
+    关于上述内容的更详细论述可参考《预报检验-大气科学从业者指南》 4.3.2节
+    :param p1: 实况第1分类的概率
+    :param p2: 实况第2分类的概率
+    :param p3: 实况第3分类的概率
+    :param k1:权重系数s12
+    :param k2:权重系数s23
+    :return: 3×3的权重系数矩阵。
+    '''
+
+    s_array = np.zeros((3,3))
+
+    s_array[0,1] = k1
+    s_array[1, 0] = k1  #对称
+    s_array[1,2] = k2
+    s_array[2, 1] = k2  #对称
+
+    #《预报检验-大气科学从业者指南》 4.3.2节 公式4.13
+    s_array[0,0] = (p3 + p1 * (p3 - p2) * k1 + p3 * (p2 + p3) * k2) / (p1 * (p1 + p3))
+    s_array[0, 2] = -(1 + (p1 + p2) * k1 + (p2 + p3) * k2) / (p1 + p3)
+    s_array[1,1] = -(p1 * k1 + p3 * k2) / p2
+    s_array[2,2] = (p1 + p1 * (p1 + p2) * k1 + p3 * (p1 - p2) * k2) / (p3 * (p1 + p3))
+
+    s_array[2,0] = s_array[0,2]  #对称
+
+    return s_array
+
+
+
+def murphy_ctable(p_array,s_array):
+    '''
+    根据3×3的列联表，和评分权重矩阵 计算 Murphy 矩阵
+    评分公式参考《预报检验-大气科学从业者指南》 4.3.2节，公式 4.8
+    :param ctable_array:  3×3的观测预报列联表
+    :param s_array:  评分权重矩阵
+    :return:  Murphy评分
+    '''
+
+    score = np.sum(p_array * s_array)
+    return score
+
+
+
+def murphy_score(ob,fo,grade_list = None,p1 = None,p2 = None,p3 = None,k1 = -0.25,k2 = 0.25):
+    '''
+    计算Murphy 评分。
+    步骤包括：
+    1. 根据实况和预报数据，以及等级划分阈值，统计列联表
+    2. 根据3分类预报问题的实况气候概率p1,p2和p3，确定Murphy评分的评分权重矩阵（函数 get_s_array）
+    3. 根据列联表和权重矩阵，计算Murphy 评分。
+
+    :param ob: 实况数据，
+    :param fo: 预报数据
+    :param grade_list:实况和预报分类的阈值，如果实况和预报已经是离散的等级，则不需要该参数
+    :param p1: 实况为第1分类的气候概率
+    :param p2:实况为第2分类的气候概率
+    :param p3:实况为第2分类的气候概率
+    :param k1: 评分权重系数 s12
+    :param k2:评分权重系数 s23
+    :return: Murphy评分。
+    '''
+
+    #根据实况获取观测预报的列联表
+    ctable = meteva.method.multi_category.table.contingency_table_multicategory(ob,fo,grade_list)
+    if len(ctable.shape)==2:
+        ctable = ctable.reshape(1,ctable.shape[0],ctable.shape[1])
+
+    ctable = ctable/ctable[-1,-1]
+    if p1 is not None and p2 is not None and p3 is not None:
+        # 如果用户从外部指定实况的概率，就用用户指定的概率来生成权重矩阵s_array
+        s_array = get_s_array(p1,p2,p3,k1,k2)
+    else:
+        #如果用户未指定实况概率，则根据传入的实况数据来获取每个等级的概率，再计算权重矩阵
+        p_ob = ctable[0, :-1, -1] / ctable[0, -1, -1]  # 返回的列联表实际上是4×4的，其中最后一行是实况的概率分布
+        s_array = get_s_array(p_ob[0], p_ob[1], p_ob[2], k1, k2)
+
+
+    score_list = []
+    for i in range(ctable.shape[0]):
+        ct_array = ctable[i, :-1, :-1]
+        score1 =murphy_ctable(ct_array,s_array)  #已知列联表和权重系数矩阵，计算Murphy 评分
+        score_list.append(score1)
+
+    if len(score_list)==1:
+        return score_list[0]  #单个预报返回实数
+    else:
+        return np.array(score_list)  #多个预报返回数组
+
+
+
+
+
+if __name__ == "__main__":
+
+
+    s_array = get_s_array(-0.5,-0.25,0.2,0.5,0.3)
+    print(s_array*60)
```

### Comparing `meteva-1.8.1/meteva/method/multi_category/table.py` & `meteva-1.8.2/meteva/method/multi_category/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/probability/plot.py` & `meteva-1.8.2/meteva/method/probability/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/probability/score.py` & `meteva-1.8.2/meteva/method/probability/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/probability/table.py` & `meteva-1.8.2/meteva/method/probability/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/__init__.py` & `meteva-1.8.2/meteva/method/space/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/acc/acc.py` & `meteva-1.8.2/meteva/method/space/acc/acc.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/acc/acc_climate_pre.py` & `meteva-1.8.2/meteva/method/space/acc/acc_climate_pre.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/as_unitname.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/deltametric.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/im.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/lib/solutionset.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_default.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py` & `meteva-1.8.2/meteva/method/space/baddeley_binary_image_metric/locmeasures2d_spatial_vx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/cra/cra.py` & `meteva-1.8.2/meteva/method/space/cra/cra.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/fqi.py` & `meteva-1.8.2/meteva/method/space/fqi/fqi.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/aaft2d.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/aaft2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/ampstats.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/ampstats.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/datagrabber_spatialVx.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/distfun.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/distfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/fft2d.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/fft2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/im.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/loc_list_setup.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/locperf.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/solutionset.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/solutionset.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/lib/surrogater2d.py` & `meteva-1.8.2/meteva/method/space/fqi/lib/surrogater2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fqi/uiqi.py` & `meteva-1.8.2/meteva/method/space/fqi/uiqi.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fss/__init__.py` & `meteva-1.8.2/meteva/method/space/fss/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fss/fss.py` & `meteva-1.8.2/meteva/method/space/fss/fss.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/fss.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/fss.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/fuzzy.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/fuzzy.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/joint.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/joint.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/fss2dfun.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fss2dfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/fuzzyjoint2dfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2d.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dPrep.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dSetUpLists.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/hoods2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dmeitsjer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/kernel2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/progmatic2dfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/thresholder.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/thresholder_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/lib/vxstats.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/lib/vxstats.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/minimum_coverage.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/minimum_coverage.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/multi_event.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/multi_event.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/fuzzy_logic/pragmatic.py` & `meteva-1.8.2/meteva/method/space/fuzzy_logic/pragmatic.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/geo_box_plot/GeoBoxPlot.py` & `meteva-1.8.2/meteva/method/space/geo_box_plot/GeoBoxPlot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/geometric_characterizations/aindex.py` & `meteva-1.8.2/meteva/method/space/geometric_characterizations/aindex.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/geometric_characterizations/cindex.py` & `meteva-1.8.2/meteva/method/space/geometric_characterizations/cindex.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py` & `meteva-1.8.2/meteva/method/space/geometric_characterizations/lib/datagrabber_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/geometric_characterizations/sindex.py` & `meteva-1.8.2/meteva/method/space/geometric_characterizations/sindex.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/geometric_characterizations/spatial_index.py` & `meteva-1.8.2/meteva/method/space/geometric_characterizations/spatial_index.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/as_unitname.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/as_unitname.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/distfun.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distfun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/distmap.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/im.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/lib/solutionset.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/lib/solutionset.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/hausdorff_metric/locperf.py` & `meteva-1.8.2/meteva/method/space/hausdorff_metric/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/__init__.py` & `meteva-1.8.2/meteva/method/space/mode/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/bearing.py` & `meteva-1.8.2/meteva/method/space/mode/bearing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/censqdelta.py` & `meteva-1.8.2/meteva/method/space/mode/censqdelta.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/centmatch.py` & `meteva-1.8.2/meteva/method/space/mode/centmatch.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/consistent.py` & `meteva-1.8.2/meteva/method/space/mode/consistent.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/data_pre.py` & `meteva-1.8.2/meteva/method/space/mode/data_pre.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/deltametric.py` & `meteva-1.8.2/meteva/method/space/mode/deltametric.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/deltamm.py` & `meteva-1.8.2/meteva/method/space/mode/deltamm.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/deltammSqCen.py` & `meteva-1.8.2/meteva/method/space/mode/deltammSqCen.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/deltamm_bak.py` & `meteva-1.8.2/meteva/method/space/mode/deltamm_bak.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/distmap.py` & `meteva-1.8.2/meteva/method/space/mode/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/feature_axis.py` & `meteva-1.8.2/meteva/method/space/mode/feature_axis.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/feature_comps.py` & `meteva-1.8.2/meteva/method/space/mode/feature_comps.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/feature_finder.py` & `meteva-1.8.2/meteva/method/space/mode/feature_finder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/feature_match_analyzer.py` & `meteva-1.8.2/meteva/method/space/mode/feature_match_analyzer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/feature_props.py` & `meteva-1.8.2/meteva/method/space/mode/feature_props.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/feature_table.py` & `meteva-1.8.2/meteva/method/space/mode/feature_table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/interester.py` & `meteva-1.8.2/meteva/method/space/mode/interester.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/intersect.py` & `meteva-1.8.2/meteva/method/space/mode/intersect.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/load.py` & `meteva-1.8.2/meteva/method/space/mode/load.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/loc_list_setup.py` & `meteva-1.8.2/meteva/method/space/mode/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/locperf.py` & `meteva-1.8.2/meteva/method/space/mode/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/make_SpatialVx_bak.py` & `meteva-1.8.2/meteva/method/space/mode/make_SpatialVx_bak.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/make_spatialVx.py` & `meteva-1.8.2/meteva/method/space/mode/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/merge_force.py` & `meteva-1.8.2/meteva/method/space/mode/merge_force.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/minboundmatch.py` & `meteva-1.8.2/meteva/method/space/mode/minboundmatch.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/operater.py` & `meteva-1.8.2/meteva/method/space/mode/operater.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/plot.py` & `meteva-1.8.2/meteva/method/space/mode/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/regress2.py` & `meteva-1.8.2/meteva/method/space/mode/regress2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/sma.py` & `meteva-1.8.2/meteva/method/space/mode/sma.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/tran_to_dataframe.py` & `meteva-1.8.2/meteva/method/space/mode/tran_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/mode/utils.py` & `meteva-1.8.2/meteva/method/space/mode/utils.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/point_to_area.py` & `meteva-1.8.2/meteva/method/space/point_to_area.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/kernel2dmeitsjer.py` & `meteva-1.8.2/meteva/method/space/pphindcast/kernel2dmeitsjer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/kernel2dsmooth.py` & `meteva-1.8.2/meteva/method/space/pphindcast/kernel2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/as_unitname.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/as_unitname.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/hoods2dPrep.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/hoods2dPrep.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/im.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/im.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dmeitsjer.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/kernel2dsmooth.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/kernel2dsmooth.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/make_spatialVx.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/thresholder.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/thresholder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/lib/vxstats.py` & `meteva-1.8.2/meteva/method/space/pphindcast/lib/vxstats.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/pphindcast/pphindcast2d.py` & `meteva-1.8.2/meteva/method/space/pphindcast/pphindcast2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/rigider/fint2d.py` & `meteva-1.8.2/meteva/method/space/rigider/fint2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/rigider/fint2d_old.py` & `meteva-1.8.2/meteva/method/space/rigider/fint2d_old.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/rigider/imomenter.py` & `meteva-1.8.2/meteva/method/space/rigider/imomenter.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/rigider/rigider.py` & `meteva-1.8.2/meteva/method/space/rigider/rigider.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/s1/S1.py` & `meteva-1.8.2/meteva/method/space/s1/S1.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/saller/saller.py` & `meteva-1.8.2/meteva/method/space/saller/saller.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/LocSig.py` & `meteva-1.8.2/meteva/method/space/significance/LocSig.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/bootstrap.py` & `meteva-1.8.2/meteva/method/space/significance/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/bootstrap_ci.py` & `meteva-1.8.2/meteva/method/space/significance/bootstrap_ci.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/is_sig.py` & `meteva-1.8.2/meteva/method/space/significance/is_sig.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/sig_coverage.py` & `meteva-1.8.2/meteva/method/space/significance/sig_coverage.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/significance.py` & `meteva-1.8.2/meteva/method/space/significance/significance.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/spatbiasFS.py` & `meteva-1.8.2/meteva/method/space/significance/spatbiasFS.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/significance/tsboot.py` & `meteva-1.8.2/meteva/method/space/significance/tsboot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/uqi/uqi.py` & `meteva-1.8.2/meteva/method/space/uqi/uqi.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/vgm/rdist.py` & `meteva-1.8.2/meteva/method/space/vgm/rdist.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/vgm/structurogram.py` & `meteva-1.8.2/meteva/method/space/vgm/structurogram.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/space/vgm/structurogram_matrix.py` & `meteva-1.8.2/meteva/method/space/vgm/structurogram_matrix.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/weather_system/identify.py` & `meteva-1.8.2/meteva/method/weather_system/identify.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/yes_or_no/__init__.py` & `meteva-1.8.2/meteva/method/yes_or_no/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/yes_or_no/plot.py` & `meteva-1.8.2/meteva/method/yes_or_no/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/yes_or_no/score.py` & `meteva-1.8.2/meteva/method/yes_or_no/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/yes_or_no/skill.py` & `meteva-1.8.2/meteva/method/yes_or_no/skill.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/method/yes_or_no/table.py` & `meteva-1.8.2/meteva/method/yes_or_no/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/perspact/middel_high.py` & `meteva-1.8.2/meteva/perspact/middel_high.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,51 +3,55 @@
 import pandas as pd
 import os 
 import numpy as np
 
 
 para = {
     "mid_method":meteva.method.tase,
+    "grade_list": None,
+    "compare":None,
     "middle_result_path": r"H:\test_data\output\mps\tase_z.h5",
     "begin_time": datetime.datetime(2018,8,1,0),
     "end_time": datetime.datetime(2018,8,2,0),
     "time_type":"UT",
     "time_step":12,     #起报时间间隔
     "grid" :  meteva.base.grid([70,140,0.25],[10,60,0.25]),  # 检验区域
     "level_list":  [ 850, 700, 500],
     "step":5,  #masker间隔（单位：°）
     "recover":False,
     "ob_data": {
-        "dir_ob":r"\\10.28.16.234\data2\AI\CRA40\2018\Z\LLL\YYYYMMDDHH.nc",  # 实况场数据路径
+        "CRA40":{
+        "dirm": r"\\10.28.16.234\data2\AI\CRA40\2018\Z\LLL\YYYYMMDDHH.nc",  # 实况场数据路径
         "read_method": meteva.base.read_griddata_from_nc,
         "read_para": {},
-        "time_type": "UT",  #实况数据时间类型
-        "multiple": 1,    #当文件数据的单位是位势米，通过乘以9.8转换成位势
+        "time_type": "UT",  # 实况数据时间类型
+        "multiple": 1,  # 当文件数据的单位是位势米，通过乘以9.8转换成位势
+        }
     },
     "fo_data": {
-        "NMC":{
-            "dir_fo": r"\\10.28.16.234\data2\AI\NMC_CRA40\Z\LLL\YYYYMMDDHH\YYYYMMDDHH.TTT.nc",
+        "ECMWF":{
+            "dirm": r"\\10.28.16.234\data2\AI\ECMWF\grib\YYMMDD\YYMMDDHH.TTT.grib",
             "dtime": [12, 240, 12],
-            "reasonable_value": [-100, 400],
-            "read_method": meteva.base.read_griddata_from_nc,
-            "read_para": {},
+            "read_method": meteva.base.read_griddata_from_grib,
+            "read_para": {"level_type":"isobaricInhPa","value_name":"gh"},
             "time_type": "UT",  # 预报数据时间类型是北京时，即08时起报
             "multiple": 1,  # 当文件数据的单位是位势米，通过乘以9.8转换成位势
-            "move_fo_time":0
+            "move_fo_time":0,
+            "veri_by":"self"
         },
 
-        "ECMWF": {
-            "dir_fo":  r"\\10.28.16.177\NMC_Tsinghua_reforecast\cra40\YYYYMMDDHH.nc",
+        "NMC1": {
+            "dirm":  r"\\10.28.16.177\NMC_Tsinghua_reforecast\cra40\YYYYMMDDHH.nc",
             "dtime": [12, 240, 12],
-            "reasonable_value": [-100, 400],
             "read_method": meteva.base.read_griddata_from_nc,
             "read_para": {"value_name": "GPH"},
             "time_type": "UT",#预报数据时间类型是北京时，即08时起报
             "multiple":1, #当文件数据的单位是位势米，通过乘以9.8转换成位势
-            "move_fo_time": 12
+            "move_fo_time": 12,
+            "veri_by": "CRA40"
         },
     },
 }
 
 
 
 def middle_of_score(para):
@@ -78,14 +82,19 @@
 
 
     for model in model_name_list:
         df1_= df1.loc[df1['member'].isin([model])]
         time1 = begin_time
         para_fo1 = para["fo_data"][model]
         move_fo_time = para_fo1["move_fo_time"]
+        veri_by = para_fo1["veri_by"]
+        if veri_by =="self":
+            para_ob1 = para_fo1
+        else:
+            para_ob1 = para["ob_data"][veri_by]
 
         save_k = 0  # 用来在收集的过程间隔一段时间报错一下结果，避免程序错误时没有任何输出导致要重头再来
         dtime_list = np.arange(para_fo1["dtime"][0], para_fo1["dtime"][1] + 1, para_fo1["dtime"][2]).tolist()
         while time1 <= end_time:
             df2 = meteva.base.in_time_list(df1_, time1)
 
             if len(df2.index) ==len(dtime_list):
@@ -95,67 +104,76 @@
                     df3 = meteva.base.in_dtime_list(df2, dtime_list=dh)
                     for level in level_list:
                         df4 = meteva.base.in_level_list(df3, level_list=level)
                         if len(df4.index) ==0:
                             save_k += 1  #
                             time_ob = time1 + datetime.timedelta(hours=dh)
                             time_ob_bt = time_ob + datetime.timedelta(hours=8)
-                            if para["ob_data"]["time_type"].lower() == "bt":
+                            if para_ob1["time_type"].lower() == "bt":
                                 time_path = time_ob_bt
                             else:
                                 time_path = time_ob
 
-                            path0 = meteva.base.get_path(para["ob_data"]["dir_ob"], time_path)
+                            path0 = meteva.base.get_path(para_ob1["dirm"], time_path)
                             path0 = path0.replace("LLL",str(level))
                             if not os.path.exists(path0):
                                 print(path0 +" not exist")
                                 continue
-                            grd_obs = para["ob_data"]["read_method"](path0, grid=para["grid"], time=time_ob,
+                            grd_obs = para_ob1["read_method"](path0, grid=para["grid"], time=time_ob,
                                                                          dtime=0, data_name="OBS", show=True,level = level,
-                                                                         **para["ob_data"]["read_para"])
+                                                                         **para_ob1["read_para"])
                             if grd_obs is None:
                                 print("faild to read "+ path0)
                                 continue
 
-                            grd_obs.values *= para["ob_data"]["multiple"]
+                            grd_obs.values *= para_ob1["multiple"]
 
                             time1_ = time1
                             if para_fo1["time_type"].lower() == "bt":
                                 time1_ = time1 + datetime.timedelta(hours=8)
                             time1_ -= datetime.timedelta(hours=move_fo_time)
 
 
-                            path1 = meteva.base.get_path(para_fo1["dir_fo"], time1_, dh+move_fo_time)
+                            path1 = meteva.base.get_path(para_fo1["dirm"], time1_, dh+move_fo_time)
 
                             path1 = path1.replace("LLL", str(level))
                             grd_fo = para_fo1["read_method"](path1, grid=para["grid"], time=time1, dtime=dh,level = level,
                                                              data_name=model, show=True, **para_fo1["read_para"])
                             if grd_fo is not None:
                                 grd_fo.values *= para_fo1["multiple"]
-                                df_mid = meteva.perspact.middle_df_grd(grd_obs, grd_fo,mid_method, marker=marker)
+                                df_mid = meteva.perspact.middle_df_grd(grd_obs, grd_fo,mid_method, marker=marker,
+                                                                       grade_list=para["grade_list"],compare=para["compare"])
                                 mid_list.append(df_mid)
                             else:
                                 print("faild to read " + path1)
-                time1 = time1 + datetime.timedelta(hours=para["time_step"])  # 在统计时段内时间递增，遍历所有时间。在程序调试阶段，参数hours的取值可以设得大一点，比如2400，全年先算个几天看看结果是否合理,如果合理再改成240，再看结果合理再改成24，或12
-                # 当收集了超过200个时效的数据时就输出一次
-                if save_k % 500 == 0:
-                    mid_all = meteva.base.concat(mid_list)
-                    # 先删除文件在重新输出文件，避免文件大小膨胀
-                    if os.path.exists(middle_result_path):
-                        os.remove(middle_result_path)
-                    mid_all.to_hdf(middle_result_path, "df")  # 将结果输出到文件
 
+                            # 当收集了超过500个时效的数据时就输出一次
+                            if save_k % 500 == 0:
+                                mid_all = meteva.base.concat(mid_list)
+                                # 先删除文件在重新输出文件，避免文件大小膨胀
+                                if os.path.exists(middle_result_path):
+                                    os.remove(middle_result_path)
+                                mid_all.to_hdf(middle_result_path, "df")  # 将结果输出到文件
+
+                # 在统计时段内时间递增，遍历所有时间。在程序调试阶段，参数hours的取值可以设得大一点，比如2400，全年先算个几天看看结果是否合理,如果合理再改成240，再看结果合理再改成24，或12
+                time1 = time1 + datetime.timedelta(hours=para["time_step"])
     mid_all = meteva.base.concat(mid_list)
     # 先删除文件在重新输出文件，避免文件大小膨胀
     if os.path.exists(middle_result_path):
         os.remove(middle_result_path)
     mid_all.to_hdf(middle_result_path, "df")  # 将结果输出到文件
     print("中间量统计程序运行完毕")
     print("中间结果已输出至"+middle_result_path)
     return
 
 
 if __name__ == "__main__":
+    # path = meteva.base.get_path(r"\\10.28.16.234\data2\AI\ECMWF\grib\YYMMDD\YYMMDDHH.TTT.grib",datetime.datetime(2018,1,1,0))
+    # #meteva.base.print_grib_file_info(path,filter_by_keys={"typeOfLevel":"isobaricInhPa"})
+    #
+    # grd = meteva.base.read_griddata_from_grib(path,level_type="isobaricInhPa",value_name="gh",level=[850,500])
+    #print(grd)
     middle_of_score(para)
     path = r"H:\test_data\output\mps\tase_z.h5"
     df = pd.read_hdf(path)
-    print(df)
+    print(df)
+    meteva.perspact.score_df(df,meteva.method.rmse,g = ["member","dtime"],plot = "line")
```

### Comparing `meteva-1.8.1/meteva/perspact/middle_prepare.py` & `meteva-1.8.2/meteva/perspact/middle_prepare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/perspact/multi_element_veri.py` & `meteva-1.8.2/meteva/perspact/multi_element_veri.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/perspact/score.py` & `meteva-1.8.2/meteva/perspact/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/__init__.py` & `meteva-1.8.2/meteva/product/application/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/data_collection.py` & `meteva-1.8.2/meteva/product/application/data_collection.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/data_distribute.py` & `meteva-1.8.2/meteva/product/application/data_distribute.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/data_prepare.py` & `meteva-1.8.2/meteva/product/application/data_prepare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/fun.py` & `meteva-1.8.2/meteva/product/application/fun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/terrain_height_correction.py` & `meteva-1.8.2/meteva/product/application/terrain_height_correction.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/application/time_compare.py` & `meteva-1.8.2/meteva/product/application/time_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/__init__.py` & `meteva-1.8.2/meteva/product/program/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/diurnal.py` & `meteva-1.8.2/meteva/product/program/diurnal.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/error_ana_list.py` & `meteva-1.8.2/meteva/product/program/error_ana_list.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/error_ana_scatter.py` & `meteva-1.8.2/meteva/product/program/error_ana_scatter.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/fun.py` & `meteva-1.8.2/meteva/product/program/fun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/plot.py` & `meteva-1.8.2/meteva/product/program/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/process_compare.py` & `meteva-1.8.2/meteva/product/program/process_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/sample_statistic.py` & `meteva-1.8.2/meteva/product/program/sample_statistic.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/score.py` & `meteva-1.8.2/meteva/product/program/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/space_compare.py` & `meteva-1.8.2/meteva/product/program/space_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/table.py` & `meteva-1.8.2/meteva/product/program/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/time_compare.py` & `meteva-1.8.2/meteva/product/program/time_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/time_space_compare.py` & `meteva-1.8.2/meteva/product/program/time_space_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/program/typhoon.py` & `meteva-1.8.2/meteva/product/program/typhoon.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/regulation/environment.py` & `meteva-1.8.2/meteva/product/regulation/environment.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/regulation/short_term_heavy_rainfall.py` & `meteva-1.8.2/meteva/product/regulation/short_term_heavy_rainfall.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/regulation/temperature.py` & `meteva-1.8.2/meteva/product/regulation/temperature.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva/product/regulation/thunderstrom_gale.py` & `meteva-1.8.2/meteva/product/regulation/thunderstrom_gale.py`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/meteva.egg-info/PKG-INFO` & `meteva-1.8.2/meteva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteva
-Version: 1.8.1
+Version: 1.8.2
 Summary: A collections of functions for meteorological verification.
 Author: liucouhua,daikan,wangbaoli,tangbuxing
 Author-email: liucouhua@163.com
 License: GPL3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meteva-1.8.1/meteva.egg-info/SOURCES.txt` & `meteva-1.8.2/meteva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meteva-1.8.1/setup.py` & `meteva-1.8.2/setup.py`

 * *Files identical despite different names*

