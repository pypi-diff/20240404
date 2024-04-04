# Comparing `tmp/osml-model-runner-test-2.0.0.tar.gz` & `tmp/osml-model-runner-test-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osml-model-runner-test-2.0.0.tar", last modified: Fri Mar  8 20:01:20 2024, max compression
+gzip compressed data, was "osml-model-runner-test-2.0.1.tar", last modified: Thu Apr  4 18:43:13 2024, max compression
```

## Comparing `osml-model-runner-test-2.0.0.tar` & `osml-model-runner-test-2.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.795528 osml-model-runner-test-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-03-08 20:01:20.795528 osml-model-runner-test-2.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3799 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1988 2024-03-08 20:01:20.795528 osml-model-runner-test-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.787528 osml-model-runner-test-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.787528 osml-model-runner-test-2.0.0/src/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.787528 osml-model-runner-test-2.0.0/src/aws/osml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.787528 osml-model-runner-test-2.0.0/src/aws/osml/integ/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/integ/http_centerpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/http_centerpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/http_centerpoint/test_http_centerpoint_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_aircraft/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_aircraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_aircraft/test_sm_aircraft_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_centerpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_centerpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_centerpoint/test_sm_centerpoint_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_flood/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_flood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_flood/test_sm_flood_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/load/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15097 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/load/load_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/process_image/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/process_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/process_image/test_process_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.791528 osml-model-runner-test-2.0.0/src/aws/osml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/utils/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/utils/integ_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-08 20:01:16.000000 osml-model-runner-test-2.0.0/src/aws/osml/utils/osml_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:01:20.795528 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-03-08 20:01:20.000000 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-08 20:01:20.000000 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:01:20.000000 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:01:20.000000 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-08 20:01:20.000000 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-08 20:01:20.000000 osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.298233 osml-model-runner-test-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-04 18:43:13.298233 osml-model-runner-test-2.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4196 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1988 2024-04-04 18:43:13.298233 osml-model-runner-test-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.290233 osml-model-runner-test-2.0.1/src/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/integ/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/integ/http_centerpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/http_centerpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/http_centerpoint/test_http_centerpoint_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_aircraft/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_aircraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_aircraft/test_sm_aircraft_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_centerpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_centerpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_centerpoint/test_sm_centerpoint_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_flood/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_flood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_flood/test_sm_flood_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/load/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15097 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/load/load_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/process_image/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/process_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/process_image/test_process_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.294233 osml-model-runner-test-2.0.1/src/aws/osml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/utils/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25301 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/utils/integ_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-04 18:43:07.000000 osml-model-runner-test-2.0.1/src/aws/osml/utils/osml_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:43:13.298233 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-04 18:43:13.000000 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-04 18:43:13.000000 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:43:13.000000 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:43:13.000000 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 18:43:13.000000 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 18:43:13.000000 osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/top_level.txt
```

### Comparing `osml-model-runner-test-2.0.0/LICENSE` & `osml-model-runner-test-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/README.md` & `osml-model-runner-test-2.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 
 ### Table of Contents
 * [Getting Started](#getting-started)
     * [Prerequisites](#prerequisites)
     * [Installation Guide](#installation-guide)
     * [Documentation](#documentation)
     * [Build and Local Testing](#build-and-local-testing)
-    * [Running Tests in Docker](#running-tests-in-docker)
     * [Running LoadTest](#running-loadtest)
 * [Support & Feedback](#support--feedback)
 * [Security](#security)
 * [License](#license)
 
 
 ## Getting Started
 ### Prerequisites
 
 First, ensure you have installed the following tools locally
 
 1. [aws cli](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
-2. [docker](https://nodejs.org/en)
-3. [tox](https://tox.wiki/en/latest/installation.html)
+2. [tox](https://tox.wiki/en/latest/installation.html)
 
 ### Installation Guide
 
 1. Clone `osml-model-runner-test` package into your desktop
 
 ```sh
 git clone https://github.com/aws-solutions-library-samples/osml-model-runner-test.git
@@ -44,61 +42,63 @@
 You can find documentation for this library in the `./doc` directory. Sphinx is used to construct a searchable HTML
 version of the API documents.
 
 ```shell
 tox -e docs
 ```
 
-### Build and Local Testing
+### Local Testing
 
-You can run the hydra tests against your dev account by exporting the required parameters and using the pytest CLI by
-using the demo utility ``bin/run_test.sh``. Do not forget to load up your AWS credentials into your terminal, please follow this [guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) on how to load your aws credentials.
 
+####  Credentials
 
-```
-export ACCOUNT="INSERT YOUR ACCOUNT"
-export IMAGE_TYPE="INSERT YOUR IMAGE TYPE" # small, medium, large, or tile.<tif|ntf|jpeg|png>
-export MODEL_TYPE="INSERT YOUR MODEL TYPE" # centerpoint, flood, or aircraft
-
-./bin/run_test.sh ${IMAGE_TYPE} ${MODEL_TYPE} NITF JPEG us-west-2 $ACCOUNT_NUMBER
-```
-
-**Examples:**
+Credentials from the user's account are volume mounted into the container's root directory.
 
-```
-./bin/run_test.sh small centerpoint NITF JPEG us-west-2 $ACCOUNT_NUMBER
+**Processing an image:**
 
-./bin/run_test.sh medium flood NITF JPEG us-west-2 $ACCOUNT_NUMBER
+You can run the integration tests against your dev account by exporting the required parameters and using the pytest CLI by
+using the python script ``bin/process_image.py``. Remember to load up your AWS credentials into your terminal, please follow this [guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) on how to load your aws credentials.
 
-./bin/run_test.sh large centerpoint NITF JPEG us-west-2 $ACCOUNT_NUMBER
 
-./bin/run_test.sh tile.tif aircraft NITF JPEG us-west-2 $ACCOUNT_NUMBER
+```
+python bin/process_image.py --image <image type> --model <model type>
 ```
 
-If you prefer, you can execute the python script:
+**Examples:**
 
 ```
 python3 bin/process_image.py --image small --model centerpoint
+
+python3 bin/process_image.py --image meta --model centerpoint
+
+python3 bin/process_image.py --image large --model flood
+
+python3 bin/process_image.py --image tile_tif --model aircraft
 ```
 
 To print out the usage for python script, execute:
 ```
 python3 bin/process_image.py --help
 ```
 
-### Running Tests in Docker
-Arguments can be passed in to docker run in the same way that they are provided to the shell script.
-For example, the container can be built and run as follows:
+To execute the integration test, exclude `--skip_integ` from the command line interface. It is essential that the images and models listed in the table below are aligned accurately for the test to succeed. Conversely, by adding `--skip_integ` to the CLI, all comparison checks will be bypassed, rendering the table irrelevant for testing purposes.
 
-```
-docker build . -t model-runner-hydra-test:latest
-docker run -v ~/.aws:/root/.aws model-runner-hydra-test:latest small centerpoint NITF JPEG us-west-2 $ACCOUNT_NUMBER
-```
-
-Credentials from the user's account are volume mounted into the container's root directory.
+| image                       | model       |
+|-----------------------------|-------------|
+| small                       | centerpoint |
+| meta                        | centerpoint |
+| sicd_capella_chip_ntf       | centerpoint |
+| sicd_umbra_chip_ntf         | centerpoint |
+| sicd_interferometric_hh_ntf | centerpoint |
+| wbid                        | centerpoint |
+| large                       | flood       |
+| tile_tif                    | aircraft    |
+| tile_ntf                    | aircraft    |
+| tile_jpeg                   | aircraft    |
+| tile_png                    | aircraft    |
 
 ### Running LoadTest
 
 You can run the load test against your dev account and be able to determine the cost and the performance. **Please advise** it can potentially rack up your AWS bills!
 
 **Examples:**
 ```
@@ -111,16 +111,16 @@
 python3 bin/run_load_test.py --help
 ```
 
 ## Support & Feedback
 
 To post feedback, submit feature ideas, or report bugs, please use the [Issues](https://github.com/aws-solutions-library-samples/osml-model-runner-test/issues) section of this GitHub repo.
 
-If you are interested in contributing to OversightML Model Runner, see the [CONTRIBUTING](CONTRIBUTING.md) guide.
+If you are interested in contributing to OversightML Model Runner, see the [CONTRIBUTING](https://github.com/aws-solutions-library-samples/osml-model-runner-test/tree/main/CONTRIBUTING.md) guide.
 
 ## Security
 
-See [CONTRIBUTING](CONTRIBUTING.md) for more information.
+See [CONTRIBUTING](https://github.com/aws-solutions-library-samples/osml-model-runner-test/tree/main/CONTRIBUTING.md) for more information.
 
 ## License
 
-MIT No Attribution Licensed. See [LICENSE](LICENSE).
+MIT No Attribution Licensed. See [LICENSE](https://github.com/aws-solutions-library-samples/osml-model-runner-test/tree/main/LICENSE).
```

### Comparing `osml-model-runner-test-2.0.0/setup.cfg` & `osml-model-runner-test-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osml-model-runner-test
-version = 2.0.0
+version = 2.0.1
 description = Package to run tests against osml-model-runner deployments.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Amazon Web Services
 author_email = aws-osml-admin@amazon.com
 license = 
 	MIT No Attribution
```

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/integ/http_centerpoint/test_http_centerpoint_model.py` & `osml-model-runner-test-2.0.1/src/aws/osml/integ/http_centerpoint/test_http_centerpoint_model.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_aircraft/test_sm_aircraft_model.py` & `osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_aircraft/test_sm_aircraft_model.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_centerpoint/test_sm_centerpoint_model.py` & `osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_centerpoint/test_sm_centerpoint_model.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/integ/sm_flood/test_sm_flood_model.py` & `osml-model-runner-test-2.0.1/src/aws/osml/integ/sm_flood/test_sm_flood_model.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/load/load_test.py` & `osml-model-runner-test-2.0.1/src/aws/osml/load/load_test.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/process_image/test_process_image.py` & `osml-model-runner-test-2.0.1/src/aws/osml/process_image/test_process_image.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/utils/__init__.py` & `osml-model-runner-test-2.0.1/src/aws/osml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/utils/clients.py` & `osml-model-runner-test-2.0.1/src/aws/osml/utils/clients.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/utils/integ_utils.py` & `osml-model-runner-test-2.0.1/src/aws/osml/utils/integ_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -315,27 +315,58 @@
     :param expected: Feature we expect to match the result
     :param actual: Feature that was generated by the test
 
     :return: Whether the features match
     """
     actual_pixel_coords = actual.get("properties", {}).get("detection", {}).get("pixelCoordinates")
     expected_pixel_coords = expected.get("properties", {}).get("detection", {}).get("pixelCoordinates")
+
     return (
         expected.type == actual.type
         and expected.geometry == actual.geometry
         and expected_pixel_coords == actual_pixel_coords
         and expected.properties.get("inferenceMetadata") is not None
-        and expected.properties.get("sourceMetadata") == actual.properties.get("sourceMetadata")
+        and source_metadata_equal(expected.properties.get("sourceMetadata"), actual.properties.get("sourceMetadata"))
         and expected.properties.get("featureClasses") == actual.properties.get("featureClasses")
         and expected.properties.get("imageGeometry") == actual.properties.get("imageGeometry")
         and expected.properties.get("center_longitude") == actual.properties.get("center_longitude")
         and expected.properties.get("center_latitude") == actual.properties.get("center_latitude")
     )
 
 
+def source_metadata_equal(expected: List, actual: List) -> bool:
+    """
+    Determines if two lists of source metadata are equal.
+
+    :param expected: List of expected source metadata
+    :param actual: List of actual source metadata
+
+    :return: Whether the lists are equal
+    """
+
+    # Some image(s) may not have source metadata
+    if expected is None and actual is None:
+        return True
+
+    if not len(expected) == len(actual):
+        logging.info(f"Expected {len(expected)} source metadata but found {len(actual)}")
+        return False
+
+    for expected_source_metadata, actual_source_metadata in zip(expected, actual):
+        is_equal = set({"location", "sourceDT"}).issuperset(
+            k for (k, v) in expected_source_metadata.items() ^ actual_source_metadata.items()
+        )
+
+        if not is_equal:
+            logging.info(f"Source metadata {expected_source_metadata} does not match actual {actual_source_metadata}")
+            return False
+
+    return True
+
+
 def feature_collections_equal(expected: List[geojson.Feature], actual: List[geojson.Feature]) -> bool:
     """
     Determines whether the supplied unordered feature lists are equal
 
     :param expected: An unordered list of expected features
     :param actual: An unordered list of detected features
```

### Comparing `osml-model-runner-test-2.0.0/src/aws/osml/utils/osml_config.py` & `osml-model-runner-test-2.0.1/src/aws/osml/utils/osml_config.py`

 * *Files identical despite different names*

### Comparing `osml-model-runner-test-2.0.0/src/osml_model_runner_test.egg-info/SOURCES.txt` & `osml-model-runner-test-2.0.1/src/osml_model_runner_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

