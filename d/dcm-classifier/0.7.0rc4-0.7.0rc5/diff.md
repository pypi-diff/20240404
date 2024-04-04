# Comparing `tmp/dcm_classifier-0.7.0rc4.tar.gz` & `tmp/dcm_classifier-0.7.0rc5.tar.gz`

## Comparing `dcm_classifier-0.7.0rc4.tar` & `dcm_classifier-0.7.0rc5.tar`

### file list

```diff
@@ -1,53 +1,83 @@
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/README.md
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/pyproject.toml
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/Activate.ps1
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/activate
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/activate.csh
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/activate.fish
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/coloredlogs
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/f2py
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmanon
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmconv
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmdiff
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmdump
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmgendir
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmimg
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcminfo
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmpap3
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmraw
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmscanner
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmscu
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmtar
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmxml
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/humanfriendly
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/isympy
+-rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/onnxruntime_test
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/pip
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/pip3
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/pydicom
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/python3 -> /usr/bin/python3
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/tabulate
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/README.md
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/PKG-INFO
```

### Comparing `dcm_classifier-0.7.0rc4/.pre-commit-config.yaml` & `dcm_classifier-0.7.0rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.7.0rc5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/.github/workflows/push_to_main.yml` & `dcm_classifier-0.7.0rc5/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/models/rf_classifier.onnx` & `dcm_classifier-0.7.0rc5/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.7.0rc5/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/classify_study.py` & `dcm_classifier-0.7.0rc5/scripts/classify_study.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         "--session_directory",
         required=True,
         help="Path to the patient session directory with dicom data",
     )
     parser.add_argument(
         "-m",
         "--model",
-        required=True,
+        required=False,
+        default=None,
         help="Path to the model used for image type inference",
     )
     parser.add_argument(
         "-n",
         "--nifti_dir",
         required=False,
         default=None,
```

### Comparing `dcm_classifier-0.7.0rc4/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.7.0rc5/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/create_training_sheet.py` & `dcm_classifier-0.7.0rc5/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.7.0rc5/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/modality_classifier_training.py` & `dcm_classifier-0.7.0rc5/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.7.0rc5/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/orientation_model_training.py` & `dcm_classifier-0.7.0rc5/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.7.0rc5/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/running_classifier.ipynb` & `dcm_classifier-0.7.0rc5/scripts/running_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/todo_list` & `dcm_classifier-0.7.0rc5/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/training_config.py` & `dcm_classifier-0.7.0rc5/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/scripts/utilities.py` & `dcm_classifier-0.7.0rc5/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/image_type_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 )
 from pathlib import Path
 import warnings
 
 import numpy as np
 import pandas as pd
 
-from typing import Any
+from typing import Any, Optional
 
 
 imagetype_to_integer_mapping = {
     "t1w": 0,
     "gret2star": 1,
     "t2w": 2,
     "flair": 3,
@@ -39,14 +39,17 @@
     "tracew": 5,
     "adc": 6,
     "fa": 7,
     "eadc": 8,
     "dwig": 9,
 }
 
+current_file_path = Path(__file__).absolute()
+dcm_classifier_path = current_file_path.parent
+
 
 class ImageTypeClassifierBase:
     """
     Inference class for image type classification. The base implementation is for our standard model. This class
     can be customized by users to implement their own models for targeted for specific datasets.
 
     Attributes:
@@ -75,15 +78,17 @@
         infer_modality(self, feature_dict: dict = None) -> (str, pd.DataFrame):
 
         run_inference(self) -> None:
     """
 
     def __init__(
         self,
-        classification_model_filename: str | Path,
+        classification_model_filename: Optional[(str | Path)] = dcm_classifier_path
+        / "models"
+        / "ova_rf_classifier.onnx",
         classification_feature_list: list[str] = inference_features,
         image_type_map: dict[str, int] = imagetype_to_integer_mapping,
         min_probability_threshold: float = 0.4,
     ):
         """
         Initialize the ImageTypeClassifierBase.
```

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.7.0rc5/src/dcm_classifier/utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.7.0rc5/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/conftest.py` & `dcm_classifier-0.7.0rc5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.7.0rc5/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/testing_data/mock_data.txt` & `dcm_classifier-0.7.0rc5/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/testing_data/test.py` & `dcm_classifier-0.7.0rc5/tests/testing_data/test.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.7.0rc5/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.7.0rc5/tests/unit_testing/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/.gitignore` & `dcm_classifier-0.7.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/LICENSE` & `dcm_classifier-0.7.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/README.md` & `dcm_classifier-0.7.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc4/pyproject.toml` & `dcm_classifier-0.7.0rc5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.7.0.rc4'
+version = '0.7.0.rc5'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `dcm_classifier-0.7.0rc4/PKG-INFO` & `dcm_classifier-0.7.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.7.0rc4
+Version: 0.7.0rc5
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: itk-core>=5.3.0
```

