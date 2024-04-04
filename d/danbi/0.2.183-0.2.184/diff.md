# Comparing `tmp/danbi-0.2.183.tar.gz` & `tmp/danbi-0.2.184.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danbi-0.2.183.tar", max compression
+gzip compressed data, was "danbi-0.2.184.tar", max compression
```

## Comparing `danbi-0.2.183.tar` & `danbi-0.2.184.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    11357 2023-01-16 04:29:47.588484 danbi-0.2.183/LICENSE
--rw-r--r--   0        0        0      294 2023-01-16 04:29:47.588573 danbi-0.2.183/README.md
--rw-r--r--   0        0        0       93 2024-03-10 05:34:51.697086 danbi-0.2.183/danbi/__init__.py
--rw-r--r--   0        0        0      611 2023-03-09 08:51:44.539618 danbi-0.2.183/danbi/analysis/__init__.py
--rw-r--r--   0        0        0     1985 2023-06-26 09:29:39.904412 danbi-0.2.183/danbi/analysis/convert.py
--rw-r--r--   0        0        0     6353 2023-07-15 10:56:45.715151 danbi-0.2.183/danbi/analysis/normalization.py
--rw-r--r--   0        0        0     4657 2023-01-16 04:29:47.589162 danbi-0.2.183/danbi/analysis/pandas_ext.py
--rw-r--r--   0        0        0    18326 2023-07-30 09:30:17.506694 danbi-0.2.183/danbi/analysis/plot_bokeh.py
--rw-r--r--   0        0        0     2672 2023-01-16 04:29:47.589457 danbi-0.2.183/danbi/analysis/relation.py
--rw-r--r--   0        0        0     1125 2023-01-16 04:29:47.589592 danbi-0.2.183/danbi/database/ConnMngPsql.py
--rw-r--r--   0        0        0     1011 2023-01-16 04:29:47.589675 danbi-0.2.183/danbi/database/ConnMngPsqlAsync.py
--rw-r--r--   0        0        0     3939 2023-04-10 07:25:06.747546 danbi-0.2.183/danbi/database/DBPsql.py
--rw-r--r--   0        0        0     3313 2023-03-23 04:33:57.770664 danbi-0.2.183/danbi/database/DBPsqlAsync.py
--rw-r--r--   0        0        0      709 2023-01-16 04:29:47.589979 danbi-0.2.183/danbi/database/IConnectionManager.py
--rw-r--r--   0        0        0     5747 2023-04-05 04:44:15.617593 danbi-0.2.183/danbi/database/IDB.py
--rw-r--r--   0        0        0      961 2023-01-16 04:29:47.590182 danbi-0.2.183/danbi/database/__init__.py
--rw-r--r--   0        0        0     1121 2023-01-16 04:29:47.590263 danbi-0.2.183/danbi/database/factory.py
--rw-r--r--   0        0        0     1686 2023-10-10 01:38:44.711674 danbi-0.2.183/danbi/dataprocess/TimeseriesToImage.py
--rw-r--r--   0        0        0     6170 2024-03-01 02:38:24.088343 danbi-0.2.183/danbi/dataprocess/ZeroBaseMinMaxScaler.py
--rw-r--r--   0        0        0      216 2023-11-24 00:23:29.654127 danbi-0.2.183/danbi/dataprocess/__init__.py
--rw-r--r--   0        0        0     1464 2023-09-28 07:05:16.420158 danbi-0.2.183/danbi/dataprocess/convert.py
--rw-r--r--   0        0        0     1095 2023-11-27 07:07:35.007945 danbi-0.2.183/danbi/dataprocess/signal.py
--rw-r--r--   0        0        0       23 2023-01-16 04:29:47.590383 danbi-0.2.183/danbi/extends/__init__.py
--rw-r--r--   0        0        0      241 2023-08-11 00:03:31.112539 danbi-0.2.183/danbi/extends/bibokeh/__init__.py
--rw-r--r--   0        0        0     7273 2023-08-11 03:37:26.402966 danbi-0.2.183/danbi/extends/bibokeh/plot_chart.py
--rw-r--r--   0        0        0     6008 2023-08-11 07:46:32.916645 danbi-0.2.183/danbi/extends/bibokeh/show.py
--rw-r--r--   0        0        0       85 2023-01-16 04:29:47.590501 danbi-0.2.183/danbi/extends/bipandas/__init__.py
--rw-r--r--   0        0        0     5014 2023-07-27 00:00:42.827043 danbi-0.2.183/danbi/extends/bipandas/column_ext.py
--rw-r--r--   0        0        0     3649 2023-11-21 13:01:06.534824 danbi-0.2.183/danbi/extends/bipandas/dataframe_ext.py
--rw-r--r--   0        0        0     1296 2023-01-16 04:29:47.590775 danbi-0.2.183/danbi/extends/bipandas/state.py
--rw-r--r--   0        0        0       36 2023-10-18 04:00:18.006888 danbi-0.2.183/danbi/extends/biray/__init__.py
--rw-r--r--   0        0        0     2924 2023-10-18 06:13:44.971183 danbi-0.2.183/danbi/extends/biray/ray.py
--rw-r--r--   0        0        0       87 2023-09-04 14:47:58.168716 danbi-0.2.183/danbi/extends/bitensorflow/__init__.py
--rw-r--r--   0        0        0     2196 2023-09-18 11:36:28.989926 danbi-0.2.183/danbi/extends/bitensorflow/tfrecord_ext.py
--rw-r--r--   0        0        0        0 2023-01-16 04:29:47.590907 danbi-0.2.183/danbi/extlib/__init__.py
--rw-r--r--   0        0        0     1897 2023-01-16 04:29:47.591123 danbi-0.2.183/danbi/extlib/pandas.py
--rw-r--r--   0        0        0     1759 2023-01-16 04:29:47.591327 danbi-0.2.183/danbi/extlib/stock.py
--rw-r--r--   0        0        0     3106 2023-01-16 04:29:47.591418 danbi-0.2.183/danbi/extlib/tensorflow.py
--rw-r--r--   0        0        0     5451 2023-01-16 04:29:47.591578 danbi-0.2.183/danbi/gym/TradeSingleEnv.py
--rw-r--r--   0        0        0      318 2023-01-16 04:29:47.591678 danbi-0.2.183/danbi/gym/__init__.py
--rw-r--r--   0        0        0      788 2023-01-16 04:29:47.591765 danbi-0.2.183/danbi/gym/simulation.py
--rw-r--r--   0        0        0      194 2023-01-16 04:29:47.591846 danbi-0.2.183/danbi/gym/trade.py
--rw-r--r--   0        0        0      481 2023-01-16 04:29:47.591984 danbi-0.2.183/danbi/mapping/IMapper.py
--rw-r--r--   0        0        0     1329 2023-01-16 04:29:47.592071 danbi-0.2.183/danbi/mapping/Jinja2Mapper.py
--rw-r--r--   0        0        0     6169 2023-01-16 04:29:47.592179 danbi-0.2.183/danbi/mapping/YAMLConfig.py
--rw-r--r--   0        0        0      103 2023-01-16 04:29:47.592252 danbi-0.2.183/danbi/mapping/__init__.py
--rw-r--r--   0        0        0      498 2023-01-16 04:29:47.592663 danbi-0.2.183/danbi/plugable/IPlugin.py
--rw-r--r--   0        0        0      508 2023-01-16 04:29:47.592749 danbi-0.2.183/danbi/plugable/IPluginAsync.py
--rw-r--r--   0        0        0     3058 2023-07-05 13:30:57.365028 danbi-0.2.183/danbi/plugable/PluginManager.py
--rw-r--r--   0        0        0      108 2023-01-16 04:29:47.592919 danbi-0.2.183/danbi/plugable/__init__.py
--rw-r--r--   0        0        0     9014 2023-09-04 14:47:58.170172 danbi-0.2.183/danbi/utils/EduPlot.py
--rw-r--r--   0        0        0      415 2023-09-28 07:05:16.420411 danbi-0.2.183/danbi/utils/__init__.py
--rw-r--r--   0        0        0     5159 2023-01-16 04:29:47.593200 danbi-0.2.183/danbi/utils/day_time.py
--rw-r--r--   0        0        0     2284 2023-01-16 04:29:47.593302 danbi-0.2.183/danbi/utils/info.py
--rw-r--r--   0        0        0     1629 2023-09-04 14:47:58.171432 danbi-0.2.183/danbi/utils/jupyter.py
--rw-r--r--   0        0        0      259 2024-03-10 05:34:28.485677 danbi-0.2.183/danbi/utils/util.py
--rw-r--r--   0        0        0     1581 2023-10-05 07:17:36.597754 danbi-0.2.183/danbi/utils/with_print.py
--rw-r--r--   0        0        0      901 2024-03-10 05:35:09.831938 danbi-0.2.183/pyproject.toml
--rw-r--r--   0        0        0     1118 2024-03-10 05:35:15.153266 danbi-0.2.183/setup.py
--rw-r--r--   0        0        0     1257 2024-03-10 05:35:15.153430 danbi-0.2.183/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-16 04:29:47.588484 danbi-0.2.184/LICENSE
+-rw-r--r--   0        0        0      294 2023-01-16 04:29:47.588573 danbi-0.2.184/README.md
+-rw-r--r--   0        0        0       93 2024-03-20 00:06:00.601503 danbi-0.2.184/danbi/__init__.py
+-rw-r--r--   0        0        0      611 2023-03-09 08:51:44.539618 danbi-0.2.184/danbi/analysis/__init__.py
+-rw-r--r--   0        0        0     1985 2023-06-26 09:29:39.904412 danbi-0.2.184/danbi/analysis/convert.py
+-rw-r--r--   0        0        0     6353 2023-07-15 10:56:45.715151 danbi-0.2.184/danbi/analysis/normalization.py
+-rw-r--r--   0        0        0     4657 2023-01-16 04:29:47.589162 danbi-0.2.184/danbi/analysis/pandas_ext.py
+-rw-r--r--   0        0        0    18326 2023-07-30 09:30:17.506694 danbi-0.2.184/danbi/analysis/plot_bokeh.py
+-rw-r--r--   0        0        0     2672 2023-01-16 04:29:47.589457 danbi-0.2.184/danbi/analysis/relation.py
+-rw-r--r--   0        0        0     1125 2023-01-16 04:29:47.589592 danbi-0.2.184/danbi/database/ConnMngPsql.py
+-rw-r--r--   0        0        0     1011 2023-01-16 04:29:47.589675 danbi-0.2.184/danbi/database/ConnMngPsqlAsync.py
+-rw-r--r--   0        0        0     3939 2023-04-10 07:25:06.747546 danbi-0.2.184/danbi/database/DBPsql.py
+-rw-r--r--   0        0        0     3313 2023-03-23 04:33:57.770664 danbi-0.2.184/danbi/database/DBPsqlAsync.py
+-rw-r--r--   0        0        0      709 2023-01-16 04:29:47.589979 danbi-0.2.184/danbi/database/IConnectionManager.py
+-rw-r--r--   0        0        0     5747 2023-04-05 04:44:15.617593 danbi-0.2.184/danbi/database/IDB.py
+-rw-r--r--   0        0        0      961 2023-01-16 04:29:47.590182 danbi-0.2.184/danbi/database/__init__.py
+-rw-r--r--   0        0        0     1121 2023-01-16 04:29:47.590263 danbi-0.2.184/danbi/database/factory.py
+-rw-r--r--   0        0        0     1686 2023-10-10 01:38:44.711674 danbi-0.2.184/danbi/dataprocess/TimeseriesToImage.py
+-rw-r--r--   0        0        0     6170 2024-03-01 02:38:24.088343 danbi-0.2.184/danbi/dataprocess/ZeroBaseMinMaxScaler.py
+-rw-r--r--   0        0        0      216 2023-11-24 00:23:29.654127 danbi-0.2.184/danbi/dataprocess/__init__.py
+-rw-r--r--   0        0        0     1464 2023-09-28 07:05:16.420158 danbi-0.2.184/danbi/dataprocess/convert.py
+-rw-r--r--   0        0        0     1095 2023-11-27 07:07:35.007945 danbi-0.2.184/danbi/dataprocess/signal.py
+-rw-r--r--   0        0        0       23 2023-01-16 04:29:47.590383 danbi-0.2.184/danbi/extends/__init__.py
+-rw-r--r--   0        0        0      241 2023-08-11 00:03:31.112539 danbi-0.2.184/danbi/extends/bibokeh/__init__.py
+-rw-r--r--   0        0        0     7273 2023-08-11 03:37:26.402966 danbi-0.2.184/danbi/extends/bibokeh/plot_chart.py
+-rw-r--r--   0        0        0     6008 2023-08-11 07:46:32.916645 danbi-0.2.184/danbi/extends/bibokeh/show.py
+-rw-r--r--   0        0        0       85 2023-01-16 04:29:47.590501 danbi-0.2.184/danbi/extends/bipandas/__init__.py
+-rw-r--r--   0        0        0     5014 2023-07-27 00:00:42.827043 danbi-0.2.184/danbi/extends/bipandas/column_ext.py
+-rw-r--r--   0        0        0     3649 2023-11-21 13:01:06.534824 danbi-0.2.184/danbi/extends/bipandas/dataframe_ext.py
+-rw-r--r--   0        0        0     1296 2023-01-16 04:29:47.590775 danbi-0.2.184/danbi/extends/bipandas/state.py
+-rw-r--r--   0        0        0       36 2023-10-18 04:00:18.006888 danbi-0.2.184/danbi/extends/biray/__init__.py
+-rw-r--r--   0        0        0     2961 2024-03-20 00:05:25.129469 danbi-0.2.184/danbi/extends/biray/ray.py
+-rw-r--r--   0        0        0       87 2023-09-04 14:47:58.168716 danbi-0.2.184/danbi/extends/bitensorflow/__init__.py
+-rw-r--r--   0        0        0     2196 2023-09-18 11:36:28.989926 danbi-0.2.184/danbi/extends/bitensorflow/tfrecord_ext.py
+-rw-r--r--   0        0        0        0 2023-01-16 04:29:47.590907 danbi-0.2.184/danbi/extlib/__init__.py
+-rw-r--r--   0        0        0     1897 2023-01-16 04:29:47.591123 danbi-0.2.184/danbi/extlib/pandas.py
+-rw-r--r--   0        0        0     1759 2023-01-16 04:29:47.591327 danbi-0.2.184/danbi/extlib/stock.py
+-rw-r--r--   0        0        0     3106 2023-01-16 04:29:47.591418 danbi-0.2.184/danbi/extlib/tensorflow.py
+-rw-r--r--   0        0        0     5451 2023-01-16 04:29:47.591578 danbi-0.2.184/danbi/gym/TradeSingleEnv.py
+-rw-r--r--   0        0        0      318 2023-01-16 04:29:47.591678 danbi-0.2.184/danbi/gym/__init__.py
+-rw-r--r--   0        0        0      788 2023-01-16 04:29:47.591765 danbi-0.2.184/danbi/gym/simulation.py
+-rw-r--r--   0        0        0      194 2023-01-16 04:29:47.591846 danbi-0.2.184/danbi/gym/trade.py
+-rw-r--r--   0        0        0      481 2023-01-16 04:29:47.591984 danbi-0.2.184/danbi/mapping/IMapper.py
+-rw-r--r--   0        0        0     1329 2023-01-16 04:29:47.592071 danbi-0.2.184/danbi/mapping/Jinja2Mapper.py
+-rw-r--r--   0        0        0     6169 2023-01-16 04:29:47.592179 danbi-0.2.184/danbi/mapping/YAMLConfig.py
+-rw-r--r--   0        0        0      103 2023-01-16 04:29:47.592252 danbi-0.2.184/danbi/mapping/__init__.py
+-rw-r--r--   0        0        0      498 2023-01-16 04:29:47.592663 danbi-0.2.184/danbi/plugable/IPlugin.py
+-rw-r--r--   0        0        0      508 2023-01-16 04:29:47.592749 danbi-0.2.184/danbi/plugable/IPluginAsync.py
+-rw-r--r--   0        0        0     3058 2023-07-05 13:30:57.365028 danbi-0.2.184/danbi/plugable/PluginManager.py
+-rw-r--r--   0        0        0      108 2023-01-16 04:29:47.592919 danbi-0.2.184/danbi/plugable/__init__.py
+-rw-r--r--   0        0        0     9014 2023-09-04 14:47:58.170172 danbi-0.2.184/danbi/utils/EduPlot.py
+-rw-r--r--   0        0        0      415 2023-09-28 07:05:16.420411 danbi-0.2.184/danbi/utils/__init__.py
+-rw-r--r--   0        0        0     5159 2023-01-16 04:29:47.593200 danbi-0.2.184/danbi/utils/day_time.py
+-rw-r--r--   0        0        0     2284 2023-01-16 04:29:47.593302 danbi-0.2.184/danbi/utils/info.py
+-rw-r--r--   0        0        0     1629 2023-09-04 14:47:58.171432 danbi-0.2.184/danbi/utils/jupyter.py
+-rw-r--r--   0        0        0      259 2024-03-10 05:34:28.485677 danbi-0.2.184/danbi/utils/util.py
+-rw-r--r--   0        0        0     1581 2023-10-05 07:17:36.597754 danbi-0.2.184/danbi/utils/with_print.py
+-rw-r--r--   0        0        0      901 2024-03-20 00:06:11.105455 danbi-0.2.184/pyproject.toml
+-rw-r--r--   0        0        0     1118 2024-03-20 00:06:29.340598 danbi-0.2.184/setup.py
+-rw-r--r--   0        0        0     1257 2024-03-20 00:06:29.340767 danbi-0.2.184/PKG-INFO
```

### Comparing `danbi-0.2.183/LICENSE` & `danbi-0.2.184/LICENSE`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/analysis/__init__.py` & `danbi-0.2.184/danbi/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/analysis/convert.py` & `danbi-0.2.184/danbi/analysis/convert.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/analysis/normalization.py` & `danbi-0.2.184/danbi/analysis/normalization.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/analysis/pandas_ext.py` & `danbi-0.2.184/danbi/analysis/pandas_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/analysis/plot_bokeh.py` & `danbi-0.2.184/danbi/analysis/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/analysis/relation.py` & `danbi-0.2.184/danbi/analysis/relation.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/ConnMngPsql.py` & `danbi-0.2.184/danbi/database/ConnMngPsql.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/ConnMngPsqlAsync.py` & `danbi-0.2.184/danbi/database/ConnMngPsqlAsync.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/DBPsql.py` & `danbi-0.2.184/danbi/database/DBPsql.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/DBPsqlAsync.py` & `danbi-0.2.184/danbi/database/DBPsqlAsync.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/IConnectionManager.py` & `danbi-0.2.184/danbi/database/IConnectionManager.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/IDB.py` & `danbi-0.2.184/danbi/database/IDB.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/__init__.py` & `danbi-0.2.184/danbi/database/__init__.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/database/factory.py` & `danbi-0.2.184/danbi/database/factory.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/dataprocess/TimeseriesToImage.py` & `danbi-0.2.184/danbi/dataprocess/TimeseriesToImage.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/dataprocess/ZeroBaseMinMaxScaler.py` & `danbi-0.2.184/danbi/dataprocess/ZeroBaseMinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/dataprocess/convert.py` & `danbi-0.2.184/danbi/dataprocess/convert.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/dataprocess/signal.py` & `danbi-0.2.184/danbi/dataprocess/signal.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extends/bibokeh/plot_chart.py` & `danbi-0.2.184/danbi/extends/bibokeh/plot_chart.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extends/bibokeh/show.py` & `danbi-0.2.184/danbi/extends/bibokeh/show.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extends/bipandas/column_ext.py` & `danbi-0.2.184/danbi/extends/bipandas/column_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extends/bipandas/dataframe_ext.py` & `danbi-0.2.184/danbi/extends/bipandas/dataframe_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extends/bipandas/state.py` & `danbi-0.2.184/danbi/extends/bipandas/state.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extends/biray/ray.py` & `danbi-0.2.184/danbi/extends/biray/ray.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,21 +52,21 @@
     if chunk is None:
         chunk = int(psutil.cpu_count() * 0.9)
     
     ray_refs = []
     cnt_total = len(vals)
     for idx, val in enumerate(vals):
         if vervos:
-            print(f"{idx+1}/{cnt_total} ({round((idx+1)/cnt_total*100)}%)", end="\r")
+            print(f"{idx+1}/{cnt_total} ({round((idx+1)/cnt_total*100)}%) {len(ray_refs)} {' '*20}", end="\r")
         if isinstance(val, (list, tuple)):
             ray_refs.append(func_ray.remote(*val))
         else:
             ray_refs.append(func_ray.remote(val))
         if idx % chunk == 0:
             while len(ray_refs) > int(chunk * 0.5):
                 done_id, ray_refs = ray.wait(ray_refs)
-                if func_callback:
+                if func_callback is not None:
                     func_callback(*ray.get(done_id)[0])
     while len(ray_refs):
         done_id, ray_refs = ray.wait(ray_refs)
         if func_callback:
             func_callback(*ray.get(done_id)[0])
```

