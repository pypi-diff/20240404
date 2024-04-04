# Comparing `tmp/secure-learn-0.2.1.tar.gz` & `tmp/secure-learn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-learn-0.2.1.tar", last modified: Wed Apr  3 16:30:30 2024, max compression
+gzip compressed data, was "secure-learn-0.2.2.tar", last modified: Thu Apr  4 00:18:10 2024, max compression
```

## Comparing `secure-learn-0.2.1.tar` & `secure-learn-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.140937 secure-learn-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 16:30:11.000000 secure-learn-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 16:30:30.140937 secure-learn-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-03 16:30:11.000000 secure-learn-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 16:30:11.000000 secure-learn-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 16:30:30.140937 secure-learn-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-03 16:30:11.000000 secure-learn-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.136937 secure-learn-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.140937 secure-learn-0.2.1/src/SecuPy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/auditing.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/data_privacy_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.140937 secure-learn-0.2.1/src/secure_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:18:10.227004 secure-learn-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 00:17:50.000000 secure-learn-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-04 00:18:10.227004 secure-learn-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-04 00:17:50.000000 secure-learn-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-04 00:17:50.000000 secure-learn-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-04 00:18:10.227004 secure-learn-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-04 00:17:50.000000 secure-learn-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:18:10.223004 secure-learn-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:18:10.227004 secure-learn-0.2.2/src/SecuPy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:17:50.000000 secure-learn-0.2.2/src/SecuPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 00:17:50.000000 secure-learn-0.2.2/src/SecuPy/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-04 00:17:50.000000 secure-learn-0.2.2/src/SecuPy/auditing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-04 00:17:50.000000 secure-learn-0.2.2/src/SecuPy/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-04 00:17:50.000000 secure-learn-0.2.2/src/SecuPy/data_privacy_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 00:17:50.000000 secure-learn-0.2.2/src/SecuPy/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:18:10.227004 secure-learn-0.2.2/src/secure_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-04 00:18:10.000000 secure-learn-0.2.2/src/secure_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 00:18:10.000000 secure-learn-0.2.2/src/secure_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:18:10.000000 secure-learn-0.2.2/src/secure_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 00:18:10.000000 secure-learn-0.2.2/src/secure_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 00:18:10.000000 secure-learn-0.2.2/src/secure_learn.egg-info/top_level.txt
```

### Comparing `secure-learn-0.2.1/LICENSE` & `secure-learn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secure-learn-0.2.1/PKG-INFO` & `secure-learn-0.2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,150 @@
 Metadata-Version: 2.1
 Name: secure-learn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.
 Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
 Author: DeependraVerma
 Author-email: deependra.verma00@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: faker
 Requires-Dist: cryptography
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.3; extra == "testing"
 Requires-Dist: mypy>=0.971; extra == "testing"
 Requires-Dist: flake8>=5.0.4; extra == "testing"
 Requires-Dist: tox>=3.25.1; extra == "testing"
 Requires-Dist: black>=22.8.0; extra == "testing"
 
-# secure-learn: Secure Data Privacy Framework for Python Data Scientists
+secure-learn: Secure Data Privacy Framework for Python Data Scientists
+======================================================================
 
