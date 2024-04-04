# Comparing `tmp/africanwhisper-0.2.8.tar.gz` & `tmp/africanwhisper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.2.8.tar", last modified: Wed Apr  3 20:00:59 2024, max compression
+gzip compressed data, was "africanwhisper-0.2.9.tar", last modified: Thu Apr  4 16:02:38 2024, max compression
```

## Comparing `africanwhisper-0.2.8.tar` & `africanwhisper-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.201283 africanwhisper-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/deployment/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:38.333479 africanwhisper-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-04-04 16:02:38.333479 africanwhisper-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-04 16:02:38.333479 africanwhisper-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:38.329479 africanwhisper-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:38.333479 africanwhisper-0.2.9/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-04-04 16:02:38.000000 africanwhisper-0.2.9/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 16:02:38.000000 africanwhisper-0.2.9/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:02:38.000000 africanwhisper-0.2.9/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-04 16:02:38.000000 africanwhisper-0.2.9/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 16:02:38.000000 africanwhisper-0.2.9/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:38.329479 africanwhisper-0.2.9/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/deployment/speech_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:38.329479 africanwhisper-0.2.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:38.333479 africanwhisper-0.2.9/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-04 16:02:34.000000 africanwhisper-0.2.9/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.2.8/LICENSE` & `africanwhisper-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/PKG-INFO` & `africanwhisper-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,27 +14,27 @@
 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: jiwer==3.0.3
 Requires-Dist: bitsandbytes==0.43.0
 Requires-Dist: accelerate==0.28.0
 Requires-Dist: peft==0.9.0
-Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3
 Requires-Dist: panel==1.3.8
 Requires-Dist: gradio==4.24.0
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
-Requires-Dist: yt-dlp==2023.10.13
+Requires-Dist: yt-dlp==2023.11.14
+Requires-Dist: torch==2.2.1
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
@@ -49,15 +49,15 @@
 
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
-## Description
+# Description
 African Whisper is an open-source project aimed at enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages. 
 This is done by developing a package to allow seamless fine-tuning and deployment of the Whisper ASR model developed by OpenAI to better recognize and transcribe African languages for all developers.
 
 ## Why Whisper?
 
 Whisper is an open-source Automatic Speech Recognition (ASR) system developed by OpenAI.<br> 
 Here’s why Whisper stands out:
@@ -107,78 +107,134 @@
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
 - Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
 
-## Usage on a Notebook
+# A Guide to Usage on a Notebook
+
+## Step 1: Installation
 
 ```python
 !pip install africanwhisper
-# Restart the runtime/session: because of an issue with the latest transformers package version
+# If you're on Colab, restart the session due to issue with numpy installation on colab.
 ```
 
-```python
-from training.data_prep import DataPrep
-from training.model_trainer import Trainer
-from training.gradio_inference import WhisperDemo
-```
+## Step 2: Set Parameters
 
 ```python
-# refer to the Usage on VM section below to know more about these parameters
+# Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
-dataset_name = "mozilla-foundation/common_voice_16_1"
-# choose a small dataset so as to not run out of memory, see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1
-language_abbr= "af" 
-model_id= "openai/whisper-small"
+dataset_name = "mozilla-foundation/common_voice_16_1" 
+language_abbr= " " # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+                    # Note: choose a small dataset so as to not run out of memory,
+model_id= "model-id" # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
-# Note: PEFT only works on a notbeook with GPU-support.
-use_peft = True
+use_peft = True  # Note: PEFT only works on a notebook with GPU-support.
+
 ```
 
+## Step 3: Prepare the Model
 ```python
-# Downloading the model, tokenizer, feature extractor and processor
-process = DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task, use_peft)
+from training.data_prep import DataPrep
 
+# Initialize the DataPrep class and prepare the model
+process = DataPrep(
+    huggingface_read_token,
+    dataset_name,
+    language_abbr,
+    model_id,
+    processing_task,
+    use_peft
+)
 tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
+
 ```
 
+## Step 4: Preprocess the Dataset
 ```python
-# Preprocessing the Dataset
-processed_dataset = process.load_dataset(feature_extractor, tokenizer, feature_processor) 
+# Load and preprocess the dataset
+processed_dataset = process.load_dataset(
+    feature_extractor=feature_extractor,
+    tokenizer=tokenizer,
+    feature_processor=feature_processor
+)
 ```
 
+## Step 5: Train the Model
+
 ```python
-# Training the model
-trainer = Trainer(huggingface_write_token, model_id, processed_dataset, model, feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key, use_peft)
-trainer.train(max_steps=100, 
-              learning_rate=1e-5, 
-              per_device_train_batch_size=96,  
-              per_device_eval_batch_size=64, 
-              optim="adamw_bnb_8bit")
+from training.model_trainer import Trainer
+
+# Initialize the Trainer class and train the model
+trainer = Trainer(
+    huggingface_write_token,
+    model_id,
+    processed_dataset,
+    model,
+    feature_processor,
+    feature_extractor,
+    tokenizer,
+    language_abbr,
+    wandb_api_key,
+    use_peft
+)
+trainer.train(
+    max_steps=100,
+    learning_rate=1e-5,
+    per_device_train_batch_size=96,
+    per_device_eval_batch_size=64,
+    optim="adamw_bnb_8bit"
+)
 
 # Optional parameters for training:
 #     max_steps (int): The maximum number of training steps (default is 100).
 #     learning_rate (float): The learning rate for training (default is 1e-5).
 #     per_device_train_batch_size (int): The batch size per GPU for training (default is 96).
 #     per_device_eval_batch_size (int): The batch size per GPU for evaluation (default is 64).
 #     optim (str): The optimizer used for training (default is "adamw_bnb_8bit")
 
 ```
 
