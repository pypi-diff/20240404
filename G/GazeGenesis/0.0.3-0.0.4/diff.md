# Comparing `tmp/GazeGenesis-0.0.3.tar.gz` & `tmp/GazeGenesis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazeGenesis-0.0.3.tar", last modified: Sun Mar 31 20:50:39 2024, max compression
+gzip compressed data, was "GazeGenesis-0.0.4.tar", last modified: Thu Apr  4 19:24:24 2024, max compression
```

## Comparing `GazeGenesis-0.0.3.tar` & `GazeGenesis-0.0.4.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.045486 GazeGenesis-0.0.3/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1302 2024-03-31 20:50:39.045204 GazeGenesis-0.0.3/PKG-INFO
--rw-r--r--   0 sinamoghimi   (501) staff       (20)      595 2024-03-31 20:47:27.000000 GazeGenesis-0.0.3/README.md
--rw-r--r--   0 sinamoghimi   (501) staff       (20)      764 2024-03-31 20:46:15.000000 GazeGenesis-0.0.3/pyproject.toml
--rw-r--r--   0 sinamoghimi   (501) staff       (20)       38 2024-03-31 20:50:39.045549 GazeGenesis-0.0.3/setup.cfg
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.030062 GazeGenesis-0.0.3/src/
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.032744 GazeGenesis-0.0.3/src/GazeGenesis/
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.033815 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.033971 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.034518 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)      890 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     3371 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.035043 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     4394 2024-03-31 14:51:44.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     3374 2024-03-31 14:50:52.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.035600 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/LeNet/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/LeNet/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1140 2024-03-31 14:09:18.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/LeNet/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     3358 2024-03-30 17:11:59.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/LeNet/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.036264 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)      456 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     3701 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.036649 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ResNet/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 19:49:23.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ResNet/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     2222 2024-03-31 20:41:59.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ResNet/model.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.037530 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VGG/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VGG/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1980 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VGG/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     3713 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VGG/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.038138 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 19:49:05.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     5640 2024-03-31 13:46:59.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     4206 2024-03-31 09:55:18.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/user.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/__init__.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.039153 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1754 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/CIFAR10.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1766 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/CIFAR100.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1873 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/ImageNet.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1704 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/MNIST.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/__init__.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.039322 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.039847 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/DCGAN/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/DCGAN/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     4184 2024-03-24 18:10:32.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/DCGAN/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     5374 2024-03-26 19:42:03.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/DCGAN/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.040424 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/GAN/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/GAN/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)      890 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/GAN/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     5397 2024-03-26 19:42:31.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/GAN/user.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.040986 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/WGAN/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/WGAN/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     4184 2024-03-24 18:10:32.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/WGAN/model.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     5373 2024-03-26 19:43:33.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/WGAN/user.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/__init__.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.041310 GazeGenesis-0.0.3/src/GazeGenesis/Extras/
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.042691 GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)       81 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/README.md
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     6135 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/fourteen_seg.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1256 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/main.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)   711686 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/result.gif
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Extras/__init__.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.044171 GazeGenesis-0.0.3/src/GazeGenesis/ImageProcessing/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/ImageProcessing/__init__.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.044537 GazeGenesis-0.0.3/src/GazeGenesis/Utility/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Utility/__init__.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)      344 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/Utility/device.py
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.3/src/GazeGenesis/__init__.py
-drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 20:50:39.044794 GazeGenesis-0.0.3/src/GazeGenesis.egg-info/
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     1302 2024-03-31 20:50:38.000000 GazeGenesis-0.0.3/src/GazeGenesis.egg-info/PKG-INFO
--rw-r--r--   0 sinamoghimi   (501) staff       (20)     2900 2024-03-31 20:50:39.000000 GazeGenesis-0.0.3/src/GazeGenesis.egg-info/SOURCES.txt
--rw-r--r--   0 sinamoghimi   (501) staff       (20)        1 2024-03-31 20:50:38.000000 GazeGenesis-0.0.3/src/GazeGenesis.egg-info/dependency_links.txt
--rw-r--r--   0 sinamoghimi   (501) staff       (20)       65 2024-03-31 20:50:38.000000 GazeGenesis-0.0.3/src/GazeGenesis.egg-info/requires.txt
--rw-r--r--   0 sinamoghimi   (501) staff       (20)       12 2024-03-31 20:50:38.000000 GazeGenesis-0.0.3/src/GazeGenesis.egg-info/top_level.txt
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.608485 GazeGenesis-0.0.4/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1354 2024-04-04 19:24:24.608170 GazeGenesis-0.0.4/PKG-INFO
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)      647 2024-04-01 20:48:52.000000 GazeGenesis-0.0.4/README.md
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)      764 2024-04-04 19:23:40.000000 GazeGenesis-0.0.4/pyproject.toml
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)       38 2024-04-04 19:24:24.608550 GazeGenesis-0.0.4/setup.cfg
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.594728 GazeGenesis-0.0.4/src/
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.596898 GazeGenesis-0.0.4/src/GazeGenesis/
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.597899 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.598041 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.598571 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)      890 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     3371 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.599061 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     4394 2024-03-31 14:51:44.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     3374 2024-03-31 14:50:52.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.599556 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/LeNet/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/LeNet/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1140 2024-03-31 14:09:18.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/LeNet/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     3358 2024-03-30 17:11:59.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/LeNet/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.600091 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)      456 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     3701 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.600604 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ResNet/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 19:49:23.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ResNet/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     5888 2024-04-03 17:47:19.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ResNet/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     3399 2024-04-03 17:37:31.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ResNet/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.601092 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VGG/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VGG/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1980 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VGG/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     3713 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VGG/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.601552 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-31 19:49:05.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     5757 2024-04-04 19:03:00.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     4162 2024-04-04 19:19:15.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/user.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/__init__.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.602348 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1754 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/CIFAR10.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1766 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/CIFAR100.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1873 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/ImageNet.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1704 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/MNIST.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/__init__.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.602471 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.602919 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/DCGAN/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/DCGAN/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     4184 2024-03-24 18:10:32.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/DCGAN/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     5374 2024-03-26 19:42:03.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/DCGAN/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.603451 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/GAN/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/GAN/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)      890 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/GAN/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     5397 2024-03-26 19:42:31.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/GAN/user.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.603950 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/WGAN/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/WGAN/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     4184 2024-03-24 18:10:32.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/WGAN/model.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     5373 2024-03-26 19:43:33.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/WGAN/user.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/__init__.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.604122 GazeGenesis-0.0.4/src/GazeGenesis/Extras/
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.605406 GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)       81 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/README.md
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     6135 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/fourteen_seg.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1256 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/main.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)   711686 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/result.gif
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Extras/__init__.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.606969 GazeGenesis-0.0.4/src/GazeGenesis/ImageProcessing/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/ImageProcessing/__init__.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.607342 GazeGenesis-0.0.4/src/GazeGenesis/Utility/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Utility/__init__.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)      344 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/Utility/device.py
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        0 2024-03-24 08:46:43.000000 GazeGenesis-0.0.4/src/GazeGenesis/__init__.py
+drwxr-xr-x   0 sinamoghimi   (501) staff       (20)        0 2024-04-04 19:24:24.607732 GazeGenesis-0.0.4/src/GazeGenesis.egg-info/
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     1354 2024-04-04 19:24:24.000000 GazeGenesis-0.0.4/src/GazeGenesis.egg-info/PKG-INFO
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)     2961 2024-04-04 19:24:24.000000 GazeGenesis-0.0.4/src/GazeGenesis.egg-info/SOURCES.txt
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)        1 2024-04-04 19:24:24.000000 GazeGenesis-0.0.4/src/GazeGenesis.egg-info/dependency_links.txt
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)       65 2024-04-04 19:24:24.000000 GazeGenesis-0.0.4/src/GazeGenesis.egg-info/requires.txt
+-rw-r--r--   0 sinamoghimi   (501) staff       (20)       12 2024-04-04 19:24:24.000000 GazeGenesis-0.0.4/src/GazeGenesis.egg-info/top_level.txt
```

### Comparing `GazeGenesis-0.0.3/PKG-INFO` & `GazeGenesis-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GazeGenesis
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package including Computer Vision Pytorch projects.
 Author-email: Sina Moghimi <sinamoghimi73@gmail.com>
 Project-URL: Homepage, https://github.com/sinamoghimi73/GazeGenesis
 Project-URL: Issues, https://github.com/sinamoghimi73/GazeGenesis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,16 @@
 Requires-Dist: tensorboard
 
 # GazeGenesis
 GazeGenesis: This repository is a playground for innovative computer vision projects, exploring cutting-edge algorithms, and pushing the boundaries of visual perception.🔭📸 #ComputerVision #AI #Innovation"
 
 **The project is intended to leverage the cutting-edge Apple Silicon Architectures using MLX and PyTorch!**
 
