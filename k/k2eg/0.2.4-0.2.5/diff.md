# Comparing `tmp/k2eg-0.2.4.tar.gz` & `tmp/k2eg-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k2eg-0.2.4.tar", last modified: Fri Jan 26 22:04:33 2024, max compression
+gzip compressed data, was "k2eg-0.2.5.tar", last modified: Thu Apr  4 03:41:34 2024, max compression
```

## Comparing `k2eg-0.2.4.tar` & `k2eg-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:04:33.714870 k2eg-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-26 22:04:33.714870 k2eg-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-01-26 22:04:10.000000 k2eg-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:04:33.710870 k2eg-0.2.4/k2eg/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:04:33.714870 k2eg-0.2.4/k2eg/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/cli/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/cli/put.py
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2024-01-26 22:04:10.000000 k2eg-0.2.4/k2eg/dml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:04:33.714870 k2eg-0.2.4/k2eg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-26 22:04:33.000000 k2eg-0.2.4/k2eg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-26 22:04:33.000000 k2eg-0.2.4/k2eg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 22:04:33.000000 k2eg-0.2.4/k2eg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-26 22:04:33.000000 k2eg-0.2.4/k2eg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-26 22:04:33.000000 k2eg-0.2.4/k2eg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-26 22:04:33.000000 k2eg-0.2.4/k2eg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-26 22:04:15.000000 k2eg-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 22:04:33.714870 k2eg-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:04:33.714870 k2eg-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-26 22:04:10.000000 k2eg-0.2.4/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-01-26 22:04:10.000000 k2eg-0.2.4/tests/test_dml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 03:41:34.120003 k2eg-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 03:41:16.000000 k2eg-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.116003 k2eg-0.2.5/k2eg/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/k2eg/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/cli/put.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15793 2024-04-04 03:41:16.000000 k2eg-0.2.5/k2eg/dml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/k2eg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 03:41:34.000000 k2eg-0.2.5/k2eg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 03:41:20.000000 k2eg-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:41:34.120003 k2eg-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:41:34.120003 k2eg-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 03:41:16.000000 k2eg-0.2.5/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-04 03:41:16.000000 k2eg-0.2.5/tests/test_dml.py
```

### Comparing `k2eg-0.2.4/PKG-INFO` & `k2eg-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2eg
-Version: 0.2.4
+Version: 0.2.5
 Summary: A k2eg library
 Author-email: Claudio Bisegni <bisegni@slac.stanford.edu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `k2eg-0.2.4/README.md` & `k2eg-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.4/k2eg/broker.py` & `k2eg-0.2.5/k2eg/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,18 +119,18 @@
             'bootstrap.servers': self.__config.get(
                 self.__enviroment_set, 'kafka_broker_url'
                 ), 
             'group.id': group_name,
             'group.instance.id': app_name+'_'+app_instance_unique_id,
             'auto.offset.reset': 'latest',
             'enable.auto.commit': 'true',
-            'topic.metadata.refresh.interval.ms': '60000'
+            'topic.metadata.refresh.interval.ms': '60000',
         }
         if enable_kafka_debug is True:
-            config_consumer['debug'] = 'consumer,cgrp,topic' #fetch
+            config_consumer['debug'] = 'consumer,fetch'
 
         self.__consumer = Consumer(config_consumer)
         config_producer = {
             'bootstrap.servers': self.__config.get(
                 self.__enviroment_set, 'kafka_broker_url'
                 ),
             #'debug': 'consumer,cgrp,topic,fetch',
@@ -160,15 +160,15 @@
         for p in partitions:
             logging.debug(f"Joined topic {p.topic} with partition {p.partition}")
             if p.topic == self.__reply_topic:
                 self.__reply_topic_joined = True
                 self.__reply_partition_assigned.set()
                 #if p.offset==-1 or p.offset==-1001:
                 logging.debug(f'Force to reading from the end for topic: {p.topic}')
-                p.offset = OFFSET_END
+                #p.offset = OFFSET_END
             else:
                 try:
                     low, high = consumer.get_watermark_offsets(p)
                     logging.debug(f'Found max and min [{high},{low}] index for topic: {p.topic}')
                     # in this case we have to go one index behing to start reading from the
                     # last element in the queue
                     if high >= 1:
@@ -232,15 +232,18 @@
             logging.error(e)
        
     def get_next_message(self, timeout = 0.300):
         message = self.__consumer.poll(timeout=timeout)
         # give a chanche to update metadata ofr pending topics
         self.__topic_checker.update_metadata(self.__consumer)
         if message is None:
-            return None    
+            return None
+        # tp = TopicPartition(message.topic(), message.partition(), message.offset() + 1)
+        # # Asynchronous commit
+        # self.__consumer.commit(offsets=[tp], asynchronous=True)
         if message.error():
             if message.error().code() == KafkaError.UNKNOWN_TOPIC_OR_PART:
                 logging.info(f"Topic {message.topic()} not found, add it to checker")
                 self.__topic_checker.add_topic(message.topic())
         return message
     
     def commit_current_fetched_message(self):
```

