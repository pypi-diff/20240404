# Comparing `tmp/multi_emotion-0.1.14.tar.gz` & `tmp/multi_emotion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_emotion-0.1.14.tar", last modified: Thu Apr  4 16:23:34 2024, max compression
+gzip compressed data, was "multi_emotion-0.1.3.tar", last modified: Wed Aug 30 08:34:32 2023, max compression
```

## Comparing `multi_emotion-0.1.14.tar` & `multi_emotion-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.169247 multi_emotion-0.1.14/
--rw-rw-rw-   0        0        0     8473 2024-04-04 16:23:34.166745 multi_emotion-0.1.14/PKG-INFO
--rw-rw-rw-   0        0        0     7694 2023-09-02 15:22:04.000000 multi_emotion-0.1.14/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.112706 multi_emotion-0.1.14/configs/
--rw-rw-rw-   0        0        0       82 2023-04-11 02:34:34.000000 multi_emotion-0.1.14/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.116210 multi_emotion-0.1.14/multi_emotion/
--rw-rw-rw-   0        0        0        0 2023-04-11 02:34:34.000000 multi_emotion-0.1.14/multi_emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.135224 multi_emotion-0.1.14/multi_emotion/data/
--rw-rw-rw-   0        0        0        0 2023-04-11 02:34:34.000000 multi_emotion-0.1.14/multi_emotion/data/__init__.py
--rw-rw-rw-   0        0        0     6863 2023-08-30 11:52:38.000000 multi_emotion-0.1.14/multi_emotion/data/data.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.141731 multi_emotion-0.1.14/multi_emotion/model/
--rw-rw-rw-   0        0        0        0 2023-04-08 04:00:53.000000 multi_emotion-0.1.14/multi_emotion/model/__init__.py
--rw-rw-rw-   0        0        0     3255 2023-08-29 16:04:29.000000 multi_emotion-0.1.14/multi_emotion/model/attention.py
--rw-rw-rw-   0        0        0     6084 2023-08-29 16:09:10.000000 multi_emotion-0.1.14/multi_emotion/model/base_model.py
--rw-rw-rw-   0        0        0     9749 2023-08-30 11:52:38.000000 multi_emotion-0.1.14/multi_emotion/model/lm.py
--rw-rw-rw-   0        0        0     4935 2023-11-27 11:16:50.000000 multi_emotion-0.1.14/multi_emotion/multi_emotion.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.158740 multi_emotion-0.1.14/multi_emotion/utils/
--rw-rw-rw-   0        0        0        0 2023-08-19 13:22:34.000000 multi_emotion-0.1.14/multi_emotion/utils/__init__.py
--rw-rw-rw-   0        0        0      365 2023-08-29 16:09:10.000000 multi_emotion-0.1.14/multi_emotion/utils/callbacks.py
--rw-rw-rw-   0        0        0     2140 2023-08-29 16:09:10.000000 multi_emotion-0.1.14/multi_emotion/utils/conf.py
--rw-rw-rw-   0        0        0      846 2023-08-29 16:09:10.000000 multi_emotion-0.1.14/multi_emotion/utils/data.py
--rw-rw-rw-   0        0        0     4050 2023-08-30 12:14:54.000000 multi_emotion-0.1.14/multi_emotion/utils/logging.py
--rw-rw-rw-   0        0        0      471 2023-08-29 16:09:10.000000 multi_emotion-0.1.14/multi_emotion/utils/losses.py
--rw-rw-rw-   0        0        0     1166 2023-08-29 16:09:10.000000 multi_emotion-0.1.14/multi_emotion/utils/metrics.py
--rw-rw-rw-   0        0        0     5744 2023-08-29 08:26:14.000000 multi_emotion-0.1.14/multi_emotion/utils/optim.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.162745 multi_emotion-0.1.14/multi_emotion/utils/sentiTree/
--rw-rw-rw-   0        0        0       73 2023-08-30 11:34:30.000000 multi_emotion-0.1.14/multi_emotion/utils/sentiTree/__init__.py
--rw-rw-rw-   0        0        0     7461 2023-09-02 07:51:53.000000 multi_emotion-0.1.14/multi_emotion/utils/sentiTree/data_utils.py
--rw-rw-rw-   0        0        0     7220 2023-08-30 11:52:38.000000 multi_emotion-0.1.14/multi_emotion/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:23:34.164744 multi_emotion-0.1.14/multi_emotion.egg-info/
--rw-rw-rw-   0        0        0     8473 2024-04-04 16:23:34.000000 multi_emotion-0.1.14/multi_emotion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      819 2024-04-04 16:23:34.000000 multi_emotion-0.1.14/multi_emotion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:23:34.000000 multi_emotion-0.1.14/multi_emotion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-04-04 16:23:34.000000 multi_emotion-0.1.14/multi_emotion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-04 16:23:34.000000 multi_emotion-0.1.14/multi_emotion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 16:23:34.169247 multi_emotion-0.1.14/setup.cfg
--rw-rw-rw-   0        0        0     1079 2024-04-04 16:23:08.000000 multi_emotion-0.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-30 08:34:32.640866 multi_emotion-0.1.3/
+-rw-rw-rw-   0        0        0     8236 2023-08-30 08:34:32.640866 multi_emotion-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7667 2023-08-30 07:38:34.000000 multi_emotion-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-30 08:34:32.640866 multi_emotion-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-08-30 08:34:30.000000 multi_emotion-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-30 08:34:32.612813 multi_emotion-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-30 08:34:32.614800 multi_emotion-0.1.3/src/data/
+-rw-rw-rw-   0        0        0        0 2023-04-11 02:34:34.000000 multi_emotion-0.1.3/src/data/__init__.py
+-rw-rw-rw-   0        0        0     6853 2023-08-29 16:04:29.000000 multi_emotion-0.1.3/src/data/data.py
+drwxrwxrwx   0        0        0        0 2023-08-30 08:34:32.616794 multi_emotion-0.1.3/src/model/
+-rw-rw-rw-   0        0        0        0 2023-04-08 04:00:53.000000 multi_emotion-0.1.3/src/model/__init__.py
+-rw-rw-rw-   0        0        0     3255 2023-08-29 16:04:29.000000 multi_emotion-0.1.3/src/model/attention.py
+-rw-rw-rw-   0        0        0     6084 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/model/base_model.py
+-rw-rw-rw-   0        0        0     9669 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/model/lm.py
+drwxrwxrwx   0        0        0        0 2023-08-30 08:34:32.627766 multi_emotion-0.1.3/src/multi_emotion.egg-info/
+-rw-rw-rw-   0        0        0     8236 2023-08-30 08:34:32.000000 multi_emotion-0.1.3/src/multi_emotion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-08-30 08:34:32.000000 multi_emotion-0.1.3/src/multi_emotion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-30 08:34:32.000000 multi_emotion-0.1.3/src/multi_emotion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-08-30 08:34:32.000000 multi_emotion-0.1.3/src/multi_emotion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-30 08:34:32.000000 multi_emotion-0.1.3/src/multi_emotion.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-30 08:34:32.639831 multi_emotion-0.1.3/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-19 13:22:34.000000 multi_emotion-0.1.3/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/callbacks.py
+-rw-rw-rw-   0        0        0     2140 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/conf.py
+-rw-rw-rw-   0        0        0      846 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/data.py
+-rw-rw-rw-   0        0        0     5062 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/logging.py
+-rw-rw-rw-   0        0        0      471 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/losses.py
+-rw-rw-rw-   0        0        0     1166 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/metrics.py
+-rw-rw-rw-   0        0        0     5744 2023-08-29 08:26:14.000000 multi_emotion-0.1.3/src/utils/optim.py
+-rw-rw-rw-   0        0        0     7210 2023-08-29 16:09:10.000000 multi_emotion-0.1.3/src/utils/utils.py
```

### Comparing `multi_emotion-0.1.14/PKG-INFO` & `multi_emotion-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 Metadata-Version: 2.1
 Name: multi_emotion
