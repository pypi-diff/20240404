# Comparing `tmp/vios-2.2.6-py3-none-any.whl.zip` & `tmp/vios-2.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 46575 bytes, number of entries: 25
+Zip file size: 46584 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat     2858 b- defN 24-Mar-19 07:04 quark/__main__.py
--rw-rw-rw-  2.0 fat    18341 b- defN 24-Apr-04 04:18 quark/proxy.py
+-rw-rw-rw-  2.0 fat    18428 b- defN 24-Apr-04 05:47 quark/proxy.py
 -rw-rw-rw-  2.0 fat    18861 b- defN 24-Mar-21 01:49 quark/app/__init__.py
 -rw-rw-rw-  2.0 fat     2575 b- defN 24-Mar-25 05:43 quark/app/_data.py
 -rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 07:04 quark/app/demo.py
 -rw-rw-rw-  2.0 fat     9043 b- defN 24-Mar-19 07:04 quark/app/task.py
 -rw-rw-rw-  2.0 fat     5876 b- defN 24-Mar-19 07:16 quark/app/uapi.py
 -rw-rw-rw-  2.0 fat     7914 b- defN 24-Mar-19 07:04 quark/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat      386 b- defN 24-Mar-19 07:04 quark/driver/__init__.py
@@ -13,15 +13,15 @@
 -rw-rw-rw-  2.0 fat     4663 b- defN 24-Mar-19 07:04 quark/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5432 b- defN 24-Mar-19 07:04 quark/driver/common/visadriver.py
 -rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-19 07:04 quark/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    15111 b- defN 24-Mar-19 07:04 quark/envelope/assembler.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 24-Mar-19 07:04 quark/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-19 07:04 quark/envelope/device.py
 -rw-rw-rw-  2.0 fat     3758 b- defN 24-Mar-25 01:32 quark/envelope/processor.py
--rw-rw-rw-  2.0 fat     4216 b- defN 24-Apr-04 04:17 quark/envelope/router.py
+-rw-rw-rw-  2.0 fat     4224 b- defN 24-Apr-04 05:48 quark/envelope/router.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 24-Mar-25 01:32 quark/envelope/systemq.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-04 04:20 vios-2.2.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-04 04:20 vios-2.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 04:20 vios-2.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-04 04:20 vios-2.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-04 04:20 vios-2.2.6.dist-info/RECORD
-25 files, 127784 bytes uncompressed, 43399 bytes compressed:  66.0%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-04 05:55 vios-2.2.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-04 05:55 vios-2.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 05:55 vios-2.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-04 05:55 vios-2.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-04 05:55 vios-2.2.7.dist-info/RECORD
+25 files, 127879 bytes uncompressed, 43408 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: quark/envelope/router.py
 Comment: 
 
 Filename: quark/envelope/systemq.py
 Comment: 
 
-Filename: vios-2.2.6.dist-info/LICENSE
+Filename: vios-2.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: vios-2.2.6.dist-info/METADATA
+Filename: vios-2.2.7.dist-info/METADATA
 Comment: 
 
-Filename: vios-2.2.6.dist-info/WHEEL
+Filename: vios-2.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: vios-2.2.6.dist-info/top_level.txt
+Filename: vios-2.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-2.2.6.dist-info/RECORD
+Filename: vios-2.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quark/proxy.py

```diff
@@ -490,15 +490,14 @@
             try:
                 # data: list[dict] = result['data']['count']
                 data: list[np.ndarray] = result['data']['count']
                 status = 'finished'
             except Exception as e:
                 logger.error(f'Failed to postprocess result: {e}')
 
-        raw, new = {}, {}
         if status == 'finished':
             dres = {}
             for dat in data:
                 # for k, v in dat.items():  # dat[()][0]
                 #     dres[k] = dres.get(k, 0)+v
                 for kv in dat:
                     if kv[-1] < 0:
@@ -517,18 +516,19 @@
                 # if meta['coqis']['correct']:
                 from home.ylfeng.cloud import correct_readout
                 cdres = correct_readout(dres, meta['other']['measure'])
             except Exception as e:
                 cdres = dres
                 logger.error(f'Failed to correct readout, {e}!')
 
-            for k, v in dres.items():
-                raw[''.join((str(i) for i in k))] = v
-            for k, v in cdres.items():
-                new[''.join((str(i) for i in k))] = v
-        return status, new, raw
+        ret = {'count': {''.join((str(i) for i in k)): v for k, v in dres.items()},
+               'corrected': {''.join((str(i) for i in k)): v for k, v in cdres.items()},
+               'transpiled': meta['coqis']['qasm'] if meta['coqis']['compile'] else '',
+               'status': status,
+               }
+        return ret
 
     def sysinfo(self):
         return self.server.sysinfo(False)
 
     def snr(self, data):
         return data
```

## quark/envelope/router.py