+[PyPI Link](https://pypi.org/project/GazeGenesis/)
+
 **Install**
 ```zsh
 python3 -m pip install GazeGenesis
 ```
 
 <color style="color : orange">To receive the up-to-date package:</color>
```

### Comparing `GazeGenesis-0.0.3/pyproject.toml` & `GazeGenesis-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GazeGenesis"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Sina Moghimi", email = "sinamoghimi73@gmail.com" }]
 description = "A package including Computer Vision Pytorch projects."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/ConvolutionalNeuralNetwork/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/GoogLeNet/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/LeNet/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/LeNet/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/LeNet/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/LeNet/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VGG/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VGG/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VGG/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VGG/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class PatchEmbeddings(nn.Module):
     def __init__(self, image_size = 224, patch_size = 16, in_channels = 3, embed_dim = 768):
         super(PatchEmbeddings, self).__init__()
         self.image_size = image_size
         self.patch_size = patch_size
 
         self.num_patches = int(image_size // patch_size) ** 2
-        self.patchifier = nn.Conv2d(in_channels, embed_dim, kernel_size=patch_size, stride=patch_size)
+        self.patchifier = nn.Conv2d(in_channels=in_channels, out_channels=embed_dim, kernel_size=patch_size, stride=patch_size)
 
     def forward(self, x):
         # (batch_size, in_channels, image_size, image_size) -> (batch_size, num_patches, embed_dim)
         x = self.patchifier(x) # (batch_size, embed_dim, num_patches ** 0.5, num_patches ** 0.5)
         x = x.flatten(2) # (batch_size, embed_dim, num_patches)
         x = x.transpose(1, 2) # (batch_size, num_patches, embed_dim) 
         return x
@@ -28,29 +28,31 @@
         self.scale = self.head_dim ** -0.5
 
         self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
         self.attn_drop = nn.Dropout(attn_p)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_p)
 