-[![GitHub stars](https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers)
-[![GitHub license](https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE)
+.. image:: https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg
+    :target: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers
 
-secure-learn is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by [Deependra Verma](https://www.linkedin.com/in/deependra-verma-data-science/), secure-learn offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+.. image:: https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg
+    :target: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE
 
-## Introduction
+secure-learn is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by `Deependra Verma <https://www.linkedin.com/in/deependra-verma-data-science/>`__, secure-learn offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+
+Introduction
+------------
 
 secure-learn: Your all-in-one Python package for robust data privacy and security. Encrypt, anonymize, and control access to sensitive data effortlessly.
 
-## Features
+Features
+--------
+
+secure-learn provides the following key methods:
 
-### secure-learn provides the following key methods:
-- `encrypt_data(data)`: Encrypts sensitive data to ensure confidentiality.
-- `decrypt_data(encrypted_data)`: Decrypts encrypted data to its original form.
-- `anonymize_data(data, columns_to_anonymize)`: Anonymizes specific columns in a DataFrame.
-- `add_role(role_name, permissions)`: Adds a new role with associated permissions to the access control system.
-- `check_permission(role_name, permission)`: Checks if a role has the specified permission.
+- ``encrypt_data(data)``: Encrypts sensitive data to ensure confidentiality.
+- ``decrypt_data(encrypted_data)``: Decrypts encrypted data to its original form.
+- ``anonymize_data(data, columns_to_anonymize)``: Anonymizes specific columns in a DataFrame.
+- ``add_role(role_name, permissions)``: Adds a new role with associated permissions to the access control system.
+- ``check_permission(role_name, permission)``: Checks if a role has the specified permission.
 
-## Installation
+Installation
+------------
 
 To install secure-learn, simply run:
 
-```bash
-pip install secure-learn
-```
+.. code-block:: bash
+
+    pip install secure-learn
 
 Alternatively, you can clone the GitHub repository:
 
-```bash
-git clone https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.git
-cd SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
-python setup.py install
-```
+.. code-block:: bash
+
+    git clone https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.git
+    cd SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
+    python setup.py install
 
-## Dependencies
+Dependencies
+------------
 
 secure-learn relies on the following dependencies:
-- `pandas>=1.0.0`
-- `faker>=8.0.0`
-- `cryptography>=3.0`
 
-## Usage
+- ``pandas>=1.0.0``
+- ``faker>=8.0.0``
+- ``cryptography>=3.0``
+
+Usage
+-----
+
+Import the package:
+
+.. code-block:: python
+
+    from PrivacyPy import DataPrivacyFramework
 
+Initialize PrivacyPy with encryption key:
 
-# Import the package
-from PrivacyPy import DataPrivacyFramework
+.. code-block:: python
 
-# Initialize PrivacyPy with encryption key
-encryption_key = "your_encryption_key"
-privacy_framework = DataPrivacyFramework(encryption_key)
+    encryption_key = "your_encryption_key"
+    privacy_framework = DataPrivacyFramework(encryption_key)
 
-# Anonymize sensitive columns (Name, Email)
-anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
+Anonymize sensitive columns (Name, Email):
 
-# Encrypt entire DataFrame
-encrypted_df = privacy_framework.encrypt_data(anonymized_df)
-print("Encrypted DataFrame:")
-print(encrypted_df)
+.. code-block:: python
 
+    anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
 
-## Users Benefit
+Encrypt entire DataFrame:
+
+.. code-block:: python
+
+    encrypted_df = privacy_framework.encrypt_data(anonymized_df)
+    print("Encrypted DataFrame:")
+    print(encrypted_df)
+
+Users Benefit
+-------------
 
 secure-learn empowers data scientists with the following benefits:
+
 - **Data Confidentiality:** Encrypt sensitive data to prevent unauthorized access.
 - **Anonymization:** Anonymize personally identifiable information for privacy protection.
 - **Access Control:** Control data access based on user roles and permissions.
 - **Compliance:** Ensure compliance with data protection regulations (e.g., GDPR, HIPAA).
 
-## Use Cases
+Use Cases
+---------
 
 secure-learn can be used in various data science scenarios, including:
+
 - Healthcare data analysis
 - Financial data processing
 - User authentication systems
 - Research collaborations with external parties
 
-
-## Invitation for Contribution
+Invitation for Contribution
+---------------------------
 
 Contributions to secure-learn are welcome! To contribute, follow these steps:
+
 1. Fork the repository on GitHub.
 2. Clone the forked repository to your local machine.
 3. Create a new branch for your changes.
 4. Make your modifications and improvements.
 5. Test your changes to ensure they work as expected.
 6. Commit your changes and push them to your forked repository.
 7. Submit a pull request to the original repository.
 
-We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
+We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our `Contributing Guidelines <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki>`__ to get started.
+
+License
+-------
 
-## License
+secure-learn is licensed under the `MIT License <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE>`__. See the `LICENSE <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE>`__ file for details.
 
-secure-learn is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
+About the Author
+----------------
 
-## About the Author
-```
-[Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
-```
+`Email <mailto:deependra.verma00@gmail.com>`__ | `LinkedIn <https://www.linkedin.com/in/deependra-verma-data-science/>`__ | `GitHub <https://github.com/DeependraVerma>`__ | `Portfolio <https://deependradatascience-productportfolio.netlify.app/>`__
```

### Comparing `secure-learn-0.2.1/README.md` & `secure-learn-0.2.2/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,127 @@
-# secure-learn: Secure Data Privacy Framework for Python Data Scientists
+secure-learn: Secure Data Privacy Framework for Python Data Scientists
+======================================================================
 
-[![GitHub stars](https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers)
-[![GitHub license](https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE)
+.. image:: https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg
+    :target: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers
 
-secure-learn is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by [Deependra Verma](https://www.linkedin.com/in/deependra-verma-data-science/), secure-learn offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+.. image:: https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg
+    :target: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE
 
-## Introduction
+secure-learn is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by `Deependra Verma <https://www.linkedin.com/in/deependra-verma-data-science/>`__, secure-learn offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+
+Introduction
+------------
 
 secure-learn: Your all-in-one Python package for robust data privacy and security. Encrypt, anonymize, and control access to sensitive data effortlessly.
 
-## Features
+Features
+--------
+
+secure-learn provides the following key methods:
 
-### secure-learn provides the following key methods:
-- `encrypt_data(data)`: Encrypts sensitive data to ensure confidentiality.
-- `decrypt_data(encrypted_data)`: Decrypts encrypted data to its original form.
-- `anonymize_data(data, columns_to_anonymize)`: Anonymizes specific columns in a DataFrame.
-- `add_role(role_name, permissions)`: Adds a new role with associated permissions to the access control system.
-- `check_permission(role_name, permission)`: Checks if a role has the specified permission.
+- ``encrypt_data(data)``: Encrypts sensitive data to ensure confidentiality.
+- ``decrypt_data(encrypted_data)``: Decrypts encrypted data to its original form.
+- ``anonymize_data(data, columns_to_anonymize)``: Anonymizes specific columns in a DataFrame.
+- ``add_role(role_name, permissions)``: Adds a new role with associated permissions to the access control system.
+- ``check_permission(role_name, permission)``: Checks if a role has the specified permission.
 
-## Installation
+Installation
+------------
 
 To install secure-learn, simply run:
 
-```bash
-pip install secure-learn
-```
+.. code-block:: bash
+
+    pip install secure-learn
 
 Alternatively, you can clone the GitHub repository:
 
-```bash
-git clone https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.git
-cd SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
-python setup.py install
-```
+.. code-block:: bash
+
+    git clone https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.git
+    cd SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
+    python setup.py install
 
-## Dependencies
+Dependencies
+------------
 
 secure-learn relies on the following dependencies:
-- `pandas>=1.0.0`
-- `faker>=8.0.0`
-- `cryptography>=3.0`
 
-## Usage
+- ``pandas>=1.0.0``
+- ``faker>=8.0.0``
+- ``cryptography>=3.0``
+
+Usage
+-----
+
+Import the package:
+
+.. code-block:: python
+
+    from PrivacyPy import DataPrivacyFramework
 
+Initialize PrivacyPy with encryption key:
 
-# Import the package
-from PrivacyPy import DataPrivacyFramework
+.. code-block:: python
 
-# Initialize PrivacyPy with encryption key
-encryption_key = "your_encryption_key"
-privacy_framework = DataPrivacyFramework(encryption_key)
+    encryption_key = "your_encryption_key"
+    privacy_framework = DataPrivacyFramework(encryption_key)
 
-# Anonymize sensitive columns (Name, Email)
-anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
+Anonymize sensitive columns (Name, Email):
 
-# Encrypt entire DataFrame
-encrypted_df = privacy_framework.encrypt_data(anonymized_df)
-print("Encrypted DataFrame:")
-print(encrypted_df)
+.. code-block:: python
 
+    anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
 
-## Users Benefit
+Encrypt entire DataFrame:
+
+.. code-block:: python
+
+    encrypted_df = privacy_framework.encrypt_data(anonymized_df)
+    print("Encrypted DataFrame:")
+    print(encrypted_df)
+
+Users Benefit
+-------------
 
 secure-learn empowers data scientists with the following benefits:
+
 - **Data Confidentiality:** Encrypt sensitive data to prevent unauthorized access.
 - **Anonymization:** Anonymize personally identifiable information for privacy protection.
 - **Access Control:** Control data access based on user roles and permissions.
 - **Compliance:** Ensure compliance with data protection regulations (e.g., GDPR, HIPAA).
 
-## Use Cases
+Use Cases
+---------
 
 secure-learn can be used in various data science scenarios, including:
+
 - Healthcare data analysis
 - Financial data processing
 - User authentication systems
 - Research collaborations with external parties
 
-
-## Invitation for Contribution
+Invitation for Contribution
+---------------------------
 
 Contributions to secure-learn are welcome! To contribute, follow these steps:
+
 1. Fork the repository on GitHub.
 2. Clone the forked repository to your local machine.
 3. Create a new branch for your changes.
 4. Make your modifications and improvements.
 5. Test your changes to ensure they work as expected.
 6. Commit your changes and push them to your forked repository.
 7. Submit a pull request to the original repository.
 
-We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
+We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our `Contributing Guidelines <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki>`__ to get started.
+
+License
+-------
 
-## License
+secure-learn is licensed under the `MIT License <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE>`__. See the `LICENSE <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE>`__ file for details.
 
-secure-learn is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
+About the Author
+----------------
 
-## About the Author
-```
-[Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
-```
+`Email <mailto:deependra.verma00@gmail.com>`__ | `LinkedIn <https://www.linkedin.com/in/deependra-verma-data-science/>`__ | `GitHub <https://github.com/DeependraVerma>`__ | `Portfolio <https://deependradatascience-productportfolio.netlify.app/>`__
```

### Comparing `secure-learn-0.2.1/setup.cfg` & `secure-learn-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `secure-learn-0.2.1/setup.py` & `secure-learn-0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 from typing import List
 
-with open('README.md', 'r', encoding='utf-8') as f:
+with open('README.rst', 'r', encoding='utf-8') as f:
     long_description = f.read()     
 
 HYPEN_E_DOT = "-e ."
 def get_requirements(file_path:str)-> List[str]:
     requirements = []
     with open(file_path) as file_obj:
         requirements = file_obj.readlines()
         requirements = [req.replace("\n","") for req in requirements]
 
         if HYPEN_E_DOT in requirements:
             requirements.remove(HYPEN_E_DOT)
     return requirements
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 REPO_NAME = "SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists"
 PKG_NAME= "secure-learn"
 AUTHOR_USER_NAME = "DeependraVerma"
 AUTHOR_EMAIL = "deependra.verma00@gmail.com"
 
 setup(
     name=PKG_NAME,
@@ -31,9 +31,14 @@
     long_description_content="text/x-rst",
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    install_requires = ["pandas", "faker","cryptography"]
+    install_requires = ["pandas", "faker","cryptography"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
     )
```

### Comparing `secure-learn-0.2.1/src/SecuPy/data_privacy_framework.py` & `secure-learn-0.2.2/src/SecuPy/data_privacy_framework.py`

 * *Files identical despite different names*

### Comparing `secure-learn-0.2.1/src/secure_learn.egg-info/PKG-INFO` & `secure-learn-0.2.2/src/secure_learn.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,150 @@
 Metadata-Version: 2.1
 Name: secure-learn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.
 Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
 Author: DeependraVerma
 Author-email: deependra.verma00@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: faker
 Requires-Dist: cryptography
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.3; extra == "testing"
 Requires-Dist: mypy>=0.971; extra == "testing"
 Requires-Dist: flake8>=5.0.4; extra == "testing"
 Requires-Dist: tox>=3.25.1; extra == "testing"
 Requires-Dist: black>=22.8.0; extra == "testing"
 
-# secure-learn: Secure Data Privacy Framework for Python Data Scientists
+secure-learn: Secure Data Privacy Framework for Python Data Scientists
+======================================================================
 
-[![GitHub stars](https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers)
-[![GitHub license](https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE)
+.. image:: https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg
+    :target: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers
 
-secure-learn is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by [Deependra Verma](https://www.linkedin.com/in/deependra-verma-data-science/), secure-learn offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+.. image:: https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg
+    :target: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE
 
-## Introduction
+secure-learn is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by `Deependra Verma <https://www.linkedin.com/in/deependra-verma-data-science/>`__, secure-learn offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+
+Introduction
+------------
 
 secure-learn: Your all-in-one Python package for robust data privacy and security. Encrypt, anonymize, and control access to sensitive data effortlessly.
 
-## Features
+Features
+--------
+
+secure-learn provides the following key methods:
 
-### secure-learn provides the following key methods:
-- `encrypt_data(data)`: Encrypts sensitive data to ensure confidentiality.
-- `decrypt_data(encrypted_data)`: Decrypts encrypted data to its original form.
-- `anonymize_data(data, columns_to_anonymize)`: Anonymizes specific columns in a DataFrame.
-- `add_role(role_name, permissions)`: Adds a new role with associated permissions to the access control system.
-- `check_permission(role_name, permission)`: Checks if a role has the specified permission.
+- ``encrypt_data(data)``: Encrypts sensitive data to ensure confidentiality.
+- ``decrypt_data(encrypted_data)``: Decrypts encrypted data to its original form.
+- ``anonymize_data(data, columns_to_anonymize)``: Anonymizes specific columns in a DataFrame.
+- ``add_role(role_name, permissions)``: Adds a new role with associated permissions to the access control system.
+- ``check_permission(role_name, permission)``: Checks if a role has the specified permission.
 
-## Installation
+Installation
+------------
 
 To install secure-learn, simply run:
 
-```bash
-pip install secure-learn
-```
+.. code-block:: bash
+
+    pip install secure-learn
 
 Alternatively, you can clone the GitHub repository:
 
-```bash
-git clone https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.git
-cd SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
-python setup.py install
-```
+.. code-block:: bash
+
+    git clone https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.git
+    cd SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
+    python setup.py install
 
-## Dependencies
+Dependencies
+------------
 
 secure-learn relies on the following dependencies:
-- `pandas>=1.0.0`
-- `faker>=8.0.0`
-- `cryptography>=3.0`
 
-## Usage
+- ``pandas>=1.0.0``
+- ``faker>=8.0.0``
+- ``cryptography>=3.0``
+
+Usage
+-----
+
+Import the package:
+
+.. code-block:: python
+
+    from PrivacyPy import DataPrivacyFramework
 
+Initialize PrivacyPy with encryption key:
 
-# Import the package
-from PrivacyPy import DataPrivacyFramework
+.. code-block:: python
 
-# Initialize PrivacyPy with encryption key
-encryption_key = "your_encryption_key"
-privacy_framework = DataPrivacyFramework(encryption_key)
+    encryption_key = "your_encryption_key"
+    privacy_framework = DataPrivacyFramework(encryption_key)
 
-# Anonymize sensitive columns (Name, Email)
-anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
+Anonymize sensitive columns (Name, Email):
 
-# Encrypt entire DataFrame
-encrypted_df = privacy_framework.encrypt_data(anonymized_df)
-print("Encrypted DataFrame:")
-print(encrypted_df)
+.. code-block:: python
 
+    anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
 
-## Users Benefit
+Encrypt entire DataFrame:
+
+.. code-block:: python
+
+    encrypted_df = privacy_framework.encrypt_data(anonymized_df)
+    print("Encrypted DataFrame:")
+    print(encrypted_df)
+
+Users Benefit
+-------------
 
 secure-learn empowers data scientists with the following benefits:
+
 - **Data Confidentiality:** Encrypt sensitive data to prevent unauthorized access.
 - **Anonymization:** Anonymize personally identifiable information for privacy protection.
 - **Access Control:** Control data access based on user roles and permissions.
 - **Compliance:** Ensure compliance with data protection regulations (e.g., GDPR, HIPAA).
 
-## Use Cases
+Use Cases
+---------
 
 secure-learn can be used in various data science scenarios, including:
+
 - Healthcare data analysis
 - Financial data processing
 - User authentication systems
 - Research collaborations with external parties
 
-
-## Invitation for Contribution
+Invitation for Contribution
+---------------------------
 
 Contributions to secure-learn are welcome! To contribute, follow these steps:
+
 1. Fork the repository on GitHub.
 2. Clone the forked repository to your local machine.
 3. Create a new branch for your changes.
 4. Make your modifications and improvements.
 5. Test your changes to ensure they work as expected.
 6. Commit your changes and push them to your forked repository.
 7. Submit a pull request to the original repository.
 
-We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
+We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our `Contributing Guidelines <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki>`__ to get started.
+
+License
+-------
 
-## License
+secure-learn is licensed under the `MIT License <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE>`__. See the `LICENSE <https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE>`__ file for details.
 
-secure-learn is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
+About the Author
+----------------
 
-## About the Author
-```
-[Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
-```
+`Email <mailto:deependra.verma00@gmail.com>`__ | `LinkedIn <https://www.linkedin.com/in/deependra-verma-data-science/>`__ | `GitHub <https://github.com/DeependraVerma>`__ | `Portfolio <https://deependradatascience-productportfolio.netlify.app/>`__
```

