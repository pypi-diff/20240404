# Comparing `tmp/Fr1997v011-1.2.2.tar.gz` & `tmp/Fr1997v011-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.2.2.tar", last modified: Tue Apr  2 02:58:55 2024, max compression
+gzip compressed data, was "Fr1997v011-1.2.3.tar", last modified: Thu Apr  4 11:14:16 2024, max compression
```

## Comparing `Fr1997v011-1.2.2.tar` & `Fr1997v011-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.138230 Fr1997v011-1.2.2/
-drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.128719 Fr1997v011-1.2.2/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-02 02:58:55.136230 Fr1997v011-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-03-26 06:16:58.000000 Fr1997v011-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.129719 Fr1997v011-1.2.2/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.2/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.132719 Fr1997v011-1.2.2/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.2/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   126840 2024-04-02 02:58:52.000000 Fr1997v011-1.2.2/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.135230 Fr1997v011-1.2.2/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.2/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-02 02:58:55.138230 Fr1997v011-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-02 02:56:58.000000 Fr1997v011-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.007455 Fr1997v011-1.2.3/
+drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.000945 Fr1997v011-1.2.3/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-04 11:14:16.006466 Fr1997v011-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-02 02:58:59.000000 Fr1997v011-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.001945 Fr1997v011-1.2.3/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.3/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.003945 Fr1997v011-1.2.3/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.3/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   125905 2024-04-04 11:13:38.000000 Fr1997v011-1.2.3/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:14:16.005449 Fr1997v011-1.2.3/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.3/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 11:14:16.007455 Fr1997v011-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-04 11:14:15.000000 Fr1997v011-1.2.3/setup.py
```

### Comparing `Fr1997v011-1.2.2/LICENSE` & `Fr1997v011-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.2.2/README.md` & `Fr1997v011-1.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.2.1.tar.gz
+pip install dist/Fr1997v011-1.2.2.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.2.2/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.2.3/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 """
     pip install redis
     pip install elasticsearch
     pip install python-memcached
     pip install PyExecJS
     pip install -U cos-python-sdk-v5
+    pip install pypinyin
 """
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
@@ -1177,14 +1178,21 @@
                 wav_url_list = bt['play_addr']['url_list']
                 if wav_url_list:
                     if '&cs=2' in wav_url_list[0]:
                         base_ret_data['wav_size'] = bt['bit_rate']
                         base_ret_data['wav_url'] = bt['play_addr']['url_list']
 
             return base_ret_data
+        elif tp == 'wav_small':
+            # 获取音频
+            bit_rate = res_data['video']['bit_rate'][-1]
+            base_ret_data['sec_uid'] = sec_uid
+            base_ret_data['wav_size'] = bit_rate['bit_rate']
+            base_ret_data['wav_url'] = bit_rate['play_addr']['url_list']
+            return base_ret_data
         else:
             return base_ret_data
 
 
 # 抖音
 class DouyinJike:
     # 抖音视频id短链
@@ -1392,15 +1400,15 @@
             data_data = response.json
             user_detail = data_data.get('user')
 
             data_json = self.analysis_douyin_user(user_detail)  # 数据获取
             return data_json
 
     # 【api】 视频详情
-    def api_douyin_video(self, video_id, use_proxies=1):
+    def api_douyin_video(self, video_id, use_proxies=1, res_tp='video_info'):
         cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
         headers = {
             "authority": "www.douyin.com",
             "pragma": "no-cache",
             "cache-control": "no-cache",
             "accept": "application/json, text/plain, */*",
             "user-agent": config_dict['base_ua'],
@@ -1420,15 +1428,15 @@
                 data_data = response.json
 
                 # 是否存在
                 if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(data_data):
                     return {'aweme_type': 1, 'is_alive': 0, 'err': 'del'}
 
                 video_detail = data_data['aweme_detail']
-                data_json = mode_spider.douyin_video_response(video_detail, tp='video_info')  # 数据获取
+                data_json = mode_spider.douyin_video_response(video_detail, tp=res_tp)  # 数据获取
                 return data_json
         except Exception as E:
             return {'aweme_type': 1, 'is_alive': 0, 'err': E}
 
     # 【api】 用户主页视频列表 amemv版本
     def user_video_list_mv(self, sec_uid, max_cursor='0', timeout=30):
         ret_data = {
@@ -3241,41 +3249,7 @@
 mode_douyin = DouyinJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
-
-# def fast_douyin_video_text():
-#     text = 'https://www.douyin.com/search/%E8%B6%B3%E7%90%83?modal_id=7105766792102038821&type=video'
-#     video_id = mode_douyin.get_video_id(text)  # 获取video_id
-#     video_info = mode_douyin.api_douyin_video(video_id, use_proxies=1)
-#
-#     """
-#         如果视频详细自带 mp3格式可以直接转
-#     """
-#
-#     if video_info:
-#         print(video_info)
-#         mp3_url_list = video_info['mp3_url_list']
-#         print(mp3_url_list)
-#
-#         if mp3_url_list:
-#             mp3_url = mp3_url_list[0]
-#             print(mp3_url_list)
-#
-#         #     headers = {
-#         #         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36 Edg/122.0.0.0',
-#         #     }
-#         #     mp3_url_bs64 = base64.b64encode(mp3_url.encode()).decode()
-#         #     response_text = requests.get(url=f'http://49.234.188.96:7677/hello/{mp3_url_bs64}', headers=headers)
-#         #     print(response_text.text)
-#         # else:
-#         #     wav_url = video_info['download_addr_url_list'][0]
-#         #     print(wav_url)
-#         #     # response = requests.get(wav_url)
-#         #     # print(response.content)
-#
-#
-# fast_douyin_video_text()
-
```

