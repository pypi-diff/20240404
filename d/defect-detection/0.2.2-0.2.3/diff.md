# Comparing `tmp/defect_detection-0.2.2.tar.gz` & `tmp/defect_detection-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defect_detection-0.2.2.tar", last modified: Wed Apr  3 06:44:03 2024, max compression
+gzip compressed data, was "defect_detection-0.2.3.tar", last modified: Thu Apr  4 04:26:46 2024, max compression
```

## Comparing `defect_detection-0.2.2.tar` & `defect_detection-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:44:02.999544 defect_detection-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-03 06:43:59.000000 defect_detection-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 06:43:59.000000 defect_detection-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-03 06:44:02.999544 defect_detection-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 06:43:59.000000 defect_detection-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-03 06:43:59.000000 defect_detection-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:44:02.999544 defect_detection-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:44:02.999544 defect_detection-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:44:02.999544 defect_detection-0.2.2/src/defect_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 06:43:59.000000 defect_detection-0.2.2/src/defect_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-03 06:43:59.000000 defect_detection-0.2.2/src/defect_detection/deep_AE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 06:43:59.000000 defect_detection-0.2.2/src/defect_detection/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-03 06:43:59.000000 defect_detection-0.2.2/src/defect_detection/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-03 06:43:59.000000 defect_detection-0.2.2/src/defect_detection/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 06:44:02.000000 defect_detection-0.2.2/src/defect_detection/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:44:02.999544 defect_detection-0.2.2/src/defect_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-03 06:44:02.000000 defect_detection-0.2.2/src/defect_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 06:44:02.000000 defect_detection-0.2.2/src/defect_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:44:02.000000 defect_detection-0.2.2/src/defect_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 06:44:02.000000 defect_detection-0.2.2/src/defect_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 06:44:02.000000 defect_detection-0.2.2/src/defect_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:26:46.932561 defect_detection-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-04 04:26:43.000000 defect_detection-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 04:26:43.000000 defect_detection-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-04 04:26:46.932561 defect_detection-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-04 04:26:43.000000 defect_detection-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-04 04:26:43.000000 defect_detection-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:26:46.932561 defect_detection-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:26:46.928561 defect_detection-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:26:46.932561 defect_detection-0.2.3/src/defect_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 04:26:43.000000 defect_detection-0.2.3/src/defect_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-04 04:26:43.000000 defect_detection-0.2.3/src/defect_detection/deep_AE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-04 04:26:43.000000 defect_detection-0.2.3/src/defect_detection/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-04 04:26:43.000000 defect_detection-0.2.3/src/defect_detection/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-04 04:26:43.000000 defect_detection-0.2.3/src/defect_detection/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 04:26:46.000000 defect_detection-0.2.3/src/defect_detection/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:26:46.932561 defect_detection-0.2.3/src/defect_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-04 04:26:46.000000 defect_detection-0.2.3/src/defect_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-04 04:26:46.000000 defect_detection-0.2.3/src/defect_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:26:46.000000 defect_detection-0.2.3/src/defect_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 04:26:46.000000 defect_detection-0.2.3/src/defect_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 04:26:46.000000 defect_detection-0.2.3/src/defect_detection.egg-info/top_level.txt
```

### Comparing `defect_detection-0.2.2/LICENSE` & `defect_detection-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `defect_detection-0.2.2/PKG-INFO` & `defect_detection-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defect_detection
-Version: 0.2.2
+Version: 0.2.3
 Summary: API for defect detection in PCB and other components.
 Author-email: Louis Vaslin <lovaslin@post.kek.jp>
 Maintainer-email: Louis Vaslin <lovaslin@post.kek.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Louis VASLIN
         
@@ -60,15 +60,15 @@
 Requires-Dist: scikit-learn
 
 # defect_detection
 
 [![PyPI](https://img.shields.io/pypi/v/defect_detection)](https://pypi.org/project/defect_detection/)
 [![Build](https://github.com/lovaslin/defect_detection/actions/workflows/cd.yml/badge.svg)](https://github.com/lovaslin/defect_detection/actions)
 
-This packge provides a basic API to implement defect detection algorithms. 
+This packge provides a basic API to implement defect detection algorithms.
 These algorithms can be tune in order to automatically detect any defects in a PCB or other components.
 
 ## Requirement
 
 The following package are required :
 - numpy
 - opencv-python
@@ -91,9 +91,7 @@
 pip install -e .
 ```
 
 For the local install, you should of course run the commands using a clean python environment.
 I recommend to use `venv` to setup a pip-friendly environemnt.
 
 ## Usage