### Comparing `danbi-0.2.183/danbi/extends/bitensorflow/tfrecord_ext.py` & `danbi-0.2.184/danbi/extends/bitensorflow/tfrecord_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extlib/pandas.py` & `danbi-0.2.184/danbi/extlib/pandas.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extlib/stock.py` & `danbi-0.2.184/danbi/extlib/stock.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/extlib/tensorflow.py` & `danbi-0.2.184/danbi/extlib/tensorflow.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/gym/TradeSingleEnv.py` & `danbi-0.2.184/danbi/gym/TradeSingleEnv.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/gym/simulation.py` & `danbi-0.2.184/danbi/gym/simulation.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/mapping/Jinja2Mapper.py` & `danbi-0.2.184/danbi/mapping/Jinja2Mapper.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/mapping/YAMLConfig.py` & `danbi-0.2.184/danbi/mapping/YAMLConfig.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/plugable/PluginManager.py` & `danbi-0.2.184/danbi/plugable/PluginManager.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/utils/EduPlot.py` & `danbi-0.2.184/danbi/utils/EduPlot.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/utils/day_time.py` & `danbi-0.2.184/danbi/utils/day_time.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/utils/info.py` & `danbi-0.2.184/danbi/utils/info.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/utils/jupyter.py` & `danbi-0.2.184/danbi/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/danbi/utils/with_print.py` & `danbi-0.2.184/danbi/utils/with_print.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.183/pyproject.toml` & `danbi-0.2.184/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "danbi"
-version = "0.2.183"
+version = "0.2.184"
 description = "python utility library"
 authors = ["nockchun <nockchun@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nockchun/danbi"
 repository = "https://github.com/nockchun/danbi"
 keywords = ["mybatis like", "sql mapper", "python utils"]
```

### Comparing `danbi-0.2.183/setup.py` & `danbi-0.2.184/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'danbi.utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'danbi',
-    'version': '0.2.183',
+    'version': '0.2.184',
     'description': 'python utility library',
     'long_description': '# danbi\n[![license]](/LICENSE)\n[![pypi]](https://pypi.org/project/danbi/)\n[![pyversions]](http://pypi.python.org/pypi/danbi)\n[![Downloads](https://pepy.tech/badge/danbi)](https://pepy.tech/project/danbi)\n\n---\n\ndanbi is python utility library.\n\n## Installation\n\n```python\npip install danbi\n```\n\n',
     'author': 'nockchun',
     'author_email': 'nockchun@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/nockchun/danbi',
```

### Comparing `danbi-0.2.183/PKG-INFO` & `danbi-0.2.184/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danbi
-Version: 0.2.183
+Version: 0.2.184
 Summary: python utility library
 Home-page: https://github.com/nockchun/danbi
 License: Apache-2.0
 Keywords: mybatis like,sql mapper,python utils
 Author: nockchun
 Author-email: nockchun@gmail.com
 Requires-Python: >=3.7,<4.0
```

