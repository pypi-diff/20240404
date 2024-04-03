# Comparing `tmp/snac-1.1.0.tar.gz` & `tmp/snac-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snac-1.1.0.tar", last modified: Tue Mar  5 20:45:03 2024, max compression
+gzip compressed data, was "snac-1.2.0.tar", last modified: Wed Apr  3 23:41:49 2024, max compression
```

## Comparing `snac-1.1.0.tar` & `snac-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:45:03.467576 snac-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-05 20:44:59.000000 snac-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-05 20:45:03.467576 snac-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-05 20:44:59.000000 snac-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 20:45:03.467576 snac-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-05 20:44:59.000000 snac-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:45:03.463576 snac-1.1.0/snac/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-05 20:44:59.000000 snac-1.1.0/snac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-05 20:44:59.000000 snac-1.1.0/snac/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-03-05 20:44:59.000000 snac-1.1.0/snac/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-05 20:44:59.000000 snac-1.1.0/snac/snac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-03-05 20:44:59.000000 snac-1.1.0/snac/vq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:45:03.467576 snac-1.1.0/snac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-05 20:45:03.000000 snac-1.1.0/snac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-05 20:45:03.000000 snac-1.1.0/snac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:45:03.000000 snac-1.1.0/snac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-05 20:45:03.000000 snac-1.1.0/snac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-05 20:45:03.000000 snac-1.1.0/snac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:41:49.779244 snac-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 23:41:46.000000 snac-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-03 23:41:49.779244 snac-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-03 23:41:46.000000 snac-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:41:49.779244 snac-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 23:41:46.000000 snac-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:41:49.779244 snac-1.2.0/snac/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 23:41:46.000000 snac-1.2.0/snac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-03 23:41:46.000000 snac-1.2.0/snac/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-03 23:41:46.000000 snac-1.2.0/snac/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-03 23:41:46.000000 snac-1.2.0/snac/snac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-03 23:41:46.000000 snac-1.2.0/snac/vq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:41:49.779244 snac-1.2.0/snac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-03 23:41:49.000000 snac-1.2.0/snac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 23:41:49.000000 snac-1.2.0/snac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:41:49.000000 snac-1.2.0/snac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 23:41:49.000000 snac-1.2.0/snac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 23:41:49.000000 snac-1.2.0/snac.egg-info/top_level.txt
```

### Comparing `snac-1.1.0/LICENSE` & `snac-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snac-1.1.0/PKG-INFO` & `snac-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snac
-Version: 1.1.0
+Version: 1.2.0
 Summary: Multi-Scale Neural Audio Codec
 Home-page: https://github.com/hubertsiuzdak/snac
 Author: Hubert Siuzdak
 Author-email: hubert.siuzdak@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
@@ -48,25 +48,33 @@
 
 Install it using:
 
 ```bash
 pip install snac
 ```
 
-To encode (and reconstruct) audio with SNAC in Python, use the following code:
+To encode (and decode) audio with SNAC in Python, use the following code:
 
 ```python
 import torch
 from snac import SNAC
 
 model = SNAC.from_pretrained("hubertsiuzdak/snac_32khz").eval().cuda()
-audio = torch.randn(1, 1, 32000).cuda()  # B, 1, T
+audio = torch.randn(1, 1, 32000).cuda()  # placeholder for actual audio with shape (B, 1, T)
 
 with torch.inference_mode():
-    audio_hat, _, codes, _, _ = model(audio)
+    codes = model.encode(audio)
+    audio_hat = model.decode(codes)
+```
+
+You can also encode and reconstruct in a single call:
+
+```python
+with torch.inference_mode():
+    audio_hat, codes = model(audio)
 ```
 
 ⚠️ Note that `codes` is a list of token sequences of variable lengths, each corresponding to a different temporal
 resolution.
 
 ```
 >>> [code.shape[1] for code in codes]
```

### Comparing `snac-1.1.0/README.md` & `snac-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -34,25 +34,33 @@
 
 Install it using:
 
 ```bash
 pip install snac
 ```
 
