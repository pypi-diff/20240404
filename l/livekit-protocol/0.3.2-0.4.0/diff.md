# Comparing `tmp/livekit-protocol-0.3.2.tar.gz` & `tmp/livekit-protocol-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-protocol-0.3.2.tar", last modified: Wed Mar 27 17:01:04 2024, max compression
+gzip compressed data, was "livekit-protocol-0.4.0.tar", last modified: Thu Apr  4 00:52:23 2024, max compression
```

## Comparing `livekit-protocol-0.3.2.tar` & `livekit-protocol-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:04.152536 livekit-protocol-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-27 17:01:04.148536 livekit-protocol-0.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:04.144535 livekit-protocol-0.3.2/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:04.148536 livekit-protocol-0.3.2/livekit/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/analytics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21348 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/egress.py
--rw-r--r--   0 runner    (1001) docker     (127)    31454 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/egress.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/ingress.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/ingress.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16346 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29005 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/room.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/livekit/protocol/webhook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:04.148536 livekit-protocol-0.3.2/livekit_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-27 17:01:04.000000 livekit-protocol-0.3.2/livekit_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-27 17:01:04.000000 livekit-protocol-0.3.2/livekit_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:01:04.000000 livekit-protocol-0.3.2/livekit_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 17:01:04.000000 livekit-protocol-0.3.2/livekit_protocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 17:01:04.000000 livekit-protocol-0.3.2/livekit_protocol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 17:01:04.152536 livekit-protocol-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-27 17:00:52.000000 livekit-protocol-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.287329 livekit-protocol-0.4.0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/livekit/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/analytics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/egress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/egress.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/ingress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/ingress.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18390 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31005 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/room.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/webhook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/livekit_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/setup.py
```

### Comparing `livekit-protocol-0.3.2/PKG-INFO` & `livekit-protocol-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-protocol
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python protocol stubs for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/agent.py` & `livekit-protocol-0.4.0/livekit/protocol/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,44 +11,54 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import models as _models_
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13livekit_agent.proto\x12\x07livekit\x1a\x14livekit_models.proto\"6\n\tAgentInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\x92\x01\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x04type\x18\x02 \x01(\x0e\x32\x10.livekit.JobType\x12\x1b\n\x04room\x18\x03 \x01(\x0b\x32\r.livekit.Room\x12\x32\n\x0bparticipant\x18\x04 \x01(\x0b\x32\x18.livekit.ParticipantInfoH\x00\x88\x01\x01\x42\x0e\n\x0c_participant\"\xe4\x01\n\rWorkerMessage\x12\x32\n\x08register\x18\x01 \x01(\x0b\x32\x1e.livekit.RegisterWorkerRequestH\x00\x12\x35\n\x0c\x61vailability\x18\x02 \x01(\x0b\x32\x1d.livekit.AvailabilityResponseH\x00\x12-\n\x06status\x18\x03 \x01(\x0b\x32\x1b.livekit.UpdateWorkerStatusH\x00\x12.\n\njob_update\x18\x04 \x01(\x0b\x32\x18.livekit.JobStatusUpdateH\x00\x42\t\n\x07message\"\xb3\x01\n\rServerMessage\x12\x33\n\x08register\x18\x01 \x01(\x0b\x32\x1f.livekit.RegisterWorkerResponseH\x00\x12\x34\n\x0c\x61vailability\x18\x02 \x01(\x0b\x32\x1c.livekit.AvailabilityRequestH\x00\x12,\n\nassignment\x18\x03 \x01(\x0b\x32\x16.livekit.JobAssignmentH\x00\x42\t\n\x07message\"i\n\x15RegisterWorkerRequest\x12\x1e\n\x04type\x18\x01 \x01(\x0e\x32\x10.livekit.JobType\x12\x11\n\tworker_id\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\"C\n\x16RegisterWorkerResponse\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x16\n\x0eserver_version\x18\x02 \x01(\t\"0\n\x13\x41vailabilityRequest\x12\x19\n\x03job\x18\x01 \x01(\x0b\x32\x0c.livekit.Job\"9\n\x14\x41vailabilityResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x08\"g\n\x0fJobStatusUpdate\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\"\n\x06status\x18\x02 \x01(\x0e\x32\x12.livekit.JobStatus\x12\r\n\x05\x65rror\x18\x03 \x01(\t\x12\x11\n\tuser_data\x18\x04 \x01(\t\"*\n\rJobAssignment\x12\x19\n\x03job\x18\x01 \x01(\x0b\x32\x0c.livekit.Job\";\n\x12UpdateWorkerStatus\x12%\n\x06status\x18\x01 \x01(\x0e\x32\x15.livekit.WorkerStatus*(\n\x07JobType\x12\x0b\n\x07JT_ROOM\x10\x00\x12\x10\n\x0cJT_PUBLISHER\x10\x01*-\n\x0cWorkerStatus\x12\x10\n\x0cWS_AVAILABLE\x10\x00\x12\x0b\n\x07WS_FULL\x10\x01*:\n\tJobStatus\x12\x0e\n\nJS_UNKNOWN\x10\x00\x12\x0e\n\nJS_SUCCESS\x10\x01\x12\r\n\tJS_FAILED\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13livekit_agent.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\xa7\x01\n\nWorkerInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x1e\n\x04type\x18\x05 \x01(\x0e\x32\x10.livekit.JobType\x12;\n\x13\x61llowed_permissions\x18\x06 \x01(\x0b\x32\x1e.livekit.ParticipantPermission\"6\n\tAgentInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\xa5\x01\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x04type\x18\x02 \x01(\x0e\x32\x10.livekit.JobType\x12\x1b\n\x04room\x18\x03 \x01(\x0b\x32\r.livekit.Room\x12\x32\n\x0bparticipant\x18\x04 \x01(\x0b\x32\x18.livekit.ParticipantInfoH\x00\x88\x01\x01\x12\x11\n\tnamespace\x18\x05 \x01(\tB\x0e\n\x0c_participant\"\xf8\x02\n\rWorkerMessage\x12\x32\n\x08register\x18\x01 \x01(\x0b\x32\x1e.livekit.RegisterWorkerRequestH\x00\x12\x35\n\x0c\x61vailability\x18\x02 \x01(\x0b\x32\x1d.livekit.AvailabilityResponseH\x00\x12\x34\n\rupdate_worker\x18\x03 \x01(\x0b\x32\x1b.livekit.UpdateWorkerStatusH\x00\x12.\n\nupdate_job\x18\x04 \x01(\x0b\x32\x18.livekit.UpdateJobStatusH\x00\x12#\n\x04ping\x18\x05 \x01(\x0b\x32\x13.livekit.WorkerPingH\x00\x12\x33\n\x0csimulate_job\x18\x06 \x01(\x0b\x32\x1b.livekit.SimulateJobRequestH\x00\x12\x31\n\x0bmigrate_job\x18\x07 \x01(\x0b\x32\x1a.livekit.MigrateJobRequestH\x00\x42\t\n\x07message\"\xd8\x01\n\rServerMessage\x12\x33\n\x08register\x18\x01 \x01(\x0b\x32\x1f.livekit.RegisterWorkerResponseH\x00\x12\x34\n\x0c\x61vailability\x18\x02 \x01(\x0b\x32\x1c.livekit.AvailabilityRequestH\x00\x12,\n\nassignment\x18\x03 \x01(\x0b\x32\x16.livekit.JobAssignmentH\x00\x12#\n\x04pong\x18\x04 \x01(\x0b\x32\x13.livekit.WorkerPongH\x00\x42\t\n\x07message\"\x80\x01\n\x12SimulateJobRequest\x12\x1e\n\x04type\x18\x01 \x01(\x0e\x32\x10.livekit.JobType\x12\x1b\n\x04room\x18\x02 \x01(\x0b\x32\r.livekit.Room\x12-\n\x0bparticipant\x18\x03 \x01(\x0b\x32\x18.livekit.ParticipantInfo\"\x1f\n\nWorkerPing\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\"7\n\nWorkerPong\x12\x16\n\x0elast_timestamp\x18\x01 \x01(\x03\x12\x11\n\ttimestamp\x18\x02 \x01(\x03\"\xd0\x01\n\x15RegisterWorkerRequest\x12\x1e\n\x04type\x18\x01 \x01(\x0e\x32\x10.livekit.JobType\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x15\n\rping_interval\x18\x05 \x01(\r\x12\x16\n\tnamespace\x18\x06 \x01(\tH\x00\x88\x01\x01\x12;\n\x13\x61llowed_permissions\x18\x07 \x01(\x0b\x32\x1e.livekit.ParticipantPermissionB\x0c\n\n_namespace\"U\n\x16RegisterWorkerResponse\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12(\n\x0bserver_info\x18\x03 \x01(\x0b\x32\x13.livekit.ServerInfo\"#\n\x11MigrateJobRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"B\n\x13\x41vailabilityRequest\x12\x19\n\x03job\x18\x01 \x01(\x0b\x32\x0c.livekit.Job\x12\x10\n\x08resuming\x18\x02 \x01(\x08\"\xa8\x01\n\x14\x41vailabilityResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x08\x12\x17\n\x0fsupports_resume\x18\x03 \x01(\x08\x12\x18\n\x10participant_name\x18\x04 \x01(\t\x12\x1c\n\x14participant_identity\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\x06 \x01(\t\"\x96\x01\n\x0fUpdateJobStatus\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\'\n\x06status\x18\x02 \x01(\x0e\x32\x12.livekit.JobStatusH\x00\x88\x01\x01\x12\r\n\x05\x65rror\x18\x03 \x01(\t\x12\x15\n\x08metadata\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x0c\n\x04load\x18\x05 \x01(\x02\x42\t\n\x07_statusB\x0b\n\t_metadata\"}\n\x12UpdateWorkerStatus\x12*\n\x06status\x18\x01 \x01(\x0e\x32\x15.livekit.WorkerStatusH\x00\x88\x01\x01\x12\x15\n\x08metadata\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x0c\n\x04load\x18\x03 \x01(\x02\x42\t\n\x07_statusB\x0b\n\t_metadata\"S\n\rJobAssignment\x12\x19\n\x03job\x18\x01 \x01(\x0b\x32\x0c.livekit.Job\x12\x10\n\x03url\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\r\n\x05token\x18\x03 \x01(\tB\x06\n\x04_url*(\n\x07JobType\x12\x0b\n\x07JT_ROOM\x10\x00\x12\x10\n\x0cJT_PUBLISHER\x10\x01*-\n\x0cWorkerStatus\x12\x10\n\x0cWS_AVAILABLE\x10\x00\x12\x0b\n\x07WS_FULL\x10\x01*:\n\tJobStatus\x12\x0e\n\nJS_UNKNOWN\x10\x00\x12\x0e\n\nJS_SUCCESS\x10\x01\x12\r\n\tJS_FAILED\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
-  _globals['_JOBTYPE']._serialized_start=1167
-  _globals['_JOBTYPE']._serialized_end=1207
-  _globals['_WORKERSTATUS']._serialized_start=1209
-  _globals['_WORKERSTATUS']._serialized_end=1254
-  _globals['_JOBSTATUS']._serialized_start=1256
-  _globals['_JOBSTATUS']._serialized_end=1314
-  _globals['_AGENTINFO']._serialized_start=54
-  _globals['_AGENTINFO']._serialized_end=108
-  _globals['_JOB']._serialized_start=111
-  _globals['_JOB']._serialized_end=257
-  _globals['_WORKERMESSAGE']._serialized_start=260
-  _globals['_WORKERMESSAGE']._serialized_end=488
-  _globals['_SERVERMESSAGE']._serialized_start=491
-  _globals['_SERVERMESSAGE']._serialized_end=670
-  _globals['_REGISTERWORKERREQUEST']._serialized_start=672
-  _globals['_REGISTERWORKERREQUEST']._serialized_end=777
-  _globals['_REGISTERWORKERRESPONSE']._serialized_start=779
-  _globals['_REGISTERWORKERRESPONSE']._serialized_end=846
-  _globals['_AVAILABILITYREQUEST']._serialized_start=848
-  _globals['_AVAILABILITYREQUEST']._serialized_end=896
-  _globals['_AVAILABILITYRESPONSE']._serialized_start=898
-  _globals['_AVAILABILITYRESPONSE']._serialized_end=955
-  _globals['_JOBSTATUSUPDATE']._serialized_start=957
-  _globals['_JOBSTATUSUPDATE']._serialized_end=1060
-  _globals['_JOBASSIGNMENT']._serialized_start=1062
-  _globals['_JOBASSIGNMENT']._serialized_end=1104
-  _globals['_UPDATEWORKERSTATUS']._serialized_start=1106
-  _globals['_UPDATEWORKERSTATUS']._serialized_end=1165
+  _globals['_JOBTYPE']._serialized_start=2206
+  _globals['_JOBTYPE']._serialized_end=2246
+  _globals['_WORKERSTATUS']._serialized_start=2248
+  _globals['_WORKERSTATUS']._serialized_end=2293
+  _globals['_JOBSTATUS']._serialized_start=2295
+  _globals['_JOBSTATUS']._serialized_end=2353
+  _globals['_WORKERINFO']._serialized_start=55
+  _globals['_WORKERINFO']._serialized_end=222
+  _globals['_AGENTINFO']._serialized_start=224
+  _globals['_AGENTINFO']._serialized_end=278
+  _globals['_JOB']._serialized_start=281
+  _globals['_JOB']._serialized_end=446
+  _globals['_WORKERMESSAGE']._serialized_start=449
+  _globals['_WORKERMESSAGE']._serialized_end=825
+  _globals['_SERVERMESSAGE']._serialized_start=828
+  _globals['_SERVERMESSAGE']._serialized_end=1044
+  _globals['_SIMULATEJOBREQUEST']._serialized_start=1047
+  _globals['_SIMULATEJOBREQUEST']._serialized_end=1175
+  _globals['_WORKERPING']._serialized_start=1177
+  _globals['_WORKERPING']._serialized_end=1208
+  _globals['_WORKERPONG']._serialized_start=1210
+  _globals['_WORKERPONG']._serialized_end=1265
+  _globals['_REGISTERWORKERREQUEST']._serialized_start=1268
+  _globals['_REGISTERWORKERREQUEST']._serialized_end=1476
+  _globals['_REGISTERWORKERRESPONSE']._serialized_start=1478
+  _globals['_REGISTERWORKERRESPONSE']._serialized_end=1563
+  _globals['_MIGRATEJOBREQUEST']._serialized_start=1565
+  _globals['_MIGRATEJOBREQUEST']._serialized_end=1600
+  _globals['_AVAILABILITYREQUEST']._serialized_start=1602
+  _globals['_AVAILABILITYREQUEST']._serialized_end=1668
+  _globals['_AVAILABILITYRESPONSE']._serialized_start=1671
+  _globals['_AVAILABILITYRESPONSE']._serialized_end=1839
+  _globals['_UPDATEJOBSTATUS']._serialized_start=1842
+  _globals['_UPDATEJOBSTATUS']._serialized_end=1992
+  _globals['_UPDATEWORKERSTATUS']._serialized_start=1994
+  _globals['_UPDATEWORKERSTATUS']._serialized_end=2119
+  _globals['_JOBASSIGNMENT']._serialized_start=2121
+  _globals['_JOBASSIGNMENT']._serialized_end=2204
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/analytics.py` & `livekit-protocol-0.4.0/livekit/protocol/analytics.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import models as _models_
 from . import egress as _egress_
 from . import ingress as _ingress_
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17livekit_analytics.proto\x12\x07livekit\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\x1a\x15livekit_ingress.proto\"T\n\x13\x41nalyticsVideoLayer\x12\r\n\x05layer\x18\x01 \x01(\x05\x12\x0f\n\x07packets\x18\x02 \x01(\r\x12\r\n\x05\x62ytes\x18\x03 \x01(\x04\x12\x0e\n\x06\x66rames\x18\x04 \x01(\r\"\xd7\x02\n\x0f\x41nalyticsStream\x12\x0c\n\x04ssrc\x18\x01 \x01(\r\x12\x17\n\x0fprimary_packets\x18\x02 \x01(\r\x12\x15\n\rprimary_bytes\x18\x03 \x01(\x04\x12\x1a\n\x12retransmit_packets\x18\x04 \x01(\r\x12\x18\n\x10retransmit_bytes\x18\x05 \x01(\x04\x12\x17\n\x0fpadding_packets\x18\x06 \x01(\r\x12\x15\n\rpadding_bytes\x18\x07 \x01(\x04\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x0e\n\x06\x66rames\x18\t \x01(\r\x12\x0b\n\x03rtt\x18\n \x01(\r\x12\x0e\n\x06jitter\x18\x0b \x01(\r\x12\r\n\x05nacks\x18\x0c \x01(\r\x12\x0c\n\x04plis\x18\r \x01(\r\x12\x0c\n\x04\x66irs\x18\x0e \x01(\r\x12\x32\n\x0cvideo_layers\x18\x0f \x03(\x0b\x32\x1c.livekit.AnalyticsVideoLayer\"\xda\x02\n\rAnalyticsStat\x12\x15\n\ranalytics_key\x18\x01 \x01(\t\x12!\n\x04kind\x18\x02 \x01(\x0e\x32\x13.livekit.StreamType\x12.\n\ntime_stamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04node\x18\x04 \x01(\t\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x11\n\troom_name\x18\x06 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x07 \x01(\t\x12\x10\n\x08track_id\x18\x08 \x01(\t\x12\r\n\x05score\x18\t \x01(\x02\x12)\n\x07streams\x18\n \x03(\x0b\x32\x18.livekit.AnalyticsStream\x12\x0c\n\x04mime\x18\x0b \x01(\t\x12\x11\n\tmin_score\x18\x0c \x01(\x02\x12\x14\n\x0cmedian_score\x18\r \x01(\x02\x12\x12\n\nproject_id\x18\x0e \x01(\t\"7\n\x0e\x41nalyticsStats\x12%\n\x05stats\x18\x01 \x03(\x0b\x32\x16.livekit.AnalyticsStat\"\xb2\x01\n\x13\x41nalyticsClientMeta\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x13\n\x0b\x63lient_addr\x18\x03 \x01(\t\x12\x1b\n\x13\x63lient_connect_time\x18\x04 \x01(\r\x12\x17\n\x0f\x63onnection_type\x18\x05 \x01(\t\x12\x32\n\x10reconnect_reason\x18\x06 \x01(\x0e\x32\x18.livekit.ReconnectReason\"\xd1\x05\n\x0e\x41nalyticsEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.livekit.AnalyticsEventType\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07room_id\x18\x03 \x01(\t\x12\x1b\n\x04room\x18\x04 \x01(\x0b\x32\r.livekit.Room\x12\x16\n\x0eparticipant_id\x18\x05 \x01(\t\x12-\n\x0bparticipant\x18\x06 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x10\n\x08track_id\x18\x07 \x01(\t\x12!\n\x05track\x18\x08 \x01(\x0b\x32\x12.livekit.TrackInfo\x12\x15\n\ranalytics_key\x18\n \x01(\t\x12(\n\x0b\x63lient_info\x18\x0b \x01(\x0b\x32\x13.livekit.ClientInfo\x12\x31\n\x0b\x63lient_meta\x18\x0c \x01(\x0b\x32\x1c.livekit.AnalyticsClientMeta\x12\x11\n\tegress_id\x18\r \x01(\t\x12\x12\n\ningress_id\x18\x13 \x01(\t\x12;\n\x1cmax_subscribed_video_quality\x18\x0e \x01(\x0e\x32\x15.livekit.VideoQuality\x12+\n\tpublisher\x18\x0f \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x0c\n\x04mime\x18\x10 \x01(\t\x12#\n\x06\x65gress\x18\x11 \x01(\x0b\x32\x13.livekit.EgressInfo\x12%\n\x07ingress\x18\x12 \x01(\x0b\x32\x14.livekit.IngressInfo\x12\r\n\x05\x65rror\x18\x14 \x01(\t\x12$\n\trtp_stats\x18\x15 \x01(\x0b\x32\x11.livekit.RTPStats\x12\x13\n\x0bvideo_layer\x18\x16 \x01(\x05\x12\x12\n\nproject_id\x18\x17 \x01(\t\":\n\x0f\x41nalyticsEvents\x12\'\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x17.livekit.AnalyticsEvent\"\xa4\x01\n\x18\x41nalyticsRoomParticipant\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12-\n\x05state\x18\x04 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12-\n\tjoined_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x92\x01\n\rAnalyticsRoom\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x0cparticipants\x18\x04 \x03(\x0b\x32!.livekit.AnalyticsRoomParticipant\"\x94\x01\n\x12\x41nalyticsNodeRooms\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x17\n\x0fsequence_number\x18\x02 \x01(\x04\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\x05rooms\x18\x04 \x03(\x0b\x32\x16.livekit.AnalyticsRoom**\n\nStreamType\x12\x0c\n\x08UPSTREAM\x10\x00\x12\x0e\n\nDOWNSTREAM\x10\x01*\x95\x05\n\x12\x41nalyticsEventType\x12\x10\n\x0cROOM_CREATED\x10\x00\x12\x0e\n\nROOM_ENDED\x10\x01\x12\x16\n\x12PARTICIPANT_JOINED\x10\x02\x12\x14\n\x10PARTICIPANT_LEFT\x10\x03\x12\x13\n\x0fTRACK_PUBLISHED\x10\x04\x12\x1b\n\x17TRACK_PUBLISH_REQUESTED\x10\x14\x12\x15\n\x11TRACK_UNPUBLISHED\x10\x05\x12\x14\n\x10TRACK_SUBSCRIBED\x10\x06\x12\x1d\n\x19TRACK_SUBSCRIBE_REQUESTED\x10\x15\x12\x1a\n\x16TRACK_SUBSCRIBE_FAILED\x10\x19\x12\x16\n\x12TRACK_UNSUBSCRIBED\x10\x07\x12\x1a\n\x16TRACK_PUBLISHED_UPDATE\x10\n\x12\x0f\n\x0bTRACK_MUTED\x10\x17\x12\x11\n\rTRACK_UNMUTED\x10\x18\x12\x17\n\x13TRACK_PUBLISH_STATS\x10\x1a\x12\x19\n\x15TRACK_SUBSCRIBE_STATS\x10\x1b\x12\x16\n\x12PARTICIPANT_ACTIVE\x10\x0b\x12\x17\n\x13PARTICIPANT_RESUMED\x10\x16\x12\x12\n\x0e\x45GRESS_STARTED\x10\x0c\x12\x10\n\x0c\x45GRESS_ENDED\x10\r\x12\x12\n\x0e\x45GRESS_UPDATED\x10\x1c\x12&\n\"TRACK_MAX_SUBSCRIBED_VIDEO_QUALITY\x10\x0e\x12\x0f\n\x0bRECONNECTED\x10\x0f\x12\x13\n\x0fINGRESS_CREATED\x10\x12\x12\x13\n\x0fINGRESS_DELETED\x10\x13\x12\x13\n\x0fINGRESS_STARTED\x10\x10\x12\x11\n\rINGRESS_ENDED\x10\x11\x12\x13\n\x0fINGRESS_UPDATED\x10\x1d\x32\xf5\x01\n\x18\x41nalyticsRecorderService\x12\x42\n\x0bIngestStats\x12\x17.livekit.AnalyticsStats\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12\x44\n\x0cIngestEvents\x12\x18.livekit.AnalyticsEvents\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12O\n\x14IngestNodeRoomStates\x12\x1b.livekit.AnalyticsNodeRooms\x1a\x16.google.protobuf.Empty\"\x00(\x01\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17livekit_analytics.proto\x12\x07livekit\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\x1a\x15livekit_ingress.proto\"T\n\x13\x41nalyticsVideoLayer\x12\r\n\x05layer\x18\x01 \x01(\x05\x12\x0f\n\x07packets\x18\x02 \x01(\r\x12\r\n\x05\x62ytes\x18\x03 \x01(\x04\x12\x0e\n\x06\x66rames\x18\x04 \x01(\r\"\xb5\x03\n\x0f\x41nalyticsStream\x12\x0c\n\x04ssrc\x18\x01 \x01(\r\x12\x17\n\x0fprimary_packets\x18\x02 \x01(\r\x12\x15\n\rprimary_bytes\x18\x03 \x01(\x04\x12\x1a\n\x12retransmit_packets\x18\x04 \x01(\r\x12\x18\n\x10retransmit_bytes\x18\x05 \x01(\x04\x12\x17\n\x0fpadding_packets\x18\x06 \x01(\r\x12\x15\n\rpadding_bytes\x18\x07 \x01(\x04\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x0e\n\x06\x66rames\x18\t \x01(\r\x12\x0b\n\x03rtt\x18\n \x01(\r\x12\x0e\n\x06jitter\x18\x0b \x01(\r\x12\r\n\x05nacks\x18\x0c \x01(\r\x12\x0c\n\x04plis\x18\r \x01(\r\x12\x0c\n\x04\x66irs\x18\x0e \x01(\r\x12\x32\n\x0cvideo_layers\x18\x0f \x03(\x0b\x32\x1c.livekit.AnalyticsVideoLayer\x12.\n\nstart_time\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xc6\x02\n\rAnalyticsStat\x12\x15\n\ranalytics_key\x18\x01 \x01(\t\x12!\n\x04kind\x18\x02 \x01(\x0e\x32\x13.livekit.StreamType\x12.\n\ntime_stamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04node\x18\x04 \x01(\t\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x11\n\troom_name\x18\x06 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x07 \x01(\t\x12\x10\n\x08track_id\x18\x08 \x01(\t\x12\r\n\x05score\x18\t \x01(\x02\x12)\n\x07streams\x18\n \x03(\x0b\x32\x18.livekit.AnalyticsStream\x12\x0c\n\x04mime\x18\x0b \x01(\t\x12\x11\n\tmin_score\x18\x0c \x01(\x02\x12\x14\n\x0cmedian_score\x18\r \x01(\x02\"7\n\x0e\x41nalyticsStats\x12%\n\x05stats\x18\x01 \x03(\x0b\x32\x16.livekit.AnalyticsStat\"\x9a\x02\n\x13\x41nalyticsClientMeta\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x13\n\x0b\x63lient_addr\x18\x03 \x01(\t\x12\x1b\n\x13\x63lient_connect_time\x18\x04 \x01(\r\x12\x17\n\x0f\x63onnection_type\x18\x05 \x01(\t\x12\x32\n\x10reconnect_reason\x18\x06 \x01(\x0e\x32\x18.livekit.ReconnectReason\x12\x15\n\x08geo_hash\x18\x07 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07\x63ountry\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07isp_asn\x18\t \x01(\rH\x02\x88\x01\x01\x42\x0b\n\t_geo_hashB\n\n\x08_countryB\n\n\x08_isp_asn\"\xbd\x05\n\x0e\x41nalyticsEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.livekit.AnalyticsEventType\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07room_id\x18\x03 \x01(\t\x12\x1b\n\x04room\x18\x04 \x01(\x0b\x32\r.livekit.Room\x12\x16\n\x0eparticipant_id\x18\x05 \x01(\t\x12-\n\x0bparticipant\x18\x06 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x10\n\x08track_id\x18\x07 \x01(\t\x12!\n\x05track\x18\x08 \x01(\x0b\x32\x12.livekit.TrackInfo\x12\x15\n\ranalytics_key\x18\n \x01(\t\x12(\n\x0b\x63lient_info\x18\x0b \x01(\x0b\x32\x13.livekit.ClientInfo\x12\x31\n\x0b\x63lient_meta\x18\x0c \x01(\x0b\x32\x1c.livekit.AnalyticsClientMeta\x12\x11\n\tegress_id\x18\r \x01(\t\x12\x12\n\ningress_id\x18\x13 \x01(\t\x12;\n\x1cmax_subscribed_video_quality\x18\x0e \x01(\x0e\x32\x15.livekit.VideoQuality\x12+\n\tpublisher\x18\x0f \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x0c\n\x04mime\x18\x10 \x01(\t\x12#\n\x06\x65gress\x18\x11 \x01(\x0b\x32\x13.livekit.EgressInfo\x12%\n\x07ingress\x18\x12 \x01(\x0b\x32\x14.livekit.IngressInfo\x12\r\n\x05\x65rror\x18\x14 \x01(\t\x12$\n\trtp_stats\x18\x15 \x01(\x0b\x32\x11.livekit.RTPStats\x12\x13\n\x0bvideo_layer\x18\x16 \x01(\x05\":\n\x0f\x41nalyticsEvents\x12\'\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x17.livekit.AnalyticsEvent\"\xa4\x01\n\x18\x41nalyticsRoomParticipant\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12-\n\x05state\x18\x04 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12-\n\tjoined_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa6\x01\n\rAnalyticsRoom\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x0cparticipants\x18\x04 \x03(\x0b\x32!.livekit.AnalyticsRoomParticipant\"\x94\x01\n\x12\x41nalyticsNodeRooms\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x17\n\x0fsequence_number\x18\x02 \x01(\x04\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\x05rooms\x18\x04 \x03(\x0b\x32\x16.livekit.AnalyticsRoom**\n\nStreamType\x12\x0c\n\x08UPSTREAM\x10\x00\x12\x0e\n\nDOWNSTREAM\x10\x01*\x95\x05\n\x12\x41nalyticsEventType\x12\x10\n\x0cROOM_CREATED\x10\x00\x12\x0e\n\nROOM_ENDED\x10\x01\x12\x16\n\x12PARTICIPANT_JOINED\x10\x02\x12\x14\n\x10PARTICIPANT_LEFT\x10\x03\x12\x13\n\x0fTRACK_PUBLISHED\x10\x04\x12\x1b\n\x17TRACK_PUBLISH_REQUESTED\x10\x14\x12\x15\n\x11TRACK_UNPUBLISHED\x10\x05\x12\x14\n\x10TRACK_SUBSCRIBED\x10\x06\x12\x1d\n\x19TRACK_SUBSCRIBE_REQUESTED\x10\x15\x12\x1a\n\x16TRACK_SUBSCRIBE_FAILED\x10\x19\x12\x16\n\x12TRACK_UNSUBSCRIBED\x10\x07\x12\x1a\n\x16TRACK_PUBLISHED_UPDATE\x10\n\x12\x0f\n\x0bTRACK_MUTED\x10\x17\x12\x11\n\rTRACK_UNMUTED\x10\x18\x12\x17\n\x13TRACK_PUBLISH_STATS\x10\x1a\x12\x19\n\x15TRACK_SUBSCRIBE_STATS\x10\x1b\x12\x16\n\x12PARTICIPANT_ACTIVE\x10\x0b\x12\x17\n\x13PARTICIPANT_RESUMED\x10\x16\x12\x12\n\x0e\x45GRESS_STARTED\x10\x0c\x12\x10\n\x0c\x45GRESS_ENDED\x10\r\x12\x12\n\x0e\x45GRESS_UPDATED\x10\x1c\x12&\n\"TRACK_MAX_SUBSCRIBED_VIDEO_QUALITY\x10\x0e\x12\x0f\n\x0bRECONNECTED\x10\x0f\x12\x13\n\x0fINGRESS_CREATED\x10\x12\x12\x13\n\x0fINGRESS_DELETED\x10\x13\x12\x13\n\x0fINGRESS_STARTED\x10\x10\x12\x11\n\rINGRESS_ENDED\x10\x11\x12\x13\n\x0fINGRESS_UPDATED\x10\x1d\x32\xf5\x01\n\x18\x41nalyticsRecorderService\x12\x42\n\x0bIngestStats\x12\x17.livekit.AnalyticsStats\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12\x44\n\x0cIngestEvents\x12\x18.livekit.AnalyticsEvents\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12O\n\x14IngestNodeRoomStates\x12\x1b.livekit.AnalyticsNodeRooms\x1a\x16.google.protobuf.Empty\"\x00(\x01\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'analytics', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
-  _globals['_STREAMTYPE']._serialized_start=2435
-  _globals['_STREAMTYPE']._serialized_end=2477
-  _globals['_ANALYTICSEVENTTYPE']._serialized_start=2480
-  _globals['_ANALYTICSEVENTTYPE']._serialized_end=3141
+  _globals['_STREAMTYPE']._serialized_start=2613
+  _globals['_STREAMTYPE']._serialized_end=2655
+  _globals['_ANALYTICSEVENTTYPE']._serialized_start=2658
+  _globals['_ANALYTICSEVENTTYPE']._serialized_end=3319
   _globals['_ANALYTICSVIDEOLAYER']._serialized_start=165
   _globals['_ANALYTICSVIDEOLAYER']._serialized_end=249
   _globals['_ANALYTICSSTREAM']._serialized_start=252
-  _globals['_ANALYTICSSTREAM']._serialized_end=595
-  _globals['_ANALYTICSSTAT']._serialized_start=598
-  _globals['_ANALYTICSSTAT']._serialized_end=944
-  _globals['_ANALYTICSSTATS']._serialized_start=946
-  _globals['_ANALYTICSSTATS']._serialized_end=1001
-  _globals['_ANALYTICSCLIENTMETA']._serialized_start=1004
-  _globals['_ANALYTICSCLIENTMETA']._serialized_end=1182
-  _globals['_ANALYTICSEVENT']._serialized_start=1185
-  _globals['_ANALYTICSEVENT']._serialized_end=1906
-  _globals['_ANALYTICSEVENTS']._serialized_start=1908
-  _globals['_ANALYTICSEVENTS']._serialized_end=1966
-  _globals['_ANALYTICSROOMPARTICIPANT']._serialized_start=1969
-  _globals['_ANALYTICSROOMPARTICIPANT']._serialized_end=2133
-  _globals['_ANALYTICSROOM']._serialized_start=2136
-  _globals['_ANALYTICSROOM']._serialized_end=2282
-  _globals['_ANALYTICSNODEROOMS']._serialized_start=2285
-  _globals['_ANALYTICSNODEROOMS']._serialized_end=2433
-  _globals['_ANALYTICSRECORDERSERVICE']._serialized_start=3144
-  _globals['_ANALYTICSRECORDERSERVICE']._serialized_end=3389
+  _globals['_ANALYTICSSTREAM']._serialized_end=689
+  _globals['_ANALYTICSSTAT']._serialized_start=692
+  _globals['_ANALYTICSSTAT']._serialized_end=1018
+  _globals['_ANALYTICSSTATS']._serialized_start=1020
+  _globals['_ANALYTICSSTATS']._serialized_end=1075
+  _globals['_ANALYTICSCLIENTMETA']._serialized_start=1078
+  _globals['_ANALYTICSCLIENTMETA']._serialized_end=1360
+  _globals['_ANALYTICSEVENT']._serialized_start=1363
+  _globals['_ANALYTICSEVENT']._serialized_end=2064
+  _globals['_ANALYTICSEVENTS']._serialized_start=2066
+  _globals['_ANALYTICSEVENTS']._serialized_end=2124
+  _globals['_ANALYTICSROOMPARTICIPANT']._serialized_start=2127
+  _globals['_ANALYTICSROOMPARTICIPANT']._serialized_end=2291
+  _globals['_ANALYTICSROOM']._serialized_start=2294
+  _globals['_ANALYTICSROOM']._serialized_end=2460
+  _globals['_ANALYTICSNODEROOMS']._serialized_start=2463
+  _globals['_ANALYTICSNODEROOMS']._serialized_end=2611
+  _globals['_ANALYTICSRECORDERSERVICE']._serialized_start=3322
+  _globals['_ANALYTICSRECORDERSERVICE']._serialized_end=3567
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/analytics.pyi` & `livekit-protocol-0.4.0/livekit/protocol/analytics.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     layer: int
     packets: int
     bytes: int
     frames: int
     def __init__(self, layer: _Optional[int] = ..., packets: _Optional[int] = ..., bytes: _Optional[int] = ..., frames: _Optional[int] = ...) -> None: ...
 
 class AnalyticsStream(_message.Message):
-    __slots__ = ("ssrc", "primary_packets", "primary_bytes", "retransmit_packets", "retransmit_bytes", "padding_packets", "padding_bytes", "packets_lost", "frames", "rtt", "jitter", "nacks", "plis", "firs", "video_layers")
+    __slots__ = ("ssrc", "primary_packets", "primary_bytes", "retransmit_packets", "retransmit_bytes", "padding_packets", "padding_bytes", "packets_lost", "frames", "rtt", "jitter", "nacks", "plis", "firs", "video_layers", "start_time", "end_time")
     SSRC_FIELD_NUMBER: _ClassVar[int]
     PRIMARY_PACKETS_FIELD_NUMBER: _ClassVar[int]
     PRIMARY_BYTES_FIELD_NUMBER: _ClassVar[int]
     RETRANSMIT_PACKETS_FIELD_NUMBER: _ClassVar[int]
     RETRANSMIT_BYTES_FIELD_NUMBER: _ClassVar[int]
     PADDING_PACKETS_FIELD_NUMBER: _ClassVar[int]
     PADDING_BYTES_FIELD_NUMBER: _ClassVar[int]
@@ -102,14 +102,16 @@
     FRAMES_FIELD_NUMBER: _ClassVar[int]
     RTT_FIELD_NUMBER: _ClassVar[int]
     JITTER_FIELD_NUMBER: _ClassVar[int]
     NACKS_FIELD_NUMBER: _ClassVar[int]
     PLIS_FIELD_NUMBER: _ClassVar[int]
     FIRS_FIELD_NUMBER: _ClassVar[int]
     VIDEO_LAYERS_FIELD_NUMBER: _ClassVar[int]
+    START_TIME_FIELD_NUMBER: _ClassVar[int]
+    END_TIME_FIELD_NUMBER: _ClassVar[int]
     ssrc: int
     primary_packets: int
     primary_bytes: int
     retransmit_packets: int
     retransmit_bytes: int
     padding_packets: int
     padding_bytes: int
@@ -117,72 +119,78 @@
     frames: int
     rtt: int
     jitter: int
     nacks: int
     plis: int
     firs: int
     video_layers: _containers.RepeatedCompositeFieldContainer[AnalyticsVideoLayer]
-    def __init__(self, ssrc: _Optional[int] = ..., primary_packets: _Optional[int] = ..., primary_bytes: _Optional[int] = ..., retransmit_packets: _Optional[int] = ..., retransmit_bytes: _Optional[int] = ..., padding_packets: _Optional[int] = ..., padding_bytes: _Optional[int] = ..., packets_lost: _Optional[int] = ..., frames: _Optional[int] = ..., rtt: _Optional[int] = ..., jitter: _Optional[int] = ..., nacks: _Optional[int] = ..., plis: _Optional[int] = ..., firs: _Optional[int] = ..., video_layers: _Optional[_Iterable[_Union[AnalyticsVideoLayer, _Mapping]]] = ...) -> None: ...
+    start_time: _timestamp_pb2.Timestamp
+    end_time: _timestamp_pb2.Timestamp
+    def __init__(self, ssrc: _Optional[int] = ..., primary_packets: _Optional[int] = ..., primary_bytes: _Optional[int] = ..., retransmit_packets: _Optional[int] = ..., retransmit_bytes: _Optional[int] = ..., padding_packets: _Optional[int] = ..., padding_bytes: _Optional[int] = ..., packets_lost: _Optional[int] = ..., frames: _Optional[int] = ..., rtt: _Optional[int] = ..., jitter: _Optional[int] = ..., nacks: _Optional[int] = ..., plis: _Optional[int] = ..., firs: _Optional[int] = ..., video_layers: _Optional[_Iterable[_Union[AnalyticsVideoLayer, _Mapping]]] = ..., start_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., end_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class AnalyticsStat(_message.Message):
-    __slots__ = ("analytics_key", "kind", "time_stamp", "node", "room_id", "room_name", "participant_id", "track_id", "score", "streams", "mime", "min_score", "median_score", "project_id")
+    __slots__ = ("analytics_key", "kind", "time_stamp", "node", "room_id", "room_name", "participant_id", "track_id", "score", "streams", "mime", "min_score", "median_score")
     ANALYTICS_KEY_FIELD_NUMBER: _ClassVar[int]
     KIND_FIELD_NUMBER: _ClassVar[int]
     TIME_STAMP_FIELD_NUMBER: _ClassVar[int]
     NODE_FIELD_NUMBER: _ClassVar[int]
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
     TRACK_ID_FIELD_NUMBER: _ClassVar[int]
     SCORE_FIELD_NUMBER: _ClassVar[int]
     STREAMS_FIELD_NUMBER: _ClassVar[int]
     MIME_FIELD_NUMBER: _ClassVar[int]
     MIN_SCORE_FIELD_NUMBER: _ClassVar[int]
     MEDIAN_SCORE_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     analytics_key: str
     kind: StreamType
     time_stamp: _timestamp_pb2.Timestamp
     node: str
     room_id: str
     room_name: str
     participant_id: str
     track_id: str
     score: float
     streams: _containers.RepeatedCompositeFieldContainer[AnalyticsStream]
     mime: str
     min_score: float
     median_score: float
-    project_id: str
-    def __init__(self, analytics_key: _Optional[str] = ..., kind: _Optional[_Union[StreamType, str]] = ..., time_stamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., node: _Optional[str] = ..., room_id: _Optional[str] = ..., room_name: _Optional[str] = ..., participant_id: _Optional[str] = ..., track_id: _Optional[str] = ..., score: _Optional[float] = ..., streams: _Optional[_Iterable[_Union[AnalyticsStream, _Mapping]]] = ..., mime: _Optional[str] = ..., min_score: _Optional[float] = ..., median_score: _Optional[float] = ..., project_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, analytics_key: _Optional[str] = ..., kind: _Optional[_Union[StreamType, str]] = ..., time_stamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., node: _Optional[str] = ..., room_id: _Optional[str] = ..., room_name: _Optional[str] = ..., participant_id: _Optional[str] = ..., track_id: _Optional[str] = ..., score: _Optional[float] = ..., streams: _Optional[_Iterable[_Union[AnalyticsStream, _Mapping]]] = ..., mime: _Optional[str] = ..., min_score: _Optional[float] = ..., median_score: _Optional[float] = ...) -> None: ...
 
 class AnalyticsStats(_message.Message):
     __slots__ = ("stats",)
     STATS_FIELD_NUMBER: _ClassVar[int]
     stats: _containers.RepeatedCompositeFieldContainer[AnalyticsStat]
     def __init__(self, stats: _Optional[_Iterable[_Union[AnalyticsStat, _Mapping]]] = ...) -> None: ...
 
 class AnalyticsClientMeta(_message.Message):
-    __slots__ = ("region", "node", "client_addr", "client_connect_time", "connection_type", "reconnect_reason")
+    __slots__ = ("region", "node", "client_addr", "client_connect_time", "connection_type", "reconnect_reason", "geo_hash", "country", "isp_asn")
     REGION_FIELD_NUMBER: _ClassVar[int]
     NODE_FIELD_NUMBER: _ClassVar[int]
     CLIENT_ADDR_FIELD_NUMBER: _ClassVar[int]
     CLIENT_CONNECT_TIME_FIELD_NUMBER: _ClassVar[int]
     CONNECTION_TYPE_FIELD_NUMBER: _ClassVar[int]
     RECONNECT_REASON_FIELD_NUMBER: _ClassVar[int]
+    GEO_HASH_FIELD_NUMBER: _ClassVar[int]
+    COUNTRY_FIELD_NUMBER: _ClassVar[int]
+    ISP_ASN_FIELD_NUMBER: _ClassVar[int]
     region: str
     node: str
     client_addr: str
     client_connect_time: int
     connection_type: str
     reconnect_reason: _models.ReconnectReason
-    def __init__(self, region: _Optional[str] = ..., node: _Optional[str] = ..., client_addr: _Optional[str] = ..., client_connect_time: _Optional[int] = ..., connection_type: _Optional[str] = ..., reconnect_reason: _Optional[_Union[_models.ReconnectReason, str]] = ...) -> None: ...
+    geo_hash: str
+    country: str
+    isp_asn: int
+    def __init__(self, region: _Optional[str] = ..., node: _Optional[str] = ..., client_addr: _Optional[str] = ..., client_connect_time: _Optional[int] = ..., connection_type: _Optional[str] = ..., reconnect_reason: _Optional[_Union[_models.ReconnectReason, str]] = ..., geo_hash: _Optional[str] = ..., country: _Optional[str] = ..., isp_asn: _Optional[int] = ...) -> None: ...
 
 class AnalyticsEvent(_message.Message):
-    __slots__ = ("type", "timestamp", "room_id", "room", "participant_id", "participant", "track_id", "track", "analytics_key", "client_info", "client_meta", "egress_id", "ingress_id", "max_subscribed_video_quality", "publisher", "mime", "egress", "ingress", "error", "rtp_stats", "video_layer", "project_id")
+    __slots__ = ("type", "timestamp", "room_id", "room", "participant_id", "participant", "track_id", "track", "analytics_key", "client_info", "client_meta", "egress_id", "ingress_id", "max_subscribed_video_quality", "publisher", "mime", "egress", "ingress", "error", "rtp_stats", "video_layer")
     TYPE_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
     ROOM_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     TRACK_ID_FIELD_NUMBER: _ClassVar[int]
@@ -196,15 +204,14 @@
     PUBLISHER_FIELD_NUMBER: _ClassVar[int]
     MIME_FIELD_NUMBER: _ClassVar[int]
     EGRESS_FIELD_NUMBER: _ClassVar[int]
     INGRESS_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     RTP_STATS_FIELD_NUMBER: _ClassVar[int]
     VIDEO_LAYER_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     type: AnalyticsEventType
     timestamp: _timestamp_pb2.Timestamp
     room_id: str
     room: _models.Room
     participant_id: str
     participant: _models.ParticipantInfo
     track_id: str
@@ -218,16 +225,15 @@
     publisher: _models.ParticipantInfo
     mime: str
     egress: _egress.EgressInfo
     ingress: _ingress.IngressInfo
     error: str
     rtp_stats: _models.RTPStats
     video_layer: int
-    project_id: str
-    def __init__(self, type: _Optional[_Union[AnalyticsEventType, str]] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., room_id: _Optional[str] = ..., room: _Optional[_Union[_models.Room, _Mapping]] = ..., participant_id: _Optional[str] = ..., participant: _Optional[_Union[_models.ParticipantInfo, _Mapping]] = ..., track_id: _Optional[str] = ..., track: _Optional[_Union[_models.TrackInfo, _Mapping]] = ..., analytics_key: _Optional[str] = ..., client_info: _Optional[_Union[_models.ClientInfo, _Mapping]] = ..., client_meta: _Optional[_Union[AnalyticsClientMeta, _Mapping]] = ..., egress_id: _Optional[str] = ..., ingress_id: _Optional[str] = ..., max_subscribed_video_quality: _Optional[_Union[_models.VideoQuality, str]] = ..., publisher: _Optional[_Union[_models.ParticipantInfo, _Mapping]] = ..., mime: _Optional[str] = ..., egress: _Optional[_Union[_egress.EgressInfo, _Mapping]] = ..., ingress: _Optional[_Union[_ingress.IngressInfo, _Mapping]] = ..., error: _Optional[str] = ..., rtp_stats: _Optional[_Union[_models.RTPStats, _Mapping]] = ..., video_layer: _Optional[int] = ..., project_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, type: _Optional[_Union[AnalyticsEventType, str]] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., room_id: _Optional[str] = ..., room: _Optional[_Union[_models.Room, _Mapping]] = ..., participant_id: _Optional[str] = ..., participant: _Optional[_Union[_models.ParticipantInfo, _Mapping]] = ..., track_id: _Optional[str] = ..., track: _Optional[_Union[_models.TrackInfo, _Mapping]] = ..., analytics_key: _Optional[str] = ..., client_info: _Optional[_Union[_models.ClientInfo, _Mapping]] = ..., client_meta: _Optional[_Union[AnalyticsClientMeta, _Mapping]] = ..., egress_id: _Optional[str] = ..., ingress_id: _Optional[str] = ..., max_subscribed_video_quality: _Optional[_Union[_models.VideoQuality, str]] = ..., publisher: _Optional[_Union[_models.ParticipantInfo, _Mapping]] = ..., mime: _Optional[str] = ..., egress: _Optional[_Union[_egress.EgressInfo, _Mapping]] = ..., ingress: _Optional[_Union[_ingress.IngressInfo, _Mapping]] = ..., error: _Optional[str] = ..., rtp_stats: _Optional[_Union[_models.RTPStats, _Mapping]] = ..., video_layer: _Optional[int] = ...) -> None: ...
 
 class AnalyticsEvents(_message.Message):
     __slots__ = ("events",)
     EVENTS_FIELD_NUMBER: _ClassVar[int]
     events: _containers.RepeatedCompositeFieldContainer[AnalyticsEvent]
     def __init__(self, events: _Optional[_Iterable[_Union[AnalyticsEvent, _Mapping]]] = ...) -> None: ...
 
@@ -242,24 +248,26 @@
     identity: str
     name: str
     state: _models.ParticipantInfo.State
     joined_at: _timestamp_pb2.Timestamp
     def __init__(self, id: _Optional[str] = ..., identity: _Optional[str] = ..., name: _Optional[str] = ..., state: _Optional[_Union[_models.ParticipantInfo.State, str]] = ..., joined_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class AnalyticsRoom(_message.Message):
-    __slots__ = ("id", "name", "created_at", "participants")
+    __slots__ = ("id", "name", "project_id", "created_at", "participants")
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANTS_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
+    project_id: str
     created_at: _timestamp_pb2.Timestamp
     participants: _containers.RepeatedCompositeFieldContainer[AnalyticsRoomParticipant]
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., participants: _Optional[_Iterable[_Union[AnalyticsRoomParticipant, _Mapping]]] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., project_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., participants: _Optional[_Iterable[_Union[AnalyticsRoomParticipant, _Mapping]]] = ...) -> None: ...
 
 class AnalyticsNodeRooms(_message.Message):
     __slots__ = ("node_id", "sequence_number", "timestamp", "rooms")
     NODE_ID_FIELD_NUMBER: _ClassVar[int]
     SEQUENCE_NUMBER_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     ROOMS_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/egress.py` & `livekit-protocol-0.4.0/livekit/protocol/egress.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import models as _models_
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14livekit_egress.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\xcd\x04\n\x1aRoomCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t\x12\x12\n\naudio_only\x18\x03 \x01(\x08\x12\x12\n\nvideo_only\x18\x04 \x01(\x08\x12\x17\n\x0f\x63ustom_base_url\x18\x05 \x01(\t\x12.\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x07 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\n \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x08 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\t \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\x0b \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x0c \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\r \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\x0e \x03(\x0b\x32\x14.livekit.ImageOutputB\x08\n\x06outputB\t\n\x07options\"\xb0\x04\n\x10WebEgressRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\naudio_only\x18\x02 \x01(\x08\x12\x12\n\nvideo_only\x18\x03 \x01(\x08\x12\x1a\n\x12\x61wait_start_signal\x18\x0c \x01(\x08\x12.\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\x06 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x07 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x08 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\t \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\n \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\x0b \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\r \x03(\x0b\x32\x14.livekit.ImageOutputB\x08\n\x06outputB\t\n\x07options\"\x85\x03\n\x18ParticipantEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x14\n\x0cscreen_share\x18\x03 \x01(\x08\x12\x30\n\x06preset\x18\x04 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x00\x12,\n\x08\x61\x64vanced\x18\x05 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x00\x12\x30\n\x0c\x66ile_outputs\x18\x06 \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x07 \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\x08 \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\t \x03(\x0b\x32\x14.livekit.ImageOutputB\t\n\x07options\"\xad\x04\n\x1bTrackCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x16\n\x0e\x61udio_track_id\x18\x02 \x01(\t\x12\x16\n\x0evideo_track_id\x18\x03 \x01(\t\x12.\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\x08 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x06 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x07 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\x0b \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x0c \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\r \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\x0e \x03(\x0b\x32\x14.livekit.ImageOutputB\x08\n\x06outputB\t\n\x07options\"\x87\x01\n\x12TrackEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12)\n\x04\x66ile\x18\x03 \x01(\x0b\x32\x19.livekit.DirectFileOutputH\x00\x12\x17\n\rwebsocket_url\x18\x04 \x01(\tH\x00\x42\x08\n\x06output\"\x8e\x02\n\x11\x45ncodedFileOutput\x12+\n\tfile_type\x18\x01 \x01(\x0e\x32\x18.livekit.EncodedFileType\x12\x10\n\x08\x66ilepath\x18\x02 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x06 \x01(\x08\x12\x1f\n\x02s3\x18\x03 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x04 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x05 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x07 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xa0\x03\n\x13SegmentedFileOutput\x12\x30\n\x08protocol\x18\x01 \x01(\x0e\x32\x1e.livekit.SegmentedFileProtocol\x12\x17\n\x0f\x66ilename_prefix\x18\x02 \x01(\t\x12\x15\n\rplaylist_name\x18\x03 \x01(\t\x12\x1a\n\x12live_playlist_name\x18\x0b \x01(\t\x12\x18\n\x10segment_duration\x18\x04 \x01(\r\x12\x35\n\x0f\x66ilename_suffix\x18\n \x01(\x0e\x32\x1c.livekit.SegmentedFileSuffix\x12\x18\n\x10\x64isable_manifest\x18\x08 \x01(\x08\x12\x1f\n\x02s3\x18\x05 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x06 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x07 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\t \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xe0\x01\n\x10\x44irectFileOutput\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x06 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xf8\x02\n\x0bImageOutput\x12\x18\n\x10\x63\x61pture_interval\x18\x01 \x01(\r\x12\r\n\x05width\x18\x02 \x01(\x05\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\x17\n\x0f\x66ilename_prefix\x18\x04 \x01(\t\x12\x31\n\x0f\x66ilename_suffix\x18\x05 \x01(\x0e\x32\x18.livekit.ImageFileSuffix\x12(\n\x0bimage_codec\x18\x06 \x01(\x0e\x32\x13.livekit.ImageCodec\x12\x18\n\x10\x64isable_manifest\x18\x07 \x01(\x08\x12\x1f\n\x02s3\x18\x08 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\t \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\n \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x0b \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\x8c\x02\n\x08S3Upload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t\x12\x18\n\x10\x66orce_path_style\x18\x06 \x01(\x08\x12\x31\n\x08metadata\x18\x07 \x03(\x0b\x32\x1f.livekit.S3Upload.MetadataEntry\x12\x0f\n\x07tagging\x18\x08 \x01(\t\x12\x1b\n\x13\x63ontent_disposition\x18\t \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"0\n\tGCPUpload\x12\x13\n\x0b\x63redentials\x18\x01 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x02 \x01(\t\"T\n\x0f\x41zureBlobUpload\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t\"d\n\x0c\x41liOSSUpload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t\"G\n\x0cStreamOutput\x12)\n\x08protocol\x18\x01 \x01(\x0e\x32\x17.livekit.StreamProtocol\x12\x0c\n\x04urls\x18\x02 \x03(\t\"\xb7\x02\n\x0f\x45ncodingOptions\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\r\n\x05\x64\x65pth\x18\x03 \x01(\x05\x12\x11\n\tframerate\x18\x04 \x01(\x05\x12(\n\x0b\x61udio_codec\x18\x05 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x15\n\raudio_bitrate\x18\x06 \x01(\x05\x12\x15\n\raudio_quality\x18\x0b \x01(\x05\x12\x17\n\x0f\x61udio_frequency\x18\x07 \x01(\x05\x12(\n\x0bvideo_codec\x18\x08 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x15\n\rvideo_bitrate\x18\t \x01(\x05\x12\x15\n\rvideo_quality\x18\x0c \x01(\x05\x12\x1a\n\x12key_frame_interval\x18\n \x01(\x01\"8\n\x13UpdateLayoutRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t\"]\n\x13UpdateStreamRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64_output_urls\x18\x02 \x03(\t\x12\x1a\n\x12remove_output_urls\x18\x03 \x03(\t\"I\n\x11ListEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x11\n\tegress_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\"8\n\x12ListEgressResponse\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.livekit.EgressInfo\"&\n\x11StopEgressRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\"\x91\x06\n\nEgressInfo\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0f\n\x07room_id\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\r \x01(\t\x12%\n\x06status\x18\x03 \x01(\x0e\x32\x15.livekit.EgressStatus\x12\x12\n\nstarted_at\x18\n \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x12 \x01(\x03\x12\r\n\x05\x65rror\x18\t \x01(\t\x12=\n\x0eroom_composite\x18\x04 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequestH\x00\x12(\n\x03web\x18\x0e \x01(\x0b\x32\x19.livekit.WebEgressRequestH\x00\x12\x38\n\x0bparticipant\x18\x13 \x01(\x0b\x32!.livekit.ParticipantEgressRequestH\x00\x12?\n\x0ftrack_composite\x18\x05 \x01(\x0b\x32$.livekit.TrackCompositeEgressRequestH\x00\x12,\n\x05track\x18\x06 \x01(\x0b\x32\x1b.livekit.TrackEgressRequestH\x00\x12-\n\x06stream\x18\x07 \x01(\x0b\x32\x17.livekit.StreamInfoListB\x02\x18\x01H\x01\x12%\n\x04\x66ile\x18\x08 \x01(\x0b\x32\x11.livekit.FileInfoB\x02\x18\x01H\x01\x12-\n\x08segments\x18\x0c \x01(\x0b\x32\x15.livekit.SegmentsInfoB\x02\x18\x01H\x01\x12+\n\x0estream_results\x18\x0f \x03(\x0b\x32\x13.livekit.StreamInfo\x12\'\n\x0c\x66ile_results\x18\x10 \x03(\x0b\x32\x11.livekit.FileInfo\x12.\n\x0fsegment_results\x18\x11 \x03(\x0b\x32\x15.livekit.SegmentsInfo\x12*\n\rimage_results\x18\x14 \x03(\x0b\x32\x13.livekit.ImagesInfoB\t\n\x07requestB\x08\n\x06result\"7\n\x0eStreamInfoList\x12!\n\x04info\x18\x01 \x03(\x0b\x32\x13.livekit.StreamInfo:\x02\x18\x01\"\xbc\x01\n\nStreamInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x04 \x01(\x03\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.livekit.StreamInfo.Status\x12\r\n\x05\x65rror\x18\x06 \x01(\t\".\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08\x46INISHED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\"t\n\x08\x46ileInfo\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x06 \x01(\x03\x12\x0c\n\x04size\x18\x04 \x01(\x03\x12\x10\n\x08location\x18\x05 \x01(\t\"\xd9\x01\n\x0cSegmentsInfo\x12\x15\n\rplaylist_name\x18\x01 \x01(\t\x12\x1a\n\x12live_playlist_name\x18\x08 \x01(\t\x12\x10\n\x08\x64uration\x18\x02 \x01(\x03\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\x19\n\x11playlist_location\x18\x04 \x01(\t\x12\x1e\n\x16live_playlist_location\x18\t \x01(\t\x12\x15\n\rsegment_count\x18\x05 \x01(\x03\x12\x12\n\nstarted_at\x18\x06 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x07 \x01(\x03\"G\n\nImagesInfo\x12\x13\n\x0bimage_count\x18\x01 \x01(\x03\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\"\xeb\x01\n\x15\x41utoParticipantEgress\x12\x30\n\x06preset\x18\x01 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x00\x12,\n\x08\x61\x64vanced\x18\x02 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x00\x12\x30\n\x0c\x66ile_outputs\x18\x03 \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12\x35\n\x0fsegment_outputs\x18\x04 \x03(\x0b\x32\x1c.livekit.SegmentedFileOutputB\t\n\x07options\"\xb6\x01\n\x0f\x41utoTrackEgress\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x42\x08\n\x06output*9\n\x0f\x45ncodedFileType\x12\x14\n\x10\x44\x45\x46\x41ULT_FILETYPE\x10\x00\x12\x07\n\x03MP4\x10\x01\x12\x07\n\x03OGG\x10\x02*N\n\x15SegmentedFileProtocol\x12#\n\x1f\x44\x45\x46\x41ULT_SEGMENTED_FILE_PROTOCOL\x10\x00\x12\x10\n\x0cHLS_PROTOCOL\x10\x01*/\n\x13SegmentedFileSuffix\x12\t\n\x05INDEX\x10\x00\x12\r\n\tTIMESTAMP\x10\x01*E\n\x0fImageFileSuffix\x12\x16\n\x12IMAGE_SUFFIX_INDEX\x10\x00\x12\x1a\n\x16IMAGE_SUFFIX_TIMESTAMP\x10\x01*0\n\x0eStreamProtocol\x12\x14\n\x10\x44\x45\x46\x41ULT_PROTOCOL\x10\x00\x12\x08\n\x04RTMP\x10\x01*\xcf\x01\n\x15\x45ncodingOptionsPreset\x12\x10\n\x0cH264_720P_30\x10\x00\x12\x10\n\x0cH264_720P_60\x10\x01\x12\x11\n\rH264_1080P_30\x10\x02\x12\x11\n\rH264_1080P_60\x10\x03\x12\x19\n\x15PORTRAIT_H264_720P_30\x10\x04\x12\x19\n\x15PORTRAIT_H264_720P_60\x10\x05\x12\x1a\n\x16PORTRAIT_H264_1080P_30\x10\x06\x12\x1a\n\x16PORTRAIT_H264_1080P_60\x10\x07*\x9f\x01\n\x0c\x45gressStatus\x12\x13\n\x0f\x45GRESS_STARTING\x10\x00\x12\x11\n\rEGRESS_ACTIVE\x10\x01\x12\x11\n\rEGRESS_ENDING\x10\x02\x12\x13\n\x0f\x45GRESS_COMPLETE\x10\x03\x12\x11\n\rEGRESS_FAILED\x10\x04\x12\x12\n\x0e\x45GRESS_ABORTED\x10\x05\x12\x18\n\x14\x45GRESS_LIMIT_REACHED\x10\x06\x32\x9c\x05\n\x06\x45gress\x12T\n\x18StartRoomCompositeEgress\x12#.livekit.RoomCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12@\n\x0eStartWebEgress\x12\x19.livekit.WebEgressRequest\x1a\x13.livekit.EgressInfo\x12P\n\x16StartParticipantEgress\x12!.livekit.ParticipantEgressRequest\x1a\x13.livekit.EgressInfo\x12V\n\x19StartTrackCompositeEgress\x12$.livekit.TrackCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12\x44\n\x10StartTrackEgress\x12\x1b.livekit.TrackEgressRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateLayout\x12\x1c.livekit.UpdateLayoutRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateStream\x12\x1c.livekit.UpdateStreamRequest\x1a\x13.livekit.EgressInfo\x12\x45\n\nListEgress\x12\x1a.livekit.ListEgressRequest\x1a\x1b.livekit.ListEgressResponse\x12=\n\nStopEgress\x12\x1a.livekit.StopEgressRequest\x1a\x13.livekit.EgressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14livekit_egress.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\xcd\x04\n\x1aRoomCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t\x12\x12\n\naudio_only\x18\x03 \x01(\x08\x12\x12\n\nvideo_only\x18\x04 \x01(\x08\x12\x17\n\x0f\x63ustom_base_url\x18\x05 \x01(\t\x12.\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x07 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\n \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x08 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\t \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\x0b \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x0c \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\r \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\x0e \x03(\x0b\x32\x14.livekit.ImageOutputB\x08\n\x06outputB\t\n\x07options\"\xb0\x04\n\x10WebEgressRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\naudio_only\x18\x02 \x01(\x08\x12\x12\n\nvideo_only\x18\x03 \x01(\x08\x12\x1a\n\x12\x61wait_start_signal\x18\x0c \x01(\x08\x12.\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\x06 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x07 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x08 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\t \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\n \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\x0b \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\r \x03(\x0b\x32\x14.livekit.ImageOutputB\x08\n\x06outputB\t\n\x07options\"\x85\x03\n\x18ParticipantEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x14\n\x0cscreen_share\x18\x03 \x01(\x08\x12\x30\n\x06preset\x18\x04 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x00\x12,\n\x08\x61\x64vanced\x18\x05 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x00\x12\x30\n\x0c\x66ile_outputs\x18\x06 \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x07 \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\x08 \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\t \x03(\x0b\x32\x14.livekit.ImageOutputB\t\n\x07options\"\xad\x04\n\x1bTrackCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x16\n\x0e\x61udio_track_id\x18\x02 \x01(\t\x12\x16\n\x0evideo_track_id\x18\x03 \x01(\t\x12.\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\x08 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x06 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x07 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\x0b \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x0c \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\r \x03(\x0b\x32\x1c.livekit.SegmentedFileOutput\x12+\n\rimage_outputs\x18\x0e \x03(\x0b\x32\x14.livekit.ImageOutputB\x08\n\x06outputB\t\n\x07options\"\x87\x01\n\x12TrackEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12)\n\x04\x66ile\x18\x03 \x01(\x0b\x32\x19.livekit.DirectFileOutputH\x00\x12\x17\n\rwebsocket_url\x18\x04 \x01(\tH\x00\x42\x08\n\x06output\"\x8e\x02\n\x11\x45ncodedFileOutput\x12+\n\tfile_type\x18\x01 \x01(\x0e\x32\x18.livekit.EncodedFileType\x12\x10\n\x08\x66ilepath\x18\x02 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x06 \x01(\x08\x12\x1f\n\x02s3\x18\x03 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x04 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x05 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x07 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xa0\x03\n\x13SegmentedFileOutput\x12\x30\n\x08protocol\x18\x01 \x01(\x0e\x32\x1e.livekit.SegmentedFileProtocol\x12\x17\n\x0f\x66ilename_prefix\x18\x02 \x01(\t\x12\x15\n\rplaylist_name\x18\x03 \x01(\t\x12\x1a\n\x12live_playlist_name\x18\x0b \x01(\t\x12\x18\n\x10segment_duration\x18\x04 \x01(\r\x12\x35\n\x0f\x66ilename_suffix\x18\n \x01(\x0e\x32\x1c.livekit.SegmentedFileSuffix\x12\x18\n\x10\x64isable_manifest\x18\x08 \x01(\x08\x12\x1f\n\x02s3\x18\x05 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x06 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x07 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\t \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xe0\x01\n\x10\x44irectFileOutput\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x06 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xf8\x02\n\x0bImageOutput\x12\x18\n\x10\x63\x61pture_interval\x18\x01 \x01(\r\x12\r\n\x05width\x18\x02 \x01(\x05\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\x17\n\x0f\x66ilename_prefix\x18\x04 \x01(\t\x12\x31\n\x0f\x66ilename_suffix\x18\x05 \x01(\x0e\x32\x18.livekit.ImageFileSuffix\x12(\n\x0bimage_codec\x18\x06 \x01(\x0e\x32\x13.livekit.ImageCodec\x12\x18\n\x10\x64isable_manifest\x18\x07 \x01(\x08\x12\x1f\n\x02s3\x18\x08 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\t \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\n \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x0b \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output\"\xb1\x02\n\x08S3Upload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t\x12\x18\n\x10\x66orce_path_style\x18\x06 \x01(\x08\x12\x31\n\x08metadata\x18\x07 \x03(\x0b\x32\x1f.livekit.S3Upload.MetadataEntry\x12\x0f\n\x07tagging\x18\x08 \x01(\t\x12\x1b\n\x13\x63ontent_disposition\x18\t \x01(\t\x12#\n\x05proxy\x18\n \x01(\x0b\x32\x14.livekit.ProxyConfig\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"U\n\tGCPUpload\x12\x13\n\x0b\x63redentials\x18\x01 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x02 \x01(\t\x12#\n\x05proxy\x18\x03 \x01(\x0b\x32\x14.livekit.ProxyConfig\"T\n\x0f\x41zureBlobUpload\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t\"d\n\x0c\x41liOSSUpload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t\">\n\x0bProxyConfig\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"G\n\x0cStreamOutput\x12)\n\x08protocol\x18\x01 \x01(\x0e\x32\x17.livekit.StreamProtocol\x12\x0c\n\x04urls\x18\x02 \x03(\t\"\xb7\x02\n\x0f\x45ncodingOptions\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\r\n\x05\x64\x65pth\x18\x03 \x01(\x05\x12\x11\n\tframerate\x18\x04 \x01(\x05\x12(\n\x0b\x61udio_codec\x18\x05 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x15\n\raudio_bitrate\x18\x06 \x01(\x05\x12\x15\n\raudio_quality\x18\x0b \x01(\x05\x12\x17\n\x0f\x61udio_frequency\x18\x07 \x01(\x05\x12(\n\x0bvideo_codec\x18\x08 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x15\n\rvideo_bitrate\x18\t \x01(\x05\x12\x15\n\rvideo_quality\x18\x0c \x01(\x05\x12\x1a\n\x12key_frame_interval\x18\n \x01(\x01\"8\n\x13UpdateLayoutRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t\"]\n\x13UpdateStreamRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64_output_urls\x18\x02 \x03(\t\x12\x1a\n\x12remove_output_urls\x18\x03 \x03(\t\"I\n\x11ListEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x11\n\tegress_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\"8\n\x12ListEgressResponse\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.livekit.EgressInfo\"&\n\x11StopEgressRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\"\xa2\x06\n\nEgressInfo\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0f\n\x07room_id\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\r \x01(\t\x12%\n\x06status\x18\x03 \x01(\x0e\x32\x15.livekit.EgressStatus\x12\x12\n\nstarted_at\x18\n \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x12 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x15 \x01(\t\x12\r\n\x05\x65rror\x18\t \x01(\t\x12=\n\x0eroom_composite\x18\x04 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequestH\x00\x12(\n\x03web\x18\x0e \x01(\x0b\x32\x19.livekit.WebEgressRequestH\x00\x12\x38\n\x0bparticipant\x18\x13 \x01(\x0b\x32!.livekit.ParticipantEgressRequestH\x00\x12?\n\x0ftrack_composite\x18\x05 \x01(\x0b\x32$.livekit.TrackCompositeEgressRequestH\x00\x12,\n\x05track\x18\x06 \x01(\x0b\x32\x1b.livekit.TrackEgressRequestH\x00\x12-\n\x06stream\x18\x07 \x01(\x0b\x32\x17.livekit.StreamInfoListB\x02\x18\x01H\x01\x12%\n\x04\x66ile\x18\x08 \x01(\x0b\x32\x11.livekit.FileInfoB\x02\x18\x01H\x01\x12-\n\x08segments\x18\x0c \x01(\x0b\x32\x15.livekit.SegmentsInfoB\x02\x18\x01H\x01\x12+\n\x0estream_results\x18\x0f \x03(\x0b\x32\x13.livekit.StreamInfo\x12\'\n\x0c\x66ile_results\x18\x10 \x03(\x0b\x32\x11.livekit.FileInfo\x12.\n\x0fsegment_results\x18\x11 \x03(\x0b\x32\x15.livekit.SegmentsInfo\x12*\n\rimage_results\x18\x14 \x03(\x0b\x32\x13.livekit.ImagesInfoB\t\n\x07requestB\x08\n\x06result\"7\n\x0eStreamInfoList\x12!\n\x04info\x18\x01 \x03(\x0b\x32\x13.livekit.StreamInfo:\x02\x18\x01\"\xbc\x01\n\nStreamInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x04 \x01(\x03\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.livekit.StreamInfo.Status\x12\r\n\x05\x65rror\x18\x06 \x01(\t\".\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08\x46INISHED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\"t\n\x08\x46ileInfo\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x06 \x01(\x03\x12\x0c\n\x04size\x18\x04 \x01(\x03\x12\x10\n\x08location\x18\x05 \x01(\t\"\xd9\x01\n\x0cSegmentsInfo\x12\x15\n\rplaylist_name\x18\x01 \x01(\t\x12\x1a\n\x12live_playlist_name\x18\x08 \x01(\t\x12\x10\n\x08\x64uration\x18\x02 \x01(\x03\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\x19\n\x11playlist_location\x18\x04 \x01(\t\x12\x1e\n\x16live_playlist_location\x18\t \x01(\t\x12\x15\n\rsegment_count\x18\x05 \x01(\x03\x12\x12\n\nstarted_at\x18\x06 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x07 \x01(\x03\"G\n\nImagesInfo\x12\x13\n\x0bimage_count\x18\x01 \x01(\x03\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\"\xeb\x01\n\x15\x41utoParticipantEgress\x12\x30\n\x06preset\x18\x01 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x00\x12,\n\x08\x61\x64vanced\x18\x02 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x00\x12\x30\n\x0c\x66ile_outputs\x18\x03 \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12\x35\n\x0fsegment_outputs\x18\x04 \x03(\x0b\x32\x1c.livekit.SegmentedFileOutputB\t\n\x07options\"\xb6\x01\n\x0f\x41utoTrackEgress\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x42\x08\n\x06output*9\n\x0f\x45ncodedFileType\x12\x14\n\x10\x44\x45\x46\x41ULT_FILETYPE\x10\x00\x12\x07\n\x03MP4\x10\x01\x12\x07\n\x03OGG\x10\x02*N\n\x15SegmentedFileProtocol\x12#\n\x1f\x44\x45\x46\x41ULT_SEGMENTED_FILE_PROTOCOL\x10\x00\x12\x10\n\x0cHLS_PROTOCOL\x10\x01*/\n\x13SegmentedFileSuffix\x12\t\n\x05INDEX\x10\x00\x12\r\n\tTIMESTAMP\x10\x01*E\n\x0fImageFileSuffix\x12\x16\n\x12IMAGE_SUFFIX_INDEX\x10\x00\x12\x1a\n\x16IMAGE_SUFFIX_TIMESTAMP\x10\x01*0\n\x0eStreamProtocol\x12\x14\n\x10\x44\x45\x46\x41ULT_PROTOCOL\x10\x00\x12\x08\n\x04RTMP\x10\x01*\xcf\x01\n\x15\x45ncodingOptionsPreset\x12\x10\n\x0cH264_720P_30\x10\x00\x12\x10\n\x0cH264_720P_60\x10\x01\x12\x11\n\rH264_1080P_30\x10\x02\x12\x11\n\rH264_1080P_60\x10\x03\x12\x19\n\x15PORTRAIT_H264_720P_30\x10\x04\x12\x19\n\x15PORTRAIT_H264_720P_60\x10\x05\x12\x1a\n\x16PORTRAIT_H264_1080P_30\x10\x06\x12\x1a\n\x16PORTRAIT_H264_1080P_60\x10\x07*\x9f\x01\n\x0c\x45gressStatus\x12\x13\n\x0f\x45GRESS_STARTING\x10\x00\x12\x11\n\rEGRESS_ACTIVE\x10\x01\x12\x11\n\rEGRESS_ENDING\x10\x02\x12\x13\n\x0f\x45GRESS_COMPLETE\x10\x03\x12\x11\n\rEGRESS_FAILED\x10\x04\x12\x12\n\x0e\x45GRESS_ABORTED\x10\x05\x12\x18\n\x14\x45GRESS_LIMIT_REACHED\x10\x06\x32\x9c\x05\n\x06\x45gress\x12T\n\x18StartRoomCompositeEgress\x12#.livekit.RoomCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12@\n\x0eStartWebEgress\x12\x19.livekit.WebEgressRequest\x1a\x13.livekit.EgressInfo\x12P\n\x16StartParticipantEgress\x12!.livekit.ParticipantEgressRequest\x1a\x13.livekit.EgressInfo\x12V\n\x19StartTrackCompositeEgress\x12$.livekit.TrackCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12\x44\n\x10StartTrackEgress\x12\x1b.livekit.TrackEgressRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateLayout\x12\x1c.livekit.UpdateLayoutRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateStream\x12\x1c.livekit.UpdateStreamRequest\x1a\x13.livekit.EgressInfo\x12\x45\n\nListEgress\x12\x1a.livekit.ListEgressRequest\x1a\x1b.livekit.ListEgressResponse\x12=\n\nStopEgress\x12\x1a.livekit.StopEgressRequest\x1a\x13.livekit.EgressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'egress', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
@@ -47,28 +47,28 @@
   _globals['_EGRESSINFO'].fields_by_name['stream']._serialized_options = b'\030\001'
   _globals['_EGRESSINFO'].fields_by_name['file']._options = None
   _globals['_EGRESSINFO'].fields_by_name['file']._serialized_options = b'\030\001'
   _globals['_EGRESSINFO'].fields_by_name['segments']._options = None
   _globals['_EGRESSINFO'].fields_by_name['segments']._serialized_options = b'\030\001'
   _globals['_STREAMINFOLIST']._options = None
   _globals['_STREAMINFOLIST']._serialized_options = b'\030\001'
-  _globals['_ENCODEDFILETYPE']._serialized_start=6690
-  _globals['_ENCODEDFILETYPE']._serialized_end=6747
-  _globals['_SEGMENTEDFILEPROTOCOL']._serialized_start=6749
-  _globals['_SEGMENTEDFILEPROTOCOL']._serialized_end=6827
-  _globals['_SEGMENTEDFILESUFFIX']._serialized_start=6829
-  _globals['_SEGMENTEDFILESUFFIX']._serialized_end=6876
-  _globals['_IMAGEFILESUFFIX']._serialized_start=6878
-  _globals['_IMAGEFILESUFFIX']._serialized_end=6947
-  _globals['_STREAMPROTOCOL']._serialized_start=6949
-  _globals['_STREAMPROTOCOL']._serialized_end=6997
-  _globals['_ENCODINGOPTIONSPRESET']._serialized_start=7000
-  _globals['_ENCODINGOPTIONSPRESET']._serialized_end=7207
-  _globals['_EGRESSSTATUS']._serialized_start=7210
-  _globals['_EGRESSSTATUS']._serialized_end=7369
+  _globals['_ENCODEDFILETYPE']._serialized_start=6845
+  _globals['_ENCODEDFILETYPE']._serialized_end=6902
+  _globals['_SEGMENTEDFILEPROTOCOL']._serialized_start=6904
+  _globals['_SEGMENTEDFILEPROTOCOL']._serialized_end=6982
+  _globals['_SEGMENTEDFILESUFFIX']._serialized_start=6984
+  _globals['_SEGMENTEDFILESUFFIX']._serialized_end=7031
+  _globals['_IMAGEFILESUFFIX']._serialized_start=7033
+  _globals['_IMAGEFILESUFFIX']._serialized_end=7102
+  _globals['_STREAMPROTOCOL']._serialized_start=7104
+  _globals['_STREAMPROTOCOL']._serialized_end=7152
+  _globals['_ENCODINGOPTIONSPRESET']._serialized_start=7155
+  _globals['_ENCODINGOPTIONSPRESET']._serialized_end=7362
+  _globals['_EGRESSSTATUS']._serialized_start=7365
+  _globals['_EGRESSSTATUS']._serialized_end=7524
   _globals['_ROOMCOMPOSITEEGRESSREQUEST']._serialized_start=56
   _globals['_ROOMCOMPOSITEEGRESSREQUEST']._serialized_end=645
   _globals['_WEBEGRESSREQUEST']._serialized_start=648
   _globals['_WEBEGRESSREQUEST']._serialized_end=1208
   _globals['_PARTICIPANTEGRESSREQUEST']._serialized_start=1211
   _globals['_PARTICIPANTEGRESSREQUEST']._serialized_end=1600
   _globals['_TRACKCOMPOSITEEGRESSREQUEST']._serialized_start=1603
@@ -80,51 +80,53 @@
   _globals['_SEGMENTEDFILEOUTPUT']._serialized_start=2574
   _globals['_SEGMENTEDFILEOUTPUT']._serialized_end=2990
   _globals['_DIRECTFILEOUTPUT']._serialized_start=2993
   _globals['_DIRECTFILEOUTPUT']._serialized_end=3217
   _globals['_IMAGEOUTPUT']._serialized_start=3220
   _globals['_IMAGEOUTPUT']._serialized_end=3596
   _globals['_S3UPLOAD']._serialized_start=3599
-  _globals['_S3UPLOAD']._serialized_end=3867
-  _globals['_S3UPLOAD_METADATAENTRY']._serialized_start=3820
-  _globals['_S3UPLOAD_METADATAENTRY']._serialized_end=3867
-  _globals['_GCPUPLOAD']._serialized_start=3869
-  _globals['_GCPUPLOAD']._serialized_end=3917
-  _globals['_AZUREBLOBUPLOAD']._serialized_start=3919
-  _globals['_AZUREBLOBUPLOAD']._serialized_end=4003
-  _globals['_ALIOSSUPLOAD']._serialized_start=4005
-  _globals['_ALIOSSUPLOAD']._serialized_end=4105
-  _globals['_STREAMOUTPUT']._serialized_start=4107
-  _globals['_STREAMOUTPUT']._serialized_end=4178
-  _globals['_ENCODINGOPTIONS']._serialized_start=4181
-  _globals['_ENCODINGOPTIONS']._serialized_end=4492
-  _globals['_UPDATELAYOUTREQUEST']._serialized_start=4494
-  _globals['_UPDATELAYOUTREQUEST']._serialized_end=4550
-  _globals['_UPDATESTREAMREQUEST']._serialized_start=4552
-  _globals['_UPDATESTREAMREQUEST']._serialized_end=4645
-  _globals['_LISTEGRESSREQUEST']._serialized_start=4647
-  _globals['_LISTEGRESSREQUEST']._serialized_end=4720
-  _globals['_LISTEGRESSRESPONSE']._serialized_start=4722
-  _globals['_LISTEGRESSRESPONSE']._serialized_end=4778
-  _globals['_STOPEGRESSREQUEST']._serialized_start=4780
-  _globals['_STOPEGRESSREQUEST']._serialized_end=4818
-  _globals['_EGRESSINFO']._serialized_start=4821
-  _globals['_EGRESSINFO']._serialized_end=5606
-  _globals['_STREAMINFOLIST']._serialized_start=5608
-  _globals['_STREAMINFOLIST']._serialized_end=5663
-  _globals['_STREAMINFO']._serialized_start=5666
-  _globals['_STREAMINFO']._serialized_end=5854
-  _globals['_STREAMINFO_STATUS']._serialized_start=5808
-  _globals['_STREAMINFO_STATUS']._serialized_end=5854
-  _globals['_FILEINFO']._serialized_start=5856
-  _globals['_FILEINFO']._serialized_end=5972
-  _globals['_SEGMENTSINFO']._serialized_start=5975
-  _globals['_SEGMENTSINFO']._serialized_end=6192
-  _globals['_IMAGESINFO']._serialized_start=6194
-  _globals['_IMAGESINFO']._serialized_end=6265
-  _globals['_AUTOPARTICIPANTEGRESS']._serialized_start=6268
-  _globals['_AUTOPARTICIPANTEGRESS']._serialized_end=6503
-  _globals['_AUTOTRACKEGRESS']._serialized_start=6506
-  _globals['_AUTOTRACKEGRESS']._serialized_end=6688
-  _globals['_EGRESS']._serialized_start=7372
-  _globals['_EGRESS']._serialized_end=8040
+  _globals['_S3UPLOAD']._serialized_end=3904
+  _globals['_S3UPLOAD_METADATAENTRY']._serialized_start=3857
+  _globals['_S3UPLOAD_METADATAENTRY']._serialized_end=3904
+  _globals['_GCPUPLOAD']._serialized_start=3906
+  _globals['_GCPUPLOAD']._serialized_end=3991
+  _globals['_AZUREBLOBUPLOAD']._serialized_start=3993
+  _globals['_AZUREBLOBUPLOAD']._serialized_end=4077
+  _globals['_ALIOSSUPLOAD']._serialized_start=4079
+  _globals['_ALIOSSUPLOAD']._serialized_end=4179
+  _globals['_PROXYCONFIG']._serialized_start=4181
+  _globals['_PROXYCONFIG']._serialized_end=4243
+  _globals['_STREAMOUTPUT']._serialized_start=4245
+  _globals['_STREAMOUTPUT']._serialized_end=4316
+  _globals['_ENCODINGOPTIONS']._serialized_start=4319
+  _globals['_ENCODINGOPTIONS']._serialized_end=4630
+  _globals['_UPDATELAYOUTREQUEST']._serialized_start=4632
+  _globals['_UPDATELAYOUTREQUEST']._serialized_end=4688
+  _globals['_UPDATESTREAMREQUEST']._serialized_start=4690
+  _globals['_UPDATESTREAMREQUEST']._serialized_end=4783
+  _globals['_LISTEGRESSREQUEST']._serialized_start=4785
+  _globals['_LISTEGRESSREQUEST']._serialized_end=4858
+  _globals['_LISTEGRESSRESPONSE']._serialized_start=4860
+  _globals['_LISTEGRESSRESPONSE']._serialized_end=4916
+  _globals['_STOPEGRESSREQUEST']._serialized_start=4918
+  _globals['_STOPEGRESSREQUEST']._serialized_end=4956
+  _globals['_EGRESSINFO']._serialized_start=4959
+  _globals['_EGRESSINFO']._serialized_end=5761
+  _globals['_STREAMINFOLIST']._serialized_start=5763
+  _globals['_STREAMINFOLIST']._serialized_end=5818
+  _globals['_STREAMINFO']._serialized_start=5821
+  _globals['_STREAMINFO']._serialized_end=6009
+  _globals['_STREAMINFO_STATUS']._serialized_start=5963
+  _globals['_STREAMINFO_STATUS']._serialized_end=6009
+  _globals['_FILEINFO']._serialized_start=6011
+  _globals['_FILEINFO']._serialized_end=6127
+  _globals['_SEGMENTSINFO']._serialized_start=6130
+  _globals['_SEGMENTSINFO']._serialized_end=6347
+  _globals['_IMAGESINFO']._serialized_start=6349
+  _globals['_IMAGESINFO']._serialized_end=6420
+  _globals['_AUTOPARTICIPANTEGRESS']._serialized_start=6423
+  _globals['_AUTOPARTICIPANTEGRESS']._serialized_end=6658
+  _globals['_AUTOTRACKEGRESS']._serialized_start=6661
+  _globals['_AUTOTRACKEGRESS']._serialized_end=6843
+  _globals['_EGRESS']._serialized_start=7527
+  _globals['_EGRESS']._serialized_end=8195
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/egress.pyi` & `livekit-protocol-0.4.0/livekit/protocol/egress.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     s3: S3Upload
     gcp: GCPUpload
     azure: AzureBlobUpload
     aliOSS: AliOSSUpload
     def __init__(self, capture_interval: _Optional[int] = ..., width: _Optional[int] = ..., height: _Optional[int] = ..., filename_prefix: _Optional[str] = ..., filename_suffix: _Optional[_Union[ImageFileSuffix, str]] = ..., image_codec: _Optional[_Union[_models.ImageCodec, str]] = ..., disable_manifest: bool = ..., s3: _Optional[_Union[S3Upload, _Mapping]] = ..., gcp: _Optional[_Union[GCPUpload, _Mapping]] = ..., azure: _Optional[_Union[AzureBlobUpload, _Mapping]] = ..., aliOSS: _Optional[_Union[AliOSSUpload, _Mapping]] = ...) -> None: ...
 
 class S3Upload(_message.Message):
-    __slots__ = ("access_key", "secret", "region", "endpoint", "bucket", "force_path_style", "metadata", "tagging", "content_disposition")
+    __slots__ = ("access_key", "secret", "region", "endpoint", "bucket", "force_path_style", "metadata", "tagging", "content_disposition", "proxy")
     class MetadataEntry(_message.Message):
         __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
@@ -304,32 +304,36 @@
     REGION_FIELD_NUMBER: _ClassVar[int]
     ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     FORCE_PATH_STYLE_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     TAGGING_FIELD_NUMBER: _ClassVar[int]
     CONTENT_DISPOSITION_FIELD_NUMBER: _ClassVar[int]
+    PROXY_FIELD_NUMBER: _ClassVar[int]
     access_key: str
     secret: str
     region: str
     endpoint: str
     bucket: str
     force_path_style: bool
     metadata: _containers.ScalarMap[str, str]
     tagging: str
     content_disposition: str
-    def __init__(self, access_key: _Optional[str] = ..., secret: _Optional[str] = ..., region: _Optional[str] = ..., endpoint: _Optional[str] = ..., bucket: _Optional[str] = ..., force_path_style: bool = ..., metadata: _Optional[_Mapping[str, str]] = ..., tagging: _Optional[str] = ..., content_disposition: _Optional[str] = ...) -> None: ...
+    proxy: ProxyConfig
+    def __init__(self, access_key: _Optional[str] = ..., secret: _Optional[str] = ..., region: _Optional[str] = ..., endpoint: _Optional[str] = ..., bucket: _Optional[str] = ..., force_path_style: bool = ..., metadata: _Optional[_Mapping[str, str]] = ..., tagging: _Optional[str] = ..., content_disposition: _Optional[str] = ..., proxy: _Optional[_Union[ProxyConfig, _Mapping]] = ...) -> None: ...
 
 class GCPUpload(_message.Message):
-    __slots__ = ("credentials", "bucket")
+    __slots__ = ("credentials", "bucket", "proxy")
     CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
+    PROXY_FIELD_NUMBER: _ClassVar[int]
     credentials: str
     bucket: str
-    def __init__(self, credentials: _Optional[str] = ..., bucket: _Optional[str] = ...) -> None: ...
+    proxy: ProxyConfig
+    def __init__(self, credentials: _Optional[str] = ..., bucket: _Optional[str] = ..., proxy: _Optional[_Union[ProxyConfig, _Mapping]] = ...) -> None: ...
 
 class AzureBlobUpload(_message.Message):
     __slots__ = ("account_name", "account_key", "container_name")
     ACCOUNT_NAME_FIELD_NUMBER: _ClassVar[int]
     ACCOUNT_KEY_FIELD_NUMBER: _ClassVar[int]
     CONTAINER_NAME_FIELD_NUMBER: _ClassVar[int]
     account_name: str
@@ -347,14 +351,24 @@
     access_key: str
     secret: str
     region: str
     endpoint: str
     bucket: str
     def __init__(self, access_key: _Optional[str] = ..., secret: _Optional[str] = ..., region: _Optional[str] = ..., endpoint: _Optional[str] = ..., bucket: _Optional[str] = ...) -> None: ...
 
+class ProxyConfig(_message.Message):
+    __slots__ = ("url", "username", "password")
+    URL_FIELD_NUMBER: _ClassVar[int]
+    USERNAME_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    url: str
+    username: str
+    password: str
+    def __init__(self, url: _Optional[str] = ..., username: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
+
 class StreamOutput(_message.Message):
     __slots__ = ("protocol", "urls")
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     URLS_FIELD_NUMBER: _ClassVar[int]
     protocol: StreamProtocol
     urls: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, protocol: _Optional[_Union[StreamProtocol, str]] = ..., urls: _Optional[_Iterable[str]] = ...) -> None: ...
@@ -424,22 +438,23 @@
 class StopEgressRequest(_message.Message):
     __slots__ = ("egress_id",)
     EGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     egress_id: str
     def __init__(self, egress_id: _Optional[str] = ...) -> None: ...
 
 class EgressInfo(_message.Message):
-    __slots__ = ("egress_id", "room_id", "room_name", "status", "started_at", "ended_at", "updated_at", "error", "room_composite", "web", "participant", "track_composite", "track", "stream", "file", "segments", "stream_results", "file_results", "segment_results", "image_results")
+    __slots__ = ("egress_id", "room_id", "room_name", "status", "started_at", "ended_at", "updated_at", "details", "error", "room_composite", "web", "participant", "track_composite", "track", "stream", "file", "segments", "stream_results", "file_results", "segment_results", "image_results")
     EGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
     UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
+    DETAILS_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     ROOM_COMPOSITE_FIELD_NUMBER: _ClassVar[int]
     WEB_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     TRACK_COMPOSITE_FIELD_NUMBER: _ClassVar[int]
     TRACK_FIELD_NUMBER: _ClassVar[int]
     STREAM_FIELD_NUMBER: _ClassVar[int]
@@ -452,28 +467,29 @@
     egress_id: str
     room_id: str
     room_name: str
     status: EgressStatus
     started_at: int
     ended_at: int
     updated_at: int
+    details: str
     error: str
     room_composite: RoomCompositeEgressRequest
     web: WebEgressRequest
     participant: ParticipantEgressRequest
     track_composite: TrackCompositeEgressRequest
     track: TrackEgressRequest
     stream: StreamInfoList
     file: FileInfo
     segments: SegmentsInfo
     stream_results: _containers.RepeatedCompositeFieldContainer[StreamInfo]
     file_results: _containers.RepeatedCompositeFieldContainer[FileInfo]
     segment_results: _containers.RepeatedCompositeFieldContainer[SegmentsInfo]
     image_results: _containers.RepeatedCompositeFieldContainer[ImagesInfo]
-    def __init__(self, egress_id: _Optional[str] = ..., room_id: _Optional[str] = ..., room_name: _Optional[str] = ..., status: _Optional[_Union[EgressStatus, str]] = ..., started_at: _Optional[int] = ..., ended_at: _Optional[int] = ..., updated_at: _Optional[int] = ..., error: _Optional[str] = ..., room_composite: _Optional[_Union[RoomCompositeEgressRequest, _Mapping]] = ..., web: _Optional[_Union[WebEgressRequest, _Mapping]] = ..., participant: _Optional[_Union[ParticipantEgressRequest, _Mapping]] = ..., track_composite: _Optional[_Union[TrackCompositeEgressRequest, _Mapping]] = ..., track: _Optional[_Union[TrackEgressRequest, _Mapping]] = ..., stream: _Optional[_Union[StreamInfoList, _Mapping]] = ..., file: _Optional[_Union[FileInfo, _Mapping]] = ..., segments: _Optional[_Union[SegmentsInfo, _Mapping]] = ..., stream_results: _Optional[_Iterable[_Union[StreamInfo, _Mapping]]] = ..., file_results: _Optional[_Iterable[_Union[FileInfo, _Mapping]]] = ..., segment_results: _Optional[_Iterable[_Union[SegmentsInfo, _Mapping]]] = ..., image_results: _Optional[_Iterable[_Union[ImagesInfo, _Mapping]]] = ...) -> None: ...
+    def __init__(self, egress_id: _Optional[str] = ..., room_id: _Optional[str] = ..., room_name: _Optional[str] = ..., status: _Optional[_Union[EgressStatus, str]] = ..., started_at: _Optional[int] = ..., ended_at: _Optional[int] = ..., updated_at: _Optional[int] = ..., details: _Optional[str] = ..., error: _Optional[str] = ..., room_composite: _Optional[_Union[RoomCompositeEgressRequest, _Mapping]] = ..., web: _Optional[_Union[WebEgressRequest, _Mapping]] = ..., participant: _Optional[_Union[ParticipantEgressRequest, _Mapping]] = ..., track_composite: _Optional[_Union[TrackCompositeEgressRequest, _Mapping]] = ..., track: _Optional[_Union[TrackEgressRequest, _Mapping]] = ..., stream: _Optional[_Union[StreamInfoList, _Mapping]] = ..., file: _Optional[_Union[FileInfo, _Mapping]] = ..., segments: _Optional[_Union[SegmentsInfo, _Mapping]] = ..., stream_results: _Optional[_Iterable[_Union[StreamInfo, _Mapping]]] = ..., file_results: _Optional[_Iterable[_Union[FileInfo, _Mapping]]] = ..., segment_results: _Optional[_Iterable[_Union[SegmentsInfo, _Mapping]]] = ..., image_results: _Optional[_Iterable[_Union[ImagesInfo, _Mapping]]] = ...) -> None: ...
 
 class StreamInfoList(_message.Message):
     __slots__ = ("info",)
     INFO_FIELD_NUMBER: _ClassVar[int]
     info: _containers.RepeatedCompositeFieldContainer[StreamInfo]
     def __init__(self, info: _Optional[_Iterable[_Union[StreamInfo, _Mapping]]] = ...) -> None: ...
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/ingress.py` & `livekit-protocol-0.4.0/livekit/protocol/ingress.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,52 +11,52 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import models as _models_
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15livekit_ingress.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\x9d\x02\n\x14\x43reateIngressRequest\x12)\n\ninput_type\x18\x01 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x0b\n\x03url\x18\t \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1a\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\"\xcd\x01\n\x13IngressAudioOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressAudioEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressAudioEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\xcd\x01\n\x13IngressVideoOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressVideoEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressVideoEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\x7f\n\x1bIngressAudioEncodingOptions\x12(\n\x0b\x61udio_codec\x18\x01 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x0f\n\x07\x62itrate\x18\x02 \x01(\r\x12\x13\n\x0b\x64isable_dtx\x18\x03 \x01(\x08\x12\x10\n\x08\x63hannels\x18\x04 \x01(\r\"\x80\x01\n\x1bIngressVideoEncodingOptions\x12(\n\x0bvideo_codec\x18\x01 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x12\n\nframe_rate\x18\x02 \x01(\x01\x12#\n\x06layers\x18\x03 \x03(\x0b\x32\x13.livekit.VideoLayer\"\xf4\x02\n\x0bIngressInfo\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nstream_key\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12)\n\ninput_type\x18\x05 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x1a\n\x12\x62ypass_transcoding\x18\r \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\x12\x11\n\troom_name\x18\x08 \x01(\t\x12\x1c\n\x14participant_identity\x18\t \x01(\t\x12\x18\n\x10participant_name\x18\n \x01(\t\x12\x10\n\x08reusable\x18\x0b \x01(\x08\x12$\n\x05state\x18\x0c \x01(\x0b\x32\x15.livekit.IngressState\"\x8a\x03\n\x0cIngressState\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.livekit.IngressState.Status\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\'\n\x05video\x18\x03 \x01(\x0b\x32\x18.livekit.InputVideoState\x12\'\n\x05\x61udio\x18\x04 \x01(\x0b\x32\x18.livekit.InputAudioState\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x12\n\nstarted_at\x18\x07 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x08 \x01(\x03\x12\x13\n\x0bresource_id\x18\t \x01(\t\x12\"\n\x06tracks\x18\x06 \x03(\x0b\x32\x12.livekit.TrackInfo\"{\n\x06Status\x12\x15\n\x11\x45NDPOINT_INACTIVE\x10\x00\x12\x16\n\x12\x45NDPOINT_BUFFERING\x10\x01\x12\x17\n\x13\x45NDPOINT_PUBLISHING\x10\x02\x12\x12\n\x0e\x45NDPOINT_ERROR\x10\x03\x12\x15\n\x11\x45NDPOINT_COMPLETE\x10\x04\"o\n\x0fInputVideoState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x11\n\tframerate\x18\x05 \x01(\x01\"d\n\x0fInputAudioState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\x10\n\x08\x63hannels\x18\x03 \x01(\r\x12\x13\n\x0bsample_rate\x18\x04 \x01(\r\"\x95\x02\n\x14UpdateIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1f\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08H\x00\x88\x01\x01\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptionsB\x15\n\x13_bypass_transcoding\";\n\x12ListIngressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x12\n\ningress_id\x18\x02 \x01(\t\":\n\x13ListIngressResponse\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.livekit.IngressInfo\"*\n\x14\x44\x65leteIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t*=\n\x0cIngressInput\x12\x0e\n\nRTMP_INPUT\x10\x00\x12\x0e\n\nWHIP_INPUT\x10\x01\x12\r\n\tURL_INPUT\x10\x02*I\n\x1aIngressAudioEncodingPreset\x12\x16\n\x12OPUS_STEREO_96KBPS\x10\x00\x12\x13\n\x0fOPUS_MONO_64KBS\x10\x01*\x84\x03\n\x1aIngressVideoEncodingPreset\x12\x1c\n\x18H264_720P_30FPS_3_LAYERS\x10\x00\x12\x1d\n\x19H264_1080P_30FPS_3_LAYERS\x10\x01\x12\x1c\n\x18H264_540P_25FPS_2_LAYERS\x10\x02\x12\x1b\n\x17H264_720P_30FPS_1_LAYER\x10\x03\x12\x1c\n\x18H264_1080P_30FPS_1_LAYER\x10\x04\x12(\n$H264_720P_30FPS_3_LAYERS_HIGH_MOTION\x10\x05\x12)\n%H264_1080P_30FPS_3_LAYERS_HIGH_MOTION\x10\x06\x12(\n$H264_540P_25FPS_2_LAYERS_HIGH_MOTION\x10\x07\x12\'\n#H264_720P_30FPS_1_LAYER_HIGH_MOTION\x10\x08\x12(\n$H264_1080P_30FPS_1_LAYER_HIGH_MOTION\x10\t2\xa5\x02\n\x07Ingress\x12\x44\n\rCreateIngress\x12\x1d.livekit.CreateIngressRequest\x1a\x14.livekit.IngressInfo\x12\x44\n\rUpdateIngress\x12\x1d.livekit.UpdateIngressRequest\x1a\x14.livekit.IngressInfo\x12H\n\x0bListIngress\x12\x1b.livekit.ListIngressRequest\x1a\x1c.livekit.ListIngressResponse\x12\x44\n\rDeleteIngress\x12\x1d.livekit.DeleteIngressRequest\x1a\x14.livekit.IngressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15livekit_ingress.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\xbb\x02\n\x14\x43reateIngressRequest\x12)\n\ninput_type\x18\x01 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x0b\n\x03url\x18\t \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\n \x01(\t\x12\x1a\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\"\xcd\x01\n\x13IngressAudioOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressAudioEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressAudioEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\xcd\x01\n\x13IngressVideoOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressVideoEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressVideoEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\x7f\n\x1bIngressAudioEncodingOptions\x12(\n\x0b\x61udio_codec\x18\x01 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x0f\n\x07\x62itrate\x18\x02 \x01(\r\x12\x13\n\x0b\x64isable_dtx\x18\x03 \x01(\x08\x12\x10\n\x08\x63hannels\x18\x04 \x01(\r\"\x80\x01\n\x1bIngressVideoEncodingOptions\x12(\n\x0bvideo_codec\x18\x01 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x12\n\nframe_rate\x18\x02 \x01(\x01\x12#\n\x06layers\x18\x03 \x03(\x0b\x32\x13.livekit.VideoLayer\"\x92\x03\n\x0bIngressInfo\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nstream_key\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12)\n\ninput_type\x18\x05 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x1a\n\x12\x62ypass_transcoding\x18\r \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\x12\x11\n\troom_name\x18\x08 \x01(\t\x12\x1c\n\x14participant_identity\x18\t \x01(\t\x12\x18\n\x10participant_name\x18\n \x01(\t\x12\x1c\n\x14participant_metadata\x18\x0e \x01(\t\x12\x10\n\x08reusable\x18\x0b \x01(\x08\x12$\n\x05state\x18\x0c \x01(\x0b\x32\x15.livekit.IngressState\"\x8a\x03\n\x0cIngressState\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.livekit.IngressState.Status\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\'\n\x05video\x18\x03 \x01(\x0b\x32\x18.livekit.InputVideoState\x12\'\n\x05\x61udio\x18\x04 \x01(\x0b\x32\x18.livekit.InputAudioState\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x12\n\nstarted_at\x18\x07 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x08 \x01(\x03\x12\x13\n\x0bresource_id\x18\t \x01(\t\x12\"\n\x06tracks\x18\x06 \x03(\x0b\x32\x12.livekit.TrackInfo\"{\n\x06Status\x12\x15\n\x11\x45NDPOINT_INACTIVE\x10\x00\x12\x16\n\x12\x45NDPOINT_BUFFERING\x10\x01\x12\x17\n\x13\x45NDPOINT_PUBLISHING\x10\x02\x12\x12\n\x0e\x45NDPOINT_ERROR\x10\x03\x12\x15\n\x11\x45NDPOINT_COMPLETE\x10\x04\"o\n\x0fInputVideoState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x11\n\tframerate\x18\x05 \x01(\x01\"d\n\x0fInputAudioState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\x10\n\x08\x63hannels\x18\x03 \x01(\r\x12\x13\n\x0bsample_rate\x18\x04 \x01(\r\"\xb3\x02\n\x14UpdateIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\t \x01(\t\x12\x1f\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08H\x00\x88\x01\x01\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptionsB\x15\n\x13_bypass_transcoding\";\n\x12ListIngressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x12\n\ningress_id\x18\x02 \x01(\t\":\n\x13ListIngressResponse\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.livekit.IngressInfo\"*\n\x14\x44\x65leteIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t*=\n\x0cIngressInput\x12\x0e\n\nRTMP_INPUT\x10\x00\x12\x0e\n\nWHIP_INPUT\x10\x01\x12\r\n\tURL_INPUT\x10\x02*I\n\x1aIngressAudioEncodingPreset\x12\x16\n\x12OPUS_STEREO_96KBPS\x10\x00\x12\x13\n\x0fOPUS_MONO_64KBS\x10\x01*\x84\x03\n\x1aIngressVideoEncodingPreset\x12\x1c\n\x18H264_720P_30FPS_3_LAYERS\x10\x00\x12\x1d\n\x19H264_1080P_30FPS_3_LAYERS\x10\x01\x12\x1c\n\x18H264_540P_25FPS_2_LAYERS\x10\x02\x12\x1b\n\x17H264_720P_30FPS_1_LAYER\x10\x03\x12\x1c\n\x18H264_1080P_30FPS_1_LAYER\x10\x04\x12(\n$H264_720P_30FPS_3_LAYERS_HIGH_MOTION\x10\x05\x12)\n%H264_1080P_30FPS_3_LAYERS_HIGH_MOTION\x10\x06\x12(\n$H264_540P_25FPS_2_LAYERS_HIGH_MOTION\x10\x07\x12\'\n#H264_720P_30FPS_1_LAYER_HIGH_MOTION\x10\x08\x12(\n$H264_1080P_30FPS_1_LAYER_HIGH_MOTION\x10\t2\xa5\x02\n\x07Ingress\x12\x44\n\rCreateIngress\x12\x1d.livekit.CreateIngressRequest\x1a\x14.livekit.IngressInfo\x12\x44\n\rUpdateIngress\x12\x1d.livekit.UpdateIngressRequest\x1a\x14.livekit.IngressInfo\x12H\n\x0bListIngress\x12\x1b.livekit.ListIngressRequest\x1a\x1c.livekit.ListIngressResponse\x12\x44\n\rDeleteIngress\x12\x1d.livekit.DeleteIngressRequest\x1a\x14.livekit.IngressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ingress', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
-  _globals['_INGRESSINPUT']._serialized_start=2452
-  _globals['_INGRESSINPUT']._serialized_end=2513
-  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_start=2515
-  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_end=2588
-  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_start=2591
-  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_end=2979
+  _globals['_INGRESSINPUT']._serialized_start=2542
+  _globals['_INGRESSINPUT']._serialized_end=2603
+  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_start=2605
+  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_end=2678
+  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_start=2681
+  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_end=3069
   _globals['_CREATEINGRESSREQUEST']._serialized_start=57
-  _globals['_CREATEINGRESSREQUEST']._serialized_end=342
-  _globals['_INGRESSAUDIOOPTIONS']._serialized_start=345
-  _globals['_INGRESSAUDIOOPTIONS']._serialized_end=550
-  _globals['_INGRESSVIDEOOPTIONS']._serialized_start=553
-  _globals['_INGRESSVIDEOOPTIONS']._serialized_end=758
-  _globals['_INGRESSAUDIOENCODINGOPTIONS']._serialized_start=760
-  _globals['_INGRESSAUDIOENCODINGOPTIONS']._serialized_end=887
-  _globals['_INGRESSVIDEOENCODINGOPTIONS']._serialized_start=890
-  _globals['_INGRESSVIDEOENCODINGOPTIONS']._serialized_end=1018
-  _globals['_INGRESSINFO']._serialized_start=1021
-  _globals['_INGRESSINFO']._serialized_end=1393
-  _globals['_INGRESSSTATE']._serialized_start=1396
-  _globals['_INGRESSSTATE']._serialized_end=1790
-  _globals['_INGRESSSTATE_STATUS']._serialized_start=1667
-  _globals['_INGRESSSTATE_STATUS']._serialized_end=1790
-  _globals['_INPUTVIDEOSTATE']._serialized_start=1792
-  _globals['_INPUTVIDEOSTATE']._serialized_end=1903
-  _globals['_INPUTAUDIOSTATE']._serialized_start=1905
-  _globals['_INPUTAUDIOSTATE']._serialized_end=2005
-  _globals['_UPDATEINGRESSREQUEST']._serialized_start=2008
-  _globals['_UPDATEINGRESSREQUEST']._serialized_end=2285
-  _globals['_LISTINGRESSREQUEST']._serialized_start=2287
-  _globals['_LISTINGRESSREQUEST']._serialized_end=2346
-  _globals['_LISTINGRESSRESPONSE']._serialized_start=2348
-  _globals['_LISTINGRESSRESPONSE']._serialized_end=2406
-  _globals['_DELETEINGRESSREQUEST']._serialized_start=2408
-  _globals['_DELETEINGRESSREQUEST']._serialized_end=2450
-  _globals['_INGRESS']._serialized_start=2982
-  _globals['_INGRESS']._serialized_end=3275
+  _globals['_CREATEINGRESSREQUEST']._serialized_end=372
+  _globals['_INGRESSAUDIOOPTIONS']._serialized_start=375
+  _globals['_INGRESSAUDIOOPTIONS']._serialized_end=580
+  _globals['_INGRESSVIDEOOPTIONS']._serialized_start=583
+  _globals['_INGRESSVIDEOOPTIONS']._serialized_end=788
+  _globals['_INGRESSAUDIOENCODINGOPTIONS']._serialized_start=790
+  _globals['_INGRESSAUDIOENCODINGOPTIONS']._serialized_end=917
+  _globals['_INGRESSVIDEOENCODINGOPTIONS']._serialized_start=920
+  _globals['_INGRESSVIDEOENCODINGOPTIONS']._serialized_end=1048
+  _globals['_INGRESSINFO']._serialized_start=1051
+  _globals['_INGRESSINFO']._serialized_end=1453
+  _globals['_INGRESSSTATE']._serialized_start=1456
+  _globals['_INGRESSSTATE']._serialized_end=1850
+  _globals['_INGRESSSTATE_STATUS']._serialized_start=1727
+  _globals['_INGRESSSTATE_STATUS']._serialized_end=1850
+  _globals['_INPUTVIDEOSTATE']._serialized_start=1852
+  _globals['_INPUTVIDEOSTATE']._serialized_end=1963
+  _globals['_INPUTAUDIOSTATE']._serialized_start=1965
+  _globals['_INPUTAUDIOSTATE']._serialized_end=2065
+  _globals['_UPDATEINGRESSREQUEST']._serialized_start=2068
+  _globals['_UPDATEINGRESSREQUEST']._serialized_end=2375
+  _globals['_LISTINGRESSREQUEST']._serialized_start=2377
+  _globals['_LISTINGRESSREQUEST']._serialized_end=2436
+  _globals['_LISTINGRESSRESPONSE']._serialized_start=2438
+  _globals['_LISTINGRESSRESPONSE']._serialized_end=2496
+  _globals['_DELETEINGRESSREQUEST']._serialized_start=2498
+  _globals['_DELETEINGRESSREQUEST']._serialized_end=2540
+  _globals['_INGRESS']._serialized_start=3072
+  _globals['_INGRESS']._serialized_end=3365
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/ingress.pyi` & `livekit-protocol-0.4.0/livekit/protocol/ingress.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -43,34 +43,36 @@
 H264_720P_30FPS_3_LAYERS_HIGH_MOTION: IngressVideoEncodingPreset
 H264_1080P_30FPS_3_LAYERS_HIGH_MOTION: IngressVideoEncodingPreset
 H264_540P_25FPS_2_LAYERS_HIGH_MOTION: IngressVideoEncodingPreset
 H264_720P_30FPS_1_LAYER_HIGH_MOTION: IngressVideoEncodingPreset
 H264_1080P_30FPS_1_LAYER_HIGH_MOTION: IngressVideoEncodingPreset
 
 class CreateIngressRequest(_message.Message):
-    __slots__ = ("input_type", "url", "name", "room_name", "participant_identity", "participant_name", "bypass_transcoding", "audio", "video")
+    __slots__ = ("input_type", "url", "name", "room_name", "participant_identity", "participant_name", "participant_metadata", "bypass_transcoding", "audio", "video")
     INPUT_TYPE_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_NAME_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_METADATA_FIELD_NUMBER: _ClassVar[int]
     BYPASS_TRANSCODING_FIELD_NUMBER: _ClassVar[int]
     AUDIO_FIELD_NUMBER: _ClassVar[int]
     VIDEO_FIELD_NUMBER: _ClassVar[int]
     input_type: IngressInput
     url: str
     name: str
     room_name: str
     participant_identity: str
     participant_name: str
+    participant_metadata: str
     bypass_transcoding: bool
     audio: IngressAudioOptions
     video: IngressVideoOptions
-    def __init__(self, input_type: _Optional[_Union[IngressInput, str]] = ..., url: _Optional[str] = ..., name: _Optional[str] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ...) -> None: ...
+    def __init__(self, input_type: _Optional[_Union[IngressInput, str]] = ..., url: _Optional[str] = ..., name: _Optional[str] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., participant_metadata: _Optional[str] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ...) -> None: ...
 
 class IngressAudioOptions(_message.Message):
     __slots__ = ("name", "source", "preset", "options")
     NAME_FIELD_NUMBER: _ClassVar[int]
     SOURCE_FIELD_NUMBER: _ClassVar[int]
     PRESET_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
@@ -111,42 +113,44 @@
     LAYERS_FIELD_NUMBER: _ClassVar[int]
     video_codec: _models.VideoCodec
     frame_rate: float
     layers: _containers.RepeatedCompositeFieldContainer[_models.VideoLayer]
     def __init__(self, video_codec: _Optional[_Union[_models.VideoCodec, str]] = ..., frame_rate: _Optional[float] = ..., layers: _Optional[_Iterable[_Union[_models.VideoLayer, _Mapping]]] = ...) -> None: ...
 
 class IngressInfo(_message.Message):
-    __slots__ = ("ingress_id", "name", "stream_key", "url", "input_type", "bypass_transcoding", "audio", "video", "room_name", "participant_identity", "participant_name", "reusable", "state")
+    __slots__ = ("ingress_id", "name", "stream_key", "url", "input_type", "bypass_transcoding", "audio", "video", "room_name", "participant_identity", "participant_name", "participant_metadata", "reusable", "state")
     INGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     STREAM_KEY_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     INPUT_TYPE_FIELD_NUMBER: _ClassVar[int]
     BYPASS_TRANSCODING_FIELD_NUMBER: _ClassVar[int]
     AUDIO_FIELD_NUMBER: _ClassVar[int]
     VIDEO_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_NAME_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_METADATA_FIELD_NUMBER: _ClassVar[int]
     REUSABLE_FIELD_NUMBER: _ClassVar[int]
     STATE_FIELD_NUMBER: _ClassVar[int]
     ingress_id: str
     name: str
     stream_key: str
     url: str
     input_type: IngressInput
     bypass_transcoding: bool
     audio: IngressAudioOptions
     video: IngressVideoOptions
     room_name: str
     participant_identity: str
     participant_name: str
+    participant_metadata: str
     reusable: bool
     state: IngressState
-    def __init__(self, ingress_id: _Optional[str] = ..., name: _Optional[str] = ..., stream_key: _Optional[str] = ..., url: _Optional[str] = ..., input_type: _Optional[_Union[IngressInput, str]] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., reusable: bool = ..., state: _Optional[_Union[IngressState, _Mapping]] = ...) -> None: ...
+    def __init__(self, ingress_id: _Optional[str] = ..., name: _Optional[str] = ..., stream_key: _Optional[str] = ..., url: _Optional[str] = ..., input_type: _Optional[_Union[IngressInput, str]] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., participant_metadata: _Optional[str] = ..., reusable: bool = ..., state: _Optional[_Union[IngressState, _Mapping]] = ...) -> None: ...
 
 class IngressState(_message.Message):
     __slots__ = ("status", "error", "video", "audio", "room_id", "started_at", "ended_at", "resource_id", "tracks")
     class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         ENDPOINT_INACTIVE: _ClassVar[IngressState.Status]
         ENDPOINT_BUFFERING: _ClassVar[IngressState.Status]
@@ -201,32 +205,34 @@
     mime_type: str
     average_bitrate: int
     channels: int
     sample_rate: int
     def __init__(self, mime_type: _Optional[str] = ..., average_bitrate: _Optional[int] = ..., channels: _Optional[int] = ..., sample_rate: _Optional[int] = ...) -> None: ...
 
 class UpdateIngressRequest(_message.Message):
-    __slots__ = ("ingress_id", "name", "room_name", "participant_identity", "participant_name", "bypass_transcoding", "audio", "video")
+    __slots__ = ("ingress_id", "name", "room_name", "participant_identity", "participant_name", "participant_metadata", "bypass_transcoding", "audio", "video")
     INGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_NAME_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_METADATA_FIELD_NUMBER: _ClassVar[int]
     BYPASS_TRANSCODING_FIELD_NUMBER: _ClassVar[int]
     AUDIO_FIELD_NUMBER: _ClassVar[int]
     VIDEO_FIELD_NUMBER: _ClassVar[int]
     ingress_id: str
     name: str
     room_name: str
     participant_identity: str
     participant_name: str
+    participant_metadata: str
     bypass_transcoding: bool
     audio: IngressAudioOptions
     video: IngressVideoOptions
-    def __init__(self, ingress_id: _Optional[str] = ..., name: _Optional[str] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ...) -> None: ...
+    def __init__(self, ingress_id: _Optional[str] = ..., name: _Optional[str] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., participant_metadata: _Optional[str] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ...) -> None: ...
 
 class ListIngressRequest(_message.Message):
     __slots__ = ("room_name", "ingress_id")
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     INGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     room_name: str
     ingress_id: str
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/models.py` & `livekit-protocol-0.4.0/livekit/protocol/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,98 +11,114 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14livekit_models.proto\x12\x07livekit\x1a\x1fgoogle/protobuf/timestamp.proto\"\xae\x02\n\x04Room\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rempty_timeout\x18\x03 \x01(\r\x12\x18\n\x10max_participants\x18\x04 \x01(\r\x12\x15\n\rcreation_time\x18\x05 \x01(\x03\x12\x15\n\rturn_password\x18\x06 \x01(\t\x12&\n\x0e\x65nabled_codecs\x18\x07 \x03(\x0b\x32\x0e.livekit.Codec\x12\x10\n\x08metadata\x18\x08 \x01(\t\x12\x18\n\x10num_participants\x18\t \x01(\r\x12\x16\n\x0enum_publishers\x18\x0b \x01(\r\x12\x18\n\x10\x61\x63tive_recording\x18\n \x01(\x08\x12&\n\x07version\x18\r \x01(\x0b\x32\x15.livekit.TimedVersion\"(\n\x05\x43odec\x12\x0c\n\x04mime\x18\x01 \x01(\t\x12\x11\n\tfmtp_line\x18\x02 \x01(\t\"9\n\x0cPlayoutDelay\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\r\x12\x0b\n\x03max\x18\x03 \x01(\r\"\xde\x01\n\x15ParticipantPermission\x12\x15\n\rcan_subscribe\x18\x01 \x01(\x08\x12\x13\n\x0b\x63\x61n_publish\x18\x02 \x01(\x08\x12\x18\n\x10\x63\x61n_publish_data\x18\x03 \x01(\x08\x12\x31\n\x13\x63\x61n_publish_sources\x18\t \x03(\x0e\x32\x14.livekit.TrackSource\x12\x0e\n\x06hidden\x18\x07 \x01(\x08\x12\x10\n\x08recorder\x18\x08 \x01(\x08\x12\x1b\n\x13\x63\x61n_update_metadata\x18\n \x01(\x08\x12\r\n\x05\x61gent\x18\x0b \x01(\x08\"\xd1\x03\n\x0fParticipantInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12-\n\x05state\x18\x03 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12\"\n\x06tracks\x18\x04 \x03(\x0b\x32\x12.livekit.TrackInfo\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12\x11\n\tjoined_at\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\t \x01(\t\x12\x0f\n\x07version\x18\n \x01(\r\x12\x32\n\npermission\x18\x0b \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\x14\n\x0cis_publisher\x18\r \x01(\x08\x12+\n\x04kind\x18\x0e \x01(\x0e\x32\x1d.livekit.ParticipantInfo.Kind\">\n\x05State\x12\x0b\n\x07JOINING\x10\x00\x12\n\n\x06JOINED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x10\n\x0c\x44ISCONNECTED\x10\x03\"A\n\x04Kind\x12\x0c\n\x08STANDARD\x10\x00\x12\x0b\n\x07INGRESS\x10\x01\x12\n\n\x06\x45GRESS\x10\x02\x12\x07\n\x03SIP\x10\x03\x12\t\n\x05\x41GENT\x10\x04\"3\n\nEncryption\"%\n\x04Type\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GCM\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\"f\n\x12SimulcastCodecInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\t\x12\x0b\n\x03\x63id\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer\"\xc1\x03\n\tTrackInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.livekit.TrackType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x11\n\tsimulcast\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x08 \x01(\x08\x12$\n\x06source\x18\t \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\n \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x11\n\tmime_type\x18\x0b \x01(\t\x12\x0b\n\x03mid\x18\x0c \x01(\t\x12+\n\x06\x63odecs\x18\r \x03(\x0b\x32\x1b.livekit.SimulcastCodecInfo\x12\x0e\n\x06stereo\x18\x0e \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\x0f \x01(\x08\x12,\n\nencryption\x18\x10 \x01(\x0e\x32\x18.livekit.Encryption.Type\x12\x0e\n\x06stream\x18\x11 \x01(\t\x12&\n\x07version\x18\x12 \x01(\x0b\x32\x15.livekit.TimedVersion\"r\n\nVideoLayer\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x0c\n\x04ssrc\x18\x05 \x01(\r\"\xb4\x01\n\nDataPacket\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12#\n\x04user\x18\x02 \x01(\x0b\x32\x13.livekit.UserPacketH\x00\x12/\n\x07speaker\x18\x03 \x01(\x0b\x32\x1c.livekit.ActiveSpeakerUpdateH\x00\"\x1f\n\x04Kind\x12\x0c\n\x08RELIABLE\x10\x00\x12\t\n\x05LOSSY\x10\x01\x42\x07\n\x05value\"=\n\x13\x41\x63tiveSpeakerUpdate\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo\"9\n\x0bSpeakerInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\"\xac\x01\n\nUserPacket\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x1c\n\x14participant_identity\x18\x05 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x18\n\x10\x64\x65stination_sids\x18\x03 \x03(\t\x12\x1e\n\x16\x64\x65stination_identities\x18\x06 \x03(\t\x12\x12\n\x05topic\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic\"@\n\x11ParticipantTracks\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\ntrack_sids\x18\x02 \x03(\t\"\xb6\x01\n\nServerInfo\x12,\n\x07\x65\x64ition\x18\x01 \x01(\x0e\x32\x1b.livekit.ServerInfo.Edition\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\x0e\n\x06region\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x12\n\ndebug_info\x18\x06 \x01(\t\"\"\n\x07\x45\x64ition\x12\x0c\n\x08Standard\x10\x00\x12\t\n\x05\x43loud\x10\x01\"\xdd\x02\n\nClientInfo\x12$\n\x03sdk\x18\x01 \x01(\x0e\x32\x17.livekit.ClientInfo.SDK\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\n\n\x02os\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\x06 \x01(\t\x12\x0f\n\x07\x62rowser\x18\x07 \x01(\t\x12\x17\n\x0f\x62rowser_version\x18\x08 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\t \x01(\t\x12\x0f\n\x07network\x18\n \x01(\t\"\x83\x01\n\x03SDK\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02JS\x10\x01\x12\t\n\x05SWIFT\x10\x02\x12\x0b\n\x07\x41NDROID\x10\x03\x12\x0b\n\x07\x46LUTTER\x10\x04\x12\x06\n\x02GO\x10\x05\x12\t\n\x05UNITY\x10\x06\x12\x10\n\x0cREACT_NATIVE\x10\x07\x12\x08\n\x04RUST\x10\x08\x12\n\n\x06PYTHON\x10\t\x12\x07\n\x03\x43PP\x10\n\"\x8c\x02\n\x13\x43lientConfiguration\x12*\n\x05video\x18\x01 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12+\n\x06screen\x18\x02 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12\x37\n\x11resume_connection\x18\x03 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\x12\x30\n\x0f\x64isabled_codecs\x18\x04 \x01(\x0b\x32\x17.livekit.DisabledCodecs\x12\x31\n\x0b\x66orce_relay\x18\x05 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"L\n\x12VideoConfiguration\x12\x36\n\x10hardware_encoder\x18\x01 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"Q\n\x0e\x44isabledCodecs\x12\x1e\n\x06\x63odecs\x18\x01 \x03(\x0b\x32\x0e.livekit.Codec\x12\x1f\n\x07publish\x18\x02 \x03(\x0b\x32\x0e.livekit.Codec\"\x80\x02\n\x08RTPDrift\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x17\n\x0fstart_timestamp\x18\x04 \x01(\x04\x12\x15\n\rend_timestamp\x18\x05 \x01(\x04\x12\x17\n\x0frtp_clock_ticks\x18\x06 \x01(\x04\x12\x15\n\rdrift_samples\x18\x07 \x01(\x03\x12\x10\n\x08\x64rift_ms\x18\x08 \x01(\x01\x12\x12\n\nclock_rate\x18\t \x01(\x01\"\xef\t\n\x08RTPStats\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x0f\n\x07packets\x18\x04 \x01(\r\x12\x13\n\x0bpacket_rate\x18\x05 \x01(\x01\x12\r\n\x05\x62ytes\x18\x06 \x01(\x04\x12\x14\n\x0cheader_bytes\x18\' \x01(\x04\x12\x0f\n\x07\x62itrate\x18\x07 \x01(\x01\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x18\n\x10packet_loss_rate\x18\t \x01(\x01\x12\x1e\n\x16packet_loss_percentage\x18\n \x01(\x02\x12\x19\n\x11packets_duplicate\x18\x0b \x01(\r\x12\x1d\n\x15packet_duplicate_rate\x18\x0c \x01(\x01\x12\x17\n\x0f\x62ytes_duplicate\x18\r \x01(\x04\x12\x1e\n\x16header_bytes_duplicate\x18( \x01(\x04\x12\x19\n\x11\x62itrate_duplicate\x18\x0e \x01(\x01\x12\x17\n\x0fpackets_padding\x18\x0f \x01(\r\x12\x1b\n\x13packet_padding_rate\x18\x10 \x01(\x01\x12\x15\n\rbytes_padding\x18\x11 \x01(\x04\x12\x1c\n\x14header_bytes_padding\x18) \x01(\x04\x12\x17\n\x0f\x62itrate_padding\x18\x12 \x01(\x01\x12\x1c\n\x14packets_out_of_order\x18\x13 \x01(\r\x12\x0e\n\x06\x66rames\x18\x14 \x01(\r\x12\x12\n\nframe_rate\x18\x15 \x01(\x01\x12\x16\n\x0ejitter_current\x18\x16 \x01(\x01\x12\x12\n\njitter_max\x18\x17 \x01(\x01\x12:\n\rgap_histogram\x18\x18 \x03(\x0b\x32#.livekit.RTPStats.GapHistogramEntry\x12\r\n\x05nacks\x18\x19 \x01(\r\x12\x11\n\tnack_acks\x18% \x01(\r\x12\x13\n\x0bnack_misses\x18\x1a \x01(\r\x12\x15\n\rnack_repeated\x18& \x01(\r\x12\x0c\n\x04plis\x18\x1b \x01(\r\x12,\n\x08last_pli\x18\x1c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x66irs\x18\x1d \x01(\r\x12,\n\x08last_fir\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brtt_current\x18\x1f \x01(\r\x12\x0f\n\x07rtt_max\x18  \x01(\r\x12\x12\n\nkey_frames\x18! \x01(\r\x12\x32\n\x0elast_key_frame\x18\" \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flayer_lock_plis\x18# \x01(\r\x12\x37\n\x13last_layer_lock_pli\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x0cpacket_drift\x18, \x01(\x0b\x32\x11.livekit.RTPDrift\x12\'\n\x0creport_drift\x18- \x01(\x0b\x32\x11.livekit.RTPDrift\x1a\x33\n\x11GapHistogramEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"1\n\x0cTimedVersion\x12\x12\n\nunix_micro\x18\x01 \x01(\x03\x12\r\n\x05ticks\x18\x02 \x01(\x05*/\n\nAudioCodec\x12\x0e\n\nDEFAULT_AC\x10\x00\x12\x08\n\x04OPUS\x10\x01\x12\x07\n\x03\x41\x41\x43\x10\x02*V\n\nVideoCodec\x12\x0e\n\nDEFAULT_VC\x10\x00\x12\x11\n\rH264_BASELINE\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH264_HIGH\x10\x03\x12\x07\n\x03VP8\x10\x04*)\n\nImageCodec\x12\x0e\n\nIC_DEFAULT\x10\x00\x12\x0b\n\x07IC_JPEG\x10\x01*+\n\tTrackType\x12\t\n\x05\x41UDIO\x10\x00\x12\t\n\x05VIDEO\x10\x01\x12\x08\n\x04\x44\x41TA\x10\x02*`\n\x0bTrackSource\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43\x41MERA\x10\x01\x12\x0e\n\nMICROPHONE\x10\x02\x12\x10\n\x0cSCREEN_SHARE\x10\x03\x12\x16\n\x12SCREEN_SHARE_AUDIO\x10\x04*6\n\x0cVideoQuality\x12\x07\n\x03LOW\x10\x00\x12\n\n\x06MEDIUM\x10\x01\x12\x08\n\x04HIGH\x10\x02\x12\x07\n\x03OFF\x10\x03*@\n\x11\x43onnectionQuality\x12\x08\n\x04POOR\x10\x00\x12\x08\n\x04GOOD\x10\x01\x12\r\n\tEXCELLENT\x10\x02\x12\x08\n\x04LOST\x10\x03*;\n\x13\x43lientConfigSetting\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02*\xba\x01\n\x10\x44isconnectReason\x12\x12\n\x0eUNKNOWN_REASON\x10\x00\x12\x14\n\x10\x43LIENT_INITIATED\x10\x01\x12\x16\n\x12\x44UPLICATE_IDENTITY\x10\x02\x12\x13\n\x0fSERVER_SHUTDOWN\x10\x03\x12\x17\n\x13PARTICIPANT_REMOVED\x10\x04\x12\x10\n\x0cROOM_DELETED\x10\x05\x12\x12\n\x0eSTATE_MISMATCH\x10\x06\x12\x10\n\x0cJOIN_FAILURE\x10\x07*\x89\x01\n\x0fReconnectReason\x12\x0e\n\nRR_UNKNOWN\x10\x00\x12\x1a\n\x16RR_SIGNAL_DISCONNECTED\x10\x01\x12\x17\n\x13RR_PUBLISHER_FAILED\x10\x02\x12\x18\n\x14RR_SUBSCRIBER_FAILED\x10\x03\x12\x17\n\x13RR_SWITCH_CANDIDATE\x10\x04*T\n\x11SubscriptionError\x12\x0e\n\nSE_UNKNOWN\x10\x00\x12\x18\n\x14SE_CODEC_UNSUPPORTED\x10\x01\x12\x15\n\x11SE_TRACK_NOTFOUND\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14livekit_models.proto\x12\x07livekit\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc9\x02\n\x04Room\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rempty_timeout\x18\x03 \x01(\r\x12\x19\n\x11\x64\x65parture_timeout\x18\x0e \x01(\r\x12\x18\n\x10max_participants\x18\x04 \x01(\r\x12\x15\n\rcreation_time\x18\x05 \x01(\x03\x12\x15\n\rturn_password\x18\x06 \x01(\t\x12&\n\x0e\x65nabled_codecs\x18\x07 \x03(\x0b\x32\x0e.livekit.Codec\x12\x10\n\x08metadata\x18\x08 \x01(\t\x12\x18\n\x10num_participants\x18\t \x01(\r\x12\x16\n\x0enum_publishers\x18\x0b \x01(\r\x12\x18\n\x10\x61\x63tive_recording\x18\n \x01(\x08\x12&\n\x07version\x18\r \x01(\x0b\x32\x15.livekit.TimedVersion\"(\n\x05\x43odec\x12\x0c\n\x04mime\x18\x01 \x01(\t\x12\x11\n\tfmtp_line\x18\x02 \x01(\t\"9\n\x0cPlayoutDelay\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\r\x12\x0b\n\x03max\x18\x03 \x01(\r\"\xde\x01\n\x15ParticipantPermission\x12\x15\n\rcan_subscribe\x18\x01 \x01(\x08\x12\x13\n\x0b\x63\x61n_publish\x18\x02 \x01(\x08\x12\x18\n\x10\x63\x61n_publish_data\x18\x03 \x01(\x08\x12\x31\n\x13\x63\x61n_publish_sources\x18\t \x03(\x0e\x32\x14.livekit.TrackSource\x12\x0e\n\x06hidden\x18\x07 \x01(\x08\x12\x10\n\x08recorder\x18\x08 \x01(\x08\x12\x1b\n\x13\x63\x61n_update_metadata\x18\n \x01(\x08\x12\r\n\x05\x61gent\x18\x0b \x01(\x08\"\xd1\x03\n\x0fParticipantInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12-\n\x05state\x18\x03 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12\"\n\x06tracks\x18\x04 \x03(\x0b\x32\x12.livekit.TrackInfo\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12\x11\n\tjoined_at\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\t \x01(\t\x12\x0f\n\x07version\x18\n \x01(\r\x12\x32\n\npermission\x18\x0b \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\x14\n\x0cis_publisher\x18\r \x01(\x08\x12+\n\x04kind\x18\x0e \x01(\x0e\x32\x1d.livekit.ParticipantInfo.Kind\">\n\x05State\x12\x0b\n\x07JOINING\x10\x00\x12\n\n\x06JOINED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x10\n\x0c\x44ISCONNECTED\x10\x03\"A\n\x04Kind\x12\x0c\n\x08STANDARD\x10\x00\x12\x0b\n\x07INGRESS\x10\x01\x12\n\n\x06\x45GRESS\x10\x02\x12\x07\n\x03SIP\x10\x03\x12\t\n\x05\x41GENT\x10\x04\"3\n\nEncryption\"%\n\x04Type\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GCM\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\"f\n\x12SimulcastCodecInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\t\x12\x0b\n\x03\x63id\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer\"\xc1\x03\n\tTrackInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.livekit.TrackType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x11\n\tsimulcast\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x08 \x01(\x08\x12$\n\x06source\x18\t \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\n \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x11\n\tmime_type\x18\x0b \x01(\t\x12\x0b\n\x03mid\x18\x0c \x01(\t\x12+\n\x06\x63odecs\x18\r \x03(\x0b\x32\x1b.livekit.SimulcastCodecInfo\x12\x0e\n\x06stereo\x18\x0e \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\x0f \x01(\x08\x12,\n\nencryption\x18\x10 \x01(\x0e\x32\x18.livekit.Encryption.Type\x12\x0e\n\x06stream\x18\x11 \x01(\t\x12&\n\x07version\x18\x12 \x01(\x0b\x32\x15.livekit.TimedVersion\"r\n\nVideoLayer\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x0c\n\x04ssrc\x18\x05 \x01(\r\"\xa0\x02\n\nDataPacket\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x18.livekit.DataPacket.KindB\x02\x18\x01\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x1e\n\x16\x64\x65stination_identities\x18\x05 \x03(\t\x12#\n\x04user\x18\x02 \x01(\x0b\x32\x13.livekit.UserPacketH\x00\x12\x33\n\x07speaker\x18\x03 \x01(\x0b\x32\x1c.livekit.ActiveSpeakerUpdateB\x02\x18\x01H\x00\x12$\n\x08sip_dtmf\x18\x06 \x01(\x0b\x32\x10.livekit.SipDTMFH\x00\"\x1f\n\x04Kind\x12\x0c\n\x08RELIABLE\x10\x00\x12\t\n\x05LOSSY\x10\x01\x42\x07\n\x05value\"=\n\x13\x41\x63tiveSpeakerUpdate\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo\"9\n\x0bSpeakerInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\"\xbc\x01\n\nUserPacket\x12\x1b\n\x0fparticipant_sid\x18\x01 \x01(\tB\x02\x18\x01\x12 \n\x14participant_identity\x18\x05 \x01(\tB\x02\x18\x01\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x1c\n\x10\x64\x65stination_sids\x18\x03 \x03(\tB\x02\x18\x01\x12\"\n\x16\x64\x65stination_identities\x18\x06 \x03(\tB\x02\x18\x01\x12\x12\n\x05topic\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic\"&\n\x07SipDTMF\x12\x0c\n\x04\x63ode\x18\x03 \x01(\r\x12\r\n\x05\x64igit\x18\x04 \x01(\t\"@\n\x11ParticipantTracks\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\ntrack_sids\x18\x02 \x03(\t\"\xce\x01\n\nServerInfo\x12,\n\x07\x65\x64ition\x18\x01 \x01(\x0e\x32\x1b.livekit.ServerInfo.Edition\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\x0e\n\x06region\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x12\n\ndebug_info\x18\x06 \x01(\t\x12\x16\n\x0e\x61gent_protocol\x18\x07 \x01(\x05\"\"\n\x07\x45\x64ition\x12\x0c\n\x08Standard\x10\x00\x12\t\n\x05\x43loud\x10\x01\"\xdd\x02\n\nClientInfo\x12$\n\x03sdk\x18\x01 \x01(\x0e\x32\x17.livekit.ClientInfo.SDK\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\n\n\x02os\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\x06 \x01(\t\x12\x0f\n\x07\x62rowser\x18\x07 \x01(\t\x12\x17\n\x0f\x62rowser_version\x18\x08 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\t \x01(\t\x12\x0f\n\x07network\x18\n \x01(\t\"\x83\x01\n\x03SDK\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02JS\x10\x01\x12\t\n\x05SWIFT\x10\x02\x12\x0b\n\x07\x41NDROID\x10\x03\x12\x0b\n\x07\x46LUTTER\x10\x04\x12\x06\n\x02GO\x10\x05\x12\t\n\x05UNITY\x10\x06\x12\x10\n\x0cREACT_NATIVE\x10\x07\x12\x08\n\x04RUST\x10\x08\x12\n\n\x06PYTHON\x10\t\x12\x07\n\x03\x43PP\x10\n\"\x8c\x02\n\x13\x43lientConfiguration\x12*\n\x05video\x18\x01 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12+\n\x06screen\x18\x02 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12\x37\n\x11resume_connection\x18\x03 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\x12\x30\n\x0f\x64isabled_codecs\x18\x04 \x01(\x0b\x32\x17.livekit.DisabledCodecs\x12\x31\n\x0b\x66orce_relay\x18\x05 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"L\n\x12VideoConfiguration\x12\x36\n\x10hardware_encoder\x18\x01 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"Q\n\x0e\x44isabledCodecs\x12\x1e\n\x06\x63odecs\x18\x01 \x03(\x0b\x32\x0e.livekit.Codec\x12\x1f\n\x07publish\x18\x02 \x03(\x0b\x32\x0e.livekit.Codec\"\x80\x02\n\x08RTPDrift\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x17\n\x0fstart_timestamp\x18\x04 \x01(\x04\x12\x15\n\rend_timestamp\x18\x05 \x01(\x04\x12\x17\n\x0frtp_clock_ticks\x18\x06 \x01(\x04\x12\x15\n\rdrift_samples\x18\x07 \x01(\x03\x12\x10\n\x08\x64rift_ms\x18\x08 \x01(\x01\x12\x12\n\nclock_rate\x18\t \x01(\x01\"\xa0\n\n\x08RTPStats\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x0f\n\x07packets\x18\x04 \x01(\r\x12\x13\n\x0bpacket_rate\x18\x05 \x01(\x01\x12\r\n\x05\x62ytes\x18\x06 \x01(\x04\x12\x14\n\x0cheader_bytes\x18\' \x01(\x04\x12\x0f\n\x07\x62itrate\x18\x07 \x01(\x01\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x18\n\x10packet_loss_rate\x18\t \x01(\x01\x12\x1e\n\x16packet_loss_percentage\x18\n \x01(\x02\x12\x19\n\x11packets_duplicate\x18\x0b \x01(\r\x12\x1d\n\x15packet_duplicate_rate\x18\x0c \x01(\x01\x12\x17\n\x0f\x62ytes_duplicate\x18\r \x01(\x04\x12\x1e\n\x16header_bytes_duplicate\x18( \x01(\x04\x12\x19\n\x11\x62itrate_duplicate\x18\x0e \x01(\x01\x12\x17\n\x0fpackets_padding\x18\x0f \x01(\r\x12\x1b\n\x13packet_padding_rate\x18\x10 \x01(\x01\x12\x15\n\rbytes_padding\x18\x11 \x01(\x04\x12\x1c\n\x14header_bytes_padding\x18) \x01(\x04\x12\x17\n\x0f\x62itrate_padding\x18\x12 \x01(\x01\x12\x1c\n\x14packets_out_of_order\x18\x13 \x01(\r\x12\x0e\n\x06\x66rames\x18\x14 \x01(\r\x12\x12\n\nframe_rate\x18\x15 \x01(\x01\x12\x16\n\x0ejitter_current\x18\x16 \x01(\x01\x12\x12\n\njitter_max\x18\x17 \x01(\x01\x12:\n\rgap_histogram\x18\x18 \x03(\x0b\x32#.livekit.RTPStats.GapHistogramEntry\x12\r\n\x05nacks\x18\x19 \x01(\r\x12\x11\n\tnack_acks\x18% \x01(\r\x12\x13\n\x0bnack_misses\x18\x1a \x01(\r\x12\x15\n\rnack_repeated\x18& \x01(\r\x12\x0c\n\x04plis\x18\x1b \x01(\r\x12,\n\x08last_pli\x18\x1c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x66irs\x18\x1d \x01(\r\x12,\n\x08last_fir\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brtt_current\x18\x1f \x01(\r\x12\x0f\n\x07rtt_max\x18  \x01(\r\x12\x12\n\nkey_frames\x18! \x01(\r\x12\x32\n\x0elast_key_frame\x18\" \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flayer_lock_plis\x18# \x01(\r\x12\x37\n\x13last_layer_lock_pli\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x0cpacket_drift\x18, \x01(\x0b\x32\x11.livekit.RTPDrift\x12\'\n\x0creport_drift\x18- \x01(\x0b\x32\x11.livekit.RTPDrift\x12/\n\x14rebased_report_drift\x18. \x01(\x0b\x32\x11.livekit.RTPDrift\x1a\x33\n\x11GapHistogramEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"1\n\x0cTimedVersion\x12\x12\n\nunix_micro\x18\x01 \x01(\x03\x12\r\n\x05ticks\x18\x02 \x01(\x05*/\n\nAudioCodec\x12\x0e\n\nDEFAULT_AC\x10\x00\x12\x08\n\x04OPUS\x10\x01\x12\x07\n\x03\x41\x41\x43\x10\x02*V\n\nVideoCodec\x12\x0e\n\nDEFAULT_VC\x10\x00\x12\x11\n\rH264_BASELINE\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH264_HIGH\x10\x03\x12\x07\n\x03VP8\x10\x04*)\n\nImageCodec\x12\x0e\n\nIC_DEFAULT\x10\x00\x12\x0b\n\x07IC_JPEG\x10\x01*+\n\tTrackType\x12\t\n\x05\x41UDIO\x10\x00\x12\t\n\x05VIDEO\x10\x01\x12\x08\n\x04\x44\x41TA\x10\x02*`\n\x0bTrackSource\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43\x41MERA\x10\x01\x12\x0e\n\nMICROPHONE\x10\x02\x12\x10\n\x0cSCREEN_SHARE\x10\x03\x12\x16\n\x12SCREEN_SHARE_AUDIO\x10\x04*6\n\x0cVideoQuality\x12\x07\n\x03LOW\x10\x00\x12\n\n\x06MEDIUM\x10\x01\x12\x08\n\x04HIGH\x10\x02\x12\x07\n\x03OFF\x10\x03*@\n\x11\x43onnectionQuality\x12\x08\n\x04POOR\x10\x00\x12\x08\n\x04GOOD\x10\x01\x12\r\n\tEXCELLENT\x10\x02\x12\x08\n\x04LOST\x10\x03*;\n\x13\x43lientConfigSetting\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02*\xdb\x01\n\x10\x44isconnectReason\x12\x12\n\x0eUNKNOWN_REASON\x10\x00\x12\x14\n\x10\x43LIENT_INITIATED\x10\x01\x12\x16\n\x12\x44UPLICATE_IDENTITY\x10\x02\x12\x13\n\x0fSERVER_SHUTDOWN\x10\x03\x12\x17\n\x13PARTICIPANT_REMOVED\x10\x04\x12\x10\n\x0cROOM_DELETED\x10\x05\x12\x12\n\x0eSTATE_MISMATCH\x10\x06\x12\x10\n\x0cJOIN_FAILURE\x10\x07\x12\r\n\tMIGRATION\x10\x08\x12\x10\n\x0cSIGNAL_CLOSE\x10\t*\x89\x01\n\x0fReconnectReason\x12\x0e\n\nRR_UNKNOWN\x10\x00\x12\x1a\n\x16RR_SIGNAL_DISCONNECTED\x10\x01\x12\x17\n\x13RR_PUBLISHER_FAILED\x10\x02\x12\x18\n\x14RR_SUBSCRIBER_FAILED\x10\x03\x12\x17\n\x13RR_SWITCH_CANDIDATE\x10\x04*T\n\x11SubscriptionError\x12\x0e\n\nSE_UNKNOWN\x10\x00\x12\x18\n\x14SE_CODEC_UNSUPPORTED\x10\x01\x12\x15\n\x11SE_TRACK_NOTFOUND\x10\x02*\xa3\x01\n\x11\x41udioTrackFeature\x12\r\n\tTF_STEREO\x10\x00\x12\r\n\tTF_NO_DTX\x10\x01\x12\x18\n\x14TF_AUTO_GAIN_CONTROL\x10\x02\x12\x18\n\x14TF_ECHO_CANCELLATION\x10\x03\x12\x18\n\x14TF_NOISE_SUPPRESSION\x10\x04\x12\"\n\x1eTF_ENHANCED_NOISE_CANCELLATION\x10\x05\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'models', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
+  _globals['_DATAPACKET'].fields_by_name['kind']._options = None
+  _globals['_DATAPACKET'].fields_by_name['kind']._serialized_options = b'\030\001'
+  _globals['_DATAPACKET'].fields_by_name['speaker']._options = None
+  _globals['_DATAPACKET'].fields_by_name['speaker']._serialized_options = b'\030\001'
+  _globals['_USERPACKET'].fields_by_name['participant_sid']._options = None
+  _globals['_USERPACKET'].fields_by_name['participant_sid']._serialized_options = b'\030\001'
+  _globals['_USERPACKET'].fields_by_name['participant_identity']._options = None
+  _globals['_USERPACKET'].fields_by_name['participant_identity']._serialized_options = b'\030\001'
+  _globals['_USERPACKET'].fields_by_name['destination_sids']._options = None
+  _globals['_USERPACKET'].fields_by_name['destination_sids']._serialized_options = b'\030\001'
+  _globals['_USERPACKET'].fields_by_name['destination_identities']._options = None
+  _globals['_USERPACKET'].fields_by_name['destination_identities']._serialized_options = b'\030\001'
   _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._options = None
   _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_options = b'8\001'
-  _globals['_AUDIOCODEC']._serialized_start=4981
-  _globals['_AUDIOCODEC']._serialized_end=5028
-  _globals['_VIDEOCODEC']._serialized_start=5030
-  _globals['_VIDEOCODEC']._serialized_end=5116
-  _globals['_IMAGECODEC']._serialized_start=5118
-  _globals['_IMAGECODEC']._serialized_end=5159
-  _globals['_TRACKTYPE']._serialized_start=5161
-  _globals['_TRACKTYPE']._serialized_end=5204
-  _globals['_TRACKSOURCE']._serialized_start=5206
-  _globals['_TRACKSOURCE']._serialized_end=5302
-  _globals['_VIDEOQUALITY']._serialized_start=5304
-  _globals['_VIDEOQUALITY']._serialized_end=5358
-  _globals['_CONNECTIONQUALITY']._serialized_start=5360
-  _globals['_CONNECTIONQUALITY']._serialized_end=5424
-  _globals['_CLIENTCONFIGSETTING']._serialized_start=5426
-  _globals['_CLIENTCONFIGSETTING']._serialized_end=5485
-  _globals['_DISCONNECTREASON']._serialized_start=5488
-  _globals['_DISCONNECTREASON']._serialized_end=5674
-  _globals['_RECONNECTREASON']._serialized_start=5677
-  _globals['_RECONNECTREASON']._serialized_end=5814
-  _globals['_SUBSCRIPTIONERROR']._serialized_start=5816
-  _globals['_SUBSCRIPTIONERROR']._serialized_end=5900
+  _globals['_AUDIOCODEC']._serialized_start=5245
+  _globals['_AUDIOCODEC']._serialized_end=5292
+  _globals['_VIDEOCODEC']._serialized_start=5294
+  _globals['_VIDEOCODEC']._serialized_end=5380
+  _globals['_IMAGECODEC']._serialized_start=5382
+  _globals['_IMAGECODEC']._serialized_end=5423
+  _globals['_TRACKTYPE']._serialized_start=5425
+  _globals['_TRACKTYPE']._serialized_end=5468
+  _globals['_TRACKSOURCE']._serialized_start=5470
+  _globals['_TRACKSOURCE']._serialized_end=5566
+  _globals['_VIDEOQUALITY']._serialized_start=5568
+  _globals['_VIDEOQUALITY']._serialized_end=5622
+  _globals['_CONNECTIONQUALITY']._serialized_start=5624
+  _globals['_CONNECTIONQUALITY']._serialized_end=5688
+  _globals['_CLIENTCONFIGSETTING']._serialized_start=5690
+  _globals['_CLIENTCONFIGSETTING']._serialized_end=5749
+  _globals['_DISCONNECTREASON']._serialized_start=5752
+  _globals['_DISCONNECTREASON']._serialized_end=5971
+  _globals['_RECONNECTREASON']._serialized_start=5974
+  _globals['_RECONNECTREASON']._serialized_end=6111
+  _globals['_SUBSCRIPTIONERROR']._serialized_start=6113
+  _globals['_SUBSCRIPTIONERROR']._serialized_end=6197
+  _globals['_AUDIOTRACKFEATURE']._serialized_start=6200
+  _globals['_AUDIOTRACKFEATURE']._serialized_end=6363
   _globals['_ROOM']._serialized_start=67
-  _globals['_ROOM']._serialized_end=369
-  _globals['_CODEC']._serialized_start=371
-  _globals['_CODEC']._serialized_end=411
-  _globals['_PLAYOUTDELAY']._serialized_start=413
-  _globals['_PLAYOUTDELAY']._serialized_end=470
-  _globals['_PARTICIPANTPERMISSION']._serialized_start=473
-  _globals['_PARTICIPANTPERMISSION']._serialized_end=695
-  _globals['_PARTICIPANTINFO']._serialized_start=698
-  _globals['_PARTICIPANTINFO']._serialized_end=1163
-  _globals['_PARTICIPANTINFO_STATE']._serialized_start=1034
-  _globals['_PARTICIPANTINFO_STATE']._serialized_end=1096
-  _globals['_PARTICIPANTINFO_KIND']._serialized_start=1098
-  _globals['_PARTICIPANTINFO_KIND']._serialized_end=1163
-  _globals['_ENCRYPTION']._serialized_start=1165
-  _globals['_ENCRYPTION']._serialized_end=1216
-  _globals['_ENCRYPTION_TYPE']._serialized_start=1179
-  _globals['_ENCRYPTION_TYPE']._serialized_end=1216
-  _globals['_SIMULCASTCODECINFO']._serialized_start=1218
-  _globals['_SIMULCASTCODECINFO']._serialized_end=1320
-  _globals['_TRACKINFO']._serialized_start=1323
-  _globals['_TRACKINFO']._serialized_end=1772
-  _globals['_VIDEOLAYER']._serialized_start=1774
-  _globals['_VIDEOLAYER']._serialized_end=1888
-  _globals['_DATAPACKET']._serialized_start=1891
-  _globals['_DATAPACKET']._serialized_end=2071
-  _globals['_DATAPACKET_KIND']._serialized_start=2031
-  _globals['_DATAPACKET_KIND']._serialized_end=2062
-  _globals['_ACTIVESPEAKERUPDATE']._serialized_start=2073
-  _globals['_ACTIVESPEAKERUPDATE']._serialized_end=2134
-  _globals['_SPEAKERINFO']._serialized_start=2136
-  _globals['_SPEAKERINFO']._serialized_end=2193
-  _globals['_USERPACKET']._serialized_start=2196
-  _globals['_USERPACKET']._serialized_end=2368
-  _globals['_PARTICIPANTTRACKS']._serialized_start=2370
-  _globals['_PARTICIPANTTRACKS']._serialized_end=2434
-  _globals['_SERVERINFO']._serialized_start=2437
-  _globals['_SERVERINFO']._serialized_end=2619
-  _globals['_SERVERINFO_EDITION']._serialized_start=2585
-  _globals['_SERVERINFO_EDITION']._serialized_end=2619
-  _globals['_CLIENTINFO']._serialized_start=2622
-  _globals['_CLIENTINFO']._serialized_end=2971
-  _globals['_CLIENTINFO_SDK']._serialized_start=2840
-  _globals['_CLIENTINFO_SDK']._serialized_end=2971
-  _globals['_CLIENTCONFIGURATION']._serialized_start=2974
-  _globals['_CLIENTCONFIGURATION']._serialized_end=3242
-  _globals['_VIDEOCONFIGURATION']._serialized_start=3244
-  _globals['_VIDEOCONFIGURATION']._serialized_end=3320
-  _globals['_DISABLEDCODECS']._serialized_start=3322
-  _globals['_DISABLEDCODECS']._serialized_end=3403
-  _globals['_RTPDRIFT']._serialized_start=3406
-  _globals['_RTPDRIFT']._serialized_end=3662
-  _globals['_RTPSTATS']._serialized_start=3665
-  _globals['_RTPSTATS']._serialized_end=4928
-  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_start=4877
-  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_end=4928
-  _globals['_TIMEDVERSION']._serialized_start=4930
-  _globals['_TIMEDVERSION']._serialized_end=4979
+  _globals['_ROOM']._serialized_end=396
+  _globals['_CODEC']._serialized_start=398
+  _globals['_CODEC']._serialized_end=438
+  _globals['_PLAYOUTDELAY']._serialized_start=440
+  _globals['_PLAYOUTDELAY']._serialized_end=497
+  _globals['_PARTICIPANTPERMISSION']._serialized_start=500
+  _globals['_PARTICIPANTPERMISSION']._serialized_end=722
+  _globals['_PARTICIPANTINFO']._serialized_start=725
+  _globals['_PARTICIPANTINFO']._serialized_end=1190
+  _globals['_PARTICIPANTINFO_STATE']._serialized_start=1061
+  _globals['_PARTICIPANTINFO_STATE']._serialized_end=1123
+  _globals['_PARTICIPANTINFO_KIND']._serialized_start=1125
+  _globals['_PARTICIPANTINFO_KIND']._serialized_end=1190
+  _globals['_ENCRYPTION']._serialized_start=1192
+  _globals['_ENCRYPTION']._serialized_end=1243
+  _globals['_ENCRYPTION_TYPE']._serialized_start=1206
+  _globals['_ENCRYPTION_TYPE']._serialized_end=1243
+  _globals['_SIMULCASTCODECINFO']._serialized_start=1245
+  _globals['_SIMULCASTCODECINFO']._serialized_end=1347
+  _globals['_TRACKINFO']._serialized_start=1350
+  _globals['_TRACKINFO']._serialized_end=1799
+  _globals['_VIDEOLAYER']._serialized_start=1801
+  _globals['_VIDEOLAYER']._serialized_end=1915
+  _globals['_DATAPACKET']._serialized_start=1918
+  _globals['_DATAPACKET']._serialized_end=2206
+  _globals['_DATAPACKET_KIND']._serialized_start=2166
+  _globals['_DATAPACKET_KIND']._serialized_end=2197
+  _globals['_ACTIVESPEAKERUPDATE']._serialized_start=2208
+  _globals['_ACTIVESPEAKERUPDATE']._serialized_end=2269
+  _globals['_SPEAKERINFO']._serialized_start=2271
+  _globals['_SPEAKERINFO']._serialized_end=2328
+  _globals['_USERPACKET']._serialized_start=2331
+  _globals['_USERPACKET']._serialized_end=2519
+  _globals['_SIPDTMF']._serialized_start=2521
+  _globals['_SIPDTMF']._serialized_end=2559
+  _globals['_PARTICIPANTTRACKS']._serialized_start=2561
+  _globals['_PARTICIPANTTRACKS']._serialized_end=2625
+  _globals['_SERVERINFO']._serialized_start=2628
+  _globals['_SERVERINFO']._serialized_end=2834
+  _globals['_SERVERINFO_EDITION']._serialized_start=2800
+  _globals['_SERVERINFO_EDITION']._serialized_end=2834
+  _globals['_CLIENTINFO']._serialized_start=2837
+  _globals['_CLIENTINFO']._serialized_end=3186
+  _globals['_CLIENTINFO_SDK']._serialized_start=3055
+  _globals['_CLIENTINFO_SDK']._serialized_end=3186
+  _globals['_CLIENTCONFIGURATION']._serialized_start=3189
+  _globals['_CLIENTCONFIGURATION']._serialized_end=3457
+  _globals['_VIDEOCONFIGURATION']._serialized_start=3459
+  _globals['_VIDEOCONFIGURATION']._serialized_end=3535
+  _globals['_DISABLEDCODECS']._serialized_start=3537
+  _globals['_DISABLEDCODECS']._serialized_end=3618
+  _globals['_RTPDRIFT']._serialized_start=3621
+  _globals['_RTPDRIFT']._serialized_end=3877
+  _globals['_RTPSTATS']._serialized_start=3880
+  _globals['_RTPSTATS']._serialized_end=5192
+  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_start=5141
+  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_end=5192
+  _globals['_TIMEDVERSION']._serialized_start=5194
+  _globals['_TIMEDVERSION']._serialized_end=5243
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/models.pyi` & `livekit-protocol-0.4.0/livekit/protocol/models.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,28 +66,39 @@
     CLIENT_INITIATED: _ClassVar[DisconnectReason]
     DUPLICATE_IDENTITY: _ClassVar[DisconnectReason]
     SERVER_SHUTDOWN: _ClassVar[DisconnectReason]
     PARTICIPANT_REMOVED: _ClassVar[DisconnectReason]
     ROOM_DELETED: _ClassVar[DisconnectReason]
     STATE_MISMATCH: _ClassVar[DisconnectReason]
     JOIN_FAILURE: _ClassVar[DisconnectReason]
+    MIGRATION: _ClassVar[DisconnectReason]
+    SIGNAL_CLOSE: _ClassVar[DisconnectReason]
 
 class ReconnectReason(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     RR_UNKNOWN: _ClassVar[ReconnectReason]
     RR_SIGNAL_DISCONNECTED: _ClassVar[ReconnectReason]
     RR_PUBLISHER_FAILED: _ClassVar[ReconnectReason]
     RR_SUBSCRIBER_FAILED: _ClassVar[ReconnectReason]
     RR_SWITCH_CANDIDATE: _ClassVar[ReconnectReason]
 
 class SubscriptionError(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     SE_UNKNOWN: _ClassVar[SubscriptionError]
     SE_CODEC_UNSUPPORTED: _ClassVar[SubscriptionError]
     SE_TRACK_NOTFOUND: _ClassVar[SubscriptionError]
+
+class AudioTrackFeature(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    TF_STEREO: _ClassVar[AudioTrackFeature]
+    TF_NO_DTX: _ClassVar[AudioTrackFeature]
+    TF_AUTO_GAIN_CONTROL: _ClassVar[AudioTrackFeature]
+    TF_ECHO_CANCELLATION: _ClassVar[AudioTrackFeature]
+    TF_NOISE_SUPPRESSION: _ClassVar[AudioTrackFeature]
+    TF_ENHANCED_NOISE_CANCELLATION: _ClassVar[AudioTrackFeature]
 DEFAULT_AC: AudioCodec
 OPUS: AudioCodec
 AAC: AudioCodec
 DEFAULT_VC: VideoCodec
 H264_BASELINE: VideoCodec
 H264_MAIN: VideoCodec
 H264_HIGH: VideoCodec
@@ -117,50 +128,60 @@
 CLIENT_INITIATED: DisconnectReason
 DUPLICATE_IDENTITY: DisconnectReason
 SERVER_SHUTDOWN: DisconnectReason
 PARTICIPANT_REMOVED: DisconnectReason
 ROOM_DELETED: DisconnectReason
 STATE_MISMATCH: DisconnectReason
 JOIN_FAILURE: DisconnectReason
+MIGRATION: DisconnectReason
+SIGNAL_CLOSE: DisconnectReason
 RR_UNKNOWN: ReconnectReason
 RR_SIGNAL_DISCONNECTED: ReconnectReason
 RR_PUBLISHER_FAILED: ReconnectReason
 RR_SUBSCRIBER_FAILED: ReconnectReason
 RR_SWITCH_CANDIDATE: ReconnectReason
 SE_UNKNOWN: SubscriptionError
 SE_CODEC_UNSUPPORTED: SubscriptionError
 SE_TRACK_NOTFOUND: SubscriptionError
+TF_STEREO: AudioTrackFeature
+TF_NO_DTX: AudioTrackFeature
+TF_AUTO_GAIN_CONTROL: AudioTrackFeature
+TF_ECHO_CANCELLATION: AudioTrackFeature
+TF_NOISE_SUPPRESSION: AudioTrackFeature
+TF_ENHANCED_NOISE_CANCELLATION: AudioTrackFeature
 
 class Room(_message.Message):
-    __slots__ = ("sid", "name", "empty_timeout", "max_participants", "creation_time", "turn_password", "enabled_codecs", "metadata", "num_participants", "num_publishers", "active_recording", "version")
+    __slots__ = ("sid", "name", "empty_timeout", "departure_timeout", "max_participants", "creation_time", "turn_password", "enabled_codecs", "metadata", "num_participants", "num_publishers", "active_recording", "version")
     SID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     EMPTY_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
+    DEPARTURE_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     MAX_PARTICIPANTS_FIELD_NUMBER: _ClassVar[int]
     CREATION_TIME_FIELD_NUMBER: _ClassVar[int]
     TURN_PASSWORD_FIELD_NUMBER: _ClassVar[int]
     ENABLED_CODECS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     NUM_PARTICIPANTS_FIELD_NUMBER: _ClassVar[int]
     NUM_PUBLISHERS_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_RECORDING_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     sid: str
     name: str
     empty_timeout: int
+    departure_timeout: int
     max_participants: int
     creation_time: int
     turn_password: str
     enabled_codecs: _containers.RepeatedCompositeFieldContainer[Codec]
     metadata: str
     num_participants: int
     num_publishers: int
     active_recording: bool
     version: TimedVersion
-    def __init__(self, sid: _Optional[str] = ..., name: _Optional[str] = ..., empty_timeout: _Optional[int] = ..., max_participants: _Optional[int] = ..., creation_time: _Optional[int] = ..., turn_password: _Optional[str] = ..., enabled_codecs: _Optional[_Iterable[_Union[Codec, _Mapping]]] = ..., metadata: _Optional[str] = ..., num_participants: _Optional[int] = ..., num_publishers: _Optional[int] = ..., active_recording: bool = ..., version: _Optional[_Union[TimedVersion, _Mapping]] = ...) -> None: ...
+    def __init__(self, sid: _Optional[str] = ..., name: _Optional[str] = ..., empty_timeout: _Optional[int] = ..., departure_timeout: _Optional[int] = ..., max_participants: _Optional[int] = ..., creation_time: _Optional[int] = ..., turn_password: _Optional[str] = ..., enabled_codecs: _Optional[_Iterable[_Union[Codec, _Mapping]]] = ..., metadata: _Optional[str] = ..., num_participants: _Optional[int] = ..., num_publishers: _Optional[int] = ..., active_recording: bool = ..., version: _Optional[_Union[TimedVersion, _Mapping]] = ...) -> None: ...
 
 class Codec(_message.Message):
     __slots__ = ("mime", "fmtp_line")
     MIME_FIELD_NUMBER: _ClassVar[int]
     FMTP_LINE_FIELD_NUMBER: _ClassVar[int]
     mime: str
     fmtp_line: str
@@ -321,28 +342,34 @@
     width: int
     height: int
     bitrate: int
     ssrc: int
     def __init__(self, quality: _Optional[_Union[VideoQuality, str]] = ..., width: _Optional[int] = ..., height: _Optional[int] = ..., bitrate: _Optional[int] = ..., ssrc: _Optional[int] = ...) -> None: ...
 
 class DataPacket(_message.Message):
-    __slots__ = ("kind", "user", "speaker")
+    __slots__ = ("kind", "participant_identity", "destination_identities", "user", "speaker", "sip_dtmf")
     class Kind(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         RELIABLE: _ClassVar[DataPacket.Kind]
         LOSSY: _ClassVar[DataPacket.Kind]
     RELIABLE: DataPacket.Kind
     LOSSY: DataPacket.Kind
     KIND_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
+    DESTINATION_IDENTITIES_FIELD_NUMBER: _ClassVar[int]
     USER_FIELD_NUMBER: _ClassVar[int]
     SPEAKER_FIELD_NUMBER: _ClassVar[int]
+    SIP_DTMF_FIELD_NUMBER: _ClassVar[int]
     kind: DataPacket.Kind
+    participant_identity: str
+    destination_identities: _containers.RepeatedScalarFieldContainer[str]
     user: UserPacket
     speaker: ActiveSpeakerUpdate
-    def __init__(self, kind: _Optional[_Union[DataPacket.Kind, str]] = ..., user: _Optional[_Union[UserPacket, _Mapping]] = ..., speaker: _Optional[_Union[ActiveSpeakerUpdate, _Mapping]] = ...) -> None: ...
+    sip_dtmf: SipDTMF
+    def __init__(self, kind: _Optional[_Union[DataPacket.Kind, str]] = ..., participant_identity: _Optional[str] = ..., destination_identities: _Optional[_Iterable[str]] = ..., user: _Optional[_Union[UserPacket, _Mapping]] = ..., speaker: _Optional[_Union[ActiveSpeakerUpdate, _Mapping]] = ..., sip_dtmf: _Optional[_Union[SipDTMF, _Mapping]] = ...) -> None: ...
 
 class ActiveSpeakerUpdate(_message.Message):
     __slots__ = ("speakers",)
     SPEAKERS_FIELD_NUMBER: _ClassVar[int]
     speakers: _containers.RepeatedCompositeFieldContainer[SpeakerInfo]
     def __init__(self, speakers: _Optional[_Iterable[_Union[SpeakerInfo, _Mapping]]] = ...) -> None: ...
 
@@ -368,43 +395,53 @@
     participant_identity: str
     payload: bytes
     destination_sids: _containers.RepeatedScalarFieldContainer[str]
     destination_identities: _containers.RepeatedScalarFieldContainer[str]
     topic: str
     def __init__(self, participant_sid: _Optional[str] = ..., participant_identity: _Optional[str] = ..., payload: _Optional[bytes] = ..., destination_sids: _Optional[_Iterable[str]] = ..., destination_identities: _Optional[_Iterable[str]] = ..., topic: _Optional[str] = ...) -> None: ...
 
+class SipDTMF(_message.Message):
+    __slots__ = ("code", "digit")
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    DIGIT_FIELD_NUMBER: _ClassVar[int]
+    code: int
+    digit: str
+    def __init__(self, code: _Optional[int] = ..., digit: _Optional[str] = ...) -> None: ...
+
 class ParticipantTracks(_message.Message):
     __slots__ = ("participant_sid", "track_sids")
     PARTICIPANT_SID_FIELD_NUMBER: _ClassVar[int]
     TRACK_SIDS_FIELD_NUMBER: _ClassVar[int]
     participant_sid: str
     track_sids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, participant_sid: _Optional[str] = ..., track_sids: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class ServerInfo(_message.Message):
-    __slots__ = ("edition", "version", "protocol", "region", "node_id", "debug_info")
+    __slots__ = ("edition", "version", "protocol", "region", "node_id", "debug_info", "agent_protocol")
     class Edition(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         Standard: _ClassVar[ServerInfo.Edition]
         Cloud: _ClassVar[ServerInfo.Edition]
     Standard: ServerInfo.Edition
     Cloud: ServerInfo.Edition
     EDITION_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     REGION_FIELD_NUMBER: _ClassVar[int]
     NODE_ID_FIELD_NUMBER: _ClassVar[int]
     DEBUG_INFO_FIELD_NUMBER: _ClassVar[int]
+    AGENT_PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     edition: ServerInfo.Edition
     version: str
     protocol: int
     region: str
     node_id: str
     debug_info: str
-    def __init__(self, edition: _Optional[_Union[ServerInfo.Edition, str]] = ..., version: _Optional[str] = ..., protocol: _Optional[int] = ..., region: _Optional[str] = ..., node_id: _Optional[str] = ..., debug_info: _Optional[str] = ...) -> None: ...
+    agent_protocol: int
+    def __init__(self, edition: _Optional[_Union[ServerInfo.Edition, str]] = ..., version: _Optional[str] = ..., protocol: _Optional[int] = ..., region: _Optional[str] = ..., node_id: _Optional[str] = ..., debug_info: _Optional[str] = ..., agent_protocol: _Optional[int] = ...) -> None: ...
 
 class ClientInfo(_message.Message):
     __slots__ = ("sdk", "version", "protocol", "os", "os_version", "device_model", "browser", "browser_version", "address", "network")
     class SDK(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         UNKNOWN: _ClassVar[ClientInfo.SDK]
         JS: _ClassVar[ClientInfo.SDK]
@@ -497,15 +534,15 @@
     rtp_clock_ticks: int
     drift_samples: int
     drift_ms: float
     clock_rate: float
     def __init__(self, start_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., end_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[float] = ..., start_timestamp: _Optional[int] = ..., end_timestamp: _Optional[int] = ..., rtp_clock_ticks: _Optional[int] = ..., drift_samples: _Optional[int] = ..., drift_ms: _Optional[float] = ..., clock_rate: _Optional[float] = ...) -> None: ...
 
 class RTPStats(_message.Message):
-    __slots__ = ("start_time", "end_time", "duration", "packets", "packet_rate", "bytes", "header_bytes", "bitrate", "packets_lost", "packet_loss_rate", "packet_loss_percentage", "packets_duplicate", "packet_duplicate_rate", "bytes_duplicate", "header_bytes_duplicate", "bitrate_duplicate", "packets_padding", "packet_padding_rate", "bytes_padding", "header_bytes_padding", "bitrate_padding", "packets_out_of_order", "frames", "frame_rate", "jitter_current", "jitter_max", "gap_histogram", "nacks", "nack_acks", "nack_misses", "nack_repeated", "plis", "last_pli", "firs", "last_fir", "rtt_current", "rtt_max", "key_frames", "last_key_frame", "layer_lock_plis", "last_layer_lock_pli", "packet_drift", "report_drift")
+    __slots__ = ("start_time", "end_time", "duration", "packets", "packet_rate", "bytes", "header_bytes", "bitrate", "packets_lost", "packet_loss_rate", "packet_loss_percentage", "packets_duplicate", "packet_duplicate_rate", "bytes_duplicate", "header_bytes_duplicate", "bitrate_duplicate", "packets_padding", "packet_padding_rate", "bytes_padding", "header_bytes_padding", "bitrate_padding", "packets_out_of_order", "frames", "frame_rate", "jitter_current", "jitter_max", "gap_histogram", "nacks", "nack_acks", "nack_misses", "nack_repeated", "plis", "last_pli", "firs", "last_fir", "rtt_current", "rtt_max", "key_frames", "last_key_frame", "layer_lock_plis", "last_layer_lock_pli", "packet_drift", "report_drift", "rebased_report_drift")
     class GapHistogramEntry(_message.Message):
         __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: int
         value: int
         def __init__(self, key: _Optional[int] = ..., value: _Optional[int] = ...) -> None: ...
@@ -548,14 +585,15 @@
     RTT_MAX_FIELD_NUMBER: _ClassVar[int]
     KEY_FRAMES_FIELD_NUMBER: _ClassVar[int]
     LAST_KEY_FRAME_FIELD_NUMBER: _ClassVar[int]
     LAYER_LOCK_PLIS_FIELD_NUMBER: _ClassVar[int]
     LAST_LAYER_LOCK_PLI_FIELD_NUMBER: _ClassVar[int]
     PACKET_DRIFT_FIELD_NUMBER: _ClassVar[int]
     REPORT_DRIFT_FIELD_NUMBER: _ClassVar[int]
+    REBASED_REPORT_DRIFT_FIELD_NUMBER: _ClassVar[int]
     start_time: _timestamp_pb2.Timestamp
     end_time: _timestamp_pb2.Timestamp
     duration: float
     packets: int
     packet_rate: float
     bytes: int
     header_bytes: int
@@ -591,15 +629,16 @@
     rtt_max: int
     key_frames: int
     last_key_frame: _timestamp_pb2.Timestamp
     layer_lock_plis: int
     last_layer_lock_pli: _timestamp_pb2.Timestamp
     packet_drift: RTPDrift
     report_drift: RTPDrift
-    def __init__(self, start_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., end_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[float] = ..., packets: _Optional[int] = ..., packet_rate: _Optional[float] = ..., bytes: _Optional[int] = ..., header_bytes: _Optional[int] = ..., bitrate: _Optional[float] = ..., packets_lost: _Optional[int] = ..., packet_loss_rate: _Optional[float] = ..., packet_loss_percentage: _Optional[float] = ..., packets_duplicate: _Optional[int] = ..., packet_duplicate_rate: _Optional[float] = ..., bytes_duplicate: _Optional[int] = ..., header_bytes_duplicate: _Optional[int] = ..., bitrate_duplicate: _Optional[float] = ..., packets_padding: _Optional[int] = ..., packet_padding_rate: _Optional[float] = ..., bytes_padding: _Optional[int] = ..., header_bytes_padding: _Optional[int] = ..., bitrate_padding: _Optional[float] = ..., packets_out_of_order: _Optional[int] = ..., frames: _Optional[int] = ..., frame_rate: _Optional[float] = ..., jitter_current: _Optional[float] = ..., jitter_max: _Optional[float] = ..., gap_histogram: _Optional[_Mapping[int, int]] = ..., nacks: _Optional[int] = ..., nack_acks: _Optional[int] = ..., nack_misses: _Optional[int] = ..., nack_repeated: _Optional[int] = ..., plis: _Optional[int] = ..., last_pli: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., firs: _Optional[int] = ..., last_fir: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., rtt_current: _Optional[int] = ..., rtt_max: _Optional[int] = ..., key_frames: _Optional[int] = ..., last_key_frame: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., layer_lock_plis: _Optional[int] = ..., last_layer_lock_pli: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., packet_drift: _Optional[_Union[RTPDrift, _Mapping]] = ..., report_drift: _Optional[_Union[RTPDrift, _Mapping]] = ...) -> None: ...
+    rebased_report_drift: RTPDrift
+    def __init__(self, start_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., end_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[float] = ..., packets: _Optional[int] = ..., packet_rate: _Optional[float] = ..., bytes: _Optional[int] = ..., header_bytes: _Optional[int] = ..., bitrate: _Optional[float] = ..., packets_lost: _Optional[int] = ..., packet_loss_rate: _Optional[float] = ..., packet_loss_percentage: _Optional[float] = ..., packets_duplicate: _Optional[int] = ..., packet_duplicate_rate: _Optional[float] = ..., bytes_duplicate: _Optional[int] = ..., header_bytes_duplicate: _Optional[int] = ..., bitrate_duplicate: _Optional[float] = ..., packets_padding: _Optional[int] = ..., packet_padding_rate: _Optional[float] = ..., bytes_padding: _Optional[int] = ..., header_bytes_padding: _Optional[int] = ..., bitrate_padding: _Optional[float] = ..., packets_out_of_order: _Optional[int] = ..., frames: _Optional[int] = ..., frame_rate: _Optional[float] = ..., jitter_current: _Optional[float] = ..., jitter_max: _Optional[float] = ..., gap_histogram: _Optional[_Mapping[int, int]] = ..., nacks: _Optional[int] = ..., nack_acks: _Optional[int] = ..., nack_misses: _Optional[int] = ..., nack_repeated: _Optional[int] = ..., plis: _Optional[int] = ..., last_pli: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., firs: _Optional[int] = ..., last_fir: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., rtt_current: _Optional[int] = ..., rtt_max: _Optional[int] = ..., key_frames: _Optional[int] = ..., last_key_frame: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., layer_lock_plis: _Optional[int] = ..., last_layer_lock_pli: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., packet_drift: _Optional[_Union[RTPDrift, _Mapping]] = ..., report_drift: _Optional[_Union[RTPDrift, _Mapping]] = ..., rebased_report_drift: _Optional[_Union[RTPDrift, _Mapping]] = ...) -> None: ...
 
 class TimedVersion(_message.Message):
     __slots__ = ("unix_micro", "ticks")
     UNIX_MICRO_FIELD_NUMBER: _ClassVar[int]
     TICKS_FIELD_NUMBER: _ClassVar[int]
     unix_micro: int
     ticks: int
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/room.py` & `livekit-protocol-0.4.0/livekit/protocol/room.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,56 +12,56 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import models as _models_
 from . import egress as _egress_
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12livekit_room.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\"\xe6\x01\n\x11\x43reateRoomRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rempty_timeout\x18\x02 \x01(\r\x12\x18\n\x10max_participants\x18\x03 \x01(\r\x12\x0f\n\x07node_id\x18\x04 \x01(\t\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12#\n\x06\x65gress\x18\x06 \x01(\x0b\x32\x13.livekit.RoomEgress\x12\x19\n\x11min_playout_delay\x18\x07 \x01(\r\x12\x19\n\x11max_playout_delay\x18\x08 \x01(\r\x12\x14\n\x0csync_streams\x18\t \x01(\x08\"\x9e\x01\n\nRoomEgress\x12\x31\n\x04room\x18\x01 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequest\x12\x33\n\x0bparticipant\x18\x03 \x01(\x0b\x32\x1e.livekit.AutoParticipantEgress\x12(\n\x06tracks\x18\x02 \x01(\x0b\x32\x18.livekit.AutoTrackEgress\"!\n\x10ListRoomsRequest\x12\r\n\x05names\x18\x01 \x03(\t\"1\n\x11ListRoomsResponse\x12\x1c\n\x05rooms\x18\x01 \x03(\x0b\x32\r.livekit.Room\"!\n\x11\x44\x65leteRoomRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\"\x14\n\x12\x44\x65leteRoomResponse\"\'\n\x17ListParticipantsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\"J\n\x18ListParticipantsResponse\x12.\n\x0cparticipants\x18\x01 \x03(\x0b\x32\x18.livekit.ParticipantInfo\"9\n\x17RoomParticipantIdentity\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\"\x1b\n\x19RemoveParticipantResponse\"X\n\x14MuteRoomTrackRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x11\n\ttrack_sid\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\":\n\x15MuteRoomTrackResponse\x12!\n\x05track\x18\x01 \x01(\x0b\x32\x12.livekit.TrackInfo\"\x8e\x01\n\x18UpdateParticipantRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\t\x12\x32\n\npermission\x18\x04 \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0c\n\x04name\x18\x05 \x01(\t\"\x9b\x01\n\x1aUpdateSubscriptionsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x12\n\ntrack_sids\x18\x03 \x03(\t\x12\x11\n\tsubscribe\x18\x04 \x01(\x08\x12\x36\n\x12participant_tracks\x18\x05 \x03(\x0b\x32\x1a.livekit.ParticipantTracks\"\x1d\n\x1bUpdateSubscriptionsResponse\"\xb1\x01\n\x0fSendDataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12&\n\x04kind\x18\x03 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12\x1c\n\x10\x64\x65stination_sids\x18\x04 \x03(\tB\x02\x18\x01\x12\x1e\n\x16\x64\x65stination_identities\x18\x06 \x03(\t\x12\x12\n\x05topic\x18\x05 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic\"\x12\n\x10SendDataResponse\";\n\x19UpdateRoomMetadataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08metadata\x18\x02 \x01(\t2\xe6\x06\n\x0bRoomService\x12\x37\n\nCreateRoom\x12\x1a.livekit.CreateRoomRequest\x1a\r.livekit.Room\x12\x42\n\tListRooms\x12\x19.livekit.ListRoomsRequest\x1a\x1a.livekit.ListRoomsResponse\x12\x45\n\nDeleteRoom\x12\x1a.livekit.DeleteRoomRequest\x1a\x1b.livekit.DeleteRoomResponse\x12W\n\x10ListParticipants\x12 .livekit.ListParticipantsRequest\x1a!.livekit.ListParticipantsResponse\x12L\n\x0eGetParticipant\x12 .livekit.RoomParticipantIdentity\x1a\x18.livekit.ParticipantInfo\x12Y\n\x11RemoveParticipant\x12 .livekit.RoomParticipantIdentity\x1a\".livekit.RemoveParticipantResponse\x12S\n\x12MutePublishedTrack\x12\x1d.livekit.MuteRoomTrackRequest\x1a\x1e.livekit.MuteRoomTrackResponse\x12P\n\x11UpdateParticipant\x12!.livekit.UpdateParticipantRequest\x1a\x18.livekit.ParticipantInfo\x12`\n\x13UpdateSubscriptions\x12#.livekit.UpdateSubscriptionsRequest\x1a$.livekit.UpdateSubscriptionsResponse\x12?\n\x08SendData\x12\x18.livekit.SendDataRequest\x1a\x19.livekit.SendDataResponse\x12G\n\x12UpdateRoomMetadata\x12\".livekit.UpdateRoomMetadataRequest\x1a\r.livekit.RoomBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12livekit_room.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\"\x81\x02\n\x11\x43reateRoomRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rempty_timeout\x18\x02 \x01(\r\x12\x19\n\x11\x64\x65parture_timeout\x18\n \x01(\r\x12\x18\n\x10max_participants\x18\x03 \x01(\r\x12\x0f\n\x07node_id\x18\x04 \x01(\t\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12#\n\x06\x65gress\x18\x06 \x01(\x0b\x32\x13.livekit.RoomEgress\x12\x19\n\x11min_playout_delay\x18\x07 \x01(\r\x12\x19\n\x11max_playout_delay\x18\x08 \x01(\r\x12\x14\n\x0csync_streams\x18\t \x01(\x08\"\x9e\x01\n\nRoomEgress\x12\x31\n\x04room\x18\x01 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequest\x12\x33\n\x0bparticipant\x18\x03 \x01(\x0b\x32\x1e.livekit.AutoParticipantEgress\x12(\n\x06tracks\x18\x02 \x01(\x0b\x32\x18.livekit.AutoTrackEgress\"!\n\x10ListRoomsRequest\x12\r\n\x05names\x18\x01 \x03(\t\"1\n\x11ListRoomsResponse\x12\x1c\n\x05rooms\x18\x01 \x03(\x0b\x32\r.livekit.Room\"!\n\x11\x44\x65leteRoomRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\"\x14\n\x12\x44\x65leteRoomResponse\"\'\n\x17ListParticipantsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\"J\n\x18ListParticipantsResponse\x12.\n\x0cparticipants\x18\x01 \x03(\x0b\x32\x18.livekit.ParticipantInfo\"9\n\x17RoomParticipantIdentity\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\"\x1b\n\x19RemoveParticipantResponse\"X\n\x14MuteRoomTrackRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x11\n\ttrack_sid\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\":\n\x15MuteRoomTrackResponse\x12!\n\x05track\x18\x01 \x01(\x0b\x32\x12.livekit.TrackInfo\"\x8e\x01\n\x18UpdateParticipantRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\t\x12\x32\n\npermission\x18\x04 \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0c\n\x04name\x18\x05 \x01(\t\"\x9b\x01\n\x1aUpdateSubscriptionsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x12\n\ntrack_sids\x18\x03 \x03(\t\x12\x11\n\tsubscribe\x18\x04 \x01(\x08\x12\x36\n\x12participant_tracks\x18\x05 \x03(\x0b\x32\x1a.livekit.ParticipantTracks\"\x1d\n\x1bUpdateSubscriptionsResponse\"\xb1\x01\n\x0fSendDataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12&\n\x04kind\x18\x03 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12\x1c\n\x10\x64\x65stination_sids\x18\x04 \x03(\tB\x02\x18\x01\x12\x1e\n\x16\x64\x65stination_identities\x18\x06 \x03(\t\x12\x12\n\x05topic\x18\x05 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic\"\x12\n\x10SendDataResponse\";\n\x19UpdateRoomMetadataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08metadata\x18\x02 \x01(\t2\xe6\x06\n\x0bRoomService\x12\x37\n\nCreateRoom\x12\x1a.livekit.CreateRoomRequest\x1a\r.livekit.Room\x12\x42\n\tListRooms\x12\x19.livekit.ListRoomsRequest\x1a\x1a.livekit.ListRoomsResponse\x12\x45\n\nDeleteRoom\x12\x1a.livekit.DeleteRoomRequest\x1a\x1b.livekit.DeleteRoomResponse\x12W\n\x10ListParticipants\x12 .livekit.ListParticipantsRequest\x1a!.livekit.ListParticipantsResponse\x12L\n\x0eGetParticipant\x12 .livekit.RoomParticipantIdentity\x1a\x18.livekit.ParticipantInfo\x12Y\n\x11RemoveParticipant\x12 .livekit.RoomParticipantIdentity\x1a\".livekit.RemoveParticipantResponse\x12S\n\x12MutePublishedTrack\x12\x1d.livekit.MuteRoomTrackRequest\x1a\x1e.livekit.MuteRoomTrackResponse\x12P\n\x11UpdateParticipant\x12!.livekit.UpdateParticipantRequest\x1a\x18.livekit.ParticipantInfo\x12`\n\x13UpdateSubscriptions\x12#.livekit.UpdateSubscriptionsRequest\x1a$.livekit.UpdateSubscriptionsResponse\x12?\n\x08SendData\x12\x18.livekit.SendDataRequest\x1a\x19.livekit.SendDataResponse\x12G\n\x12UpdateRoomMetadata\x12\".livekit.UpdateRoomMetadataRequest\x1a\r.livekit.RoomBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'room', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
   _globals['_SENDDATAREQUEST'].fields_by_name['destination_sids']._options = None
   _globals['_SENDDATAREQUEST'].fields_by_name['destination_sids']._serialized_options = b'\030\001'
   _globals['_CREATEROOMREQUEST']._serialized_start=76
-  _globals['_CREATEROOMREQUEST']._serialized_end=306
-  _globals['_ROOMEGRESS']._serialized_start=309
-  _globals['_ROOMEGRESS']._serialized_end=467
-  _globals['_LISTROOMSREQUEST']._serialized_start=469
-  _globals['_LISTROOMSREQUEST']._serialized_end=502
-  _globals['_LISTROOMSRESPONSE']._serialized_start=504
-  _globals['_LISTROOMSRESPONSE']._serialized_end=553
-  _globals['_DELETEROOMREQUEST']._serialized_start=555
-  _globals['_DELETEROOMREQUEST']._serialized_end=588
-  _globals['_DELETEROOMRESPONSE']._serialized_start=590
-  _globals['_DELETEROOMRESPONSE']._serialized_end=610
-  _globals['_LISTPARTICIPANTSREQUEST']._serialized_start=612
-  _globals['_LISTPARTICIPANTSREQUEST']._serialized_end=651
-  _globals['_LISTPARTICIPANTSRESPONSE']._serialized_start=653
-  _globals['_LISTPARTICIPANTSRESPONSE']._serialized_end=727
-  _globals['_ROOMPARTICIPANTIDENTITY']._serialized_start=729
-  _globals['_ROOMPARTICIPANTIDENTITY']._serialized_end=786
-  _globals['_REMOVEPARTICIPANTRESPONSE']._serialized_start=788
-  _globals['_REMOVEPARTICIPANTRESPONSE']._serialized_end=815
-  _globals['_MUTEROOMTRACKREQUEST']._serialized_start=817
-  _globals['_MUTEROOMTRACKREQUEST']._serialized_end=905
-  _globals['_MUTEROOMTRACKRESPONSE']._serialized_start=907
-  _globals['_MUTEROOMTRACKRESPONSE']._serialized_end=965
-  _globals['_UPDATEPARTICIPANTREQUEST']._serialized_start=968
-  _globals['_UPDATEPARTICIPANTREQUEST']._serialized_end=1110
-  _globals['_UPDATESUBSCRIPTIONSREQUEST']._serialized_start=1113
-  _globals['_UPDATESUBSCRIPTIONSREQUEST']._serialized_end=1268
-  _globals['_UPDATESUBSCRIPTIONSRESPONSE']._serialized_start=1270
-  _globals['_UPDATESUBSCRIPTIONSRESPONSE']._serialized_end=1299
-  _globals['_SENDDATAREQUEST']._serialized_start=1302
-  _globals['_SENDDATAREQUEST']._serialized_end=1479
-  _globals['_SENDDATARESPONSE']._serialized_start=1481
-  _globals['_SENDDATARESPONSE']._serialized_end=1499
-  _globals['_UPDATEROOMMETADATAREQUEST']._serialized_start=1501
-  _globals['_UPDATEROOMMETADATAREQUEST']._serialized_end=1560
-  _globals['_ROOMSERVICE']._serialized_start=1563
-  _globals['_ROOMSERVICE']._serialized_end=2433
+  _globals['_CREATEROOMREQUEST']._serialized_end=333
+  _globals['_ROOMEGRESS']._serialized_start=336
+  _globals['_ROOMEGRESS']._serialized_end=494
+  _globals['_LISTROOMSREQUEST']._serialized_start=496
+  _globals['_LISTROOMSREQUEST']._serialized_end=529
+  _globals['_LISTROOMSRESPONSE']._serialized_start=531
+  _globals['_LISTROOMSRESPONSE']._serialized_end=580
+  _globals['_DELETEROOMREQUEST']._serialized_start=582
+  _globals['_DELETEROOMREQUEST']._serialized_end=615
+  _globals['_DELETEROOMRESPONSE']._serialized_start=617
+  _globals['_DELETEROOMRESPONSE']._serialized_end=637
+  _globals['_LISTPARTICIPANTSREQUEST']._serialized_start=639
+  _globals['_LISTPARTICIPANTSREQUEST']._serialized_end=678
+  _globals['_LISTPARTICIPANTSRESPONSE']._serialized_start=680
+  _globals['_LISTPARTICIPANTSRESPONSE']._serialized_end=754
+  _globals['_ROOMPARTICIPANTIDENTITY']._serialized_start=756
+  _globals['_ROOMPARTICIPANTIDENTITY']._serialized_end=813
+  _globals['_REMOVEPARTICIPANTRESPONSE']._serialized_start=815
+  _globals['_REMOVEPARTICIPANTRESPONSE']._serialized_end=842
+  _globals['_MUTEROOMTRACKREQUEST']._serialized_start=844
+  _globals['_MUTEROOMTRACKREQUEST']._serialized_end=932
+  _globals['_MUTEROOMTRACKRESPONSE']._serialized_start=934
+  _globals['_MUTEROOMTRACKRESPONSE']._serialized_end=992
+  _globals['_UPDATEPARTICIPANTREQUEST']._serialized_start=995
+  _globals['_UPDATEPARTICIPANTREQUEST']._serialized_end=1137
+  _globals['_UPDATESUBSCRIPTIONSREQUEST']._serialized_start=1140
+  _globals['_UPDATESUBSCRIPTIONSREQUEST']._serialized_end=1295
+  _globals['_UPDATESUBSCRIPTIONSRESPONSE']._serialized_start=1297
+  _globals['_UPDATESUBSCRIPTIONSRESPONSE']._serialized_end=1326
+  _globals['_SENDDATAREQUEST']._serialized_start=1329
+  _globals['_SENDDATAREQUEST']._serialized_end=1506
+  _globals['_SENDDATARESPONSE']._serialized_start=1508
+  _globals['_SENDDATARESPONSE']._serialized_end=1526
+  _globals['_UPDATEROOMMETADATAREQUEST']._serialized_start=1528
+  _globals['_UPDATEROOMMETADATAREQUEST']._serialized_end=1587
+  _globals['_ROOMSERVICE']._serialized_start=1590
+  _globals['_ROOMSERVICE']._serialized_end=2460
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/room.pyi` & `livekit-protocol-0.4.0/livekit/protocol/room.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class CreateRoomRequest(_message.Message):
-    __slots__ = ("name", "empty_timeout", "max_participants", "node_id", "metadata", "egress", "min_playout_delay", "max_playout_delay", "sync_streams")
+    __slots__ = ("name", "empty_timeout", "departure_timeout", "max_participants", "node_id", "metadata", "egress", "min_playout_delay", "max_playout_delay", "sync_streams")
     NAME_FIELD_NUMBER: _ClassVar[int]
     EMPTY_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
+    DEPARTURE_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     MAX_PARTICIPANTS_FIELD_NUMBER: _ClassVar[int]
     NODE_ID_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     EGRESS_FIELD_NUMBER: _ClassVar[int]
     MIN_PLAYOUT_DELAY_FIELD_NUMBER: _ClassVar[int]
     MAX_PLAYOUT_DELAY_FIELD_NUMBER: _ClassVar[int]
     SYNC_STREAMS_FIELD_NUMBER: _ClassVar[int]
     name: str
     empty_timeout: int
+    departure_timeout: int
     max_participants: int
     node_id: str
     metadata: str
     egress: RoomEgress
     min_playout_delay: int
     max_playout_delay: int
     sync_streams: bool
-    def __init__(self, name: _Optional[str] = ..., empty_timeout: _Optional[int] = ..., max_participants: _Optional[int] = ..., node_id: _Optional[str] = ..., metadata: _Optional[str] = ..., egress: _Optional[_Union[RoomEgress, _Mapping]] = ..., min_playout_delay: _Optional[int] = ..., max_playout_delay: _Optional[int] = ..., sync_streams: bool = ...) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., empty_timeout: _Optional[int] = ..., departure_timeout: _Optional[int] = ..., max_participants: _Optional[int] = ..., node_id: _Optional[str] = ..., metadata: _Optional[str] = ..., egress: _Optional[_Union[RoomEgress, _Mapping]] = ..., min_playout_delay: _Optional[int] = ..., max_playout_delay: _Optional[int] = ..., sync_streams: bool = ...) -> None: ...
 
 class RoomEgress(_message.Message):
     __slots__ = ("room", "participant", "tracks")
     ROOM_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     TRACKS_FIELD_NUMBER: _ClassVar[int]
     room: _egress.RoomCompositeEgressRequest
```

### Comparing `livekit-protocol-0.3.2/livekit/protocol/webhook.py` & `livekit-protocol-0.4.0/livekit/protocol/webhook.py`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.3.2/livekit/protocol/webhook.pyi` & `livekit-protocol-0.4.0/livekit/protocol/webhook.pyi`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.3.2/livekit_protocol.egg-info/PKG-INFO` & `livekit-protocol-0.4.0/livekit_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-protocol
-Version: 0.3.2
+Version: 0.4.0
 Summary: Python protocol stubs for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit-protocol-0.3.2/livekit_protocol.egg-info/SOURCES.txt` & `livekit-protocol-0.4.0/livekit_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.3.2/setup.py` & `livekit-protocol-0.4.0/setup.py`

 * *Files identical despite different names*