-Version: 0.1.14
+Version: 0.1.3
 Summary: detect multiple emotions in a sentence including [anger, anticipation, disgust, fear, joy, love, optimism, pessimism, sadness,                    surprise, trust]
 Home-page: https://github.com/JinfenLi/multi_emotion_recognition
 Author: Jinfen Li
 Author-email: jli284@syr.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-Requires-Dist: lightning>=2
-Requires-Dist: emotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: rich
-Requires-Dist: torchmetrics>=1
-Requires-Dist: tqdm
-Requires-Dist: transformers==4.31.0
 
 # Multi-emotion Recognition Using Multi-EmoBERT and Emotion Analysis in Fake News
 
 This is the official PyTorch [repo](https://github.com/JinfenLi/multi_emotion_recognition) for [Multi-EmoBERT](https://dl.acm.org/doi/abs/10.1145/3578503.3583595), a learning framework for multi-emotion recognition.
 
 ```
 Multi-emotion Recognition Using Multi-EmoBERT and Emotion Analysis in Fake News
@@ -40,22 +32,22 @@
   pages={128--135},
   year={2023}
 }
 ```
 ## Usage via Pip Package
 install pip package
 ```
-pip install multi-emotion==0.1.12
+pip install multi-emotion
 ```
 use pip package
 ```
-from multi_emotion import multi_emotion
+import multi_emotion
 multi_emotion.predict(["I am so happy today"])
 ```
-preview result
+result preview
 ```
 [{'text': 'i am so happy today', 'pred_label': 'joy,love,optimism', 'probability': '[{"anger": 0.00022063202050048858}, {"anticipation": 0.007108359131962061}, {"disgust": 0.0006860275752842426}, {"fear": 0.00044393239659257233}, {"joy": 0.9998739957809448}, {"love": 0.8244059085845947}, {"optimism": 0.931083083152771}, {"pessimism": 0.0002464792341925204}, {"sadness": 0.007342423778027296}, {"surprise": 0.001668739365413785}, {"trust": 0.009098367765545845}]'}]
 
 ```
```

### Comparing `multi_emotion-0.1.14/README.md` & `multi_emotion-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
   pages={128--135},
   year={2023}
 }
 ```
 ## Usage via Pip Package
 install pip package
 ```