```diff
@@ -86,28 +86,28 @@
     # print(result.keys(),result['meta'].keys())
 
     quafu = result['meta'].get('coqis', {})
     # savefig(result)
     if not quafu.get('token', ''):
         return
 
-    status, new, raw = QuarkProxy.process(result)
+    res = QuarkProxy.process(result)
 
     rshot = 0
     post_data = {"task_id": quafu['eid'],
-                 "status": status,
+                 "status": res['status'],
                  "raw": "",
                  "res": "",
-                 'transpiled_circuit': quafu['qasm'] if quafu['compile'] else '',
+                 'transpiled_circuit': res['transpiled'],
                  "server": quafu['systemid']}
 
-    if status == 'finished':
-        rshot = sum(new.values())
-        post_data.update({"raw": str(raw).replace("\'", "\""),
-                          "res": str(new).replace("\'", "\""),
+    if res['status'] == 'finished':
+        rshot = sum(res['count'].values())
+        post_data.update({"raw": str(res['count']).replace("\'", "\""),
+                          "res": str(res['corrected']).replace("\'", "\""),
                           })
 
     try:
         resp = requests.post(url=f"http://124.70.54.59/qbackend/scq_result/",
                              data=post_data,
                              headers={'api_token': quafu['token']})
         logger.info(f'Back to quafu: {resp.text} {rshot}')
```

## Comparing `vios-2.2.6.dist-info/LICENSE` & `vios-2.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-2.2.6.dist-info/METADATA` & `vios-2.2.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 2.2.6
+Version: 2.2.7
 Summary: runtime requirements for systemq
 Author-email: YL Feng <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-2.2.6.dist-info/RECORD` & `vios-2.2.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 quark/__main__.py,sha256=ky318p_RHmGRdMyzIL2meu-JOgqzRrH-hWfFvhceZGE,2858
-quark/proxy.py,sha256=lxnWpquNyqcE8NLNTqJCF5mynzSrmaqTFNahfSyErrc,18341
+quark/proxy.py,sha256=VipnCD1gmbkn-37HmW1cVfGDTQhXxbFwruh40_RkA-8,18428
 quark/app/__init__.py,sha256=MjOh4mkjvwFzEEfPNv-dMOcoktAtYCBtl-P5_UA7MzQ,18861
 quark/app/_data.py,sha256=EGGTD2FrZ8vlbMh4jlmWhYk4fEG3FolGoWaQ26qxoss,2575
 quark/app/demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
 quark/app/task.py,sha256=QEZuNia59sLEWa8pl2XIjItx2NismSTPZFnFt8-90HM,9043
 quark/app/uapi.py,sha256=itjEa89SUXozZqBGLH-3o4mKtRssNQODDj60knC-cGE,5876
 quark/driver/VirtualDevice.py,sha256=Cswl_ykFhIsocGV6Okh_YS1b48FeLm2fh1ruXqmNoyw,7914
 quark/driver/__init__.py,sha256=p1pVx1xTulBT8-qdp_zJ859tdIsA92XdvwrkqcVHL4s,386
@@ -12,14 +12,14 @@
 quark/driver/common/quantity.py,sha256=fV9DMmjys44efe7TTvzXmFdozqGdS2QUm23wtfLxeBE,4663
 quark/driver/common/visadriver.py,sha256=LRyYDBF0u9EYf6p47LeGGKhx9pHiq4pux_pzDakaICY,5432
 quark/envelope/__init__.py,sha256=5_cs0tZ7mV4GjOsY2isx8sUQu4u6Y3WN-9DUGG27SQM,1188
 quark/envelope/assembler.py,sha256=ENwX7FutJvpg6_Wcm42_Zx-ddq40JozuYqHPwJp09ZA,15111
 quark/envelope/calculator.py,sha256=0rZAA46sWh_X8wOBmpBvmljqCV53ID4VHPX1cE_abEc,4322
 quark/envelope/device.py,sha256=5E3oWZ84IYnQdzlmzltgPyayYz_au7p7UIbFVpJUa0Q,1106
 quark/envelope/processor.py,sha256=uMIwu83a4SDZVM3OE5_WrBya_4jxtdcXPd6pYa0osrk,3758
-quark/envelope/router.py,sha256=YuqzlKNIsiOKe5tA5d2XwU3wOYcy_yLgyNz68Ymjyzs,4216
+quark/envelope/router.py,sha256=wVx-rWnCZg_BrPV8fja4kjI5jiQ5vEoAyXsCtDpdBdA,4224
 quark/envelope/systemq.py,sha256=QAaHLv68C9UjMp9qHt9t-HJkOTpCkbHZTlNVOsAzIBc,2841
-vios-2.2.6.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
-vios-2.2.6.dist-info/METADATA,sha256=4LG8cXvPPVHcpftKxe2SDWUGNDB95GmiqxIFmWR6FzM,1215
-vios-2.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vios-2.2.6.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
-vios-2.2.6.dist-info/RECORD,,
+vios-2.2.7.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
+vios-2.2.7.dist-info/METADATA,sha256=LM4Zt8MGYdBEmXNSjBtgEqzEJvCKn2xMYwcK_YP_B5s,1215
+vios-2.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vios-2.2.7.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
+vios-2.2.7.dist-info/RECORD,,
```