### Comparing `k2eg-0.2.4/k2eg/cli/__main__.py` & `k2eg-0.2.5/k2eg/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.4/k2eg/cli/get.py` & `k2eg-0.2.5/k2eg/cli/get.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.4/k2eg/cli/monitor.py` & `k2eg-0.2.5/k2eg/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.4/k2eg/cli/put.py` & `k2eg-0.2.5/k2eg/cli/put.py`

 * *Files identical despite different names*

### Comparing `k2eg-0.2.4/k2eg/dml.py` & `k2eg-0.2.5/k2eg/dml.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import msgpack
 import logging
 import threading
 from readerwriterlock import rwlock
 from confluent_kafka import KafkaError
 from typing import Callable
 from k2eg.broker import Broker
+from concurrent.futures import ThreadPoolExecutor
 
 _protocol_regex = r"^(pva?|ca)://((?:[A-Za-z0-9-_:]+(?:\.[A-Za-z0-9-_]+)*))$"
 
 def _filter_pv_uri(uri: str):
     match = re.match(_protocol_regex, uri)
     if match:
         return match.group(1), match.group(2)
@@ -110,55 +111,60 @@
                 elif st == "msgpack-compact":
                     msg_id, converted_msg = self.__from_msgpack_compack(
                         msg.value()
                         )
                 break   
         return msg_id, converted_msg
 
-
+    def process_event(self, topic_name, msg_id, decoded_message):
+        logging.debug(f"received event on topic {topic_name}")
+        self.__monitor_pv_handler[msg_id](msg_id, decoded_message)
+    
     def __consumer_handler(self):
         """ Consume message form kafka consumer
         after the message has been consumed the header 'k2eg-ser-type' is checked 
         for find the serialization:
             json, 
             msgpack, 
             msgpack-compact
         """
-        while self.__consume_data:
-        #for msg in self.__consumer:
-            message = self.__broker.get_next_message()
-            if message is None: 
-                continue
-            if message.error():
-                if message.error().code() == KafkaError._PARTITION_EOF:
-                    # End of partition event
-                    logging.error(
-                        f"{message.topic()} [{message.partition()}]reached "+
-                        f"end at offset {message.offset()}"
-                    )
-                else:
-                    continue
-            else:
-                was_a_reply = False
-                #msg_id could be a reply id or pv name
-                msg_id, decoded_message = self.__decode_message(message)
-                if msg_id is None or decoded_message is None:
+        with  ThreadPoolExecutor(max_workers=10) as executor:
+            while self.__consume_data:
+                message = self.__broker.get_next_message()
+                if message is None: 
                     continue
-                with self.reply_wait_condition:
-                    was_a_reply = msg_id in self.reply_message
-                    if was_a_reply is True:
-                        logging.debug(f"received reply on topic {message.topic()}")
-                        self.reply_message[msg_id] = decoded_message
-                        self.reply_wait_condition.notifyAll()
-                    elif msg_id in self.__monitor_pv_handler:
-                        logging.debug(f"received event on topic {message.topic()}")
-                        self.__monitor_pv_handler[msg_id](
-                            msg_id, decoded_message[msg_id]
-                            )
-                self.__broker.commit_current_fetched_message()
+                if message.error():
+                    if message.error().code() == KafkaError._PARTITION_EOF:
+                        # End of partition event
+                        logging.error(
+                            f"{message.topic()} [{message.partition()}]reached "+
+                            f"end at offset {message.offset()}"
+                        )
+                    else:
+                        continue
+                else:
+                    was_a_reply = False
+                    #msg_id could be a reply id or pv name
+                    msg_id, decoded_message = self.__decode_message(message)
+                    if msg_id is None or decoded_message is None:
+                        continue
+                    with self.reply_wait_condition:
+                        was_a_reply = msg_id in self.reply_message
+                        if was_a_reply is True:
+                            # print(f"message received from topic: {message.topic()} offset: {message.offset()}")
+                            logging.debug(f"received reply on topic {message.topic()}")
+                            self.reply_message[msg_id] = decoded_message
+                            self.reply_wait_condition.notifyAll()
+                        elif msg_id in self.__monitor_pv_handler:
+                                executor.submit(
+                                    self.process_event,
+                                    message.topic(),
+                                    msg_id,
+                                    decoded_message[msg_id]
+                                )
 
     def parse_pv_url(self, pv_url):
         protocol, pv_name = _filter_pv_uri(pv_url)
         if protocol is None  or pv_name is None:
             raise ValueError(
                 "The url is not well formed"
             )