-
-
```

### Comparing `defect_detection-0.2.2/README.md` & `defect_detection-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # defect_detection
 
 [![PyPI](https://img.shields.io/pypi/v/defect_detection)](https://pypi.org/project/defect_detection/)
 [![Build](https://github.com/lovaslin/defect_detection/actions/workflows/cd.yml/badge.svg)](https://github.com/lovaslin/defect_detection/actions)
 
-This packge provides a basic API to implement defect detection algorithms. 
+This packge provides a basic API to implement defect detection algorithms.
 These algorithms can be tune in order to automatically detect any defects in a PCB or other components.
 
 ## Requirement
 
 The following package are required :
 - numpy
 - opencv-python
@@ -30,9 +30,7 @@
 pip install -e .
 ```
 
 For the local install, you should of course run the commands using a clean python environment.
 I recommend to use `venv` to setup a pip-friendly environemnt.
 
 ## Usage
-
-
```

### Comparing `defect_detection-0.2.2/pyproject.toml` & `defect_detection-0.2.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -46,7 +46,11 @@
 
 [project.urls]
 "Documentation" = "https://github.com/lovaslin/defect_detection"
 "Homepage" = "https://github.com/lovaslin/defect_detection"
 "Bug Tracker" = "https://github.com/lovaslin/defect_detection/issues"
 "Source" = "https://github.com/lovaslin/defect_detection"
 
+[tool.flake8]
+max-complexity = 12
+extend-ignore = "E203, E266, E402, E501, C901"
+extend-select = "B, B9"
```

### Comparing `defect_detection-0.2.2/src/defect_detection/deep_AE.py` & `defect_detection-0.2.3/src/defect_detection/deep_AE.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,256 +6,288 @@
 ## Class methods :                                                      ##
 ##     batch_train : perform one training step on a batch of inputs     ##
 ##     batch_apply : perform one evaluation step on a batch of inputs   ##
 ##########################################################################
 
 
 import torch
-import numpy
 import os
 
 
 class AE_cls(torch.nn.Module):
-    '''
+    """
     Class inplementing the deep AE architecture using pyTorch.
     Provides also methods for training and appalying model using input batches.
-    '''
-    
+    """
+
     # Initialization method
     def __init__(self, p, apply_only=False, loss_fn=None, opt=None, opt_param=None):
-        '''
+        """
         Arguments :
             p : dict()
                 Python dict containing all the information about the AE architecture.
-            
+
             apply_only : (bool)
                 Specify if the model is used only for application (default: False).
                 Note that the training method is not usable if set to True.
-            
+
             loss_fn : (function)
                 The loss function used to train the model.
                 Must be compatible with torch API.
                 If you plan to use event weights, use a loss that returns one value per individual inputs.
                 Not required if apply_only is set to True.
-            
+
             opt : (torch.optim object)
                 Instance of the torch optimizer used to compute gradient and update model parameters.
                 Not required if apply_only is set to True.
-            
+
             opt_param : (dict)
                 Python dict containing the additionnal arguments to be passed to the optimizer.
                 If not specify, no argument are given to the optimizer.
                 *Optional*
-        '''
+        """
         super().__init__()
-        
+
         dt = torch.float32
-        
+
         # Function to define one encoding block
         def get_block_en(bf, ksize, drop):
             b = torch.nn.Sequential(
-                torch.nn.Conv2d(bf[0], bf[1], kernel_size=ksize, padding=ksize // 2, dtype=dt),
+                torch.nn.Conv2d(
+                    bf[0], bf[1], kernel_size=ksize, padding=ksize // 2, dtype=dt
+                ),
                 torch.nn.LeakyReLU(negative_slope=0.1),
-                torch.nn.Conv2d(bf[1], bf[2], kernel_size=ksize, padding=ksize // 2, stride=2, dtype=dt),
+                torch.nn.Conv2d(
+                    bf[1],
+                    bf[2],
+                    kernel_size=ksize,
+                    padding=ksize // 2,
+                    stride=2,
+                    dtype=dt,
+                ),
                 torch.nn.Dropout(drop),
                 torch.nn.LeakyReLU(negative_slope=0.1),
             )
             return b
-        
+
         # Function to define one decoding block
         def get_block_de(bf, ksize, drop, opad, last=False):
             if last:
                 b = torch.nn.Sequential(
-                    torch.nn.ConvTranspose2d(bf[0], bf[1], kernel_size=ksize, padding=ksize // 2, output_padding=opad, stride=2, dtype=dt),
+                    torch.nn.ConvTranspose2d(
+                        bf[0],
+                        bf[1],
+                        kernel_size=ksize,
+                        padding=ksize // 2,
+                        output_padding=opad,
+                        stride=2,
+                        dtype=dt,
+                    ),
                     torch.nn.Dropout(drop),
                     torch.nn.LeakyReLU(negative_slope=0.1),
-                    torch.nn.ConvTranspose2d(bf[1], bf[2], kernel_size=ksize, padding=ksize // 2, dtype=dt),
+                    torch.nn.ConvTranspose2d(
+                        bf[1], bf[2], kernel_size=ksize, padding=ksize // 2, dtype=dt
+                    ),
                 )
             else:
                 b = torch.nn.Sequential(
-                    torch.nn.ConvTranspose2d(bf[0], bf[1], kernel_size=ksize, padding=ksize // 2, output_padding=opad, stride=2, dtype=dt),
+                    torch.nn.ConvTranspose2d(
+                        bf[0],
+                        bf[1],
+                        kernel_size=ksize,
+                        padding=ksize // 2,
+                        output_padding=opad,
+                        stride=2,
+                        dtype=dt,
+                    ),
                     torch.nn.Dropout(drop),
                     torch.nn.LeakyReLU(negative_slope=0.1),
-                    torch.nn.ConvTranspose2d(bf[1], bf[2], kernel_size=ksize, padding=ksize // 2, dtype=dt),
+                    torch.nn.ConvTranspose2d(
+                        bf[1], bf[2], kernel_size=ksize, padding=ksize // 2, dtype=dt
+                    ),
                     torch.nn.LeakyReLU(negative_slope=0.1),
                 )
             return b
-        
+
         # Define the encoding sequense
         en_seq = (
             get_block_en(bf, ksize, drop)
-            for bf, ksize, drop in zip(p['block_size_in'], p['block_ker'], p['drop'])
+            for bf, ksize, drop in zip(p["block_size_in"], p["block_ker"], p["drop"])
         )
-        
+
         # Define the decoding sequence
         de_seq = (
-            get_block_de(bf, ksize, drop, opad, i+1==len(p['drop']))
-            for i, (bf, ksize, drop, opad) in enumerate(zip(p['block_size_out'], p['block_ker'][::-1], p['drop'][::-1], p['out_pad']))
+            get_block_de(bf, ksize, drop, opad, i + 1 == len(p["drop"]))
+            for i, (bf, ksize, drop, opad) in enumerate(
+                zip(
+                    p["block_size_out"],
+                    p["block_ker"][::-1],
+                    p["drop"][::-1],
+                    p["out_pad"],
+                )
+            )
         )
-        
+
         # Set the encoder sequence
         self.encoder = torch.nn.Sequential(
             *en_seq,
             torch.nn.Conv2d(
-                p['block_size_in'][-1][-1],
-                p['latent_size'],
-                kernel_size=p['latent_ker'],
-                padding=p['latent_ker'] // 2,
+                p["block_size_in"][-1][-1],
+                p["latent_size"],
+                kernel_size=p["latent_ker"],
+                padding=p["latent_ker"] // 2,
                 stride=2,
-                dtype=dt
+                dtype=dt,
             )
         )
-        
+
         # Set the decoder sequence
         self.decoder = torch.nn.Sequential(
             torch.nn.ConvTranspose2d(
-                p['latent_size'],
-                p['block_size_out'][0][0],
-                kernel_size=p['block_ker'][-1],
-                padding=p['block_ker'][-1] // 2,
+                p["latent_size"],
+                p["block_size_out"][0][0],
+                kernel_size=p["block_ker"][-1],
+                padding=p["block_ker"][-1] // 2,
                 stride=2,
-                output_padding=p['latent_opad'],
-                dtype=dt
+                output_padding=p["latent_opad"],
+                dtype=dt,
             ),
             *de_seq
         )
-        
+
         # Store the configuration
         self.config = p
-        
+
         # Set the loss function and optimiser (if needed)
         self.apply_only = apply_only
         if not apply_only:
             self.loss_fn = loss_fn
             if opt_param is None:
                 opt_param = dict()
             self.opt = opt(self.parameters(), **opt_param)
-        
+
         return
-    
+
     # Device selection method (includes automatic selection)
     def to_dev(self, dev):
-        '''
+        """
         Select the device torch should use for this model.
         Supports automatic selection.
-        
+
         Arguments :
             dev : (str)
                 Specify the device to use for this model.
                 Supported values are 'cuda', 'cpu' and 'auto'.
-        '''
+        """
         # Check if auto
-        if dev=='auto':
+        if dev == "auto":
             # Check if cuda is available
             if torch.cuda.is_available():
-                dev = 'cuda'
+                dev = "cuda"
             else:
-                dev = 'cpu'
-        
+                dev = "cpu"
+
         # Set device
         self.to(dev)
-        
+
         return
-    
+
     # Forward pass method (internal use only)
     def forward(self, x):
-        '''
+        """
         Return the output of the model given input x.
-        '''
+        """
         return self.decoder(self.encoder(x))
-    
+
     # Model training method
     def batch_train(self, x, x_n, w=None):
-        '''
+        """
         Train model on a batch of inputs with the possibility to use input weights.
         Arguments :
             x :
                 Input batch tensor, stored on the same device than the model.
                 Used as target for the loss calculation.
-            x_n : 
+            x_n :
                 Noisy version of the input tensor, stored on the same device than the model.
                 Used as input of the model.
             w : *optional*
                 The input weight tensor, stored on the same device than the model.
                 Default to None (don't use input weight).
-        '''
+        """
         # Check if apply_only
         if self.apply_only:
             print("This model is in apply ony mode, cannot call the train method.")
             return None
-        
+
         # Apply model and get output
         y = self(x_n)
-        
+
         # Compute loss
         loss = self.loss_fn(x, y)
-        
+
         # Check if weights must be applied
         if w is not None:
             # Ponderate mean
             loss = (w * loss).sum() / w.sum()
         else:
             # Simple mean
             loss = loss.mean()
-        
+
         # Gradient and optimization step
         self.opt.zero_grad()
         loss.backward()
         self.opt.step()
-        
-        return loss.detach().to('cpu').numpy()
-    
+
+        return loss.detach().to("cpu").numpy()
+
     # Model aplication method
     def batch_apply(self, x, alt_loss_fn=None):
-        '''
+        """
         Apply model on a batch of inputs and return both output and loss values.
         Make sure to set the model in evaluation mode before calling this method.
         Arguments :
             x :
                 Input tensor on which inference is performed (must be on same device as model).
             alt_loss_fn : *optional*
                 Alternative loss function to be used for model evaluation (default to None).
                 If None, the default training loss function is used.
         Returns :
             y :
                 The output of the model in numpy format.
             loss :
                 The corresponding loss values in numpy format.
-        '''
+        """
         # Skip gradient computation (not needed for inference)
         with torch.inference_mode():
             # Get output
             y = self(x)
-            
+
             # Get loss (check for alternative)
             if alt_loss_fn is None:
                 loss = self.loss_fn(x, y)
             else:
                 loss = alt_loss_fn(x, y)
-        
-        return y.detach().to('cpu').numpy(), loss.detach().to('cpu').numpy()
-    
+
+        return y.detach().to("cpu").numpy(), loss.detach().to("cpu").numpy()
+
     # Model save method
     def save_model(self, path):
-        '''
+        """
         Save both the model configuration and state in two separate files.
         Argument :
             path :
                 Path to the directory in which save files are created.
-        '''
+        """
         # Check if path exits and try to create it if not
         if not os.path.exists(path):
             os.mkdir(path, 0o755)
-        
+
         # Save config in text file
-        with open(path + 'AE_config.txt', 'w') as f:
+        with open(path + "AE_config.txt", "w") as f:
             print(self.config, file=f)
-        
-        # Save state_dict
-        torch.save(self.state_dict(), path + 'AE_state.save')
-        
-        return
-    
-    ##END OF AE_cls##
 
+        # Save state_dict
+        torch.save(self.state_dict(), path + "AE_state.save")
 
+        return
 
+    # END OF AE_cls
```

### Comparing `defect_detection-0.2.2/src/defect_detection/filtering.py` & `defect_detection-0.2.3/src/defect_detection/filtering.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 import numpy as np
 from sklearn.cluster import DBSCAN
 
 
 # Function that takes in an input image and configuration and returns the selected pixels
 def get_pixels(emap, th, dbs_param, pix_th):
-    '''
+    """
     Perform a selection of anomalous pixels based on the error map associated to the an image.
     The basic selection is done based on the given threshold value.
     The obtained list is then denoised using the DBSCAN clustering algorithm.
-    
+
     Arguments :
         emap : the error map associated to the image
         th : the initial selection threshold
         dbs_param : dict of additional arguments to be passed to the DBSCAN instance
         pix_th : The minimum number of pixels required per clusters (None means no requirement)
-    
+
     Returns :
         pix : clean list of selected pixels
-    '''
-    
+    """
+
     # Get raw selection (set non selected to 0)
     emap[emap <= th] = 0
-    
+
     # Get pixel coordinates
     pix = np.argwhere(emap)
     del emap
-    
+
     # Initialise DBSCAN with parameters and run clustering
     dbs = DBSCAN(**dbs_param)
     fil = dbs.fit_predict(pix)
-    
+
     # Add the pix_th criteria
     if pix_th:
         # Remove small cluster and remove noisy labels
         lab, count = np.unique(fil, return_counts=True)
         lab = lab[1:]
         count = count[1:]
         pix = pix[np.isin(fil, lab[count >= pix_th])]
         del lab
         del count
     else:
         # Only filter out noisy labels
         pix = pix[fil > -1]
-    
+
     # Return the filtered pixel list
     return pix
-
-
-
-
-
```

### Comparing `defect_detection-0.2.2/src/defect_detection/functions.py` & `defect_detection-0.2.3/src/defect_detection/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,53 +4,53 @@
 
 import torch
 from .deep_AE import AE_cls
 
 
 # Error map using mean
 def emap_mean(x, y):
-    return torch.mean(torch.square(x - y), (0)).detach().to('cpu').numpy()
+    return torch.mean(torch.square(x - y), (0)).detach().to("cpu").numpy()
+
 
 # Error map using sum
 def emap_sum(x, y):
-    return torch.sum(torch.square(x - y), (0)).detach().to('cpu').numpy()
+    return torch.sum(torch.square(x - y), (0)).detach().to("cpu").numpy()
+
 
 # Load a trained model
 def deepAE_load(path, use_only=True, loss_fn=None, opt=None, opt_param=None):
-    '''
+    """
     Function to load a trained deepAE model.
-    
+
     Arguments :
         path : (Path or str)
             The path to the directory where the model is stored.
             The folder must contain the hyperparameter file and the trained parameters.
-        
+
         use_only : (bool)
             Specify if the model is intended for application only.
             If true, the training method cannot be called.
             Default to True.
-        
+
         loss_fn : (function)
             The loss function used to train the model.
             Ignored if use_only is set to True.
-        
+
         opt : (torch.optim object)
             The optimizer used to trained the model.
             Ignored if use_only is set to True.
-        
+
         opt_param : (None or dict)
             The parameters to be passed to the optimizer.
             If None, a empty dict is assumed.
-    '''
+    """
     # Load the model hyperparameter
-    with open(path + 'AE_config.txt', 'r') as f:
+    with open(path + "AE_config.txt") as f:
         param = eval(f.read())
-    
+
     # Initilize the model
     ae = AE_cls(param, use_only, loss_fn, opt, opt_param)
-    
-    # Load trained parameters
-    ae.load_state_dict(torch.load(path + 'AE_state.save'))
-    
-    return ae
 
+    # Load trained parameters
+    ae.load_state_dict(torch.load(path + "AE_state.save"))
 
+    return ae
```

### Comparing `defect_detection-0.2.2/src/defect_detection.egg-info/PKG-INFO` & `defect_detection-0.2.3/src/defect_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defect_detection
-Version: 0.2.2
+Version: 0.2.3
 Summary: API for defect detection in PCB and other components.
 Author-email: Louis Vaslin <lovaslin@post.kek.jp>
 Maintainer-email: Louis Vaslin <lovaslin@post.kek.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Louis VASLIN
         
@@ -60,15 +60,15 @@
 Requires-Dist: scikit-learn
 
 # defect_detection
 
 [![PyPI](https://img.shields.io/pypi/v/defect_detection)](https://pypi.org/project/defect_detection/)
 [![Build](https://github.com/lovaslin/defect_detection/actions/workflows/cd.yml/badge.svg)](https://github.com/lovaslin/defect_detection/actions)
 
-This packge provides a basic API to implement defect detection algorithms. 
+This packge provides a basic API to implement defect detection algorithms.
 These algorithms can be tune in order to automatically detect any defects in a PCB or other components.
 
 ## Requirement
 
 The following package are required :
 - numpy
 - opencv-python
@@ -91,9 +91,7 @@
 pip install -e .
 ```
 
 For the local install, you should of course run the commands using a clean python environment.
 I recommend to use `venv` to setup a pip-friendly environemnt.
 
 ## Usage
-
-
```