+## Step 6: Generate a Demo using GradioUI
 ```python
-# Generate demo
-model_name = " " # Your finetuned model name on huggingface hub e.g "KevinKibe/whisper-small-af"
+from training.gradio_inference import WhisperDemo
+
+# Generate a demo
+model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
+## Step 7: Test Model using Audio File
+
+```python
+from deployment.speech_inference import SpeechInference
+
+model_name = "your-finetuned-model-name-on-huggingface-hub"  # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " "
+task = "desired-task"  # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"  # filetype should be .mp3 or .wav
+
+# Initialize the SpeechInference class and run inference
+inference = SpeechInference(model_name, huggingface_read_token)
+pipeline = inference.pipe_initialization()
+transcription = inference.output(pipeline, audiofile_dir, task)
+
+# Access different parts of the output
+transcription.text  # The entire text transcription.
+transcription.chunks  # List of individual text chunks with timestamps.
+transcription.timestamps  # List of timestamps for each chunk.
+transcription.chunk_texts  # List of texts for each chunk.
+
+```
+
 ## Usage on a Virtual Machine
 
 <details>
 
   - Clone the Repository: Clone or download the application code to your local machine.
   ```
   git clone https://github.com/KevKibe/African-Whisper.git
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.8 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.9 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.43.0 Requires-Dist:
-accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.5
-Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
-gradio==4.24.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
-Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
-scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0 Requires-Dist: yt-
-dlp==2023.10.13
+accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
+Requires-Dist: wandb==0.16.5 Requires-Dist: holoviews==1.18.3 Requires-Dist:
+panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
+Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
+Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
+probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist:
+torch==2.2.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
-## Description African Whisper is an open-source project aimed at enhancing
+# Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
 better recognize and transcribe African languages for all developers. ## Why
 Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
 developed by OpenAI.
 Hereâs why Whisper stands out: - **Extensive Training Data**: Trained on