```

### Comparing `k2eg-0.2.4/k2eg.egg-info/PKG-INFO` & `k2eg-0.2.5/k2eg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k2eg
-Version: 0.2.4
+Version: 0.2.5
 Summary: A k2eg library
 Author-email: Claudio Bisegni <bisegni@slac.stanford.edu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `k2eg-0.2.4/pyproject.toml` & `k2eg-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "k2eg"
-version = "0.2.4"
+version = "0.2.5"
 description = "A k2eg library"
 readme = "README.md"
 authors = [{name = "Claudio Bisegni", email = "bisegni@slac.stanford.edu"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `k2eg-0.2.4/tests/test_dml.py` & `k2eg-0.2.5/tests/test_dml.py`

 * *Files 13% similar despite different names*

```diff
@@ -85,46 +85,14 @@
         while received_message is None and retry < 20:
             retry = retry+1
             time.sleep(2)
     finally:
         k.stop_monitor("channel:ramp:ramp")
     assert received_message is not None, "value should not be None"
 
-# def test_k2eg_monitor_on_already_started_mon():
-#     last_received_data = None
-#     previous_event_data = None
-#     def monitor_handler(pv_name, new_value):
-#         nonlocal last_received_data
-#         logging.info(f"Received event from {pv_name}")
-#         last_received_data = new_value
-#     try:
-#         retry = 0
-#         #this will emit only one message
-#         k.monitor('pva://variable:a', monitor_handler)
-#         while last_received_data is None and retry < 50:
-#             retry = retry+1
-#             time.sleep(2)
-        
-#         assert last_received_data is not None, "value should not be None"
-#         # now stop the consume
-#         k.stop_monitor('variable:a')
-#         logging.info("retry to reread form the same pv should receive the same last record")
-#         previous_event_data = last_received_data
-#         #reset variable for receive data
-#         last_received_data = None
-#         retry = 0
-#         k.monitor('pva://variable:a', monitor_handler)
-#         while last_received_data is None and retry < 50:
-#             retry = retry+1
-#             time.sleep(2)
-#     finally:
-#         k.stop_monitor("variable:a")
-#     # now the two variable previous_event and last_received_method
-#     # should be the same
-#     assert (json.dumps(last_received_data) == json.dumps(previous_event_data)), "Dictionary need to be the same"
 
 def test_k2eg_monitor_wrong():
     retry = 0
     received_message = None
 
     def monitor_handler(pv_name, new_value):
         nonlocal received_message
@@ -170,14 +138,50 @@
     k.put("pva://variable:a", 2)
     k.put("pva://variable:b", 2)
     #give some time to ioc to update
     time.sleep(1)
     res_get = k.get("pva://variable:sum")
     assert res_get['value'] == 4, "value should not be 0"
 
+# def test_multiple_put():
+#     def monitor_handler(pv_name, new_value):
+#        pass
+        
+#     monitor_pv = [
+#                     'ca://SOLN:IN20:121:BACT',
+#                     'ca://QUAD:IN20:121:BACT',
+#                     'ca://QUAD:IN20:122:BACT',
+#                     'ca://ACCL:IN20:300:L0A_PDES',
+#                     'ca://ACCL:IN20:400:L0B_PDES',
+#                     'ca://ACCL:IN20:300:L0A_ADES',
+#                     'ca://ACCL:IN20:400:L0B_ADES',
+#                     'ca://QUAD:IN20:361:BACT',
+#                     'ca://QUAD:IN20:371:BACT',
+#                     'ca://QUAD:IN20:425:BACT',
+#                     'ca://QUAD:IN20:441:BACT',
+#                     'ca://QUAD:IN20:511:BACT',
+#                     'ca://QUAD:IN20:525:BACT',
+#                     'ca://FBCK:BCI0:1:CHRG_S',
+#                     'ca://CAMR:IN20:186:XRMS',
+#                     'ca://CAMR:IN20:186:YRMS'
+#                     ]
+#     k.monitor_many(monitor_pv, monitor_handler)
+#     monitor_put = {
+#         'LUME:MLFLOW:SIGMA_X': '-99830.6330126242',
+#         'LUME:MLFLOW:SIGMA_Y': '225322.341204345',
+#         'LUME:MLFLOW:SIGMA_Z': '10352.2788770893'
+#     }
+#     for key, value in monitor_put.items():  # Add .items() method to iterate over key-value pairs
+#         print(f"Output: {key}, Value: {value}")  # Update print statement to use f-strings
+#         try:
+#             msg = k.put("pva://" + key, value, 1000000)
+#             print(f"Message: {msg}")
+#         except Exception as e:
+#             print(f"An error occurred: {e}")
+
 def test_put_timeout():
     with pytest.raises(k2eg.OperationTimeout, 
                     match=r"Timeout.*"):
                     k.put("pva://bad:pv:name", 0, timeout=0.5)
 
 
 def test_put_wrong_device_timeout():
```

