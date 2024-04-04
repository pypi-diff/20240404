# Comparing `tmp/spirems-0.1.2-py3-none-any.whl.zip` & `tmp/spirems-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,19 @@
-Zip file size: 23111 bytes, number of entries: 31
--rw-rw-rw-  2.0 fat      546 b- defN 24-Apr-04 14:23 spirems/__init__.py
+Zip file size: 26751 bytes, number of entries: 37
+-rw-rw-rw-  2.0 fat      546 b- defN 24-Apr-04 14:30 spirems/__init__.py
 -rw-rw-rw-  2.0 fat      878 b- defN 24-Mar-31 06:11 spirems/error_code.py
 -rw-rw-rw-  2.0 fat     1009 b- defN 24-Apr-04 14:11 spirems/log.py
 -rw-rw-rw-  2.0 fat     4807 b- defN 24-Mar-31 09:46 spirems/msg_helper.py
 -rw-rw-rw-  2.0 fat     6597 b- defN 24-Apr-04 14:09 spirems/publisher.py
 -rw-rw-rw-  2.0 fat    13447 b- defN 24-Apr-04 14:05 spirems/server.py
 -rw-rw-rw-  2.0 fat     5255 b- defN 24-Mar-31 18:32 spirems/sms.py
 -rw-rw-rw-  2.0 fat     5462 b- defN 24-Apr-04 14:12 spirems/subscriber.py
+-rw-rw-rw-  2.0 fat       48 b- defN 24-Apr-04 14:27 spirems/image_io/__init__.py
+-rw-rw-rw-  2.0 fat     1396 b- defN 24-Apr-02 11:34 spirems/image_io/adaptor.py
+-rw-rw-rw-  2.0 fat      549 b- defN 24-Apr-02 11:34 spirems/image_io/recv_testcase.py
 -rw-rw-rw-  2.0 fat       17 b- defN 24-Mar-31 07:05 spirems/logs/README.md
 -rw-rw-rw-  2.0 fat       54 b- defN 24-Mar-25 14:45 spirems/msgs/_sys_msgs/HeartBeat.json
 -rw-rw-rw-  2.0 fat       99 b- defN 24-Mar-25 17:12 spirems/msgs/_sys_msgs/Publisher.json
 -rw-rw-rw-  2.0 fat       82 b- defN 24-Mar-25 17:07 spirems/msgs/_sys_msgs/Result.json
 -rw-rw-rw-  2.0 fat       57 b- defN 24-Mar-27 09:42 spirems/msgs/_sys_msgs/SmsTopicList.json
 -rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-25 17:13 spirems/msgs/_sys_msgs/Subscriber.json
 -rw-rw-rw-  2.0 fat       52 b- defN 24-Mar-27 15:25 spirems/msgs/_sys_msgs/Suspend.json
@@ -20,14 +23,17 @@
 -rw-rw-rw-  2.0 fat       67 b- defN 24-Mar-24 10:30 spirems/msgs/std_msgs/Boolean.json
 -rw-rw-rw-  2.0 fat       79 b- defN 24-Mar-24 10:30 spirems/msgs/std_msgs/BooleanMultiArray.json
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Mar-24 10:35 spirems/msgs/std_msgs/Null.json
 -rw-rw-rw-  2.0 fat       64 b- defN 24-Mar-26 11:39 spirems/msgs/std_msgs/Number.json
 -rw-rw-rw-  2.0 fat       76 b- defN 24-Mar-24 10:30 spirems/msgs/std_msgs/NumberMultiArray.json
 -rw-rw-rw-  2.0 fat       63 b- defN 24-Mar-24 10:30 spirems/msgs/std_msgs/String.json
 -rw-rw-rw-  2.0 fat       75 b- defN 24-Mar-24 10:30 spirems/msgs/std_msgs/StringMultiArray.json
--rw-rw-rw-  2.0 fat     5241 b- defN 24-Apr-04 14:23 spirems-0.1.2.data/scripts/sms.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-04 14:23 spirems-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1248 b- defN 24-Apr-04 14:23 spirems-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 14:23 spirems-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-04 14:23 spirems-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2630 b- defN 24-Apr-04 14:23 spirems-0.1.2.dist-info/RECORD
-31 files, 59944 bytes uncompressed, 18825 bytes compressed:  68.6%
+-rw-rw-rw-  2.0 fat       48 b- defN 24-Apr-04 14:27 spirems/sys_monit/__init__.py
+-rw-rw-rw-  2.0 fat     2271 b- defN 24-Apr-03 02:38 spirems/sys_monit/a2rl_sys_monit.py
+-rw-rw-rw-  2.0 fat     3487 b- defN 24-Apr-03 02:38 spirems/sys_monit/psutil_pub.py
+-rw-rw-rw-  2.0 fat     5241 b- defN 24-Apr-04 14:31 spirems-0.1.3.data/scripts/sms.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-04 14:31 spirems-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1248 b- defN 24-Apr-04 14:31 spirems-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 14:31 spirems-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-04 14:31 spirems-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3150 b- defN 24-Apr-04 14:31 spirems-0.1.3.dist-info/RECORD
+37 files, 68263 bytes uncompressed, 21643 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -18,14 +18,23 @@
 
 Filename: spirems/sms.py
 Comment: 
 
 Filename: spirems/subscriber.py
 Comment: 
 
