# Comparing `tmp/vmware-cloud-foundation-health-monitoring-2.1.0.1004.tar.gz` & `tmp/vmware-cloud-foundation-health-monitoring-2.1.1.1001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-cloud-foundation-health-monitoring-2.1.0.1004.tar", last modified: Tue Jan 30 16:20:21 2024, max compression
+gzip compressed data, was "vmware-cloud-foundation-health-monitoring-2.1.1.1001.tar", last modified: Thu Apr  4 18:46:16 2024, max compression
```

## Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004.tar` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.990660 vmware-cloud-foundation-health-monitoring-2.1.0.1004/
--rw-rw-rw-   0        0        0     1363 2024-01-09 00:47:14.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/LICENSE
--rw-rw-rw-   0        0        0      429 2024-01-09 00:47:14.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/NOTICE
--rw-rw-rw-   0        0        0    18601 2024-01-30 16:20:20.990660 vmware-cloud-foundation-health-monitoring-2.1.0.1004/PKG-INFO
--rw-rw-rw-   0        0        0    17724 2024-01-18 21:30:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/README.md
--rw-rw-rw-   0        0        0       86 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/pyproject.toml
--rw-rw-rw-   0        0        0     1078 2024-01-30 16:20:21.006287 vmware-cloud-foundation-health-monitoring-2.1.0.1004/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.803156 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.818785 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/
--rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.865659 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/
--rw-rw-rw-   0        0        0   160429 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Alert_Definitions.xml
--rw-rw-rw-   0        0        0    31371 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Dashboards.zip
--rw-rw-rw-   0        0        0    17264 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Supermetrics.json
--rw-rw-rw-   0        0        0    18396 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Views.zip
--rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.881289 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/examples/
--rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/examples/__init__.py
--rwxrwxrwx   0        0        0       55 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/examples/run_send-data-to-vrops.bat
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.928157 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/
--rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/__init__.py
--rw-rw-rw-   0        0        0     2693 2024-01-09 00:47:14.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/encrypt-passwords.py
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.928157 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/encrypted_files/
--rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/encrypted_files/__init__.py
--rw-rw-rw-   0        0        0     1655 2024-01-09 00:47:14.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/env.json
--rw-rw-rw-   0        0        0   129113 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/notifications-template.json
--rw-rw-rw-   0        0        0     4381 2024-01-09 00:47:14.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/notifications.py
--rw-rw-rw-   0        0        0    82457 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/send-data-to-vrops.py
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.975032 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/
--rw-rw-rw-   0        0        0     5364 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/FolderUtility.py
--rw-rw-rw-   0        0        0     3929 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/LogUtility.py
--rw-rw-rw-   0        0        0     2528 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/PSUtility.py
--rw-rw-rw-   0        0        0     6886 2024-01-18 21:29:57.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/SosRest.py
--rw-rw-rw-   0        0        0        0 2023-08-25 20:53:55.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 16:20:20.990660 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/
--rw-rw-rw-   0        0        0    18601 2024-01-30 16:20:20.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-01-30 16:20:20.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-30 16:20:20.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-01-30 16:20:20.000000 vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.717364 vmware-cloud-foundation-health-monitoring-2.1.1.1001/
+-rw-rw-rw-   0        0        0     1368 2024-04-04 18:15:00.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/LICENSE
+-rw-rw-rw-   0        0        0      434 2024-04-04 18:15:00.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/NOTICE
+-rw-rw-rw-   0        0        0    19547 2024-04-04 18:46:16.717364 vmware-cloud-foundation-health-monitoring-2.1.1.1001/PKG-INFO
+-rw-rw-rw-   0        0        0    18670 2024-04-04 18:35:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/pyproject.toml
+-rw-rw-rw-   0        0        0     1078 2024-04-04 18:46:16.732992 vmware-cloud-foundation-health-monitoring-2.1.1.1001/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.561116 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.576737 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.592365 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/
+-rw-rw-rw-   0        0        0   160429 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Alert_Definitions.xml
+-rw-rw-rw-   0        0        0    31502 2024-04-04 18:39:57.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Dashboards.zip
+-rw-rw-rw-   0        0        0    17918 2024-04-04 18:37:03.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Supermetrics.json
+-rw-rw-rw-   0        0        0    18400 2024-04-04 18:22:11.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Views.zip
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.592365 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/examples/__init__.py
+-rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/examples/run_send-data-to-vrops.bat
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.654866 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/__init__.py
+-rw-rw-rw-   0        0        0     2693 2024-01-10 20:39:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypt-passwords.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.654866 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypted_files/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypted_files/__init__.py
+-rw-rw-rw-   0        0        0     1655 2024-01-10 20:39:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/env.json
+-rw-rw-rw-   0        0        0   129113 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications-template.json
+-rw-rw-rw-   0        0        0     4381 2024-01-10 20:39:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications.py
+-rw-rw-rw-   0        0        0    82701 2024-04-04 18:17:29.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/send-data-to-vrops.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.686115 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/
+-rw-rw-rw-   0        0        0     5364 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/FolderUtility.py
+-rw-rw-rw-   0        0        0     3929 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/LogUtility.py
+-rw-rw-rw-   0        0        0     2528 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/PSUtility.py
+-rw-rw-rw-   0        0        0     6886 2024-01-24 16:35:38.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/SosRest.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:46:16.717364 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/
+-rw-rw-rw-   0        0        0    19547 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1002 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-04 18:46:16.000000 vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/LICENSE` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright 2023 Broadcom. All Rights Reserved.
+Copyright 2023-2024 Broadcom. All Rights Reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
    1. Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 2.1.0.1004
+Version: 2.1.1.1001
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Broadcom
 Author-email: bhumitra.nagar@broadcom.com, olga.efremov@broadcom.com
 License: BSD-2-Clause
 Project-URL: Issues, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: Source, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -18,27 +18,37 @@
 
 # Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
 
 ![PyPI](https://img.shields.io/pypi/v/vmware-cloud-foundation-health-monitoring?logo=python&logoColor=yellow&label=PyPI&labelColor=Grey&link=https%3A%2F%2Fpypi.org%2Fproject%2Fvmware-cloud-foundation-health-monitoring%2F)
 &nbsp;&nbsp;
 [![Downloads](https://static.pepy.tech/personalized-badge/vmware-cloud-foundation-health-monitoring?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=DOWNLOADS)](https://pepy.tech/project/vmware-cloud-foundation-health-monitoring) &nbsp;&nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/vmware-cloud-foundation-health-monitoring?period=month&units=international_system&left_color=grey&right_color=green&left_text=DOWNLOADS/WEEK)](https://pepy.tech/project/vmware-cloud-foundation-health-monitoring) &nbsp;&nbsp; [<img src="https://img.shields.io/badge/CHANGELOG-READ-blue?&logo=github&logoColor=white" alt="CHANGELOG" >][changelog]
 
-
 ## Table of Contents
 
-- [Health Reporting and Monitoring for VMware Cloud Foundation](#health-reporting-and-monitoring-vmware-cloud-foundation)
+- [Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations](#python-module-for-vmware-cloud-foundation-health-monitoring-in-vmware-aria-operations)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
   - [Requirements](#requirements)
+    - [Platforms](#platforms)
+    - [Operating Systems](#operating-systems)
+    - [Python Version](#python-version)
+    - [Python Libraries](#python-libraries)
+    - [PowerShell Editions and Versions](#powershell-editions-and-versions)
+    - [PowerShell Modules](#powershell-modules)
   - [Implementation](#implementation)
   - [Install the Python Module in a Disconnected Environment](#install-the-python-module-in-a-disconnected-environment)
+    - [For Photon OS](#for-photon-os)
+    - [For Windows Server](#for-windows-server)
   - [Updating the Python Module to the Latest Version](#updating-the-python-module-to-the-latest-version)
+    - [For Photon OS](#for-photon-os-1)
+    - [For Windows Server](#for-windows-server-1)
   - [VMware Aria Operations Dashboards Preview](#vmware-aria-operations-dashboards-preview)
   - [Known Issues](#known-issues)
   - [Support](#support)
+  - [License](#license)
 
 ## Introduction
 
 This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native VMware Aria Operations dashboards and dashboards that are enabled using the respective management packs.
 
 ## Requirements
 
@@ -59,260 +69,314 @@
 
 Follow the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download) to download and install Python.
 
 ### Python Libraries
 
 Install required Python libraries by running the following commands on the host virtual machine:
 
-  ```python
-  pip install requests
-  pip install setuptools
-  pip install paramiko
-  pip install maskpass==0.3.1
-  ```
+```python
+pip install requests
+pip install setuptools
+pip install paramiko
+pip install maskpass==0.3.1
+```
 
 ### PowerShell Editions and Versions
 
-- Microsoft Windows PowerShell 5.1
 - PowerShell Core 7.2.0 or later
 
 ### PowerShell Modules
 
 - [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) - latest version
 
 ## Implementation
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
 ## Install the Python Module in a Disconnected Environment
-For environments disconnected from the Internet (e.g., dark-site, air-gapped), you can save the Health Reporting and Monitoring Python module and its dependencies from the PyPI using the below instructions. 
 
-### For Photon OS - 
+For disconnected environments (_e.g._, dark-site, air-gapped), you can save the Health Reporting and Monitoring Python module and its dependencies from the PyPI using the below instructions.
+
+### For Photon OS
 
 - On the target system, create a directory to save the Python modules
-```
+
+  ```console
   mkdir -p /opt/vmware/hrm-modules
-```
+  ```
 
-- From a system with an Internet connection, make a modules directory and create a new file `requirements.txt` inside it. 
-```
+- From a system with an Internet connection, make a modules directory and create a new file `requirements.txt` inside it.
+
+  ```console
   mkdir -p /home/hrm-modules/
   cd /home/hrm-modules/
   vi requirements.txt
-```
-- Add below content to the `requirements.txt` file and save it. 
-```
-requests
-setuptools
-paramiko
-maskpass==0.3.1
-```
+  ```
+
+- Add below content to the `requirements.txt` file and save it.
+
+  ```console
+  requests
+  setuptools
+  paramiko
+  maskpass==0.3.1
+  ```
 
 - Create another file `module.txt` in the same location.
-```
+
+  ```console
   vi module.txt
-```
+  ```
   
-- Add below content to the `module.txt` file and save it. 
-```
-vmware-cloud-foundation-health-monitoring
-```
+- Add below content to the `module.txt` file and save it.
+
+  ```console
+  vmware-cloud-foundation-health-monitoring
+  ```
   
 - From a system with an Internet connection, save the module and its dependencies from PyPI by running the following commands in the terminal:
 
-```
+  ```console
   pip download -r module.txt
   pip download -r requirements.txt
-```
+  ```
 
 - From the system with an Internet connection, copy the module and its dependencies to a target system by running the following commands in the terminal:
-```
+
+  ```console
   scp -r /home/vcf/hrm-modules/* username@remote_host:/opt/vmware/hrm-modules/
-```
+  ```
   
 - On the target system, install the module and its dependencies by running the following commands in the terminal:
-```
+
+  ```console
   cd /opt/vmware/hrm-modules
   pip install -r requirements.txt --no-index --find-links .
   pip install -r module.txt --no-index --find-links . -t /opt/vmware/hrm-<sddc_manager_vm_name>
-```
+  ```
 
-### For Windows Server -
+### For Windows Server
 
 - From a system with an Internet connection, make a modules folder `F:\hrm-modules`.
+- Create a new file `requirements.txt` inside the modules folder.
+- Add the below content to the `requirements.txt` file and save it.
 
-- Create a new file `requirements.txt` inside the modules folder. 
+  ```console
+  requests
+  setuptools
+  paramiko
+  maskpass==0.3.1
+  ```
 
-- Add the below content to the `requirements.txt` file and save it. 
-```
-requests
-setuptools
-paramiko
-maskpass==0.3.1
-```
-- In the modules folder `f:\hrm-modules`, create a new file `module.txt` 
-  
-- Add below content to `module.txt` file and save it. 
-```
-vmware-cloud-foundation-health-monitoring
-```
+- In the modules folder `f:\hrm-modules`, create a new file `module.txt`
+- Add below content to `module.txt` file and save it.
+
+  ```console
+  vmware-cloud-foundation-health-monitoring
+  ```
 
 - From a system with an Internet connection, save the module and its dependencies from PyPI by running the following commands from cmdline:
 
-```
+  ```console
   cd f:\hrm-modules
   pip download -r module.txt 
   pip download -r requirements.txt
-```
+  ```
 
 - From the system with the Internet connection, copy the module and its dependencies to a target system by running the following commands in the PowerShell console:
 
-```
+  ```powershell
   Copy-Item -Path F:\hrm-modules\* -Destination '\\<destination_host>\C$\vmware\hrm-modules
-```
+  ```
 
 - On the target system, install the module and its dependencies by running the following commands in the terminal:
-```
+
+  ```console
   cd c:\vmware\hrm-modules
   pip install -r requirements.txt --no-index --find-links .
   pip install -r module.txt --no-index --find-links . -t c:\vmware\hrm-<sddc_manager_vm_name>
-```
-
+  ```
 
 **Once the Python modules are installed, continue to follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)**
 
 ## Updating the Python Module to the Latest Version
 
-### For Photon OS - 
+### For Photon OS
 
 - Log in to the host virtual machine at `<host_virtual_machine_fqdn>:22` as the `root` user by using a Secure Shell (SSH) client.
 
 - Update the Python Module for Health Reporting and Monitoring in VMware Aria Operations.
-```
+
+  ```console
   pip install vmware-cloud-foundation-health-monitoring --target=/opt/vmware/hrm-<sddc_manager_vm_name> --upgrade
-```  
+  ```  
+
 - Provide execute permissions to the files in the `hrm-<sddc_manager_vm_name>` directory.
-```
+
+  ```console
   chmod -R 755 /opt/vmware/hrm-<sddc_manager_vm_name>
-```  
+  ```  
+
 - Switch to the `hrm-<sddc_manager_vm_name>/main` directory.
-```
+
+  ```console
   cd /opt/vmware/hrm-<sddc_manager_vm_name>/main
-```
+  ```
+
 - Edit the `env.json` file and configure the values according to your VMware Cloud Foundation Planning and Preparation Workbook.
-```
+
+  ```console
   vi env.json
-```
+  ```
+
 - Encrypt the service account passwords.
-```
+
+  ```console
   python encrypt-passwords.py
-```
+  ```
+
 - Enter the password for the VMware Aria Operations service account.
 - Enter the password for the SDDC Manager service account.
 - Enter the password for the SDDC Manager appliance local user.
 - Repeat this procedure for each VMware Cloud Foundation instance.
 
-
-### For Windows Server - 
+### For Windows Server
 
 - Log in to the host virtual machine at `<host_virtual_machine_fqdn>` as the `Administrator` user by using a Remote Desktop Connection (RDC) client and open a PowerShell console.
 - Start Windows Command Prompt.
 - Update the Python Module for Health Reporting and Monitoring in VMware Aria Operations.
-```
+
+  ```console
   pip install vmware-cloud-foundation-health-monitoring --target=C:\vmware\hrm-<sddc_manager_vm_name>\ --upgrade
-```
- 
+  ```
+
 - Change to the `hrm-<sddc_manager_vm_name>\main` folder.
-```
+
+  ```console
   cd c:\vmware\hrm-<sddc_manager_vm_name>\main
-```
+  ```
+
 - Edit the `env.json` file and configure the values according to your VMware Cloud Foundation Planning and Preparation Workbook.
-```
+
+  ```console
   notepad env.json
-```
+  ```
+
 - Encrypt the service account passwords.
-```
+
+  ```console
   python encrypt-passwords.py
-```
+  ```
+
 - Enter the password for the VMware Aria Operations service account.
 - Enter the password for the SDDC Manager service account.
 - Enter the password for the SDDC Manager appliance local user.
 - Repeat this procedure for each VMware Cloud Foundation instance.
 
 ## VMware Aria Operations Dashboards Preview
 
 1. VCF Health Rollup
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
 
 2. VCF Backup Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
 
 3. VCF Certificate Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
 
 4. VCF Compute Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
 
 5. VCF Connectivity Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
 
 6. VCF DNS Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
 
 7. VCF Hardware Compatibility
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
 
 8. VCF Networking Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
 
 9. VCF NTP Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
 
 10. VCF Password Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
 
 11. VCF SDDC Manager and vCenter Services Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
 
 12. VCF Snapshot Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
 
 13. VCF Storage Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage2-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/connected-roms-min.png)
 
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/connected-roms-min.png)
 
 14. VCF vSAN Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
 
 15. VCF Version Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/version-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/version-min.png)
 
 ## Known Issues
 
 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in VMware Aria Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
     Please make sure that your NSX-T account name is configured as mentioned in this issue.
 
-2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the VMware Aria Operations dashboards depend on the name.
+2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.x. The filters on the VMware Aria Operations dashboards depend on the name.
 
     To set the Product Name for the vCenter Server, follow the below steps:
 
     1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
     2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
     3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
     4. In the `Settings` pane select `vApp Options`.
@@ -339,15 +403,15 @@
 
 - A reproducible test case or series of steps.
 - Any modifications you've made relevant to the bug.
 - Anything unusual about your environment or deployment.
 
 ## License
 
-Copyright 2023 Broadcom. All Rights Reserved.
+Copyright 2023-2024 Broadcom. All Rights Reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/README.md` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,54 @@
+Metadata-Version: 2.1
+Name: vmware-cloud-foundation-health-monitoring
+Version: 2.1.1.1001
+Summary: Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
+Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
+Author: Broadcom
+Author-email: bhumitra.nagar@broadcom.com, olga.efremov@broadcom.com
+License: BSD-2-Clause
+Project-URL: Issues, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
+Project-URL: Source, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 # Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
 
 ![PyPI](https://img.shields.io/pypi/v/vmware-cloud-foundation-health-monitoring?logo=python&logoColor=yellow&label=PyPI&labelColor=Grey&link=https%3A%2F%2Fpypi.org%2Fproject%2Fvmware-cloud-foundation-health-monitoring%2F)
 &nbsp;&nbsp;
 [![Downloads](https://static.pepy.tech/personalized-badge/vmware-cloud-foundation-health-monitoring?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=DOWNLOADS)](https://pepy.tech/project/vmware-cloud-foundation-health-monitoring) &nbsp;&nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/vmware-cloud-foundation-health-monitoring?period=month&units=international_system&left_color=grey&right_color=green&left_text=DOWNLOADS/WEEK)](https://pepy.tech/project/vmware-cloud-foundation-health-monitoring) &nbsp;&nbsp; [<img src="https://img.shields.io/badge/CHANGELOG-READ-blue?&logo=github&logoColor=white" alt="CHANGELOG" >][changelog]
 
-
 ## Table of Contents
 
-- [Health Reporting and Monitoring for VMware Cloud Foundation](#health-reporting-and-monitoring-vmware-cloud-foundation)
+- [Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations](#python-module-for-vmware-cloud-foundation-health-monitoring-in-vmware-aria-operations)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
   - [Requirements](#requirements)
+    - [Platforms](#platforms)
+    - [Operating Systems](#operating-systems)
+    - [Python Version](#python-version)
+    - [Python Libraries](#python-libraries)
+    - [PowerShell Editions and Versions](#powershell-editions-and-versions)
+    - [PowerShell Modules](#powershell-modules)
   - [Implementation](#implementation)
   - [Install the Python Module in a Disconnected Environment](#install-the-python-module-in-a-disconnected-environment)
+    - [For Photon OS](#for-photon-os)
+    - [For Windows Server](#for-windows-server)
   - [Updating the Python Module to the Latest Version](#updating-the-python-module-to-the-latest-version)
+    - [For Photon OS](#for-photon-os-1)
+    - [For Windows Server](#for-windows-server-1)
   - [VMware Aria Operations Dashboards Preview](#vmware-aria-operations-dashboards-preview)
   - [Known Issues](#known-issues)
   - [Support](#support)
+  - [License](#license)
 
 ## Introduction
 
 This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native VMware Aria Operations dashboards and dashboards that are enabled using the respective management packs.
 
 ## Requirements
 
@@ -41,260 +69,314 @@
 
 Follow the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download) to download and install Python.
 
 ### Python Libraries
 
 Install required Python libraries by running the following commands on the host virtual machine:
 
-  ```python
-  pip install requests
-  pip install setuptools
-  pip install paramiko
-  pip install maskpass==0.3.1
-  ```
+```python
+pip install requests
+pip install setuptools
+pip install paramiko
+pip install maskpass==0.3.1
+```
 
 ### PowerShell Editions and Versions
 
-- Microsoft Windows PowerShell 5.1
 - PowerShell Core 7.2.0 or later
 
 ### PowerShell Modules
 
 - [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) - latest version
 
 ## Implementation
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
 ## Install the Python Module in a Disconnected Environment
-For environments disconnected from the Internet (e.g., dark-site, air-gapped), you can save the Health Reporting and Monitoring Python module and its dependencies from the PyPI using the below instructions. 
 
-### For Photon OS - 
+For disconnected environments (_e.g._, dark-site, air-gapped), you can save the Health Reporting and Monitoring Python module and its dependencies from the PyPI using the below instructions.
+
+### For Photon OS
 
 - On the target system, create a directory to save the Python modules
-```
+
+  ```console
   mkdir -p /opt/vmware/hrm-modules
-```
+  ```
 
-- From a system with an Internet connection, make a modules directory and create a new file `requirements.txt` inside it. 
-```
+- From a system with an Internet connection, make a modules directory and create a new file `requirements.txt` inside it.
+
+  ```console
   mkdir -p /home/hrm-modules/
   cd /home/hrm-modules/
   vi requirements.txt
-```
-- Add below content to the `requirements.txt` file and save it. 
-```
-requests
-setuptools
-paramiko
-maskpass==0.3.1
-```
+  ```
+
+- Add below content to the `requirements.txt` file and save it.
+
+  ```console
+  requests
+  setuptools
+  paramiko
+  maskpass==0.3.1
+  ```
 
 - Create another file `module.txt` in the same location.
-```
+
+  ```console
   vi module.txt
-```
+  ```
   
-- Add below content to the `module.txt` file and save it. 
-```
-vmware-cloud-foundation-health-monitoring
-```
+- Add below content to the `module.txt` file and save it.
+
+  ```console
+  vmware-cloud-foundation-health-monitoring
+  ```
   
 - From a system with an Internet connection, save the module and its dependencies from PyPI by running the following commands in the terminal:
 
-```
+  ```console
   pip download -r module.txt
   pip download -r requirements.txt
-```
+  ```
 
 - From the system with an Internet connection, copy the module and its dependencies to a target system by running the following commands in the terminal:
-```
+
+  ```console
   scp -r /home/vcf/hrm-modules/* username@remote_host:/opt/vmware/hrm-modules/
-```
+  ```
   
 - On the target system, install the module and its dependencies by running the following commands in the terminal:
-```
+
+  ```console
   cd /opt/vmware/hrm-modules
   pip install -r requirements.txt --no-index --find-links .
   pip install -r module.txt --no-index --find-links . -t /opt/vmware/hrm-<sddc_manager_vm_name>
-```
+  ```
 
-### For Windows Server -
+### For Windows Server
 
 - From a system with an Internet connection, make a modules folder `F:\hrm-modules`.
+- Create a new file `requirements.txt` inside the modules folder.
+- Add the below content to the `requirements.txt` file and save it.
 
-- Create a new file `requirements.txt` inside the modules folder. 
+  ```console
+  requests
+  setuptools
+  paramiko
+  maskpass==0.3.1
+  ```
 
-- Add the below content to the `requirements.txt` file and save it. 
-```
-requests
-setuptools
-paramiko
-maskpass==0.3.1
-```
-- In the modules folder `f:\hrm-modules`, create a new file `module.txt` 
-  
-- Add below content to `module.txt` file and save it. 
-```
-vmware-cloud-foundation-health-monitoring
-```
+- In the modules folder `f:\hrm-modules`, create a new file `module.txt`
+- Add below content to `module.txt` file and save it.
+
+  ```console
+  vmware-cloud-foundation-health-monitoring
+  ```
 
 - From a system with an Internet connection, save the module and its dependencies from PyPI by running the following commands from cmdline:
 
-```
+  ```console
   cd f:\hrm-modules
   pip download -r module.txt 
   pip download -r requirements.txt
-```
+  ```
 
 - From the system with the Internet connection, copy the module and its dependencies to a target system by running the following commands in the PowerShell console:
 
-```
+  ```powershell
   Copy-Item -Path F:\hrm-modules\* -Destination '\\<destination_host>\C$\vmware\hrm-modules
-```
+  ```
 
 - On the target system, install the module and its dependencies by running the following commands in the terminal:
-```
+
+  ```console
   cd c:\vmware\hrm-modules
   pip install -r requirements.txt --no-index --find-links .
   pip install -r module.txt --no-index --find-links . -t c:\vmware\hrm-<sddc_manager_vm_name>
-```
-
+  ```
 
 **Once the Python modules are installed, continue to follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)**
 
 ## Updating the Python Module to the Latest Version
 
-### For Photon OS - 
+### For Photon OS
 
 - Log in to the host virtual machine at `<host_virtual_machine_fqdn>:22` as the `root` user by using a Secure Shell (SSH) client.
 
 - Update the Python Module for Health Reporting and Monitoring in VMware Aria Operations.
-```
+
+  ```console
   pip install vmware-cloud-foundation-health-monitoring --target=/opt/vmware/hrm-<sddc_manager_vm_name> --upgrade
-```  
+  ```  
+
 - Provide execute permissions to the files in the `hrm-<sddc_manager_vm_name>` directory.
-```
+
+  ```console
   chmod -R 755 /opt/vmware/hrm-<sddc_manager_vm_name>
-```  
+  ```  
+
 - Switch to the `hrm-<sddc_manager_vm_name>/main` directory.
-```
+
+  ```console
   cd /opt/vmware/hrm-<sddc_manager_vm_name>/main
-```
+  ```
+
 - Edit the `env.json` file and configure the values according to your VMware Cloud Foundation Planning and Preparation Workbook.
-```
+
+  ```console
   vi env.json
-```
+  ```
+
 - Encrypt the service account passwords.
-```
+
+  ```console
   python encrypt-passwords.py
-```
+  ```
+
 - Enter the password for the VMware Aria Operations service account.
 - Enter the password for the SDDC Manager service account.
 - Enter the password for the SDDC Manager appliance local user.
 - Repeat this procedure for each VMware Cloud Foundation instance.
 
-
-### For Windows Server - 
+### For Windows Server
 
 - Log in to the host virtual machine at `<host_virtual_machine_fqdn>` as the `Administrator` user by using a Remote Desktop Connection (RDC) client and open a PowerShell console.
 - Start Windows Command Prompt.
 - Update the Python Module for Health Reporting and Monitoring in VMware Aria Operations.
-```
+
+  ```console
   pip install vmware-cloud-foundation-health-monitoring --target=C:\vmware\hrm-<sddc_manager_vm_name>\ --upgrade
-```
- 
+  ```
+
 - Change to the `hrm-<sddc_manager_vm_name>\main` folder.
-```
+
+  ```console
   cd c:\vmware\hrm-<sddc_manager_vm_name>\main
-```
+  ```
+
 - Edit the `env.json` file and configure the values according to your VMware Cloud Foundation Planning and Preparation Workbook.
-```
+
+  ```console
   notepad env.json
-```
+  ```
+
 - Encrypt the service account passwords.
-```
+
+  ```console
   python encrypt-passwords.py
-```
+  ```
+
 - Enter the password for the VMware Aria Operations service account.
 - Enter the password for the SDDC Manager service account.
 - Enter the password for the SDDC Manager appliance local user.
 - Repeat this procedure for each VMware Cloud Foundation instance.
 
 ## VMware Aria Operations Dashboards Preview
 
 1. VCF Health Rollup
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
 
 2. VCF Backup Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
 
 3. VCF Certificate Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
 
 4. VCF Compute Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
 
 5. VCF Connectivity Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
 
 6. VCF DNS Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
 
 7. VCF Hardware Compatibility
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
 
 8. VCF Networking Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
 
 9. VCF NTP Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
 
 10. VCF Password Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
 
 11. VCF SDDC Manager and vCenter Services Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
 
 12. VCF Snapshot Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
 
 13. VCF Storage Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage2-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/connected-roms-min.png)
 
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/connected-roms-min.png)
 
 14. VCF vSAN Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
 
 15. VCF Version Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/version-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/version-min.png)
 
 ## Known Issues
 
 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in VMware Aria Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
     Please make sure that your NSX-T account name is configured as mentioned in this issue.
 
-2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the VMware Aria Operations dashboards depend on the name.
+2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.x. The filters on the VMware Aria Operations dashboards depend on the name.
 
     To set the Product Name for the vCenter Server, follow the below steps:
 
     1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
     2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
     3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
     4. In the `Settings` pane select `vApp Options`.
@@ -321,15 +403,15 @@
 
 - A reproducible test case or series of steps.
 - Any modifications you've made relevant to the bug.
 - Anything unusual about your environment or deployment.
 
 ## License
 
-Copyright 2023 Broadcom. All Rights Reserved.
+Copyright 2023-2024 Broadcom. All Rights Reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/setup.cfg` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6d77 6172 652d 636c 6f75 642d   = vmware-cloud-
 00000020: 666f 756e 6461 7469 6f6e 2d68 6561 6c74  foundation-healt
 00000030: 682d 6d6f 6e69 746f 7269 6e67 0d0a 7665  h-monitoring..ve
-00000040: 7273 696f 6e20 3d20 322e 312e 302e 3130  rsion = 2.1.0.10
-00000050: 3034 0d0a 6175 7468 6f72 203d 2042 726f  04..author = Bro
+00000040: 7273 696f 6e20 3d20 322e 312e 312e 3130  rsion = 2.1.1.10
+00000050: 3031 0d0a 6175 7468 6f72 203d 2042 726f  01..author = Bro
 00000060: 6164 636f 6d0d 0a61 7574 686f 725f 656d  adcom..author_em
 00000070: 6169 6c20 3d20 6268 756d 6974 7261 2e6e  ail = bhumitra.n
 00000080: 6167 6172 4062 726f 6164 636f 6d2e 636f  agar@broadcom.co
 00000090: 6d2c 206f 6c67 612e 6566 7265 6d6f 7640  m, olga.efremov@
 000000a0: 6272 6f61 6463 6f6d 2e63 6f6d 0d0a 6465  broadcom.com..de
 000000b0: 7363 7269 7074 696f 6e20 3d20 5079 7468  scription = Pyth
 000000c0: 6f6e 204d 6f64 756c 6520 666f 7220 564d  on Module for VM
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Alert_Definitions.xml` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Alert_Definitions.xml`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Supermetrics.json` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Supermetrics.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8246173469387753%*

 * *Differences: {"'072d0b10-9dbe-4c4f-92e2-12026bfab7b5'": "{'modificationTime': 1711063932961, 'modifiedBy': "*

 * *                                           "'48cb73fe-ebce-4d0c-870c-eb9fed3192bc'}",*

 * * "'2063f4b6-fbf1-4258-9c5c-dc4d20057e3e'": "{'resourceKinds': {delete: [0]}, 'modificationTime': "*

 * *                                           "1712178345261, 'description': 'HRM Snapshots status', "*

 * *                                           "'modifiedBy': '48cb73fe-ebce-4d0c-870c-eb9fed3192bc'}",*

 * * "'21073512-e5f4-4841-a231-93f6 […]*

```diff
@@ -1,361 +1,391 @@
 {
     "072d0b10-9dbe-4c4f-92e2-12026bfab7b5": {
         "description": "SOS General for NSX",
         "formula": "max(${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS General|alert_code, depth=8})\n",
-        "modificationTime": 1699402159707,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063932961,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM General NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "2063f4b6-fbf1-4258-9c5c-dc4d20057e3e": {
-        "description": "HRM Backups status",
+        "description": "HRM Snapshots status",
         "formula": "max([max(${adaptertype=VMWARE, objecttype=*, attribute=HRM Snapshot Status|alert_code, depth=8}), max(${this, attribute=HRM Snapshot Status|alert_code, depth=8})])",
-        "modificationTime": 1699402159725,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1712178345261,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Snapshots health",
         "resourceKinds": [
             {
-                "adapterKindKey": "NSXTAdapter",
-                "resourceKindKey": "NSXTAdapterInstance"
-            },
-            {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "21073512-e5f4-4841-a231-93f6c6f962df": {
         "description": "SOS Compute for VC",
         "formula": "max([${adaptertype=VMWARE, objecttype=*, attribute=SOS Compute Summary|alert_code, depth=8}, ${adaptertype=VMWARE, objecttype=*, attribute=HRM ESXi Connection Health Status|alert_code, depth=8}, ${adaptertype=VMWARE, objecttype=*, attribute=HRM SDDC Free Pool Status|alert_code, depth=8}])",
-        "modificationTime": 1705103746333,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933264,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Compute vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "231aa5a2-8e8f-4c2e-9306-80f5c17c904e": {
         "description": "SOS Connectivity for VC adapter",
         "formula": "max([${adaptertype=VMWARE, objecttype=*, attribute=SOS Ping status|alert_code, depth=8}, ${adaptertype=VMWARE, objecttype=*, attribute=SOS SSH Connectivity status|alert_code, depth=8},${adaptertype=VMWARE, objecttype=*, attribute=SOS API Connectivity status|alert_code, depth=8}] )\n",
-        "modificationTime": 1699402159786,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933042,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Connectivity vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "3643068c-3bc6-475b-bbfa-45a6ae46be3c": {
         "description": "SOS certificates for NSX",
         "formula": "max(${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS Certificate Health Summary|alert_code, depth=8})",
-        "modificationTime": 1699402159731,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933209,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Certificates NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "3d5c46d3-dc1f-4503-8b6d-fa1d575044f1": {
         "description": "Rollup Metric for all VC adapter instances under the VCF world - Management or Workload",
         "formula": "max([${adaptertype=VMWARE, objecttype=VMwareAdapter Instance, attribute=Super Metric|sm_649ff777-2e13-4449-bff8-5dddd852f55d, depth=1}, ${adaptertype=NSXTAdapter, objecttype=NSXTAdapterInstance, metric=Super Metric|sm_d0782eb2-26e1-419b-be30-227a10c8007f, depth=1}])",
-        "modificationTime": 1699402159822,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933106,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM VCF World Status",
         "resourceKinds": [
             {
                 "adapterKindKey": "VcfAdapter",
                 "resourceKindKey": "VCFDomain"
             }
         ],
         "unitId": ""
     },
     "41c1eeb2-0ed3-4bf9-a2d1-4aa8a45bd540": {
         "description": "HRM Rollup metric for all metrics collected in a cluster",
         "formula": "max([${this, metric=Super Metric|sm_aea41667-8725-48da-b05b-7dc51f11a6f8}, ${this, metric=Super Metric|sm_56d2aa1b-e4ea-4904-b41a-b7f1569f8e06}\n,${this, metric=Super Metric|sm_f71d9b18-11fc-4849-b4e6-17217fc788c5}, ${this, metric=Super Metric|sm_4a1613d9-287c-40ea-8a70-4b7cb97ee59f}, ${this, metric=Super Metric|sm_e13931f6-068e-41a1-9538-6b288646b062},${this, metric=Super Metric|sm_21073512-e5f4-4841-a231-93f6c6f962df},${this, metric=Super Metric|sm_231aa5a2-8e8f-4c2e-9306-80f5c17c904e},${this, metric=Super Metric|sm_6794b888-f44c-444d-bb61-f420a29a9376},${this, metric=Super Metric|sm_81066432-d8c8-47e4-a138-fa989db62c64}, ${this, metric=Super Metric|sm_87f97f01-8892-4fc8-947e-bee3d8d3917f},${this, metric=Super Metric|sm_4a1de09e-84d7-49b6-b76a-d3926dd63686}, ${this, metric=Super Metric|sm_2063f4b6-fbf1-4258-9c5c-dc4d20057e3e}, ${this, metric=Super Metric|sm_d63f9eab-f990-4a82-aa19-e86c9fe61056}, ${this, metric=Super Metric|sm_eb94e7c6-7d73-4de2-bc1c-f947681a2114}])",
-        "modificationTime": 1705105974080,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063932930,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Cluster Overall Status",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
+    "46ee1bfb-27b6-459f-bfd4-f262bbec440d": {
+        "description": "HRM Backups status",
+        "formula": "max(${this, attribute=HRM Backup Status|alert_code, depth=4}) ",
+        "modificationTime": 1712176766881,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
+        "name": "SM Backups status NSX",
+        "resourceKinds": [
+            {
+                "adapterKindKey": "NSXTAdapter",
+                "resourceKindKey": "NSXTAdapterInstance"
+            }
+        ],
+        "unitId": ""
+    },
     "4a1613d9-287c-40ea-8a70-4b7cb97ee59f": {
         "description": "SOS Password status for vcadapter object types",
         "formula": "max(${adaptertype=VMWARE, objecttype=*, attribute=SOS Password Summary|alert_code, depth=8})",
-        "modificationTime": 1699402159792,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933058,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Passwords vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "4a1de09e-84d7-49b6-b76a-d3926dd63686": {
         "description": "HRM Backups status",
         "formula": "max([max(${adaptertype=VMWARE, objecttype=*, attribute=HRM Backup Status|alert_code, depth=8}), max(${this, attribute=HRM Backup Status|alert_code, depth=4})])",
-        "modificationTime": 1699402159719,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1712176838070,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Backups status",
         "resourceKinds": [
             {
-                "adapterKindKey": "NSXTAdapter",
-                "resourceKindKey": "NSXTAdapterInstance"
-            },
-            {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
+    "56ae79bd-f05e-4ce0-8995-ac5ecb7c6991": {
+        "description": "HRM Snapshot status for nsx",
+        "formula": "max(${this, attribute=HRM Snapshot Status|alert_code, depth=8})",
+        "modificationTime": 1712178335987,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
+        "name": "SM Snapshots Health NSX",
+        "resourceKinds": [
+            {
+                "adapterKindKey": "NSXTAdapter",
+                "resourceKindKey": "NSXTAdapterInstance"
+            }
+        ],
+        "unitId": ""
+    },
     "56d2aa1b-e4ea-4904-b41a-b7f1569f8e06": {
         "description": "SOS DNS status for vcdapter object types",
         "formula": "max([max(${adaptertype=VMWARE, objecttype=*, attribute=SOS DNS Forward lookup Status Summary|alert_code, depth=8}), max(${adaptertype=VMWARE, objecttype=*, attribute=SOS DNS Reverse lookup Status Summary|alert_code, depth=8})])",
-        "modificationTime": 1699402159810,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933356,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM DNS status",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "649ff777-2e13-4449-bff8-5dddd852f55d": {
         "description": "HRM rollup metric for all datacenters in the vCenter ",
         "formula": "max(${adaptertype=VMWARE, objecttype=Datacenter, attribute=Super Metric|sm_7a281938-e3ff-422c-a049-57ecd0818696, depth=1})",
-        "modificationTime": 1699402159762,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933008,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM vCenter Status",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "VMwareAdapter Instance"
             }
         ],
         "unitId": ""
     },
     "6794b888-f44c-444d-bb61-f420a29a9376": {
         "description": "SOS General for VCadapter",
         "formula": "max(${adaptertype=VMWARE, objecttype=*, attribute=SOS General|alert_code, depth=8})\n",
-        "modificationTime": 1699402159780,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933320,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM General vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "7a281938-e3ff-422c-a049-57ecd0818696": {
         "description": "HRM Rollup metric for all clusters in a datacenter",
         "formula": "max(${adaptertype=VMWARE, objecttype=ClusterComputeResource, attribute=Super Metric|sm_41c1eeb2-0ed3-4bf9-a2d1-4aa8a45bd540, depth=3})",
-        "modificationTime": 1699402159798,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933074,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Datacenter status",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "Datacenter"
             }
         ],
         "unitId": ""
     },
     "81066432-d8c8-47e4-a138-fa989db62c64": {
         "description": "SOS vSAN status",
         "formula": "max([max(${adaptertype=VMWARE, objecttype=*, attribute=SOS vSAN Summary|alert_code, depth=8}), max(${this, attribute=SOS vSAN Summary|alert_code})])",
-        "modificationTime": 1699402159685,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933174,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM vSAN vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "86e09c35-a0d1-4842-acf9-89fd360f3943": {
         "description": "SOS DNS status for NSX",
         "formula": "max([max(${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS DNS Forward lookup Status Summary|alert_code, depth=8}), max(${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS DNS Reverse lookup Status Summary|alert_code, depth=8})])",
-        "modificationTime": 1699402159756,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933281,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM DNS NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "87f97f01-8892-4fc8-947e-bee3d8d3917f": {
         "description": "SOS hardware compatibility ",
         "formula": "max([${this, metric=SOS Hardware Compatibility|Controller disk group mode is VMware certified|alert_code},${this, metric=SOS Hardware Compatibility|Controller driver is VMware certified|alert_code}, ${this, metric=SOS Hardware Compatibility|Controller firmware is VMware certified|alert_code},${this, metric=SOS Hardware Compatibility|Controller is VMware certified for ESXi release|alert_code}, ${this, metric=SOS Hardware Compatibility|SCSI controller is VMware certified|alert_code},${this, metric=SOS Hardware Compatibility|vSAN firmware version recommendation|alert_code},${this, metric=SOS Hardware Compatibility|vSAN HCL DB Auto Update|alert_code},${this, metric=SOS Hardware Compatibility|vSAN HCL DB up-to-date|alert_code}])",
-        "modificationTime": 1699402159828,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933124,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Hardware Compatibility vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "aea41667-8725-48da-b05b-7dc51f11a6f8": {
         "description": "SOS Certificate status for vcdapter object types",
         "formula": "max(${adaptertype=VMWARE, objecttype=*, attribute=SOS Certificate Health Summary|alert_code, depth=8})",
-        "modificationTime": 1699402159736,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933225,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Certificates vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "b2857516-a17b-4b2e-a3f3-e609db101c24": {
         "description": "SOS Password Expiry for NSX",
         "formula": "max(${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS Password Summary|alert_code, depth=8})",
-        "modificationTime": 1699402159713,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063932976,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Passwords NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "c86590e5-daef-4dcd-8cdc-a8cc74d5db0c": {
         "description": "SOS Connectivity for NSX",
         "formula": "max([${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS Ping status|alert_code, depth=8}, ${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS SSH Connectivity status|alert_code, depth=8},${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS API Connectivity status|alert_code, depth=8}] )\n",
-        "modificationTime": 1699402159804,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933337,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Connectivity NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "cf8a23ce-a87a-4e06-8955-27d9ab085405": {
         "description": "SOS NTP status for NSX",
         "formula": "max(${adaptertype=NSXTAdapter, objecttype=*, attribute=SOS NTP Status Summary|alert_code, depth=8})",
-        "modificationTime": 1699402159744,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933243,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM NTP NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "d0782eb2-26e1-419b-be30-227a10c8007f": {
         "description": "HRM overall cluster status for NSX",
-        "formula": "max([${this, metric=Super Metric|sm_3643068c-3bc6-475b-bbfa-45a6ae46be3c},${this, metric=Super Metric|sm_86e09c35-a0d1-4842-acf9-89fd360f3943},${this, metric=Super Metric|sm_cf8a23ce-a87a-4e06-8955-27d9ab085405},${this, metric=Super Metric|sm_b2857516-a17b-4b2e-a3f3-e609db101c24},${this, metric=Super Metric|sm_072d0b10-9dbe-4c4f-92e2-12026bfab7b5},${this, metric=Super Metric|sm_c86590e5-daef-4dcd-8cdc-a8cc74d5db0c},${this, metric=Super Metric|sm_4a1de09e-84d7-49b6-b76a-d3926dd63686}, ${this, metric=Super Metric|sm_2063f4b6-fbf1-4258-9c5c-dc4d20057e3e}, ${this, metric=Super Metric|sm_eb94e7c6-7d73-4de2-bc1c-f947681a2114}])",
-        "modificationTime": 1705105931073,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "formula": "max([${this, metric=Super Metric|sm_3643068c-3bc6-475b-bbfa-45a6ae46be3c},${this, metric=Super Metric|sm_86e09c35-a0d1-4842-acf9-89fd360f3943},${this, metric=Super Metric|sm_cf8a23ce-a87a-4e06-8955-27d9ab085405},${this, metric=Super Metric|sm_b2857516-a17b-4b2e-a3f3-e609db101c24},${this, metric=Super Metric|sm_072d0b10-9dbe-4c4f-92e2-12026bfab7b5},${this, metric=Super Metric|sm_c86590e5-daef-4dcd-8cdc-a8cc74d5db0c},${this, metric=Super Metric|sm_46ee1bfb-27b6-459f-bfd4-f262bbec440d}, ${this, metric=Super Metric|sm_56ae79bd-f05e-4ce0-8995-ac5ecb7c6991}, ${this, metric=Super Metric|sm_e2e1dda7-c51c-469d-983d-653e4bc6ad82}])",
+        "modificationTime": 1712177286772,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM NSX overall status",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
             }
         ],
         "unitId": ""
     },
     "d63f9eab-f990-4a82-aa19-e86c9fe61056": {
         "description": "HRM Storage Capacity",
         "formula": "max([max(${adaptertype=VMWARE, objecttype=*, attribute=HRM StorageCapacityHealth Status|alert_code, depth=8}), max(${adaptertype=VMWARE, objecttype=*, attribute=HRM StorageCapacityDatatoreHealth Status|alert_code, depth=8}), max(${adaptertype=VMWARE, objecttype=*, attribute=HRM StorageCapacityFilesystemHealth Status|alert_code, depth=8}), max(${adaptertype=VMWARE, objecttype=*, attribute=HRM VM Connected CDROM Status|alert_code, depth=8})])",
-        "modificationTime": 1705102333934,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933302,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Storage Capacity",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "e13931f6-068e-41a1-9538-6b288646b062": {
         "description": "SOS Services status for vcadapter object types",
         "formula": "max(${adaptertype=VMWARE, objecttype=*, attribute=SOS Services Summary|alert_code, depth=8})",
-        "modificationTime": 1699402159817,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933090,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM Services vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
-    "eb94e7c6-7d73-4de2-bc1c-f947681a2114": {
+    "e2e1dda7-c51c-469d-983d-653e4bc6ad82": {
         "description": "SOS Version Health",
-        "formula": "max(${adaptertype=VMWARE, objecttype=*, attribute=SOS Version Health Summary|alert_code, depth=8})",
-        "modificationTime": 1705104291140,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
-        "name": "SM Version Health",
+        "formula": "max(${this, attribute=SOS Version Health Summary|alert_code, depth=8})",
+        "modificationTime": 1712177053825,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
+        "name": "SM Version Health NSX",
         "resourceKinds": [
             {
                 "adapterKindKey": "NSXTAdapter",
                 "resourceKindKey": "NSXTAdapterInstance"
-            },
+            }
+        ],
+        "unitId": ""
+    },
+    "eb94e7c6-7d73-4de2-bc1c-f947681a2114": {
+        "description": "SOS Version Health",
+        "formula": "max(${adaptertype=VMWARE, objecttype=*, attribute=SOS Version Health Summary|alert_code, depth=8})",
+        "modificationTime": 1712176903895,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
+        "name": "SM Version Health",
+        "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
         "unitId": ""
     },
     "f71d9b18-11fc-4849-b4e6-17217fc788c5": {
         "description": "SOS NTP status for vcdapter object types",
         "formula": "max([max(${adaptertype=VMWARE, objecttype=*, attribute=SOS NTP Status Summary|alert_code, depth=8}), max(${adaptertype=VMWARE, objecttype=*, attribute=SOS ESXi Time Status Summary|alert_code, depth=8})])\n",
-        "modificationTime": 1705103934778,
-        "modifiedBy": "8dbd1889-d8fd-4475-a63b-358e04053750",
+        "modificationTime": 1711063933158,
+        "modifiedBy": "48cb73fe-ebce-4d0c-870c-eb9fed3192bc",
         "name": "SM NTP vcadapter",
         "resourceKinds": [
             {
                 "adapterKindKey": "VMWARE",
                 "resourceKindKey": "ClusterComputeResource"
             }
         ],
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/artifacts/vSAN/Views.zip` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/artifacts/vSAN/Views.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
-Zip file size: 18396 bytes, number of entries: 1
--rw-a--     2.0 fat   570039 t- defN 24-Jan-13 00:53 content.xml
-1 file, 570039 bytes uncompressed, 18276 bytes compressed:  96.8%
+Zip file size: 18400 bytes, number of entries: 1
+-rw-a--     2.0 fat   570045 t- defN 24-Apr-04 19:21 content.xml
+1 file, 570045 bytes uncompressed, 18280 bytes compressed:  96.8%
```

#### content.xml

##### content.xml

```diff
@@ -4624,15 +4624,15 @@
                   <Property name="addTimestampAsColumn" value="false"/>
                   <Property name="isShowRelativeTimestamp" value="false"/>
                 </Value>
               </Item>
               <Item>
                 <Value>
                   <Property name="objectType" value="RESOURCE"/>
-                  <Property name="attributeKey" value="HRM Backup Status:Cluster Backup Operation|date"/>
+                  <Property name="attributeKey" value="HRM Backup Status:Cluster Backup Operation|date_taken"/>
                   <Property name="isStringAttribute" value="true"/>
                   <Property name="adapterKind" value="NSXTAdapter"/>
                   <Property name="resourceKind" value="NSXTAdapterInstance"/>
                   <Property name="rollUpCount" value="0"/>
                   <Property name="transformations">
                     <List>
                       <Item value="LAST"/>
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/encrypt-passwords.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/encrypt-passwords.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/env.json` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/env.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/notifications-template.json` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications-template.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/notifications.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/notifications.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/send-data-to-vrops.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/send-data-to-vrops.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,27 @@
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from utils.LogUtility import LogUtility
 from utils.FolderUtility import FolderUtility
 from utils.SosRest import SosRest
 from utils.PSUtility import PSUtility
 from cryptography.fernet import Fernet
 
+
 def push_handler(func):
     def inner_function(*args, **kwargs):
         try:
             func(*args, **kwargs)
             args[0].logger.info('############################################################################')
         except Exception as e:
             args[0].logger.error('Exception occurred. Details - ')
             args[0].logger.error(e)
+
     return inner_function
 
+
 class PushDataVrops:
 
     def __init__(self, args):
         os.chdir(os.path.dirname(os.path.abspath(__file__)))
         env_file = args.env_json
         env_info = self.read_data(env_file)
 
@@ -321,15 +324,14 @@
 
         file_name = self.get_complete_json_file_name(self.esxi_connection_status_json)
         self.push_esxi_connection_health(file_name)
 
         file_name = self.get_complete_json_file_name(self.sddc_manager_free_pool_status_json)
         self.push_sddc_manager_free_pool_status(file_name)
 
-
         # pushing data from sos utility health-results.json
         if self.data:
             self.push_data_password()
             self.push_data_certificates()
             self.push_dns_lookup(self.forward_lookup)
             self.push_dns_lookup(self.reverse_lookup)
             self.push_ntp()
@@ -370,18 +372,18 @@
             return 2
         else:
             if self.push_to_vrops:
                 self.vrops.add_stats(metrics_payload_json, id=resource_id)
                 self.logger.info(suc_log_msg)
                 return 0
             else:
-                self.logger.info(f"********************** Will not push '{category}' data to VMware Aria Operations ******************")
+                self.logger.info(
+                    f"********************** Will not push '{category}' data to VMware Aria Operations ******************")
                 return 1
 
-
     @push_handler
     def push_general(self):
         category = "General"
         update_count = 0
         for d, parent_key, prev_keys in self.get_most_nested_dict(self.data[category]):
             if parent_key == "":
                 continue
@@ -1077,15 +1079,15 @@
             hostname = data["vCenter Server"]
             resource_name = data["VM Name"]
             self.logger.info(f'Resource: {resource_name} that recides on hostname {hostname}')
             metrics_payload = {"stat-content": []}
 
             # timestamp_raw = value['timestamp']
             timestamp = time.mktime(datetime.datetime.now().timetuple())
-            
+
             resource_id = self.get_resource_id(hostname, resource_name)
 
             for k, v in data.items():
                 if k.lower() == 'latest':
                     k = "date_taken"
                     if v:
                         match = re.search(r"\d{10}", v)
@@ -1122,15 +1124,14 @@
             self.logger.info(resource_id)
             self.logger.info(metrics_payload_json)
             self.push_data_to_vrops(category, resource_id, hostname, metrics_payload_json)
             update_count = update_count + 1
 
         self.logger.info(f'Total object update requests = {update_count} ')
 
-
     @push_handler
     def push_localuserexpiry_status(self, file_name):
         data_type = "Localuserexpiry"
         datastruct = self.get_complete_json_file_name(file_name)
         update_count = self.push_flat_struct(data_type, datastruct, None)
         self.logger.info(f'Total object update requests = {update_count} ')
 
@@ -1319,15 +1320,15 @@
             self.logger.info(metrics_payload_json)
             self.push_data_to_vrops(category, resource_id, hostname, metrics_payload_json)
             update_count = update_count + 1
 
         self.logger.info(f'Total object update requests = {update_count} ')
 
     @push_handler
-    def push_sddc_manager_free_pool_status (self, file_name):
+    def push_sddc_manager_free_pool_status(self, file_name):
         data_arr = self.read_data(file_name)
         category = "HRM Free Pool Health"
         data_type = "SDDC Free Pool"
         self.logger.info(f'Pushing {data_type} status data to VMware Aria Operations')
         update_count = 0
         for data in data_arr:
             component = data["Component"]
@@ -1659,42 +1660,48 @@
                 update_count = update_count + 1
 
         self.logger.info(f'Total object update requests = {update_count}')
 
     @push_handler
     def push_sddc_versions(self):
         category = "Version Check Status"
-        self.logger.info('Pushing SOS version health check of BOM components (vCenter Server, NSX, ESXi, and SDDC Manager) data to VMware Aria Operations')
+        self.logger.info(
+            'Pushing SOS version health check of BOM components (vCenter Server, NSX, ESXi, and SDDC Manager) data to VMware Aria Operations')
         update_count = 0
         for key, value in self.data[category].items():
             hostname = key.rstrip()
             resource_name = hostname.split(".")[0]
             self.logger.info(f'Hostname = {hostname}')
             metrics_payload = {"stat-content": []}
 
             timestamp_raw = value['timestamp']
             timestamp = time.mktime(datetime.datetime.strptime(timestamp_raw, "%c").timetuple())
             resource_id = self.get_resource_id(hostname, resource_name)
 
             for k, val in value.items():
                 if k == 'title' and val:
+                    try:
+                        title_value = val[0] if type(val[0]) == type("") else val[0][0]
+                    except Exception as e:
+                        title_value = "Unable to get the version. Please check the logs."
+
                     details = {
                         "statKey": f"SOS Version Health Summary|{k}",
                         "timestamps": [int(timestamp * 1000)],
-                        "values": [val[0]]
+                        "values": [title_value]
                     }
                 else:
                     details = {
                         "statKey": f"SOS Version Health Summary|{k}",
                         "timestamps": [int(timestamp * 1000)],
                         "values": [val]
                     }
-                
+
                 metrics_payload["stat-content"].append(details)
-                
+
                 if k == 'alert':
                     details = {
                         "statKey": f"SOS Version Health Summary|alert_code",
                         "timestamps": [int(timestamp * 1000)],
                         "data": [self.codes[val.lower()]]
                     }
                     metrics_payload["stat-content"].append(details)
@@ -1703,15 +1710,15 @@
 
             self.logger.info(resource_id)
             self.logger.info(metrics_payload_json)
             self.push_data_to_vrops(category, resource_id, hostname, metrics_payload_json)
             update_count = update_count + 1
 
         self.logger.info(f'Total object update requests = {update_count}')
-    
+
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument("-e", "--env-json", default='env.json',
                         help="path of env.json file. Default is in same directory as this file")
     parser.add_argument('-p', '--push-data', dest='push_data', action='store_true',
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/FolderUtility.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/FolderUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/LogUtility.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/LogUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/PSUtility.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/PSUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/main/utils/SosRest.py` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/main/utils/SosRest.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-Metadata-Version: 2.1
-Name: vmware-cloud-foundation-health-monitoring
-Version: 2.1.0.1004
-Summary: Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
-Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
-Author: Broadcom
-Author-email: bhumitra.nagar@broadcom.com, olga.efremov@broadcom.com
-License: BSD-2-Clause
-Project-URL: Issues, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
-Project-URL: Source, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 # Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations
 
 ![PyPI](https://img.shields.io/pypi/v/vmware-cloud-foundation-health-monitoring?logo=python&logoColor=yellow&label=PyPI&labelColor=Grey&link=https%3A%2F%2Fpypi.org%2Fproject%2Fvmware-cloud-foundation-health-monitoring%2F)
 &nbsp;&nbsp;
 [![Downloads](https://static.pepy.tech/personalized-badge/vmware-cloud-foundation-health-monitoring?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=DOWNLOADS)](https://pepy.tech/project/vmware-cloud-foundation-health-monitoring) &nbsp;&nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/vmware-cloud-foundation-health-monitoring?period=month&units=international_system&left_color=grey&right_color=green&left_text=DOWNLOADS/WEEK)](https://pepy.tech/project/vmware-cloud-foundation-health-monitoring) &nbsp;&nbsp; [<img src="https://img.shields.io/badge/CHANGELOG-READ-blue?&logo=github&logoColor=white" alt="CHANGELOG" >][changelog]
 
-
 ## Table of Contents
 
-- [Health Reporting and Monitoring for VMware Cloud Foundation](#health-reporting-and-monitoring-vmware-cloud-foundation)
+- [Python Module for VMware Cloud Foundation Health Monitoring in VMware Aria Operations](#python-module-for-vmware-cloud-foundation-health-monitoring-in-vmware-aria-operations)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
   - [Requirements](#requirements)
+    - [Platforms](#platforms)
+    - [Operating Systems](#operating-systems)
+    - [Python Version](#python-version)
+    - [Python Libraries](#python-libraries)
+    - [PowerShell Editions and Versions](#powershell-editions-and-versions)
+    - [PowerShell Modules](#powershell-modules)
   - [Implementation](#implementation)
   - [Install the Python Module in a Disconnected Environment](#install-the-python-module-in-a-disconnected-environment)
+    - [For Photon OS](#for-photon-os)
+    - [For Windows Server](#for-windows-server)
   - [Updating the Python Module to the Latest Version](#updating-the-python-module-to-the-latest-version)
+    - [For Photon OS](#for-photon-os-1)
+    - [For Windows Server](#for-windows-server-1)
   - [VMware Aria Operations Dashboards Preview](#vmware-aria-operations-dashboards-preview)
   - [Known Issues](#known-issues)
   - [Support](#support)
+  - [License](#license)
 
 ## Introduction
 
 This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native VMware Aria Operations dashboards and dashboards that are enabled using the respective management packs.
 
 ## Requirements
 
@@ -59,260 +51,314 @@
 
 Follow the [Python Beginners Guide](https://wiki.python.org/moin/BeginnersGuide/Download) to download and install Python.
 
 ### Python Libraries
 
 Install required Python libraries by running the following commands on the host virtual machine:
 
-  ```python
-  pip install requests
-  pip install setuptools
-  pip install paramiko
-  pip install maskpass==0.3.1
-  ```
+```python
+pip install requests
+pip install setuptools
+pip install paramiko
+pip install maskpass==0.3.1
+```
 
 ### PowerShell Editions and Versions
 
-- Microsoft Windows PowerShell 5.1
 - PowerShell Core 7.2.0 or later
 
 ### PowerShell Modules
 
 - [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) - latest version
 
 ## Implementation
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
 ## Install the Python Module in a Disconnected Environment
-For environments disconnected from the Internet (e.g., dark-site, air-gapped), you can save the Health Reporting and Monitoring Python module and its dependencies from the PyPI using the below instructions. 
 
-### For Photon OS - 
+For disconnected environments (_e.g._, dark-site, air-gapped), you can save the Health Reporting and Monitoring Python module and its dependencies from the PyPI using the below instructions.
+
+### For Photon OS
 
 - On the target system, create a directory to save the Python modules
-```
+
+  ```console
   mkdir -p /opt/vmware/hrm-modules
-```
+  ```
 
-- From a system with an Internet connection, make a modules directory and create a new file `requirements.txt` inside it. 
-```
+- From a system with an Internet connection, make a modules directory and create a new file `requirements.txt` inside it.
+
+  ```console
   mkdir -p /home/hrm-modules/
   cd /home/hrm-modules/
   vi requirements.txt
-```
-- Add below content to the `requirements.txt` file and save it. 
-```
-requests
-setuptools
-paramiko
-maskpass==0.3.1
-```
+  ```
+
+- Add below content to the `requirements.txt` file and save it.
+
+  ```console
+  requests
+  setuptools
+  paramiko
+  maskpass==0.3.1
+  ```
 
 - Create another file `module.txt` in the same location.
-```
+
+  ```console
   vi module.txt
-```
+  ```
   
-- Add below content to the `module.txt` file and save it. 
-```
-vmware-cloud-foundation-health-monitoring
-```
+- Add below content to the `module.txt` file and save it.
+
+  ```console
+  vmware-cloud-foundation-health-monitoring
+  ```
   
 - From a system with an Internet connection, save the module and its dependencies from PyPI by running the following commands in the terminal:
 
-```
+  ```console
   pip download -r module.txt
   pip download -r requirements.txt
-```
+  ```
 
 - From the system with an Internet connection, copy the module and its dependencies to a target system by running the following commands in the terminal:
-```
+
+  ```console
   scp -r /home/vcf/hrm-modules/* username@remote_host:/opt/vmware/hrm-modules/
-```
+  ```
   
 - On the target system, install the module and its dependencies by running the following commands in the terminal:
-```
+
+  ```console
   cd /opt/vmware/hrm-modules
   pip install -r requirements.txt --no-index --find-links .
   pip install -r module.txt --no-index --find-links . -t /opt/vmware/hrm-<sddc_manager_vm_name>
-```
+  ```
 
-### For Windows Server -
+### For Windows Server
 
 - From a system with an Internet connection, make a modules folder `F:\hrm-modules`.
+- Create a new file `requirements.txt` inside the modules folder.
+- Add the below content to the `requirements.txt` file and save it.
 
-- Create a new file `requirements.txt` inside the modules folder. 
+  ```console
+  requests
+  setuptools
+  paramiko
+  maskpass==0.3.1
+  ```
 
-- Add the below content to the `requirements.txt` file and save it. 
-```
-requests
-setuptools
-paramiko
-maskpass==0.3.1
-```
-- In the modules folder `f:\hrm-modules`, create a new file `module.txt` 
-  
-- Add below content to `module.txt` file and save it. 
-```
-vmware-cloud-foundation-health-monitoring
-```
+- In the modules folder `f:\hrm-modules`, create a new file `module.txt`
+- Add below content to `module.txt` file and save it.
+
+  ```console
+  vmware-cloud-foundation-health-monitoring
+  ```
 
 - From a system with an Internet connection, save the module and its dependencies from PyPI by running the following commands from cmdline:
 
-```
+  ```console
   cd f:\hrm-modules
   pip download -r module.txt 
   pip download -r requirements.txt
-```
+  ```
 
 - From the system with the Internet connection, copy the module and its dependencies to a target system by running the following commands in the PowerShell console:
 
-```
+  ```powershell
   Copy-Item -Path F:\hrm-modules\* -Destination '\\<destination_host>\C$\vmware\hrm-modules
-```
+  ```
 
 - On the target system, install the module and its dependencies by running the following commands in the terminal:
-```
+
+  ```console
   cd c:\vmware\hrm-modules
   pip install -r requirements.txt --no-index --find-links .
   pip install -r module.txt --no-index --find-links . -t c:\vmware\hrm-<sddc_manager_vm_name>
-```
-
+  ```
 
 **Once the Python modules are installed, continue to follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)**
 
 ## Updating the Python Module to the Latest Version
 
-### For Photon OS - 
+### For Photon OS
 
 - Log in to the host virtual machine at `<host_virtual_machine_fqdn>:22` as the `root` user by using a Secure Shell (SSH) client.
 
 - Update the Python Module for Health Reporting and Monitoring in VMware Aria Operations.
-```
+
+  ```console
   pip install vmware-cloud-foundation-health-monitoring --target=/opt/vmware/hrm-<sddc_manager_vm_name> --upgrade
-```  
+  ```  
+
 - Provide execute permissions to the files in the `hrm-<sddc_manager_vm_name>` directory.
-```
+
+  ```console
   chmod -R 755 /opt/vmware/hrm-<sddc_manager_vm_name>
-```  
+  ```  
+
 - Switch to the `hrm-<sddc_manager_vm_name>/main` directory.
-```
+
+  ```console
   cd /opt/vmware/hrm-<sddc_manager_vm_name>/main
-```
+  ```
+
 - Edit the `env.json` file and configure the values according to your VMware Cloud Foundation Planning and Preparation Workbook.
-```
+
+  ```console
   vi env.json
-```
+  ```
+
 - Encrypt the service account passwords.
-```
+
+  ```console
   python encrypt-passwords.py
-```
+  ```
+
 - Enter the password for the VMware Aria Operations service account.
 - Enter the password for the SDDC Manager service account.
 - Enter the password for the SDDC Manager appliance local user.
 - Repeat this procedure for each VMware Cloud Foundation instance.
 
-
-### For Windows Server - 
+### For Windows Server
 
 - Log in to the host virtual machine at `<host_virtual_machine_fqdn>` as the `Administrator` user by using a Remote Desktop Connection (RDC) client and open a PowerShell console.
 - Start Windows Command Prompt.
 - Update the Python Module for Health Reporting and Monitoring in VMware Aria Operations.
-```
+
+  ```console
   pip install vmware-cloud-foundation-health-monitoring --target=C:\vmware\hrm-<sddc_manager_vm_name>\ --upgrade
-```
- 
+  ```
+
 - Change to the `hrm-<sddc_manager_vm_name>\main` folder.
-```
+
+  ```console
   cd c:\vmware\hrm-<sddc_manager_vm_name>\main
-```
+  ```
+
 - Edit the `env.json` file and configure the values according to your VMware Cloud Foundation Planning and Preparation Workbook.
-```
+
+  ```console
   notepad env.json
-```
+  ```
+
 - Encrypt the service account passwords.
-```
+
+  ```console
   python encrypt-passwords.py
-```
+  ```
+
 - Enter the password for the VMware Aria Operations service account.
 - Enter the password for the SDDC Manager service account.
 - Enter the password for the SDDC Manager appliance local user.
 - Repeat this procedure for each VMware Cloud Foundation instance.
 
 ## VMware Aria Operations Dashboards Preview
 
 1. VCF Health Rollup
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Rollup3-min.png)
 
 2. VCF Backup Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Backups1-min.png)
 
 3. VCF Certificate Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Certificates2-min.png)
 
 4. VCF Compute Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Compute2-min.png)
 
 5. VCF Connectivity Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Connectivity2-min.png)
 
 6. VCF DNS Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS1-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/DNS2-min.png)
 
 7. VCF Hardware Compatibility
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/hw-compatibility-min2.png)
 
 8. VCF Networking Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Networking4-min.png)
 
 9. VCF NTP Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP-min.png)
+
+   ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/NTP3-min.png)
 
 10. VCF Password Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Password2-min.png)
 
 11. VCF SDDC Manager and vCenter Services Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Services2-min.png)
 
 12. VCF Snapshot Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/Snapshots2-min.png)
 
 13. VCF Storage Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage2-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/connected-roms-min.png)
 
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage1-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/storage2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/connected-roms-min.png)
 
 14. VCF vSAN Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/vSAN2-min.png)
 
 15. VCF Version Health
-![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/version-min.png)
+
+    ![](https://raw.githubusercontent.com/vmware-samples/validated-solutions-for-cloud-foundation/main/hrm/images/version-min.png)
 
 ## Known Issues
 
 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in VMware Aria Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
     Please make sure that your NSX-T account name is configured as mentioned in this issue.
 
-2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the VMware Aria Operations dashboards depend on the name.
+2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.x. The filters on the VMware Aria Operations dashboards depend on the name.
 
     To set the Product Name for the vCenter Server, follow the below steps:
 
     1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
     2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
     3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
     4. In the `Settings` pane select `vApp Options`.
@@ -339,15 +385,15 @@
 
 - A reproducible test case or series of steps.
 - Any modifications you've made relevant to the bug.
 - Anything unusual about your environment or deployment.
 
 ## License
 
-Copyright 2023 Broadcom. All Rights Reserved.
+Copyright 2023-2024 Broadcom. All Rights Reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `vmware-cloud-foundation-health-monitoring-2.1.0.1004/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt` & `vmware-cloud-foundation-health-monitoring-2.1.1.1001/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