+        self.softmax = nn.Softmax(dim=-1)
+
 
     def forward(self, x):
         n_samples, n_tokens, dim = x.shape
 
         if dim != self.dim:
             raise ValueError
 
         qkv = self.qkv(x)  # (n_samples, n_patches + 1, 3 * dim)
         qkv = qkv.reshape(n_samples, n_tokens, 3, self.n_heads, self.head_dim)  # (n_smaples, n_patches + 1, 3, n_heads, head_dim)
         qkv = qkv.permute(2, 0, 3, 1, 4)  # (3, n_samples, n_heads, n_patches + 1, head_dim)
 
         q, k, v = qkv[0], qkv[1], qkv[2]
         k_t = k.transpose(-2, -1)  # (n_samples, n_heads, head_dim, n_patches + 1)
         attention_scores = torch.matmul(q, k_t) * self.scale # (n_samples, n_heads, n_patches + 1, n_patches + 1)
-        attention_probs = attention_scores.softmax(dim=-1)  # (n_samples, n_heads, n_patches + 1, n_patches + 1)
+        attention_probs = self.softmax(attention_scores)  # (n_samples, n_heads, n_patches + 1, n_patches + 1)
         attention_probs = self.attn_drop(attention_probs)
 
         weighted_avg = torch.matmul(attention_probs, v)  # (n_samples, n_heads, n_patches +1, head_dim)
         weighted_avg = weighted_avg.transpose(1, 2)  # (n_samples, n_patches + 1, n_heads, head_dim)
         weighted_avg = weighted_avg.flatten(2)  # (n_samples, n_patches + 1, dim)
 
         x = self.proj(weighted_avg)  # (n_samples, n_patches + 1, dim)