-To encode (and reconstruct) audio with SNAC in Python, use the following code:
+To encode (and decode) audio with SNAC in Python, use the following code:
 
 ```python
 import torch
 from snac import SNAC
 
 model = SNAC.from_pretrained("hubertsiuzdak/snac_32khz").eval().cuda()
-audio = torch.randn(1, 1, 32000).cuda()  # B, 1, T
+audio = torch.randn(1, 1, 32000).cuda()  # placeholder for actual audio with shape (B, 1, T)
 
 with torch.inference_mode():
-    audio_hat, _, codes, _, _ = model(audio)
+    codes = model.encode(audio)
+    audio_hat = model.decode(codes)
+```
+
+You can also encode and reconstruct in a single call:
+
+```python
+with torch.inference_mode():
+    audio_hat, codes = model(audio)
 ```
 
 ⚠️ Note that `codes` is a list of token sequences of variable lengths, each corresponding to a different temporal
 resolution.
 
 ```
 >>> [code.shape[1] for code in codes]
```

### Comparing `snac-1.1.0/setup.py` & `snac-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `snac-1.1.0/snac/attention.py` & `snac-1.2.0/snac/attention.py`

 * *Files identical despite different names*

### Comparing `snac-1.1.0/snac/layers.py` & `snac-1.2.0/snac/layers.py`

 * *Files identical despite different names*

### Comparing `snac-1.1.0/snac/snac.py` & `snac-1.2.0/snac/snac.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import math
+from typing import List, Tuple
 
 import numpy as np
 import torch
 from torch import nn
 
 from .layers import Encoder, Decoder
 from .vq import ResidualVectorQuantize
@@ -65,21 +66,32 @@
         length = audio_data.shape[-1]
         lcm = math.lcm(self.vq_strides[0], self.attn_window_size or 1)
         pad_to = self.hop_length * lcm
         right_pad = math.ceil(length / pad_to) * pad_to - length
         audio_data = nn.functional.pad(audio_data, (0, right_pad))
         return audio_data
 
-    def forward(self, audio_data):
+    def forward(self, audio_data: torch.Tensor) -> Tuple[torch.Tensor, List[torch.Tensor]]:
         length = audio_data.shape[-1]
         audio_data = self.preprocess(audio_data)
         z = self.encoder(audio_data)
-        z, codes, commitment_loss, codebook_loss = self.quantizer(z)
-        x = self.decoder(z)
-        return x[..., :length], z, codes, commitment_loss, codebook_loss
+        z_q, codes = self.quantizer(z)
+        audio_hat = self.decoder(z_q)
+        return audio_hat[..., :length], codes
+
+    def encode(self, audio_data: torch.Tensor) -> List[torch.Tensor]:
+        audio_data = self.preprocess(audio_data)
+        z = self.encoder(audio_data)
+        _, codes = self.quantizer(z)
+        return codes
+
+    def decode(self, codes: List[torch.Tensor]) -> torch.Tensor:
+        z_q = self.quantizer.from_codes(codes)
+        audio_hat = self.decoder(z_q)
+        return audio_hat
 
     @classmethod
     def from_config(cls, config_path):
         with open(config_path, "r") as f:
             config = json.load(f)
         model = cls(**config)
         return model
```

### Comparing `snac-1.1.0/snac.egg-info/PKG-INFO` & `snac-1.2.0/snac.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snac
-Version: 1.1.0
+Version: 1.2.0
 Summary: Multi-Scale Neural Audio Codec
 Home-page: https://github.com/hubertsiuzdak/snac
 Author: Hubert Siuzdak
 Author-email: hubert.siuzdak@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
@@ -48,25 +48,33 @@
 
 Install it using:
 
 ```bash
 pip install snac
 ```
 
-To encode (and reconstruct) audio with SNAC in Python, use the following code:
+To encode (and decode) audio with SNAC in Python, use the following code:
 
 ```python
 import torch
 from snac import SNAC
 
 model = SNAC.from_pretrained("hubertsiuzdak/snac_32khz").eval().cuda()
-audio = torch.randn(1, 1, 32000).cuda()  # B, 1, T
+audio = torch.randn(1, 1, 32000).cuda()  # placeholder for actual audio with shape (B, 1, T)
 
 with torch.inference_mode():
-    audio_hat, _, codes, _, _ = model(audio)
+    codes = model.encode(audio)
+    audio_hat = model.decode(codes)
+```
+
+You can also encode and reconstruct in a single call:
+
+```python
+with torch.inference_mode():
+    audio_hat, codes = model(audio)
 ```
 
 ⚠️ Note that `codes` is a list of token sequences of variable lengths, each corresponding to a different temporal
 resolution.
 
 ```
 >>> [code.shape[1] for code in codes]
```