@@ -47,58 +47,72 @@
 any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
 Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
 ). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
 fro transcription of Audio files. 5. Containerize your REST API endpoint and
 push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
 keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
 Sign up for wandb and get your token keys use this [guide](https://
-app.wandb.ai/login?signup=true) ## Usage on a Notebook ```python !pip install
-africanwhisper # Restart the runtime/session: because of an issue with the
-latest transformers package version ``` ```python from training.data_prep
-import DataPrep from training.model_trainer import Trainer from
-training.gradio_inference import WhisperDemo ``` ```python # refer to the Usage
-on VM section below to know more about these parameters huggingface_read_token
-= " " huggingface_write_token = " " dataset_name = "mozilla-foundation/
-common_voice_16_1" # choose a small dataset so as to not run out of memory, see
-abbreviations here https://huggingface.co/datasets/mozilla-foundation/
-common_voice_16_1 language_abbr= "af" model_id= "openai/whisper-small"
-processing_task= "automatic-speech-recognition" wandb_api_key = " " # Note:
-PEFT only works on a notbeook with GPU-support. use_peft = True ``` ```python #
-Downloading the model, tokenizer, feature extractor and processor process =
-DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id,
-processing_task, use_peft) tokenizer, feature_extractor, feature_processor,
-model = process.prepare_model() ``` ```python # Preprocessing the Dataset
-processed_dataset = process.load_dataset(feature_extractor, tokenizer,
-feature_processor) ``` ```python # Training the model trainer = Trainer
-(huggingface_write_token, model_id, processed_dataset, model,
-feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key,
-use_peft) trainer.train(max_steps=100, learning_rate=1e-5,
-per_device_train_batch_size=96, per_device_eval_batch_size=64,
-optim="adamw_bnb_8bit") # Optional parameters for training: # max_steps (int):
-The maximum number of training steps (default is 100). # learning_rate (float):
-The learning rate for training (default is 1e-5). # per_device_train_batch_size
-(int): The batch size per GPU for training (default is 96). #
-per_device_eval_batch_size (int): The batch size per GPU for evaluation
-(default is 64). # optim (str): The optimizer used for training (default is
-"adamw_bnb_8bit") ``` ```python # Generate demo model_name = " " # Your
-finetuned model name on huggingface hub e.g "KevinKibe/whisper-small-af" demo =
-WhisperDemo(model_name, huggingface_read_token) demo.generate_demo() ``` ##
-Usage on a Virtual Machine - Clone the Repository: Clone or download the
-application code to your local machine. ``` git clone https://github.com/
-KevKibe/African-Whisper.git ``` - Create a virtual environment for the project
-and activate it. ``` python3 -m venv env source venv/bin/activate ``` - Install
-dependencies by running this command ``` pip install -r requirements.txt ``` -
-Navigate to: ``` cd src ``` - To start the training , use the following
-command: ``` python -m training.main \ --huggingface_read_token
-YOUR_HUGGING_FACE_READ_TOKEN_HERE \ --huggingface_write_token
-YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name DATASET_NAME \ --
-language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --processing_task
-PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --use_peft ```
-Here's a short description of each argument used in the command: - **--
-huggingface_read_token**: Your Hugging Face authentication token for read
+app.wandb.ai/login?signup=true) # A Guide to Usage on a Notebook ## Step 1:
+Installation ```python !pip install africanwhisper # If you're on Colab,
+restart the session due to issue with numpy installation on colab. ``` ## Step
+2: Set Parameters ```python # Set the parameters (refer to the 'Usage on VM'
+section for more details) huggingface_read_token = " " huggingface_write_token
+= " " dataset_name = "mozilla-foundation/common_voice_16_1" language_abbr= " "
+# Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/
+mozilla-foundation/common_voice_16_1. # Note: choose a small dataset so as to
+not run out of memory, model_id= "model-id" # Example openai/whisper-small,
+openai/whisper-medium processing_task= "automatic-speech-recognition"
+wandb_api_key = " " use_peft = True # Note: PEFT only works on a notebook with
+GPU-support. ``` ## Step 3: Prepare the Model ```python from training.data_prep
+import DataPrep # Initialize the DataPrep class and prepare the model process =
+DataPrep( huggingface_read_token, dataset_name, language_abbr, model_id,
+processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
+# Load and preprocess the dataset processed_dataset = process.load_dataset
+( feature_extractor=feature_extractor, tokenizer=tokenizer,
+feature_processor=feature_processor ) ``` ## Step 5: Train the Model ```python
+from training.model_trainer import Trainer # Initialize the Trainer class and
+train the model trainer = Trainer( huggingface_write_token, model_id,
+processed_dataset, model, feature_processor, feature_extractor, tokenizer,
+language_abbr, wandb_api_key, use_peft ) trainer.train( max_steps=100,
+learning_rate=1e-5, per_device_train_batch_size=96,
+per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
+for training: # max_steps (int): The maximum number of training steps (default
+is 100). # learning_rate (float): The learning rate for training (default is
+1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
+(default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
+evaluation (default is 64). # optim (str): The optimizer used for training
+(default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
+```python from training.gradio_inference import WhisperDemo # Generate a demo
+model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/
+whisper-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
+demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
+deployment.speech_inference import SpeechInference model_name = "your-
+finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " " task = "desired-task" # either 'translate' or
+'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
+or .wav # Initialize the SpeechInference class and run inference inference =
+SpeechInference(model_name, huggingface_read_token) pipeline =
+inference.pipe_initialization() transcription = inference.output(pipeline,
+audiofile_dir, task) # Access different parts of the output transcription.text
+# The entire text transcription. transcription.chunks # List of individual text
+chunks with timestamps. transcription.timestamps # List of timestamps for each
+chunk. transcription.chunk_texts # List of texts for each chunk. ``` ## Usage
+on a Virtual Machine - Clone the Repository: Clone or download the application
+code to your local machine. ``` git clone https://github.com/KevKibe/African-
+Whisper.git ``` - Create a virtual environment for the project and activate it.
+``` python3 -m venv env source venv/bin/activate ``` - Install dependencies by
+running this command ``` pip install -r requirements.txt ``` - Navigate to: ```
+cd src ``` - To start the training , use the following command: ``` python -
+m training.main \ --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
+--huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name
+DATASET_NAME \ --language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --
+processing_task PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --
+use_peft ``` Here's a short description of each argument used in the command: -
+**--huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. - **--
 huggingface_push_token**: Your Hugging Face authentication token for write
 access. It's used for uploading models to your Hugging Face account. - **--
 dataset_name**: The name of the dataset you wish to use for training. Example:
 'mozilla-foundation/common_voice_16_1'. This should match the dataset's
 identifier on the Hugging Face Datasets Hub. - **--language_abbr**: The
 abbreviation of the language for the dataset you're using. Example: 'sw' for
```

### Comparing `africanwhisper-0.2.8/README.md` & `africanwhisper-0.2.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
-## Description
+# Description
 African Whisper is an open-source project aimed at enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages. 
 This is done by developing a package to allow seamless fine-tuning and deployment of the Whisper ASR model developed by OpenAI to better recognize and transcribe African languages for all developers.
 
 ## Why Whisper?
 
 Whisper is an open-source Automatic Speech Recognition (ASR) system developed by OpenAI.<br> 
 Here’s why Whisper stands out:
@@ -73,78 +73,134 @@
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
 - Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
 
-## Usage on a Notebook
+# A Guide to Usage on a Notebook
+
+## Step 1: Installation
 
 ```python
 !pip install africanwhisper
-# Restart the runtime/session: because of an issue with the latest transformers package version
+# If you're on Colab, restart the session due to issue with numpy installation on colab.
 ```
 
-```python
-from training.data_prep import DataPrep
-from training.model_trainer import Trainer
-from training.gradio_inference import WhisperDemo
-```
+## Step 2: Set Parameters
 
 ```python
-# refer to the Usage on VM section below to know more about these parameters
+# Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
-dataset_name = "mozilla-foundation/common_voice_16_1"
-# choose a small dataset so as to not run out of memory, see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1
-language_abbr= "af" 
-model_id= "openai/whisper-small"
+dataset_name = "mozilla-foundation/common_voice_16_1" 
+language_abbr= " " # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+                    # Note: choose a small dataset so as to not run out of memory,
+model_id= "model-id" # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
-# Note: PEFT only works on a notbeook with GPU-support.
-use_peft = True
+use_peft = True  # Note: PEFT only works on a notebook with GPU-support.
+
 ```
 
+## Step 3: Prepare the Model
 ```python
-# Downloading the model, tokenizer, feature extractor and processor
-process = DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task, use_peft)
+from training.data_prep import DataPrep
 
+# Initialize the DataPrep class and prepare the model
+process = DataPrep(
+    huggingface_read_token,
+    dataset_name,
+    language_abbr,
+    model_id,
+    processing_task,
+    use_peft
+)
 tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
+
 ```
 
+## Step 4: Preprocess the Dataset
 ```python
-# Preprocessing the Dataset
-processed_dataset = process.load_dataset(feature_extractor, tokenizer, feature_processor) 
+# Load and preprocess the dataset
+processed_dataset = process.load_dataset(
+    feature_extractor=feature_extractor,
+    tokenizer=tokenizer,
+    feature_processor=feature_processor
+)
 ```
 
+## Step 5: Train the Model
+
 ```python
-# Training the model
-trainer = Trainer(huggingface_write_token, model_id, processed_dataset, model, feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key, use_peft)
-trainer.train(max_steps=100, 
-              learning_rate=1e-5, 
-              per_device_train_batch_size=96,  
-              per_device_eval_batch_size=64, 
-              optim="adamw_bnb_8bit")
+from training.model_trainer import Trainer
+
+# Initialize the Trainer class and train the model
+trainer = Trainer(
+    huggingface_write_token,
+    model_id,
+    processed_dataset,
+    model,
+    feature_processor,
+    feature_extractor,
+    tokenizer,
+    language_abbr,
+    wandb_api_key,
+    use_peft
+)
+trainer.train(
+    max_steps=100,
+    learning_rate=1e-5,
+    per_device_train_batch_size=96,
+    per_device_eval_batch_size=64,
+    optim="adamw_bnb_8bit"
+)
 
 # Optional parameters for training:
 #     max_steps (int): The maximum number of training steps (default is 100).
 #     learning_rate (float): The learning rate for training (default is 1e-5).
 #     per_device_train_batch_size (int): The batch size per GPU for training (default is 96).
 #     per_device_eval_batch_size (int): The batch size per GPU for evaluation (default is 64).
 #     optim (str): The optimizer used for training (default is "adamw_bnb_8bit")
 
 ```
 
+## Step 6: Generate a Demo using GradioUI
 ```python
-# Generate demo
-model_name = " " # Your finetuned model name on huggingface hub e.g "KevinKibe/whisper-small-af"
+from training.gradio_inference import WhisperDemo
+
+# Generate a demo
+model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
+## Step 7: Test Model using Audio File
+
+```python
+from deployment.speech_inference import SpeechInference
+
+model_name = "your-finetuned-model-name-on-huggingface-hub"  # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " "
+task = "desired-task"  # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"  # filetype should be .mp3 or .wav
+
+# Initialize the SpeechInference class and run inference
+inference = SpeechInference(model_name, huggingface_read_token)
+pipeline = inference.pipe_initialization()
+transcription = inference.output(pipeline, audiofile_dir, task)
+
+# Access different parts of the output
+transcription.text  # The entire text transcription.
+transcription.chunks  # List of individual text chunks with timestamps.
+transcription.timestamps  # List of timestamps for each chunk.
+transcription.chunk_texts  # List of texts for each chunk.
+
+```
+
 ## Usage on a Virtual Machine
 
 <details>
 
   - Clone the Repository: Clone or download the application code to your local machine.
   ```
   git clone https://github.com/KevKibe/African-Whisper.git
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
-## Description African Whisper is an open-source project aimed at enhancing
+# Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
 better recognize and transcribe African languages for all developers. ## Why
 Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
 developed by OpenAI.
 Hereâs why Whisper stands out: - **Extensive Training Data**: Trained on
@@ -31,58 +31,72 @@
 any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
 Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
 ). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
 fro transcription of Audio files. 5. Containerize your REST API endpoint and
 push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
 keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
 Sign up for wandb and get your token keys use this [guide](https://
-app.wandb.ai/login?signup=true) ## Usage on a Notebook ```python !pip install
-africanwhisper # Restart the runtime/session: because of an issue with the
-latest transformers package version ``` ```python from training.data_prep
-import DataPrep from training.model_trainer import Trainer from
-training.gradio_inference import WhisperDemo ``` ```python # refer to the Usage
-on VM section below to know more about these parameters huggingface_read_token
-= " " huggingface_write_token = " " dataset_name = "mozilla-foundation/
-common_voice_16_1" # choose a small dataset so as to not run out of memory, see
-abbreviations here https://huggingface.co/datasets/mozilla-foundation/
-common_voice_16_1 language_abbr= "af" model_id= "openai/whisper-small"
-processing_task= "automatic-speech-recognition" wandb_api_key = " " # Note:
-PEFT only works on a notbeook with GPU-support. use_peft = True ``` ```python #
-Downloading the model, tokenizer, feature extractor and processor process =
-DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id,
-processing_task, use_peft) tokenizer, feature_extractor, feature_processor,
-model = process.prepare_model() ``` ```python # Preprocessing the Dataset
-processed_dataset = process.load_dataset(feature_extractor, tokenizer,
-feature_processor) ``` ```python # Training the model trainer = Trainer
-(huggingface_write_token, model_id, processed_dataset, model,
-feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key,
-use_peft) trainer.train(max_steps=100, learning_rate=1e-5,
-per_device_train_batch_size=96, per_device_eval_batch_size=64,
-optim="adamw_bnb_8bit") # Optional parameters for training: # max_steps (int):
-The maximum number of training steps (default is 100). # learning_rate (float):
-The learning rate for training (default is 1e-5). # per_device_train_batch_size
-(int): The batch size per GPU for training (default is 96). #
-per_device_eval_batch_size (int): The batch size per GPU for evaluation
-(default is 64). # optim (str): The optimizer used for training (default is
-"adamw_bnb_8bit") ``` ```python # Generate demo model_name = " " # Your
-finetuned model name on huggingface hub e.g "KevinKibe/whisper-small-af" demo =
-WhisperDemo(model_name, huggingface_read_token) demo.generate_demo() ``` ##
-Usage on a Virtual Machine - Clone the Repository: Clone or download the
-application code to your local machine. ``` git clone https://github.com/
-KevKibe/African-Whisper.git ``` - Create a virtual environment for the project
-and activate it. ``` python3 -m venv env source venv/bin/activate ``` - Install
-dependencies by running this command ``` pip install -r requirements.txt ``` -
-Navigate to: ``` cd src ``` - To start the training , use the following
-command: ``` python -m training.main \ --huggingface_read_token
-YOUR_HUGGING_FACE_READ_TOKEN_HERE \ --huggingface_write_token
-YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name DATASET_NAME \ --
-language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --processing_task
-PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --use_peft ```
-Here's a short description of each argument used in the command: - **--
-huggingface_read_token**: Your Hugging Face authentication token for read
+app.wandb.ai/login?signup=true) # A Guide to Usage on a Notebook ## Step 1:
+Installation ```python !pip install africanwhisper # If you're on Colab,
+restart the session due to issue with numpy installation on colab. ``` ## Step
+2: Set Parameters ```python # Set the parameters (refer to the 'Usage on VM'
+section for more details) huggingface_read_token = " " huggingface_write_token
+= " " dataset_name = "mozilla-foundation/common_voice_16_1" language_abbr= " "
+# Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/
+mozilla-foundation/common_voice_16_1. # Note: choose a small dataset so as to
+not run out of memory, model_id= "model-id" # Example openai/whisper-small,
+openai/whisper-medium processing_task= "automatic-speech-recognition"
+wandb_api_key = " " use_peft = True # Note: PEFT only works on a notebook with
+GPU-support. ``` ## Step 3: Prepare the Model ```python from training.data_prep
+import DataPrep # Initialize the DataPrep class and prepare the model process =
+DataPrep( huggingface_read_token, dataset_name, language_abbr, model_id,
+processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
+# Load and preprocess the dataset processed_dataset = process.load_dataset
+( feature_extractor=feature_extractor, tokenizer=tokenizer,
+feature_processor=feature_processor ) ``` ## Step 5: Train the Model ```python
+from training.model_trainer import Trainer # Initialize the Trainer class and
+train the model trainer = Trainer( huggingface_write_token, model_id,
+processed_dataset, model, feature_processor, feature_extractor, tokenizer,
+language_abbr, wandb_api_key, use_peft ) trainer.train( max_steps=100,
+learning_rate=1e-5, per_device_train_batch_size=96,
+per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
+for training: # max_steps (int): The maximum number of training steps (default
+is 100). # learning_rate (float): The learning rate for training (default is
+1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
+(default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
+evaluation (default is 64). # optim (str): The optimizer used for training
+(default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
+```python from training.gradio_inference import WhisperDemo # Generate a demo
+model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/
+whisper-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
+demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
+deployment.speech_inference import SpeechInference model_name = "your-
+finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " " task = "desired-task" # either 'translate' or
+'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
+or .wav # Initialize the SpeechInference class and run inference inference =
+SpeechInference(model_name, huggingface_read_token) pipeline =
+inference.pipe_initialization() transcription = inference.output(pipeline,
+audiofile_dir, task) # Access different parts of the output transcription.text
+# The entire text transcription. transcription.chunks # List of individual text
+chunks with timestamps. transcription.timestamps # List of timestamps for each
+chunk. transcription.chunk_texts # List of texts for each chunk. ``` ## Usage
+on a Virtual Machine - Clone the Repository: Clone or download the application
+code to your local machine. ``` git clone https://github.com/KevKibe/African-
+Whisper.git ``` - Create a virtual environment for the project and activate it.
+``` python3 -m venv env source venv/bin/activate ``` - Install dependencies by
+running this command ``` pip install -r requirements.txt ``` - Navigate to: ```
+cd src ``` - To start the training , use the following command: ``` python -
+m training.main \ --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
+--huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name
+DATASET_NAME \ --language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --
+processing_task PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --
+use_peft ``` Here's a short description of each argument used in the command: -
+**--huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. - **--
 huggingface_push_token**: Your Hugging Face authentication token for write
 access. It's used for uploading models to your Hugging Face account. - **--
 dataset_name**: The name of the dataset you wish to use for training. Example:
 'mozilla-foundation/common_voice_16_1'. This should match the dataset's
 identifier on the Hugging Face Datasets Hub. - **--language_abbr**: The
 abbreviation of the language for the dataset you're using. Example: 'sw' for
```

### Comparing `africanwhisper-0.2.8/setup.cfg` & `africanwhisper-0.2.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.2.8
+version = 0.2.9
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
 
@@ -18,27 +18,27 @@
 	datasets==2.18.0
 	librosa==0.10.1
 	evaluate==0.4.1
 	jiwer==3.0.3
 	bitsandbytes==0.43.0
 	accelerate==0.28.0
 	peft==0.9.0
-	python-dotenv==1.0.1
 	numpy==1.26.4
 	wandb==0.16.5
 	holoviews==1.18.3
 	panel==1.3.8
 	gradio==4.24.0
 	pytube==15.0.0
 	tf-keras==2.16.0
 	tensorflow==2.16.1
 	keras==3.1.1
 	scipy==1.12.0
 	tensorflow-probability==0.24.0
-	yt-dlp==2023.10.13
+	yt-dlp==2023.11.14
+	torch==2.2.1
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `africanwhisper-0.2.8/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.2.9/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,27 +14,27 @@
 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: jiwer==3.0.3
 Requires-Dist: bitsandbytes==0.43.0
 Requires-Dist: accelerate==0.28.0
 Requires-Dist: peft==0.9.0
-Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3
 Requires-Dist: panel==1.3.8
 Requires-Dist: gradio==4.24.0
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
-Requires-Dist: yt-dlp==2023.10.13
+Requires-Dist: yt-dlp==2023.11.14
+Requires-Dist: torch==2.2.1
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
@@ -49,15 +49,15 @@
 
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
-## Description
+# Description
 African Whisper is an open-source project aimed at enhancing Automatic Speech Recognition (ASR): translation and transcription capabilities for African languages. 
 This is done by developing a package to allow seamless fine-tuning and deployment of the Whisper ASR model developed by OpenAI to better recognize and transcribe African languages for all developers.
 
 ## Why Whisper?
 
 Whisper is an open-source Automatic Speech Recognition (ASR) system developed by OpenAI.<br> 
 Here’s why Whisper stands out:
@@ -107,78 +107,134 @@
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
 - Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
 
-## Usage on a Notebook
+# A Guide to Usage on a Notebook
+
+## Step 1: Installation
 
 ```python
 !pip install africanwhisper
-# Restart the runtime/session: because of an issue with the latest transformers package version
+# If you're on Colab, restart the session due to issue with numpy installation on colab.
 ```
 
-```python
-from training.data_prep import DataPrep
-from training.model_trainer import Trainer
-from training.gradio_inference import WhisperDemo
-```
+## Step 2: Set Parameters
 
 ```python
-# refer to the Usage on VM section below to know more about these parameters
+# Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
-dataset_name = "mozilla-foundation/common_voice_16_1"
-# choose a small dataset so as to not run out of memory, see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1
-language_abbr= "af" 
-model_id= "openai/whisper-small"
+dataset_name = "mozilla-foundation/common_voice_16_1" 
+language_abbr= " " # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+                    # Note: choose a small dataset so as to not run out of memory,
+model_id= "model-id" # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
-# Note: PEFT only works on a notbeook with GPU-support.
-use_peft = True
+use_peft = True  # Note: PEFT only works on a notebook with GPU-support.
+
 ```
 
+## Step 3: Prepare the Model
 ```python
-# Downloading the model, tokenizer, feature extractor and processor
-process = DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task, use_peft)
+from training.data_prep import DataPrep
 
+# Initialize the DataPrep class and prepare the model
+process = DataPrep(
+    huggingface_read_token,
+    dataset_name,
+    language_abbr,
+    model_id,
+    processing_task,
+    use_peft
+)
 tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
+
 ```
 
+## Step 4: Preprocess the Dataset
 ```python
-# Preprocessing the Dataset
-processed_dataset = process.load_dataset(feature_extractor, tokenizer, feature_processor) 
+# Load and preprocess the dataset
+processed_dataset = process.load_dataset(
+    feature_extractor=feature_extractor,
+    tokenizer=tokenizer,
+    feature_processor=feature_processor
+)
 ```
 
+## Step 5: Train the Model
+
 ```python
-# Training the model
-trainer = Trainer(huggingface_write_token, model_id, processed_dataset, model, feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key, use_peft)
-trainer.train(max_steps=100, 
-              learning_rate=1e-5, 
-              per_device_train_batch_size=96,  
-              per_device_eval_batch_size=64, 
-              optim="adamw_bnb_8bit")
+from training.model_trainer import Trainer
+
+# Initialize the Trainer class and train the model
+trainer = Trainer(
+    huggingface_write_token,
+    model_id,
+    processed_dataset,
+    model,
+    feature_processor,
+    feature_extractor,
+    tokenizer,
+    language_abbr,
+    wandb_api_key,
+    use_peft
+)
+trainer.train(
+    max_steps=100,
+    learning_rate=1e-5,
+    per_device_train_batch_size=96,
+    per_device_eval_batch_size=64,
+    optim="adamw_bnb_8bit"
+)
 
 # Optional parameters for training:
 #     max_steps (int): The maximum number of training steps (default is 100).
 #     learning_rate (float): The learning rate for training (default is 1e-5).
 #     per_device_train_batch_size (int): The batch size per GPU for training (default is 96).
 #     per_device_eval_batch_size (int): The batch size per GPU for evaluation (default is 64).
 #     optim (str): The optimizer used for training (default is "adamw_bnb_8bit")
 
 ```
 
+## Step 6: Generate a Demo using GradioUI
 ```python
-# Generate demo
-model_name = " " # Your finetuned model name on huggingface hub e.g "KevinKibe/whisper-small-af"
+from training.gradio_inference import WhisperDemo
+
+# Generate a demo
+model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
+## Step 7: Test Model using Audio File
+
+```python
+from deployment.speech_inference import SpeechInference
+
+model_name = "your-finetuned-model-name-on-huggingface-hub"  # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " "
+task = "desired-task"  # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"  # filetype should be .mp3 or .wav
+
+# Initialize the SpeechInference class and run inference
+inference = SpeechInference(model_name, huggingface_read_token)
+pipeline = inference.pipe_initialization()
+transcription = inference.output(pipeline, audiofile_dir, task)
+
+# Access different parts of the output
+transcription.text  # The entire text transcription.
+transcription.chunks  # List of individual text chunks with timestamps.
+transcription.timestamps  # List of timestamps for each chunk.
+transcription.chunk_texts  # List of texts for each chunk.
+
+```
+
 ## Usage on a Virtual Machine
 
 <details>
 
   - Clone the Repository: Clone or download the application code to your local machine.
   ```
   git clone https://github.com/KevKibe/African-Whisper.git
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.8 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.9 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.43.0 Requires-Dist:
-accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.5
-Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
-gradio==4.24.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
-Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
-scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0 Requires-Dist: yt-
-dlp==2023.10.13
+accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
+Requires-Dist: wandb==0.16.5 Requires-Dist: holoviews==1.18.3 Requires-Dist:
+panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
+Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
+Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
+probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist:
+torch==2.2.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
-## Description African Whisper is an open-source project aimed at enhancing
+# Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
 better recognize and transcribe African languages for all developers. ## Why
 Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
 developed by OpenAI.
 Hereâs why Whisper stands out: - **Extensive Training Data**: Trained on
@@ -47,58 +47,72 @@
 any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
 Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
 ). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
 fro transcription of Audio files. 5. Containerize your REST API endpoint and
 push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
 keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
 Sign up for wandb and get your token keys use this [guide](https://
-app.wandb.ai/login?signup=true) ## Usage on a Notebook ```python !pip install
-africanwhisper # Restart the runtime/session: because of an issue with the
-latest transformers package version ``` ```python from training.data_prep
-import DataPrep from training.model_trainer import Trainer from
-training.gradio_inference import WhisperDemo ``` ```python # refer to the Usage
-on VM section below to know more about these parameters huggingface_read_token
-= " " huggingface_write_token = " " dataset_name = "mozilla-foundation/
-common_voice_16_1" # choose a small dataset so as to not run out of memory, see
-abbreviations here https://huggingface.co/datasets/mozilla-foundation/
-common_voice_16_1 language_abbr= "af" model_id= "openai/whisper-small"
-processing_task= "automatic-speech-recognition" wandb_api_key = " " # Note:
-PEFT only works on a notbeook with GPU-support. use_peft = True ``` ```python #
-Downloading the model, tokenizer, feature extractor and processor process =
-DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id,
-processing_task, use_peft) tokenizer, feature_extractor, feature_processor,
-model = process.prepare_model() ``` ```python # Preprocessing the Dataset
-processed_dataset = process.load_dataset(feature_extractor, tokenizer,
-feature_processor) ``` ```python # Training the model trainer = Trainer
-(huggingface_write_token, model_id, processed_dataset, model,
-feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key,
-use_peft) trainer.train(max_steps=100, learning_rate=1e-5,
-per_device_train_batch_size=96, per_device_eval_batch_size=64,
-optim="adamw_bnb_8bit") # Optional parameters for training: # max_steps (int):
-The maximum number of training steps (default is 100). # learning_rate (float):
-The learning rate for training (default is 1e-5). # per_device_train_batch_size
-(int): The batch size per GPU for training (default is 96). #
-per_device_eval_batch_size (int): The batch size per GPU for evaluation
-(default is 64). # optim (str): The optimizer used for training (default is
-"adamw_bnb_8bit") ``` ```python # Generate demo model_name = " " # Your
-finetuned model name on huggingface hub e.g "KevinKibe/whisper-small-af" demo =
-WhisperDemo(model_name, huggingface_read_token) demo.generate_demo() ``` ##
-Usage on a Virtual Machine - Clone the Repository: Clone or download the
-application code to your local machine. ``` git clone https://github.com/
-KevKibe/African-Whisper.git ``` - Create a virtual environment for the project
-and activate it. ``` python3 -m venv env source venv/bin/activate ``` - Install
-dependencies by running this command ``` pip install -r requirements.txt ``` -
-Navigate to: ``` cd src ``` - To start the training , use the following
-command: ``` python -m training.main \ --huggingface_read_token
-YOUR_HUGGING_FACE_READ_TOKEN_HERE \ --huggingface_write_token
-YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name DATASET_NAME \ --
-language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --processing_task
-PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --use_peft ```
-Here's a short description of each argument used in the command: - **--
-huggingface_read_token**: Your Hugging Face authentication token for read
+app.wandb.ai/login?signup=true) # A Guide to Usage on a Notebook ## Step 1:
+Installation ```python !pip install africanwhisper # If you're on Colab,
+restart the session due to issue with numpy installation on colab. ``` ## Step
+2: Set Parameters ```python # Set the parameters (refer to the 'Usage on VM'
+section for more details) huggingface_read_token = " " huggingface_write_token
+= " " dataset_name = "mozilla-foundation/common_voice_16_1" language_abbr= " "
+# Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/
+mozilla-foundation/common_voice_16_1. # Note: choose a small dataset so as to
+not run out of memory, model_id= "model-id" # Example openai/whisper-small,
+openai/whisper-medium processing_task= "automatic-speech-recognition"
+wandb_api_key = " " use_peft = True # Note: PEFT only works on a notebook with
+GPU-support. ``` ## Step 3: Prepare the Model ```python from training.data_prep
+import DataPrep # Initialize the DataPrep class and prepare the model process =
+DataPrep( huggingface_read_token, dataset_name, language_abbr, model_id,
+processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
+# Load and preprocess the dataset processed_dataset = process.load_dataset
+( feature_extractor=feature_extractor, tokenizer=tokenizer,
+feature_processor=feature_processor ) ``` ## Step 5: Train the Model ```python
+from training.model_trainer import Trainer # Initialize the Trainer class and
+train the model trainer = Trainer( huggingface_write_token, model_id,
+processed_dataset, model, feature_processor, feature_extractor, tokenizer,
+language_abbr, wandb_api_key, use_peft ) trainer.train( max_steps=100,
+learning_rate=1e-5, per_device_train_batch_size=96,
+per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
+for training: # max_steps (int): The maximum number of training steps (default
+is 100). # learning_rate (float): The learning rate for training (default is
+1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
+(default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
+evaluation (default is 64). # optim (str): The optimizer used for training
+(default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
+```python from training.gradio_inference import WhisperDemo # Generate a demo
+model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/
+whisper-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
+demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
+deployment.speech_inference import SpeechInference model_name = "your-
+finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " " task = "desired-task" # either 'translate' or
+'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
+or .wav # Initialize the SpeechInference class and run inference inference =
+SpeechInference(model_name, huggingface_read_token) pipeline =
+inference.pipe_initialization() transcription = inference.output(pipeline,
+audiofile_dir, task) # Access different parts of the output transcription.text
+# The entire text transcription. transcription.chunks # List of individual text
+chunks with timestamps. transcription.timestamps # List of timestamps for each
+chunk. transcription.chunk_texts # List of texts for each chunk. ``` ## Usage
+on a Virtual Machine - Clone the Repository: Clone or download the application
+code to your local machine. ``` git clone https://github.com/KevKibe/African-
+Whisper.git ``` - Create a virtual environment for the project and activate it.
+``` python3 -m venv env source venv/bin/activate ``` - Install dependencies by
+running this command ``` pip install -r requirements.txt ``` - Navigate to: ```
+cd src ``` - To start the training , use the following command: ``` python -
+m training.main \ --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \
+--huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name
+DATASET_NAME \ --language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --
+processing_task PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --
+use_peft ``` Here's a short description of each argument used in the command: -
+**--huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. - **--
 huggingface_push_token**: Your Hugging Face authentication token for write
 access. It's used for uploading models to your Hugging Face account. - **--
 dataset_name**: The name of the dataset you wish to use for training. Example:
 'mozilla-foundation/common_voice_16_1'. This should match the dataset's
 identifier on the Hugging Face Datasets Hub. - **--language_abbr**: The
 abbreviation of the language for the dataset you're using. Example: 'sw' for
```

### Comparing `africanwhisper-0.2.8/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.2.9/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/africanwhisper.egg-info/PKG-INFO
 src/africanwhisper.egg-info/SOURCES.txt
 src/africanwhisper.egg-info/dependency_links.txt
 src/africanwhisper.egg-info/requires.txt
 src/africanwhisper.egg-info/top_level.txt
 src/deployment/__init__.py
 src/deployment/main.py
+src/deployment/speech_inference.py
 src/tests/__init__.py
 src/tests/test_dataset.py
 src/training/__init__.py
 src/training/audio_data_processor.py
 src/training/collator.py
 src/training/data_prep.py
 src/training/evaluation.py
```

### Comparing `africanwhisper-0.2.8/src/tests/test_dataset.py` & `africanwhisper-0.2.9/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/audio_data_processor.py` & `africanwhisper-0.2.9/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/collator.py` & `africanwhisper-0.2.9/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/data_prep.py` & `africanwhisper-0.2.9/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/evaluation.py` & `africanwhisper-0.2.9/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/gradio_demo.py` & `africanwhisper-0.2.9/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/gradio_inference.py` & `africanwhisper-0.2.9/src/training/gradio_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,27 +14,38 @@
         self.model_name = model_name
         self.huggingface_read_token = huggingface_read_token
         self.pipe = None
 
 
     def initialize_pipeline(self):
         device = 0 if torch.cuda.is_available() else "cpu"
+        if torch.cuda.is_available() and torch.cuda.is_bf16_supported():
+            dtype = torch.bfloat16
+        else:
+            dtype = None
+
         self.pipe = pipeline(
             task="automatic-speech-recognition",
             model=self.model_name,
             token=self.huggingface_read_token,
-            chunk_length_s=30,
             device=device,
+            torch_dtype=dtype
         )
 
+
     def transcribe(self, inputs, task):
         if inputs is None:
             raise gr.Error("No audio file submitted! Please upload or record an audio file before submitting your request.")
-        BATCH_SIZE = 8
-        text = self.pipe(inputs, batch_size=BATCH_SIZE, generate_kwargs={"task": task}, return_timestamps=True)["text"]
+        text = self.pipe(
+                        inputs,
+                        chunk_length_s=30,
+                        batch_size=24, 
+                        return_timestamps=True,
+                        generate_kwargs={"task": task}
+                        )["text"]
         return  text
     
     def _return_yt_html_embed(self, yt_url):
         video_id = yt_url.split("?v=")[-1]
         HTML_str = (
             f'<center> <iframe width="500" height="320" src="https://www.youtube.com/embed/{video_id}"> </iframe>'
             " </center>"
```

### Comparing `africanwhisper-0.2.8/src/training/load_data.py` & `africanwhisper-0.2.9/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/main.py` & `africanwhisper-0.2.9/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/model_trainer.py` & `africanwhisper-0.2.9/src/training/model_trainer.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/wandb_callback.py` & `africanwhisper-0.2.9/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.8/src/training/whisper_model_prep.py` & `africanwhisper-0.2.9/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