@@ -83,42 +85,43 @@
 
         hidden_features = int(dim * mlp_ratio)
         self.mlp = MLP(
             in_features = dim, hidden_features = hidden_features, out_features = dim, p = 0.
         )
 
     def forward(self, x):
-        x += x + self.attn(self.norm1(x))
-        x += self.mlp(self.norm2(x))
+        x = x + self.attn(self.norm1(x))
+        x = x + self.mlp(self.norm2(x))
         return x
     
 class VisionTransformer(nn.Module):
     def __init__(self, 
                  img_size = 384, patch_size = 16, in_channels = 3, n_classes = 10, embed_dim = 768, depth = 12, n_heads = 12, mlp_ratio = 4., qkv_bias = True, p = 0., attn_p = 0.
                  ):
         super(VisionTransformer, self).__init__()
+        print(f"Model: ViT-{depth}")
         self.patch_embed = PatchEmbeddings(image_size = img_size, patch_size = patch_size, in_channels = in_channels, embed_dim = embed_dim)
 
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dim))
         self.pos_embed = nn.Parameter(torch.zeros(1, 1 + self.patch_embed.num_patches, embed_dim))
 
         self.pos_drop = nn.Dropout(p)
         self.blocks = nn.ModuleList([Block(dim = embed_dim, n_heads = n_heads, mlp_ratio = mlp_ratio, qkv_bias = qkv_bias, p = p, attn_p = attn_p)]*depth)
 
         self.norm = nn.LayerNorm(embed_dim, eps = 1e-6)
         self.head = nn.Linear(embed_dim, n_classes)
 
     def forward(self, x):
         batch_size = x.shape[0]
         x = self.patch_embed(x)
-
+        
         cls_token = self.cls_token.expand(batch_size, -1, -1) # (n_samples, 1, embed_dim)
         x = torch.cat((cls_token, x), dim = 1) # (n_samples, 1 + n_patches, embed_dim)
 
-        x += self.pos_embed # (n_samples, 1 + n_patches, embed_dim)
+        x = x + self.pos_embed # (n_samples, 1 + n_patches, embed_dim)
         x = self.pos_drop(x)
 
         for block in self.blocks:
             x = block(x)
         
         x = self.norm(x)
         cls_token_final = x[:, 0] # just the CLS token
@@ -132,15 +135,15 @@
 if __name__ == "__main__":
     x = torch.randn(1, 3, 28, 28)
     vit = VisionTransformer(
         img_size = 28,
         patch_size= 4,
         in_channels = 3,
         n_classes = 10,
-        embed_dim = 8,
+        embed_dim = 48,
         depth = 1,
         n_heads = 4,
         mlp_ratio= 4.,
         qkv_bias= True,
         p = 0.1,
         attn_p= 0.1
     )