+Filename: spirems/image_io/__init__.py
+Comment: 
+
+Filename: spirems/image_io/adaptor.py
+Comment: 
+
+Filename: spirems/image_io/recv_testcase.py
+Comment: 
+
 Filename: spirems/logs/README.md
 Comment: 
 
 Filename: spirems/msgs/_sys_msgs/HeartBeat.json
 Comment: 
 
 Filename: spirems/msgs/_sys_msgs/Publisher.json
@@ -69,26 +78,35 @@
 
 Filename: spirems/msgs/std_msgs/String.json
 Comment: 
 
 Filename: spirems/msgs/std_msgs/StringMultiArray.json
 Comment: 
 
-Filename: spirems-0.1.2.data/scripts/sms.py
+Filename: spirems/sys_monit/__init__.py
+Comment: 
+
+Filename: spirems/sys_monit/a2rl_sys_monit.py
+Comment: 
+
+Filename: spirems/sys_monit/psutil_pub.py
+Comment: 
+
+Filename: spirems-0.1.3.data/scripts/sms.py
 Comment: 
 
-Filename: spirems-0.1.2.dist-info/LICENSE
+Filename: spirems-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: spirems-0.1.2.dist-info/METADATA
+Filename: spirems-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: spirems-0.1.2.dist-info/WHEEL
+Filename: spirems-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: spirems-0.1.2.dist-info/top_level.txt
+Filename: spirems-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: spirems-0.1.2.dist-info/RECORD
+Filename: spirems-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spirems/__init__.py

```diff
@@ -6,13 +6,13 @@
 from spirems.subscriber import Subscriber
 from spirems.publisher import Publisher
 from spirems.server import Server
 from spirems.image_io.adaptor import cvimg2sms, sms2cvimg
 from spirems.msg_helper import get_all_msg_types
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 __all__ = [
     'a2rl_pub', 'a2rl_sub', 'cvimg2sms', 'cvimg2sms', 'get_all_msg_types',
     'Subscriber', 'Publisher', 'Server'
 ]
```

## Comparing `spirems-0.1.2.data/scripts/sms.py` & `spirems-0.1.3.data/scripts/sms.py`

 * *Files identical despite different names*