-pip install multi-emotion==0.1.12
+pip install multi-emotion
 ```
 use pip package
 ```
-from multi_emotion import multi_emotion
+import multi_emotion
 multi_emotion.predict(["I am so happy today"])
 ```
-preview result
+result preview
 ```
 [{'text': 'i am so happy today', 'pred_label': 'joy,love,optimism', 'probability': '[{"anger": 0.00022063202050048858}, {"anticipation": 0.007108359131962061}, {"disgust": 0.0006860275752842426}, {"fear": 0.00044393239659257233}, {"joy": 0.9998739957809448}, {"love": 0.8244059085845947}, {"optimism": 0.931083083152771}, {"pessimism": 0.0002464792341925204}, {"sadness": 0.007342423778027296}, {"surprise": 0.001668739365413785}, {"trust": 0.009098367765545845}]'}]
 
 ```
```

### Comparing `multi_emotion-0.1.14/multi_emotion/data/data.py` & `multi_emotion-0.1.3/src/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 import pickle
 from lightning.pytorch import LightningDataModule
 import torch
 from torch.utils.data import DataLoader, Dataset
 from tqdm import tqdm
-from multi_emotion.utils.data import data_keys
+from src.utils.data import data_keys
 
 
 class DataModule(LightningDataModule):
 
     def __init__(self,
                  use_hashtag: bool = False,
                  use_senti_tree: bool = False, phrase_num: int = 0, dataset: str = None,
```

### Comparing `multi_emotion-0.1.14/multi_emotion/model/attention.py` & `multi_emotion-0.1.3/src/model/attention.py`

 * *Files identical despite different names*

### Comparing `multi_emotion-0.1.14/multi_emotion/model/base_model.py` & `multi_emotion-0.1.3/src/model/base_model.py`

 * *Files identical despite different names*

### Comparing `multi_emotion-0.1.14/multi_emotion/model/lm.py` & `multi_emotion-0.1.3/src/model/lm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import torch
 from torch import nn
 
 from transformers import AutoModel, AutoTokenizer
-from multi_emotion.model.base_model import BaseModel
-from multi_emotion.model.attention import TokenAttention
-from multi_emotion.utils.data import English_Hashtag_Voc_Size, Spanish_Hashtag_Voc_Size
-from multi_emotion.utils.losses import calc_task_loss
-from multi_emotion.utils.metrics import init_best_metrics, init_perf_metrics
-from multi_emotion.utils.optim import setup_optimizer_params, setup_scheduler, freeze_layers
-from multi_emotion.utils.logging import log_step_losses, log_epoch_losses, log_epoch_metrics
-from multi_emotion.utils.utils import generate_output_file
+from src.model.base_model import BaseModel
+from src.model.attention import TokenAttention
+from src.utils.data import English_Hashtag_Voc_Size, Spanish_Hashtag_Voc_Size
+from src.utils.losses import calc_task_loss
+from src.utils.metrics import init_best_metrics, init_perf_metrics
+from src.utils.optim import setup_optimizer_params, setup_scheduler, freeze_layers
+from src.utils.logging import log_step_losses, log_epoch_losses, log_epoch_metrics
+from src.utils.utils import generate_output_file
 
 
 class MultiEmoModel(BaseModel):
     def __init__(self, arch: str, use_hashtag: bool = True, use_senti_tree: bool = True, use_emo_cor: bool = True,
                  hashtag_emb_dim: int = 0,
                  phrase_emb_dim: int = 0, senti_emb_dim: int = 0, max_length: int = 0, num_classes: int = None,
                  dataset: str = None, num_freeze_layers: int = 0, freeze_epochs=-1, neg_weight=1,
```

### Comparing `multi_emotion-0.1.14/multi_emotion/utils/conf.py` & `multi_emotion-0.1.3/src/utils/conf.py`

 * *Files identical despite different names*

### Comparing `multi_emotion-0.1.14/multi_emotion/utils/data.py` & `multi_emotion-0.1.3/src/utils/data.py`

 * *Files identical despite different names*

### Comparing `multi_emotion-0.1.14/multi_emotion/utils/logging.py` & `multi_emotion-0.1.3/src/utils/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import getpass, socket
 from typing import Any, List
 import torch
 from lightning_utilities.core.rank_zero import rank_zero_only
-from lightning.pytorch.loggers import CSVLogger
-from multi_emotion.utils.metrics import get_step_metrics, get_epoch_metrics
+from omegaconf.dictconfig import DictConfig
+from omegaconf.omegaconf import OmegaConf
+from lightning.pytorch.loggers import NeptuneLogger, CSVLogger
+from src.utils.metrics import get_step_metrics, get_epoch_metrics
+from dotenv import load_dotenv
 import logging
-
+load_dotenv(override=True)
 
 
 log = logging.getLogger(__name__)
 
 def get_username():
     return getpass.getuser()
 
@@ -27,59 +30,92 @@
 
 def get_logger(name=__name__, level=logging.INFO) -> logging.Logger:
     logger = logging.getLogger(name)
     logger.setLevel(level)
     return logger
 
 def get_csv_logger(
-    cfg, logger, save_dir, name, offline
+    cfg: DictConfig, logger:str, save_dir: str, name: str, offline: bool
 ):
     csv_logger = CSVLogger(
         save_dir=save_dir,
         name=name
     )
 
     return csv_logger
 
 
+def get_neptune_logger(
+    cfg: DictConfig,
+    tag_attrs: List[str], log_db: str,
+    api_key: str, project_name: str,
+    offline: bool, logger: str,
+):
+
+    args_dict = {
+        **flatten_cfg(OmegaConf.to_object(cfg)),
+        "hostname": socket.gethostname()
+    }
+    tags = tag_attrs
+    if cfg.model.expl_reg:
+        tags.append('expl_reg')
+
+    tags.append(log_db)
+
+    neptune_logger = NeptuneLogger(
+        api_key=api_key,
+        project_name=project_name,
+        # name="Prediction model",
+        params=args_dict,
+        tags=tags,
+        offline_mode=offline,
+    )
+
+    try:
+        # for unknown reason, must access this field otherwise becomes None
+        print(neptune_logger.experiment)
+    except BaseException:
+        pass
+
+    return neptune_logger
 
-def log_data_to_model(model_class, data, data_name, data_type, suffix, split, ret_dict=None, detach_data=True):
+def log_data_to_neptune(model_class, data, data_name, data_type, suffix, split, ret_dict=None, detach_data=True):
 
     data_key = 'loss' if f'{data_name}_{data_type}' == 'total_loss' else f'{data_name}_{data_type}'
     model_class.log(f'{split}_{data_key}_{suffix}', data.detach(), prog_bar=True, sync_dist=(split != 'train'))
     if ret_dict is not None:
         ret_dict[data_key] = data.detach() if detach_data else data
     
     return ret_dict
 
 def log_step_losses(model_class, loss_dict, ret_dict, split):
-    ret_dict = log_data_to_model(model_class, loss_dict['loss'], 'total', 'loss', 'step', split, ret_dict, detach_data=False)
+    ret_dict = log_data_to_neptune(model_class, loss_dict['loss'], 'total', 'loss', 'step', split, ret_dict, detach_data=False)
     return ret_dict
 
 
 def log_epoch_losses(model_class, outputs, split):
     loss = outputs['loss'].mean()
-    log_data_to_model(model_class, loss, 'total', 'loss', 'epoch', split, ret_dict=None)
+    log_data_to_neptune(model_class, loss, 'total', 'loss', 'epoch', split, ret_dict=None)
 
 def log_epoch_metrics(model_class, outputs, split):
     probs = outputs['probs']
     targets = outputs['targets']
     get_step_metrics(probs, targets, model_class.perf_metrics)
     perf_metrics = get_epoch_metrics(model_class.perf_metrics)
 
-    log_data_to_model(model_class, perf_metrics['acc'], 'acc', 'metric', 'epoch', split, ret_dict=None)
-    log_data_to_model(model_class, perf_metrics['macro_f1'], 'macro_f1', 'metric', 'epoch', split, ret_dict=None)
+    log_data_to_neptune(model_class, perf_metrics['acc'], 'acc', 'metric', 'epoch', split, ret_dict=None)
+    log_data_to_neptune(model_class, perf_metrics['macro_f1'], 'macro_f1', 'metric', 'epoch', split, ret_dict=None)
 
     if model_class.num_classes == 2:
-        log_data_to_model(model_class, perf_metrics['binary_f1'], 'binary_f1', 'metric', 'epoch', split, ret_dict=None)
+        log_data_to_neptune(model_class, perf_metrics['binary_f1'], 'binary_f1', 'metric', 'epoch', split, ret_dict=None)
 
 
     if 'delta' in outputs.keys():
         delta = torch.abs(outputs['delta']).mean()
-        log_data_to_model(model_class, delta, 'convergence_delta', 'metric', 'epoch', split, ret_dict=None)
+        log_data_to_neptune(model_class, delta, 'convergence_delta', 'metric', 'epoch', split, ret_dict=None)
 
 @rank_zero_only
 def log_hyperparameters(object_dict: dict) -> None:
     """Controls which config parts are saved by lightning loggers.
 
     Additionally saves:
     - Number of model parameters
```

### Comparing `multi_emotion-0.1.14/multi_emotion/utils/metrics.py` & `multi_emotion-0.1.3/src/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `multi_emotion-0.1.14/multi_emotion/utils/optim.py` & `multi_emotion-0.1.3/src/utils/optim.py`

 * *Files identical despite different names*

### Comparing `multi_emotion-0.1.14/multi_emotion/utils/utils.py` & `multi_emotion-0.1.3/src/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import random
 from collections import Counter
 
 import emotlib
 import numpy as np
 from tqdm import tqdm
 
-from multi_emotion.utils.data import dataset_info, data_keys
+from src.utils.data import dataset_info, data_keys
 import pandas as pd
 
 def nrc_hashtag_lexicon(nrc_lexicon):
     hashtag_vocab = []
     for nl in nrc_lexicon:
         hashtag_vocab.append(nl.split('\t')[1].replace("#", ""))
     return hashtag_vocab
```

### Comparing `multi_emotion-0.1.14/multi_emotion.egg-info/PKG-INFO` & `multi_emotion-0.1.3/src/multi_emotion.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 Metadata-Version: 2.1
-Name: multi_emotion
-Version: 0.1.14
+Name: multi-emotion
+Version: 0.1.3
 Summary: detect multiple emotions in a sentence including [anger, anticipation, disgust, fear, joy, love, optimism, pessimism, sadness,                    surprise, trust]
 Home-page: https://github.com/JinfenLi/multi_emotion_recognition
 Author: Jinfen Li
 Author-email: jli284@syr.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-Requires-Dist: lightning>=2
-Requires-Dist: emotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: rich
-Requires-Dist: torchmetrics>=1
-Requires-Dist: tqdm
-Requires-Dist: transformers==4.31.0
 
 # Multi-emotion Recognition Using Multi-EmoBERT and Emotion Analysis in Fake News
 
 This is the official PyTorch [repo](https://github.com/JinfenLi/multi_emotion_recognition) for [Multi-EmoBERT](https://dl.acm.org/doi/abs/10.1145/3578503.3583595), a learning framework for multi-emotion recognition.
 
 ```
 Multi-emotion Recognition Using Multi-EmoBERT and Emotion Analysis in Fake News
@@ -40,22 +32,22 @@
   pages={128--135},
   year={2023}
 }
 ```
 ## Usage via Pip Package
 install pip package
 ```
-pip install multi-emotion==0.1.12
+pip install multi-emotion
 ```
 use pip package
 ```
-from multi_emotion import multi_emotion
+import multi_emotion
 multi_emotion.predict(["I am so happy today"])
 ```
-preview result
+result preview
 ```
 [{'text': 'i am so happy today', 'pred_label': 'joy,love,optimism', 'probability': '[{"anger": 0.00022063202050048858}, {"anticipation": 0.007108359131962061}, {"disgust": 0.0006860275752842426}, {"fear": 0.00044393239659257233}, {"joy": 0.9998739957809448}, {"love": 0.8244059085845947}, {"optimism": 0.931083083152771}, {"pessimism": 0.0002464792341925204}, {"sadness": 0.007342423778027296}, {"surprise": 0.001668739365413785}, {"trust": 0.009098367765545845}]'}]
 
 ```
```

### Comparing `multi_emotion-0.1.14/setup.py` & `multi_emotion-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="multi_emotion",
-    version='0.1.14',
+    version='0.1.3',
 
     description="detect multiple emotions in a sentence including [anger, anticipation, disgust, fear, joy, love, optimism, pessimism, sadness,\
                     surprise, trust]",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jinfen Li",
     author_email="jli284@syr.edu",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         'Programming Language :: Python :: 3.9'
     ],
     url="https://github.com/JinfenLi/multi_emotion_recognition",
     license="MIT",
-    install_requires=["lightning>=2",
+    install_requires=["lightning>=2","torch>=2",
                       "emotlib",
                       "numpy", "pandas", "rich", "torchmetrics>=1",
                       "tqdm",
                       "transformers==4.31.0"],
-    packages=find_packages(),
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
 
 
 )
```