```

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Classification/VisionTransformer/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/python3
 
 import torch
-import torch.nn as nn
-import torch.optim as optim
+from torch import nn, optim
 from GazeGenesis.Utility.device import get_device_name
 from GazeGenesis.ComputerVision.Classification.VisionTransformer.model import VisionTransformer
 
 from rich.progress import track
 
 
 class User:
@@ -47,15 +46,14 @@
         self.optimizer = optim.Adam(self.model.parameters(), lr=learning_rate, betas = (0.9, 0.98), eps = 1e-9)
         
 
     def train(self, epochs=10):
         if self.dataset is not None:
             digits = int(torch.log10(torch.tensor(epochs))) + 1
             for epoch in range(epochs):
-                print()
                 ls = []
                 for batch_idx, (inputs, targets) in enumerate(
                     track(
                         self.dataset.train_loader,
                         description=f"[TRAIN] {epoch+1:0{digits}d}/{epochs}",
                     )
                 ):
@@ -80,15 +78,15 @@
                     self.dataset.train_loader, "evaluate: train"
                 )
                 valid_accuracy = self.evaluate(
                     self.dataset.valid_loader, "evaluate: validation"
                 )
 
                 print(
-                    f"EPOCH: {epoch+1:0{digits}d}/{epochs}, LOSS: {torch.tensor(ls).mean():.4f}, TRAIN_ACC: {train_accuracy:.4f}, VAL_ACC: {valid_accuracy:.4f}"
+                    f"EPOCH: {epoch+1:0{digits}d}/{epochs}, LOSS: {torch.tensor(ls).mean():.4f}, TRAIN_ACC: {train_accuracy:.4f}, VAL_ACC: {valid_accuracy:.4f}\n"
                 )
         else:
             raise Exception("Dataset is None.")
 
     def evaluate(self, loader, name):
         if self.dataset is not None:
             self.model.eval()  # This is evaluation mode
```

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/CIFAR10.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/CIFAR10.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/CIFAR100.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/CIFAR100.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/ImageNet.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/ImageNet.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Datasets/MNIST.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Datasets/MNIST.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/DCGAN/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/DCGAN/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/DCGAN/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/DCGAN/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/GAN/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/GAN/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/GAN/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/GAN/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/WGAN/model.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/WGAN/model.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/ComputerVision/Generative/WGAN/user.py` & `GazeGenesis-0.0.4/src/GazeGenesis/ComputerVision/Generative/WGAN/user.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/fourteen_seg.py` & `GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/fourteen_seg.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/main.py` & `GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/main.py`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis/Extras/00_hello_world/result.gif` & `GazeGenesis-0.0.4/src/GazeGenesis/Extras/00_hello_world/result.gif`

 * *Files identical despite different names*

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis.egg-info/PKG-INFO` & `GazeGenesis-0.0.4/src/GazeGenesis.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GazeGenesis
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package including Computer Vision Pytorch projects.
 Author-email: Sina Moghimi <sinamoghimi73@gmail.com>
 Project-URL: Homepage, https://github.com/sinamoghimi73/GazeGenesis
 Project-URL: Issues, https://github.com/sinamoghimi73/GazeGenesis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,16 @@
 Requires-Dist: tensorboard
 
 # GazeGenesis
 GazeGenesis: This repository is a playground for innovative computer vision projects, exploring cutting-edge algorithms, and pushing the boundaries of visual perception.🔭📸 #ComputerVision #AI #Innovation"
 
 **The project is intended to leverage the cutting-edge Apple Silicon Architectures using MLX and PyTorch!**
 
+[PyPI Link](https://pypi.org/project/GazeGenesis/)
+
 **Install**
 ```zsh
 python3 -m pip install GazeGenesis
 ```
 
 <color style="color : orange">To receive the up-to-date package:</color>
```

### Comparing `GazeGenesis-0.0.3/src/GazeGenesis.egg-info/SOURCES.txt` & `GazeGenesis-0.0.4/src/GazeGenesis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/GazeGenesis/ComputerVision/Classification/LeNet/model.py
 src/GazeGenesis/ComputerVision/Classification/LeNet/user.py
 src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/__init__.py
 src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/model.py
 src/GazeGenesis/ComputerVision/Classification/MultiLayerPerceptron/user.py
 src/GazeGenesis/ComputerVision/Classification/ResNet/__init__.py
 src/GazeGenesis/ComputerVision/Classification/ResNet/model.py
+src/GazeGenesis/ComputerVision/Classification/ResNet/user.py
 src/GazeGenesis/ComputerVision/Classification/VGG/__init__.py
 src/GazeGenesis/ComputerVision/Classification/VGG/model.py
 src/GazeGenesis/ComputerVision/Classification/VGG/user.py
 src/GazeGenesis/ComputerVision/Classification/VisionTransformer/__init__.py
 src/GazeGenesis/ComputerVision/Classification/VisionTransformer/model.py
 src/GazeGenesis/ComputerVision/Classification/VisionTransformer/user.py
 src/GazeGenesis/ComputerVision/Datasets/CIFAR10.py
```

