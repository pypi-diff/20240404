# Comparing `tmp/hijiki-1.0.56.tar.gz` & `tmp/hijiki-1.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijiki-1.0.56.tar", last modified: Tue Mar 19 20:47:41 2024, max compression
+gzip compressed data, was "hijiki-1.0.57.tar", last modified: Thu Apr  4 18:24:56 2024, max compression
```

## Comparing `hijiki-1.0.56.tar` & `hijiki-1.0.57.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.758116 hijiki-1.0.56/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 20:46:43.000000 hijiki-1.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-19 20:47:41.758116 hijiki-1.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-19 20:46:43.000000 hijiki-1.0.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.754115 hijiki-1.0.56/hijiki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.758116 hijiki-1.0.56/hijiki/broker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/broker/broker_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/broker/hijiki_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/broker/hijiki_rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.758116 hijiki-1.0.56/hijiki/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/decorator/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/hijiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.758116 hijiki-1.0.56/hijiki/publisher/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/publisher/Publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 20:46:43.000000 hijiki-1.0.56/hijiki/publisher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.758116 hijiki-1.0.56/hijiki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-19 20:47:41.000000 hijiki-1.0.56/hijiki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-19 20:47:41.000000 hijiki-1.0.56/hijiki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 20:47:41.000000 hijiki-1.0.56/hijiki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-19 20:47:41.000000 hijiki-1.0.56/hijiki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-19 20:47:41.000000 hijiki-1.0.56/hijiki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 20:47:41.758116 hijiki-1.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-19 20:47:09.000000 hijiki-1.0.56/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:47:41.758116 hijiki-1.0.56/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-19 20:46:43.000000 hijiki-1.0.56/tests/test_broker_data_server_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-19 20:46:43.000000 hijiki-1.0.56/tests/test_publisher_consumer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 18:23:27.000000 hijiki-1.0.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 18:24:56.162686 hijiki-1.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-04 18:23:27.000000 hijiki-1.0.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.158686 hijiki-1.0.57/hijiki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.158686 hijiki-1.0.57/hijiki/broker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/broker_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/hijiki_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/broker/hijiki_rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.158686 hijiki-1.0.57/hijiki/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/decorator/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/hijiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/hijiki/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/publisher/Publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:27.000000 hijiki-1.0.57/hijiki/publisher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/hijiki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 18:24:56.000000 hijiki-1.0.57/hijiki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:24:56.162686 hijiki-1.0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-04 18:24:02.000000 hijiki-1.0.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:24:56.162686 hijiki-1.0.57/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-04 18:23:27.000000 hijiki-1.0.57/tests/test_broker_data_server_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-04 18:23:27.000000 hijiki-1.0.57/tests/test_publisher_consumer_test.py
```

### Comparing `hijiki-1.0.56/LICENSE` & `hijiki-1.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.56/PKG-INFO` & `hijiki-1.0.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.56
+Version: 1.0.57
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
```

### Comparing `hijiki-1.0.56/README.md` & `hijiki-1.0.57/README.md`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.56/hijiki/broker/broker_data.py` & `hijiki-1.0.57/hijiki/broker/broker_data.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.56/hijiki/broker/hijiki_rabbit.py` & `hijiki-1.0.57/hijiki/broker/hijiki_rabbit.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,16 +64,18 @@
         return self
 
     def init_queues(self, ):
         for q in self.queue_exchanges:
             name = q.name
             if name not in self.queues:
                 self.queues[name] = []
+                self.queues[name+ "_dlq"] = []
             if name not in self.callbacks:
                 self.callbacks[name] = []
+                self.callbacks[name + "_dlq"] = []
 
             logger.debug("Setting up %s" % name)
             routing_key = "*"
 
             task_exchange = Exchange(f'{q.exchange_name}', type='topic')
             task_exchange_dlq = Exchange(f'{q.exchange_name}_dlq', type='topic')
 
@@ -89,17 +91,18 @@
                               task_exchange_dlq,
                               routing_key=routing_key,
                               queue_arguments={'x-queue-type': 'quorum'})
 
             queue_dlq.bind(self.connection).declare()
 
             self.queues[name].append(queue)
+            self.queues[name + "_dlq"].append(queue_dlq)
 
     def _wrap_function(self, function, callback, queue_name, task=False):
-
+        
         self.callbacks[queue_name].append(callback)
 
         # The function returned by the decorator don't really do
         # anything.  The process_msg callback added to the consumer
         # is what actually responds to messages  from the client
         # on this particular queue.
 
@@ -135,12 +138,22 @@
                 logger.debug("Ack'ing message.")
                 message.ack()
 
         return self._wrap_function(
             func, process_message, queue_name, task=True)
 
     def run(self):
+        consumers_without_callbacks = [
+            key 
+            for (key, callbacks) in self.callbacks.items()
+            if not callbacks
+        ]
+
+        for key in consumers_without_callbacks:
+            self.callbacks.pop(key)
+            self.queues.pop(key)
+
         try:
             self.worker = Worker(self.connection, self)
             self.worker.run()
         except KeyboardInterrupt:
             print('bye bye')
```

### Comparing `hijiki-1.0.56/hijiki/decorator/worker.py` & `hijiki-1.0.57/hijiki/decorator/worker.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.56/hijiki/publisher/Publisher.py` & `hijiki-1.0.57/hijiki/publisher/Publisher.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.56/hijiki.egg-info/PKG-INFO` & `hijiki-1.0.57/hijiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.56
+Version: 1.0.57
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
```

### Comparing `hijiki-1.0.56/hijiki.egg-info/SOURCES.txt` & `hijiki-1.0.57/hijiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.56/tests/test_broker_data_server_exists.py` & `hijiki-1.0.57/tests/test_broker_data_server_exists.py`

 * *Files identical despite different names*

