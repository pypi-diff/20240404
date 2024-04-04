# Comparing `tmp/birdset-0.1.0.tar.gz` & `tmp/birdset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdset-0.1.0.tar", max compression
+gzip compressed data, was "birdset-0.1.1.tar", max compression
```

## Comparing `birdset-0.1.0.tar` & `birdset-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0     6816 2024-03-18 15:43:26.353722 birdset-0.1.0/README.md
--rw-r--r--   0        0        0       21 2024-03-13 13:04:08.967605 birdset-0.1.0/birdset/__init__.py
--rw-r--r--   0        0        0       83 2024-03-13 13:04:08.971605 birdset-0.1.0/birdset/callbacks/__init__.py
--rw-r--r--   0        0        0      416 2024-03-13 13:04:08.971605 birdset-0.1.0/birdset/callbacks/metric_collector.py
--rw-r--r--   0        0        0      731 2024-03-13 13:04:08.971605 birdset-0.1.0/birdset/callbacks/timetracker.py
--rw-r--r--   0        0        0      150 2024-03-18 15:42:48.527324 birdset-0.1.0/birdset/datamodule/__init__.py
--rw-r--r--   0        0        0    22392 2024-03-18 15:42:48.531324 birdset-0.1.0/birdset/datamodule/base_datamodule.py
--rw-r--r--   0        0        0     6911 2024-03-18 16:06:01.420493 birdset-0.1.0/birdset/datamodule/birdset_datamodule.py
--rw-r--r--   0        0        0      139 2024-03-13 13:04:08.979604 birdset-0.1.0/birdset/datamodule/components/__init__.py
--rw-r--r--   0        0        0    47815 2024-03-13 13:04:08.979604 birdset-0.1.0/birdset/datamodule/components/augmentations.py
--rw-r--r--   0        0        0     1620 2024-03-13 13:04:08.979604 birdset-0.1.0/birdset/datamodule/components/bird_premapping.py
--rw-r--r--   0        0        0     2906 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/datamodule/components/calculate_normalization_parameters.py
--rw-r--r--   0        0        0     4520 2024-03-13 13:04:08.983604 birdset-0.1.0/birdset/datamodule/components/event_decoding.py
--rw-r--r--   0        0        0     6247 2024-03-13 13:04:08.987604 birdset-0.1.0/birdset/datamodule/components/event_mapping.py
--rw-r--r--   0        0        0     2344 2024-03-13 13:04:08.987604 birdset-0.1.0/birdset/datamodule/components/feature_extraction.py
--rw-r--r--   0        0        0     4164 2024-03-13 13:04:08.987604 birdset-0.1.0/birdset/datamodule/components/resize.py
--rw-r--r--   0        0        0    23881 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/datamodule/components/tests/test_augmentations.py
--rw-r--r--   0        0        0    19800 2024-03-18 15:42:48.531324 birdset-0.1.0/birdset/datamodule/components/transforms.py
--rw-r--r--   0        0        0     1406 2024-03-18 15:42:48.527324 birdset-0.1.0/birdset/datamodule/esc50_datamodule.py
--rw-r--r--   0        0        0     4364 2024-03-18 15:42:48.527324 birdset-0.1.0/birdset/datamodule/pretrain_datamodule.py
--rw-r--r--   0        0        0    20304 2024-03-18 16:29:43.915005 birdset-0.1.0/birdset/datamodule/subset_datamodules.py
--rw-r--r--   0        0        0     4585 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/main.py
--rw-r--r--   0        0        0      130 2024-03-13 13:04:09.003603 birdset-0.1.0/birdset/modules/__init__,py
--rw-r--r--   0        0        0    13972 2024-03-19 15:19:41.497738 birdset-0.1.0/birdset/modules/base_module.py
--rw-r--r--   0        0        0        0 2024-03-13 13:04:09.007603 birdset-0.1.0/birdset/modules/components/__init__.py
--rw-r--r--   0        0        0      118 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/modules/losses/__init__.py
--rw-r--r--   0        0        0     3572 2024-03-13 13:04:09.011603 birdset-0.1.0/birdset/modules/losses/asymmetric_loss.py
--rw-r--r--   0        0        0     2312 2024-03-13 13:04:09.011603 birdset-0.1.0/birdset/modules/losses/focal_loss.py
--rw-r--r--   0        0        0      890 2024-03-13 13:04:09.011603 birdset-0.1.0/birdset/modules/losses/loader.py
--rw-r--r--   0        0        0      457 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/modules/metrics/__init__.py
--rw-r--r--   0        0        0      935 2024-03-13 13:04:09.015603 birdset-0.1.0/birdset/modules/metrics/loader.py
--rw-r--r--   0        0        0     3331 2024-03-13 13:04:09.015603 birdset-0.1.0/birdset/modules/metrics/multiclass.py
--rw-r--r--   0        0        0     8013 2024-03-13 13:04:09.019603 birdset-0.1.0/birdset/modules/metrics/multilabel.py
--rw-r--r--   0        0        0      207 2024-03-13 13:04:09.019603 birdset-0.1.0/birdset/modules/models/__init__.py
--rw-r--r--   0        0        0     4095 2024-03-13 13:04:09.019603 birdset-0.1.0/birdset/modules/models/ast.py
--rw-r--r--   0        0        0    13191 2024-03-13 13:04:09.019603 birdset-0.1.0/birdset/modules/models/benchmark_models.py
--rw-r--r--   0        0        0     3849 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/modules/models/convnext.py
--rw-r--r--   0        0        0     7788 2024-03-13 13:04:09.023603 birdset-0.1.0/birdset/modules/models/eat_soundnet.py
--rw-r--r--   0        0        0     8356 2024-03-13 13:04:09.027602 birdset-0.1.0/birdset/modules/models/efficientnet.py
--rw-r--r--   0        0        0     3580 2024-03-13 13:04:09.027602 birdset-0.1.0/birdset/modules/models/hubert.py
--rw-r--r--   0        0        0     3685 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/modules/models/mobilenet.py
--rw-r--r--   0        0        0    10058 2024-03-13 13:04:09.031602 birdset-0.1.0/birdset/modules/models/perch.py
--rw-r--r--   0        0        0     4271 2024-03-13 13:04:09.035602 birdset-0.1.0/birdset/modules/models/resnet.py
--rw-r--r--   0        0        0     4017 2024-03-13 13:04:09.035602 birdset-0.1.0/birdset/modules/models/wav2vec2.py
--rw-r--r--   0        0        0     4727 2024-03-19 15:34:32.171517 birdset-0.1.0/birdset/modules/multilabel_module.py
--rw-r--r--   0        0        0      392 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/utils/__init__.py
--rw-r--r--   0        0        0     1209 2024-03-13 13:04:09.039602 birdset-0.1.0/birdset/utils/extras.py
--rw-r--r--   0        0        0     1837 2024-03-18 15:38:04.587394 birdset-0.1.0/birdset/utils/instantiate.py
--rw-r--r--   0        0        0     2069 2024-03-13 13:04:09.043602 birdset-0.1.0/birdset/utils/label_utils.py
--rw-r--r--   0        0        0      448 2024-03-13 13:04:09.043602 birdset-0.1.0/birdset/utils/pylogger.py
--rw-r--r--   0        0        0     2296 2024-03-18 15:38:04.591394 birdset-0.1.0/birdset/utils/rich_utils.py
--rw-r--r--   0        0        0     2150 2024-03-18 15:38:04.591394 birdset-0.1.0/birdset/utils/saving_utils.py
--rw-r--r--   0        0        0     4710 2024-03-18 15:38:04.591394 birdset-0.1.0/birdset/utils/utils.py
--rw-r--r--   0        0        0     1897 2024-03-20 09:21:49.503933 birdset-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8434 1970-01-01 00:00:00.000000 birdset-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7950 2024-03-26 14:15:22.824751 birdset-0.1.1/README.md
+-rw-r--r--   0        0        0       21 2024-03-26 14:15:22.824751 birdset-0.1.1/birdset/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-26 14:15:22.824751 birdset-0.1.1/birdset/callbacks/__init__.py
+-rw-r--r--   0        0        0      416 2024-03-26 14:15:22.828750 birdset-0.1.1/birdset/callbacks/metric_collector.py
+-rw-r--r--   0        0        0      731 2024-03-26 14:15:22.828750 birdset-0.1.1/birdset/callbacks/timetracker.py
+-rw-r--r--   0        0        0      150 2024-03-26 14:15:22.828750 birdset-0.1.1/birdset/datamodule/__init__.py
+-rw-r--r--   0        0        0    22387 2024-03-26 14:15:22.832750 birdset-0.1.1/birdset/datamodule/base_datamodule.py
+-rw-r--r--   0        0        0     6911 2024-03-26 14:15:22.832750 birdset-0.1.1/birdset/datamodule/birdset_datamodule.py
+-rw-r--r--   0        0        0      139 2024-03-26 14:15:22.832750 birdset-0.1.1/birdset/datamodule/components/__init__.py
+-rw-r--r--   0        0        0    47815 2024-03-26 14:15:22.836750 birdset-0.1.1/birdset/datamodule/components/augmentations.py
+-rw-r--r--   0        0        0     1620 2024-03-26 14:15:22.836750 birdset-0.1.1/birdset/datamodule/components/bird_premapping.py
+-rw-r--r--   0        0        0     2906 2024-03-26 14:15:22.836750 birdset-0.1.1/birdset/datamodule/components/calculate_normalization_parameters.py
+-rw-r--r--   0        0        0     4520 2024-03-26 14:15:22.840750 birdset-0.1.1/birdset/datamodule/components/event_decoding.py
+-rw-r--r--   0        0        0     6247 2024-03-26 14:15:22.840750 birdset-0.1.1/birdset/datamodule/components/event_mapping.py
+-rw-r--r--   0        0        0     2344 2024-03-26 14:15:22.840750 birdset-0.1.1/birdset/datamodule/components/feature_extraction.py
+-rw-r--r--   0        0        0     4164 2024-03-26 14:15:22.844750 birdset-0.1.1/birdset/datamodule/components/resize.py
+-rw-r--r--   0        0        0    23881 2024-03-26 14:15:22.844750 birdset-0.1.1/birdset/datamodule/components/tests/test_augmentations.py
+-rw-r--r--   0        0        0    19800 2024-03-26 14:15:22.848749 birdset-0.1.1/birdset/datamodule/components/transforms.py
+-rw-r--r--   0        0        0     1406 2024-03-26 14:15:22.848749 birdset-0.1.1/birdset/datamodule/esc50_datamodule.py
+-rw-r--r--   0        0        0     4364 2024-03-26 14:15:22.852749 birdset-0.1.1/birdset/datamodule/pretrain_datamodule.py
+-rw-r--r--   0        0        0    20304 2024-03-26 14:15:22.852749 birdset-0.1.1/birdset/datamodule/subset_datamodules.py
+-rw-r--r--   0        0        0      130 2024-03-26 14:15:22.852749 birdset-0.1.1/birdset/modules/__init__,py
+-rw-r--r--   0        0        0      130 2024-03-26 14:15:22.856749 birdset-0.1.1/birdset/modules/__init__.py
+-rw-r--r--   0        0        0    14844 2024-04-04 14:18:31.392853 birdset-0.1.1/birdset/modules/base_module.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:15:22.856749 birdset-0.1.1/birdset/modules/components/__init__.py
+-rw-r--r--   0        0        0      118 2024-03-26 14:15:22.860749 birdset-0.1.1/birdset/modules/losses/__init__.py
+-rw-r--r--   0        0        0     3572 2024-03-26 14:15:22.860749 birdset-0.1.1/birdset/modules/losses/asymmetric_loss.py
+-rw-r--r--   0        0        0     2312 2024-03-26 14:15:22.860749 birdset-0.1.1/birdset/modules/losses/focal_loss.py
+-rw-r--r--   0        0        0      890 2024-03-26 14:15:22.864749 birdset-0.1.1/birdset/modules/losses/loader.py
+-rw-r--r--   0        0        0      457 2024-03-26 14:15:22.864749 birdset-0.1.1/birdset/modules/metrics/__init__.py
+-rw-r--r--   0        0        0      935 2024-03-26 14:15:22.864749 birdset-0.1.1/birdset/modules/metrics/loader.py
+-rw-r--r--   0        0        0     3331 2024-03-26 14:15:22.864749 birdset-0.1.1/birdset/modules/metrics/multiclass.py
+-rw-r--r--   0        0        0     8013 2024-03-26 14:15:22.868749 birdset-0.1.1/birdset/modules/metrics/multilabel.py
+-rw-r--r--   0        0        0      207 2024-03-26 14:15:22.868749 birdset-0.1.1/birdset/modules/models/__init__.py
+-rw-r--r--   0        0        0     4095 2024-03-26 14:15:22.868749 birdset-0.1.1/birdset/modules/models/ast.py
+-rw-r--r--   0        0        0    13191 2024-03-26 14:15:22.872748 birdset-0.1.1/birdset/modules/models/benchmark_models.py
+-rw-r--r--   0        0        0     3849 2024-03-26 14:15:22.872748 birdset-0.1.1/birdset/modules/models/convnext.py
+-rw-r--r--   0        0        0     7788 2024-03-26 14:15:22.872748 birdset-0.1.1/birdset/modules/models/eat_soundnet.py
+-rw-r--r--   0        0        0     8356 2024-03-26 14:15:22.876748 birdset-0.1.1/birdset/modules/models/efficientnet.py
+-rw-r--r--   0        0        0     3580 2024-03-26 14:15:22.876748 birdset-0.1.1/birdset/modules/models/hubert.py
+-rw-r--r--   0        0        0     3685 2024-03-26 14:15:22.876748 birdset-0.1.1/birdset/modules/models/mobilenet.py
+-rw-r--r--   0        0        0    10058 2024-03-26 14:15:22.880748 birdset-0.1.1/birdset/modules/models/perch.py
+-rw-r--r--   0        0        0     4271 2024-03-26 14:15:22.880748 birdset-0.1.1/birdset/modules/models/resnet.py
+-rw-r--r--   0        0        0     4017 2024-03-26 14:15:22.880748 birdset-0.1.1/birdset/modules/models/wav2vec2.py
+-rw-r--r--   0        0        0     4782 2024-03-26 14:15:22.884748 birdset-0.1.1/birdset/modules/multilabel_module.py
+-rw-r--r--   0        0        0     4479 2024-03-26 14:15:22.884748 birdset-0.1.1/birdset/train.py
+-rw-r--r--   0        0        0      392 2024-03-26 14:15:22.884748 birdset-0.1.1/birdset/utils/__init__.py
+-rw-r--r--   0        0        0     1209 2024-03-26 14:15:22.888748 birdset-0.1.1/birdset/utils/extras.py
+-rw-r--r--   0        0        0     1837 2024-03-26 14:15:22.888748 birdset-0.1.1/birdset/utils/instantiate.py
+-rw-r--r--   0        0        0     2069 2024-03-26 14:15:22.888748 birdset-0.1.1/birdset/utils/label_utils.py
+-rw-r--r--   0        0        0      448 2024-03-26 14:15:22.892747 birdset-0.1.1/birdset/utils/pylogger.py
+-rw-r--r--   0        0        0     2296 2024-03-26 14:15:22.892747 birdset-0.1.1/birdset/utils/rich_utils.py
+-rw-r--r--   0        0        0     2150 2024-03-26 14:15:22.892747 birdset-0.1.1/birdset/utils/saving_utils.py
+-rw-r--r--   0        0        0     4710 2024-03-26 14:15:22.892747 birdset-0.1.1/birdset/utils/utils.py
+-rw-r--r--   0        0        0     1787 2024-04-04 14:19:01.351654 birdset-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9568 1970-01-01 00:00:00.000000 birdset-0.1.1/PKG-INFO
```

### Comparing `birdset-0.1.0/README.md` & `birdset-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Results
 | <sub>Title</sub> | <sub>Notes</sub> |<sub>PER</sub> | <sub>NES</sub> | <sub>UHH</sub> | <sub>HSN</sub> | <sub>NBP</sub> | <sub>POW</sub> | <sub>SSW</sub> | <sub>SNE</sub>  | <sub>Overall</sub> | <sub>Code</sub> |
 | :----| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
 | <sub>**BirdSet: A Multi-Task Benchmark For Classification In Avian Bioacoustics**</sub> | | | | | | | |
 | <sub>**BIRB: A Generalization Benchmark for Information Retrieval in Bioacoustics**</sub> | | | | | | | | 
 