## Comparing `spirems-0.1.2.dist-info/LICENSE` & `spirems-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spirems-0.1.2.dist-info/METADATA` & `spirems-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spirems
-Version: 0.1.2
+Version: 0.1.3
 Author: jin&team
 Author-email: renjin@bit.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `spirems-0.1.2.dist-info/RECORD` & `spirems-0.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-spirems/__init__.py,sha256=dB-kunPDOa51to404RBrOMBvciCtmgBUhB0Iv87AmeY,546
+spirems/__init__.py,sha256=BkYEwk3FUC0Rn5FuKcRT4ucDvgtIGI7S__ZiHOCQSNo,546
 spirems/error_code.py,sha256=CrFS5cLLLrLKRxGoTGoMeW4w9f8TjmVYZ-7FdHmZdp0,878
 spirems/log.py,sha256=JujtjV1_AQWNdkEmnooBG8zCzXwl6ykl4J5H_BkAtQ8,1009
 spirems/msg_helper.py,sha256=e6rNT3mjiQy_7VH6oSj6M2PQokPuNujiWBvN0MADiBI,4807
 spirems/publisher.py,sha256=KqSIj5NAOxE6mFNRDwQdH9UMnPzix4bpnyXwI5lXoVY,6597
 spirems/server.py,sha256=DlxlEOg8klelmT31JEQoAVw1s6KQFlZljB0Z8H1akmk,13447
 spirems/sms.py,sha256=4uAFAU8W-wDOTVs6UitoQfzUWkmJeU55mIcEgrUqAGs,5255
 spirems/subscriber.py,sha256=75usIv27l-rYhHLfiwS9wEmFRnrci_h8xSQcioBgMJA,5462
+spirems/image_io/__init__.py,sha256=M11gWrr6dDI3LEeCVFCvvONgzfKA8qxwPtMNbnbW1AA,48
+spirems/image_io/adaptor.py,sha256=YyLEXYV43YHHz9T1gMCPmcVTdVsllHHfVmXxtrCjaPU,1396
+spirems/image_io/recv_testcase.py,sha256=1mVqLjAvsjeJL2osUsq4iyppvNSPulRppq9lCBJfyRY,549
 spirems/logs/README.md,sha256=-A-iurCwjSy1aV-LUkB1QZa3ORQifwKkclC3yMh2N9U,17
 spirems/msgs/_sys_msgs/HeartBeat.json,sha256=36MqpL_AjS3SDBzbCXGZf0vlGmqfqMnQWHnmjJLrKKs,54
 spirems/msgs/_sys_msgs/Publisher.json,sha256=6XQMxBGWvsey7j59eY7BEPHgtEsFA3LffQ57F4Z_gJw,99
 spirems/msgs/_sys_msgs/Result.json,sha256=sl7DnthrkRaP6_Ur70zdg-G64QUChvnkkCZpBaMsh-0,82
 spirems/msgs/_sys_msgs/SmsTopicList.json,sha256=AKBGrqD5rnAaFKzA6zy9cW0V_JpQl8Q7oY4j_UBtX7E,57
 spirems/msgs/_sys_msgs/Subscriber.json,sha256=zzxyDaNmGnAbSwAvmEPHOkIB2mjy82OfhVQN8vaa-NA,100
 spirems/msgs/_sys_msgs/Suspend.json,sha256=OB-vSPGCh4zFZlUjco6RYX-G3fszRV-M231QdTxEfoM,52
@@ -19,13 +22,16 @@
 spirems/msgs/std_msgs/Boolean.json,sha256=a5V2SeTxwamfkdtxysAUWPCUxT6NrwrCurW4-jN43Ug,67
 spirems/msgs/std_msgs/BooleanMultiArray.json,sha256=veLyvBpYFztR_7ZyO4ICnvxiT5eWCGaP3yrrJHbLtBY,79
 spirems/msgs/std_msgs/Null.json,sha256=MGBvN6uIpgEpaYZQhgUfFRHXBpx7FsvngISqBvBciHI,48
 spirems/msgs/std_msgs/Number.json,sha256=cZ8O3NrZ8pFE3cnEnGhe8jbye5j6HHSoQiV_s9xw4_Q,64
 spirems/msgs/std_msgs/NumberMultiArray.json,sha256=doBT3ukrotfw0UpcFqWPDFkLsxctpOKDtX8HkbZ6aNA,76
 spirems/msgs/std_msgs/String.json,sha256=jcBACqMkZOe3wW59EupJkB7ZzJ7hXhZ_10NHHRUccwQ,63
 spirems/msgs/std_msgs/StringMultiArray.json,sha256=PN8fg_P5Zqa7BjBaptMQyoR_IuOppAetGOsg-Nvbpuk,75
-spirems-0.1.2.data/scripts/sms.py,sha256=eaqngSfCzgPtkBXjw0nZ82o17pLHW2ZPDxXku6xkR94,5241
-spirems-0.1.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-spirems-0.1.2.dist-info/METADATA,sha256=FED1iYlKG8imGTfyp6aoUX5w1LHomt7MinOCyXqADxU,1248
-spirems-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-spirems-0.1.2.dist-info/top_level.txt,sha256=ra9zu_vB-BRVXDwvqhouFCHIwnalKkMGq3JmTZijtmE,8
-spirems-0.1.2.dist-info/RECORD,,
+spirems/sys_monit/__init__.py,sha256=M11gWrr6dDI3LEeCVFCvvONgzfKA8qxwPtMNbnbW1AA,48
+spirems/sys_monit/a2rl_sys_monit.py,sha256=KfP0Vd_D3oFX-ZACm6OmuWRI6tVl0vR-FisMW28A1BI,2271
+spirems/sys_monit/psutil_pub.py,sha256=PQWs5vAq916xPNyGIPtWDJ1MJZLzkFLqgsDHJ5pJKH4,3487
+spirems-0.1.3.data/scripts/sms.py,sha256=eaqngSfCzgPtkBXjw0nZ82o17pLHW2ZPDxXku6xkR94,5241
+spirems-0.1.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+spirems-0.1.3.dist-info/METADATA,sha256=iTzg4npUNbTSWvP4u-kzCnT3VPBo2JAOJkXZ_Yq7UpY,1248
+spirems-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+spirems-0.1.3.dist-info/top_level.txt,sha256=ra9zu_vB-BRVXDwvqhouFCHIwnalKkMGq3JmTZijtmE,8
+spirems-0.1.3.dist-info/RECORD,,
```