-## Setup
+## Get Started
 
 ### Devcontainer
 
 You can use the [devcontainer](https://code.visualstudio.com/docs/devcontainers/containers) configured as as git submodule:
 ```bash
 git submodule update --init --recursive
 ```
@@ -21,19 +21,22 @@
 ```
 conda create -n birdset python=3.10
 pip install -e .
 ```
 
 Or [poetry](https://python-poetry.org/).
 ```
-mv pyproject.poetry pyproject.toml
 poetry install
 poetry shell
 ```
 
+
+
+# Minimal Working Example
+
 ## Log in to Huggingface
 
 Our datasets are shared via HuggingFace Datasets in our [HuggingFace BirdSet repository](https://huggingface.co/datasets/DBD-research-group/birdset_v1). Huggingface is a central hub for sharing and utilizing datasets and models, particularly beneficial for machine learning and data science projects. For accessing private datasets hosted on HuggingFace, you need to be authenticated. Here's how you can log in to HuggingFace:
 
 1. **Install HuggingFace CLI**: If you haven't already, you need to install the HuggingFace CLI (Command Line Interface). This tool enables you to interact with HuggingFace services directly from your terminal. You can install it using pip:
 
    ```bash
@@ -43,15 +46,65 @@
 2. **Login via CLI**: Once the HuggingFace CLI is installed, you can log in to your HuggingFace account directly from your terminal. This step is essential for accessing private datasets or contributing to the HuggingFace community. Use the following command:
 
    ```bash
    huggingface-cli login
    ```
 
    After executing this command, you'll be prompted to enter your HuggingFace credentials ([User Access Token](https://huggingface.co/docs/hub/security-tokens)). Once authenticated, your credentials will be saved locally, allowing seamless access to HuggingFace resources.
+   
+## Prepare Data
+
+```
+from birdset.datamodule.base_datamodule import DatasetConfig
+from birdset.datamodule.birdset_datamodule import BirdSetDataModule
+
+# initiate the data module
+dm = BirdSetDataModule(
+    dataset= DatasetConfig(
+        data_dir='../../data_birdset/HSN',
+        dataset_name='HSN',
+        hf_path='DBD-research-group/BirdSet',
+        hf_name='HSN',
+        n_classes=21,
+        n_workers=3,
+        val_split=0.2,
+        task="multilabel",
+        classlimit=500,
+        eventlimit=5,
+        sampling_rate=32000,
+    ),
+)
+
+# prepare the data (download dataset, ...)
+dm.prepare_data()
 
+# setup the dataloaders
+dm.setup(stage="fit")
+
+# get the dataloaders
+train_loader = dm.train_dataloader()
+```
+
+## Prepare Model and Start Training
+
+```
+from lightning import Trainer
+min_epochs = 1
+max_epochs = 5
+trainer = Trainer(min_epochs=min_epochs, max_epochs=max_epochs, accelerator="gpu", devices=1)
+
+from birdset.modules.base_module import BaseModule
+model = BaseModule(
+    len_trainset=dm.len_trainset,
+    task=dm.task,
+    batch_size=dm.train_batch_size,
+    num_epochs=max_epochs)
+
+trainer.fit(model, dm)
+```
 
 ## Logging
 Logs will be written to [Weights&Biases](https://wandb.ai/) by default.
 
 ## Background noise
 To enhance model performance we mix in additional background noise from downloaded from the [DCASE18](https://dcase.community/challenge2018/index). To download the files and convert them to the correct format, run the notebook 'download_background_noise.ipynb' in the 'notebooks' folder.
```

### Comparing `birdset-0.1.0/birdset/callbacks/timetracker.py` & `birdset-0.1.1/birdset/callbacks/timetracker.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/base_datamodule.py` & `birdset-0.1.1/birdset/datamodule/base_datamodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         Args:
             dataset (DatasetDict): A Hugging Face `datasets.DatasetDict` object containing the dataset splits.
             size (int, optional): The number of examples to select from each split. Default is 500.
 
         Returns:
             DatasetDict: The subsetted dataset. The keys are the names of the dataset splits and the values are the subsetted datasets.
         """
-        for split in dataset.keys():
+        for split in ["train"]:
             random_indices = random.sample(range(len(dataset[split])), size)
             dataset[split] = dataset[split].select(random_indices)
         return dataset
     
  
     def _get_dataset(self, split):
         """
```

### Comparing `birdset-0.1.0/birdset/datamodule/birdset_datamodule.py` & `birdset-0.1.1/birdset/datamodule/birdset_datamodule.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/augmentations.py` & `birdset-0.1.1/birdset/datamodule/components/augmentations.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/bird_premapping.py` & `birdset-0.1.1/birdset/datamodule/components/bird_premapping.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/calculate_normalization_parameters.py` & `birdset-0.1.1/birdset/datamodule/components/calculate_normalization_parameters.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/event_decoding.py` & `birdset-0.1.1/birdset/datamodule/components/event_decoding.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/event_mapping.py` & `birdset-0.1.1/birdset/datamodule/components/event_mapping.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/feature_extraction.py` & `birdset-0.1.1/birdset/datamodule/components/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/resize.py` & `birdset-0.1.1/birdset/datamodule/components/resize.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/tests/test_augmentations.py` & `birdset-0.1.1/birdset/datamodule/components/tests/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/components/transforms.py` & `birdset-0.1.1/birdset/datamodule/components/transforms.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/esc50_datamodule.py` & `birdset-0.1.1/birdset/datamodule/esc50_datamodule.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/pretrain_datamodule.py` & `birdset-0.1.1/birdset/datamodule/pretrain_datamodule.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/datamodule/subset_datamodules.py` & `birdset-0.1.1/birdset/datamodule/subset_datamodules.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/main.py` & `birdset-0.1.1/birdset/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 import lightning as L 
 from omegaconf import OmegaConf
 import json
 from birdset import utils
 import pyrootutils 
 
 log = utils.get_pylogger(__name__)
-#rootutils.setup_root(__file__, indicator=".project-root", pythonpath=True)
+
 root = pyrootutils.setup_root(
     search_from=__file__,
     indicator=[".git"],
     pythonpath=True,
     dotenv=True,
 )
 
 _HYDRA_PARAMS = {
     "version_base":None,
-    #"config_path": "../configs",
     "config_path": str(root / "configs"),
-    "config_name": "main.yaml"
+    "config_name": "train.yaml"
 }
 
 # @utils.register_custom_resolvers(**_HYDRA_PARAMS)
 @hydra.main(**_HYDRA_PARAMS)
-def main(cfg):
+def train(cfg):
     log.info('Using config: \n%s', OmegaConf.to_yaml(cfg))
 
     log.info(f"Dataset path: <{os.path.abspath(cfg.paths.dataset_path)}>")
     os.makedirs(cfg.paths.dataset_path, exist_ok=True)
 
     log.info(f"Log path: <{os.path.abspath(cfg.paths.log_dir)}>")
     os.makedirs(cfg.paths.log_dir, exist_ok=True)
@@ -134,8 +133,8 @@
         file_path = os.path.join(cfg.paths.output_dir, "finalmetrics.json")
         with open(file_path, 'w') as json_file:
             json.dump(metric_dict, json_file)
     
     utils.close_loggers()
 
 if __name__ == "__main__":    
-    main()
+    train()
```

### Comparing `birdset-0.1.0/birdset/modules/base_module.py` & `birdset-0.1.1/birdset/modules/base_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass, field, asdict
 from functools import partial
-from typing import Callable, Dict, Literal, Type, Optional
+from typing import Callable, Dict, List, Literal, Type, Optional, Union
 
 from birdset.modules.metrics.multilabel import TopKAccuracy, cmAP, cmAP5, mAP, pcmAP
 from birdset.modules.models.efficientnet import EfficientNetClassifier
 import torch
 import math
 import hydra
 
@@ -15,14 +15,32 @@
 import torch.nn as nn
 from torch.nn import BCEWithLogitsLoss
 from torch.nn.modules.loss import _Loss
 from torch.optim import AdamW, Optimizer, lr_scheduler 
 from transformers import get_scheduler, SchedulerType
 from torchmetrics import AUROC, Metric, MaxMetric, MetricCollection
 
+def get_num_gpu(num_gpus: Union[int|str|List[int]]) -> int:
+    """
+    Returns the number of GPU`s infered from lightnings trainer devices argument.
+    https://lightning.ai/docs/pytorch/stable/api/lightning.pytorch.trainer.trainer.Trainer.html#lightning.pytorch.trainer.trainer.Trainer
+    """
+     # check if num_gpus is a list
+    if not isinstance(num_gpus, int) and not isinstance(num_gpus, str):
+        return len(num_gpus)
+    elif isinstance(num_gpus, str):
+        if num_gpus == "auto" or num_gpus == "-1":
+            return torch.cuda.device_count()
+        elif len(num_gpus.split(",")) > 1:
+            return len(num_gpus.split(",")) 
+        else:
+            return int(num_gpus)
+    else:    
+        return num_gpus
+
 @dataclass
 class NetworkConfig:
     """
     A dataclass for configuring a neural network model for training.
 
     Attributes:
         model (nn.Module): The model to be used for training. Defaults to an instance of `EfficientNetClassifier`.
@@ -43,25 +61,25 @@
     model_type: Literal['vision', 'waveform'] = "vision"
     torch_compile: bool = False
     sample_rate: int = 32000
     normalize_waveform: bool = False
     normalize_spectrogram: bool = True
 
 
-@dataclass
-class LRSchedulerExtrasConfig:
-    """
-    A dataclass for configuring the extras of the learning rate scheduler.
-
-    Attributes:
-        interval (str): The interval at which the scheduler performs its step. Defaults to "step".
-        warmup_ratio (float): The ratio of warmup steps to total steps. Defaults to 0.5.
-    """
-    interval: str = "step"
-    warmup_ratio: float = 0.5
+# @dataclass
+# class LRSchedulerExtrasConfig:
+#     """
+#     A dataclass for configuring the extras of the learning rate scheduler.
+
+#     Attributes:
+#         interval (str): The interval at which the scheduler performs its step. Defaults to "step".
+#         warmup_ratio (float): The ratio of warmup steps to total steps. Defaults to 0.5.
+#     """
+#     interval: str = "step"
+#     warmup_ratio: float = 0.05
 
 
 @dataclass
 class LRSchedulerConfig:
     """
     A dataclass for configuring the learning rate scheduler.
 
@@ -73,63 +91,73 @@
         get_scheduler,
         name = "cosine",
         scheduler_specific_kwargs = {
             'num_cycles': 0.5,
             'last_epoch': -1,
         }
     )
-    extras: LRSchedulerExtrasConfig = LRSchedulerExtrasConfig()
 
+    interval: str = "step"
+    warmup_ratio: float = 0.05
 
-@dataclass
+    #extras: LRSchedulerExtrasConfig = LRSchedulerExtrasConfig()
+    
 class MetricsConfig:
     """
-    A dataclass for configuring the metrics used during model training and evaluation.
+    A class for configuring the metrics used during model training and evaluation.
 
     Attributes:
-        main_metric (Metric): The main metric used for model training. Defaults to an instance of `cmAP`.
-        val_metric_best (Metric): The metric used for model validation. Defaults to an instance of `MaxMetric`.
-        add_metrics (MetricCollection): A collection of additional metrics used during model training. 
-            Defaults to a `MetricCollection` with 'MultilabelAUROC', 'T1Accuracy', 'T3Accuracy', and 'mAP'.
-        eval_complete (MetricCollection): A collection of metrics used during model evaluation. 
-            Defaults to a `MetricCollection` with 'cmAP5' and 'pcmAP'.
-    """
-    main_metric: Metric = cmAP(
-        num_labels = 21,
-        thresholds = None
-    )
-    val_metric_best: Metric = MaxMetric()
-    add_metrics: MetricCollection  = MetricCollection(
-        metrics ={
-        'MultilabelAUROC': AUROC(
-            task="multilabel",
-            num_labels=21,
-            average='macro',
-            thresholds=None
-        ),
-        'T1Accuracy': TopKAccuracy(topk= 1),
-        'T3Accuracy': TopKAccuracy(topk= 3),
-        'mAP': mAP(
-            num_labels= 21,
-            thresholds=None
-        )  
-    })
-    eval_complete: MetricCollection = MetricCollection({
-        'cmAP5': cmAP5(
-            num_labels=21,
-            sample_threshold=5,
-            thresholds=None
-        ),
-        'pcmAP': pcmAP(
-            num_labels=21,
-            padding_factor=5,
-            average="macro",
+        main_metric (Metric): The main metric used for model training.
+        val_metric_best (Metric): The metric used for model validation.
+        add_metrics (MetricCollection): A collection of additional metrics used during model training.
+        eval_complete (MetricCollection): A collection of metrics used during model evaluation.
+    """
+
+    def __init__(
+        self,
+        num_labels: int = 21,
+    ):
+        """
+        Initializes the MetricsConfig class.
+
+        Args:
+            num_labels (int): The number of labels in the dataset. Defaults to 21 as in the HSN dataset.
+        """
+        self.main_metric: Metric = cmAP(
+            num_labels=num_labels,
             thresholds=None
         )
-    })
+        self.val_metric_best: Metric = MaxMetric()
+        self.add_metrics: MetricCollection = MetricCollection({
+            'MultilabelAUROC': AUROC(
+                task="multilabel",
+                num_labels=num_labels,
+                average='macro',
+                thresholds=None
+            ),
+            'T1Accuracy': TopKAccuracy(topk= 1),
+            'T3Accuracy': TopKAccuracy(topk= 3),
+            'mAP': mAP(
+                num_labels= 21,
+                thresholds=None
+            )  
+        })
+        self.eval_complete: MetricCollection = MetricCollection({
+            'cmAP5': cmAP5(
+                num_labels=num_labels,
+                sample_threshold=5,
+                thresholds=None
+            ),
+            'pcmAP': pcmAP(
+                num_labels=num_labels,
+                padding_factor=5,
+                average="macro",
+                thresholds=None
+            )
+        })
 
 @dataclass
 class LoggingParamsConfig:
     """
     A dataclass for configuring the logging parameters during model training.
 
     Attributes:
@@ -140,16 +168,14 @@
     """
     on_step: bool = False
     on_epoch: bool = True
     sync_dist: bool = False
     prog_bar: bool = True         
 
 
-
-
 class BaseModule(L.LightningModule):
     """
     BaseModule is a PyTorch Lightning module that serves as a base for all models.
 
     Attributes:
         network (NetworkConfig): Configuration for the network.
         output_activation (Callable): The output activation function.
@@ -192,25 +218,24 @@
         self.network = network
         self.output_activation = output_activation
         # TODO: refactor load_loss
         # self.loss = load_loss(loss, class_weights_loss, label_counts)
         self.loss = loss
         self.optimizer = optimizer
         self.lr_scheduler = lr_scheduler
+        self.warmup_ratio = 0.05
         self.metrics = metrics
         self.logging_params = logging_params
 
         # partial
         self.num_epochs = num_epochs
         self.batch_size = batch_size
         self.len_trainset = len_trainset
         self.task = task
-        self.num_gpus = num_gpus
-
-
+        self.num_gpus = get_num_gpu(num_gpus)
 
         self.model = self.network.model
 
         # configure main metric
         self.train_metric = self.metrics.main_metric.clone()
         self.valid_metric = self.metrics.main_metric.clone()
         self.test_metric = self.metrics.main_metric.clone()
@@ -245,25 +270,30 @@
 
     def configure_optimizers(self):
         self.optimizer = self.optimizer(self.model.parameters())
         if self.lr_scheduler is not None:
             # TODO: Handle the case when we do not want warmup
             num_training_steps = math.ceil((self.num_epochs * self.len_trainset) / self.batch_size * self.num_gpus)
             num_warmup_steps = math.ceil(
-                    num_training_steps * self.lr_scheduler.extras.warmup_ratio
+                    num_training_steps * self.lr_scheduler.warmup_ratio
                 )
             # TODO: Handle the case when drop_last=True more explicitly   
 
             self.scheduler = self.lr_scheduler.scheduler(
                 optimizer=self.optimizer,
                 num_training_steps=num_training_steps,
                 num_warmup_steps=num_warmup_steps,
             )
 
-            return {"optimizer": self.optimizer, "lr_scheduler": self.scheduler}
+            scheduler_dict = {
+                "scheduler": self.scheduler,
+                "interval": self.lr_scheduler.interval,
+                "warmup_ratio":self.lr_scheduler.warmup_ratio}                      
+
+            return {"optimizer": self.optimizer, "lr_scheduler": scheduler_dict}
 
         return {"optimizer": self.optimizer}
 
     def model_step(self, batch, batch_idx):
         logits = self.forward(**batch)
         if self.class_mask:
             logits = logits[:, self.class_mask]
@@ -280,29 +310,21 @@
             f"train/{self.loss.__class__.__name__}",
             train_loss,
             on_step=True,
             on_epoch=True,
             prog_bar=True
         )
 
-        # additionaly log "train/loss" to have a fixed loss name to monitor
-        self.log(
-            f"train/loss",
-            train_loss,
-            on_step=True,
-            on_epoch=True,
-            prog_bar=False
-        )
-
-        self.train_metric(preds, targets.int())
-        self.log(
-            f"train/{self.train_metric.__class__.__name__}",
-            self.train_metric,
-            **asdict(self.logging_params)
-        )
+        # remove metrics from train to significantly improve training time for many classes
+        # self.train_metric(preds, targets.int())
+        # self.log(
+        #     f"train/{self.train_metric.__class__.__name__}",
+        #     self.train_metric,
+        #     **asdict(self.logging_params)
+        # )
 
         # self.train_add_metrics(preds, targets)
         # self.log_dict(self.train_add_metrics, **self.logging_params)
 
         return {"loss": train_loss}
 
     def validation_step(self, batch, batch_idx):
@@ -312,23 +334,14 @@
             f"val/{self.loss.__class__.__name__}",
             val_loss,
             on_step=True,
             on_epoch=True,
             prog_bar=True
         )
 
-        # additionaly log "val/loss" to have a fixed loss name to monitor
-        self.log(
-            f"val/loss",
-            val_loss,
-            on_step=True,
-            on_epoch=True,
-            prog_bar=False
-        )
-
         self.valid_metric(preds, targets.int())
         self.log(
             f"val/{self.valid_metric.__class__.__name__}",
             self.valid_metric,
             **asdict(self.logging_params),
         )
```

### Comparing `birdset-0.1.0/birdset/modules/losses/asymmetric_loss.py` & `birdset-0.1.1/birdset/modules/losses/asymmetric_loss.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/losses/focal_loss.py` & `birdset-0.1.1/birdset/modules/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/losses/loader.py` & `birdset-0.1.1/birdset/modules/losses/loader.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/metrics/loader.py` & `birdset-0.1.1/birdset/modules/metrics/loader.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/metrics/multiclass.py` & `birdset-0.1.1/birdset/modules/metrics/multiclass.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/metrics/multilabel.py` & `birdset-0.1.1/birdset/modules/metrics/multilabel.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/ast.py` & `birdset-0.1.1/birdset/modules/models/ast.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/benchmark_models.py` & `birdset-0.1.1/birdset/modules/models/benchmark_models.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/convnext.py` & `birdset-0.1.1/birdset/modules/models/convnext.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/eat_soundnet.py` & `birdset-0.1.1/birdset/modules/models/eat_soundnet.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/efficientnet.py` & `birdset-0.1.1/birdset/modules/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/hubert.py` & `birdset-0.1.1/birdset/modules/models/hubert.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/mobilenet.py` & `birdset-0.1.1/birdset/modules/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/perch.py` & `birdset-0.1.1/birdset/modules/models/perch.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/resnet.py` & `birdset-0.1.1/birdset/modules/models/resnet.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/models/wav2vec2.py` & `birdset-0.1.1/birdset/modules/models/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/modules/multilabel_module.py` & `birdset-0.1.1/birdset/modules/multilabel_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import asdict
 import torch
 from .base_module import BaseModule, NetworkConfig, LRSchedulerConfig, MetricsConfig, LoggingParamsConfig
 import wandb
 from typing import Callable, Literal, Type, Optional
 from torch.nn import BCEWithLogitsLoss
 from torch.nn.modules.loss import _Loss
 from torch.optim import AdamW, Optimizer
@@ -71,19 +72,19 @@
             prog_bar=True
         )
 
         self.test_metric(preds, targets.int())
         self.log(
             f"test/{self.test_metric.__class__.__name__}",
             self.test_metric,
-            **self.logging_params,
+            **asdict(self.logging_params),
         )
 
         self.test_add_metrics(preds, targets.int())
-        self.log_dict(self.test_add_metrics, **self.logging_params)
+        self.log_dict(self.test_add_metrics, **asdict(self.logging_params))
 
         return {"loss": test_loss, "preds": preds, "targets": targets}
     
     
     def on_test_epoch_end(self):
         test_targets = torch.cat(self.test_targets).int()
         test_preds = torch.cat(self.test_preds)
@@ -92,15 +93,15 @@
         log_dict = {}
 
         # Rename cmap to cmap5!
         for metric_name, metric in self.test_complete_metrics.named_children():
             value = metric(test_preds, test_targets)
             log_dict[f"test/{metric_name}"] = value
 
-        self.log_dict(log_dict, **self.logging_params)
+        self.log_dict(log_dict, **asdict(self.logging_params))
 
         if self.prediction_table:
             self._wandb_prediction_table(test_preds, test_targets)
 
 
     def _wandb_prediction_table(self, preds, targets):
         top5_values_preds, top5_indices_preds = preds.topk(dim=1, k=5, sorted=True)
```

### Comparing `birdset-0.1.0/birdset/utils/extras.py` & `birdset-0.1.1/birdset/utils/extras.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/utils/instantiate.py` & `birdset-0.1.1/birdset/utils/instantiate.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/utils/label_utils.py` & `birdset-0.1.1/birdset/utils/label_utils.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/utils/rich_utils.py` & `birdset-0.1.1/birdset/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/utils/saving_utils.py` & `birdset-0.1.1/birdset/utils/saving_utils.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/birdset/utils/utils.py` & `birdset-0.1.1/birdset/utils/utils.py`

 * *Files identical despite different names*

### Comparing `birdset-0.1.0/pyproject.toml` & `birdset-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "birdset"
-version = "0.1.0"
+version = "0.1.1"
 description = "BirdSet: A multi-task benchmark and data pipeline for deep learning based avian bioacoustics"
 authors = ["Lukas Rauch <lukas.rauch@uni-kassel.de>", "Raphael Schwinger <rsc@informatik.uni-kiel.de>", "Moritz Wirth <moritz.wirt@uni-kassel.de>", "Rene  Heinrich <rene.heinrich@iee.fraunhofer.de>", "Jonas Lange <jla@informatik.uni-kiel.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 scipy = "^1.11.3"
@@ -53,19 +53,15 @@
 mlflow = "^2.11.0"
 pydub = "^0.25.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.2"
 
-[[tool.poetry.source]]
-name = "pytorch"
-url = "https://download.pytorch.org/whl/cu121"
-priority = "explicit"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `birdset-0.1.0/PKG-INFO` & `birdset-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdset
-Version: 0.1.0
+Version: 0.1.1
 Summary: BirdSet: A multi-task benchmark and data pipeline for deep learning based avian bioacoustics
 Author: Lukas Rauch
 Author-email: lukas.rauch@uni-kassel.de
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -42,15 +42,15 @@
 
 ## Results
 | <sub>Title</sub> | <sub>Notes</sub> |<sub>PER</sub> | <sub>NES</sub> | <sub>UHH</sub> | <sub>HSN</sub> | <sub>NBP</sub> | <sub>POW</sub> | <sub>SSW</sub> | <sub>SNE</sub>  | <sub>Overall</sub> | <sub>Code</sub> |
 | :----| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
 | <sub>**BirdSet: A Multi-Task Benchmark For Classification In Avian Bioacoustics**</sub> | | | | | | | |
 | <sub>**BIRB: A Generalization Benchmark for Information Retrieval in Bioacoustics**</sub> | | | | | | | | 
 
-## Setup
+## Get Started
 
 ### Devcontainer
 
 You can use the [devcontainer](https://code.visualstudio.com/docs/devcontainers/containers) configured as as git submodule:
 ```bash
 git submodule update --init --recursive
 ```
@@ -61,19 +61,22 @@
 ```
 conda create -n birdset python=3.10
 pip install -e .
 ```
 
 Or [poetry](https://python-poetry.org/).
 ```
-mv pyproject.poetry pyproject.toml
 poetry install
 poetry shell
 ```
 
+
+
+# Minimal Working Example
+
 ## Log in to Huggingface
 
 Our datasets are shared via HuggingFace Datasets in our [HuggingFace BirdSet repository](https://huggingface.co/datasets/DBD-research-group/birdset_v1). Huggingface is a central hub for sharing and utilizing datasets and models, particularly beneficial for machine learning and data science projects. For accessing private datasets hosted on HuggingFace, you need to be authenticated. Here's how you can log in to HuggingFace:
 
 1. **Install HuggingFace CLI**: If you haven't already, you need to install the HuggingFace CLI (Command Line Interface). This tool enables you to interact with HuggingFace services directly from your terminal. You can install it using pip:
 
    ```bash
@@ -83,15 +86,65 @@
 2. **Login via CLI**: Once the HuggingFace CLI is installed, you can log in to your HuggingFace account directly from your terminal. This step is essential for accessing private datasets or contributing to the HuggingFace community. Use the following command:
 
    ```bash
    huggingface-cli login
    ```
 
    After executing this command, you'll be prompted to enter your HuggingFace credentials ([User Access Token](https://huggingface.co/docs/hub/security-tokens)). Once authenticated, your credentials will be saved locally, allowing seamless access to HuggingFace resources.
+   
+## Prepare Data
+
+```
+from birdset.datamodule.base_datamodule import DatasetConfig
+from birdset.datamodule.birdset_datamodule import BirdSetDataModule
+
+# initiate the data module
+dm = BirdSetDataModule(
+    dataset= DatasetConfig(
+        data_dir='../../data_birdset/HSN',
+        dataset_name='HSN',
+        hf_path='DBD-research-group/BirdSet',
+        hf_name='HSN',
+        n_classes=21,
+        n_workers=3,
+        val_split=0.2,
+        task="multilabel",
+        classlimit=500,
+        eventlimit=5,
+        sampling_rate=32000,
+    ),
+)
+
+# prepare the data (download dataset, ...)
+dm.prepare_data()
 
+# setup the dataloaders
+dm.setup(stage="fit")
+
+# get the dataloaders
+train_loader = dm.train_dataloader()
+```
+
+## Prepare Model and Start Training
+
+```
+from lightning import Trainer
+min_epochs = 1
+max_epochs = 5
+trainer = Trainer(min_epochs=min_epochs, max_epochs=max_epochs, accelerator="gpu", devices=1)
+
+from birdset.modules.base_module import BaseModule
+model = BaseModule(
+    len_trainset=dm.len_trainset,
+    task=dm.task,
+    batch_size=dm.train_batch_size,
+    num_epochs=max_epochs)
+
+trainer.fit(model, dm)
+```
 
 ## Logging
 Logs will be written to [Weights&Biases](https://wandb.ai/) by default.
 
 ## Background noise
 To enhance model performance we mix in additional background noise from downloaded from the [DCASE18](https://dcase.community/challenge2018/index). To download the files and convert them to the correct format, run the notebook 'download_background_noise.ipynb' in the 'notebooks' folder.
```

